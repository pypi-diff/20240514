# Comparing `tmp/llama_index_postprocessor_rankllm_rerank-0.1.2.tar.gz` & `tmp/llama_index_postprocessor_rankllm_rerank-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_rankllm_rerank-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_rankllm_rerank-0.1.3.tar", max compression
```

## Comparing `llama_index_postprocessor_rankllm_rerank-0.1.2.tar` & `llama_index_postprocessor_rankllm_rerank-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2156 2024-04-03 22:38:05.992227 llama_index_postprocessor_rankllm_rerank-0.1.2/README.md
--rw-r--r--   0        0        0      102 2024-04-03 22:38:05.992227 llama_index_postprocessor_rankllm_rerank-0.1.2/llama_index/postprocessor/rankllm_rerank/__init__.py
--rw-r--r--   0        0        0     4436 2024-04-03 22:38:05.992227 llama_index_postprocessor_rankllm_rerank-0.1.2/llama_index/postprocessor/rankllm_rerank/base.py
--rw-r--r--   0        0        0     1618 2024-04-03 22:38:05.992227 llama_index_postprocessor_rankllm_rerank-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 llama_index_postprocessor_rankllm_rerank-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2156 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankllm_rerank-0.1.3/README.md
+-rw-r--r--   0        0        0      102 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankllm_rerank-0.1.3/llama_index/postprocessor/rankllm_rerank/__init__.py
+-rw-r--r--   0        0        0     5065 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankllm_rerank-0.1.3/llama_index/postprocessor/rankllm_rerank/base.py
+-rw-r--r--   0        0        0     1619 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankllm_rerank-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 llama_index_postprocessor_rankllm_rerank-0.1.3/PKG-INFO
```

### Comparing `llama_index_postprocessor_rankllm_rerank-0.1.2/README.md` & `llama_index_postprocessor_rankllm_rerank-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_postprocessor_rankllm_rerank-0.1.2/llama_index/postprocessor/rankllm_rerank/base.py` & `llama_index_postprocessor_rankllm_rerank-0.1.3/llama_index/postprocessor/rankllm_rerank/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from typing import Any, List, Optional
 from enum import Enum
 
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
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
 
 
 class RankLLMRerank(BaseNodePostprocessor):
     """RankLLM-based reranker."""
 
     top_n: int = Field(default=5, description="Top N nodes to return from reranking.")
     model: str = Field(default="zephyr", description="Reranker model name.")
@@ -81,15 +88,28 @@
         return "RankLLMRerank"
 
     def _postprocess_nodes(
         self,
         nodes: List[NodeWithScore],
         query_bundle: QueryBundle,
     ) -> List[NodeWithScore]:
-        docs = [(node.get_content(), node.get_score()) for node in nodes]
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
+        docs = [
+            (node.get_content(metadata_mode=MetadataMode.EMBED), node.get_score())
+            for node in nodes
+        ]
 
         if self.with_retrieval:
             hits = [
                 {
                     "content": doc[0],
                     "qid": 1,
                     "docid": str(index),
@@ -127,14 +147,16 @@
 
         new_nodes: List[NodeWithScore] = []
         for hit in permutation[0].hits:
             idx: int = int(hit["docid"])
             new_nodes.append(
                 NodeWithScore(node=nodes[idx].node, score=nodes[idx].score)
             )
+
+        dispatch_event(ReRankEndEvent(nodes=new_nodes[: self.top_n]))
         return new_nodes[: self.top_n]
 
 
 class ModelType(Enum):
     VICUNA = "vicuna"
     ZEPHYR = "zephyr"
     GPT = "gpt"
```

### Comparing `llama_index_postprocessor_rankllm_rerank-0.1.2/pyproject.toml` & `llama_index_postprocessor_rankllm_rerank-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor rankllm-rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-rankllm-rerank"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.0"
+llama-index-core = "^0.10.35"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_postprocessor_rankllm_rerank-0.1.2/PKG-INFO` & `llama_index_postprocessor_rankllm_rerank-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-rankllm-rerank
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index postprocessor rankllm-rerank integration
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
 
 # LlamaIndex Postprocessor Integration: Rankllm-Rerank
 
 RankLLM offers a suite of listwise rerankers, albeit with focus on open source LLMs finetuned for the task. Currently, RankLLM supports 2 of these models: RankZephyr (`model="zephyr"`) and RankVicuna (`model="vicuna"`). RankLLM also support RankGPT usage (`model="gpt"`, `gpt_model="VALID_OPENAI_MODEL_NAME"`).
 
 Please `pip install llama-index-postprocessor-rankllm-rerank` to install RankLLM rerank package.
```

