# Comparing `tmp/csa_ai_foundation_model_api_clients-0.1.6.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.1.7.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.1.6.tar` & `csa_ai_foundation_model_api_clients-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/TODO.md
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/manual-package-update.md
--rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/output-example.json
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     7052 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3412 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2900 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     2353 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/tests/dev/ask-chatgpt-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/tests/dev/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/tests/dev/ask-gemini-the-capital-of-france.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/LICENSE
--rwxr-xr-x   0        0        0     2065 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/README.md
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/TODO.md
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/manual-package-update.md
+-rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/output-example.json
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     7683 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     2710 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2197 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     1851 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/LICENSE
+-rwxr-xr-x   0        0        0     2221 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/README.md
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/TODO.md` & `csa_ai_foundation_model_api_clients-0.1.7/TODO.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/output-example.json` & `csa_ai_foundation_model_api_clients-0.1.7/output-example.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7821969696969697%*

 * *Differences: {"'api_response'": "{'ai_response_time': '2024-05-11T12:34:56Z', 'ai_runtime': '1', 'model_name': "*

 * *                   "'full model name', 'temperature': 'temperature'}",*

 * * "'arguments'": "{'system_prompt_absolute': '/foo/filename.txt', 'user_prompt_absolute': "*

 * *                "'/foo/other.txt', 'user_data_file_absolute': '/foo/data.txt', "*

 * *                "'output_file_absolute': '/foo/foo.json'}",*

 * * 'delete': "['api_parameters']"}*

