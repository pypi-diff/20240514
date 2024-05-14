# Comparing `tmp/release_gitter-2.2.1.tar.gz` & `tmp/release_gitter-2.3.0.tar.gz`

## Comparing `release_gitter-2.2.1.tar` & `release_gitter-2.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 release_gitter-2.2.1/pseudo_builder.py
--rwxr-xr-x   0        0        0    18601 2020-02-02 00:00:00.000000 release_gitter-2.2.1/release_gitter.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 release_gitter-2.2.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 release_gitter-2.2.1/LICENSE
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 release_gitter-2.2.1/README.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 release_gitter-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 release_gitter-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 release_gitter-2.3.0/pseudo_builder.py
+-rwxr-xr-x   0        0        0    19429 2020-02-02 00:00:00.000000 release_gitter-2.3.0/release_gitter.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 release_gitter-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 release_gitter-2.3.0/LICENSE
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 release_gitter-2.3.0/README.md
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 release_gitter-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 release_gitter-2.3.0/PKG-INFO
```

### Comparing `release_gitter-2.2.1/pseudo_builder.py` & `release_gitter-2.3.0/pseudo_builder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 This builder functions as a pseudo builder that instead downloads and installs a binary file using
 release-gitter based on a pyproject.toml file. It's a total hack...
 """
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
 from shutil import copy
 from shutil import copytree
 from shutil import move
 
 import toml
 from wheel.wheelfile import WheelFile
 
 import release_gitter as rg
 from release_gitter import removeprefix
 
-
 PACKAGE_NAME = "pseudo"
 
 
 @dataclass
 class Config:
     format: str
     git_url: str
```

### Comparing `release_gitter-2.2.1/release_gitter.py` & `release_gitter-2.3.0/release_gitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 from __future__ import annotations
 
 import argparse
 import platform
 from collections.abc import Sequence
 from dataclasses import dataclass
 from io import BytesIO
+from itertools import product
 from mimetypes import guess_type
 from pathlib import Path
 from subprocess import check_call
 from subprocess import check_output
 from tarfile import TarFile
 from tarfile import TarInfo
 from typing import Any
 from urllib.parse import urlparse
 from zipfile import ZipFile
 
 import requests
 
-__version__ = "2.2.1"
+__version__ = "2.3.0"
 
 
 class UnsupportedContentTypeError(ValueError):
     pass
 
 
 class InvalidRemoteError(ValueError):
@@ -43,14 +44,39 @@
     try:
         return s.removesuffix(suf)  # type: ignore
     except AttributeError:
         # Py < 3.9
         return s[: -len(suf)] if s and s.endswith(suf) else s
 
 
+SYSTEM_SYNONYMS: list[list[str]] = [
+    ["Darwin", "darwin", "MacOS", "macos", "macOS"],
+    ["Windows", "windows", "win", "win32", "win64"],
+    ["Linux", "linux"],
+]
+
+ARCH_SYNONYMS: list[list[str]] = [
+    ["arm"],
+    ["x86_64", "amd64", "AMD64"],
+    ["arm64", "aarch64", "armv8b", "armv8l"],
+    ["x86", "i386", "i686"],
+]
+
+
+def get_synonyms(value: str, thesaurus: list[list[str]]) -> list[str]:
+    """Gets synonym list for a given value."""
+    results = [value]
+
+    for l in thesaurus:
+        if value in l:
+            results += l
+
+    return results
+
+
 @dataclass
 class GitRemoteInfo:
     """Extracts information about a repository"""
 
     hostname: str
     owner: str
     repo: str
@@ -241,29 +267,37 @@
             )
         else:
             # This should never happen, but since version isn't used anywhere, we can make it an empty string
             version = ""
 
     system = platform.system()
     if system_mapping:
-        system = system_mapping.get(system, system)
+        systems = [system_mapping.get(system, system)]
+    else:
+        systems = get_synonyms(system, SYSTEM_SYNONYMS)
 
     arch = platform.machine()
     if arch_mapping:
-        arch = arch_mapping.get(arch, arch)
+        archs = [arch_mapping.get(arch, arch)]
+    else:
+        archs = get_synonyms(arch, ARCH_SYNONYMS)
 
     expected_names = {
         format.format(
-            version=normalized_version,
-            system=system,
-            arch=arch,
+            version=version_opt,
+            system=system_opt,
+            arch=arch_opt,
         )
-        for normalized_version in (
-            version.lstrip("v"),
-            "v" + version if not version.startswith("v") else version,
+        for version_opt, system_opt, arch_opt in product(
+            (
+                version.lstrip("v"),
+                "v" + version if not version.startswith("v") else version,
+            ),
+            systems,
+            archs,
         )
     }
 
     for asset in release["assets"]:
         if asset["name"] in expected_names:
             return asset
```

### Comparing `release_gitter-2.2.1/.gitignore` & `release_gitter-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `release_gitter-2.2.1/LICENSE` & `release_gitter-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `release_gitter-2.2.1/README.md` & `release_gitter-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `release_gitter-2.2.1/pyproject.toml` & `release_gitter-2.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -49,16 +49,21 @@
 run = [
     "coverage erase",
     "coverage run --source=release_gitter -m unittest discover . *_test.py",
     "coverage report -m # --fail-under 70",
 ]
 
 [[tool.hatch.envs.test.matrix]]
-python = ["3", "3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = ["pre-commit"]
 
 [tool.hatch.envs.lint.scripts]
 all = "pre-commit run --all-files"
 install-hooks = "pre-commit install --install-hooks"
+
+[tool.isort]
+add_imports = ["from __future__ import annotations"]
+force_single_line = true
+profile = "black"
```

### Comparing `release_gitter-2.2.1/PKG-INFO` & `release_gitter-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: release-gitter
-Version: 2.2.1
+Version: 2.3.0
 Summary: Easily download releases from sites like Github and Gitea
 Project-URL: Homepage, https://git.iamthefij.com/iamthefij/release-gitter
 Author-email: Ian Fijolek <iamthefij@gmail.com>
 Maintainer-email: Ian Fijolek <iamthefij@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

