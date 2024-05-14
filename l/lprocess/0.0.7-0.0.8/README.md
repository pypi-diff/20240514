# Comparing `tmp/lprocess-0.0.7.tar.gz` & `tmp/lprocess-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lprocess-0.0.7.tar", last modified: Mon May 13 15:45:12 2024, max compression
+gzip compressed data, was "lprocess-0.0.8.tar", last modified: Tue May 14 17:41:17 2024, max compression
```

## Comparing `lprocess-0.0.7.tar` & `lprocess-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-13 15:45:12.792983 lprocess-0.0.7/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-13 15:45:12.792983 lprocess-0.0.7/PKG-INFO
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-13 15:45:12.792983 lprocess-0.0.7/lprocess/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)     2114 2024-05-13 15:37:37.000000 lprocess-0.0.7/lprocess/EDA.py
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       21 2024-05-11 11:47:06.000000 lprocess-0.0.7/lprocess/__init__.py
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-13 15:45:12.792983 lprocess-0.0.7/lprocess.egg-info/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/PKG-INFO
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      204 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/requires.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/top_level.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-13 15:45:12.792983 lprocess-0.0.7/setup.cfg
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-13 15:44:38.000000 lprocess-0.0.7/setup.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-14 17:41:17.943553 lprocess-0.0.8/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-14 17:41:17.943553 lprocess-0.0.8/PKG-INFO
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-14 17:41:17.943553 lprocess-0.0.8/lprocess/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)     5630 2024-05-14 17:40:52.000000 lprocess-0.0.8/lprocess/EDA.py
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       21 2024-05-11 11:47:06.000000 lprocess-0.0.8/lprocess/__init__.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-14 17:41:17.943553 lprocess-0.0.8/lprocess.egg-info/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      204 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/requires.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/top_level.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-14 17:41:17.943553 lprocess-0.0.8/setup.cfg
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-14 17:41:01.000000 lprocess-0.0.8/setup.py
```

### Comparing `lprocess-0.0.7/setup.py` & `lprocess-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Data Preprocessing library'
 
 
 # Setting up
 setup(
     name="lprocess",
     version=VERSION,
```

