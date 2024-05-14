# Comparing `tmp/stac_fastapi_opensearch-3.0.0a0.tar.gz` & `tmp/stac_fastapi_opensearch-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_opensearch-3.0.0a0.tar", last modified: Sat May 11 12:06:43 2024, max compression
+gzip compressed data, was "stac_fastapi_opensearch-3.0.0a1.tar", last modified: Tue May 14 06:51:45 2024, max compression
```

## Comparing `stac_fastapi_opensearch-3.0.0a0.tar` & `stac_fastapi_opensearch-3.0.0a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.661950 stac_fastapi_opensearch-3.0.0a0/
--rw-r--r--   0 primeradiant   (501) staff       (20)    14904 2024-05-11 12:06:43.661594 stac_fastapi_opensearch-3.0.0a0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_opensearch-3.0.0a0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-05-11 12:06:43.693953 stac_fastapi_opensearch-3.0.0a0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1593 2024-05-11 10:41:59.000000 stac_fastapi_opensearch-3.0.0a0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.489185 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.652075 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3272 2024-05-02 09:57:35.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2366 2024-04-09 14:42:19.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    35204 2024-05-11 10:43:40.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-11 10:41:59.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.652884 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)    14904 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      242 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:51:45.120406 stac_fastapi_opensearch-3.0.0a1/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14904 2024-05-14 06:51:45.118112 stac_fastapi_opensearch-3.0.0a1/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_opensearch-3.0.0a1/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-05-14 06:51:45.121384 stac_fastapi_opensearch-3.0.0a1/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1593 2024-05-14 06:50:36.000000 stac_fastapi_opensearch-3.0.0a1/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:51:45.079212 stac_fastapi_opensearch-3.0.0a1/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:51:45.109863 stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3226 2024-05-14 06:29:09.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2366 2024-04-09 14:42:19.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    35204 2024-05-11 10:43:40.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-14 06:50:36.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:51:45.111269 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14904 2024-05-14 06:51:45.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-05-14 06:51:45.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-14 06:51:45.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-05-14 06:51:45.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      242 2024-05-14 06:51:45.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-14 06:51:45.000000 stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/top_level.txt
```

### Comparing `stac_fastapi_opensearch-3.0.0a0/PKG-INFO` & `stac_fastapi_opensearch-3.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.opensearch
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: Opensearch stac-fastapi backend.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: stac-fastapi.core==3.0.0a0
+Requires-Dist: stac-fastapi.core==3.0.0a1
 Requires-Dist: opensearch-py==2.4.2
 Requires-Dist: opensearch-py[async]==2.4.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac_fastapi_opensearch-3.0.0a0/README.md` & `stac_fastapi_opensearch-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `stac_fastapi_opensearch-3.0.0a0/setup.py` & `stac_fastapi_opensearch-3.0.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==3.0.0a0",
+    "stac-fastapi.core==3.0.0a1",
     "opensearch-py==2.4.2",
     "opensearch-py[async]==2.4.2",
     "uvicorn",
     "starlette",
 ]
 
 extra_reqs = {
```

### Comparing `stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/app.py` & `stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     CoreClient,
     EsAsyncBaseFiltersClient,
     TransactionsClient,
 )
 from stac_fastapi.core.extensions import QueryExtension
 from stac_fastapi.core.session import Session
 from stac_fastapi.extensions.core import (
-    ContextExtension,
     FieldsExtension,
     FilterExtension,
     SortExtension,
     TokenPaginationExtension,
     TransactionExtension,
 )
 from stac_fastapi.extensions.third_party import BulkTransactionExtension
@@ -53,15 +52,14 @@
             settings=settings,
         )
     ),
     FieldsExtension(),
     QueryExtension(),
     SortExtension(),
     TokenPaginationExtension(),
-    ContextExtension(),
     filter_extension,
 ]
 
 post_request_model = create_post_request_model(extensions)
 
 api = StacApi(
     title=os.getenv("STAC_FASTAPI_TITLE", "stac-fastapi-opensearch"),
```

### Comparing `stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/config.py` & `stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/database_logic.py` & `stac_fastapi_opensearch-3.0.0a1/stac_fastapi/opensearch/database_logic.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/PKG-INFO` & `stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.opensearch
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: Opensearch stac-fastapi backend.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: stac-fastapi.core==3.0.0a0
+Requires-Dist: stac-fastapi.core==3.0.0a1
 Requires-Dist: opensearch-py==2.4.2
 Requires-Dist: opensearch-py[async]==2.4.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/SOURCES.txt` & `stac_fastapi_opensearch-3.0.0a1/stac_fastapi.opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

