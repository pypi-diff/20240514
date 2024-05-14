# Comparing `tmp/martian_adapters-5.1.0.tar.gz` & `tmp/martian_adapters-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-5.1.0.tar", max compression
+gzip compressed data, was "martian_adapters-5.1.1.tar", max compression
```

## Comparing `martian_adapters-5.1.0.tar` & `martian_adapters-5.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-04-30 00:30:40.565520 martian_adapters-5.1.0/LICENSE
--rw-r--r--   0        0        0     3553 2024-05-07 17:41:03.767019 martian_adapters-5.1.0/README.md
--rw-r--r--   0        0        0      725 2024-04-24 23:08:19.279531 martian_adapters-5.1.0/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-03-12 21:13:48.732102 martian_adapters-5.1.0/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-07 19:47:15.365233 martian_adapters-5.1.0/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     2125 2024-05-08 20:30:10.661406 martian_adapters-5.1.0/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-03-15 23:53:07.585309 martian_adapters-5.1.0/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-04-01 03:49:11.566774 martian_adapters-5.1.0/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2486 2024-05-08 20:30:10.661990 martian_adapters-5.1.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0      523 2024-05-08 20:31:29.074585 martian_adapters-5.1.0/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5893 2024-05-08 20:30:10.662891 martian_adapters-5.1.0/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     6154 2024-05-09 23:13:50.806383 martian_adapters-5.1.0/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-03-12 21:13:48.733334 martian_adapters-5.1.0/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3416 2024-05-08 20:31:29.075074 martian_adapters-5.1.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0     1017 2024-05-07 19:47:15.365833 martian_adapters-5.1.0/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9231 2024-05-08 20:30:10.664702 martian_adapters-5.1.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4102 2024-05-01 00:33:38.184553 martian_adapters-5.1.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2412 2024-05-03 19:59:21.221407 martian_adapters-5.1.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2587 2024-05-03 19:59:21.222405 martian_adapters-5.1.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-05-09 17:04:08.545597 martian_adapters-5.1.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1836 2024-05-03 19:59:21.223228 martian_adapters-5.1.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2985 2024-05-08 20:30:10.665123 martian_adapters-5.1.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-04-25 03:58:20.009986 martian_adapters-5.1.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-04-25 21:01:54.034177 martian_adapters-5.1.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4444 2024-05-01 00:14:43.670186 martian_adapters-5.1.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2450 2024-05-03 19:59:21.223851 martian_adapters-5.1.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2602 2024-05-07 01:28:18.596534 martian_adapters-5.1.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    11047 2024-05-09 23:23:31.640555 martian_adapters-5.1.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2023-11-30 19:57:07.662865 martian_adapters-5.1.0/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-02-06 20:08:59.751016 martian_adapters-5.1.0/adapters/rate_limiter.py
--rw-r--r--   0        0        0      316 2024-05-09 17:04:11.400632 martian_adapters-5.1.0/adapters/requirements.txt
--rw-r--r--   0        0        0     7005 2024-05-09 23:29:02.658037 martian_adapters-5.1.0/adapters/types.py
--rw-r--r--   0        0        0        0 2023-11-09 21:00:33.698900 martian_adapters-5.1.0/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-04-24 23:08:19.285444 martian_adapters-5.1.0/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-03-12 21:13:48.734260 martian_adapters-5.1.0/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-03-08 00:01:49.626651 martian_adapters-5.1.0/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-04-24 23:08:19.285987 martian_adapters-5.1.0/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1147 2024-05-09 23:24:02.263070 martian_adapters-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     4905 1970-01-01 00:00:00.000000 martian_adapters-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/LICENSE
+-rw-r--r--   0        0        0     3553 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/README.md
+-rw-r--r--   0        0        0      725 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     2125 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2486 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0      523 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5893 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     6154 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3416 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0     1017 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9231 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3934 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2412 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2587 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1836 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3196 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1757 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1331 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4444 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2450 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2602 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    11047 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      316 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/requirements.txt
+-rw-r--r--   0        0        0     7005 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1147 2024-05-14 19:42:09.252781 martian_adapters-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 martian_adapters-5.1.1/PKG-INFO
```

### Comparing `martian_adapters-5.1.0/LICENSE` & `martian_adapters-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/README.md` & `martian_adapters-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/__init__.py` & `martian_adapters-5.1.1/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-5.1.1/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-5.1.1/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-5.1.1/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-5.1.1/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-5.1.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-5.1.1/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-5.1.1/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/adapter_factory.py` & `martian_adapters-5.1.1/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-5.1.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/__init__.py` & `martian_adapters-5.1.1/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,20 +109,14 @@
     ),
     AnyscaleModel(
         name="Llama-3-70b-chat-hf",
         cost=Cost(prompt=1.0e-6, completion=1.0e-6),
         context_length=8000,
         vendor_name="meta-llama",
     ),
-    AnyscaleModel(
-        name="gemma-7b-it",
-        cost=Cost(prompt=0.15e-6, completion=0.15e-6),
-        context_length=8192,
-        vendor_name="google",
-    ),
 ]
 
 
 class AnyscaleSDKChatProviderAdapter(ProviderAdapterMixin, OpenAISDKChatAdapter):
     @staticmethod
     def get_supported_models():
         return MODELS
```

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,18 +91,23 @@
         self._async_client.base_url = URL(self._current_model.base_url)
 
     def get_model_name(self) -> str:
         if self._current_model is None:
             raise ValueError("Model not set")
         return self._current_model.name
 
-    # It must be the last response from Lepton that is empty.
     def extract_stream_response(self, request, response: ChatCompletionChunk) -> str:
+        # It must be the last response from Lepton that is empty.
         if not response.choices:
             response.choices = [
                 Choice(
                     delta=ChoiceDelta(),
                     finish_reason="stop",
                     index=0,
                 ),
             ]
+        elif response.choices[0].delta.content is None:
+            # It must be the first response.
+            # Most models start with an empty string.
+            response.choices[0].delta.content = ""
+
         return f"data: {response.model_dump_json()}\n\n"
```

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/rate_limiter.py` & `martian_adapters-5.1.1/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/types.py` & `martian_adapters-5.1.1/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/utils/general_utils.py` & `martian_adapters-5.1.1/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/utils/network_utils.py` & `martian_adapters-5.1.1/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/adapters/utils/openai_client_factory.py` & `martian_adapters-5.1.1/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.0/pyproject.toml` & `martian_adapters-5.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "5.1.0"
+version = "5.1.1"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `martian_adapters-5.1.0/PKG-INFO` & `martian_adapters-5.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 5.1.0
+Version: 5.1.1
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: aiosignal (>=1.3.1,<2.0.0)
 Requires-Dist: anthropic (==0.16.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
```
