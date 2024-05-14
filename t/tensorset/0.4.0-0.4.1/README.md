# Comparing `tmp/tensorset-0.4.0.tar.gz` & `tmp/tensorset-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorset-0.4.0.tar", last modified: Sat May 11 03:18:35 2024, max compression
+gzip compressed data, was "tensorset-0.4.1.tar", last modified: Tue May 14 16:52:55 2024, max compression
```

## Comparing `tensorset-0.4.0.tar` & `tensorset-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:35.472149 tensorset-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-11 03:18:35.472149 tensorset-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-11 03:18:31.000000 tensorset-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:18:35.472149 tensorset-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 03:18:31.000000 tensorset-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:35.472149 tensorset-0.4.0/tensorset/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-11 03:18:31.000000 tensorset-0.4.0/tensorset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-11 03:18:31.000000 tensorset-0.4.0/tensorset/tensorsequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:35.472149 tensorset-0.4.0/tensorset/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:31.000000 tensorset-0.4.0/tensorset/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-11 03:18:31.000000 tensorset-0.4.0/tensorset/tests/test_tensorsequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:35.472149 tensorset-0.4.0/tensorset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-11 03:18:35.000000 tensorset-0.4.0/tensorset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-11 03:18:35.000000 tensorset-0.4.0/tensorset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:18:35.000000 tensorset-0.4.0/tensorset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 03:18:35.000000 tensorset-0.4.0/tensorset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 03:18:35.000000 tensorset-0.4.0/tensorset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.732997 tensorset-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-14 16:52:55.732997 tensorset-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-14 16:52:48.000000 tensorset-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:52:55.732997 tensorset-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-14 16:52:48.000000 tensorset-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.728997 tensorset-0.4.1/tensorset/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/tensorset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.732997 tensorset-0.4.1/tensorset/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/tests/test_tensorset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.732997 tensorset-0.4.1/tensorset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/top_level.txt
```

### Comparing `tensorset-0.4.0/PKG-INFO` & `tensorset-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorset
-Version: 0.4.0
+Version: 0.4.1
 Summary: manipulate sets of tensors
 Home-page: https://github.com/theAdamColton/tensorset
 Author: Adam Colton
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.0.1
 
 # tensorset
```

### Comparing `tensorset-0.4.0/README.md` & `tensorset-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tensorset-0.4.0/tensorset/tensorsequence.py` & `tensorset-0.4.1/tensorset/tensorset.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,20 +181,22 @@
         Assign to a new or existing column of this tensorset
         """
         if isinstance(key, int):
             self.columns[key] = item
         elif isinstance(key, str):
             self.named_columns[key] = item
 
-    def to_device(self, device):
+    def to_device(self, device, **kwargs):
         """
         in-place
         """
-        self.columns = [c.to(device) for c in self.columns]
-        self.named_columns = {k: c.to(device) for k, c in self.named_columns.items()}
+        self.columns = [c.to(device, **kwargs) for c in self.columns]
+        self.named_columns = {
+            k: c.to(device, **kwargs) for k, c in self.named_columns.items()
+        }
         return self
 
     def pad(
         self,
         amount: int,
         dim: int,
         value=None,
```

### Comparing `tensorset-0.4.0/tensorset/tests/test_tensorsequence.py` & `tensorset-0.4.1/tensorset/tests/test_tensorset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import torch
-from .. import tensorsequence as ts
+from .. import tensorset as ts
 
 
 class TestTensorSet(unittest.TestCase):
     def assert_error(self, do):
         occurred = False
         try:
             do()
```

### Comparing `tensorset-0.4.0/tensorset.egg-info/PKG-INFO` & `tensorset-0.4.1/tensorset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorset
-Version: 0.4.0
+Version: 0.4.1
 Summary: manipulate sets of tensors
 Home-page: https://github.com/theAdamColton/tensorset
 Author: Adam Colton
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.0.1
 
 # tensorset
```

