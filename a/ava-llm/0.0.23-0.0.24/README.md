# Comparing `tmp/ava_llm-0.0.23.tar.gz` & `tmp/ava_llm-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ava_llm-0.0.23.tar", last modified: Mon May 13 21:44:51 2024, max compression
+gzip compressed data, was "ava_llm-0.0.24.tar", last modified: Tue May 14 07:48:06 2024, max compression
```

## Comparing `ava_llm-0.0.23.tar` & `ava_llm-0.0.24.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.23/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-13 21:44:51.869802 ava_llm-0.0.23/PKG-INFO
--rwxr-xr-x   0 mihai     (1000) mihai     (1000)      173 2024-05-13 19:06:40.000000 ava_llm-0.0.23/README.md
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.866802 ava_llm-0.0.23/ava_llm/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.23/ava_llm/__init__.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.867802 ava_llm-0.0.23/ava_llm/conversations/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.23/ava_llm/conversations/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.23/ava_llm/conversations/buffer.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.23/ava_llm/conversations/chat_history.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.23/ava_llm/conversations/chat_memory.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.23/ava_llm/conversations/memory.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.868802 ava_llm-0.0.23/ava_llm/conversations/messages/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.23/ava_llm/conversations/messages/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.23/ava_llm/conversations/messages/ai.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      390 2024-05-13 14:34:08.000000 ava_llm-0.0.23/ava_llm/conversations/messages/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.23/ava_llm/conversations/messages/human.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.868802 ava_llm-0.0.23/ava_llm/handlers/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.23/ava_llm/handlers/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     2641 2024-05-11 18:07:45.000000 ava_llm-0.0.23/ava_llm/handlers/meta.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3025 2024-05-11 18:02:03.000000 ava_llm-0.0.23/ava_llm/handlers/openai.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.868802 ava_llm-0.0.23/ava_llm/language_models/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.23/ava_llm/language_models/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3782 2024-05-13 21:42:21.000000 ava_llm-0.0.23/ava_llm/language_models/llm.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/ava_llm/prompts/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.23/ava_llm/prompts/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.23/ava_llm/prompts/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.23/ava_llm/prompts/template.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/ava_llm/utils/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.23/ava_llm/utils/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.23/ava_llm/utils/utils.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/ava_llm.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       26 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/requires.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/top_level.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-13 21:44:51.869802 ava_llm-0.0.23/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)      476 2024-05-13 21:43:53.000000 ava_llm-0.0.23/setup.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.400752 ava_llm-0.0.24/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.24/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 07:48:06.400752 ava_llm-0.0.24/PKG-INFO
+-rwxr-xr-x   0 mihai     (1000) mihai     (1000)      173 2024-05-13 19:06:40.000000 ava_llm-0.0.24/README.md
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.397752 ava_llm-0.0.24/ava_llm/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.24/ava_llm/__init__.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.398752 ava_llm-0.0.24/ava_llm/conversations/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.24/ava_llm/conversations/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.24/ava_llm/conversations/buffer.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.24/ava_llm/conversations/chat_history.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.24/ava_llm/conversations/chat_memory.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.24/ava_llm/conversations/memory.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.398752 ava_llm-0.0.24/ava_llm/conversations/messages/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.24/ava_llm/conversations/messages/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.24/ava_llm/conversations/messages/ai.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      390 2024-05-13 14:34:08.000000 ava_llm-0.0.24/ava_llm/conversations/messages/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.24/ava_llm/conversations/messages/human.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/handlers/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.24/ava_llm/handlers/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3292 2024-05-14 07:45:24.000000 ava_llm-0.0.24/ava_llm/handlers/meta.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3345 2024-05-14 07:13:22.000000 ava_llm-0.0.24/ava_llm/handlers/openai.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/language_models/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.24/ava_llm/language_models/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     4374 2024-05-14 07:46:24.000000 ava_llm-0.0.24/ava_llm/language_models/llm.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/prompts/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.24/ava_llm/prompts/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.24/ava_llm/prompts/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.24/ava_llm/prompts/template.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/utils/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.24/ava_llm/utils/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.24/ava_llm/utils/utils.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.400752 ava_llm-0.0.24/ava_llm.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       26 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/requires.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/top_level.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-14 07:48:06.400752 ava_llm-0.0.24/setup.cfg
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      476 2024-05-14 07:32:35.000000 ava_llm-0.0.24/setup.py
```

### Comparing `ava_llm-0.0.23/LICENSE` & `ava_llm-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.23/ava_llm/conversations/buffer.py` & `ava_llm-0.0.24/ava_llm/conversations/buffer.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.23/ava_llm/conversations/chat_history.py` & `ava_llm-0.0.24/ava_llm/conversations/chat_history.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.23/ava_llm/conversations/chat_memory.py` & `ava_llm-0.0.24/ava_llm/conversations/chat_memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.23/ava_llm/conversations/memory.py` & `ava_llm-0.0.24/ava_llm/conversations/memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.23/ava_llm/handlers/meta.py` & `ava_llm-0.0.24/ava_llm/handlers/meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-from groq import Groq
+from groq import Groq, AsyncGroq
 from dotenv import load_dotenv
 import os
 
 load_dotenv()
 
 meta_key = os.getenv("META_KEY")
 
 client = Groq(api_key=meta_key)
