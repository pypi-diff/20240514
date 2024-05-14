# Comparing `tmp/test_core_package-0.0.9.tar.gz` & `tmp/test_core_package-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-0.0.9.tar", last modified: Tue May 14 05:25:23 2024, max compression
+gzip compressed data, was "test_core_package-0.1.0.tar", last modified: Tue May 14 07:03:24 2024, max compression
```

## Comparing `test_core_package-0.0.9.tar` & `test_core_package-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.386014 test_core_package-0.0.9/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.9/LICENCE.txt
--rw-rw-rw-   0        0        0      241 2024-05-14 05:25:23.386014 test_core_package-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:22.975067 test_core_package-0.0.9/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.9/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.061498 test_core_package-0.0.9/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.9/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.9/qa_qc_check/controller/checks.json
--rw-rw-rw-   0        0        0     4307 2024-05-13 08:57:22.000000 test_core_package-0.0.9/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     9343 2024-05-13 08:50:49.000000 test_core_package-0.0.9/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1581 2024-05-13 08:51:08.000000 test_core_package-0.0.9/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.085829 test_core_package-0.0.9/qa_qc_check/model/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-0.0.9/qa_qc_check/model/__init__.py
--rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.9/qa_qc_check/model/metadata_model.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.102176 test_core_package-0.0.9/qa_qc_check/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.9/qa_qc_check/tests/__init__.py
--rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.9/qa_qc_check/tests/test_meta_data_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.129851 test_core_package-0.0.9/qa_qc_check/validator/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-0.0.9/qa_qc_check/validator/__init__.py
--rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.9/qa_qc_check/validator/meta_data_validator.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.151820 test_core_package-0.0.9/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.234461 test_core_package-0.0.9/satelite/sentinel2/
--rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.249497 test_core_package-0.0.9/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.315933 test_core_package-0.0.9/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.9/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0       42 2024-05-14 05:25:23.386014 test_core_package-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-14 05:25:19.000000 test_core_package-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:23.382348 test_core_package-0.0.9/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-14 05:25:22.000000 test_core_package-0.0.9/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:24.027385 test_core_package-0.1.0/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.1.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      241 2024-05-14 07:03:24.026365 test_core_package-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.898959 test_core_package-0.1.0/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.1.0/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.930274 test_core_package-0.1.0/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.1.0/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4307 2024-05-13 08:57:22.000000 test_core_package-0.1.0/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     9936 2024-05-14 07:03:21.000000 test_core_package-0.1.0/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1581 2024-05-13 08:51:08.000000 test_core_package-0.1.0/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.936674 test_core_package-0.1.0/qa_qc_check/model/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-0.1.0/qa_qc_check/model/__init__.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.1.0/qa_qc_check/model/metadata_model.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.942249 test_core_package-0.1.0/qa_qc_check/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.1.0/qa_qc_check/tests/__init__.py
+-rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.1.0/qa_qc_check/tests/test_meta_data_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.947262 test_core_package-0.1.0/qa_qc_check/validator/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-0.1.0/qa_qc_check/validator/__init__.py
+-rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.1.0/qa_qc_check/validator/meta_data_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.950921 test_core_package-0.1.0/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.958866 test_core_package-0.1.0/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.962169 test_core_package-0.1.0/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:23.971653 test_core_package-0.1.0/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.1.0/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 07:03:24.028379 test_core_package-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      899 2024-05-14 07:02:58.000000 test_core_package-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:24.021897 test_core_package-0.1.0/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-14 07:03:23.000000 test_core_package-0.1.0/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1080 2024-05-14 07:03:23.000000 test_core_package-0.1.0/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:03:23.000000 test_core_package-0.1.0/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      289 2024-05-14 07:03:23.000000 test_core_package-0.1.0/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-14 07:03:23.000000 test_core_package-0.1.0/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-0.0.9/qa_qc_check/controller/meta_data.py` & `test_core_package-0.1.0/qa_qc_check/controller/meta_data.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/qa_qc_check/controller/meta_data_extractor.py` & `test_core_package-0.1.0/qa_qc_check/controller/meta_data_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import logging
+import os
 from dataclasses import asdict
 from typing import Dict
 
 from qa_qc_check.controller.meta_data import MetaData
