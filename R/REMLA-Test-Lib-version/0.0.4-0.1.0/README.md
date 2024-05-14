# Comparing `tmp/REMLA-Test-Lib-version-0.0.4.tar.gz` & `tmp/REMLA-Test-Lib-version-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REMLA-Test-Lib-version-0.0.4.tar", last modified: Tue May 14 14:09:20 2024, max compression
+gzip compressed data, was "REMLA-Test-Lib-version-0.1.0.tar", last modified: Sat May 11 14:06:13 2024, max compression
```

## Comparing `REMLA-Test-Lib-version-0.0.4.tar` & `REMLA-Test-Lib-version-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:09:20.138642 REMLA-Test-Lib-version-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 14:09:19.000000 REMLA-Test-Lib-version-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 14:09:20.138642 REMLA-Test-Lib-version-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-14 14:09:19.000000 REMLA-Test-Lib-version-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:09:20.138642 REMLA-Test-Lib-version-0.0.4/REMLA_Test_Lib_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 14:09:20.000000 REMLA-Test-Lib-version-0.0.4/REMLA_Test_Lib_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-14 14:09:20.000000 REMLA-Test-Lib-version-0.0.4/REMLA_Test_Lib_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:09:20.000000 REMLA-Test-Lib-version-0.0.4/REMLA_Test_Lib_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 14:09:20.000000 REMLA-Test-Lib-version-0.0.4/REMLA_Test_Lib_version.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:09:20.138642 REMLA-Test-Lib-version-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-14 14:09:19.000000 REMLA-Test-Lib-version-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:09:20.138642 REMLA-Test-Lib-version-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-14 14:09:19.000000 REMLA-Test-Lib-version-0.0.4/src/VersionUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:09:19.000000 REMLA-Test-Lib-version-0.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-11 14:06:12.000000 REMLA-Test-Lib-version-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-11 14:06:12.000000 REMLA-Test-Lib-version-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 14:06:12.000000 REMLA-Test-Lib-version-0.1.0/setup.py
```

### Comparing `REMLA-Test-Lib-version-0.0.4/LICENSE` & `REMLA-Test-Lib-version-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `REMLA-Test-Lib-version-0.0.4/PKG-INFO` & `REMLA-Test-Lib-version-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: REMLA-Test-Lib-version
-Version: 0.0.4
+Version: 0.1.0
 Summary: A version-aware library designed to provide robust version management and utility functions
 Home-page: UNKNOWN
 Author: Nick Dubbeldam
 Author-email: nick.dubbeldasm@live.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LIB-VERSION
+\n# LIB-VERSION
 
 LIB-VERSION is a version-aware library designed to provide robust version management and utility functions. This library is ideal for projects requiring precise version tracking, such as in detailed logging or system monitoring environments.
 
 ## Features
 
 - **Version Retrieval**: Easily retrieve the current library version using the `VersionUtil` class.
 - **Automatic Versioning**: Utilizes Git tags to automatically version the library.
@@ -26,24 +26,25 @@
 
 ## Getting Started
 
 ### Prerequisites
 
 - Git (for versioning)
 - Python 3.x (if using Python)
-- Access to a package registry pip
+- Access to a package registry (e.g., PyPI, npm)
 
 ### Installation
 
 To install Library Name, use the following command:
 
 ```bash
-pip install REMLA-Test-Lib-version
+pip install lib-version
 ```
 
+Replace pip with the package manager relevant to your programming language or environment.
 
 ### Usage
 To retrieve the current version of the library:
 
 ```python
 from version_util import VersionUtil
 print(VersionUtil.get_version())
```

### Comparing `REMLA-Test-Lib-version-0.0.4/README.md` & `REMLA-Test-Lib-version-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 
 ## Getting Started
 
 ### Prerequisites
 
 - Git (for versioning)
 - Python 3.x (if using Python)
-- Access to a package registry pip
+- Access to a package registry (e.g., PyPI, npm)
 
 ### Installation
 
 To install Library Name, use the following command:
 
 ```bash
-pip install REMLA-Test-Lib-version
+pip install lib-version
 ```
 
+Replace pip with the package manager relevant to your programming language or environment.
 
 ### Usage
 To retrieve the current version of the library:
 
 ```python
 from version_util import VersionUtil
 print(VersionUtil.get_version())
```

### Comparing `REMLA-Test-Lib-version-0.0.4/REMLA_Test_Lib_version.egg-info/PKG-INFO` & `REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: REMLA-Test-Lib-version
-Version: 0.0.4
+Version: 0.1.0
 Summary: A version-aware library designed to provide robust version management and utility functions
 Home-page: UNKNOWN
 Author: Nick Dubbeldam
 Author-email: nick.dubbeldasm@live.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LIB-VERSION
+\n# LIB-VERSION
 
 LIB-VERSION is a version-aware library designed to provide robust version management and utility functions. This library is ideal for projects requiring precise version tracking, such as in detailed logging or system monitoring environments.
 
 ## Features
 
 - **Version Retrieval**: Easily retrieve the current library version using the `VersionUtil` class.
 - **Automatic Versioning**: Utilizes Git tags to automatically version the library.
@@ -26,24 +26,25 @@
 
 ## Getting Started
 
 ### Prerequisites
 
 - Git (for versioning)
 - Python 3.x (if using Python)
-- Access to a package registry pip
+- Access to a package registry (e.g., PyPI, npm)
 
 ### Installation
 
 To install Library Name, use the following command:
 
 ```bash
-pip install REMLA-Test-Lib-version
+pip install lib-version
 ```
 
+Replace pip with the package manager relevant to your programming language or environment.
 
 ### Usage
 To retrieve the current version of the library:
 
 ```python
 from version_util import VersionUtil
 print(VersionUtil.get_version())
```

### Comparing `REMLA-Test-Lib-version-0.0.4/setup.py` & `REMLA-Test-Lib-version-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 
 # Read version from the VERSION file
-with open('src/VERSION', 'r') as version_file:
+with open('VERSION', 'r') as version_file:
     version = version_file.read().strip()
 
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    # long_description = "\\n" + fh.read()
-    long_description = fh.read()
+    long_description = "\\n" + fh.read()
 
 setup(
 name='REMLA-Test-Lib-version',
 version=version,
 author='Nick Dubbeldam',
 author_email='nick.dubbeldasm@live.nl',
 description='A version-aware library designed to provide robust version management and utility functions',
```

