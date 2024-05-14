# Comparing `tmp/totokenizers-1.2.4.1.tar.gz` & `tmp/totokenizers-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totokenizers-1.2.4.1.tar", last modified: Thu May  9 18:08:52 2024, max compression
+gzip compressed data, was "totokenizers-1.2.5.tar", last modified: Tue May 14 20:24:43 2024, max compression
```

## Comparing `totokenizers-1.2.4.1.tar` & `totokenizers-1.2.5.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:52.635196 totokenizers-1.2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 18:08:52.631196 totokenizers-1.2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:08:52.635196 totokenizers-1.2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:52.627196 totokenizers-1.2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/tests/test_jsonschema_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:52.627196 totokenizers-1.2.4.1/totokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:52.631196 totokenizers-1.2.4.1/totokenizers/anthropic/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/anthropic/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/anthropic/info.py
--rw-r--r--   0 runner    (1001) docker     (127)  1774213 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/anthropic/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/jsonschema_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:52.631196 totokenizers-1.2.4.1/totokenizers/mockai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/mockai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/mockai/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/mockai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/model_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/openai_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 18:08:36.000000 totokenizers-1.2.4.1/totokenizers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:08:52.631196 totokenizers-1.2.4.1/totokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 18:08:52.000000 totokenizers-1.2.4.1/totokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 18:08:52.000000 totokenizers-1.2.4.1/totokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:08:52.000000 totokenizers-1.2.4.1/totokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 18:08:52.000000 totokenizers-1.2.4.1/totokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 18:08:52.000000 totokenizers-1.2.4.1/totokenizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:08:52.000000 totokenizers-1.2.4.1/totokenizers.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:43.601405 totokenizers-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-14 20:24:43.601405 totokenizers-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-14 20:24:32.000000 totokenizers-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:24:43.601405 totokenizers-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-14 20:24:32.000000 totokenizers-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:43.593405 totokenizers-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-14 20:24:32.000000 totokenizers-1.2.5/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-14 20:24:32.000000 totokenizers-1.2.5/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-14 20:24:32.000000 totokenizers-1.2.5/tests/test_jsonschema_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 20:24:32.000000 totokenizers-1.2.5/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:43.597405 totokenizers-1.2.5/totokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:43.597405 totokenizers-1.2.5/totokenizers/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/anthropic/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/anthropic/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1774213 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/anthropic/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:43.601405 totokenizers-1.2.5/totokenizers/google/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/google/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/jsonschema_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:43.601405 totokenizers-1.2.5/totokenizers/mockai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/mockai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/mockai/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/mockai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/openai_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-14 20:24:32.000000 totokenizers-1.2.5/totokenizers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:43.601405 totokenizers-1.2.5/totokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-14 20:24:43.000000 totokenizers-1.2.5/totokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-14 20:24:43.000000 totokenizers-1.2.5/totokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:24:43.000000 totokenizers-1.2.5/totokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 20:24:43.000000 totokenizers-1.2.5/totokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 20:24:43.000000 totokenizers-1.2.5/totokenizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:24:43.000000 totokenizers-1.2.5/totokenizers.egg-info/zip-safe
```

### Comparing `totokenizers-1.2.4.1/PKG-INFO` & `totokenizers-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: totokenizers
-Version: 1.2.4.1
+Version: 1.2.5
 Summary: Text tokenizers.
 Home-page: https://github.com/TeiaLabs/totokenizers
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Requires-Dist: google-cloud-aiplatform
 Requires-Dist: tiktoken
-Requires-Dist: tokenizers
+Requires-Dist: tokenizers>=0.7.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # totokenizers
 
 A model-agnostic library to encode text into tokens and couting them using different tokenizers.
