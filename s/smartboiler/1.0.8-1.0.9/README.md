# Comparing `tmp/smartboiler-1.0.8.tar.gz` & `tmp/smartboiler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.8.tar", last modified: Tue May 14 15:51:50 2024, max compression
+gzip compressed data, was "smartboiler-1.0.9.tar", last modified: Tue May 14 15:54:18 2024, max compression
```

## Comparing `smartboiler-1.0.8.tar` & `smartboiler-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:51:50.299679 smartboiler-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 15:51:47.000000 smartboiler-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:51:50.299679 smartboiler-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 15:51:48.000000 smartboiler-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.937108 smartboiler-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:54:18.937108 smartboiler-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 15:54:16.000000 smartboiler-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:54:18.937108 smartboiler-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 15:54:18.000000 smartboiler-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.933108 smartboiler-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.937108 smartboiler-1.0.9/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30822 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.937108 smartboiler-1.0.9/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0.8/PKG-INFO` & `smartboiler-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.8/README.md` & `smartboiler-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/setup.py` & `smartboiler-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0.8",  # Required
+    version="1.0.9",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-1.0.8/src/smartboiler/boiler.py` & `smartboiler-1.0.9/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/src/smartboiler/controller.py` & `smartboiler-1.0.9/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/src/smartboiler/data_handler.py` & `smartboiler-1.0.9/src/smartboiler/data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
         # extraction of features from device position
         df = self.extract_features_from_longitude_latitude(df)
 
         # cleaning the outliners from speed feature
         df.loc[df["speed"] > 200, "speed"] = 0
 
         # aggregate by 60 minutes
-        df = df.groupby(pd.Grouper(freq="60T"))
+        df = df.groupby(pd.Grouper(freq="60min"))
         df = df.agg(
             {
                 "consumed_heat_kJ": "sum",
                 "water_flow_L_per_minute_mean": "mean",
                 "water_temperature_mean": "mean",
                 "outside_temperature_mean": "mean",
                 "outside_humidity_mean": "mean",
@@ -493,18 +493,18 @@
 
         left_time_interval = datetime.now() - timedelta(days=14)
         queries = self.get_database_queries(
             left_time_interval=left_time_interval, right_time_interval=datetime.now()
         )
         df_all = self.get_df_from_queries(queries)
         df_all.index = df_all.index.tz_localize(None)
-        data_resampled = df_all.resample("10T").max()
+        data_resampled = df_all.resample("10min").max()
         data_resampled = data_resampled["boiler_relay_status"]
         data_resampled = data_resampled.notna().astype(int)
-        data_resampled = data_resampled.resample("30T").sum() * 10
+        data_resampled = data_resampled.resample("30min").sum() * 10
         # group by weekday and hour and minute and calculate max
         grouped = data_resampled.groupby(
             [
                 data_resampled.index.weekday,
                 data_resampled.index.hour,
                 data_resampled.index.minute,
             ]
```

### Comparing `smartboiler-1.0.8/src/smartboiler/event_checker.py` & `smartboiler-1.0.9/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/src/smartboiler/forecast.py` & `smartboiler-1.0.9/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/src/smartboiler/fotovoltaics.py` & `smartboiler-1.0.9/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/src/smartboiler/switch.py` & `smartboiler-1.0.9/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/src/smartboiler/time_handler.py` & `smartboiler-1.0.9/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.8/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.0.9/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.8/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.0.9/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

