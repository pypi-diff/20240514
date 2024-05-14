# Comparing `tmp/cvprocessor-0.5.2.tar.gz` & `tmp/cvprocessor-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.5.2.tar", last modified: Tue May 14 06:45:26 2024, max compression
+gzip compressed data, was "cvprocessor-0.5.3.tar", last modified: Tue May 14 07:00:18 2024, max compression
```

## Comparing `cvprocessor-0.5.2.tar` & `cvprocessor-0.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.070267 cvprocessor-0.5.2/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.2/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:45:26.069712 cvprocessor-0.5.2/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.2/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 06:44:30.000000 cvprocessor-0.5.2/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 06:45:26.070427 cvprocessor-0.5.2/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.052506 cvprocessor-0.5.2/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.065968 cvprocessor-0.5.2/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.2/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     7926 2024-05-14 06:19:48.000000 cvprocessor-0.5.2/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.2/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     6464 2024-05-14 06:28:52.000000 cvprocessor-0.5.2/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.2/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.2/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.2/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     5427 2024-05-14 06:16:10.000000 cvprocessor-0.5.2/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.2/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.2/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.2/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    17960 2024-05-14 06:45:01.000000 cvprocessor-0.5.2/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.2/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.2/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.2/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.2/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     4907 2024-05-14 06:11:22.000000 cvprocessor-0.5.2/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.2/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.2/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 06:45:26.069001 cvprocessor-0.5.2/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 06:45:26.000000 cvprocessor-0.5.2/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:00:18.761137 cvprocessor-0.5.3/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.3/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 07:00:18.760709 cvprocessor-0.5.3/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.3/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 06:55:22.000000 cvprocessor-0.5.3/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 07:00:18.761228 cvprocessor-0.5.3/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:00:18.739249 cvprocessor-0.5.3/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:00:18.757023 cvprocessor-0.5.3/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.3/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.3/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.3/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7051 2024-05-14 06:55:13.000000 cvprocessor-0.5.3/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.3/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.3/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.3/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.3/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.3/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.3/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.3/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    18098 2024-05-14 06:49:23.000000 cvprocessor-0.5.3/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.3/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1355 2024-05-14 05:24:15.000000 cvprocessor-0.5.3/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.3/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.3/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4907 2024-05-14 06:11:22.000000 cvprocessor-0.5.3/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.3/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.3/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 07:00:18.760213 cvprocessor-0.5.3/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 07:00:18.000000 cvprocessor-0.5.3/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 07:00:18.000000 cvprocessor-0.5.3/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 07:00:18.000000 cvprocessor-0.5.3/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 07:00:18.000000 cvprocessor-0.5.3/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 07:00:18.000000 cvprocessor-0.5.3/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.5.2/LICENSE` & `cvprocessor-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/PKG-INFO` & `cvprocessor-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.2
+Version: 0.5.3
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.2/README.md` & `cvprocessor-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/pyproject.toml` & `cvprocessor-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.5.2/src/cvprocessor/authors.py` & `cvprocessor-0.5.3/src/cvprocessor/authors.py`

 * *Files 25% similar despite different names*

```diff
@@ -164,14 +164,128 @@
     def __init__(self):
         self.id = int()
         self.affiliations = []
         self.personal_info = PersonalInfo()
         self.contact_info = ContactInfo()
         self.research_info = ResearchInfo()
 
+    def get_id(self):
+        """
+        Returns the ID of the author.
+        """
+        return self.id
+
+    def get_affiliations(self):
+        """
+        Returns the affiliations of the author.
+        """
+        return self.affiliations
+
+    def get_name(self):
+        """
+        Returns the name of the author.
+        """
+        return self.personal_info.name
+
+    def get_lastname(self):
+        """
+        Returns the lastname of the author.
+        """
+        return self.personal_info.lastname
+
+    def get_alias_long(self):
+        """
+        Returns the long alias of the author.
+        """
+        return self.personal_info.alias_long
+
+    def get_alias_short(self):
+        """
+        Returns the short alias of the author.
+        """
+        return self.personal_info.alias_short
+
+    def get_job_title(self):
+        """
+        Returns the job title of the author.
+        """
+        return self.personal_info.job_title
+
+    def get_fingerprint(self):
+        """
+        Returns the fingerprint of the author.
+        """
+        return self.personal_info.fingerprint
+
+    def get_public_key(self):
+        """
+        Returns the public key of the author.
+        """
+        return self.personal_info.public_key
+
+    def get_email(self):
+        """
+        Returns the email of the author.
+        """
+        return self.contact_info.email
+
+    def get_telephone(self):
+        """
+        Returns the telephone of the author.
+        """
+        return self.contact_info.telephone
+
+    def get_website(self):
+        """
+        Returns the website of the author.
+        """
+        return self.contact_info.website
+
+    def get_address(self):
+        """
+        Returns the address of the author.
+        """
+        return self.contact_info.address
+
+    def get_location(self):
+        """
+        Returns the location of the author.
+        """
+        return self.contact_info.location
+
+    def get_linkedin(self):
+        """
+        Returns the LinkedIn of the author.
+        """
+        return self.research_info.linkedin
+
+    def get_github(self):
+        """
+        Returns the GitHub of the author.
+        """
+        return self.research_info.github
+
+    def get_google_scholar(self):
+        """
+        Returns the Google Scholar of the author.
+        """
+        return self.research_info.google_scholar
+
+    def get_orcid(self):
+        """
+        Returns the ORCID of the author.
+        """
+        return self.research_info.orcid
+
+    def get_researchgate(self):
+        """
+        Returns the ResearchGate of the author.
+        """
+        return self.research_info.researchgate
+
     def load(self, filename):
         """
         Loads the author data from the file.
         """
         self.id = filename["id"]
         if isinstance(filename["Affiliations"], str) and\
                 ("," in filename["Affiliations"] or ";" in filename["Affiliations"]):
