# Comparing `tmp/envoy.code.check-0.5.8.tar.gz` & `tmp/envoy.code.check-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.code.check-0.5.8.tar", last modified: Sun Sep 10 09:25:38 2023, max compression
+gzip compressed data, was "envoy.code.check-0.5.9.tar", last modified: Mon Apr 29 10:10:42 2024, max compression
```

## Comparing `envoy.code.check-0.5.8.tar` & `envoy.code.check-0.5.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/envoy/code/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/envoy/code/check/
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/envoy/code/check/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    15502 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    17054 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/flake8.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/glint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/gofmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/runtime_guards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7134 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/shellcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/yamllint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/abstract/yapf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy/code/check/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/envoy.code.check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy.code.check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy.code.check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy.code.check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy.code.check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy.code.check.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy.code.check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/envoy.code.check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-10 09:25:38.386020 envoy.code.check-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-09-10 09:25:38.000000 envoy.code.check-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:42.720537 envoy.code.check-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-29 10:10:42.720537 envoy.code.check-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:42.716537 envoy.code.check-0.5.9/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:42.716537 envoy.code.check-0.5.9/envoy/code/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:42.720537 envoy.code.check-0.5.9/envoy/code/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:42.720537 envoy.code.check-0.5.9/envoy/code/check/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15502 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17081 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/flake8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/glint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/gofmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/runtime_guards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/shellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/yamllint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/abstract/yapf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy/code/check/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:42.716537 envoy.code.check-0.5.9/envoy.code.check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy.code.check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy.code.check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy.code.check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy.code.check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy.code.check.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy.code.check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/envoy.code.check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:10:42.720537 envoy.code.check-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-29 10:10:42.000000 envoy.code.check-0.5.9/setup.py
```

### Comparing `envoy.code.check-0.5.8/backend_shim.py` & `envoy.code.check-0.5.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/__init__.py` & `envoy.code.check-0.5.9/envoy/code/check/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/__init__.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/base.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/base.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/changelog.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/checker.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/checker.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/extensions.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,16 @@
     def _owners_expected(self, path: str, default: int = 1) -> int:
         return self.ownership_exceptions.get(
             path, {}).get("owners", default)
 
     def _owners_extension_match_line(
             self,
             line: str,
-            matcher: Pattern[str] = None) -> dict[str, dict[str, set]]:
+            matcher: Optional[
+                Pattern[str]] = None) -> dict[str, dict[str, set]]:
         if line.startswith('#'):
             return {}
         m = (matcher or self.codeowners_extensions_re).search(line)
         if m is None:
             return {}
         path = m.group(1).strip().lstrip("/")
         owners = set(
```

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/flake8.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/flake8.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/glint.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/glint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/gofmt.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/gofmt.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/rst.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/rst.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/runtime_guards.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/runtime_guards.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/shellcheck.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/shellcheck.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/yamllint.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/yamllint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 import io
 import pathlib
-import re
 from functools import cached_property, partial
 from typing import (
     AsyncIterator, Dict, Generator, Iterator, List, Optional,
-    Pattern, Set, Tuple)
+    Set, Tuple)
 
 from yamllint import linter  # type:ignore
 from yamllint.config import YamlLintConfig  # type:ignore
 
 import abstracts
 
 from aio.core.dev import debug
@@ -19,20 +18,14 @@
     AwaitableGenerator)
 from aio.run import checker
 
 from envoy.code.check import abstract, typing
 
 
 YAMLLINT_CONFIG = '.yamllint'
-YAMLLINT_MATCH_RE = (
-    r"[\w/\.]*\.yml$",
-    r"[\w/\.]*\.yaml$", )
-YAMLLINT_NOMATCH_RE = (
-    r"[\w/\.]*\.template\.yaml$",
-    r"[\w/\.]*/server_xds\.cds\.with_unknown_field\.*\.yaml$")
 
 
 @abstracts.implementer(directory.IDirectoryContext)
 class YamllintFilesCheck(directory.ADirectoryContext):
 
     def __init__(
             self,
@@ -99,40 +92,24 @@
             root_path: str,
             config: YamlLintConfig,
             *args) -> Tuple["typing.YamllintProblemTuple", ...]:
         return YamllintFilesCheck(root_path, config, *args).run_checks()
 
     @async_property
     async def checker_files(self) -> Set[str]:
-        """Files with a `.yaml` suffix, but that are not excluded."""
-        return set(
-            path
-            for path
-            in await self.directory.files
-            if (self.path_match_re.match(path)
-                and not self.path_match_exclude_re.match(path)))
+        return await self.directory.files
 
     @cached_property
     def config(self) -> YamlLintConfig:
         return YamlLintConfig(file=self.config_path)
 
     @property
     def config_path(self) -> pathlib.Path:
         return self.directory.path.joinpath(YAMLLINT_CONFIG)
 
-    @cached_property
-    def path_match_re(self) -> Pattern[str]:
-        """Regex to match files to check."""
-        return re.compile("|".join(YAMLLINT_MATCH_RE))
-
-    @cached_property
-    def path_match_exclude_re(self) -> Pattern[str]:
-        """Regex to match files not to check."""
-        return re.compile("|".join(YAMLLINT_NOMATCH_RE))
-
     @async_property(cache=True)
     async def problem_files(self) -> "typing.ProblemDict":
         return dict(await AwaitableGenerator(self._problem_files))
 
     @async_property
     async def _problem_files(self) -> AsyncIterator[
             "typing.YamllintProblemTuple"]:
```

### Comparing `envoy.code.check-0.5.8/envoy/code/check/abstract/yapf.py` & `envoy.code.check-0.5.9/envoy/code/check/abstract/yapf.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/checker.py` & `envoy.code.check-0.5.9/envoy/code/check/checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 @abstracts.implementer(interface.IYapfCheck)
 class YapfCheck(abstract.AYapfCheck):
     pass
 
 
 @abstracts.implementer(abstract.AYamllintCheck)
-class YamllintCheck:
+class YamllintCheck(abstract.AYamllintCheck):
     pass
 
 
 @abstracts.implementer(interface.IRSTCheck)
 class BackticksCheck(abstract.ABackticksCheck):
     pass
```

### Comparing `envoy.code.check-0.5.8/envoy/code/check/interface.py` & `envoy.code.check-0.5.9/envoy/code/check/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy/code/check/typing.py` & `envoy.code.check-0.5.9/envoy/code/check/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/envoy.code.check.egg-info/SOURCES.txt` & `envoy.code.check-0.5.9/envoy.code.check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.8/setup.py` & `envoy.code.check-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'entry_points': {
         'console_scripts': [
             'envoy.code.check=envoy.code.check:run',
         ],
     },
     'install_requires': (
         'abstracts>=0.0.12',
-        'aio.core>=0.10.0',
+        'aio.core>=0.10.1',
         'aio.run.checker>=0.5.7',
         'envoy.base.utils>=0.4.7',
         'flake8>=6',
         'packaging>=23.0',
         'yamllint',
         'yapf',
     ),
@@ -42,9 +42,9 @@
     },
     'packages': (
         'envoy.code.check',
         'envoy.code.check.abstract',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/toolshed/tree/main/envoy.code.check',
-    'version': '0.5.8',
+    'version': '0.5.9',
 })
```

