# Comparing `tmp/mypy-boto3-s3-1.34.65.tar.gz` & `tmp/mypy_boto3_s3-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3-1.34.65.tar", last modified: Mon Mar 18 20:47:31 2024, max compression
+gzip compressed data, was "mypy_boto3_s3-1.34.91.tar", last modified: Thu Apr 25 00:48:26 2024, max compression
```

## Comparing `mypy-boto3-s3-1.34.65.tar` & `mypy_boto3_s3-1.34.91.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:31.230607 mypy-boto3-s3-1.34.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-03-18 20:47:31.230607 mypy-boto3-s3-1.34.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:31.226607 mypy-boto3-s3-1.34.65/mypy_boto3_s3/
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79800 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    79797 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-03-18 20:47:15.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-03-18 20:47:15.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-03-18 20:47:15.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-03-18 20:47:15.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   117059 2024-03-18 20:47:15.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   117016 2024-03-18 20:47:14.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   159279 2024-03-18 20:47:19.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   159279 2024-03-18 20:47:17.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 20:47:13.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-03-18 20:47:15.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-18 20:47:15.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:31.230607 mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-03-18 20:47:31.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-18 20:47:31.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:31.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:31.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-18 20:47:31.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-18 20:47:31.000000 mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 20:47:31.230607 mypy-boto3-s3-1.34.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-18 20:47:12.000000 mypy-boto3-s3-1.34.65/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:26.688523 mypy_boto3_s3-1.34.91/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17736 2024-04-25 00:48:26.688523 mypy_boto3_s3-1.34.91/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16201 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:26.678523 mypy_boto3_s3-1.34.91/mypy_boto3_s3/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2510 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2510 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      899 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    79880 2024-04-24 23:44:00.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    79877 2024-04-24 23:43:58.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17952 2024-04-24 23:44:07.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17952 2024-04-24 23:44:06.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8374 2024-04-24 23:44:05.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8367 2024-04-24 23:44:05.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   116809 2024-04-24 23:44:05.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   116766 2024-04-24 23:44:03.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   170104 2024-04-24 23:44:19.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   170104 2024-04-24 23:44:15.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       62 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5280 2024-04-24 23:44:06.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5276 2024-04-24 23:44:06.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:26.688523 mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17736 2024-04-25 00:48:26.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      703 2024-04-25 00:48:26.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:26.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:26.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       53 2024-04-25 00:48:26.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       14 2024-04-25 00:48:26.000000 mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2024-04-25 00:48:26.688523 mypy_boto3_s3-1.34.91/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1939 2024-04-24 23:43:55.000000 mypy_boto3_s3-1.34.91/setup.py
```

### Comparing `mypy-boto3-s3-1.34.65/LICENSE` & `mypy_boto3_s3-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/PKG-INFO` & `mypy_boto3_s3-1.34.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.34.65
-Summary: Type annotations for boto3.S3 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.S3 1.34.91 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3)](https://pepy.tech/project/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3-1.34.65/README.md` & `mypy_boto3_s3-1.34.91/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3)](https://pepy.tech/project/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/__init__.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/__init__.pyi` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/__main__.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3 1.34.65\n"
-        "Version:         1.34.65\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.S3 1.34.91\n"
+        "Version:         1.34.91\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.65")
+    print("1.34.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/client.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
-    AnalyticsConfigurationTypeDef,
+    AnalyticsConfigurationUnionTypeDef,
     BlobTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
     CompleteMultipartUploadOutputTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
@@ -95,53 +95,53 @@
     GetObjectRetentionOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     GetObjectTorrentOutputTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     HeadBucketOutputTypeDef,
     HeadObjectOutputTypeDef,
     InputSerializationTypeDef,
-    IntelligentTieringConfigurationTypeDef,
-    InventoryConfigurationTypeDef,
+    IntelligentTieringConfigurationUnionTypeDef,
+    InventoryConfigurationUnionTypeDef,
     LifecycleConfigurationTypeDef,
     ListBucketAnalyticsConfigurationsOutputTypeDef,
     ListBucketIntelligentTieringConfigurationsOutputTypeDef,
     ListBucketInventoryConfigurationsOutputTypeDef,
     ListBucketMetricsConfigurationsOutputTypeDef,
     ListBucketsOutputTypeDef,
     ListDirectoryBucketsOutputTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListObjectsOutputTypeDef,
     ListObjectsV2OutputTypeDef,
     ListObjectVersionsOutputTypeDef,
     ListPartsOutputTypeDef,
-    MetricsConfigurationTypeDef,
+    MetricsConfigurationUnionTypeDef,
     NotificationConfigurationDeprecatedResponseTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     NotificationConfigurationResponseTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
-    ObjectLockRetentionTypeDef,
+    ObjectLockRetentionUnionTypeDef,
     OutputSerializationTypeDef,
-    OwnershipControlsTypeDef,
+    OwnershipControlsUnionTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectLegalHoldOutputTypeDef,
     PutObjectLockConfigurationOutputTypeDef,
     PutObjectOutputTypeDef,
     PutObjectRetentionOutputTypeDef,
     PutObjectTaggingOutputTypeDef,
-    ReplicationConfigurationTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
     SelectObjectContentOutputTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
+    ServerSideEncryptionConfigurationUnionTypeDef,
     TaggingTypeDef,
     TimestampTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
@@ -1263,15 +1263,15 @@
         """
 
     def put_bucket_analytics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        AnalyticsConfiguration: AnalyticsConfigurationTypeDef,
+        AnalyticsConfiguration: AnalyticsConfigurationUnionTypeDef,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_analytics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_analytics_configuration)
@@ -1292,15 +1292,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_cors)
         """
 
     def put_bucket_encryption(
         self,
         *,
         Bucket: str,
-        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
+        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationUnionTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
@@ -1309,29 +1309,29 @@
         """
 
     def put_bucket_intelligent_tiering_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef,
+        IntelligentTieringConfiguration: IntelligentTieringConfigurationUnionTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_intelligent_tiering_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_intelligent_tiering_configuration)
         """
 
     def put_bucket_inventory_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        InventoryConfiguration: InventoryConfigurationTypeDef,
+        InventoryConfiguration: InventoryConfigurationUnionTypeDef,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_inventory_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_inventory_configuration)
@@ -1383,15 +1383,15 @@
         """
 
     def put_bucket_metrics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        MetricsConfiguration: MetricsConfigurationTypeDef,
+        MetricsConfiguration: MetricsConfigurationUnionTypeDef,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_metrics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_metrics_configuration)
@@ -1427,15 +1427,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_notification_configuration)
         """
 
     def put_bucket_ownership_controls(
         self,
         *,
         Bucket: str,
-        OwnershipControls: OwnershipControlsTypeDef,
+        OwnershipControls: OwnershipControlsUnionTypeDef,
         ContentMD5: str = ...,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_ownership_controls)
@@ -1458,15 +1458,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_policy)
         """
 
     def put_bucket_replication(
         self,
         *,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationTypeDef,
+        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         Token: str = ...,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
@@ -1645,15 +1645,15 @@
         """
 
     def put_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
-        Retention: ObjectLockRetentionTypeDef = ...,
+        Retention: ObjectLockRetentionUnionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> PutObjectRetentionOutputTypeDef:
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/client.pyi` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
-    AnalyticsConfigurationTypeDef,
+    AnalyticsConfigurationUnionTypeDef,
     BlobTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
     CompleteMultipartUploadOutputTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
@@ -95,53 +95,53 @@
     GetObjectRetentionOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     GetObjectTorrentOutputTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     HeadBucketOutputTypeDef,
     HeadObjectOutputTypeDef,
     InputSerializationTypeDef,
-    IntelligentTieringConfigurationTypeDef,
-    InventoryConfigurationTypeDef,
+    IntelligentTieringConfigurationUnionTypeDef,
+    InventoryConfigurationUnionTypeDef,
     LifecycleConfigurationTypeDef,
     ListBucketAnalyticsConfigurationsOutputTypeDef,
     ListBucketIntelligentTieringConfigurationsOutputTypeDef,
     ListBucketInventoryConfigurationsOutputTypeDef,
     ListBucketMetricsConfigurationsOutputTypeDef,
     ListBucketsOutputTypeDef,
     ListDirectoryBucketsOutputTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListObjectsOutputTypeDef,
     ListObjectsV2OutputTypeDef,
     ListObjectVersionsOutputTypeDef,
     ListPartsOutputTypeDef,
-    MetricsConfigurationTypeDef,
+    MetricsConfigurationUnionTypeDef,
     NotificationConfigurationDeprecatedResponseTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     NotificationConfigurationResponseTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
-    ObjectLockRetentionTypeDef,
+    ObjectLockRetentionUnionTypeDef,
     OutputSerializationTypeDef,
-    OwnershipControlsTypeDef,
+    OwnershipControlsUnionTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectLegalHoldOutputTypeDef,
     PutObjectLockConfigurationOutputTypeDef,
     PutObjectOutputTypeDef,
     PutObjectRetentionOutputTypeDef,
     PutObjectTaggingOutputTypeDef,
-    ReplicationConfigurationTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
     SelectObjectContentOutputTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
+    ServerSideEncryptionConfigurationUnionTypeDef,
     TaggingTypeDef,
     TimestampTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
@@ -1260,15 +1260,15 @@
         """
 
     def put_bucket_analytics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        AnalyticsConfiguration: AnalyticsConfigurationTypeDef,
+        AnalyticsConfiguration: AnalyticsConfigurationUnionTypeDef,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_analytics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_analytics_configuration)
@@ -1289,15 +1289,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_cors)
         """
 
     def put_bucket_encryption(
         self,
         *,
         Bucket: str,
-        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
+        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationUnionTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
@@ -1306,29 +1306,29 @@
         """
 
     def put_bucket_intelligent_tiering_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef,
+        IntelligentTieringConfiguration: IntelligentTieringConfigurationUnionTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_intelligent_tiering_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_intelligent_tiering_configuration)
         """
 
     def put_bucket_inventory_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        InventoryConfiguration: InventoryConfigurationTypeDef,
+        InventoryConfiguration: InventoryConfigurationUnionTypeDef,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_inventory_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_inventory_configuration)
@@ -1380,15 +1380,15 @@
         """
 
     def put_bucket_metrics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        MetricsConfiguration: MetricsConfigurationTypeDef,
+        MetricsConfiguration: MetricsConfigurationUnionTypeDef,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_metrics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_metrics_configuration)
@@ -1424,15 +1424,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_notification_configuration)
         """
 
     def put_bucket_ownership_controls(
         self,
         *,
         Bucket: str,
-        OwnershipControls: OwnershipControlsTypeDef,
+        OwnershipControls: OwnershipControlsUnionTypeDef,
         ContentMD5: str = ...,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_ownership_controls)
@@ -1455,15 +1455,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_bucket_policy)
         """
 
     def put_bucket_replication(
         self,
         *,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationTypeDef,
+        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         Token: str = ...,
         ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
@@ -1642,15 +1642,15 @@
         """
 
     def put_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
-        Retention: ObjectLockRetentionTypeDef = ...,
+        Retention: ObjectLockRetentionUnionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> PutObjectRetentionOutputTypeDef:
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/literals.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -371,24 +372,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -585,14 +588,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/literals.pyi` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -371,24 +372,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -585,14 +588,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/paginator.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/paginator.pyi` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/service_resource.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,54 +63,54 @@
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccessControlPolicyTypeDef,
     BlobTypeDef,
-    BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef,
-    BucketLoggingStatusBucketLoggingTypeDef,
+    BucketLifecycleConfigurationTypeDef,
+    BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
     CopySourceTypeDef,
-    CORSConfigurationBucketCorsTypeDef,
-    CORSRuleBucketCorsTypeDef,
+    CORSConfigurationTypeDef,
+    CORSRuleExtraOutputTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketOutputTypeDef,
     DeleteObjectOutputTypeDef,
     DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseTypeDef,
     FileobjTypeDef,
     GetObjectOutputTypeDef,
     GrantTypeDef,
     HeadObjectOutputTypeDef,
     IndexDocumentResponseTypeDef,
     InitiatorResponseTypeDef,
-    LambdaFunctionConfigurationBucketNotificationTypeDef,
-    LifecycleConfigurationBucketLifecycleTypeDef,
-    LifecycleRuleBucketLifecycleConfigurationTypeDef,
+    LambdaFunctionConfigurationExtraOutputTypeDef,
+    LifecycleConfigurationTypeDef,
+    LifecycleRuleExtraOutputTypeDef,
     LoggingEnabledResponseTypeDef,
-    NotificationConfigurationBucketNotificationTypeDef,
+    NotificationConfigurationTypeDef,
     OwnerResponseTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectOutputTypeDef,
-    QueueConfigurationBucketNotificationTypeDef,
+    QueueConfigurationExtraOutputTypeDef,
     RedirectAllRequestsToResponseTypeDef,
     RequestPaymentConfigurationTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     RestoreStatusResponseTypeDef,
     RoutingRuleTypeDef,
-    RuleBucketLifecycleTypeDef,
+    RuleExtraOutputTypeDef,
     TaggingTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TopicConfigurationBucketNotificationTypeDef,
+    TopicConfigurationExtraOutputTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 12):
@@ -472,15 +472,15 @@
 
 class BucketCors(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcors)
     """
 
-    cors_rules: List[CORSRuleBucketCorsTypeDef]
+    cors_rules: List[CORSRuleExtraOutputTypeDef]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -513,15 +513,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcorsload-method)
         """
 
     def put(
         self,
         *,
-        CORSConfiguration: CORSConfigurationBucketCorsTypeDef,
+        CORSConfiguration: CORSConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.put)
@@ -544,15 +544,15 @@
 
 class BucketLifecycle(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycle)
     """
 
-    rules: List[RuleBucketLifecycleTypeDef]
+    rules: List[RuleExtraOutputTypeDef]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -586,15 +586,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleload-method)
         """
 
     def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: LifecycleConfigurationBucketLifecycleTypeDef = ...,
+        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleput-method)
@@ -616,15 +616,15 @@
 
 class BucketLifecycleConfiguration(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
-    rules: List[LifecycleRuleBucketLifecycleConfigurationTypeDef]
+    rules: List[LifecycleRuleExtraOutputTypeDef]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -658,15 +658,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfigurationload-method)
         """
 
     def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = ...,
+        LifecycleConfiguration: BucketLifecycleConfigurationTypeDef = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfigurationput-method)
@@ -721,15 +721,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketloggingload-method)
         """
 
     def put(
         self,
         *,
-        BucketLoggingStatus: BucketLoggingStatusBucketLoggingTypeDef,
+        BucketLoggingStatus: BucketLoggingStatusTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.put)
@@ -752,17 +752,17 @@
 
 class BucketNotification(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketnotification)
     """
 
-    topic_configurations: List[TopicConfigurationBucketNotificationTypeDef]
-    queue_configurations: List[QueueConfigurationBucketNotificationTypeDef]
-    lambda_function_configurations: List[LambdaFunctionConfigurationBucketNotificationTypeDef]
+    topic_configurations: List[TopicConfigurationExtraOutputTypeDef]
+    queue_configurations: List[QueueConfigurationExtraOutputTypeDef]
+    lambda_function_configurations: List[LambdaFunctionConfigurationExtraOutputTypeDef]
     event_bridge_configuration: Dict[str, Any]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
@@ -788,15 +788,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketnotificationload-method)
         """
 
     def put(
         self,
         *,
-        NotificationConfiguration: NotificationConfigurationBucketNotificationTypeDef,
+        NotificationConfiguration: NotificationConfigurationTypeDef,
         ExpectedBucketOwner: str = ...,
         SkipDestinationValidation: bool = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.put)
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/service_resource.pyi` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,54 +63,54 @@
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccessControlPolicyTypeDef,
     BlobTypeDef,
