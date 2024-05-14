# Comparing `tmp/AlphaDSSP-0.2.tar.gz` & `tmp/AlphaDSSP-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlphaDSSP-0.2.tar", last modified: Tue May 14 18:58:23 2024, max compression
+gzip compressed data, was "AlphaDSSP-0.3.tar", last modified: Tue May 14 19:13:59 2024, max compression
```

## Comparing `AlphaDSSP-0.2.tar` & `AlphaDSSP-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-14 18:58:23.235045 AlphaDSSP-0.2/
-drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-14 18:58:23.235045 AlphaDSSP-0.2/AlphaDSSP.egg-info/
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      488 2024-05-14 18:58:23.000000 AlphaDSSP-0.2/AlphaDSSP.egg-info/PKG-INFO
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      235 2024-05-14 18:58:23.000000 AlphaDSSP-0.2/AlphaDSSP.egg-info/SOURCES.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)        1 2024-05-14 18:58:23.000000 AlphaDSSP-0.2/AlphaDSSP.egg-info/dependency_links.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       21 2024-05-14 18:58:23.000000 AlphaDSSP-0.2/AlphaDSSP.egg-info/requires.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       10 2024-05-14 18:58:23.000000 AlphaDSSP-0.2/AlphaDSSP.egg-info/top_level.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)    35129 2024-04-27 00:47:33.000000 AlphaDSSP-0.2/LICENSE
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      488 2024-05-14 18:58:23.235045 AlphaDSSP-0.2/PKG-INFO
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       69 2024-04-27 00:47:33.000000 AlphaDSSP-0.2/README.md
-drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-14 18:58:23.235045 AlphaDSSP-0.2/alphadssp/
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-14 18:54:28.000000 AlphaDSSP-0.2/alphadssp/__init__.py
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     5389 2024-05-14 18:33:41.000000 AlphaDSSP-0.2/alphadssp/alphadssp.py
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       38 2024-05-14 18:58:23.235045 AlphaDSSP-0.2/setup.cfg
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      656 2024-05-14 18:58:15.000000 AlphaDSSP-0.2/setup.py
+drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-14 19:13:59.434410 AlphaDSSP-0.3/
+drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-14 19:13:59.433410 AlphaDSSP-0.3/AlphaDSSP.egg-info/
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      488 2024-05-14 19:13:59.000000 AlphaDSSP-0.3/AlphaDSSP.egg-info/PKG-INFO
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      235 2024-05-14 19:13:59.000000 AlphaDSSP-0.3/AlphaDSSP.egg-info/SOURCES.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)        1 2024-05-14 19:13:59.000000 AlphaDSSP-0.3/AlphaDSSP.egg-info/dependency_links.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       21 2024-05-14 19:13:59.000000 AlphaDSSP-0.3/AlphaDSSP.egg-info/requires.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       10 2024-05-14 19:13:59.000000 AlphaDSSP-0.3/AlphaDSSP.egg-info/top_level.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)    35129 2024-04-27 00:47:33.000000 AlphaDSSP-0.3/LICENSE
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      488 2024-05-14 19:13:59.434410 AlphaDSSP-0.3/PKG-INFO
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       69 2024-04-27 00:47:33.000000 AlphaDSSP-0.3/README.md
+drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-14 19:13:59.433410 AlphaDSSP-0.3/alphadssp/
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       36 2024-05-14 19:12:55.000000 AlphaDSSP-0.3/alphadssp/__init__.py
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     5389 2024-05-14 18:33:41.000000 AlphaDSSP-0.3/alphadssp/alphadssp.py
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       38 2024-05-14 19:13:59.434410 AlphaDSSP-0.3/setup.cfg
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      656 2024-05-14 19:13:54.000000 AlphaDSSP-0.3/setup.py
```

### Comparing `AlphaDSSP-0.2/LICENSE` & `AlphaDSSP-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AlphaDSSP-0.2/alphadssp/alphadssp.py` & `AlphaDSSP-0.3/alphadssp/alphadssp.py`

 * *Files identical despite different names*

### Comparing `AlphaDSSP-0.2/setup.py` & `AlphaDSSP-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AlphaDSSP",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     description="Tool for converting Alphafold tar shards to a database of DSSP secondary structure information.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Noel Garber",
     author_email="ngarber93@gmail.com",
     url="https://github.com/noelgarber/AlphaDSSP",
```

