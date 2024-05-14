# Comparing `tmp/s3_radar-0.1.1.tar.gz` & `tmp/s3_radar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3_radar-0.1.1.tar", max compression
+gzip compressed data, was "s3_radar-0.1.2.tar", max compression
```

## Comparing `s3_radar-0.1.1.tar` & `s3_radar-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-14 07:45:00.069944 s3_radar-0.1.1/LICENSE
--rw-r--r--   0        0        0      244 2024-05-14 07:41:35.237213 s3_radar-0.1.1/README.md
--rw-r--r--   0        0        0      435 2024-05-14 12:36:07.016469 s3_radar-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 07:43:59.652753 s3_radar-0.1.1/s3_radar/__init__.py
--rw-r--r--   0        0        0     1902 2024-05-14 12:18:27.848150 s3_radar-0.1.1/s3_radar/__main__.py
--rw-r--r--   0        0        0       28 2024-05-14 11:23:46.236589 s3_radar-0.1.1/s3_radar/constants.py
--rw-r--r--   0        0        0      411 2024-05-14 12:07:27.793357 s3_radar-0.1.1/s3_radar/data_generator.py
--rw-r--r--   0        0        0     2227 2024-05-14 12:17:05.141278 s3_radar-0.1.1/s3_radar/s3_client.py
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 s3_radar-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-14 07:45:00.069944 s3_radar-0.1.2/LICENSE
+-rw-r--r--   0        0        0      244 2024-05-14 07:41:35.237213 s3_radar-0.1.2/README.md
+-rw-r--r--   0        0        0      432 2024-05-14 12:38:35.861966 s3_radar-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 07:43:59.652753 s3_radar-0.1.2/s3_radar/__init__.py
+-rw-r--r--   0        0        0     1902 2024-05-14 12:18:27.848150 s3_radar-0.1.2/s3_radar/__main__.py
+-rw-r--r--   0        0        0       28 2024-05-14 11:23:46.236589 s3_radar-0.1.2/s3_radar/constants.py
+-rw-r--r--   0        0        0      411 2024-05-14 12:07:27.793357 s3_radar-0.1.2/s3_radar/data_generator.py
+-rw-r--r--   0        0        0     2227 2024-05-14 12:17:05.141278 s3_radar-0.1.2/s3_radar/s3_client.py
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 s3_radar-0.1.2/PKG-INFO
```

### Comparing `s3_radar-0.1.1/LICENSE` & `s3_radar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3_radar-0.1.1/s3_radar/__main__.py` & `s3_radar-0.1.2/s3_radar/__main__.py`

 * *Files identical despite different names*

### Comparing `s3_radar-0.1.1/s3_radar/s3_client.py` & `s3_radar-0.1.2/s3_radar/s3_client.py`

 * *Files identical despite different names*

### Comparing `s3_radar-0.1.1/PKG-INFO` & `s3_radar-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3-radar
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Ilya Kochankov
 Author-email: ilyakochankov@yandex.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

