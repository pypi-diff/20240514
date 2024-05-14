# Comparing `tmp/eoapi-cdk-7.0.1.tar.gz` & `tmp/eoapi-cdk-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eoapi-cdk-7.0.1.tar", last modified: Fri Feb 23 13:21:38 2024, max compression
+gzip compressed data, was "eoapi-cdk-7.1.0.tar", last modified: Wed Mar 13 15:14:38 2024, max compression
```

## Comparing `eoapi-cdk-7.0.1.tar` & `eoapi-cdk-7.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:21:38.740002 eoapi-cdk-7.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-23 13:21:31.000000 eoapi-cdk-7.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-23 13:21:32.000000 eoapi-cdk-7.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-02-23 13:21:38.740002 eoapi-cdk-7.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-02-23 13:21:32.000000 eoapi-cdk-7.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-23 13:21:32.000000 eoapi-cdk-7.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 13:21:38.740002 eoapi-cdk-7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-02-23 13:21:32.000000 eoapi-cdk-7.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:21:38.736002 eoapi-cdk-7.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:21:38.736002 eoapi-cdk-7.0.1/src/eoapi_cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   188753 2024-02-23 13:21:32.000000 eoapi-cdk-7.0.1/src/eoapi_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:21:38.736002 eoapi-cdk-7.0.1/src/eoapi_cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-23 13:21:32.000000 eoapi-cdk-7.0.1/src/eoapi_cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   716139 2024-02-23 13:21:31.000000 eoapi-cdk-7.0.1/src/eoapi_cdk/_jsii/eoapi-cdk@7.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:21:32.000000 eoapi-cdk-7.0.1/src/eoapi_cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:21:38.736002 eoapi-cdk-7.0.1/src/eoapi_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-02-23 13:21:38.000000 eoapi-cdk-7.0.1/src/eoapi_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-23 13:21:38.000000 eoapi-cdk-7.0.1/src/eoapi_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:21:38.000000 eoapi-cdk-7.0.1/src/eoapi_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-23 13:21:38.000000 eoapi-cdk-7.0.1/src/eoapi_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-23 13:21:38.000000 eoapi-cdk-7.0.1/src/eoapi_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:14:38.833162 eoapi-cdk-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-13 15:14:38.829162 eoapi-cdk-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 15:14:38.833162 eoapi-cdk-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:14:38.829162 eoapi-cdk-7.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:14:38.829162 eoapi-cdk-7.1.0/src/eoapi_cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   188753 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/src/eoapi_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:14:38.829162 eoapi-cdk-7.1.0/src/eoapi_cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/src/eoapi_cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   716687 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/src/eoapi_cdk/_jsii/eoapi-cdk@7.1.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:14:32.000000 eoapi-cdk-7.1.0/src/eoapi_cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:14:38.829162 eoapi-cdk-7.1.0/src/eoapi_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-13 15:14:38.000000 eoapi-cdk-7.1.0/src/eoapi_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-13 15:14:38.000000 eoapi-cdk-7.1.0/src/eoapi_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:14:38.000000 eoapi-cdk-7.1.0/src/eoapi_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-13 15:14:38.000000 eoapi-cdk-7.1.0/src/eoapi_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-13 15:14:38.000000 eoapi-cdk-7.1.0/src/eoapi_cdk.egg-info/top_level.txt
```

### Comparing `eoapi-cdk-7.0.1/LICENSE` & `eoapi-cdk-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eoapi-cdk-7.0.1/PKG-INFO` & `eoapi-cdk-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eoapi-cdk
-Version: 7.0.1
+Version: 7.1.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/eoapi-cdk.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/eoapi-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `eoapi-cdk-7.0.1/README.md` & `eoapi-cdk-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eoapi-cdk-7.0.1/setup.py` & `eoapi-cdk-7.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "eoapi-cdk",
-    "version": "7.0.1",
+    "version": "7.1.0",
     "description": "A set of constructs deploying pgSTAC with CDK",
     "license": "ISC",
     "url": "https://github.com/developmentseed/eoapi-cdk.git",
     "long_description_content_type": "text/markdown",
     "author": "Anthony Lukach<anthony@developmentseed.org>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "eoapi_cdk",
         "eoapi_cdk._jsii"
     ],
     "package_data": {
         "eoapi_cdk._jsii": [
-            "eoapi-cdk@7.0.1.jsii.tgz"
+            "eoapi-cdk@7.1.0.jsii.tgz"
         ],
         "eoapi_cdk": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `eoapi-cdk-7.0.1/src/eoapi_cdk/__init__.py` & `eoapi-cdk-7.1.0/src/eoapi_cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `eoapi-cdk-7.0.1/src/eoapi_cdk.egg-info/PKG-INFO` & `eoapi-cdk-7.1.0/src/eoapi_cdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eoapi-cdk
-Version: 7.0.1
+Version: 7.1.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/eoapi-cdk.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/eoapi-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

