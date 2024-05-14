# Comparing `tmp/ARS_Test_Runner-0.2.0.tar.gz` & `tmp/ARS_Test_Runner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARS_Test_Runner-0.2.0.tar", last modified: Mon May  6 16:25:42 2024, max compression
+gzip compressed data, was "ARS_Test_Runner-0.2.1.tar", last modified: Tue May 14 18:46:47 2024, max compression
```

## Comparing `ARS_Test_Runner-0.2.0.tar` & `ARS_Test_Runner-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.363081 ARS_Test_Runner-0.2.0/
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.355103 ARS_Test_Runner-0.2.0/ARS_Test_Runner/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/__init__.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/cli.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22749 2024-05-06 13:56:31.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/semantic_test.py
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.360930 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/affects_creative.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/treats.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/treats_creative.json
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.361897 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-05-06 16:25:42.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/SOURCES.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/dependency_links.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/entry_points.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/requires.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/top_level.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.2.0/LICENSE.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-05-06 16:25:42.362730 ARS_Test_Runner-0.2.0/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.2.0/README.md
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-05-06 16:25:42.364063 ARS_Test_Runner-0.2.0/setup.cfg
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-05-06 16:23:19.000000 ARS_Test_Runner-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:46:47.725303 ARS_Test_Runner-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:46:47.725303 ARS_Test_Runner-0.2.1/ARS_Test_Runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22749 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner/semantic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:46:47.725303 ARS_Test_Runner-0.2.1/ARS_Test_Runner/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner/templates/affects_creative.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner/templates/treats.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner/templates/treats_creative.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:46:47.725303 ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-14 18:46:47.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-14 18:46:47.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:46:47.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 18:46:47.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 18:46:47.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 18:46:47.000000 ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-14 18:46:47.725303 ARS_Test_Runner-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 18:46:47.729303 ARS_Test_Runner-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-14 18:46:30.000000 ARS_Test_Runner-0.2.1/setup.py
```

### Comparing `ARS_Test_Runner-0.2.0/ARS_Test_Runner/cli.py` & `ARS_Test_Runner-0.2.1/ARS_Test_Runner/cli.py`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.2.0/ARS_Test_Runner/semantic_test.py` & `ARS_Test_Runner-0.2.1/ARS_Test_Runner/semantic_test.py`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/affects_creative.json` & `ARS_Test_Runner-0.2.1/ARS_Test_Runner/templates/affects_creative.json`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/PKG-INFO` & `ARS_Test_Runner-0.2.1/ARS_Test_Runner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: ARS-Test-Runner
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: requests
-Requires-Dist: httpx
-Requires-Dist: reasoner-validator
-Requires-Dist: numpy
-Requires-Dist: attrs>=20.3.0
-Requires-Dist: click
-Requires-Dist: twine
 
 
 Translator ARS Pass/Fail Testing 
 ==========================================================
 
 This testing framework performs single level pass/Fail analysis on queries it receives from the Test Runner. 
 
@@ -65,7 +59,9 @@
 ```
 
 
 
 
 
 
+
+
```

### Comparing `ARS_Test_Runner-0.2.0/LICENSE.txt` & `ARS_Test_Runner-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.2.0/PKG-INFO` & `ARS_Test_Runner-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: ARS_Test_Runner
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: requests
-Requires-Dist: httpx
-Requires-Dist: reasoner-validator
-Requires-Dist: numpy
-Requires-Dist: attrs>=20.3.0
-Requires-Dist: click
-Requires-Dist: twine
 
 
 Translator ARS Pass/Fail Testing 
 ==========================================================
 
 This testing framework performs single level pass/Fail analysis on queries it receives from the Test Runner. 
 
@@ -65,7 +59,9 @@
 ```
 
 
 
 
 
 
+
+
```

### Comparing `ARS_Test_Runner-0.2.0/README.md` & `ARS_Test_Runner-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.2.0/setup.py` & `ARS_Test_Runner-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from semantic_release import setup_hook
     setup_hook(sys.argv)
 except ImportError:
     pass
 
-__version__='0.2.0'
+__version__='0.2.1'
 setup(
     name="ARS_Test_Runner",
     version= __version__,
     description="Python package for ARS pass/fail test",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Shervin Abdollahi, Mark Williams",
```

