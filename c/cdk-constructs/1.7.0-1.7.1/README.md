# Comparing `tmp/cdk-constructs-1.7.0.tar.gz` & `tmp/cdk-constructs-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-constructs-1.7.0.tar", last modified: Tue May 14 14:34:17 2024, max compression
+gzip compressed data, was "cdk-constructs-1.7.1.tar", last modified: Tue May 14 15:14:45 2024, max compression
```

## Comparing `cdk-constructs-1.7.0.tar` & `cdk-constructs-1.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.669517 cdk-constructs-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.669517 cdk-constructs-1.7.0/src/cdk-constructs/
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/src/cdk-constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.669517 cdk-constructs-1.7.0/src/cdk-constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/src/cdk-constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35271 2024-05-14 14:34:01.000000 cdk-constructs-1.7.0/src/cdk-constructs/_jsii/cdk-constructs@1.7.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:34:02.000000 cdk-constructs-1.7.0/src/cdk-constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:34:17.673517 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 14:34:17.000000 cdk-constructs-1.7.0/src/cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:45.300745 cdk-constructs-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 15:14:45.300745 cdk-constructs-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:14:45.300745 cdk-constructs-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:45.296745 cdk-constructs-1.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:45.300745 cdk-constructs-1.7.1/src/cdk-constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/src/cdk-constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:45.300745 cdk-constructs-1.7.1/src/cdk-constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/src/cdk-constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35954 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/src/cdk-constructs/_jsii/cdk-constructs@1.7.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:14:35.000000 cdk-constructs-1.7.1/src/cdk-constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:45.300745 cdk-constructs-1.7.1/src/cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 15:14:45.000000 cdk-constructs-1.7.1/src/cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 15:14:45.000000 cdk-constructs-1.7.1/src/cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:14:45.000000 cdk-constructs-1.7.1/src/cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 15:14:45.000000 cdk-constructs-1.7.1/src/cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 15:14:45.000000 cdk-constructs-1.7.1/src/cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdk-constructs-1.7.0/LICENSE` & `cdk-constructs-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.7.0/PKG-INFO` & `cdk-constructs-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.7.0
+Version: 1.7.1
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-constructs-1.7.0/README.md` & `cdk-constructs-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.7.0/setup.py` & `cdk-constructs-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-constructs",
-    "version": "1.7.0",
+    "version": "1.7.1",
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
-            "cdk-constructs@1.7.0.jsii.tgz"
+            "cdk-constructs@1.7.1.jsii.tgz"
         ],
         "cdk-constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-constructs-1.7.0/src/cdk-constructs/__init__.py` & `cdk-constructs-1.7.1/src/cdk-constructs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,66 +107,80 @@
 import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
 import aws_cdk.pipelines as _aws_cdk_pipelines_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
 @jsii.interface(jsii_type="cdk-constructs.IVpcBase")
 class IVpcBase(typing_extensions.Protocol):
+    '''Represents the configuration for a VPC.'''
+
     @builtins.property
     @jsii.member(jsii_name="cidr")
     def cidr(self) -> builtins.str:
+        '''The CIDR block for the VPC.'''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="enableEndpointDynamoDB")
     def enable_endpoint_dynamo_db(self) -> typing.Optional[builtins.bool]:
+        '''Indicates whether to enable the DynamoDB endpoint for the VPC.'''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="enableEndpointS3")
     def enable_endpoint_s3(self) -> typing.Optional[builtins.bool]:
+        '''Indicates whether to enable the S3 endpoint for the VPC.'''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="maxAzs")
     def max_azs(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of availability zones to use for the VPC.'''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="natGateways")
     def nat_gateways(self) -> typing.Optional[jsii.Number]:
+        '''The number of NAT gateways to create for the VPC.'''
         ...
 
 
 class _IVpcBaseProxy:
+    '''Represents the configuration for a VPC.'''
+
     __jsii_type__: typing.ClassVar[str] = "cdk-constructs.IVpcBase"
 
     @builtins.property
     @jsii.member(jsii_name="cidr")
     def cidr(self) -> builtins.str:
+        '''The CIDR block for the VPC.'''
         return typing.cast(builtins.str, jsii.get(self, "cidr"))
 
     @builtins.property
     @jsii.member(jsii_name="enableEndpointDynamoDB")
     def enable_endpoint_dynamo_db(self) -> typing.Optional[builtins.bool]:
+        '''Indicates whether to enable the DynamoDB endpoint for the VPC.'''
         return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableEndpointDynamoDB"))
 
     @builtins.property
     @jsii.member(jsii_name="enableEndpointS3")
     def enable_endpoint_s3(self) -> typing.Optional[builtins.bool]:
+        '''Indicates whether to enable the S3 endpoint for the VPC.'''
         return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableEndpointS3"))
 
     @builtins.property
     @jsii.member(jsii_name="maxAzs")
     def max_azs(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of availability zones to use for the VPC.'''
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "maxAzs"))
 
     @builtins.property
     @jsii.member(jsii_name="natGateways")
     def nat_gateways(self) -> typing.Optional[jsii.Number]:
+        '''The number of NAT gateways to create for the VPC.'''
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "natGateways"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IVpcBase).__jsii_proxy_class__ = lambda : _IVpcBaseProxy
 
 
 class PipelineCdk(
@@ -270,14 +284,16 @@
 
 
 class VpcBase(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-constructs.VpcBase",
 ):
+    '''A VPC construct that creates a VPC with public and private subnets.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         props: IVpcBase,
     ) -> None:
         '''
@@ -291,14 +307,15 @@
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="vpc")
     def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.Vpc:
+        '''The VPC created by the construct.'''
         return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Vpc, jsii.get(self, "vpc"))
 
 
 __all__ = [
     "IVpcBase",
     "PipelineCdk",
     "PipelineProps",
```

### Comparing `cdk-constructs-1.7.0/src/cdk_constructs.egg-info/PKG-INFO` & `cdk-constructs-1.7.1/src/cdk_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.7.0
+Version: 1.7.1
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

