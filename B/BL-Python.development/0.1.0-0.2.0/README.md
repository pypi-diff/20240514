# Comparing `tmp/BL_Python.development-0.1.0.tar.gz` & `tmp/bl_python_development-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.development-0.1.0.tar", last modified: Wed Feb  7 18:58:52 2024, max compression
+gzip compressed data, was "bl_python_development-0.2.0.tar", last modified: Tue May 14 21:44:37 2024, max compression
```

## Comparing `BL_Python.development-0.1.0.tar` & `bl_python_development-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.261444 BL_Python.development-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.257444 BL_Python.development-0.1.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.261444 BL_Python.development-0.1.0/BL_Python/development/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-07 18:58:39.000000 BL_Python.development-0.1.0/BL_Python/development/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-07 18:58:39.000000 BL_Python.development-0.1.0/BL_Python/development/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.261444 BL_Python.development-0.1.0/BL_Python.development.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-07 18:58:52.000000 BL_Python.development-0.1.0/BL_Python.development.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-07 18:58:52.000000 BL_Python.development-0.1.0/BL_Python.development.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:58:52.000000 BL_Python.development-0.1.0/BL_Python.development.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 18:58:52.000000 BL_Python.development-0.1.0/BL_Python.development.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-07 18:58:39.000000 BL_Python.development-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-07 18:58:39.000000 BL_Python.development-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-07 18:58:52.261444 BL_Python.development-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-07 18:58:39.000000 BL_Python.development-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:39.000000 BL_Python.development-0.1.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-07 18:58:39.000000 BL_Python.development-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 18:58:52.261444 BL_Python.development-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:44:37.923889 bl_python_development-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:44:37.919890 bl_python_development-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:44:37.923889 bl_python_development-0.2.0/BL_Python/development/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 21:44:34.000000 bl_python_development-0.2.0/BL_Python/development/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-14 21:44:34.000000 bl_python_development-0.2.0/BL_Python/development/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:44:37.923889 bl_python_development-0.2.0/BL_Python.development.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-14 21:44:37.000000 bl_python_development-0.2.0/BL_Python.development.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-14 21:44:37.000000 bl_python_development-0.2.0/BL_Python.development.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:44:37.000000 bl_python_development-0.2.0/BL_Python.development.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 21:44:37.000000 bl_python_development-0.2.0/BL_Python.development.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:44:34.000000 bl_python_development-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 21:44:34.000000 bl_python_development-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-14 21:44:37.923889 bl_python_development-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 21:44:34.000000 bl_python_development-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:44:34.000000 bl_python_development-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-14 21:44:34.000000 bl_python_development-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:44:37.923889 bl_python_development-0.2.0/setup.cfg
```

### Comparing `BL_Python.development-0.1.0/BL_Python/development/profiling.py` & `bl_python_development-0.2.0/BL_Python/development/profiling.py`

 * *Files identical despite different names*

### Comparing `BL_Python.development-0.1.0/BL_Python.development.egg-info/PKG-INFO` & `bl_python_development-0.2.0/BL_Python.development.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.development
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utilities and tools for assisting in development of software.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.development-0.1.0/LICENSE.md` & `bl_python_development-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.development-0.1.0/PKG-INFO` & `bl_python_development-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.development
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utilities and tools for assisting in development of software.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.development-0.1.0/pyproject.toml` & `bl_python_development-0.2.0/pyproject.toml`

 * *Files identical despite different names*

