# Comparing `tmp/sddgen-0.0.8.tar.gz` & `tmp/sddgen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddgen-0.0.8.tar", last modified: Tue May 14 07:03:04 2024, max compression
+gzip compressed data, was "sddgen-0.0.9.tar", last modified: Tue May 14 07:07:24 2024, max compression
```

## Comparing `sddgen-0.0.8.tar` & `sddgen-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:03:04.929413 sddgen-0.0.8/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      229 2024-05-14 07:03:04.929413 sddgen-0.0.8/PKG-INFO
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:03:04.929413 sddgen-0.0.8/scripts/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     2342 2024-05-14 06:44:15.000000 sddgen-0.0.8/scripts/sdd-gencode.py
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:03:04.929413 sddgen-0.0.8/sddgen/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      299 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/__init__.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      166 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/cgeom.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      421 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/datarep.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     8061 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/generator.py
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:03:04.929413 sddgen-0.0.8/sddgen/guitk/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      244 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/guitk/__init__.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)    11871 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/guitk/generator.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     6241 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/guitk/guiComponents.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     4658 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/htmlcss.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)    11334 2024-05-14 06:44:15.000000 sddgen-0.0.8/sddgen/model.py
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:03:04.929413 sddgen-0.0.8/sddgen.egg-info/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      229 2024-05-14 07:03:04.000000 sddgen-0.0.8/sddgen.egg-info/PKG-INFO
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      396 2024-05-14 07:03:04.000000 sddgen-0.0.8/sddgen.egg-info/SOURCES.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)        1 2024-05-14 07:03:04.000000 sddgen-0.0.8/sddgen.egg-info/dependency_links.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)       13 2024-05-14 07:03:04.000000 sddgen-0.0.8/sddgen.egg-info/requires.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)        7 2024-05-14 07:03:04.000000 sddgen-0.0.8/sddgen.egg-info/top_level.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      318 2024-05-14 07:03:04.929413 sddgen-0.0.8/setup.cfg
--rw-rw-r--   0 tkono     (1000) tkono     (1000)       38 2024-05-14 06:44:15.000000 sddgen-0.0.8/setup.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:07:24.593799 sddgen-0.0.9/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      229 2024-05-14 07:07:24.593799 sddgen-0.0.9/PKG-INFO
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:07:24.593799 sddgen-0.0.9/scripts/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     2342 2024-05-14 06:44:15.000000 sddgen-0.0.9/scripts/sdd-gencode.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:07:24.593799 sddgen-0.0.9/sddgen/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      299 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/__init__.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      166 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/cgeom.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      421 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/datarep.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     8061 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/generator.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:07:24.593799 sddgen-0.0.9/sddgen/guitk/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      244 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/guitk/__init__.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)    11871 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/guitk/generator.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     6241 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/guitk/guiComponents.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     4658 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/htmlcss.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)    11334 2024-05-14 06:44:15.000000 sddgen-0.0.9/sddgen/model.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 07:07:24.593799 sddgen-0.0.9/sddgen.egg-info/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      229 2024-05-14 07:07:24.000000 sddgen-0.0.9/sddgen.egg-info/PKG-INFO
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      396 2024-05-14 07:07:24.000000 sddgen-0.0.9/sddgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)        1 2024-05-14 07:07:24.000000 sddgen-0.0.9/sddgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)        7 2024-05-14 07:07:24.000000 sddgen-0.0.9/sddgen.egg-info/requires.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)        7 2024-05-14 07:07:24.000000 sddgen-0.0.9/sddgen.egg-info/top_level.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      310 2024-05-14 07:07:24.593799 sddgen-0.0.9/setup.cfg
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)       38 2024-05-14 06:44:15.000000 sddgen-0.0.9/setup.py
```

### Comparing `sddgen-0.0.8/scripts/sdd-gencode.py` & `sddgen-0.0.9/scripts/sdd-gencode.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.8/sddgen/generator.py` & `sddgen-0.0.9/sddgen/generator.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.8/sddgen/guitk/generator.py` & `sddgen-0.0.9/sddgen/guitk/generator.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.8/sddgen/guitk/guiComponents.py` & `sddgen-0.0.9/sddgen/guitk/guiComponents.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.8/sddgen/htmlcss.py` & `sddgen-0.0.9/sddgen/htmlcss.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.8/sddgen/model.py` & `sddgen-0.0.9/sddgen/model.py`

 * *Files identical despite different names*

