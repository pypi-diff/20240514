# Comparing `tmp/openai_responses-0.2.1.tar.gz` & `tmp/openai_responses-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.2.1.tar", max compression
+gzip compressed data, was "openai_responses-0.3.0.tar", max compression
```

## Comparing `openai_responses-0.2.1.tar` & `openai_responses-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,43 @@
--rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.2.1/LICENSE
--rw-r--r--   0        0        0     3182 2024-04-29 14:18:24.992114 openai_responses-0.2.1/README.md
--rw-r--r--   0        0        0     1204 2024-04-29 17:51:43.342527 openai_responses-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1031 2024-04-26 21:00:00.629710 openai_responses-0.2.1/src/openai_responses/__init__.py
--rw-r--r--   0        0        0     1304 2024-03-21 18:06:20.705461 openai_responses-0.2.1/src/openai_responses/decorators.py
--rw-r--r--   0        0        0     5182 2024-04-26 20:03:26.180623 openai_responses-0.2.1/src/openai_responses/endpoints/_base.py
--rw-r--r--   0        0        0     3645 2024-04-24 19:35:49.112709 openai_responses-0.2.1/src/openai_responses/endpoints/_partial_schemas.py
--rw-r--r--   0        0        0     8405 2024-04-26 20:03:26.181090 openai_responses-0.2.1/src/openai_responses/endpoints/assistants.py
--rw-r--r--   0        0        0     5561 2024-04-26 20:03:26.181494 openai_responses-0.2.1/src/openai_responses/endpoints/chat.py
--rw-r--r--   0        0        0     2126 2024-04-26 21:00:00.629975 openai_responses-0.2.1/src/openai_responses/endpoints/embeddings.py
--rw-r--r--   0        0        0     4726 2024-04-26 20:03:26.182119 openai_responses-0.2.1/src/openai_responses/endpoints/files.py
--rw-r--r--   0        0        0     8962 2024-04-26 21:00:00.630246 openai_responses-0.2.1/src/openai_responses/endpoints/messages.py
--rw-r--r--   0        0        0     6622 2024-04-26 21:00:00.630518 openai_responses-0.2.1/src/openai_responses/endpoints/run_steps.py
--rw-r--r--   0        0        0    15709 2024-04-26 21:00:00.630654 openai_responses-0.2.1/src/openai_responses/endpoints/runs.py
--rw-r--r--   0        0        0     5261 2024-04-26 21:00:00.630964 openai_responses-0.2.1/src/openai_responses/endpoints/threads.py
--rw-r--r--   0        0        0     1785 2024-03-22 20:38:26.409131 openai_responses-0.2.1/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.2.1/src/openai_responses/py.typed
--rw-r--r--   0        0        0     5155 2024-03-21 19:42:49.038879 openai_responses-0.2.1/src/openai_responses/state.py
--rw-r--r--   0        0        0      154 2024-04-26 20:23:05.154688 openai_responses-0.2.1/src/openai_responses/tokens.py
--rw-r--r--   0        0        0      740 2024-04-24 14:35:49.271898 openai_responses-0.2.1/src/openai_responses/utils.py
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 openai_responses-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.0/README.md
+-rw-r--r--   0        0        0     1234 2024-05-13 17:16:29.612949 openai_responses-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.0/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.0/src/openai_responses/_api.py
+-rw-r--r--   0        0        0     1845 2024-05-14 15:18:04.142883 openai_responses-0.3.0/src/openai_responses/_mock.py
+-rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.0/src/openai_responses/_routes/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.0/src/openai_responses/_routes/_base.py
+-rw-r--r--   0        0        0     6208 2024-05-10 14:26:39.440069 openai_responses-0.3.0/src/openai_responses/_routes/assistants.py
+-rw-r--r--   0        0        0     1124 2024-05-13 15:47:22.432858 openai_responses-0.3.0/src/openai_responses/_routes/chat.py
+-rw-r--r--   0        0        0     1386 2024-05-03 15:49:36.164682 openai_responses-0.3.0/src/openai_responses/_routes/embeddings.py
+-rw-r--r--   0        0        0     4978 2024-05-03 18:04:28.339502 openai_responses-0.3.0/src/openai_responses/_routes/files.py
+-rw-r--r--   0        0        0     8041 2024-05-10 14:28:24.653989 openai_responses-0.3.0/src/openai_responses/_routes/messages.py
+-rw-r--r--   0        0        0     3767 2024-05-13 15:31:22.122002 openai_responses-0.3.0/src/openai_responses/_routes/run_steps.py
+-rw-r--r--   0        0        0    11056 2024-05-10 19:13:45.175334 openai_responses-0.3.0/src/openai_responses/_routes/runs.py
+-rw-r--r--   0        0        0     5335 2024-05-10 18:39:23.363809 openai_responses-0.3.0/src/openai_responses/_routes/threads.py
+-rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.0/src/openai_responses/_stores/__init__.py
+-rw-r--r--   0        0        0     6059 2024-05-13 14:43:27.895252 openai_responses-0.3.0/src/openai_responses/_stores/state_store.py
+-rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.0/src/openai_responses/_types/generics.py
+-rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.0/src/openai_responses/_types/partials/assistants.py
+-rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.0/src/openai_responses/_types/partials/chat.py
+-rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.0/src/openai_responses/_types/partials/embeddings.py
+-rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.0/src/openai_responses/_types/partials/files.py
+-rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.0/src/openai_responses/_types/partials/messages.py
+-rw-r--r--   0        0        0     2945 2024-05-13 15:43:24.432019 openai_responses-0.3.0/src/openai_responses/_types/partials/run_steps.py
+-rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.0/src/openai_responses/_types/partials/runs.py
+-rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.0/src/openai_responses/_types/partials/threads.py
+-rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.0/src/openai_responses/_utils/copy.py
+-rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.0/src/openai_responses/_utils/faker.py
+-rw-r--r--   0        0        0      446 2024-05-03 15:46:30.517193 openai_responses-0.3.0/src/openai_responses/_utils/serde.py
+-rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.0/src/openai_responses/_utils/time.py
+-rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.0/src/openai_responses/helpers/builders/_base.py
+-rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.0/src/openai_responses/helpers/builders/assistants.py
+-rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.0/src/openai_responses/helpers/builders/chat.py
+-rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.0/src/openai_responses/helpers/builders/embeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.0/src/openai_responses/helpers/builders/messages.py
+-rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.0/src/openai_responses/helpers/builders/run_steps.py
+-rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.0/src/openai_responses/helpers/builders/runs.py
+-rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.0/src/openai_responses/helpers/builders/threads.py
+-rw-r--r--   0        0        0     1271 2024-05-13 15:42:07.751993 openai_responses-0.3.0/src/openai_responses/helpers/state_store.py
+-rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.0/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.0/src/openai_responses/py.typed
+-rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 openai_responses-0.3.0/PKG-INFO
```

### Comparing `openai_responses-0.2.1/LICENSE` & `openai_responses-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.2.1/README.md` & `openai_responses-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,70 @@
+Metadata-Version: 2.1
+Name: openai-responses
+Version: 0.3.0
+Summary: Automatically mock OpenAI requests
+Home-page: https://mharrisb1.github.io/openai-responses-python/
+License: MIT
+Author: Michael Harris
+Author-email: mharris@definite.app
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: faker-openai-api-provider (>=0.1.0,<0.2.0)
+Requires-Dist: openai (>=1.25,<2.0)
+Requires-Dist: respx (>=0.20.2,<0.21.0)
+Project-URL: Documentation, https://mharrisb1.github.io/openai-responses-python/
+Project-URL: Repository, https://github.com/mharrisb1/openai-responses-python
+Description-Content-Type: text/markdown
+
 # 🧪🤖 openai-responses
 
