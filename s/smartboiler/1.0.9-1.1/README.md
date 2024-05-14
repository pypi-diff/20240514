# Comparing `tmp/smartboiler-1.0.9.tar.gz` & `tmp/smartboiler-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.9.tar", last modified: Tue May 14 15:54:18 2024, max compression
+gzip compressed data, was "smartboiler-1.1.tar", last modified: Tue May 14 17:58:12 2024, max compression
```

## Comparing `smartboiler-1.0.9.tar` & `smartboiler-1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.937108 smartboiler-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:54:18.937108 smartboiler-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 15:54:16.000000 smartboiler-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:54:18.937108 smartboiler-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 15:54:18.000000 smartboiler-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.933108 smartboiler-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.937108 smartboiler-1.0.9/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    30822 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 15:54:16.000000 smartboiler-1.0.9/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:18.937108 smartboiler-1.0.9/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 15:54:18.000000 smartboiler-1.0.9/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:58:12.254503 smartboiler-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-14 17:58:12.254503 smartboiler-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 17:58:10.000000 smartboiler-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:58:12.254503 smartboiler-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-14 17:58:11.000000 smartboiler-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:58:12.250503 smartboiler-1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:58:12.254503 smartboiler-1.1/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30822 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15582 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 17:58:10.000000 smartboiler-1.1/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:58:12.254503 smartboiler-1.1/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-14 17:58:12.000000 smartboiler-1.1/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 17:58:12.000000 smartboiler-1.1/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:58:12.000000 smartboiler-1.1/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 17:58:12.000000 smartboiler-1.1/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 17:58:12.000000 smartboiler-1.1/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 17:58:12.000000 smartboiler-1.1/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0.9/PKG-INFO` & `smartboiler-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.9
+Version: 1.1
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.9/README.md` & `smartboiler-1.1/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/setup.py` & `smartboiler-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0.9",  # Required
+    version="1.1",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
@@ -48,14 +48,15 @@
         "influxdb==5.3.1",
         "keras==2.15.0",
         "matplotlib==3.5.1",
         "numpy>=1.22.2",
         "pandas>=1.4.1",
         "pytz>=2021.1",
         "requests>=2.25.1",
+        "scikit-learn==1.3.2",
         "scipy<1.9.0",
         "skforecast>=0.10.1",
         "tensorflow",
         "wheel",
     ],
     # Optional
     entry_points={  # Optional
```

### Comparing `smartboiler-1.0.9/src/smartboiler/boiler.py` & `smartboiler-1.1/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/src/smartboiler/controller.py` & `smartboiler-1.1/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/src/smartboiler/data_handler.py` & `smartboiler-1.1/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/src/smartboiler/event_checker.py` & `smartboiler-1.1/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/src/smartboiler/forecast.py` & `smartboiler-1.1/src/smartboiler/forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
                 restore_best_weights=True,
             ),
             ModelCheckpoint(
                 verbose=1,
                 filepath=self.model_path,
                 save_best_only=True,
                 save_weights_only=True,
+                include_optimizer=True,
             ),
         ]
 
         # fit the model
         history = self.model.fit(
             self.train_gen,
             steps_per_epoch=self.train_steps,
```

### Comparing `smartboiler-1.0.9/src/smartboiler/fotovoltaics.py` & `smartboiler-1.1/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/src/smartboiler/switch.py` & `smartboiler-1.1/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/src/smartboiler/time_handler.py` & `smartboiler-1.1/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.9/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.1/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.9
+Version: 1.1
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.9/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.1/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

