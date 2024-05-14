# Comparing `tmp/paradi-0.1.1.tar.gz` & `tmp/paradi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradi-0.1.1.tar", last modified: Mon May 13 13:29:54 2024, max compression
+gzip compressed data, was "paradi-0.1.2.tar", last modified: Tue May 14 06:55:18 2024, max compression
```

## Comparing `paradi-0.1.1.tar` & `paradi-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 13:29:54.875883 paradi-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-04-30 09:47:54.000000 paradi-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3022 2024-05-13 13:29:54.874886 paradi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2400 2024-05-13 13:10:09.000000 paradi-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 13:29:54.873889 paradi-0.1.1/paradi.egg-info/
--rw-rw-rw-   0        0        0     3022 2024-05-13 13:29:54.000000 paradi-0.1.1/paradi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-05-13 13:29:54.000000 paradi-0.1.1/paradi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 13:29:54.000000 paradi-0.1.1/paradi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-13 13:29:54.000000 paradi-0.1.1/paradi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      676 2024-05-13 13:17:19.000000 paradi-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 13:29:54.875883 paradi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      298 2024-05-13 13:17:19.000000 paradi-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 13:29:54.872891 paradi-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:32:38.000000 paradi-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2276 2024-05-13 10:23:13.000000 paradi-0.1.1/tests/flask_test_api.py
--rw-rw-rw-   0        0        0     2172 2024-05-13 10:22:23.000000 paradi-0.1.1/tests/test_paradi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:18.256995 paradi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 06:55:13.000000 paradi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 06:55:18.256995 paradi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-14 06:55:13.000000 paradi-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:18.256995 paradi-0.1.2/paradi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 06:55:18.000000 paradi-0.1.2/paradi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 06:55:13.000000 paradi-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:55:18.256995 paradi-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 06:55:13.000000 paradi-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:18.256995 paradi-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:55:13.000000 paradi-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 06:55:13.000000 paradi-0.1.2/tests/flask_test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-14 06:55:13.000000 paradi-0.1.2/tests/test_paradi.py
```

### Comparing `paradi-0.1.1/LICENSE` & `paradi-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Julien Crambes
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Julien Crambes
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `paradi-0.1.1/PKG-INFO` & `paradi-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: paradi
-Version: 0.1.1
-Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
-Author: Julien Crambes
-Author-email: Julien Crambes <julien.crambes@gmail.com>
-Project-URL: Homepage, https://github.com/Elektriman/paradi
-Project-URL: Issues, https://github.com/Elektriman/paradi/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Paradi
-### Python Abstract Restful Api Dialoger Interface
-
-This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities. <br/>
-It is meant to be very simple to allow a flexible implementation of the many ways to interact with any API, especially regarding the many different authentication methods. <br/>
-You should also put in the child class any code that would parse the requests kwargs or read the output data format of the API and turn it into something more readable than a json (like a pandas dataframe). <br/>
-
-# Example Implementation
-The API is hosted at `https://exampleapiurl.com`. <br/>
-To log in, you need to provide a username and a password in a **post** request at `https://exampleapiurl.com/login` which will return you a temporary connection token in the response. <br/>
-To log out, you need to do a **get** request at `https://exampleapiurl.com/logout` with your credentials. <br/>
-For any other request, to get your private data at `https://exampleapiurl.com/values` you need to provide your credentials in the header. <br/>
-
-```py
-class Dummy(Paradi):
-    def __init__(self):
-        super().__init__(entry=os.getenv('API_ENDPOINT')",
-                         login_uri="login",
-                         logout_uri="logout",
-                         login_kwargs={"headers": {"Content-Type": r"application/x-www-form-urlencoded"},
-                                       "data": {"username":os.getenv("API_USERNAME"),
-                                                "password":os.getenv("API_PASSWORD")}})
-        
-        def _save_auth(self,
-                       response: requests.Response
-                       ):
-            self.access_token = json.loads(response.text)['access_token']
-            self.token_type = json.loads(response.text)['token_type']
-            self.session.headers.update({'Authorization': f'{self.token_type} {self.access_token}'})
-
-        def get_raw_data(self):
-            response = self.get("values")
-            return pd.json_normalize(json.loads(response.text), "data")
-```
-
-To use your newly made class you need to use the `with` syntax provided by python:
-
-```py
-with Dummy() as dummy:
-    raw_data = dummy.get_raw_data()
-```
-This will ensure that the connection with your API is closed as soon as you are finished with the data recovery.
-
+Metadata-Version: 2.1
+Name: paradi
+Version: 0.1.2
+Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
+Author: Julien Crambes
+Author-email: Julien Crambes <julien.crambes@gmail.com>
+Project-URL: Homepage, https://github.com/Elektriman/paradi
+Project-URL: Issues, https://github.com/Elektriman/paradi/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Paradi
+### Python Abstract Restful Api Dialoger Interface
+
+This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities. <br/>
+It is meant to be very simple to allow a flexible implementation of the many ways to interact with any API, especially regarding the many different authentication methods. <br/>
+You should also put in the child class any code that would parse the requests kwargs or read the output data format of the API and turn it into something more readable than a json (like a pandas dataframe). <br/>
+
+# Example Implementation
+The API is hosted at `https://exampleapiurl.com`. <br/>
+To log in, you need to provide a username and a password in a **post** request at `https://exampleapiurl.com/login` which will return you a temporary connection token in the response. <br/>
+To log out, you need to do a **get** request at `https://exampleapiurl.com/logout` with your credentials. <br/>
+For any other request, to get your private data at `https://exampleapiurl.com/values` you need to provide your credentials in the header. <br/>
+
+```py
+class Dummy(Paradi):
+    def __init__(self):
+        super().__init__(entry=os.getenv('API_ENDPOINT')",
+                         login_uri="login",
+                         logout_uri="logout",
+                         login_kwargs={"headers": {"Content-Type": r"application/x-www-form-urlencoded"},
+                                       "data": {"username":os.getenv("API_USERNAME"),
+                                                "password":os.getenv("API_PASSWORD")}})
+        
+        def _save_auth(self,
+                       response: requests.Response
+                       ):
+            self.access_token = json.loads(response.text)['access_token']
+            self.token_type = json.loads(response.text)['token_type']
+            self.session.headers.update({'Authorization': f'{self.token_type} {self.access_token}'})
+
+        def get_raw_data(self):
+            response = self.get("values")
+            return pd.json_normalize(json.loads(response.text), "data")
+```
+
+To use your newly made class you need to use the `with` syntax provided by python:
+
+```py
+with Dummy() as dummy:
+    raw_data = dummy.get_raw_data()
+```
+This will ensure that the connection with your API is closed as soon as you are finished with the data recovery.
+
```

### Comparing `paradi-0.1.1/README.md` & `paradi-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Paradi
-### Python Abstract Restful Api Dialoger Interface
-
-This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities. <br/>
-It is meant to be very simple to allow a flexible implementation of the many ways to interact with any API, especially regarding the many different authentication methods. <br/>
-You should also put in the child class any code that would parse the requests kwargs or read the output data format of the API and turn it into something more readable than a json (like a pandas dataframe). <br/>
-
-# Example Implementation
-The API is hosted at `https://exampleapiurl.com`. <br/>
-To log in, you need to provide a username and a password in a **post** request at `https://exampleapiurl.com/login` which will return you a temporary connection token in the response. <br/>
-To log out, you need to do a **get** request at `https://exampleapiurl.com/logout` with your credentials. <br/>
-For any other request, to get your private data at `https://exampleapiurl.com/values` you need to provide your credentials in the header. <br/>
-
-```py
-class Dummy(Paradi):
-    def __init__(self):
-        super().__init__(entry=os.getenv('API_ENDPOINT')",
-                         login_uri="login",
-                         logout_uri="logout",
-                         login_kwargs={"headers": {"Content-Type": r"application/x-www-form-urlencoded"},
-                                       "data": {"username":os.getenv("API_USERNAME"),
-                                                "password":os.getenv("API_PASSWORD")}})
-        
-        def _save_auth(self,
-                       response: requests.Response
-                       ):
-            self.access_token = json.loads(response.text)['access_token']
-            self.token_type = json.loads(response.text)['token_type']
-            self.session.headers.update({'Authorization': f'{self.token_type} {self.access_token}'})
-
-        def get_raw_data(self):
-            response = self.get("values")
-            return pd.json_normalize(json.loads(response.text), "data")
-```
-
-To use your newly made class you need to use the `with` syntax provided by python:
-
-```py
-with Dummy() as dummy:
-    raw_data = dummy.get_raw_data()
-```
-This will ensure that the connection with your API is closed as soon as you are finished with the data recovery.
-
+# Paradi
+### Python Abstract Restful Api Dialoger Interface
+
+This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities. <br/>
+It is meant to be very simple to allow a flexible implementation of the many ways to interact with any API, especially regarding the many different authentication methods. <br/>
+You should also put in the child class any code that would parse the requests kwargs or read the output data format of the API and turn it into something more readable than a json (like a pandas dataframe). <br/>
+
+# Example Implementation
+The API is hosted at `https://exampleapiurl.com`. <br/>
+To log in, you need to provide a username and a password in a **post** request at `https://exampleapiurl.com/login` which will return you a temporary connection token in the response. <br/>
+To log out, you need to do a **get** request at `https://exampleapiurl.com/logout` with your credentials. <br/>
+For any other request, to get your private data at `https://exampleapiurl.com/values` you need to provide your credentials in the header. <br/>
+
+```py
+class Dummy(Paradi):
+    def __init__(self):
+        super().__init__(entry=os.getenv('API_ENDPOINT')",
+                         login_uri="login",
+                         logout_uri="logout",
+                         login_kwargs={"headers": {"Content-Type": r"application/x-www-form-urlencoded"},
+                                       "data": {"username":os.getenv("API_USERNAME"),
+                                                "password":os.getenv("API_PASSWORD")}})
+        
+        def _save_auth(self,
+                       response: requests.Response
+                       ):
+            self.access_token = json.loads(response.text)['access_token']
+            self.token_type = json.loads(response.text)['token_type']
+            self.session.headers.update({'Authorization': f'{self.token_type} {self.access_token}'})
+
+        def get_raw_data(self):
+            response = self.get("values")
+            return pd.json_normalize(json.loads(response.text), "data")
+```
+
+To use your newly made class you need to use the `with` syntax provided by python:
+
+```py
+with Dummy() as dummy:
+    raw_data = dummy.get_raw_data()
+```
+This will ensure that the connection with your API is closed as soon as you are finished with the data recovery.
+
```

### Comparing `paradi-0.1.1/paradi.egg-info/PKG-INFO` & `paradi-0.1.2/paradi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: paradi
-Version: 0.1.1
-Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
-Author: Julien Crambes
-Author-email: Julien Crambes <julien.crambes@gmail.com>
-Project-URL: Homepage, https://github.com/Elektriman/paradi
-Project-URL: Issues, https://github.com/Elektriman/paradi/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Paradi
-### Python Abstract Restful Api Dialoger Interface
-
-This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities. <br/>
-It is meant to be very simple to allow a flexible implementation of the many ways to interact with any API, especially regarding the many different authentication methods. <br/>
-You should also put in the child class any code that would parse the requests kwargs or read the output data format of the API and turn it into something more readable than a json (like a pandas dataframe). <br/>
-
-# Example Implementation
-The API is hosted at `https://exampleapiurl.com`. <br/>
-To log in, you need to provide a username and a password in a **post** request at `https://exampleapiurl.com/login` which will return you a temporary connection token in the response. <br/>
-To log out, you need to do a **get** request at `https://exampleapiurl.com/logout` with your credentials. <br/>
-For any other request, to get your private data at `https://exampleapiurl.com/values` you need to provide your credentials in the header. <br/>
-
-```py
-class Dummy(Paradi):
-    def __init__(self):
-        super().__init__(entry=os.getenv('API_ENDPOINT')",
-                         login_uri="login",
-                         logout_uri="logout",
-                         login_kwargs={"headers": {"Content-Type": r"application/x-www-form-urlencoded"},
-                                       "data": {"username":os.getenv("API_USERNAME"),
-                                                "password":os.getenv("API_PASSWORD")}})
-        
-        def _save_auth(self,
-                       response: requests.Response
-                       ):
-            self.access_token = json.loads(response.text)['access_token']
-            self.token_type = json.loads(response.text)['token_type']
-            self.session.headers.update({'Authorization': f'{self.token_type} {self.access_token}'})
-
-        def get_raw_data(self):
-            response = self.get("values")
-            return pd.json_normalize(json.loads(response.text), "data")
-```
-
-To use your newly made class you need to use the `with` syntax provided by python:
-
-```py
-with Dummy() as dummy:
-    raw_data = dummy.get_raw_data()
-```
-This will ensure that the connection with your API is closed as soon as you are finished with the data recovery.
-
+Metadata-Version: 2.1
+Name: paradi
+Version: 0.1.2
+Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
+Author: Julien Crambes
+Author-email: Julien Crambes <julien.crambes@gmail.com>
+Project-URL: Homepage, https://github.com/Elektriman/paradi
+Project-URL: Issues, https://github.com/Elektriman/paradi/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Paradi
+### Python Abstract Restful Api Dialoger Interface
+
+This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities. <br/>
+It is meant to be very simple to allow a flexible implementation of the many ways to interact with any API, especially regarding the many different authentication methods. <br/>
+You should also put in the child class any code that would parse the requests kwargs or read the output data format of the API and turn it into something more readable than a json (like a pandas dataframe). <br/>
+
+# Example Implementation
+The API is hosted at `https://exampleapiurl.com`. <br/>
+To log in, you need to provide a username and a password in a **post** request at `https://exampleapiurl.com/login` which will return you a temporary connection token in the response. <br/>
+To log out, you need to do a **get** request at `https://exampleapiurl.com/logout` with your credentials. <br/>
+For any other request, to get your private data at `https://exampleapiurl.com/values` you need to provide your credentials in the header. <br/>
+
+```py
+class Dummy(Paradi):
+    def __init__(self):
+        super().__init__(entry=os.getenv('API_ENDPOINT')",
+                         login_uri="login",
+                         logout_uri="logout",
+                         login_kwargs={"headers": {"Content-Type": r"application/x-www-form-urlencoded"},
+                                       "data": {"username":os.getenv("API_USERNAME"),
+                                                "password":os.getenv("API_PASSWORD")}})
+        
+        def _save_auth(self,
+                       response: requests.Response
+                       ):
+            self.access_token = json.loads(response.text)['access_token']
+            self.token_type = json.loads(response.text)['token_type']
+            self.session.headers.update({'Authorization': f'{self.token_type} {self.access_token}'})
+
+        def get_raw_data(self):
+            response = self.get("values")
+            return pd.json_normalize(json.loads(response.text), "data")
+```
+
+To use your newly made class you need to use the `with` syntax provided by python:
+
+```py
+with Dummy() as dummy:
+    raw_data = dummy.get_raw_data()
+```
+This will ensure that the connection with your API is closed as soon as you are finished with the data recovery.
+
```

### Comparing `paradi-0.1.1/pyproject.toml` & `paradi-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "paradi"
-version = "0.1.1"
-authors = [
-    { name="Julien Crambes", email="julien.crambes@gmail.com" },
-]
-description = "This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities."
-readme = "README.md"
-requires-python = ">=3.12"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/Elektriman/paradi"
-Issues = "https://github.com/Elektriman/paradi/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "paradi"
+version = "0.1.2"
+authors = [
+    { name="Julien Crambes", email="julien.crambes@gmail.com" },
+]
+description = "This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities."
+readme = "README.md"
+requires-python = ">=3.12"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+Homepage = "https://github.com/Elektriman/paradi"
+Issues = "https://github.com/Elektriman/paradi/issues"
```

### Comparing `paradi-0.1.1/tests/flask_test_api.py` & `paradi-0.1.2/tests/flask_test_api.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# %% imports
-import json
-import os
-from flask import Flask, abort, request, make_response
-from dotenv import load_dotenv
-
-# %% constants
-load_dotenv()
-with open("http.json", "r") as f:
-    http_dict = json.load(f)
-
-
-def create_app(config: dict = None):
-    app_instance = Flask(__name__)
-    app_instance.config.from_object(config)
-    return app_instance
-
-
-app = create_app()
-
-
-def shutdown_server():
-    func = request.environ.get('werkzeug.server.shutdown')
-    if func is None:
-        raise RuntimeError('Not running with the Werkzeug Server')
-    func()
-
-
-# %% Routing
-
-
-@app.route("/")
-def index():
-    return make_response(http_dict["200"], 200)
-
-
-@app.route("/http/<int:status_code>", methods=["GET", "POST", "PUT", "PATCH", "DELETE"])
-def http_code_check(status_code: int):
-    if status_code >= 400:
-        try:
-            abort(status_code)
-        except LookupError:
-            abort(500)
-
-    return make_response(http_dict[str(status_code)], status_code)
-
-
-@app.route("/post/<string:input_type>", methods=["GET", "POST"])
-def post(input_type: str):
-    response = make_response(f"{input_type} post successfully", 200)
-    response.content_type = "application/json"
-
-    match input_type:
-        case "data":
-            response.data = request.data
-        case "args":
-            response.data = json.dumps(request.args)
-        case "form":
-            response.data = json.dumps(request.form)
-        case "files":
-            files_submitted = {filename: file.content_length for filename, file in request.files.items()}
-            response.data = json.dumps(files_submitted)
-        case "values":
-            data_submitted = {"args": request.args,
-                              "form": request.form}
-            response.data = json.dumps(data_submitted)
-        case "json":
-            response.data = request.json
-        case _:
-            abort(400)
-
-    return response
-
-
-@app.route('/shutdown')
-def shutdown():
-    shutdown_server()
-    return 'Server shutting down...'
-
-
-if __name__ == "__main__":
-    app.run(host=os.getenv("TEST_SERVER_HOSTNAME"),
-            port=os.getenv("TEST_SERVER_PORT"),
-            debug=True,
-            use_reloader=False)
+# %% imports
+import json
+import os
+from flask import Flask, abort, request, make_response
+from dotenv import load_dotenv
+
+# %% constants
+load_dotenv()
+with open("http.json", "r") as f:
+    http_dict = json.load(f)
+
+
+def create_app(config: dict = None):
+    app_instance = Flask(__name__)
+    app_instance.config.from_object(config)
+    return app_instance
+
+
+app = create_app()
+
+
+def shutdown_server():
+    func = request.environ.get('werkzeug.server.shutdown')
+    if func is None:
+        raise RuntimeError('Not running with the Werkzeug Server')
+    func()
+
+
+# %% Routing
+
+
+@app.route("/")
+def index():
+    return make_response(http_dict["200"], 200)
+
+
+@app.route("/http/<int:status_code>", methods=["GET", "POST", "PUT", "PATCH", "DELETE"])
+def http_code_check(status_code: int):
+    if status_code >= 400:
+        try:
+            abort(status_code)
+        except LookupError:
+            abort(500)
+
+    return make_response(http_dict[str(status_code)], status_code)
+
+
+@app.route("/post/<string:input_type>", methods=["GET", "POST"])
+def post(input_type: str):
+    response = make_response(f"{input_type} post successfully", 200)
+    response.content_type = "application/json"
+
+    match input_type:
+        case "data":
+            response.data = request.data
+        case "args":
+            response.data = json.dumps(request.args)
+        case "form":
+            response.data = json.dumps(request.form)
+        case "files":
+            files_submitted = {filename: file.content_length for filename, file in request.files.items()}
+            response.data = json.dumps(files_submitted)
+        case "values":
+            data_submitted = {"args": request.args,
+                              "form": request.form}
+            response.data = json.dumps(data_submitted)
+        case "json":
+            response.data = request.json
+        case _:
+            abort(400)
+
+    return response
+
+
+@app.route('/shutdown')
+def shutdown():
+    shutdown_server()
+    return 'Server shutting down...'
+
+
+if __name__ == "__main__":
+    app.run(host=os.getenv("TEST_SERVER_HOSTNAME"),
+            port=os.getenv("TEST_SERVER_PORT"),
+            debug=True,
+            use_reloader=False)
```

