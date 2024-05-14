# Comparing `tmp/BL_Python.programming-0.1.1.tar.gz` & `tmp/bl_python_programming-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.programming-0.1.1.tar", last modified: Fri Feb 16 20:09:35 2024, max compression
+gzip compressed data, was "bl_python_programming-0.2.0.tar", last modified: Tue May 14 21:46:30 2024, max compression
```

## Comparing `BL_Python.programming-0.1.1.tar` & `bl_python_programming-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.327459 BL_Python.programming-0.1.1/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.327459 BL_Python.programming-0.1.1/BL_Python/programming/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/BL_Python/programming/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/cli/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/BL_Python/programming/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/collections/dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/BL_Python/programming/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/dependency_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/BL_Python/programming/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/patterns/dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/patterns/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/BL_Python/programming/str/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/BL_Python/programming/str/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/BL_Python.programming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-16 20:09:35.000000 BL_Python.programming-0.1.1/BL_Python.programming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 20:09:35.000000 BL_Python.programming-0.1.1/BL_Python.programming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 20:09:35.000000 BL_Python.programming-0.1.1/BL_Python.programming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-16 20:09:35.000000 BL_Python.programming-0.1.1/BL_Python.programming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-16 20:09:35.000000 BL_Python.programming-0.1.1/BL_Python.programming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.327459 BL_Python.programming-0.1.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:09:35.331459 BL_Python.programming-0.1.1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-02-16 20:09:26.000000 BL_Python.programming-0.1.1/test/unit/test_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.234622 bl_python_programming-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.238622 bl_python_programming-0.2.0/BL_Python/programming/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.238622 bl_python_programming-0.2.0/BL_Python/programming/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/cli/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.238622 bl_python_programming-0.2.0/BL_Python/programming/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/collections/dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.238622 bl_python_programming-0.2.0/BL_Python/programming/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/BL_Python/programming/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/patterns/dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/patterns/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/BL_Python/programming/str/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/BL_Python/programming/str/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/BL_Python.programming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-14 21:46:30.000000 bl_python_programming-0.2.0/BL_Python.programming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 21:46:30.000000 bl_python_programming-0.2.0/BL_Python.programming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:46:30.000000 bl_python_programming-0.2.0/BL_Python.programming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 21:46:30.000000 bl_python_programming-0.2.0/BL_Python.programming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 21:46:30.000000 bl_python_programming-0.2.0/BL_Python.programming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.238622 bl_python_programming-0.2.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:46:30.242622 bl_python_programming-0.2.0/test/unit/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/test/unit/patterns/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/test/unit/patterns/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/test/unit/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 21:46:24.000000 bl_python_programming-0.2.0/test/unit/test_dependency_injection.py
```

### Comparing `BL_Python.programming-0.1.1/BL_Python/programming/cli/argparse.py` & `bl_python_programming-0.2.0/BL_Python/programming/cli/argparse.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,63 @@
     Action,
     ArgumentError,
     ArgumentParser,
     ArgumentTypeError,
     FileType,
     Namespace,
 )
+from pathlib import Path
 from typing import Any, Callable, Iterable, Sequence, TypeVar
 
 from typing_extensions import override
 
 _T = TypeVar("_T")
 
 
+class PathExists(Action):
+    """
+    Checks if one or more paths specified are valid paths.
+
+    :param PathExists Action: self
+    :raises ArgumentError: Raised when a value is not a path, or the path does not exist.
+    """
+
+    @override
+    def __call__(
+        self,
+        parser: ArgumentParser,
+        namespace: Namespace,
+        values: str | Path | Sequence[Any] | None,
+        option_string: str | None = None,
+    ) -> None:
+        attr: list[Any] | None
+        if not (attr := getattr(namespace, self.dest, None)):
+            attr = []
+            setattr(namespace, self.dest, attr)
+
+        if values is None:
+            raise ArgumentError(self, "Path cannot be `None`")
+
+        def _check_path(path: str | Path):
+            _path = Path(path)
+            if not _path.exists():
+                raise ArgumentError(self, f"Path does not exists: `{path}`")
+
+        # check all paths first
+        if isinstance(values, str) or isinstance(values, Path):
+            _check_path(values)
+        else:
+            for value in values:
+                _check_path(value)
+
+        # add the values once all paths are checked
+        attr.append(values)
+        setattr(namespace, self.dest, attr)
+
+
 class DisallowDuplicateValues(Action):
     """
     Checks for duplicated values for the argument using this Action.
     If a value is duplicated, an ArgumentError is raised. Otherwise,
     the argument is treated as a "Append" action, and the value is
     added to a list of values for that argument.
```

### Comparing `BL_Python.programming-0.1.1/BL_Python/programming/collections/dict.py` & `bl_python_programming-0.2.0/BL_Python/programming/collections/dict.py`

 * *Files identical despite different names*

### Comparing `BL_Python.programming-0.1.1/BL_Python/programming/config/__init__.py` & `bl_python_programming-0.2.0/BL_Python/programming/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+from pathlib import Path
 from typing import Any, Generic, TypeVar, cast
 
 import toml
 from BL_Python.programming.collections.dict import AnyDict, merge
 
 TConfig = TypeVar("TConfig")
 
@@ -55,15 +56,15 @@
         )
 
         return _new_type
 
 
 def load_config(
     config_type: type[TConfig],
-    toml_file_path: str,
+    toml_file_path: str | Path,
     config_overrides: AnyDict | None = None,
 ) -> TConfig:
     config_dict: dict[str, Any] = toml.load(toml_file_path)
 
     if config_overrides is not None:
         config_dict = merge(config_dict, config_overrides)
```

### Comparing `BL_Python.programming-0.1.1/BL_Python/programming/patterns/dependency_injection.py` & `bl_python_programming-0.2.0/BL_Python/programming/patterns/dependency_injection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import sys
-from typing import Any
+from typing import Callable, TypeVar
 
-from injector import Binder, Module
+from injector import Binder, Module, Provider
 from typing_extensions import override
 
 
 class LoggerModule(Module):
     def __init__(
         self,
         name: str | None = None,
@@ -22,16 +22,21 @@
             self._logger.addHandler(handler)
 
     @override
     def configure(self, binder: Binder) -> None:
         binder.bind(logging.Logger, to=self._logger)
 
 
+T = TypeVar("T")
+
+
 class BatchModule(Module):
-    def __init__(self, registrations: dict[Any, Any]) -> None:
+    def __init__(
+        self, registrations: dict[type[T], None | T | Callable[..., T] | Provider[T]]
+    ) -> None:
         super().__init__()
         self._registrations = registrations
 
     @override
     def configure(self, binder: Binder) -> None:
         for interface, to in self._registrations.items():
             binder.bind(interface, to)
```

### Comparing `BL_Python.programming-0.1.1/BL_Python.programming.egg-info/PKG-INFO` & `bl_python_programming-0.2.0/BL_Python.programming.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.programming
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libraries for writing software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.programming-0.1.1/LICENSE.md` & `bl_python_programming-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.programming-0.1.1/PKG-INFO` & `bl_python_programming-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.programming
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libraries for writing software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.programming-0.1.1/pyproject.toml` & `bl_python_programming-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `BL_Python.programming-0.1.1/test/unit/test_argparse.py` & `bl_python_programming-0.2.0/test/unit/test_argparse.py`

 * *Files identical despite different names*

