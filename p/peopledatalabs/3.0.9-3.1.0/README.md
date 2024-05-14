# Comparing `tmp/peopledatalabs-3.0.9.tar.gz` & `tmp/peopledatalabs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopledatalabs-3.0.9.tar", max compression
+gzip compressed data, was "peopledatalabs-3.1.0.tar", max compression
```

## Comparing `peopledatalabs-3.0.9.tar` & `peopledatalabs-3.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2024-03-18 18:18:58.390740 peopledatalabs-3.0.9/LICENSE
--rw-r--r--   0        0        0    14018 2024-03-18 18:18:58.390740 peopledatalabs-3.0.9/README.md
--rw-r--r--   0        0        0     1632 2024-03-18 18:18:58.390740 peopledatalabs-3.0.9/pyproject.toml
--rw-r--r--   0        0        0      108 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/__init__.py
--rw-r--r--   0        0        0     6427 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/endpoints/__init__.py
--rw-r--r--   0        0        0     2102 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/endpoints/company.py
--rw-r--r--   0        0        0      764 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/endpoints/location.py
--rw-r--r--   0        0        0     2817 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/endpoints/person.py
--rw-r--r--   0        0        0      746 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/endpoints/school.py
--rw-r--r--   0        0        0      314 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/errors.py
--rw-r--r--   0        0        0      983 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/logger.py
--rw-r--r--   0        0        0     5830 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/main.py
--rw-r--r--   0        0        0     2940 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/models/__init__.py
--rw-r--r--   0        0        0     3131 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/models/company.py
--rw-r--r--   0        0        0      214 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/models/location.py
--rw-r--r--   0        0        0     4395 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/models/person.py
--rw-r--r--   0        0        0      785 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/models/school.py
--rw-r--r--   0        0        0     2246 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/requests.py
--rw-r--r--   0        0        0     1145 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/settings.py
--rw-r--r--   0        0        0      459 2024-03-18 18:18:58.394740 peopledatalabs-3.0.9/src/peopledatalabs/utils.py
--rw-r--r--   0        0        0    15467 1970-01-01 00:00:00.000000 peopledatalabs-3.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/LICENSE
+-rw-r--r--   0        0        0    14018 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/README.md
+-rw-r--r--   0        0        0     1632 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/__init__.py
+-rw-r--r--   0        0        0     6427 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/endpoints/__init__.py
+-rw-r--r--   0        0        0     2102 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/endpoints/company.py
+-rw-r--r--   0        0        0      764 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/endpoints/location.py
+-rw-r--r--   0        0        0     2817 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/endpoints/person.py
+-rw-r--r--   0        0        0      746 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/endpoints/school.py
+-rw-r--r--   0        0        0      314 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/errors.py
+-rw-r--r--   0        0        0      983 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/logger.py
+-rw-r--r--   0        0        0     5830 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/main.py
+-rw-r--r--   0        0        0     2940 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/models/__init__.py
+-rw-r--r--   0        0        0     3131 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/models/company.py
+-rw-r--r--   0        0        0      214 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/models/location.py
+-rw-r--r--   0        0        0     4395 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/models/person.py
+-rw-r--r--   0        0        0      785 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/models/school.py
+-rw-r--r--   0        0        0     2246 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/requests.py
+-rw-r--r--   0        0        0     1145 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/settings.py
+-rw-r--r--   0        0        0      459 2024-05-14 14:15:03.301560 peopledatalabs-3.1.0/src/peopledatalabs/utils.py
+-rw-r--r--   0        0        0    15463 1970-01-01 00:00:00.000000 peopledatalabs-3.1.0/PKG-INFO
```

### Comparing `peopledatalabs-3.0.9/LICENSE` & `peopledatalabs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/README.md` & `peopledatalabs-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/pyproject.toml` & `peopledatalabs-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peopledatalabs"
-version = "3.0.9"
+version = "3.1.0"
 description = "Official Python client for the People Data Labs API"
 homepage = "https://www.peopledatalabs.com"
 repository = "https://github.com/peopledatalabs/peopledatalabs-python"
 documentation = "https://docs.peopledatalabs.com"
 keywords = [
   "data enrichment",
   "people data labs",
@@ -27,25 +27,25 @@
 "Bug Tracker" = "https://github.com/peopledatalabs/peopledatalabs-python/issues"
 "Source Code" = 'https://github.com/peopledatalabs/peopledatalabs-python'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 email-validator = ">=1.1,<3.0"
 pydantic = "^2"
-python-dotenv = "^0"
+python-dotenv = "<2"
 requests = "^2"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.7"
-black = "^24.2.0"
-coverage = "^7.4.0"
+black = "^24.4.2"
+coverage = "^7.5.1"
 docformatter = "^1.7"
 flake8 = "^5.0.4"
 pylint = "^3.0.3"
-pytest = "^8.1.1"
+pytest = "^8.2.0"
 pyupgrade = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/endpoints/__init__.py` & `peopledatalabs-3.1.0/src/peopledatalabs/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/endpoints/company.py` & `peopledatalabs-3.1.0/src/peopledatalabs/endpoints/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/endpoints/location.py` & `peopledatalabs-3.1.0/src/peopledatalabs/endpoints/location.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/endpoints/person.py` & `peopledatalabs-3.1.0/src/peopledatalabs/endpoints/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/endpoints/school.py` & `peopledatalabs-3.1.0/src/peopledatalabs/endpoints/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/logger.py` & `peopledatalabs-3.1.0/src/peopledatalabs/logger.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/main.py` & `peopledatalabs-3.1.0/src/peopledatalabs/main.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/models/__init__.py` & `peopledatalabs-3.1.0/src/peopledatalabs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/models/company.py` & `peopledatalabs-3.1.0/src/peopledatalabs/models/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/models/person.py` & `peopledatalabs-3.1.0/src/peopledatalabs/models/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/models/school.py` & `peopledatalabs-3.1.0/src/peopledatalabs/models/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/requests.py` & `peopledatalabs-3.1.0/src/peopledatalabs/requests.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/src/peopledatalabs/settings.py` & `peopledatalabs-3.1.0/src/peopledatalabs/settings.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-3.0.9/PKG-INFO` & `peopledatalabs-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peopledatalabs
-Version: 3.0.9
+Version: 3.1.0
 Summary: Official Python client for the People Data Labs API
 Home-page: https://www.peopledatalabs.com
 License: MIT
 Keywords: data enrichment,people data labs,person enrichment,company enrichment,search
 Author: People Data Labs
 Author-email: hello@peopledatalabs.com
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: email-validator (>=1.1,<3.0)
 Requires-Dist: pydantic (>=2,<3)
-Requires-Dist: python-dotenv (>=0,<1)
+Requires-Dist: python-dotenv (<2)
 Requires-Dist: requests (>=2,<3)
 Project-URL: Bug Tracker, https://github.com/peopledatalabs/peopledatalabs-python/issues
 Project-URL: Documentation, https://docs.peopledatalabs.com
 Project-URL: Repository, https://github.com/peopledatalabs/peopledatalabs-python
 Project-URL: Source Code, https://github.com/peopledatalabs/peopledatalabs-python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: peopledatalabs Version: 3.0.9 Summary: Official
+Metadata-Version: 2.1 Name: peopledatalabs Version: 3.1.0 Summary: Official
 Python client for the People Data Labs API Home-page: https://
 www.peopledatalabs.com License: MIT Keywords: data enrichment,people data
 labs,person enrichment,company enrichment,search Author: People Data Labs
 Author-email: hello@peopledatalabs.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Requires-Dist: email-
 validator (>=1.1,<3.0) Requires-Dist: pydantic (>=2,<3) Requires-Dist: python-
-dotenv (>=0,<1) Requires-Dist: requests (>=2,<3) Project-URL: Bug Tracker,
-https://github.com/peopledatalabs/peopledatalabs-python/issues Project-URL:
+dotenv (<2) Requires-Dist: requests (>=2,<3) Project-URL: Bug Tracker, https://
+github.com/peopledatalabs/peopledatalabs-python/issues Project-URL:
 Documentation, https://docs.peopledatalabs.com Project-URL: Repository, https:/
 /github.com/peopledatalabs/peopledatalabs-python Project-URL: Source Code,
 https://github.com/peopledatalabs/peopledatalabs-python Description-Content-
 Type: text/markdown
                             [People Data Labs Logo]
                  ************ PPeeooppllee DDaattaa LLaabbss PPyytthhoonn CClliieenntt ************
              Official Python client for the People Data Labs API.
```

