# Comparing `tmp/grassland_production-0.3.3.tar.gz` & `tmp/grassland_production-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassland_production-0.3.3.tar", max compression
+gzip compressed data, was "grassland_production-0.3.4.tar", max compression
```

## Comparing `grassland_production-0.3.3.tar` & `grassland_production-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 grassland_production-0.3.3/LICENSE
--rw-r--r--   0        0        0     5196 2024-04-29 06:04:55.493506 grassland_production-0.3.3/README.md
--rw-r--r--   0        0        0      522 2024-04-29 06:04:55.517506 grassland_production-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 08:43:36.000000 grassland_production-0.3.3/src/grassland_production/__init__.py
--rw-r--r--   0        0        0      222 2024-02-21 12:18:55.520411 grassland_production-0.3.3/src/grassland_production/database/__init__.py
--rw-r--r--   0        0        0   114688 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/database/grassland_management_database.db
--rw-r--r--   0        0        0    36738 2024-03-28 08:10:44.376066 grassland_production-0.3.3/src/grassland_production/dry_matter.py
--rw-r--r--   0        0        0    17071 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/farm_data_generation.py
--rw-r--r--   0        0        0    20504 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/fertilisation.py
--rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/__init__.py
--rw-r--r--   0        0        0     7884 2024-02-21 12:18:55.532411 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/catchment_grassland.py
--rw-r--r--   0        0        0    20198 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py
--rw-r--r--   0        0        0    12515 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_fertilisation.py
--rw-r--r--   0        0        0    12382 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_grass_yield.py
--rw-r--r--   0        0        0     6878 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_grassland_output.py
--rw-r--r--   0        0        0     6264 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_grassland_soils.py
--rw-r--r--   0        0        0    12577 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_spared_area.py
--rw-r--r--   0        0        0    12359 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/grass_yield.py
--rw-r--r--   0        0        0     8887 2024-02-21 12:18:55.532411 grassland_production-0.3.3/src/grassland_production/grassland_area.py
--rw-r--r--   0        0        0     6758 2024-01-11 17:45:50.600302 grassland_production-0.3.3/src/grassland_production/grassland_output.py
--rw-r--r--   0        0        0     6235 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/grassland_soils.py
--rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.3/src/grassland_production/resource_manager/__init__.py
--rw-r--r--   0        0        0    11395 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/resource_manager/data_loader.py
--rw-r--r--   0        0        0    12745 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/resource_manager/database_manager.py
--rw-r--r--   0        0        0    13171 2024-03-28 08:10:44.380066 grassland_production-0.3.3/src/grassland_production/resource_manager/grassland_data_manager.py
--rw-r--r--   0        0        0     4894 2024-02-21 12:18:55.536411 grassland_production-0.3.3/src/grassland_production/resource_manager/scenario_data_fetcher.py
--rw-r--r--   0        0        0    12602 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/spared_area.py
--rw-r--r--   0        0        0    14033 2024-02-28 12:18:46.717106 grassland_production-0.3.3/src/grassland_production/stocking_rate.py
--rw-r--r--   0        0        0    18369 2024-02-28 12:18:46.721106 grassland_production-0.3.3/src/grassland_production/utilisation_rate.py
--rw-r--r--   0        0        0     5870 1970-01-01 00:00:00.000000 grassland_production-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 grassland_production-0.3.4/LICENSE
+-rw-r--r--   0        0        0     5216 2024-04-29 07:11:43.031249 grassland_production-0.3.4/README.md
+-rw-r--r--   0        0        0      522 2024-05-14 10:30:50.857386 grassland_production-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 08:43:36.000000 grassland_production-0.3.4/src/grassland_production/__init__.py
+-rw-r--r--   0        0        0      222 2024-02-21 12:18:55.520411 grassland_production-0.3.4/src/grassland_production/database/__init__.py
+-rw-r--r--   0        0        0   114688 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/database/grassland_management_database.db
+-rw-r--r--   0        0        0    36812 2024-05-14 10:30:50.857386 grassland_production-0.3.4/src/grassland_production/dry_matter.py
+-rw-r--r--   0        0        0    17071 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/farm_data_generation.py
+-rw-r--r--   0        0        0    20504 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/fertilisation.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/__init__.py
+-rw-r--r--   0        0        0     7884 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/catchment_grassland.py
+-rw-r--r--   0        0        0    20198 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py
+-rw-r--r--   0        0        0    12515 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_fertilisation.py
+-rw-r--r--   0        0        0    12382 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grass_yield.py
+-rw-r--r--   0        0        0     6878 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_output.py
+-rw-r--r--   0        0        0     6264 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_soils.py
+-rw-r--r--   0        0        0    12577 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_spared_area.py
+-rw-r--r--   0        0        0    12359 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/grass_yield.py
+-rw-r--r--   0        0        0     8887 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/grassland_area.py
+-rw-r--r--   0        0        0     6758 2024-01-11 17:45:50.600301 grassland_production-0.3.4/src/grassland_production/grassland_output.py
+-rw-r--r--   0        0        0     6235 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/grassland_soils.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/resource_manager/__init__.py
+-rw-r--r--   0        0        0    11395 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/resource_manager/data_loader.py
+-rw-r--r--   0        0        0    12745 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/resource_manager/database_manager.py
+-rw-r--r--   0        0        0    13171 2024-03-28 08:10:44.380066 grassland_production-0.3.4/src/grassland_production/resource_manager/grassland_data_manager.py
+-rw-r--r--   0        0        0     4894 2024-02-21 12:18:55.536411 grassland_production-0.3.4/src/grassland_production/resource_manager/scenario_data_fetcher.py
+-rw-r--r--   0        0        0    12602 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/spared_area.py
+-rw-r--r--   0        0        0    14033 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/stocking_rate.py
+-rw-r--r--   0        0        0    18369 2024-02-28 12:18:46.721106 grassland_production-0.3.4/src/grassland_production/utilisation_rate.py
+-rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 grassland_production-0.3.4/PKG-INFO
```

### Comparing `grassland_production-0.3.3/LICENSE` & `grassland_production-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/README.md` & `grassland_production-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,17 @@
     #set up test data
     path_to_data = "./data/"
 
     ef_country = "ireland"
     calibration_year = 2020
     target_year = 2050
 
