# Comparing `tmp/unfold-1.1.9.tar.gz` & `tmp/unfold-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfold-1.1.9.tar", last modified: Mon Feb 12 15:33:28 2024, max compression
+gzip compressed data, was "unfold-1.2.0.tar", last modified: Tue May 14 15:05:15 2024, max compression
```

## Comparing `unfold-1.1.9.tar` & `unfold-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:33:28.180663 unfold-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-12 15:33:22.000000 unfold-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-12 15:33:22.000000 unfold-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    45920 2024-02-12 15:33:28.176663 unfold-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-02-12 15:33:22.000000 unfold-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 15:33:28.180663 unfold-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-12 15:33:22.000000 unfold-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:33:28.176663 unfold-1.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-12 15:33:22.000000 unfold-1.1.9/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-12 15:33:22.000000 unfold-1.1.9/tests/test_reproducing_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:33:28.176663 unfold-1.1.9/unfold/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/brightway25_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/brightway2_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:33:28.176663 unfold-1.1.9/unfold/data/
--rw-r--r--   0 runner    (1001) docker     (127)   395147 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/data/flows_biosphere_38.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/data/outdated_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/data/outdated_units.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    31167 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/fold.py
--rw-r--r--   0 runner    (1001) docker     (127)    50524 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/unfold.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-12 15:33:22.000000 unfold-1.1.9/unfold/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:33:28.176663 unfold-1.1.9/unfold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45920 2024-02-12 15:33:28.000000 unfold-1.1.9/unfold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-12 15:33:28.000000 unfold-1.1.9/unfold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 15:33:28.000000 unfold-1.1.9/unfold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-12 15:33:28.000000 unfold-1.1.9/unfold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-12 15:33:28.000000 unfold-1.1.9/unfold.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:05:15.296815 unfold-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-14 15:05:08.000000 unfold-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 15:05:08.000000 unfold-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    45920 2024-05-14 15:05:15.296815 unfold-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-14 15:05:08.000000 unfold-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:05:15.296815 unfold-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 15:05:08.000000 unfold-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:05:15.292816 unfold-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 15:05:08.000000 unfold-1.2.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-14 15:05:08.000000 unfold-1.2.0/tests/test_reproducing_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:05:15.292816 unfold-1.2.0/unfold/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/brightway25_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/brightway2_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:05:15.296815 unfold-1.2.0/unfold/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   395147 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/data/flows_biosphere_38.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/data/outdated_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/data/outdated_units.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31167 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50757 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/unfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 15:05:08.000000 unfold-1.2.0/unfold/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:05:15.296815 unfold-1.2.0/unfold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45920 2024-05-14 15:05:15.000000 unfold-1.2.0/unfold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 15:05:15.000000 unfold-1.2.0/unfold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:05:15.000000 unfold-1.2.0/unfold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 15:05:15.000000 unfold-1.2.0/unfold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 15:05:15.000000 unfold-1.2.0/unfold.egg-info/top_level.txt
```

### Comparing `unfold-1.1.9/LICENSE` & `unfold-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/PKG-INFO` & `unfold-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfold
-Version: 1.1.9
+Version: 1.2.0
 Summary: Unpacks LCA scenario databases.
 Home-page: https://github.com/polca/premise
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `unfold-1.1.9/README.md` & `unfold-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/setup.py` & `unfold-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         for filename in filenames:
             paths.append(os.path.join("..", path, filename))
     return paths
 
 
 setup(
     name="unfold",
-    version="1.1.9",
+    version="1.2.0",
     python_requires=">=3.10",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     license=open("LICENSE").read(),
     # Only if you have non-python data (CSV, etc.). Might need to change the directory name as well.
     include_package_data=True,
     install_requires=[
```

### Comparing `unfold-1.1.9/tests/test_reproducing_db.py` & `unfold-1.2.0/tests/test_reproducing_db.py`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/unfold/brightway25_export.py` & `unfold-1.2.0/unfold/brightway25_export.py`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/unfold/brightway2_export.py` & `unfold-1.2.0/unfold/brightway2_export.py`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/unfold/data/flows_biosphere_38.csv` & `unfold-1.2.0/unfold/data/flows_biosphere_38.csv`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/unfold/data/outdated_flows.yaml` & `unfold-1.2.0/unfold/data/outdated_flows.yaml`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/unfold/data/outdated_units.yaml` & `unfold-1.2.0/unfold/data/outdated_units.yaml`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/unfold/data_cleaning.py` & `unfold-1.2.0/unfold/data_cleaning.py`

 * *Files 3% similar despite different names*

