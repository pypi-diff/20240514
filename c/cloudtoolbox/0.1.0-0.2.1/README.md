# Comparing `tmp/cloudtoolbox-0.1.0.tar.gz` & `tmp/cloudtoolbox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudtoolbox-0.1.0.tar", last modified: Mon May 13 19:50:40 2024, max compression
+gzip compressed data, was "cloudtoolbox-0.2.1.tar", last modified: Mon May 13 23:52:00 2024, max compression
```

## Comparing `cloudtoolbox-0.1.0.tar` & `cloudtoolbox-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/cloud/amazon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/amazon/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/cloud/google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/google/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/google/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/cloud/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/cloudtoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 19:50:40.000000 cloudtoolbox-0.1.0/cloudtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 19:50:40.000000 cloudtoolbox-0.1.0/cloudtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:50:40.000000 cloudtoolbox-0.1.0/cloudtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 19:50:40.000000 cloudtoolbox-0.1.0/cloudtoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 19:50:40.000000 cloudtoolbox-0.1.0/cloudtoolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:50:40.343963 cloudtoolbox-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-13 19:50:11.000000 cloudtoolbox-0.1.0/tests/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:52:00.321911 cloudtoolbox-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-13 23:52:00.317911 cloudtoolbox-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:52:00.317911 cloudtoolbox-0.2.1/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:52:00.317911 cloudtoolbox-0.2.1/cloud/amazon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/amazon/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/amazon/sns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/amazon/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:52:00.317911 cloudtoolbox-0.2.1/cloud/google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/google/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/google/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/cloud/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:52:00.317911 cloudtoolbox-0.2.1/cloudtoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-13 23:52:00.000000 cloudtoolbox-0.2.1/cloudtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 23:52:00.000000 cloudtoolbox-0.2.1/cloudtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 23:52:00.000000 cloudtoolbox-0.2.1/cloudtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-13 23:52:00.000000 cloudtoolbox-0.2.1/cloudtoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 23:52:00.000000 cloudtoolbox-0.2.1/cloudtoolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 23:52:00.321911 cloudtoolbox-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:52:00.317911 cloudtoolbox-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 23:51:33.000000 cloudtoolbox-0.2.1/tests/test_factory.py
```

### Comparing `cloudtoolbox-0.1.0/LICENSE` & `cloudtoolbox-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudtoolbox-0.1.0/cloud/factory.py` & `cloudtoolbox-0.2.1/cloud/factory.py`

 * *Files identical despite different names*

### Comparing `cloudtoolbox-0.1.0/tests/test_factory.py` & `cloudtoolbox-0.2.1/tests/test_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from unittest import mock
 
 from cloud import factory
-from cloud.amazon import s3
+from cloud.amazon import s3, sns, sqs
 from cloud.google import pubsub, storage
 from cloud.protocols import MessagePublisher, StorageUploader
 
 
 class NotStorageUploader:
     def upload_file(self):
         pass
@@ -46,12 +46,22 @@
     def test_google_publisher(self, _):
         Publisher = factory.message_publisher(pubsub.Publisher)
         publisher = Publisher()
 
         self.assertIsInstance(publisher, MessagePublisher)
         self.assertIsInstance(publisher, pubsub.Publisher)
 
+    @mock.patch("boto3.client")
+    def test_amazon_publisher(self, _):
+        for cls in (sns.Publisher, sqs.Publisher):
+            with self.subTest(class_name=cls.__name__):
+                Publisher = factory.message_publisher(cls)
+                publisher = Publisher()
+
+                self.assertIsInstance(publisher, MessagePublisher)
+                self.assertIsInstance(publisher, cls)
+
     def test_publisher_protocol_validation(self):
         error = "NotMessagePublisher does not implement MessagePublisher protocol"
 
         with self.assertRaisesRegex(AssertionError, error):
             factory.message_publisher(NotMessagePublisher)  # type: ignore
```

