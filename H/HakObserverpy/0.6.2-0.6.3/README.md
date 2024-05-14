# Comparing `tmp/HakObserverpy-0.6.2.tar.gz` & `tmp/HakObserverpy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HakObserverpy-0.6.2.tar", last modified: Mon May 13 14:38:26 2024, max compression
+gzip compressed data, was "HakObserverpy-0.6.3.tar", last modified: Tue May 14 05:43:09 2024, max compression
```

## Comparing `HakObserverpy-0.6.2.tar` & `HakObserverpy-0.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:38:26.969594 HakObserverpy-0.6.2/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:38:26.952595 HakObserverpy-0.6.2/HakObserverpy/
--rw-rw-rw-   0        0        0     9609 2024-05-13 14:38:21.000000 HakObserverpy-0.6.2/HakObserverpy/HakObserverpy.py
--rw-rw-rw-   0        0        0      251 2024-05-13 14:37:02.000000 HakObserverpy-0.6.2/HakObserverpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:38:26.968594 HakObserverpy-0.6.2/HakObserverpy.egg-info/
--rw-rw-rw-   0        0        0      705 2024-05-13 14:38:26.000000 HakObserverpy-0.6.2/HakObserverpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-13 14:38:26.000000 HakObserverpy-0.6.2/HakObserverpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:38:26.000000 HakObserverpy-0.6.2/HakObserverpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-13 14:38:26.000000 HakObserverpy-0.6.2/HakObserverpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 14:38:26.000000 HakObserverpy-0.6.2/HakObserverpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      705 2024-05-13 14:38:26.969594 HakObserverpy-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 09:19:09.000000 HakObserverpy-0.6.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 14:38:26.969594 HakObserverpy-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1044 2024-05-13 14:36:50.000000 HakObserverpy-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:43:09.980902 HakObserverpy-0.6.3/
+drwxrwxrwx   0        0        0        0 2024-05-14 05:43:09.959928 HakObserverpy-0.6.3/HakObserverpy/
+-rw-rw-rw-   0        0        0     9609 2024-05-14 05:41:30.000000 HakObserverpy-0.6.3/HakObserverpy/HakObserverpy.py
+-rw-rw-rw-   0        0        0      237 2024-05-14 05:41:35.000000 HakObserverpy-0.6.3/HakObserverpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:43:09.978901 HakObserverpy-0.6.3/HakObserverpy.egg-info/
+-rw-rw-rw-   0        0        0      705 2024-05-14 05:43:09.000000 HakObserverpy-0.6.3/HakObserverpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 05:43:09.000000 HakObserverpy-0.6.3/HakObserverpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 05:43:09.000000 HakObserverpy-0.6.3/HakObserverpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-14 05:43:09.000000 HakObserverpy-0.6.3/HakObserverpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 05:43:09.000000 HakObserverpy-0.6.3/HakObserverpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2024-05-14 05:43:09.979903 HakObserverpy-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-13 09:19:09.000000 HakObserverpy-0.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 05:43:09.980902 HakObserverpy-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-05-14 05:41:28.000000 HakObserverpy-0.6.3/setup.py
```

### Comparing `HakObserverpy-0.6.2/HakObserverpy/HakObserverpy.py` & `HakObserverpy-0.6.3/HakObserverpy/HakObserverpy.py`

 * *Files identical despite different names*

### Comparing `HakObserverpy-0.6.2/HakObserverpy.egg-info/PKG-INFO` & `HakObserverpy-0.6.3/HakObserverpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverpy
-Version: 0.6.2
+Version: 0.6.3
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverpy-0.6.2/PKG-INFO` & `HakObserverpy-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverpy
-Version: 0.6.2
+Version: 0.6.3
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverpy-0.6.2/setup.py` & `HakObserverpy-0.6.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 from setuptools import setup, find_packages
 
 setup(
     name='HakObserverpy',  # Your package name
-    version='0.6.2',  # Start with a version number
+    version='0.6.3',  # Start with a version number
     description='A package connect endpoints to the Hakware Application',  # Short description
     long_description=open('README.md').read(),  # Long description from README
     long_description_content_type='text/markdown',
     author='Jacob O\'Brien',  # Your name
     # author_email='your.email@example.com',  # Your email
     # url='https://github.com/your-username/XGRCPy',  # Your package's URL (if applicable)
     packages=find_packages(),  # Find all sub-packages
```

