# Comparing `tmp/crop_lca-0.2.1.tar.gz` & `tmp/crop_lca-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_lca-0.2.1.tar", max compression
+gzip compressed data, was "crop_lca-0.2.2.tar", max compression
```

## Comparing `crop_lca-0.2.1.tar` & `crop_lca-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 crop_lca-0.2.1/LICENSE
--rw-r--r--   0        0        0     4343 2024-04-25 06:32:33.950001 crop_lca-0.2.1/README.md
--rw-r--r--   0        0        0      421 2024-04-25 06:32:33.962001 crop_lca-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 08:43:36.000000 crop_lca-0.2.1/src/crop_lca/__init__.py
--rw-r--r--   0        0        0      222 2023-05-25 19:56:50.000000 crop_lca-0.2.1/src/crop_lca/database/__init__.py
--rw-r--r--   0        0        0   565248 2023-07-21 09:05:39.000000 crop_lca-0.2.1/src/crop_lca/database/crop_database.db
--rw-r--r--   0        0        0        0 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/geo_crop_lca/__init__.py
--rw-r--r--   0        0        0     2749 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/geo_crop_lca/catchment_crop_generator.py
--rw-r--r--   0        0        0     7665 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/geo_crop_lca/catchment_crop_production.py
--rw-r--r--   0        0        0    62864 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/lca.py
--rw-r--r--   0        0        0    27606 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/models.py
--rw-r--r--   0        0        0     7131 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/national_crop_production.py
--rw-r--r--   0        0        0        0 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/resource_manager/__init__.py
--rw-r--r--   0        0        0     1401 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/resource_manager/crop_lca_data_manager.py
--rw-r--r--   0        0        0     4307 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/resource_manager/data_loader.py
--rw-r--r--   0        0        0     6872 2024-02-26 08:01:03.358287 crop_lca-0.2.1/src/crop_lca/resource_manager/database_manager.py
--rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 crop_lca-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 crop_lca-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4343 2024-04-25 06:32:33.950001 crop_lca-0.2.2/README.md
+-rw-r--r--   0        0        0      421 2024-05-14 07:29:34.470499 crop_lca-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 08:43:36.000000 crop_lca-0.2.2/src/crop_lca/__init__.py
+-rw-r--r--   0        0        0      222 2023-05-25 19:56:50.000000 crop_lca-0.2.2/src/crop_lca/database/__init__.py
+-rw-r--r--   0        0        0   565248 2023-07-21 09:05:39.000000 crop_lca-0.2.2/src/crop_lca/database/crop_database.db
+-rw-r--r--   0        0        0        0 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/geo_crop_lca/__init__.py
+-rw-r--r--   0        0        0     2749 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/geo_crop_lca/catchment_crop_generator.py
+-rw-r--r--   0        0        0     7677 2024-05-14 07:29:34.474499 crop_lca-0.2.2/src/crop_lca/geo_crop_lca/catchment_crop_production.py
+-rw-r--r--   0        0        0    62864 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/lca.py
+-rw-r--r--   0        0        0    27606 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/models.py
+-rw-r--r--   0        0        0     7131 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/national_crop_production.py
+-rw-r--r--   0        0        0        0 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/resource_manager/__init__.py
+-rw-r--r--   0        0        0     1401 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/resource_manager/crop_lca_data_manager.py
+-rw-r--r--   0        0        0     4307 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/resource_manager/data_loader.py
+-rw-r--r--   0        0        0     6872 2024-02-26 08:01:03.358287 crop_lca-0.2.2/src/crop_lca/resource_manager/database_manager.py
+-rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 crop_lca-0.2.2/PKG-INFO
```

### Comparing `crop_lca-0.2.1/LICENSE` & `crop_lca-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/README.md` & `crop_lca-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/database/crop_database.db` & `crop_lca-0.2.2/src/crop_lca/database/crop_database.db`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/geo_crop_lca/catchment_crop_generator.py` & `crop_lca-0.2.2/src/crop_lca/geo_crop_lca/catchment_crop_generator.py`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/geo_crop_lca/catchment_crop_production.py` & `crop_lca-0.2.2/src/crop_lca/geo_crop_lca/catchment_crop_production.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,27 +164,27 @@
 
             farm_data.at[sc, "total_urea"] = 0
             farm_data.at[sc, "total_urea_abated"] = 0
             farm_data.at[sc, "total_n_fert"] = 0
             farm_data.at[sc, "total_p_fert"] = 0
             farm_data.at[sc, "total_k_fert"] = 0
 
-            for crop in crop_dataframe.crop_type.unique():
+            for crop in crop_dataframe.lucas_crop_type.unique():
 
                 try:
                     urea_value = urea_proportion.at[sc, "Urea proportion"]
 
                     urea_abated_value = urea_proportion.at[sc, "Urea abated proportion"]
                 
                 except KeyError:
                     urea_value = default_urea
                     urea_abated_value = default_urea_abated
 
 
-                mask = ((crop_dataframe["farm_id"]== sc) & (crop_dataframe["crop_type"]==crop))
+                mask = ((crop_dataframe["farm_id"]== sc) & (crop_dataframe["lucas_crop_type"]==crop))
 
                 farm_data.at[sc, "total_urea"] += crop_dataframe.loc[mask, "area"].item() *(application_rate.get_fert_kg_n_per_ha(crop)
                         * urea_value)
 
                 farm_data.at[sc, "total_urea_abated"] += crop_dataframe.loc[mask, "area"].item() * (crop_dataframe.loc[mask, "area"].item() * (application_rate.get_fert_kg_n_per_ha(crop)
                         * urea_value * urea_abated_value))
```

### Comparing `crop_lca-0.2.1/src/crop_lca/lca.py` & `crop_lca-0.2.2/src/crop_lca/lca.py`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/models.py` & `crop_lca-0.2.2/src/crop_lca/models.py`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/national_crop_production.py` & `crop_lca-0.2.2/src/crop_lca/national_crop_production.py`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/resource_manager/crop_lca_data_manager.py` & `crop_lca-0.2.2/src/crop_lca/resource_manager/crop_lca_data_manager.py`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/resource_manager/data_loader.py` & `crop_lca-0.2.2/src/crop_lca/resource_manager/data_loader.py`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/src/crop_lca/resource_manager/database_manager.py` & `crop_lca-0.2.2/src/crop_lca/resource_manager/database_manager.py`

 * *Files identical despite different names*

### Comparing `crop_lca-0.2.1/PKG-INFO` & `crop_lca-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: crop_lca
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tier 1 Environmental Impact Assessment tool for crops.
 License: MIT
 Author: Colm Duffy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: catchment_data_api (>=0.1.0,<0.2.0)
+Requires-Dist: catchment_data_api (>=0.1.2,<0.2.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (==2.1.4)
 Requires-Dist: sqlalchemy (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # 🌾 Crop_lca, a lifecycle assessment tool for cropping systems in Ireland
 [![license](https://img.shields.io/badge/License-MIT-red)](https://github.com/GOBLIN-Proj/crop_lca/blob/0.1.0/LICENSE)
```

