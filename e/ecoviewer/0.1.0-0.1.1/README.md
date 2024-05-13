# Comparing `tmp/ecoviewer-0.1.0.tar.gz` & `tmp/ecoviewer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoviewer-0.1.0.tar", last modified: Thu May  9 21:19:50 2024, max compression
+gzip compressed data, was "ecoviewer-0.1.1.tar", last modified: Mon May 13 22:13:47 2024, max compression
```

## Comparing `ecoviewer-0.1.0.tar` & `ecoviewer-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.819043 ecoviewer-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.819043 ecoviewer-0.1.0/src/ecoviewer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.819043 ecoviewer-0.1.0/src/ecoviewer/config/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/config/configutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/src/ecoviewer/display/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/display/displayutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23365 2024-05-09 21:19:23.000000 ecoviewer-0.1.0/src/ecoviewer/display/graphutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:50.823043 ecoviewer-0.1.0/src/ecoviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 21:19:50.000000 ecoviewer-0.1.0/src/ecoviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/src/ecoviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/src/ecoviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/src/ecoviewer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/src/ecoviewer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/src/ecoviewer/config/configutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/src/ecoviewer/display/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/src/ecoviewer/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/src/ecoviewer/display/displayutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23365 2024-05-13 22:13:21.000000 ecoviewer-0.1.1/src/ecoviewer/display/graphutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:13:47.637562 ecoviewer-0.1.1/src/ecoviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 22:13:47.000000 ecoviewer-0.1.1/src/ecoviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 22:13:47.000000 ecoviewer-0.1.1/src/ecoviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:13:47.000000 ecoviewer-0.1.1/src/ecoviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 22:13:47.000000 ecoviewer-0.1.1/src/ecoviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 22:13:47.000000 ecoviewer-0.1.1/src/ecoviewer.egg-info/top_level.txt
```

### Comparing `ecoviewer-0.1.0/LICENSE` & `ecoviewer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.1.0/PKG-INFO` & `ecoviewer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecoviewer-0.1.0/setup.cfg` & `ecoviewer-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoviewer
-version = 0.1.0
+version = 0.1.1
 authors = ["Ecotope"]
 description = Contains functions for use in HVAC Dash applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoviewer-0.1.0/src/ecoviewer/config/configutils.py` & `ecoviewer-0.1.1/src/ecoviewer/config/configutils.py`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.1.0/src/ecoviewer/display/displayutils.py` & `ecoviewer-0.1.1/src/ecoviewer/display/displayutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from dash import dcc, html, Dash, dash_table
 from ecoviewer.config import get_organized_mapping
 
-def create_meta_data_table(site_df : pd.DataFrame, selected_table : str, app : Dash):
+def create_meta_data_table(site_df : pd.DataFrame, selected_table : str, app : Dash, anonymize_data : bool = True):
     wh_unit_name = site_df.loc[selected_table, 'wh_unit_name']
     wh_manufacturer = site_df.loc[selected_table, 'wh_manufacturer']
     swing_tank_volume = site_df.loc[selected_table, 'swing_tank_volume']
+    zip_code = site_df.loc[selected_table, 'zip_code']
+    swing_t_elem = site_df.loc[selected_table, 'swing_element_kw']
+    primary_volume = site_df.loc[selected_table, 'tank_size_gallons']
 
     mapping = {
         "Address" : site_df.loc[selected_table, 'address'] if site_df.loc[selected_table, 'address'] is not None else "Unknown", 
+        "Zip Code" : f"{zip_code}" if not (zip_code is None or pd.isna(zip_code)) else "Unknown",
         "Building Specifications" : site_df.loc[selected_table, 'building_specs'] if site_df.loc[selected_table, 'building_specs'] is not None else "Unknown", 
         "Primary System Model" : f"{wh_manufacturer} {wh_unit_name}" if not wh_manufacturer is None and not wh_unit_name is None else None, 
         "Primary HPWHs" : site_df.loc[selected_table, 'number_heat_pumps'], 
-        "Primary Tank Volume" : site_df.loc[selected_table, 'tank_size_gallons'], 
-        "Swing Tank Element" : site_df.loc[selected_table, 'swing_element_kw'], 
-        "Temperature Maintenance Storage Volume" : site_df.loc[selected_table, 'swing_tank_volume'],
+        "Primary Tank Volume" : f"{primary_volume} Gallons" if not (primary_volume is None or pd.isna(primary_volume)) else None, 
+        "Swing Tank Element" : f"{swing_t_elem} kW" if not (swing_t_elem is None or pd.isna(swing_t_elem)) else None, 
+        "Temperature Maintenance Storage Volume" : f"{swing_tank_volume} Gallons" if not (swing_tank_volume is None or pd.isna(swing_tank_volume)) else None,
         "Schematic Drawing": f"![]({app.get_asset_url('schematic-swingtank.jpg')})" if not (swing_tank_volume is None or pd.isna(swing_tank_volume)) else None
     }
 
+    if anonymize_data:
+        mapping['Address'] = None
+
+
     detail = []
     info = []
 
     for key, value in mapping.items():
         if not (value is None or pd.isna(value)):
             detail.append(key)
             info.append(value)
```

### Comparing `ecoviewer-0.1.0/src/ecoviewer/display/graphutils.py` & `ecoviewer-0.1.1/src/ecoviewer/display/graphutils.py`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.1.0/src/ecoviewer.egg-info/PKG-INFO` & `ecoviewer-0.1.1/src/ecoviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

