# Comparing `tmp/geoglows-1.6.0.tar.gz` & `tmp/geoglows-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.6.0.tar", last modified: Fri May 10 15:06:43 2024, max compression
+gzip compressed data, was "geoglows-1.6.1.tar", last modified: Tue May 14 04:33:59 2024, max compression
```

## Comparing `geoglows-1.6.0.tar` & `geoglows-1.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-10 15:06:34.000000 geoglows-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 15:06:34.000000 geoglows-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 15:06:43.936335 geoglows-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 15:06:34.000000 geoglows-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_download_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 15:06:34.000000 geoglows-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:06:43.936335 geoglows-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-10 15:06:34.000000 geoglows-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:33:59.276489 geoglows-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-14 04:33:50.000000 geoglows-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 04:33:50.000000 geoglows-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-14 04:33:59.276489 geoglows-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-14 04:33:50.000000 geoglows-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:33:59.276489 geoglows-1.6.1/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_download_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:33:59.276489 geoglows-1.6.1/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-14 04:33:50.000000 geoglows-1.6.1/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:33:59.276489 geoglows-1.6.1/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-14 04:33:59.000000 geoglows-1.6.1/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-14 04:33:59.000000 geoglows-1.6.1/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:33:59.000000 geoglows-1.6.1/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 04:33:59.000000 geoglows-1.6.1/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 04:33:59.000000 geoglows-1.6.1/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 04:33:50.000000 geoglows-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 04:33:59.276489 geoglows-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-14 04:33:50.000000 geoglows-1.6.1/setup.py
```

### Comparing `geoglows-1.6.0/LICENSE` & `geoglows-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/PKG-INFO` & `geoglows-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.6.0
+Version: 1.6.1
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.6.0/README.md` & `geoglows-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_constants.py` & `geoglows-1.6.1/geoglows/_constants.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_download_decorators.py` & `geoglows-1.6.1/geoglows/_download_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,17 @@
 def _forecast(function):
     def from_aws(*args, **kwargs):
         product_name = function.__name__.replace("_", "").lower()
         if product_name == 'forecastrecords':
             warnings.warn('forecast_records are not available from the AWS Open Data Program.')
             return from_rest(*args, **kwargs)
 
-        river_id = kwargs.get('river_id', '')
-        river_id = args[0] if len(args) > 0 else river_id
+        river_id = args[0] if len(args) > 0 else kwargs.get('river_id', '')
+        if river_id is None or river_id == '':
+            raise ValueError('River ID must be provided to retrieve forecast data.')
 
         return_format = kwargs.get('format', 'df')
         assert return_format in ('df', 'xarray'), f'Unsupported return format requested: {return_format}'
 
         if kwargs.get('skip_log', False):
             requests.post(f'{DEFAULT_REST_ENDPOINT}{DEFAULT_REST_ENDPOINT_VERSION}/log',
                           json={'river_id': river_id, 'product': product_name, 'format': return_format},
@@ -114,16 +115,15 @@
         endpoint = f'https://{endpoint}' if not endpoint.startswith(('https://', 'http://')) else endpoint
 
         version = kwargs.get('version', DEFAULT_REST_ENDPOINT_VERSION)
         assert version in ('v2',), ValueError(f'Unrecognized model version parameter: {version}')
 
         product_name = function.__name__.replace("_", "").lower()
 
-        river_id = args[0] if len(args) > 0 else None
-        river_id = kwargs.get('river_id', '') if not river_id else river_id
+        river_id = args[0] if len(args) > 0 else kwargs.get('river_id', '')
         if isinstance(river_id, list):
             raise ValueError('Multiple river_ids are not available via REST API or on v1. '
                              'Use data_source="aws" for multiple river_ids.')
         river_id = int(river_id) if river_id else None
         if river_id and version == 'v2':
             assert 1_000_000_000 > river_id >= 110_000_000, ValueError('River ID must be a 9 digit integer')
 
@@ -178,16 +178,17 @@
     return main
 
 
 def _retrospective(function):
     def main(*args, **kwargs):
         product_name = function.__name__.replace("_", "-").lower()
 
-        river_id = args[0] if len(args) > 0 else None
-        river_id = kwargs.get('river_id', '') if not river_id else river_id
+        river_id = args[0] if len(args) > 0 else kwargs.get('river_id', '')
+        if river_id is None or river_id == '':
+            raise ValueError('River ID must be provided to retrieve retrospective data.')
 
         return_format = kwargs.get('format', 'df')
         assert return_format in ('df', 'xarray'), f'Unsupported return format requested: {return_format}'
 
         method = kwargs.get('method', 'gumbel1')
 
         if kwargs.get('skip_log', False):
```

### Comparing `geoglows-1.6.0/geoglows/_plots/__init__.py` & `geoglows-1.6.1/geoglows/_plots/__init__.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_plots/format_tools.py` & `geoglows-1.6.1/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.6.1/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.6.1/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_plots/plotly_helpers.py` & `geoglows-1.6.1/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.6.1/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/_plots/plots.py` & `geoglows-1.6.1/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/analyze.py` & `geoglows-1.6.1/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/bias.py` & `geoglows-1.6.1/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/data.py` & `geoglows-1.6.1/geoglows/data.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/streamflow.py` & `geoglows-1.6.1/geoglows/streamflow.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/streams.py` & `geoglows-1.6.1/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows/tables.py` & `geoglows-1.6.1/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/geoglows.egg-info/PKG-INFO` & `geoglows-1.6.1/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.6.0
+Version: 1.6.1
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.6.0/geoglows.egg-info/SOURCES.txt` & `geoglows-1.6.1/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.0/setup.py` & `geoglows-1.6.1/setup.py`

 * *Files identical despite different names*

