# Comparing `tmp/foamlib-0.3.8.tar.gz` & `tmp/foamlib-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.3.8.tar", last modified: Mon May 13 16:43:48 2024, max compression
+gzip compressed data, was "foamlib-0.3.9.tar", last modified: Tue May 14 00:17:29 2024, max compression
```

## Comparing `foamlib-0.3.8.tar` & `foamlib-0.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.977108 foamlib-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-05-13 16:43:41.000000 foamlib-0.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-13 16:43:48.977108 foamlib-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-13 16:43:41.000000 foamlib-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.973108 foamlib-0.3.8/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21142 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.973108 foamlib-0.3.8/foamlib/_files/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.973108 foamlib-0.3.8/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-13 16:43:41.000000 foamlib-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:43:48.977108 foamlib-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:17:29.615459 foamlib-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-05-14 00:17:21.000000 foamlib-0.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-14 00:17:29.615459 foamlib-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-14 00:17:21.000000 foamlib-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:17:29.611459 foamlib-0.3.9/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21417 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:17:29.615459 foamlib-0.3.9/foamlib/_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_files/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_files/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_files/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_files/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_files/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 00:17:21.000000 foamlib-0.3.9/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:17:29.615459 foamlib-0.3.9/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-14 00:17:29.000000 foamlib-0.3.9/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-14 00:17:29.000000 foamlib-0.3.9/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:17:29.000000 foamlib-0.3.9/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 00:17:29.000000 foamlib-0.3.9/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 00:17:29.000000 foamlib-0.3.9/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-14 00:17:21.000000 foamlib-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 00:17:29.615459 foamlib-0.3.9/setup.cfg
```

### Comparing `foamlib-0.3.8/LICENSE.txt` & `foamlib-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.8/PKG-INFO` & `foamlib-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.8/README.md` & `foamlib-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.8/foamlib/_cases.py` & `foamlib-0.3.9/foamlib/_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,31 +52,37 @@
 
         @property
         def name(self) -> str:
             """The name of this time directory."""
             return self.path.name
 
         def __getitem__(self, key: str) -> FoamFieldFile:
-            try:
+            if (self.path / key).is_file():
                 return FoamFieldFile(self.path / key)
-            except FileNotFoundError as e:
-                raise KeyError(key) from e
+            elif (self.path / f"{key}.gz").is_file():
+                return FoamFieldFile(self.path / f"{key}.gz")
+            else:
+                raise KeyError(key)
 
         def __contains__(self, obj: object) -> bool:
             if isinstance(obj, FoamFieldFile):
                 return obj.path.parent == self.path
             elif isinstance(obj, str):
-                return (self.path / obj).is_file()
+                return (self.path / obj).is_file() or (
+                    self.path / f"{obj}.gz"
+                ).is_file()
             else:
                 return False
 
         def __iter__(self) -> Iterator[FoamFieldFile]:
             for p in self.path.iterdir():
-                if p.is_file():
-                    yield FoamFieldFile(p.name)
+                if p.is_file() and (
+                    p.suffix != ".gz" or not p.with_suffix("").is_file()
+                ):
+                    yield FoamFieldFile(p)
 
         def __len__(self) -> int:
             return len(list(iter(self)))
 
         def __fspath__(self) -> str:
             return str(self.path)
 
@@ -110,15 +116,15 @@
     @overload
     def __getitem__(self, index: slice) -> Sequence["FoamCaseBase.TimeDirectory"]: ...
 
     def __getitem__(
         self, index: Union[int, slice, float, str]
     ) -> Union["FoamCaseBase.TimeDirectory", Sequence["FoamCaseBase.TimeDirectory"]]:
         if isinstance(index, str):
-            return FoamCaseBase.TimeDirectory(self.path / str(index))
+            return FoamCaseBase.TimeDirectory(self.path / index)
         elif isinstance(index, float):
             for time in self._times:
                 if time.time == index:
                     return time
             raise IndexError(f"Time {index} not found")
         return self._times[index]
```

### Comparing `foamlib-0.3.8/foamlib/_files/_base.py` & `foamlib-0.3.9/foamlib/_files/_base.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.8/foamlib/_files/_files.py` & `foamlib-0.3.9/foamlib/_files/_files.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.8/foamlib/_files/_io.py` & `foamlib-0.3.9/foamlib/_files/_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import gzip
 import sys
 from copy import deepcopy
 from pathlib import Path
 from types import TracebackType
 from typing import (
     Optional,
     Tuple,
@@ -43,14 +44,18 @@
             assert self.__contents is not None
             self._write(self.__contents)
         assert not self.__dirty
 
     def _read(self) -> Tuple[bytes, Parsed]:
         if not self.__defer_io:
             contents = self.path.read_bytes()
+
+            if self.path.suffix == ".gz":
+                contents = gzip.decompress(contents)
+
             if contents != self.__contents:
                 self.__contents = contents
                 self.__parsed = None
 
         assert self.__contents is not None
 
         if self.__parsed is None:
@@ -59,14 +64,17 @@
 
         return self.__contents, deepcopy(self.__parsed)
 
     def _write(self, contents: bytes) -> None:
         self.__contents = contents
         self.__parsed = None
         if not self.__defer_io:
+            if self.path.suffix == ".gz":
+                contents = gzip.compress(contents)
+
             self.path.write_bytes(contents)
             self.__dirty = False
         else:
             self.__dirty = True
 
     def __repr__(self) -> str:
         return f"{type(self).__qualname__}('{self.path}')"
```

### Comparing `foamlib-0.3.8/foamlib/_files/_parsing.py` & `foamlib-0.3.9/foamlib/_files/_parsing.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.8/foamlib/_files/_serialization.py` & `foamlib-0.3.9/foamlib/_files/_serialization.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.8/foamlib/_util.py` & `foamlib-0.3.9/foamlib/_util.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.8/foamlib.egg-info/PKG-INFO` & `foamlib-0.3.9/foamlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.8/pyproject.toml` & `foamlib-0.3.9/pyproject.toml`

 * *Files identical despite different names*

