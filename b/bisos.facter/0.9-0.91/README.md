# Comparing `tmp/bisos.facter-0.9.tar.gz` & `tmp/bisos.facter-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.facter-0.9.tar", last modified: Mon May 13 04:22:55 2024, max compression
+gzip compressed data, was "bisos.facter-0.91.tar", last modified: Tue May 14 04:08:27 2024, max compression
```

## Comparing `bisos.facter-0.9.tar` & `bisos.facter-0.91.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-12 04:31:16.000000 bisos.facter-0.9/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7223 2024-05-13 04:22:55.109379 bisos.facter-0.9/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5840 2024-05-13 04:21:27.000000 bisos.facter-0.9/README.org
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.9/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.9/bin/facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.9/bin/roInv-facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.9/bin/roPerf-facter.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bisos/facter/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/facter/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/facter/facter.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.9/bisos/facter/facter_csu.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-13 04:22:55.109379 bisos.facter-0.9/bisos.facter.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7223 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-13 04:22:55.000000 bisos.facter-0.9/bisos.facter.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-13 04:22:54.000000 bisos.facter-0.9/bisos.facter.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-13 04:22:55.000000 bisos.facter-0.9/bisos.facter.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-13 04:22:54.000000 bisos.facter-0.9/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-13 04:22:55.109379 bisos.facter-0.9/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2127 2024-05-13 04:21:27.000000 bisos.facter-0.9/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-14 04:08:27.072123 bisos.facter-0.91/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-12 04:31:16.000000 bisos.facter-0.91/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7224 2024-05-14 04:08:27.068123 bisos.facter-0.91/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5840 2024-05-13 04:21:27.000000 bisos.facter-0.91/README.org
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-14 04:08:27.068123 bisos.facter-0.91/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.91/bin/facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.91/bin/roInv-facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.91/bin/roPerf-facter.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-14 04:08:27.068123 bisos.facter-0.91/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.91/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-14 04:08:27.068123 bisos.facter-0.91/bisos/facter/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.91/bisos/facter/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.91/bisos/facter/facter.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.91/bisos/facter/facter_csu.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-14 04:08:27.068123 bisos.facter-0.91/bisos.facter.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7224 2024-05-14 04:08:26.000000 bisos.facter-0.91/bisos.facter.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      420 2024-05-14 04:08:27.000000 bisos.facter-0.91/bisos.facter.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-14 04:08:26.000000 bisos.facter-0.91/bisos.facter.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-14 04:08:26.000000 bisos.facter-0.91/bisos.facter.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-14 04:08:26.000000 bisos.facter-0.91/bisos.facter.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-14 04:08:26.000000 bisos.facter-0.91/bisos.facter.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-14 04:08:25.000000 bisos.facter-0.91/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-14 04:08:27.072123 bisos.facter-0.91/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1993 2024-05-14 04:04:58.000000 bisos.facter-0.91/setup.py
```

### Comparing `bisos.facter-0.9/PKG-INFO` & `bisos.facter-0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.9
+Version: 0.91
 Summary: bisos.facter:  Adoption and adaptation of facter to Python and as Service
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -13,21 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires: bisos
 Requires: blee
 Requires: blee.csPlayer
-Requires: bisos.transit
+Requires: bisos
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
+Requires: bisos.transit
 
 Overview
 ========
 
 bisos.facter is a python package for adoption and adaptation of
 **facter** to python and PyCS-Framework. It is a BISOS capability and a
 standalone piece of BISOS.
```

### Comparing `bisos.facter-0.9/README.org` & `bisos.facter-0.91/README.org`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.9/bin/facter.cs` & `bisos.facter-0.91/bin/facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.9/bin/roInv-facter.cs` & `bisos.facter-0.91/bin/roInv-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.9/bin/roPerf-facter.cs` & `bisos.facter-0.91/bin/roPerf-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.9/bisos/facter/facter.py` & `bisos.facter-0.91/bisos/facter/facter.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.9/bisos/facter/facter_csu.py` & `bisos.facter-0.91/bisos/facter/facter_csu.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.9/bisos.facter.egg-info/PKG-INFO` & `bisos.facter-0.91/bisos.facter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.9
+Version: 0.91
 Summary: bisos.facter:  Adoption and adaptation of facter to Python and as Service
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -13,21 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires: bisos
 Requires: blee
 Requires: blee.csPlayer
-Requires: bisos.transit
+Requires: bisos
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
+Requires: bisos.transit
 
 Overview
 ========
 
 bisos.facter is a python package for adoption and adaptation of
 **facter** to python and PyCS-Framework. It is a BISOS capability and a
 standalone piece of BISOS.
```

### Comparing `bisos.facter-0.9/lh-agpl3-LICENSE.txt` & `bisos.facter-0.91/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.9/setup.py` & `bisos.facter-0.91/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,45 +14,43 @@
 
 def longDescription():
     try:
         import pypandoc
     except ImportError:
         result = "warning: pypandoc module not found, could not convert to RST"
         return result
-
     return pypandoc.convert_file('README.org', 'rst')
 
+####+BEGIN: b:py3:pypi/nextVersion :increment 0.01
 
+__version__ = 0.91
 
-# from setuphelpers import get_version, require_python
-# from setuptools import setup
-
-# __version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.9'
+####+END:
 
+####+BEGIN: b:py3:pypi/requires :extras ("bisos.transit")
 
 requires = [
-    "bisos",
-    "blee",
-    "blee.csPlayer",
-    "bisos.transit",   # is used in bisos.b
-    "bisos.b",
-    "bisos.banna",
-    "bisos.common",
+"blee",
+"blee.csPlayer",
+"bisos",
+"bisos.b",
+"bisos.banna",
+"bisos.common",
+"bisos.transit",
 ]
+####+END:
 
-
-# print('Setting up under python version %s' % sys.version)
-# print('Requirements: %s' % ','.join(requires))
+####+BEGIN: b:py3:pypi/scripts :comment ""
 
 scripts = [
-    "./bin/facter.cs",
-    "./bin/roInv-facter.cs",
-    "./bin/roPerf-facter.cs",
+'./bin/facter.cs',
+'./bin/roInv-facter.cs',
+'./bin/roPerf-facter.cs',
 ]
+####+END:
 
 
 setuptools.setup(
     name='bisos.facter',
     version=__version__,
     # namespace_packages=['bisos'],
     packages=setuptools.find_packages(),
```

