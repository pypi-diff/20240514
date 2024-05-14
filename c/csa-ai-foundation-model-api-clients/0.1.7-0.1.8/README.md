# Comparing `tmp/csa_ai_foundation_model_api_clients-0.1.7.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.1.8.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.1.7.tar` & `csa_ai_foundation_model_api_clients-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/TODO.md
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/manual-package-update.md
--rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/output-example.json
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     7683 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     2710 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2197 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     1851 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-chatgpt-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-gemini-the-capital-of-france.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/LICENSE
--rwxr-xr-x   0        0        0     2221 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/README.md
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/TODO.md
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/manual-package-update.md
+-rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/output-example.json
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     7683 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     1792 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     1740 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     1721 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/LICENSE
+-rwxr-xr-x   0        0        0     2221 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/README.md
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/TODO.md` & `csa_ai_foundation_model_api_clients-0.1.8/TODO.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/output-example.json` & `csa_ai_foundation_model_api_clients-0.1.8/output-example.json`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from csa_ai_foundation_model_api_clients.ai_client import claude, chatgpt, gemini
 
 class FoundationModelAPIClient:
     def __init__(self, *, model, api_key=None, system_prompt, system_prompt_type, user_prompt, user_prompt_type, user_data=None, user_data_type, output_file=None, temperature=None, max_tokens=None):
         #
         # Increment this when updating the model
         #
-        self.csa_ai_foundation_model_api_clients_version = "0.1.7"
+        self.csa_ai_foundation_model_api_clients_version = "0.1.8"
         self.model = model
         self.api_key = api_key or self.get_model_api_key()
         self.model_name = self.get_model_mapping()
         self.system_prompt = system_prompt
         self.system_prompt_type = system_prompt_type
         self.user_prompt = user_prompt
         self.user_prompt_type = user_prompt_type
@@ -61,15 +61,15 @@
         self.system_prompt_absolute_path = os.path.abspath(system_prompt)
         self.user_prompt_absolute_path = os.path.abspath(user_prompt)
         self.user_data_absolute_path = os.path.abspath(user_data)
         self.output_file_absolute_path = os.path.abspath(output_file)
 
         output_data = {
             "dataType": "csa-ai-foundation-model-api-clients-JSON-output",
-            "dataVersion": "0.1",
+            "dataVersion": "0.2",
             "csa-ai-foundation-model-api-clients-version": self.csa_ai_foundation_model_api_clients_version,
             "arguments": {
                 "model": self.model_name,
                 "system_prompt": self.system_prompt,
                 "user_prompt": self.user_prompt,
                 "user_data_file": self.user_data,
                 "system_prompt_absolute": self.system_prompt_absolute_path,
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,58 @@
 #!/usr/bin/env python3
 
 import openai
 import datetime
 
 def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
-    TIME_START = datetime.datetime.now().isoformat()
+    TIME_START = datetime.datetime.now()
 
     openai.api_key = api_key
 
     temperature = kwargs.get('temperature', 1)
     max_tokens = kwargs.get('max_tokens', 4096)
 
     completion = openai.chat.completions.create(
         model=model_name,
         temperature=temperature,
         max_tokens=max_tokens,
+        #
+        # Set interactive=false
+        #
+        interactive="false",
         messages=[
             {"role": "system", "content": system_prompt},
             {"role": "user", "content": user_prompt}
         ]
     )
 
-    TIME_FINISHED = datetime.datetime.now().isoformat()
-
-    time_start = datetime.datetime.fromisoformat(TIME_START)
-    time_complete = datetime.datetime.fromisoformat(TIME_FINISHED)
-
-    duration = time_complete - time_start
+    TIME_FINISHED = datetime.datetime.now()
+    duration = TIME_START - TIME_FINISHED
     TIME_TO_RUN = duration.total_seconds()
 
     try:
         tokens_input = completion.usage.prompt_tokens
         tokens_output = completion.usage.completion_tokens
         total_tokens = completion.usage.total_tokens
     except AttributeError:
         tokens_input = tokens_output = total_tokens = None
     
-    serialized_completion = {
-        "id": getattr(completion, 'id', None),
-        "model": getattr(completion, 'model', None),
-        "created": getattr(completion, 'created', None),
-        "system_fingerprint": getattr(completion, 'system_fingerprint', None),
-        "choices": [
-            {
-                "finish_reason": choice.finish_reason,
-                "index": choice.index,
-                "message": {
-                    "content": getattr(choice.message, 'content', None),
-                    "role": getattr(choice.message, 'role', None)
-                }
-            } for choice in getattr(completion, 'choices', [])
-        ] if hasattr(completion, 'choices') else [],
-        "usage": {
-            "prompt_tokens": tokens_input,
-            "completion_tokens": tokens_output,
-            "total_tokens": total_tokens
-        }
-    }
-    
     try:
         response_message = completion.choices[0].message.content
         status = "success"
     except AttributeError:
         response_message = None
         status = "error"
 
     api_response = {
         "status": "success",
         "model_name": model_name,
         "temperature": temperature,
-        "ai_query_time": TIME_START,
-        "ai_response_time": TIME_FINISHED,
+        "ai_query_time": TIME_START.isoformat(),
+        "ai_response_time": TIME_FINISHED.isoformat(),
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": tokens_input,
         "tokens_output": tokens_output,
         "tokens_total": total_tokens,
         "ai_response_http_status_code": None,
         "ai_response_stop_reason": None,
         "ai_response_data": response_message
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import anthropic
 import datetime
 
 def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
-    TIME_START = datetime.datetime.now().isoformat()
+    TIME_START = datetime.datetime.now()
 
     client = anthropic.Anthropic(api_key=api_key)
 
     temperature = kwargs.get('temperature', 1)
     max_tokens = kwargs.get('max_tokens', 4096)
 
     completion = client.messages.create(
@@ -17,56 +17,41 @@
         max_tokens=max_tokens,
         system=system_prompt,
         messages=[
             {"role": "user", "content": user_prompt}
         ],
     )
 
-    TIME_FINISHED = datetime.datetime.now().isoformat()
-
-    time_start = datetime.datetime.fromisoformat(TIME_START)
-    time_complete = datetime.datetime.fromisoformat(TIME_FINISHED)
-
-    duration = time_complete - time_start
+    TIME_FINISHED = datetime.datetime.now()
+    duration = TIME_START - TIME_FINISHED
     TIME_TO_RUN = duration.total_seconds()
 
     try:
         tokens_input = completion.usage.input_tokens
         tokens_output = completion.usage.output_tokens
         total_tokens = completion.usage.input_tokens + completion.usage.output_tokens
     except AttributeError:
         tokens_input = tokens_output = total_tokens = None
     
-    serialized_completion = {
-        "id": getattr(completion, 'id', None),
-        "model": getattr(completion, 'model', None),
-        "stop_reason": completion.stop_reason,
-        "usage": {
-            "prompt_tokens": tokens_input,
-            "completion_tokens": tokens_output,
-            "total_tokens": total_tokens
-        }
-    }
-
     try:
         response_message = completion.content[0].text
         status = "success"
     except AttributeError:
         response_message = None
         status = "error"
 
     api_response = {
         "status": status,
         "model_name": model_name,
         "temperature": temperature,
-        "ai_query_time": TIME_START,
-        "ai_response_time": TIME_FINISHED,
+        "ai_query_time": TIME_START.isoformat(),
+        "ai_response_time": TIME_FINISHED.isoformat(),
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": tokens_input,
         "tokens_output": tokens_output,
         "tokens_total": total_tokens,
         "ai_response_http_status_code": None,
-        "ai_response_stop_reason": None,
+        "ai_response_stop_reason": completion.stop_reason,
         "ai_response_data": response_message
     }
 
     return api_response
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import google.generativeai as genai
 from google.generativeai import types
 import datetime
 
 def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
-    TIME_START = datetime.datetime.now().isoformat()
+    TIME_START = datetime.datetime.now()
 
     genai.configure(api_key=api_key)
 
     gemini_model = genai.GenerativeModel(
         model_name=model_name,
         system_instruction=system_prompt
         )
@@ -21,20 +21,16 @@
         candidate_count=1,
         max_output_tokens=max_tokens,
         temperature=temperature
     )
 
     response = gemini_model.generate_content(user_prompt, generation_config=config)
 
-    TIME_FINISHED = datetime.datetime.now().isoformat()
-
-    time_start = datetime.datetime.fromisoformat(TIME_START)
-    time_complete = datetime.datetime.fromisoformat(TIME_FINISHED)
-
-    duration = time_complete - time_start
+    TIME_FINISHED = datetime.datetime.now()
+    duration = TIME_START - TIME_FINISHED
     TIME_TO_RUN = duration.total_seconds()
 
     try:
         response_message = response.text
         status = "success"
     except AttributeError:
         response_message = None
@@ -44,16 +40,16 @@
     # response = model.count_tokens(prompt)
     # print(f"Prompt Token Count: {response.total_tokens}")
 
     api_response = {
         "status": "success",
         "model_name": model_name,
         "temperature": temperature,
-        "ai_query_time": TIME_START,
-        "ai_response_time": TIME_FINISHED,
+        "ai_query_time": TIME_START.isoformat(),
+        "ai_response_time": TIME_FINISHED.isoformat(),
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": None,
         "tokens_output": None,
         "tokens_total": None,
         "ai_response_http_status_code": None,
         "ai_response_stop_reason": None,
         "ai_response_data": response_message
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-chatgpt-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-chatgpt-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-claude-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-claude-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/tests/dev/ask-gemini-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-gemini-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/.gitignore` & `csa_ai_foundation_model_api_clients-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/LICENSE` & `csa_ai_foundation_model_api_clients-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/README.md` & `csa_ai_foundation_model_api_clients-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.7/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

