# Comparing `tmp/llama_index_postprocessor_voyageai_rerank-0.1.1.tar.gz` & `tmp/llama_index_postprocessor_voyageai_rerank-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_voyageai_rerank-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_voyageai_rerank-0.1.2.tar", max compression
```

## Comparing `llama_index_postprocessor_voyageai_rerank-0.1.1.tar` & `llama_index_postprocessor_voyageai_rerank-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       56 2024-03-26 16:04:35.563567 llama_index_postprocessor_voyageai_rerank-0.1.1/README.md
--rw-r--r--   0        0        0       17 2024-03-26 16:04:35.563774 llama_index_postprocessor_voyageai_rerank-0.1.1/llama_index/postprocessor/voyageai_rerank/BUILD
--rw-r--r--   0        0        0      104 2024-03-26 16:04:35.563882 llama_index_postprocessor_voyageai_rerank-0.1.1/llama_index/postprocessor/voyageai_rerank/__init__.py
--rw-r--r--   0        0        0     2682 2024-03-26 16:04:35.564125 llama_index_postprocessor_voyageai_rerank-0.1.1/llama_index/postprocessor/voyageai_rerank/base.py
--rw-r--r--   0        0        0     1630 2024-03-26 22:08:46.103338 llama_index_postprocessor_voyageai_rerank-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 llama_index_postprocessor_voyageai_rerank-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-05-13 21:57:40.367680 llama_index_postprocessor_voyageai_rerank-0.1.2/README.md
+-rw-r--r--   0        0        0       17 2024-05-13 21:57:40.367680 llama_index_postprocessor_voyageai_rerank-0.1.2/llama_index/postprocessor/voyageai_rerank/BUILD
+-rw-r--r--   0        0        0      104 2024-05-13 21:57:40.367680 llama_index_postprocessor_voyageai_rerank-0.1.2/llama_index/postprocessor/voyageai_rerank/__init__.py
+-rw-r--r--   0        0        0     3259 2024-05-13 21:57:40.367680 llama_index_postprocessor_voyageai_rerank-0.1.2/llama_index/postprocessor/voyageai_rerank/base.py
+-rw-r--r--   0        0        0     1631 2024-05-13 21:57:40.367680 llama_index_postprocessor_voyageai_rerank-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 llama_index_postprocessor_voyageai_rerank-0.1.2/PKG-INFO
```

### Comparing `llama_index_postprocessor_voyageai_rerank-0.1.1/llama_index/postprocessor/voyageai_rerank/base.py` & `llama_index_postprocessor_voyageai_rerank-0.1.2/llama_index/postprocessor/voyageai_rerank/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from typing import Any, List, Optional
 
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.callbacks import CBEventType, EventPayload
+from llama_index.core.instrumentation import get_dispatcher
+from llama_index.core.instrumentation.events.rerank import (
+    ReRankEndEvent,
+    ReRankStartEvent,
+)
 from llama_index.core.postprocessor.types import BaseNodePostprocessor
-from llama_index.core.schema import NodeWithScore, QueryBundle
+from llama_index.core.schema import MetadataMode, NodeWithScore, QueryBundle
+
+dispatcher = get_dispatcher(__name__)
 
 
 class VoyageAIRerank(BaseNodePostprocessor):
     model: str = Field(description="Name of the model to use.")
     top_k: int = Field(
         description="The number of most relevant documents to return. If not specified, the reranking results of all documents will be returned."
     )
@@ -39,29 +46,39 @@
         return "VoyageAIRerank"
 
     def _postprocess_nodes(
         self,
         nodes: List[NodeWithScore],
         query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
+        dispatch_event = dispatcher.get_dispatch_event()
+        dispatch_event(
+            ReRankStartEvent(
+                query=query_bundle, nodes=nodes, top_n=self.top_k, model_name=self.model
+            )
+        )
+
         if query_bundle is None:
             raise ValueError("Missing query bundle in extra info.")
         if len(nodes) == 0:
             return []
 
         with self.callback_manager.event(
             CBEventType.RERANKING,
             payload={
                 EventPayload.NODES: nodes,
                 EventPayload.MODEL_NAME: self.model,
                 EventPayload.QUERY_STR: query_bundle.query_str,
                 EventPayload.TOP_K: self.top_k,
             },
         ) as event:
-            texts = [node.node.get_content() for node in nodes]
+            texts = [
+                node.node.get_content(metadata_mode=MetadataMode.EMBED)
+                for node in nodes
+            ]
             results = self._client.rerank(
                 model=self.model,
                 top_k=self.top_k,
                 query=query_bundle.query_str,
                 documents=texts,
                 truncation=self.truncation,
             )
@@ -70,8 +87,9 @@
             for result in results:
                 new_node_with_score = NodeWithScore(
                     node=nodes[result.index].node, score=result.relevance_score
                 )
                 new_nodes.append(new_node_with_score)
             event.on_end(payload={EventPayload.NODES: new_nodes})
 
+        dispatch_event(ReRankEndEvent(nodes=new_nodes))
         return new_nodes
```

### Comparing `llama_index_postprocessor_voyageai_rerank-0.1.1/pyproject.toml` & `llama_index_postprocessor_voyageai_rerank-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor voyageai-rerank integration"
 license = "MIT"
 name = "llama-index-postprocessor-voyageai-rerank"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.0"
+llama-index-core = "^0.10.35"
 voyageai = "^0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
```

### Comparing `llama_index_postprocessor_voyageai_rerank-0.1.1/PKG-INFO` & `llama_index_postprocessor_voyageai_rerank-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-voyageai-rerank
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index postprocessor voyageai-rerank integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Requires-Dist: voyageai (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: Voyageai-Rerank
```

