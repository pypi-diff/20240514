# Comparing `tmp/flyflowclient-1.14.6.tar.gz` & `tmp/flyflowclient-1.14.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyflowclient-1.14.6.tar", last modified: Mon May 13 00:57:34 2024, max compression
+gzip compressed data, was "flyflowclient-1.14.7.tar", last modified: Tue May 14 00:50:10 2024, max compression
```

## Comparing `flyflowclient-1.14.6.tar` & `flyflowclient-1.14.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-13 00:57:34.774289 flyflowclient-1.14.6/
--rw-r--r--   0 carlcortright   (501) staff       (20)    11357 2024-05-12 23:23:34.000000 flyflowclient-1.14.6/LICENSE
--rw-r--r--   0 carlcortright   (501) staff       (20)     3824 2024-05-13 00:57:34.774098 flyflowclient-1.14.6/PKG-INFO
--rw-r--r--   0 carlcortright   (501) staff       (20)     3366 2024-05-12 23:58:02.000000 flyflowclient-1.14.6/README.md
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-13 00:57:34.773056 flyflowclient-1.14.6/flyflowclient/
--rw-r--r--   0 carlcortright   (501) staff       (20)       27 2024-05-13 00:56:24.000000 flyflowclient-1.14.6/flyflowclient/__init__.py
--rw-r--r--   0 carlcortright   (501) staff       (20)     3647 2024-05-12 23:45:58.000000 flyflowclient-1.14.6/flyflowclient/client.py
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-13 00:57:34.773898 flyflowclient-1.14.6/flyflowclient.egg-info/
--rw-r--r--   0 carlcortright   (501) staff       (20)     3824 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/PKG-INFO
--rw-r--r--   0 carlcortright   (501) staff       (20)      260 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/SOURCES.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)        1 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/dependency_links.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       17 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/requires.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       14 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/top_level.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       38 2024-05-13 00:57:34.774348 flyflowclient-1.14.6/setup.cfg
--rw-r--r--   0 carlcortright   (501) staff       (20)      634 2024-05-13 00:57:32.000000 flyflowclient-1.14.6/setup.py
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-14 00:50:10.009791 flyflowclient-1.14.7/
+-rw-r--r--   0 carlcortright   (501) staff       (20)    11357 2024-05-12 23:23:34.000000 flyflowclient-1.14.7/LICENSE
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3817 2024-05-14 00:50:10.009168 flyflowclient-1.14.7/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3359 2024-05-13 01:08:29.000000 flyflowclient-1.14.7/README.md
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-14 00:50:09.992414 flyflowclient-1.14.7/flyflowclient/
+-rw-r--r--   0 carlcortright   (501) staff       (20)       27 2024-05-13 00:56:24.000000 flyflowclient-1.14.7/flyflowclient/__init__.py
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3825 2024-05-14 00:44:35.000000 flyflowclient-1.14.7/flyflowclient/client.py
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-14 00:50:10.000765 flyflowclient-1.14.7/flyflowclient.egg-info/
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3817 2024-05-14 00:50:09.000000 flyflowclient-1.14.7/flyflowclient.egg-info/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)      260 2024-05-14 00:50:09.000000 flyflowclient-1.14.7/flyflowclient.egg-info/SOURCES.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)        1 2024-05-14 00:50:09.000000 flyflowclient-1.14.7/flyflowclient.egg-info/dependency_links.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       17 2024-05-14 00:50:09.000000 flyflowclient-1.14.7/flyflowclient.egg-info/requires.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       14 2024-05-14 00:50:09.000000 flyflowclient-1.14.7/flyflowclient.egg-info/top_level.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       38 2024-05-14 00:50:10.009882 flyflowclient-1.14.7/setup.cfg
+-rw-r--r--   0 carlcortright   (501) staff       (20)      634 2024-05-14 00:50:08.000000 flyflowclient-1.14.7/setup.py
```

### Comparing `flyflowclient-1.14.6/LICENSE` & `flyflowclient-1.14.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flyflowclient-1.14.6/PKG-INFO` & `flyflowclient-1.14.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyflowclient
-Version: 1.14.6
+Version: 1.14.7
 Summary: A client library for the FlyFlow API
 Home-page: https://github.com/flyflow-devs/flyflow-python
 Author: Carl Cortright
 Author-email: carl@flyflow.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 ```
 
 ## Usage
 
 To use the Flyflow client library, you need to import the `Flyflow` class from the `flyflow.client` module:
 
 ```python
