# Comparing `tmp/resik-0.0.5.tar.gz` & `tmp/resik-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resik-0.0.5.tar", last modified: Tue May 14 17:43:41 2024, max compression
+gzip compressed data, was "resik-0.0.6.tar", last modified: Tue May 14 17:55:18 2024, max compression
```

## Comparing `resik-0.0.5.tar` & `resik-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:43:41.609040 resik-0.0.5/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      454 2024-05-14 17:43:41.609040 resik-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-14 17:43:35.000000 resik-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 17:43:41.580040 resik-0.0.5/resik/
--rw-rw-rw-   0        0        0       33 2024-05-14 17:36:03.000000 resik-0.0.5/resik/__init__.py
--rw-rw-rw-   0        0        0      967 2024-05-14 17:35:42.000000 resik-0.0.5/resik/app.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:43:41.607040 resik-0.0.5/resik.egg-info/
--rw-rw-rw-   0        0        0      454 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 17:43:41.000000 resik-0.0.5/resik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:43:41.610040 resik-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      949 2024-05-14 17:40:39.000000 resik-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:55:18.236473 resik-0.0.6/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:36:07.000000 resik-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       67 2024-05-14 16:37:09.000000 resik-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      454 2024-05-14 17:55:18.235473 resik-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-14 17:43:35.000000 resik-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 17:55:18.186092 resik-0.0.6/resik/
+-rw-rw-rw-   0        0        0       33 2024-05-14 17:36:03.000000 resik-0.0.6/resik/__init__.py
+-rw-rw-rw-   0        0        0      189 2024-05-14 17:48:04.000000 resik-0.0.6/resik/__main__.py
+-rw-rw-rw-   0        0        0      967 2024-05-14 17:35:42.000000 resik-0.0.6/resik/app.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:55:18.233473 resik-0.0.6/resik.egg-info/
+-rw-rw-rw-   0        0        0      454 2024-05-14 17:55:18.000000 resik-0.0.6/resik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-14 17:55:18.000000 resik-0.0.6/resik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:55:18.000000 resik-0.0.6/resik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 17:55:18.000000 resik-0.0.6/resik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 17:55:18.000000 resik-0.0.6/resik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:55:18.236473 resik-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      897 2024-05-14 17:55:16.000000 resik-0.0.6/setup.py
```

### Comparing `resik-0.0.5/resik/app.py` & `resik-0.0.6/resik/app.py`

 * *Files identical despite different names*

### Comparing `resik-0.0.5/setup.py` & `resik-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 PACKAGE_NAME = 'resik'
 AUTHOR = 'Master'
 AUTHOR_EMAIL = 'name@email.com'
 LICENSE = 'License'
 DESCRIPTION = 'Description about the project.'
 # Read the contents of your README file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # Add your required packages to INSTALL_REQUIRES list
-INSTALL_REQUIRES = []
+INSTALL_REQUIRES = ['tkinter']
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',  # Specify the type of content
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     install_requires=INSTALL_REQUIRES,
     license=LICENSE,
     packages=find_packages(),
     include_package_data=True,
-    test_suite='nose.collector',
-    tests_require=['nose'],
+
 )
```