-    BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef,
-    BucketLoggingStatusBucketLoggingTypeDef,
+    BucketLifecycleConfigurationTypeDef,
+    BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
     CopySourceTypeDef,
-    CORSConfigurationBucketCorsTypeDef,
-    CORSRuleBucketCorsTypeDef,
+    CORSConfigurationTypeDef,
+    CORSRuleExtraOutputTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketOutputTypeDef,
     DeleteObjectOutputTypeDef,
     DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseTypeDef,
     FileobjTypeDef,
     GetObjectOutputTypeDef,
     GrantTypeDef,
     HeadObjectOutputTypeDef,
     IndexDocumentResponseTypeDef,
     InitiatorResponseTypeDef,
-    LambdaFunctionConfigurationBucketNotificationTypeDef,
-    LifecycleConfigurationBucketLifecycleTypeDef,
-    LifecycleRuleBucketLifecycleConfigurationTypeDef,
+    LambdaFunctionConfigurationExtraOutputTypeDef,
+    LifecycleConfigurationTypeDef,
+    LifecycleRuleExtraOutputTypeDef,
     LoggingEnabledResponseTypeDef,
-    NotificationConfigurationBucketNotificationTypeDef,
+    NotificationConfigurationTypeDef,
     OwnerResponseTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectOutputTypeDef,
-    QueueConfigurationBucketNotificationTypeDef,
+    QueueConfigurationExtraOutputTypeDef,
     RedirectAllRequestsToResponseTypeDef,
     RequestPaymentConfigurationTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     RestoreStatusResponseTypeDef,
     RoutingRuleTypeDef,
-    RuleBucketLifecycleTypeDef,
+    RuleExtraOutputTypeDef,
     TaggingTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TopicConfigurationBucketNotificationTypeDef,
+    TopicConfigurationExtraOutputTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 12):
@@ -464,15 +464,15 @@
 
 class BucketCors(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcors)
     """
 
-    cors_rules: List[CORSRuleBucketCorsTypeDef]
+    cors_rules: List[CORSRuleExtraOutputTypeDef]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -505,15 +505,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcorsload-method)
         """
 
     def put(
         self,
         *,
-        CORSConfiguration: CORSConfigurationBucketCorsTypeDef,
+        CORSConfiguration: CORSConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.put)
@@ -534,15 +534,15 @@
 
 class BucketLifecycle(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycle)
     """
 
-    rules: List[RuleBucketLifecycleTypeDef]
+    rules: List[RuleExtraOutputTypeDef]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -576,15 +576,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleload-method)
         """
 
     def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: LifecycleConfigurationBucketLifecycleTypeDef = ...,
+        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleput-method)
@@ -604,15 +604,15 @@
 
 class BucketLifecycleConfiguration(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
-    rules: List[LifecycleRuleBucketLifecycleConfigurationTypeDef]
+    rules: List[LifecycleRuleExtraOutputTypeDef]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -646,15 +646,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfigurationload-method)
         """
 
     def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = ...,
+        LifecycleConfiguration: BucketLifecycleConfigurationTypeDef = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfigurationput-method)
@@ -707,15 +707,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketloggingload-method)
         """
 
     def put(
         self,
         *,
-        BucketLoggingStatus: BucketLoggingStatusBucketLoggingTypeDef,
+        BucketLoggingStatus: BucketLoggingStatusTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.put)
@@ -736,17 +736,17 @@
 
 class BucketNotification(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketnotification)
     """
 
-    topic_configurations: List[TopicConfigurationBucketNotificationTypeDef]
-    queue_configurations: List[QueueConfigurationBucketNotificationTypeDef]
-    lambda_function_configurations: List[LambdaFunctionConfigurationBucketNotificationTypeDef]
+    topic_configurations: List[TopicConfigurationExtraOutputTypeDef]
+    queue_configurations: List[QueueConfigurationExtraOutputTypeDef]
+    lambda_function_configurations: List[LambdaFunctionConfigurationExtraOutputTypeDef]
     event_bridge_configuration: Dict[str, Any]
     bucket_name: str
     meta: "S3ResourceMeta"
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
@@ -772,15 +772,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketnotificationload-method)
         """
 
     def put(
         self,
         *,
-        NotificationConfiguration: NotificationConfigurationBucketNotificationTypeDef,
+        NotificationConfiguration: NotificationConfigurationTypeDef,
         ExpectedBucketOwner: str = ...,
         SkipDestinationValidation: bool = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.put)
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/type_defs.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,22 +99,24 @@
     "BlobTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "FileobjTypeDef",
     "BucketInfoTypeDef",
     "BucketTypeDef",
     "BucketUploadFileRequestTypeDef",
-    "CORSRuleBucketCorsTypeDef",
     "CORSRuleTypeDef",
+    "CORSRuleExtraOutputTypeDef",
+    "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "ChecksumTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
+    "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
     "CompletedPartTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "TimestampTypeDef",
     "CopyPartResultTypeDef",
@@ -183,15 +185,15 @@
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "ObjectLockRetentionTypeDef",
+    "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeTypeDef",
@@ -200,32 +202,37 @@
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
-    "LifecycleExpirationTypeDef",
+    "LifecycleExpirationExtraExtraOutputTypeDef",
+    "LifecycleExpirationExtraOutputTypeDef",
+    "LifecycleExpirationOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
-    "TransitionTypeDef",
+    "TransitionExtraOutputTypeDef",
+    "TransitionOutputTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListDirectoryBucketsRequestRequestTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueTypeDef",
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "OwnershipControlsRuleTypeDef",
     "PartitionedPrefixTypeDef",
@@ -236,14 +243,15 @@
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
     "RecordsEventTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
+    "TransitionExtraExtraOutputTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StatsTypeDef",
     "AbortMultipartUploadOutputTypeDef",
     "CompleteMultipartUploadOutputTypeDef",
     "CreateBucketOutputTypeDef",
@@ -272,21 +280,26 @@
     "PutObjectTaggingOutputTypeDef",
     "RedirectAllRequestsToResponseTypeDef",
     "RestoreObjectOutputTypeDef",
     "RestoreStatusResponseTypeDef",
     "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "DeleteMarkerEntryTypeDef",
+    "AnalyticsAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
+    "IntelligentTieringAndOperatorOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
-    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
+    "LifecycleRuleAndOperatorExtraOutputTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
+    "MetricsAndOperatorOutputTypeDef",
     "MetricsAndOperatorTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "TaggingTypeDef",
     "AnalyticsExportDestinationTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
@@ -296,15 +309,14 @@
     "BucketUploadFileobjRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
     "ListBucketsOutputTypeDef",
     "ListDirectoryBucketsOutputTypeDef",
-    "CORSConfigurationBucketCorsTypeDef",
     "CORSConfigurationTypeDef",
     "GetBucketCorsOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
     "CopyObjectOutputTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
@@ -312,190 +324,217 @@
     "CreateMultipartUploadRequestRequestTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
-    "LifecycleExpirationBucketLifecycleTypeDef",
+    "LifecycleExpirationTypeDef",
+    "ObjectLockRetentionTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "TransitionBucketLifecycleConfigurationTypeDef",
-    "TransitionBucketLifecycleTypeDef",
+    "TransitionTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "UploadPartCopyOutputTypeDef",
     "CreateBucketConfigurationTypeDef",
     "CreateSessionOutputTypeDef",
     "ObjectLockRuleTypeDef",
     "DeleteObjectsOutputTypeDef",
     "DeleteTypeDef",
-    "S3KeyFilterBucketNotificationTypeDef",
+    "S3KeyFilterExtraOutputTypeDef",
+    "S3KeyFilterOutputTypeDef",
     "S3KeyFilterTypeDef",
     "GetBucketPolicyStatusOutputTypeDef",
     "GetObjectAttributesPartsTypeDef",
     "GetObjectLegalHoldOutputTypeDef",
     "PutObjectLegalHoldRequestRequestTypeDef",
     "GetObjectRetentionOutputTypeDef",
-    "PutObjectRetentionRequestRequestTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
     "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
+    "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
-    "RuleTypeDef",
+    "RuleOutputTypeDef",
     "ListDirectoryBucketsRequestListDirectoryBucketsPaginateTypeDef",
     "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
     "ObjectTypeDef",
     "ObjectVersionTypeDef",
+    "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
-    "TargetObjectKeyFormatBucketLoggingTypeDef",
+    "TargetObjectKeyFormatExtraOutputTypeDef",
+    "TargetObjectKeyFormatOutputTypeDef",
     "TargetObjectKeyFormatTypeDef",
     "ProgressEventTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "RoutingRuleTypeDef",
+    "RuleExtraOutputTypeDef",
     "ServerSideEncryptionRuleTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "StatsEventTypeDef",
+    "AnalyticsFilterOutputTypeDef",
     "AnalyticsFilterTypeDef",
+    "IntelligentTieringFilterOutputTypeDef",
     "IntelligentTieringFilterTypeDef",
-    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
+    "LifecycleRuleFilterExtraOutputTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
+    "MetricsFilterOutputTypeDef",
     "MetricsFilterTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestBucketTaggingPutTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "PutObjectTaggingRequestRequestTypeDef",
     "StorageClassAnalysisDataExportTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     "PutBucketCorsRequestRequestTypeDef",
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadRequestRequestTypeDef",
-    "RuleBucketLifecycleTypeDef",
+    "ObjectLockRetentionUnionTypeDef",
+    "PutObjectRetentionRequestRequestTypeDef",
+    "RuleTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
-    "NotificationConfigurationFilterBucketNotificationTypeDef",
+    "NotificationConfigurationFilterExtraOutputTypeDef",
+    "NotificationConfigurationFilterOutputTypeDef",
     "NotificationConfigurationFilterTypeDef",
     "GetObjectAttributesOutputTypeDef",
     "AccessControlPolicyTypeDef",
     "GetBucketAclOutputTypeDef",
     "GetObjectAclOutputTypeDef",
     "S3LocationTypeDef",
     "ListMultipartUploadsOutputTypeDef",
+    "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
     "GetBucketLifecycleOutputTypeDef",
-    "LifecycleConfigurationTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
     "ListObjectsOutputTypeDef",
     "ListObjectsV2OutputTypeDef",
     "ListObjectVersionsOutputTypeDef",
     "GetBucketOwnershipControlsOutputTypeDef",
+    "OwnershipControlsUnionTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
-    "LoggingEnabledBucketLoggingTypeDef",
     "LoggingEnabledResponseTypeDef",
+    "LoggingEnabledOutputTypeDef",
     "LoggingEnabledTypeDef",
     "GetBucketWebsiteOutputTypeDef",
     "WebsiteConfigurationTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "SelectObjectContentEventStreamTypeDef",
+    "IntelligentTieringConfigurationOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
-    "LifecycleRuleBucketLifecycleConfigurationTypeDef",
+    "LifecycleRuleExtraOutputTypeDef",
+    "LifecycleRuleOutputTypeDef",
     "LifecycleRuleTypeDef",
+    "MetricsConfigurationOutputTypeDef",
     "MetricsConfigurationTypeDef",
     "StorageClassAnalysisTypeDef",
-    "LifecycleConfigurationBucketLifecycleTypeDef",
+    "LifecycleConfigurationTypeDef",
     "GetObjectLockConfigurationOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
-    "LambdaFunctionConfigurationBucketNotificationTypeDef",
-    "QueueConfigurationBucketNotificationTypeDef",
-    "TopicConfigurationBucketNotificationTypeDef",
+    "LambdaFunctionConfigurationExtraOutputTypeDef",
+    "QueueConfigurationExtraOutputTypeDef",
+    "TopicConfigurationExtraOutputTypeDef",
+    "LambdaFunctionConfigurationOutputTypeDef",
+    "QueueConfigurationOutputTypeDef",
+    "TopicConfigurationOutputTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
+    "InventoryDestinationOutputTypeDef",
     "InventoryDestinationTypeDef",
-    "PutBucketLifecycleRequestRequestTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
-    "BucketLoggingStatusBucketLoggingTypeDef",
-    "BucketLoggingStatusTypeDef",
     "GetBucketLoggingOutputTypeDef",
+    "BucketLoggingStatusTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
     "GetBucketEncryptionOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
+    "ServerSideEncryptionConfigurationUnionTypeDef",
     "SelectObjectContentOutputTypeDef",
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+    "IntelligentTieringConfigurationUnionTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
-    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
-    "BucketLifecycleConfigurationTypeDef",
     "GetBucketLifecycleConfigurationOutputTypeDef",
+    "BucketLifecycleConfigurationTypeDef",
     "GetBucketMetricsConfigurationOutputTypeDef",
     "ListBucketMetricsConfigurationsOutputTypeDef",
+    "MetricsConfigurationUnionTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
+    "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
-    "NotificationConfigurationBucketNotificationTypeDef",
+    "PutBucketLifecycleRequestRequestTypeDef",
     "NotificationConfigurationResponseTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
+    "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
+    "AnalyticsConfigurationUnionTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
     "GetBucketInventoryConfigurationOutputTypeDef",
     "ListBucketInventoryConfigurationsOutputTypeDef",
+    "InventoryConfigurationUnionTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketReplicationOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": NotRequired[int],
     },
@@ -602,27 +641,38 @@
         "Filename": str,
         "Key": str,
         "ExtraArgs": NotRequired[Optional[Dict[str, Any]]],
         "Callback": NotRequired[Optional[Callable[..., Any]]],
         "Config": NotRequired[Optional[TransferConfig]],
     },
 )