@@ -225,21 +339,20 @@
         """
         Gets the author by ID and affiliation ID.
         """
         if isinstance(author_id, str):
             author_id = int(author_id)
         if affiliation_id is None:
             for author in self.authors:
-                if author.id == author_id:
+                if author.get_id() == author_id:
                     return author
             return None
         for author in self.authors:
-            if author.id == author_id and affiliation_id in author.affiliations:
+            if author.get_id() == author_id and affiliation_id in author.get_affiliations():
                 return author
-        return None
 
     def load(self, filename):
         """
         Loads the authors from the file.
         """
         authors_df = pd.read_excel(filename, sheet_name="Authors")
         for _, row in authors_df.iterrows():
```

### Comparing `cvprocessor-0.5.2/src/cvprocessor/cv.py` & `cvprocessor-0.5.3/src/cvprocessor/cv.py`

 * *Files 20% similar despite different names*

```diff
@@ -142,14 +142,32 @@
         self.professional_info = ProfessionalInfo()
         self.personal_info = PersonalInfo()
         self.academic_info = AcademicInfo()
         self.software = Software()
         self.news = News()
         self._load_cv(filename)
 
+    def get_author(self, author_id):
+        """
+        The get_author method is used to get the author by the given author ID.
+
+        :param author_id: The author ID.
+        :type author_id: int
+        """
+        return self.personal_info.authors.get_author(author_id)
+
+    def get_institute(self, institute_id):
+        """
+        The get_institute method is used to get the institute by the given institute ID.
+
+        :param institute_id: The institute ID.
+        :type institute_id: int
+        """
+        return self.academic_info.institutes.get_institute(institute_id)
+
     def _load_cv(self, filename):
         """
         The _load_cv method is used to load the CV file.
 
         :param filename: The filename of the CV file.
         :type filename: str
         """
```

### Comparing `cvprocessor-0.5.2/src/cvprocessor/education.py` & `cvprocessor-0.5.3/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/experience.py` & `cvprocessor-0.5.3/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/grants_awards.py` & `cvprocessor-0.5.3/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/institutes.py` & `cvprocessor-0.5.3/src/cvprocessor/institutes.py`

 * *Files 22% similar despite different names*

```diff
@@ -114,14 +114,74 @@
     """
 
     def __init__(self):
         self.info = InstituteInfo()
         self.location = InstituteLocation()
         self.url = None
 
+    def get_id(self):
+        """
+        Get the ID of the institute.
+        """
+        return self.info.id
+
+    def get_name(self):
+        """
+        Get the name of the institute.
+        """
+        return self.info.name
+
+    def get_name_abbr(self):
+        """
+        Get the name abbreviation of the institute.
+        """
+        return self.info.name_abbr
+
+    def get_department(self):
+        """
+        Get the department of the institute.
+        """
+        return self.info.department
+
+    def get_department_abbr(self):
+        """
+        Get the department abbreviation of the institute.
+        """
+        return self.info.department_abbr
+
+    def get_address(self):
+        """
+        Get the address of the institute.
+        """
+        return self.location.address
+
+    def get_city(self):
+        """
+        Get the city of the institute.
+        """
+        return self.location.city
+
+    def get_country(self):
+        """
+        Get the country of the institute.
+        """
+        return self.location.country
+
+    def get_coordinates(self):
+        """
+        Get the coordinates of the institute.
+        """
+        return self.location.coordinates
+
+    def get_url(self):
+        """
+        Get the URL of the institute.
+        """
+        return self.url
+
     def load(self, pd_dataframe):
         """
         Load the data from a pandas dataframe.
         """
         self.info.load(pd_dataframe)
         self.location.load(pd_dataframe)
         self.url = pd_dataframe["URL"]
@@ -160,15 +220,15 @@
     def get_institute(self, institute_id):
         """
         Get the institute by its ID.
         """
         if isinstance(institute_id, str):
             institute_id = int(institute_id)
         for institute in self.institutes:
-            if institute.info.id == institute_id:
+            if institute.get_id() == institute_id:
                 return institute
         return None
 
     def load(self, filename):
         """
         Load the institutes from the filename.
         """
```

### Comparing `cvprocessor-0.5.2/src/cvprocessor/intro.py` & `cvprocessor-0.5.3/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/memberships.py` & `cvprocessor-0.5.3/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/news.py` & `cvprocessor-0.5.3/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/publications.py` & `cvprocessor-0.5.3/src/cvprocessor/publications.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,20 @@
 
     def get_copyright(self):
         """
         Get the copyright of the publication.
         """
         return self.rights.copyright
 
+    def get_authors_ids(self):
+        """
+        Get the authors' IDs and affiliation IDs.
+        """
+        return self.authors_ids
+
     def load(self, filename):
         """
         Load the publication data from the file.
         """
         authors_list = filename["Authors"].split(",")
         authors = []
         for author in authors_list:
```

### Comparing `cvprocessor-0.5.2/src/cvprocessor/references.py` & `cvprocessor-0.5.3/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/research_interests.py` & `cvprocessor-0.5.3/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/service.py` & `cvprocessor-0.5.3/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/skills.py` & `cvprocessor-0.5.3/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/software.py` & `cvprocessor-0.5.3/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/supervision.py` & `cvprocessor-0.5.3/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor/teaching.py` & `cvprocessor-0.5.3/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.2/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.5.3/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.2
+Version: 0.5.3
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.2/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.5.3/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

