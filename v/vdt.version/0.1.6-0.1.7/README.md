# Comparing `tmp/vdt.version-0.1.6.tar.gz` & `tmp/vdt.version-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdt.version-0.1.6.tar", last modified: Mon Aug 13 16:01:44 2018, max compression
+gzip compressed data, was "vdt.version-0.1.7.tar", last modified: Tue May 14 07:36:19 2024, max compression
```

## Comparing `vdt.version-0.1.6.tar` & `vdt.version-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2018-08-13 16:01:44.000000 vdt.version-0.1.6/
--rw-r--r--   0 ebone      (502) staff       (20)      352 2018-08-13 16:01:44.000000 vdt.version-0.1.6/PKG-INFO
--rw-r--r--   0 ebone      (502) staff       (20)     4380 2018-08-13 15:14:11.000000 vdt.version-0.1.6/README.rst
--rw-r--r--   0 ebone      (502) staff       (20)       38 2018-08-13 16:01:44.000000 vdt.version-0.1.6/setup.cfg
--rw-r--r--   0 ebone      (502) staff       (20)      798 2018-08-13 16:00:16.000000 vdt.version-0.1.6/setup.py
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt/
--rw-r--r--   0 ebone      (502) staff       (20)       56 2018-08-13 15:14:11.000000 vdt.version-0.1.6/vdt/__init__.py
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt/version/
--rw-r--r--   0 ebone      (502) staff       (20)        1 2018-08-13 15:14:11.000000 vdt.version-0.1.6/vdt/version/__init__.py
--rw-r--r--   0 ebone      (502) staff       (20)     2919 2018-08-13 15:19:01.000000 vdt.version-0.1.6/vdt/version/main.py
--rw-r--r--   0 ebone      (502) staff       (20)     2215 2018-08-13 15:14:11.000000 vdt.version-0.1.6/vdt/version/repo.py
--rw-r--r--   0 ebone      (502) staff       (20)     3876 2018-08-13 15:29:53.000000 vdt.version-0.1.6/vdt/version/shared.py
--rw-r--r--   0 ebone      (502) staff       (20)     2965 2018-08-13 15:15:29.000000 vdt.version-0.1.6/vdt/version/utils.py
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/
--rw-r--r--   0 ebone      (502) staff       (20)        1 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/dependency_links.txt
--rw-r--r--   0 ebone      (502) staff       (20)       51 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/entry_points.txt
--rw-r--r--   0 ebone      (502) staff       (20)        4 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/namespace_packages.txt
--rw-r--r--   0 ebone      (502) staff       (20)      352 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/PKG-INFO
--rw-r--r--   0 ebone      (502) staff       (20)       67 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/requires.txt
--rw-r--r--   0 ebone      (502) staff       (20)      428 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/SOURCES.txt
--rw-r--r--   0 ebone      (502) staff       (20)        4 2018-08-13 16:01:44.000000 vdt.version-0.1.6/vdt.version.egg-info/top_level.txt
--rw-r--r--   0 ebone      (502) staff       (20)        1 2018-08-13 15:14:19.000000 vdt.version-0.1.6/vdt.version.egg-info/zip-safe
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.614934 vdt.version-0.1.7/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     1491 2024-05-14 07:17:41.000000 vdt.version-0.1.7/LICENSE
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      318 2024-05-14 07:36:19.614814 vdt.version-0.1.7/PKG-INFO
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     4380 2024-05-14 07:17:41.000000 vdt.version-0.1.7/README.rst
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       38 2024-05-14 07:36:19.614973 vdt.version-0.1.7/setup.cfg
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      798 2024-05-14 07:17:41.000000 vdt.version-0.1.7/setup.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.612962 vdt.version-0.1.7/vdt/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       56 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/__init__.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.614657 vdt.version-0.1.7/vdt/version/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/__init__.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2919 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/main.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2215 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/repo.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     4284 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/shared.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2965 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/utils.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.613996 vdt.version-0.1.7/vdt.version.egg-info/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      318 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/PKG-INFO
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      436 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       50 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/entry_points.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        4 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/namespace_packages.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       67 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/requires.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        4 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/top_level.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:18:21.000000 vdt.version-0.1.7/vdt.version.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vdt.version-0.1.6/README.rst` & `vdt.version-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `vdt.version-0.1.6/setup.py` & `vdt.version-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 from setuptools import find_packages, setup
 
 pkgname = "vdt.version"
 
 setup(name=pkgname,
-      version="0.1.6",
+      version="0.1.7",
       description="Version Increment Tool for GIT",
       author="Lars van de Kerkhof",
       author_email="lars@devopsconsulting.nl",
       maintainer="Lars van de Kerkhof",
       maintainer_email="lars@devopsconsulting.nl",
       url="https://github.com/devopsconsulting/vdt.version",
       packages=find_packages(),
```

### Comparing `vdt.version-0.1.6/vdt/version/main.py` & `vdt.version-0.1.7/vdt/version/main.py`

 * *Files identical despite different names*

### Comparing `vdt.version-0.1.6/vdt/version/repo.py` & `vdt.version-0.1.7/vdt/version/repo.py`

 * *Files identical despite different names*

### Comparing `vdt.version-0.1.6/vdt/version/shared.py` & `vdt.version-0.1.7/vdt/version/shared.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The functions and objects in this file can be used in your plugins.
 """
+from functools import total_ordering
 import contextlib
 import logging
 import os.path
 import subprocess
 import sys
 
 
@@ -50,14 +51,15 @@
 class VersionError(Exception):
     pass
 
 class VersionNotFound(VersionError):
     pass
 
 
+@total_ordering
 class Version(object):
     """
     Represent a version object with a nice
     interface for incrementing.
     
     >>> a = Version('1.2.3-koe-4646', extra_args=['hai'])
     >>> a.extra_args
@@ -73,14 +75,28 @@
     '4.0.0-koe-4646'
     >>> a.build_tag = 'lol'
     >>> str(a)
     '4.0.0-lol-4646'
     >>> a.build_number = 876876
     >>> str(a)
     '4.0.0-lol-876876'
+    >>> b = Version('4.0.0-lol-8768778')
+    >>> b == a
+    True
+    >>> b >= a
+    True
+    >>> b.major += 1
+    >>> b > a
+    True
+    >>> b >= a
+    True
+    >>> b <= a
+    False
+    >>> b < a
+    False
     """
     def __init__(self, version_string, annotated=False, changelog="", extra_args=[], userdata={}):
         (version, self.build_tag, self.build_number) = \
             parse_version_string(version_string)
         
         version.extend([0, 0, 0])
         self._major = version[0]
@@ -110,14 +126,20 @@
         self._minor = value
         self.patch = 0
 
     @property
     def version(self):
         return [self._major, self._minor, self.patch]
 
+    def __eq__(self, other):
+        return self.version == other.version
+
+    def __lt__(self, other):
+        return self.version < other.version
+
     @property
     def changelog(self):
         if os.path.isfile(self._changelog):
             with open(self._changelog) as f:
                 changelog = f.read()
         else:
             changelog = self._changelog
```

### Comparing `vdt.version-0.1.6/vdt/version/utils.py` & `vdt.version-0.1.7/vdt/version/utils.py`

 * *Files identical despite different names*

