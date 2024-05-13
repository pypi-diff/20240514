# Comparing `tmp/llama_index_postprocessor_colbert_rerank-0.1.1.tar.gz` & `tmp/llama_index_postprocessor_colbert_rerank-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_colbert_rerank-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_colbert_rerank-0.1.2.tar", max compression
```

## Comparing `llama_index_postprocessor_colbert_rerank-0.1.1.tar` & `llama_index_postprocessor_colbert_rerank-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      350 2024-02-23 20:04:18.607323 llama_index_postprocessor_colbert_rerank-0.1.1/README.md
--rw-r--r--   0        0        0      101 2024-02-23 20:04:18.607323 llama_index_postprocessor_colbert_rerank-0.1.1/llama_index/postprocessor/colbert_rerank/__init__.py
--rw-r--r--   0        0        0     4392 2024-02-24 00:50:02.667720 llama_index_postprocessor_colbert_rerank-0.1.1/llama_index/postprocessor/colbert_rerank/base.py
--rw-r--r--   0        0        0     1671 2024-02-24 00:54:24.363097 llama_index_postprocessor_colbert_rerank-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 llama_index_postprocessor_colbert_rerank-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      350 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/README.md
+-rw-r--r--   0        0        0      101 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/llama_index/postprocessor/colbert_rerank/__init__.py
+-rw-r--r--   0        0        0     4882 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/llama_index/postprocessor/colbert_rerank/base.py
+-rw-r--r--   0        0        0     1672 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 llama_index_postprocessor_colbert_rerank-0.1.2/PKG-INFO
```

### Comparing `llama_index_postprocessor_colbert_rerank-0.1.1/llama_index/postprocessor/colbert_rerank/base.py` & `llama_index_postprocessor_colbert_rerank-0.1.2/llama_index/postprocessor/colbert_rerank/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
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
 
 import torch
 from transformers import AutoTokenizer, AutoModel
 
 DEFAULT_COLBERT_MAX_LENGTH = 512
 
+dispatcher = get_dispatcher(__name__)
+
 
 class ColbertRerank(BaseNodePostprocessor):
     model: str = Field(description="Colbert model name.")
     top_n: int = Field(description="Number of nodes to return sorted by score.")
     device: str = Field(
         default="cpu",
         description="Device to use for sentence transformer.",
@@ -74,14 +81,21 @@
         return rerank_score_list
 
     def _postprocess_nodes(
         self,
         nodes: List[NodeWithScore],
         query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
+        dispatch_event = dispatcher.get_dispatch_event()
+        dispatch_event(
+            ReRankStartEvent(
+                query=query_bundle, nodes=nodes, top_n=self.top_n, model_name=self.model
+            )
+        )
+
         if query_bundle is None:
             raise ValueError("Missing query bundle in extra info.")
         if len(nodes) == 0:
             return []
 
         nodes_text_list = [
             str(node.node.get_content(metadata_mode=MetadataMode.EMBED))
@@ -108,8 +122,9 @@
                 node.score = float(score)
 
             reranked_nodes = sorted(nodes, key=lambda x: -x.score if x.score else 0)[
                 : self.top_n
             ]
             event.on_end(payload={EventPayload.NODES: reranked_nodes})
 
+        dispatch_event(ReRankEndEvent(nodes=reranked_nodes))
         return reranked_nodes
```

### Comparing `llama_index_postprocessor_colbert_rerank-0.1.1/pyproject.toml` & `llama_index_postprocessor_colbert_rerank-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor colbert-rerank integration"
+exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-colbert-rerank"
 packages = [{include = "llama_index/"}]
-exclude = ["**/BUILD"]
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.0"
+llama-index-core = "^0.10.35"
 torch = "^2.2.0"
 transformers = "^4.37.2"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
```

### Comparing `llama_index_postprocessor_colbert_rerank-0.1.1/PKG-INFO` & `llama_index_postprocessor_colbert_rerank-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-colbert-rerank
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index postprocessor colbert-rerank integration
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
-Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Requires-Dist: torch (>=2.2.0,<3.0.0)
 Requires-Dist: transformers (>=4.37.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: Colbert Rerank
 
 [Colbert](https://github.com/stanford-futuredata/ColBERT): ColBERT is a fast and accurate retrieval model, enabling scalable BERT-based search over large text collections in tens of milliseconds.
```