-Pytest plugin for automatically mocking OpenAI requests. Built on top of [RESPX](https://github.com/lundberg/respx).
+Pytest plugin for automatically mocking OpenAI requests. Powered by [RESPX](https://github.com/lundberg/respx).
+
+[![sdk support](https://img.shields.io/badge/SDK_Support-v1.25+-white?logo=openai&logoColor=black&labelColor=white)](https://github.com/openai/openai-python)
 
-## Supported endpoints
+## Supported Routes
 
 - `/v1/chat/completions`
 - `/v1/embeddings`
 - `/v1/files`
 - `/v1/assistants`
 - `/v1/threads` (+ messages, runs, and steps)
 
-View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/endpoints/).
+View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/routes).
 
 ## Usage
 
-Simply decorate any test function that contains code that makes a call to an OpenAI endpoint. See [docs](https://mharrisb1.github.io/openai-responses-python) for more.
+Just decorate any test function that makes a call to the OpenAI API (either using [openai-python](https://github.com/openai/openai-python) or with [HTTPX](https://www.python-httpx.org/)).
 
 ```python
+import openai
+
 import openai_responses
-from openai import OpenAI
 
 
-@openai_responses.mock.chat.completions(
-    choices=[
-        {"message": {"content": "Hello, how can I help?"}},
-        {"message": {"content": "Hi! I'm here to help!"}},
-        {"message": {"content": "How can I help?"}},
-    ],
-)
-def test_create_completion_with_multiple_choices():
-    client = OpenAI(api_key="fakeKey")
-    completion = client.chat.completions.create(
-        model="gpt-3.5-turbo",
-        messages=[
-            {"role": "system", "content": "You are a helpful assistant."},
-            {"role": "user", "content": "Hello!"},
-        ],
-        n=3,
+@openai_responses.mock()
+def test_create_assistant():
+    client = openai.Client(api_key="sk-fake123")
+
+    assistant = client.beta.assistants.create(
+        instructions="You are a personal math tutor.",
+        name="Math Tutor",
+        tools=[{"type": "code_interpreter"}],
+        model="gpt-4-turbo",
     )
-    assert len(completion.choices) == 3
+
+    assert assistant.name == "Math Tutor"
 ```
 
-> [!IMPORTANT]
-> This project does not try to generate fake responses from the models. Any part of a response that would be generated by a model will need to be defined by the user or will fallback to a default value.
+See [examples](https://github.com/mharrisb1/openai-responses-python/tree/main/examples) or [docs](https://mharrisb1.github.io/openai-responses-python) for more.
 
 ## Installation
 
 [![PyPI version](https://badge.fury.io/py/openai-responses.svg)](https://badge.fury.io/py/openai-responses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openai-responses.svg)](https://pypi.org/project/openai-responses/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/openai-responses)](https://pypi.org/project/openai-responses/)
 
@@ -74,7 +92,8 @@
 [![Stargazers](https://img.shields.io/github/stars/mharrisb1/openai-responses-python?style)](https://pypistats.org/packages/openai-responses)
 
 See [CONTRIBUTING.md](https://github.com/mharrisb1/openai-responses-python/blob/main/CONTRIBUTING.md) for info on PRs, issues, and feature requests.
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/mharrisb1/openai-responses-python/blob/main/CHANGELOG.md) for summarized notes on changes or view [releases](https://github.com/mharrisb1/openai-responses-python/releases) for more details information on changes.
+
```

### Comparing `openai_responses-0.2.1/pyproject.toml` & `openai_responses-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.2.1"
+version = "0.3.0"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
-homepage = "https://github.com/mharrisb1/openai-responses-python"
+homepage = "https://mharrisb1.github.io/openai-responses-python/"
+documentation = "https://mharrisb1.github.io/openai-responses-python/"
 packages = [{ include = "openai_responses", from = "src" }]
 
 [tool.poetry.plugins.pytest11]
 openai_responses = "openai_responses.plugin"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-openai = "^1.23"
+openai = "^1.25"
 respx = "^0.20.2"
-decorator = "^5.1.1"
 faker-openai-api-provider = "^0.1.0"
-tiktoken = "^0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 types-decorator = "^5.1.8.20240310"
```

### Comparing `openai_responses-0.2.1/src/openai_responses/endpoints/_partial_schemas.py` & `openai_responses-0.3.0/src/openai_responses/_types/partials/run_steps.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,143 +1,119 @@
-from typing import Annotated, Literal, List, Optional, TypedDict, Union
-from typing_extensions import Required
+from typing import Annotated, Dict, List, Literal, TypedDict, Union
+from typing_extensions import NotRequired
 
-from openai._utils._transform import PropertyInfo
-from openai.types.beta.assistant_tool_param import AssistantToolParam
-from openai.types.beta.threads.run_status import RunStatus
+from openai._utils import PropertyInfo
 
-__all__ = ["PartialRun", "PartialRunStep"]
+__all__ = ["PartialRunStep", "PartialRunStepList"]
 
 
-class PartialIncompleteDetails(TypedDict):
-    reason: Optional[Literal["max_completion_tokens", "max_prompt_tokens"]]
-
-
-class PartialFunctionNoOutput(TypedDict):
-    name: str
-    arguments: str
-
-
-class PartialRequiredActionFunctionToolCall(TypedDict):
-    id: str
-    function: PartialFunctionNoOutput
-    type: Literal["function"]
-
-
-class PartialRequiredActionSubmitToolOutputs(TypedDict):
-    tool_calls: List[PartialRequiredActionFunctionToolCall]
-
-
-class PartialRequiredAction(TypedDict):
-    submit_tool_outputs: PartialRequiredActionSubmitToolOutputs
-    type: Literal["submit_tool_outputs"]
+class PartialLastError(TypedDict):
+    code: Literal["server_error", "rate_limit_exceeded"]
+    message: str
 
 
-class PartialLastError(TypedDict, total=False):
-    code: Literal["server_error", "rate_limit_exceeded", "invalid_prompt"]
-    message: str
+class PartialMessageCreation(TypedDict):
+    message_id: str
 
 
-class PartialRun(TypedDict, total=False):
-    cancelled_at: int
-    completed_at: int
-    expires_at: int
-    failed_at: int
-    incomplete_details: PartialIncompleteDetails
-    instructions: str
-    last_error: PartialLastError
-    model: str
-    required_action: PartialRequiredAction
-    started_at: int
-    status: RunStatus
-    tools: List[AssistantToolParam]
+class PartialMessageCreationStepDetails(TypedDict):
+    message_creation: PartialMessageCreation
+    type: Literal["message_creation"]
 
 
 class PartialCodeInterpreterOutputLogs(TypedDict):
     logs: str
     type: Literal["logs"]
 
 
 class PartialCodeInterpreterOutputImageImage(TypedDict):
     file_id: str
 
 
 class PartialCodeInterpreterOutputImage(TypedDict):
-    type: Literal["image"]
     image: PartialCodeInterpreterOutputImageImage
+    type: Literal["image"]
 
 
 class PartialCodeInterpreter(TypedDict):
     input: str
     outputs: List[
         Annotated[
-            Union[
-                PartialCodeInterpreterOutputLogs,
-                PartialCodeInterpreterOutputImage,
-            ],
+            Union[PartialCodeInterpreterOutputLogs, PartialCodeInterpreterOutputImage],
             PropertyInfo(discriminator="type"),
         ]
     ]
 
 
 class PartialCodeInterpreterToolCall(TypedDict):
-    type: Literal["code_interpreter"]
     id: str
     code_interpreter: PartialCodeInterpreter
+    type: Literal["code_interpreter"]
 
 
-class PartialRetrievalToolCall(TypedDict):
-    type: Literal["retrieval"]
+class PartialFileSearchToolCall(TypedDict):
     id: str
+    file_search: object
+    type: Literal["file_search"]
 
 
-class PartialFunction(TypedDict, total=False):
-    name: Required[str]
-    arguments: Required[str]
-    output: Optional[str]
+class PartialFunction(TypedDict):
+    arguments: str
+    name: str
+    output: NotRequired[str]
 
 
 class PartialFunctionToolCall(TypedDict):
-    type: Literal["function"]
     id: str
     function: PartialFunction
+    type: Literal["function"]
 
 
 class PartialToolCallsStepDetails(TypedDict):
-    type: Literal["tool_calls"]
-    tool_calls: List[
-        Annotated[
-            Union[
-                PartialCodeInterpreterToolCall,
-                PartialRetrievalToolCall,
-                PartialFunctionToolCall,
-            ],
-            PropertyInfo(discriminator="type"),
-        ]
+    tool_calls: Annotated[
+        Union[
+            PartialCodeInterpreterToolCall,
+            PartialFileSearchToolCall,
+            PartialFunctionToolCall,
+        ],
+        PropertyInfo(discriminator="type"),
     ]
+    type: Literal["tool_calls"]
 
 
-class PartialMessageCreation(TypedDict):
-    message_id: str
+class PartialUsage(TypedDict):
+    completion_tokens: int
+    prompt_tokens: int
+    total_tokens: int
 
 
-class PartialMessageCreationStepDetails(TypedDict):
-    type: Literal["message_creation"]
-    message_creation: PartialMessageCreation
+PartialStepDetails = Annotated[
+    Union[PartialMessageCreationStepDetails, PartialToolCallsStepDetails],
+    PropertyInfo(discriminator="type"),
+]
 
 
-class PartialRunStep(TypedDict, total=False):
-    id: str
+class PartialRunStep(TypedDict):
+    id: NotRequired[str]
     assistant_id: str
-    cancelled_at: Optional[int]
-    completed_at: Optional[int]
-    expired_at: Optional[int]
-    failed_at: Optional[int]
-    last_error: Optional[PartialLastError]
+    cancelled_at: NotRequired[int]
+    completed_at: NotRequired[int]
+    created_at: NotRequired[int]
+    expired_at: NotRequired[int]
+    failed_at: NotRequired[int]
+    last_error: NotRequired[PartialLastError]
+    metadata: NotRequired[Dict[str, str]]
+    object: NotRequired[Literal["thread.run.step"]]
+    run_id: str
     status: Literal["in_progress", "cancelled", "failed", "completed", "expired"]
-    step_details: Required[
-        Annotated[
-            Union[PartialMessageCreationStepDetails, PartialToolCallsStepDetails],
-            PropertyInfo(discriminator="type"),
-        ]
-    ]
+    step_details: PartialStepDetails
+    thread_id: str
     type: Literal["message_creation", "tool_calls"]
+    usage: NotRequired[PartialUsage]
+
+
+class PartialRunStepList(TypedDict):
+    object: NotRequired[Literal["list"]]
+    data: NotRequired[List[PartialRunStep]]
+    first_id: NotRequired[str]
+    last_id: NotRequired[str]
+    has_more: NotRequired[bool]
```

### Comparing `openai_responses-0.2.1/src/openai_responses/endpoints/threads.py` & `openai_responses-0.3.0/src/openai_responses/_routes/threads.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,179 +1,166 @@
 import json
-from typing import Any, Optional
+from typing import Any
+from typing_extensions import override
 
 import httpx
 import respx
 
-from openai.types.beta.thread import Thread, ToolResources
-from openai.types.beta.thread_deleted import ThreadDeleted
-from openai.types.beta.thread_update_params import ThreadUpdateParams
+from openai.types.beta.thread import Thread
 from openai.types.beta.thread_create_params import ThreadCreateParams
+from openai.types.beta.thread_update_params import ThreadUpdateParams
+from openai.types.beta.thread_deleted import ThreadDeleted
 
-from ._base import StatefulMock, CallContainer
-from .messages import MessagesMock
-from .runs import RunsMock
+from ._base import StatefulRoute
 
-from ..decorators import side_effect
-from ..state import StateStore
-from ..utils import model_dict, model_parse, utcnow_unix_timestamp_s
+from ..helpers.builders.messages import message_from_create_request
 
-__all__ = ["ThreadsMock"]
+from .._stores import StateStore
+from .._types.partials.threads import PartialThread, PartialThreadDeleted
 
+from .._utils.faker import faker
+from .._utils.serde import model_dict, model_parse
+from .._utils.time import utcnow_unix_timestamp_s
 
-class ThreadsMock(StatefulMock):
-    def __init__(self) -> None:
-        super().__init__(
-            name="threads_mock",
-            endpoint="/v1/threads",
-            route_registrations=[
-                {
-                    "name": "create",
-                    "method": respx.post,
-                    "pattern": None,
-                    "side_effect": self._create,
-                },
-                {
-                    "name": "retrieve",
-                    "method": respx.get,
-                    "pattern": r"/(?P<id>\w+)",
-                    "side_effect": self._retrieve,
-                },
-                {
-                    "name": "update",
-                    "method": respx.post,
-                    "pattern": r"/(?P<id>\w+)",
-                    "side_effect": self._update,
-                },
-                {
-                    "name": "delete",
-                    "method": respx.delete,
-                    "pattern": r"/(?P<id>\w+)",
-                    "side_effect": self._delete,
-                },
-            ],
-        )
-
-        # NOTE: these are explicitly defined to help with autocomplete and type hints
-        self.create = CallContainer()
-        self.retrieve = CallContainer()
-        self.update = CallContainer()
-        self.delete = CallContainer()
 
-        self.messages = MessagesMock()
-        self.runs = RunsMock()
+__all__ = [
+    "ThreadCreateRoute",
+    "ThreadRetrieveRoute",
+    "ThreadUpdateRoute",
+    "ThreadDeleteRoute",
+]
 
-    def __call__(
-        self,
-        *,
-        latency: Optional[float] = None,
-        failures: Optional[int] = None,
-        state_store: Optional[StateStore] = None,
-    ):
-        def getter(*args: Any, **kwargs: Any):
-            return dict(
-                latency=latency or 0,
-                failures=failures or 0,
-                state_store=kwargs["used_state"],
-            )
 
-        return self._make_decorator(getter, state_store or StateStore())
+class ThreadCreateRoute(StatefulRoute[Thread, PartialThread]):
+    def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
+        super().__init__(
+            route=router.post(url__regex="/v1/threads"),
+            status_code=201,
+            state=state,
+        )
 
-    @side_effect
-    def _create(
-        self,
-        request: httpx.Request,
-        route: respx.Route,
-        state_store: StateStore,
-        **kwargs: Any,
-    ) -> httpx.Response:
-        self.create.route = route
+    @override
+    def _handler(self, request: httpx.Request, route: respx.Route) -> httpx.Response:
+        self._route = route
 
         content: ThreadCreateParams = json.loads(request.content)
+        model = self._build({}, request)
+        self._state.beta.threads.put(model)
+
+        if content.get("messages"):
+            for message_create_params in content.get("messages", []):
+                encoded = json.dumps(message_create_params).encode("utf-8")
+                create_message_req = httpx.Request(method="", url="", content=encoded)
+                message = message_from_create_request(model.id, create_message_req)
+                self._state.beta.threads.messages.put(message)
+
+        return httpx.Response(
+            status_code=self._status_code,
+            json=model_dict(model),
+        )
 
-        thread = Thread(
-            id=self._faker.beta.thread.id(),
-            created_at=utcnow_unix_timestamp_s(),
-            tool_resources=model_parse(ToolResources, content.get("tool_resources")),
-            metadata=content.get("metadata"),
-            object="thread",
-        )
-        messages = [
-            self.messages._parse_message_create_params(thread.id, m)
-            for m in content.get("messages", [])
-        ]
-
-        state_store.beta.threads.put(thread)
-        for message in messages:
-            state_store.beta.threads.messages.put(message)
+    @staticmethod
+    def _build(partial: PartialThread, request: httpx.Request) -> Thread:
+        content = json.loads(request.content)
+        if content.get("messages"):
+            del content["messages"]
+        if content.get("tool_resources"):
+            del content["tool_resources"]
+        defaults: PartialThread = {
+            "id": faker.beta.thread.id(),
+            "created_at": utcnow_unix_timestamp_s(),
+            "object": "thread",
+        }
+        return model_parse(Thread, defaults | partial | content)
 
-        return httpx.Response(status_code=201, json=model_dict(thread))
 
-    @side_effect
-    def _retrieve(
+class ThreadRetrieveRoute(StatefulRoute[Thread, PartialThread]):
+    def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
+        super().__init__(
+            route=router.get(url__regex=r"/v1/threads/(?P<id>[a-zA-Z0-9\_]+)"),
+            status_code=200,
+            state=state,
+        )
+
+    @override
+    def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
-        id: str,
-        state_store: StateStore,
         **kwargs: Any,
     ) -> httpx.Response:
-        self.retrieve.route = route
+        self._route = route
+        id = kwargs["id"]
+        found = self._state.beta.threads.get(id)
+        if not found:
+            return httpx.Response(404)
+
+        return httpx.Response(status_code=200, json=model_dict(found))
 
-        *_, id = request.url.path.split("/")
-        thread = state_store.beta.threads.get(id)
+    @staticmethod
+    def _build(partial: PartialThread, request: httpx.Request) -> Thread:
+        raise NotImplementedError
 
-        if not thread:
-            return httpx.Response(status_code=404)
 
-        else:
-            return httpx.Response(status_code=200, json=model_dict(thread))
+class ThreadUpdateRoute(StatefulRoute[Thread, PartialThread]):
+    def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
+        super().__init__(
+            route=router.post(
+                url__regex=r"/v1/threads/(?P<id>(?!.*runs)[a-zA-Z0-9_]+)"  # NOTE: avoids match on /threads/runs
+            ),
+            status_code=200,
+            state=state,
+        )
 
-    @side_effect
-    def _update(
+    @override
+    def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
-        id: str,
-        state_store: StateStore,
         **kwargs: Any,
     ) -> httpx.Response:
-        self.update.route = route
+        self._route = route
+        id = kwargs["id"]
+        found = self._state.beta.threads.get(id)
+        if not found:
+            return httpx.Response(404)
 
-        *_, id = request.url.path.split("/")
         content: ThreadUpdateParams = json.loads(request.content)
+        deserialized = model_dict(found)
+        updated = model_parse(Thread, deserialized | content)
+        self._state.beta.threads.put(updated)
 
-        thread = state_store.beta.threads.get(id)
+        return httpx.Response(status_code=200, json=model_dict(updated))
 
-        if not thread:
-            return httpx.Response(status_code=404)
+    @staticmethod
+    def _build(partial: PartialThread, request: httpx.Request) -> Thread:
+        raise NotImplementedError
 
-        thread.tool_resources = (
-            model_parse(ToolResources, content.get("tool_resources"))
-            or thread.tool_resources
-        )
-        thread.metadata = content.get("metadata", thread.metadata)
-
-        state_store.beta.threads.put(thread)
 
-        return httpx.Response(status_code=200, json=model_dict(thread))
+class ThreadDeleteRoute(StatefulRoute[ThreadDeleted, PartialThreadDeleted]):
+    def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
+        super().__init__(
+            route=router.delete(url__regex=r"/v1/threads/(?P<id>[a-zA-Z0-9\_]+)"),
+            status_code=200,
+            state=state,
+        )
 
-    @side_effect
-    def _delete(
+    @override
+    def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
-        id: str,
-        state_store: StateStore,
         **kwargs: Any,
     ) -> httpx.Response:
-        self.delete.route = route
-
-        *_, id = request.url.path.split("/")
-        deleted = state_store.beta.threads.delete(id)
-
+        self._route = route
+        id = kwargs["id"]
+        deleted = self._state.beta.threads.delete(id)
         return httpx.Response(
             status_code=200,
             json=model_dict(
                 ThreadDeleted(id=id, deleted=deleted, object="thread.deleted")
             ),
         )
+
+    @staticmethod
+    def _build(partial: PartialThreadDeleted, request: httpx.Request) -> ThreadDeleted:
+        raise NotImplementedError
```

### Comparing `openai_responses-0.2.1/src/openai_responses/state.py` & `openai_responses-0.3.0/src/openai_responses/_stores/state_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Generic, List, Literal, Optional, TypeVar, Union
+from typing import Any, Dict, Generic, List, Literal, Optional, TypeVar, Union
 
 from openai.types import FileObject
 from openai.types.beta.assistant import Assistant
 from openai.types.beta.thread import Thread
 from openai.types.beta.threads.message import Message
 from openai.types.beta.threads.run import Run
 from openai.types.beta.threads.runs.run_step import RunStep
@@ -18,20 +18,38 @@
         Thread,
         Message,
         Run,
         RunStep,
     ],
 )
 
+Resource = Union[FileObject, Assistant, Thread, Message, Run, RunStep, Any]
+
 
 class StateStore:
     def __init__(self) -> None:
         self.files = FileStore()
         self.beta = Beta()
 
+    def _blind_put(self, resource: Resource) -> None:
+        if isinstance(resource, FileObject):
+            self.files.put(resource)
+        elif isinstance(resource, Assistant):
+            self.beta.assistants.put(resource)
+        elif isinstance(resource, Thread):
+            self.beta.threads.put(resource)
+        elif isinstance(resource, Message):
+            self.beta.threads.messages.put(resource)
+        elif isinstance(resource, Run):
+            self.beta.threads.runs.put(resource)
+        elif isinstance(resource, RunStep):
+            self.beta.threads.runs.steps.put(resource)
+        else:
+            raise TypeError(f"Cannot put object of type {type(resource)} in store")
+
 
 class Beta:
     def __init__(self) -> None:
         self.assistants = AssistantStore()
         self.threads = ThreadStore()
 
 
@@ -110,16 +128,19 @@
     def list(
         self,
         thread_id: str,
         limit: Optional[int] = None,
         order: Optional[str] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
+        run_id: Optional[str] = None,
     ) -> List[Message]:
         objs = [m for m in list(self._data.values()) if m.thread_id == thread_id]
+        if run_id:
+            objs = [obj for obj in objs if obj.run_id == run_id]
         objs = list(reversed(objs)) if (order or "desc") == "desc" else objs
 
         start_ix = 0
         if after:
             obj = self._data.get(after)
             if obj:
                 start_ix = objs.index(obj) + 1
```

