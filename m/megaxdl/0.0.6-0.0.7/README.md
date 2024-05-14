# Comparing `tmp/megaxdl-0.0.6.tar.gz` & `tmp/megaxdl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaxdl-0.0.6.tar", last modified: Tue May 14 13:54:59 2024, max compression
+gzip compressed data, was "megaxdl-0.0.7.tar", last modified: Tue May 14 15:37:10 2024, max compression
```

## Comparing `megaxdl-0.0.6.tar` & `megaxdl-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:54:59.306736 megaxdl-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 13:54:54.000000 megaxdl-0.0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:54:59.306736 megaxdl-0.0.6/Megaxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 13:54:54.000000 megaxdl-0.0.6/Megaxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 13:54:54.000000 megaxdl-0.0.6/Megaxdl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 13:54:54.000000 megaxdl-0.0.6/Megaxdl/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-14 13:54:54.000000 megaxdl-0.0.6/Megaxdl/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 13:54:59.306736 megaxdl-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 13:54:54.000000 megaxdl-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:54:59.306736 megaxdl-0.0.6/megaxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 13:54:59.000000 megaxdl-0.0.6/megaxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 13:54:59.000000 megaxdl-0.0.6/megaxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:54:59.000000 megaxdl-0.0.6/megaxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 13:54:59.000000 megaxdl-0.0.6/megaxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 13:54:59.000000 megaxdl-0.0.6/megaxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:54:59.310736 megaxdl-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 13:54:54.000000 megaxdl-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:37:10.838658 megaxdl-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 15:37:06.000000 megaxdl-0.0.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:37:10.838658 megaxdl-0.0.7/Megaxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:37:10.838658 megaxdl-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 15:37:06.000000 megaxdl-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:37:10.838658 megaxdl-0.0.7/megaxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:37:10.838658 megaxdl-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 15:37:06.000000 megaxdl-0.0.7/setup.py
```

### Comparing `megaxdl-0.0.6/LICENSE` & `megaxdl-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.6/Megaxdl/crypto.py` & `megaxdl-0.0.7/Megaxdl/crypto.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.6/Megaxdl/errors.py` & `megaxdl-0.0.7/Megaxdl/errors.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.6/PKG-INFO` & `megaxdl-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.6
+Version: 0.0.7
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.6/README.md` & `megaxdl-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.6/megaxdl.egg-info/PKG-INFO` & `megaxdl-0.0.7/megaxdl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.6
+Version: 0.0.7
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

