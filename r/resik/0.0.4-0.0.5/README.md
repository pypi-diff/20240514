# Comparing `tmp/resik-0.0.4.tar.gz` & `tmp/resik-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resik-0.0.4.tar", last modified: Tue May 14 17:29:20 2024, max compression
+gzip compressed data, was "resik-0.0.5.tar", last modified: Tue May 14 17:43:41 2024, max compression
```

## Comparing `resik-0.0.4.tar` & `resik-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:29:20.601419 resik-0.0.4/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      281 2024-05-14 17:29:20.599415 resik-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-05-14 17:29:15.000000 resik-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 17:29:20.580415 resik-0.0.4/resik/
--rw-rw-rw-   0        0        0       29 2024-05-14 17:04:14.000000 resik-0.0.4/resik/__init__.py
--rw-rw-rw-   0        0        0      330 2024-05-14 16:08:02.000000 resik-0.0.4/resik/imp.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:29:20.598436 resik-0.0.4/resik.egg-info/
--rw-rw-rw-   0        0        0      281 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:29:20.601419 resik-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      949 2024-05-14 17:28:46.000000 resik-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:43:41.609040 resik-0.0.5/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      454 2024-05-14 17:43:41.609040 resik-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-14 17:43:35.000000 resik-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 17:43:41.580040 resik-0.0.5/resik/
+-rw-rw-rw-   0        0        0       33 2024-05-14 17:36:03.000000 resik-0.0.5/resik/__init__.py
+-rw-rw-rw-   0        0        0      967 2024-05-14 17:35:42.000000 resik-0.0.5/resik/app.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:43:41.607040 resik-0.0.5/resik.egg-info/
+-rw-rw-rw-   0        0        0      454 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:43:41.610040 resik-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      949 2024-05-14 17:40:39.000000 resik-0.0.5/setup.py
```

### Comparing `resik-0.0.4/setup.py` & `resik-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 PACKAGE_NAME = 'resik'
 AUTHOR = 'Master'
 AUTHOR_EMAIL = 'name@email.com'
 LICENSE = 'License'
 DESCRIPTION = 'Description about the project.'
 # Read the contents of your README file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
```

