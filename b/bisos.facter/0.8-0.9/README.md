# Comparing `tmp/bisos.facter-0.8.tar.gz` & `tmp/bisos.facter-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.facter-0.8.tar", last modified: Sun May 12 04:40:28 2024, max compression
+gzip compressed data, was "bisos.facter-0.9.tar", last modified: Mon May 13 04:22:55 2024, max compression
```

## Comparing `bisos.facter-0.8.tar` & `bisos.facter-0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-12 04:31:16.000000 bisos.facter-0.8/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1993 2024-05-12 04:40:28.342722 bisos.facter-0.8/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1350 2024-05-12 04:31:16.000000 bisos.facter-0.8/README.org
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.8/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.8/bin/facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.8/bin/roInv-facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.8/bin/roPerf-facter.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bisos/facter/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/facter/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/facter/facter.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/facter/facter_csu.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bisos.facter.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1993 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-12 04:40:27.000000 bisos.facter-0.8/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-12 04:40:28.342722 bisos.facter-0.8/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1896 2024-05-12 04:39:04.000000 bisos.facter-0.8/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-12 04:31:16.000000 bisos.facter-0.9/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7223 2024-05-13 04:22:55.109379 bisos.facter-0.9/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5840 2024-05-13 04:21:27.000000 bisos.facter-0.9/README.org
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.9/TITLE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.9/bin/facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.9/bin/roInv-facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.9/bin/roPerf-facter.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bisos/facter/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/facter/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/facter/facter.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/facter/facter_csu.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bisos.facter.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7223 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-13 04:22:55.000000 bisos.facter-0.9/bisos.facter.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-13 04:22:55.000000 bisos.facter-0.9/bisos.facter.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-13 04:22:54.000000 bisos.facter-0.9/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-13 04:22:55.109379 bisos.facter-0.9/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2127 2024-05-13 04:21:27.000000 bisos.facter-0.9/setup.py
```

### Comparing `bisos.facter-0.8/bin/facter.cs` & `bisos.facter-0.9/bin/facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.8/bin/roInv-facter.cs` & `bisos.facter-0.9/bin/roInv-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.8/bin/roPerf-facter.cs` & `bisos.facter-0.9/bin/roPerf-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.8/bisos/facter/facter.py` & `bisos.facter-0.9/bisos/facter/facter.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.8/bisos/facter/facter_csu.py` & `bisos.facter-0.9/bisos/facter/facter_csu.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.8/lh-agpl3-LICENSE.txt` & `bisos.facter-0.9/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.8/setup.py` & `bisos.facter-0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 #!/usr/bin/env python
 
 import setuptools
 # import sys
-
-import pypandoc
+import re
 
 
 def readme():
-    with open('TITLE.txt') as f:
-        return f.readline().rstrip('\n')
-
-
-def longDescriptionOld():
-    with open('README.rst') as f:
-        return f.read()
+    with open('./README.org') as file:
+        while line := file.readline():
+            if match := re.search(r'^#\+title: (.*)',  line.rstrip()):
+                return match.group(1)
+            return "MISSING TITLE in ./README.org"
 
 def longDescription():
+    try:
+        import pypandoc
+    except ImportError:
+        result = "warning: pypandoc module not found, could not convert to RST"
+        return result
+
     return pypandoc.convert_file('README.org', 'rst')
 
 
 
 # from setuphelpers import get_version, require_python
 # from setuptools import setup
 
 # __version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.8'
+__version__ = '0.9'
 
 
 requires = [
     "bisos",
     "blee",
     "blee.csPlayer",
     "bisos.transit",   # is used in bisos.b
```

