# Comparing `tmp/tidyxbrl-1.1.0.tar.gz` & `tmp/tidyxbrl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyxbrl-1.1.0.tar", last modified: Tue May 14 05:41:13 2024, max compression
+gzip compressed data, was "tidyxbrl-1.1.1.tar", last modified: Tue May 14 06:07:33 2024, max compression
```

## Comparing `tidyxbrl-1.1.0.tar` & `tidyxbrl-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.1.0/LICENSE
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.1.0/MANIFEST.in
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5699 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4804 2024-05-14 05:40:47.000000 tidyxbrl-1.1.0/README.md
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      844 2024-05-14 05:40:11.000000 tidyxbrl-1.1.0/pyproject.toml
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       38 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/setup.cfg
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/src/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        0 2022-12-27 22:39:13.000000 tidyxbrl-1.1.0/src/__init__.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/src/tidyxbrl/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.1.0/src/tidyxbrl/__init__.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.1.0/src/tidyxbrl/edgar_cik.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.1.0/src/tidyxbrl/edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.1.0/src/tidyxbrl/edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.1.0/src/tidyxbrl/xbrl_apikey.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.1.0/src/tidyxbrl/xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.1.0/src/tidyxbrl/xbrl_query.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5699 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      497 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/SOURCES.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/dependency_links.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       18 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/top_level.txt
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/tests/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      161 2024-05-14 04:33:17.000000 tidyxbrl-1.1.0/tests/test_edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      795 2024-05-14 04:32:17.000000 tidyxbrl-1.1.0/tests/test_edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      687 2024-05-14 04:33:27.000000 tidyxbrl-1.1.0/tests/test_xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:35:33.000000 tidyxbrl-1.1.0/tests/test_xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 06:07:33.030381 tidyxbrl-1.1.1/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.1.1/LICENSE
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.1.1/MANIFEST.in
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5892 2024-05-14 06:07:33.030381 tidyxbrl-1.1.1/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4889 2024-05-14 06:07:09.000000 tidyxbrl-1.1.1/README.md
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      952 2024-05-14 05:56:47.000000 tidyxbrl-1.1.1/pyproject.toml
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       38 2024-05-14 06:07:33.030381 tidyxbrl-1.1.1/setup.cfg
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 06:07:33.030381 tidyxbrl-1.1.1/src/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        0 2022-12-27 22:39:13.000000 tidyxbrl-1.1.1/src/__init__.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 06:07:33.030381 tidyxbrl-1.1.1/src/tidyxbrl/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.1.1/src/tidyxbrl/__init__.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.1.1/src/tidyxbrl/edgar_cik.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.1.1/src/tidyxbrl/edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.1.1/src/tidyxbrl/edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.1.1/src/tidyxbrl/xbrl_apikey.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.1.1/src/tidyxbrl/xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.1.1/src/tidyxbrl/xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 06:07:33.030381 tidyxbrl-1.1.1/src/tidyxbrl.egg-info/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5892 2024-05-14 06:07:33.000000 tidyxbrl-1.1.1/src/tidyxbrl.egg-info/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      497 2024-05-14 06:07:33.000000 tidyxbrl-1.1.1/src/tidyxbrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 06:07:33.000000 tidyxbrl-1.1.1/src/tidyxbrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       18 2024-05-14 06:07:33.000000 tidyxbrl-1.1.1/src/tidyxbrl.egg-info/top_level.txt
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 06:07:33.030381 tidyxbrl-1.1.1/tests/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      161 2024-05-14 04:33:17.000000 tidyxbrl-1.1.1/tests/test_edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      795 2024-05-14 04:32:17.000000 tidyxbrl-1.1.1/tests/test_edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      687 2024-05-14 04:33:27.000000 tidyxbrl-1.1.1/tests/test_xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:35:33.000000 tidyxbrl-1.1.1/tests/test_xbrl_query.py
```

### Comparing `tidyxbrl-1.1.0/LICENSE` & `tidyxbrl-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/PKG-INFO` & `tidyxbrl-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.1.0
-Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
+Version: 1.1.1
+Summary: A python package to parse the XBRL file format & interface with XBRL APIs in a tidy format. A powerful tool for automated financial analysis, accounting, and investment research using Pandas.
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 -----------------
 
 [![PyPI](https://img.shields.io/pypi/v/tidyxbrl)](https://pypi.org/project/tidyxbrl/#history)
 [![PyPI - Status](https://img.shields.io/pypi/status/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 
-# tidyxbrl: The tidy XBRL Interface
+# tidyxbrl: The tidy Python XBRL Interface
 
 ## What is it?
 
 **tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
 
 ## The XBRL Standard
 eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
@@ -94,13 +94,17 @@
 ```
 
 **edgar_frames** - Aggregates one fact for each reporting entity
 ```
 tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
 ```
 
+## Data Visualization
+
+![Real Estate Assets](figures/real_estate_assets.png)
+
 ## Dependencies
 - [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
 - [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
 - [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
 - [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
 - [tqdm - Instantly make your loops show a smart progress meter - just wrap any iterable with tqdm(iterable), and you're done!](https://tqdm.github.io/)
```

### Comparing `tidyxbrl-1.1.0/README.md` & `tidyxbrl-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 -----------------
 
 [![PyPI](https://img.shields.io/pypi/v/tidyxbrl)](https://pypi.org/project/tidyxbrl/#history)
 [![PyPI - Status](https://img.shields.io/pypi/status/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 
-# tidyxbrl: The tidy XBRL Interface
+# tidyxbrl: The tidy Python XBRL Interface
 
 ## What is it?
 
 **tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
 
 ## The XBRL Standard
 eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
@@ -74,13 +74,17 @@
 ```
 
 **edgar_frames** - Aggregates one fact for each reporting entity
 ```
 tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
 ```
 
+## Data Visualization
+
+![Real Estate Assets](figures/real_estate_assets.png)
+
 ## Dependencies
 - [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
 - [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
 - [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
 - [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
 - [tqdm - Instantly make your loops show a smart progress meter - just wrap any iterable with tqdm(iterable), and you're done!](https://tqdm.github.io/)
```

### Comparing `tidyxbrl-1.1.0/src/tidyxbrl/edgar_cik.py` & `tidyxbrl-1.1.1/src/tidyxbrl/edgar_cik.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/src/tidyxbrl/edgar_frames.py` & `tidyxbrl-1.1.1/src/tidyxbrl/edgar_frames.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/src/tidyxbrl/edgar_query.py` & `tidyxbrl-1.1.1/src/tidyxbrl/edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/src/tidyxbrl/xbrl_apikey.py` & `tidyxbrl-1.1.1/src/tidyxbrl/xbrl_apikey.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/src/tidyxbrl/xbrl_parse.py` & `tidyxbrl-1.1.1/src/tidyxbrl/xbrl_parse.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/src/tidyxbrl/xbrl_query.py` & `tidyxbrl-1.1.1/src/tidyxbrl/xbrl_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/src/tidyxbrl.egg-info/PKG-INFO` & `tidyxbrl-1.1.1/src/tidyxbrl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.1.0
-Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
+Version: 1.1.1
+Summary: A python package to parse the XBRL file format & interface with XBRL APIs in a tidy format. A powerful tool for automated financial analysis, accounting, and investment research using Pandas.
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 -----------------
 
 [![PyPI](https://img.shields.io/pypi/v/tidyxbrl)](https://pypi.org/project/tidyxbrl/#history)
 [![PyPI - Status](https://img.shields.io/pypi/status/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidyxbrl)](https://pypi.org/project/tidyxbrl/)
 
-# tidyxbrl: The tidy XBRL Interface
+# tidyxbrl: The tidy Python XBRL Interface
 
 ## What is it?
 
 **tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
 
 ## The XBRL Standard
 eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
@@ -94,13 +94,17 @@
 ```
 
 **edgar_frames** - Aggregates one fact for each reporting entity
 ```
 tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
 ```
 
+## Data Visualization
+
+![Real Estate Assets](figures/real_estate_assets.png)
+
 ## Dependencies
 - [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
 - [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
 - [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
 - [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
 - [tqdm - Instantly make your loops show a smart progress meter - just wrap any iterable with tqdm(iterable), and you're done!](https://tqdm.github.io/)
```

### Comparing `tidyxbrl-1.1.0/tests/test_edgar_query.py` & `tidyxbrl-1.1.1/tests/test_edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/tests/test_xbrl_parse.py` & `tidyxbrl-1.1.1/tests/test_xbrl_parse.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.1.0/tests/test_xbrl_query.py` & `tidyxbrl-1.1.1/tests/test_xbrl_query.py`

 * *Files identical despite different names*

