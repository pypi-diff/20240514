# Comparing `tmp/stac_fastapi_elasticsearch-3.0.0a0.tar.gz` & `tmp/stac_fastapi_elasticsearch-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_elasticsearch-3.0.0a0.tar", last modified: Sat May 11 12:04:26 2024, max compression
+gzip compressed data, was "stac_fastapi_elasticsearch-3.0.0a1.tar", last modified: Tue May 14 06:54:08 2024, max compression
```

## Comparing `stac_fastapi_elasticsearch-3.0.0a0.tar` & `stac_fastapi_elasticsearch-3.0.0a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.977320 stac_fastapi_elasticsearch-3.0.0a0/
--rw-r--r--   0 primeradiant   (501) staff       (20)    14981 2024-05-11 12:04:26.976882 stac_fastapi_elasticsearch-3.0.0a0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_elasticsearch-3.0.0a0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-05-11 12:04:26.979784 stac_fastapi_elasticsearch-3.0.0a0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1777 2024-05-11 10:41:59.000000 stac_fastapi_elasticsearch-3.0.0a0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.696045 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.935650 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3293 2024-05-02 09:57:35.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2405 2024-04-09 14:42:19.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    34398 2024-05-11 10:43:13.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-11 10:41:59.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.938938 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)    14981 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-05-11 12:04:26.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      248 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:54:08.072279 stac_fastapi_elasticsearch-3.0.0a1/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14981 2024-05-14 06:54:08.069543 stac_fastapi_elasticsearch-3.0.0a1/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_elasticsearch-3.0.0a1/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-05-14 06:54:08.073684 stac_fastapi_elasticsearch-3.0.0a1/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1777 2024-05-14 06:50:36.000000 stac_fastapi_elasticsearch-3.0.0a1/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:54:08.037844 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:54:08.062029 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3247 2024-05-14 06:29:09.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2405 2024-04-09 14:42:19.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    34398 2024-05-11 10:43:13.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-14 06:50:36.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:54:08.063223 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14981 2024-05-14 06:54:08.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-05-14 06:54:08.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-14 06:54:08.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-05-14 06:54:08.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      248 2024-05-14 06:54:08.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-14 06:54:08.000000 stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/top_level.txt
```

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/PKG-INFO` & `stac_fastapi_elasticsearch-3.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.elasticsearch
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework with both Elasticsearch and Opensearch.
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
 Requires-Dist: elasticsearch[async]==8.11.0
 Requires-Dist: elasticsearch-dsl==8.11.0
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/README.md` & `stac_fastapi_elasticsearch-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/setup.py` & `stac_fastapi_elasticsearch-3.0.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==3.0.0a0",
+    "stac-fastapi.core==3.0.0a1",
     "elasticsearch[async]==8.11.0",
     "elasticsearch-dsl==8.11.0",
     "uvicorn",
     "starlette",
 ]
 
 extra_reqs = {
```

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/app.py` & `stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from stac_fastapi.elasticsearch.config import ElasticsearchSettings
 from stac_fastapi.elasticsearch.database_logic import (
     DatabaseLogic,
     create_collection_index,
     create_index_templates,
 )
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
     title=os.getenv("STAC_FASTAPI_TITLE", "stac-fastapi-elasticsearch"),
```

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/config.py` & `stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/database_logic.py` & `stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi/elasticsearch/database_logic.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/PKG-INFO` & `stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.elasticsearch
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework with both Elasticsearch and Opensearch.
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
 Requires-Dist: elasticsearch[async]==8.11.0
 Requires-Dist: elasticsearch-dsl==8.11.0
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt` & `stac_fastapi_elasticsearch-3.0.0a1/stac_fastapi.elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

