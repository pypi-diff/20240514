# Comparing `tmp/donware-0.1.5.tar.gz` & `tmp/donware-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donware-0.1.5.tar", last modified: Tue May 14 06:20:58 2024, max compression
+gzip compressed data, was "donware-0.1.6.tar", last modified: Tue May 14 06:28:56 2024, max compression
```

## Comparing `donware-0.1.5.tar` & `donware-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:20:58.970531 donware-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 06:20:41.000000 donware-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 06:20:41.000000 donware-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:20:58.970531 donware-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:20:41.000000 donware-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:20:58.970531 donware-0.1.5/donware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:20:41.000000 donware-0.1.5/donware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:20:58.970531 donware-0.1.5/donware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:20:58.000000 donware-0.1.5/donware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 06:20:58.000000 donware-0.1.5/donware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:20:58.000000 donware-0.1.5/donware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 06:20:58.000000 donware-0.1.5/donware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:20:58.970531 donware-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 06:20:41.000000 donware-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:56.938332 donware-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 06:28:40.000000 donware-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 06:28:40.000000 donware-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:28:56.938332 donware-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:40.000000 donware-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:56.938332 donware-0.1.6/donware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:40.000000 donware-0.1.6/donware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:56.938332 donware-0.1.6/donware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:40.000000 donware-0.1.6/donware/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:56.938332 donware-0.1.6/donware/src/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:40.000000 donware-0.1.6/donware/src/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:56.938332 donware-0.1.6/donware/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:40.000000 donware-0.1.6/donware/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-14 06:28:40.000000 donware-0.1.6/donware/src/utils/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:28:56.938332 donware-0.1.6/donware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 06:28:56.000000 donware-0.1.6/donware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-14 06:28:56.000000 donware-0.1.6/donware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:28:56.000000 donware-0.1.6/donware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 06:28:56.000000 donware-0.1.6/donware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:28:56.938332 donware-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 06:28:40.000000 donware-0.1.6/setup.py
```

### Comparing `donware-0.1.5/LICENSE` & `donware-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `donware-0.1.5/setup.py` & `donware-0.1.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="donware",
-    version="0.1.5",
+    version="0.1.6",
     author="Don Yin",
     author_email="Don_Yin@outlook.com",
     description="Don's personal toolkits for data science and machine learning.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Don-Yin/donware",
     packages=find_packages(),
```

