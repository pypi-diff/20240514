# Comparing `tmp/dalgorithms-0.1.0.tar.gz` & `tmp/dalgorithms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalgorithms-0.1.0.tar", last modified: Mon May 13 22:42:36 2024, max compression
+gzip compressed data, was "dalgorithms-0.1.1.tar", last modified: Mon May 13 23:21:45 2024, max compression
```

## Comparing `dalgorithms-0.1.0.tar` & `dalgorithms-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 22:42:36.668988 dalgorithms-0.1.0/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      836 2024-05-13 22:42:36.667988 dalgorithms-0.1.0/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       22 2024-05-06 18:11:07.000000 dalgorithms-0.1.0/README.md
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 22:42:36.665988 dalgorithms-0.1.0/algorithms/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      153 2024-05-13 21:48:44.000000 dalgorithms-0.1.0/algorithms/__init__.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     6136 2024-05-13 22:21:35.000000 dalgorithms-0.1.0/algorithms/huffman.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2200 2024-05-13 22:23:14.000000 dalgorithms-0.1.0/algorithms/lzw.py
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 22:42:36.667988 dalgorithms-0.1.0/dalgorithms.egg-info/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      836 2024-05-13 22:42:36.000000 dalgorithms-0.1.0/dalgorithms.egg-info/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      255 2024-05-13 22:42:36.000000 dalgorithms-0.1.0/dalgorithms.egg-info/SOURCES.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-13 22:42:36.000000 dalgorithms-0.1.0/dalgorithms.egg-info/dependency_links.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-13 22:42:36.000000 dalgorithms-0.1.0/dalgorithms.egg-info/requires.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-13 22:42:36.000000 dalgorithms-0.1.0/dalgorithms.egg-info/top_level.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-13 22:42:36.668988 dalgorithms-0.1.0/setup.cfg
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1103 2024-05-13 22:42:34.000000 dalgorithms-0.1.0/setup.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 23:21:45.532020 dalgorithms-0.1.1/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      836 2024-05-13 23:21:45.532020 dalgorithms-0.1.1/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       22 2024-05-06 18:11:07.000000 dalgorithms-0.1.1/README.md
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 23:21:45.530020 dalgorithms-0.1.1/algorithms/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      153 2024-05-13 21:48:44.000000 dalgorithms-0.1.1/algorithms/__init__.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2871 2024-05-13 22:03:56.000000 dalgorithms-0.1.1/algorithms/deflate.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     6136 2024-05-13 22:21:35.000000 dalgorithms-0.1.1/algorithms/huffman.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     3049 2024-05-13 21:57:15.000000 dalgorithms-0.1.1/algorithms/lz77.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       89 2024-05-13 21:46:27.000000 dalgorithms-0.1.1/algorithms/lz78.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2200 2024-05-13 22:23:14.000000 dalgorithms-0.1.1/algorithms/lzw.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 23:21:45.531020 dalgorithms-0.1.1/dalgorithms.egg-info/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      836 2024-05-13 23:21:45.000000 dalgorithms-0.1.1/dalgorithms.egg-info/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      315 2024-05-13 23:21:45.000000 dalgorithms-0.1.1/dalgorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-13 23:21:45.000000 dalgorithms-0.1.1/dalgorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-13 23:21:45.000000 dalgorithms-0.1.1/dalgorithms.egg-info/requires.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       11 2024-05-13 23:21:45.000000 dalgorithms-0.1.1/dalgorithms.egg-info/top_level.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-13 23:21:45.532020 dalgorithms-0.1.1/setup.cfg
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1085 2024-05-13 23:21:29.000000 dalgorithms-0.1.1/setup.py
```

### Comparing `dalgorithms-0.1.0/PKG-INFO` & `dalgorithms-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalgorithms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Compress algorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dalgorithms-0.1.0/algorithms/huffman.py` & `dalgorithms-0.1.1/algorithms/huffman.py`

 * *Files identical despite different names*

### Comparing `dalgorithms-0.1.0/algorithms/lzw.py` & `dalgorithms-0.1.1/algorithms/lzw.py`

 * *Files identical despite different names*

### Comparing `dalgorithms-0.1.0/dalgorithms.egg-info/PKG-INFO` & `dalgorithms-0.1.1/dalgorithms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalgorithms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Compress algorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dalgorithms-0.1.0/setup.py` & `dalgorithms-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 '''Setup'''
 from setuptools import setup, find_packages
 
 LONG_DESCRIPTION = 'A package that allows to compress different types of data using different algorithms such as LZW, LZ78, Deflate, Huffman'
 
 setup(
     name="dalgorithms",
-    version="0.1.0",
+    version="0.1.1",
     author="UCUgllekk",
     author_email="pavlosiuk.pn@ucu.edu.ua",
     description='Compress algorithms',
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
-    packages=find_packages(where="algorithms"),
+    packages=find_packages(),
     url="https://github.com/UCUgllekk/compression_research",
     install_requires=["tk>=0.1.0"],
     extras_require={
         "dev": ["twine>=4.0.2"]},
     keywords=['python', 'compress', 'compression', 'algorithm',
               'lz78', 'lzw', 'huffman', 'deflate'],
     classifiers=[
```

