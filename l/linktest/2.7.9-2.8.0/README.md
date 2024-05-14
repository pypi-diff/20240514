# Comparing `tmp/linktest-2.7.9.tar.gz` & `tmp/linktest-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.9.tar", last modified: Mon May 13 05:54:22 2024, max compression
+gzip compressed data, was "linktest-2.8.0.tar", last modified: Mon May 13 08:05:04 2024, max compression
```

## Comparing `linktest-2.7.9.tar` & `linktest-2.8.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 05:54:22.311805 linktest-2.7.9/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-13 05:54:22.311226 linktest-2.7.9/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 05:54:22.306775 linktest-2.7.9/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-12 15:05:15.000000 linktest-2.7.9/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-12 14:47:28.000000 linktest-2.7.9/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38132 2024-05-12 15:03:30.000000 linktest-2.7.9/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102112 2024-05-12 14:11:01.000000 linktest-2.7.9/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-12 15:05:20.000000 linktest-2.7.9/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 05:54:22.310367 linktest-2.7.9/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-13 05:54:22.311943 linktest-2.7.9/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-13 05:54:16.000000 linktest-2.7.9/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 08:05:04.975772 linktest-2.8.0/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-13 08:05:04.975491 linktest-2.8.0/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 08:05:04.973767 linktest-2.8.0/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-13 07:27:13.000000 linktest-2.8.0/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38245 2024-05-13 07:34:42.000000 linktest-2.8.0/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102237 2024-05-13 07:16:20.000000 linktest-2.8.0/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-13 07:27:22.000000 linktest-2.8.0/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-13 05:55:07.000000 linktest-2.8.0/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 08:05:04.975165 linktest-2.8.0/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-13 08:05:04.000000 linktest-2.8.0/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-13 08:05:04.000000 linktest-2.8.0/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-13 08:05:04.000000 linktest-2.8.0/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-13 08:05:04.000000 linktest-2.8.0/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-13 08:05:04.000000 linktest-2.8.0/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-13 08:05:04.975816 linktest-2.8.0/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-13 08:04:59.000000 linktest-2.8.0/setup.py
```

### Comparing `linktest-2.7.9/linktest/appium_utils.py` & `linktest-2.8.0/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/auto_generate_testcase_list.py` & `linktest-2.8.0/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.8.0/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/base_testcase.py` & `linktest-2.8.0/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/clean_data.py` & `linktest-2.8.0/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/conver_xml_into_db.py` & `linktest-2.8.0/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/database_helper.py` & `linktest-2.8.0/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/date_utilities.py` & `linktest-2.8.0/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/doctor.py` & `linktest-2.8.0/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/framework_log.py` & `linktest-2.8.0/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/generate_html_log.py` & `linktest-2.8.0/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/get_adb_devices.py` & `linktest-2.8.0/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/get_ios_devices_list.py` & `linktest-2.8.0/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/get_platform_info.py` & `linktest-2.8.0/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/get_project_info.py` & `linktest-2.8.0/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/html_report.py` & `linktest-2.8.0/linktest/html_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 
         testcase_filter_tag = testcase_filter_tag[0:testcase_filter_tag.rfind(".")]
         map_testcases_package(all_testcases_package, testcase_map_tag, testcase_filter_tag, testcase)
 
 
 class Reporter(object):
 
-    def __init__(self, output_folder, passed_cases, failed_cases, error_cases, start_time, platform_info, create_global_data_list_flag=False, auto_refresh=False):
+    def __init__(self, output_folder, passed_cases, failed_cases, error_cases, start_time, platform_info, create_global_data_list_flag=False, rerun_flag=False):
         try:
             self.generate_html_report(output_folder, passed_cases, failed_cases, error_cases, start_time,
-                                      platform_info, create_global_data_list_flag, auto_refresh)
+                                      platform_info, create_global_data_list_flag, rerun_flag)
         except BaseException:
             traceback.print_exc()
 
     def generate_html_report(self, output_folder, passed_cases, failed_cases, error_cases, start_time, platform_info,
-                             create_global_data_list_flag, auto_refresh):
+                             create_global_data_list_flag, rerun_flag):
         with open(output_folder + os.sep + "report.html", "w") as report_file_handler:
             end_time = datetime.datetime.now()
             execution_time = end_time - start_time
             execution_time = convert_to_seconds(execution_time)
 
             failed_cases_count = len(failed_cases)
             if failed_cases_count > 1:
