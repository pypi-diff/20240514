# Comparing `tmp/flyflowclient-1.14.4.tar.gz` & `tmp/flyflowclient-1.14.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyflowclient-1.14.4.tar", last modified: Sun May 12 23:53:58 2024, max compression
+gzip compressed data, was "flyflowclient-1.14.6.tar", last modified: Mon May 13 00:57:34 2024, max compression
```

## Comparing `flyflowclient-1.14.4.tar` & `flyflowclient-1.14.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:53:58.022524 flyflowclient-1.14.4/
--rw-r--r--   0 carlcortright   (501) staff       (20)    11357 2024-05-12 23:23:34.000000 flyflowclient-1.14.4/LICENSE
--rw-r--r--   0 carlcortright   (501) staff       (20)     3825 2024-05-12 23:53:58.022318 flyflowclient-1.14.4/PKG-INFO
--rw-r--r--   0 carlcortright   (501) staff       (20)     3367 2024-05-12 23:53:44.000000 flyflowclient-1.14.4/README.md
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:53:58.021150 flyflowclient-1.14.4/flyflowclient/
--rw-r--r--   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:29:28.000000 flyflowclient-1.14.4/flyflowclient/__init__.py
--rw-r--r--   0 carlcortright   (501) staff       (20)     3647 2024-05-12 23:45:58.000000 flyflowclient-1.14.4/flyflowclient/client.py
-drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:53:58.022035 flyflowclient-1.14.4/flyflowclient.egg-info/
--rw-r--r--   0 carlcortright   (501) staff       (20)     3825 2024-05-12 23:53:57.000000 flyflowclient-1.14.4/flyflowclient.egg-info/PKG-INFO
--rw-r--r--   0 carlcortright   (501) staff       (20)      260 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/SOURCES.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)        1 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/dependency_links.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       17 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/requires.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       14 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/top_level.txt
--rw-r--r--   0 carlcortright   (501) staff       (20)       38 2024-05-12 23:53:58.022572 flyflowclient-1.14.4/setup.cfg
--rw-r--r--   0 carlcortright   (501) staff       (20)      634 2024-05-12 23:53:54.000000 flyflowclient-1.14.4/setup.py
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-13 00:57:34.774289 flyflowclient-1.14.6/
+-rw-r--r--   0 carlcortright   (501) staff       (20)    11357 2024-05-12 23:23:34.000000 flyflowclient-1.14.6/LICENSE
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3824 2024-05-13 00:57:34.774098 flyflowclient-1.14.6/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3366 2024-05-12 23:58:02.000000 flyflowclient-1.14.6/README.md
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-13 00:57:34.773056 flyflowclient-1.14.6/flyflowclient/
+-rw-r--r--   0 carlcortright   (501) staff       (20)       27 2024-05-13 00:56:24.000000 flyflowclient-1.14.6/flyflowclient/__init__.py
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3647 2024-05-12 23:45:58.000000 flyflowclient-1.14.6/flyflowclient/client.py
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-13 00:57:34.773898 flyflowclient-1.14.6/flyflowclient.egg-info/
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3824 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)      260 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/SOURCES.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)        1 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/dependency_links.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       17 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/requires.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       14 2024-05-13 00:57:34.000000 flyflowclient-1.14.6/flyflowclient.egg-info/top_level.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       38 2024-05-13 00:57:34.774348 flyflowclient-1.14.6/setup.cfg
+-rw-r--r--   0 carlcortright   (501) staff       (20)      634 2024-05-13 00:57:32.000000 flyflowclient-1.14.6/setup.py
```

### Comparing `flyflowclient-1.14.4/LICENSE` & `flyflowclient-1.14.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flyflowclient-1.14.4/PKG-INFO` & `flyflowclient-1.14.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyflowclient
-Version: 1.14.4
+Version: 1.14.6
 Summary: A client library for the FlyFlow API
 Home-page: https://github.com/flyflow-devs/flyflow-python
 Author: Carl Cortright
 Author-email: carl@flyflow.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Flyflow is a Python client library for interacting with the Flyflow API. It provides a simple and intuitive interface to manage agents, calls, and perform various operations related to the Flyflow platform.
 
 ## Installation
 
 You can install the Flyflow package using pip:
 
 ```
-pip install flyflow-client
+pip install flyflowclient
 ```
 
 ## Usage
 
 To use the Flyflow client library, you need to import the `Flyflow` class from the `flyflow.client` module:
 
 ```python
```

### Comparing `flyflowclient-1.14.4/README.md` & `flyflowclient-1.14.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Flyflow is a Python client library for interacting with the Flyflow API. It provides a simple and intuitive interface to manage agents, calls, and perform various operations related to the Flyflow platform.
 
 ## Installation
 
 You can install the Flyflow package using pip:
 
 ```
-pip install flyflow-client
+pip install flyflowclient
 ```
 
 ## Usage
 
 To use the Flyflow client library, you need to import the `Flyflow` class from the `flyflow.client` module:
 
 ```python
```

### Comparing `flyflowclient-1.14.4/flyflowclient/client.py` & `flyflowclient-1.14.6/flyflowclient/client.py`

 * *Files identical despite different names*

### Comparing `flyflowclient-1.14.4/flyflowclient.egg-info/PKG-INFO` & `flyflowclient-1.14.6/flyflowclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyflowclient
-Version: 1.14.4
+Version: 1.14.6
 Summary: A client library for the FlyFlow API
 Home-page: https://github.com/flyflow-devs/flyflow-python
 Author: Carl Cortright
 Author-email: carl@flyflow.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Flyflow is a Python client library for interacting with the Flyflow API. It provides a simple and intuitive interface to manage agents, calls, and perform various operations related to the Flyflow platform.
 
 ## Installation
 
 You can install the Flyflow package using pip:
 
 ```
-pip install flyflow-client
+pip install flyflowclient
 ```
 
 ## Usage
 
 To use the Flyflow client library, you need to import the `Flyflow` class from the `flyflow.client` module:
 
 ```python
```

### Comparing `flyflowclient-1.14.4/setup.py` & `flyflowclient-1.14.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="flyflowclient",
-    version="1.14.4",
+    version="1.14.6",
     packages=find_packages(),
     install_requires=[
         "requests>=2.25.1"
     ],
     author="Carl Cortright",
     author_email="carl@flyflow.dev",
     description="A client library for the FlyFlow API",
```

