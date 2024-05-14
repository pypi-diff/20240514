# Comparing `tmp/cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3.tar.gz` & `tmp/cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3.tar", last modified: Mon May 13 15:31:36 2024, max compression
+gzip compressed data, was "cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4.tar", last modified: Tue May 14 19:10:38 2024, max compression
```

## Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3.tar` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:36.591631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-13 15:31:36.591631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:31:36.591631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:36.587631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:36.587631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:36.587631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/
--rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:36.591631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1212960 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:31:24.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:36.587631 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-13 15:31:36.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-13 15:31:36.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:31:36.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 15:31:36.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 15:31:36.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:10:38.864643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-14 19:10:38.864643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:10:38.864643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:10:38.860643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:10:38.860643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:10:38.864643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:10:38.864643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1212778 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:10:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:10:38.864643 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-14 19:10:38.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-14 19:10:38.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:10:38.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 19:10:38.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 19:10:38.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/LICENSE` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/PKG-INFO` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-iot-thing-certificate-policy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Creates an AWS IoT thing, certificate, policy, and associates the three together
 Home-page: https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -88,17 +88,17 @@
 // Add this
 import "github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go/cdklabscdkawsiotthingcertificatepolicy"
 ```
 
 ## Usage
 
 ```python
+from cdklabs.cdk_aws_iot_thing_certificate_policy import PolicyMapping, PolicyMapping
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import IotThingCertificatePolicy
-
 #
 # A minimum IoT Policy template using substitution variables for actual
 # policy to be deployed for "region", "account", and "thingname". Allows
 # the thing to publish and subscribe on any topics under "thing/*" topic
 # namespace. Normal IoT Policy conventions such as "*", apply.
 #
 minimal_iot_policy = """{
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/README.md` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 // Add this
 import "github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go/cdklabscdkawsiotthingcertificatepolicy"
 ```
 
 ## Usage
 
 ```python
+from cdklabs.cdk_aws_iot_thing_certificate_policy import PolicyMapping, PolicyMapping
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import IotThingCertificatePolicy
-
 #
 # A minimum IoT Policy template using substitution variables for actual
 # policy to be deployed for "region", "account", and "thingname". Allows
 # the thing to publish and subscribe on any topics under "thing/*" topic
 # namespace. Normal IoT Policy conventions such as "*", apply.
 #
 minimal_iot_policy = """{
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/setup.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-aws-iot-thing-certificate-policy",
-    "version": "0.0.3",
+    "version": "0.0.4",
     "description": "Creates an AWS IoT thing, certificate, policy, and associates the three together",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_aws_iot_thing_certificate_policy",
         "cdklabs.cdk_aws_iot_thing_certificate_policy._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_aws_iot_thing_certificate_policy._jsii": [
-            "cdk-aws-iot-thing-certificate-policy@0.0.3.jsii.tgz"
+            "cdk-aws-iot-thing-certificate-policy@0.0.4.jsii.tgz"
         ],
         "cdklabs.cdk_aws_iot_thing_certificate_policy": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 // Add this
 import "github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go/cdklabscdkawsiotthingcertificatepolicy"
 ```
 
 ## Usage
 
 ```python
+from cdklabs.cdk_aws_iot_thing_certificate_policy import PolicyMapping, PolicyMapping
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import IotThingCertificatePolicy
-
 #
 # A minimum IoT Policy template using substitution variables for actual
 # policy to be deployed for "region", "account", and "thingname". Allows
 # the thing to publish and subscribe on any topics under "thing/*" topic
 # namespace. Normal IoT Policy conventions such as "*", apply.
 #
 minimal_iot_policy = """{
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/cdk-aws-iot-thing-certificate-policy",
-    "0.0.3",
+    "0.0.4",
     __name__[0:-6],
-    "cdk-aws-iot-thing-certificate-policy@0.0.3.jsii.tgz",
+    "cdk-aws-iot-thing-certificate-policy@0.0.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-iot-thing-certificate-policy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Creates an AWS IoT thing, certificate, policy, and associates the three together
 Home-page: https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -88,17 +88,17 @@
 // Add this
 import "github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go/cdklabscdkawsiotthingcertificatepolicy"
 ```
 
 ## Usage
 
 ```python
+from cdklabs.cdk_aws_iot_thing_certificate_policy import PolicyMapping, PolicyMapping
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import IotThingCertificatePolicy
-
 #
 # A minimum IoT Policy template using substitution variables for actual
 # policy to be deployed for "region", "account", and "thingname". Allows
 # the thing to publish and subscribe on any topics under "thing/*" topic
 # namespace. Normal IoT Policy conventions such as "*", apply.
 #
 minimal_iot_policy = """{
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.3/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.4/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
-src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.3.jsii.tgz
+src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.4.jsii.tgz
```

