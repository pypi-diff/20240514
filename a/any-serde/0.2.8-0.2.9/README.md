# Comparing `tmp/any_serde-0.2.8.tar.gz` & `tmp/any_serde-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "any_serde-0.2.8.tar", last modified: Thu Dec 14 05:40:50 2023, max compression
+gzip compressed data, was "any_serde-0.2.9.tar", last modified: Thu Dec 14 06:25:21 2023, max compression
```

## Comparing `any_serde-0.2.8.tar` & `any_serde-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 05:40:50.386120 any_serde-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-14 05:40:41.000000 any_serde-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-12-14 05:40:50.386120 any_serde-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-12-14 05:40:41.000000 any_serde-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 05:40:50.386120 any_serde-0.2.8/any_serde/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/bytes_serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8840 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/dataclass_serde.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/enum_serde.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/json_serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/primitives_serde.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/serde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 05:40:50.386120 any_serde-0.2.8/any_serde/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/typescript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/typescript/type_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/typescript/typescript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-14 05:40:41.000000 any_serde-0.2.8/any_serde/union_serde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 05:40:50.386120 any_serde-0.2.8/any_serde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-12-14 05:40:50.000000 any_serde-0.2.8/any_serde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-14 05:40:50.000000 any_serde-0.2.8/any_serde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 05:40:50.000000 any_serde-0.2.8/any_serde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-14 05:40:50.000000 any_serde-0.2.8/any_serde.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-14 05:40:41.000000 any_serde-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 05:40:50.386120 any_serde-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-14 05:40:41.000000 any_serde-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:25:21.969206 any_serde-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-14 06:25:13.000000 any_serde-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-12-14 06:25:21.969206 any_serde-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-12-14 06:25:13.000000 any_serde-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:25:21.969206 any_serde-0.2.9/any_serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/bytes_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8840 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/dataclass_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/enum_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/json_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/primitives_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/serde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:25:21.969206 any_serde-0.2.9/any_serde/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/bool_typedef.ts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/dataclass_typedef.ts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/float_typedef.ts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/list_typedef.ts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/string_typedef.ts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/type_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/typescript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/typescript/union_typedef.ts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-14 06:25:13.000000 any_serde-0.2.9/any_serde/union_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:25:21.969206 any_serde-0.2.9/any_serde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-12-14 06:25:21.000000 any_serde-0.2.9/any_serde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2023-12-14 06:25:21.000000 any_serde-0.2.9/any_serde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 06:25:21.000000 any_serde-0.2.9/any_serde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-14 06:25:21.000000 any_serde-0.2.9/any_serde.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-14 06:25:13.000000 any_serde-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 06:25:21.969206 any_serde-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-14 06:25:13.000000 any_serde-0.2.9/setup.py
```

### Comparing `any_serde-0.2.8/LICENSE` & `any_serde-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/PKG-INFO` & `any_serde-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: any_serde
-Version: 0.2.8
+Version: 0.2.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AnySerde
 
 AnySerde is a Python package that simplifies the task of converting Python variables to and from serializable data. Whether you need to serialize Python objects to JSON, YAML, or other common formats, or deserialize data from these formats back into Python objects, AnySerde has got you covered.
```

### Comparing `any_serde-0.2.8/README.md` & `any_serde-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/__init__.py` & `any_serde-0.2.9/any_serde/__init__.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/bytes_serde.py` & `any_serde-0.2.9/any_serde/bytes_serde.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/common.py` & `any_serde-0.2.9/any_serde/common.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/dataclass_serde.py` & `any_serde-0.2.9/any_serde/dataclass_serde.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/enum_serde.py` & `any_serde-0.2.9/any_serde/enum_serde.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/json_serde.py` & `any_serde-0.2.9/any_serde/json_serde.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/primitives_serde.py` & `any_serde-0.2.9/any_serde/primitives_serde.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/serde.py` & `any_serde-0.2.9/any_serde/serde.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/typescript/type_gen.py` & `any_serde-0.2.9/any_serde/typescript/type_gen.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde/union_serde.py` & `any_serde-0.2.9/any_serde/union_serde.py`

 * *Files identical despite different names*

### Comparing `any_serde-0.2.8/any_serde.egg-info/PKG-INFO` & `any_serde-0.2.9/any_serde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: any-serde
-Version: 0.2.8
+Version: 0.2.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AnySerde
 
 AnySerde is a Python package that simplifies the task of converting Python variables to and from serializable data. Whether you need to serialize Python objects to JSON, YAML, or other common formats, or deserialize data from these formats back into Python objects, AnySerde has got you covered.
```

### Comparing `any_serde-0.2.8/any_serde.egg-info/SOURCES.txt` & `any_serde-0.2.9/any_serde.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,9 +13,15 @@
 any_serde/serde.py
 any_serde/union_serde.py
 any_serde.egg-info/PKG-INFO
 any_serde.egg-info/SOURCES.txt
 any_serde.egg-info/dependency_links.txt
 any_serde.egg-info/top_level.txt
 any_serde/typescript/__init__.py
+any_serde/typescript/bool_typedef.ts.jinja2
+any_serde/typescript/dataclass_typedef.ts.jinja2
+any_serde/typescript/float_typedef.ts.jinja2
+any_serde/typescript/list_typedef.ts.jinja2
+any_serde/typescript/string_typedef.ts.jinja2
 any_serde/typescript/type_gen.py
-any_serde/typescript/typescript_utils.py
+any_serde/typescript/typescript_utils.py
+any_serde/typescript/union_typedef.ts.jinja2
```

