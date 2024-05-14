# Comparing `tmp/tidyxbrl-1.0.3.tar.gz` & `tmp/tidyxbrl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyxbrl-1.0.3.tar", last modified: Tue May 14 05:28:21 2024, max compression
+gzip compressed data, was "tidyxbrl-1.0.5.tar", last modified: Tue May 14 05:32:20 2024, max compression
```

## Comparing `tidyxbrl-1.0.3.tar` & `tidyxbrl-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.3/LICENSE
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.0.3/MANIFEST.in
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4225 2022-12-27 22:39:13.000000 tidyxbrl-1.0.3/README.md
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      844 2024-05-14 05:28:05.000000 tidyxbrl-1.0.3/pyproject.toml
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      769 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/setup.cfg
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/src/
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/src/tidyxbrl/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.3/src/tidyxbrl/__init__.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.3/src/tidyxbrl/edgar_cik.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.3/src/tidyxbrl/edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.3/src/tidyxbrl/edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.3/src/tidyxbrl/xbrl_apikey.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.0.3/src/tidyxbrl/xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.3/src/tidyxbrl/xbrl_query.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      491 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/SOURCES.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/dependency_links.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        9 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/top_level.txt
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/tests/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      161 2024-05-14 04:33:17.000000 tidyxbrl-1.0.3/tests/test_edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      795 2024-05-14 04:32:17.000000 tidyxbrl-1.0.3/tests/test_edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      687 2024-05-14 04:33:27.000000 tidyxbrl-1.0.3/tests/test_xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:35:33.000000 tidyxbrl-1.0.3/tests/test_xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.5/LICENSE
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.0.5/MANIFEST.in
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5525 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4631 2024-05-14 05:29:56.000000 tidyxbrl-1.0.5/README.md
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      844 2024-05-14 05:32:09.000000 tidyxbrl-1.0.5/pyproject.toml
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       38 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/setup.cfg
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/src/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        0 2022-12-27 22:39:13.000000 tidyxbrl-1.0.5/src/__init__.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/src/tidyxbrl/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.5/src/tidyxbrl/__init__.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.5/src/tidyxbrl/edgar_cik.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.5/src/tidyxbrl/edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.5/src/tidyxbrl/edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.5/src/tidyxbrl/xbrl_apikey.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.0.5/src/tidyxbrl/xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.5/src/tidyxbrl/xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5525 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      497 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       18 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/top_level.txt
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/tests/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      161 2024-05-14 04:33:17.000000 tidyxbrl-1.0.5/tests/test_edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      795 2024-05-14 04:32:17.000000 tidyxbrl-1.0.5/tests/test_edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      687 2024-05-14 04:33:27.000000 tidyxbrl-1.0.5/tests/test_xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:35:33.000000 tidyxbrl-1.0.5/tests/test_xbrl_query.py
```

### Comparing `tidyxbrl-1.0.3/LICENSE` & `tidyxbrl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/PKG-INFO` & `tidyxbrl-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.0.3
+Version: 1.0.5
 Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
-Home-page: https://github.com/cowboycodeman/tidyxbrl/
-Author: Ryan McDonald
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +20,19 @@
 
 <div align="center">
   <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
 </div>
 
 -----------------
 
+[![PyPI](https://img.shields.io/pypi/v/tidyxbrl)](https://pypi.org/project/tidyxbrl/#history)
+[![PyPI - Status](https://img.shields.io/pypi/status/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+
 # tidyxbrl: The tidy XBRL Interface
 
 ## What is it?
 
 **tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
 
 ## The XBRL Standard
```

### Comparing `tidyxbrl-1.0.3/README.md` & `tidyxbrl-1.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 <div align="center">
   <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
 </div>
 
 -----------------
 
+[![PyPI](https://img.shields.io/pypi/v/tidyxbrl)](https://pypi.org/project/tidyxbrl/#history)
+[![PyPI - Status](https://img.shields.io/pypi/status/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+
 # tidyxbrl: The tidy XBRL Interface
 
 ## What is it?
 
 **tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
 
 ## The XBRL Standard
```

### Comparing `tidyxbrl-1.0.3/pyproject.toml` & `tidyxbrl-1.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tidyxbrl"
-version = "1.0.3"
+version = "1.0.5"
 authors = [
   { name="Ryan McDonald", email="ryancmcdonald@gmail.com" },
 ]
 description = "A package to parse the XBRL file format & interface with XBRL APIs in a tidy format"
 readme = "README.md"
 requires-python = ">=3.9,<3.12"
 classifiers = [
```

### Comparing `tidyxbrl-1.0.3/src/tidyxbrl/edgar_cik.py` & `tidyxbrl-1.0.5/src/tidyxbrl/edgar_cik.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/src/tidyxbrl/edgar_frames.py` & `tidyxbrl-1.0.5/src/tidyxbrl/edgar_frames.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/src/tidyxbrl/edgar_query.py` & `tidyxbrl-1.0.5/src/tidyxbrl/edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/src/tidyxbrl/xbrl_apikey.py` & `tidyxbrl-1.0.5/src/tidyxbrl/xbrl_apikey.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/src/tidyxbrl/xbrl_parse.py` & `tidyxbrl-1.0.5/src/tidyxbrl/xbrl_parse.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/src/tidyxbrl/xbrl_query.py` & `tidyxbrl-1.0.5/src/tidyxbrl/xbrl_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/src/tidyxbrl.egg-info/PKG-INFO` & `tidyxbrl-1.0.5/src/tidyxbrl.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.0.3
+Version: 1.0.5
 Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
-Home-page: https://github.com/cowboycodeman/tidyxbrl/
-Author: Ryan McDonald
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +20,19 @@
 
 <div align="center">
   <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
 </div>
 
 -----------------
 
+[![PyPI](https://img.shields.io/pypi/v/tidyxbrl)](https://pypi.org/project/tidyxbrl/#history)
+[![PyPI - Status](https://img.shields.io/pypi/status/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
+
 # tidyxbrl: The tidy XBRL Interface
 
 ## What is it?
 
 **tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
 
 ## The XBRL Standard
```

### Comparing `tidyxbrl-1.0.3/tests/test_edgar_query.py` & `tidyxbrl-1.0.5/tests/test_edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/tests/test_xbrl_parse.py` & `tidyxbrl-1.0.5/tests/test_xbrl_parse.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.3/tests/test_xbrl_query.py` & `tidyxbrl-1.0.5/tests/test_xbrl_query.py`

 * *Files identical despite different names*

