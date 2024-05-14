# Comparing `tmp/test_core_package-0.0.7.tar.gz` & `tmp/test_core_package-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-0.0.7.tar", last modified: Mon May 13 08:51:43 2024, max compression
+gzip compressed data, was "test_core_package-0.0.8.tar", last modified: Mon May 13 08:53:54 2024, max compression
```

## Comparing `test_core_package-0.0.7.tar` & `test_core_package-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.380723 test_core_package-0.0.7/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.7/LICENCE.txt
--rw-rw-rw-   0        0        0      241 2024-05-13 08:51:43.377600 test_core_package-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.273646 test_core_package-0.0.7/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.7/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.299071 test_core_package-0.0.7/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.7/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.7/qa_qc_check/controller/checks.json
--rw-rw-rw-   0        0        0     4305 2024-05-13 08:50:56.000000 test_core_package-0.0.7/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     9343 2024-05-13 08:50:49.000000 test_core_package-0.0.7/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1581 2024-05-13 08:51:08.000000 test_core_package-0.0.7/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.302811 test_core_package-0.0.7/qa_qc_check/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.7/qa_qc_check/tests/__init__.py
--rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.7/qa_qc_check/tests/test_meta_data_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.304835 test_core_package-0.0.7/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.319032 test_core_package-0.0.7/satelite/sentinel2/
--rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/sentinel2/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.323167 test_core_package-0.0.7/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.338563 test_core_package-0.0.7/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.7/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0       42 2024-05-13 08:51:43.381170 test_core_package-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-13 08:51:40.000000 test_core_package-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:51:43.374617 test_core_package-0.0.7/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-13 08:51:43.000000 test_core_package-0.0.7/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      970 2024-05-13 08:51:43.000000 test_core_package-0.0.7/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:51:43.000000 test_core_package-0.0.7/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2024-05-13 08:51:43.000000 test_core_package-0.0.7/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 08:51:43.000000 test_core_package-0.0.7/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.532261 test_core_package-0.0.8/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.8/LICENCE.txt
+-rw-rw-rw-   0        0        0      241 2024-05-13 08:53:54.530806 test_core_package-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.464076 test_core_package-0.0.8/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.8/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.471117 test_core_package-0.0.8/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.8/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.8/qa_qc_check/controller/checks.json
+-rw-rw-rw-   0        0        0     4305 2024-05-13 08:50:56.000000 test_core_package-0.0.8/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     9343 2024-05-13 08:50:49.000000 test_core_package-0.0.8/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1581 2024-05-13 08:51:08.000000 test_core_package-0.0.8/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.474686 test_core_package-0.0.8/qa_qc_check/model/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-0.0.8/qa_qc_check/model/__init__.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.8/qa_qc_check/model/metadata_model.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.477686 test_core_package-0.0.8/qa_qc_check/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.8/qa_qc_check/tests/__init__.py
+-rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.8/qa_qc_check/tests/test_meta_data_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.479687 test_core_package-0.0.8/qa_qc_check/validator/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-0.0.8/qa_qc_check/validator/__init__.py
+-rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.8/qa_qc_check/validator/meta_data_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.481979 test_core_package-0.0.8/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.491095 test_core_package-0.0.8/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.493115 test_core_package-0.0.8/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.498989 test_core_package-0.0.8/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.8/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:53:54.533277 test_core_package-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-13 08:53:07.000000 test_core_package-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:53:54.529830 test_core_package-0.0.8/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      289 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 08:53:54.000000 test_core_package-0.0.8/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-0.0.7/qa_qc_check/controller/checks.json` & `test_core_package-0.0.8/qa_qc_check/controller/checks.json`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/qa_qc_check/controller/meta_data.py` & `test_core_package-0.0.8/qa_qc_check/controller/meta_data.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/qa_qc_check/controller/meta_data_extractor.py` & `test_core_package-0.0.8/qa_qc_check/controller/meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/qa_qc_check/controller/qa_qc.py` & `test_core_package-0.0.8/qa_qc_check/controller/qa_qc.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/qa_qc_check/tests/test_meta_data_extractor.py` & `test_core_package-0.0.8/qa_qc_check/tests/test_meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/satelite/config.py` & `test_core_package-0.0.8/satelite/config.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-0.0.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/satelite/sentinel2/get_tiles.py` & `test_core_package-0.0.8/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/satelite/tests/conftest.py` & `test_core_package-0.0.8/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-0.0.8/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.7/setup.py` & `test_core_package-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="test_core_package",
-    version="0.0.7",
+    version="0.0.8",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
```

### Comparing `test_core_package-0.0.7/test_core_package.egg-info/SOURCES.txt` & `test_core_package-0.0.8/test_core_package.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 setup.py
 qa_qc_check/__init__.py
 qa_qc_check/controller/__init__.py
 qa_qc_check/controller/checks.json
 qa_qc_check/controller/meta_data.py
 qa_qc_check/controller/meta_data_extractor.py
 qa_qc_check/controller/qa_qc.py
+qa_qc_check/model/__init__.py
+qa_qc_check/model/metadata_model.py
 qa_qc_check/tests/__init__.py
 qa_qc_check/tests/test_meta_data_extractor.py
+qa_qc_check/validator/__init__.py
+qa_qc_check/validator/meta_data_validator.py
 satelite/__init__.py
 satelite/config.py
 satelite/sentinel2/__init__.py
 satelite/sentinel2/fetch_unique_tile_date.py
 satelite/sentinel2/fetch_unique_tile_date_pystac.py
 satelite/sentinel2/get_tiles.py
 satelite/tests/__init__.py
```

