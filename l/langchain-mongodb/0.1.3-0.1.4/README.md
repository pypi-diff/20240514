# Comparing `tmp/langchain_mongodb-0.1.3.tar.gz` & `tmp/langchain_mongodb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mongodb-0.1.3.tar", max compression
+gzip compressed data, was "langchain_mongodb-0.1.4.tar", max compression
```

## Comparing `langchain_mongodb-0.1.3.tar` & `langchain_mongodb-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/LICENSE
--rw-r--r--   0        0        0     1449 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/README.md
--rw-r--r--   0        0        0      365 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/langchain_mongodb/__init__.py
--rw-r--r--   0        0        0    10505 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/langchain_mongodb/cache.py
--rw-r--r--   0        0        0     2617 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/langchain_mongodb/chat_message_histories.py
--rw-r--r--   0        0        0        0 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/langchain_mongodb/py.typed
--rw-r--r--   0        0        0     3165 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/langchain_mongodb/utils.py
--rw-r--r--   0        0        0    17210 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/langchain_mongodb/vectorstores.py
--rw-r--r--   0        0        0     2548 2024-03-19 18:30:31.707899 langchain_mongodb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 langchain_mongodb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1449 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/README.md
+-rw-r--r--   0        0        0      365 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/__init__.py
+-rw-r--r--   0        0        0    10505 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/cache.py
+-rw-r--r--   0        0        0     2617 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/chat_message_histories.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/py.typed
+-rw-r--r--   0        0        0     3176 2024-05-14 18:55:01.299252 langchain_mongodb-0.1.4/langchain_mongodb/utils.py
+-rw-r--r--   0        0        0    17861 2024-05-14 18:55:01.299252 langchain_mongodb-0.1.4/langchain_mongodb/vectorstores.py
+-rw-r--r--   0        0        0     2636 2024-05-14 18:55:01.299252 langchain_mongodb-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 langchain_mongodb-0.1.4/PKG-INFO
```

### Comparing `langchain_mongodb-0.1.3/LICENSE` & `langchain_mongodb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.3/README.md` & `langchain_mongodb-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.3/langchain_mongodb/cache.py` & `langchain_mongodb-0.1.4/langchain_mongodb/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.3/langchain_mongodb/chat_message_histories.py` & `langchain_mongodb-0.1.4/langchain_mongodb/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.3/langchain_mongodb/utils.py` & `langchain_mongodb-0.1.4/langchain_mongodb/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         import simsimd as simd  # type: ignore
 
         X = np.array(X, dtype=np.float32)
         Y = np.array(Y, dtype=np.float32)
         Z = 1 - simd.cdist(X, Y, metric="cosine")
         if isinstance(Z, float):
             return np.array([Z])
-        return Z
+        return np.array(Z)
     except ImportError:
-        logger.info(
+        logger.debug(
             "Unable to import simsimd, defaulting to NumPy implementation. If you want "
             "to use simsimd please install with `pip install simsimd`."
         )
         X_norm = np.linalg.norm(X, axis=1)
         Y_norm = np.linalg.norm(Y, axis=1)
         # Ignore divide by zero errors run time warnings as those are handled below.
         with np.errstate(divide="ignore", invalid="ignore"):
```

### Comparing `langchain_mongodb-0.1.3/langchain_mongodb/vectorstores.py` & `langchain_mongodb-0.1.4/langchain_mongodb/vectorstores.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Optional,
     Tuple,
     TypeVar,
     Union,
 )
 
 import numpy as np
+from bson import ObjectId, json_util
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.runnables.config import run_in_executor
 from langchain_core.vectorstores import VectorStore
 from pymongo import MongoClient
 from pymongo.collection import Collection
 from pymongo.driver_info import DriverInfo
@@ -41,16 +42,16 @@
     - the ``pymongo`` python package installed
     - a connection string associated with a MongoDB Atlas Cluster having deployed an
         Atlas Search index
 
     Example:
         .. code-block:: python
 
-            from langchain_community.vectorstores import MongoDBAtlasVectorSearch
-            from langchain_community.embeddings.openai import OpenAIEmbeddings
+            from langchain_mongodb import MongoDBAtlasVectorSearch
+            from langchain_openai import OpenAIEmbeddings
             from pymongo import MongoClient
 
             mongo_client = MongoClient("<YOUR-CONNECTION-STRING>")
             collection = mongo_client["<db_name>"]["<collection_name>"]
             embeddings = OpenAIEmbeddings()
             vectorstore = MongoDBAtlasVectorSearch(collection, embeddings)
     """
@@ -206,17 +207,31 @@
         if not include_embedding:
             pipeline.append({"$project": {self._embedding_key: 0}})
 
         if post_filter_pipeline is not None:
             pipeline.extend(post_filter_pipeline)
         cursor = self._collection.aggregate(pipeline)  # type: ignore[arg-type]
         docs = []
+
+        def _make_serializable(obj: Dict[str, Any]) -> None:
+            for k, v in obj.items():
+                if isinstance(v, dict):
+                    _make_serializable(v)
+                elif isinstance(v, list) and v and isinstance(v[0], ObjectId):
+                    obj[k] = [json_util.default(item) for item in v]
+                elif isinstance(v, ObjectId):
+                    obj[k] = json_util.default(v)
+
         for res in cursor:
             text = res.pop(self._text_key)
             score = res.pop("score")
+            # Make every ObjectId found JSON-Serializable
+            # following format used in bson.json_util.loads
+            # e.g. loads('{"_id": {"$oid": "664..."}}') == {'_id': ObjectId('664..')} # noqa: E501
+            _make_serializable(res)
             docs.append((Document(page_content=text, metadata=res), score))
         return docs
 
     def similarity_search_with_score(
         self,
         query: str,
         k: int = 4,
@@ -348,16 +363,16 @@
 
         This is intended to be a quick way to get started.
 
         Example:
             .. code-block:: python
                 from pymongo import MongoClient
 
-                from langchain_community.vectorstores import MongoDBAtlasVectorSearch
-                from langchain_community.embeddings import OpenAIEmbeddings
+                from langchain_mongodb import MongoDBAtlasVectorSearch
+                from langchain_openai import OpenAIEmbeddings
 
                 mongo_client = MongoClient("<YOUR-CONNECTION-STRING>")
                 collection = mongo_client["<db_name>"]["<collection_name>"]
                 embeddings = OpenAIEmbeddings()
                 vectorstore = MongoDBAtlasVectorSearch.from_texts(
                     texts,
                     embeddings,
```

### Comparing `langchain_mongodb-0.1.3/pyproject.toml` & `langchain_mongodb-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [tool.poetry]
 name = "langchain-mongodb"
-version = "0.1.3"
+version = "0.1.4"
 description = "An integration package connecting MongoDB and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/mongodb"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 pymongo = ">=4.6.1,<5.0"
-langchain-core = "^0.1.25"
+langchain-core = ">=0.1.46,<0.3"
 numpy = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain = { path = "../../langchain", develop = true }
 langchain-core = { path = "../../core", develop = true }
+langchain-text-splitters = { path = "../../text-splitters", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -52,15 +53,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
 
 [tool.mypy]
```

### Comparing `langchain_mongodb-0.1.3/PKG-INFO` & `langchain_mongodb-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-mongodb
-Version: 0.1.3
+Version: 0.1.4
 Summary: An integration package connecting MongoDB and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.25,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.46,<0.3)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pymongo (>=4.6.1,<5.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/mongodb
 Description-Content-Type: text/markdown
 
 # langchain-mongodb
```

