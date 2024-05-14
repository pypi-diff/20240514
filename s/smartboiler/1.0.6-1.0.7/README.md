# Comparing `tmp/smartboiler-1.0.6.tar.gz` & `tmp/smartboiler-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.6.tar", last modified: Tue May 14 15:31:31 2024, max compression
+gzip compressed data, was "smartboiler-1.0.7.tar", last modified: Tue May 14 15:44:23 2024, max compression
```

## Comparing `smartboiler-1.0.6.tar` & `smartboiler-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:31:31.872965 smartboiler-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:31:31.872965 smartboiler-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 15:31:26.000000 smartboiler-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:31:31.872965 smartboiler-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 15:31:30.000000 smartboiler-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:31:31.868965 smartboiler-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:31:31.868965 smartboiler-1.0.6/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 15:31:26.000000 smartboiler-1.0.6/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:31:31.872965 smartboiler-1.0.6/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:31:31.000000 smartboiler-1.0.6/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 15:31:31.000000 smartboiler-1.0.6/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:31:31.000000 smartboiler-1.0.6/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:31:31.000000 smartboiler-1.0.6/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 15:31:31.000000 smartboiler-1.0.6/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 15:31:31.000000 smartboiler-1.0.6/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.759455 smartboiler-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:44:23.759455 smartboiler-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 15:44:19.000000 smartboiler-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:44:23.759455 smartboiler-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 15:44:22.000000 smartboiler-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.755455 smartboiler-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.759455 smartboiler-1.0.7/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 15:44:19.000000 smartboiler-1.0.7/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:44:23.759455 smartboiler-1.0.7/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 15:44:23.000000 smartboiler-1.0.7/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0.6/PKG-INFO` & `smartboiler-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.6
+Version: 1.0.7
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.6/README.md` & `smartboiler-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/setup.py` & `smartboiler-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0.6",  # Required
+    version="1.0.7",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-1.0.6/src/smartboiler/boiler.py` & `smartboiler-1.0.7/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/src/smartboiler/controller.py` & `smartboiler-1.0.7/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/src/smartboiler/data_handler.py` & `smartboiler-1.0.7/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/src/smartboiler/event_checker.py` & `smartboiler-1.0.7/src/smartboiler/event_checker.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,18 +99,18 @@
                     start = self.TimeHandler.date_to_datetime(
                         e["start"].get("dateTime", e["start"].get("date"))
                     )
                     end = self.TimeHandler.date_to_datetime(
                         e["end"].get("dateTime", e["end"].get("date"))
                     )
                     time_to_event = (
-                        start - (datetime.now() + timedelta(hours=1))
+                        start - datetime.now(timezone.utc)
                     ) / timedelta(hours=1)
                     time_to_end_event = (
-                        end - (datetime.now() + timedelta(hours=1))
+                        end - datetime.now(timezone.utc)
                     ) / timedelta(hours=1)
 
                     if time_to_event > 0:
 
                         return_dict["minutes_to_event"] = time_to_event * 60
                         return_dict["degree_target"] = degree_target
```

### Comparing `smartboiler-1.0.6/src/smartboiler/forecast.py` & `smartboiler-1.0.7/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/src/smartboiler/fotovoltaics.py` & `smartboiler-1.0.7/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/src/smartboiler/switch.py` & `smartboiler-1.0.7/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/src/smartboiler/time_handler.py` & `smartboiler-1.0.7/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.6/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.0.7/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.6
+Version: 1.0.7
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.6/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.0.7/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

