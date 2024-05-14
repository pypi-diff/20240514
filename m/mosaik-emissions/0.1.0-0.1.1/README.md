# Comparing `tmp/mosaik_emissions-0.1.0.tar.gz` & `tmp/mosaik_emissions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik_emissions-0.1.0.tar", max compression
+gzip compressed data, was "mosaik_emissions-0.1.1.tar", max compression
```

## Comparing `mosaik_emissions-0.1.0.tar` & `mosaik_emissions-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2024-04-08 12:34:55.791338 mosaik_emissions-0.1.0/AUTHORS.txt
--rw-r--r--   0        0        0      230 2024-04-08 12:34:55.791338 mosaik_emissions-0.1.0/CHANGELOG
--rw-r--r--   0        0        0     1080 2024-04-08 12:34:55.791338 mosaik_emissions-0.1.0/LICENSE
--rw-r--r--   0        0        0     5955 2024-04-08 12:34:55.791338 mosaik_emissions-0.1.0/README.md
--rw-r--r--   0        0        0       94 2024-04-08 12:34:55.915339 mosaik_emissions-0.1.0/mosaik_components/emissions/__init__.py
--rw-r--r--   0        0        0 26611502 2024-04-08 12:34:55.966340 mosaik_emissions-0.1.0/mosaik_components/emissions/data/data.csv
--rw-r--r--   0        0        0     7306 2024-04-08 12:34:55.967340 mosaik_emissions-0.1.0/mosaik_components/emissions/emission_simulator.py
--rw-r--r--   0        0        0      508 2024-04-08 12:34:55.968340 mosaik_emissions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7034 1970-01-01 00:00:00.000000 mosaik_emissions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-05-14 09:04:29.325355 mosaik_emissions-0.1.1/AUTHORS.txt
+-rw-r--r--   0        0        0      315 2024-05-14 09:04:29.325355 mosaik_emissions-0.1.1/CHANGELOG
+-rw-r--r--   0        0        0     1080 2024-05-14 09:04:29.325355 mosaik_emissions-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5955 2024-05-14 09:04:29.325355 mosaik_emissions-0.1.1/README.md
+-rw-r--r--   0        0        0       94 2024-05-14 09:04:29.489354 mosaik_emissions-0.1.1/mosaik_components/emissions/__init__.py
+-rw-r--r--   0        0        0 26611502 2024-05-14 09:04:29.557354 mosaik_emissions-0.1.1/mosaik_components/emissions/data/data.csv
+-rw-r--r--   0        0        0     7314 2024-05-14 09:04:29.558354 mosaik_emissions-0.1.1/mosaik_components/emissions/emission_simulator.py
+-rw-r--r--   0        0        0      508 2024-05-14 09:04:29.558354 mosaik_emissions-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7119 1970-01-01 00:00:00.000000 mosaik_emissions-0.1.1/PKG-INFO
```

### Comparing `mosaik_emissions-0.1.0/LICENSE` & `mosaik_emissions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaik_emissions-0.1.0/README.md` & `mosaik_emissions-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mosaik_emissions-0.1.0/mosaik_components/emissions/data/data.csv` & `mosaik_emissions-0.1.1/mosaik_components/emissions/data/data.csv`

 * *Files identical despite different names*

### Comparing `mosaik_emissions-0.1.0/mosaik_components/emissions/emission_simulator.py` & `mosaik_emissions-0.1.1/mosaik_components/emissions/emission_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,26 +117,26 @@
             if len(filtered_data) == 0:
                 filtered_data = data[data['year'] == data['year'].max()]
                 ydiff = self.current_step.year - filtered_data.index[0].year
                 filtered_data.index += pd.offsets.DateOffset(years=ydiff) 
                 filtered_data['year'] += ydiff
             
             if len(filtered_data) > 0:
-                filtered_data.drop('year', axis=1, inplace=True)
+                filtered_data = filtered_data.drop('year', axis=1)
                 return filtered_data
 
             raise ValueError(f"No data for: {kwargs}")
         except Exception as e:
             raise ValueError(f"Getting value error for: {kwargs}, error: {str(e)}")
         
     def get_emission_factor(self, eid, attr, entity):
         params = self.entities[eid]['params']
         if attr in ['P[MW]']:
             if 'method' in params and callable(params['method']):
-                return params['method'](eid, attr, entity, self.current_step, params)
+                return params['method'](self, eid, attr, entity, self.current_step, params)
             elif 'co2_emission_factor' in params and pd.notna(params['co2_emission_factor']):
                 return params['co2_emission_factor']
             else:
                 factor = self.get_stored_values(**params)
                 index = factor.index.get_indexer([self.current_step], method='nearest')[0]
                 if index < 0:
                     index = 0
```

### Comparing `mosaik_emissions-0.1.0/PKG-INFO` & `mosaik_emissions-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-emissions
-Version: 0.1.0
+Version: 0.1.1
 Summary: Emissions simulator for Mosaik
 License: LICENSE
 Author: Danila Valko
 Author-email: mosaik@offis.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -143,14 +143,20 @@
 
 * Ember - Yearly Electricity Data (2023); Ember - European Electricity Review (2022); Energy Institute - Statistical Review of World Energy (2023) – with major processing by Our World in Data. “Carbon intensity of electricity generation” [dataset]. Ember, “Yearly Electricity Data”; Ember, “European Electricity Review”; Energy Institute, “Statistical Review of World Energy” [original data]. Retrieved February 27, 2024 from https://ourworldindata.org/grapher/carbon-intensity-electricity
 
 * Hourly consumption-based CO2 emissions intensity in Germany / [co2map.de](https://co2map.de/), INATECH, University of Freiburg. Retrieved February 27, 2024 from https://api.co2map.de/docs
 Changelog
 =========
 
+0.1.1 - 2024-05-14
+------------------
+
+- Examples were extended
+- Minor corrections
+
 0.1.0 - 2024-04-08
 ------------------
 
 - Carbon intensity from co2map.de was added
 - Restructured as a mosaik component
 - Readme and examples are added
 - Initial release of version implemented by Danila Valko
```