```

### Comparing `totokenizers-1.2.4.1/README.md` & `totokenizers-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/setup.py` & `totokenizers-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/tests/test_anthropic.py` & `totokenizers-1.2.5/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/tests/test_code.py` & `totokenizers-1.2.5/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/tests/test_jsonschema_formatter.py` & `totokenizers-1.2.5/tests/test_jsonschema_formatter.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers/anthropic/anthropic.py` & `totokenizers-1.2.5/totokenizers/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers/anthropic/info.py` & `totokenizers-1.2.5/totokenizers/anthropic/info.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 
 ANTHROPIC_CHAT_MODELS = {
     info.name: info
     for info in [
         ChatModelInfo(
             completion_token_cost=0.024,
             cutoff="2023-01-01",
+            feature_flags=[],
+            max_output_tokens=204_096,
             max_tokens=204_096,
             name="claude-2.1",
             prompt_token_cost=0.008,
-            supports_functions=False,
         ),
         ChatModelInfo(
             completion_token_cost=0.0024,
             cutoff="2023-01-01",
+            feature_flags=[],
+            max_output_tokens=104_096,
             max_tokens=104_096,
             name="claude-instant-1.2",
             prompt_token_cost=0.0008,
-            supports_functions=False,
-        )
+        ),
     ]
 }
 
 
 ANTHROPIC_MODELS: dict[str, ChatModelInfo] = {**ANTHROPIC_CHAT_MODELS}
```

### Comparing `totokenizers-1.2.4.1/totokenizers/anthropic/tokenizer.json` & `totokenizers-1.2.5/totokenizers/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers/errors.py` & `totokenizers-1.2.5/totokenizers/errors.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers/factories.py` & `totokenizers-1.2.5/totokenizers/factories.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,65 @@
+from typing import Literal, overload
 
-from .anthropic import AnthropicTokenizer, ANTHROPIC_MODELS
-from .errors import ModelNotFound, ModelProviderNotFound, BadFormatForModelTag
+from .anthropic import ANTHROPIC_MODELS, AnthropicTokenizer
+from .errors import BadFormatForModelTag, ModelNotFound, ModelProviderNotFound
 from .mockai.info import MODELS as MOCKAI_MODELS
 from .mockai.tokenizer import MockAITokenizer
 from .openai import OpenAITokenizer
 from .openai_info import OPEN_AI_MODELS
 
+TokenizerType = OpenAITokenizer | AnthropicTokenizer | MockAITokenizer
+
 
 class Totokenizer:
 
     @classmethod
-    def from_model(cls, model: str) -> OpenAITokenizer:
+    def from_model(cls, model: str) -> TokenizerType:
         try:
             provider, model_name = model.split("/", 1)
         except (ValueError, TypeError):
             raise BadFormatForModelTag(model)
-        if provider == "anthropic":
-            return AnthropicTokenizer(model_name)  # type: ignore
-        if provider == "openai":
-            return OpenAITokenizer(model_name)  # type: ignore
-        if provider == "mockai":
-            return MockAITokenizer(model_name)  # type: ignore
-        raise ModelProviderNotFound(provider)
+        return cls.from_provider(provider, model_name)
+
+    @overload
+    @classmethod
+    def from_provider(
+        cls, provider: Literal["openai"], model: str
+    ) -> OpenAITokenizer: ...
+    @overload
+    @classmethod
+    def from_provider(
+        cls, provider: Literal["anthropic"], model: str
+    ) -> AnthropicTokenizer: ...
+    @overload
+    @classmethod
+    def from_provider(
+        cls, provider: Literal["mockai"], model: str
+    ) -> MockAITokenizer: ...
+
+    @classmethod
+    def from_provider(cls, provider: str, model: str) -> TokenizerType:
+        # use pattern matching
+        match provider:
+            case "anthropic":
+                return AnthropicTokenizer(model)
+            case "openai":
+                return OpenAITokenizer(model)
+            case "mockai":
+                return MockAITokenizer(model)
+            case _:
+                raise ModelProviderNotFound(provider)
 
     def encode(self, text: str) -> list[int]:
         raise NotImplementedError
 
     def count_tokens(self, text: str) -> int:
         raise NotImplementedError
 
 
-
-
 class TotoModelInfo:
 
     @classmethod
     def from_model(cls, model: str):
         try:
             provider, model_name = model.split("/", 1)
         except ValueError:
