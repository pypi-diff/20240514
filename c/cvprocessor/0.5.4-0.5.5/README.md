# Comparing `tmp/cvprocessor-0.5.4.tar.gz` & `tmp/cvprocessor-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.5.4.tar", last modified: Tue May 14 07:06:08 2024, max compression
+gzip compressed data, was "cvprocessor-0.5.5.tar", last modified: Tue May 14 07:38:09 2024, max compression
```

## Comparing `cvprocessor-0.5.4.tar` & `cvprocessor-0.5.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:06:08.846519 cvprocessor-0.5.4/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.4/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 07:06:08.846111 cvprocessor-0.5.4/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.4/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 07:05:24.000000 cvprocessor-0.5.4/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 07:06:08.846595 cvprocessor-0.5.4/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:06:08.828525 cvprocessor-0.5.4/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:06:08.842534 cvprocessor-0.5.4/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.4/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.4/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.4/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     7051 2024-05-14 06:55:13.000000 cvprocessor-0.5.4/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.4/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.4/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.4/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.4/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.4/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.4/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.4/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    18338 2024-05-14 07:05:10.000000 cvprocessor-0.5.4/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.4/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.4/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.4/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.4/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     4907 2024-05-14 06:11:22.000000 cvprocessor-0.5.4/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.4/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.4/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:06:08.845666 cvprocessor-0.5.4/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 07:06:08.000000 cvprocessor-0.5.4/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 07:06:08.000000 cvprocessor-0.5.4/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 07:06:08.000000 cvprocessor-0.5.4/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 07:06:08.000000 cvprocessor-0.5.4/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 07:06:08.000000 cvprocessor-0.5.4/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:38:09.612504 cvprocessor-0.5.5/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.5/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 07:38:09.611854 cvprocessor-0.5.5/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.5/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 07:37:31.000000 cvprocessor-0.5.5/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 07:38:09.612594 cvprocessor-0.5.5/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:38:09.595767 cvprocessor-0.5.5/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:38:09.607955 cvprocessor-0.5.5/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.5/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.5/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.5/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7335 2024-05-14 07:36:11.000000 cvprocessor-0.5.5/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.5/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.5/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.5/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.5/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.5/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.5/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.5/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    18338 2024-05-14 07:05:10.000000 cvprocessor-0.5.5/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.5/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.5/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.5/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.5/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6050 2024-05-14 07:37:26.000000 cvprocessor-0.5.5/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.5/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.5/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:38:09.611050 cvprocessor-0.5.5/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 07:38:09.000000 cvprocessor-0.5.5/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 07:38:09.000000 cvprocessor-0.5.5/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 07:38:09.000000 cvprocessor-0.5.5/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 07:38:09.000000 cvprocessor-0.5.5/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 07:38:09.000000 cvprocessor-0.5.5/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.5.4/LICENSE` & `cvprocessor-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/PKG-INFO` & `cvprocessor-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.4
+Version: 0.5.5
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.4/README.md` & `cvprocessor-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/pyproject.toml` & `cvprocessor-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.5.4/src/cvprocessor/authors.py` & `cvprocessor-0.5.5/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/cv.py` & `cvprocessor-0.5.5/src/cvprocessor/cv.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,14 +160,23 @@
         The get_institute method is used to get the institute by the given institute ID.
 
         :param institute_id: The institute ID.
         :type institute_id: int
         """
         return self.academic_info.institutes.get_institute(institute_id)
 
+    def get_software(self, software_id):
+        """
+        The get_software method is used to get the software by the given software ID.
+
+        :param software_id: The software ID.
+        :type software_id: int
+        """
+        return self.software.get_software(software_id)
+
     def _load_cv(self, filename):
         """
         The _load_cv method is used to load the CV file.
 
         :param filename: The filename of the CV file.
         :type filename: str
         """
```

### Comparing `cvprocessor-0.5.4/src/cvprocessor/education.py` & `cvprocessor-0.5.5/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/experience.py` & `cvprocessor-0.5.5/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/grants_awards.py` & `cvprocessor-0.5.5/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/institutes.py` & `cvprocessor-0.5.5/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/intro.py` & `cvprocessor-0.5.5/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/memberships.py` & `cvprocessor-0.5.5/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/news.py` & `cvprocessor-0.5.5/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/publications.py` & `cvprocessor-0.5.5/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/references.py` & `cvprocessor-0.5.5/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/research_interests.py` & `cvprocessor-0.5.5/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/service.py` & `cvprocessor-0.5.5/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/skills.py` & `cvprocessor-0.5.5/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/supervision.py` & `cvprocessor-0.5.5/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor/teaching.py` & `cvprocessor-0.5.5/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.4/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.5.5/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.4
+Version: 0.5.5
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.4/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.5.5/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

