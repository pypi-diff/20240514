# Comparing `tmp/smartboiler-1.0.4.tar.gz` & `tmp/smartboiler-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-1.0.4.tar", last modified: Tue May 14 14:48:46 2024, max compression
+gzip compressed data, was "smartboiler-1.0.5.tar", last modified: Tue May 14 14:59:14 2024, max compression
```

## Comparing `smartboiler-1.0.4.tar` & `smartboiler-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:46.358687 smartboiler-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 14:48:46.358687 smartboiler-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 14:48:44.000000 smartboiler-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:48:46.358687 smartboiler-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-14 14:48:45.000000 smartboiler-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:46.354688 smartboiler-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:46.358687 smartboiler-1.0.4/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 14:48:44.000000 smartboiler-1.0.4/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:46.358687 smartboiler-1.0.4/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 14:48:46.000000 smartboiler-1.0.4/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 14:48:46.000000 smartboiler-1.0.4/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:48:46.000000 smartboiler-1.0.4/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 14:48:46.000000 smartboiler-1.0.4/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-14 14:48:46.000000 smartboiler-1.0.4/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 14:48:46.000000 smartboiler-1.0.4/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:59:14.960199 smartboiler-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 14:59:14.960199 smartboiler-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-14 14:59:12.000000 smartboiler-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:59:14.960199 smartboiler-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 14:59:14.000000 smartboiler-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:59:14.956199 smartboiler-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:59:14.960199 smartboiler-1.0.5/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 14:59:12.000000 smartboiler-1.0.5/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:59:14.960199 smartboiler-1.0.5/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 14:59:14.000000 smartboiler-1.0.5/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 14:59:14.000000 smartboiler-1.0.5/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:59:14.000000 smartboiler-1.0.5/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 14:59:14.000000 smartboiler-1.0.5/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 14:59:14.000000 smartboiler-1.0.5/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 14:59:14.000000 smartboiler-1.0.5/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-1.0.4/PKG-INFO` & `smartboiler-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.4
+Version: 1.0.5
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.4/README.md` & `smartboiler-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/setup.py` & `smartboiler-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="1.0.4",  # Required
+    version="1.0.5",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
@@ -50,15 +50,15 @@
         "matplotlib==3.5.1",
         "numpy>=1.22.2",
         "pandas>=1.4.1",
         "pytz>=2021.1",
         "requests>=2.25.1",
         "scipy<1.9.0",
         "skforecast>=0.10.1",
-        "tensorflow==2.15.0",
+        "tensorflow",
         "wheel",
     ],
     # Optional
     entry_points={  # Optional
         "console_scripts": [
             "smartboiler=smartboiler.command_line:main",
         ],
```

### Comparing `smartboiler-1.0.4/src/smartboiler/boiler.py` & `smartboiler-1.0.5/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler/controller.py` & `smartboiler-1.0.5/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler/data_handler.py` & `smartboiler-1.0.5/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler/event_checker.py` & `smartboiler-1.0.5/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler/forecast.py` & `smartboiler-1.0.5/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler/fotovoltaics.py` & `smartboiler-1.0.5/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler/switch.py` & `smartboiler-1.0.5/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler/time_handler.py` & `smartboiler-1.0.5/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-1.0.4/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-1.0.5/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 1.0.4
+Version: 1.0.5
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-1.0.4/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-1.0.5/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

