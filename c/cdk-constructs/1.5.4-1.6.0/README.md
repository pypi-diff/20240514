# Comparing `tmp/cdk-constructs-1.5.4.tar.gz` & `tmp/cdk-constructs-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-constructs-1.5.4.tar", last modified: Mon May 13 18:52:04 2024, max compression
+gzip compressed data, was "cdk-constructs-1.6.0.tar", last modified: Tue May 14 12:41:00 2024, max compression
```

## Comparing `cdk-constructs-1.5.4.tar` & `cdk-constructs-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:04.080042 cdk-constructs-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-13 18:52:04.080042 cdk-constructs-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:52:04.080042 cdk-constructs-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:04.076042 cdk-constructs-1.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:04.076042 cdk-constructs-1.5.4/src/cdk-constructs/
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/src/cdk-constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:04.080042 cdk-constructs-1.5.4/src/cdk-constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/src/cdk-constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33592 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/src/cdk-constructs/_jsii/cdk-constructs@1.5.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:51:53.000000 cdk-constructs-1.5.4/src/cdk-constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:04.080042 cdk-constructs-1.5.4/src/cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-13 18:52:04.000000 cdk-constructs-1.5.4/src/cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 18:52:04.000000 cdk-constructs-1.5.4/src/cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:52:04.000000 cdk-constructs-1.5.4/src/cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 18:52:04.000000 cdk-constructs-1.5.4/src/cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 18:52:04.000000 cdk-constructs-1.5.4/src/cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.501948 cdk-constructs-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/src/cdk-constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/src/cdk-constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34139 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/_jsii/cdk-constructs@1.6.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdk-constructs-1.5.4/LICENSE` & `cdk-constructs-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.5.4/PKG-INFO` & `cdk-constructs-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.5.4
+Version: 1.6.0
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-constructs-1.5.4/README.md` & `cdk-constructs-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.5.4/setup.py` & `cdk-constructs-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-constructs",
-    "version": "1.5.4",
+    "version": "1.6.0",
     "description": "A CDK construct library",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-constructs",
         "cdk-constructs._jsii"
     ],
     "package_data": {
         "cdk-constructs._jsii": [
-            "cdk-constructs@1.5.4.jsii.tgz"
+            "cdk-constructs@1.6.0.jsii.tgz"
         ],
         "cdk-constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-constructs-1.5.4/src/cdk_constructs.egg-info/PKG-INFO` & `cdk-constructs-1.6.0/src/cdk_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.5.4
+Version: 1.6.0
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

