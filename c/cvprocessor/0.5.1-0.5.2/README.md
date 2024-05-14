# Comparing `tmp/cvprocessor-0.5.1.tar.gz` & `tmp/cvprocessor-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.5.1.tar", last modified: Tue May 14 06:40:37 2024, max compression
+gzip compressed data, was "cvprocessor-0.5.2.tar", last modified: Tue May 14 06:45:26 2024, max compression
```

## Comparing `cvprocessor-0.5.1.tar` & `cvprocessor-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:40:37.414503 cvprocessor-0.5.1/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.1/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:40:37.414032 cvprocessor-0.5.1/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.1/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 06:40:10.000000 cvprocessor-0.5.1/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 06:40:37.414589 cvprocessor-0.5.1/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:40:37.393705 cvprocessor-0.5.1/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:40:37.410969 cvprocessor-0.5.1/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.1/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     7926 2024-05-14 06:19:48.000000 cvprocessor-0.5.1/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.1/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     6464 2024-05-14 06:28:52.000000 cvprocessor-0.5.1/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.1/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.1/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.1/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     5427 2024-05-14 06:16:10.000000 cvprocessor-0.5.1/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.1/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.1/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.1/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    15480 2024-05-14 06:40:04.000000 cvprocessor-0.5.1/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.1/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.1/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.1/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.1/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     4907 2024-05-14 06:11:22.000000 cvprocessor-0.5.1/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.1/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.1/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:40:37.413405 cvprocessor-0.5.1/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:40:37.000000 cvprocessor-0.5.1/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 06:40:37.000000 cvprocessor-0.5.1/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 06:40:37.000000 cvprocessor-0.5.1/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 06:40:37.000000 cvprocessor-0.5.1/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 06:40:37.000000 cvprocessor-0.5.1/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.070267 cvprocessor-0.5.2/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.2/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:45:26.069712 cvprocessor-0.5.2/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.2/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 06:44:30.000000 cvprocessor-0.5.2/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 06:45:26.070427 cvprocessor-0.5.2/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.052506 cvprocessor-0.5.2/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.065968 cvprocessor-0.5.2/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.2/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7926 2024-05-14 06:19:48.000000 cvprocessor-0.5.2/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.2/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6464 2024-05-14 06:28:52.000000 cvprocessor-0.5.2/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.2/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.2/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.2/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5427 2024-05-14 06:16:10.000000 cvprocessor-0.5.2/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.2/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.2/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.2/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    17960 2024-05-14 06:45:01.000000 cvprocessor-0.5.2/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.2/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.2/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.2/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.2/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4907 2024-05-14 06:11:22.000000 cvprocessor-0.5.2/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.2/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.2/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.069001 cvprocessor-0.5.2/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.5.1/LICENSE` & `cvprocessor-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/PKG-INFO` & `cvprocessor-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.1
+Version: 0.5.2
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.1/README.md` & `cvprocessor-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/pyproject.toml` & `cvprocessor-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.5.1/src/cvprocessor/authors.py` & `cvprocessor-0.5.2/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/cv.py` & `cvprocessor-0.5.2/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/education.py` & `cvprocessor-0.5.2/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/experience.py` & `cvprocessor-0.5.2/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/grants_awards.py` & `cvprocessor-0.5.2/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/institutes.py` & `cvprocessor-0.5.2/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/intro.py` & `cvprocessor-0.5.2/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/memberships.py` & `cvprocessor-0.5.2/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/news.py` & `cvprocessor-0.5.2/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/publications.py` & `cvprocessor-0.5.2/src/cvprocessor/publications.py`

 * *Files 14% similar despite different names*

```diff
@@ -307,14 +307,122 @@
 
     def __init__(self):
         self.authors_ids = []
         self.details = PublicationDetails()
         self.resources = PublicationResources()
         self.rights = PublicationRights()
 
+    def get_title(self):
+        """
+        Get the title of the publication.
+        """
+        return self.details.basic_info.title
+
+    def get_year(self):
+        """
+        Get the year of the publication.
+        """
+        return self.details.basic_info.year
+
+    def get_source(self):
+        """
+        Get the source of the publication.
+        """
+        return self.details.basic_info.source
+
+    def get_volume(self):
+        """
+        Get the volume of the publication.
+        """
+        return self.details.journal_info.volume
+
+    def get_issue(self):
+        """
+        Get the issue of the publication.
+        """
+        return self.details.journal_info.issue
+
+    def get_artno(self):
+        """
+        Get the article number of the publication.
+        """
+        return self.details.journal_info.artno
+
+    def get_page_start(self):
+        """
+        Get the starting page of the publication.
+        """
+        return self.details.page_info.page_start
+
+    def get_page_end(self):
+        """
+        Get the ending page of the publication.
+        """
+        return self.details.page_info.page_end
+
+    def get_document_type(self):
+        """
+        Get the document type of the publication.
+        """
+        return self.details.document_type
+
+    def get_code(self):
+        """
+        Get the code of the publication.
+        """
+        return self.resources.code
+
+    def get_slides(self):
+        """
+        Get the slides of the publication.
+        """
+        return self.resources.slides
+
+    def get_abstract(self):
+        """
+        Get the abstract of the publication.
+        """
+        return self.resources.abstract
+
+    def get_keywords(self):
+        """
+        Get the keywords of the publication.
+        """
+        return self.resources.keywords
+
+    def get_doi(self):
+        """
+        Get the DOI of the publication.
+        """
+        return self.resources.doi
+
+    def get_preprint_doi(self):
+        """
+        Get the preprint DOI of the publication.
+        """
+        return self.resources.preprint_doi
+
+    def get_jcr(self):
+        """
+        Get the JCR of the publication.
+        """
+        return self.rights.jcr
+
+    def get_license(self):
+        """
+        Get the license of the publication.
+        """
+        return self.rights.license
+
+    def get_copyright(self):
+        """
+        Get the copyright of the publication.
+        """
+        return self.rights.copyright
+
     def load(self, filename):
         """
         Load the publication data from the file.
         """
         authors_list = filename["Authors"].split(",")
         authors = []
         for author in authors_list:
```

### Comparing `cvprocessor-0.5.1/src/cvprocessor/references.py` & `cvprocessor-0.5.2/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/research_interests.py` & `cvprocessor-0.5.2/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/service.py` & `cvprocessor-0.5.2/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/skills.py` & `cvprocessor-0.5.2/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/software.py` & `cvprocessor-0.5.2/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/supervision.py` & `cvprocessor-0.5.2/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor/teaching.py` & `cvprocessor-0.5.2/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.1/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.5.2/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.1
+Version: 0.5.2
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.1/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.5.2/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