+aclient = AsyncGroq(api_key=meta_key)
 
 
 class Meta:
     def __init__(self, model, temperature=None):
         self.model = model or "llama3-8b-8192"
         self.temperature = temperature
 
     def invoke(self, prompt, temperature=None, force_json=False, **kwargs):
         temperature = temperature if temperature is not None else self.temperature
         response = self._generate(prompt, temperature, force_json=force_json, **kwargs)
         response_dict = self._response_to_dict(response)
         return response_dict
 
     async def ainvoke(self, prompt, temperature=None, **kwargs):
-        raise NotImplementedError(
-            "Asynchronous invocation is not supported for the llama model"
-        )
+        temperature = temperature if temperature is not None else self.temperature
+        response = await self._agenerate(prompt, temperature, **kwargs)
+        response_dict = self._response_to_dict(response)
+        return response_dict
 
     def stream(self, prompt, temperature=None, **kwargs):
         temperature = temperature if temperature is not None else self.temperature
         response = self._generate(prompt, temperature, stream=True, **kwargs)
         for chunk in response:
             yield chunk.choices[0].delta.content
 
+    async def astream(self, prompt, temperature=None, **kwargs):
+        temperature = temperature if temperature is not None else self.temperature
+        response = await self._agenerate(prompt, temperature, stream=True, **kwargs)
+        async for chunk in response:
+            yield chunk.choices[0].delta.content
+
     def _response_to_dict(self, response):
         # metadata dict
         metadata_dict = {}
         metadata_dict["input_tokens"] = response.usage.prompt_tokens
         metadata_dict["output_tokens"] = response.usage.completion_tokens
         metadata_dict["total_tokens"] = response.usage.total_tokens
 
@@ -61,17 +69,23 @@
             temperature=temperature,
             stream=stream,
             **kwargs
         )
         return response
 
     async def _agenerate(self, prompt, temperature=1.0, stream=False, **kwargs):
-        raise NotImplementedError(
-            "Asynchronous generation is not supported for the llama model"
+        prompt = self._format_prompt(prompt)
+        response = await aclient.chat.completions.create(
+            model=self.model,
+            messages=prompt,
+            temperature=temperature,
+            stream=stream,
+            **kwargs
         )
+        return response
 
     def _format_prompt(self, prompt):
         if isinstance(prompt, str):
             return [{"role": "user", "content": prompt}]
         elif isinstance(prompt, list):
             return prompt
         else:
```

### Comparing `ava_llm-0.0.23/ava_llm/handlers/openai.py` & `ava_llm-0.0.24/ava_llm/handlers/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 
     def stream(self, prompt, temperature=None, **kwargs):
         temperature = temperature if temperature is not None else self.temperature
         response = self._generate(prompt, temperature, stream=True, **kwargs)
         for chunk in response:
             yield chunk.choices[0].delta.content
 
+    async def astream(self, prompt, temperature=None, **kwargs):
+        temperature = temperature if temperature is not None else self.temperature
+        response = await self._agenerate(prompt, temperature, stream=True, **kwargs)
+        async for chunk in response:
+            yield chunk.choices[0].delta.content
+
     def _response_to_dict(self, response):
         # metadata dict
         metadata_dict = {}
         metadata_dict["input_tokens"] = response.usage.prompt_tokens
         metadata_dict["output_tokens"] = response.usage.completion_tokens
         metadata_dict["total_tokens"] = response.usage.total_tokens
```

### Comparing `ava_llm-0.0.23/ava_llm/language_models/llm.py` & `ava_llm-0.0.24/ava_llm/language_models/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,24 @@
                 if hasattr(chunk, "content"):
                     yield chunk
                 elif isinstance(chunk, str):
                     yield chunk
                 else:
                     raise TypeError("Unexpected response type")
 
+    async def astream(self, prompt, **kwargs):
+        async for chunk in self.handler.astream(prompt, **kwargs):
+            if chunk:
+                if hasattr(chunk, "content"):
+                    yield chunk
+                elif isinstance(chunk, str):
+                    yield chunk
+                else:
+                    raise TypeError("Unexpected response type")
+
     def _format_response(self, response):
 
         # langchain response
         if hasattr(response, "content") and hasattr(response, "response_metadata"):
             return LLMResponse(response.content, response.response_metadata)
 
         # this library response
@@ -108,7 +118,14 @@
             if verbose:
                 print(chunk, end="", flush=True)
 
         outputs = {"response": "".join(chunks)}
         self.memory.save_context(inputs, outputs)
 
         return clean_response
+
+    async def astream(self, message: str, verbose=True) -> Any:
+        prompt = self.prompt.format(history=self.memory.buffer, input=message)
+
+        response = self.llm.astream(prompt)
+
+        return response
```

### Comparing `ava_llm-0.0.23/ava_llm/prompts/base.py` & `ava_llm-0.0.24/ava_llm/prompts/base.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.23/ava_llm/utils/utils.py` & `ava_llm-0.0.24/ava_llm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.23/ava_llm.egg-info/SOURCES.txt` & `ava_llm-0.0.24/ava_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

