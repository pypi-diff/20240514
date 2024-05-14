# Comparing `tmp/tidyxbrl-1.0.2.tar.gz` & `tmp/tidyxbrl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyxbrl-1.0.2.tar", last modified: Tue May 14 04:22:09 2024, max compression
+gzip compressed data, was "tidyxbrl-1.0.3.tar", last modified: Tue May 14 05:28:21 2024, max compression
```

## Comparing `tidyxbrl-1.0.2.tar` & `tidyxbrl-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.2/LICENSE
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.0.2/MANIFEST.in
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4225 2022-12-27 22:39:13.000000 tidyxbrl-1.0.2/README.md
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      548 2024-05-14 04:21:47.000000 tidyxbrl-1.0.2/pyproject.toml
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      769 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/setup.cfg
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/src/
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/src/tidyxbrl/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.2/src/tidyxbrl/__init__.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.2/src/tidyxbrl/edgar_cik.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.2/src/tidyxbrl/edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.2/src/tidyxbrl/edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.2/src/tidyxbrl/xbrl_apikey.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.0.2/src/tidyxbrl/xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.2/src/tidyxbrl/xbrl_query.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      491 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/SOURCES.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/dependency_links.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        9 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/top_level.txt
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/tests/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      119 2024-05-14 03:59:03.000000 tidyxbrl-1.0.2/tests/test_edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      681 2024-05-14 03:59:11.000000 tidyxbrl-1.0.2/tests/test_edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      503 2024-04-28 22:25:53.000000 tidyxbrl-1.0.2/tests/test_xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:14:20.000000 tidyxbrl-1.0.2/tests/test_xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.3/LICENSE
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.0.3/MANIFEST.in
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4225 2022-12-27 22:39:13.000000 tidyxbrl-1.0.3/README.md
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      844 2024-05-14 05:28:05.000000 tidyxbrl-1.0.3/pyproject.toml
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      769 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/setup.cfg
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/src/
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/src/tidyxbrl/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.3/src/tidyxbrl/__init__.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.3/src/tidyxbrl/edgar_cik.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.3/src/tidyxbrl/edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.3/src/tidyxbrl/edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.3/src/tidyxbrl/xbrl_apikey.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.0.3/src/tidyxbrl/xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.3/src/tidyxbrl/xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      491 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        9 2024-05-14 05:28:21.000000 tidyxbrl-1.0.3/src/tidyxbrl.egg-info/top_level.txt
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 05:28:21.721022 tidyxbrl-1.0.3/tests/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      161 2024-05-14 04:33:17.000000 tidyxbrl-1.0.3/tests/test_edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      795 2024-05-14 04:32:17.000000 tidyxbrl-1.0.3/tests/test_edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      687 2024-05-14 04:33:27.000000 tidyxbrl-1.0.3/tests/test_xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:35:33.000000 tidyxbrl-1.0.3/tests/test_xbrl_query.py
```

### Comparing `tidyxbrl-1.0.2/LICENSE` & `tidyxbrl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/PKG-INFO` & `tidyxbrl-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: tidyxbrl
-Version: 1.0.2
-Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
-Home-page: https://github.com/cowboycodeman/tidyxbrl/
-Author: Ryan McDonald
-Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
-Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
-Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
 </div>
 
 -----------------
 
 # tidyxbrl: The tidy XBRL Interface
```

### Comparing `tidyxbrl-1.0.2/README.md` & `tidyxbrl-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: tidyxbrl
+Version: 1.0.3
+Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
+Home-page: https://github.com/cowboycodeman/tidyxbrl/
+Author: Ryan McDonald
+Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
+Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
+Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Topic :: Office/Business :: Financial :: Accounting
+Classifier: Natural Language :: English
+Requires-Python: <3.12,>=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
   <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
 </div>
 
 -----------------
 
 # tidyxbrl: The tidy XBRL Interface
```

### Comparing `tidyxbrl-1.0.2/setup.cfg` & `tidyxbrl-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/src/tidyxbrl/edgar_cik.py` & `tidyxbrl-1.0.3/src/tidyxbrl/edgar_cik.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/src/tidyxbrl/edgar_frames.py` & `tidyxbrl-1.0.3/src/tidyxbrl/edgar_frames.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/src/tidyxbrl/edgar_query.py` & `tidyxbrl-1.0.3/src/tidyxbrl/edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/src/tidyxbrl/xbrl_apikey.py` & `tidyxbrl-1.0.3/src/tidyxbrl/xbrl_apikey.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/src/tidyxbrl/xbrl_parse.py` & `tidyxbrl-1.0.3/src/tidyxbrl/xbrl_parse.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/src/tidyxbrl/xbrl_query.py` & `tidyxbrl-1.0.3/src/tidyxbrl/xbrl_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.2/src/tidyxbrl.egg-info/PKG-INFO` & `tidyxbrl-1.0.3/src/tidyxbrl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
 Home-page: https://github.com/cowboycodeman/tidyxbrl/
 Author: Ryan McDonald
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Topic :: Office/Business :: Financial :: Accounting
+Classifier: Natural Language :: English
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
 </div>
```

### Comparing `tidyxbrl-1.0.2/tests/test_xbrl_query.py` & `tidyxbrl-1.0.3/tests/test_xbrl_query.py`

 * *Files identical despite different names*

