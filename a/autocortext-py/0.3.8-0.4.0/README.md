# Comparing `tmp/autocortext_py-0.3.8.tar.gz` & `tmp/autocortext_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocortext_py-0.3.8.tar", last modified: Sun May  5 15:01:23 2024, max compression
+gzip compressed data, was "autocortext_py-0.4.0.tar", last modified: Mon May 13 22:20:30 2024, max compression
```

## Comparing `autocortext_py-0.3.8.tar` & `autocortext_py-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-05 15:01:23.303606 autocortext_py-0.3.8/
--rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.3.8/LICENSE
--rw-r--r--   0 mark       (502) staff       (20)     1445 2024-05-05 15:01:23.303495 autocortext_py-0.3.8/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      958 2024-04-27 15:23:27.000000 autocortext_py-0.3.8/README.md
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-05 15:01:23.302537 autocortext_py-0.3.8/autocortext_py/
--rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.3.8/autocortext_py/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)    13101 2024-05-05 15:01:11.000000 autocortext_py-0.3.8/autocortext_py/client.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-05 15:01:23.303249 autocortext_py-0.3.8/autocortext_py.egg-info/
--rw-r--r--   0 mark       (502) staff       (20)     1445 2024-05-05 15:01:23.000000 autocortext_py-0.3.8/autocortext_py.egg-info/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      267 2024-05-05 15:01:23.000000 autocortext_py-0.3.8/autocortext_py.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2024-05-05 15:01:23.000000 autocortext_py-0.3.8/autocortext_py.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (502) staff       (20)       18 2024-05-05 15:01:23.000000 autocortext_py-0.3.8/autocortext_py.egg-info/requires.txt
--rw-r--r--   0 mark       (502) staff       (20)       15 2024-05-05 15:01:23.000000 autocortext_py-0.3.8/autocortext_py.egg-info/top_level.txt
--rw-r--r--   0 mark       (502) staff       (20)       38 2024-05-05 15:01:23.303652 autocortext_py-0.3.8/setup.cfg
--rw-r--r--   0 mark       (502) staff       (20)      687 2024-05-05 15:00:59.000000 autocortext_py-0.3.8/setup.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:20:30.135336 autocortext_py-0.4.0/
+-rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.4.0/LICENSE
+-rw-r--r--   0 mark       (502) staff       (20)     1445 2024-05-13 22:20:30.135178 autocortext_py-0.4.0/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      958 2024-05-13 21:40:43.000000 autocortext_py-0.4.0/README.md
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:20:30.134132 autocortext_py-0.4.0/autocortext_py/
+-rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.4.0/autocortext_py/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)    13437 2024-05-13 21:46:34.000000 autocortext_py-0.4.0/autocortext_py/client.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:20:30.134992 autocortext_py-0.4.0/autocortext_py.egg-info/
+-rw-r--r--   0 mark       (502) staff       (20)     1445 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      267 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (502) staff       (20)       18 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/requires.txt
+-rw-r--r--   0 mark       (502) staff       (20)       15 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/top_level.txt
+-rw-r--r--   0 mark       (502) staff       (20)       38 2024-05-13 22:20:30.135385 autocortext_py-0.4.0/setup.cfg
+-rw-r--r--   0 mark       (502) staff       (20)      687 2024-05-13 21:40:57.000000 autocortext_py-0.4.0/setup.py
```

### Comparing `autocortext_py-0.3.8/LICENSE` & `autocortext_py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.3.8/PKG-INFO` & `autocortext_py-0.4.0/autocortext_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: autocortext_py
-Version: 0.3.8
+Name: autocortext-py
+Version: 0.4.0
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
```

### Comparing `autocortext_py-0.3.8/README.md` & `autocortext_py-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.3.8/autocortext_py/client.py` & `autocortext_py-0.4.0/autocortext_py/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,43 +11,50 @@
 
     Attributes:
         org_id (str): The organization ID required for API requests.
         api_key (str): The API key used for secure communication with the API.
         base_url (str): The base URL for the API endpoints.
     """
 
-    def __init__(self, org_id, api_key):
+    def __init__(self, org_id, api_key, env="prod"):
         """
         Initializes the AutoCortext client with necessary authentication credentials.
 
         Args:
             org_id (str): The organization ID for the API.
             api_key (str): The API key for accessing the API.
+            env (str): The environment to use. Must be either "prod" or "dev".
 
         Raises:
             ValueError: If either org_id or api_key is not provided.
         """
         if not org_id:
             raise ValueError("Organization ID must be provided and cannot be empty.")
         if not api_key:
             raise ValueError("API key must be provided and cannot be empty.")
+        if env not in ["prod", "dev"]:
+            raise ValueError("Environment must be either 'prod' or 'dev'.")
 
         self.configured = False
         self.system = "Not specified"
         self.machine = "Not specified"
         self.verbosity = "concise"
         self.response_type = "Technician"
         self.history = [
             {
                 "id": 1,
                 "content": f"Auto Cortext: Hello sir/madam.\n\nToday's date is {datetime.datetime.now().date()}, and the local time is {datetime.datetime.now().time().strftime('%H:%M:%S')}. \n\nWhat machine are you having trouble with?",
                 "role": "assistant",
             },
         ]
-        self.base_url = "https://ascend-six.vercel.app/"
+        self.base_url = (
+            "https://ascend-six.vercel.app/"
+            if env == "prod"
+            else "https://ascend-git-develop-ascend-engineering.vercel.app/"
+        )
         self.org_id = org_id
         self.headers = {
             "Authorization": f"Bearer {api_key}",
             "Content-Type": "application/json",
         }
 
     def config(self, verbosity=None, machine=None, system=None, response_type=None):
```

### Comparing `autocortext_py-0.3.8/autocortext_py.egg-info/PKG-INFO` & `autocortext_py-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: autocortext-py
-Version: 0.3.8
+Name: autocortext_py
+Version: 0.4.0
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
```

### Comparing `autocortext_py-0.3.8/setup.py` & `autocortext_py-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autocortext_py",
-    version="0.3.8",
+    version="0.4.0",
     description="Simple client for AutoCortext API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Mark Watson",
     author_email="markus.c.watson@gmail.com",
     url="https://autocortext.com",
     keywords=["autocortext"],
```