```

### Comparing `totokenizers-1.2.4.1/totokenizers/jsonschema_formatter.py` & `totokenizers-1.2.5/totokenizers/jsonschema_formatter.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers/mockai/info.py` & `totokenizers-1.2.5/totokenizers/mockai/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from ..model_info import ChatModelInfo
 
-
 CHAT_MODELS = {
     info.name: info
     for info in [
         ChatModelInfo(
             completion_token_cost=0,
             cutoff="1997-01-01",
             max_tokens=4096,
+            max_output_tokens=4096,
             name="always-func",
             prompt_token_cost=0,
         ),
         ChatModelInfo(
             completion_token_cost=0,
             cutoff="1997-01-01",
             max_tokens=4096,
+            max_output_tokens=4096,
             name="always-chat",
             prompt_token_cost=0,
-            supports_functions=True,
         ),
     ]
 }
 
 MODELS: dict[str, ChatModelInfo] = {**CHAT_MODELS}
```

### Comparing `totokenizers-1.2.4.1/totokenizers/mockai/tokenizer.py` & `totokenizers-1.2.5/totokenizers/mockai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers/openai.py` & `totokenizers-1.2.5/totokenizers/openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import logging
-from typing import Literal, Optional, Sequence, Mapping
+from typing import Literal, Mapping, Optional, Sequence
 
 import tiktoken
 
 from .errors import ModelNotFound, ModelNotSupported
 from .jsonschema_formatter import FunctionJSONSchema
-from .schemas import Chat, ChatMLMessage, FunctionCallChatMLMessage, FunctionChatMLMessage
+from .schemas import (
+    Chat,
+    ChatMLMessage,
+    FunctionCallChatMLMessage,
+    FunctionChatMLMessage,
+)
 
 logger = logging.getLogger("totokenizers")
 
 
 class OpenAITokenizer:
     funcion_header = "\n".join(
         [
@@ -21,59 +26,53 @@
             "",
             "} // namespace functions",
         ]
     )
 
     def __init__(
         self,
-        model_name: Literal[
-            "gpt-3.5-turbo",
-            "gpt-3.5-turbo-0301",
-            "gpt-3.5-turbo-0613",
-            "gpt-3.5-turbo-16k-0613",
-            "gpt-4-0314",
-            "gpt-4-32k-0314",
-            "gpt-4-0613",
-            "gpt-4-32k-0613",
-        ],
+        model_name: str,
     ):
         self.model = model_name
         try:
             self.encoder = tiktoken.encoding_for_model(model_name)
         except KeyError:
             raise ModelNotFound(model_name)
         self._init_model_params()
 
     def _init_model_params(self):
         """https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb"""
-        if self.model in ("text-embedding-ada-002", "text-davinci-003", "gpt-3.5-turbo-instruct"):
+        if self.model in (
+            "text-embedding-ada-002",
+            "text-embedding-3-small",
+            "text-embedding-3-large",
+            "text-davinci-003",
+            "gpt-3.5-turbo-instruct",
+        ):
             self.count_chatml_tokens = NotImplementedError
             self.count_functions_tokens = NotImplementedError
             self.count_message_tokens = NotImplementedError
             return
-        if self.model in ("gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-4", "gpt-4-32k"):
-            logger.warning(
-                f"'{self.model}' may update over time. Returning num tokens assuming '{self.model}-0613'."
-            )
-            self.model = f"{self.model}-0613"
-            self.model = "gpt-4-0613"
         if self.model in {
+            "gpt-4-0314",
+            "gpt-4-32k-0314",
             "gpt-3.5-turbo-0613",
             "gpt-3.5-turbo-16k-0613",
-            "gpt-3.5-turbo-1106",
-            "gpt-3.5-turbo-0125",
-            "gpt-4-0314",
             "gpt-4-0613",
+            "gpt-4-32k-0613",
+            "gpt-3.5-turbo-1106",
             "gpt-4-1106-preview",
             "gpt-4-0125-preview",
             "gpt-4-turbo-preview", # currently points to gpt-4-0125-preview
             "gpt-4-32k-0314",
             "gpt-4-32k-0613",
             "gpt-4-turbo-2024-04-09",
-            "gpt-4-turbo"
+            "gpt-3.5-turbo-0125",
+            "gpt-4-turbo-2024-04-09",
+            "gpt-4o-2024-05-13",
         }:
             self.tokens_per_message = 3
             self.tokens_per_name = 1
         elif self.model == "gpt-3.5-turbo-0301":
             self.tokens_per_message = (
                 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
             )
