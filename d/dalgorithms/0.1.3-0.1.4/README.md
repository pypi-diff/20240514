# Comparing `tmp/dalgorithms-0.1.3.tar.gz` & `tmp/dalgorithms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalgorithms-0.1.3.tar", last modified: Tue May 14 00:40:40 2024, max compression
+gzip compressed data, was "dalgorithms-0.1.4.tar", last modified: Tue May 14 00:47:58 2024, max compression
```

## Comparing `dalgorithms-0.1.3.tar` & `dalgorithms-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:40:40.930708 dalgorithms-0.1.3/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      828 2024-05-14 00:40:40.930708 dalgorithms-0.1.3/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       22 2024-05-06 18:11:07.000000 dalgorithms-0.1.3/README.md
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:40:40.927708 dalgorithms-0.1.3/algorithms/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      147 2024-05-14 00:23:21.000000 dalgorithms-0.1.3/algorithms/__init__.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2871 2024-05-14 00:23:21.000000 dalgorithms-0.1.3/algorithms/deflate.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     6256 2024-05-14 00:29:09.000000 dalgorithms-0.1.3/algorithms/huffman.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     3049 2024-05-14 00:23:21.000000 dalgorithms-0.1.3/algorithms/lz77.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       89 2024-05-14 00:23:21.000000 dalgorithms-0.1.3/algorithms/lz78.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2201 2024-05-14 00:23:21.000000 dalgorithms-0.1.3/algorithms/lzw.py
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:40:40.929708 dalgorithms-0.1.3/dalgorithms.egg-info/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      828 2024-05-14 00:40:40.000000 dalgorithms-0.1.3/dalgorithms.egg-info/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      334 2024-05-14 00:40:40.000000 dalgorithms-0.1.3/dalgorithms.egg-info/SOURCES.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-14 00:40:40.000000 dalgorithms-0.1.3/dalgorithms.egg-info/dependency_links.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-14 00:40:40.000000 dalgorithms-0.1.3/dalgorithms.egg-info/requires.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       11 2024-05-14 00:40:40.000000 dalgorithms-0.1.3/dalgorithms.egg-info/top_level.txt
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:40:40.929708 dalgorithms-0.1.3/other_files/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     8194 2024-05-14 00:37:29.000000 dalgorithms-0.1.3/other_files/app.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-14 00:40:40.930708 dalgorithms-0.1.3/setup.cfg
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1077 2024-05-14 00:39:58.000000 dalgorithms-0.1.3/setup.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:47:58.991803 dalgorithms-0.1.4/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      828 2024-05-14 00:47:58.990803 dalgorithms-0.1.4/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       22 2024-05-06 18:11:07.000000 dalgorithms-0.1.4/README.md
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:47:58.987803 dalgorithms-0.1.4/algorithms/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      131 2024-05-14 00:46:41.000000 dalgorithms-0.1.4/algorithms/__init__.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2871 2024-05-14 00:23:21.000000 dalgorithms-0.1.4/algorithms/deflate.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     6256 2024-05-14 00:29:09.000000 dalgorithms-0.1.4/algorithms/huffman.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     3049 2024-05-14 00:23:21.000000 dalgorithms-0.1.4/algorithms/lz77.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       89 2024-05-14 00:23:21.000000 dalgorithms-0.1.4/algorithms/lz78.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2201 2024-05-14 00:23:21.000000 dalgorithms-0.1.4/algorithms/lzw.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:47:58.989802 dalgorithms-0.1.4/dalgorithms.egg-info/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      828 2024-05-14 00:47:58.000000 dalgorithms-0.1.4/dalgorithms.egg-info/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      334 2024-05-14 00:47:58.000000 dalgorithms-0.1.4/dalgorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-14 00:47:58.000000 dalgorithms-0.1.4/dalgorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-14 00:47:58.000000 dalgorithms-0.1.4/dalgorithms.egg-info/requires.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       11 2024-05-14 00:47:58.000000 dalgorithms-0.1.4/dalgorithms.egg-info/top_level.txt
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 00:47:58.989802 dalgorithms-0.1.4/other_files/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     8194 2024-05-14 00:37:29.000000 dalgorithms-0.1.4/other_files/app.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-14 00:47:58.991803 dalgorithms-0.1.4/setup.cfg
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1065 2024-05-14 00:47:44.000000 dalgorithms-0.1.4/setup.py
```

### Comparing `dalgorithms-0.1.3/PKG-INFO` & `dalgorithms-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalgorithms
-Version: 0.1.3
+Version: 0.1.4
 Summary: dalgorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dalgorithms-0.1.3/algorithms/deflate.py` & `dalgorithms-0.1.4/algorithms/deflate.py`

 * *Files identical despite different names*

### Comparing `dalgorithms-0.1.3/algorithms/huffman.py` & `dalgorithms-0.1.4/algorithms/huffman.py`

 * *Files identical despite different names*

### Comparing `dalgorithms-0.1.3/algorithms/lz77.py` & `dalgorithms-0.1.4/algorithms/lz77.py`

 * *Files identical despite different names*

### Comparing `dalgorithms-0.1.3/algorithms/lzw.py` & `dalgorithms-0.1.4/algorithms/lzw.py`

 * *Files identical despite different names*

### Comparing `dalgorithms-0.1.3/dalgorithms.egg-info/PKG-INFO` & `dalgorithms-0.1.4/dalgorithms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalgorithms
-Version: 0.1.3
+Version: 0.1.4
 Summary: dalgorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dalgorithms-0.1.3/other_files/app.py` & `dalgorithms-0.1.4/other_files/app.py`

 * *Files identical despite different names*

### Comparing `dalgorithms-0.1.3/setup.py` & `dalgorithms-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-'''Setup'''
 from setuptools import setup, find_packages
 
 LONG_DESCRIPTION = 'A package that allows to compress different types of data using different algorithms such as LZW, LZ78, Deflate, Huffman'
 
 setup(
     name="dalgorithms",
-    version="0.1.3",
+    version="0.1.4",
     author="UCUgllekk",
     author_email="pavlosiuk.pn@ucu.edu.ua",
     description='dalgorithms',
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     url="https://github.com/UCUgllekk/compression_research",
```

