# Comparing `tmp/wrapworks-1.0.0.tar.gz` & `tmp/wrapworks-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapworks-1.0.0.tar", last modified: Sun May 12 14:21:20 2024, max compression
+gzip compressed data, was "wrapworks-1.0.1.tar", last modified: Tue May 14 06:51:14 2024, max compression
```

## Comparing `wrapworks-1.0.0.tar` & `wrapworks-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:21:20.238517 wrapworks-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-12 14:21:20.234517 wrapworks-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-12 14:21:15.000000 wrapworks-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-12 14:21:15.000000 wrapworks-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:21:20.238517 wrapworks-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:21:20.234517 wrapworks-1.0.0/wrapworks/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-12 14:21:15.000000 wrapworks-1.0.0/wrapworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 14:21:15.000000 wrapworks-1.0.0/wrapworks/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 14:21:15.000000 wrapworks-1.0.0/wrapworks/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:21:20.234517 wrapworks-1.0.0/wrapworks/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:21:15.000000 wrapworks-1.0.0/wrapworks/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-12 14:21:15.000000 wrapworks-1.0.0/wrapworks/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-12 14:21:15.000000 wrapworks-1.0.0/wrapworks/tests/test_wraps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-12 14:21:15.000000 wrapworks-1.0.0/wrapworks/wraps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:21:20.234517 wrapworks-1.0.0/wrapworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-12 14:21:20.000000 wrapworks-1.0.0/wrapworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-12 14:21:20.000000 wrapworks-1.0.0/wrapworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:21:20.000000 wrapworks-1.0.0/wrapworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-12 14:21:20.000000 wrapworks-1.0.0/wrapworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 14:21:20.000000 wrapworks-1.0.0/wrapworks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:14.610724 wrapworks-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 06:51:14.610724 wrapworks-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-14 06:51:10.000000 wrapworks-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 06:51:10.000000 wrapworks-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:51:14.610724 wrapworks-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:14.606724 wrapworks-1.0.1/wrapworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 06:51:10.000000 wrapworks-1.0.1/wrapworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 06:51:10.000000 wrapworks-1.0.1/wrapworks/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 06:51:10.000000 wrapworks-1.0.1/wrapworks/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:14.610724 wrapworks-1.0.1/wrapworks/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:10.000000 wrapworks-1.0.1/wrapworks/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-14 06:51:10.000000 wrapworks-1.0.1/wrapworks/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-14 06:51:10.000000 wrapworks-1.0.1/wrapworks/tests/test_wraps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-14 06:51:10.000000 wrapworks-1.0.1/wrapworks/wraps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:14.610724 wrapworks-1.0.1/wrapworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 06:51:14.000000 wrapworks-1.0.1/wrapworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-14 06:51:14.000000 wrapworks-1.0.1/wrapworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:51:14.000000 wrapworks-1.0.1/wrapworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 06:51:14.000000 wrapworks-1.0.1/wrapworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 06:51:14.000000 wrapworks-1.0.1/wrapworks.egg-info/top_level.txt
```

### Comparing `wrapworks-1.0.0/PKG-INFO` & `wrapworks-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapworks
-Version: 1.0.0
+Version: 1.0.1
 Summary: Decorators for Developers
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/wrapworks
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -74,15 +74,15 @@
 ```python
 from wrapworks import eprint
 
 def some_function():
     try:
         raise ValueError()
     except Exception as e:
-        eprint(e , some_func)
+        eprint(e , some_function)
 
 ```
 
 ### Add current directory to system path and load environment variables
 
 ```python
 from wrapworks import cwdtoenv
```

### Comparing `wrapworks-1.0.0/README.md` & `wrapworks-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ```python
 from wrapworks import eprint
 
 def some_function():
     try:
         raise ValueError()
     except Exception as e:
-        eprint(e , some_func)
+        eprint(e , some_function)
 
 ```
 
 ### Add current directory to system path and load environment variables
 
 ```python
 from wrapworks import cwdtoenv
```

### Comparing `wrapworks-1.0.0/pyproject.toml` & `wrapworks-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools >= 61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 dependencies = ["python-dotenv>=0.5.0", "rich>=11.0.0"]
 name = "wrapworks"
-version = "1.0.0"
+version = "1.0.1"
 description = "Decorators for Developers"
 readme = "README.md"
 requires-python = ">= 3.10"
 authors = [{ name = "Asaniczka", email = "asaniczka@gmail.com" }]
 maintainers = [{ name = "Asaniczka", email = "asaniczka@gmail.com" }]
 license = { text = "Apache-2.0" }
 classifiers = [
```

### Comparing `wrapworks-1.0.0/wrapworks/tests/test_error_handling.py` & `wrapworks-1.0.1/wrapworks/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `wrapworks-1.0.0/wrapworks/tests/test_wraps.py` & `wrapworks-1.0.1/wrapworks/tests/test_wraps.py`

 * *Files identical despite different names*

### Comparing `wrapworks-1.0.0/wrapworks/wraps.py` & `wrapworks-1.0.1/wrapworks/wraps.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def timeit(level: int = 1):
     """
     Prints the execution duration of the function.
 
     This is a decorator factory
 
     ## Args:
-    `level`: An arbitary int assigned to the wrapper. Use this combined with `WRAPWORKSLEVEL` env to control whether this wrapper uses print
+    - `level`: An arbitary int assigned to the wrapper. Use this combined with `WRAPWORKSLEVEL` env to control whether this wrapper uses print
     """
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             start_time = time.perf_counter()
             try:
@@ -42,16 +42,16 @@
 def tryexcept(default_return: Any = None, level: int = 1):
     """
     Adds a try except block around the function saving to a bunch of keystrokes.
 
     This is a decorator factory.
 
     ## Args:
-    `default_return`: What to return when the function fails
-    `level`: An arbitary int assigned to the wrapper. Use this combined with `WRAPWORKSLEVEL` env to control whether this wrapper uses print
+    - `default_return`: What to return when the function fails
+    - `level`: An arbitary int assigned to the wrapper. Use this combined with `WRAPWORKSLEVEL` env to control whether this wrapper uses print
     """
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 result = func(*args, **kwargs)
@@ -69,18 +69,18 @@
 def retry(max_retries=5, delay=1, default_return: Any = None, level=1):
     """
     Automatically retry the function.
 
     This is a decorator factory.
 
     ## Args:
-    `max_retries`: Maximum number of retires
-    `delay`: Delay in seconds between retries
-    `default_return`: What to return when the function fails
-    `level`: An arbitary int assigned to the wrapper. Use this combined with `WRAPWORKSLEVEL` env to control whether this wrapper uses print
+    - `max_retries`: Maximum number of retires
+    - `delay`: Delay in seconds between retries
+    - `default_return`: What to return when the function fails
+    - `level`: An arbitary int assigned to the wrapper. Use this combined with `WRAPWORKSLEVEL` env to control whether this wrapper uses print
     """
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             retries = 0
             while retries < max_retries:
```

### Comparing `wrapworks-1.0.0/wrapworks.egg-info/PKG-INFO` & `wrapworks-1.0.1/wrapworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapworks
-Version: 1.0.0
+Version: 1.0.1
 Summary: Decorators for Developers
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/wrapworks
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -74,15 +74,15 @@
 ```python
 from wrapworks import eprint
 
 def some_function():
     try:
         raise ValueError()
     except Exception as e:
-        eprint(e , some_func)
+        eprint(e , some_function)
 
 ```
 
 ### Add current directory to system path and load environment variables
 
 ```python
 from wrapworks import cwdtoenv
```

