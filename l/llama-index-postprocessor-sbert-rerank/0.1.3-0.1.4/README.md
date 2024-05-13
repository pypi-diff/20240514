# Comparing `tmp/llama_index_postprocessor_sbert_rerank-0.1.3.tar.gz` & `tmp/llama_index_postprocessor_sbert_rerank-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_sbert_rerank-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_sbert_rerank-0.1.4.tar", max compression
```

## Comparing `llama_index_postprocessor_sbert_rerank-0.1.3.tar` & `llama_index_postprocessor_sbert_rerank-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       53 2024-02-13 13:53:01.713292 llama_index_postprocessor_sbert_rerank-0.1.3/README.md
--rw-r--r--   0        0        0      123 2024-02-13 13:53:01.713497 llama_index_postprocessor_sbert_rerank-0.1.3/llama_index/postprocessor/sbert_rerank/__init__.py
--rw-r--r--   0        0        0     3338 2024-02-20 18:45:10.280837 llama_index_postprocessor_sbert_rerank-0.1.3/llama_index/postprocessor/sbert_rerank/base.py
--rw-r--r--   0        0        0     1485 2024-02-21 18:50:46.825726 llama_index_postprocessor_sbert_rerank-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 llama_index_postprocessor_sbert_rerank-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       53 2024-05-13 21:57:40.367680 llama_index_postprocessor_sbert_rerank-0.1.4/README.md
+-rw-r--r--   0        0        0      123 2024-05-13 21:57:40.367680 llama_index_postprocessor_sbert_rerank-0.1.4/llama_index/postprocessor/sbert_rerank/__init__.py
+-rw-r--r--   0        0        0     3872 2024-05-13 21:57:40.367680 llama_index_postprocessor_sbert_rerank-0.1.4/llama_index/postprocessor/sbert_rerank/base.py
+-rw-r--r--   0        0        0     1486 2024-05-13 21:57:40.367680 llama_index_postprocessor_sbert_rerank-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 llama_index_postprocessor_sbert_rerank-0.1.4/PKG-INFO
```

### Comparing `llama_index_postprocessor_sbert_rerank-0.1.3/llama_index/postprocessor/sbert_rerank/base.py` & `llama_index_postprocessor_sbert_rerank-0.1.4/llama_index/postprocessor/sbert_rerank/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,24 @@
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
 from llama_index.core.utils import infer_torch_device
 
 DEFAULT_SENTENCE_TRANSFORMER_MAX_LENGTH = 512
 
+dispatcher = get_dispatcher(__name__)
+
 
 class SentenceTransformerRerank(BaseNodePostprocessor):
     model: str = Field(description="Sentence transformer model name.")
     top_n: int = Field(description="Number of nodes to return sorted by score.")
     device: str = Field(
         default="cpu",
         description="Device to use for sentence transformer.",
@@ -52,14 +59,24 @@
         return "SentenceTransformerRerank"
 
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
@@ -89,8 +106,9 @@
                 node.score = float(score)
 
             new_nodes = sorted(nodes, key=lambda x: -x.score if x.score else 0)[
                 : self.top_n
             ]
             event.on_end(payload={EventPayload.NODES: new_nodes})
 
+        dispatch_event(ReRankEndEvent(nodes=new_nodes))
         return new_nodes
```

### Comparing `llama_index_postprocessor_sbert_rerank-0.1.3/pyproject.toml` & `llama_index_postprocessor_sbert_rerank-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor sbert rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-sbert-rerank"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
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

### Comparing `llama_index_postprocessor_sbert_rerank-0.1.3/PKG-INFO` & `llama_index_postprocessor_sbert_rerank-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-sbert-rerank
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index postprocessor sbert rerank integration
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
 
 # LlamaIndex Postprocessor Integration: Sbert Rerank
```

