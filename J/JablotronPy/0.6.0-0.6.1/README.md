# Comparing `tmp/JablotronPy-0.6.0.tar.gz` & `tmp/jablotronpy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JablotronPy-0.6.0.tar", last modified: Sat Nov  4 10:43:47 2023, max compression
+gzip compressed data, was "jablotronpy-0.6.1.tar", last modified: Tue May 14 13:18:49 2024, max compression
```

## Comparing `JablotronPy-0.6.0.tar` & `jablotronpy-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 10:43:47.182771 JablotronPy-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 10:43:47.178771 JablotronPy-0.6.0/JablotronPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-11-04 10:43:47.000000 JablotronPy-0.6.0/JablotronPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-11-04 10:43:47.000000 JablotronPy-0.6.0/JablotronPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-04 10:43:47.000000 JablotronPy-0.6.0/JablotronPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-04 10:43:47.000000 JablotronPy-0.6.0/JablotronPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-04 10:43:47.000000 JablotronPy-0.6.0/JablotronPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-11-04 10:43:37.000000 JablotronPy-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-04 10:43:37.000000 JablotronPy-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-11-04 10:43:47.178771 JablotronPy-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-11-04 10:43:37.000000 JablotronPy-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 10:43:47.178771 JablotronPy-0.6.0/jablotronpy/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-04 10:43:37.000000 JablotronPy-0.6.0/jablotronpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14679 2023-11-04 10:43:37.000000 JablotronPy-0.6.0/jablotronpy/jablotronpy.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-04 10:43:47.182771 JablotronPy-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-11-04 10:43:37.000000 JablotronPy-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 10:43:47.178771 JablotronPy-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-11-04 10:43:37.000000 JablotronPy-0.6.0/tests/test_jablotron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:18:49.265577 jablotronpy-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:18:49.265577 jablotronpy-0.6.1/JablotronPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-14 13:18:49.000000 jablotronpy-0.6.1/JablotronPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-14 13:18:49.000000 jablotronpy-0.6.1/JablotronPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:18:49.000000 jablotronpy-0.6.1/JablotronPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 13:18:49.000000 jablotronpy-0.6.1/JablotronPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 13:18:49.000000 jablotronpy-0.6.1/JablotronPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-14 13:18:45.000000 jablotronpy-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 13:18:45.000000 jablotronpy-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-14 13:18:49.265577 jablotronpy-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-14 13:18:45.000000 jablotronpy-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:18:49.265577 jablotronpy-0.6.1/jablotronpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 13:18:45.000000 jablotronpy-0.6.1/jablotronpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-14 13:18:45.000000 jablotronpy-0.6.1/jablotronpy/jablotronpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:18:49.265577 jablotronpy-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-14 13:18:45.000000 jablotronpy-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:18:49.265577 jablotronpy-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-14 13:18:45.000000 jablotronpy-0.6.1/tests/test_jablotron.py
```

### Comparing `JablotronPy-0.6.0/JablotronPy.egg-info/PKG-INFO` & `jablotronpy-0.6.1/JablotronPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JablotronPy
-Version: 0.6.0
+Version: 0.6.1
 Summary: A client to interact with the Jablotron API to control Jablotron alarm systems
 Home-page: https://github.com/fdegier/JablotronPy
 Author: F. de Gier
 Author-email: freddegier@me.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `JablotronPy-0.6.0/LICENSE` & `jablotronpy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `JablotronPy-0.6.0/PKG-INFO` & `jablotronpy-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JablotronPy
-Version: 0.6.0
+Version: 0.6.1
 Summary: A client to interact with the Jablotron API to control Jablotron alarm systems
 Home-page: https://github.com/fdegier/JablotronPy
 Author: F. de Gier
 Author-email: freddegier@me.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `JablotronPy-0.6.0/README.md` & `jablotronpy-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `JablotronPy-0.6.0/jablotronpy/jablotronpy.py` & `jablotronpy-0.6.1/jablotronpy/jablotronpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import logging
 from typing import Union, Any
 
 import requests
 
+logger = logging.getLogger(__name__)
+
 
 class UnexpectedResponse(Exception):
     """Specialization of exception for cases when request does note return expected data."""
     pass
 
 
 class Jablotron:
@@ -54,34 +57,32 @@
         if r.ok:
             data = r.json()
             if end_point == "userAuthorize.json":
                 return True, r.cookies.get("PHPSESSID")
             if data.get('data') is not None:
                 return True, data["data"]
             else:
-                print(f"Unexpected response from API:")
-                print(data)
+                logger.error(f"Unexpected response from API: {data}")
                 return False, None
 
         data = r.json()
         if data.get('http-code', 0) == 401:
             self.set_cookies()
             if retry >= 3:
-                print(f"Exhausted all retry options, response:")
-                print(data.json())
+                logger.error(f"Exhausted all retry options, response: {data.json()}")
                 if 'errors' in data:
-                    print(data['errors'])
+                    logger.error(data['errors'])
                 return False, None
             else:
                 retry += 1
                 return self._make_request(end_point=end_point, headers=headers, payload=payload, retry=retry)
         else:
-            print(f"An unexpected error occurred")
+            logger.error(f"An unexpected error occurred, status code: {r.status_code}")
             if 'errors' in data:
-                print(data['errors'])
+                logger.error(data['errors'])
             return False, None
 
     def get_session_id(self) -> str:
         """
         Function to log in to Jablotron and retrieve the session_id which is used in the cookie
         for authentication.
         :return: session_id
```

### Comparing `JablotronPy-0.6.0/setup.py` & `jablotronpy-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="JablotronPy",
-    version="0.6.0",
+    version="0.6.1",
     author="F. de Gier",
     author_email="freddegier@me.com",
     description="A client to interact with the Jablotron API to control Jablotron alarm systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fdegier/JablotronPy",
     packages=["jablotronpy"],
```

### Comparing `JablotronPy-0.6.0/tests/test_jablotron.py` & `jablotronpy-0.6.1/tests/test_jablotron.py`

 * *Files identical despite different names*

