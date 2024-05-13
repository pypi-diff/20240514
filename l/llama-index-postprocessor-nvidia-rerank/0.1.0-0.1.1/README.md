# Comparing `tmp/llama_index_postprocessor_nvidia_rerank-0.1.0.tar.gz` & `tmp/llama_index_postprocessor_nvidia_rerank-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_nvidia_rerank-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_nvidia_rerank-0.1.1.tar", max compression
```

## Comparing `llama_index_postprocessor_nvidia_rerank-0.1.0.tar` & `llama_index_postprocessor_nvidia_rerank-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3559 2024-05-03 17:02:12.168127 llama_index_postprocessor_nvidia_rerank-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-05-03 17:02:12.168127 llama_index_postprocessor_nvidia_rerank-0.1.0/llama_index/postprocessor/nvidia_rerank/BUILD
--rw-r--r--   0        0        0       99 2024-05-03 17:02:12.168127 llama_index_postprocessor_nvidia_rerank-0.1.0/llama_index/postprocessor/nvidia_rerank/__init__.py
--rw-r--r--   0        0        0     7935 2024-05-03 17:02:12.172127 llama_index_postprocessor_nvidia_rerank-0.1.0/llama_index/postprocessor/nvidia_rerank/base.py
--rw-r--r--   0        0        0     1709 2024-05-03 17:02:12.172127 llama_index_postprocessor_nvidia_rerank-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4138 1970-01-01 00:00:00.000000 llama_index_postprocessor_nvidia_rerank-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3559 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/BUILD
+-rw-r--r--   0        0        0       99 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/__init__.py
+-rw-r--r--   0        0        0     8583 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/base.py
+-rw-r--r--   0        0        0     1710 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 llama_index_postprocessor_nvidia_rerank-0.1.1/PKG-INFO
```

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.0/README.md` & `llama_index_postprocessor_nvidia_rerank-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.0/llama_index/postprocessor/nvidia_rerank/base.py` & `llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from typing import Any, List, Optional, Literal, Generator
 
 from urllib.parse import urlparse
 from llama_index.core.bridge.pydantic import Field, PrivateAttr, BaseModel
 from llama_index.core.callbacks import CBEventType, EventPayload
+from llama_index.core.instrumentation import get_dispatcher
+from llama_index.core.instrumentation.events.rerank import (
+    ReRankEndEvent,
+    ReRankStartEvent,
+)
 from llama_index.core.postprocessor.types import BaseNodePostprocessor
-from llama_index.core.schema import NodeWithScore, QueryBundle
+from llama_index.core.schema import MetadataMode, NodeWithScore, QueryBundle
 import requests
 
 from llama_index.core.base.llms.generic_utils import get_from_param_or_env
 
 
 DEFAULT_MODEL = "nv-rerank-qa-mistral-4b:1"
 DEFAULT_BASE_URL = "https://ai.api.nvidia.com/v1"
 
+dispatcher = get_dispatcher(__name__)
+
 
 class Model(BaseModel):
     id: str
 
 
 class NVIDIARerank(BaseNodePostprocessor):
     """NVIDIA's API Catalog Reranker Connector."""
@@ -130,14 +137,24 @@
         return "NVIDIARerank"
 
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
             raise ValueError(
                 "Missing query bundle in extra info. Please do not give empty query!"
             )
         if len(nodes) == 0:
             return []
 
@@ -163,15 +180,18 @@
             },
         ) as event:
             results = []
             for batch in batched(nodes, self.max_batch_size):
                 payloads = {
                     "model": self.model,
                     "query": {"text": query_bundle.query_str},
-                    "passages": [{"text": n.get_content()} for n in batch],
+                    "passages": [
+                        {"text": n.get_content(metadata_mode=MetadataMode.EMBED)}
+                        for n in batch
+                    ],
                 }
                 # the hosted NIM path is different from the local NIM path
                 url = self._base_url
                 if self._mode == "nvidia":
                     url += "/retrieval/nvidia/reranking"
                 else:
                     url += "/ranking"
@@ -207,8 +227,9 @@
                         )
                     )
             if len(nodes) > self.max_batch_size:
                 results.sort(key=lambda x: x.score, reverse=True)
             results = results[: self.top_n]
             event.on_end(payload={EventPayload.NODES: results})
 
+        dispatch_event(ReRankEndEvent(nodes=results))
         return results
```

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.0/pyproject.toml` & `llama_index_postprocessor_nvidia_rerank-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor nvidia_rerank integration"
 license = "MIT"
 name = "llama-index-postprocessor-nvidia-rerank"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.0"
+llama-index-core = "^0.10.35"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 faker = "^24.14.0"
 ipython = "8.10.0"
 jupyter = "^1.0.0"
```

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.0/PKG-INFO` & `llama_index_postprocessor_nvidia_rerank-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-nvidia-rerank
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index postprocessor nvidia_rerank integration
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
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: Nvidia_Rerank
 
 The `llama-index-postprocessor-nvidia-rerank` package contains LlamaIndex integrations for rerank model powered by the [NVIDIA AI Foundation Model](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) playground environment.
 
 > [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) give users easy access to hosted endpoints for generative AI models like Llama-2, SteerLM, Mistral, etc. Using the API, you can query live endpoints available on the [NVIDIA GPU Cloud (NGC)](https://catalog.ngc.nvidia.com/ai-foundation-models) to get quick results from a DGX-hosted cloud compute environment. All models are source-accessible and can be deployed on your own compute cluster.
```

