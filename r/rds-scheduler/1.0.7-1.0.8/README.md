# Comparing `tmp/rds-scheduler-1.0.7.tar.gz` & `tmp/rds-scheduler-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-scheduler-1.0.7.tar", last modified: Mon Apr  8 04:59:42 2024, max compression
+gzip compressed data, was "rds-scheduler-1.0.8.tar", last modified: Tue May 14 00:20:24 2024, max compression
```

## Comparing `rds-scheduler-1.0.7.tar` & `rds-scheduler-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:59:42.550736 rds-scheduler-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-08 04:59:42.550736 rds-scheduler-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:59:42.550736 rds-scheduler-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:59:42.546736 rds-scheduler-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:59:42.550736 rds-scheduler-1.0.7/src/rds_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/src/rds_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:59:42.550736 rds-scheduler-1.0.7/src/rds_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/src/rds_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62196 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/src/rds_scheduler/_jsii/cdk-rds-scheduler@1.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:59:31.000000 rds-scheduler-1.0.7/src/rds_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:59:42.550736 rds-scheduler-1.0.7/src/rds_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-08 04:59:42.000000 rds-scheduler-1.0.7/src/rds_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 04:59:42.000000 rds-scheduler-1.0.7/src/rds_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:59:42.000000 rds-scheduler-1.0.7/src/rds_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 04:59:42.000000 rds-scheduler-1.0.7/src/rds_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 04:59:42.000000 rds-scheduler-1.0.7/src/rds_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/rds_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/rds_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62194 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/_jsii/cdk-rds-scheduler@1.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/top_level.txt
```

### Comparing `rds-scheduler-1.0.7/LICENSE` & `rds-scheduler-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rds-scheduler-1.0.7/PKG-INFO` & `rds-scheduler-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds-scheduler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Automatic Start and Stop Scheduler for AWS RDS
 Home-page: https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rds-scheduler-1.0.7/README.md` & `rds-scheduler-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rds-scheduler-1.0.7/setup.py` & `rds-scheduler-1.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "rds-scheduler",
-    "version": "1.0.7",
+    "version": "1.0.8",
     "description": "Automatic Start and Stop Scheduler for AWS RDS",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "rds_scheduler",
         "rds_scheduler._jsii"
     ],
     "package_data": {
         "rds_scheduler._jsii": [
-            "cdk-rds-scheduler@1.0.7.jsii.tgz"
+            "cdk-rds-scheduler@1.0.8.jsii.tgz"
         ],
         "rds_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.120.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `rds-scheduler-1.0.7/src/rds_scheduler/__init__.py` & `rds-scheduler-1.0.8/src/rds_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-scheduler-1.0.7/src/rds_scheduler.egg-info/PKG-INFO` & `rds-scheduler-1.0.8/src/rds_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds-scheduler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Automatic Start and Stop Scheduler for AWS RDS
 Home-page: https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

