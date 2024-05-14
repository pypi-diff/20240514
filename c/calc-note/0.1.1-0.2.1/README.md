# Comparing `tmp/calc_note-0.1.1.tar.gz` & `tmp/calc_note-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\calc_note-0.1.1.tar", last modified: Mon Jul  6 12:29:46 2020, max compression
+gzip compressed data, was "dist\calc_note-0.2.1.tar", last modified: Tue May 14 15:16:39 2024, max compression
```

## Comparing `calc_note-0.1.1.tar` & `calc_note-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2020-07-06 12:29:46.628865 calc_note-0.1.1/
--rw-rw-rw-   0        0        0     2249 2020-07-06 12:29:46.628865 calc_note-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2020-07-06 12:28:42.000000 calc_note-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2020-07-06 12:29:46.612868 calc_note-0.1.1/calc_note/
--rw-rw-rw-   0        0        0        0 2020-07-06 12:06:21.000000 calc_note-0.1.1/calc_note/__init__.py
--rw-rw-rw-   0        0        0       64 2020-07-06 12:29:05.000000 calc_note-0.1.1/calc_note/__version__.py
--rw-rw-rw-   0        0        0      918 2020-07-06 12:14:26.000000 calc_note-0.1.1/calc_note/display.py
-drwxrwxrwx   0        0        0        0 2020-07-06 12:29:46.626868 calc_note-0.1.1/calc_note.egg-info/
--rw-rw-rw-   0        0        0     2249 2020-07-06 12:29:46.000000 calc_note-0.1.1/calc_note.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2020-07-06 12:29:46.000000 calc_note-0.1.1/calc_note.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-06 12:29:46.000000 calc_note-0.1.1/calc_note.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2020-07-06 12:29:46.000000 calc_note-0.1.1/calc_note.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-07-06 12:29:46.628865 calc_note-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3963 2020-07-06 12:29:00.000000 calc_note-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:16:39.038929 calc_note-0.2.1/
+-rw-rw-rw-   0        0        0     2253 2024-05-14 15:16:39.036914 calc_note-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2020-07-06 12:28:42.000000 calc_note-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:16:39.014924 calc_note-0.2.1/calc_note/
+-rw-rw-rw-   0        0        0        0 2020-07-06 12:06:21.000000 calc_note-0.2.1/calc_note/__init__.py
+-rw-rw-rw-   0        0        0       64 2024-05-14 15:14:03.000000 calc_note-0.2.1/calc_note/__version__.py
+-rw-rw-rw-   0        0        0     1003 2024-05-14 15:09:39.000000 calc_note-0.2.1/calc_note/display.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:16:39.033916 calc_note-0.2.1/calc_note.egg-info/
+-rw-rw-rw-   0        0        0     2253 2024-05-14 15:16:38.000000 calc_note-0.2.1/calc_note.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-14 15:16:38.000000 calc_note-0.2.1/calc_note.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:16:38.000000 calc_note-0.2.1/calc_note.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-14 15:16:38.000000 calc_note-0.2.1/calc_note.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 15:16:39.038929 calc_note-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     3967 2024-05-14 15:13:59.000000 calc_note-0.2.1/setup.py
```

### Comparing `calc_note-0.1.1/PKG-INFO` & `calc_note-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc_note
-Version: 0.1.1
+Version: 0.2.1
 Summary: Collection of utilities to ease the production of professional calculation notes using Python and Jupyter.
 Home-page: https://github.com/miek770/calc_note
 Author: Michel Lavoie
 Author-email: lavoie.michel@gmail.com
 License: MIT
 Description: 
         # Calculation Note
@@ -29,15 +29,15 @@
         
         ## Contributing
         
         If you wish to contribute, please submit [issues](https://github.com/miek770/calc_note/issues) and [pull requests](https://github.com/miek770/calc_note/pulls) through [this repo](https://gitlab.com/miek770/energy_tools#contributing).
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.5
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `calc_note-0.1.1/README.md` & `calc_note-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `calc_note-0.1.1/calc_note/display.py` & `calc_note-0.2.1/calc_note/display.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import pandas as pd
 from IPython.display import display
 from IPython.display import Markdown as md
 
+import warnings
+warnings.filterwarnings('ignore')
+warnings.simplefilter('ignore')
 
 # Pretty DataFrame output in Markdown (makes it possible for LaTeX to convert it to a
 # pretty table afterwards)
 # ===================================================================================
 
 
 def show(df):
```

### Comparing `calc_note-0.1.1/calc_note.egg-info/PKG-INFO` & `calc_note-0.2.1/calc_note.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc-note
-Version: 0.1.1
+Version: 0.2.1
 Summary: Collection of utilities to ease the production of professional calculation notes using Python and Jupyter.
 Home-page: https://github.com/miek770/calc_note
 Author: Michel Lavoie
 Author-email: lavoie.michel@gmail.com
 License: MIT
 Description: 
         # Calculation Note
@@ -29,15 +29,15 @@
         
         ## Contributing
         
         If you wish to contribute, please submit [issues](https://github.com/miek770/calc_note/issues) and [pull requests](https://github.com/miek770/calc_note/pulls) through [this repo](https://gitlab.com/miek770/energy_tools#contributing).
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.5
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `calc_note-0.1.1/setup.py` & `calc_note-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 # Package meta-data.
 NAME = 'calc_note'
 DESCRIPTION = 'Collection of utilities to ease the production of professional calculation notes using Python and Jupyter.'
 URL = 'https://github.com/miek770/calc_note'
 EMAIL = 'lavoie.michel@gmail.com'
 AUTHOR = 'Michel Lavoie'
-REQUIRES_PYTHON = '>=3.6.5'
-VERSION = '0.1.1'
+REQUIRES_PYTHON = '>=3.8.0'
+VERSION = '0.2.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
@@ -115,18 +115,18 @@
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

