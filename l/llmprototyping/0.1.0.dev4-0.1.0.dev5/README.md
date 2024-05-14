# Comparing `tmp/llmprototyping-0.1.0.dev4.tar.gz` & `tmp/llmprototyping-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmprototyping-0.1.0.dev4.tar", last modified: Thu May  9 11:09:13 2024, max compression
+gzip compressed data, was "llmprototyping-0.1.0.dev5.tar", last modified: Tue May 14 15:59:27 2024, max compression
```

## Comparing `llmprototyping-0.1.0.dev4.tar` & `llmprototyping-0.1.0.dev5.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.027473 llmprototyping-0.1.0.dev4/
--rw-r--r--   0 alejandro   (501) staff       (20)    11357 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev4/LICENSE
--rw-r--r--   0 alejandro   (501) staff       (20)     8044 2024-05-09 11:09:13.027415 llmprototyping-0.1.0.dev4/PKG-INFO
--rw-r--r--   0 alejandro   (501) staff       (20)     7326 2024-05-08 23:49:15.000000 llmprototyping-0.1.0.dev4/README.md
--rw-r--r--   0 alejandro   (501) staff       (20)       74 2024-05-09 11:09:13.027665 llmprototyping-0.1.0.dev4/setup.cfg
--rw-r--r--   0 alejandro   (501) staff       (20)     1152 2024-05-09 11:06:40.000000 llmprototyping-0.1.0.dev4/setup.py
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.024452 llmprototyping-0.1.0.dev4/src/
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.026377 llmprototyping-0.1.0.dev4/src/llmprototyping/
--rw-r--r--   0 alejandro   (501) staff       (20)      777 2024-05-09 10:01:17.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/__init__.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1919 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_interface.py
--rw-r--r--   0 alejandro   (501) staff       (20)        0 2024-05-09 09:48:40.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_ollama.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3148 2024-05-09 10:49:51.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_openai.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1159 2024-05-09 10:06:53.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/error.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1570 2024-05-09 10:44:25.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/factory.py
--rw-r--r--   0 alejandro   (501) staff       (20)     6457 2024-05-09 10:58:15.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_em_ollama.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3260 2024-05-08 23:25:51.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_groq.py
--rw-r--r--   0 alejandro   (501) staff       (20)     2909 2024-05-08 23:38:17.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_interface.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3573 2024-05-08 23:28:38.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_openai.py
--rw-r--r--   0 alejandro   (501) staff       (20)      434 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/serializable.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1930 2024-05-07 22:50:32.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/vectordb.py
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.027200 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/
--rw-r--r--   0 alejandro   (501) staff       (20)     8044 2024-05-09 11:09:12.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/PKG-INFO
--rw-r--r--   0 alejandro   (501) staff       (20)      659 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/SOURCES.txt
--rw-r--r--   0 alejandro   (501) staff       (20)        1 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/dependency_links.txt
--rw-r--r--   0 alejandro   (501) staff       (20)       48 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/requires.txt
--rw-r--r--   0 alejandro   (501) staff       (20)       15 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/top_level.txt
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-14 15:59:27.704349 llmprototyping-0.1.0.dev5/
+-rw-r--r--   0 alejandro   (501) staff       (20)    11357 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev5/LICENSE
+-rw-r--r--   0 alejandro   (501) staff       (20)     9232 2024-05-14 15:59:27.704242 llmprototyping-0.1.0.dev5/PKG-INFO
+-rw-r--r--   0 alejandro   (501) staff       (20)     8489 2024-05-14 15:56:40.000000 llmprototyping-0.1.0.dev5/README.md
+-rw-r--r--   0 alejandro   (501) staff       (20)       74 2024-05-14 15:59:27.704632 llmprototyping-0.1.0.dev5/setup.cfg
+-rw-r--r--   0 alejandro   (501) staff       (20)     1152 2024-05-14 15:57:31.000000 llmprototyping-0.1.0.dev5/setup.py
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-14 15:59:27.698958 llmprototyping-0.1.0.dev5/src/
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-14 15:59:27.703138 llmprototyping-0.1.0.dev5/src/llmprototyping/
+-rw-r--r--   0 alejandro   (501) staff       (20)      975 2024-05-14 11:16:28.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/__init__.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1062 2024-05-13 17:32:11.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/cache.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1919 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/embeddings_interface.py
+-rw-r--r--   0 alejandro   (501) staff       (20)        0 2024-05-09 09:48:40.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/embeddings_ollama.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3148 2024-05-09 10:49:51.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/embeddings_openai.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1168 2024-05-11 14:46:36.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/error.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1573 2024-05-11 14:46:36.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/factory.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     4273 2024-05-14 11:23:51.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/llm_anthropic.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     6463 2024-05-11 14:46:38.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/llm_em_ollama.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3263 2024-05-13 00:51:04.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/llm_groq.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     5941 2024-05-14 10:45:59.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/llm_interface.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3698 2024-05-14 10:57:54.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/llm_openai.py
+-rw-r--r--   0 alejandro   (501) staff       (20)      540 2024-05-11 23:22:41.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/serializable.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     2454 2024-05-12 23:21:20.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/templates.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1932 2024-05-11 14:46:40.000000 llmprototyping-0.1.0.dev5/src/llmprototyping/vectordb.py
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-14 15:59:27.704001 llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/
+-rw-r--r--   0 alejandro   (501) staff       (20)     9232 2024-05-14 15:59:27.000000 llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/PKG-INFO
+-rw-r--r--   0 alejandro   (501) staff       (20)      755 2024-05-14 15:59:27.000000 llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/SOURCES.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)        1 2024-05-14 15:59:27.000000 llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/dependency_links.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)       58 2024-05-14 15:59:27.000000 llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/requires.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)       15 2024-05-14 15:59:27.000000 llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/top_level.txt
```

### Comparing `llmprototyping-0.1.0.dev4/LICENSE` & `llmprototyping-0.1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev4/PKG-INFO` & `llmprototyping-0.1.0.dev5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: llmprototyping
-Version: 0.1.0.dev4
-Summary: A lightweight set of tools to use several llm and embeddings apis
-Home-page: https://github.com/alejandrolc/llmprototyping
-Author: Alejandro López Correa
-Keywords: llm,rag,openai,groq,ollama
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.9, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: groq
-Requires-Dist: openai
-Requires-Dist: tiktoken
-Requires-Dist: packaging
-Requires-Dist: faiss-cpu
-Requires-Dist: ollama
-
 # llmprototyping
 
 `llmprototyping` is a Python package designed to provide easy and uniform access to various large language model (LLM) and embedding APIs, along with basic functionality for building small-scale artificial intelligence applications.
 
 ## Features
 
 - **Uniform API Access**: Simplify your interactions with different LLM and embedding APIs using a single interface.
