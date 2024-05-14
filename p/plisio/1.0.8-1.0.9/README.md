# Comparing `tmp/plisio-1.0.8.tar.gz` & `tmp/plisio-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plisio-1.0.8.tar", last modified: Tue Mar 19 06:34:48 2024, max compression
+gzip compressed data, was "plisio-1.0.9.tar", last modified: Tue May 14 19:13:58 2024, max compression
```

## Comparing `plisio-1.0.8.tar` & `plisio-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-03-19 06:34:48.768856 plisio-1.0.8/
--rw-r--r--   0 alexey     (501) staff       (20)     1059 2023-06-11 18:00:39.000000 plisio-1.0.8/LICENSE.txt
--rw-r--r--   0 alexey     (501) staff       (20)    15856 2024-03-19 06:34:48.768606 plisio-1.0.8/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)    14854 2024-03-19 06:33:16.000000 plisio-1.0.8/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-03-19 06:34:48.766817 plisio-1.0.8/plisio/
--rw-r--r--   0 alexey     (501) staff       (20)     1109 2023-06-23 17:49:31.000000 plisio-1.0.8/plisio/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    22753 2024-03-19 06:33:16.000000 plisio-1.0.8/plisio/plisio_client.py
--rw-r--r--   0 alexey     (501) staff       (20)     6033 2024-03-19 06:33:16.000000 plisio-1.0.8/plisio/plisio_enums.py
--rw-r--r--   0 alexey     (501) staff       (20)     3351 2023-06-11 18:00:39.000000 plisio-1.0.8/plisio/plisio_exceptions.py
--rw-r--r--   0 alexey     (501) staff       (20)    22325 2023-06-23 17:49:35.000000 plisio-1.0.8/plisio/plisio_models.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-03-19 06:34:48.768284 plisio-1.0.8/plisio.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)    15856 2024-03-19 06:34:48.000000 plisio-1.0.8/plisio.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      307 2024-03-19 06:34:48.000000 plisio-1.0.8/plisio.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2024-03-19 06:34:48.000000 plisio-1.0.8/plisio.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)       30 2024-03-19 06:34:48.000000 plisio-1.0.8/plisio.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)        7 2024-03-19 06:34:48.000000 plisio-1.0.8/plisio.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)       79 2024-03-19 06:34:48.769151 plisio-1.0.8/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1238 2024-03-19 06:34:13.000000 plisio-1.0.8/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-14 19:13:58.359408 plisio-1.0.9/
+-rw-r--r--   0 alex       (501) staff       (20)     1059 2024-05-14 19:01:57.000000 plisio-1.0.9/LICENSE.txt
+-rw-r--r--   0 alex       (501) staff       (20)    15957 2024-05-14 19:13:58.358845 plisio-1.0.9/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)    14854 2024-05-14 19:01:57.000000 plisio-1.0.9/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-14 19:13:58.354907 plisio-1.0.9/plisio/
+-rw-r--r--   0 alex       (501) staff       (20)     1109 2024-05-14 19:01:57.000000 plisio-1.0.9/plisio/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    22761 2024-05-14 19:04:42.000000 plisio-1.0.9/plisio/plisio_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     6033 2024-05-14 19:01:57.000000 plisio-1.0.9/plisio/plisio_enums.py
+-rw-r--r--   0 alex       (501) staff       (20)     3351 2024-05-14 19:01:57.000000 plisio-1.0.9/plisio/plisio_exceptions.py
+-rw-r--r--   0 alex       (501) staff       (20)    22325 2024-05-14 19:01:57.000000 plisio-1.0.9/plisio/plisio_models.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-14 19:13:58.357891 plisio-1.0.9/plisio.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)    15957 2024-05-14 19:13:58.000000 plisio-1.0.9/plisio.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      307 2024-05-14 19:13:58.000000 plisio-1.0.9/plisio.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-14 19:13:58.000000 plisio-1.0.9/plisio.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       58 2024-05-14 19:13:58.000000 plisio-1.0.9/plisio.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        7 2024-05-14 19:13:58.000000 plisio-1.0.9/plisio.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       79 2024-05-14 19:13:58.361256 plisio-1.0.9/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1379 2024-05-14 19:13:54.000000 plisio-1.0.9/setup.py
```

### Comparing `plisio-1.0.8/LICENSE.txt` & `plisio-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plisio-1.0.8/PKG-INFO` & `plisio-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plisio
-Version: 1.0.8
+Version: 1.0.9
 Summary: Official Python SDK for Plisio API
 Home-page: https://github.com/Plisio/plisio-python
 Download-URL: https://github.com/Plisio/plisio-python
 Author: Plisio
 Author-email: support@plisio.net
 License: MIT
 Keywords: plisio,crypto payment,sdk,bitcoin,etherium,crypto,blockchain