```diff
@@ -404,7 +404,25 @@
 
     scenario_db_unique_datasets = get_list_of_unique_datasets(scenario_db)
     if not set(original_db_unique_datasets).intersection(scenario_db_unique_datasets):
         raise ValueError(
             "Could not find datasets in common between the reference database "
             f"and {db_name}."
         )
+
+
+def change_db_name(data, name):
+    """
+    Originally from `wurst.linking` module.
+    Change the database of all datasets in ``data`` to ``name``.
+
+    Raises errors if each dataset does not have exactly one reference production exchange.
+    """
+
+    get_input_databases = lambda data: {ds.get("database") for ds in data}
+    old_names = get_input_databases(data)
+    for ds in data:
+        ds["database"] = name
+        for exc in ds["exchanges"]:
+            if exc.get("input") and exc["input"][0] in old_names:
+                exc["input"] = (name, exc["input"][1])
+    return data
```

### Comparing `unfold-1.1.9/unfold/fold.py` & `unfold-1.2.0/unfold/fold.py`

 * *Files identical despite different names*

### Comparing `unfold-1.1.9/unfold/unfold.py` & `unfold-1.2.0/unfold/unfold.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,23 @@
 import numpy as np
 import pandas as pd
 import sparse
 from datapackage import Package
 from prettytable import PrettyTable
 from scipy import sparse as nsp
 from wurst import extract_brightway2_databases
-from wurst.linking import (
-    change_db_name,
-    check_duplicate_codes,
-    check_internal_linking,
-    link_internal,
-)
+from wurst.linking import check_duplicate_codes, check_internal_linking, link_internal
 
 from .data_cleaning import (
     add_biosphere_links,
     add_product_field_to_exchanges,
+    change_db_name,
     check_exchanges_input,
     check_for_duplicates,
     correct_fields_format,
-    get_list_of_unique_datasets,
     get_outdated_flows,
     get_outdated_units,
     remove_categories_for_technosphere_flows,
     remove_missing_fields,
 )
 
 try:
@@ -373,15 +368,27 @@
 
         The resulting factors are stored in the factors attribute,
         which is a dictionary that maps flow ids to their corresponding
         factors.
 
         """
         self.factors = (
-            self.scenario_df.groupby("flow id").sum(numeric_only=True).to_dict("index")
+            self.scenario_df[
+                [
+                    c
+                    for c in self.scenario_df.columns
+                    if c
+                    not in [
+                        "to database",
+                    ]
+                ]
+            ]
+            .groupby("flow id")
+            .sum(numeric_only=True)
+            .to_dict("index")
         )
 
     def store_datasets_metadata(self) -> None:
         """
         Stores metadata for each dataset in the database attribute.
 
         The resulting metadata is stored in the dict_meta attribute, which is a dictionary that maps dataset identifiers to their
@@ -1114,14 +1121,15 @@
 
         # Create a new scenario dataframe from the updated factors dictionary
         self.scenario_df = pd.DataFrame.from_dict(self.factors).T.reset_index()
 
         # Rename columns
         # and add new columns
         # for database information and metadata
+
         self.scenario_df.columns = [
             "to activity name",
             "to reference product",
             "to location",
             "to unit",
             "from activity name",
             "from reference product",
@@ -1305,15 +1313,15 @@
 
             self.scenario_df.to_csv(
                 filename,
                 index=False,
                 encoding="utf-8-sig",
             )
 
-            print(f"Scenario difference file exported to {filename}")
+            print(f"Scenario difference file exported to {filename}.")
             print("")
             print("Writing superstructure database...")
             change_db_name(self.database, self.name or self.package.descriptor["name"])
             self.database = check_exchanges_input(
                 self.database, self.dependency_mapping
             )
             link_internal(self.database)
```

### Comparing `unfold-1.1.9/unfold.egg-info/PKG-INFO` & `unfold-1.2.0/unfold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfold
-Version: 1.1.9
+Version: 1.2.0
 Summary: Unpacks LCA scenario databases.
 Home-page: https://github.com/polca/premise
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