@@ -90,42 +89,47 @@
     def count_chatml_tokens(
         self, messages: Chat, functions: Optional[Sequence[Mapping]] = None
     ) -> int:
         num_tokens = sum(map(self.count_message_tokens, messages))
         num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
         if functions:
             if messages[0]["role"] == "system":
-                num_tokens -= 1  # I believe a newline gets removed somewhere for somereason
+                num_tokens -= (
+                    1  # I believe a newline gets removed somewhere for somereason
+                )
             else:
                 num_tokens += self.tokens_per_message
             num_tokens += self.count_functions_tokens(functions)
         return num_tokens
 
-    def count_message_tokens(self, message: ChatMLMessage | FunctionCallChatMLMessage | FunctionChatMLMessage) -> int:
+    def count_message_tokens(
+        self, message: ChatMLMessage | FunctionCallChatMLMessage | FunctionChatMLMessage
+    ) -> int:
         """https://github.com/openai/openai-python/blob/main/chatml.md"""
         num_tokens = self.tokens_per_message
         if message["role"] == "function":
             num_tokens += (
                 self.count_tokens(message["content"])
                 + self.count_tokens(message["name"])
                 + self.count_tokens(message["role"])
                 - 1  # omission of a delimiter?
             )
         elif "function_call" in message:
             # https://github.com/forestwanglin/openai-java/blob/308a3423d34905bd28aca976fd0f2fa030f9a3a1/jtokkit/src/main/java/xyz/felh/openai/jtokkit/utils/TikTokenUtils.java#L202-L205
             num_tokens += (
                 self.count_tokens(message["function_call"]["name"])
-                + self.count_tokens(message["function_call"]["arguments"])  # TODO: what if there are no arguments?
+                + self.count_tokens(
+                    message["function_call"]["arguments"]
+                )  # TODO: what if there are no arguments?
                 + self.count_tokens(message["role"])
                 + 3  # I believe this is due to delimiter tokens being added
             )
         else:
