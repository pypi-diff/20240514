# Comparing `tmp/llama_index_agent_openai-0.2.4.tar.gz` & `tmp/llama_index_agent_openai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai-0.2.4.tar", max compression
+gzip compressed data, was "llama_index_agent_openai-0.2.5.tar", max compression
```

## Comparing `llama_index_agent_openai-0.2.4.tar` & `llama_index_agent_openai-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       39 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/README.md
--rw-r--r--   0        0        0      342 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/__init__.py
--rw-r--r--   0        0        0     4745 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/base.py
--rw-r--r--   0        0        0    18794 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/openai_assistant_agent.py
--rw-r--r--   0        0        0    28597 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/step.py
--rw-r--r--   0        0        0      772 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/utils.py
--rw-r--r--   0        0        0     1522 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/README.md
+-rw-r--r--   0        0        0      342 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/base.py
+-rw-r--r--   0        0        0    18955 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/openai_assistant_agent.py
+-rw-r--r--   0        0        0    28597 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/step.py
+-rw-r--r--   0        0        0      772 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/utils.py
+-rw-r--r--   0        0        0     1522 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.5/PKG-INFO
```

### Comparing `llama_index_agent_openai-0.2.4/llama_index/agent/openai/base.py` & `llama_index_agent_openai-0.2.5/llama_index/agent/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.4/llama_index/agent/openai/openai_assistant_agent.py` & `llama_index_agent_openai-0.2.5/llama_index/agent/openai/openai_assistant_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """OpenAI Assistant Agent."""
+
 import asyncio
 import json
 import logging
 import time
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 from llama_index.agent.openai.utils import get_function_by_name
@@ -130,14 +131,20 @@
     file_dict = {}
     for file in files:
         file_obj = client.files.create(file=open(file, "rb"), purpose="assistants")
         file_dict[file_obj.id] = file
     return file_dict
 
 
+def format_attachments(file_ids: Optional[List[str]] = None) -> List[Dict[str, str]]:
+    """Create attachments from file_ids."""
+    file_ids = file_ids or []
+    return [{"file_id": file_id} for file_id in file_ids]
+
+
 class OpenAIAssistantAgent(BaseAgent):
     """OpenAIAssistant agent.
 
     Wrapper around OpenAI assistant API: https://platform.openai.com/docs/assistants/overview
 
     """
 
@@ -219,24 +226,22 @@
         client = OpenAI(api_key=api_key)
 
         # process files
         files = files or []
         file_ids = file_ids or []
 
         file_dict = _process_files(client, files)
-        all_file_ids = list(file_dict.keys()) + file_ids
 
         # TODO: openai's typing is a bit sus
         all_openai_tools = cast(List[Any], all_openai_tools)
         assistant = client.beta.assistants.create(
             name=name,
             instructions=instructions,
             tools=cast(List[Any], all_openai_tools),
             model=model,
-            file_ids=all_file_ids,
         )
         return cls(
             client,
             assistant,
             tools,
             callback_manager=callback_manager,
             thread_id=thread_id,
@@ -331,20 +336,20 @@
 
     def upload_files(self, files: List[str]) -> Dict[str, Any]:
         """Upload files."""
         return _process_files(self._client, files)
 
     def add_message(self, message: str, file_ids: Optional[List[str]] = None) -> Any:
         """Add message to assistant."""
-        file_ids = file_ids or []
+        attachments = format_attachments(file_ids=file_ids)
         return self._client.beta.threads.messages.create(
             thread_id=self._thread_id,
             role="user",
             content=message,
-            file_ids=file_ids,
+            attachments=attachments,
         )
 
     def _run_function_calling(self, run: Any) -> List[ToolOutput]:
         """Run function calling."""
         tool_calls = run.required_action.submit_tool_outputs.tool_calls
         tool_output_dicts = []
         tool_output_objs: List[ToolOutput] = []
```

### Comparing `llama_index_agent_openai-0.2.4/llama_index/agent/openai/step.py` & `llama_index_agent_openai-0.2.5/llama_index/agent/openai/step.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.4/llama_index/agent/openai/utils.py` & `llama_index_agent_openai-0.2.5/llama_index/agent/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.4/pyproject.toml` & `llama_index_agent_openai-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai"
 readme = "README.md"
-version = "0.2.4"
+version = "0.2.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.35"
 llama-index-llms-openai = "^0.1.5"
 openai = ">=1.14.0"
```

### Comparing `llama_index_agent_openai-0.2.4/PKG-INFO` & `llama_index_agent_openai-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai
-Version: 0.2.4
+Version: 0.2.5
 Summary: llama-index agent openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

