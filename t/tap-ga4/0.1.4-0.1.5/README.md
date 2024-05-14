# Comparing `tmp/tap-ga4-0.1.4.tar.gz` & `tmp/tap-ga4-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-ga4-0.1.4.tar", last modified: Tue Mar 26 14:04:23 2024, max compression
+gzip compressed data, was "tap-ga4-0.1.5.tar", last modified: Tue May 14 15:30:27 2024, max compression
```

## Comparing `tap-ga4-0.1.4.tar` & `tap-ga4-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,21 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-26 14:04:23.479527 tap-ga4-0.1.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-08-03 04:27:50.000000 tap-ga4-0.1.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-08-03 04:27:50.000000 tap-ga4-0.1.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2024-03-26 14:04:23.479527 tap-ga4-0.1.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-08-03 04:27:50.000000 tap-ga4-0.1.4/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-26 14:04:23.479527 tap-ga4-0.1.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2024-03-26 14:03:06.000000 tap-ga4-0.1.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-26 14:04:23.475527 tap-ga4-0.1.4/tap_ga4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1128 2024-02-22 11:30:54.000000 tap-ga4-0.1.4/tap_ga4/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5350 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tap_ga4/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11969 2024-03-26 14:03:06.000000 tap-ga4-0.1.4/tap_ga4/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   705258 2024-03-26 10:10:47.000000 tap-ga4-0.1.4/tap_ga4/field_exclusions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19003 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tap_ga4/reports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10706 2023-08-03 04:27:50.000000 tap-ga4-0.1.4/tap_ga4/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-26 14:04:23.479527 tap-ga4-0.1.4/tap_ga4.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2024-03-26 14:04:23.000000 tap-ga4-0.1.4/tap_ga4.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      639 2024-03-26 14:04:23.000000 tap-ga4-0.1.4/tap_ga4.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-26 14:04:23.000000 tap-ga4-0.1.4/tap_ga4.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-03-26 14:04:23.000000 tap-ga4-0.1.4/tap_ga4.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2024-03-26 14:04:23.000000 tap-ga4-0.1.4/tap_ga4.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-03-26 14:04:23.000000 tap-ga4-0.1.4/tap_ga4.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-26 14:04:23.479527 tap-ga4-0.1.4/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9546 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_all_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      450 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4558 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_bookmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      985 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5285 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_ga4_conversion_window.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3497 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_ga4_conversion_window_invalid.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3961 2024-02-22 18:29:43.000000 tap-ga4-0.1.4/tests/test_interrupted_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      782 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1009 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_start_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4445 2024-02-22 12:44:07.000000 tap-ga4-0.1.4/tests/test_sync_canary.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-14 15:30:27.332232 tap-ga4-0.1.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-08-14 12:11:34.000000 tap-ga4-0.1.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-08-14 12:11:34.000000 tap-ga4-0.1.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2024-05-14 15:30:27.332232 tap-ga4-0.1.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-08-14 12:11:34.000000 tap-ga4-0.1.5/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-14 15:30:27.332232 tap-ga4-0.1.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2024-05-14 15:30:00.000000 tap-ga4-0.1.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-14 15:30:27.332232 tap-ga4-0.1.5/tap_ga4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1128 2024-05-14 06:01:51.000000 tap-ga4-0.1.5/tap_ga4/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5350 2023-08-14 12:11:34.000000 tap-ga4-0.1.5/tap_ga4/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11969 2024-05-14 10:51:03.000000 tap-ga4-0.1.5/tap_ga4/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   705279 2024-05-14 15:30:00.000000 tap-ga4-0.1.5/tap_ga4/field_exclusions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19003 2023-08-14 12:11:34.000000 tap-ga4-0.1.5/tap_ga4/reports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10706 2023-08-14 12:11:34.000000 tap-ga4-0.1.5/tap_ga4/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-14 15:30:27.332232 tap-ga4-0.1.5/tap_ga4.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2024-05-14 15:30:27.000000 tap-ga4-0.1.5/tap_ga4.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      349 2024-05-14 15:30:27.000000 tap-ga4-0.1.5/tap_ga4.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-14 15:30:27.000000 tap-ga4-0.1.5/tap_ga4.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2024-05-14 15:30:27.000000 tap-ga4-0.1.5/tap_ga4.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2024-05-14 15:30:27.000000 tap-ga4-0.1.5/tap_ga4.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-05-14 15:30:27.000000 tap-ga4-0.1.5/tap_ga4.egg-info/top_level.txt
```

### Comparing `tap-ga4-0.1.4/LICENSE` & `tap-ga4-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-ga4-0.1.4/setup.py` & `tap-ga4-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-ga4",
-    version="0.1.4",
+    version="0.1.5",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_ga4"],
     install_requires=[
         "google-analytics-data==0.14.0",
```

### Comparing `tap-ga4-0.1.4/tap_ga4/__init__.py` & `tap-ga4-0.1.5/tap_ga4/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-ga4-0.1.4/tap_ga4/client.py` & `tap-ga4-0.1.5/tap_ga4/client.py`

 * *Files identical despite different names*

### Comparing `tap-ga4-0.1.4/tap_ga4/discover.py` & `tap-ga4-0.1.5/tap_ga4/discover.py`

 * *Files identical despite different names*

### Comparing `tap-ga4-0.1.4/tap_ga4/field_exclusions.json` & `tap-ga4-0.1.5/tap_ga4/field_exclusions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977973568281938%*

 * *Differences: {"'comparison'": '[]'}*

```diff
@@ -4369,14 +4369,15 @@
         "scrolledUsers",
         "shippingAmount",
         "taxAmount",
         "transactions",
         "transactionsPerPurchaser",
         "userEngagementDuration"
     ],
+    "comparison": [],
     "contentGroup": [
         "cohortNthDay",
         "cohortNthMonth",
         "cohortNthWeek",
         "advertiserAdClicks",
         "advertiserAdCost",
         "advertiserAdCostPerClick",
```

### Comparing `tap-ga4-0.1.4/tap_ga4/reports.py` & `tap-ga4-0.1.5/tap_ga4/reports.py`

 * *Files identical despite different names*

### Comparing `tap-ga4-0.1.4/tap_ga4/sync.py` & `tap-ga4-0.1.5/tap_ga4/sync.py`

 * *Files identical despite different names*

