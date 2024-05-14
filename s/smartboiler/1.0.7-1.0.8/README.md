# Comparing `tmp/smartboiler-1.0.7.tar.gz` & `tmp/smartboiler-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.7.tar", last modified: Tue May 14 15:44:23 2024, max compression
+gzip compressed data, was "smartboiler-1.0.8.tar", last modified: Tue May 14 15:51:50 2024, max compression
```

## Comparing `smartboiler-1.0.7.tar` & `smartboiler-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.759455 smartboiler-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:44:23.759455 smartboiler-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 15:44:19.000000 smartboiler-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:44:23.759455 smartboiler-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 15:44:22.000000 smartboiler-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.755455 smartboiler-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.759455 smartboiler-1.0.7/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.759455 smartboiler-1.0.7/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:51:50.299679 smartboiler-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 15:51:47.000000 smartboiler-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:51:50.299679 smartboiler-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 15:51:48.000000 smartboiler-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 15:51:47.000000 smartboiler-1.0.8/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:50.299679 smartboiler-1.0.8/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 15:51:50.000000 smartboiler-1.0.8/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0.7/PKG-INFO` & `smartboiler-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.7/README.md` & `smartboiler-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/setup.py` & `smartboiler-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0.7",  # Required
+    version="1.0.8",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-1.0.7/src/smartboiler/boiler.py` & `smartboiler-1.0.8/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/src/smartboiler/controller.py` & `smartboiler-1.0.8/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/src/smartboiler/data_handler.py` & `smartboiler-1.0.8/src/smartboiler/data_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,34 +547,34 @@
         # fill consumed_heat_kWh with 0 if nan
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].fillna(0)
 
         # fill negative values with 0
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].clip(lower=0)
 
         # ffill na in df based on column
-        df["temperature"] = df[f"outside_temperature_mean"].fillna(method="ffill")
-        df["humidity"] = df[f"outside_humidity_mean"].fillna(method="ffill")
-        df["wind_speed"] = df[f"outside_wind_speed_mean"].fillna(method="ffill")
-        df["count"] = df["device_presence_distinct_count"].fillna(method="ffill")
+        df["temperature"] = df[f"outside_temperature_mean"].ffill()
+        df["humidity"] = df[f"outside_humidity_mean"].ffill()
+        df["wind_speed"] = df[f"outside_wind_speed_mean"].ffill()
+        df["count"] = df["device_presence_distinct_count"].ffill()
 
-        df["mean_longitude"] = df["mean_longitude"].fillna(method="ffill")
-        df["mean_latitude"] = df["mean_latitude"].fillna(method="ffill")
+        df["mean_longitude"] = df["mean_longitude"].ffill()
+        df["mean_latitude"] = df["mean_latitude"].ffill()
         df["speed"] = df["speed"].fillna(0)
         df["speed_towards_home"] = df["speed_towards_home"].fillna(0)
-        df["distance_from_home"] = df["distance_from_home"].fillna(method="ffill")
-        df["heading_to_home_sin"] = df["heading_to_home_sin"].fillna(method="ffill")
-        df["heading_to_home_cos"] = df["heading_to_home_cos"].fillna(method="ffill")
+        df["distance_from_home"] = df["distance_from_home"].ffill()
+        df["heading_to_home_sin"] = df["heading_to_home_sin"].ffill()
+        df["heading_to_home_cos"] = df["heading_to_home_cos"].ffill()
 
-        df["mean_longitude_2"] = df["mean_longitude_2"].fillna(method="ffill")
-        df["mean_latitude_2"] = df["mean_latitude_2"].fillna(method="ffill")
+        df["mean_longitude_2"] = df["mean_longitude_2"].ffill()
+        df["mean_latitude_2"] = df["mean_latitude_2"].ffill()
         df["speed_2"] = df["speed_2"].fillna(0)
         df["speed_towards_home_2"] = df["speed_towards_home_2"].fillna(0)
-        df["distance_from_home_2"] = df["distance_from_home_2"].fillna(method="ffill")
-        df["heading_to_home_sin_2"] = df["heading_to_home_sin_2"].fillna(method="ffill")
-        df["heading_to_home_cos_2"] = df["heading_to_home_cos_2"].fillna(method="ffill")
+        df["distance_from_home_2"] = df["distance_from_home_2"].ffill()
+        df["heading_to_home_sin_2"] = df["heading_to_home_sin_2"].ffill()
+        df["heading_to_home_cos_2"] = df["heading_to_home_cos_2"].ffill()
 
         # adding cooling down to the consumed heat
         df["consumed_heat_kWh"] += 1.25 / (24 // freq)
 
         window = 3
         # creating a 3 hour rolling window for the mean of the consumed heat for better prediction
         df["longtime_mean"] = (
@@ -585,56 +585,56 @@
         # extrahing next features
         df["last_3_week_mean"] = (
             df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
             .rolling(window=3, min_periods=1)
             .mean()
             .reset_index(level=[0, 1], drop=True)
         )
-        df["last_3_week_mean"] = df["last_3_week_mean"].fillna(method="ffill")
+        df["last_3_week_mean"] = df["last_3_week_mean"].ffill()
 
         df["last_3_week_std"] = (
             df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
             .rolling(window=3, min_periods=1)
             .std()
             .reset_index(level=[0, 1], drop=True)
         )
-        df["last_3_week_std"] = df["last_3_week_std"].fillna(method="ffill")
+        df["last_3_week_std"] = df["last_3_week_std"].ffill()
 
         df["last_3_week_max"] = (
             df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
             .rolling(window=3, min_periods=1)
             .max()
             .reset_index(level=[0, 1], drop=True)
         )
-        df["last_3_week_max"] = df["last_3_week_max"].fillna(method="ffill")
+        df["last_3_week_max"] = df["last_3_week_max"].ffill()
 
         df["last_3_week_min"] = (
             df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
             .rolling(window=3, min_periods=1)
             .min()
             .reset_index(level=[0, 1], drop=True)
         )
-        df["last_3_week_min"] = df["last_3_week_min"].fillna(method="ffill")
+        df["last_3_week_min"] = df["last_3_week_min"].ffill()
 
         df["last_3_week_skew"] = (
             df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
             .rolling(window=3, min_periods=1)
             .skew()
             .reset_index(level=[0, 1], drop=True)
         )
-        df["last_3_week_skew"] = df["last_3_week_skew"].fillna(method="ffill")
+        df["last_3_week_skew"] = df["last_3_week_skew"].ffill()
         # fill
 
         df["last_3_week_median"] = (
             df.groupby([df.index.weekday, df.index.hour])["consumed_heat_kWh"]
             .rolling(window=3, min_periods=1)
             .median()
             .reset_index(level=[0, 1], drop=True)
         )
-        df["last_3_week_median"] = df["last_3_week_median"].fillna(method="ffill")
+        df["last_3_week_median"] = df["last_3_week_median"].ffill()
 
         df_reverse = df.iloc[::-1]
 
         # getting nan indices and filling them with rolling mean from the end of the dataframe
         nan_indices = df_reverse[df_reverse["last_3_week_skew"].isna()].index
         for index in nan_indices:
```

### Comparing `smartboiler-1.0.7/src/smartboiler/event_checker.py` & `smartboiler-1.0.8/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/src/smartboiler/forecast.py` & `smartboiler-1.0.8/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/src/smartboiler/fotovoltaics.py` & `smartboiler-1.0.8/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/src/smartboiler/switch.py` & `smartboiler-1.0.8/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/src/smartboiler/time_handler.py` & `smartboiler-1.0.8/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.7/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.0.8/src/smartboiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.7/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.0.8/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

