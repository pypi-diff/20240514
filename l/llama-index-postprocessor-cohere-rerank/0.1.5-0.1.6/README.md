# Comparing `tmp/llama_index_postprocessor_cohere_rerank-0.1.5.tar.gz` & `tmp/llama_index_postprocessor_cohere_rerank-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_cohere_rerank-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_cohere_rerank-0.1.6.tar", max compression
```

## Comparing `llama_index_postprocessor_cohere_rerank-0.1.5.tar` & `llama_index_postprocessor_cohere_rerank-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       54 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/README.md
--rw-r--r--   0        0        0       98 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/llama_index/postprocessor/cohere_rerank/__init__.py
--rw-r--r--   0        0        0     3168 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/llama_index/postprocessor/cohere_rerank/base.py
--rw-r--r--   0        0        0     1493 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 llama_index_postprocessor_cohere_rerank-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/README.md
+-rw-r--r--   0        0        0       98 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/llama_index/postprocessor/cohere_rerank/__init__.py
+-rw-r--r--   0        0        0     3168 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/llama_index/postprocessor/cohere_rerank/base.py
+-rw-r--r--   0        0        0     1494 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_postprocessor_cohere_rerank-0.1.6/PKG-INFO
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.5/llama_index/postprocessor/cohere_rerank/base.py` & `llama_index_postprocessor_cohere_rerank-0.1.6/llama_index/postprocessor/cohere_rerank/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.5/pyproject.toml` & `llama_index_postprocessor_cohere_rerank-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor cohere rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-cohere-rerank"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.35"
 cohere = "^5.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.5/PKG-INFO` & `llama_index_postprocessor_cohere_rerank-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-cohere-rerank
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index postprocessor cohere rerank integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cohere (>=5.1.1,<6.0.0)
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: Cohere Rerank
```

