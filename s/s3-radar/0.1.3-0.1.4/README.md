# Comparing `tmp/s3_radar-0.1.3.tar.gz` & `tmp/s3_radar-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3_radar-0.1.3.tar", max compression
+gzip compressed data, was "s3_radar-0.1.4.tar", max compression
```

## Comparing `s3_radar-0.1.3.tar` & `s3_radar-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-14 07:45:00.069944 s3_radar-0.1.3/LICENSE
--rw-r--r--   0        0        0      244 2024-05-14 07:41:35.237213 s3_radar-0.1.3/README.md
--rw-r--r--   0        0        0      432 2024-05-14 12:42:18.703001 s3_radar-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 07:43:59.652753 s3_radar-0.1.3/s3_radar/__init__.py
--rw-r--r--   0        0        0     1902 2024-05-14 12:18:27.848150 s3_radar-0.1.3/s3_radar/__main__.py
--rw-r--r--   0        0        0       28 2024-05-14 11:23:46.236589 s3_radar-0.1.3/s3_radar/constants.py
--rw-r--r--   0        0        0      411 2024-05-14 12:07:27.793357 s3_radar-0.1.3/s3_radar/data_generator.py
--rw-r--r--   0        0        0     2227 2024-05-14 12:17:05.141278 s3_radar-0.1.3/s3_radar/s3_client.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 s3_radar-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-14 07:45:00.069944 s3_radar-0.1.4/LICENSE
+-rw-r--r--   0        0        0      244 2024-05-14 07:41:35.237213 s3_radar-0.1.4/README.md
+-rw-r--r--   0        0        0      412 2024-05-14 12:51:22.208239 s3_radar-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 07:43:59.652753 s3_radar-0.1.4/s3_radar/__init__.py
+-rw-r--r--   0        0        0     1902 2024-05-14 12:46:43.357243 s3_radar-0.1.4/s3_radar/__main__.py
+-rw-r--r--   0        0        0       28 2024-05-14 11:23:46.236589 s3_radar-0.1.4/s3_radar/constants.py
+-rw-r--r--   0        0        0      604 2024-05-14 12:50:31.540731 s3_radar-0.1.4/s3_radar/data_generator.py
+-rw-r--r--   0        0        0     2227 2024-05-14 12:17:05.141278 s3_radar-0.1.4/s3_radar/s3_client.py
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 s3_radar-0.1.4/PKG-INFO
```

### Comparing `s3_radar-0.1.3/LICENSE` & `s3_radar-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `s3_radar-0.1.3/s3_radar/__main__.py` & `s3_radar-0.1.4/s3_radar/__main__.py`

 * *Files identical despite different names*

### Comparing `s3_radar-0.1.3/s3_radar/s3_client.py` & `s3_radar-0.1.4/s3_radar/s3_client.py`

 * *Files identical despite different names*

### Comparing `s3_radar-0.1.3/PKG-INFO` & `s3_radar-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: s3-radar
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Ilya Kochankov
 Author-email: ilyakochankov@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.104,<2.0.0)
-Requires-Dist: mimesis (>=16.0.0,<17.0.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # :package:  S3 radar
 
 Simple cli tool for measurement s3 network bandwidth
```