-from qa_qc_check.model.metadata_model import MetadataModel, QaQcModel
 from qa_qc_check.controller.qa_qc import QaQc
+from qa_qc_check.model.metadata_model import MetadataModel, QaQcModel
 
 logger = logging.getLogger()
 
 
 class MetadataExtractor:
 
     def __init__(self, file: str, check_type: str):
@@ -17,145 +18,152 @@
 
         Args:
             file (str): S3 File Path
             check_type (str): QA/QC check type
         """
         self.file = file
         self.check_type = check_type
-        # self.checks_json = json.load(open("checks.json", "r"))
-        self.checks_json = {
-            "ndvi": {
-                "entry": {},
-                "exit": {
-                    "filename_parts_count": 3,
-                    "filename_endswith": ".tif",
-                    "filename_date_chars": 8,
-                    "filename_product_code": [
-                        "TCX8021",
-                        "IS18021",
-                        "TCX8020",
-                        "IS18020",
-                    ],
-                    "filename_product_code_count": 7,
-                    "filename_season_code_count": 0,
-                    "filename_season_code_startswith": [""],
-                    "epsg_code_count": 5,
-                    "pixelsize": "10.0 -10.0",
-                    "nodata_value": "0.0",
-                    "values_range": [0, 200],
-                    "compression_type": "LZW",
-                },
-                "product_list": ["TCX8021", "IS18021", "TCX8020", "IS18020"],
-                "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
-            },
-            "ndwi": {
-                "entry": {},
-                "exit": {
-                    "filename_parts_count": 3,
-                    "filename_endswith": ".tif",
-                    "filename_date_chars": 8,
-                    "filename_product_code": [
-                        "TCX9021",
-                        "IS19021",
-                        "TCX9020",
-                        "IS19020",
-                    ],
-                    "filename_product_code_count": 7,
-                    "filename_season_code_count": 0,
-                    "filename_season_code_startswith": [""],
-                    "pixelsize": "10.0 -10.0",
-                    "nodata_value": "0.0",
-                    "values_range": [0, 200],
-                    "compression_type": "LZW",
-                },
-                "product_list": ["TCX9021", "IS19021", "TCX9020", "IS19020"],
-                "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
-            },
-            "mndwi": {
-                "entry": {},
-                "exit": {
-                    "filename_parts_count": 3,
-                    "filename_endswith": ".tif",
-                    "filename_date_chars": 8,
-                    "filename_product_code": [
-                        "TCXD021",
-                        "IS1D021",
-                        "TCXD020",
-                        "IS1D020",
-                    ],
-                    "filename_product_code_count": 7,
-                    "filename_season_code_count": 0,
-                    "filename_season_code_startswith": [""],
-                    "epsg_code_count": 5,
-                    "pixelsize": "10.0 -10.0",
-                    "nodata_value": "0.0",
-                    "values_range": [0, 200],
-                    "compression_type": "LZW",
-                },
-                "product_list": ["TCXD021", "IS1D021", "TCXD020", "IS1D020"],
-                "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
-            },
-            "fcc": {
-                "entry": {},
-                "exit": {
-                    "filename_parts_count": 3,
-                    "filename_endswith": ".tif",
-                    "filename_date_chars": 8,
-                    "filename_product_code": ["IS51010", "IS51011"],
-                    "filename_product_code_count": 7,
-                    "filename_season_code_count": 0,
-                    "filename_season_code_startswith": [""],
-                    "epsg_code_count": 5,
-                    "pixelsize": "10.0 -10.0",
-                    "nodata_value": "0.0",
-                    "values_range": [0, 10000],
-                    "compression_type": "LZW",
-                },
-                "product_list": ["IS51010", "IS51011"],
-                "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
-            },
-            "cs": {
-                "entry": {},
-                "exit": {
-                    "filename_parts_count": 4,
-                    "filename_endswith": ".tif",
-                    "filename_date_chars": 8,
-                    "filename_product_code": ["CS"],
-                    "filename_product_code_count": 7,
-                    "filename_season_code_count": 4,
-                    "filename_season_code_startswith": ["K", "R"],
-                    "epsg_code_count": 5,
-                    "pixelsize": "10.0 -10.0",
-                    "nodata_value": "0.0",
-                    "values_range": [0, 1],
-                    "compression_type": "LZW",
-                },
-                "product_list": ["CS"],
-                "s3_bucket_names": ["satsure-products"],
-            },
-            "ch": {
-                "entry": {},
-                "exit": {
-                    "filename_parts_count": 4,
-                    "filename_endswith": ".tif",
-                    "filename_date_chars": 8,
-                    "filename_product_code": ["CH"],
-                    "filename_product_code_count": 7,
-                    "filename_season_code_count": 4,
-                    "filename_season_code_startswith": ["K", "R"],
-                    "epsg_code_count": 5,
-                    "pixelsize": "10.0 -10.0",
-                    "nodata_value": "0.0",
-                    "values_range": [0, 1],
-                    "compression_type": "LZW",
-                },
-                "product_list": ["CH"],
-                "s3_bucket_names": ["satsure-products"],
-            },
-        }
+        script_dir = os.path.dirname(os.path.abspath(__file__))
+
+        # Path to your JSON file relative to the script's location
+        json_file_path = os.path.join(script_dir, "checks.json")
+
+        # Resolve the absolute path of the JSON file
+        abs_json_file_path = os.path.abspath(json_file_path)
+        self.checks_json = json.load(open(abs_json_file_path, "r"))
+        # self.checks_json = {
+        #     "ndvi": {
+        #         "entry": {},
+        #         "exit": {
+        #             "filename_parts_count": 3,
+        #             "filename_endswith": ".tif",
+        #             "filename_date_chars": 8,
+        #             "filename_product_code": [
+        #                 "TCX8021",
+        #                 "IS18021",
+        #                 "TCX8020",
+        #                 "IS18020",
+        #             ],
+        #             "filename_product_code_count": 7,
+        #             "filename_season_code_count": 0,
+        #             "filename_season_code_startswith": [""],
+        #             "epsg_code_count": 5,
+        #             "pixelsize": "10.0 -10.0",
+        #             "nodata_value": "0.0",
+        #             "values_range": [0, 200],
+        #             "compression_type": "LZW",
+        #         },
+        #         "product_list": ["TCX8021", "IS18021", "TCX8020", "IS18020"],
+        #         "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
+        #     },
+        #     "ndwi": {
+        #         "entry": {},
+        #         "exit": {
+        #             "filename_parts_count": 3,
+        #             "filename_endswith": ".tif",
+        #             "filename_date_chars": 8,
+        #             "filename_product_code": [
+        #                 "TCX9021",
+        #                 "IS19021",
+        #                 "TCX9020",
+        #                 "IS19020",
+        #             ],
+        #             "filename_product_code_count": 7,
+        #             "filename_season_code_count": 0,
+        #             "filename_season_code_startswith": [""],
+        #             "pixelsize": "10.0 -10.0",
+        #             "nodata_value": "0.0",
+        #             "values_range": [0, 200],
+        #             "compression_type": "LZW",
+        #         },
+        #         "product_list": ["TCX9021", "IS19021", "TCX9020", "IS19020"],
+        #         "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
+        #     },
+        #     "mndwi": {
+        #         "entry": {},
+        #         "exit": {
+        #             "filename_parts_count": 3,
+        #             "filename_endswith": ".tif",
+        #             "filename_date_chars": 8,
+        #             "filename_product_code": [
+        #                 "TCXD021",
+        #                 "IS1D021",
+        #                 "TCXD020",
+        #                 "IS1D020",
+        #             ],
+        #             "filename_product_code_count": 7,
+        #             "filename_season_code_count": 0,
+        #             "filename_season_code_startswith": [""],
+        #             "epsg_code_count": 5,
+        #             "pixelsize": "10.0 -10.0",
+        #             "nodata_value": "0.0",
+        #             "values_range": [0, 200],
+        #             "compression_type": "LZW",
+        #         },
+        #         "product_list": ["TCXD021", "IS1D021", "TCXD020", "IS1D020"],
+        #         "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
+        #     },
+        #     "fcc": {
+        #         "entry": {},
+        #         "exit": {
+        #             "filename_parts_count": 3,
+        #             "filename_endswith": ".tif",
+        #             "filename_date_chars": 8,
+        #             "filename_product_code": ["IS51010", "IS51011"],
+        #             "filename_product_code_count": 7,
+        #             "filename_season_code_count": 0,
+        #             "filename_season_code_startswith": [""],
+        #             "epsg_code_count": 5,
+        #             "pixelsize": "10.0 -10.0",
+        #             "nodata_value": "0.0",
+        #             "values_range": [0, 10000],
+        #             "compression_type": "LZW",
+        #         },
+        #         "product_list": ["IS51010", "IS51011"],
+        #         "s3_bucket_names": ["satsure-satimg", "satimg-to-be-deleted"],
+        #     },
+        #     "cs": {
+        #         "entry": {},
+        #         "exit": {
+        #             "filename_parts_count": 4,
+        #             "filename_endswith": ".tif",
+        #             "filename_date_chars": 8,
+        #             "filename_product_code": ["CS"],
+        #             "filename_product_code_count": 7,
+        #             "filename_season_code_count": 4,
+        #             "filename_season_code_startswith": ["K", "R"],
+        #             "epsg_code_count": 5,
+        #             "pixelsize": "10.0 -10.0",
+        #             "nodata_value": "0.0",
+        #             "values_range": [0, 1],
+        #             "compression_type": "LZW",
+        #         },
+        #         "product_list": ["CS"],
+        #         "s3_bucket_names": ["satsure-products"],
+        #     },
+        #     "ch": {
+        #         "entry": {},
+        #         "exit": {
+        #             "filename_parts_count": 4,
+        #             "filename_endswith": ".tif",
+        #             "filename_date_chars": 8,
+        #             "filename_product_code": ["CH"],
+        #             "filename_product_code_count": 7,
+        #             "filename_season_code_count": 4,
+        #             "filename_season_code_startswith": ["K", "R"],
+        #             "epsg_code_count": 5,
+        #             "pixelsize": "10.0 -10.0",
+        #             "nodata_value": "0.0",
+        #             "values_range": [0, 1],
+        #             "compression_type": "LZW",
+        #         },
+        #         "product_list": ["CH"],
+        #         "s3_bucket_names": ["satsure-products"],
+        #     },
+        # }
         self.product = self._fetch_product()
 
     def _fetch_product(self):
         """
         Fetch product name from file path
 
         Returns:
