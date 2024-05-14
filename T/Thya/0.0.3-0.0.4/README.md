# Comparing `tmp/Thya-0.0.3.tar.gz` & `tmp/thya-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Thya-0.0.3.tar", last modified: Thu Jul 13 14:34:57 2023, max compression
+gzip compressed data, was "thya-0.0.4.tar", last modified: Tue May 14 14:10:30 2024, max compression
```

## Comparing `Thya-0.0.3.tar` & `thya-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-13 14:34:40.000000 Thya-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 14:34:40.000000 Thya-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 14:34:57.875403 Thya-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 14:34:40.000000 Thya-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.871403 Thya-0.0.3/Thya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 14:34:57.875403 Thya-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-13 14:34:40.000000 Thya-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/thya/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/apis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/thya/convert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/boundingboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/imagelabels.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/polygons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/thya/data/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/data/example.json
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:10:30.364740 thya-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-14 14:10:17.000000 thya-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 14:10:17.000000 thya-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-14 14:10:30.364740 thya-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 14:10:17.000000 thya-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:10:30.364740 thya-0.0.4/Thya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-14 14:10:30.000000 thya-0.0.4/Thya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-14 14:10:30.000000 thya-0.0.4/Thya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:10:30.000000 thya-0.0.4/Thya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 14:10:30.000000 thya-0.0.4/Thya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 14:10:30.000000 thya-0.0.4/Thya.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 14:10:30.364740 thya-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-14 14:10:17.000000 thya-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:10:30.364740 thya-0.0.4/thya/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 14:10:17.000000 thya-0.0.4/thya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-14 14:10:17.000000 thya-0.0.4/thya/apis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:10:30.364740 thya-0.0.4/thya/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:10:17.000000 thya-0.0.4/thya/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-14 14:10:17.000000 thya-0.0.4/thya/convert/boundingboxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 14:10:17.000000 thya-0.0.4/thya/convert/imagelabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 14:10:17.000000 thya-0.0.4/thya/convert/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 14:10:17.000000 thya-0.0.4/thya/convert/polygons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:10:30.364740 thya-0.0.4/thya/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 14:10:17.000000 thya-0.0.4/thya/data/example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-14 14:10:17.000000 thya-0.0.4/thya/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-14 14:10:17.000000 thya-0.0.4/thya/summarize.py
```

### Comparing `Thya-0.0.3/LICENSE` & `thya-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Thya-0.0.3/PKG-INFO` & `thya-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thya
-Version: 0.0.3
+Version: 0.0.4
 Summary: ThyaTechnology SDK
 Home-page: https://github.com/ThyaTechnology/thya
 Author: Silvio Giancola
 Author-email: silvio@thya-technology.com
 License: GNU Affero General Public License v3.0
 Keywords: Thya,Technology,SDK,Cloud,Computer Vision,Object Detection,Instance Segmentation
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tqdm
+Requires-Dist: xmltodict
+Requires-Dist: imagesize
+Requires-Dist: xlsxwriter
 
 [![Python](https://img.shields.io/pypi/pyversions/thya)](https://img.shields.io/pypi/pyversions/thya)
 [![Pypi](https://img.shields.io/pypi/v/thya)](https://pypi.org/project/thya/)
 [![Downloads](https://static.pepy.tech/personalized-badge/thya?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/thya)
 [![Downloads](https://static.pepy.tech/personalized-badge/thya?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/thya)
 [![License](https://img.shields.io/badge/license-AGPLv3-green)](https://github.com/ThyaTechnology/thya/blob/master/LICENSE)
```

### Comparing `Thya-0.0.3/Thya.egg-info/PKG-INFO` & `thya-0.0.4/Thya.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thya
-Version: 0.0.3
+Version: 0.0.4
 Summary: ThyaTechnology SDK
 Home-page: https://github.com/ThyaTechnology/thya
 Author: Silvio Giancola
 Author-email: silvio@thya-technology.com
 License: GNU Affero General Public License v3.0
 Keywords: Thya,Technology,SDK,Cloud,Computer Vision,Object Detection,Instance Segmentation
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tqdm
+Requires-Dist: xmltodict
+Requires-Dist: imagesize
+Requires-Dist: xlsxwriter
 
 [![Python](https://img.shields.io/pypi/pyversions/thya)](https://img.shields.io/pypi/pyversions/thya)
 [![Pypi](https://img.shields.io/pypi/v/thya)](https://pypi.org/project/thya/)
 [![Downloads](https://static.pepy.tech/personalized-badge/thya?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/thya)
 [![Downloads](https://static.pepy.tech/personalized-badge/thya?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/thya)
 [![License](https://img.shields.io/badge/license-AGPLv3-green)](https://github.com/ThyaTechnology/thya/blob/master/LICENSE)
```

### Comparing `Thya-0.0.3/setup.py` & `thya-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `Thya-0.0.3/thya/apis.py` & `thya-0.0.4/thya/apis.py`

 * *Files identical despite different names*

### Comparing `Thya-0.0.3/thya/convert/boundingboxes.py` & `thya-0.0.4/thya/convert/boundingboxes.py`

 * *Files identical despite different names*

### Comparing `Thya-0.0.3/thya/convert/imagelabels.py` & `thya-0.0.4/thya/convert/imagelabels.py`

 * *Files identical despite different names*

### Comparing `Thya-0.0.3/thya/convert/keypoints.py` & `thya-0.0.4/thya/convert/keypoints.py`

 * *Files identical despite different names*

### Comparing `Thya-0.0.3/thya/convert/polygons.py` & `thya-0.0.4/thya/convert/polygons.py`

 * *Files identical despite different names*

### Comparing `Thya-0.0.3/thya/summarize.py` & `thya-0.0.4/thya/summarize.py`

 * *Files identical despite different names*

