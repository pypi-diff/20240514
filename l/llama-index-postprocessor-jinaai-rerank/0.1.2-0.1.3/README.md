# Comparing `tmp/llama_index_postprocessor_jinaai_rerank-0.1.2.tar.gz` & `tmp/llama_index_postprocessor_jinaai_rerank-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_jinaai_rerank-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_jinaai_rerank-0.1.3.tar", max compression
```

## Comparing `llama_index_postprocessor_jinaai_rerank-0.1.2.tar` & `llama_index_postprocessor_jinaai_rerank-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      481 2024-02-28 16:22:35.192345 llama_index_postprocessor_jinaai_rerank-0.1.2/README.md
--rw-r--r--   0        0        0       94 2024-02-28 16:22:35.192648 llama_index_postprocessor_jinaai_rerank-0.1.2/llama_index/postprocessor/jinaai_rerank/__init__.py
--rw-r--r--   0        0        0     2889 2024-02-28 16:22:35.192762 llama_index_postprocessor_jinaai_rerank-0.1.2/llama_index/postprocessor/jinaai_rerank/base.py
--rw-r--r--   0        0        0     1489 2024-02-28 16:22:35.192880 llama_index_postprocessor_jinaai_rerank-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 llama_index_postprocessor_jinaai_rerank-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      481 2024-05-13 21:57:40.363680 llama_index_postprocessor_jinaai_rerank-0.1.3/README.md
+-rw-r--r--   0        0        0       94 2024-05-13 21:57:40.363680 llama_index_postprocessor_jinaai_rerank-0.1.3/llama_index/postprocessor/jinaai_rerank/__init__.py
+-rw-r--r--   0        0        0     3521 2024-05-13 21:57:40.363680 llama_index_postprocessor_jinaai_rerank-0.1.3/llama_index/postprocessor/jinaai_rerank/base.py
+-rw-r--r--   0        0        0     1490 2024-05-13 21:57:40.363680 llama_index_postprocessor_jinaai_rerank-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 llama_index_postprocessor_jinaai_rerank-0.1.3/PKG-INFO
```

### Comparing `llama_index_postprocessor_jinaai_rerank-0.1.2/llama_index/postprocessor/jinaai_rerank/base.py` & `llama_index_postprocessor_jinaai_rerank-0.1.3/llama_index/postprocessor/jinaai_rerank/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from typing import Any, List, Optional
 import requests
 
 from llama_index.core.base.llms.generic_utils import get_from_param_or_env
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
 
 API_URL = "https://api.jina.ai/v1/rerank"
 
+dispatcher = get_dispatcher(__name__)
+
 
 class JinaRerank(BaseNodePostprocessor):
     api_key: str = Field(default=None, description="The JinaAI API key.")
     model: str = Field(
         default="jina-reranker-v1-base-en",
         description="The model to use when calling Jina AI API",
     )
@@ -40,29 +47,42 @@
         return "JinaRerank"
 
     def _postprocess_nodes(
         self,
         nodes: List[NodeWithScore],
         query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
+        dispatcher_event = dispatcher.get_dispatch_event()
+        dispatcher_event(
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
 
         with self.callback_manager.event(
             CBEventType.RERANKING,
             payload={
                 EventPayload.NODES: nodes,
                 EventPayload.MODEL_NAME: self.model,
                 EventPayload.QUERY_STR: query_bundle.query_str,
                 EventPayload.TOP_K: self.top_n,
             },
         ) as event:
-            texts = [node.node.get_content() for node in nodes]
+            texts = [
+                node.node.get_content(metadata_mode=MetadataMode.EMBED)
+                for node in nodes
+            ]
             resp = self._session.post(  # type: ignore
                 API_URL,
                 json={
                     "query": query_bundle.query_str,
                     "documents": texts,
                     "model": self.model,
                     "top_n": self.top_n,
@@ -77,8 +97,9 @@
             for result in results:
                 new_node_with_score = NodeWithScore(
                     node=nodes[result["index"]].node, score=result["relevance_score"]
                 )
                 new_nodes.append(new_node_with_score)
             event.on_end(payload={EventPayload.NODES: new_nodes})
 
+        dispatcher_event(ReRankEndEvent(nodes=new_nodes))
         return new_nodes
```

### Comparing `llama_index_postprocessor_jinaai_rerank-0.1.2/pyproject.toml` & `llama_index_postprocessor_jinaai_rerank-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Joan Fontanals <joan.fontanals.martinez@jina.ai>"]
 description = "llama-index postprocessor jinaai rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-jinaai-rerank"
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

### Comparing `llama_index_postprocessor_jinaai_rerank-0.1.2/PKG-INFO` & `llama_index_postprocessor_jinaai_rerank-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-jinaai-rerank
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index postprocessor jinaai rerank integration
 License: MIT
 Author: Joan Fontanals
 Author-email: joan.fontanals.martinez@jina.ai
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
 
 # LlamaIndex Postprocessor Integration: Jina AI Rerank
 
 Jina Rerank is based on [Jina Reranking](), which is a state-of-the-art reranking model in terms of
 
 1. Input context length - Jina Reranking is capable of accepting 8K-length input context
```

