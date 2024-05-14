# Comparing `tmp/geovizir-1.7.3.tar.gz` & `tmp/geovizir-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovizir-1.7.3.tar", max compression
+gzip compressed data, was "geovizir-1.8.0.tar", max compression
```

## Comparing `geovizir-1.7.3.tar` & `geovizir-1.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1074 2024-04-22 14:41:30.846687 geovizir-1.7.3/LICENSE
--rw-r--r--   0        0        0      946 2024-04-22 14:41:30.846687 geovizir-1.7.3/README.md
--rw-r--r--   0        0        0     1290 2024-04-22 14:42:07.118122 geovizir-1.7.3/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-22 14:41:30.850687 geovizir-1.7.3/src/geovizir/__init__.py
--rw-r--r--   0        0        0     1767 2024-04-22 14:41:30.850687 geovizir-1.7.3/src/geovizir/data.py
--rw-r--r--   0        0        0     1312 2024-04-22 14:41:30.850687 geovizir-1.7.3/src/geovizir/dplyr.py
--rw-r--r--   0        0        0     1996 2024-04-22 14:41:30.850687 geovizir-1.7.3/src/geovizir/features.py
--rw-r--r--   0        0        0      614 2024-04-22 14:41:30.850687 geovizir-1.7.3/src/geovizir/scales.py
--rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 geovizir-1.7.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-05-14 06:46:46.938838 geovizir-1.8.0/LICENSE
+-rw-r--r--   0        0        0      946 2024-05-14 06:46:46.938838 geovizir-1.8.0/README.md
+-rw-r--r--   0        0        0     1290 2024-05-14 06:47:26.810672 geovizir-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/__init__.py
+-rw-r--r--   0        0        0     1767 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/data.py
+-rw-r--r--   0        0        0     1312 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/dplyr.py
+-rw-r--r--   0        0        0     1996 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/features.py
+-rw-r--r--   0        0        0     1086 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/scales.py
+-rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 geovizir-1.8.0/PKG-INFO
```

### Comparing `geovizir-1.7.3/LICENSE` & `geovizir-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geovizir-1.7.3/README.md` & `geovizir-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `geovizir-1.7.3/pyproject.toml` & `geovizir-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geovizir"
-version = "1.7.3"
+version = "1.8.0"
 description = "Support package for geo visuals."
 authors = ["Pascal Burkhard"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `geovizir-1.7.3/src/geovizir/data.py` & `geovizir-1.8.0/src/geovizir/data.py`

 * *Files identical despite different names*

### Comparing `geovizir-1.7.3/src/geovizir/dplyr.py` & `geovizir-1.8.0/src/geovizir/dplyr.py`

 * *Files identical despite different names*

### Comparing `geovizir-1.7.3/src/geovizir/features.py` & `geovizir-1.8.0/src/geovizir/features.py`

 * *Files identical despite different names*

### Comparing `geovizir-1.7.3/PKG-INFO` & `geovizir-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geovizir
-Version: 1.7.3
+Version: 1.8.0
 Summary: Support package for geo visuals.
 License: MIT
 Author: Pascal Burkhard
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

