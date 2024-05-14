# Comparing `tmp/ras_stac-0.1.0b1.tar.gz` & `tmp/ras_stac-0.1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ras_stac-0.1.0b1.tar", last modified: Mon May 13 15:43:34 2024, max compression
+gzip compressed data, was "ras_stac-0.1.1b1.tar", last modified: Tue May 14 19:04:05 2024, max compression
```

## Comparing `ras_stac-0.1.0b1.tar` & `ras_stac-0.1.1b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:43:34.962892 ras_stac-0.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 15:43:34.962892 ras_stac-0.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:43:34.958892 ras_stac-0.1.0b1/ras_stac/
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/ras_geom_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/ras_plan_dg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/ras_plan_hdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:43:34.962892 ras_stac-0.1.0b1/ras_stac/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/utils/data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/utils/dg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/utils/ras_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/utils/ras_stac.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-05-13 15:43:22.000000 ras_stac-0.1.0b1/ras_stac/utils/s3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:43:34.962892 ras_stac-0.1.0b1/ras_stac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 15:43:34.000000 ras_stac-0.1.0b1/ras_stac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-13 15:43:34.000000 ras_stac-0.1.0b1/ras_stac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:43:34.000000 ras_stac-0.1.0b1/ras_stac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 15:43:34.000000 ras_stac-0.1.0b1/ras_stac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 15:43:34.000000 ras_stac-0.1.0b1/ras_stac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:43:34.962892 ras_stac-0.1.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:04:05.355427 ras_stac-0.1.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 19:04:05.355427 ras_stac-0.1.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:04:05.351427 ras_stac-0.1.1b1/ras_stac/
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/ras_geom_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/ras_plan_dg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/ras_plan_hdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:04:05.355427 ras_stac-0.1.1b1/ras_stac/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/utils/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/utils/dg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/utils/ras_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/utils/ras_stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-14 19:03:49.000000 ras_stac-0.1.1b1/ras_stac/utils/s3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:04:05.355427 ras_stac-0.1.1b1/ras_stac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 19:04:05.000000 ras_stac-0.1.1b1/ras_stac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 19:04:05.000000 ras_stac-0.1.1b1/ras_stac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:04:05.000000 ras_stac-0.1.1b1/ras_stac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 19:04:05.000000 ras_stac-0.1.1b1/ras_stac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 19:04:05.000000 ras_stac-0.1.1b1/ras_stac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:04:05.355427 ras_stac-0.1.1b1/setup.cfg
```

### Comparing `ras_stac-0.1.0b1/LICENSE` & `ras_stac-0.1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ras_stac-0.1.0b1/PKG-INFO` & `ras_stac-0.1.1b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ras-stac
-Version: 0.1.0b1
+Version: 0.1.1b1
 Summary: Create SpatioTemporal Asset Catalog (STAC) objects from HEC-RAS model data.
 Maintainer-email: Seth Lawler <slawler@dewberry.com>
 License: MIT
 Project-URL: repository, https://github.com/fema-ffrd/ras-stac
 Keywords: hec-ras,catalog,STAC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,26 +13,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5py
-Requires-Dist: geopandas
-Requires-Dist: s3fs
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: fsspec
-Requires-Dist: h5py
 Requires-Dist: mypy
 Requires-Dist: numpy
 Requires-Dist: papipyplug
 Requires-Dist: python-dotenv
