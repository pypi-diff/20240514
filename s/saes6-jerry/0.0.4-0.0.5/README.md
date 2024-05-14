# Comparing `tmp/saes6-jerry-0.0.4.tar.gz` & `tmp/saes6-jerry-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saes6-jerry-0.0.4.tar", last modified: Tue May 14 09:14:06 2024, max compression
+gzip compressed data, was "saes6-jerry-0.0.5.tar", last modified: Tue May 14 09:21:15 2024, max compression
```

## Comparing `saes6-jerry-0.0.4.tar` & `saes6-jerry-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:14:06.308413 saes6-jerry-0.0.4/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:14:06.308171 saes6-jerry-0.0.4/PKG-INFO
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:14:06.306190 saes6-jerry-0.0.4/jerry/
--rw-r--r--   0 gonzales   (501) staff       (20)       85 2024-05-14 09:14:03.000000 saes6-jerry-0.0.4/jerry/__init__.py
--rw-r--r--   0 gonzales   (501) staff       (20)      136 2024-05-14 09:05:06.000000 saes6-jerry-0.0.4/jerry/default.py
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:14:06.307956 saes6-jerry-0.0.4/saes6_jerry.egg-info/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:14:06.000000 saes6-jerry-0.0.4/saes6_jerry.egg-info/PKG-INFO
--rw-r--r--   0 gonzales   (501) staff       (20)      221 2024-05-14 09:14:06.000000 saes6-jerry-0.0.4/saes6_jerry.egg-info/SOURCES.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-14 09:14:06.000000 saes6-jerry-0.0.4/saes6_jerry.egg-info/dependency_links.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       43 2024-05-14 09:14:06.000000 saes6-jerry-0.0.4/saes6_jerry.egg-info/entry_points.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-14 09:14:06.000000 saes6-jerry-0.0.4/saes6_jerry.egg-info/top_level.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 09:14:06.308461 saes6-jerry-0.0.4/setup.cfg
--rw-r--r--   0 gonzales   (501) staff       (20)      659 2024-05-14 09:13:11.000000 saes6-jerry-0.0.4/setup.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:21:15.004458 saes6-jerry-0.0.5/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:21:15.004241 saes6-jerry-0.0.5/PKG-INFO
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:21:15.003136 saes6-jerry-0.0.5/jerry/
+-rw-r--r--   0 gonzales   (501) staff       (20)       21 2024-05-14 09:21:03.000000 saes6-jerry-0.0.5/jerry/__init__.py
+-rw-r--r--   0 gonzales   (501) staff       (20)       97 2024-05-14 09:19:05.000000 saes6-jerry-0.0.5/jerry/default.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:21:15.004048 saes6-jerry-0.0.5/saes6_jerry.egg-info/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:21:14.000000 saes6-jerry-0.0.5/saes6_jerry.egg-info/PKG-INFO
+-rw-r--r--   0 gonzales   (501) staff       (20)      221 2024-05-14 09:21:14.000000 saes6-jerry-0.0.5/saes6_jerry.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-14 09:21:14.000000 saes6-jerry-0.0.5/saes6_jerry.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       45 2024-05-14 09:21:14.000000 saes6-jerry-0.0.5/saes6_jerry.egg-info/entry_points.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-14 09:21:14.000000 saes6-jerry-0.0.5/saes6_jerry.egg-info/top_level.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 09:21:15.004517 saes6-jerry-0.0.5/setup.cfg
+-rw-r--r--   0 gonzales   (501) staff       (20)      661 2024-05-14 09:20:36.000000 saes6-jerry-0.0.5/setup.py
```

### Comparing `saes6-jerry-0.0.4/setup.py` & `saes6-jerry-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     packages=find_packages(),
 
     extras_require={},
 
     entry_points={
         'console_scripts': [
-            'saes6-jerry = jerry:main',
+            'saes6-jerry = default:main',
         ],
     },
 
     classifiers=[
         'Intended Audience :: Developers',
 
         'Programming Language :: Python',
```

