# Comparing `tmp/resik-0.0.2.tar.gz` & `tmp/resik-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resik-0.0.2.tar", last modified: Tue May 14 17:09:12 2024, max compression
+gzip compressed data, was "resik-0.0.3.tar", last modified: Tue May 14 17:26:00 2024, max compression
```

## Comparing `resik-0.0.2.tar` & `resik-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:09:12.196849 resik-0.0.2/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      276 2024-05-14 17:09:12.195848 resik-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-05-14 16:39:28.000000 resik-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 17:09:12.187849 resik-0.0.2/resik/
--rw-rw-rw-   0        0        0       29 2024-05-14 17:04:14.000000 resik-0.0.2/resik/__init__.py
--rw-rw-rw-   0        0        0      330 2024-05-14 16:08:02.000000 resik-0.0.2/resik/imp.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:09:12.194849 resik-0.0.2/resik.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-14 17:09:12.000000 resik-0.0.2/resik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-14 17:09:12.000000 resik-0.0.2/resik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:09:12.000000 resik-0.0.2/resik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 17:09:12.000000 resik-0.0.2/resik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:09:12.198850 resik-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-05-14 17:07:47.000000 resik-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:26:00.653592 resik-0.0.3/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      276 2024-05-14 17:26:00.653071 resik-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-05-14 17:25:53.000000 resik-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 17:26:00.629464 resik-0.0.3/resik/
+-rw-rw-rw-   0        0        0       29 2024-05-14 17:04:14.000000 resik-0.0.3/resik/__init__.py
+-rw-rw-rw-   0        0        0      330 2024-05-14 16:08:02.000000 resik-0.0.3/resik/imp.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:26:00.649684 resik-0.0.3/resik.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:26:00.654114 resik-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-05-14 17:24:20.000000 resik-0.0.3/setup.py
```

### Comparing `resik-0.0.2/setup.py` & `resik-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 PACKAGE_NAME = 'resik'
 AUTHOR = 'Master'
 AUTHOR_EMAIL = 'name@email.com'
 LICENSE = 'License'
 DESCRIPTION = 'Description about the project.'
 # Read the contents of your README file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
```