-            num_tokens += (
-                self.count_tokens(message["content"])
-                + self.count_tokens(message["role"])
+            num_tokens += self.count_tokens(message["content"]) + self.count_tokens(
+                message["role"]
             )
             if "name" in message:
                 num_tokens += self.tokens_per_name + self.count_tokens(message["name"])
         return num_tokens
 
     def count_functions_tokens(self, functions: list[dict]) -> int:
         num_tokens = len(self.encode(self.funcion_header))
```

### Comparing `totokenizers-1.2.4.1/totokenizers/openai_info.py` & `totokenizers-1.2.5/totokenizers/openai_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,148 @@
 """
 https://github.com/Significant-Gravitas/Auto-GPT/blob/3a2d08fb415071cc94dd6fcee24cfbdd1fb487dd/autogpt/llm/base.py#L47
 """
 
-from .model_info import ChatModelInfo, TextModelInfo, EmbeddingModelInfo
-
+from .model_info import ChatModelInfo, EmbeddingModelInfo, TextModelInfo
 
 OPEN_AI_CHAT_MODELS = {
     info.name: info
     for info in [
         ChatModelInfo(
-             completion_token_cost=0.03,
-             cutoff="2023-12-01",
-             max_tokens=128_000,
-             name="gpt-4-turbo-2024-04-09",
-             prompt_token_cost=0.01,
-             supports_functions=True,
-         ),
+            completion_token_cost=0.015,
+            cutoff="2023-10-01",
+            feature_flags=["functions", "tools", "json", "vision", "voice"],
+            max_output_tokens=128_000,
+            max_tokens=128_000,
+            name="gpt-4o-2024-05-13",
+            prompt_token_cost=0.005,
+        ),
         ChatModelInfo(
             completion_token_cost=0.03,
-            cutoff="2023-04-01",
-            max_tokens=128000,
-            name="gpt-4-0125-preview",
+            cutoff="2023-12-01",
+            feature_flags=["functions", "tools", "json", "vision"],
+            max_output_tokens=128_000,
+            max_tokens=128_000,
+            name="gpt-4-turbo-2024-04-09",
             prompt_token_cost=0.01,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.03,
-            cutoff="2023-04-01",
-            max_tokens=128000,
-            name="gpt-4-turbo-preview",
+            cutoff="2023-12-01",
+            feature_flags=["functions", "tools", "json"],
+            max_output_tokens=4096,
+            max_tokens=128_000,
+            name="gpt-4-0125-preview",
             prompt_token_cost=0.01,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.03,
             cutoff="2023-04-01",
-            max_tokens=128000,
+            feature_flags=["functions", "tools", "json"],
+            max_output_tokens=4096,
+            max_tokens=128_000,
             name="gpt-4-1106-preview",
             prompt_token_cost=0.01,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.03,
             cutoff="2023-04-01",
+            feature_flags=["functions", "tools", "json", "vision"],
+            max_output_tokens=4096,
             max_tokens=128000,
             name="gpt-4-1106-vision-preview",
             prompt_token_cost=0.01,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.0015,
             cutoff="2021-09-01",
-            max_tokens=16385,
+            feature_flags=["functions", "tools", "json"],
+            max_output_tokens=4096,
+            max_tokens=16_385,
             name="gpt-3.5-turbo-0125",
             prompt_token_cost=0.0005,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.002,
             cutoff="2021-11-01",
-            max_tokens=16385,
+            feature_flags=["functions", "tools", "json"],
+            max_output_tokens=4096,
+            max_tokens=16_385,
             name="gpt-3.5-turbo-1106",
             prompt_token_cost=0.001,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.002,
             cutoff="2021-11-01",
+            deprecated=True,
+            max_output_tokens=4096,
             max_tokens=4096,
             name="gpt-3.5-turbo-0301",
             prompt_token_cost=0.0015,
         ),
         ChatModelInfo(
             completion_token_cost=0.002,
             cutoff="2021-11-01",
+            deprecated=True,
+            feature_flags=["functions"],
+            max_output_tokens=4096,
             max_tokens=4096,
             name="gpt-3.5-turbo-0613",
             prompt_token_cost=0.0015,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.004,
             cutoff="2021-11-01",
+            deprecated=True,
+            feature_flags=["functions"],
+            max_output_tokens=16385,
             max_tokens=16385,
             name="gpt-3.5-turbo-16k-0613",
             prompt_token_cost=0.003,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.06,
             cutoff="2021-11-01",
+            deprecated=True,
+            max_output_tokens=8192,
             max_tokens=8192,
             name="gpt-4-0314",
             prompt_token_cost=0.03,
         ),
         ChatModelInfo(
             completion_token_cost=0.06,
             cutoff="2021-11-01",
+            deprecated=True,
+            feature_flags=["functions"],
+            max_output_tokens=8192,
             max_tokens=8192,
             name="gpt-4-0613",
             prompt_token_cost=0.03,
-            supports_functions=True,
         ),
         ChatModelInfo(
             completion_token_cost=0.12,
             cutoff="2021-11-01",
+            deprecated=True,
+            max_output_tokens=32768,
             max_tokens=32768,
             name="gpt-4-32k-0314",
             prompt_token_cost=0.06,
         ),
         ChatModelInfo(
             completion_token_cost=0.12,
             cutoff="2021-11-01",
             max_tokens=32768,
+            max_output_tokens=32768,
             name="gpt-4-32k-0613",
             prompt_token_cost=0.06,
-            supports_functions=True,
+            feature_flags=["functions"],
         ),
     ]
 }
 
