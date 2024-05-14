# Comparing `tmp/httpdiff-0.0.3.tar.gz` & `tmp/httpdiff-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpdiff-0.0.3.tar", last modified: Sun May 12 11:01:51 2024, max compression
+gzip compressed data, was "httpdiff-0.0.4.tar", last modified: Tue May 14 09:46:36 2024, max compression
```

## Comparing `httpdiff-0.0.3.tar` & `httpdiff-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2024-05-12 11:01:51.982637 httpdiff-0.0.3/
--rw-r--r--   0 william   (1000) william   (1000)     1078 2024-02-01 17:15:03.000000 httpdiff-0.0.3/LICENSE
--rw-r--r--   0 william   (1000) william   (1000)     7560 2024-05-12 11:01:51.982637 httpdiff-0.0.3/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)     7230 2024-05-12 10:59:56.000000 httpdiff-0.0.3/README.md
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2024-05-12 11:01:51.982637 httpdiff-0.0.3/httpdiff/
--rw-r--r--   0 william   (1000) william   (1000)      139 2024-05-11 19:15:44.000000 httpdiff-0.0.3/httpdiff/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)     8522 2024-05-11 19:15:44.000000 httpdiff-0.0.3/httpdiff/analyzer.py
--rw-r--r--   0 william   (1000) william   (1000)    12770 2024-05-11 19:15:44.000000 httpdiff-0.0.3/httpdiff/blob.py
--rw-r--r--   0 william   (1000) william   (1000)     5866 2024-05-11 19:15:44.000000 httpdiff-0.0.3/httpdiff/reflection.py
--rw-r--r--   0 william   (1000) william   (1000)      901 2024-05-11 19:15:44.000000 httpdiff-0.0.3/httpdiff/response.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2024-05-12 11:01:51.982637 httpdiff-0.0.3/httpdiff.egg-info/
--rw-r--r--   0 william   (1000) william   (1000)     7560 2024-05-12 11:01:51.000000 httpdiff-0.0.3/httpdiff.egg-info/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)      288 2024-05-12 11:01:51.000000 httpdiff-0.0.3/httpdiff.egg-info/SOURCES.txt
--rw-r--r--   0 william   (1000) william   (1000)        1 2024-05-12 11:01:51.000000 httpdiff-0.0.3/httpdiff.egg-info/dependency_links.txt
--rw-r--r--   0 william   (1000) william   (1000)       10 2024-05-12 11:01:51.000000 httpdiff-0.0.3/httpdiff.egg-info/requires.txt
--rw-r--r--   0 william   (1000) william   (1000)        9 2024-05-12 11:01:51.000000 httpdiff-0.0.3/httpdiff.egg-info/top_level.txt
--rw-r--r--   0 william   (1000) william   (1000)       38 2024-05-12 11:01:51.982637 httpdiff-0.0.3/setup.cfg
--rw-r--r--   0 william   (1000) william   (1000)      576 2024-05-12 11:01:46.000000 httpdiff-0.0.3/setup.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2024-05-14 09:46:36.628517 httpdiff-0.0.4/
+-rw-r--r--   0 william   (1000) william   (1000)     1078 2024-02-01 17:15:03.000000 httpdiff-0.0.4/LICENSE
+-rw-r--r--   0 william   (1000) william   (1000)     7556 2024-05-14 09:46:36.628517 httpdiff-0.0.4/PKG-INFO
+-rw-r--r--   0 william   (1000) william   (1000)     7230 2024-05-12 10:59:56.000000 httpdiff-0.0.4/README.md
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2024-05-14 09:46:36.628517 httpdiff-0.0.4/httpdiff/
+-rw-r--r--   0 william   (1000) william   (1000)      139 2024-05-11 19:15:44.000000 httpdiff-0.0.4/httpdiff/__init__.py
+-rw-r--r--   0 william   (1000) william   (1000)     8522 2024-05-11 19:15:44.000000 httpdiff-0.0.4/httpdiff/analyzer.py
+-rw-r--r--   0 william   (1000) william   (1000)    12770 2024-05-11 19:15:44.000000 httpdiff-0.0.4/httpdiff/blob.py
+-rw-r--r--   0 william   (1000) william   (1000)     5866 2024-05-11 19:15:44.000000 httpdiff-0.0.4/httpdiff/reflection.py
+-rw-r--r--   0 william   (1000) william   (1000)      901 2024-05-11 19:15:44.000000 httpdiff-0.0.4/httpdiff/response.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2024-05-14 09:46:36.628517 httpdiff-0.0.4/httpdiff.egg-info/
+-rw-r--r--   0 william   (1000) william   (1000)     7556 2024-05-14 09:46:36.000000 httpdiff-0.0.4/httpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 william   (1000) william   (1000)      288 2024-05-14 09:46:36.000000 httpdiff-0.0.4/httpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 william   (1000) william   (1000)        1 2024-05-14 09:46:36.000000 httpdiff-0.0.4/httpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 william   (1000) william   (1000)       10 2024-05-14 09:46:36.000000 httpdiff-0.0.4/httpdiff.egg-info/requires.txt
+-rw-r--r--   0 william   (1000) william   (1000)        9 2024-05-14 09:46:36.000000 httpdiff-0.0.4/httpdiff.egg-info/top_level.txt
+-rw-r--r--   0 william   (1000) william   (1000)       38 2024-05-14 09:46:36.628517 httpdiff-0.0.4/setup.cfg
+-rw-r--r--   0 william   (1000) william   (1000)      595 2024-05-14 09:46:31.000000 httpdiff-0.0.4/setup.py
```

### Comparing `httpdiff-0.0.3/LICENSE` & `httpdiff-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `httpdiff-0.0.3/PKG-INFO` & `httpdiff-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: httpdiff
-Version: 0.0.3
+Version: 0.0.4
 Summary: HTTPDiff - Finding differences between HTTP responses
 Home-page: UNKNOWN
 Author: William Kristoffersen
 Author-email: william.kristof@gmail.com
-License: UNKNOWN
+License: MIT
 Keywords: python,httpdiff
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HTTPDiff
```

