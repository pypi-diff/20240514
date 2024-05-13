# Comparing `tmp/distclassipy-0.1.3.tar.gz` & `tmp/distclassipy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distclassipy-0.1.3.tar", last modified: Thu Apr 18 06:41:29 2024, max compression
+gzip compressed data, was "distclassipy-0.1.4.tar", last modified: Thu Apr 18 07:21:55 2024, max compression
```

## Comparing `distclassipy-0.1.3.tar` & `distclassipy-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.139538 distclassipy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 06:41:23.000000 distclassipy-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46355 2024-04-18 06:41:29.139538 distclassipy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-18 06:41:23.000000 distclassipy-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.135538 distclassipy-0.1.3/distclassipy/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 06:41:23.000000 distclassipy-0.1.3/distclassipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18143 2024-04-18 06:41:23.000000 distclassipy-0.1.3/distclassipy/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    49563 2024-04-18 06:41:23.000000 distclassipy-0.1.3/distclassipy/distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.139538 distclassipy-0.1.3/distclassipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46355 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 06:41:23.000000 distclassipy-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:41:29.139538 distclassipy-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-18 06:41:23.000000 distclassipy-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.139538 distclassipy-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-18 06:41:23.000000 distclassipy-0.1.3/tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 06:41:23.000000 distclassipy-0.1.3/tests/test_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:21:55.342859 distclassipy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 07:21:48.000000 distclassipy-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46355 2024-04-18 07:21:55.342859 distclassipy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-18 07:21:48.000000 distclassipy-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:21:55.342859 distclassipy-0.1.4/distclassipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 07:21:48.000000 distclassipy-0.1.4/distclassipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18143 2024-04-18 07:21:48.000000 distclassipy-0.1.4/distclassipy/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49563 2024-04-18 07:21:48.000000 distclassipy-0.1.4/distclassipy/distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:21:55.342859 distclassipy-0.1.4/distclassipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46355 2024-04-18 07:21:55.000000 distclassipy-0.1.4/distclassipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-18 07:21:55.000000 distclassipy-0.1.4/distclassipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:21:55.000000 distclassipy-0.1.4/distclassipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 07:21:55.000000 distclassipy-0.1.4/distclassipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 07:21:55.000000 distclassipy-0.1.4/distclassipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 07:21:48.000000 distclassipy-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:21:55.342859 distclassipy-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-18 07:21:48.000000 distclassipy-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:21:55.342859 distclassipy-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-18 07:21:48.000000 distclassipy-0.1.4/tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 07:21:48.000000 distclassipy-0.1.4/tests/test_distances.py
```

### Comparing `distclassipy-0.1.3/LICENSE` & `distclassipy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `distclassipy-0.1.3/PKG-INFO` & `distclassipy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distclassipy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for a distance-based classifier which can use several different distance metrics.
 Author-email: Siddharth Chaini <sidchaini@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,17 +690,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.3.2
-Requires-Dist: numpy>=1.26.3
-Requires-Dist: pandas>=2.2.0
-Requires-Dist: scikit-learn>=1.4.0
+Requires-Dist: numpy>=1.25.2
+Requires-Dist: pandas>=2.0.3
+Requires-Dist: scikit-learn>=1.2.2
 
 <h1 align="center">
 <picture align="center">
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sidchaini/DistClassiPy/main/docs/_static/logo-dark.svg" width="300">
   <img alt="DistClassiPy Logo" src="https://raw.githubusercontent.com/sidchaini/DistClassiPy/main/docs/_static/logo.svg" width="300">
 </picture>
 </h1>
```

### Comparing `distclassipy-0.1.3/README.md` & `distclassipy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `distclassipy-0.1.3/distclassipy/__init__.py` & `distclassipy-0.1.4/distclassipy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from .classifier import (
     DistanceMetricClassifier,
 )  # Importing the DistanceMetricClassifier from the classifier module
 from .distances import (
     Distance,
 )  # Importing the Distance class from the distances module
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `distclassipy-0.1.3/distclassipy/classifier.py` & `distclassipy-0.1.4/distclassipy/classifier.py`

 * *Files identical despite different names*

### Comparing `distclassipy-0.1.3/distclassipy/distances.py` & `distclassipy-0.1.4/distclassipy/distances.py`

 * *Files identical despite different names*

### Comparing `distclassipy-0.1.3/distclassipy.egg-info/PKG-INFO` & `distclassipy-0.1.4/distclassipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distclassipy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for a distance-based classifier which can use several different distance metrics.
 Author-email: Siddharth Chaini <sidchaini@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,17 +690,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.3.2
-Requires-Dist: numpy>=1.26.3
-Requires-Dist: pandas>=2.2.0
-Requires-Dist: scikit-learn>=1.4.0
+Requires-Dist: numpy>=1.25.2
+Requires-Dist: pandas>=2.0.3
+Requires-Dist: scikit-learn>=1.2.2
 
 <h1 align="center">
 <picture align="center">
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sidchaini/DistClassiPy/main/docs/_static/logo-dark.svg" width="300">
   <img alt="DistClassiPy Logo" src="https://raw.githubusercontent.com/sidchaini/DistClassiPy/main/docs/_static/logo.svg" width="300">
 </picture>
 </h1>
```

### Comparing `distclassipy-0.1.3/pyproject.toml` & `distclassipy-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "joblib>=1.3.2",
-    "numpy>=1.26.3",
-    "pandas>=2.2.0",
-    "scikit-learn>=1.4.0"
+    "numpy>=1.25.2",
+    "pandas>=2.0.3",
+    "scikit-learn>=1.2.2"
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "distclassipy.__version__"}
 
 [project.urls]
 Repository = "https://github.com/sidchaini/DistClassiPy"
```

### Comparing `distclassipy-0.1.3/setup.py` & `distclassipy-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `distclassipy-0.1.3/tests/test_classifier.py` & `distclassipy-0.1.4/tests/test_classifier.py`

 * *Files identical despite different names*

