# Comparing `tmp/not_again_ai-0.8.0.tar.gz` & `tmp/not_again_ai-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not_again_ai-0.8.0.tar", max compression
+gzip compressed data, was "not_again_ai-0.8.1.tar", max compression
```

## Comparing `not_again_ai-0.8.0.tar` & `not_again_ai-0.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.8.0/LICENSE
--rw-r--r--   0        0        0    12588 2024-05-06 13:18:28.310413 not_again_ai-0.8.0/README.md
--rw-r--r--   0        0        0     4258 2024-05-08 00:01:11.052089 not_again_ai-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.8.0/src/not_again_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/base/__init__.py
--rw-r--r--   0        0        0      949 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/base/file_system.py
--rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/base/parallel.py
--rw-r--r--   0        0        0      451 2024-04-20 17:53:46.881490 not_again_ai-0.8.0/src/not_again_ai/llm/__init__.py
--rw-r--r--   0        0        0     3070 2024-05-07 13:02:01.955836 not_again_ai-0.8.0/src/not_again_ai/llm/chat_completion.py
--rw-r--r--   0        0        0        0 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/__init__.py
--rw-r--r--   0        0        0     3682 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/chat_completion.py
--rw-r--r--   0        0        0      765 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/ollama_client.py
--rw-r--r--   0        0        0     2900 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/service.py
--rw-r--r--   0        0        0        0 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/__init__.py
--rw-r--r--   0        0        0     8623 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/chat_completion.py
--rw-r--r--   0        0        0     3435 2024-05-06 13:37:12.093962 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/context_management.py
--rw-r--r--   0        0        0     2500 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/embeddings.py
--rw-r--r--   0        0        0     2470 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/openai_client.py
--rw-r--r--   0        0        0     7094 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/prompts.py
--rw-r--r--   0        0        0     4301 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/tokens.py
--rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.8.0/src/not_again_ai/py.typed
--rw-r--r--   0        0        0      466 2024-04-20 17:53:46.881490 not_again_ai-0.8.0/src/not_again_ai/statistics/__init__.py
--rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.8.0/src/not_again_ai/statistics/dependence.py
--rw-r--r--   0        0        0      447 2024-04-20 17:53:46.881490 not_again_ai-0.8.0/src/not_again_ai/viz/__init__.py
--rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.8.0/src/not_again_ai/viz/barplots.py
--rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/viz/distributions.py
--rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/viz/scatterplot.py
--rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.8.0/src/not_again_ai/viz/time_series.py
--rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.8.0/src/not_again_ai/viz/utils.py
--rw-r--r--   0        0        0    14203 1970-01-01 00:00:00.000000 not_again_ai-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.8.1/LICENSE
+-rw-r--r--   0        0        0    12588 2024-05-06 13:18:28.310413 not_again_ai-0.8.1/README.md
+-rw-r--r--   0        0        0     4258 2024-05-13 23:27:49.935932 not_again_ai-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.8.1/src/not_again_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.8.1/src/not_again_ai/base/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-06 13:18:28.322414 not_again_ai-0.8.1/src/not_again_ai/base/file_system.py
+-rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.8.1/src/not_again_ai/base/parallel.py
+-rw-r--r--   0        0        0      451 2024-04-20 17:53:46.881490 not_again_ai-0.8.1/src/not_again_ai/llm/__init__.py
+-rw-r--r--   0        0        0     3070 2024-05-08 00:22:35.412143 not_again_ai-0.8.1/src/not_again_ai/llm/chat_completion.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:18:28.322414 not_again_ai-0.8.1/src/not_again_ai/llm/ollama/__init__.py
+-rw-r--r--   0        0        0     3682 2024-05-06 13:18:28.322414 not_again_ai-0.8.1/src/not_again_ai/llm/ollama/chat_completion.py
+-rw-r--r--   0        0        0      765 2024-05-06 13:18:28.322414 not_again_ai-0.8.1/src/not_again_ai/llm/ollama/ollama_client.py
+-rw-r--r--   0        0        0     2900 2024-05-06 13:18:28.322414 not_again_ai-0.8.1/src/not_again_ai/llm/ollama/service.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:22:35.412143 not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/__init__.py
+-rw-r--r--   0        0        0     8623 2024-05-08 00:22:35.412143 not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/chat_completion.py
+-rw-r--r--   0        0        0     3435 2024-05-08 00:22:35.412143 not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/context_management.py
+-rw-r--r--   0        0        0     2500 2024-05-08 00:22:35.412143 not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/embeddings.py
+-rw-r--r--   0        0        0     2470 2024-05-08 00:22:35.412143 not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/openai_client.py
+-rw-r--r--   0        0        0     7094 2024-05-08 00:22:35.412143 not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/prompts.py
+-rw-r--r--   0        0        0     4453 2024-05-13 23:33:55.652923 not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/tokens.py
+-rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.8.1/src/not_again_ai/py.typed
+-rw-r--r--   0        0        0      466 2024-04-20 17:53:46.881490 not_again_ai-0.8.1/src/not_again_ai/statistics/__init__.py
+-rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.8.1/src/not_again_ai/statistics/dependence.py
+-rw-r--r--   0        0        0      447 2024-04-20 17:53:46.881490 not_again_ai-0.8.1/src/not_again_ai/viz/__init__.py
+-rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.8.1/src/not_again_ai/viz/barplots.py
+-rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.8.1/src/not_again_ai/viz/distributions.py
+-rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.8.1/src/not_again_ai/viz/scatterplot.py
+-rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.8.1/src/not_again_ai/viz/time_series.py
+-rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.8.1/src/not_again_ai/viz/utils.py
+-rw-r--r--   0        0        0    14203 1970-01-01 00:00:00.000000 not_again_ai-0.8.1/PKG-INFO
```

### Comparing `not_again_ai-0.8.0/LICENSE` & `not_again_ai-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/README.md` & `not_again_ai-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/pyproject.toml` & `not_again_ai-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "not-again-ai"
-version = "0.8.0"
+version = "0.8.1"
 description = "Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place."
 authors = ["DaveCoDev <dave.co.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DaveCoDev/not-again-ai"
 documentation = "https://github.com/DaveCoDev/not-again-ai"
 classifiers = [
@@ -24,22 +24,22 @@
 # Some packages, such as scipy, constrain their upper bound of Python versions they support.
 # Without also constraining the upper bound here, Poetry will not select those versions and will
 # result in an old version being resolved/locked.
 python = "^3.11, <3.13"
 
 # Optional dependencies are defined here, and groupings are defined below.
 numpy = { version = "^1.26.4", optional = true }
-ollama = { version = "^0.1.9", optional = true }
-openai = { version = "^1.25.1", optional = true }
+ollama = { version = "^0.2.0", optional = true }
+openai = { version = "^1.29.0", optional = true }
 pandas = { version = "^2.2.2", optional = true }
 python-liquid = { version = "^1.12.1", optional = true }
 scipy = { version = "^1.13.0", optional = true }
 scikit-learn = { version = "^1.4.2", optional = true }
 seaborn = { version = "^0.13.2", optional = true }
-tiktoken = { version = "^0.6.0", optional = true }
+tiktoken = { version = "^0.7.0", optional = true }
 
 [tool.poetry.extras]
 llm = ["ollama", "openai", "python-liquid", "tiktoken"]
 statistics = ["numpy", "scikit-learn", "scipy"]
 viz = ["numpy", "pandas", "seaborn"]
 
 [tool.poetry.dev-dependencies]
```

### Comparing `not_again_ai-0.8.0/src/not_again_ai/base/file_system.py` & `not_again_ai-0.8.1/src/not_again_ai/base/file_system.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/base/parallel.py` & `not_again_ai-0.8.1/src/not_again_ai/base/parallel.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/chat_completion.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/chat_completion.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/ollama/chat_completion.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/ollama/chat_completion.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/ollama/ollama_client.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/ollama/ollama_client.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/ollama/service.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/ollama/service.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/chat_completion.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/chat_completion.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/context_management.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/context_management.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/embeddings.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/embeddings.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/openai_client.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/openai_client.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/prompts.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/prompts.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/tokens.py` & `not_again_ai-0.8.1/src/not_again_ai/llm/openai_api/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,23 +78,27 @@
         "gpt-4-0613",
         "gpt-4-32k-0613",
         "gpt-4-1106-preview",
         "gpt-4-turbo-preview",
         "gpt-4-0125-preview",
         "gpt-4-turbo",
         "gpt-4-turbo-2024-04-09",
+        "gpt-4o",
+        "gpt-4o-2024-05-13",
     }:
         tokens_per_message = 3  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         tokens_per_name = 1  # if there's a name, the role is omitted
     elif model == "gpt-3.5-turbo-0301":
         tokens_per_message = 4
         tokens_per_name = -1
     # Approximate catch-all. Assumes future versions of 3.5 and 4 will have the same token counts as the 0613 versions.
     elif "gpt-3.5-turbo" in model:
         return num_tokens_from_messages(messages, model="gpt-3.5-turbo-0613")
+    elif "gpt-4o" in model:
+        return num_tokens_from_messages(messages, model="gpt-4o-2024-05-13")
     elif "gpt-4" in model:
         return num_tokens_from_messages(messages, model="gpt-4-0613")
     else:
         raise NotImplementedError(
             f"""num_tokens_from_messages() is not implemented for model {model}.
 See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens."""
         )
```

### Comparing `not_again_ai-0.8.0/src/not_again_ai/statistics/dependence.py` & `not_again_ai-0.8.1/src/not_again_ai/statistics/dependence.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/viz/barplots.py` & `not_again_ai-0.8.1/src/not_again_ai/viz/barplots.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/viz/distributions.py` & `not_again_ai-0.8.1/src/not_again_ai/viz/distributions.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/viz/scatterplot.py` & `not_again_ai-0.8.1/src/not_again_ai/viz/scatterplot.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/src/not_again_ai/viz/time_series.py` & `not_again_ai-0.8.1/src/not_again_ai/viz/time_series.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.8.0/PKG-INFO` & `not_again_ai-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not-again-ai
-Version: 0.8.0
+Version: 0.8.1
 Summary: Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place.
 Home-page: https://github.com/DaveCoDev/not-again-ai
 License: MIT
 Author: DaveCoDev
 Author-email: dave.co.dev@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 3 - Alpha
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Provides-Extra: llm
 Provides-Extra: statistics
 Provides-Extra: viz
 Requires-Dist: numpy (>=1.26.4,<2.0.0) ; extra == "statistics" or extra == "viz"
-Requires-Dist: ollama (>=0.1.9,<0.2.0) ; extra == "llm"
-Requires-Dist: openai (>=1.25.1,<2.0.0) ; extra == "llm"
+Requires-Dist: ollama (>=0.2.0,<0.3.0) ; extra == "llm"
+Requires-Dist: openai (>=1.29.0,<2.0.0) ; extra == "llm"
 Requires-Dist: pandas (>=2.2.2,<3.0.0) ; extra == "viz"
 Requires-Dist: python-liquid (>=1.12.1,<2.0.0) ; extra == "llm"
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0) ; extra == "statistics"
 Requires-Dist: scipy (>=1.13.0,<2.0.0) ; extra == "statistics"
 Requires-Dist: seaborn (>=0.13.2,<0.14.0) ; extra == "viz"
-Requires-Dist: tiktoken (>=0.6.0,<0.7.0) ; extra == "llm"
+Requires-Dist: tiktoken (>=0.7.0,<0.8.0) ; extra == "llm"
 Project-URL: Documentation, https://github.com/DaveCoDev/not-again-ai
 Project-URL: Repository, https://github.com/DaveCoDev/not-again-ai
 Description-Content-Type: text/markdown
 
 # not-again-ai
 
 [![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/python-blueprint/actions)
```

