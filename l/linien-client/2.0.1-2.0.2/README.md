# Comparing `tmp/linien_client-2.0.1.tar.gz` & `tmp/linien_client-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien_client-2.0.1.tar", last modified: Mon May 13 15:18:08 2024, max compression
+gzip compressed data, was "linien_client-2.0.2.tar", last modified: Tue May 14 13:14:42 2024, max compression
```

## Comparing `linien_client-2.0.1.tar` & `linien_client-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:07.997424 linien_client-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-13 15:18:07.997424 linien_client-2.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:07.997424 linien_client-2.0.1/linien_client/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 15:17:51.000000 linien_client-2.0.1/linien_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-13 15:17:51.000000 linien_client-2.0.1/linien_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-13 15:17:51.000000 linien_client-2.0.1/linien_client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-13 15:17:51.000000 linien_client-2.0.1/linien_client/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-13 15:17:51.000000 linien_client-2.0.1/linien_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-05-13 15:17:51.000000 linien_client-2.0.1/linien_client/remote_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:07.997424 linien_client-2.0.1/linien_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-13 15:18:07.000000 linien_client-2.0.1/linien_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-13 15:18:07.000000 linien_client-2.0.1/linien_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:18:07.000000 linien_client-2.0.1/linien_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 15:18:07.000000 linien_client-2.0.1/linien_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 15:18:07.000000 linien_client-2.0.1/linien_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-13 15:17:51.000000 linien_client-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:18:07.997424 linien_client-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:14:42.822848 linien_client-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-14 13:14:42.822848 linien_client-2.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:14:42.818848 linien_client-2.0.2/linien_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-14 13:14:26.000000 linien_client-2.0.2/linien_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-14 13:14:26.000000 linien_client-2.0.2/linien_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-14 13:14:26.000000 linien_client-2.0.2/linien_client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-14 13:14:26.000000 linien_client-2.0.2/linien_client/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-14 13:14:26.000000 linien_client-2.0.2/linien_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-05-14 13:14:26.000000 linien_client-2.0.2/linien_client/remote_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:14:42.822848 linien_client-2.0.2/linien_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-14 13:14:42.000000 linien_client-2.0.2/linien_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 13:14:42.000000 linien_client-2.0.2/linien_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:14:42.000000 linien_client-2.0.2/linien_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 13:14:42.000000 linien_client-2.0.2/linien_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 13:14:42.000000 linien_client-2.0.2/linien_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-14 13:14:26.000000 linien_client-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:14:42.822848 linien_client-2.0.2/setup.cfg
```

### Comparing `linien_client-2.0.1/PKG-INFO` & `linien_client-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 2.0.1
+Version: 2.0.2
 Summary: Client components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fabric<3.0,>=2.7.0
 Requires-Dist: typing_extensions<5.0,>=4.5.0
-Requires-Dist: linien-common==2.0.1
+Requires-Dist: linien-common==2.0.2
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien_client-2.0.1/linien_client/__init__.py` & `linien_client-2.0.2/linien_client/__init__.py`

 * *Files identical despite different names*

### Comparing `linien_client-2.0.1/linien_client/connection.py` & `linien_client-2.0.2/linien_client/connection.py`

 * *Files identical despite different names*

### Comparing `linien_client-2.0.1/linien_client/deploy.py` & `linien_client-2.0.2/linien_client/deploy.py`

 * *Files identical despite different names*

### Comparing `linien_client-2.0.1/linien_client/device.py` & `linien_client-2.0.2/linien_client/device.py`

 * *Files identical despite different names*

### Comparing `linien_client-2.0.1/linien_client/exceptions.py` & `linien_client-2.0.2/linien_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `linien_client-2.0.1/linien_client/remote_parameters.py` & `linien_client-2.0.2/linien_client/remote_parameters.py`

 * *Files identical despite different names*

### Comparing `linien_client-2.0.1/linien_client.egg-info/PKG-INFO` & `linien_client-2.0.2/linien_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 2.0.1
+Version: 2.0.2
 Summary: Client components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fabric<3.0,>=2.7.0
 Requires-Dist: typing_extensions<5.0,>=4.5.0
-Requires-Dist: linien-common==2.0.1
+Requires-Dist: linien-common==2.0.2
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien_client-2.0.1/pyproject.toml` & `linien_client-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linien-client"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
     { name = "Benjamin Wiegand", email = "benjamin.wiegand@physik.hu-berlin.de" },
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
     { name = "Robert Jördens", email = "rj@quartiq.de" },
     { name = "Christian Freier", email = "christian.freier@gmail.com" },
     { name = "Doron Behar", email = "doron.behar@gmail.com" },
 ]
@@ -21,15 +21,15 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "fabric>=2.7.0,<3.0",
     "typing_extensions>=4.5.0,<5.0",
-    "linien-common==2.0.1",
+    "linien-common==2.0.2",
 ]
 
 [project.readme]
 text = "Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions."
 content-type = "text/markdown"
 
 [project.urls]
```
