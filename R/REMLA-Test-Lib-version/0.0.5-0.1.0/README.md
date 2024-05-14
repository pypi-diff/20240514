# Comparing `tmp/REMLA-Test-Lib-version-0.0.5.tar.gz` & `tmp/REMLA-Test-Lib-version-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REMLA-Test-Lib-version-0.0.5.tar", last modified: Tue May 14 14:51:30 2024, max compression
+gzip compressed data, was "REMLA-Test-Lib-version-0.1.0.tar", last modified: Sat May 11 14:06:13 2024, max compression
```

## Comparing `REMLA-Test-Lib-version-0.0.5.tar` & `REMLA-Test-Lib-version-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:51:30.022973 REMLA-Test-Lib-version-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 14:51:29.000000 REMLA-Test-Lib-version-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 14:51:30.022973 REMLA-Test-Lib-version-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-14 14:51:29.000000 REMLA-Test-Lib-version-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:51:30.022973 REMLA-Test-Lib-version-0.0.5/REMLA_Test_Lib_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 14:51:30.000000 REMLA-Test-Lib-version-0.0.5/REMLA_Test_Lib_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 14:51:30.000000 REMLA-Test-Lib-version-0.0.5/REMLA_Test_Lib_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:51:30.000000 REMLA-Test-Lib-version-0.0.5/REMLA_Test_Lib_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 14:51:30.000000 REMLA-Test-Lib-version-0.0.5/REMLA_Test_Lib_version.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:51:30.022973 REMLA-Test-Lib-version-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-14 14:51:29.000000 REMLA-Test-Lib-version-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:51:30.022973 REMLA-Test-Lib-version-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 14:51:29.000000 REMLA-Test-Lib-version-0.0.5/src/VersionUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 14:51:29.000000 REMLA-Test-Lib-version-0.0.5/src/VersionUtil2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:51:29.000000 REMLA-Test-Lib-version-0.0.5/src/__init__.py
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

### Comparing `REMLA-Test-Lib-version-0.0.5/LICENSE` & `REMLA-Test-Lib-version-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `REMLA-Test-Lib-version-0.0.5/PKG-INFO` & `REMLA-Test-Lib-version-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: REMLA-Test-Lib-version
-Version: 0.0.5
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

### Comparing `REMLA-Test-Lib-version-0.0.5/README.md` & `REMLA-Test-Lib-version-0.1.0/README.md`

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

### Comparing `REMLA-Test-Lib-version-0.0.5/REMLA_Test_Lib_version.egg-info/PKG-INFO` & `REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: REMLA-Test-Lib-version
-Version: 0.0.5
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

