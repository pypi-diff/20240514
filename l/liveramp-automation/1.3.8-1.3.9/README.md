# Comparing `tmp/liveramp_automation-1.3.8.tar.gz` & `tmp/liveramp_automation-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.3.8.tar", last modified: Wed Apr 24 07:52:14 2024, max compression
+gzip compressed data, was "liveramp_automation-1.3.9.tar", last modified: Tue May 14 02:02:15 2024, max compression
```

## Comparing `liveramp_automation-1.3.8.tar` & `liveramp_automation-1.3.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.465773 liveramp_automation-1.3.8/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.8/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-04-24 07:52:14.465298 liveramp_automation-1.3.8/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.8/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.446187 liveramp_automation-1.3.8/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.8/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-24 07:51:56.000000 liveramp_automation-1.3.8/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.450471 liveramp_automation-1.3.8/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.8/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.8/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.3.8/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.8/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7369 2024-04-17 09:01:03.000000 liveramp_automation-1.3.8/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6184 2024-04-17 08:58:00.000000 liveramp_automation-1.3.8/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.3.8/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.455915 liveramp_automation-1.3.8/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.8/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.8/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.8/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     5025 2024-04-17 09:04:21.000000 liveramp_automation-1.3.8/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.8/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.8/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.8/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.8/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.8/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      795 2024-04-23 06:11:59.000000 liveramp_automation-1.3.8/liveramp_automation/utils/steps.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8423 2024-04-23 05:42:40.000000 liveramp_automation-1.3.8/liveramp_automation/utils/testrail.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.8/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.464699 liveramp_automation-1.3.8/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-04-24 07:52:14.000000 liveramp_automation-1.3.8/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1608 2024-04-24 07:52:14.000000 liveramp_automation-1.3.8/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-24 07:52:14.000000 liveramp_automation-1.3.8/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      474 2024-04-24 07:52:14.000000 liveramp_automation-1.3.8/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-24 07:52:14.000000 liveramp_automation-1.3.8/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-24 07:52:14.465824 liveramp_automation-1.3.8/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1516 2024-04-24 07:51:56.000000 liveramp_automation-1.3.8/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.456335 liveramp_automation-1.3.8/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.8/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.458955 liveramp_automation-1.3.8/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.8/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.8/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.8/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.8/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.8/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.8/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.8/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-24 07:52:14.464053 liveramp_automation-1.3.8/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.8/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.8/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.8/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3340 2024-04-23 05:46:11.000000 liveramp_automation-1.3.8/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.8/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.8/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.8/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.8/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     5406 2024-04-23 05:42:40.000000 liveramp_automation-1.3.8/tests/test_utils/test_testrail.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.8/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.771607 liveramp_automation-1.3.9/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.9/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-05-14 02:02:15.771136 liveramp_automation-1.3.9/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.9/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.751365 liveramp_automation-1.3.9/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.9/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-05-14 02:02:05.000000 liveramp_automation-1.3.9/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.755945 liveramp_automation-1.3.9/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.9/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10762 2024-05-14 01:35:40.000000 liveramp_automation-1.3.9/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.3.9/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.9/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7369 2024-04-17 09:01:03.000000 liveramp_automation-1.3.9/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6184 2024-04-17 08:58:00.000000 liveramp_automation-1.3.9/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.3.9/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.762051 liveramp_automation-1.3.9/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.9/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.9/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.9/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     5025 2024-04-17 09:04:21.000000 liveramp_automation-1.3.9/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.9/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.9/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.9/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.9/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.9/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      795 2024-04-23 06:11:59.000000 liveramp_automation-1.3.9/liveramp_automation/utils/steps.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8423 2024-04-23 05:42:40.000000 liveramp_automation-1.3.9/liveramp_automation/utils/testrail.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.9/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.770453 liveramp_automation-1.3.9/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-05-14 02:02:15.000000 liveramp_automation-1.3.9/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1608 2024-05-14 02:02:15.000000 liveramp_automation-1.3.9/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-05-14 02:02:15.000000 liveramp_automation-1.3.9/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      474 2024-05-14 02:02:15.000000 liveramp_automation-1.3.9/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-05-14 02:02:15.000000 liveramp_automation-1.3.9/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-05-14 02:02:15.771670 liveramp_automation-1.3.9/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1516 2024-04-24 07:51:56.000000 liveramp_automation-1.3.9/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.762470 liveramp_automation-1.3.9/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.9/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.765051 liveramp_automation-1.3.9/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.9/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4210 2024-05-14 02:00:56.000000 liveramp_automation-1.3.9/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2347 2024-05-10 03:04:44.000000 liveramp_automation-1.3.9/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.9/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.9/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.9/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.9/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 02:02:15.769855 liveramp_automation-1.3.9/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.9/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.9/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.9/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3324 2024-05-10 03:07:09.000000 liveramp_automation-1.3.9/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.9/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.9/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.9/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.9/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     5406 2024-05-10 03:16:07.000000 liveramp_automation-1.3.9/tests/test_utils/test_testrail.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.9/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.3.8/LICENSE` & `liveramp_automation-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/PKG-INFO` & `liveramp_automation-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.3.8
+Version: 1.3.9
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.3.8/README.md` & `liveramp_automation-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.3.9/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/helpers/file.py` & `liveramp_automation-1.3.9/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.3.9/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/helpers/login.py` & `liveramp_automation-1.3.9/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.3.9/liveramp_automation/helpers/notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/allure.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/log.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/request.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/slack.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/steps.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/steps.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/testrail.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/testrail.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation/utils/time.py` & `liveramp_automation-1.3.9/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.3.9/liveramp_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.3.8
+Version: 1.3.9
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.3.8/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.3.9/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/setup.py` & `liveramp_automation-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.3.9/tests/test_helpers/test_bucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,19 @@
     assert result
 
 
 def test_download_files():
     result = bucket_helper.download_files(destination_blob_name, download_folder_1)
     assert result
 
