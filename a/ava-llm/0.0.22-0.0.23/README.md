# Comparing `tmp/ava_llm-0.0.22.tar.gz` & `tmp/ava_llm-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ava_llm-0.0.22.tar", last modified: Mon May 13 18:51:38 2024, max compression
+gzip compressed data, was "ava_llm-0.0.23.tar", last modified: Mon May 13 21:44:51 2024, max compression
```

## Comparing `ava_llm-0.0.22.tar` & `ava_llm-0.0.23.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.033908 ava_llm-0.0.22/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.22/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)      310 2024-05-13 18:51:38.033908 ava_llm-0.0.22/PKG-INFO
--rwxr-xr-x   0 mihai     (1000) mihai     (1000)       38 2024-05-13 18:36:13.000000 ava_llm-0.0.22/README.md
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.030907 ava_llm-0.0.22/ava_llm/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.22/ava_llm/__init__.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.031908 ava_llm-0.0.22/ava_llm/conversations/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.22/ava_llm/conversations/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.22/ava_llm/conversations/buffer.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.22/ava_llm/conversations/chat_history.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.22/ava_llm/conversations/chat_memory.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.22/ava_llm/conversations/memory.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.031908 ava_llm-0.0.22/ava_llm/conversations/messages/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.22/ava_llm/conversations/messages/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.22/ava_llm/conversations/messages/ai.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      390 2024-05-13 14:34:08.000000 ava_llm-0.0.22/ava_llm/conversations/messages/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.22/ava_llm/conversations/messages/human.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.032908 ava_llm-0.0.22/ava_llm/handlers/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.22/ava_llm/handlers/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     2641 2024-05-11 18:07:45.000000 ava_llm-0.0.22/ava_llm/handlers/meta.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3025 2024-05-11 18:02:03.000000 ava_llm-0.0.22/ava_llm/handlers/openai.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.032908 ava_llm-0.0.22/ava_llm/language_models/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.22/ava_llm/language_models/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3728 2024-05-13 18:37:29.000000 ava_llm-0.0.22/ava_llm/language_models/llm.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.032908 ava_llm-0.0.22/ava_llm/prompts/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.22/ava_llm/prompts/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.22/ava_llm/prompts/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.22/ava_llm/prompts/template.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.032908 ava_llm-0.0.22/ava_llm/utils/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.22/ava_llm/utils/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.22/ava_llm/utils/utils.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:51:38.033908 ava_llm-0.0.22/ava_llm.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      310 2024-05-13 18:51:37.000000 ava_llm-0.0.22/ava_llm.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-13 18:51:37.000000 ava_llm-0.0.22/ava_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-13 18:51:37.000000 ava_llm-0.0.22/ava_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       12 2024-05-13 18:51:37.000000 ava_llm-0.0.22/ava_llm.egg-info/requires.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-13 18:51:37.000000 ava_llm-0.0.22/ava_llm.egg-info/top_level.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-13 18:51:38.033908 ava_llm-0.0.22/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)      459 2024-05-13 18:49:25.000000 ava_llm-0.0.22/setup.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.23/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-13 21:44:51.869802 ava_llm-0.0.23/PKG-INFO
+-rwxr-xr-x   0 mihai     (1000) mihai     (1000)      173 2024-05-13 19:06:40.000000 ava_llm-0.0.23/README.md
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.866802 ava_llm-0.0.23/ava_llm/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.23/ava_llm/__init__.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.867802 ava_llm-0.0.23/ava_llm/conversations/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.23/ava_llm/conversations/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.23/ava_llm/conversations/buffer.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.23/ava_llm/conversations/chat_history.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.23/ava_llm/conversations/chat_memory.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.23/ava_llm/conversations/memory.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.868802 ava_llm-0.0.23/ava_llm/conversations/messages/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.23/ava_llm/conversations/messages/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.23/ava_llm/conversations/messages/ai.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      390 2024-05-13 14:34:08.000000 ava_llm-0.0.23/ava_llm/conversations/messages/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.23/ava_llm/conversations/messages/human.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.868802 ava_llm-0.0.23/ava_llm/handlers/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.23/ava_llm/handlers/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     2641 2024-05-11 18:07:45.000000 ava_llm-0.0.23/ava_llm/handlers/meta.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3025 2024-05-11 18:02:03.000000 ava_llm-0.0.23/ava_llm/handlers/openai.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.868802 ava_llm-0.0.23/ava_llm/language_models/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.23/ava_llm/language_models/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3782 2024-05-13 21:42:21.000000 ava_llm-0.0.23/ava_llm/language_models/llm.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/ava_llm/prompts/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.23/ava_llm/prompts/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.23/ava_llm/prompts/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.23/ava_llm/prompts/template.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/ava_llm/utils/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.23/ava_llm/utils/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.23/ava_llm/utils/utils.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 21:44:51.869802 ava_llm-0.0.23/ava_llm.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       26 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/requires.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-13 21:44:51.000000 ava_llm-0.0.23/ava_llm.egg-info/top_level.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-13 21:44:51.869802 ava_llm-0.0.23/setup.cfg
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      476 2024-05-13 21:43:53.000000 ava_llm-0.0.23/setup.py
```

### Comparing `ava_llm-0.0.22/LICENSE` & `ava_llm-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/conversations/buffer.py` & `ava_llm-0.0.23/ava_llm/conversations/buffer.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/conversations/chat_history.py` & `ava_llm-0.0.23/ava_llm/conversations/chat_history.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/conversations/chat_memory.py` & `ava_llm-0.0.23/ava_llm/conversations/chat_memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/conversations/memory.py` & `ava_llm-0.0.23/ava_llm/conversations/memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/handlers/meta.py` & `ava_llm-0.0.23/ava_llm/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/handlers/openai.py` & `ava_llm-0.0.23/ava_llm/handlers/openai.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/language_models/llm.py` & `ava_llm-0.0.23/ava_llm/language_models/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ava_llm.conversations.chat_history import (
     BaseChatMessageHistory,
     InMemoryChatMessageHistory,
 )
 from ava_llm.prompts.base import PromptTemplate
 from ava_llm.prompts.template import ConversationTemplate
 import uuid
+from itertools import tee
 
 
 class LLM:
     def __init__(self, model=None, handler=None, temperature=None) -> None:
         self.model = model or "gpt-3.5-turbo"
         self.handler = handler or self._get_handler()
         self.temperature = temperature if not None else self.handler.temperature
@@ -96,17 +97,18 @@
 
     def stream(self, message: str, verbose=True) -> Any:
         inputs = {"prompt": message}
 
         prompt = self.prompt.format(history=self.memory.buffer, input=message)
 
         chunks = []
-        response = self.llm.stream(prompt)
+        response, clean_response = tee(self.llm.stream(prompt))
+
         for chunk in response:
             chunks.append(chunk)
             if verbose:
                 print(chunk, end="", flush=True)
 
         outputs = {"response": "".join(chunks)}
         self.memory.save_context(inputs, outputs)
 
-        return response
+        return clean_response
```

### Comparing `ava_llm-0.0.22/ava_llm/prompts/base.py` & `ava_llm-0.0.23/ava_llm/prompts/base.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm/utils/utils.py` & `ava_llm-0.0.23/ava_llm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.22/ava_llm.egg-info/SOURCES.txt` & `ava_llm-0.0.23/ava_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

