# Comparing `tmp/pinscrape-3.0.3.tar.gz` & `tmp/pinscrape-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinscrape-3.0.3.tar", last modified: Mon Jun 19 15:47:46 2023, max compression
+gzip compressed data, was "pinscrape-3.0.5.tar", last modified: Tue May 14 10:02:45 2024, max compression
```

## Comparing `pinscrape-3.0.3.tar` & `pinscrape-3.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-19 15:47:27.000000 pinscrape-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-19 15:47:46.580795 pinscrape-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-19 15:47:27.000000 pinscrape-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/pinscrape/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-19 15:47:27.000000 pinscrape-3.0.3/pinscrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 15:47:27.000000 pinscrape-3.0.3/pinscrape/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-19 15:47:27.000000 pinscrape-3.0.3/pinscrape/pinscrape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/pinscrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 15:47:46.000000 pinscrape-3.0.3/pinscrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:47:46.580795 pinscrape-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 15:47:27.000000 pinscrape-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:46.580795 pinscrape-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:47:27.000000 pinscrape-3.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-19 15:47:27.000000 pinscrape-3.0.3/tests/e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 10:02:30.000000 pinscrape-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-14 10:02:45.396049 pinscrape-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-14 10:02:30.000000 pinscrape-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/pinscrape/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 10:02:30.000000 pinscrape-3.0.5/pinscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 10:02:30.000000 pinscrape-3.0.5/pinscrape/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-14 10:02:30.000000 pinscrape-3.0.5/pinscrape/pinscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/pinscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:02:45.396049 pinscrape-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 10:02:30.000000 pinscrape-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:30.000000 pinscrape-3.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 10:02:30.000000 pinscrape-3.0.5/tests/e2e.py
```

### Comparing `pinscrape-3.0.3/LICENSE` & `pinscrape-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pinscrape-3.0.3/PKG-INFO` & `pinscrape-3.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.0.3
+Version: 3.0.5
 Summary: Pinterest data scraper
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests==2.28.1
+Requires-Dist: beautifulsoup4==4.11.1
+Requires-Dist: tqdm==4.66.3
+Requires-Dist: pydotmap
+Requires-Dist: opencv-python
+Requires-Dist: pytest==7.2.0
 
 # pinscrape
 [![built with Python3](https://img.shields.io/badge/built%20with-Python3.6+-red.svg)](https://www.python.org/)
 
 ### This package can be use to scrape images from pinterest just by using any search keywords. Install it just by using <br><br>
 `pip install pinscrape`
 ### How to use?
```

### Comparing `pinscrape-3.0.3/README.md` & `pinscrape-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pinscrape-3.0.3/pinscrape/pinscrape.py` & `pinscrape-3.0.5/pinscrape/pinscrape.py`

 * *Files identical despite different names*

### Comparing `pinscrape-3.0.3/pinscrape.egg-info/PKG-INFO` & `pinscrape-3.0.5/pinscrape.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.0.3
+Version: 3.0.5
 Summary: Pinterest data scraper
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests==2.28.1
+Requires-Dist: beautifulsoup4==4.11.1
+Requires-Dist: tqdm==4.66.3
+Requires-Dist: pydotmap
+Requires-Dist: opencv-python
+Requires-Dist: pytest==7.2.0
 
 # pinscrape
 [![built with Python3](https://img.shields.io/badge/built%20with-Python3.6+-red.svg)](https://www.python.org/)
 
 ### This package can be use to scrape images from pinterest just by using any search keywords. Install it just by using <br><br>
 `pip install pinscrape`
 ### How to use?
```

### Comparing `pinscrape-3.0.3/setup.py` & `pinscrape-3.0.5/setup.py`

 * *Files identical despite different names*

