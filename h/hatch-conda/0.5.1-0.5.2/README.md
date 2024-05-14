# Comparing `tmp/hatch_conda-0.5.1.tar.gz` & `tmp/hatch_conda-0.5.2.tar.gz`

## Comparing `hatch_conda-0.5.1.tar` & `hatch_conda-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/.gitattributes
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/HISTORY.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/hatch_conda/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/hatch_conda/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/hatch_conda/hooks.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/hatch_conda/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/tests/test_config.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/tests/utils.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/hatch.toml
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 hatch_conda-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/.gitattributes
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/HISTORY.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/hatch_conda/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/hatch_conda/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/hatch_conda/hooks.py
+-rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/hatch_conda/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/tests/test_config.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/tests/utils.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/hatch.toml
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 hatch_conda-0.5.2/PKG-INFO
```

### Comparing `hatch_conda-0.5.1/HISTORY.md` & `hatch_conda-0.5.2/HISTORY.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 -----
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.5.2] - 14/05/2024
+
+### Fixed
+- dependencies_in_sync uses hatchling by import rather than cli.
+
 ## [0.5.1] - 01/02/2024
 
 ### Fixed
 - Only use --no-capture-output for conda commands.
 
 ## [0.5.0] - 15/01/2024
```

### Comparing `hatch_conda-0.5.1/.github/workflows/build.yml` & `hatch_conda-0.5.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/.github/workflows/test.yml` & `hatch_conda-0.5.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/hatch_conda/plugin.py` & `hatch_conda-0.5.2/hatch_conda/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from contextlib import contextmanager
 from pathlib import Path
 from types import FrameType
 from typing import Callable
 
 import pexpect
 from hatch.env.plugin.interface import EnvironmentInterface
+from hatch.utils.env import PythonInfo
 
 
 class ShellManager:
     def __init__(self, environment: EnvironmentInterface):
         self.environment = environment
 
     def enter_bash(self, path: str, args: list[str], cmdl: str) -> None:
@@ -180,15 +181,15 @@
         env_path = self._get_conda_env_path(self.conda_env_name)
         if env_path is not None:
             return Path(self._get_conda_env_path(self.conda_env_name)).exists()
         return False
 
     def construct_conda_run_command(self, command):
         head = [self.config_command, "run"]
-        if self.config_command in ["conda" , "mamba"]:
+        if self.config_command in ["conda", "mamba"]:
             head.append("--no-capture-output")
 
         if self.config_prefix is not None:
             head += ["--prefix", self.config_prefix]
         else:
             head += ["-n", self.conda_env_name]
 
@@ -209,20 +210,22 @@
                 self.construct_pip_install_command(["--editable", self.apply_features(self.project_path)])
             )
 
     def dependencies_in_sync(self):
         if not self.dependencies:
             return True
         self.apply_env_vars()
+
+        from hatchling.dep.core import dependencies_in_sync
+
+        python_info = PythonInfo(self.platform)
         with self:
-            process = self.platform.run_command(
-                " ".join(["hatchling", "dep", "synced", "-p", "python", *self.dependencies]),
-                capture_output=True,
+            return dependencies_in_sync(
+                self.dependencies_complex, sys_path=python_info.sys_path, environment=python_info.environment
             )
-            return not process.returncode
 
     def sync_dependencies(self):
         self.apply_env_vars()
         with self:
             self.platform.check_command(self.construct_pip_install_command(self.dependencies))
 
     @contextmanager
```

### Comparing `hatch_conda-0.5.1/tests/conftest.py` & `hatch_conda-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/tests/test_config.py` & `hatch_conda-0.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/tests/utils.py` & `hatch_conda-0.5.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/LICENSE.txt` & `hatch_conda-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/README.md` & `hatch_conda-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/hatch.toml` & `hatch_conda-0.5.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.5.1/pyproject.toml` & `hatch_conda-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Framework :: Hatch",
 ]
 dependencies = [
   "hatch>=1.2.0",
+  "hatchling>=1.0.0",
   "pexpect~=4.8",
 ]
 dynamic = ["version"]
 
 [project.urls]
 History = "https://github.com/OldGrumpyViking/hatch-conda/blob/master/HISTORY.md"
 Issues = "https://github.com/OldGrumpyViking/hatch-conda/issues"
@@ -83,8 +84,8 @@
 skip_empty = true
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:", "raise NotImplementedError"]
 
 [tool.flake8]
 exclude = [".direnv", ]
 select = ["B","C","E","F","W","B001","B003","B006","B007","B301","B305","B306","B902","Q001","Q002","Q003"]
 ignore = ["E203","E722","W503"]
-max-line-length = 120
+max-line-length = 120
```

### Comparing `hatch_conda-0.5.1/PKG-INFO` & `hatch_conda-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hatch-conda
-Version: 0.5.1
+Version: 0.5.2
 Summary: Hatch plugin for conda environments
 Project-URL: History, https://github.com/OldGrumpyViking/hatch-conda/blob/master/HISTORY.md
 Project-URL: Issues, https://github.com/OldGrumpyViking/hatch-conda/issues
 Project-URL: Source, https://github.com/OldGrumpyViking/hatch-conda
 Author-email: OldGrumpyViking <old.grumpy.viking@hotmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: hatch>=1.2.0
+Requires-Dist: hatchling>=1.0.0
 Requires-Dist: pexpect~=4.8
 Description-Content-Type: text/markdown
 
 # hatch-conda
 
 | | |
 | --- | --- |
```