@@ -170,14 +170,16 @@
                             num_failed_case = num_failed_case + 1;
                         }
                         if ("all_passed_case"==l[i].className){
                             num_passed_case = num_passed_case + 1;
                         }
                     }
 
+                    %s
+                    
                     if (document.getElementById("num_fail")){
                         var button = document.getElementById("failed_testcase_names");
                         if (num_failed_case > 1){
                             var new_str = num_failed_case + " Failed Test Cases";
                             document.getElementById("num_fail").innerHTML=new_str;
                             button.style.display = "";
                         } else {
@@ -200,15 +202,15 @@
                             var new_str = num_passed_case + " Passed Test Case";
                             document.getElementById("num_pass").innerHTML=new_str;
                         }
                     }
                 }
 
             </script>
-            """
+            """ % ("num_failed_case = Math.floor(num_failed_case / 2);" if rerun_flag else "")
 
             java_script_code_for_filter
 
             java_script_copy_failed_testcases = """
             <script>
                 function copyFailedTestCase(){
                     var button = document.getElementById("failed_testcase_names");
@@ -471,19 +473,19 @@
                                 """ % str_failed_testcase_names
 
                 failed_testcase_table = """
                 <table align='center'>
                 <tr><td>
                 <table class='table table-hover' border='0'>
                     <tr id='all_failed_test_cases' style='color:black; background-color: whitesmoke;'>
-                        <th width='100'>
+                        <th width='80'>
                                CaseID
                         </th>
                     
-                        <th width='860' style='color: #DC3912;'>
+                        <th width='880' style='color: #DC3912;'>
                                 <font id='num_fail'>%s &nbsp; Failed %s</font>
                                 <font style='margin-left: 18px;'>%s</font>
                         </th>
                         <th width='160'>
                             Duration(Seconds)
                         </th>
                         
@@ -519,20 +521,20 @@
                     module_name = failed_testcase.__module__.replace(".", "_") + os.sep + failed_testcase.__class__.__name__
                     module_name_display = failed_testcase.__module__.replace("tests.", "&#x0009;")
                     module_name_display += os.sep + failed_testcase.__class__.__name__
                     report_file_handler.write(
                         "<tr class='all_failed_case' name=%s>" % failed_testcase.testcase_filter_tag)
 
                     report_file_handler.write(
-                        "<td width='100' align='center' style='word-break:break-all;no-wrap:no-wrap'>")
+                        "<td width='80' align='center' style='word-break:break-all;no-wrap:no-wrap'>")
                     report_file_handler.write("%s" % ('-' if getattr(failed_testcase, "testcase_id", "None") == None else getattr(failed_testcase, "testcase_id")))
                     report_file_handler.write("</font></td>")
 
                     testcase_information = """
-                        <td width='860' style='word-break:break-all'>
+                        <td width='880' style='word-break:break-all'>
                         <a  href='%s'>
                             <font color='#333'>
                                 %s
                             </font>
                         </a>
                         """ % (
                         module_name,
@@ -583,19 +585,19 @@
             if len(passed_cases) > 0:
                 passed_testcase_table = """
                 <table align='center'>
                 <tr><td>
 
                 <table class='table table-hover' border='0'>
                     <tr id='all_passed_test_cases' style='color:balck; background-color: whitesmoke;'>
-                        <th width='100'>
+                        <th width='80'>
                             CaseID
                         </th>
                 
-                        <th width='860' style='color: #3366C5;'>
+                        <th width='880' style='color: #3366C5;'>
                             <font id='num_pass'>%s &nbsp;Passed %s</font>
                         </th>
                         
                         <th width='160'>
                             Duration(Seconds)
                         </th>
                         
@@ -612,19 +614,19 @@
                     module_name_display += os.sep + passed_testcase.__class__.__name__
 
                     report_file_handler.write(
                         "<tr class='all_passed_case' name=%s>" % getattr(passed_testcase,
                                                                                       "testcase_filter_tag",
                                                                                       "None"))
 
-                    report_file_handler.write("<td width='100' align='center' >")
+                    report_file_handler.write("<td width='80' align='center' >")
                     report_file_handler.write("%s" % ('-' if getattr(passed_testcase, "testcase_id", "None") == None else getattr(passed_testcase, "testcase_id")))
                     report_file_handler.write("</font></td>")
 
