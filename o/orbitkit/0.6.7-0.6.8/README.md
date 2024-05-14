# Comparing `tmp/orbitkit-0.6.7.tar.gz` & `tmp/orbitkit-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.6.7.tar", last modified: Sat May 11 09:01:42 2024, max compression
+gzip compressed data, was "dist/orbitkit-0.6.8.tar", last modified: Tue May 14 05:12:33 2024, max compression
```

## Comparing `orbitkit-0.6.7.tar` & `orbitkit-0.6.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.7/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.7/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-11 09:01:42.000000 orbitkit-0.6.7/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.7/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2024-05-11 05:38:59.000000 orbitkit-0.6.7/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.7/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.7/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.7/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.7/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.7/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/pdf_embedding/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.7/orbitkit/pdf_embedding/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.7/orbitkit/pdf_embedding/pdf_txt_embedding.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
--rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_azure.py
--rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_orbit.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/
--rw-r--r--   0 crown      (501) staff       (20)     1231 2024-05-11 05:36:15.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      785 2024-04-23 09:31:55.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/base.py
--rw-r--r--   0 crown      (501) staff       (20)     4593 2024-05-11 05:36:15.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/cloud_provider.py
--rw-r--r--   0 crown      (501) staff       (20)     4078 2024-05-11 07:46:00.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/core.py
--rw-r--r--   0 crown      (501) staff       (20)       59 2024-04-23 05:22:52.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)     8078 2024-05-10 08:28:59.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/extractors.py
--rw-r--r--   0 crown      (501) staff       (20)      687 2024-05-10 07:36:30.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/utils.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.7/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.7/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.7/orbitkit/util/util_aliyun.py
--rw-r--r--   0 crown      (501) staff       (20)     1000 2024-05-11 08:50:16.000000 orbitkit-0.6.7/orbitkit/util/util_aliyun_oss_simple.py
--rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.7/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.7/orbitkit/util/util_aws_s3_wrapper.py
--rw-r--r--   0 crown      (501) staff       (20)     4698 2023-11-24 05:44:22.000000 orbitkit-0.6.7/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.7/orbitkit/util/util_html.py
--rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.7/orbitkit/util/util_md5.py
--rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.7/orbitkit/util/util_selenium.py
--rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.7/orbitkit/util/util_simple_timer.py
--rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.7/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.7/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1452 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       74 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2024-05-11 09:01:42.000000 orbitkit-0.6.7/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.7/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.8/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.8/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-14 05:12:33.000000 orbitkit-0.6.8/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.8/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2024-05-14 05:12:12.000000 orbitkit-0.6.8/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.8/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.8/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.8/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.8/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.8/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/pdf_embedding/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.8/orbitkit/pdf_embedding/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.8/orbitkit/pdf_embedding/pdf_txt_embedding.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+-rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_azure.py
+-rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_orbit.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/
+-rw-r--r--   0 crown      (501) staff       (20)     1233 2024-05-14 03:51:14.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      785 2024-04-23 09:31:55.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/base.py
+-rw-r--r--   0 crown      (501) staff       (20)     4593 2024-05-11 05:36:15.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/cloud_provider.py
+-rw-r--r--   0 crown      (501) staff       (20)     4078 2024-05-11 07:46:00.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/core.py
+-rw-r--r--   0 crown      (501) staff       (20)       59 2024-04-23 05:22:52.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)     8078 2024-05-10 08:28:59.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/extractors.py
+-rw-r--r--   0 crown      (501) staff       (20)     1002 2024-05-14 04:33:27.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/utils.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.8/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.8/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.8/orbitkit/util/util_aliyun.py
+-rw-r--r--   0 crown      (501) staff       (20)     1000 2024-05-11 08:50:16.000000 orbitkit-0.6.8/orbitkit/util/util_aliyun_oss_simple.py
+-rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.8/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.8/orbitkit/util/util_aws_s3_wrapper.py
+-rw-r--r--   0 crown      (501) staff       (20)     4698 2024-05-14 05:11:29.000000 orbitkit-0.6.8/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.8/orbitkit/util/util_html.py
+-rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.8/orbitkit/util/util_md5.py
+-rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.8/orbitkit/util/util_selenium.py
+-rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.8/orbitkit/util/util_simple_timer.py
+-rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.8/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.8/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1452 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       74 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2024-05-14 05:12:33.000000 orbitkit-0.6.8/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.8/setup.py
```

### Comparing `orbitkit-0.6.7/LICENSE` & `orbitkit-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/PKG-INFO` & `orbitkit-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.7
+Version: 0.6.8
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.7/README.md` & `orbitkit-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/id_srv/id_gen.py` & `orbitkit-0.6.8/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/lark_send/lark.py` & `orbitkit-0.6.8/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_embedding/pdf_txt_embedding.py` & `orbitkit-0.6.8/orbitkit/pdf_embedding/pdf_txt_embedding.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor/exceptions.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_azure.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_azure.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_orbit.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_orbit.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/__init__.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from orbitkit.pdf_extractor_simple.extractors import PyPdfPdfExtractor, MixedPdfPdfExtractor
 
 
 class ExtractPdfSimpleTxtByCloud:
     def __init__(self, *args, **kwargs):
         self.core_pdf_extract = CorePdfExtract(*args, **kwargs)
         # Add extractor
-        self.core_pdf_extract.add_pdf_extractor(PyPdfPdfExtractor())
+        # self.core_pdf_extract.add_pdf_extractor(PyPdfPdfExtractor())
         self.core_pdf_extract.add_pdf_extractor(MixedPdfPdfExtractor(issue_page_per=95))
 
     def pdf_extract(self,
                     cloud_path: str,
                     cloud_txt_path: Optional[str] = None,
                     copy_path: Optional[str] = None,
                     auto_upload: bool = True):
```

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/base.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/cloud_provider.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/core.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/core.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/extractors.py` & `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/extractors.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/__init__.py` & `orbitkit-0.6.8/orbitkit/util/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/common.py` & `orbitkit-0.6.8/orbitkit/util/common.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_aliyun_oss_simple.py` & `orbitkit-0.6.8/orbitkit/util/util_aliyun_oss_simple.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_aws.py` & `orbitkit-0.6.8/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_aws_s3_wrapper.py` & `orbitkit-0.6.8/orbitkit/util/util_aws_s3_wrapper.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_date.py` & `orbitkit-0.6.8/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_md5.py` & `orbitkit-0.6.8/orbitkit/util/util_md5.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_selenium.py` & `orbitkit-0.6.8/orbitkit/util/util_selenium.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_str.py` & `orbitkit-0.6.8/orbitkit/util/util_str.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit/util/util_type_mapping.py` & `orbitkit-0.6.8/orbitkit/util/util_type_mapping.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.6.8/orbitkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.7
+Version: 0.6.8
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.7/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.6.8/orbitkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.7/setup.py` & `orbitkit-0.6.8/setup.py`

 * *Files identical despite different names*

