# Comparing `tmp/cvprocessor-0.5.7.tar.gz` & `tmp/cvprocessor-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.5.7.tar", last modified: Tue May 14 08:03:41 2024, max compression
+gzip compressed data, was "cvprocessor-0.5.8.tar", last modified: Tue May 14 08:07:22 2024, max compression
```

## Comparing `cvprocessor-0.5.7.tar` & `cvprocessor-0.5.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:03:41.389317 cvprocessor-0.5.7/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.7/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:03:41.388530 cvprocessor-0.5.7/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.7/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 08:03:14.000000 cvprocessor-0.5.7/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 08:03:41.389477 cvprocessor-0.5.7/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:03:41.372138 cvprocessor-0.5.7/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:03:41.384377 cvprocessor-0.5.7/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.7/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.7/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.7/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     8890 2024-05-14 07:57:28.000000 cvprocessor-0.5.7/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.7/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.7/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.7/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.7/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.7/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.7/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.7/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    18348 2024-05-14 08:03:10.000000 cvprocessor-0.5.7/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.7/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.7/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.7/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.7/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     6050 2024-05-14 07:37:26.000000 cvprocessor-0.5.7/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.7/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.7/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:03:41.387765 cvprocessor-0.5.7/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:03:41.000000 cvprocessor-0.5.7/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 08:03:41.000000 cvprocessor-0.5.7/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 08:03:41.000000 cvprocessor-0.5.7/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 08:03:41.000000 cvprocessor-0.5.7/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 08:03:41.000000 cvprocessor-0.5.7/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.108686 cvprocessor-0.5.8/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.8/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:07:22.107955 cvprocessor-0.5.8/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.8/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 08:06:50.000000 cvprocessor-0.5.8/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 08:07:22.108809 cvprocessor-0.5.8/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.092789 cvprocessor-0.5.8/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.104161 cvprocessor-0.5.8/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.8/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.8/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.8/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9312 2024-05-14 08:06:44.000000 cvprocessor-0.5.8/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.8/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.8/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.8/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.8/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.8/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.8/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.8/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    18348 2024-05-14 08:03:10.000000 cvprocessor-0.5.8/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.8/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-14 08:06:36.000000 cvprocessor-0.5.8/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.8/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.8/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6050 2024-05-14 07:37:26.000000 cvprocessor-0.5.8/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.8/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.8/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.107141 cvprocessor-0.5.8/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.5.7/LICENSE` & `cvprocessor-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/PKG-INFO` & `cvprocessor-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.7
+Version: 0.5.8
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.7/README.md` & `cvprocessor-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/pyproject.toml` & `cvprocessor-0.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.5.7"
+version = "0.5.8"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.5.7/src/cvprocessor/authors.py` & `cvprocessor-0.5.8/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/cv.py` & `cvprocessor-0.5.8/src/cvprocessor/cv.py`

 * *Files 7% similar despite different names*

```diff
@@ -205,14 +205,26 @@
         The get_publications_num_publications_by_author method is used to get the number of publications by the given author.
 
         :param author_id: The author ID.
         :type author_id: int
         """
         return self.academic_info.publications.get_num_publications_by_author(author_id)
 
+    def get_research_interests(self):
+        """
+        The get_reserach_interests method is used to get the research interests.
+        """
+        return self.academic_info.research_interests.get_interests()
+
+    def get_research_keywords(self):
+        """
+        The get_research_keywords method is used to get the research keywords.
+        """
+        return self.academic_info.research_interests.get_keywords()
+
     def _load_cv(self, filename):
         """
         The _load_cv method is used to load the CV file.
 
         :param filename: The filename of the CV file.
         :type filename: str
         """
```

### Comparing `cvprocessor-0.5.7/src/cvprocessor/education.py` & `cvprocessor-0.5.8/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/experience.py` & `cvprocessor-0.5.8/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/grants_awards.py` & `cvprocessor-0.5.8/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/institutes.py` & `cvprocessor-0.5.8/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/intro.py` & `cvprocessor-0.5.8/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/memberships.py` & `cvprocessor-0.5.8/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/news.py` & `cvprocessor-0.5.8/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/publications.py` & `cvprocessor-0.5.8/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/references.py` & `cvprocessor-0.5.8/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/research_interests.py` & `cvprocessor-0.5.8/src/cvprocessor/research_interests.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,29 @@
 
     Attributes:
     research_interests (str): The research interests of the person.
     keywords (list): The keywords related to the research interests.
     """
 
     def __init__(self):
-        self.research_interests = None
+        self.research_interests = str()
         self.keywords = []
 
+    def get_interests(self) -> str:
+        """
+        Get the research interests of the person.
+        """
+        return self.research_interests
+
+    def get_keywords(self) -> list:
+        """
+        Get the keywords related to the research interests.
+        """
+        return self.keywords
+
     def load(self, filename) -> None:
         """
         Load the research interests and keywords from the given file.
         """
         research_interests_pd = pd.read_excel(
             filename, sheet_name="Research_Interests")
         self.research_interests = research_interests_pd["Interests"].values[0]
```

### Comparing `cvprocessor-0.5.7/src/cvprocessor/service.py` & `cvprocessor-0.5.8/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/skills.py` & `cvprocessor-0.5.8/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/software.py` & `cvprocessor-0.5.8/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/supervision.py` & `cvprocessor-0.5.8/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor/teaching.py` & `cvprocessor-0.5.8/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.7/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.5.8/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.7
+Version: 0.5.8
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.7/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.5.8/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