@@ -14,20 +14,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp
 Requires-Dist: requests
-Requires-Dist: hashlib
-Requires-Dist: hmac
+Requires-Dist: hashlib; python_version <= "3.9"
+Requires-Dist: hmac; python_version <= "3.9"
 
 # Python SDK for Plisio API
 
 Current project is a **Python SDK for [Plisio API](https://plisio.net/documentation)**.
 To use it, you should be registered on Plisio
 The account can be created [here](https://plisio.net/account/signup "Sign up"))
 You will receive a personal secret key, that is used for all calls to API.
```

### Comparing `plisio-1.0.8/README.md` & `plisio-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `plisio-1.0.8/plisio/__init__.py` & `plisio-1.0.9/plisio/__init__.py`

 * *Files identical despite different names*

### Comparing `plisio-1.0.8/plisio/plisio_client.py` & `plisio-1.0.9/plisio/plisio_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,23 +240,23 @@
         return self.__create_request(
             self._url.operations + '/' + kwargs['id_'],
             {},
             plisio.Operation
         )
 
     def validate_callback(self, data: str) -> bool:
-        jsonObj = json.loads(data)
-        verifyHash = jsonObj['verify_hash']
-        del jsonObj["verify_hash"]
-        json.dumps(jsonObj, sort_keys=True)
+        json_obj = json.loads(data)
+        verify_hash = json_obj['verify_hash']
+        del json_obj["verify_hash"]
+        json.dumps(json_obj, sort_keys=True)
         key = bytes(str(self.__api_key), 'utf8')
-        postStr = bytes(json.dumps(jsonObj, separators=(',', ':')), 'utf8');
-        digester = hmac.new(key, postStr, hashlib.sha1)
+        post_str = bytes(json.dumps(json_obj, separators=(',', ':')), 'utf8')
+        digester = hmac.new(key, post_str, hashlib.sha1)
         hash = digester.hexdigest()
-        return hash == verifyHash
+        return hash == verify_hash
 
 
 class PlisioClient(_BaseClient):
     @staticmethod
     def _send_request(request: '_PlisioRequest') -> 'plisio.ModelType':
         try:
             _req = requests.request(
```

### Comparing `plisio-1.0.8/plisio/plisio_enums.py` & `plisio-1.0.9/plisio/plisio_enums.py`

 * *Files identical despite different names*

### Comparing `plisio-1.0.8/plisio/plisio_exceptions.py` & `plisio-1.0.9/plisio/plisio_exceptions.py`

 * *Files identical despite different names*

### Comparing `plisio-1.0.8/plisio/plisio_models.py` & `plisio-1.0.9/plisio/plisio_models.py`

 * *Files identical despite different names*

### Comparing `plisio-1.0.8/plisio.egg-info/PKG-INFO` & `plisio-1.0.9/plisio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plisio
-Version: 1.0.8
+Version: 1.0.9
 Summary: Official Python SDK for Plisio API
 Home-page: https://github.com/Plisio/plisio-python
 Download-URL: https://github.com/Plisio/plisio-python
 Author: Plisio
 Author-email: support@plisio.net
 License: MIT
 Keywords: plisio,crypto payment,sdk,bitcoin,etherium,crypto,blockchain
@@ -14,20 +14,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp
 Requires-Dist: requests
-Requires-Dist: hashlib
-Requires-Dist: hmac
+Requires-Dist: hashlib; python_version <= "3.9"
+Requires-Dist: hmac; python_version <= "3.9"
 
 # Python SDK for Plisio API
 
 Current project is a **Python SDK for [Plisio API](https://plisio.net/documentation)**.
 To use it, you should be registered on Plisio
 The account can be created [here](https://plisio.net/account/signup "Sign up"))
 You will receive a personal secret key, that is used for all calls to API.
```

