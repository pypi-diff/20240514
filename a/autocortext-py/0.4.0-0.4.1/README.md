# Comparing `tmp/autocortext_py-0.4.0.tar.gz` & `tmp/autocortext_py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocortext_py-0.4.0.tar", last modified: Mon May 13 22:20:30 2024, max compression
+gzip compressed data, was "autocortext_py-0.4.1.tar", last modified: Mon May 13 22:34:56 2024, max compression
```

## Comparing `autocortext_py-0.4.0.tar` & `autocortext_py-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:20:30.135336 autocortext_py-0.4.0/
--rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.4.0/LICENSE
--rw-r--r--   0 mark       (502) staff       (20)     1445 2024-05-13 22:20:30.135178 autocortext_py-0.4.0/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      958 2024-05-13 21:40:43.000000 autocortext_py-0.4.0/README.md
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:20:30.134132 autocortext_py-0.4.0/autocortext_py/
--rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.4.0/autocortext_py/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)    13437 2024-05-13 21:46:34.000000 autocortext_py-0.4.0/autocortext_py/client.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:20:30.134992 autocortext_py-0.4.0/autocortext_py.egg-info/
--rw-r--r--   0 mark       (502) staff       (20)     1445 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      267 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (502) staff       (20)       18 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/requires.txt
--rw-r--r--   0 mark       (502) staff       (20)       15 2024-05-13 22:20:30.000000 autocortext_py-0.4.0/autocortext_py.egg-info/top_level.txt
--rw-r--r--   0 mark       (502) staff       (20)       38 2024-05-13 22:20:30.135385 autocortext_py-0.4.0/setup.cfg
--rw-r--r--   0 mark       (502) staff       (20)      687 2024-05-13 21:40:57.000000 autocortext_py-0.4.0/setup.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:34:56.928357 autocortext_py-0.4.1/
+-rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.4.1/LICENSE
+-rw-r--r--   0 mark       (502) staff       (20)     1461 2024-05-13 22:34:56.928190 autocortext_py-0.4.1/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      974 2024-05-13 22:33:07.000000 autocortext_py-0.4.1/README.md
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:34:56.927116 autocortext_py-0.4.1/autocortext_py/
+-rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.4.1/autocortext_py/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)    13626 2024-05-13 22:34:14.000000 autocortext_py-0.4.1/autocortext_py/client.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-05-13 22:34:56.927949 autocortext_py-0.4.1/autocortext_py.egg-info/
+-rw-r--r--   0 mark       (502) staff       (20)     1461 2024-05-13 22:34:56.000000 autocortext_py-0.4.1/autocortext_py.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      267 2024-05-13 22:34:56.000000 autocortext_py-0.4.1/autocortext_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2024-05-13 22:34:56.000000 autocortext_py-0.4.1/autocortext_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (502) staff       (20)       18 2024-05-13 22:34:56.000000 autocortext_py-0.4.1/autocortext_py.egg-info/requires.txt
+-rw-r--r--   0 mark       (502) staff       (20)       15 2024-05-13 22:34:56.000000 autocortext_py-0.4.1/autocortext_py.egg-info/top_level.txt
+-rw-r--r--   0 mark       (502) staff       (20)       38 2024-05-13 22:34:56.928417 autocortext_py-0.4.1/setup.cfg
+-rw-r--r--   0 mark       (502) staff       (20)      687 2024-05-13 22:32:30.000000 autocortext_py-0.4.1/setup.py
```

### Comparing `autocortext_py-0.4.0/LICENSE` & `autocortext_py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.4.0/PKG-INFO` & `autocortext_py-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocortext_py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
@@ -47,14 +47,15 @@
 )
 
 client.config(
     verbosity="concise",
     machine="Conveyor System",
     system="Electrical",
     response_type="Technician",
+    env="prod",
 )
 
 res = client.troubleshoot("The 24 volt system in the conveyor is not powering on.")
 print(res)
 
 client.set_verbosity("verbose")
 res = client.troubleshoot("OK how do I fix it?")
```

### Comparing `autocortext_py-0.4.0/README.md` & `autocortext_py-0.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 )
 
 client.config(
     verbosity="concise",
     machine="Conveyor System",
     system="Electrical",
     response_type="Technician",
+    env="prod",
 )
 
 res = client.troubleshoot("The 24 volt system in the conveyor is not powering on.")
 print(res)
 
 client.set_verbosity("verbose")
 res = client.troubleshoot("OK how do I fix it?")
```

### Comparing `autocortext_py-0.4.0/autocortext_py/client.py` & `autocortext_py-0.4.1/autocortext_py/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,68 +11,64 @@
 
     Attributes:
         org_id (str): The organization ID required for API requests.
         api_key (str): The API key used for secure communication with the API.
         base_url (str): The base URL for the API endpoints.
     """
 
-    def __init__(self, org_id, api_key, env="prod"):
+    def __init__(self, org_id, api_key):
         """
         Initializes the AutoCortext client with necessary authentication credentials.
 
         Args:
             org_id (str): The organization ID for the API.
             api_key (str): The API key for accessing the API.