-CORSRuleBucketCorsTypeDef = TypedDict(
-    "CORSRuleBucketCorsTypeDef",
+CORSRuleTypeDef = TypedDict(
+    "CORSRuleTypeDef",
     {
         "AllowedMethods": Sequence[str],
         "AllowedOrigins": Sequence[str],
         "ID": NotRequired[str],
         "AllowedHeaders": NotRequired[Sequence[str]],
         "ExposeHeaders": NotRequired[Sequence[str]],
         "MaxAgeSeconds": NotRequired[int],
     },
 )
-CORSRuleTypeDef = TypedDict(
-    "CORSRuleTypeDef",
+CORSRuleExtraOutputTypeDef = TypedDict(
+    "CORSRuleExtraOutputTypeDef",
+    {
+        "AllowedMethods": List[str],
+        "AllowedOrigins": List[str],
+        "ID": NotRequired[str],
+        "AllowedHeaders": NotRequired[List[str]],
+        "ExposeHeaders": NotRequired[List[str]],
+        "MaxAgeSeconds": NotRequired[int],
+    },
+)
+CORSRuleOutputTypeDef = TypedDict(
+    "CORSRuleOutputTypeDef",
     {
         "AllowedMethods": List[str],
         "AllowedOrigins": List[str],
         "ID": NotRequired[str],
         "AllowedHeaders": NotRequired[List[str]],
         "ExposeHeaders": NotRequired[List[str]],
         "MaxAgeSeconds": NotRequired[int],
@@ -687,20 +737,30 @@
         "Bucket": str,
         "Key": str,
         "ExtraArgs": NotRequired[Optional[Dict[str, Any]]],
         "Callback": NotRequired[Optional[Callable[..., Any]]],
         "Config": NotRequired[Optional[TransferConfig]],
     },
 )
+CloudFunctionConfigurationOutputTypeDef = TypedDict(
+    "CloudFunctionConfigurationOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Event": NotRequired[EventType],
+        "Events": NotRequired[List[EventType]],
+        "CloudFunction": NotRequired[str],
+        "InvocationRole": NotRequired[str],
+    },
+)
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": NotRequired[str],
         "Event": NotRequired[EventType],
-        "Events": NotRequired[List[EventType]],
+        "Events": NotRequired[Sequence[EventType]],
         "CloudFunction": NotRequired[str],
         "InvocationRole": NotRequired[str],
     },
 )
 CommonPrefixTypeDef = TypedDict(
     "CommonPrefixTypeDef",
     {
@@ -1262,16 +1322,16 @@
 GetObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "GetObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-ObjectLockRetentionTypeDef = TypedDict(
-    "ObjectLockRetentionTypeDef",
+ObjectLockRetentionOutputTypeDef = TypedDict(
+    "ObjectLockRetentionOutputTypeDef",
     {
         "Mode": NotRequired[ObjectLockRetentionModeType],
         "RetainUntilDate": NotRequired[datetime],
     },
 )
 GetObjectRetentionRequestRequestTypeDef = TypedDict(
     "GetObjectRetentionRequestRequestTypeDef",
@@ -1388,16 +1448,32 @@
 )
 JSONOutputTypeDef = TypedDict(
     "JSONOutputTypeDef",
     {
         "RecordDelimiter": NotRequired[str],
     },
 )
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
+LifecycleExpirationExtraExtraOutputTypeDef = TypedDict(
+    "LifecycleExpirationExtraExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "ExpiredObjectDeleteMarker": NotRequired[bool],
+    },
+)
+LifecycleExpirationExtraOutputTypeDef = TypedDict(
+    "LifecycleExpirationExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "ExpiredObjectDeleteMarker": NotRequired[bool],
+    },
+)
+LifecycleExpirationOutputTypeDef = TypedDict(
+    "LifecycleExpirationOutputTypeDef",
     {
         "Date": NotRequired[datetime],
         "Days": NotRequired[int],
         "ExpiredObjectDeleteMarker": NotRequired[bool],
     },
 )
 NoncurrentVersionExpirationTypeDef = TypedDict(
@@ -1411,16 +1487,24 @@
     "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": NotRequired[int],
         "StorageClass": NotRequired[TransitionStorageClassType],
         "NewerNoncurrentVersions": NotRequired[int],
     },
 )
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
+TransitionExtraOutputTypeDef = TypedDict(
+    "TransitionExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "StorageClass": NotRequired[TransitionStorageClassType],
+    },
+)
+TransitionOutputTypeDef = TypedDict(
+    "TransitionOutputTypeDef",
     {
         "Date": NotRequired[datetime],
         "Days": NotRequired[int],
         "StorageClass": NotRequired[TransitionStorageClassType],
     },
 )
 ListBucketAnalyticsConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1565,28 +1649,46 @@
 )
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": NotRequired[int],
     },
 )
+QueueConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Event": NotRequired[EventType],
+        "Events": NotRequired[List[EventType]],
+        "Queue": NotRequired[str],
+    },
+)
+TopicConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "TopicConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Events": NotRequired[List[EventType]],
+        "Event": NotRequired[EventType],
+        "Topic": NotRequired[str],
+    },
+)
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": NotRequired[str],
         "Event": NotRequired[EventType],
-        "Events": NotRequired[List[EventType]],
+        "Events": NotRequired[Sequence[EventType]],
         "Queue": NotRequired[str],
     },
 )
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": NotRequired[str],
-        "Events": NotRequired[List[EventType]],
+        "Events": NotRequired[Sequence[EventType]],
         "Event": NotRequired[EventType],
         "Topic": NotRequired[str],
     },
 )
 ObjectDownloadFileRequestTypeDef = TypedDict(
     "ObjectDownloadFileRequestTypeDef",
     {
@@ -1704,14 +1806,22 @@
 )
 RequestProgressTypeDef = TypedDict(
     "RequestProgressTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
+TransitionExtraExtraOutputTypeDef = TypedDict(
+    "TransitionExtraExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "StorageClass": NotRequired[TransitionStorageClassType],
+    },
+)
 ScanRangeTypeDef = TypedDict(
     "ScanRangeTypeDef",
     {
         "Start": NotRequired[int],
         "End": NotRequired[int],
     },
 )
@@ -2089,19 +2199,26 @@
         "Owner": NotRequired[OwnerTypeDef],
         "Key": NotRequired[str],
         "VersionId": NotRequired[str],
         "IsLatest": NotRequired[bool],
         "LastModified": NotRequired[datetime],
     },
 )
+AnalyticsAndOperatorOutputTypeDef = TypedDict(
+    "AnalyticsAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 AnalyticsAndOperatorTypeDef = TypedDict(
     "AnalyticsAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2111,52 +2228,83 @@
     "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
+    "IntelligentTieringAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+LifecycleRuleAndOperatorExtraOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorExtraOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
+        "ObjectSizeGreaterThan": NotRequired[int],
+        "ObjectSizeLessThan": NotRequired[int],
     },
 )
-LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "Tags": NotRequired[List[TagTypeDef]],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
     },
 )
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
     },
 )
+MetricsAndOperatorOutputTypeDef = TypedDict(
+    "MetricsAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+        "AccessPointArn": NotRequired[str],
+    },
+)
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
         "AccessPointArn": NotRequired[str],
     },
 )
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[TagTypeDef],
     },
@@ -2313,30 +2461,24 @@
     "ListDirectoryBucketsOutputTypeDef",
     {
         "Buckets": List[BucketTypeDef],
         "ContinuationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CORSConfigurationBucketCorsTypeDef = TypedDict(
-    "CORSConfigurationBucketCorsTypeDef",
-    {
-        "CORSRules": Sequence[CORSRuleBucketCorsTypeDef],
-    },
-)
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
-        "CORSRules": List[CORSRuleTypeDef],
+        "CORSRules": List[CORSRuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": NotRequired[Sequence[CompletedPartTypeDef]],
@@ -2678,28 +2820,27 @@
         "SSECustomerKeyMD5": NotRequired[str],
         "RequestPayer": NotRequired[Literal["requester"]],
         "PartNumber": NotRequired[int],
         "ExpectedBucketOwner": NotRequired[str],
         "ChecksumMode": NotRequired[Literal["ENABLED"]],
     },
 )
-LifecycleExpirationBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
+LifecycleExpirationTypeDef = TypedDict(
+    "LifecycleExpirationTypeDef",
     {
         "Date": NotRequired[TimestampTypeDef],
         "Days": NotRequired[int],
         "ExpiredObjectDeleteMarker": NotRequired[bool],
     },
 )
-LifecycleExpirationBucketLifecycleTypeDef = TypedDict(
-    "LifecycleExpirationBucketLifecycleTypeDef",
+ObjectLockRetentionTypeDef = TypedDict(
+    "ObjectLockRetentionTypeDef",
     {
-        "Date": NotRequired[TimestampTypeDef],
-        "Days": NotRequired[int],
-        "ExpiredObjectDeleteMarker": NotRequired[bool],
+        "Mode": NotRequired[ObjectLockRetentionModeType],
+        "RetainUntilDate": NotRequired[TimestampTypeDef],
     },
 )
 PutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "PutObjectRequestBucketPutObjectTypeDef",
     {
         "Key": str,
         "ACL": NotRequired[ObjectCannedACLType],
@@ -2857,24 +2998,16 @@
         "Tagging": NotRequired[str],
         "ObjectLockMode": NotRequired[ObjectLockModeType],
         "ObjectLockRetainUntilDate": NotRequired[TimestampTypeDef],
         "ObjectLockLegalHoldStatus": NotRequired[ObjectLockLegalHoldStatusType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-TransitionBucketLifecycleConfigurationTypeDef = TypedDict(
-    "TransitionBucketLifecycleConfigurationTypeDef",
-    {
-        "Date": NotRequired[TimestampTypeDef],
-        "Days": NotRequired[int],
-        "StorageClass": NotRequired[TransitionStorageClassType],
-    },
-)
-TransitionBucketLifecycleTypeDef = TypedDict(
-    "TransitionBucketLifecycleTypeDef",
+TransitionTypeDef = TypedDict(
+    "TransitionTypeDef",
     {
         "Date": NotRequired[TimestampTypeDef],
         "Days": NotRequired[int],
         "StorageClass": NotRequired[TransitionStorageClassType],
     },
 )
 WriteGetObjectResponseRequestRequestTypeDef = TypedDict(
@@ -2969,24 +3102,30 @@
 DeleteTypeDef = TypedDict(
     "DeleteTypeDef",
     {
         "Objects": Sequence[ObjectIdentifierTypeDef],
         "Quiet": NotRequired[bool],
     },
 )
-S3KeyFilterBucketNotificationTypeDef = TypedDict(
-    "S3KeyFilterBucketNotificationTypeDef",
+S3KeyFilterExtraOutputTypeDef = TypedDict(
+    "S3KeyFilterExtraOutputTypeDef",
     {
-        "FilterRules": NotRequired[Sequence[FilterRuleTypeDef]],
+        "FilterRules": NotRequired[List[FilterRuleTypeDef]],
+    },
+)
+S3KeyFilterOutputTypeDef = TypedDict(
+    "S3KeyFilterOutputTypeDef",
+    {
+        "FilterRules": NotRequired[List[FilterRuleTypeDef]],
     },
 )
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
-        "FilterRules": NotRequired[List[FilterRuleTypeDef]],
+        "FilterRules": NotRequired[Sequence[FilterRuleTypeDef]],
     },
 )
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3022,32 +3161,18 @@
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionTypeDef,
+        "Retention": ObjectLockRetentionOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "PutObjectRetentionRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-        "Retention": NotRequired[ObjectLockRetentionTypeDef],
-        "RequestPayer": NotRequired[Literal["requester"]],
-        "VersionId": NotRequired[str],
-        "BypassGovernanceRetention": NotRequired[bool],
-        "ContentMD5": NotRequired[str],
-        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "ExpectedBucketOwner": NotRequired[str],
-    },
-)
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3150,36 +3275,43 @@
     {
         "CSV": NotRequired[CSVInputTypeDef],
         "CompressionType": NotRequired[CompressionTypeType],
         "JSON": NotRequired[JSONInputTypeDef],
         "Parquet": NotRequired[Mapping[str, Any]],
     },
 )
+InventoryEncryptionOutputTypeDef = TypedDict(
+    "InventoryEncryptionOutputTypeDef",
+    {
+        "SSES3": NotRequired[Dict[str, Any]],
+        "SSEKMS": NotRequired[SSEKMSTypeDef],
+    },
+)
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
-        "SSES3": NotRequired[Dict[str, Any]],
+        "SSES3": NotRequired[Mapping[str, Any]],
         "SSEKMS": NotRequired[SSEKMSTypeDef],
     },
 )
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": NotRequired[CSVOutputTypeDef],
         "JSON": NotRequired[JSONOutputTypeDef],
     },
 )
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
-        "Expiration": NotRequired[LifecycleExpirationTypeDef],
+        "Expiration": NotRequired[LifecycleExpirationOutputTypeDef],
         "ID": NotRequired[str],
-        "Transition": NotRequired[TransitionTypeDef],
+        "Transition": NotRequired[TransitionOutputTypeDef],
         "NoncurrentVersionTransition": NotRequired[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
 ListDirectoryBucketsRequestListDirectoryBucketsPaginateTypeDef = TypedDict(
     "ListDirectoryBucketsRequestListDirectoryBucketsPaginateTypeDef",
@@ -3288,17 +3420,17 @@
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 NotificationConfigurationDeprecatedResponseTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseTypeDef",
     {
-        "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
-        "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
-        "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
+        "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
+        "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
+        "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": NotRequired[TopicConfigurationDeprecatedTypeDef],
@@ -3330,31 +3462,44 @@
         "VersionId": NotRequired[str],
         "IsLatest": NotRequired[bool],
         "LastModified": NotRequired[datetime],
         "Owner": NotRequired[OwnerTypeDef],
         "RestoreStatus": NotRequired[RestoreStatusTypeDef],
     },
 )
+OwnershipControlsOutputTypeDef = TypedDict(
+    "OwnershipControlsOutputTypeDef",
+    {
+        "Rules": List[OwnershipControlsRuleTypeDef],
+    },
+)
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
-        "Rules": List[OwnershipControlsRuleTypeDef],
+        "Rules": Sequence[OwnershipControlsRuleTypeDef],
     },
 )
-TargetObjectKeyFormatBucketLoggingTypeDef = TypedDict(
-    "TargetObjectKeyFormatBucketLoggingTypeDef",
+TargetObjectKeyFormatExtraOutputTypeDef = TypedDict(
+    "TargetObjectKeyFormatExtraOutputTypeDef",
     {
-        "SimplePrefix": NotRequired[Mapping[str, Any]],
+        "SimplePrefix": NotRequired[Dict[str, Any]],
+        "PartitionedPrefix": NotRequired[PartitionedPrefixTypeDef],
+    },
+)
+TargetObjectKeyFormatOutputTypeDef = TypedDict(
+    "TargetObjectKeyFormatOutputTypeDef",
+    {
+        "SimplePrefix": NotRequired[Dict[str, Any]],
         "PartitionedPrefix": NotRequired[PartitionedPrefixTypeDef],
     },
 )
 TargetObjectKeyFormatTypeDef = TypedDict(
     "TargetObjectKeyFormatTypeDef",
     {
-        "SimplePrefix": NotRequired[Dict[str, Any]],
+        "SimplePrefix": NotRequired[Mapping[str, Any]],
         "PartitionedPrefix": NotRequired[PartitionedPrefixTypeDef],
     },
 )
 ProgressEventTypeDef = TypedDict(
     "ProgressEventTypeDef",
     {
         "Details": NotRequired[ProgressTypeDef],
@@ -3399,14 +3544,27 @@
 RoutingRuleTypeDef = TypedDict(
     "RoutingRuleTypeDef",
     {
         "Redirect": RedirectTypeDef,
         "Condition": NotRequired[ConditionTypeDef],
     },
 )
+RuleExtraOutputTypeDef = TypedDict(
+    "RuleExtraOutputTypeDef",
+    {
+        "Prefix": str,
+        "Status": ExpirationStatusType,
+        "Expiration": NotRequired[LifecycleExpirationExtraExtraOutputTypeDef],
+        "ID": NotRequired[str],
+        "Transition": NotRequired[TransitionExtraExtraOutputTypeDef],
+        "NoncurrentVersionTransition": NotRequired[NoncurrentVersionTransitionTypeDef],
+        "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
+        "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
+    },
+)
 ServerSideEncryptionRuleTypeDef = TypedDict(
     "ServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": NotRequired[ServerSideEncryptionByDefaultTypeDef],
         "BucketKeyEnabled": NotRequired[bool],
     },
 )
@@ -3419,59 +3577,102 @@
 )
 StatsEventTypeDef = TypedDict(
     "StatsEventTypeDef",
     {
         "Details": NotRequired[StatsTypeDef],
     },
 )
+AnalyticsFilterOutputTypeDef = TypedDict(
+    "AnalyticsFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "And": NotRequired[AnalyticsAndOperatorOutputTypeDef],
+    },
+)
 AnalyticsFilterTypeDef = TypedDict(
     "AnalyticsFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "And": NotRequired[AnalyticsAndOperatorTypeDef],
     },
 )
+IntelligentTieringFilterOutputTypeDef = TypedDict(
+    "IntelligentTieringFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "And": NotRequired[IntelligentTieringAndOperatorOutputTypeDef],
+    },
+)
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "And": NotRequired[IntelligentTieringAndOperatorTypeDef],
     },
 )
-LifecycleRuleFilterBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
+LifecycleRuleFilterExtraOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterExtraOutputTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
-        "And": NotRequired[LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef],
+        "And": NotRequired[LifecycleRuleAndOperatorExtraOutputTypeDef],
+    },
+)
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "ObjectSizeGreaterThan": NotRequired[int],
+        "ObjectSizeLessThan": NotRequired[int],
+        "And": NotRequired[LifecycleRuleAndOperatorOutputTypeDef],
     },
 )
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
         "And": NotRequired[LifecycleRuleAndOperatorTypeDef],
     },
 )
+MetricsFilterOutputTypeDef = TypedDict(
+    "MetricsFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "AccessPointArn": NotRequired[str],
+        "And": NotRequired[MetricsAndOperatorOutputTypeDef],
+    },
+)
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "AccessPointArn": NotRequired[str],
         "And": NotRequired[MetricsAndOperatorTypeDef],
     },
 )
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "And": NotRequired[ReplicationRuleAndOperatorOutputTypeDef],
+    },
+)
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "And": NotRequired[ReplicationRuleAndOperatorTypeDef],
     },
@@ -3602,15 +3803,15 @@
         "ExpectedBucketOwner": NotRequired[str],
         "ExpectedSourceBucketOwner": NotRequired[str],
     },
 )
 PutBucketCorsRequestBucketCorsPutTypeDef = TypedDict(
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     {
-        "CORSConfiguration": CORSConfigurationBucketCorsTypeDef,
+        "CORSConfiguration": CORSConfigurationTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketCorsRequestRequestTypeDef = TypedDict(
     "PutBucketCorsRequestRequestTypeDef",
     {
@@ -3649,22 +3850,39 @@
         "RequestPayer": NotRequired[Literal["requester"]],
         "ExpectedBucketOwner": NotRequired[str],
         "SSECustomerAlgorithm": NotRequired[str],
         "SSECustomerKey": NotRequired[str],
         "SSECustomerKeyMD5": NotRequired[str],
     },
 )
-RuleBucketLifecycleTypeDef = TypedDict(
-    "RuleBucketLifecycleTypeDef",
+ObjectLockRetentionUnionTypeDef = Union[
+    ObjectLockRetentionTypeDef, ObjectLockRetentionOutputTypeDef
+]
+PutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "PutObjectRetentionRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "Retention": NotRequired[ObjectLockRetentionTypeDef],
+        "RequestPayer": NotRequired[Literal["requester"]],
+        "VersionId": NotRequired[str],
+        "BypassGovernanceRetention": NotRequired[bool],
+        "ContentMD5": NotRequired[str],
+        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
+        "ExpectedBucketOwner": NotRequired[str],
+    },
+)
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
-        "Expiration": NotRequired[LifecycleExpirationBucketLifecycleTypeDef],
+        "Expiration": NotRequired[LifecycleExpirationTypeDef],
         "ID": NotRequired[str],
-        "Transition": NotRequired[TransitionBucketLifecycleTypeDef],
+        "Transition": NotRequired[TransitionTypeDef],
         "NoncurrentVersionTransition": NotRequired[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
 CreateBucketRequestBucketCreateTypeDef = TypedDict(
     "CreateBucketRequestBucketCreateTypeDef",
@@ -3736,18 +3954,24 @@
         "MFA": NotRequired[str],
         "RequestPayer": NotRequired[Literal["requester"]],
         "BypassGovernanceRetention": NotRequired[bool],
         "ExpectedBucketOwner": NotRequired[str],
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
     },
 )
-NotificationConfigurationFilterBucketNotificationTypeDef = TypedDict(
-    "NotificationConfigurationFilterBucketNotificationTypeDef",
+NotificationConfigurationFilterExtraOutputTypeDef = TypedDict(
+    "NotificationConfigurationFilterExtraOutputTypeDef",
+    {
+        "Key": NotRequired[S3KeyFilterExtraOutputTypeDef],
+    },
+)
+NotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "NotificationConfigurationFilterOutputTypeDef",
     {
-        "Key": NotRequired[S3KeyFilterBucketNotificationTypeDef],
+        "Key": NotRequired[S3KeyFilterOutputTypeDef],
     },
 )
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": NotRequired[S3KeyFilterTypeDef],
     },
@@ -3813,18 +4037,28 @@
         "NextKeyMarker": str,
         "Prefix": str,
         "Delimiter": str,
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
         "Uploads": List[MultipartUploadTypeDef],
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
+    },
+)
+InventoryS3BucketDestinationOutputTypeDef = TypedDict(
+    "InventoryS3BucketDestinationOutputTypeDef",
+    {
+        "Bucket": str,
+        "Format": InventoryFormatType,
+        "AccountId": NotRequired[str],
+        "Prefix": NotRequired[str],
+        "Encryption": NotRequired[InventoryEncryptionOutputTypeDef],
     },
 )
 InventoryS3BucketDestinationTypeDef = TypedDict(
     "InventoryS3BucketDestinationTypeDef",
     {
         "Bucket": str,
         "Format": InventoryFormatType,
@@ -3858,24 +4092,18 @@
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-LifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleConfigurationTypeDef",
-    {
-        "Rules": Sequence[RuleTypeDef],
-    },
-)
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "Bucket": str,
         "Account": NotRequired[str],
         "StorageClass": NotRequired[StorageClassType],
         "AccessControlTranslation": NotRequired[AccessControlTranslationTypeDef],
@@ -3895,42 +4123,42 @@
 )
 ListObjectsOutputTypeDef = TypedDict(
     "ListObjectsOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
-        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "Contents": NotRequired[List[ObjectTypeDef]],
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
     },
 )
 ListObjectsV2OutputTypeDef = TypedDict(
     "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
-        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "Contents": NotRequired[List[ObjectTypeDef]],
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
     },
 )
 ListObjectVersionsOutputTypeDef = TypedDict(
     "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
         "KeyMarker": str,
@@ -3939,61 +4167,62 @@
         "NextVersionIdMarker": str,
         "Versions": List[ObjectVersionTypeDef],
         "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
     },
 )
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
-        "OwnershipControls": OwnershipControlsTypeDef,
+        "OwnershipControls": OwnershipControlsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+OwnershipControlsUnionTypeDef = Union[OwnershipControlsTypeDef, OwnershipControlsOutputTypeDef]
 PutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "PutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
         "OwnershipControls": OwnershipControlsTypeDef,
         "ContentMD5": NotRequired[str],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-LoggingEnabledBucketLoggingTypeDef = TypedDict(
-    "LoggingEnabledBucketLoggingTypeDef",
+LoggingEnabledResponseTypeDef = TypedDict(
+    "LoggingEnabledResponseTypeDef",
     {
         "TargetBucket": str,
+        "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "TargetGrants": NotRequired[Sequence[TargetGrantTypeDef]],
-        "TargetObjectKeyFormat": NotRequired[TargetObjectKeyFormatBucketLoggingTypeDef],
+        "TargetObjectKeyFormat": TargetObjectKeyFormatExtraOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-LoggingEnabledResponseTypeDef = TypedDict(
-    "LoggingEnabledResponseTypeDef",
+LoggingEnabledOutputTypeDef = TypedDict(
+    "LoggingEnabledOutputTypeDef",
     {
         "TargetBucket": str,
-        "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "TargetObjectKeyFormat": TargetObjectKeyFormatBucketLoggingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TargetGrants": NotRequired[List[TargetGrantTypeDef]],
+        "TargetObjectKeyFormat": NotRequired[TargetObjectKeyFormatOutputTypeDef],
     },
 )
 LoggingEnabledTypeDef = TypedDict(
     "LoggingEnabledTypeDef",
     {
         "TargetBucket": str,
         "TargetPrefix": str,
-        "TargetGrants": NotRequired[List[TargetGrantTypeDef]],
+        "TargetGrants": NotRequired[Sequence[TargetGrantTypeDef]],
         "TargetObjectKeyFormat": NotRequired[TargetObjectKeyFormatTypeDef],
     },
 )
 GetBucketWebsiteOutputTypeDef = TypedDict(
     "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
@@ -4008,84 +4237,120 @@
     {
         "ErrorDocument": NotRequired[ErrorDocumentTypeDef],
         "IndexDocument": NotRequired[IndexDocumentTypeDef],
         "RedirectAllRequestsTo": NotRequired[RedirectAllRequestsToTypeDef],
         "RoutingRules": NotRequired[Sequence[RoutingRuleTypeDef]],
     },
 )
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "Rules": List[ServerSideEncryptionRuleTypeDef],
+    },
+)
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
-        "Rules": List[ServerSideEncryptionRuleTypeDef],
+        "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
     },
 )
 SelectObjectContentEventStreamTypeDef = TypedDict(
     "SelectObjectContentEventStreamTypeDef",
     {
         "Records": NotRequired[RecordsEventTypeDef],
         "Stats": NotRequired[StatsEventTypeDef],
         "Progress": NotRequired[ProgressEventTypeDef],
         "Cont": NotRequired[Dict[str, Any]],
         "End": NotRequired[Dict[str, Any]],
     },
 )
+IntelligentTieringConfigurationOutputTypeDef = TypedDict(
+    "IntelligentTieringConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Status": IntelligentTieringStatusType,
+        "Tierings": List[TieringTypeDef],
+        "Filter": NotRequired[IntelligentTieringFilterOutputTypeDef],
+    },
+)
 IntelligentTieringConfigurationTypeDef = TypedDict(
     "IntelligentTieringConfigurationTypeDef",
     {
         "Id": str,
         "Status": IntelligentTieringStatusType,
-        "Tierings": List[TieringTypeDef],
+        "Tierings": Sequence[TieringTypeDef],
         "Filter": NotRequired[IntelligentTieringFilterTypeDef],
     },
 )
-LifecycleRuleBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleRuleBucketLifecycleConfigurationTypeDef",
+LifecycleRuleExtraOutputTypeDef = TypedDict(
+    "LifecycleRuleExtraOutputTypeDef",
     {
         "Status": ExpirationStatusType,
-        "Expiration": NotRequired[LifecycleExpirationBucketLifecycleConfigurationTypeDef],
+        "Expiration": NotRequired[LifecycleExpirationExtraOutputTypeDef],
         "ID": NotRequired[str],
         "Prefix": NotRequired[str],
-        "Filter": NotRequired[LifecycleRuleFilterBucketLifecycleConfigurationTypeDef],
-        "Transitions": NotRequired[Sequence[TransitionBucketLifecycleConfigurationTypeDef]],
-        "NoncurrentVersionTransitions": NotRequired[Sequence[NoncurrentVersionTransitionTypeDef]],
+        "Filter": NotRequired[LifecycleRuleFilterExtraOutputTypeDef],
+        "Transitions": NotRequired[List[TransitionExtraOutputTypeDef]],
+        "NoncurrentVersionTransitions": NotRequired[List[NoncurrentVersionTransitionTypeDef]],
+        "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
+        "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
+    },
+)
+LifecycleRuleOutputTypeDef = TypedDict(
+    "LifecycleRuleOutputTypeDef",
+    {
+        "Status": ExpirationStatusType,
+        "Expiration": NotRequired[LifecycleExpirationOutputTypeDef],
+        "ID": NotRequired[str],
+        "Prefix": NotRequired[str],
+        "Filter": NotRequired[LifecycleRuleFilterOutputTypeDef],
+        "Transitions": NotRequired[List[TransitionOutputTypeDef]],
+        "NoncurrentVersionTransitions": NotRequired[List[NoncurrentVersionTransitionTypeDef]],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
 LifecycleRuleTypeDef = TypedDict(
     "LifecycleRuleTypeDef",
     {
         "Status": ExpirationStatusType,
         "Expiration": NotRequired[LifecycleExpirationTypeDef],
         "ID": NotRequired[str],
         "Prefix": NotRequired[str],
         "Filter": NotRequired[LifecycleRuleFilterTypeDef],
-        "Transitions": NotRequired[List[TransitionTypeDef]],
-        "NoncurrentVersionTransitions": NotRequired[List[NoncurrentVersionTransitionTypeDef]],
+        "Transitions": NotRequired[Sequence[TransitionTypeDef]],
+        "NoncurrentVersionTransitions": NotRequired[Sequence[NoncurrentVersionTransitionTypeDef]],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
+MetricsConfigurationOutputTypeDef = TypedDict(
+    "MetricsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Filter": NotRequired[MetricsFilterOutputTypeDef],
+    },
+)
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotRequired[MetricsFilterTypeDef],
     },
 )
 StorageClassAnalysisTypeDef = TypedDict(
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": NotRequired[StorageClassAnalysisDataExportTypeDef],
     },
 )
-LifecycleConfigurationBucketLifecycleTypeDef = TypedDict(
-    "LifecycleConfigurationBucketLifecycleTypeDef",
+LifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleConfigurationTypeDef",
     {
-        "Rules": Sequence[RuleBucketLifecycleTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4099,64 +4364,91 @@
         "RequestPayer": NotRequired[Literal["requester"]],
         "Token": NotRequired[str],
         "ContentMD5": NotRequired[str],
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-LambdaFunctionConfigurationBucketNotificationTypeDef = TypedDict(
-    "LambdaFunctionConfigurationBucketNotificationTypeDef",
+LambdaFunctionConfigurationExtraOutputTypeDef = TypedDict(
+    "LambdaFunctionConfigurationExtraOutputTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Id": NotRequired[str],
-        "Filter": NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],
+        "Filter": NotRequired[NotificationConfigurationFilterExtraOutputTypeDef],
     },
 )
-QueueConfigurationBucketNotificationTypeDef = TypedDict(
-    "QueueConfigurationBucketNotificationTypeDef",
+QueueConfigurationExtraOutputTypeDef = TypedDict(
+    "QueueConfigurationExtraOutputTypeDef",
     {
         "QueueArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Id": NotRequired[str],
-        "Filter": NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],
+        "Filter": NotRequired[NotificationConfigurationFilterExtraOutputTypeDef],
     },
 )
-TopicConfigurationBucketNotificationTypeDef = TypedDict(
-    "TopicConfigurationBucketNotificationTypeDef",
+TopicConfigurationExtraOutputTypeDef = TypedDict(
+    "TopicConfigurationExtraOutputTypeDef",
     {
         "TopicArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
+        "Id": NotRequired[str],
+        "Filter": NotRequired[NotificationConfigurationFilterExtraOutputTypeDef],
+    },
+)
+LambdaFunctionConfigurationOutputTypeDef = TypedDict(
+    "LambdaFunctionConfigurationOutputTypeDef",
+    {
+        "LambdaFunctionArn": str,
+        "Events": List[EventType],
+        "Id": NotRequired[str],
+        "Filter": NotRequired[NotificationConfigurationFilterOutputTypeDef],
+    },
+)
+QueueConfigurationOutputTypeDef = TypedDict(
+    "QueueConfigurationOutputTypeDef",
+    {
+        "QueueArn": str,
+        "Events": List[EventType],
         "Id": NotRequired[str],
-        "Filter": NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],
+        "Filter": NotRequired[NotificationConfigurationFilterOutputTypeDef],
+    },
+)
+TopicConfigurationOutputTypeDef = TypedDict(
+    "TopicConfigurationOutputTypeDef",
+    {
+        "TopicArn": str,
+        "Events": List[EventType],
+        "Id": NotRequired[str],
+        "Filter": NotRequired[NotificationConfigurationFilterOutputTypeDef],
     },
 )
 LambdaFunctionConfigurationTypeDef = TypedDict(
     "LambdaFunctionConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Id": NotRequired[str],
         "Filter": NotRequired[NotificationConfigurationFilterTypeDef],
     },
 )
 QueueConfigurationTypeDef = TypedDict(
     "QueueConfigurationTypeDef",
     {
         "QueueArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Id": NotRequired[str],
         "Filter": NotRequired[NotificationConfigurationFilterTypeDef],
     },
 )
 TopicConfigurationTypeDef = TypedDict(
     "TopicConfigurationTypeDef",
     {
         "TopicArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Id": NotRequired[str],
         "Filter": NotRequired[NotificationConfigurationFilterTypeDef],
     },
 )
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
@@ -4222,27 +4514,38 @@
 )
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
         "S3": NotRequired[S3LocationTypeDef],
     },
 )