-# Set aliases for rolling model IDs
-chat_model_mapping = {
-    "gpt-3.5-turbo": "gpt-3.5-turbo-0613",
-    "gpt-3.5-turbo-16k": "gpt-3.5-turbo-16k-0613",
-    "gpt-4": "gpt-4-0613",
-    "gpt-4-turbo": "gpt-4-turbo-2024-04-09",
-    "gpt-4-32k": "gpt-4-32k-0613",
-}
-for alias, target in chat_model_mapping.items():
-    alias_info = ChatModelInfo(**OPEN_AI_CHAT_MODELS[target].__dict__)
-    alias_info.name = alias
-    OPEN_AI_CHAT_MODELS[alias] = alias_info
-
 OPEN_AI_TEXT_MODELS = {
     info.name: info
     for info in [
         TextModelInfo(
             completion_token_cost=0.02,
             cutoff="2021-11-01",
             max_tokens=4096,
@@ -154,19 +160,36 @@
 }
 
 OPEN_AI_EMBEDDING_MODELS = {
     info.name: info
     for info in [
         EmbeddingModelInfo(
             cutoff="2021-11-01",
-            embedding_dimensions=1536,
+            default_dim=1536,
+            supported_dim=[1536],
             max_tokens=8191,
             name="text-embedding-ada-002",
             prompt_token_cost=0.0001,
         ),
+        EmbeddingModelInfo(
+            cutoff="2021-11-01",
+            default_dim=3072,
+            supported_dim=[256, 1024, 3072],
+            max_tokens=8191,
+            name="text-embedding-3-large",
+            prompt_token_cost=0.00013,
+        ),
+        EmbeddingModelInfo(
+            cutoff="2021-11-01",
+            default_dim=1536,
+            supported_dim=[512, 1536],
+            max_tokens=8191,
+            name="text-embedding-3-small",
+            prompt_token_cost=0.00002,
+        ),
     ]
 }
 
 OPEN_AI_MODELS: dict[str, ChatModelInfo | EmbeddingModelInfo | TextModelInfo] = {
     **OPEN_AI_CHAT_MODELS,
     **OPEN_AI_TEXT_MODELS,
     **OPEN_AI_EMBEDDING_MODELS,
```

### Comparing `totokenizers-1.2.4.1/totokenizers/protocols.py` & `totokenizers-1.2.5/totokenizers/protocols.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers/schemas.py` & `totokenizers-1.2.5/totokenizers/schemas.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.4.1/totokenizers.egg-info/PKG-INFO` & `totokenizers-1.2.5/totokenizers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: totokenizers
-Version: 1.2.4.1
+Version: 1.2.5
 Summary: Text tokenizers.
 Home-page: https://github.com/TeiaLabs/totokenizers
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Requires-Dist: google-cloud-aiplatform
 Requires-Dist: tiktoken
-Requires-Dist: tokenizers
+Requires-Dist: tokenizers>=0.7.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # totokenizers
 
 A model-agnostic library to encode text into tokens and couting them using different tokenizers.
```

### Comparing `totokenizers-1.2.4.1/totokenizers.egg-info/SOURCES.txt` & `totokenizers-1.2.5/totokenizers.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 tests/test_anthropic.py
 tests/test_code.py
 tests/test_jsonschema_formatter.py
+tests/test_openai.py
 totokenizers/__init__.py
 totokenizers/errors.py
 totokenizers/factories.py
 totokenizers/jsonschema_formatter.py
 totokenizers/model_info.py
 totokenizers/openai.py
 totokenizers/openai_info.py
@@ -18,10 +19,12 @@
 totokenizers.egg-info/requires.txt
 totokenizers.egg-info/top_level.txt
 totokenizers.egg-info/zip-safe
 totokenizers/anthropic/__init__.py
 totokenizers/anthropic/anthropic.py
 totokenizers/anthropic/info.py
 totokenizers/anthropic/tokenizer.json
+totokenizers/google/__init__.py
+totokenizers/google/google.py
 totokenizers/mockai/__init__.py
 totokenizers/mockai/info.py
 totokenizers/mockai/tokenizer.py
```

