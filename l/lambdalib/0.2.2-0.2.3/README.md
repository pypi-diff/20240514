# Comparing `tmp/lambdalib-0.2.2.tar.gz` & `tmp/lambdalib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambdalib-0.2.2.tar", last modified: Fri Apr 19 18:41:52 2024, max compression
+gzip compressed data, was "lambdalib-0.2.3.tar", last modified: Tue May 14 20:06:37 2024, max compression
```

## Comparing `lambdalib-0.2.2.tar` & `lambdalib-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:52.708879 lambdalib-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 18:41:48.000000 lambdalib-0.2.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 18:41:48.000000 lambdalib-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-19 18:41:48.000000 lambdalib-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-19 18:41:48.000000 lambdalib-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-19 18:41:52.708879 lambdalib-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-19 18:41:48.000000 lambdalib-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:52.704879 lambdalib-0.2.2/lambdalib/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-19 18:41:48.000000 lambdalib-0.2.2/lambdalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:52.704879 lambdalib-0.2.2/lambdalib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-19 18:41:48.000000 lambdalib-0.2.2/lambdalib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:52.704879 lambdalib-0.2.2/lambdalib/utils/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-19 18:41:48.000000 lambdalib-0.2.2/lambdalib/utils/templates/la_spmemory.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:52.704879 lambdalib-0.2.2/lambdalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-19 18:41:52.000000 lambdalib-0.2.2/lambdalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 18:41:52.000000 lambdalib-0.2.2/lambdalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:41:52.000000 lambdalib-0.2.2/lambdalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 18:41:52.000000 lambdalib-0.2.2/lambdalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 18:41:52.000000 lambdalib-0.2.2/lambdalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 18:41:48.000000 lambdalib-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:41:52.708879 lambdalib-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:06:37.247604 lambdalib-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 20:06:33.000000 lambdalib-0.2.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 20:06:33.000000 lambdalib-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 20:06:33.000000 lambdalib-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 20:06:33.000000 lambdalib-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-14 20:06:37.247604 lambdalib-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-14 20:06:33.000000 lambdalib-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:06:37.243604 lambdalib-0.2.3/lambdalib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-14 20:06:33.000000 lambdalib-0.2.3/lambdalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:06:37.243604 lambdalib-0.2.3/lambdalib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-14 20:06:33.000000 lambdalib-0.2.3/lambdalib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:06:37.243604 lambdalib-0.2.3/lambdalib/utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-14 20:06:33.000000 lambdalib-0.2.3/lambdalib/utils/templates/la_spmemory.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:06:37.247604 lambdalib-0.2.3/lambdalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-14 20:06:37.000000 lambdalib-0.2.3/lambdalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 20:06:37.000000 lambdalib-0.2.3/lambdalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:06:37.000000 lambdalib-0.2.3/lambdalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 20:06:37.000000 lambdalib-0.2.3/lambdalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 20:06:37.000000 lambdalib-0.2.3/lambdalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 20:06:33.000000 lambdalib-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:06:37.247604 lambdalib-0.2.3/setup.cfg
```

### Comparing `lambdalib-0.2.2/LICENSE` & `lambdalib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.2/PKG-INFO` & `lambdalib-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdalib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Standardized ASIC design libraries
 Author: Zero ASIC
 License: MIT License
         
         Copyright (c) 2023 Zero ASIC Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `lambdalib-0.2.2/README.md` & `lambdalib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.2/lambdalib/__init__.py` & `lambdalib-0.2.3/lambdalib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from siliconcompiler import Chip, Library
 import siliconcompiler.package as sc_package
 import glob
 import os
 import shutil
-__version__ = "0.2.2"
+
+__version__ = "0.2.3"
 
 _libraries = (
     'iolib',
     'stdlib',
     'ramlib',
     'padring',
     'syslib',
```

### Comparing `lambdalib-0.2.2/lambdalib/utils/__init__.py` & `lambdalib-0.2.3/lambdalib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.2/lambdalib/utils/templates/la_spmemory.v` & `lambdalib-0.2.3/lambdalib/utils/templates/la_spmemory.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.2/lambdalib.egg-info/PKG-INFO` & `lambdalib-0.2.3/lambdalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdalib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Standardized ASIC design libraries
 Author: Zero ASIC
 License: MIT License
         
         Copyright (c) 2023 Zero ASIC Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `lambdalib-0.2.2/pyproject.toml` & `lambdalib-0.2.3/pyproject.toml`

 * *Files identical despite different names*

