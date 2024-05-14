# Comparing `tmp/saes6-jerry-0.0.1.tar.gz` & `tmp/saes6-jerry-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saes6-jerry-0.0.1.tar", last modified: Tue May 14 08:22:15 2024, max compression
+gzip compressed data, was "saes6-jerry-0.0.2.tar", last modified: Tue May 14 09:06:36 2024, max compression
```

## Comparing `saes6-jerry-0.0.1.tar` & `saes6-jerry-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 08:22:15.334471 saes6-jerry-0.0.1/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 08:22:15.334258 saes6-jerry-0.0.1/PKG-INFO
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 08:22:15.333019 saes6-jerry-0.0.1/jerry/
--rw-r--r--   0 gonzales   (501) staff       (20)       85 2024-05-14 08:14:15.000000 saes6-jerry-0.0.1/jerry/__init__.py
--rw-r--r--   0 gonzales   (501) staff       (20)      422 2024-05-14 08:06:03.000000 saes6-jerry-0.0.1/jerry/default.py
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 08:22:15.334043 saes6-jerry-0.0.1/saes6_jerry.egg-info/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 08:22:15.000000 saes6-jerry-0.0.1/saes6_jerry.egg-info/PKG-INFO
--rw-r--r--   0 gonzales   (501) staff       (20)      221 2024-05-14 08:22:15.000000 saes6-jerry-0.0.1/saes6_jerry.egg-info/SOURCES.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-14 08:22:15.000000 saes6-jerry-0.0.1/saes6_jerry.egg-info/dependency_links.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 08:22:15.000000 saes6-jerry-0.0.1/saes6_jerry.egg-info/entry_points.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-14 08:22:15.000000 saes6-jerry-0.0.1/saes6_jerry.egg-info/top_level.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 08:22:15.334520 saes6-jerry-0.0.1/setup.cfg
--rw-r--r--   0 gonzales   (501) staff       (20)      652 2024-05-14 08:22:07.000000 saes6-jerry-0.0.1/setup.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:06:36.393312 saes6-jerry-0.0.2/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:06:36.393062 saes6-jerry-0.0.2/PKG-INFO
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:06:36.391857 saes6-jerry-0.0.2/jerry/
+-rw-r--r--   0 gonzales   (501) staff       (20)       85 2024-05-14 09:06:25.000000 saes6-jerry-0.0.2/jerry/__init__.py
+-rw-r--r--   0 gonzales   (501) staff       (20)      136 2024-05-14 09:05:06.000000 saes6-jerry-0.0.2/jerry/default.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:06:36.392820 saes6-jerry-0.0.2/saes6_jerry.egg-info/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:06:36.000000 saes6-jerry-0.0.2/saes6_jerry.egg-info/PKG-INFO
+-rw-r--r--   0 gonzales   (501) staff       (20)      221 2024-05-14 09:06:36.000000 saes6-jerry-0.0.2/saes6_jerry.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-14 09:06:36.000000 saes6-jerry-0.0.2/saes6_jerry.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 09:06:36.000000 saes6-jerry-0.0.2/saes6_jerry.egg-info/entry_points.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-14 09:06:36.000000 saes6-jerry-0.0.2/saes6_jerry.egg-info/top_level.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 09:06:36.393361 saes6-jerry-0.0.2/setup.cfg
+-rw-r--r--   0 gonzales   (501) staff       (20)      652 2024-05-14 08:22:07.000000 saes6-jerry-0.0.2/setup.py
```

### Comparing `saes6-jerry-0.0.1/setup.py` & `saes6-jerry-0.0.2/setup.py`

 * *Files identical despite different names*

