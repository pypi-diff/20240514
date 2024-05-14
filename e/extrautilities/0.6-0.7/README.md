# Comparing `tmp/extrautilities-0.6.tar.gz` & `tmp/extrautilities-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-0.6.tar", last modified: Mon May 13 18:01:44 2024, max compression
+gzip compressed data, was "extrautilities-0.7.tar", last modified: Tue May 14 17:51:18 2024, max compression
```

## Comparing `extrautilities-0.6.tar` & `extrautilities-0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:01:44.500370 extrautilities-0.6/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:01:44.483251 extrautilities-0.6/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.6/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.6/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-0.6/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0     2361 2024-05-13 18:01:44.499870 extrautilities-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 18:01:44.498865 extrautilities-0.6/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     2361 2024-05-13 18:01:44.000000 extrautilities-0.6/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 18:01:44.000000 extrautilities-0.6/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:01:44.000000 extrautilities-0.6/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-13 18:01:44.000000 extrautilities-0.6/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 18:01:44.000000 extrautilities-0.6/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 18:01:44.500370 extrautilities-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1069 2024-05-13 18:01:38.000000 extrautilities-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:51:18.599098 extrautilities-0.7/
+drwxrwxrwx   0        0        0        0 2024-05-14 17:51:18.579395 extrautilities-0.7/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.7/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.7/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-0.7/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0     1491 2024-05-14 17:48:41.000000 extrautilities-0.7/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     2361 2024-05-14 17:51:18.598591 extrautilities-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 17:51:18.597080 extrautilities-0.7/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     2361 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 17:51:18.000000 extrautilities-0.7/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:51:18.599098 extrautilities-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2024-05-14 17:51:12.000000 extrautilities-0.7/setup.py
```

### Comparing `extrautilities-0.6/ExtraUtils/RateLimit.py` & `extrautilities-0.7/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.6/ExtraUtils/asyncTokens.py` & `extrautilities-0.7/ExtraUtils/asyncTokens.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.6/PKG-INFO` & `extrautilities-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.6
+Version: 0.7
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,asyncTokens
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.6/README.md` & `extrautilities-0.7/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-0.6/extrautilities.egg-info/PKG-INFO` & `extrautilities-0.7/extrautilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.6
+Version: 0.7
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,asyncTokens
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.6/setup.py` & `extrautilities-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