+InventoryDestinationOutputTypeDef = TypedDict(
+    "InventoryDestinationOutputTypeDef",
+    {
+        "S3BucketDestination": InventoryS3BucketDestinationOutputTypeDef,
+    },
+)
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
     },
 )
-PutBucketLifecycleRequestRequestTypeDef = TypedDict(
-    "PutBucketLifecycleRequestRequestTypeDef",
+ReplicationRuleOutputTypeDef = TypedDict(
+    "ReplicationRuleOutputTypeDef",
     {
-        "Bucket": str,
-        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "LifecycleConfiguration": NotRequired[LifecycleConfigurationTypeDef],
-        "ExpectedBucketOwner": NotRequired[str],
+        "Status": ReplicationRuleStatusType,
+        "Destination": DestinationTypeDef,
+        "ID": NotRequired[str],
+        "Priority": NotRequired[int],
+        "Prefix": NotRequired[str],
+        "Filter": NotRequired[ReplicationRuleFilterOutputTypeDef],
+        "SourceSelectionCriteria": NotRequired[SourceSelectionCriteriaTypeDef],
+        "ExistingObjectReplication": NotRequired[ExistingObjectReplicationTypeDef],
+        "DeleteMarkerReplication": NotRequired[DeleteMarkerReplicationTypeDef],
     },
 )
 ReplicationRuleTypeDef = TypedDict(
     "ReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
         "Destination": DestinationTypeDef,
@@ -4251,33 +4554,27 @@
         "Prefix": NotRequired[str],
         "Filter": NotRequired[ReplicationRuleFilterTypeDef],
         "SourceSelectionCriteria": NotRequired[SourceSelectionCriteriaTypeDef],
         "ExistingObjectReplication": NotRequired[ExistingObjectReplicationTypeDef],
         "DeleteMarkerReplication": NotRequired[DeleteMarkerReplicationTypeDef],
     },
 )
