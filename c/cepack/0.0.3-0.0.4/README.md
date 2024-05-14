# Comparing `tmp/cepack-0.0.3.tar.gz` & `tmp/cepack-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cepack-0.0.3.tar", last modified: Tue May 14 09:14:10 2024, max compression
+gzip compressed data, was "cepack-0.0.4.tar", last modified: Tue May 14 10:32:44 2024, max compression
```

## Comparing `cepack-0.0.3.tar` & `cepack-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:10.219095 cepack-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-14 09:14:05.000000 cepack-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 09:14:05.000000 cepack-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-14 09:14:10.219095 cepack-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 09:14:05.000000 cepack-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:10.215095 cepack-0.0.3/cepack/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 09:14:05.000000 cepack-0.0.3/cepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-14 09:14:05.000000 cepack-0.0.3/cepack/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-14 09:14:05.000000 cepack-0.0.3/cepack/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:10.219095 cepack-0.0.3/cepack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-14 09:14:10.000000 cepack-0.0.3/cepack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-14 09:14:10.000000 cepack-0.0.3/cepack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:14:10.000000 cepack-0.0.3/cepack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 09:14:10.000000 cepack-0.0.3/cepack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 09:14:10.000000 cepack-0.0.3/cepack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 09:14:10.000000 cepack-0.0.3/cepack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 09:14:05.000000 cepack-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:14:10.219095 cepack-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:10.219095 cepack-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-14 09:14:05.000000 cepack-0.0.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-14 09:14:05.000000 cepack-0.0.3/test/test_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 09:14:05.000000 cepack-0.0.3/test/test_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:10.219095 cepack-0.0.3/test/utility/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 09:14:05.000000 cepack-0.0.3/test/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-14 09:14:05.000000 cepack-0.0.3/test/utility/env_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:44.624230 cepack-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-14 10:32:39.000000 cepack-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 10:32:39.000000 cepack-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    41381 2024-05-14 10:32:44.624230 cepack-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 10:32:39.000000 cepack-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:44.620230 cepack-0.0.4/cepack/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 10:32:39.000000 cepack-0.0.4/cepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-14 10:32:39.000000 cepack-0.0.4/cepack/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-14 10:32:39.000000 cepack-0.0.4/cepack/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:44.624230 cepack-0.0.4/cepack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41381 2024-05-14 10:32:44.000000 cepack-0.0.4/cepack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-14 10:32:44.000000 cepack-0.0.4/cepack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:32:44.000000 cepack-0.0.4/cepack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 10:32:44.000000 cepack-0.0.4/cepack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 10:32:44.000000 cepack-0.0.4/cepack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 10:32:44.000000 cepack-0.0.4/cepack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 10:32:39.000000 cepack-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:32:44.624230 cepack-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:44.624230 cepack-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-14 10:32:39.000000 cepack-0.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-14 10:32:39.000000 cepack-0.0.4/test/test_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 10:32:39.000000 cepack-0.0.4/test/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:44.620230 cepack-0.0.4/test/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 10:32:39.000000 cepack-0.0.4/test/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-14 10:32:39.000000 cepack-0.0.4/test/utility/env_manage.py
```

### Comparing `cepack-0.0.3/LICENSE` & `cepack-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cepack-0.0.3/cepack/main.py` & `cepack-0.0.4/cepack/main.py`

 * *Files identical despite different names*

### Comparing `cepack-0.0.3/cepack/utility.py` & `cepack-0.0.4/cepack/utility.py`

 * *Files identical despite different names*

### Comparing `cepack-0.0.3/pyproject.toml` & `cepack-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "cepack"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "paopaozhi", email = "paopaozhi@hotmail.com" }]
 dependencies = ["typer","toml","requests"]
 description = "embedded pack manage"
 readme = "README.md"
 requires-python = ">=3.9"
+license = { file = "LICENSE" }
 classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3.9",
   "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 cepack = "cepack.main:run"
 
 [build-system]
```

### Comparing `cepack-0.0.3/test/test_ci.py` & `cepack-0.0.4/test/test_ci.py`

 * *Files identical despite different names*

### Comparing `cepack-0.0.3/test/test_utility.py` & `cepack-0.0.4/test/test_utility.py`

 * *Files identical despite different names*

### Comparing `cepack-0.0.3/test/utility/env_manage.py` & `cepack-0.0.4/test/utility/env_manage.py`

 * *Files identical despite different names*

