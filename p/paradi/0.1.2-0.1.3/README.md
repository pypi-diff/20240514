# Comparing `tmp/paradi-0.1.2.tar.gz` & `tmp/paradi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradi-0.1.2.tar", last modified: Tue May 14 06:55:18 2024, max compression
+gzip compressed data, was "paradi-0.1.3.tar", last modified: Tue May 14 07:41:45 2024, max compression
```

## Comparing `paradi-0.1.2.tar` & `paradi-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:18.256995 paradi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 06:55:13.000000 paradi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 06:55:18.256995 paradi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-14 06:55:13.000000 paradi-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:18.256995 paradi-0.1.2/paradi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 06:55:13.000000 paradi-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:55:18.256995 paradi-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 06:55:13.000000 paradi-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:18.256995 paradi-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:13.000000 paradi-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 06:55:13.000000 paradi-0.1.2/tests/flask_test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-14 06:55:13.000000 paradi-0.1.2/tests/test_paradi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 07:41:39.000000 paradi-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 07:41:45.873882 paradi-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-14 07:41:39.000000 paradi-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/paradi/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-14 07:41:39.000000 paradi-0.1.3/paradi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-14 07:41:39.000000 paradi-0.1.3/paradi/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-14 07:41:39.000000 paradi-0.1.3/paradi/paradi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/paradi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 07:41:39.000000 paradi-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:41:45.873882 paradi-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 07:41:39.000000 paradi-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-14 07:41:39.000000 paradi-0.1.3/tests/test_paradi.py
```

### Comparing `paradi-0.1.2/LICENSE` & `paradi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paradi-0.1.2/PKG-INFO` & `paradi-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradi
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
 Author: Julien Crambes
 Author-email: Julien Crambes <julien.crambes@gmail.com>
 Project-URL: Homepage, https://github.com/Elektriman/paradi
 Project-URL: Issues, https://github.com/Elektriman/paradi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paradi-0.1.2/README.md` & `paradi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `paradi-0.1.2/paradi.egg-info/PKG-INFO` & `paradi-0.1.3/paradi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradi
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
 Author: Julien Crambes
 Author-email: Julien Crambes <julien.crambes@gmail.com>
 Project-URL: Homepage, https://github.com/Elektriman/paradi
 Project-URL: Issues, https://github.com/Elektriman/paradi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paradi-0.1.2/pyproject.toml` & `paradi-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "paradi"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Julien Crambes", email="julien.crambes@gmail.com" },
 ]
 description = "This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities."
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `paradi-0.1.2/tests/test_paradi.py` & `paradi-0.1.3/tests/test_paradi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # %% imports
 import pytest
 import requests
 import json
 import os
-from paradi import Paradi
+from paradi.paradi import Paradi
 from dotenv import load_dotenv
 
 
 # %% constants
 load_dotenv()
 with open("http.json", "r") as f:
     http_dict = json.load(f)
```

