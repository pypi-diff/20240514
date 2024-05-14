# Comparing `tmp/anemone_daisy_maker-1.55.8.tar.gz` & `tmp/anemone_daisy_maker-1.55.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.55.8.tar", last modified: Mon May 13 05:35:26 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.55.9.tar", last modified: Mon May 13 14:58:33 2024, max compression
```

## Comparing `anemone_daisy_maker-1.55.8.tar` & `anemone_daisy_maker-1.55.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 05:35:26.685852 anemone_daisy_maker-1.55.8/
--rw-r--r--   0 silbrown   (501) staff       (20)     6838 2024-05-13 05:35:26.685251 anemone_daisy_maker-1.55.8/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 05:35:26.681274 anemone_daisy_maker-1.55.8/anemone/
--rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone/__init__.py
--rw-r--r--   0 silbrown   (501) staff       (20)       33 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 05:35:26.684670 anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)     6838 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      308 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       53 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/requires.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-13 05:35:26.000000 anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-13 05:35:26.685980 anemone_daisy_maker-1.55.8/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)     1168 2024-05-12 19:16:56.000000 anemone_daisy_maker-1.55.8/setup.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 14:58:33.894920 anemone_daisy_maker-1.55.9/
+-rw-r--r--   0 silbrown   (501) staff       (20)     6838 2024-05-13 14:58:33.894419 anemone_daisy_maker-1.55.9/PKG-INFO
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 14:58:33.890592 anemone_daisy_maker-1.55.9/anemone/
+-rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone/__init__.py
+-rw-r--r--   0 silbrown   (501) staff       (20)       33 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone/__main__.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 14:58:33.893784 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/
+-rw-r--r--   0 silbrown   (501) staff       (20)     6838 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-r--r--   0 silbrown   (501) staff       (20)      308 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       53 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/requires.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/top_level.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-13 14:58:33.895054 anemone_daisy_maker-1.55.9/setup.cfg
+-rw-r--r--   0 silbrown   (501) staff       (20)     7086 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/setup.py
```

### Comparing `anemone_daisy_maker-1.55.8/PKG-INFO` & `anemone_daisy_maker-1.55.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.55.8
+Version: 1.55.9
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `anemone_daisy_maker-1.55.8/anemone/__init__.py` & `anemone_daisy_maker-1.55.9/anemone/__init__.py`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.55.8/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.55.8
+Version: 1.55.9
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

