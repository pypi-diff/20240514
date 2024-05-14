# Comparing `tmp/BL_Python.testing-0.1.0.tar.gz` & `tmp/bl_python_testing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.testing-0.1.0.tar", last modified: Wed Feb  7 18:58:57 2024, max compression
+gzip compressed data, was "bl_python_testing-0.2.0.tar", last modified: Tue May 14 21:48:02 2024, max compression
```

## Comparing `BL_Python.testing-0.1.0.tar` & `bl_python_testing-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:57.052708 BL_Python.testing-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:57.048708 BL_Python.testing-0.1.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:57.052708 BL_Python.testing-0.1.0/BL_Python/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-07 18:58:49.000000 BL_Python.testing-0.1.0/BL_Python/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:57.052708 BL_Python.testing-0.1.0/BL_Python.testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-07 18:58:57.000000 BL_Python.testing-0.1.0/BL_Python.testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-07 18:58:57.000000 BL_Python.testing-0.1.0/BL_Python.testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:58:57.000000 BL_Python.testing-0.1.0/BL_Python.testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 18:58:57.000000 BL_Python.testing-0.1.0/BL_Python.testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-07 18:58:49.000000 BL_Python.testing-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-07 18:58:49.000000 BL_Python.testing-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-07 18:58:57.052708 BL_Python.testing-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-07 18:58:49.000000 BL_Python.testing-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:49.000000 BL_Python.testing-0.1.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-07 18:58:49.000000 BL_Python.testing-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 18:58:57.052708 BL_Python.testing-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:48:02.924745 bl_python_testing-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:48:02.920745 bl_python_testing-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:48:02.924745 bl_python_testing-0.2.0/BL_Python/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:47:59.000000 bl_python_testing-0.2.0/BL_Python/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:48:02.924745 bl_python_testing-0.2.0/BL_Python.testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-14 21:48:02.000000 bl_python_testing-0.2.0/BL_Python.testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 21:48:02.000000 bl_python_testing-0.2.0/BL_Python.testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:48:02.000000 bl_python_testing-0.2.0/BL_Python.testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 21:48:02.000000 bl_python_testing-0.2.0/BL_Python.testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:47:59.000000 bl_python_testing-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 21:47:59.000000 bl_python_testing-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-14 21:48:02.924745 bl_python_testing-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 21:47:59.000000 bl_python_testing-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:59.000000 bl_python_testing-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-14 21:47:59.000000 bl_python_testing-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:48:02.924745 bl_python_testing-0.2.0/setup.cfg
```

### Comparing `BL_Python.testing-0.1.0/BL_Python.testing.egg-info/PKG-INFO` & `bl_python_testing-0.2.0/BL_Python.testing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.testing
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries used to aid in automated testing.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.testing-0.1.0/LICENSE.md` & `bl_python_testing-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.testing-0.1.0/PKG-INFO` & `bl_python_testing-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.testing
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries used to aid in automated testing.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.testing-0.1.0/pyproject.toml` & `bl_python_testing-0.2.0/pyproject.toml`

 * *Files identical despite different names*