-from flyflowclient.client import Flyflow
+from flyflowclient import Flyflow
 
 client = Flyflow()
 ```
 
 By default, the client will load the API key from the `FLYFLOW_API_KEY` environment variable. If you want to provide the API key explicitly, you can pass it as a parameter when creating the client instance:
 
 ```python
```

### Comparing `flyflowclient-1.14.6/README.md` & `flyflowclient-1.14.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 ## Usage
 
 To use the Flyflow client library, you need to import the `Flyflow` class from the `flyflow.client` module:
 
 ```python
-from flyflowclient.client import Flyflow
+from flyflowclient import Flyflow
 
 client = Flyflow()
 ```
 
 By default, the client will load the API key from the `FLYFLOW_API_KEY` environment variable. If you want to provide the API key explicitly, you can pass it as a parameter when creating the client instance:
 
 ```python
```

### Comparing `flyflowclient-1.14.6/flyflowclient/client.py` & `flyflowclient-1.14.7/flyflowclient/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,41 +40,43 @@
             'limit': limit,
             'agent_id': agent_id
         }
         response = requests.get(f'{self.base_url}/calls', params=params, headers=self.headers)
         response.raise_for_status()
         return response.json()
 
-    def create_agent(self, name, system_prompt, initial_message, llm_model, voice_id, webhook, tools, filler_words, area_code):
+    def create_agent(self, name, system_prompt, initial_message, llm_model, voice_id, webhook, tools, filler_words, filler_words_whitelist, area_code):
         payload = {
             'name': name,
             'system_prompt': system_prompt,
             'initial_message': initial_message,
             'llm_model': llm_model,
             'voice_id': voice_id,
             'webhook': webhook,
             'tools': tools,
             'filler_words': filler_words,
+            'filler_words_whitelist': filler_words_whitelist,
             'area_code': area_code
         }
         response = requests.post(f'{self.base_url}/agent', json=payload, headers=self.headers)
         response.raise_for_status()
         return response.json()
 
-    def update_agent(self, agent_id, name=None, system_prompt=None, initial_message=None, llm_model=None, voice_id=None, webhook=None, tools=None, filler_words=None):
+    def update_agent(self, agent_id, name=None, system_prompt=None, initial_message=None, llm_model=None, voice_id=None, webhook=None, tools=None, filler_words=None, filler_words_whitelist=None):
         payload = {
             'id': agent_id,
             'name': name,
             'system_prompt': system_prompt,
             'initial_message': initial_message,
             'llm_model': llm_model,
             'voice_id': voice_id,
             'webhook': webhook,
             'tools': tools,
-            'filler_words': filler_words
+            'filler_words': filler_words,
+            'filler_words_whitelist': filler_words_whitelist,
         }
         payload = {k: v for k, v in payload.items() if v is not None}
         response = requests.post(f'{self.base_url}/agent', json=payload, headers=self.headers)
         response.raise_for_status()
         return response.json()
 
     def get_agent(self, agent_id):
```

### Comparing `flyflowclient-1.14.6/flyflowclient.egg-info/PKG-INFO` & `flyflowclient-1.14.7/flyflowclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyflowclient
-Version: 1.14.6
+Version: 1.14.7
 Summary: A client library for the FlyFlow API
 Home-page: https://github.com/flyflow-devs/flyflow-python
 Author: Carl Cortright
 Author-email: carl@flyflow.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 ```
 
 ## Usage
 
 To use the Flyflow client library, you need to import the `Flyflow` class from the `flyflow.client` module:
 
 ```python
-from flyflowclient.client import Flyflow
+from flyflowclient import Flyflow
 
 client = Flyflow()
 ```
 
 By default, the client will load the API key from the `FLYFLOW_API_KEY` environment variable. If you want to provide the API key explicitly, you can pass it as a parameter when creating the client instance:
 
 ```python
```

### Comparing `flyflowclient-1.14.6/setup.py` & `flyflowclient-1.14.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="flyflowclient",
-    version="1.14.6",
+    version="1.14.7",
     packages=find_packages(),
     install_requires=[
         "requests>=2.25.1"
     ],
     author="Carl Cortright",
     author_email="carl@flyflow.dev",
     description="A client library for the FlyFlow API",
```

