# Comparing `tmp/composio_griptape-0.2.59.tar.gz` & `tmp/composio_griptape-0.2.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_griptape-0.2.59.tar", last modified: Mon May 13 09:47:53 2024, max compression
+gzip compressed data, was "composio_griptape-0.2.60.tar", last modified: Tue May 14 10:58:43 2024, max compression
```

## Comparing `composio_griptape-0.2.59.tar` & `composio_griptape-0.2.60.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:53.888395 composio_griptape-0.2.59/
--rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-13 09:47:53.888183 composio_griptape-0.2.59/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     1851 2024-05-13 07:27:09.000000 composio_griptape-0.2.59/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:53.886424 composio_griptape-0.2.59/composio_griptape/
--rw-r--r--   0 sawradip   (501) staff       (20)      161 2024-05-13 07:27:09.000000 composio_griptape-0.2.59/composio_griptape/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     5393 2024-05-13 07:27:09.000000 composio_griptape-0.2.59/composio_griptape/griptape_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:53.887955 composio_griptape-0.2.59/composio_griptape.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-13 09:47:53.000000 composio_griptape-0.2.59/composio_griptape.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      291 2024-05-13 09:47:53.000000 composio_griptape-0.2.59/composio_griptape.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-13 09:47:53.000000 composio_griptape-0.2.59/composio_griptape.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       40 2024-05-13 09:47:53.000000 composio_griptape-0.2.59/composio_griptape.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       18 2024-05-13 09:47:53.000000 composio_griptape-0.2.59/composio_griptape.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-13 09:47:53.888439 composio_griptape-0.2.59/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      853 2024-05-13 09:47:44.000000 composio_griptape-0.2.59/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:43.163425 composio_griptape-0.2.60/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-14 10:58:43.163194 composio_griptape-0.2.60/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     1851 2024-05-13 07:27:09.000000 composio_griptape-0.2.60/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:43.161930 composio_griptape-0.2.60/composio_griptape/
+-rw-r--r--   0 sawradip   (501) staff       (20)      161 2024-05-13 07:27:09.000000 composio_griptape-0.2.60/composio_griptape/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     5395 2024-05-14 10:49:45.000000 composio_griptape-0.2.60/composio_griptape/griptape_toolspec.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:43.162954 composio_griptape-0.2.60/composio_griptape.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      291 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       40 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       18 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-14 10:58:43.163473 composio_griptape-0.2.60/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      853 2024-05-14 10:58:34.000000 composio_griptape-0.2.60/setup.py
```

### Comparing `composio_griptape-0.2.59/PKG-INFO` & `composio_griptape-0.2.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.59
+Version: 0.2.60
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.59
+Requires-Dist: composio_core===0.2.60
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.2.59/README.md` & `composio_griptape-0.2.60/README.md`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.2.59/composio_griptape/griptape_toolspec.py` & `composio_griptape-0.2.60/composio_griptape/griptape_toolspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         }
 
         class tool_class(BaseTool):
             @activity(
                 config=griptape_activity_config
             )
             def execute_task(nested_self, params: dict):
-                print(params)
+                # print(params)
                 params_dict = params["values"]
                 return self.client.execute_action(
                             self.client.get_action_enum(name, appName), 
                             params_dict, 
                             entity_id= self.entity_id
                         )
```

### Comparing `composio_griptape-0.2.59/composio_griptape.egg-info/PKG-INFO` & `composio_griptape-0.2.60/composio_griptape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.59
+Version: 0.2.60
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.59
+Requires-Dist: composio_core===0.2.60
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.2.59/setup.py` & `composio_griptape-0.2.60/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_griptape",
-    version="0.2.59",
+    version="0.2.60",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Griptape wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
     install_requires=[
-        "composio_core===0.2.59",
+        "composio_core===0.2.60",
         "griptape>=0.24.2"
     ],
     include_package_data=True,
 )
```
