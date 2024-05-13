# Comparing `tmp/llama_index_postprocessor_flag_embedding_reranker-0.1.2.tar.gz` & `tmp/llama_index_postprocessor_flag_embedding_reranker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_flag_embedding_reranker-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_flag_embedding_reranker-0.1.3.tar", max compression
```

## Comparing `llama_index_postprocessor_flag_embedding_reranker-0.1.2.tar` & `llama_index_postprocessor_flag_embedding_reranker-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       64 2024-02-13 13:53:01.709784 llama_index_postprocessor_flag_embedding_reranker-0.1.2/README.md
--rw-r--r--   0        0        0      126 2024-02-13 13:53:01.710038 llama_index_postprocessor_flag_embedding_reranker-0.1.2/llama_index/postprocessor/flag_embedding_reranker/__init__.py
--rw-r--r--   0        0        0     2787 2024-02-13 13:53:01.710103 llama_index_postprocessor_flag_embedding_reranker-0.1.2/llama_index/postprocessor/flag_embedding_reranker/base.py
--rw-r--r--   0        0        0     1514 2024-02-21 18:47:01.693325 llama_index_postprocessor_flag_embedding_reranker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 llama_index_postprocessor_flag_embedding_reranker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-05-13 21:57:40.363680 llama_index_postprocessor_flag_embedding_reranker-0.1.3/README.md
+-rw-r--r--   0        0        0      126 2024-05-13 21:57:40.363680 llama_index_postprocessor_flag_embedding_reranker-0.1.3/llama_index/postprocessor/flag_embedding_reranker/__init__.py
+-rw-r--r--   0        0        0     3321 2024-05-13 21:57:40.363680 llama_index_postprocessor_flag_embedding_reranker-0.1.3/llama_index/postprocessor/flag_embedding_reranker/base.py
+-rw-r--r--   0        0        0     1515 2024-05-13 21:57:40.363680 llama_index_postprocessor_flag_embedding_reranker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 llama_index_postprocessor_flag_embedding_reranker-0.1.3/PKG-INFO
```

### Comparing `llama_index_postprocessor_flag_embedding_reranker-0.1.2/llama_index/postprocessor/flag_embedding_reranker/base.py` & `llama_index_postprocessor_flag_embedding_reranker-0.1.3/llama_index/postprocessor/flag_embedding_reranker/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from typing import Any, List, Optional
 
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.callbacks import CBEventType, EventPayload
+from llama_index.core.instrumentation import get_dispatcher
+from llama_index.core.instrumentation.events.rerank import (
+    ReRankEndEvent,
+    ReRankStartEvent,
+)
 from llama_index.core.postprocessor.types import BaseNodePostprocessor
 from llama_index.core.schema import MetadataMode, NodeWithScore, QueryBundle
 
+dispatcher = get_dispatcher(__name__)
+
 
 class FlagEmbeddingReranker(BaseNodePostprocessor):
     """Flag Embedding Reranker."""
 
     model: str = Field(description="BAAI Reranker model name.")
     top_n: int = Field(description="Number of nodes to return sorted by score.")
     use_fp16: bool = Field(description="Whether to use fp16 for inference.")
@@ -38,14 +45,24 @@
         return "FlagEmbeddingReranker"
 
     def _postprocess_nodes(
         self,
         nodes: List[NodeWithScore],
         query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
+        dispatch_event = dispatcher.get_dispatch_event()
+        dispatch_event(
+            ReRankStartEvent(
+                query=query_bundle,
+                nodes=nodes,
+                top_n=self.top_n,
+                model_name=self.model,
+            )
+        )
+
         if query_bundle is None:
             raise ValueError("Missing query bundle in extra info.")
         if len(nodes) == 0:
             return []
 
         query_and_nodes = [
             (
@@ -76,8 +93,9 @@
                 node.score = score
 
             new_nodes = sorted(nodes, key=lambda x: -x.score if x.score else 0)[
                 : self.top_n
             ]
             event.on_end(payload={EventPayload.NODES: new_nodes})
 
+        dispatch_event(ReRankEndEvent(nodes=new_nodes))
         return new_nodes
```

### Comparing `llama_index_postprocessor_flag_embedding_reranker-0.1.2/pyproject.toml` & `llama_index_postprocessor_flag_embedding_reranker-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor flag embedding reranker integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-flag-embedding-reranker"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.35"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_postprocessor_flag_embedding_reranker-0.1.2/PKG-INFO` & `llama_index_postprocessor_flag_embedding_reranker-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-flag-embedding-reranker
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index postprocessor flag embedding reranker integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: Flag Embedding Reranker
```