@@ -46,24 +25,29 @@
 
 ### chat completion models
 
 - groq/llama3-70b-8192
 - groq/llama3-8b-8192
 - groq/mixtral-8x7b-32768
 - groq/gemma-7b-it
+- openai/gpt-4o
 - openai/gpt-4-turbo
 - openai/gpt-4-turbo-preview
 - openai/gpt-3.5-turbo
+- anthropic/claude-3-opus-20240229
+- anthropic/claude-3-sonnet-20240229
+- anthropic/claude-3-haiku-20240307
 - ollama/*
 
 ### embedding models
 
 - openai/text-embedding-3-small
 - openai/text-embedding-3-large
 - openai/text-embedding-ada-002
+- ollama/*
 
 ## Usage
 
 Note: The examples use python-dotenv. This is not required by llmprototyping, so it needs to be installed separatedly. 
 
 ### Simple chat completion call
 
@@ -218,15 +202,15 @@
 
 print('chat completion models:')
 for model_name in llmp.LLMChatCompletionFactory.available_models:
     print(f"  {model_name}")
 print()
 
 factory = llmp.LLMChatCompletionFactory
-model = factory.build('ollama/phi3:latest')
+model = factory.build('ollama/phi3')
 user_msg = llmp.Message(content="Please give me a list of ten colours and some place that is related to each one.")
 sys_msg = llmp.Message(content="Provide an answer in json", role="system")
 resp = model.query([user_msg,sys_msg], json_response=True, temperature=0)
 
 resp.show_header()
 print(resp.message.content)
 ```
@@ -236,18 +220,23 @@
 
 ```
 chat completion models:
   groq/llama3-70b-8192
   groq/llama3-8b-8192
   groq/mixtral-8x7b-32768
   groq/gemma-7b-it
+  openai/gpt-4o
   openai/gpt-4-turbo
   openai/gpt-4-turbo-preview
   openai/gpt-3.5-turbo
+  anthropic/claude-3-opus-20240229
+  anthropic/claude-3-sonnet-20240229
+  anthropic/claude-3-haiku-20240307
   ollama/phi3:latest
+  ollama/phi3
 
 Response successful; tokens: i:40 o:189
 {
   "Colours": [
     {"Red": "The Eiffel Tower, Paris"},
     {"Blue": "Pacific Ocean near Hawaii"},
     {"Green": "Yellowstone National Park, USA"},
@@ -257,7 +246,46 @@
     {"Purple": "Royal Palace of Caserta, Italy"},
     {"Gray": "Snowy landscapes in the Swiss Alps"},
     {"Brown": "Amazon Rainforest, Brazil"},
     {"Yellow": "Kilimanjaro's snow-capped peak, Tanzania"}
   ]
 }
 ```
+</details>
+
+### Templates example
+
+Write templates.txt file:
+```
+# template: question_yesno_json_sys
+# role: system
+
+Answer the question with any of these responses: yes, no, unknown, ambiguous.
+Respond in json using this schema:
+{ "answer": "..." }
+
+# template: question_yesno_user
+# role: user
+
+{{question}}
+
+# template: extract_keywords_json_sys
+# role: system
+
+Extract keywords from the provided text.
+Respond in json using this schema:
+{ "keywords": ["keyword1", "keyword2", ...] }
+```
+
+Use it in code:
+
+```python
+import llmprototyping as llmp
+
+template_repo = llmp.TemplateFileRepository("templates.txt")
+msg_sys = template_repo.render_message('question_yesno_json_sys', {})
+msg_user = template_repo.render_message('question_yesno_user', {"question": "Is 1+1 = 2?"})
+
+# model is an LLMChatCompletion object, see examples above
+resp = model.query([msg_sys,msg_text], json_response=True)
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `llmprototyping-0.1.0.dev4/README.md` & `llmprototyping-0.1.0.dev5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: llmprototyping
+Version: 0.1.0.dev5
+Summary: A lightweight set of tools to use several llm and embeddings apis
+Home-page: https://github.com/alejandrolc/llmprototyping
+Author: Alejandro López Correa
+Keywords: llm,rag,openai,groq,ollama
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.9, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: groq
+Requires-Dist: openai
+Requires-Dist: tiktoken
+Requires-Dist: packaging
+Requires-Dist: faiss-cpu
+Requires-Dist: ollama
+Requires-Dist: anthropic
+
 # llmprototyping
 
 `llmprototyping` is a Python package designed to provide easy and uniform access to various large language model (LLM) and embedding APIs, along with basic functionality for building small-scale artificial intelligence applications.
 
 ## Features
 
 - **Uniform API Access**: Simplify your interactions with different LLM and embedding APIs using a single interface.
@@ -25,24 +47,29 @@
 
 ### chat completion models
 
 - groq/llama3-70b-8192
 - groq/llama3-8b-8192
 - groq/mixtral-8x7b-32768
 - groq/gemma-7b-it
+- openai/gpt-4o
 - openai/gpt-4-turbo
 - openai/gpt-4-turbo-preview
 - openai/gpt-3.5-turbo
+- anthropic/claude-3-opus-20240229
+- anthropic/claude-3-sonnet-20240229
+- anthropic/claude-3-haiku-20240307
 - ollama/*
 
 ### embedding models
 
 - openai/text-embedding-3-small
 - openai/text-embedding-3-large
 - openai/text-embedding-ada-002
+- ollama/*
 
 ## Usage
 
 Note: The examples use python-dotenv. This is not required by llmprototyping, so it needs to be installed separatedly. 
 
 ### Simple chat completion call
 
@@ -197,15 +224,15 @@
 
 print('chat completion models:')
 for model_name in llmp.LLMChatCompletionFactory.available_models:
     print(f"  {model_name}")
 print()
 
 factory = llmp.LLMChatCompletionFactory
-model = factory.build('ollama/phi3:latest')
+model = factory.build('ollama/phi3')
 user_msg = llmp.Message(content="Please give me a list of ten colours and some place that is related to each one.")
 sys_msg = llmp.Message(content="Provide an answer in json", role="system")
 resp = model.query([user_msg,sys_msg], json_response=True, temperature=0)
 
 resp.show_header()
 print(resp.message.content)
 ```
@@ -215,18 +242,23 @@
 
 ```
 chat completion models:
   groq/llama3-70b-8192
   groq/llama3-8b-8192
   groq/mixtral-8x7b-32768
   groq/gemma-7b-it
+  openai/gpt-4o
   openai/gpt-4-turbo
   openai/gpt-4-turbo-preview
   openai/gpt-3.5-turbo
+  anthropic/claude-3-opus-20240229
+  anthropic/claude-3-sonnet-20240229
+  anthropic/claude-3-haiku-20240307
   ollama/phi3:latest
+  ollama/phi3
 
 Response successful; tokens: i:40 o:189
 {
   "Colours": [
     {"Red": "The Eiffel Tower, Paris"},
     {"Blue": "Pacific Ocean near Hawaii"},
     {"Green": "Yellowstone National Park, USA"},
@@ -236,7 +268,46 @@
     {"Purple": "Royal Palace of Caserta, Italy"},
     {"Gray": "Snowy landscapes in the Swiss Alps"},
     {"Brown": "Amazon Rainforest, Brazil"},
     {"Yellow": "Kilimanjaro's snow-capped peak, Tanzania"}
   ]
 }
 ```
+</details>
+
+### Templates example
+
+Write templates.txt file:
+```
+# template: question_yesno_json_sys
+# role: system
+
+Answer the question with any of these responses: yes, no, unknown, ambiguous.
+Respond in json using this schema:
+{ "answer": "..." }
+
+# template: question_yesno_user
+# role: user
+
+{{question}}
+
+# template: extract_keywords_json_sys
+# role: system
+
+Extract keywords from the provided text.
+Respond in json using this schema:
+{ "keywords": ["keyword1", "keyword2", ...] }
+```
+
+Use it in code:
+
+```python
+import llmprototyping as llmp
+
+template_repo = llmp.TemplateFileRepository("templates.txt")
+msg_sys = template_repo.render_message('question_yesno_json_sys', {})
+msg_user = template_repo.render_message('question_yesno_user', {"question": "Is 1+1 = 2?"})
+
+# model is an LLMChatCompletion object, see examples above
+resp = model.query([msg_sys,msg_text], json_response=True)
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llmprototyping-0.1.0.dev4/setup.py` & `llmprototyping-0.1.0.dev5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="llmprototyping",
     # https://packaging.python.org/en/latest/discussions/versioning/
-    version="0.1.0.dev4",
+    version="0.1.0.dev5",
     description="A lightweight set of tools to use several llm and embeddings apis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alejandrolc/llmprototyping",
     author="Alejandro López Correa",
     #author_email="...",
     classifiers=[
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/__init__.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from .llm_interface import Message, Response, LLMChatCompletionFactory
+from .llm_interface import Message, Response, LLMChatCompletionFactory, LLMChatCompletionCache
 from .embeddings_interface import EmbeddingVector, EmbeddingComputerFactory
 from .vectordb import FAISSDatabase
-from .error import LLMException
+from .templates import Template, TemplateFileRepository
+from .error import LLMPException
 
 try:
     from .llm_groq import init as groq_llm_init
     groq_llm_init()
 except ImportError:
     pass
 
@@ -17,15 +18,20 @@
 
 try:
     from .embeddings_openai import init as openai_emb_init
     openai_emb_init()
 except ImportError:
     pass
 
-
 try:
     from .llm_em_ollama import init as ollama_llm_init
     from .llm_em_ollama import pull_model as ollama_pull_model
     ollama_llm_init()
     from .llm_em_ollama import discover as ollama_discover
 except ImportError:
+    pass
+
+try:
+    from .llm_anthropic import init as anthropic_llm_init
+    anthropic_llm_init()
+except ImportError:
     pass
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_interface.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/embeddings_interface.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_openai.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/embeddings_openai.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/error.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 
-class LLMException(Exception):
+class LLMPException(Exception):
     def __init__(self, error_type, info, retryable, extra_data=None):
         Exception.__init__(self)
 
         self.error_type = error_type
         self.info = info
         self.retryable = retryable
         self.extra_data = extra_data
 
     def __str__(self) -> str:
-        return f"LLMException {self.error_type} ({'retryable' if self.retryable else 'final'}) {self.info}"
+        return f"LLMPException {self.error_type} ({'retryable' if self.retryable else 'final'}) {self.info}"
 
     @staticmethod
     def not_available(info):
-        return LLMException("not available", info, True)
+        return LLMPException("not available", info, True)
     @staticmethod
     def unknown_backend(info):
-        return LLMException("unknown backend", info, False)
+        return LLMPException("unknown backend", info, False)
     @staticmethod
     def timeout(info):
-        return LLMException("timeout", info, True)   
+        return LLMPException("timeout", info, True)   
     @staticmethod
     def service_error(info, retryable):
-        return LLMException("service error", info, retryable == True)   
+        return LLMPException("service error", info, retryable == True)   
     @staticmethod
     def param_error(info):
-        return LLMException("error with parameter", info, False)
+        return LLMPException("error with parameter", info, False)
     @staticmethod
     def not_found(info):
-        return LLMException("not found", info, False)
+        return LLMPException("not found", info, False)
     @staticmethod
     def database_error(info):
-        return LLMException("docdb error", info, False)
+        return LLMPException("docdb error", info, False)
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/factory.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .error import LLMException
+from .error import LLMPException
 
 class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             instance = cls.__call__(*args, **kwargs)
@@ -36,17 +36,17 @@
     def register(cls, name, class_obj, alias = None):
         if issubclass(class_obj, cls._class):
             registry = cls.__get_registry()
             registry[name] = class_obj
             if alias is not None:
                 registry[alias] = class_obj
         else:
-            raise LLMException.param_error(f"error registering {class_obj}: type mismatch; expected {cls._class}")
+            raise LLMPException.param_error(f"error registering {class_obj}: type mismatch; expected {cls._class}")
 
     @classmethod
     def build(cls, name, data={}):
         registry = cls.__get_registry()
         obj_cls = registry.get(name)
         if obj_cls:
             return obj_cls.from_dict(data)
         else:
-            raise LLMException.not_found(f"No model registered with name '{name}'")
+            raise LLMPException.not_found(f"No model registered with name '{name}'")
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/llm_em_ollama.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/llm_em_ollama.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 import inspect
 import ollama
 from .llm_interface import LLMChatCompletion, LLMChatCompletionFactory, Message, Response
 from .embeddings_interface import EmbeddingComputer, EmbeddingComputerFactory, EmbeddingVector
-from .error import LLMException
+from .error import LLMPException
 
 class OLlamaEmbeddingComputer(EmbeddingComputer):
     @property
     def model_name(self):
         return self._model_name
 
     @property
@@ -38,23 +38,23 @@
         return f"ollama/{model_name}"
 
     def get_embedding(self, text):
         text = text.replace("\n", " ").strip()
         try:
             resp = self._client.embeddings(prompt=text, model=self._ollama_model_name)
         except ollama.ResponseError as e:
-            raise LLMException(e.status_code, e.error, True)
+            raise LLMPException(e.status_code, e.error, True)
         except Exception as e:
-            raise LLMException("exception", e, False)
+            raise LLMPException("exception", e, False)
 
         if 'embedding' not in resp:
-            raise LLMException("unexpected response", resp, False)
+            raise LLMPException("unexpected response", resp, False)
         v = resp.get('embedding',[])
         if len(v) != self.vector_size:
-            raise LLMException("vector size mismatch", f"vector size mismatch; expected:{self.vector_size} got:{len(v)}", False)
+            raise LLMPException("vector size mismatch", f"vector size mismatch; expected:{self.vector_size} got:{len(v)}", False)
         return EmbeddingVector(v, self.get_computer_name(self.model_name))
 
     def __init__(self, host, model_name, vector_size, comparison_method, ollama_model_name):
         self._model_name = model_name
         self._client = ollama.Client(host=host)
         self._vector_size = vector_size
         self._comparison_method = comparison_method
@@ -69,15 +69,15 @@
 
     @property
     def context_size(self):
         raise NotImplemented()
 
     def query(self, messages:List[Message], json_response=False, temperature=1.0):
         if not isinstance(temperature,float) and not isinstance(temperature,int):
-            raise LLMException.param_error("temperature must be a float")
+            raise LLMPException.param_error("temperature must be a float")
 
         try:
             rformat = 'json' if json_response else ''
             r = self._client.chat(
                 messages = [m.to_dict() for m in messages],
                 model = self._ollama_model_name,
                 options = {'temperature': temperature},
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/llm_groq.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/llm_groq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import List
 import inspect
 import groq
 from .llm_interface import LLMChatCompletion, LLMChatCompletionFactory, Message, Response
-from .error import LLMException
+from .error import LLMPException
 
 class LLMGroqChatCompletion(LLMChatCompletion):
     def __init__(self, api_key, model_name, context_size):
         self.model_name = model_name
         self._client = groq.Groq(api_key=api_key)
         self._context_size = context_size
 
     @property
     def context_size(self):
         return self._context_size
 
     def query(self, messages:List[Message], json_response=False, temperature=1.0):
         if not isinstance(temperature,float) and not isinstance(temperature,int):
-            raise LLMException.param_error("temperature must be a float in range [0.0,2.0]")
+            raise LLMPException.param_error("temperature must be a float in range [0.0,2.0]")
         if temperature < 0 or temperature > 2:
-            raise LLMException.param_error("temperature must be a float in range [0.0,2.0]")
+            raise LLMPException.param_error("temperature must be a float in range [0.0,2.0]")
 
         try:
             rformat = {"type": "json_object"} if json_response else None
             r = self._client.chat.completions.create(
                 messages = [m.to_dict() for m in messages],
                 model = self.model_name,
                 response_format = rformat,
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/llm_openai.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/llm_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import List
 import inspect
 import openai
 from .llm_interface import LLMChatCompletion, LLMChatCompletionFactory, Message, Response
-from .error import LLMException
+from .error import LLMPException
 
 class LLMOpenAIChatCompletion(LLMChatCompletion):
     def __init__(self, api_key, model_name, context_size):
         self.model_name = model_name
         self._client = openai.OpenAI(api_key=api_key)
         self._context_size = context_size
 
     @property
     def context_size(self):
         return self._context_size
 
     def query(self, messages:List[Message], json_response=False, temperature=1.0):
         if not isinstance(temperature,float) and not isinstance(temperature,int):
-            raise LLMException.param_error("temperature must be a float in range [0.0,2.0]")
+            raise LLMPException.param_error("temperature must be a float in range [0.0,2.0]")
         if temperature < 0 or temperature > 2:
-            raise LLMException.param_error("temperature must be a float in range [0.0,2.0]")
+            raise LLMPException.param_error("temperature must be a float in range [0.0,2.0]")
 
         try:
             rformat = {"type": "json_object"} if json_response else None
             r = self._client.chat.completions.create(
                 messages = [m.to_dict() for m in messages],
                 model = self.model_name,
                 response_format = rformat,
@@ -41,28 +41,32 @@
         except openai.BadRequestError as e:
             response = Response.error_response(status_code = e.status_code, error = f"{e.body}")
         except openai.AuthenticationError as e:
             response = Response.error_response(status_code = e.status_code, error = f"{e.body}")
         except openai.PermissionDeniedError as e:
             response = Response.error_response(status_code = e.status_code, error = f"{e.body}")
         except openai.RateLimitError as e:
-            response = Response(status_code = e.status_code, error = f"{e.body}")
+            response = Response.error_response(status_code = e.status_code, error = f"{e.body}")
         except openai.APIError as e:
             response = Response.error_response(status_code = e.status_code, error = f"{e.body}")
         except Exception as e:
             print(type(e))
             print(dir(e))
             response = Response.error_response(status_code = "exception", error = e)
 
         return response
 
     @classmethod
     def from_dict(cls, data):
         return cls(model_name=cls.cls_model_name, context_size=cls.cls_context_size, api_key=data['api_key'])
 
+class OpenAI_GPT_4o(LLMOpenAIChatCompletion):
+    cls_model_name = 'gpt-4o'
+    cls_context_size = 128000
+
 class OpenAI_GPT_4_turbo(LLMOpenAIChatCompletion):
     cls_model_name = 'gpt-4-turbo'
     cls_context_size = 128000
 
 class OpenAI_GPT_4_turbo_preview(LLMOpenAIChatCompletion):
     cls_model_name = 'gpt-4-turbo-preview'
     cls_context_size = 128000
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping/vectordb.py` & `llmprototyping-0.1.0.dev5/src/llmprototyping/vectordb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import faiss
 import numpy as np
 from typing import List, Dict
-from .error import LLMException
+from .error import LLMPException
 from .embeddings_interface import EmbeddingVector
 
 class FAISSDatabase:
     def __init__(self, embedding_type, embedding_size):
         self.embedding_type = embedding_type
         self.embedding_size = embedding_size
         self.index1 = faiss.IndexFlatL2(embedding_size)
         self.index = faiss.IndexIDMap(self.index1)
 
     def _handle_embedding(self, embedding:EmbeddingVector):
         ae = embedding.vector.reshape(1, -1)
         if ae.shape[1] != self.embedding_size:
-            raise LLMException.param_error(f"embedding size mismatch: {ae.shape[1]} dimensions vs {self.embedding_size} expected")
+            raise LLMPException.param_error(f"embedding size mismatch: {ae.shape[1]} dimensions vs {self.embedding_size} expected")
         n = np.linalg.norm(ae[0])
         if n != 0:
             ae[0] = ae[0] / n
         return ae
 
     @property
     def count(self):
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/PKG-INFO` & `llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmprototyping
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: A lightweight set of tools to use several llm and embeddings apis
 Home-page: https://github.com/alejandrolc/llmprototyping
 Author: Alejandro López Correa
 Keywords: llm,rag,openai,groq,ollama
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,14 +14,15 @@
 License-File: LICENSE
 Requires-Dist: groq
 Requires-Dist: openai
 Requires-Dist: tiktoken
 Requires-Dist: packaging
 Requires-Dist: faiss-cpu
 Requires-Dist: ollama
+Requires-Dist: anthropic
 
 # llmprototyping
 
 `llmprototyping` is a Python package designed to provide easy and uniform access to various large language model (LLM) and embedding APIs, along with basic functionality for building small-scale artificial intelligence applications.
 
 ## Features
 
@@ -46,24 +47,29 @@
 
 ### chat completion models
 
 - groq/llama3-70b-8192
 - groq/llama3-8b-8192
 - groq/mixtral-8x7b-32768
 - groq/gemma-7b-it
+- openai/gpt-4o
 - openai/gpt-4-turbo
 - openai/gpt-4-turbo-preview
 - openai/gpt-3.5-turbo
+- anthropic/claude-3-opus-20240229
+- anthropic/claude-3-sonnet-20240229
+- anthropic/claude-3-haiku-20240307
 - ollama/*
 
 ### embedding models
 
 - openai/text-embedding-3-small
 - openai/text-embedding-3-large
 - openai/text-embedding-ada-002
+- ollama/*
 
 ## Usage
 
 Note: The examples use python-dotenv. This is not required by llmprototyping, so it needs to be installed separatedly. 
 
 ### Simple chat completion call
 
@@ -218,15 +224,15 @@
 
 print('chat completion models:')
 for model_name in llmp.LLMChatCompletionFactory.available_models:
     print(f"  {model_name}")
 print()
 
 factory = llmp.LLMChatCompletionFactory
-model = factory.build('ollama/phi3:latest')
+model = factory.build('ollama/phi3')
 user_msg = llmp.Message(content="Please give me a list of ten colours and some place that is related to each one.")
 sys_msg = llmp.Message(content="Provide an answer in json", role="system")
 resp = model.query([user_msg,sys_msg], json_response=True, temperature=0)
 
 resp.show_header()
 print(resp.message.content)
 ```
@@ -236,18 +242,23 @@
 
 ```
 chat completion models:
   groq/llama3-70b-8192
   groq/llama3-8b-8192
   groq/mixtral-8x7b-32768
   groq/gemma-7b-it
+  openai/gpt-4o
   openai/gpt-4-turbo
   openai/gpt-4-turbo-preview
   openai/gpt-3.5-turbo
+  anthropic/claude-3-opus-20240229
+  anthropic/claude-3-sonnet-20240229
+  anthropic/claude-3-haiku-20240307
   ollama/phi3:latest
+  ollama/phi3
 
 Response successful; tokens: i:40 o:189
 {
   "Colours": [
     {"Red": "The Eiffel Tower, Paris"},
     {"Blue": "Pacific Ocean near Hawaii"},
     {"Green": "Yellowstone National Park, USA"},
@@ -257,7 +268,46 @@
     {"Purple": "Royal Palace of Caserta, Italy"},
     {"Gray": "Snowy landscapes in the Swiss Alps"},
     {"Brown": "Amazon Rainforest, Brazil"},
     {"Yellow": "Kilimanjaro's snow-capped peak, Tanzania"}
   ]
 }
 ```
+</details>
+
+### Templates example
+
+Write templates.txt file:
+```
+# template: question_yesno_json_sys
+# role: system
+
+Answer the question with any of these responses: yes, no, unknown, ambiguous.
+Respond in json using this schema:
+{ "answer": "..." }
+
+# template: question_yesno_user
+# role: user
+
+{{question}}
+
+# template: extract_keywords_json_sys
+# role: system
+
+Extract keywords from the provided text.
+Respond in json using this schema:
+{ "keywords": ["keyword1", "keyword2", ...] }
+```
+
+Use it in code:
+
+```python
+import llmprototyping as llmp
+
+template_repo = llmp.TemplateFileRepository("templates.txt")
+msg_sys = template_repo.render_message('question_yesno_json_sys', {})
+msg_user = template_repo.render_message('question_yesno_user', {"question": "Is 1+1 = 2?"})
+
+# model is an LLMChatCompletion object, see examples above
+resp = model.query([msg_sys,msg_text], json_response=True)
+```
+
```

### Comparing `llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/SOURCES.txt` & `llmprototyping-0.1.0.dev5/src/llmprototyping.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/llmprototyping/__init__.py
+src/llmprototyping/cache.py
 src/llmprototyping/embeddings_interface.py
 src/llmprototyping/embeddings_ollama.py
 src/llmprototyping/embeddings_openai.py
 src/llmprototyping/error.py
 src/llmprototyping/factory.py
+src/llmprototyping/llm_anthropic.py
 src/llmprototyping/llm_em_ollama.py
 src/llmprototyping/llm_groq.py
 src/llmprototyping/llm_interface.py
 src/llmprototyping/llm_openai.py
 src/llmprototyping/serializable.py
+src/llmprototyping/templates.py
 src/llmprototyping/vectordb.py
 src/llmprototyping.egg-info/PKG-INFO
 src/llmprototyping.egg-info/SOURCES.txt
 src/llmprototyping.egg-info/dependency_links.txt
 src/llmprototyping.egg-info/requires.txt
 src/llmprototyping.egg-info/top_level.txt
```

