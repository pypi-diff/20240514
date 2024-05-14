# Comparing `tmp/resik-0.0.3.tar.gz` & `tmp/resik-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resik-0.0.3.tar", last modified: Tue May 14 17:26:00 2024, max compression
+gzip compressed data, was "resik-0.0.4.tar", last modified: Tue May 14 17:29:20 2024, max compression
```

## Comparing `resik-0.0.3.tar` & `resik-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:26:00.653592 resik-0.0.3/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      276 2024-05-14 17:26:00.653071 resik-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-05-14 17:25:53.000000 resik-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 17:26:00.629464 resik-0.0.3/resik/
--rw-rw-rw-   0        0        0       29 2024-05-14 17:04:14.000000 resik-0.0.3/resik/__init__.py
--rw-rw-rw-   0        0        0      330 2024-05-14 16:08:02.000000 resik-0.0.3/resik/imp.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:26:00.649684 resik-0.0.3/resik.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 17:26:00.000000 resik-0.0.3/resik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:26:00.654114 resik-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-05-14 17:24:20.000000 resik-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:29:20.601419 resik-0.0.4/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      281 2024-05-14 17:29:20.599415 resik-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-05-14 17:29:15.000000 resik-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 17:29:20.580415 resik-0.0.4/resik/
+-rw-rw-rw-   0        0        0       29 2024-05-14 17:04:14.000000 resik-0.0.4/resik/__init__.py
+-rw-rw-rw-   0        0        0      330 2024-05-14 16:08:02.000000 resik-0.0.4/resik/imp.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:29:20.598436 resik-0.0.4/resik.egg-info/
+-rw-rw-rw-   0        0        0      281 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 17:29:20.000000 resik-0.0.4/resik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:29:20.601419 resik-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      949 2024-05-14 17:28:46.000000 resik-0.0.4/setup.py
```

### Comparing `resik-0.0.3/setup.py` & `resik-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 PACKAGE_NAME = 'resik'
 AUTHOR = 'Master'
 AUTHOR_EMAIL = 'name@email.com'
 LICENSE = 'License'
 DESCRIPTION = 'Description about the project.'
 # Read the contents of your README file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
@@ -23,9 +23,11 @@
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',  # Specify the type of content
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     install_requires=INSTALL_REQUIRES,
     license=LICENSE,
     packages=find_packages(),
-    include_package_data=True
+    include_package_data=True,
+    test_suite='nose.collector',
+    tests_require=['nose'],
 )
```

