# Comparing `tmp/abstract_utilities-0.2.2.8.tar.gz` & `tmp/abstract_utilities-0.2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_utilities-0.2.2.8.tar", last modified: Fri Oct 27 19:39:27 2023, max compression
+gzip compressed data, was "abstract_utilities-0.2.2.9.tar", last modified: Fri Oct 27 19:40:05 2023, max compression
```

## Comparing `abstract_utilities-0.2.2.8.tar` & `abstract_utilities-0.2.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-10-27 19:39:27.483749 abstract_utilities-0.2.2.8/
--rw-rw-rw-   0        0        0     4819 2023-10-27 19:39:27.483749 abstract_utilities-0.2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3953 2023-08-25 15:23:14.000000 abstract_utilities-0.2.2.8/README.md
--rw-rw-rw-   0        0        0       85 2023-08-25 15:23:14.000000 abstract_utilities-0.2.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-27 19:39:27.484799 abstract_utilities-0.2.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1156 2023-10-27 19:39:18.000000 abstract_utilities-0.2.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-27 19:39:27.445743 abstract_utilities-0.2.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-10-27 19:39:27.462752 abstract_utilities-0.2.2.8/src/abstract_utilities/
--rw-rw-rw-   0        0        0     1318 2023-10-27 19:27:03.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/__init__.py
--rw-rw-rw-   0        0        0    11454 2023-09-09 01:29:56.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/class_utils.py
--rw-rw-rw-   0        0        0     8536 2023-09-02 12:40:12.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/cmd_utils.py
--rw-rw-rw-   0        0        0     2348 2023-08-27 13:11:00.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/collator_utils.py
--rw-rw-rw-   0        0        0    15744 2023-10-18 01:01:41.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/compare_utils.py
--rw-rw-rw-   0        0        0     2204 2023-05-31 13:54:32.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/global_utils.py
--rw-rw-rw-   0        0        0     1633 2023-10-26 02:40:30.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/history_utils.py
--rw-rw-rw-   0        0        0    10686 2023-10-27 19:26:50.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/json_utils.py
--rw-rw-rw-   0        0        0     4925 2023-10-26 02:54:40.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/list_utils.py
--rw-rw-rw-   0        0        0     1294 2023-05-29 20:40:08.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/main.py
--rw-rw-rw-   0        0        0     2450 2023-10-13 13:24:55.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/math_utils.py
--rw-rw-rw-   0        0        0    11550 2023-10-13 04:49:14.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/path_utils.py
--rw-rw-rw-   0        0        0     9133 2023-10-13 12:20:10.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/read_write_utils.py
--rw-rw-rw-   0        0        0     4582 2023-08-27 12:51:36.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/string_clean.py
--rw-rw-rw-   0        0        0     6410 2023-10-27 06:49:25.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/thread_utils.py
--rw-rw-rw-   0        0        0     6754 2023-10-13 05:00:52.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/time_utils.py
--rw-rw-rw-   0        0        0    17929 2023-10-13 13:26:52.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/type_utils.py
--rw-rw-rw-   0        0        0   185049 2023-10-08 23:55:29.000000 abstract_utilities-0.2.2.8/src/abstract_utilities/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-27 19:39:27.482758 abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/
--rw-rw-rw-   0        0        0     4819 2023-10-27 19:39:27.000000 abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-10-27 19:39:27.000000 abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-27 19:39:27.000000 abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-10-27 19:39:27.000000 abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-10-27 19:39:27.000000 abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-27 19:40:05.004232 abstract_utilities-0.2.2.9/
+-rw-rw-rw-   0        0        0     4819 2023-10-27 19:40:05.004232 abstract_utilities-0.2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3953 2023-08-25 15:23:14.000000 abstract_utilities-0.2.2.9/README.md
+-rw-rw-rw-   0        0        0       85 2023-08-25 15:23:14.000000 abstract_utilities-0.2.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-10-27 19:40:05.006233 abstract_utilities-0.2.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2023-10-27 19:40:01.000000 abstract_utilities-0.2.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-27 19:40:04.956655 abstract_utilities-0.2.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-10-27 19:40:04.973653 abstract_utilities-0.2.2.9/src/abstract_utilities/
+-rw-rw-rw-   0        0        0     1318 2023-10-27 19:27:03.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/__init__.py
+-rw-rw-rw-   0        0        0    11454 2023-09-09 01:29:56.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/class_utils.py
+-rw-rw-rw-   0        0        0     8536 2023-09-02 12:40:12.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/cmd_utils.py
+-rw-rw-rw-   0        0        0     2348 2023-08-27 13:11:00.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/collator_utils.py
+-rw-rw-rw-   0        0        0    15744 2023-10-18 01:01:41.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/compare_utils.py
+-rw-rw-rw-   0        0        0     2204 2023-05-31 13:54:32.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/global_utils.py
+-rw-rw-rw-   0        0        0     1633 2023-10-26 02:40:30.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/history_utils.py
+-rw-rw-rw-   0        0        0    10686 2023-10-27 19:26:50.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/json_utils.py
+-rw-rw-rw-   0        0        0     4925 2023-10-26 02:54:40.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/list_utils.py
+-rw-rw-rw-   0        0        0     1294 2023-05-29 20:40:08.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/main.py
+-rw-rw-rw-   0        0        0     2450 2023-10-13 13:24:55.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/math_utils.py
+-rw-rw-rw-   0        0        0    11550 2023-10-13 04:49:14.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/path_utils.py
+-rw-rw-rw-   0        0        0     9133 2023-10-13 12:20:10.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/read_write_utils.py
+-rw-rw-rw-   0        0        0     4582 2023-08-27 12:51:36.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/string_clean.py
+-rw-rw-rw-   0        0        0     6410 2023-10-27 06:49:25.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/thread_utils.py
+-rw-rw-rw-   0        0        0     6754 2023-10-13 05:00:52.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/time_utils.py
+-rw-rw-rw-   0        0        0    17929 2023-10-13 13:26:52.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/type_utils.py
+-rw-rw-rw-   0        0        0   185049 2023-10-08 23:55:29.000000 abstract_utilities-0.2.2.9/src/abstract_utilities/utils.py
+drwxrwxrwx   0        0        0        0 2023-10-27 19:40:05.004232 abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/
+-rw-rw-rw-   0        0        0     4819 2023-10-27 19:40:04.000000 abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-10-27 19:40:04.000000 abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-27 19:40:04.000000 abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-10-27 19:40:04.000000 abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-10-27 19:40:04.000000 abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/top_level.txt
```

### Comparing `abstract_utilities-0.2.2.8/PKG-INFO` & `abstract_utilities-0.2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_utilities
-Version: 0.2.2.8
+Version: 0.2.2.9
 Summary: abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_utilities
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_utilities-0.2.2.8/README.md` & `abstract_utilities-0.2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/setup.py` & `abstract_utilities-0.2.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_utilities',
-    version='0.2.2.8',
+    version='0.2.2.9',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_utilities',
     classifiers=[
```

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/__init__.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/class_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/class_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/cmd_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/collator_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/collator_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/compare_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/compare_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/global_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/global_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/history_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/history_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/json_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/json_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/list_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/list_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/main.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/main.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/math_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/math_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/path_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/path_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/read_write_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/read_write_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/string_clean.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/string_clean.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/thread_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/thread_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/time_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/time_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/type_utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/type_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities/utils.py` & `abstract_utilities-0.2.2.9/src/abstract_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/PKG-INFO` & `abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-utilities
-Version: 0.2.2.8
+Version: 0.2.2.9
 Summary: abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_utilities
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_utilities-0.2.2.8/src/abstract_utilities.egg-info/SOURCES.txt` & `abstract_utilities-0.2.2.9/src/abstract_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

