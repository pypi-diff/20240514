# Comparing `tmp/gen_wrappers-0.3.2.tar.gz` & `tmp/gen_wrappers-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.3.2.tar", last modified: Mon May 13 20:05:36 2024, max compression
+gzip compressed data, was "gen_wrappers-0.3.3.tar", last modified: Tue May 14 12:45:46 2024, max compression
```

## Comparing `gen_wrappers-0.3.2.tar` & `gen_wrappers-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.890579 gen_wrappers-0.3.2/
--rw-rw-rw-   0        0        0      847 2024-05-13 20:05:36.888144 gen_wrappers-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.800836 gen_wrappers-0.3.2/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.2/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.819467 gen_wrappers-0.3.2/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.2/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.2/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.2/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.2/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.830990 gen_wrappers-0.3.2/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.2/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.2/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.2/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.2/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.2/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.838251 gen_wrappers-0.3.2/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.2/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.2/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.3.2/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.2/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.845921 gen_wrappers-0.3.2/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.2/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.2/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.2/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.2/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.852569 gen_wrappers-0.3.2/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.2/creator/util/__init__.py
--rw-rw-rw-   0        0        0     6060 2024-05-13 20:04:32.000000 gen_wrappers-0.3.2/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:36.885483 gen_wrappers-0.3.2/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-13 20:05:36.000000 gen_wrappers-0.3.2/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-13 20:05:36.000000 gen_wrappers-0.3.2/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:05:36.000000 gen_wrappers-0.3.2/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-13 20:05:36.000000 gen_wrappers-0.3.2/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 20:05:36.000000 gen_wrappers-0.3.2/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 20:05:36.890579 gen_wrappers-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-13 20:05:18.000000 gen_wrappers-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.680182 gen_wrappers-0.3.3/
+-rw-rw-rw-   0        0        0      847 2024-05-14 12:45:46.679182 gen_wrappers-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.533172 gen_wrappers-0.3.3/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.3/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.561246 gen_wrappers-0.3.3/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.3/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.3/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.3/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.3/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.593377 gen_wrappers-0.3.3/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.3/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.3/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.3/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.3/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.3/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.618538 gen_wrappers-0.3.3/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.3/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.3/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.3.3/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.3/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.646154 gen_wrappers-0.3.3/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.3/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.3/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.3/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.3/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.656666 gen_wrappers-0.3.3/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.3/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     6060 2024-05-13 20:04:32.000000 gen_wrappers-0.3.3/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.677201 gen_wrappers-0.3.3/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:45:46.680182 gen_wrappers-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-14 12:45:33.000000 gen_wrappers-0.3.3/setup.py
```

### Comparing `gen_wrappers-0.3.2/PKG-INFO` & `gen_wrappers-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.3.2
+Version: 0.3.3
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.2/creator/auto/creator_auto.py` & `gen_wrappers-0.3.3/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/auto/request_auto.py` & `gen_wrappers-0.3.3/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/auto/response_auto.py` & `gen_wrappers-0.3.3/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/base/base_app.py` & `gen_wrappers-0.3.3/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/base/base_request.py` & `gen_wrappers-0.3.3/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/base/base_response.py` & `gen_wrappers-0.3.3/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.3.3/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.3.3/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.3.3/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.3.3/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.3.3/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/creator/util/helper.py` & `gen_wrappers-0.3.3/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.3.3/gen_wrappers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.3.2
+Version: 0.3.3
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.2/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.3.3/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.2/setup.py` & `gen_wrappers-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.3.2',
+    version='0.3.3',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

