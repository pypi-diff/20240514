# Comparing `tmp/smartboiler-1.0.tar.gz` & `tmp/smartboiler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.tar", last modified: Tue May 14 08:11:19 2024, max compression
+gzip compressed data, was "smartboiler-1.0.1.tar", last modified: Tue May 14 11:39:59 2024, max compression
```

## Comparing `smartboiler-1.0.tar` & `smartboiler-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:11:19.667735 smartboiler-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-14 08:11:19.667735 smartboiler-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 08:11:17.000000 smartboiler-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:11:19.667735 smartboiler-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-14 08:11:19.000000 smartboiler-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:11:19.663735 smartboiler-1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:11:19.667735 smartboiler-1.0/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31760 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 08:11:17.000000 smartboiler-1.0/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:11:19.667735 smartboiler-1.0/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-14 08:11:19.000000 smartboiler-1.0/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 08:11:19.000000 smartboiler-1.0/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:11:19.000000 smartboiler-1.0/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 08:11:19.000000 smartboiler-1.0/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 08:11:19.000000 smartboiler-1.0/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 08:11:19.000000 smartboiler-1.0/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.843484 smartboiler-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 11:39:59.843484 smartboiler-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 11:39:57.000000 smartboiler-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:39:59.843484 smartboiler-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 11:39:59.000000 smartboiler-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.839484 smartboiler-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.843484 smartboiler-1.0.1/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31760 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 11:39:57.000000 smartboiler-1.0.1/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:39:59.843484 smartboiler-1.0.1/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 11:39:59.000000 smartboiler-1.0.1/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0/PKG-INFO` & `smartboiler-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0
+Version: 1.0.1
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0/README.md` & `smartboiler-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/setup.py` & `smartboiler-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0",  # Required
+    version="1.0.1",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
@@ -46,16 +46,16 @@
         "pandas>=1.4.1",
         "pvlib>=0.10.1",
         "protobuf>=3.0.0",
         "pytz>=2021.1",
         "requests>=2.25.1",
         "beautifulsoup4>=4.9.3",
         "pulp>=2.4",
-        "tensorflow",
-        "keras",
+        "tensorflow==2.15.0",
+        "keras==2.15.0",
         "Mako==1.3.2",
         "pyyaml>=5.4.1",
         "tables==3.7.0",
         "skforecast==0.10.1",
         "influxdb==5.3.1",
         "matplotlib==3.5.1",
         "flask>=2.0.2",
```

### Comparing `smartboiler-1.0/src/smartboiler/boiler.py` & `smartboiler-1.0.1/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/src/smartboiler/controller.py` & `smartboiler-1.0.1/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/src/smartboiler/data_handler.py` & `smartboiler-1.0.1/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/src/smartboiler/event_checker.py` & `smartboiler-1.0.1/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/src/smartboiler/forecast.py` & `smartboiler-1.0.1/src/smartboiler/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,20 +181,25 @@
         model.add(Input(shape=(None, self.num_of_features)))
         model.add(LSTM(100))
         model.add(Dense(1))
 
         # compile the model with the quantile loss and adam optimizer
         self.model = model
         self.model.compile(
-            loss=[
-                lambda y_true, y_pred: self.quantile_loss(q, y_true, y_pred)
-                for q in self.quantiles
-            ],
+          loss=lambda y_true, y_pred: self.quantile_loss_wrapper(y_true, y_pred),
+
             optimizer="adam",
         )
+        
+    def quantile_loss_wrapper(self, y_true, y_pred) -> float:
+        """Wrapper function to compute quantile loss for multiple quantiles"""
+        loss = 0
+        for i, q in enumerate(self.quantiles):
+            loss += self.quantile_loss(q, y_true, y_pred)
+        return loss
 
     def add_empty_row(
         self, df: pd.DataFrame, date_time: datetime, predicted_value: float
     ) -> pd.DataFrame:
         """Methot adding an empty row to the dataframe
 
         Args:
```

### Comparing `smartboiler-1.0/src/smartboiler/fotovoltaics.py` & `smartboiler-1.0.1/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/src/smartboiler/switch.py` & `smartboiler-1.0.1/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/src/smartboiler/time_handler.py` & `smartboiler-1.0.1/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.0.1/src/smartboiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0
+Version: 1.0.1
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.0.1/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

