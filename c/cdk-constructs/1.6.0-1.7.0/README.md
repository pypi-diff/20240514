# Comparing `tmp/cdk-constructs-1.6.0.tar.gz` & `tmp/cdk-constructs-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-constructs-1.6.0.tar", last modified: Tue May 14 12:41:00 2024, max compression
+gzip compressed data, was "cdk-constructs-1.7.0.tar", last modified: Tue May 14 14:34:17 2024, max compression
```

## Comparing `cdk-constructs-1.6.0.tar` & `cdk-constructs-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.501948 cdk-constructs-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/src/cdk-constructs/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/src/cdk-constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34139 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/_jsii/cdk-constructs@1.6.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:40:47.000000 cdk-constructs-1.6.0/src/cdk-constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:41:00.505948 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 12:41:00.000000 cdk-constructs-1.6.0/src/cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.669517 cdk-constructs-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.669517 cdk-constructs-1.7.0/src/cdk-constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/src/cdk-constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.669517 cdk-constructs-1.7.0/src/cdk-constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/src/cdk-constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35271 2024-05-14 14:34:01.000000 cdk-constructs-1.7.0/src/cdk-constructs/_jsii/cdk-constructs@1.7.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/src/cdk-constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdk-constructs-1.6.0/LICENSE` & `cdk-constructs-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.6.0/PKG-INFO` & `cdk-constructs-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.6.0
+Version: 1.7.0
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-constructs-1.6.0/README.md` & `cdk-constructs-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.6.0/setup.py` & `cdk-constructs-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-constructs",
-    "version": "1.6.0",
+    "version": "1.7.0",
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
-            "cdk-constructs@1.6.0.jsii.tgz"
+            "cdk-constructs@1.7.0.jsii.tgz"
         ],
         "cdk-constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-constructs-1.6.0/src/cdk-constructs/__init__.py` & `cdk-constructs-1.7.0/src/cdk-constructs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,24 @@
 class IVpcBase(typing_extensions.Protocol):
     @builtins.property
     @jsii.member(jsii_name="cidr")
     def cidr(self) -> builtins.str:
         ...
 
     @builtins.property
+    @jsii.member(jsii_name="enableEndpointDynamoDB")
+    def enable_endpoint_dynamo_db(self) -> typing.Optional[builtins.bool]:
+        ...
+
+    @builtins.property
+    @jsii.member(jsii_name="enableEndpointS3")
+    def enable_endpoint_s3(self) -> typing.Optional[builtins.bool]:
+        ...
+
+    @builtins.property
     @jsii.member(jsii_name="maxAzs")
     def max_azs(self) -> typing.Optional[jsii.Number]:
         ...
 
     @builtins.property
     @jsii.member(jsii_name="natGateways")
     def nat_gateways(self) -> typing.Optional[jsii.Number]:
@@ -132,14 +142,24 @@
 
     @builtins.property
     @jsii.member(jsii_name="cidr")
     def cidr(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "cidr"))
 
     @builtins.property
+    @jsii.member(jsii_name="enableEndpointDynamoDB")
+    def enable_endpoint_dynamo_db(self) -> typing.Optional[builtins.bool]:
+        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableEndpointDynamoDB"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableEndpointS3")
+    def enable_endpoint_s3(self) -> typing.Optional[builtins.bool]:
+        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableEndpointS3"))
+
+    @builtins.property
     @jsii.member(jsii_name="maxAzs")
     def max_azs(self) -> typing.Optional[jsii.Number]:
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "maxAzs"))
 
     @builtins.property
     @jsii.member(jsii_name="natGateways")
     def nat_gateways(self) -> typing.Optional[jsii.Number]:
```

### Comparing `cdk-constructs-1.6.0/src/cdk_constructs.egg-info/PKG-INFO` & `cdk-constructs-1.7.0/src/cdk_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.6.0
+Version: 1.7.0
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

