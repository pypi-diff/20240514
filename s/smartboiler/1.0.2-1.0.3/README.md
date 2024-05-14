# Comparing `tmp/smartboiler-1.0.2.tar.gz` & `tmp/smartboiler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.2.tar", last modified: Tue May 14 12:09:17 2024, max compression
+gzip compressed data, was "smartboiler-1.0.3.tar", last modified: Tue May 14 13:56:23 2024, max compression
```

## Comparing `smartboiler-1.0.2.tar` & `smartboiler-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 12:09:17.123467 smartboiler-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 12:09:13.000000 smartboiler-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:09:17.123467 smartboiler-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 12:09:15.000000 smartboiler-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 12:09:13.000000 smartboiler-1.0.2/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:17.123467 smartboiler-1.0.2/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 12:09:17.000000 smartboiler-1.0.2/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:56:23.354311 smartboiler-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 13:56:23.354311 smartboiler-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 13:56:21.000000 smartboiler-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:56:23.354311 smartboiler-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 13:56:22.000000 smartboiler-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:56:23.350311 smartboiler-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:56:23.350311 smartboiler-1.0.3/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 13:56:21.000000 smartboiler-1.0.3/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:56:23.350311 smartboiler-1.0.3/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 13:56:23.000000 smartboiler-1.0.3/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 13:56:23.000000 smartboiler-1.0.3/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:56:23.000000 smartboiler-1.0.3/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 13:56:23.000000 smartboiler-1.0.3/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 13:56:23.000000 smartboiler-1.0.3/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 13:56:23.000000 smartboiler-1.0.3/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0.2/PKG-INFO` & `smartboiler-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.2/README.md` & `smartboiler-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/setup.py` & `smartboiler-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0.2",  # Required
+    version="1.0.3",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-1.0.2/src/smartboiler/boiler.py` & `smartboiler-1.0.3/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/src/smartboiler/controller.py` & `smartboiler-1.0.3/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/src/smartboiler/data_handler.py` & `smartboiler-1.0.3/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/src/smartboiler/event_checker.py` & `smartboiler-1.0.3/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/src/smartboiler/forecast.py` & `smartboiler-1.0.3/src/smartboiler/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,25 +181,21 @@
         model.add(Input(shape=(None, self.num_of_features)))
         model.add(LSTM(100))
         model.add(Dense(1))
 
         # compile the model with the quantile loss and adam optimizer
         self.model = model
         self.model.compile(
-          loss=lambda y_true, y_pred: self.quantile_loss_wrapper(y_true, y_pred),
+          loss=[
+                lambda y_true, y_pred: self.quantile_loss(q, y_true, y_pred)
+                for q in self.quantiles
+            ],
 
             optimizer="adam",
         )
-        
-    def quantile_loss_wrapper(self, y_true, y_pred) -> float:
-        """Wrapper function to compute quantile loss for multiple quantiles"""
-        loss = 0
-        for i, q in enumerate(self.quantiles):
-            loss += self.quantile_loss(q, y_true, y_pred)
-        return loss
 
     def add_empty_row(
         self, df: pd.DataFrame, date_time: datetime, predicted_value: float
     ) -> pd.DataFrame:
         """Methot adding an empty row to the dataframe
 
         Args:
```

### Comparing `smartboiler-1.0.2/src/smartboiler/fotovoltaics.py` & `smartboiler-1.0.3/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/src/smartboiler/switch.py` & `smartboiler-1.0.3/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/src/smartboiler/time_handler.py` & `smartboiler-1.0.3/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.2/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.0.3/src/smartboiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.2/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.0.3/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