-Requires-Dist: pyproj
 Requires-Dist: pystac
 Requires-Dist: shapely
 Requires-Dist: rasterio
 Requires-Dist: rashdf
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
@@ -40,15 +35,15 @@
 # ras-stac
 [![CI](https://github.com/fema-ffrd/rashdf/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/fema-ffrd/ras-stac/actions/workflows/continuous-integration.yml)
 [![Release](https://github.com/fema-ffrd/ras-stac/actions/workflows/release.yml/badge.svg)](https://github.com/fema-ffrd/ras-stac/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/ras-stac.svg)](https://badge.fury.io/py/ras-stac)
 
 Utilities for making SpatioTemporal Asset Catalogs of HEC-RAS models
 
-This repository contains code for developing STAC items from HEC-RAS models. Current activities focus on creating items for geometry files `g**.hdf` stored in AWS S3. More to come. 
+This repository contains code for developing STAC items from HEC-RAS models. Current activities focus on creating items for geometry files `g**.hdf` and plan files `p**.hdf stored in AWS S3. More to come. 
 
 *Source code largely ported from [ffrd-stac](https://github.com/arc-pts/ffrd-stac/blob/204e1ec85068936856b317fa9446da3c4da5d8d4/ffrd_stac/rasmeta.py).*
 
 
 ## Getting Started
 
 1. For local development, create a `.env` file using the `example.env` file.
```

### Comparing `ras_stac-0.1.0b1/README.md` & `ras_stac-0.1.1b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ras-stac
 [![CI](https://github.com/fema-ffrd/rashdf/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/fema-ffrd/ras-stac/actions/workflows/continuous-integration.yml)
 [![Release](https://github.com/fema-ffrd/ras-stac/actions/workflows/release.yml/badge.svg)](https://github.com/fema-ffrd/ras-stac/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/ras-stac.svg)](https://badge.fury.io/py/ras-stac)
 
 Utilities for making SpatioTemporal Asset Catalogs of HEC-RAS models
 
-This repository contains code for developing STAC items from HEC-RAS models. Current activities focus on creating items for geometry files `g**.hdf` stored in AWS S3. More to come. 
+This repository contains code for developing STAC items from HEC-RAS models. Current activities focus on creating items for geometry files `g**.hdf` and plan files `p**.hdf stored in AWS S3. More to come. 
 
 *Source code largely ported from [ffrd-stac](https://github.com/arc-pts/ffrd-stac/blob/204e1ec85068936856b317fa9446da3c4da5d8d4/ffrd_stac/rasmeta.py).*
 
 
 ## Getting Started
 
 1. For local development, create a `.env` file using the `example.env` file.
```

### Comparing `ras_stac-0.1.0b1/pyproject.toml` & `ras_stac-0.1.1b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.1.0-beta.1"
+version = "0.1.1-beta.1"
 requires-python = ">=3.9"
-dependencies = ["h5py", "geopandas", "s3fs", "boto3", "botocore", "fsspec", "h5py", "mypy", "numpy", "papipyplug",
-               "python-dotenv", "pyproj", "pystac", "shapely", "rasterio", "rashdf"]
+dependencies = ["boto3", "botocore", "fsspec", "mypy", "numpy", "papipyplug",
+               "python-dotenv", "pystac", "shapely", "rasterio", "rashdf"]
 
 [project.optional-dependencies]
 dev = ["pre-commit", "ruff"]
 
 [project.urls]
 repository = "https://github.com/fema-ffrd/ras-stac"
```

### Comparing `ras_stac-0.1.0b1/ras_stac/ras_geom_hdf.py` & `ras_stac-0.1.1b1/ras_stac/ras_geom_hdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import logging
-from .utils.s3_utils import *
-from .utils.ras_hdf import *
-from .utils.ras_stac import *
-
-from dotenv import find_dotenv, load_dotenv
 import numpy as np
-from .utils.common import check_params, GEOM_HDF_IGNORE_PROPERTIES
-import logging
+import pystac
 import sys
-from papipyplug import parse_input, plugin_logger, print_results
+
 from dotenv import load_dotenv, find_dotenv
+from papipyplug import parse_input, plugin_logger, print_results
+from typing import List
+
+from .utils.common import check_params, GEOM_HDF_IGNORE_PROPERTIES
+from .utils.ras_stac import create_model_item, new_geom_assets, ras_geom_asset_info
+from .utils.s3_utils import (
+    verify_safe_prefix,
+    s3_key_public_url_converter,
+    split_s3_key,
+    init_s3_resources,
+    get_basic_object_metadata,
+    copy_item_to_s3,
+)
 
 logging.getLogger("boto3").setLevel(logging.WARNING)
 logging.getLogger("botocore").setLevel(logging.WARNING)
 
 # Set up logging
 logging.basicConfig(
     level=logging.INFO,
@@ -33,28 +40,32 @@
     other_assets: list = None,
     item_props_to_remove: List = None,
     item_props_to_add: dict = None,
     minio_mode=False,
 ):
     verify_safe_prefix(new_item_s3_key)
     logging.info(f"Creating geom item: {new_item_s3_key}")
-    item_public_url = s3_key_public_url_converter(new_item_s3_key, minio_mode=minio_mode)
+    item_public_url = s3_key_public_url_converter(
+        new_item_s3_key, minio_mode=minio_mode
+    )
     logging.debug(f"item_public_url: {item_public_url}")
 
     # Prep parameters
     bucket_name, _ = split_s3_key(geom_hdf)
     other_assets.append(geom_hdf)
 
     _, s3_client, s3_resource = init_s3_resources(minio_mode=minio_mode)
     bucket = s3_resource.Bucket(bucket_name)
     # Create geometry item
     if item_props_to_remove:
         item = create_model_item(geom_hdf, item_props_to_remove, minio_mode=minio_mode)
     else:
-        item = create_model_item(geom_hdf, GEOM_HDF_IGNORE_PROPERTIES, minio_mode=minio_mode)
+        item = create_model_item(
+            geom_hdf, GEOM_HDF_IGNORE_PROPERTIES, minio_mode=minio_mode
+        )
 
     if item_props_to_add:
         item.properties.update(item_props_to_add)
     # Create list of assets to add to item
     geom_assets = new_geom_assets(
         topo_assets=topo_assets,
         lulc_assets=lulc_assets,
@@ -67,16 +78,16 @@
         logging.debug(asset_type)
         for asset_file in asset_list:
             _, asset_key = split_s3_key(asset_file)
             logging.info(f"Adding asset {asset_file} to item")
             obj = bucket.Object(asset_key)
             try:
                 metadata = get_basic_object_metadata(obj)
-            except:
-                logging.error(f"unable to fetch metadata for :{obj}")
+            except Exception as e:
+                logging.error(f"unable to fetch metadata for {obj}:{e}")
                 metadata = {}
             asset_info = ras_geom_asset_info(asset_file, asset_type)
             asset = pystac.Asset(
                 s3_key_public_url_converter(asset_file, minio_mode=minio_mode),
                 extra_fields=metadata,
                 roles=asset_info["roles"],
                 description=asset_info["description"],
```

### Comparing `ras_stac-0.1.0b1/ras_stac/ras_plan_dg.py` & `ras_stac-0.1.1b1/ras_stac/ras_plan_dg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import logging
+import pystac
 import sys
-from .utils.s3_utils import *
-from .utils.dg_utils import *
-from .utils.ras_stac import *
-from pathlib import Path
-from rasterio.session import AWSSession
+
 from dotenv import find_dotenv, load_dotenv
-import numpy as np
-from .utils.common import check_params, PLAN_HDF_IGNORE_PROPERTIES
+from rasterio.session import AWSSession
 from papipyplug import parse_input, plugin_logger, print_results
+
+from .utils.common import check_params
 from .utils.dg_utils import create_depth_grid_item
+from utils.ras_stac import ras_plan_asset_info
+from .utils.s3_utils import (
+    verify_safe_prefix,
+    s3_key_public_url_converter,
+    split_s3_key,
+    init_s3_resources,
+    get_basic_object_metadata,
+    copy_item_to_s3,
+)
 
 logging.getLogger("boto3").setLevel(logging.WARNING)
 logging.getLogger("botocore").setLevel(logging.WARNING)
 
 # Set up logging
 logging.basicConfig(
     level=logging.INFO,
@@ -30,16 +37,20 @@
     item_props: dict = None,
     asset_list: list = None,
     minio_mode: bool = False,
 ):
     logging.info("Creating plan item")
     verify_safe_prefix(new_dg_item_s3_key)
 
-    dg_item_public_url = s3_key_public_url_converter(new_dg_item_s3_key, minio_mode=minio_mode)
-    plan_item_public_url = s3_key_public_url_converter(plan_item_s3_key, minio_mode=minio_mode)
+    dg_item_public_url = s3_key_public_url_converter(
+        new_dg_item_s3_key, minio_mode=minio_mode
+    )
+    plan_item_public_url = s3_key_public_url_converter(
+        plan_item_s3_key, minio_mode=minio_mode
+    )
 
     # Prep parameters
     bucket_name, _ = split_s3_key(plan_dg)
 
     # Instantitate S3 resources
     session, s3_client, s3_resource = init_s3_resources(minio_mode)
     bucket = s3_resource.Bucket(bucket_name)
```

### Comparing `ras_stac-0.1.0b1/ras_stac/ras_plan_hdf.py` & `ras_stac-0.1.1b1/ras_stac/ras_plan_hdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 import logging
+import pystac
 import sys
-from .utils.s3_utils import *
-from .utils.ras_hdf import *
-from .utils.ras_stac import *
-from pathlib import Path
-from rasterio.session import AWSSession
+
 from dotenv import find_dotenv, load_dotenv
-import numpy as np
-from .utils.common import check_params, PLAN_HDF_IGNORE_PROPERTIES
 from papipyplug import parse_input, plugin_logger, print_results
+from typing import List
+
+from .utils.common import check_params, PLAN_HDF_IGNORE_PROPERTIES
+from .utils.ras_stac import (
+    get_simulation_metadata,
+    create_model_simulation_item,
+    ras_plan_asset_info,
+)
+from .utils.s3_utils import (
+    verify_safe_prefix,
+    s3_key_public_url_converter,
+    split_s3_key,
+    init_s3_resources,
+    get_basic_object_metadata,
+    copy_item_to_s3,
+)
+
 
 logging.getLogger("boto3").setLevel(logging.WARNING)
 logging.getLogger("botocore").setLevel(logging.WARNING)
 
 # Set up logging
 logging.basicConfig(
     level=logging.INFO,
@@ -28,43 +40,52 @@
     sim_id: str,
     asset_list: list = None,
     item_props: dict = None,
     item_props_to_remove: List = None,
     minio_mode: bool = False,
 ):
     verify_safe_prefix(new_plan_item_s3_key)
-    plan_item_public_url = s3_key_public_url_converter(new_plan_item_s3_key, minio_mode=minio_mode)
-    geom_item_public_url = s3_key_public_url_converter(geom_item_s3_key, minio_mode=minio_mode)
+    plan_item_public_url = s3_key_public_url_converter(
+        new_plan_item_s3_key, minio_mode=minio_mode
+    )
+    geom_item_public_url = s3_key_public_url_converter(
+        geom_item_s3_key, minio_mode=minio_mode
+    )
 
     # Prep parameters
     bucket_name, _ = split_s3_key(plan_hdf)
     asset_list.append(plan_hdf)
 
     # Instantitate S3 resources
     session, s3_client, s3_resource = init_s3_resources(minio_mode)
     bucket = s3_resource.Bucket(bucket_name)
-    AWS_SESSION = AWSSession(session)
+    # AWSSession(session)
 
     logging.info("Creating plan item")
 
     # Create geometry item
     geom_item = pystac.Item.from_file(geom_item_public_url)
 
     logging.info("fetching plan metadata")
     plan_meta = get_simulation_metadata(plan_hdf, sim_id, minio_mode=minio_mode)
     if plan_meta:
         try:
             logging.info("creating plan item")
             if item_props_to_remove:
-                plan_item = create_model_simulation_item(geom_item, plan_meta, sim_id, item_props_to_remove)
+                plan_item = create_model_simulation_item(
+                    geom_item, plan_meta, sim_id, item_props_to_remove
+                )
             else:
-                plan_item = create_model_simulation_item(geom_item, plan_meta, sim_id, PLAN_HDF_IGNORE_PROPERTIES)
+                plan_item = create_model_simulation_item(
+                    geom_item, plan_meta, sim_id, PLAN_HDF_IGNORE_PROPERTIES
+                )
         except TypeError:
             return logging.error(
-                f"unable to retrieve model results with geom data from {geom_item_public_url} and metadata from {plan_hdf}. please verify plan was executed and results exist"
+                f"unable to retrieve model results with geom data from {geom_item_public_url} and metadata \
+                    from {plan_hdf}. please verify plan was executed and results exist"
             )
     else:
         raise AttributeError(f"No simulation metadata retrieved from {plan_hdf}")
 
     plan_item.add_derived_from(geom_item)
     plan_item.properties.update(item_props)
```

### Comparing `ras_stac-0.1.0b1/ras_stac/utils/common.py` & `ras_stac-0.1.1b1/ras_stac/utils/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 import inspect
 
 
 def check_params(func):
     sig = inspect.signature(func)
     args = sig.parameters
 
-    required = [name for name, param in args.items() if param.default == inspect.Parameter.empty]
-    optional = [name for name, param in args.items() if param.default != inspect.Parameter.empty]
+    required = [
+        name for name, param in args.items() if param.default == inspect.Parameter.empty
+    ]
+    optional = [
+        name for name, param in args.items() if param.default != inspect.Parameter.empty
+    ]
 
     return {"required": required, "optional": optional}
 
 
 def get_dict_values(dicts: List[dict], key: Any) -> list:
     """
     This function retrieves the values of a specific key from a list of dictionaries.
 
     Parameters:
         dicts (List[dict]): The list of dictionaries.
         key (Any): The key to retrieve the values of.
 
     Returns:
-        List[dict]: A list with the values of the key in the dictionaries. If a dictionary does not have the key, it is skipped.
+        List[dict]: A list with the values of the key in the dictionaries. If a dictionary
+        does not have the key, it is skipped.
     """
     results = []
     for d in dicts:
         if key in d:
             results.append(d[key])
     return results
```

### Comparing `ras_stac-0.1.0b1/ras_stac/utils/data_model.py` & `ras_stac-0.1.1b1/ras_stac/utils/data_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         other_assets: list,
     ) -> dict:
         """
         Expects keys: "prefix/file.ext"
         """
         topo_assets = [f"s3://{self.source_bucket_name}/{a}" for a in topo_assets]
         lulc_assets = [f"s3://{self.source_bucket_name}/{a}" for a in lulc_assets]
-        mannings_assets = [f"s3://{self.source_bucket_name}/{a}" for a in mannings_assets]
+        mannings_assets = [
+            f"s3://{self.source_bucket_name}/{a}" for a in mannings_assets
+        ]
         other_assets = [f"s3://{self.source_bucket_name}/{a}" for a in other_assets]
 
         return {
             "geom_hdf": f"s3://{self.source_bucket_name}/{geom_hdf}",
             "new_item_s3_key": f"s3://{self.stac_bucket_name}/{new_item_s3_key}",
             "topo_assets": topo_assets,
             "mannings_assets": mannings_assets,
```

### Comparing `ras_stac-0.1.0b1/ras_stac/utils/dg_utils.py` & `ras_stac-0.1.1b1/ras_stac/utils/dg_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,98 @@
-import boto3
-from dotenv import load_dotenv
-import pystac
-from pathlib import Path
 import json
-from datetime import datetime
-from typing import Tuple, Dict
-import shapely
-from shapely.geometry import shape, box
-import shapely.ops
+import logging
+import os
+import pystac
 import rasterio
-from rasterio.session import AWSSession
-import rasterio.warp
-from dataclasses import dataclass
+
+from datetime import datetime
 from mypy_boto3_s3.service_resource import Object
+from pathlib import Path
 from rasterio.session import AWSSession
-from .s3_utils import *
-from rasterio.session import AWSSession
-import logging
+from shapely import to_geojson
+from shapely.geometry import Polygon
+from typing import Tuple
+
+from .s3_utils import s3_key_public_url_converter, get_basic_object_metadata
 
 logging.getLogger("boto3").setLevel(logging.WARNING)
 logging.getLogger("botocore").setLevel(logging.WARNING)
 
 
 def get_raster_bounds(
     s3_key: str, aws_session: AWSSession, minio_mode: bool = False
 ) -> Tuple[float, float, float, float]:
     """
-    This function retrieves the geographic bounds of a raster file stored in an AWS S3 bucket and returns them in the WGS 84 (EPSG:4326) coordinate reference system.
+    This function retrieves the geographic bounds of a raster file stored in an AWS S3 bucket and returns them in
+    the WGS 84 (EPSG:4326) coordinate reference system.
 
     Parameters:
         s3_key (str): The key of the raster file in the S3 bucket.
         aws_session (AWSSession): The AWS session to use to access the S3 bucket.
 
     Returns:
-        Tuple[float, float, float, float]: The geographic bounds of the raster file in the WGS 84 (EPSG:4326) coordinate reference system. The bounds are returned as a tuple of four floats: (west, south, east, north).
+        Tuple[float, float, float, float]: The geographic bounds of the raster file in the WGS 84 (EPSG:4326)
+        coordinate reference system. The bounds are returned as a tuple of four floats: (west, south, east, north).
     """
     if minio_mode:
-        with rasterio.open(s3_key.replace("s3://", f"/vsicurl/{os.environ.get('MINIO_S3_ENDPOINT')}/")) as src:
+        with rasterio.open(
+            s3_key.replace("s3://", f"/vsicurl/{os.environ.get('MINIO_S3_ENDPOINT')}/")
+        ) as src:
             bounds = src.bounds
             crs = src.crs
             bounds_4326 = rasterio.warp.transform_bounds(crs, "EPSG:4326", *bounds)
             return bounds_4326
 
     else:
         with rasterio.Env(aws_session):
             with rasterio.open(s3_key) as src:
                 bounds = src.bounds
                 crs = src.crs
                 bounds_4326 = rasterio.warp.transform_bounds(crs, "EPSG:4326", *bounds)
                 return bounds_4326
 
 
-def get_raster_metadata(s3_key: str, aws_session: AWSSession, minio_mode: bool = False) -> dict:
+def get_raster_metadata(
+    s3_key: str, aws_session: AWSSession, minio_mode: bool = False
+) -> dict:
     """
     This function retrieves the metadata of a raster file stored in an AWS S3 bucket.
 
     Parameters:
         s3_key (str): The key of the raster file in the S3 bucket.
         aws_session (AWSSession): The AWS session to use to access the S3 bucket.
 
     Returns:
         dict: The metadata of the raster file. The metadata is returned as a dictionary
         where the keys are the names of the metadata items and the values are the values of the metadata items.
     """
     if minio_mode:
-        with rasterio.open(s3_key.replace("s3://", f"/vsicurl/{os.environ.get('MINIO_S3_ENDPOINT')}/")) as src:
+        with rasterio.open(
+            s3_key.replace("s3://", f"/vsicurl/{os.environ.get('MINIO_S3_ENDPOINT')}/")
+        ) as src:
             return src.tags(1)
     else:
         with rasterio.Env(aws_session):
             with rasterio.open(s3_key) as src:
                 return src.tags(1)
 
 
-def bbox_to_polygon(bbox) -> shapely.Polygon:
+def bbox_to_polygon(bbox) -> Polygon:
     """
     This function converts a bounding box to a Shapely Polygon.
 
     Parameters:
         bbox: The bounding box to convert. It should be a sequence of four numbers: (min_x, min_y, max_x, max_y).
 
     Returns:
         shapely.Polygon: The Shapely Polygon representing the bounding box. The Polygon is a rectangle with the lower
           left corner at (min_x, min_y) and the upper right corner at (max_x, max_y).
     """
     min_x, min_y, max_x, max_y = bbox
-    return shapely.Polygon(
+    return Polygon(
         [
             [min_x, min_y],
             [min_x, max_y],
             [max_x, max_y],
             [max_x, min_y],
         ]
     )
@@ -118,15 +122,15 @@
     bbox = get_raster_bounds(s3_full_key, aws_session, minio_mode=minio_mode)
     geometry = bbox_to_polygon(bbox)
     item = pystac.Item(
         id=item_id,
         properties={},
         bbox=bbox,
         datetime=datetime.now(),
-        geometry=json.loads(shapely.to_geojson(geometry)),
+        geometry=json.loads(to_geojson(geometry)),
     )
     # non_null = not raster_is_all_null(depth_grid.key)
     asset = pystac.Asset(
         href=s3_key_public_url_converter(s3_full_key, minio_mode=minio_mode),
         title=title,
         media_type=pystac.MediaType.COG,
         roles=["ras-depth-grid"],
```

### Comparing `ras_stac-0.1.0b1/ras_stac/utils/ras_hdf.py` & `ras_stac-0.1.1b1/ras_stac/utils/ras_hdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import pyproj
-import shapely
-import shapely.ops
 import logging
 from dotenv import load_dotenv, find_dotenv
 
 from rashdf import RasPlanHdf, RasGeomHdf
 from rashdf.utils import parse_duration
 
 logging.getLogger("boto3").setLevel(logging.WARNING)
@@ -74,22 +71,26 @@
         stac_plan_attrs = prep_stac_attrs(stac_plan_attrs)
     else:
         stac_plan_attrs = {}
         logging.warning("No root attributes found.")
 
     plan_info_attrs = ras_hdf.get_plan_info_attrs()
     if plan_info_attrs is not None:
-        plan_info_stac_attrs = prep_stac_attrs(plan_info_attrs, prefix="Plan Information")
+        plan_info_stac_attrs = prep_stac_attrs(
+            plan_info_attrs, prefix="Plan Information"
+        )
         stac_plan_attrs.update(plan_info_stac_attrs)
     else:
         logging.warning("No plan information attributes found.")
 
     plan_params_attrs = ras_hdf.get_plan_param_attrs()
     if plan_params_attrs is not None:
-        plan_params_stac_attrs = prep_stac_attrs(plan_params_attrs, prefix="Plan Parameters")
+        plan_params_stac_attrs = prep_stac_attrs(
+            plan_params_attrs, prefix="Plan Parameters"
+        )
         stac_plan_attrs.update(plan_params_stac_attrs)
     else:
         logging.warning("No plan parameters attributes found.")
 
     precip_attrs = ras_hdf.get_meteorology_precip_attrs()
     if precip_attrs is not None:
         precip_stac_attrs = prep_stac_attrs(precip_attrs, prefix="Meteorology")
@@ -101,52 +102,66 @@
     if include_results:
         stac_plan_attrs.update(get_stac_plan_results_attrs(ras_hdf))
     return stac_plan_attrs
 
 
 def get_stac_plan_results_attrs(ras_hdf: RasPlanHdf):
     """
-    This function retrieves the results attributes of a plan from a HEC-RAS plan HDF file, converting them to STAC format.
-    For summary atrributes, it retrieves the total computation time, the run time window,
+    This function retrieves the results attributes of a plan from a HEC-RAS plan HDF file, converting
+    them to STAC format. For summary atrributes, it retrieves the total computation time, the run time window,
     and the solution from it, and calculates the total computation time in minutes if it exists.
 
     Parameters:
         ras_hdf (RasPlanHdf): An instance of RasPlanHdf which the results attributes will be retrieved from.
 
     Returns:
         results_attrs (dict): A dictionary with the results attributes of the plan.
     """
     results_attrs = {}
 
     unsteady_results_attrs = ras_hdf.get_results_unsteady_attrs()
     if unsteady_results_attrs is not None:
-        unsteady_results_stac_attrs = prep_stac_attrs(unsteady_results_attrs, prefix="Unsteady Results")
+        unsteady_results_stac_attrs = prep_stac_attrs(
+            unsteady_results_attrs, prefix="Unsteady Results"
+        )
         results_attrs.update(unsteady_results_stac_attrs)
     else:
         logging.warning("No unsteady results attributes found.")
 
     summary_attrs = ras_hdf.get_results_unsteady_summary_attrs()
     if summary_attrs is not None:
         summary_stac_attrs = prep_stac_attrs(summary_attrs, prefix="Results Summary")
-        computation_time_total = summary_stac_attrs.get("results_summary:computation_time_total")
+        computation_time_total = summary_stac_attrs.get(
+            "results_summary:computation_time_total"
+        )
         results_summary = {
             "results_summary:computation_time_total": computation_time_total,
-            "results_summary:run_time_window": summary_stac_attrs.get("results_summary:run_time_window"),
-            "results_summary:solution": summary_stac_attrs.get("results_summary:solution"),
+            "results_summary:run_time_window": summary_stac_attrs.get(
+                "results_summary:run_time_window"
+            ),
+            "results_summary:solution": summary_stac_attrs.get(
+                "results_summary:solution"
+            ),
         }
         if computation_time_total is not None:
-            computation_time_total_minutes = parse_duration(computation_time_total).total_seconds() / 60
-            results_summary["results_summary:computation_time_total_minutes"] = computation_time_total_minutes
+            computation_time_total_minutes = (
+                parse_duration(computation_time_total).total_seconds() / 60
+            )
+            results_summary["results_summary:computation_time_total_minutes"] = (
+                computation_time_total_minutes
+            )
         results_attrs.update(results_summary)
     else:
         logging.warning("No unsteady results summary attributes found.")
 
     volume_accounting_attrs = ras_hdf.get_results_volume_accounting_attrs()
     if volume_accounting_attrs is not None:
-        volume_accounting_stac_attrs = prep_stac_attrs(volume_accounting_attrs, prefix="Volume Accounting")
+        volume_accounting_stac_attrs = prep_stac_attrs(
+            volume_accounting_attrs, prefix="Volume Accounting"
+        )
         results_attrs.update(volume_accounting_stac_attrs)
     else:
         logging.warning("No results volume accounting attributes found.")
 
     return results_attrs
 
 
@@ -180,18 +195,24 @@
         structures_stac_attrs = prep_stac_attrs(structures_attrs, prefix="Structures")
         stac_geom_attrs.update(structures_stac_attrs)
     else:
         logging.warning("No geometry structures attributes found.")
 
     d2_flow_area_attrs = ras_hdf.get_geom_2d_flow_area_attrs()
     if d2_flow_area_attrs is not None:
-        d2_flow_area_stac_attrs = prep_stac_attrs(d2_flow_area_attrs, prefix="2D Flow Areas")
-        cell_average_size = d2_flow_area_stac_attrs.get("2d_flow_area:cell_average_size", None)
+        d2_flow_area_stac_attrs = prep_stac_attrs(
+            d2_flow_area_attrs, prefix="2D Flow Areas"
+        )
+        cell_average_size = d2_flow_area_stac_attrs.get(
+            "2d_flow_area:cell_average_size", None
+        )
         if cell_average_size is not None:
-            d2_flow_area_stac_attrs["2d_flow_area:cell_average_length"] = cell_average_size**0.5
+            d2_flow_area_stac_attrs["2d_flow_area:cell_average_length"] = (
+                cell_average_size**0.5
+            )
         else:
             logging.warning("Unable to add cell average size to attributes.")
         stac_geom_attrs.update(d2_flow_area_stac_attrs)
     else:
         logging.warning("No flow area attributes found.")
 
     return stac_geom_attrs
```

### Comparing `ras_stac-0.1.0b1/ras_stac/utils/ras_stac.py` & `ras_stac-0.1.1b1/ras_stac/utils/ras_stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import pystac
 import json
 from typing import List
 import os
 import fsspec
+import shapely
 from rashdf import RasPlanHdf, RasGeomHdf
+from ras_hdf import (
+    get_stac_geom_attrs,
+    get_stac_plan_attrs,
+    get_stac_plan_results_attrs,
+)
 from pathlib import Path
 import re
 
 import logging
 
 logging.getLogger("boto3").setLevel(logging.WARNING)
 logging.getLogger("botocore").setLevel(logging.WARNING)
 
-from .ras_hdf import *
-
 
 def create_model_item(
-    ras_geom_hdf_url: str, props_to_remove: List, simplify: float = None, minio_mode: bool = False
+    ras_geom_hdf_url: str,
+    props_to_remove: List,
+    simplify: float = None,
+    minio_mode: bool = False,
 ) -> pystac.Item:
     """
     This function creates a STAC (SpatioTemporal Asset Catalog) item from a given HDF (Hierarchical Data Format)
     file URL.
 
     Parameters:
     ras_geom_hdf_url (str): The URL of the HDF file.
@@ -38,26 +45,30 @@
     3. Logs the creation of the STAC item for the model.
     4. Opens the HDF file from the URL using the `RasGeomHdf.open_uri` method.
     5. Gets the perimeter of the 2D flow area from the HDF file and simplifies it using the provided `simplify`
       parameter.
     6. Gets the attributes of the geometry from the HDF file.
     7. Extracts the geometry time from the properties.
     8. Removes unwanted properties.
-    9. Creates a new STAC item with the model ID, the geometry converted to GeoJSON, the bounding box of the perimeter, and the properties.
+    9. Creates a new STAC item with the model ID, the geometry converted to GeoJSON, the bounding box of the
+       perimeter, and the properties.
     10. Returns the created STAC item.
     """
     if Path(ras_geom_hdf_url).suffix != ".hdf":
-        raise ValueError(f"Expected pattern: `s3://bucket/prefix/ras-model-name.g**.hdf`, got {ras_geom_hdf_url}")
+        raise ValueError(
+            f"Expected pattern: `s3://bucket/prefix/ras-model-name.g**.hdf`, got {ras_geom_hdf_url}"
+        )
 
     ras_model_name = Path(ras_geom_hdf_url.replace(".hdf", "")).stem
 
     logging.info(f"Creating STAC item for model {ras_model_name}")
     if minio_mode:
         ras_hdf = RasGeomHdf.open_uri(
-            ras_geom_hdf_url, fsspec_kwargs={"endpoint_url": os.environ.get("MINIO_S3_ENDPOINT")}
+            ras_geom_hdf_url,
+            fsspec_kwargs={"endpoint_url": os.environ.get("MINIO_S3_ENDPOINT")},
         )
     else:
         ras_hdf = RasGeomHdf.open_uri(ras_geom_hdf_url)
     perimeter = ras_hdf.mesh_areas()
     perimeter = perimeter.to_crs("EPSG:4326")
     if simplify:
         perimeter_polygon = perimeter.geometry.unary_union.simplify(tolerance=simplify)
@@ -127,15 +138,15 @@
         dict: A dictionary with the roles, the description, and the title of the asset.
 
     Raises:
         ValueError: If the provided asset_type is not one of: "mannings", "lulc", "topo", "other".
     """
 
     if asset_type not in ["mannings", "lulc", "topo", "other"]:
-        raise ValueError(f"asset_type must be one of: mannings, lulc, topo, other")
+        raise ValueError("asset_type must be one of: mannings, lulc, topo, other")
 
     file_extension = Path(s3_key).suffix
     title = Path(s3_key).name
 
     if asset_type == "mannings":
         description = "Friction surface used in HEC-RAS model geometry"
 
@@ -229,15 +240,17 @@
 
     else:
         roles.extend(["ras-file"])
 
     return {"roles": roles, "description": description, "title": title}
 
 
-def get_simulation_metadata(ras_plan_hdf_url: str, simulation: str, minio_mode: bool = False) -> dict:
+def get_simulation_metadata(
+    ras_plan_hdf_url: str, simulation: str, minio_mode: bool = False
+) -> dict:
     """
     This function retrieves the metadata of a simulation from a HEC-RAS plan HDF file.
 
     Parameters:
         ras_plan_hdf_url (str): The URL of the HEC-RAS plan HDF file.
         simulation (str): The name of the simulation.
 
@@ -266,34 +279,41 @@
         s3f = fsspec.open(ras_plan_hdf_url, mode="rb")
     metadata = {
         "ras:simulation": simulation,
     }
 
     try:
         plan_hdf = RasPlanHdf(s3f.open())
-    except FileNotFoundError as e:
+    except FileNotFoundError:
         return logging.error(f"file not found: {ras_plan_hdf_url}")
 
     try:
         plan_attrs = get_stac_plan_attrs(plan_hdf)
         metadata.update(plan_attrs)
     except Exception as e:
-        return logging.error(f"unable to extract plan_attrs from {ras_plan_hdf_url}: {e}")
+        return logging.error(
+            f"unable to extract plan_attrs from {ras_plan_hdf_url}: {e}"
+        )
 
     try:
         results_attrs = get_stac_plan_results_attrs(plan_hdf)
         metadata.update(results_attrs)
     except Exception as e:
-        return logging.error(f"unable to extract results_attrs from {ras_plan_hdf_url}: {e}")
+        return logging.error(
+            f"unable to extract results_attrs from {ras_plan_hdf_url}: {e}"
+        )
 
     return metadata
 
 
 def create_model_simulation_item(
-    ras_item: pystac.Item, results_meta: dict, model_sim_id: str, item_props_to_remove: List
+    ras_item: pystac.Item,
+    results_meta: dict,
+    model_sim_id: str,
+    item_props_to_remove: List,
 ) -> pystac.Item:
     """
     This function creates a PySTAC Item for a model simulation.
 
     Parameters:
         ras_item (pystac.Item): The PySTAC Item of the RAS model.
         results_meta (dict): The metadata of the simulation results.
@@ -315,15 +335,17 @@
     start_datetime = runtime_window[0]
     end_datetime = runtime_window[1]
 
     for prop in item_props_to_remove:
         try:
             del results_meta[prop]
         except KeyError:
-            logging.warning(f"Failed to remove property:{prop} not found in simulation results metadata.")
+            logging.warning(
+                f"Failed to remove property:{prop} not found in simulation results metadata."
+            )
 
     item = pystac.Item(
         id=model_sim_id,
         geometry=ras_item.geometry,
         bbox=ras_item.bbox,
         start_datetime=start_datetime,
         end_datetime=end_datetime,
```

### Comparing `ras_stac-0.1.0b1/ras_stac/utils/s3_utils.py` & `ras_stac-0.1.1b1/ras_stac/utils/s3_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from mypy_boto3_s3.service_resource import ObjectSummary
 import boto3
 import botocore
-import os
 import json
-from datetime import datetime
-from json import JSONEncoder
 import logging
+import re
+import os
+
+from datetime import datetime
 from dotenv import load_dotenv, find_dotenv
+from mypy_boto3_s3.service_resource import ObjectSummary
 
 logging.getLogger("boto3").setLevel(logging.WARNING)
 logging.getLogger("botocore").setLevel(logging.WARNING)
 
 load_dotenv(find_dotenv())
 
 
@@ -18,37 +19,40 @@
     """
     This function retrieves basic metadata of an AWS S3 object.
 
     Parameters:
         obj (ObjectSummary): The AWS S3 object.
 
     Returns:
-        dict: A dictionary with the size, ETag, last modified date, storage platform, region, and storage tier of the object.
+        dict: A dictionary with the size, ETag, last modified date, storage platform, region, and
+              storage tier of the object.
     """
     try:
         _ = obj.load()
         return {
             "file:size": obj.content_length,
             "e_tag": obj.e_tag.strip('"'),
             "last_modified": obj.last_modified.isoformat(),
             "storage:platform": "AWS",
             "storage:region": obj.meta.client.meta.region_name,
             "storage:tier": obj.storage_class,
         }
     except botocore.exceptions.ClientError:
-        raise KeyError(f"Unable to access {obj.key} check that key exists and you have access")
+        raise KeyError(
+            f"Unable to access {obj.key} check that key exists and you have access"
+        )
 
 
-class DateTimeEncoder(JSONEncoder):
+class DateTimeEncoder(json.JSONEncoder):
     """JSON encoder for handling datetime objects."""
 
     def default(self, obj):
         if isinstance(obj, datetime):
             return obj.isoformat()
-        return JSONEncoder.default(self, obj)
+        return json.JSONEncoder.default(self, obj)
 
 
 def copy_item_to_s3(item, s3_key, s3client):
     """
     This function copies an item to an AWS S3 bucket.
 
     Parameters:
@@ -108,22 +112,26 @@
         3. If the input URL is an HTTPS URL, it converts it to an S3 URL.
     """
 
     if url.startswith("s3"):
         bucket = url.replace("s3://", "").split("/")[0]
         key = url.replace(f"s3://{bucket}", "")[1:]
         if minio_mode:
-            logging.info(f"minio_mode | using minio endpoint for s3 url conversion: {url}")
+            logging.info(
+                f"minio_mode | using minio endpoint for s3 url conversion: {url}"
+            )
             return f"{os.environ.get('MINIO_S3_ENDPOINT')}/{bucket}/{key}"
         else:
             return f"https://{bucket}.s3.amazonaws.com/{key}"
 
     elif url.startswith("http"):
         if minio_mode:
-            logging.info(f"minio_mode | using minio endpoint for s3 url conversion: {url}")
+            logging.info(
+                f"minio_mode | using minio endpoint for s3 url conversion: {url}"
+            )
             bucket = url.replace(os.environ.get("MINIO_S3_ENDPOINT"), "").split("/")[0]
             key = url.replace(os.environ.get("MINIO_S3_ENDPOINT"), "")
         else:
             bucket = url.replace("https://", "").split(".s3.amazonaws.com")[0]
             key = url.replace(f"https://{bucket}.s3.amazonaws.com/", "")
 
         return f"s3://{bucket}/{key}"
@@ -136,27 +144,33 @@
     """
     TODO: discuss this with the team. Would like some safety mechanism to ensure that the S3 key is limited to
     certain prefixes. Should there be some restriction where these files can be written?
     """
     parts = s3_key.split("/")
     logging.debug(f"parts of the s3_key: {parts}")
     if parts[3] != "stac":
-        raise ValueError(f"prefix must begin with stac/, user provided {s3_key} needs to be corrected")
+        raise ValueError(
+            f"prefix must begin with stac/, user provided {s3_key} needs to be corrected"
+        )
 
 
 def init_s3_resources(minio_mode: bool = False):
     if minio_mode:
         session = boto3.Session(
             aws_access_key_id=os.environ.get("MINIO_ACCESS_KEY_ID"),
             aws_secret_access_key=os.environ.get("MINIO_SECRET_ACCESS_KEY"),
         )
 
-        s3_client = session.client("s3", endpoint_url=os.environ.get("MINIO_S3_ENDPOINT"))
+        s3_client = session.client(
+            "s3", endpoint_url=os.environ.get("MINIO_S3_ENDPOINT")
+        )
 
-        s3_resource = session.resource("s3", endpoint_url=os.environ.get("MINIO_S3_ENDPOINT"))
+        s3_resource = session.resource(
+            "s3", endpoint_url=os.environ.get("MINIO_S3_ENDPOINT")
+        )
 
         return session, s3_client, s3_resource
     else:
         # Instantitate S3 resources
         session = boto3.Session(
             aws_access_key_id=os.environ.get("AWS_ACCESS_KEY_ID"),
             aws_secret_access_key=os.environ.get("AWS_SECRET_ACCESS_KEY"),
@@ -176,24 +190,23 @@
         try:
             kwargs["ContinuationToken"] = resp["NextContinuationToken"]
         except KeyError:
             break
     return keys
 
 
-import re
-
-
 def list_keys_regex(s3_client, bucket, prefix_includes, suffix=""):
     keys = []
     kwargs = {"Bucket": bucket, "Prefix": prefix_includes}
     prefix_pattern = re.compile(prefix_includes.replace("*", ".*"))
     while True:
         resp = s3_client.list_objects_v2(**kwargs)
         keys += [
-            obj["Key"] for obj in resp["Contents"] if prefix_pattern.match(obj["Key"]) and obj["Key"].endswith(suffix)
+            obj["Key"]
+            for obj in resp["Contents"]
+            if prefix_pattern.match(obj["Key"]) and obj["Key"].endswith(suffix)
         ]
         try:
             kwargs["ContinuationToken"] = resp["NextContinuationToken"]
         except KeyError:
             break
     return keys
```

### Comparing `ras_stac-0.1.0b1/ras_stac.egg-info/PKG-INFO` & `ras_stac-0.1.1b1/ras_stac.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ras-stac
-Version: 0.1.0b1
+Version: 0.1.1b1
 Summary: Create SpatioTemporal Asset Catalog (STAC) objects from HEC-RAS model data.
 Maintainer-email: Seth Lawler <slawler@dewberry.com>
 License: MIT
 Project-URL: repository, https://github.com/fema-ffrd/ras-stac
 Keywords: hec-ras,catalog,STAC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,26 +13,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5py
-Requires-Dist: geopandas
-Requires-Dist: s3fs
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: fsspec
-Requires-Dist: h5py
 Requires-Dist: mypy
 Requires-Dist: numpy
 Requires-Dist: papipyplug
 Requires-Dist: python-dotenv
-Requires-Dist: pyproj
 Requires-Dist: pystac
 Requires-Dist: shapely
 Requires-Dist: rasterio
 Requires-Dist: rashdf
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
@@ -40,15 +35,15 @@
 # ras-stac
 [![CI](https://github.com/fema-ffrd/rashdf/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/fema-ffrd/ras-stac/actions/workflows/continuous-integration.yml)
 [![Release](https://github.com/fema-ffrd/ras-stac/actions/workflows/release.yml/badge.svg)](https://github.com/fema-ffrd/ras-stac/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/ras-stac.svg)](https://badge.fury.io/py/ras-stac)
 
 Utilities for making SpatioTemporal Asset Catalogs of HEC-RAS models
 
-This repository contains code for developing STAC items from HEC-RAS models. Current activities focus on creating items for geometry files `g**.hdf` stored in AWS S3. More to come. 
+This repository contains code for developing STAC items from HEC-RAS models. Current activities focus on creating items for geometry files `g**.hdf` and plan files `p**.hdf stored in AWS S3. More to come. 
 
 *Source code largely ported from [ffrd-stac](https://github.com/arc-pts/ffrd-stac/blob/204e1ec85068936856b317fa9446da3c4da5d8d4/ffrd_stac/rasmeta.py).*
 
 
 ## Getting Started
 
 1. For local development, create a `.env` file using the `example.env` file.
```

