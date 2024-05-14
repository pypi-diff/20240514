# Comparing `tmp/cvprocessor-0.3.1.tar.gz` & `tmp/cvprocessor-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.3.1.tar", last modified: Sat May 11 00:43:29 2024, max compression
+gzip compressed data, was "cvprocessor-0.5.0.tar", last modified: Tue May 14 06:29:59 2024, max compression
```

## Comparing `cvprocessor-0.3.1.tar` & `cvprocessor-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:43:29.329152 cvprocessor-0.3.1/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.3.1/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-11 00:43:29.328558 cvprocessor-0.3.1/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.3.1/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-11 00:42:49.000000 cvprocessor-0.3.1/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-11 00:43:29.329289 cvprocessor-0.3.1/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:43:29.306964 cvprocessor-0.3.1/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:43:29.324132 cvprocessor-0.3.1/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.3.1/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.3.1/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.3.1/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     4722 2024-05-11 00:25:04.000000 cvprocessor-0.3.1/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.3.1/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     4633 2024-05-08 08:22:41.000000 cvprocessor-0.3.1/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.3.1/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     4581 2024-05-10 10:56:41.000000 cvprocessor-0.3.1/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.3.1/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1533 2024-05-09 01:57:53.000000 cvprocessor-0.3.1/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.3.1/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.3.1/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1866 2024-05-09 02:04:48.000000 cvprocessor-0.3.1/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.3.1/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     1980 2024-05-09 01:44:15.000000 cvprocessor-0.3.1/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2288 2024-05-09 01:28:30.000000 cvprocessor-0.3.1/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.3.1/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.3.1/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     6530 2024-05-11 00:42:16.000000 cvprocessor-0.3.1/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:43:29.327894 cvprocessor-0.3.1/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-11 00:43:29.000000 cvprocessor-0.3.1/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-11 00:43:29.000000 cvprocessor-0.3.1/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-11 00:43:29.000000 cvprocessor-0.3.1/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-11 00:43:29.000000 cvprocessor-0.3.1/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-11 00:43:29.000000 cvprocessor-0.3.1/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:29:59.586430 cvprocessor-0.5.0/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.0/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:29:59.586064 cvprocessor-0.5.0/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.0/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 05:58:13.000000 cvprocessor-0.5.0/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 06:29:59.586493 cvprocessor-0.5.0/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:29:59.570339 cvprocessor-0.5.0/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:29:59.582836 cvprocessor-0.5.0/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.0/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7926 2024-05-14 06:19:48.000000 cvprocessor-0.5.0/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.0/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6464 2024-05-14 06:28:52.000000 cvprocessor-0.5.0/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.0/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.0/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.0/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5427 2024-05-14 06:16:10.000000 cvprocessor-0.5.0/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.0/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.0/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.0/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    15416 2024-05-14 06:23:44.000000 cvprocessor-0.5.0/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.0/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.0/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.0/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.0/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4907 2024-05-14 06:11:22.000000 cvprocessor-0.5.0/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.0/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.0/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:29:59.585609 cvprocessor-0.5.0/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:29:59.000000 cvprocessor-0.5.0/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 06:29:59.000000 cvprocessor-0.5.0/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 06:29:59.000000 cvprocessor-0.5.0/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 06:29:59.000000 cvprocessor-0.5.0/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 06:29:59.000000 cvprocessor-0.5.0/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.3.1/LICENSE` & `cvprocessor-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.3.1/PKG-INFO` & `cvprocessor-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.3.1
+Version: 0.5.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.3.1/README.md` & `cvprocessor-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.3.1/pyproject.toml` & `cvprocessor-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.3.1"
+version = "0.5.0"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.3.1/src/cvprocessor/intro.py` & `cvprocessor-0.5.0/src/cvprocessor/intro.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,49 @@
-# Introduction class that receives information given a pandas dataframe
+"""
+This module contains the class Intro, which is used to store the introduction
+"""
 import pandas as pd
 
 
 class Intro:
-    def __init__(self, filename):
-        self._filename = filename
-        self._short_summary = None
-        self._long_summary = None
-        self._job_title = None
-        self._tagline = None
-        self._intro = self._get_intro()
-        self.load_intro()
-
-    @property
-    def intro(self):
-        return self._intro
-
-    @property
-    def filename(self):
-        return self._filename
-
-    @property
-    def short_summary(self):
-        return self._short_summary
-
-    @property
-    def long_summary(self):
-        return self._long_summary
-
-    @property
-    def job_title(self):
-        return self._job_title
-
-    @property
-    def tagline(self):
-        return self._tagline
-
-    def _get_intro(self):
-        return pd.read_excel(self.filename, sheet_name="Intro")
-
-    def load_intro(self):
-        self._short_summary = self.intro["Short summary"].values[0]
-        self._long_summary = self.intro["Welcome"].values[0]
-        # self._job_title = self.intro["Jobtitle"].values[0]
-        self._tagline = self.intro["Tagline"].values[0]
+    """
+    The Intro class is used to store the introduction of the CV file.
+
+    Attributes:
+    short_summary (str): A short summary of the CV file.
+    long_summary (str): A long summary of the CV file.
+    tagline (str): A tagline of the CV file.
+
+    Methods:
+    __init__(filename): Initializes the Intro class by loading the introduction from the given file.
+    __str__(): Returns a string representation of the Intro class.
+    __repr__(): Returns a string representation of the Intro class.
+    """
+
+    def __init__(self):
+        self.short_summary = None
+        self.long_summary = None
+        self.tagline = None
+
+    def load(self, filename):
+        """
+        Load the introduction from the given file.
+        """
+        intro = pd.read_excel(filename, sheet_name="Intro")
+        self.short_summary = intro["Short summary"].values[0]
+        self.long_summary = intro["Welcome"].values[0]
+        self.tagline = intro["Tagline"].values[0]
 
     def __str__(self) -> str:
         string = f"Short summary: {self.short_summary}\n"
         string += f"Long summary: {self.long_summary}\n"
-        string += f"Job title: {self.job_title}\n"
         string += f"Tagline: {self.tagline}\n\n"
         return string
 
     def __repr__(self) -> str:
-        repr = f"Intro(filename={self.filename}, short_summary={self.short_summary}, long_summary={self.long_summary}, job_title={self.job_title}, tagline={self.tagline})"
-        return repr
+        string = (
+            f"Intro("
+            f"short_summary={self.short_summary}, "
+            f"long_summary={self.long_summary}, "
+            f"tagline={self.tagline})"
+        )
+        return string
```

### Comparing `cvprocessor-0.3.1/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.5.0/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.3.1
+Version: 0.5.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.3.1/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.5.0/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

