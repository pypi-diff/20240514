# Comparing `tmp/smartboiler-1.0.1.tar.gz` & `tmp/smartboiler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.1.tar", last modified: Tue May 14 11:39:59 2024, max compression
+gzip compressed data, was "smartboiler-1.0.2.tar", last modified: Tue May 14 12:09:17 2024, max compression
```

## Comparing `smartboiler-1.0.1.tar` & `smartboiler-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.843484 smartboiler-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 11:39:59.843484 smartboiler-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 11:39:57.000000 smartboiler-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:39:59.843484 smartboiler-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 11:39:59.000000 smartboiler-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.839484 smartboiler-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.843484 smartboiler-1.0.1/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31760 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.843484 smartboiler-1.0.1/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 12:09:17.123467 smartboiler-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 12:09:13.000000 smartboiler-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:09:17.123467 smartboiler-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 12:09:15.000000 smartboiler-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0.1/PKG-INFO` & `smartboiler-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.1
+Version: 1.0.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.1/README.md` & `smartboiler-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.1/setup.py` & `smartboiler-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0.1",  # Required
+    version="1.0.2",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-1.0.1/src/smartboiler/boiler.py` & `smartboiler-1.0.2/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.1/src/smartboiler/controller.py` & `smartboiler-1.0.2/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.1/src/smartboiler/data_handler.py` & `smartboiler-1.0.2/src/smartboiler/data_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -393,54 +393,15 @@
 
         # transform kj to kWh
         df["consumed_heat_kWh"] = df["consumed_heat_kJ"] / 3600
         df = df.drop(columns=["consumed_heat_kJ"])
 
         return df
 
-    def get_data_for_training_model(
-        self,
-        left_time_interval: Optional[datetime] = None,
-        right_time_interval: Optional[datetime] = None,
-    ) -> pd.DataFrame:
-        """Method to retrieve data for training.
-
-        Args:
-            left_time_interval (Optional[datetime], optional): Left time datetime. Defaults to self.start_of_data.
-            right_time_interval (Optional[datetime], optional): Right time datetime. Defaults to datetime.now().
-
-        Returns:
-            pd.DataFrame: Resulting dataframe.
-        """
-
-        # default the intervals if None
-        if left_time_interval is None:
-            left_time_interval = self.start_of_data
-
-        if right_time_interval is None:
-            right_time_interval = datetime.now()
-
-        left_time_interval = left_time_interval.replace(
-            minute=0, second=0, microsecond=0
-        )
-        right_time_interval = right_time_interval.replace(
-            minute=0, second=0, microsecond=0
-        )
-
-        # retrieve the queries based on the intervals
-        queries = self.get_database_queries(
-            left_time_interval=left_time_interval,
-            right_time_interval=right_time_interval,
-        )
-        # get the data from the database
-        df_all = self.get_df_from_queries(queries)
-        # process the data
-        df_all = self.process_kWh_water_consumption(df_all)
-        # transform for ML
-        return self.transform_data_for_ml(df_all)
+    
 
     def get_data_for_prediction(
         self,
         left_time_interval: Optional[datetime] = None,
         right_time_interval: Optional[datetime] = None,
     ) -> tuple[pd.DataFrame, pd.DatetimeIndex]:
         """Method to get data for the prediction.
@@ -476,17 +437,34 @@
         # process the data
         df_all = self.process_kWh_water_consumption(df_all)
 
         # transform the data for ML
         df_all.index = df_all.index.tz_localize(None)
 
         # return the dataframe and the datetimes
-        df_all, datetimes = self.transform_data_for_ml(df_all)
+        df_all, _ = self.transform_data_for_ml(df_all)
+        
+        df_all['temperature'] = df_all['temperature'].combine_first(df_all['temperature'])
+        df_all['humidity'] = df_all['humidity'].combine_first(df_all['humidity'])
+        df_all['wind_speed'] = df_all['wind_speed'].combine_first(df_all['wind_speed'])
+
+        # ffill this values
+        df_all['temperature'] = df_all['temperature'].ffill()
+        df_all['humidity'] = df_all['humidity'].ffill()
+        df_all['wind_speed'] = df_all['wind_speed'].ffill()
+        df_all = df_all.reset_index(drop=True)
+        
+        df_all = df_all.reset_index(drop=True).copy()
+        # drop rows where last_3_week_skew is nan
+        df_all = df_all.dropna(subset=['last_3_week_skew'])
+        # reduce distance greater than 50
+        df_all['distance_from_home'] = df_all['distance_from_home'].apply(lambda x: x if x < 50 else 50)
+
 
-        return df_all, datetimes
+        return df_all
 
     def write_forecast_to_influxdb(self, df: pd.DataFrame) -> None:
         """Method which writes the current forecast to the influxdb.
 
         Args:
             df (pd.DataFrame): Dataframe with current prediction.
         """
```

### Comparing `smartboiler-1.0.1/src/smartboiler/event_checker.py` & `smartboiler-1.0.2/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.1/src/smartboiler/forecast.py` & `smartboiler-1.0.2/src/smartboiler/forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         # if the data for training is not provided, get the data from the dataHandler
         if df_training_data is None:
             if begin_of_training is None:
                 begin_of_training = self.start_of_data
             if end_of_training is None:
                 end_of_training = datetime.now()
-            df_training_data, _ = self.dataHandler.get_data_for_training_model(
+            df_training_data = self.dataHandler.get_data_for_prediction(
                 left_time_interval=begin_of_training,
                 right_time_interval=end_of_training,
             )
         # get the number of features
         self.num_of_features = len(df_training_data.columns) - 1
 
         # fit the scaler
@@ -336,15 +336,15 @@
         """
         if left_time_interval is None:
             left_time_interval = datetime.now() - timedelta(days=30)
         if right_time_interval is None:
             right_time_interval = datetime.now()
 
         # get data for creatig a prediction
-        df_all, datetimes = self.dataHandler.get_data_for_prediction(
+        df_all = self.dataHandler.get_data_for_prediction(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
 
         number_of_targets = len(self.predicted_columns)
         number_of_columns = len(df_all.columns)
         number_of_features = number_of_columns - number_of_targets
```

### Comparing `smartboiler-1.0.1/src/smartboiler/fotovoltaics.py` & `smartboiler-1.0.2/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.1/src/smartboiler/switch.py` & `smartboiler-1.0.2/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.1/src/smartboiler/time_handler.py` & `smartboiler-1.0.2/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.1/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.0.2/src/smartboiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.1
+Version: 1.0.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.1/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.0.2/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

