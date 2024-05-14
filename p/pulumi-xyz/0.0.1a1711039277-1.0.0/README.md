# Comparing `tmp/pulumi_xyz-0.0.1a1711039277.tar.gz` & `tmp/pulumi_xyz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_xyz-0.0.1a1711039277.tar", last modified: Thu Mar 21 16:45:17 2024, max compression
+gzip compressed data, was "pulumi_xyz-1.0.0.tar", last modified: Tue May 14 12:03:23 2024, max compression
```

## Comparing `pulumi_xyz-0.0.1a1711039277.tar` & `pulumi_xyz-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:45:17.863877 pulumi_xyz-0.0.1a1711039277/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-21 16:45:17.863877 pulumi_xyz-0.0.1a1711039277/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:45:17.863877 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/get_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:45:17.863877 pulumi_xyz-0.0.1a1711039277/pulumi_xyz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-21 16:45:17.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-21 16:45:17.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 16:45:17.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-21 16:45:17.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 16:45:17.000000 pulumi_xyz-0.0.1a1711039277/pulumi_xyz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-21 16:45:08.000000 pulumi_xyz-0.0.1a1711039277/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 16:45:17.863877 pulumi_xyz-0.0.1a1711039277/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:03:23.853271 pulumi_xyz-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-14 12:03:23.853271 pulumi_xyz-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:03:23.853271 pulumi_xyz-1.0.0/pulumi_xyz/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pulumi_xyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pulumi_xyz/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pulumi_xyz/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pulumi_xyz/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pulumi_xyz/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pulumi_xyz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pulumi_xyz/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:03:23.853271 pulumi_xyz-1.0.0/pulumi_xyz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-14 12:03:23.000000 pulumi_xyz-1.0.0/pulumi_xyz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 12:03:23.000000 pulumi_xyz-1.0.0/pulumi_xyz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:03:23.000000 pulumi_xyz-1.0.0/pulumi_xyz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 12:03:23.000000 pulumi_xyz-1.0.0/pulumi_xyz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 12:03:23.000000 pulumi_xyz-1.0.0/pulumi_xyz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-14 12:03:17.000000 pulumi_xyz-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:03:23.853271 pulumi_xyz-1.0.0/setup.cfg
```

### Comparing `pulumi_xyz-0.0.1a1711039277/PKG-INFO` & `pulumi_xyz-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_xyz
-Version: 0.0.1a1711039277
+Version: 1.0.0
 Summary: A Pulumi package for creating and managing xyz cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-xyz
 Keywords: pulumi,xyz,category/cloud
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_xyz-0.0.1a1711039277/README.md` & `pulumi_xyz-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_xyz-0.0.1a1711039277/pulumi_xyz/__init__.py` & `pulumi_xyz-1.0.0/pulumi_xyz/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .data_source import *
-from .get_data_source import *
 from .provider import *
 from .resource import *
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "xyz",
```

### Comparing `pulumi_xyz-0.0.1a1711039277/pulumi_xyz/_utilities.py` & `pulumi_xyz-1.0.0/pulumi_xyz/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_xyz-0.0.1a1711039277/pulumi_xyz/data_source.py` & `pulumi_xyz-1.0.0/pulumi_xyz/data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_xyz-0.0.1a1711039277/pulumi_xyz/provider.py` & `pulumi_xyz-1.0.0/pulumi_xyz/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_xyz-0.0.1a1711039277/pulumi_xyz/resource.py` & `pulumi_xyz-1.0.0/pulumi_xyz/resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_xyz-0.0.1a1711039277/pulumi_xyz.egg-info/PKG-INFO` & `pulumi_xyz-1.0.0/pulumi_xyz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_xyz
-Version: 0.0.1a1711039277
+Version: 1.0.0
 Summary: A Pulumi package for creating and managing xyz cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-xyz
 Keywords: pulumi,xyz,category/cloud
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_xyz-0.0.1a1711039277/pyproject.toml` & `pulumi_xyz-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_xyz"
   description = "A Pulumi package for creating and managing xyz cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "xyz", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.7"
-  version = "0.0.1a1711039277"
+  version = "1.0.0"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-xyz"
 
 [build-system]
```

