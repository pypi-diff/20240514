# Comparing `tmp/donware-0.1.3.tar.gz` & `tmp/donware-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donware-0.1.3.tar", last modified: Tue May 14 06:14:42 2024, max compression
+gzip compressed data, was "donware-0.1.4.tar", last modified: Tue May 14 06:18:17 2024, max compression
```

## Comparing `donware-0.1.3.tar` & `donware-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:14:42.859624 donware-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 06:14:24.000000 donware-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 06:14:24.000000 donware-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:14:42.859624 donware-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:14:24.000000 donware-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:14:42.859624 donware-0.1.3/donware/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 06:14:24.000000 donware-0.1.3/donware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:14:42.859624 donware-0.1.3/donware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:14:42.000000 donware-0.1.3/donware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 06:14:42.000000 donware-0.1.3/donware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:14:42.000000 donware-0.1.3/donware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 06:14:42.000000 donware-0.1.3/donware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:14:42.859624 donware-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 06:14:24.000000 donware-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:18:17.004711 donware-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 06:17:53.000000 donware-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 06:17:53.000000 donware-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:18:17.004711 donware-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:17:53.000000 donware-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:18:17.000711 donware-0.1.4/donware/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 06:18:12.000000 donware-0.1.4/donware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:18:17.004711 donware-0.1.4/donware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:18:16.000000 donware-0.1.4/donware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 06:18:17.000000 donware-0.1.4/donware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:18:16.000000 donware-0.1.4/donware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 06:18:16.000000 donware-0.1.4/donware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:18:17.004711 donware-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 06:17:53.000000 donware-0.1.4/setup.py
```

### Comparing `donware-0.1.3/LICENSE` & `donware-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `donware-0.1.3/setup.py` & `donware-0.1.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="donware",
-    version="0.1.3",
+    version="0.1.4",
     author="Don Yin",
     author_email="Don_Yin@outlook.com",
     description="Don's personal toolkits for data science and machine learning.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Don-Yin/donware",
     packages=find_packages(),
```