-BucketLoggingStatusBucketLoggingTypeDef = TypedDict(
-    "BucketLoggingStatusBucketLoggingTypeDef",
+GetBucketLoggingOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputTypeDef",
     {
-        "LoggingEnabled": NotRequired[LoggingEnabledBucketLoggingTypeDef],
+        "LoggingEnabled": LoggingEnabledOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 BucketLoggingStatusTypeDef = TypedDict(
     "BucketLoggingStatusTypeDef",
     {
         "LoggingEnabled": NotRequired[LoggingEnabledTypeDef],
     },
 )
-GetBucketLoggingOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputTypeDef",
-    {
-        "LoggingEnabled": LoggingEnabledTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 PutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     {
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
@@ -4290,138 +4587,147 @@
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "PutBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ContentMD5": NotRequired[str],
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
+ServerSideEncryptionConfigurationUnionTypeDef = Union[
+    ServerSideEncryptionConfigurationTypeDef, ServerSideEncryptionConfigurationOutputTypeDef
+]
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
         "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
+        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IntelligentTieringConfigurationUnionTypeDef = Union[
+    IntelligentTieringConfigurationTypeDef, IntelligentTieringConfigurationOutputTypeDef
+]
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
     },
 )
-BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = TypedDict(
-    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
+GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputTypeDef",
     {
-        "Rules": Sequence[LifecycleRuleBucketLifecycleConfigurationTypeDef],
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 BucketLifecycleConfigurationTypeDef = TypedDict(
     "BucketLifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
 )
-GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputTypeDef",
-    {
-        "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
-        "MetricsConfiguration": MetricsConfigurationTypeDef,
+        "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
+        "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+MetricsConfigurationUnionTypeDef = Union[
+    MetricsConfigurationTypeDef, MetricsConfigurationOutputTypeDef
+]
 PutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "MetricsConfiguration": MetricsConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
+AnalyticsConfigurationOutputTypeDef = TypedDict(
+    "AnalyticsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
+        "Filter": NotRequired[AnalyticsFilterOutputTypeDef],
+    },
+)
 AnalyticsConfigurationTypeDef = TypedDict(
     "AnalyticsConfigurationTypeDef",
     {
         "Id": str,
         "StorageClassAnalysis": StorageClassAnalysisTypeDef,
         "Filter": NotRequired[AnalyticsFilterTypeDef],
     },
 )
 PutBucketLifecycleRequestBucketLifecyclePutTypeDef = TypedDict(
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     {
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "LifecycleConfiguration": NotRequired[LifecycleConfigurationBucketLifecycleTypeDef],
+        "LifecycleConfiguration": NotRequired[LifecycleConfigurationTypeDef],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-NotificationConfigurationBucketNotificationTypeDef = TypedDict(
-    "NotificationConfigurationBucketNotificationTypeDef",
+PutBucketLifecycleRequestRequestTypeDef = TypedDict(
+    "PutBucketLifecycleRequestRequestTypeDef",
     {
-        "TopicConfigurations": NotRequired[Sequence[TopicConfigurationBucketNotificationTypeDef]],
-        "QueueConfigurations": NotRequired[Sequence[QueueConfigurationBucketNotificationTypeDef]],
-        "LambdaFunctionConfigurations": NotRequired[
-            Sequence[LambdaFunctionConfigurationBucketNotificationTypeDef]
-        ],
-        "EventBridgeConfiguration": NotRequired[Mapping[str, Any]],
+        "Bucket": str,
+        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
+        "LifecycleConfiguration": NotRequired[LifecycleConfigurationTypeDef],
+        "ExpectedBucketOwner": NotRequired[str],
     },
 )
 NotificationConfigurationResponseTypeDef = TypedDict(
     "NotificationConfigurationResponseTypeDef",
     {
-        "TopicConfigurations": List[TopicConfigurationTypeDef],
-        "QueueConfigurations": List[QueueConfigurationTypeDef],
-        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
+        "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
+        "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
+        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
@@ -4439,37 +4745,56 @@
         "Type": NotRequired[Literal["SELECT"]],
         "Tier": NotRequired[TierType],
         "Description": NotRequired[str],
         "SelectParameters": NotRequired[SelectParametersTypeDef],
         "OutputLocation": NotRequired[OutputLocationTypeDef],
     },
 )
+InventoryConfigurationOutputTypeDef = TypedDict(
+    "InventoryConfigurationOutputTypeDef",
+    {
+        "Destination": InventoryDestinationOutputTypeDef,
+        "IsEnabled": bool,
+        "Id": str,
+        "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
+        "Schedule": InventoryScheduleTypeDef,
+        "Filter": NotRequired[InventoryFilterTypeDef],
+        "OptionalFields": NotRequired[List[InventoryOptionalFieldType]],
+    },
+)
 InventoryConfigurationTypeDef = TypedDict(
     "InventoryConfigurationTypeDef",
     {
         "Destination": InventoryDestinationTypeDef,
         "IsEnabled": bool,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "Schedule": InventoryScheduleTypeDef,
         "Filter": NotRequired[InventoryFilterTypeDef],
-        "OptionalFields": NotRequired[List[InventoryOptionalFieldType]],
+        "OptionalFields": NotRequired[Sequence[InventoryOptionalFieldType]],
+    },
+)
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "Role": str,
+        "Rules": List[ReplicationRuleOutputTypeDef],
     },
 )
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": List[ReplicationRuleTypeDef],
+        "Rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 PutBucketLoggingRequestBucketLoggingPutTypeDef = TypedDict(
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     {
-        "BucketLoggingStatus": BucketLoggingStatusBucketLoggingTypeDef,
+        "BucketLoggingStatus": BucketLoggingStatusTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketLoggingRequestRequestTypeDef = TypedDict(
     "PutBucketLoggingRequestRequestTypeDef",
     {
@@ -4479,17 +4804,15 @@
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     {
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "LifecycleConfiguration": NotRequired[
-            BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef
-        ],
+        "LifecycleConfiguration": NotRequired[BucketLifecycleConfigurationTypeDef],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4497,41 +4820,44 @@
         "LifecycleConfiguration": NotRequired[BucketLifecycleConfigurationTypeDef],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
-        "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
+        "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
+        "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AnalyticsConfigurationUnionTypeDef = Union[
+    AnalyticsConfigurationTypeDef, AnalyticsConfigurationOutputTypeDef
+]
 PutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationBucketNotificationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
         "SkipDestinationValidation": NotRequired[bool],
     },
 )
 PutBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     {
@@ -4572,47 +4898,53 @@
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
-        "InventoryConfiguration": InventoryConfigurationTypeDef,
+        "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
-        "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
+        "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+InventoryConfigurationUnionTypeDef = Union[
+    InventoryConfigurationTypeDef, InventoryConfigurationOutputTypeDef
+]
 PutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "InventoryConfiguration": InventoryConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "Token": NotRequired[str],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/type_defs.pyi` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -99,22 +99,24 @@
     "BlobTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "FileobjTypeDef",
     "BucketInfoTypeDef",
     "BucketTypeDef",
     "BucketUploadFileRequestTypeDef",
-    "CORSRuleBucketCorsTypeDef",
     "CORSRuleTypeDef",
+    "CORSRuleExtraOutputTypeDef",
+    "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "ChecksumTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
+    "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
     "CompletedPartTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "TimestampTypeDef",
     "CopyPartResultTypeDef",
@@ -183,15 +185,15 @@
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "ObjectLockRetentionTypeDef",
+    "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeTypeDef",
@@ -200,32 +202,37 @@
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
-    "LifecycleExpirationTypeDef",
+    "LifecycleExpirationExtraExtraOutputTypeDef",
+    "LifecycleExpirationExtraOutputTypeDef",
+    "LifecycleExpirationOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
-    "TransitionTypeDef",
+    "TransitionExtraOutputTypeDef",
+    "TransitionOutputTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListDirectoryBucketsRequestRequestTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueTypeDef",
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "OwnershipControlsRuleTypeDef",
     "PartitionedPrefixTypeDef",
@@ -236,14 +243,15 @@
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
     "RecordsEventTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
+    "TransitionExtraExtraOutputTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StatsTypeDef",
     "AbortMultipartUploadOutputTypeDef",
     "CompleteMultipartUploadOutputTypeDef",
     "CreateBucketOutputTypeDef",
@@ -272,21 +280,26 @@
     "PutObjectTaggingOutputTypeDef",
     "RedirectAllRequestsToResponseTypeDef",
     "RestoreObjectOutputTypeDef",
     "RestoreStatusResponseTypeDef",
     "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "DeleteMarkerEntryTypeDef",
+    "AnalyticsAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
+    "IntelligentTieringAndOperatorOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
-    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
+    "LifecycleRuleAndOperatorExtraOutputTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
+    "MetricsAndOperatorOutputTypeDef",
     "MetricsAndOperatorTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "TaggingTypeDef",
     "AnalyticsExportDestinationTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
@@ -296,15 +309,14 @@
     "BucketUploadFileobjRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
     "ListBucketsOutputTypeDef",
     "ListDirectoryBucketsOutputTypeDef",
-    "CORSConfigurationBucketCorsTypeDef",
     "CORSConfigurationTypeDef",
     "GetBucketCorsOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
     "CopyObjectOutputTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
@@ -312,190 +324,217 @@
     "CreateMultipartUploadRequestRequestTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
-    "LifecycleExpirationBucketLifecycleTypeDef",
+    "LifecycleExpirationTypeDef",
+    "ObjectLockRetentionTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "TransitionBucketLifecycleConfigurationTypeDef",
-    "TransitionBucketLifecycleTypeDef",
+    "TransitionTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "UploadPartCopyOutputTypeDef",
     "CreateBucketConfigurationTypeDef",
     "CreateSessionOutputTypeDef",
     "ObjectLockRuleTypeDef",
     "DeleteObjectsOutputTypeDef",
     "DeleteTypeDef",
-    "S3KeyFilterBucketNotificationTypeDef",
+    "S3KeyFilterExtraOutputTypeDef",
+    "S3KeyFilterOutputTypeDef",
     "S3KeyFilterTypeDef",
     "GetBucketPolicyStatusOutputTypeDef",
     "GetObjectAttributesPartsTypeDef",
     "GetObjectLegalHoldOutputTypeDef",
     "PutObjectLegalHoldRequestRequestTypeDef",
     "GetObjectRetentionOutputTypeDef",
-    "PutObjectRetentionRequestRequestTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
     "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
+    "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
-    "RuleTypeDef",
+    "RuleOutputTypeDef",
     "ListDirectoryBucketsRequestListDirectoryBucketsPaginateTypeDef",
     "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
     "ObjectTypeDef",
     "ObjectVersionTypeDef",
+    "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
-    "TargetObjectKeyFormatBucketLoggingTypeDef",
+    "TargetObjectKeyFormatExtraOutputTypeDef",
+    "TargetObjectKeyFormatOutputTypeDef",
     "TargetObjectKeyFormatTypeDef",
     "ProgressEventTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "RoutingRuleTypeDef",
+    "RuleExtraOutputTypeDef",
     "ServerSideEncryptionRuleTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "StatsEventTypeDef",
+    "AnalyticsFilterOutputTypeDef",
     "AnalyticsFilterTypeDef",
+    "IntelligentTieringFilterOutputTypeDef",
     "IntelligentTieringFilterTypeDef",
-    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
+    "LifecycleRuleFilterExtraOutputTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
+    "MetricsFilterOutputTypeDef",
     "MetricsFilterTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestBucketTaggingPutTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "PutObjectTaggingRequestRequestTypeDef",
     "StorageClassAnalysisDataExportTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     "PutBucketCorsRequestRequestTypeDef",
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadRequestRequestTypeDef",
-    "RuleBucketLifecycleTypeDef",
+    "ObjectLockRetentionUnionTypeDef",
+    "PutObjectRetentionRequestRequestTypeDef",
+    "RuleTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
-    "NotificationConfigurationFilterBucketNotificationTypeDef",
+    "NotificationConfigurationFilterExtraOutputTypeDef",
+    "NotificationConfigurationFilterOutputTypeDef",
     "NotificationConfigurationFilterTypeDef",
     "GetObjectAttributesOutputTypeDef",
     "AccessControlPolicyTypeDef",
     "GetBucketAclOutputTypeDef",
     "GetObjectAclOutputTypeDef",
     "S3LocationTypeDef",
     "ListMultipartUploadsOutputTypeDef",
+    "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
     "GetBucketLifecycleOutputTypeDef",
-    "LifecycleConfigurationTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
     "ListObjectsOutputTypeDef",
     "ListObjectsV2OutputTypeDef",
     "ListObjectVersionsOutputTypeDef",
     "GetBucketOwnershipControlsOutputTypeDef",
+    "OwnershipControlsUnionTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
-    "LoggingEnabledBucketLoggingTypeDef",
     "LoggingEnabledResponseTypeDef",
+    "LoggingEnabledOutputTypeDef",
     "LoggingEnabledTypeDef",
     "GetBucketWebsiteOutputTypeDef",
     "WebsiteConfigurationTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "SelectObjectContentEventStreamTypeDef",
+    "IntelligentTieringConfigurationOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
-    "LifecycleRuleBucketLifecycleConfigurationTypeDef",
+    "LifecycleRuleExtraOutputTypeDef",
+    "LifecycleRuleOutputTypeDef",
     "LifecycleRuleTypeDef",
+    "MetricsConfigurationOutputTypeDef",
     "MetricsConfigurationTypeDef",
     "StorageClassAnalysisTypeDef",
-    "LifecycleConfigurationBucketLifecycleTypeDef",
+    "LifecycleConfigurationTypeDef",
     "GetObjectLockConfigurationOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
-    "LambdaFunctionConfigurationBucketNotificationTypeDef",
-    "QueueConfigurationBucketNotificationTypeDef",
-    "TopicConfigurationBucketNotificationTypeDef",
+    "LambdaFunctionConfigurationExtraOutputTypeDef",
+    "QueueConfigurationExtraOutputTypeDef",
+    "TopicConfigurationExtraOutputTypeDef",
+    "LambdaFunctionConfigurationOutputTypeDef",
+    "QueueConfigurationOutputTypeDef",
+    "TopicConfigurationOutputTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
+    "InventoryDestinationOutputTypeDef",
     "InventoryDestinationTypeDef",
-    "PutBucketLifecycleRequestRequestTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
-    "BucketLoggingStatusBucketLoggingTypeDef",
-    "BucketLoggingStatusTypeDef",
     "GetBucketLoggingOutputTypeDef",
+    "BucketLoggingStatusTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
     "GetBucketEncryptionOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
+    "ServerSideEncryptionConfigurationUnionTypeDef",
     "SelectObjectContentOutputTypeDef",
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+    "IntelligentTieringConfigurationUnionTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
-    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
-    "BucketLifecycleConfigurationTypeDef",
     "GetBucketLifecycleConfigurationOutputTypeDef",
+    "BucketLifecycleConfigurationTypeDef",
     "GetBucketMetricsConfigurationOutputTypeDef",
     "ListBucketMetricsConfigurationsOutputTypeDef",
+    "MetricsConfigurationUnionTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
+    "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
-    "NotificationConfigurationBucketNotificationTypeDef",
+    "PutBucketLifecycleRequestRequestTypeDef",
     "NotificationConfigurationResponseTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
+    "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
+    "AnalyticsConfigurationUnionTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
     "GetBucketInventoryConfigurationOutputTypeDef",
     "ListBucketInventoryConfigurationsOutputTypeDef",
+    "InventoryConfigurationUnionTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketReplicationOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": NotRequired[int],
     },
@@ -602,27 +641,38 @@
         "Filename": str,
         "Key": str,
         "ExtraArgs": NotRequired[Optional[Dict[str, Any]]],
         "Callback": NotRequired[Optional[Callable[..., Any]]],
         "Config": NotRequired[Optional[TransferConfig]],
     },
 )
-CORSRuleBucketCorsTypeDef = TypedDict(
-    "CORSRuleBucketCorsTypeDef",
+CORSRuleTypeDef = TypedDict(
+    "CORSRuleTypeDef",
     {
         "AllowedMethods": Sequence[str],
         "AllowedOrigins": Sequence[str],
         "ID": NotRequired[str],
         "AllowedHeaders": NotRequired[Sequence[str]],
         "ExposeHeaders": NotRequired[Sequence[str]],
         "MaxAgeSeconds": NotRequired[int],
     },
 )
-CORSRuleTypeDef = TypedDict(
-    "CORSRuleTypeDef",
+CORSRuleExtraOutputTypeDef = TypedDict(
+    "CORSRuleExtraOutputTypeDef",
+    {
+        "AllowedMethods": List[str],
+        "AllowedOrigins": List[str],
+        "ID": NotRequired[str],
+        "AllowedHeaders": NotRequired[List[str]],
+        "ExposeHeaders": NotRequired[List[str]],
+        "MaxAgeSeconds": NotRequired[int],
+    },
+)
+CORSRuleOutputTypeDef = TypedDict(
+    "CORSRuleOutputTypeDef",
     {
         "AllowedMethods": List[str],
         "AllowedOrigins": List[str],
         "ID": NotRequired[str],
         "AllowedHeaders": NotRequired[List[str]],
         "ExposeHeaders": NotRequired[List[str]],
         "MaxAgeSeconds": NotRequired[int],
@@ -687,20 +737,30 @@
         "Bucket": str,
         "Key": str,
         "ExtraArgs": NotRequired[Optional[Dict[str, Any]]],
         "Callback": NotRequired[Optional[Callable[..., Any]]],
         "Config": NotRequired[Optional[TransferConfig]],
     },
 )
+CloudFunctionConfigurationOutputTypeDef = TypedDict(
+    "CloudFunctionConfigurationOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Event": NotRequired[EventType],
+        "Events": NotRequired[List[EventType]],
+        "CloudFunction": NotRequired[str],
+        "InvocationRole": NotRequired[str],
+    },
+)
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": NotRequired[str],
         "Event": NotRequired[EventType],
-        "Events": NotRequired[List[EventType]],
+        "Events": NotRequired[Sequence[EventType]],
         "CloudFunction": NotRequired[str],
         "InvocationRole": NotRequired[str],
     },
 )
 CommonPrefixTypeDef = TypedDict(
     "CommonPrefixTypeDef",
     {
@@ -1262,16 +1322,16 @@
 GetObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "GetObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-ObjectLockRetentionTypeDef = TypedDict(
-    "ObjectLockRetentionTypeDef",
+ObjectLockRetentionOutputTypeDef = TypedDict(
+    "ObjectLockRetentionOutputTypeDef",
     {
         "Mode": NotRequired[ObjectLockRetentionModeType],
         "RetainUntilDate": NotRequired[datetime],
     },
 )
 GetObjectRetentionRequestRequestTypeDef = TypedDict(
     "GetObjectRetentionRequestRequestTypeDef",
@@ -1388,16 +1448,32 @@
 )
 JSONOutputTypeDef = TypedDict(
     "JSONOutputTypeDef",
     {
         "RecordDelimiter": NotRequired[str],
     },
 )
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
+LifecycleExpirationExtraExtraOutputTypeDef = TypedDict(
+    "LifecycleExpirationExtraExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "ExpiredObjectDeleteMarker": NotRequired[bool],
+    },
+)
+LifecycleExpirationExtraOutputTypeDef = TypedDict(
+    "LifecycleExpirationExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "ExpiredObjectDeleteMarker": NotRequired[bool],
+    },
+)
+LifecycleExpirationOutputTypeDef = TypedDict(
+    "LifecycleExpirationOutputTypeDef",
     {
         "Date": NotRequired[datetime],
         "Days": NotRequired[int],
         "ExpiredObjectDeleteMarker": NotRequired[bool],
     },
 )
 NoncurrentVersionExpirationTypeDef = TypedDict(
@@ -1411,16 +1487,24 @@
     "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": NotRequired[int],
         "StorageClass": NotRequired[TransitionStorageClassType],
         "NewerNoncurrentVersions": NotRequired[int],
     },
 )
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
+TransitionExtraOutputTypeDef = TypedDict(
+    "TransitionExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "StorageClass": NotRequired[TransitionStorageClassType],
+    },
+)
+TransitionOutputTypeDef = TypedDict(
+    "TransitionOutputTypeDef",
     {
         "Date": NotRequired[datetime],
         "Days": NotRequired[int],
         "StorageClass": NotRequired[TransitionStorageClassType],
     },
 )
 ListBucketAnalyticsConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1565,28 +1649,46 @@
 )
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": NotRequired[int],
     },
 )
+QueueConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Event": NotRequired[EventType],
+        "Events": NotRequired[List[EventType]],
+        "Queue": NotRequired[str],
+    },
+)
+TopicConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "TopicConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Events": NotRequired[List[EventType]],
+        "Event": NotRequired[EventType],
+        "Topic": NotRequired[str],
+    },
+)
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": NotRequired[str],
         "Event": NotRequired[EventType],
-        "Events": NotRequired[List[EventType]],
+        "Events": NotRequired[Sequence[EventType]],
         "Queue": NotRequired[str],
     },
 )
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": NotRequired[str],
-        "Events": NotRequired[List[EventType]],
+        "Events": NotRequired[Sequence[EventType]],
         "Event": NotRequired[EventType],
         "Topic": NotRequired[str],
     },
 )
 ObjectDownloadFileRequestTypeDef = TypedDict(
     "ObjectDownloadFileRequestTypeDef",
     {
@@ -1704,14 +1806,22 @@
 )
 RequestProgressTypeDef = TypedDict(
     "RequestProgressTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
+TransitionExtraExtraOutputTypeDef = TypedDict(
+    "TransitionExtraExtraOutputTypeDef",
+    {
+        "Date": NotRequired[datetime],
+        "Days": NotRequired[int],
+        "StorageClass": NotRequired[TransitionStorageClassType],
+    },
+)
 ScanRangeTypeDef = TypedDict(
     "ScanRangeTypeDef",
     {
         "Start": NotRequired[int],
         "End": NotRequired[int],
     },
 )
@@ -2089,19 +2199,26 @@
         "Owner": NotRequired[OwnerTypeDef],
         "Key": NotRequired[str],
         "VersionId": NotRequired[str],
         "IsLatest": NotRequired[bool],
         "LastModified": NotRequired[datetime],
     },
 )
+AnalyticsAndOperatorOutputTypeDef = TypedDict(
+    "AnalyticsAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 AnalyticsAndOperatorTypeDef = TypedDict(
     "AnalyticsAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2111,52 +2228,83 @@
     "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
+    "IntelligentTieringAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+LifecycleRuleAndOperatorExtraOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorExtraOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
+        "ObjectSizeGreaterThan": NotRequired[int],
+        "ObjectSizeLessThan": NotRequired[int],
     },
 )
-LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "Tags": NotRequired[List[TagTypeDef]],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
     },
 )
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
     },
 )
+MetricsAndOperatorOutputTypeDef = TypedDict(
+    "MetricsAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+        "AccessPointArn": NotRequired[str],
+    },
+)
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
         "AccessPointArn": NotRequired[str],
     },
 )
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[TagTypeDef],
     },
@@ -2313,30 +2461,24 @@
     "ListDirectoryBucketsOutputTypeDef",
     {
         "Buckets": List[BucketTypeDef],
         "ContinuationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CORSConfigurationBucketCorsTypeDef = TypedDict(
-    "CORSConfigurationBucketCorsTypeDef",
-    {
-        "CORSRules": Sequence[CORSRuleBucketCorsTypeDef],
-    },
-)
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
-        "CORSRules": List[CORSRuleTypeDef],
+        "CORSRules": List[CORSRuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": NotRequired[Sequence[CompletedPartTypeDef]],
@@ -2678,28 +2820,27 @@
         "SSECustomerKeyMD5": NotRequired[str],
         "RequestPayer": NotRequired[Literal["requester"]],
         "PartNumber": NotRequired[int],
         "ExpectedBucketOwner": NotRequired[str],
         "ChecksumMode": NotRequired[Literal["ENABLED"]],
     },
 )
-LifecycleExpirationBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
+LifecycleExpirationTypeDef = TypedDict(
+    "LifecycleExpirationTypeDef",
     {
         "Date": NotRequired[TimestampTypeDef],
         "Days": NotRequired[int],
         "ExpiredObjectDeleteMarker": NotRequired[bool],
     },
 )
-LifecycleExpirationBucketLifecycleTypeDef = TypedDict(
-    "LifecycleExpirationBucketLifecycleTypeDef",
+ObjectLockRetentionTypeDef = TypedDict(
+    "ObjectLockRetentionTypeDef",
     {
-        "Date": NotRequired[TimestampTypeDef],
-        "Days": NotRequired[int],
-        "ExpiredObjectDeleteMarker": NotRequired[bool],
+        "Mode": NotRequired[ObjectLockRetentionModeType],
+        "RetainUntilDate": NotRequired[TimestampTypeDef],
     },
 )
 PutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "PutObjectRequestBucketPutObjectTypeDef",
     {
         "Key": str,
         "ACL": NotRequired[ObjectCannedACLType],
@@ -2857,24 +2998,16 @@
         "Tagging": NotRequired[str],
         "ObjectLockMode": NotRequired[ObjectLockModeType],
         "ObjectLockRetainUntilDate": NotRequired[TimestampTypeDef],
         "ObjectLockLegalHoldStatus": NotRequired[ObjectLockLegalHoldStatusType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-TransitionBucketLifecycleConfigurationTypeDef = TypedDict(
-    "TransitionBucketLifecycleConfigurationTypeDef",
-    {
-        "Date": NotRequired[TimestampTypeDef],
-        "Days": NotRequired[int],
-        "StorageClass": NotRequired[TransitionStorageClassType],
-    },
-)
-TransitionBucketLifecycleTypeDef = TypedDict(
-    "TransitionBucketLifecycleTypeDef",
+TransitionTypeDef = TypedDict(
+    "TransitionTypeDef",
     {
         "Date": NotRequired[TimestampTypeDef],
         "Days": NotRequired[int],
         "StorageClass": NotRequired[TransitionStorageClassType],
     },
 )
 WriteGetObjectResponseRequestRequestTypeDef = TypedDict(
@@ -2969,24 +3102,30 @@
 DeleteTypeDef = TypedDict(
     "DeleteTypeDef",
     {
         "Objects": Sequence[ObjectIdentifierTypeDef],
         "Quiet": NotRequired[bool],
     },
 )
-S3KeyFilterBucketNotificationTypeDef = TypedDict(
-    "S3KeyFilterBucketNotificationTypeDef",
+S3KeyFilterExtraOutputTypeDef = TypedDict(
+    "S3KeyFilterExtraOutputTypeDef",
     {
-        "FilterRules": NotRequired[Sequence[FilterRuleTypeDef]],
+        "FilterRules": NotRequired[List[FilterRuleTypeDef]],
+    },
+)
+S3KeyFilterOutputTypeDef = TypedDict(
+    "S3KeyFilterOutputTypeDef",
+    {
+        "FilterRules": NotRequired[List[FilterRuleTypeDef]],
     },
 )
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
-        "FilterRules": NotRequired[List[FilterRuleTypeDef]],
+        "FilterRules": NotRequired[Sequence[FilterRuleTypeDef]],
     },
 )
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3022,32 +3161,18 @@
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionTypeDef,
+        "Retention": ObjectLockRetentionOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "PutObjectRetentionRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-        "Retention": NotRequired[ObjectLockRetentionTypeDef],
-        "RequestPayer": NotRequired[Literal["requester"]],
-        "VersionId": NotRequired[str],
-        "BypassGovernanceRetention": NotRequired[bool],
-        "ContentMD5": NotRequired[str],
-        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "ExpectedBucketOwner": NotRequired[str],
-    },
-)
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3150,36 +3275,43 @@
     {
         "CSV": NotRequired[CSVInputTypeDef],
         "CompressionType": NotRequired[CompressionTypeType],
         "JSON": NotRequired[JSONInputTypeDef],
         "Parquet": NotRequired[Mapping[str, Any]],
     },
 )
+InventoryEncryptionOutputTypeDef = TypedDict(
+    "InventoryEncryptionOutputTypeDef",
+    {
+        "SSES3": NotRequired[Dict[str, Any]],
+        "SSEKMS": NotRequired[SSEKMSTypeDef],
+    },
+)
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
-        "SSES3": NotRequired[Dict[str, Any]],
+        "SSES3": NotRequired[Mapping[str, Any]],
         "SSEKMS": NotRequired[SSEKMSTypeDef],
     },
 )
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": NotRequired[CSVOutputTypeDef],
         "JSON": NotRequired[JSONOutputTypeDef],
     },
 )
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
-        "Expiration": NotRequired[LifecycleExpirationTypeDef],
+        "Expiration": NotRequired[LifecycleExpirationOutputTypeDef],
         "ID": NotRequired[str],
-        "Transition": NotRequired[TransitionTypeDef],
+        "Transition": NotRequired[TransitionOutputTypeDef],
         "NoncurrentVersionTransition": NotRequired[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
 ListDirectoryBucketsRequestListDirectoryBucketsPaginateTypeDef = TypedDict(
     "ListDirectoryBucketsRequestListDirectoryBucketsPaginateTypeDef",
@@ -3288,17 +3420,17 @@
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 NotificationConfigurationDeprecatedResponseTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseTypeDef",
     {
-        "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
-        "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
-        "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
+        "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
+        "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
+        "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": NotRequired[TopicConfigurationDeprecatedTypeDef],
@@ -3330,31 +3462,44 @@
         "VersionId": NotRequired[str],
         "IsLatest": NotRequired[bool],
         "LastModified": NotRequired[datetime],
         "Owner": NotRequired[OwnerTypeDef],
         "RestoreStatus": NotRequired[RestoreStatusTypeDef],
     },
 )
+OwnershipControlsOutputTypeDef = TypedDict(
+    "OwnershipControlsOutputTypeDef",
+    {
+        "Rules": List[OwnershipControlsRuleTypeDef],
+    },
+)
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
-        "Rules": List[OwnershipControlsRuleTypeDef],
+        "Rules": Sequence[OwnershipControlsRuleTypeDef],
     },
 )
-TargetObjectKeyFormatBucketLoggingTypeDef = TypedDict(
-    "TargetObjectKeyFormatBucketLoggingTypeDef",
+TargetObjectKeyFormatExtraOutputTypeDef = TypedDict(
+    "TargetObjectKeyFormatExtraOutputTypeDef",
     {
-        "SimplePrefix": NotRequired[Mapping[str, Any]],
+        "SimplePrefix": NotRequired[Dict[str, Any]],
+        "PartitionedPrefix": NotRequired[PartitionedPrefixTypeDef],
+    },
+)
+TargetObjectKeyFormatOutputTypeDef = TypedDict(
+    "TargetObjectKeyFormatOutputTypeDef",
+    {
+        "SimplePrefix": NotRequired[Dict[str, Any]],
         "PartitionedPrefix": NotRequired[PartitionedPrefixTypeDef],
     },
 )
 TargetObjectKeyFormatTypeDef = TypedDict(
     "TargetObjectKeyFormatTypeDef",
     {
-        "SimplePrefix": NotRequired[Dict[str, Any]],
+        "SimplePrefix": NotRequired[Mapping[str, Any]],
         "PartitionedPrefix": NotRequired[PartitionedPrefixTypeDef],
     },
 )
 ProgressEventTypeDef = TypedDict(
     "ProgressEventTypeDef",
     {
         "Details": NotRequired[ProgressTypeDef],
@@ -3399,14 +3544,27 @@
 RoutingRuleTypeDef = TypedDict(
     "RoutingRuleTypeDef",
     {
         "Redirect": RedirectTypeDef,
         "Condition": NotRequired[ConditionTypeDef],
     },
 )
+RuleExtraOutputTypeDef = TypedDict(
+    "RuleExtraOutputTypeDef",
+    {
+        "Prefix": str,
+        "Status": ExpirationStatusType,
+        "Expiration": NotRequired[LifecycleExpirationExtraExtraOutputTypeDef],
+        "ID": NotRequired[str],
+        "Transition": NotRequired[TransitionExtraExtraOutputTypeDef],
+        "NoncurrentVersionTransition": NotRequired[NoncurrentVersionTransitionTypeDef],
+        "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
+        "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
+    },
+)
 ServerSideEncryptionRuleTypeDef = TypedDict(
     "ServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": NotRequired[ServerSideEncryptionByDefaultTypeDef],
         "BucketKeyEnabled": NotRequired[bool],
     },
 )
@@ -3419,59 +3577,102 @@
 )
 StatsEventTypeDef = TypedDict(
     "StatsEventTypeDef",
     {
         "Details": NotRequired[StatsTypeDef],
     },
 )
+AnalyticsFilterOutputTypeDef = TypedDict(
+    "AnalyticsFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "And": NotRequired[AnalyticsAndOperatorOutputTypeDef],
+    },
+)
 AnalyticsFilterTypeDef = TypedDict(
     "AnalyticsFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "And": NotRequired[AnalyticsAndOperatorTypeDef],
     },
 )
+IntelligentTieringFilterOutputTypeDef = TypedDict(
+    "IntelligentTieringFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "And": NotRequired[IntelligentTieringAndOperatorOutputTypeDef],
+    },
+)
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "And": NotRequired[IntelligentTieringAndOperatorTypeDef],
     },
 )
-LifecycleRuleFilterBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
+LifecycleRuleFilterExtraOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterExtraOutputTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
-        "And": NotRequired[LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef],
+        "And": NotRequired[LifecycleRuleAndOperatorExtraOutputTypeDef],
+    },
+)
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "ObjectSizeGreaterThan": NotRequired[int],
+        "ObjectSizeLessThan": NotRequired[int],
+        "And": NotRequired[LifecycleRuleAndOperatorOutputTypeDef],
     },
 )
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "ObjectSizeGreaterThan": NotRequired[int],
         "ObjectSizeLessThan": NotRequired[int],
         "And": NotRequired[LifecycleRuleAndOperatorTypeDef],
     },
 )
+MetricsFilterOutputTypeDef = TypedDict(
+    "MetricsFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "AccessPointArn": NotRequired[str],
+        "And": NotRequired[MetricsAndOperatorOutputTypeDef],
+    },
+)
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "AccessPointArn": NotRequired[str],
         "And": NotRequired[MetricsAndOperatorTypeDef],
     },
 )
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
+    {
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[TagTypeDef],
+        "And": NotRequired[ReplicationRuleAndOperatorOutputTypeDef],
+    },
+)
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": NotRequired[str],
         "Tag": NotRequired[TagTypeDef],
         "And": NotRequired[ReplicationRuleAndOperatorTypeDef],
     },
@@ -3602,15 +3803,15 @@
         "ExpectedBucketOwner": NotRequired[str],
         "ExpectedSourceBucketOwner": NotRequired[str],
     },
 )
 PutBucketCorsRequestBucketCorsPutTypeDef = TypedDict(
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     {
-        "CORSConfiguration": CORSConfigurationBucketCorsTypeDef,
+        "CORSConfiguration": CORSConfigurationTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketCorsRequestRequestTypeDef = TypedDict(
     "PutBucketCorsRequestRequestTypeDef",
     {
@@ -3649,22 +3850,39 @@
         "RequestPayer": NotRequired[Literal["requester"]],
         "ExpectedBucketOwner": NotRequired[str],
         "SSECustomerAlgorithm": NotRequired[str],
         "SSECustomerKey": NotRequired[str],
         "SSECustomerKeyMD5": NotRequired[str],
     },
 )
-RuleBucketLifecycleTypeDef = TypedDict(
-    "RuleBucketLifecycleTypeDef",
+ObjectLockRetentionUnionTypeDef = Union[
+    ObjectLockRetentionTypeDef, ObjectLockRetentionOutputTypeDef
+]
+PutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "PutObjectRetentionRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "Retention": NotRequired[ObjectLockRetentionTypeDef],
+        "RequestPayer": NotRequired[Literal["requester"]],
+        "VersionId": NotRequired[str],
+        "BypassGovernanceRetention": NotRequired[bool],
+        "ContentMD5": NotRequired[str],
+        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
+        "ExpectedBucketOwner": NotRequired[str],
+    },
+)
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
-        "Expiration": NotRequired[LifecycleExpirationBucketLifecycleTypeDef],
+        "Expiration": NotRequired[LifecycleExpirationTypeDef],
         "ID": NotRequired[str],
-        "Transition": NotRequired[TransitionBucketLifecycleTypeDef],
+        "Transition": NotRequired[TransitionTypeDef],
         "NoncurrentVersionTransition": NotRequired[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
 CreateBucketRequestBucketCreateTypeDef = TypedDict(
     "CreateBucketRequestBucketCreateTypeDef",
@@ -3736,18 +3954,24 @@
         "MFA": NotRequired[str],
         "RequestPayer": NotRequired[Literal["requester"]],
         "BypassGovernanceRetention": NotRequired[bool],
         "ExpectedBucketOwner": NotRequired[str],
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
     },
 )
-NotificationConfigurationFilterBucketNotificationTypeDef = TypedDict(
-    "NotificationConfigurationFilterBucketNotificationTypeDef",
+NotificationConfigurationFilterExtraOutputTypeDef = TypedDict(
+    "NotificationConfigurationFilterExtraOutputTypeDef",
+    {
+        "Key": NotRequired[S3KeyFilterExtraOutputTypeDef],
+    },
+)
+NotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "NotificationConfigurationFilterOutputTypeDef",
     {
-        "Key": NotRequired[S3KeyFilterBucketNotificationTypeDef],
+        "Key": NotRequired[S3KeyFilterOutputTypeDef],
     },
 )
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": NotRequired[S3KeyFilterTypeDef],
     },
@@ -3813,18 +4037,28 @@
         "NextKeyMarker": str,
         "Prefix": str,
         "Delimiter": str,
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
         "Uploads": List[MultipartUploadTypeDef],
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
+    },
+)
+InventoryS3BucketDestinationOutputTypeDef = TypedDict(
+    "InventoryS3BucketDestinationOutputTypeDef",
+    {
+        "Bucket": str,
+        "Format": InventoryFormatType,
+        "AccountId": NotRequired[str],
+        "Prefix": NotRequired[str],
+        "Encryption": NotRequired[InventoryEncryptionOutputTypeDef],
     },
 )
 InventoryS3BucketDestinationTypeDef = TypedDict(
     "InventoryS3BucketDestinationTypeDef",
     {
         "Bucket": str,
         "Format": InventoryFormatType,
@@ -3858,24 +4092,18 @@
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-LifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleConfigurationTypeDef",
-    {
-        "Rules": Sequence[RuleTypeDef],
-    },
-)
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "Bucket": str,
         "Account": NotRequired[str],
         "StorageClass": NotRequired[StorageClassType],
         "AccessControlTranslation": NotRequired[AccessControlTranslationTypeDef],
@@ -3895,42 +4123,42 @@
 )
 ListObjectsOutputTypeDef = TypedDict(
     "ListObjectsOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
-        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "Contents": NotRequired[List[ObjectTypeDef]],
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
     },
 )
 ListObjectsV2OutputTypeDef = TypedDict(
     "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
-        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "Contents": NotRequired[List[ObjectTypeDef]],
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
     },
 )
 ListObjectVersionsOutputTypeDef = TypedDict(
     "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
         "KeyMarker": str,
@@ -3939,61 +4167,62 @@
         "NextVersionIdMarker": str,
         "Versions": List[ObjectVersionTypeDef],
         "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "CommonPrefixes": NotRequired[List[CommonPrefixTypeDef]],
     },
 )
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
-        "OwnershipControls": OwnershipControlsTypeDef,
+        "OwnershipControls": OwnershipControlsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+OwnershipControlsUnionTypeDef = Union[OwnershipControlsTypeDef, OwnershipControlsOutputTypeDef]
 PutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "PutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
         "OwnershipControls": OwnershipControlsTypeDef,
         "ContentMD5": NotRequired[str],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-LoggingEnabledBucketLoggingTypeDef = TypedDict(
-    "LoggingEnabledBucketLoggingTypeDef",
+LoggingEnabledResponseTypeDef = TypedDict(
+    "LoggingEnabledResponseTypeDef",
     {
         "TargetBucket": str,
+        "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "TargetGrants": NotRequired[Sequence[TargetGrantTypeDef]],
-        "TargetObjectKeyFormat": NotRequired[TargetObjectKeyFormatBucketLoggingTypeDef],
+        "TargetObjectKeyFormat": TargetObjectKeyFormatExtraOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-LoggingEnabledResponseTypeDef = TypedDict(
-    "LoggingEnabledResponseTypeDef",
+LoggingEnabledOutputTypeDef = TypedDict(
+    "LoggingEnabledOutputTypeDef",
     {
         "TargetBucket": str,
-        "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "TargetObjectKeyFormat": TargetObjectKeyFormatBucketLoggingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TargetGrants": NotRequired[List[TargetGrantTypeDef]],
+        "TargetObjectKeyFormat": NotRequired[TargetObjectKeyFormatOutputTypeDef],
     },
 )
 LoggingEnabledTypeDef = TypedDict(
     "LoggingEnabledTypeDef",
     {
         "TargetBucket": str,
         "TargetPrefix": str,
-        "TargetGrants": NotRequired[List[TargetGrantTypeDef]],
+        "TargetGrants": NotRequired[Sequence[TargetGrantTypeDef]],
         "TargetObjectKeyFormat": NotRequired[TargetObjectKeyFormatTypeDef],
     },
 )
 GetBucketWebsiteOutputTypeDef = TypedDict(
     "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
@@ -4008,84 +4237,120 @@
     {
         "ErrorDocument": NotRequired[ErrorDocumentTypeDef],
         "IndexDocument": NotRequired[IndexDocumentTypeDef],
         "RedirectAllRequestsTo": NotRequired[RedirectAllRequestsToTypeDef],
         "RoutingRules": NotRequired[Sequence[RoutingRuleTypeDef]],
     },
 )
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "Rules": List[ServerSideEncryptionRuleTypeDef],
+    },
+)
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
-        "Rules": List[ServerSideEncryptionRuleTypeDef],
+        "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
     },
 )
 SelectObjectContentEventStreamTypeDef = TypedDict(
     "SelectObjectContentEventStreamTypeDef",
     {
         "Records": NotRequired[RecordsEventTypeDef],
         "Stats": NotRequired[StatsEventTypeDef],
         "Progress": NotRequired[ProgressEventTypeDef],
         "Cont": NotRequired[Dict[str, Any]],
         "End": NotRequired[Dict[str, Any]],
     },
 )
+IntelligentTieringConfigurationOutputTypeDef = TypedDict(
+    "IntelligentTieringConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Status": IntelligentTieringStatusType,
+        "Tierings": List[TieringTypeDef],
+        "Filter": NotRequired[IntelligentTieringFilterOutputTypeDef],
+    },
+)
 IntelligentTieringConfigurationTypeDef = TypedDict(
     "IntelligentTieringConfigurationTypeDef",
     {
         "Id": str,
         "Status": IntelligentTieringStatusType,
-        "Tierings": List[TieringTypeDef],
+        "Tierings": Sequence[TieringTypeDef],
         "Filter": NotRequired[IntelligentTieringFilterTypeDef],
     },
 )
-LifecycleRuleBucketLifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleRuleBucketLifecycleConfigurationTypeDef",
+LifecycleRuleExtraOutputTypeDef = TypedDict(
+    "LifecycleRuleExtraOutputTypeDef",
     {
         "Status": ExpirationStatusType,
-        "Expiration": NotRequired[LifecycleExpirationBucketLifecycleConfigurationTypeDef],
+        "Expiration": NotRequired[LifecycleExpirationExtraOutputTypeDef],
         "ID": NotRequired[str],
         "Prefix": NotRequired[str],
-        "Filter": NotRequired[LifecycleRuleFilterBucketLifecycleConfigurationTypeDef],
-        "Transitions": NotRequired[Sequence[TransitionBucketLifecycleConfigurationTypeDef]],
-        "NoncurrentVersionTransitions": NotRequired[Sequence[NoncurrentVersionTransitionTypeDef]],
+        "Filter": NotRequired[LifecycleRuleFilterExtraOutputTypeDef],
+        "Transitions": NotRequired[List[TransitionExtraOutputTypeDef]],
+        "NoncurrentVersionTransitions": NotRequired[List[NoncurrentVersionTransitionTypeDef]],
+        "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
+        "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
+    },
+)
+LifecycleRuleOutputTypeDef = TypedDict(
+    "LifecycleRuleOutputTypeDef",
+    {
+        "Status": ExpirationStatusType,
+        "Expiration": NotRequired[LifecycleExpirationOutputTypeDef],
+        "ID": NotRequired[str],
+        "Prefix": NotRequired[str],
+        "Filter": NotRequired[LifecycleRuleFilterOutputTypeDef],
+        "Transitions": NotRequired[List[TransitionOutputTypeDef]],
+        "NoncurrentVersionTransitions": NotRequired[List[NoncurrentVersionTransitionTypeDef]],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
 LifecycleRuleTypeDef = TypedDict(
     "LifecycleRuleTypeDef",
     {
         "Status": ExpirationStatusType,
         "Expiration": NotRequired[LifecycleExpirationTypeDef],
         "ID": NotRequired[str],
         "Prefix": NotRequired[str],
         "Filter": NotRequired[LifecycleRuleFilterTypeDef],
-        "Transitions": NotRequired[List[TransitionTypeDef]],
-        "NoncurrentVersionTransitions": NotRequired[List[NoncurrentVersionTransitionTypeDef]],
+        "Transitions": NotRequired[Sequence[TransitionTypeDef]],
+        "NoncurrentVersionTransitions": NotRequired[Sequence[NoncurrentVersionTransitionTypeDef]],
         "NoncurrentVersionExpiration": NotRequired[NoncurrentVersionExpirationTypeDef],
         "AbortIncompleteMultipartUpload": NotRequired[AbortIncompleteMultipartUploadTypeDef],
     },
 )
+MetricsConfigurationOutputTypeDef = TypedDict(
+    "MetricsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Filter": NotRequired[MetricsFilterOutputTypeDef],
+    },
+)
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotRequired[MetricsFilterTypeDef],
     },
 )
 StorageClassAnalysisTypeDef = TypedDict(
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": NotRequired[StorageClassAnalysisDataExportTypeDef],
     },
 )
-LifecycleConfigurationBucketLifecycleTypeDef = TypedDict(
-    "LifecycleConfigurationBucketLifecycleTypeDef",
+LifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleConfigurationTypeDef",
     {
-        "Rules": Sequence[RuleBucketLifecycleTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4099,64 +4364,91 @@
         "RequestPayer": NotRequired[Literal["requester"]],
         "Token": NotRequired[str],
         "ContentMD5": NotRequired[str],
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-LambdaFunctionConfigurationBucketNotificationTypeDef = TypedDict(
-    "LambdaFunctionConfigurationBucketNotificationTypeDef",
+LambdaFunctionConfigurationExtraOutputTypeDef = TypedDict(
+    "LambdaFunctionConfigurationExtraOutputTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Id": NotRequired[str],
-        "Filter": NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],
+        "Filter": NotRequired[NotificationConfigurationFilterExtraOutputTypeDef],
     },
 )
-QueueConfigurationBucketNotificationTypeDef = TypedDict(
-    "QueueConfigurationBucketNotificationTypeDef",
+QueueConfigurationExtraOutputTypeDef = TypedDict(
+    "QueueConfigurationExtraOutputTypeDef",
     {
         "QueueArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Id": NotRequired[str],
-        "Filter": NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],
+        "Filter": NotRequired[NotificationConfigurationFilterExtraOutputTypeDef],
     },
 )
-TopicConfigurationBucketNotificationTypeDef = TypedDict(
-    "TopicConfigurationBucketNotificationTypeDef",
+TopicConfigurationExtraOutputTypeDef = TypedDict(
+    "TopicConfigurationExtraOutputTypeDef",
     {
         "TopicArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
+        "Id": NotRequired[str],
+        "Filter": NotRequired[NotificationConfigurationFilterExtraOutputTypeDef],
+    },
+)
+LambdaFunctionConfigurationOutputTypeDef = TypedDict(
+    "LambdaFunctionConfigurationOutputTypeDef",
+    {
+        "LambdaFunctionArn": str,
+        "Events": List[EventType],
+        "Id": NotRequired[str],
+        "Filter": NotRequired[NotificationConfigurationFilterOutputTypeDef],
+    },
+)
+QueueConfigurationOutputTypeDef = TypedDict(
+    "QueueConfigurationOutputTypeDef",
+    {
+        "QueueArn": str,
+        "Events": List[EventType],
         "Id": NotRequired[str],
-        "Filter": NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],
+        "Filter": NotRequired[NotificationConfigurationFilterOutputTypeDef],
+    },
+)
+TopicConfigurationOutputTypeDef = TypedDict(
+    "TopicConfigurationOutputTypeDef",
+    {
+        "TopicArn": str,
+        "Events": List[EventType],
+        "Id": NotRequired[str],
+        "Filter": NotRequired[NotificationConfigurationFilterOutputTypeDef],
     },
 )
 LambdaFunctionConfigurationTypeDef = TypedDict(
     "LambdaFunctionConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Id": NotRequired[str],
         "Filter": NotRequired[NotificationConfigurationFilterTypeDef],
     },
 )
 QueueConfigurationTypeDef = TypedDict(
     "QueueConfigurationTypeDef",
     {
         "QueueArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Id": NotRequired[str],
         "Filter": NotRequired[NotificationConfigurationFilterTypeDef],
     },
 )
 TopicConfigurationTypeDef = TypedDict(
     "TopicConfigurationTypeDef",
     {
         "TopicArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Id": NotRequired[str],
         "Filter": NotRequired[NotificationConfigurationFilterTypeDef],
     },
 )
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
@@ -4222,27 +4514,38 @@
 )
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
         "S3": NotRequired[S3LocationTypeDef],
     },
 )
+InventoryDestinationOutputTypeDef = TypedDict(
+    "InventoryDestinationOutputTypeDef",
+    {
+        "S3BucketDestination": InventoryS3BucketDestinationOutputTypeDef,
+    },
+)
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
     },
 )
-PutBucketLifecycleRequestRequestTypeDef = TypedDict(
-    "PutBucketLifecycleRequestRequestTypeDef",
+ReplicationRuleOutputTypeDef = TypedDict(
+    "ReplicationRuleOutputTypeDef",
     {
-        "Bucket": str,
-        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "LifecycleConfiguration": NotRequired[LifecycleConfigurationTypeDef],
-        "ExpectedBucketOwner": NotRequired[str],
+        "Status": ReplicationRuleStatusType,
+        "Destination": DestinationTypeDef,
+        "ID": NotRequired[str],
+        "Priority": NotRequired[int],
+        "Prefix": NotRequired[str],
+        "Filter": NotRequired[ReplicationRuleFilterOutputTypeDef],
+        "SourceSelectionCriteria": NotRequired[SourceSelectionCriteriaTypeDef],
+        "ExistingObjectReplication": NotRequired[ExistingObjectReplicationTypeDef],
+        "DeleteMarkerReplication": NotRequired[DeleteMarkerReplicationTypeDef],
     },
 )
 ReplicationRuleTypeDef = TypedDict(
     "ReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
         "Destination": DestinationTypeDef,
@@ -4251,33 +4554,27 @@
         "Prefix": NotRequired[str],
         "Filter": NotRequired[ReplicationRuleFilterTypeDef],
         "SourceSelectionCriteria": NotRequired[SourceSelectionCriteriaTypeDef],
         "ExistingObjectReplication": NotRequired[ExistingObjectReplicationTypeDef],
         "DeleteMarkerReplication": NotRequired[DeleteMarkerReplicationTypeDef],
     },
 )
-BucketLoggingStatusBucketLoggingTypeDef = TypedDict(
-    "BucketLoggingStatusBucketLoggingTypeDef",
+GetBucketLoggingOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputTypeDef",
     {
-        "LoggingEnabled": NotRequired[LoggingEnabledBucketLoggingTypeDef],
+        "LoggingEnabled": LoggingEnabledOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 BucketLoggingStatusTypeDef = TypedDict(
     "BucketLoggingStatusTypeDef",
     {
         "LoggingEnabled": NotRequired[LoggingEnabledTypeDef],
     },
 )
-GetBucketLoggingOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputTypeDef",
-    {
-        "LoggingEnabled": LoggingEnabledTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 PutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     {
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
@@ -4290,138 +4587,147 @@
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "PutBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ContentMD5": NotRequired[str],
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
+ServerSideEncryptionConfigurationUnionTypeDef = Union[
+    ServerSideEncryptionConfigurationTypeDef, ServerSideEncryptionConfigurationOutputTypeDef
+]
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
         "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
+        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IntelligentTieringConfigurationUnionTypeDef = Union[
+    IntelligentTieringConfigurationTypeDef, IntelligentTieringConfigurationOutputTypeDef
+]
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
     },
 )
-BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = TypedDict(
-    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
+GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputTypeDef",
     {
-        "Rules": Sequence[LifecycleRuleBucketLifecycleConfigurationTypeDef],
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 BucketLifecycleConfigurationTypeDef = TypedDict(
     "BucketLifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
 )
-GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputTypeDef",
-    {
-        "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
-        "MetricsConfiguration": MetricsConfigurationTypeDef,
+        "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
+        "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+MetricsConfigurationUnionTypeDef = Union[
+    MetricsConfigurationTypeDef, MetricsConfigurationOutputTypeDef
+]
 PutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "MetricsConfiguration": MetricsConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
+AnalyticsConfigurationOutputTypeDef = TypedDict(
+    "AnalyticsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
+        "Filter": NotRequired[AnalyticsFilterOutputTypeDef],
+    },
+)
 AnalyticsConfigurationTypeDef = TypedDict(
     "AnalyticsConfigurationTypeDef",
     {
         "Id": str,
         "StorageClassAnalysis": StorageClassAnalysisTypeDef,
         "Filter": NotRequired[AnalyticsFilterTypeDef],
     },
 )
 PutBucketLifecycleRequestBucketLifecyclePutTypeDef = TypedDict(
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     {
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "LifecycleConfiguration": NotRequired[LifecycleConfigurationBucketLifecycleTypeDef],
+        "LifecycleConfiguration": NotRequired[LifecycleConfigurationTypeDef],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
-NotificationConfigurationBucketNotificationTypeDef = TypedDict(
-    "NotificationConfigurationBucketNotificationTypeDef",
+PutBucketLifecycleRequestRequestTypeDef = TypedDict(
+    "PutBucketLifecycleRequestRequestTypeDef",
     {
-        "TopicConfigurations": NotRequired[Sequence[TopicConfigurationBucketNotificationTypeDef]],
-        "QueueConfigurations": NotRequired[Sequence[QueueConfigurationBucketNotificationTypeDef]],
-        "LambdaFunctionConfigurations": NotRequired[
-            Sequence[LambdaFunctionConfigurationBucketNotificationTypeDef]
-        ],
-        "EventBridgeConfiguration": NotRequired[Mapping[str, Any]],
+        "Bucket": str,
+        "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
+        "LifecycleConfiguration": NotRequired[LifecycleConfigurationTypeDef],
+        "ExpectedBucketOwner": NotRequired[str],
     },
 )
 NotificationConfigurationResponseTypeDef = TypedDict(
     "NotificationConfigurationResponseTypeDef",
     {
-        "TopicConfigurations": List[TopicConfigurationTypeDef],
-        "QueueConfigurations": List[QueueConfigurationTypeDef],
-        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
+        "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
+        "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
+        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
@@ -4439,37 +4745,56 @@
         "Type": NotRequired[Literal["SELECT"]],
         "Tier": NotRequired[TierType],
         "Description": NotRequired[str],
         "SelectParameters": NotRequired[SelectParametersTypeDef],
         "OutputLocation": NotRequired[OutputLocationTypeDef],
     },
 )
+InventoryConfigurationOutputTypeDef = TypedDict(
+    "InventoryConfigurationOutputTypeDef",
+    {
+        "Destination": InventoryDestinationOutputTypeDef,
+        "IsEnabled": bool,
+        "Id": str,
+        "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
+        "Schedule": InventoryScheduleTypeDef,
+        "Filter": NotRequired[InventoryFilterTypeDef],
+        "OptionalFields": NotRequired[List[InventoryOptionalFieldType]],
+    },
+)
 InventoryConfigurationTypeDef = TypedDict(
     "InventoryConfigurationTypeDef",
     {
         "Destination": InventoryDestinationTypeDef,
         "IsEnabled": bool,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "Schedule": InventoryScheduleTypeDef,
         "Filter": NotRequired[InventoryFilterTypeDef],
-        "OptionalFields": NotRequired[List[InventoryOptionalFieldType]],
+        "OptionalFields": NotRequired[Sequence[InventoryOptionalFieldType]],
+    },
+)
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "Role": str,
+        "Rules": List[ReplicationRuleOutputTypeDef],
     },
 )
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": List[ReplicationRuleTypeDef],
+        "Rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 PutBucketLoggingRequestBucketLoggingPutTypeDef = TypedDict(
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     {
-        "BucketLoggingStatus": BucketLoggingStatusBucketLoggingTypeDef,
+        "BucketLoggingStatus": BucketLoggingStatusTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketLoggingRequestRequestTypeDef = TypedDict(
     "PutBucketLoggingRequestRequestTypeDef",
     {
@@ -4479,17 +4804,15 @@
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     {
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
-        "LifecycleConfiguration": NotRequired[
-            BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef
-        ],
+        "LifecycleConfiguration": NotRequired[BucketLifecycleConfigurationTypeDef],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4497,41 +4820,44 @@
         "LifecycleConfiguration": NotRequired[BucketLifecycleConfigurationTypeDef],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
-        "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
+        "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
+        "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AnalyticsConfigurationUnionTypeDef = Union[
+    AnalyticsConfigurationTypeDef, AnalyticsConfigurationOutputTypeDef
+]
 PutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationBucketNotificationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
         "SkipDestinationValidation": NotRequired[bool],
     },
 )
 PutBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     {
@@ -4572,47 +4898,53 @@
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
-        "InventoryConfiguration": InventoryConfigurationTypeDef,
+        "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
-        "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
+        "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+InventoryConfigurationUnionTypeDef = Union[
+    InventoryConfigurationTypeDef, InventoryConfigurationOutputTypeDef
+]
 PutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "InventoryConfiguration": InventoryConfigurationTypeDef,
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
         "ChecksumAlgorithm": NotRequired[ChecksumAlgorithmType],
         "Token": NotRequired[str],
         "ExpectedBucketOwner": NotRequired[str],
     },
 )
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/waiter.py` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3/waiter.pyi` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/PKG-INFO` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.34.65
-Summary: Type annotations for boto3.S3 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.S3 1.34.91 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3)](https://pepy.tech/project/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3-1.34.65/mypy_boto3_s3.egg-info/SOURCES.txt` & `mypy_boto3_s3-1.34.91/mypy_boto3_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.34.65/setup.py` & `mypy_boto3_s3-1.34.91/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3",
-    version="1.34.65",
+    version="1.34.91",
     packages=["mypy_boto3_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.S3 1.34.65 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.S3 1.34.91 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

