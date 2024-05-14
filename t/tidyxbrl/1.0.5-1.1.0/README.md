# Comparing `tmp/tidyxbrl-1.0.5.tar.gz` & `tmp/tidyxbrl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyxbrl-1.0.5.tar", last modified: Tue May 14 05:32:20 2024, max compression
+gzip compressed data, was "tidyxbrl-1.1.0.tar", last modified: Tue May 14 05:41:13 2024, max compression
```

## Comparing `tidyxbrl-1.0.5.tar` & `tidyxbrl-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.5/LICENSE
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.0.5/MANIFEST.in
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5525 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4631 2024-05-14 05:29:56.000000 tidyxbrl-1.0.5/README.md
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      844 2024-05-14 05:32:09.000000 tidyxbrl-1.0.5/pyproject.toml
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       38 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/setup.cfg
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/src/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        0 2022-12-27 22:39:13.000000 tidyxbrl-1.0.5/src/__init__.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/src/tidyxbrl/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.5/src/tidyxbrl/__init__.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.5/src/tidyxbrl/edgar_cik.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.5/src/tidyxbrl/edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.5/src/tidyxbrl/edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.5/src/tidyxbrl/xbrl_apikey.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.0.5/src/tidyxbrl/xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.5/src/tidyxbrl/xbrl_query.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5525 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      497 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/SOURCES.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/dependency_links.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       18 2024-05-14 05:32:20.000000 tidyxbrl-1.0.5/src/tidyxbrl.egg-info/top_level.txt
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:32:20.760958 tidyxbrl-1.0.5/tests/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      161 2024-05-14 04:33:17.000000 tidyxbrl-1.0.5/tests/test_edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      795 2024-05-14 04:32:17.000000 tidyxbrl-1.0.5/tests/test_edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      687 2024-05-14 04:33:27.000000 tidyxbrl-1.0.5/tests/test_xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:35:33.000000 tidyxbrl-1.0.5/tests/test_xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.1.0/LICENSE
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.1.0/MANIFEST.in
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5699 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4804 2024-05-14 05:40:47.000000 tidyxbrl-1.1.0/README.md
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      844 2024-05-14 05:40:11.000000 tidyxbrl-1.1.0/pyproject.toml
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       38 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/setup.cfg
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/src/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        0 2022-12-27 22:39:13.000000 tidyxbrl-1.1.0/src/__init__.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/src/tidyxbrl/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.1.0/src/tidyxbrl/__init__.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.1.0/src/tidyxbrl/edgar_cik.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.1.0/src/tidyxbrl/edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.1.0/src/tidyxbrl/edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.1.0/src/tidyxbrl/xbrl_apikey.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.1.0/src/tidyxbrl/xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.1.0/src/tidyxbrl/xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5699 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      497 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       18 2024-05-14 05:41:13.000000 tidyxbrl-1.1.0/src/tidyxbrl.egg-info/top_level.txt
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:41:13.600810 tidyxbrl-1.1.0/tests/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      161 2024-05-14 04:33:17.000000 tidyxbrl-1.1.0/tests/test_edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      795 2024-05-14 04:32:17.000000 tidyxbrl-1.1.0/tests/test_edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      687 2024-05-14 04:33:27.000000 tidyxbrl-1.1.0/tests/test_xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:35:33.000000 tidyxbrl-1.1.0/tests/test_xbrl_query.py
```

### Comparing `tidyxbrl-1.0.5/LICENSE` & `tidyxbrl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/PKG-INFO` & `tidyxbrl-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.0.5
+Version: 1.1.0
 Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -82,16 +82,16 @@
                                   'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
                                   'report.document-type': "10-K"
                         })
 ```
 
 **edgar_query** - Query SEC data using the Central Index Key (CIK)
 ```
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+companycik = tidyxbrl.edgar_cik("ZILLOW GROUP, INC")
+desiredcorp = str(companycik[companycik.company.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
 tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
 tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
 tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
 ```
 
 **edgar_frames** - Aggregates one fact for each reporting entity
 ```
@@ -99,7 +99,8 @@
 ```
 
 ## Dependencies
 - [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
 - [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
 - [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
 - [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
+- [tqdm - Instantly make your loops show a smart progress meter - just wrap any iterable with tqdm(iterable), and you're done!](https://tqdm.github.io/)
```

### Comparing `tidyxbrl-1.0.5/README.md` & `tidyxbrl-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,16 +62,16 @@
                                   'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
                                   'report.document-type': "10-K"
                         })
 ```
 
 **edgar_query** - Query SEC data using the Central Index Key (CIK)
 ```
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+companycik = tidyxbrl.edgar_cik("ZILLOW GROUP, INC")
+desiredcorp = str(companycik[companycik.company.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
 tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
 tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
 tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
 ```
 
 **edgar_frames** - Aggregates one fact for each reporting entity
 ```
@@ -79,7 +79,8 @@
 ```
 
 ## Dependencies
 - [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
 - [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
 - [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
 - [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
+- [tqdm - Instantly make your loops show a smart progress meter - just wrap any iterable with tqdm(iterable), and you're done!](https://tqdm.github.io/)
```

### Comparing `tidyxbrl-1.0.5/pyproject.toml` & `tidyxbrl-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tidyxbrl"
-version = "1.0.5"
+version = "1.1.0"
 authors = [
   { name="Ryan McDonald", email="ryancmcdonald@gmail.com" },
 ]
 description = "A package to parse the XBRL file format & interface with XBRL APIs in a tidy format"
 readme = "README.md"
 requires-python = ">=3.9,<3.12"
 classifiers = [
```

### Comparing `tidyxbrl-1.0.5/src/tidyxbrl/edgar_cik.py` & `tidyxbrl-1.1.0/src/tidyxbrl/edgar_cik.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/src/tidyxbrl/edgar_frames.py` & `tidyxbrl-1.1.0/src/tidyxbrl/edgar_frames.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/src/tidyxbrl/edgar_query.py` & `tidyxbrl-1.1.0/src/tidyxbrl/edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/src/tidyxbrl/xbrl_apikey.py` & `tidyxbrl-1.1.0/src/tidyxbrl/xbrl_apikey.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/src/tidyxbrl/xbrl_parse.py` & `tidyxbrl-1.1.0/src/tidyxbrl/xbrl_parse.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/src/tidyxbrl/xbrl_query.py` & `tidyxbrl-1.1.0/src/tidyxbrl/xbrl_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/src/tidyxbrl.egg-info/PKG-INFO` & `tidyxbrl-1.1.0/src/tidyxbrl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.0.5
+Version: 1.1.0
 Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -82,16 +82,16 @@
                                   'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
                                   'report.document-type': "10-K"
                         })
 ```
 
 **edgar_query** - Query SEC data using the Central Index Key (CIK)
 ```
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+companycik = tidyxbrl.edgar_cik("ZILLOW GROUP, INC")
+desiredcorp = str(companycik[companycik.company.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
 tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
 tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
 tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
 ```
 
 **edgar_frames** - Aggregates one fact for each reporting entity
 ```
@@ -99,7 +99,8 @@
 ```
 
 ## Dependencies
 - [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
 - [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
 - [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
 - [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
+- [tqdm - Instantly make your loops show a smart progress meter - just wrap any iterable with tqdm(iterable), and you're done!](https://tqdm.github.io/)
```

### Comparing `tidyxbrl-1.0.5/tests/test_edgar_query.py` & `tidyxbrl-1.1.0/tests/test_edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/tests/test_xbrl_parse.py` & `tidyxbrl-1.1.0/tests/test_xbrl_parse.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.5/tests/test_xbrl_query.py` & `tidyxbrl-1.1.0/tests/test_xbrl_query.py`

 * *Files identical despite different names*