+
 def mocked_requests_response_throw_Exception(*args, **kwargs):
     raise Exception("Test")
 
+
 @patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_throw_Exception)
 def test_download_files_exception(mock):
     result = bucket_helper.download_files(destination_blob_name, download_folder_1)
     assert len(result) == 0
 
 
 def test_download_files_with_structure():
```

### Comparing `liveramp_automation-1.3.8/tests/test_helpers/test_file.py` & `liveramp_automation-1.3.9/tests/test_helpers/test_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.3.9/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_helpers/test_login.py` & `liveramp_automation-1.3.9/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_helpers/test_notification.py` & `liveramp_automation-1.3.9/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_log.py` & `liveramp_automation-1.3.9/tests/test_utils/test_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.3.9/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_parsers.py` & `liveramp_automation-1.3.9/tests/test_utils/test_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 @pytest.fixture(autouse=True)
 def setup_parser_simple():
     return ParseUtils("I want to test {str} cases")
 
 
-def mocked_requests_response_throw_exception(*args, **kwargs):
+def mocked_unit_test_throw_exception(*args, **kwargs):
     raise ValueError("Test")
 
 
 def test_is_matching_simple(setup_parser_simple):
     assert setup_parser_simple.is_matching('I want to test all cases')
     assert setup_parser_simple.is_matching('I want to test "all" cases')
     assert setup_parser_simple.is_matching('I want to test {all} cases')
@@ -41,15 +41,15 @@
 
 def test_is_matching_with_curly_brace(setup_parser_with_curly_brace):
     assert setup_parser_with_curly_brace.is_matching('I search {username} from the box')
     assert setup_parser_with_curly_brace.is_matching('I search {username} and password from the box')
     assert setup_parser_with_curly_brace.is_matching('I search {5} from the box')
 
 
-@patch('builtins.bool', side_effect=mocked_requests_response_throw_Exception)
+@patch('builtins.bool', side_effect=mocked_unit_test_throw_exception)
 def test_is_matching_with_curly_brace_exception(mock, setup_parser_with_curly_brace):
     assert setup_parser_with_curly_brace.is_matching('I search {username} from the box') is False
     assert setup_parser_with_curly_brace.is_matching('I search {username} and password from the box') is False
     assert setup_parser_with_curly_brace.is_matching('I search {5} from the box') is False
 
 
 @pytest.fixture(autouse=True)