```

### Comparing `test_core_package-0.0.9/qa_qc_check/controller/qa_qc.py` & `test_core_package-0.1.0/qa_qc_check/controller/qa_qc.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/qa_qc_check/model/metadata_model.py` & `test_core_package-0.1.0/qa_qc_check/model/metadata_model.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/qa_qc_check/tests/test_meta_data_extractor.py` & `test_core_package-0.1.0/qa_qc_check/tests/test_meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/qa_qc_check/validator/meta_data_validator.py` & `test_core_package-0.1.0/qa_qc_check/validator/meta_data_validator.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/satelite/config.py` & `test_core_package-0.1.0/satelite/config.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-0.1.0/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-0.1.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/satelite/sentinel2/get_tiles.py` & `test_core_package-0.1.0/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/satelite/tests/conftest.py` & `test_core_package-0.1.0/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-0.1.0/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.9/setup.py` & `test_core_package-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="test_core_package",
-    version="0.0.9",
+    version="0.1.0",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
@@ -26,10 +26,10 @@
         "python-dateutil==2.9.0.post0",
         "s3transfer==0.10.1",
         "six==1.16.0",
         "urllib3==1.26.18",
         "yarl==1.9.4",
     ],
     package_data={
-        "test_core_package": ["qa_qc_check/controller/*.json"],
+        "test_core_package": ["/qa_qc_check/controller/*.json"],
     },
 )
```

### Comparing `test_core_package-0.0.9/test_core_package.egg-info/SOURCES.txt` & `test_core_package-0.1.0/test_core_package.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENCE.txt
 README.md
 setup.py
 qa_qc_check/__init__.py
 qa_qc_check/controller/__init__.py
-qa_qc_check/controller/checks.json
 qa_qc_check/controller/meta_data.py
 qa_qc_check/controller/meta_data_extractor.py
 qa_qc_check/controller/qa_qc.py
 qa_qc_check/model/__init__.py
 qa_qc_check/model/metadata_model.py
 qa_qc_check/tests/__init__.py
 qa_qc_check/tests/test_meta_data_extractor.py
```

