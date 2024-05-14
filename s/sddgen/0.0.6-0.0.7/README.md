# Comparing `tmp/sddgen-0.0.6.tar.gz` & `tmp/sddgen-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddgen-0.0.6.tar", last modified: Tue May 14 06:53:11 2024, max compression
+gzip compressed data, was "sddgen-0.0.7.tar", last modified: Tue May 14 06:59:12 2024, max compression
```

## Comparing `sddgen-0.0.6.tar` & `sddgen-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:53:11.436047 sddgen-0.0.6/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      228 2024-05-14 06:53:11.436047 sddgen-0.0.6/PKG-INFO
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:53:11.436047 sddgen-0.0.6/scripts/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     2342 2024-05-14 06:44:15.000000 sddgen-0.0.6/scripts/sdd-gencode.py
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:53:11.436047 sddgen-0.0.6/sddgen/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      299 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/__init__.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      166 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/cgeom.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      421 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/datarep.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     8061 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/generator.py
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:53:11.436047 sddgen-0.0.6/sddgen/guitk/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      244 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/guitk/__init__.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)    11871 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/guitk/generator.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     6241 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/guitk/guiComponents.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)     4658 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/htmlcss.py
--rw-rw-r--   0 tkono     (1000) tkono     (1000)    11334 2024-05-14 06:44:15.000000 sddgen-0.0.6/sddgen/model.py
-drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:53:11.436047 sddgen-0.0.6/sddgen.egg-info/
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      228 2024-05-14 06:53:11.000000 sddgen-0.0.6/sddgen.egg-info/PKG-INFO
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      396 2024-05-14 06:53:11.000000 sddgen-0.0.6/sddgen.egg-info/SOURCES.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)        1 2024-05-14 06:53:11.000000 sddgen-0.0.6/sddgen.egg-info/dependency_links.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)       21 2024-05-14 06:53:11.000000 sddgen-0.0.6/sddgen.egg-info/requires.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)        7 2024-05-14 06:53:11.000000 sddgen-0.0.6/sddgen.egg-info/top_level.txt
--rw-rw-r--   0 tkono     (1000) tkono     (1000)      326 2024-05-14 06:53:11.436047 sddgen-0.0.6/setup.cfg
--rw-rw-r--   0 tkono     (1000) tkono     (1000)       38 2024-05-14 06:44:15.000000 sddgen-0.0.6/setup.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:59:12.128984 sddgen-0.0.7/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      228 2024-05-14 06:59:12.128984 sddgen-0.0.7/PKG-INFO
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:59:12.128984 sddgen-0.0.7/scripts/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     2342 2024-05-14 06:44:15.000000 sddgen-0.0.7/scripts/sdd-gencode.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:59:12.128984 sddgen-0.0.7/sddgen/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      299 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/__init__.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      166 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/cgeom.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      421 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/datarep.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     8061 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/generator.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:59:12.128984 sddgen-0.0.7/sddgen/guitk/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      244 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/guitk/__init__.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)    11871 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/guitk/generator.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     6241 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/guitk/guiComponents.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)     4658 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/htmlcss.py
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)    11334 2024-05-14 06:44:15.000000 sddgen-0.0.7/sddgen/model.py
+drwxrwxr-x   0 tkono     (1000) tkono     (1000)        0 2024-05-14 06:59:12.128984 sddgen-0.0.7/sddgen.egg-info/
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      228 2024-05-14 06:59:12.000000 sddgen-0.0.7/sddgen.egg-info/PKG-INFO
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      396 2024-05-14 06:59:12.000000 sddgen-0.0.7/sddgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)        1 2024-05-14 06:59:12.000000 sddgen-0.0.7/sddgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)       13 2024-05-14 06:59:12.000000 sddgen-0.0.7/sddgen.egg-info/requires.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)        7 2024-05-14 06:59:12.000000 sddgen-0.0.7/sddgen.egg-info/top_level.txt
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)      317 2024-05-14 06:59:12.128984 sddgen-0.0.7/setup.cfg
+-rw-rw-r--   0 tkono     (1000) tkono     (1000)       38 2024-05-14 06:44:15.000000 sddgen-0.0.7/setup.py
```

### Comparing `sddgen-0.0.6/scripts/sdd-gencode.py` & `sddgen-0.0.7/scripts/sdd-gencode.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.6/sddgen/generator.py` & `sddgen-0.0.7/sddgen/generator.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.6/sddgen/guitk/generator.py` & `sddgen-0.0.7/sddgen/guitk/generator.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.6/sddgen/guitk/guiComponents.py` & `sddgen-0.0.7/sddgen/guitk/guiComponents.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.6/sddgen/htmlcss.py` & `sddgen-0.0.7/sddgen/htmlcss.py`

 * *Files identical despite different names*

### Comparing `sddgen-0.0.6/sddgen/model.py` & `sddgen-0.0.7/sddgen/model.py`

 * *Files identical despite different names*