```

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_playwright.py` & `liveramp_automation-1.3.9/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_request.py` & `liveramp_automation-1.3.9/tests/test_utils/test_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_selenium.py` & `liveramp_automation-1.3.9/tests/test_utils/test_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_slack.py` & `liveramp_automation-1.3.9/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_testrail.py` & `liveramp_automation-1.3.9/tests/test_utils/test_testrail.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 testrail_utils.read_suite_config_file()
 
 
 def mocked_requests_response(*args, **kwargs):
     response = Mock()
     response.status_code = 200
     response.id = 2
-    response.json = Mock(return_value={'id' : 3, 'cases' : [{'case_id' : 29438, 'type_id':7, 'id': 29438}]})
+    response.json = Mock(return_value={'id': 3, 'cases': [{'case_id': 29438, 'type_id': 7, 'id': 29438}]})
     return response
 
 
 def mocked_requests_response_no_json(*args, **kwargs):
     response = Mock()
     response.status_code = 400
     response.id = 2
@@ -55,14 +55,15 @@
 def test_add_run_only_suite_data(mock1, mock2, mock3):
     testrail_utils.add_run("only_suite_data")
     assert mock1.call_count == 1
     assert mock2.call_count == 0
     assert testrail_utils.filtered_case_ids == []
     assert testrail_utils.include_all is True
 
+
 @patch('allure.attach')
 @patch('requests.get', side_effect=mocked_requests_response)
 @patch('requests.post', side_effect=mocked_requests_response)
 def test_add_run_no_data(mock1, mock2, mock3):
     with pytest.raises(APIError):
         testrail_utils.add_run("no_data")
         assert mock1.call_count == 1
@@ -85,15 +86,15 @@
     with patch('builtins.open', mock_open(read_data="[testrail]")):
         testrail_utils.read_configuration()
         assert testrail_utils.url == 'https://liveramp.testrail.io/index.php?/api/v2/'
         assert testrail_utils.run_url == 'https://liveramp.testrail.io/index.php?/runs/view/'
         assert testrail_utils.report_file == './reports/report.json'
 
 
-def test_read_file_FileNotFoundError():
+def test_read_file_file_not_found_error():
     with patch('builtins.open', mock_open()) as mock_file:
         mock_file.side_effect = FileNotFoundError()
         testrail_utils.read_configuration()
         assert testrail_utils.url == 'https://liveramp.testrail.io/index.php?/api/v2/'
         assert testrail_utils.run_url == 'https://liveramp.testrail.io/index.php?/runs/view/'
         assert testrail_utils.report_file == './reports/report.json'
 
@@ -112,35 +113,33 @@
 @patch('allure.attach')
 @patch('requests.get', side_effect=mocked_requests_response)
 @patch('requests.post', side_effect=mocked_requests_response)
 def test_upload_results(mock1, mock2, mock3):
     testrail_utils.filtered_case_ids = []
     testrail_utils.upload_results("smoke")
     assert testrail_utils.filtered_case_ids == [29438]
-    assert testrail_utils.include_all == False
+    assert testrail_utils.include_all is False
     assert mock1.call_count == 2
     assert mock2.call_count == 1
 
 
 @patch('allure.attach')
 @patch('requests.get', side_effect=mocked_requests_response)
 @patch('requests.post', side_effect=mocked_requests_response)
 def test_upload_results_only_suite_data(mock1, mock2, mock3):
     testrail_utils.filtered_case_ids = []
     testrail_utils.upload_results("only_suite_data")
     assert testrail_utils.filtered_case_ids == []
-    assert testrail_utils.include_all == True
+    assert testrail_utils.include_all is True
     assert mock1.call_count == 2
     assert mock2.call_count == 0
 
+
 @patch('allure.attach')
 @patch('requests.get', side_effect=mocked_requests_response_no_json)
 @patch('requests.post', side_effect=mocked_requests_response)
 def test_upload_results_error(mock1, mock2, mock3):
     testrail_utils.filtered_case_ids = [29438]
     testrail_utils.upload_results("smoke")
     assert testrail_utils.filtered_case_ids == []
     assert mock1.call_count == 0
     assert mock2.call_count == 1
-
-
-
```

### Comparing `liveramp_automation-1.3.8/tests/test_utils/test_version.py` & `liveramp_automation-1.3.9/tests/test_utils/test_version.py`

 * *Files identical despite different names*

