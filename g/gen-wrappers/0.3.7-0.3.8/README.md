# Comparing `tmp/gen_wrappers-0.3.7.tar.gz` & `tmp/gen_wrappers-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.3.7.tar", last modified: Tue May 14 16:11:56 2024, max compression
+gzip compressed data, was "gen_wrappers-0.3.8.tar", last modified: Tue May 14 17:06:50 2024, max compression
```

## Comparing `gen_wrappers-0.3.7.tar` & `gen_wrappers-0.3.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.045489 gen_wrappers-0.3.7/
--rw-rw-rw-   0        0        0      847 2024-05-14 16:11:56.044481 gen_wrappers-0.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.009092 gen_wrappers-0.3.7/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.7/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.014658 gen_wrappers-0.3.7/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.7/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.3.7/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.7/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.018658 gen_wrappers-0.3.7/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.7/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.7/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.7/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.7/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.022743 gen_wrappers-0.3.7/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.7/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9489 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    10277 2024-05-14 14:43:03.000000 gen_wrappers-0.3.7/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.7/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.026751 gen_wrappers-0.3.7/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.7/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.7/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.7/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.029750 gen_wrappers-0.3.7/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.7/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.7/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.043459 gen_wrappers-0.3.7/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 16:11:56.045489 gen_wrappers-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:11:36.000000 gen_wrappers-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:50.004155 gen_wrappers-0.3.8/
+-rw-rw-rw-   0        0        0      847 2024-05-14 17:06:50.003163 gen_wrappers-0.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:49.960415 gen_wrappers-0.3.8/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.8/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:49.965424 gen_wrappers-0.3.8/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.8/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.3.8/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.3.8/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.8/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:49.971423 gen_wrappers-0.3.8/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.8/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.3.8/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.8/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.8/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.8/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:49.976035 gen_wrappers-0.3.8/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.8/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9429 2024-05-14 16:43:13.000000 gen_wrappers-0.3.8/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    10342 2024-05-14 17:06:38.000000 gen_wrappers-0.3.8/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.8/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:49.980114 gen_wrappers-0.3.8/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.8/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.3.8/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.8/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.8/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:49.982121 gen_wrappers-0.3.8/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.8/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.8/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:06:50.000629 gen_wrappers-0.3.8/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-14 17:06:49.000000 gen_wrappers-0.3.8/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-14 17:06:49.000000 gen_wrappers-0.3.8/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:06:49.000000 gen_wrappers-0.3.8/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 17:06:49.000000 gen_wrappers-0.3.8/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 17:06:49.000000 gen_wrappers-0.3.8/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:06:50.005155 gen_wrappers-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-14 17:06:45.000000 gen_wrappers-0.3.8/setup.py
```

### Comparing `gen_wrappers-0.3.7/PKG-INFO` & `gen_wrappers-0.3.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.3.7
+Version: 0.3.8
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.7/creator/auto/creator_auto.py` & `gen_wrappers-0.3.8/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/auto/request_auto.py` & `gen_wrappers-0.3.8/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/auto/response_auto.py` & `gen_wrappers-0.3.8/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/base/base_app.py` & `gen_wrappers-0.3.8/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/base/base_request.py` & `gen_wrappers-0.3.8/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/base/base_response.py` & `gen_wrappers-0.3.8/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.3.8/creator/cmfy/creator_cmfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,18 +113,17 @@
         logger.debug(f"Getting status for job {job_id}")
         while job_data is None:
             history = requests.get(url)
             if history.status_code != 200:
                 return BaseResponse.error("Error getting job status", job_id)
             logger.info(f"History: {history.json()}")
             history = history.json()
-            for history_id, job in history.items():
-                if history_id == job_id:
-                    job_data = job
-                    break
+            job = history.get(job_id, None)
+            if job:
+                job_data = job
         images_output = []
         for node_id, node_output in job_data['outputs'].items():
             if 'images' in node_output:
                 logger.debug(f"Node output: {node_output}")
                 for image in node_output['images']:
                     logger.debug(f"Getting image: {image['filename']}")
                     print(f"Getting image: {image['filename']}")
```

### Comparing `gen_wrappers-0.3.7/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.3.8/creator/cmfy/request_cmfy.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,42 +138,33 @@
       ]
     },
     "class_type": "VAEDecode",
     "_meta": {
       "title": "VAE Decode"
     }
   },
-  "69": {
-    "inputs": {
-      "images": [
-        "67",
-        0
-      ]
-    },
-    "class_type": "PreviewImage",
-    "_meta": {
-      "title": "Output"
-    }
-  },
   "99": {
     "inputs": {
-      "seed": 178120892921818
+      "seed": 792005028278295
     },
     "class_type": "CR Seed",
     "_meta": {
       "title": "🌱 CR Seed"
     }
   },
   "100": {
     "inputs": {
       "text": [
         "114:0",
         0
       ],
-      "seed": 1892035549,
+      "seed": [
+        "99",
+        0
+      ],
       "log_prompt": "No"
     },
     "class_type": "PromptExpansion",
     "_meta": {
       "title": "Prompt Expansion"
     }
   },
@@ -332,14 +323,27 @@
       "text_c": ""
     },
     "class_type": "StringFunction|pysssss",
     "_meta": {
       "title": "Tidy Negative Tags"
     }
   },
+  "148": {
+    "inputs": {
+      "filename_prefix": "ComfyUI",
+      "images": [
+        "67",
+        0
+      ]
+    },
+    "class_type": "SaveImage",
+    "_meta": {
+      "title": "Save Image"
+    }
+  },
   "119:0": {
     "inputs": {
       "text_positive": "",
       "text_negative": "",
       "style": "Fooocus Photograph",
       "log_prompt": True,
       "style_positive": True,
```

### Comparing `gen_wrappers-0.3.7/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.3.8/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.3.8/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.3.8/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/creator/util/helper.py` & `gen_wrappers-0.3.8/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.3.8/gen_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.3.7
+Version: 0.3.8
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.7/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.3.8/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.7/setup.py` & `gen_wrappers-0.3.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.3.7',
+    version='0.3.8',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

