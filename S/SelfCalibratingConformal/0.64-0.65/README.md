# Comparing `tmp/SelfCalibratingConformal-0.64.tar.gz` & `tmp/SelfCalibratingConformal-0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SelfCalibratingConformal-0.64.tar", last modified: Mon May 13 23:26:00 2024, max compression
+gzip compressed data, was "dist/SelfCalibratingConformal-0.65.tar", last modified: Mon May 13 23:28:49 2024, max compression
```

## Comparing `SelfCalibratingConformal-0.64.tar` & `SelfCalibratingConformal-0.65.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      596 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratingConformal-0.64/README.md
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)     1035 2024-05-13 23:24:06.000000 SelfCalibratingConformal-0.64/setup.py
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/SelfCalibratingConformal.egg-info/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      596 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/SelfCalibratingConformal.egg-info/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      257 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/SelfCalibratingConformal.egg-info/SOURCES.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       50 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/SelfCalibratingConformal.egg-info/requires.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/SelfCalibratingConformal.egg-info/top_level.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/SelfCalibratingConformal.egg-info/dependency_links.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-13 23:26:00.000000 SelfCalibratingConformal-0.64/setup.cfg
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      596 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratingConformal-0.65/README.md
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)     1035 2024-05-13 23:28:42.000000 SelfCalibratingConformal-0.65/setup.py
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/SelfCalibratingConformal.egg-info/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      596 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/SelfCalibratingConformal.egg-info/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      257 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/SelfCalibratingConformal.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       50 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/SelfCalibratingConformal.egg-info/requires.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/SelfCalibratingConformal.egg-info/top_level.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/SelfCalibratingConformal.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-13 23:28:49.000000 SelfCalibratingConformal-0.65/setup.cfg
```

### Comparing `SelfCalibratingConformal-0.64/PKG-INFO` & `SelfCalibratingConformal-0.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratingConformal
-Version: 0.64
+Version: 0.65
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratingConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 License: UNKNOWN
 Description: A Python implementation of Self-Calibrated Conformal Prediction
 Platform: UNKNOWN
```

### Comparing `SelfCalibratingConformal-0.64/setup.py` & `SelfCalibratingConformal-0.65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SelfCalibratingConformal',
-    version='0.64',
+    version='0.65',
     packages=find_packages(),
     description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description_content_type='text/markdown',  # assuming your description is in Markdown format
     author='Lars van der Laan',
     author_email='vanderlaanlars@yahoo.com',
     url='https://github.com/Larsvanderlaan/SelfCalibratingConformal',
```

### Comparing `SelfCalibratingConformal-0.64/SelfCalibratingConformal.egg-info/PKG-INFO` & `SelfCalibratingConformal-0.65/SelfCalibratingConformal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratingConformal
-Version: 0.64
+Version: 0.65
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratingConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 License: UNKNOWN
 Description: A Python implementation of Self-Calibrated Conformal Prediction
 Platform: UNKNOWN
```