-                    report_file_handler.write("<td width='860' style='word-break:break-all'>")
+                    report_file_handler.write("<td width='880' style='word-break:break-all'>")
                     report_file_handler.write("<a title='Click to see the log & screenshot' href='")
                     report_file_handler.write(module_name)
                     report_file_handler.write(
                         "'><font color='%s'>" % (
                             "#333" if passed_testcase.rerun_tag == 0 else "green"))
                     report_file_handler.write(module_name_display)
```

### Comparing `linktest-2.7.9/linktest/logged_requests.py` & `linktest-2.8.0/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/main.py` & `linktest-2.8.0/linktest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1954,32 +1954,34 @@
             print("***" * 20 + " will start %s threads" % thread_pool_size)
         for i in range(thread_pool_size):
             testcase_executor_list.append(TestCaseExecutor(queue, total_testcases_count, output_folder, begin_time))
 
         BaseTestCase.GlobalTotalCaseCount = total_testcases_count
 
         for testcase_executor in testcase_executor_list:
-            time.sleep(0.5)
+            time.sleep(0.1)
             testcase_executor.start()
 
         for testcase_executor in testcase_executor_list:
             testcase_executor.join()
 
         final_failed_testcase_list = []
         if len(TestCaseExecutor.failed_testcases) > 0:
             for tc in TestCaseExecutor.failed_testcases:
                 final_failed_testcase_list.append(max(set(tc.packages.split(",")), key=len) + os.sep + tc.__class__.__name__)
                 
-            # remove duplicate testcases in failed_testcase_name_list
+            # remove duplicate testcases in failed_testcase_name_list （rerun_flag=True时，会有重复的testcase）
             final_failed_testcase_list = list(set(final_failed_testcase_list))
 
         print(os.linesep + "****************** TestCases Passed: %s, TestCases Failed: %s, Total TestCases Executed: %s ******************" % (
                 len(TestCaseExecutor.passed_testcases),len(final_failed_testcase_list), total_testcases_count))
-        print("Failed TestCase List:")
-        print(final_failed_testcase_list)
+
+        if len(final_failed_testcase_list) > 0:
+            print("Failed TestCase List:")
+            print(final_failed_testcase_list)
 
         if not settings.DEBUG_RUN:
             close_browsers_and_webdrivers()
         else:
             clean_appium_env()
 
 
@@ -2015,15 +2017,15 @@
             html_report.Reporter(output_folder,
                                  TestCaseExecutor.passed_testcases,
                                  TestCaseExecutor.failed_testcases,
                                  TestCaseExecutor.error_testcases,
                                  begin_time,
                                  PLATFORM_INFO,
                                  len(BaseTestCase.GlobalDataList) > 0,
-                                 True)
+                                 rerun_flag=rerun_flag)
         except BaseException:
             traceback.print_exc()
 
         print(
             "=*=*=" * 20 + os.linesep + "Execution has been completed. For further details, please refer to the accompanying HTML report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html" + os.linesep)
 
         # save the execution summary into DB (environment, total_execution_time,
```

### Comparing `linktest-2.7.9/linktest/memory_usage.py` & `linktest-2.8.0/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/re_func.py` & `linktest-2.8.0/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/run.py` & `linktest-2.8.0/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/run_testcase_thread.py` & `linktest-2.8.0/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/scp_report_to_specified_path.py` & `linktest-2.8.0/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/selenium_helper.py` & `linktest-2.8.0/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/timeout_thread.py` & `linktest-2.8.0/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/ui_testcase.py` & `linktest-2.8.0/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/update_config.py` & `linktest-2.8.0/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/webdriver_wrapper.py` & `linktest-2.8.0/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/webdriver_wrapper_chrome.py` & `linktest-2.8.0/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/webdriver_wrapper_edge.py` & `linktest-2.8.0/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/webdriver_wrapper_firefox.py` & `linktest-2.8.0/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/webdriver_wrapper_ie.py` & `linktest-2.8.0/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/webdriver_wrapper_safari.py` & `linktest-2.8.0/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest/xml_report.py` & `linktest-2.8.0/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.9/linktest.egg-info/SOURCES.txt` & `linktest-2.8.0/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

