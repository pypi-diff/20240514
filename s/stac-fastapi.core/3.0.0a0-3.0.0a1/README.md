# Comparing `tmp/stac_fastapi_core-3.0.0a0.tar.gz` & `tmp/stac_fastapi_core-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_core-3.0.0a0.tar", last modified: Sat May 11 10:58:49 2024, max compression
+gzip compressed data, was "stac_fastapi_core-3.0.0a1.tar", last modified: Tue May 14 06:53:18 2024, max compression
```

## Comparing `stac_fastapi_core-3.0.0a0.tar` & `stac_fastapi_core-3.0.0a1.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.960157 stac_fastapi_core-3.0.0a0/
--rw-r--r--   0 primeradiant   (501) staff       (20)    14638 2024-05-11 10:58:49.959358 stac_fastapi_core-3.0.0a0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_core-3.0.0a0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-05-11 10:58:49.963905 stac_fastapi_core-3.0.0a0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1401 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.892128 stac_fastapi_core-3.0.0a0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.934731 stac_fastapi_core-3.0.0a0/stac_fastapi/core/
--rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/base_database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/base_settings.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3826 2024-05-02 09:57:35.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/basic_auth.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    37146 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1481 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/datetime_utils.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.941841 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/
--rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     6095 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/filter.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1921 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/query.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.949977 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/
--rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/links.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/search.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/serializers.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/session.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.952508 stac_fastapi_core-3.0.0a0/stac_fastapi/core/types/
--rw-r--r--   0 primeradiant   (501) staff       (20)     8120 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/types/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      952 2024-05-11 10:42:06.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/utilities.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-11 10:41:59.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.957363 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)    14638 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      850 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      223 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:53:18.869608 stac_fastapi_core-3.0.0a1/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14638 2024-05-14 06:53:18.868744 stac_fastapi_core-3.0.0a1/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_core-3.0.0a1/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-05-14 06:53:18.871929 stac_fastapi_core-3.0.0a1/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1401 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a1/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:53:18.813543 stac_fastapi_core-3.0.0a1/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:53:18.848008 stac_fastapi_core-3.0.0a1/stac_fastapi/core/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/base_database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/base_settings.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3826 2024-05-02 09:57:35.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/basic_auth.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    36576 2024-05-14 06:29:09.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/core.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1481 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/datetime_utils.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:53:18.857000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/extensions/
+-rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/extensions/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     6095 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/extensions/filter.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1921 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/extensions/query.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:53:18.864831 stac_fastapi_core-3.0.0a1/stac_fastapi/core/models/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/models/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/models/links.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/models/search.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/serializers.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/session.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      952 2024-05-11 10:42:06.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/utilities.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-14 06:50:36.000000 stac_fastapi_core-3.0.0a1/stac_fastapi/core/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-14 06:53:18.866527 stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14638 2024-05-14 06:53:18.000000 stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      818 2024-05-14 06:53:18.000000 stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-14 06:53:18.000000 stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      223 2024-05-14 06:53:18.000000 stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-14 06:53:18.000000 stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/top_level.txt
```

### Comparing `stac_fastapi_core-3.0.0a0/PKG-INFO` & `stac_fastapi_core-3.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.core
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: Core library for the Elasticsearch and Opensearch stac-fastapi backends.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `stac_fastapi_core-3.0.0a0/README.md` & `stac_fastapi_core-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/setup.py` & `stac_fastapi_core-3.0.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/base_database_logic.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/base_database_logic.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/basic_auth.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/basic_auth.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/core.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 from stac_pydantic.version import STAC_VERSION
 
 from stac_fastapi.core.base_database_logic import BaseDatabaseLogic
 from stac_fastapi.core.base_settings import ApiBaseSettings
 from stac_fastapi.core.models.links import PagingLinks
 from stac_fastapi.core.serializers import CollectionSerializer, ItemSerializer
 from stac_fastapi.core.session import Session
-from stac_fastapi.core.types.core import (
-    AsyncBaseCoreClient,
-    AsyncBaseTransactionsClient,
-)
 from stac_fastapi.extensions.third_party.bulk_transactions import (
     BaseBulkTransactionsClient,
     BulkTransactionMethod,
     Items,
 )
 from stac_fastapi.types import stac as stac_types
 from stac_fastapi.types.config import Settings
 from stac_fastapi.types.conformance import BASE_CONFORMANCE_CLASSES
-from stac_fastapi.types.core import AsyncBaseFiltersClient
+from stac_fastapi.types.core import (
+    AsyncBaseCoreClient,
+    AsyncBaseFiltersClient,
+    AsyncBaseTransactionsClient,
+)
 from stac_fastapi.types.extension import ApiExtension
 from stac_fastapi.types.requests import get_base_url
 from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.search import BaseSearchPostRequest
 
 logger = logging.getLogger(__name__)
 
@@ -308,30 +308,22 @@
             collection_ids=[collection_id],
         )
 
         items = [
             self.item_serializer.db_to_stac(item, base_url=base_url) for item in items
         ]
 
-        context_obj = None
-        if self.extension_is_enabled("ContextExtension"):
-            context_obj = {
-                "returned": len(items),
-                "limit": limit,
-            }
-            if maybe_count is not None:
-                context_obj["matched"] = maybe_count
-
         links = await PagingLinks(request=request, next=next_token).get_links()
 
         return stac_types.ItemCollection(
             type="FeatureCollection",
             features=items,
             links=links,
-            context=context_obj,
+            numReturned=len(items),
+            numMatched=maybe_count,
         )
 
     async def get_item(
         self, item_id: str, collection_id: str, **kwargs
     ) -> stac_types.Item:
         """Get an item from the database based on its id and collection id.
 
@@ -629,30 +621,22 @@
             items = [
                 orjson.loads(
                     stac_pydantic.Item(**feat).json(**filter_kwargs, exclude_unset=True)
                 )
                 for feat in items
             ]
 
-        context_obj = None
-        if self.extension_is_enabled("ContextExtension"):
-            context_obj = {
-                "returned": len(items),
-                "limit": limit,
-            }
-            if maybe_count is not None:
-                context_obj["matched"] = maybe_count
-
         links = await PagingLinks(request=request, next=next_token).get_links()
 
         return stac_types.ItemCollection(
             type="FeatureCollection",
             features=items,
             links=links,
-            context=context_obj,
+            numReturned=len(items),
+            numMatched=maybe_count,
         )
 
 
 @attr.s
 class TransactionsClient(AsyncBaseTransactionsClient):
     """Transactions extension specific CRUD operations."""
 
@@ -769,42 +753,39 @@
             collection, base_url
         )
         await self.database.create_collection(collection=collection)
         return CollectionSerializer.db_to_stac(collection, base_url)
 
     @overrides
     async def update_collection(
-        self, collection: Collection, **kwargs
+        self, collection_id: str, collection: Collection, **kwargs
     ) -> stac_types.Collection:
         """
         Update a collection.
 
         This method updates an existing collection in the database by first finding
         the collection by the id given in the keyword argument `collection_id`.
         If no `collection_id` is given the id of the given collection object is used.
         If the object and keyword collection ids don't match the sub items
         collection id is updated else the items are left unchanged.
         The updated collection is then returned.
 
         Args:
+            collection_id: id of the existing collection to be updated
             collection: A STAC collection that needs to be updated.
             kwargs: Additional keyword arguments.
 
         Returns:
             A STAC collection that has been updated in the database.
 
         """
         collection = collection.model_dump(mode="json")
 
         base_url = str(kwargs["request"].base_url)
 
-        collection_id = kwargs["request"].query_params.get(
-            "collection_id", collection["id"]
-        )
-
         collection = self.database.collection_serializer.stac_to_db(
             collection, base_url
         )
         await self.database.update_collection(
             collection_id=collection_id, collection=collection
         )
```

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/datetime_utils.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/filter.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/extensions/filter.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/query.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/links.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/models/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/serializers.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/serializers.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi/core/utilities.py` & `stac_fastapi_core-3.0.0a1/stac_fastapi/core/utilities.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/PKG-INFO` & `stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.core
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: Core library for the Elasticsearch and Opensearch stac-fastapi backends.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/SOURCES.txt` & `stac_fastapi_core-3.0.0a1/stac_fastapi.core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 stac_fastapi/core/utilities.py
 stac_fastapi/core/version.py
 stac_fastapi/core/extensions/__init__.py
 stac_fastapi/core/extensions/filter.py
 stac_fastapi/core/extensions/query.py
 stac_fastapi/core/models/__init__.py
 stac_fastapi/core/models/links.py
-stac_fastapi/core/models/search.py
-stac_fastapi/core/types/core.py
+stac_fastapi/core/models/search.py
```

