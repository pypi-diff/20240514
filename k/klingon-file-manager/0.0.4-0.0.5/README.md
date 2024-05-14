# Comparing `tmp/klingon_file_manager-0.0.4.tar.gz` & `tmp/klingon_file_manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klingon_file_manager-0.0.4.tar", last modified: Mon Oct  9 03:18:50 2023, max compression
+gzip compressed data, was "klingon_file_manager-0.0.5.tar", last modified: Mon Oct  9 04:35:14 2023, max compression
```

## Comparing `klingon_file_manager-0.0.4.tar` & `klingon_file_manager-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 03:18:50.757853 klingon_file_manager-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-09 03:18:50.757853 klingon_file_manager-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 03:18:50.757853 klingon_file_manager-0.0.4/klingon_file_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/klingon_file_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/klingon_file_manager/klingon_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/klingon_file_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 03:18:50.757853 klingon_file_manager-0.0.4/klingon_file_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-09 03:18:50.000000 klingon_file_manager-0.0.4/klingon_file_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-10-09 03:18:50.000000 klingon_file_manager-0.0.4/klingon_file_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 03:18:50.000000 klingon_file_manager-0.0.4/klingon_file_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-09 03:18:50.000000 klingon_file_manager-0.0.4/klingon_file_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-09 03:18:50.000000 klingon_file_manager-0.0.4/klingon_file_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-09 03:18:50.000000 klingon_file_manager-0.0.4/klingon_file_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 03:18:50.757853 klingon_file_manager-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-10-09 03:18:24.000000 klingon_file_manager-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 03:18:50.757853 klingon_file_manager-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2023-10-09 03:17:52.000000 klingon_file_manager-0.0.4/tests/test_klingon_file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 04:35:14.664675 klingon_file_manager-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-09 04:35:14.664675 klingon_file_manager-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 04:35:14.664675 klingon_file_manager-0.0.5/klingon_file_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/klingon_file_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/klingon_file_manager/klingon_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/klingon_file_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 04:35:14.664675 klingon_file_manager-0.0.5/klingon_file_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-09 04:35:14.000000 klingon_file_manager-0.0.5/klingon_file_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-10-09 04:35:14.000000 klingon_file_manager-0.0.5/klingon_file_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 04:35:14.000000 klingon_file_manager-0.0.5/klingon_file_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-09 04:35:14.000000 klingon_file_manager-0.0.5/klingon_file_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-09 04:35:14.000000 klingon_file_manager-0.0.5/klingon_file_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-09 04:35:14.000000 klingon_file_manager-0.0.5/klingon_file_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 04:35:14.664675 klingon_file_manager-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-10-09 04:34:36.000000 klingon_file_manager-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 04:35:14.664675 klingon_file_manager-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2023-10-09 04:34:06.000000 klingon_file_manager-0.0.5/tests/test_klingon_file_manager.py
```

### Comparing `klingon_file_manager-0.0.4/LICENSE` & `klingon_file_manager-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `klingon_file_manager-0.0.4/PKG-INFO` & `klingon_file_manager-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klingon_file_manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python module for managing files on both local and AWS S3 storage.
 Home-page: https://github.com/djh00t/module_klingon_file_manager
 Author: David Hooton
 Author-email: klingon_file_manager+david@hooton.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `klingon_file_manager-0.0.4/klingon_file_manager/klingon_file_manager.py` & `klingon_file_manager-0.0.5/klingon_file_manager/klingon_file_manager.py`

 * *Files identical despite different names*

### Comparing `klingon_file_manager-0.0.4/klingon_file_manager/utils.py` & `klingon_file_manager-0.0.5/klingon_file_manager/utils.py`

 * *Files identical despite different names*

### Comparing `klingon_file_manager-0.0.4/klingon_file_manager.egg-info/PKG-INFO` & `klingon_file_manager-0.0.5/klingon_file_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klingon-file-manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python module for managing files on both local and AWS S3 storage.
 Home-page: https://github.com/djh00t/module_klingon_file_manager
 Author: David Hooton
 Author-email: klingon_file_manager+david@hooton.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `klingon_file_manager-0.0.4/setup.py` & `klingon_file_manager-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `klingon_file_manager-0.0.4/tests/test_klingon_file_manager.py` & `klingon_file_manager-0.0.5/tests/test_klingon_file_manager.py`

 * *Files identical despite different names*

