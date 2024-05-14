# Comparing `tmp/ava_llm-0.0.24.tar.gz` & `tmp/ava_llm-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ava_llm-0.0.24.tar", last modified: Tue May 14 07:48:06 2024, max compression
+gzip compressed data, was "ava_llm-0.0.25.tar", last modified: Tue May 14 08:42:18 2024, max compression
```

## Comparing `ava_llm-0.0.24.tar` & `ava_llm-0.0.25.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.400752 ava_llm-0.0.24/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.24/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 07:48:06.400752 ava_llm-0.0.24/PKG-INFO
--rwxr-xr-x   0 mihai     (1000) mihai     (1000)      173 2024-05-13 19:06:40.000000 ava_llm-0.0.24/README.md
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.397752 ava_llm-0.0.24/ava_llm/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.24/ava_llm/__init__.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.398752 ava_llm-0.0.24/ava_llm/conversations/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.24/ava_llm/conversations/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.24/ava_llm/conversations/buffer.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.24/ava_llm/conversations/chat_history.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.24/ava_llm/conversations/chat_memory.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.24/ava_llm/conversations/memory.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.398752 ava_llm-0.0.24/ava_llm/conversations/messages/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.24/ava_llm/conversations/messages/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.24/ava_llm/conversations/messages/ai.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      390 2024-05-13 14:34:08.000000 ava_llm-0.0.24/ava_llm/conversations/messages/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.24/ava_llm/conversations/messages/human.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/handlers/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.24/ava_llm/handlers/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3292 2024-05-14 07:45:24.000000 ava_llm-0.0.24/ava_llm/handlers/meta.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3345 2024-05-14 07:13:22.000000 ava_llm-0.0.24/ava_llm/handlers/openai.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/language_models/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.24/ava_llm/language_models/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     4374 2024-05-14 07:46:24.000000 ava_llm-0.0.24/ava_llm/language_models/llm.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/prompts/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.24/ava_llm/prompts/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.24/ava_llm/prompts/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.24/ava_llm/prompts/template.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.399752 ava_llm-0.0.24/ava_llm/utils/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.24/ava_llm/utils/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.24/ava_llm/utils/utils.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 07:48:06.400752 ava_llm-0.0.24/ava_llm.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       26 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/requires.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-14 07:48:06.000000 ava_llm-0.0.24/ava_llm.egg-info/top_level.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-14 07:48:06.400752 ava_llm-0.0.24/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)      476 2024-05-14 07:32:35.000000 ava_llm-0.0.24/setup.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.255678 ava_llm-0.0.25/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.25/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 08:42:18.254678 ava_llm-0.0.25/PKG-INFO
+-rwxr-xr-x   0 mihai     (1000) mihai     (1000)      173 2024-05-13 19:06:40.000000 ava_llm-0.0.25/README.md
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.252678 ava_llm-0.0.25/ava_llm/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.25/ava_llm/__init__.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.253678 ava_llm-0.0.25/ava_llm/conversations/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.25/ava_llm/conversations/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.25/ava_llm/conversations/buffer.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.25/ava_llm/conversations/chat_history.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.25/ava_llm/conversations/chat_memory.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.25/ava_llm/conversations/memory.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.253678 ava_llm-0.0.25/ava_llm/conversations/messages/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.25/ava_llm/conversations/messages/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.25/ava_llm/conversations/messages/ai.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      390 2024-05-13 14:34:08.000000 ava_llm-0.0.25/ava_llm/conversations/messages/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.25/ava_llm/conversations/messages/human.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.253678 ava_llm-0.0.25/ava_llm/handlers/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.25/ava_llm/handlers/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3292 2024-05-14 07:45:24.000000 ava_llm-0.0.25/ava_llm/handlers/meta.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3345 2024-05-14 07:13:22.000000 ava_llm-0.0.25/ava_llm/handlers/openai.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.254678 ava_llm-0.0.25/ava_llm/language_models/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.25/ava_llm/language_models/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     4767 2024-05-14 08:40:02.000000 ava_llm-0.0.25/ava_llm/language_models/llm.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.254678 ava_llm-0.0.25/ava_llm/prompts/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.25/ava_llm/prompts/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.25/ava_llm/prompts/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.25/ava_llm/prompts/template.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.254678 ava_llm-0.0.25/ava_llm/utils/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.25/ava_llm/utils/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.25/ava_llm/utils/utils.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:42:18.254678 ava_llm-0.0.25/ava_llm.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 08:42:18.000000 ava_llm-0.0.25/ava_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-14 08:42:18.000000 ava_llm-0.0.25/ava_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-14 08:42:18.000000 ava_llm-0.0.25/ava_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       26 2024-05-14 08:42:18.000000 ava_llm-0.0.25/ava_llm.egg-info/requires.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-14 08:42:18.000000 ava_llm-0.0.25/ava_llm.egg-info/top_level.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-14 08:42:18.255678 ava_llm-0.0.25/setup.cfg
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      476 2024-05-14 08:00:41.000000 ava_llm-0.0.25/setup.py
```

### Comparing `ava_llm-0.0.24/LICENSE` & `ava_llm-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/conversations/buffer.py` & `ava_llm-0.0.25/ava_llm/conversations/buffer.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/conversations/chat_history.py` & `ava_llm-0.0.25/ava_llm/conversations/chat_history.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/conversations/chat_memory.py` & `ava_llm-0.0.25/ava_llm/conversations/chat_memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/conversations/memory.py` & `ava_llm-0.0.25/ava_llm/conversations/memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/handlers/meta.py` & `ava_llm-0.0.25/ava_llm/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/handlers/openai.py` & `ava_llm-0.0.25/ava_llm/handlers/openai.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/language_models/llm.py` & `ava_llm-0.0.25/ava_llm/language_models/llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Any
 from ava_llm.conversations.chat_history import (
     BaseChatMessageHistory,
     InMemoryChatMessageHistory,
 )
 from ava_llm.prompts.base import PromptTemplate
 from ava_llm.prompts.template import ConversationTemplate
@@ -119,13 +120,24 @@
                 print(chunk, end="", flush=True)
 
         outputs = {"response": "".join(chunks)}
         self.memory.save_context(inputs, outputs)
 
         return clean_response
 
-    async def astream(self, message: str, verbose=True) -> Any:
+    async def astream(self, message: str, verbose=True, ws_consumer=None) -> None:
+        inputs = {"prompt": message}
+
         prompt = self.prompt.format(history=self.memory.buffer, input=message)
 
-        response = self.llm.astream(prompt)
+        chunks = []
+
+        async for chunk in self.llm.astream(prompt):
+            chunks.append(chunk)
+            if ws_consumer is not None:
+                ws_consumer.send(self.send(text_data=json.dumps(chunk)))
+            if verbose:
+                print(chunk, end="", flush=True)
+
+        outputs = {"response": "".join(chunks)}
+        self.memory.save_context(inputs, outputs)
 
-        return response
```

### Comparing `ava_llm-0.0.24/ava_llm/prompts/base.py` & `ava_llm-0.0.25/ava_llm/prompts/base.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm/utils/utils.py` & `ava_llm-0.0.25/ava_llm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.24/ava_llm.egg-info/SOURCES.txt` & `ava_llm-0.0.25/ava_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

