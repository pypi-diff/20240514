# Comparing `tmp/saes6-jerry-0.0.7.tar.gz` & `tmp/saes6-jerry-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saes6-jerry-0.0.7.tar", last modified: Tue May 14 09:31:51 2024, max compression
+gzip compressed data, was "saes6-jerry-0.0.8.tar", last modified: Tue May 14 09:32:50 2024, max compression
```

## Comparing `saes6-jerry-0.0.7.tar` & `saes6-jerry-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:31:51.406173 saes6-jerry-0.0.7/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:31:51.405975 saes6-jerry-0.0.7/PKG-INFO
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:31:51.405023 saes6-jerry-0.0.7/jerry/
--rw-r--r--   0 gonzales   (501) staff       (20)       50 2024-05-14 09:31:13.000000 saes6-jerry-0.0.7/jerry/__init__.py
--rw-r--r--   0 gonzales   (501) staff       (20)       98 2024-05-14 09:26:55.000000 saes6-jerry-0.0.7/jerry/main.py
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:31:51.405791 saes6-jerry-0.0.7/saes6_jerry.egg-info/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:31:51.000000 saes6-jerry-0.0.7/saes6_jerry.egg-info/PKG-INFO
--rw-r--r--   0 gonzales   (501) staff       (20)      218 2024-05-14 09:31:51.000000 saes6-jerry-0.0.7/saes6_jerry.egg-info/SOURCES.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-14 09:31:51.000000 saes6-jerry-0.0.7/saes6_jerry.egg-info/dependency_links.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       43 2024-05-14 09:31:51.000000 saes6-jerry-0.0.7/saes6_jerry.egg-info/entry_points.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-14 09:31:51.000000 saes6-jerry-0.0.7/saes6_jerry.egg-info/top_level.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 09:31:51.406216 saes6-jerry-0.0.7/setup.cfg
--rw-r--r--   0 gonzales   (501) staff       (20)      657 2024-05-14 09:31:35.000000 saes6-jerry-0.0.7/setup.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:32:50.925967 saes6-jerry-0.0.8/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:32:50.925728 saes6-jerry-0.0.8/PKG-INFO
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:32:50.924590 saes6-jerry-0.0.8/jerry/
+-rw-r--r--   0 gonzales   (501) staff       (20)       45 2024-05-14 09:32:48.000000 saes6-jerry-0.0.8/jerry/__init__.py
+-rw-r--r--   0 gonzales   (501) staff       (20)       98 2024-05-14 09:26:55.000000 saes6-jerry-0.0.8/jerry/main.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:32:50.925508 saes6-jerry-0.0.8/saes6_jerry.egg-info/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:32:50.000000 saes6-jerry-0.0.8/saes6_jerry.egg-info/PKG-INFO
+-rw-r--r--   0 gonzales   (501) staff       (20)      218 2024-05-14 09:32:50.000000 saes6-jerry-0.0.8/saes6_jerry.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-14 09:32:50.000000 saes6-jerry-0.0.8/saes6_jerry.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       43 2024-05-14 09:32:50.000000 saes6-jerry-0.0.8/saes6_jerry.egg-info/entry_points.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-14 09:32:50.000000 saes6-jerry-0.0.8/saes6_jerry.egg-info/top_level.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 09:32:50.926012 saes6-jerry-0.0.8/setup.cfg
+-rw-r--r--   0 gonzales   (501) staff       (20)      657 2024-05-14 09:31:35.000000 saes6-jerry-0.0.8/setup.py
```

### Comparing `saes6-jerry-0.0.7/setup.py` & `saes6-jerry-0.0.8/setup.py`

 * *Files identical despite different names*