-    scenario_dataframe = pd.read_csv(os.path.join(path_to_data,"scenario_dataframe1.csv"))
-    scenario_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"future_animals.csv"))
-    baseline_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"past_animals.csv"))
+    scenario_dataframe = pd.read_csv(os.path.join(path_to_data,"scenario_input_dataframe2.csv"))
+    scenario_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"scenario_animal_data.csv"))
+    baseline_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"baseline_animal_data.csv"))
 
     #class instance
     grassland = GrasslandOutput(
         ef_country,
         calibration_year,
         target_year,
         scenario_dataframe,
```

### Comparing `grassland_production-0.3.3/pyproject.toml` & `grassland_production-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grassland_production"
-version = "0.3.3"
+version = "0.3.4"
 description = "Computation of grassland area and production based on animal energy calculations and grassland inputs"
 authors = ["Colm Duffy"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `grassland_production-0.3.3/src/grassland_production/database/grassland_management_database.db` & `grassland_production-0.3.4/src/grassland_production/database/grassland_management_database.db`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/dry_matter.py` & `grassland_production-0.3.4/src/grassland_production/dry_matter.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,23 +286,23 @@
                         animal_list,
                         animal_name,
                     )
 
                     mask_validation = (baseline_animals_df["year"] == self.calibration_year) & (
                         baseline_animals_df["cohort"] == animal_name) & (baseline_animals_df["mm_storage"] == "tank liquid") & (baseline_animals_df["pop"] > 0)
 
-   
-                    past_total_dm_df.loc[self.calibration_year, cohort] += (
-                        self.grass_feed_class.dry_matter_from_grass(
-                            animal_past,
+                    if mask_validation.any():
+                        past_total_dm_df.loc[self.calibration_year, cohort] += (
+                            self.grass_feed_class.dry_matter_from_grass(
+                                animal_past,
+                            )
+                            * kg_to_t
+                            * 365
+                            * baseline_animals_df.loc[mask_validation, "pop"].values.item()
                         )
-                        * kg_to_t
-                        * 365
-                        * baseline_animals_df.loc[mask_validation, "pop"].values.item()
-                    )
         # Process sheep
         for landtype in COHORTS["sheep"].keys():
             for animal_name in COHORTS["sheep"][landtype]:
                 if animal_name in animal_list.__dict__.keys():
                     animal_past = getattr(
                         animal_list,
                         animal_name,
```

### Comparing `grassland_production-0.3.3/src/grassland_production/farm_data_generation.py` & `grassland_production-0.3.4/src/grassland_production/farm_data_generation.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/fertilisation.py` & `grassland_production-0.3.4/src/grassland_production/fertilisation.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/geo_grassland_production/catchment_grassland.py` & `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/catchment_grassland.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py` & `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_fertilisation.py` & `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_fertilisation.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_grass_yield.py` & `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grass_yield.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_grassland_output.py` & `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_output.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_grassland_soils.py` & `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_soils.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/geo_grassland_production/geo_spared_area.py` & `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_spared_area.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/grass_yield.py` & `grassland_production-0.3.4/src/grassland_production/grass_yield.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/grassland_area.py` & `grassland_production-0.3.4/src/grassland_production/grassland_area.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/grassland_output.py` & `grassland_production-0.3.4/src/grassland_production/grassland_output.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/grassland_soils.py` & `grassland_production-0.3.4/src/grassland_production/grassland_soils.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/resource_manager/data_loader.py` & `grassland_production-0.3.4/src/grassland_production/resource_manager/data_loader.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/resource_manager/database_manager.py` & `grassland_production-0.3.4/src/grassland_production/resource_manager/database_manager.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/resource_manager/grassland_data_manager.py` & `grassland_production-0.3.4/src/grassland_production/resource_manager/grassland_data_manager.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/resource_manager/scenario_data_fetcher.py` & `grassland_production-0.3.4/src/grassland_production/resource_manager/scenario_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/spared_area.py` & `grassland_production-0.3.4/src/grassland_production/spared_area.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/stocking_rate.py` & `grassland_production-0.3.4/src/grassland_production/stocking_rate.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/src/grassland_production/utilisation_rate.py` & `grassland_production-0.3.4/src/grassland_production/utilisation_rate.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.3/PKG-INFO` & `grassland_production-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grassland_production
-Version: 0.3.3
+Version: 0.3.4
 Summary: Computation of grassland area and production based on animal energy calculations and grassland inputs
 License: MIT
 Author: Colm Duffy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -93,17 +93,17 @@
     #set up test data
     path_to_data = "./data/"
 
     ef_country = "ireland"
     calibration_year = 2020
     target_year = 2050
 
-    scenario_dataframe = pd.read_csv(os.path.join(path_to_data,"scenario_dataframe1.csv"))
-    scenario_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"future_animals.csv"))
-    baseline_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"past_animals.csv"))
+    scenario_dataframe = pd.read_csv(os.path.join(path_to_data,"scenario_input_dataframe2.csv"))
+    scenario_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"scenario_animal_data.csv"))
+    baseline_animal_dataframe = pd.read_csv(os.path.join(path_to_data,"baseline_animal_data.csv"))
 
     #class instance
     grassland = GrasslandOutput(
         ef_country,
         calibration_year,
         target_year,
         scenario_dataframe,
```

