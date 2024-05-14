# Comparing `tmp/test_core_package-0.0.8.tar.gz` & `tmp/test_core_package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-0.0.8.tar", last modified: Mon May 13 08:53:54 2024, max compression
+gzip compressed data, was "test_core_package-0.0.9.tar", last modified: Tue May 14 05:25:23 2024, max compression
```

## Comparing `test_core_package-0.0.8.tar` & `test_core_package-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.532261 test_core_package-0.0.8/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.8/LICENCE.txt
--rw-rw-rw-   0        0        0      241 2024-05-13 08:53:54.530806 test_core_package-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.464076 test_core_package-0.0.8/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.8/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.471117 test_core_package-0.0.8/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.8/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.8/qa_qc_check/controller/checks.json
--rw-rw-rw-   0        0        0     4305 2024-05-13 08:50:56.000000 test_core_package-0.0.8/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     9343 2024-05-13 08:50:49.000000 test_core_package-0.0.8/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1581 2024-05-13 08:51:08.000000 test_core_package-0.0.8/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.474686 test_core_package-0.0.8/qa_qc_check/model/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-0.0.8/qa_qc_check/model/__init__.py
--rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.8/qa_qc_check/model/metadata_model.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.477686 test_core_package-0.0.8/qa_qc_check/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.8/qa_qc_check/tests/__init__.py
--rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.8/qa_qc_check/tests/test_meta_data_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.479687 test_core_package-0.0.8/qa_qc_check/validator/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-0.0.8/qa_qc_check/validator/__init__.py
--rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.8/qa_qc_check/validator/meta_data_validator.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.481979 test_core_package-0.0.8/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.491095 test_core_package-0.0.8/satelite/sentinel2/
--rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.493115 test_core_package-0.0.8/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.498989 test_core_package-0.0.8/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0       42 2024-05-13 08:53:54.533277 test_core_package-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-13 08:53:07.000000 test_core_package-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.529830 test_core_package-0.0.8/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.386014 test_core_package-0.0.9/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.9/LICENCE.txt
+-rw-rw-rw-   0        0        0      241 2024-05-14 05:25:23.386014 test_core_package-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:22.975067 test_core_package-0.0.9/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.9/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.061498 test_core_package-0.0.9/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.9/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.9/qa_qc_check/controller/checks.json
+-rw-rw-rw-   0        0        0     4307 2024-05-13 08:57:22.000000 test_core_package-0.0.9/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     9343 2024-05-13 08:50:49.000000 test_core_package-0.0.9/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1581 2024-05-13 08:51:08.000000 test_core_package-0.0.9/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.085829 test_core_package-0.0.9/qa_qc_check/model/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-0.0.9/qa_qc_check/model/__init__.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.9/qa_qc_check/model/metadata_model.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.102176 test_core_package-0.0.9/qa_qc_check/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.9/qa_qc_check/tests/__init__.py
+-rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.9/qa_qc_check/tests/test_meta_data_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.129851 test_core_package-0.0.9/qa_qc_check/validator/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-0.0.9/qa_qc_check/validator/__init__.py
+-rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.9/qa_qc_check/validator/meta_data_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.151820 test_core_package-0.0.9/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.234461 test_core_package-0.0.9/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.249497 test_core_package-0.0.9/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.315933 test_core_package-0.0.9/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 05:25:23.386014 test_core_package-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-14 05:25:19.000000 test_core_package-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.382348 test_core_package-0.0.9/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      289 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-0.0.8/qa_qc_check/controller/checks.json` & `test_core_package-0.0.9/qa_qc_check/controller/checks.json`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/qa_qc_check/controller/meta_data.py` & `test_core_package-0.0.9/qa_qc_check/controller/meta_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from os import environ, getenv
 from urllib.parse import urlparse
 
 import boto3
 from botocore.exceptions import ClientError
-from qa_qc_check.model.metadata_model import MetadataModel
 from osgeo import gdal
 
+from qa_qc_check.model.metadata_model import MetadataModel
+
 gdal.UseExceptions()
 gdal.SetConfigOption("AWS_DEFAULT_REGION", "ap-south-1")
 gdal.SetConfigOption(
     "AWS_SECRET_ACCESS_KEY", "O532YGW4+gYA3Y+NhXiI5w6+MjNdyasgdbpE4490"
 )
 gdal.SetConfigOption("AWS_ACCESS_KEY_ID", "AKIAVMZ7IZCPHXL6UY4G")
 gdal.SetConfigOption("AWS_REQUEST_PAYER", "REQUESTER")
```

### Comparing `test_core_package-0.0.8/qa_qc_check/controller/meta_data_extractor.py` & `test_core_package-0.0.9/qa_qc_check/controller/meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/qa_qc_check/controller/qa_qc.py` & `test_core_package-0.0.9/qa_qc_check/controller/qa_qc.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/qa_qc_check/model/metadata_model.py` & `test_core_package-0.0.9/qa_qc_check/model/metadata_model.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/qa_qc_check/tests/test_meta_data_extractor.py` & `test_core_package-0.0.9/qa_qc_check/tests/test_meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/qa_qc_check/validator/meta_data_validator.py` & `test_core_package-0.0.9/qa_qc_check/validator/meta_data_validator.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/satelite/config.py` & `test_core_package-0.0.9/satelite/config.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/satelite/sentinel2/get_tiles.py` & `test_core_package-0.0.9/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/satelite/tests/conftest.py` & `test_core_package-0.0.9/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-0.0.9/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.8/setup.py` & `test_core_package-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="test_core_package",
-    version="0.0.8",
+    version="0.0.9",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
```

### Comparing `test_core_package-0.0.8/test_core_package.egg-info/SOURCES.txt` & `test_core_package-0.0.9/test_core_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