```diff
@@ -1,34 +1,32 @@
 {
-    "api_parameters": {
-        "data_prompt": "More data goes here",
-        "max_tokens": 150,
-        "model_name": "claude",
-        "system_prompt": "Please provide an overview of the JSON schema requirements.",
-        "temperature": 0.7,
-        "user_prompt": "I need a schema for an AI API that includes meta data and arguments."
-    },
     "api_response": {
         "ai_query_time": "2024-05-11T12:34:56Z",
         "ai_response_data": "some large string here",
         "ai_response_http_status_code": "200",
         "ai_response_stop_reason": "end_turn",
-        "ai_response_time": "2024-05-11T12:35:15Z",
-        "ai_runtime": 288,
+        "ai_response_time": "2024-05-11T12:34:56Z",
+        "ai_runtime": "1",
+        "model_name": "full model name",
         "status": "success|error",
+        "temperature": "temperature",
         "tokens_input": 123,
         "tokens_output": 123,
         "tokens_total": 246
     },
     "arguments": {
         "max_tokens": 150,
         "model": "claude",
         "output_file": "foo.json",
+        "output_file_absolute": "/foo/foo.json",
         "system_prompt": "filename.txt",
+        "system_prompt_absolute": "/foo/filename.txt",
         "temperature": 0.7,
         "user_data_file": "data.txt",
-        "user_prompt": "other.txt"
+        "user_data_file_absolute": "/foo/data.txt",
+        "user_prompt": "other.txt",
+        "user_prompt_absolute": "/foo/other.txt"
     },
     "csa-ai-foundation-model-api-clients-version": "0.0.9",
     "dataType": "csa-ai-foundation-model-api-clients-JSON-output",
     "dataVersion": "1.0"
 }
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from csa_ai_foundation_model_api_clients.ai_client import claude, chatgpt, gemini
 
 class FoundationModelAPIClient:
     def __init__(self, *, model, api_key=None, system_prompt, system_prompt_type, user_prompt, user_prompt_type, user_data=None, user_data_type, output_file=None, temperature=None, max_tokens=None):
         #
         # Increment this when updating the model
         #
-        self.csa_ai_foundation_model_api_clients_version = "0.1.6"
+        self.csa_ai_foundation_model_api_clients_version = "0.1.7"
         self.model = model
         self.api_key = api_key or self.get_model_api_key()
         self.model_name = self.get_model_mapping()
         self.system_prompt = system_prompt
         self.system_prompt_type = system_prompt_type
         self.user_prompt = user_prompt
         self.user_prompt_type = user_prompt_type
@@ -54,26 +54,36 @@
             self.user_prompt_final_data = f"{self.user_prompt_data}\n{self.user_data_data}"
 
         else:   
             self.user_prompt_final_data = self.user_prompt_data
 
         self.api_response = self.generate_response()
 
+        self.system_prompt_absolute_path = os.path.abspath(system_prompt)
+        self.user_prompt_absolute_path = os.path.abspath(user_prompt)
+        self.user_data_absolute_path = os.path.abspath(user_data)
+        self.output_file_absolute_path = os.path.abspath(output_file)
+
         output_data = {
             "dataType": "csa-ai-foundation-model-api-clients-JSON-output",
             "dataVersion": "0.1",
             "csa-ai-foundation-model-api-clients-version": self.csa_ai_foundation_model_api_clients_version,
             "arguments": {
                 "model": self.model_name,
                 "system_prompt": self.system_prompt,
                 "user_prompt": self.user_prompt,
                 "user_data_file": self.user_data,
+                "system_prompt_absolute": self.system_prompt_absolute_path,
+                "user_prompt_absolute": self.user_prompt_absolute_path,
+                "user_data_file_absolute": self.user_data_absolute_path,
+                # TODO: add optional _data for each file
                 "temperature": self.temperature,
                 "max_tokens": self.max_tokens,
-                "output_file": self.output_file
+                "output_file": self.output_file,
+                "output_file_absolute": self.output_file_absolute_path
             },
             "api_response": self.api_response
         }
 
         if self.output_file is not None:
             with open(self.output_file, 'w', encoding='utf-8') as file:
                 json.dump(output_data, file, sort_keys=True, indent=2)
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,43 +61,23 @@
     try:
         response_message = completion.choices[0].message.content
         status = "success"
     except AttributeError:
         response_message = None
         status = "error"
 
-    ai_output = {
-        "$id": "csa-ai-toolkit-openai-chatgpt4-JSON-v1_00",
-        "metadata": {
-            "system": system_prompt,
-            "user-prompt": user_prompt,
-            "user-data": kwargs.get('user_data'),
-            "output": kwargs.get('output_file'),                        
-            "model_name": model_name,
-            "temperature": temperature,
-            "max_tokens": max_tokens,
-            "tokens_input": tokens_input,
-            "tokens_output": tokens_output,
-            "tokens_total": total_tokens,
-            "time_start": TIME_START,
-            "time_complete": TIME_FINISHED,
-            "time_to_run": TIME_TO_RUN
-        },
-        "extracted_data": response_message,
-        "completion": serialized_completion
-    }
-
     api_response = {
         "status": "success",
+        "model_name": model_name,
+        "temperature": temperature,
         "ai_query_time": TIME_START,
         "ai_response_time": TIME_FINISHED,
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": tokens_input,
         "tokens_output": tokens_output,
         "tokens_total": total_tokens,
         "ai_response_http_status_code": None,
         "ai_response_stop_reason": None,
         "ai_response_data": response_message
     }
 
-
     return api_response
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,37 +50,18 @@
     try:
         response_message = completion.content[0].text
         status = "success"
     except AttributeError:
         response_message = None
         status = "error"
 
-    ai_output = {
-        "$id": "csa-ai-toolkit-anthropic-claude3-JSON-v1_00",
-        "metadata": {
-            "system": system_prompt,
-            "user-prompt": user_prompt,
-            "user-data": kwargs.get('user_data'),
-            "output": kwargs.get('output_file'),                        
-            "model_name": model_name,
-            "temperature": temperature,
-            "max_tokens": max_tokens,
-            "tokens_input": tokens_input,
-            "tokens_output": tokens_output,
-            "tokens_total": total_tokens,
-            "time_start": TIME_START,
-            "time_complete": TIME_FINISHED,
-            "time_to_run": TIME_TO_RUN
-        },
-        "extracted_data": response_message,
-        "completion": serialized_completion
-    }
-
     api_response = {
         "status": status,
+        "model_name": model_name,
+        "temperature": temperature,
         "ai_query_time": TIME_START,
         "ai_response_time": TIME_FINISHED,
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": tokens_input,
         "tokens_output": tokens_output,
         "tokens_total": total_tokens,
         "ai_response_http_status_code": None,
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,33 +40,18 @@
         response_message = None
         status = "error"
 
     # https://cloud.google.com/vertex-ai/generative-ai/docs/multimodal/get-token-count
     # response = model.count_tokens(prompt)
     # print(f"Prompt Token Count: {response.total_tokens}")
 
-    ai_output = {
-        "$id": "csa-ai-toolkit-google-gemini1.5-JSON-v1_00",
-        "metadata": {
-            "system": system_prompt,
-            "user-prompt": user_prompt,
-            "user-data": kwargs.get('user_data'),
-            "output": kwargs.get('output_file'),
-            "model_name": model_name,
-            "temperature": temperature,
-            "max_tokens": max_tokens,
-            "time_start": TIME_START,
-            "time_complete": TIME_FINISHED,
-            "time_to_run": TIME_TO_RUN
-        },
-        "extracted_data": response.text
-    }
-
     api_response = {
         "status": "success",
+        "model_name": model_name,
+        "temperature": temperature,
         "ai_query_time": TIME_START,
         "ai_response_time": TIME_FINISHED,
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": None,
         "tokens_output": None,
         "tokens_total": None,
         "ai_response_http_status_code": None,
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/tests/dev/ask-chatgpt-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-chatgpt-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/tests/dev/ask-claude-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-claude-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/tests/dev/ask-gemini-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-gemini-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/.gitignore` & `csa_ai_foundation_model_api_clients-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/LICENSE` & `csa_ai_foundation_model_api_clients-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/README.md` & `csa_ai_foundation_model_api_clients-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Cloud Security Alliance AI Foundation Model API Clients
 
+You can get this library at https://pypi.org/project/csa-ai-foundation-model-api-clients/ or via:
+
+```
+pip install csa-ai-foundation-model-api-clients
+```
+
 This Python library (csa_ai_foundation_model_api_clients) provides API access to text completions for:
 
 * Anthropic Claude 3
 * Google Gemini 1.5
 * OpenAI ChatGPT 4
 
 and has plans to add:
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.6/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,20 @@
 Requires-Dist: anthropic
 Requires-Dist: google-generativeai
 Requires-Dist: openai
 Description-Content-Type: text/markdown
 
 # Cloud Security Alliance AI Foundation Model API Clients
 
+You can get this library at https://pypi.org/project/csa-ai-foundation-model-api-clients/ or via:
+
+```
+pip install csa-ai-foundation-model-api-clients
+```
+
 This Python library (csa_ai_foundation_model_api_clients) provides API access to text completions for:
 
 * Anthropic Claude 3
 * Google Gemini 1.5
 * OpenAI ChatGPT 4
 
 and has plans to add:
```

