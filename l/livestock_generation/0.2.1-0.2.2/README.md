# Comparing `tmp/livestock_generation-0.2.1.tar.gz` & `tmp/livestock_generation-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livestock_generation-0.2.1.tar", max compression
+gzip compressed data, was "livestock_generation-0.2.2.tar", max compression
```

## Comparing `livestock_generation-0.2.1.tar` & `livestock_generation-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 livestock_generation-0.2.1/LICENSE
--rw-r--r--   0        0        0     3571 2024-04-25 09:32:25.185025 livestock_generation-0.2.1/README.md
--rw-r--r--   0        0        0      492 2024-04-25 09:25:43.647036 livestock_generation-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-13 11:18:50.533376 livestock_generation-0.2.1/src/livestock_generation/__init__.py
--rw-r--r--   0        0        0      222 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/database/__init__.py
--rw-r--r--   0        0        0   184320 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/database/livestock_database.db
--rw-r--r--   0        0        0        0 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/geo_livestock_generation/__init__.py
--rw-r--r--   0        0        0    27771 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/geo_livestock_generation/geo_livestock.py
--rw-r--r--   0        0        0     3564 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/geo_livestock_generation/geo_livestock_exports.py
--rw-r--r--   0        0        0    28493 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/livestock.py
--rw-r--r--   0        0        0     8545 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/livestock_exports.py
--rw-r--r--   0        0        0        0 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/resource_manager/__init__.py
--rw-r--r--   0        0        0     3130 2024-02-21 12:09:02.621754 livestock_generation-0.2.1/src/livestock_generation/resource_manager/data_loader.py
--rw-r--r--   0        0        0     4655 2024-02-21 12:09:02.625754 livestock_generation-0.2.1/src/livestock_generation/resource_manager/database_manager.py
--rw-r--r--   0        0        0    22434 2024-02-21 12:09:02.625754 livestock_generation-0.2.1/src/livestock_generation/resource_manager/livestock_data_manager.py
--rw-r--r--   0        0        0     1771 2024-02-21 12:09:02.625754 livestock_generation-0.2.1/src/livestock_generation/resource_manager/scenario_fetcher.py
--rw-r--r--   0        0        0     4229 1970-01-01 00:00:00.000000 livestock_generation-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 livestock_generation-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3571 2024-04-25 09:32:25.185025 livestock_generation-0.2.2/README.md
+-rw-r--r--   0        0        0      492 2024-05-14 10:34:18.186327 livestock_generation-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-13 11:18:50.533376 livestock_generation-0.2.2/src/livestock_generation/__init__.py
+-rw-r--r--   0        0        0      222 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/database/__init__.py
+-rw-r--r--   0        0        0   184320 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/database/livestock_database.db
+-rw-r--r--   0        0        0        0 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/geo_livestock_generation/__init__.py
+-rw-r--r--   0        0        0    27771 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/geo_livestock_generation/geo_livestock.py
+-rw-r--r--   0        0        0     3564 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/geo_livestock_generation/geo_livestock_exports.py
+-rw-r--r--   0        0        0    28493 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/livestock.py
+-rw-r--r--   0        0        0     8767 2024-05-14 10:34:18.186327 livestock_generation-0.2.2/src/livestock_generation/livestock_exports.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/resource_manager/__init__.py
+-rw-r--r--   0        0        0     3130 2024-02-21 12:09:02.621754 livestock_generation-0.2.2/src/livestock_generation/resource_manager/data_loader.py
+-rw-r--r--   0        0        0     4655 2024-02-21 12:09:02.625754 livestock_generation-0.2.2/src/livestock_generation/resource_manager/database_manager.py
+-rw-r--r--   0        0        0    22434 2024-02-21 12:09:02.625754 livestock_generation-0.2.2/src/livestock_generation/resource_manager/livestock_data_manager.py
+-rw-r--r--   0        0        0     1771 2024-02-21 12:09:02.625754 livestock_generation-0.2.2/src/livestock_generation/resource_manager/scenario_fetcher.py
+-rw-r--r--   0        0        0     4229 1970-01-01 00:00:00.000000 livestock_generation-0.2.2/PKG-INFO
```

### Comparing `livestock_generation-0.2.1/LICENSE` & `livestock_generation-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/README.md` & `livestock_generation-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/database/livestock_database.db` & `livestock_generation-0.2.2/src/livestock_generation/database/livestock_database.db`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/geo_livestock_generation/geo_livestock.py` & `livestock_generation-0.2.2/src/livestock_generation/geo_livestock_generation/geo_livestock.py`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/geo_livestock_generation/geo_livestock_exports.py` & `livestock_generation-0.2.2/src/livestock_generation/geo_livestock_generation/geo_livestock_exports.py`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/livestock.py` & `livestock_generation-0.2.2/src/livestock_generation/livestock.py`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/livestock_exports.py` & `livestock_generation-0.2.2/src/livestock_generation/livestock_exports.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,26 +57,30 @@
         milk_system_export = pd.DataFrame(
             index=df_index,
             columns=["Scenarios", "total_milk_kg"],
         )
 
         for sc in milk_system_export.index:
 
+            milk_system_export.loc[sc, "Scenarios"] = sc
+
             mask = (
                 (sc_herd_dataframe["cohort"] == "dairy_cows")
                 & (sc_herd_dataframe["Scenarios"] == sc)
                 & (sc_herd_dataframe["pop"] != 0)
             )
+            # Selecting the data based on mask
+            selected_milk_data = sc_herd_dataframe.loc[mask]
 
-            milk_system_export.loc[sc, "total_milk_kg"] = (
-                sc_herd_dataframe.loc[mask, "daily_milk"].values[0]
-                * sc_herd_dataframe.loc[mask, "pop"].values[0]
-                * 365
-            )
-            milk_system_export.loc[sc, "Scenarios"] = sc
+            if not selected_milk_data.empty:
+                daily_milk = selected_milk_data["daily_milk"].iloc[0]
+                pop = selected_milk_data["pop"].iloc[0]
+                milk_system_export.loc[sc, "total_milk_kg"] = daily_milk * pop * 365
+            else:
+                milk_system_export.loc[sc, "total_milk_kg"] = 0.0
 
         return milk_system_export
 
     def compute_system_protien_exports(self, scenario_animal_data, baseline_animal_data):
         """
         Calculates the total beef weight exported from the entire system for each scenario.
```

### Comparing `livestock_generation-0.2.1/src/livestock_generation/resource_manager/data_loader.py` & `livestock_generation-0.2.2/src/livestock_generation/resource_manager/data_loader.py`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/resource_manager/database_manager.py` & `livestock_generation-0.2.2/src/livestock_generation/resource_manager/database_manager.py`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/resource_manager/livestock_data_manager.py` & `livestock_generation-0.2.2/src/livestock_generation/resource_manager/livestock_data_manager.py`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/src/livestock_generation/resource_manager/scenario_fetcher.py` & `livestock_generation-0.2.2/src/livestock_generation/resource_manager/scenario_fetcher.py`

 * *Files identical despite different names*

### Comparing `livestock_generation-0.2.1/PKG-INFO` & `livestock_generation-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livestock_generation
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool that uses Ireland specific data to generate a baseline and scenario livestock herds for sheep and cattle.
 License: MIT
 Author: Colm Duffy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