-            env (str): The environment to use. Must be either "prod" or "dev".
 
         Raises:
             ValueError: If either org_id or api_key is not provided.
         """
         if not org_id:
             raise ValueError("Organization ID must be provided and cannot be empty.")
         if not api_key:
             raise ValueError("API key must be provided and cannot be empty.")
-        if env not in ["prod", "dev"]:
-            raise ValueError("Environment must be either 'prod' or 'dev'.")
 
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
-        self.base_url = (
-            "https://ascend-six.vercel.app/"
-            if env == "prod"
-            else "https://ascend-git-develop-ascend-engineering.vercel.app/"
-        )
+        self.base_url = "https://ascend-six.vercel.app/"
         self.org_id = org_id
         self.headers = {
             "Authorization": f"Bearer {api_key}",
             "Content-Type": "application/json",
         }
 
-    def config(self, verbosity=None, machine=None, system=None, response_type=None):
+    def config(
+        self, verbosity=None, machine=None, system=None, response_type=None, env="prod"
+    ):
         """
         Configures the AutoCortext client with machine name and verbosity level.
 
         This method allows you to set the name of the machine and system being troubleshooted, the
         verbosity level of the responses from the AutoCortext API, and the response type.
 
         Args:
             verbosity (str): The verbosity level of the responses. Must be either "concise" or "verbose".
             machine (str): The name of the machine or system being troubleshooted.
             system (str): The system or software being troubleshooted.
             response_type (str): The type of response to be given by the assistant. Must be either "Technician", "Engineer", or "Maintenance".
+            env (str): The environment to use. Must be either "prod" or "dev".
 
         Returns:
             None
 
         Raises:
             ValueError: If the AutoCortext client is already configured.
             ValueError: If the machine name, system, verbosity, or response_type are not provided or are not strings.
@@ -86,14 +82,16 @@
             raise ValueError("Machine name must be provided and cannot be empty.")
         if not verbosity:
             raise ValueError("Verbosity must be provided and cannot be empty.")
         if not system:
             raise ValueError("System name must be provided and cannot be empty.")
         if not response_type:
             raise ValueError("Response type must be provided and cannot be empty.")
+        if env not in ["prod", "dev"]:
+            raise ValueError("Environment must be either 'prod' or 'dev'.")
 
         if not isinstance(machine, str):
             raise ValueError("Machine name must be a string.")
         if not isinstance(verbosity, str):
             raise ValueError("Verbosity must be a string.")
         if not isinstance(system, str):
             raise ValueError("System name must be a string.")
@@ -107,19 +105,25 @@
                 "Response type must be either 'Technician', 'Engineer', or 'Maintenance'."
             )
 
         self.machine = machine
         self.verbosity = verbosity
         self.system = system
         self.response_type = response_type
+        self.base_url = (
+            "https://ascend-six.vercel.app/"
+            if env == "prod"
+            else "https://ascend-git-develop-ascend-engineering.vercel.app/"
+        )
 
         print(f"[autocortext_py] Machine set to {machine}.")
         print(f"[autocortext_py] Verbosity set to {verbosity}.")
         print(f"[autocortext_py] System set to {system}.")
         print(f"[autocortext_py] Response type set to {response_type}.")
+        print(f"[autocortext_py] Environment set to {env}.")
 
         # add required prompts
         new_messages = [
             {
                 "id": 2,
                 "content": f"User: The user selected the {machine}.",
                 "role": "user",
@@ -350,14 +354,15 @@
         Returns:
             None
         """
         self.configured = False
         self.system = "Not specified"
         self.machine = "Not specified"
         self.verbosity = "concise"
+        self.base_url = "https://ascend-six.vercel.app/"
         self.history = [
             {
                 "id": 1,
                 "content": f"Auto Cortext: Hello sir/madam.\n\nToday's date is {datetime.datetime.now().date()}, and the local time is {datetime.datetime.now().time().strftime('%H:%M:%S')}. \n\nWhat machine are you having trouble with?",
                 "role": "assistant",
             }
         ]
```

### Comparing `autocortext_py-0.4.0/autocortext_py.egg-info/PKG-INFO` & `autocortext_py-0.4.1/autocortext_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocortext-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
@@ -47,14 +47,15 @@
 )
 
 client.config(
     verbosity="concise",
     machine="Conveyor System",
     system="Electrical",
     response_type="Technician",
+    env="prod",
 )
 
 res = client.troubleshoot("The 24 volt system in the conveyor is not powering on.")
 print(res)
 
 client.set_verbosity("verbose")
 res = client.troubleshoot("OK how do I fix it?")
```

### Comparing `autocortext_py-0.4.0/setup.py` & `autocortext_py-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autocortext_py",
-    version="0.4.0",
+    version="0.4.1",
     description="Simple client for AutoCortext API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Mark Watson",
     author_email="markus.c.watson@gmail.com",
     url="https://autocortext.com",
     keywords=["autocortext"],
```