### Comparing `httpdiff-0.0.3/README.md` & `httpdiff-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `httpdiff-0.0.3/httpdiff/analyzer.py` & `httpdiff-0.0.4/httpdiff/analyzer.py`

 * *Files identical despite different names*

### Comparing `httpdiff-0.0.3/httpdiff/blob.py` & `httpdiff-0.0.4/httpdiff/blob.py`

 * *Files identical despite different names*

### Comparing `httpdiff-0.0.3/httpdiff/reflection.py` & `httpdiff-0.0.4/httpdiff/reflection.py`

 * *Files identical despite different names*

### Comparing `httpdiff-0.0.3/httpdiff/response.py` & `httpdiff-0.0.4/httpdiff/response.py`

 * *Files identical despite different names*

### Comparing `httpdiff-0.0.3/httpdiff.egg-info/PKG-INFO` & `httpdiff-0.0.4/httpdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: httpdiff
-Version: 0.0.3
+Version: 0.0.4
 Summary: HTTPDiff - Finding differences between HTTP responses
 Home-page: UNKNOWN
 Author: William Kristoffersen
 Author-email: william.kristof@gmail.com
-License: UNKNOWN
+License: MIT
 Keywords: python,httpdiff
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HTTPDiff
```

### Comparing `httpdiff-0.0.3/setup.py` & `httpdiff-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "HTTPDiff - Finding differences between HTTP responses"
 
 setup(
     name="httpdiff",
     version=VERSION,
     author="William Kristoffersen",
     author_email="william.kristof@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["rapidfuzz"],
     keywords=["python", "httpdiff"],
     classifiers=[],
+    license="MIT",
 )
```

