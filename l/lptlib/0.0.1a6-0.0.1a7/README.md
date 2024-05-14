# Comparing `tmp/lptlib-0.0.1a6.tar.gz` & `tmp/lptlib-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lptlib-0.0.1a6.tar", last modified: Mon May 13 21:54:43 2024, max compression
+gzip compressed data, was "lptlib-0.0.1a7.tar", last modified: Mon May 13 22:51:07 2024, max compression
```

## Comparing `lptlib-0.0.1a6.tar` & `lptlib-0.0.1a7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.573392 lptlib-0.0.1a6/
--rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a6/LICENSE
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 21:54:43.572741 lptlib-0.0.1a6/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a6/README.md
--rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 21:54:39.000000 lptlib-0.0.1a6/pyproject.toml
--rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 21:54:43.573562 lptlib-0.0.1a6/setup.cfg
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.551407 lptlib-0.0.1a6/src/
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.553850 lptlib-0.0.1a6/src/lptlib/
--rw-r--r--   0 kal        (501) staff       (20)        0 2024-05-13 21:32:10.000000 lptlib-0.0.1a6/src/lptlib/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.558461 lptlib-0.0.1a6/src/lptlib/function/
--rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a6/src/lptlib/function/__init__.py
--rwx------   0 kal        (501) staff       (20)    12533 2024-05-13 21:39:16.000000 lptlib-0.0.1a6/src/lptlib/function/plots.py
--rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a6/src/lptlib/function/timer.py
--rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a6/src/lptlib/function/variables.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.559984 lptlib-0.0.1a6/src/lptlib/io/
--rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a6/src/lptlib/io/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    14877 2024-05-13 21:52:46.000000 lptlib-0.0.1a6/src/lptlib/io/dataio.py
--rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a6/src/lptlib/io/plot3dio.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.563032 lptlib-0.0.1a6/src/lptlib/streamlines/
--rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a6/src/lptlib/streamlines/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    34469 2024-05-13 21:54:19.000000 lptlib-0.0.1a6/src/lptlib/streamlines/integration.py
--rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a6/src/lptlib/streamlines/interpolation.py
--rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a6/src/lptlib/streamlines/search.py
--rw-r--r--   0 kal        (501) staff       (20)     7537 2024-05-13 21:50:14.000000 lptlib-0.0.1a6/src/lptlib/streamlines/stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)    39727 2024-05-13 21:49:30.000000 lptlib-0.0.1a6/src/lptlib/streamlines/streamlines.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.564097 lptlib-0.0.1a6/src/lptlib/test_cases/
--rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a6/src/lptlib/test_cases/__init__.py
--rwx------   0 kal        (501) staff       (20)    10018 2024-05-13 17:51:47.000000 lptlib-0.0.1a6/src/lptlib/test_cases/oblique_shock_data.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.571878 lptlib-0.0.1a6/src/lptlib.egg-info/
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 21:54:43.000000 lptlib-0.0.1a6/src/lptlib.egg-info/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)     1010 2024-05-13 21:54:43.000000 lptlib-0.0.1a6/src/lptlib.egg-info/SOURCES.txt
--rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 21:54:43.000000 lptlib-0.0.1a6/src/lptlib.egg-info/dependency_links.txt
--rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 21:54:43.000000 lptlib-0.0.1a6/src/lptlib.egg-info/requires.txt
--rw-r--r--   0 kal        (501) staff       (20)        7 2024-05-13 21:54:43.000000 lptlib-0.0.1a6/src/lptlib.egg-info/top_level.txt
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:54:43.571154 lptlib-0.0.1a6/test/
--rw-r--r--   0 kal        (501) staff       (20)     1011 2024-05-13 17:51:47.000000 lptlib-0.0.1a6/test/test_dataio.py
--rwx------   0 kal        (501) staff       (20)      468 2024-05-13 17:51:47.000000 lptlib-0.0.1a6/test/test_import.py
--rwx------   0 kal        (501) staff       (20)     2350 2024-05-13 17:40:07.000000 lptlib-0.0.1a6/test/test_integration.py
--rw-r--r--   0 kal        (501) staff       (20)     2016 2024-05-13 17:40:07.000000 lptlib-0.0.1a6/test/test_interpolation.py
--rwx------   0 kal        (501) staff       (20)     1148 2024-05-13 17:40:08.000000 lptlib-0.0.1a6/test/test_oblique_shock_data.py
--rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a6/test/test_plot.py
--rw-r--r--   0 kal        (501) staff       (20)     7324 2024-05-13 17:40:08.000000 lptlib-0.0.1a6/test/test_plot3dio.py
--rwx------   0 kal        (501) staff       (20)     2607 2024-05-13 17:40:08.000000 lptlib-0.0.1a6/test/test_plots.py
--rw-r--r--   0 kal        (501) staff       (20)     3260 2024-05-13 17:40:07.000000 lptlib-0.0.1a6/test/test_search.py
--rw-r--r--   0 kal        (501) staff       (20)     1914 2024-05-13 17:40:07.000000 lptlib-0.0.1a6/test/test_stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)     1399 2024-05-13 17:40:07.000000 lptlib-0.0.1a6/test/test_terminal_run.py
--rwx------   0 kal        (501) staff       (20)     2696 2024-05-13 17:40:07.000000 lptlib-0.0.1a6/test/test_variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.176360 lptlib-0.0.1a7/
+-rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a7/LICENSE
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 22:51:07.175662 lptlib-0.0.1a7/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a7/README.md
+-rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 22:50:52.000000 lptlib-0.0.1a7/pyproject.toml
+-rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 22:51:07.176523 lptlib-0.0.1a7/setup.cfg
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.158154 lptlib-0.0.1a7/src/
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.161011 lptlib-0.0.1a7/src/lptlib/
+-rw-r--r--   0 kal        (501) staff       (20)        0 2024-05-13 21:32:10.000000 lptlib-0.0.1a7/src/lptlib/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.164984 lptlib-0.0.1a7/src/lptlib/function/
+-rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a7/src/lptlib/function/__init__.py
+-rwx------   0 kal        (501) staff       (20)    12533 2024-05-13 21:39:16.000000 lptlib-0.0.1a7/src/lptlib/function/plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a7/src/lptlib/function/timer.py
+-rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a7/src/lptlib/function/variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.166283 lptlib-0.0.1a7/src/lptlib/io/
+-rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a7/src/lptlib/io/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    14877 2024-05-13 21:52:46.000000 lptlib-0.0.1a7/src/lptlib/io/dataio.py
+-rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a7/src/lptlib/io/plot3dio.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.169021 lptlib-0.0.1a7/src/lptlib/streamlines/
+-rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a7/src/lptlib/streamlines/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    34469 2024-05-13 21:54:19.000000 lptlib-0.0.1a7/src/lptlib/streamlines/integration.py
+-rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a7/src/lptlib/streamlines/interpolation.py
+-rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a7/src/lptlib/streamlines/search.py
+-rw-r--r--   0 kal        (501) staff       (20)     7537 2024-05-13 21:50:14.000000 lptlib-0.0.1a7/src/lptlib/streamlines/stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)    39727 2024-05-13 21:49:30.000000 lptlib-0.0.1a7/src/lptlib/streamlines/streamlines.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.170038 lptlib-0.0.1a7/src/lptlib/test_cases/
+-rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a7/src/lptlib/test_cases/__init__.py
+-rwx------   0 kal        (501) staff       (20)     9831 2024-05-13 22:50:52.000000 lptlib-0.0.1a7/src/lptlib/test_cases/oblique_shock_data.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.174998 lptlib-0.0.1a7/src/lptlib.egg-info/
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 22:51:07.000000 lptlib-0.0.1a7/src/lptlib.egg-info/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)     1010 2024-05-13 22:51:07.000000 lptlib-0.0.1a7/src/lptlib.egg-info/SOURCES.txt
+-rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 22:51:07.000000 lptlib-0.0.1a7/src/lptlib.egg-info/dependency_links.txt
+-rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 22:51:07.000000 lptlib-0.0.1a7/src/lptlib.egg-info/requires.txt
+-rw-r--r--   0 kal        (501) staff       (20)        7 2024-05-13 22:51:07.000000 lptlib-0.0.1a7/src/lptlib.egg-info/top_level.txt
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 22:51:07.174497 lptlib-0.0.1a7/test/
+-rw-r--r--   0 kal        (501) staff       (20)     1011 2024-05-13 17:51:47.000000 lptlib-0.0.1a7/test/test_dataio.py
+-rwx------   0 kal        (501) staff       (20)      468 2024-05-13 17:51:47.000000 lptlib-0.0.1a7/test/test_import.py
+-rwx------   0 kal        (501) staff       (20)     2350 2024-05-13 17:40:07.000000 lptlib-0.0.1a7/test/test_integration.py
+-rw-r--r--   0 kal        (501) staff       (20)     2016 2024-05-13 17:40:07.000000 lptlib-0.0.1a7/test/test_interpolation.py
+-rwx------   0 kal        (501) staff       (20)     1148 2024-05-13 17:40:08.000000 lptlib-0.0.1a7/test/test_oblique_shock_data.py
+-rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a7/test/test_plot.py
+-rw-r--r--   0 kal        (501) staff       (20)     7324 2024-05-13 17:40:08.000000 lptlib-0.0.1a7/test/test_plot3dio.py
+-rwx------   0 kal        (501) staff       (20)     2607 2024-05-13 17:40:08.000000 lptlib-0.0.1a7/test/test_plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     3260 2024-05-13 17:40:07.000000 lptlib-0.0.1a7/test/test_search.py
+-rw-r--r--   0 kal        (501) staff       (20)     1914 2024-05-13 17:40:07.000000 lptlib-0.0.1a7/test/test_stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)     1399 2024-05-13 17:40:07.000000 lptlib-0.0.1a7/test/test_terminal_run.py
+-rwx------   0 kal        (501) staff       (20)     2696 2024-05-13 17:40:07.000000 lptlib-0.0.1a7/test/test_variables.py
```

### Comparing `lptlib-0.0.1a6/LICENSE` & `lptlib-0.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/PKG-INFO` & `lptlib-0.0.1a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a6/README.md` & `lptlib-0.0.1a7/README.md`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/pyproject.toml` & `lptlib-0.0.1a7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lptlib"
-version = "0.0.1a6"
+version = "0.0.1a7"
 authors = [
     {name="Dilip Kalagotla"},
     {email="dilipkalagotla@gmail.com"},
     ]
 description = "One-way coupled Lagrangian Particle Tracking algorithms."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lptlib-0.0.1a6/src/lptlib/function/plots.py` & `lptlib-0.0.1a7/src/lptlib/function/plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/function/timer.py` & `lptlib-0.0.1a7/src/lptlib/function/timer.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/function/variables.py` & `lptlib-0.0.1a7/src/lptlib/function/variables.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/io/dataio.py` & `lptlib-0.0.1a7/src/lptlib/io/dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/io/plot3dio.py` & `lptlib-0.0.1a7/src/lptlib/io/plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/streamlines/integration.py` & `lptlib-0.0.1a7/src/lptlib/streamlines/integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/streamlines/interpolation.py` & `lptlib-0.0.1a7/src/lptlib/streamlines/interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/streamlines/search.py` & `lptlib-0.0.1a7/src/lptlib/streamlines/search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/streamlines/stochastic_model.py` & `lptlib-0.0.1a7/src/lptlib/streamlines/stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/streamlines/streamlines.py` & `lptlib-0.0.1a7/src/lptlib/streamlines/streamlines.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/src/lptlib/test_cases/oblique_shock_data.py` & `lptlib-0.0.1a7/src/lptlib/test_cases/oblique_shock_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 # Class to calculate particle response across an oblique shock
 
 import numpy as np
-from scipy.optimize import newton
-from src.lptlib.streamlines.stochastic_model import StochasticModel, Particle, SpawnLocations
-import matplotlib.pyplot as plt
-import os
-import glob
 
 
 # Create a class to calculate oblique shock properties from given mach and deflection angle
 class ObliqueShock:
     """
     Class to calculate oblique shock properties from given mach and deflection angle
```

### Comparing `lptlib-0.0.1a6/src/lptlib.egg-info/PKG-INFO` & `lptlib-0.0.1a7/src/lptlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a6/src/lptlib.egg-info/SOURCES.txt` & `lptlib-0.0.1a7/src/lptlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_dataio.py` & `lptlib-0.0.1a7/test/test_dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_integration.py` & `lptlib-0.0.1a7/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_interpolation.py` & `lptlib-0.0.1a7/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_oblique_shock_data.py` & `lptlib-0.0.1a7/test/test_oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_plot.py` & `lptlib-0.0.1a7/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_plot3dio.py` & `lptlib-0.0.1a7/test/test_plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_plots.py` & `lptlib-0.0.1a7/test/test_plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_search.py` & `lptlib-0.0.1a7/test/test_search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_stochastic_model.py` & `lptlib-0.0.1a7/test/test_stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_terminal_run.py` & `lptlib-0.0.1a7/test/test_terminal_run.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a6/test/test_variables.py` & `lptlib-0.0.1a7/test/test_variables.py`

 * *Files identical despite different names*

