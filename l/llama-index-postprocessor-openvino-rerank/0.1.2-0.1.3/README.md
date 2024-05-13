# Comparing `tmp/llama_index_postprocessor_openvino_rerank-0.1.2.tar.gz` & `tmp/llama_index_postprocessor_openvino_rerank-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_openvino_rerank-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_openvino_rerank-0.1.3.tar", max compression
```

## Comparing `llama_index_postprocessor_openvino_rerank-0.1.2.tar` & `llama_index_postprocessor_openvino_rerank-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       56 2024-04-10 20:01:21.712696 llama_index_postprocessor_openvino_rerank-0.1.2/README.md
--rw-r--r--   0        0        0      104 2024-04-10 20:01:21.712696 llama_index_postprocessor_openvino_rerank-0.1.2/llama_index/postprocessor/openvino_rerank/__init__.py
--rw-r--r--   0        0        0     6391 2024-04-10 20:01:21.712696 llama_index_postprocessor_openvino_rerank-0.1.2/llama_index/postprocessor/openvino_rerank/base.py
--rw-r--r--   0        0        0     1589 2024-04-10 20:01:21.712696 llama_index_postprocessor_openvino_rerank-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 llama_index_postprocessor_openvino_rerank-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-05-13 21:57:40.367680 llama_index_postprocessor_openvino_rerank-0.1.3/README.md
+-rw-r--r--   0        0        0      104 2024-05-13 21:57:40.367680 llama_index_postprocessor_openvino_rerank-0.1.3/llama_index/postprocessor/openvino_rerank/__init__.py
+-rw-r--r--   0        0        0     6930 2024-05-13 21:57:40.367680 llama_index_postprocessor_openvino_rerank-0.1.3/llama_index/postprocessor/openvino_rerank/base.py
+-rw-r--r--   0        0        0     1590 2024-05-13 21:57:40.367680 llama_index_postprocessor_openvino_rerank-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 llama_index_postprocessor_openvino_rerank-0.1.3/PKG-INFO
```

### Comparing `llama_index_postprocessor_openvino_rerank-0.1.2/llama_index/postprocessor/openvino_rerank/base.py` & `llama_index_postprocessor_openvino_rerank-0.1.3/llama_index/postprocessor/openvino_rerank/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from typing import Any, List, Optional, Dict
 from pathlib import Path
 import numpy as np
 
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
 
 from transformers import AutoTokenizer
 from optimum.intel.openvino import OVModelForSequenceClassification
 
 DEFAULT_COLBERT_MAX_LENGTH = 512
 
+dispatcher = get_dispatcher(__name__)
+
 
 class OpenVINORerank(BaseNodePostprocessor):
     model: str = Field(description="Huggingface model id or local path.")
     top_n: int = Field(description="Number of nodes to return sorted by score.")
     keep_retrieval_score: bool = Field(
         default=False,
         description="Whether to keep the retrieval score in metadata.",
@@ -123,14 +130,24 @@
         )
 
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
 
         nodes_text_list = [
             str(node.node.get_content(metadata_mode=MetadataMode.EMBED))
@@ -168,8 +185,9 @@
                 node.score = float(score)
 
             reranked_nodes = sorted(nodes, key=lambda x: -x.score if x.score else 0)[
                 : self.top_n
             ]
             event.on_end(payload={EventPayload.NODES: reranked_nodes})
 
+        dispatch_event(ReRankEndEvent(nodes=reranked_nodes))
         return reranked_nodes
```

### Comparing `llama_index_postprocessor_openvino_rerank-0.1.2/pyproject.toml` & `llama_index_postprocessor_openvino_rerank-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor openvino rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-openvino-rerank"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.35"
 huggingface-hub = "^0.20.3"
 
 [tool.poetry.dependencies.optimum]
 extras = ["openvino"]
 version = "^1.18.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_postprocessor_openvino_rerank-0.1.2/PKG-INFO` & `llama_index_postprocessor_openvino_rerank-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-openvino-rerank
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index postprocessor openvino rerank integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: huggingface-hub (>=0.20.3,<0.21.0)
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Requires-Dist: optimum[openvino] (>=1.18.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: OpenVINO Rerank
```

