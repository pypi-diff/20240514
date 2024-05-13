# Comparing `tmp/llama_index_postprocessor_rankgpt_rerank-0.1.3.tar.gz` & `tmp/llama_index_postprocessor_rankgpt_rerank-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_rankgpt_rerank-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_rankgpt_rerank-0.1.4.tar", max compression
```

## Comparing `llama_index_postprocessor_rankgpt_rerank-0.1.3.tar` & `llama_index_postprocessor_rankgpt_rerank-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       55 2024-02-13 13:53:01.712075 llama_index_postprocessor_rankgpt_rerank-0.1.3/README.md
--rw-r--r--   0        0        0      101 2024-02-13 13:53:01.712327 llama_index_postprocessor_rankgpt_rerank-0.1.3/llama_index/postprocessor/rankgpt_rerank/__init__.py
--rw-r--r--   0        0        0     6383 2024-02-13 16:08:24.717506 llama_index_postprocessor_rankgpt_rerank-0.1.3/llama_index/postprocessor/rankgpt_rerank/base.py
--rw-r--r--   0        0        0     1479 2024-02-21 18:49:53.850286 llama_index_postprocessor_rankgpt_rerank-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 llama_index_postprocessor_rankgpt_rerank-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankgpt_rerank-0.1.4/README.md
+-rw-r--r--   0        0        0      101 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankgpt_rerank-0.1.4/llama_index/postprocessor/rankgpt_rerank/__init__.py
+-rw-r--r--   0        0        0     7121 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankgpt_rerank-0.1.4/llama_index/postprocessor/rankgpt_rerank/base.py
+-rw-r--r--   0        0        0     1480 2024-05-13 21:57:40.367680 llama_index_postprocessor_rankgpt_rerank-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 llama_index_postprocessor_rankgpt_rerank-0.1.4/PKG-INFO
```

### Comparing `llama_index_postprocessor_rankgpt_rerank-0.1.3/llama_index/postprocessor/rankgpt_rerank/base.py` & `llama_index_postprocessor_rankgpt_rerank-0.1.4/llama_index/postprocessor/rankgpt_rerank/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import logging
 from typing import Any, Dict, List, Optional, Sequence
 
 from llama_index.core.bridge.pydantic import Field
+from llama_index.core.instrumentation import get_dispatcher
+from llama_index.core.instrumentation.events.rerank import (
+    ReRankEndEvent,
+    ReRankStartEvent,
+)
 from llama_index.core.llms import LLM, ChatMessage, ChatResponse
 from llama_index.core.postprocessor.types import BaseNodePostprocessor
 from llama_index.core.prompts import BasePromptTemplate
 from llama_index.core.prompts.default_prompts import RANKGPT_RERANK_PROMPT
 from llama_index.core.prompts.mixin import PromptDictType
-from llama_index.core.schema import NodeWithScore, QueryBundle
+from llama_index.core.schema import MetadataMode, NodeWithScore, QueryBundle
 from llama_index.core.utils import print_text
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
+dispatcher = get_dispatcher(__name__)
 
 
 class RankGPTRerank(BaseNodePostprocessor):
     """RankGPT-based reranker."""
 
     top_n: int = Field(default=5, description="Top N nodes to return from reranking.")
     llm: Optional[LLM] = None
@@ -58,20 +64,33 @@
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
+                model_name=self.llm.metadata.model_name,
+            )
+        )
+
         if query_bundle is None:
             raise ValueError("Query bundle must be provided.")
 
         items = {
             "query": query_bundle.query_str,
-            "hits": [{"content": node.get_content()} for node in nodes],
+            "hits": [
+                {"content": node.get_content(metadata_mode=MetadataMode.EMBED)}
+                for node in nodes
+            ],
         }
 
         messages = self.create_permutation_instruction(item=items)
         permutation = self.run_llm(messages=messages)
         if permutation.message is not None and permutation.message.content is not None:
             rerank_ranks = self._receive_permutation(
                 items, str(permutation.message.content)
@@ -81,16 +100,19 @@
 
             initial_results: List[NodeWithScore] = []
 
             for idx in rerank_ranks:
                 initial_results.append(
                     NodeWithScore(node=nodes[idx].node, score=nodes[idx].score)
                 )
+
+            dispatch_event(ReRankEndEvent(nodes=initial_results[: self.top_n]))
             return initial_results[: self.top_n]
         else:
+            dispatch_event(ReRankEndEvent(nodes=nodes[: self.top_n]))
             return nodes[: self.top_n]
 
     def _get_prompts(self) -> PromptDictType:
         """Get prompts."""
         return {"rankgpt_rerank_prompt": self.rankgpt_rerank_prompt}
 
     def _update_prompts(self, prompts: PromptDictType) -> None:
```

### Comparing `llama_index_postprocessor_rankgpt_rerank-0.1.3/pyproject.toml` & `llama_index_postprocessor_rankgpt_rerank-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor rankgpt rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-rankgpt-rerank"
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

### Comparing `llama_index_postprocessor_rankgpt_rerank-0.1.3/PKG-INFO` & `llama_index_postprocessor_rankgpt_rerank-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-rankgpt-rerank
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index postprocessor rankgpt rerank integration
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
 
 # LlamaIndex Postprocessor Integration: Rankgpt Rerank
```

