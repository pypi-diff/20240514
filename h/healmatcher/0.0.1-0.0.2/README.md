# Comparing `tmp/healmatcher-0.0.1.tar.gz` & `tmp/healmatcher-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healmatcher-0.0.1.tar", last modified: Tue May 14 19:05:42 2024, max compression
+gzip compressed data, was "healmatcher-0.0.2.tar", last modified: Tue May 14 19:28:16 2024, max compression
```

## Comparing `healmatcher-0.0.1.tar` & `healmatcher-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:05:42.369744 healmatcher-0.0.1/
--rw-r--r--   0 kwanbo     (501) staff       (20)      599 2024-05-14 19:05:42.369655 healmatcher-0.0.1/PKG-INFO
--rw-r--r--   0 kwanbo     (501) staff       (20)       13 2024-05-14 18:43:35.000000 healmatcher-0.0.1/README.md
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:05:42.369070 healmatcher-0.0.1/healmatcher.egg-info/
--rw-r--r--   0 kwanbo     (501) staff       (20)      599 2024-05-14 19:05:42.000000 healmatcher-0.0.1/healmatcher.egg-info/PKG-INFO
--rw-r--r--   0 kwanbo     (501) staff       (20)      207 2024-05-14 19:05:42.000000 healmatcher-0.0.1/healmatcher.egg-info/SOURCES.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-14 19:05:42.000000 healmatcher-0.0.1/healmatcher.egg-info/dependency_links.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)       20 2024-05-14 19:05:42.000000 healmatcher-0.0.1/healmatcher.egg-info/requires.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)        3 2024-05-14 19:05:42.000000 healmatcher-0.0.1/healmatcher.egg-info/top_level.txt
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:05:42.369362 healmatcher-0.0.1/hm/
--rw-r--r--   0 kwanbo     (501) staff       (20)      106 2024-05-14 18:53:41.000000 healmatcher-0.0.1/hm/__init__.py
--rw-r--r--   0 kwanbo     (501) staff       (20)       38 2024-05-14 19:05:42.369779 healmatcher-0.0.1/setup.cfg
--rw-r--r--   0 kwanbo     (501) staff       (20)     1141 2024-05-14 18:57:01.000000 healmatcher-0.0.1/setup.py
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:28:16.570137 healmatcher-0.0.2/
+-rw-r--r--   0 kwanbo     (501) staff       (20)      599 2024-05-14 19:28:16.570043 healmatcher-0.0.2/PKG-INFO
+-rw-r--r--   0 kwanbo     (501) staff       (20)       13 2024-05-14 18:43:35.000000 healmatcher-0.0.2/README.md
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:28:16.569636 healmatcher-0.0.2/healmatcher.egg-info/
+-rw-r--r--   0 kwanbo     (501) staff       (20)      599 2024-05-14 19:28:16.000000 healmatcher-0.0.2/healmatcher.egg-info/PKG-INFO
+-rw-r--r--   0 kwanbo     (501) staff       (20)      207 2024-05-14 19:28:16.000000 healmatcher-0.0.2/healmatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-14 19:28:16.000000 healmatcher-0.0.2/healmatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)       20 2024-05-14 19:28:16.000000 healmatcher-0.0.2/healmatcher.egg-info/requires.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)        3 2024-05-14 19:28:16.000000 healmatcher-0.0.2/healmatcher.egg-info/top_level.txt
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:28:16.569906 healmatcher-0.0.2/hm/
+-rw-r--r--   0 kwanbo     (501) staff       (20)      106 2024-05-14 18:53:41.000000 healmatcher-0.0.2/hm/__init__.py
+-rw-r--r--   0 kwanbo     (501) staff       (20)       38 2024-05-14 19:28:16.570179 healmatcher-0.0.2/setup.cfg
+-rw-r--r--   0 kwanbo     (501) staff       (20)     1141 2024-05-14 19:24:30.000000 healmatcher-0.0.2/setup.py
```

### Comparing `healmatcher-0.0.1/PKG-INFO` & `healmatcher-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healmatcher
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast and simple probablistic data matching package
 Author: Joseph Shim
 Author-email: <joseph.shim.rok@gmail.com>
 Keywords: probablistic match,probablistic data match,splink
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `healmatcher-0.0.1/healmatcher.egg-info/PKG-INFO` & `healmatcher-0.0.2/healmatcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healmatcher
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast and simple probablistic data matching package
 Author: Joseph Shim
 Author-email: <joseph.shim.rok@gmail.com>
 Keywords: probablistic match,probablistic data match,splink
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `healmatcher-0.0.1/setup.py` & `healmatcher-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Fast and simple probablistic data matching package'
 LONG_DESCRIPTION = 'This is a simple and fast data matching package developed by NYULH HEAL LAB'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="healmatcher",
```

