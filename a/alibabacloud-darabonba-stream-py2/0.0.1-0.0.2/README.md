# Comparing `tmp/alibabacloud_darabonba_stream_py2-0.0.1.tar.gz` & `tmp/alibabacloud_darabonba_stream_py2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_darabonba_stream_py2-0.0.1.tar", last modified: Mon Jan 24 09:04:26 2022, max compression
+gzip compressed data, was "dist/alibabacloud_darabonba_stream_py2-0.0.2.tar", last modified: Tue May 14 13:40:03 2024, max compression
```

## Comparing `alibabacloud_darabonba_stream_py2-0.0.1.tar` & `alibabacloud_darabonba_stream_py2-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1039 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream/
--rw-r--r--   0 root         (0) root         (0)       22 2022-01-24 09:04:25.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)      623 2022-01-24 09:04:25.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1039 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-24 09:04:26.000000 alibabacloud_darabonba_stream_py2-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2715 2022-01-24 09:04:25.000000 alibabacloud_darabonba_stream_py2-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2715 2024-05-14 13:40:03.000000 alibabacloud_darabonba_stream_py2-0.0.2/setup.py
```

### Comparing `alibabacloud_darabonba_stream_py2-0.0.1/PKG-INFO` & `alibabacloud_darabonba_stream_py2-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_darabonba_stream_py2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alibaba Cloud Darabonba Stream SDK Library for Python2
 Home-page: https://github.com/aliyun/darabonba-stream
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,darabonba,stream,py2
```

### Comparing `alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream/client.py` & `alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,17 @@
     def read_from_file_path(path):
         return open(path, 'rb')
 
     @staticmethod
     def read_from_bytes(raw):
         f = BytesIO()
         f.write(raw)
+        f.seek(0)
         return f
 
     @staticmethod
     def read_from_string(raw):
-        by = bytes(raw, 'utf-8')
-        f = BytesIO()
-        f.write(by)
-        return f
+        return Client.read_from_bytes(bytes(raw, 'utf-8'))
 
     @staticmethod
     def reset(raw):
         raise Exception('Un-implemented')
```

### Comparing `alibabacloud_darabonba_stream_py2-0.0.1/alibabacloud_darabonba_stream_py2.egg-info/PKG-INFO` & `alibabacloud_darabonba_stream_py2-0.0.2/alibabacloud_darabonba_stream_py2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-darabonba-stream-py2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alibaba Cloud Darabonba Stream SDK Library for Python2
 Home-page: https://github.com/aliyun/darabonba-stream
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,darabonba,stream,py2
```

### Comparing `alibabacloud_darabonba_stream_py2-0.0.1/setup.py` & `alibabacloud_darabonba_stream_py2-0.0.2/setup.py`

 * *Files identical despite different names*
