# Comparing `tmp/openai_messages_token_helper-0.1.3.tar.gz` & `tmp/openai_messages_token_helper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_messages_token_helper-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai_messages_token_helper-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai_messages_token_helper-0.1.3.tar` & `openai_messages_token_helper-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      967 2024-05-02 12:35:21.311203 openai_messages_token_helper-0.1.3/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.1.3/.gitignore
--rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      536 2024-05-02 08:43:27.099990 openai_messages_token_helper-0.1.3/.vscode/launch.json
--rw-r--r--   0        0        0      323 2024-05-02 10:25:36.179140 openai_messages_token_helper-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0     1729 2024-05-02 12:23:13.095942 openai_messages_token_helper-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.1.3/LICENSE
--rw-r--r--   0        0        0     4643 2024-05-02 12:16:45.685649 openai_messages_token_helper-0.1.3/README.md
--rw-r--r--   0        0        0     1326 2024-05-02 12:23:22.903393 openai_messages_token_helper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      360 2024-05-02 08:43:27.109262 openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/__init__.py
--rw-r--r--   0        0        0     2423 2024-05-02 08:43:27.112777 openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/function_format.py
--rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/images_helper.py
--rw-r--r--   0        0        0     6263 2024-05-02 12:33:28.812340 openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/message_builder.py
--rw-r--r--   0        0        0     6512 2024-05-02 12:24:05.718823 openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/model_helper.py
--rw-r--r--   0        0        0        0 2024-05-02 10:25:36.189581 openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/py.typed
--rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0    16187 2024-05-02 08:43:27.120583 openai_messages_token_helper-0.1.3/tests/functions.py
--rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.1.3/tests/image_large.png
--rw-r--r--   0        0        0     4034 2024-05-02 08:43:27.123570 openai_messages_token_helper-0.1.3/tests/messages.py
--rw-r--r--   0        0        0     1105 2024-04-26 13:30:53.397027 openai_messages_token_helper-0.1.3/tests/test_imageshelper.py
--rw-r--r--   0        0        0    10270 2024-05-02 12:32:00.881634 openai_messages_token_helper-0.1.3/tests/test_messagebuilder.py
--rw-r--r--   0        0        0     3499 2024-05-02 08:43:27.130210 openai_messages_token_helper-0.1.3/tests/test_modelhelper.py
--rw-r--r--   0        0        0     2136 2024-05-02 10:25:36.191012 openai_messages_token_helper-0.1.3/tests/verify_functions.py
--rw-r--r--   0        0        0     2043 2024-05-02 10:25:36.191752 openai_messages_token_helper-0.1.3/tests/verify_openai.py
--rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      967 2024-05-14 04:30:21.625566 openai_messages_token_helper-0.1.4/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.1.4/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      536 2024-05-02 08:43:27.099990 openai_messages_token_helper-0.1.4/.vscode/launch.json
+-rw-r--r--   0        0        0      323 2024-05-02 10:25:36.179140 openai_messages_token_helper-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1826 2024-05-14 05:05:28.239842 openai_messages_token_helper-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4643 2024-05-14 04:30:21.631270 openai_messages_token_helper-0.1.4/README.md
+-rw-r--r--   0        0        0     1326 2024-05-14 05:04:35.230033 openai_messages_token_helper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      360 2024-05-02 08:43:27.109262 openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-02 08:43:27.112777 openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/function_format.py
+-rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/images_helper.py
+-rw-r--r--   0        0        0     6263 2024-05-14 04:30:21.635839 openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/message_builder.py
+-rw-r--r--   0        0        0     6534 2024-05-14 04:31:26.900275 openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/model_helper.py
+-rw-r--r--   0        0        0        0 2024-05-14 04:30:21.637865 openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/py.typed
+-rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0    16187 2024-05-02 08:43:27.120583 openai_messages_token_helper-0.1.4/tests/functions.py
+-rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.1.4/tests/image_large.png
+-rw-r--r--   0        0        0     4342 2024-05-14 04:53:02.689096 openai_messages_token_helper-0.1.4/tests/messages.py
+-rw-r--r--   0        0        0     1105 2024-04-26 13:30:53.397027 openai_messages_token_helper-0.1.4/tests/test_imageshelper.py
+-rw-r--r--   0        0        0    10270 2024-05-14 04:30:21.640830 openai_messages_token_helper-0.1.4/tests/test_messagebuilder.py
+-rw-r--r--   0        0        0     3795 2024-05-14 05:11:47.680012 openai_messages_token_helper-0.1.4/tests/test_modelhelper.py
+-rw-r--r--   0        0        0     2136 2024-05-02 10:25:36.191012 openai_messages_token_helper-0.1.4/tests/verify_functions.py
+-rw-r--r--   0        0        0     2198 2024-05-14 05:07:41.488127 openai_messages_token_helper-0.1.4/tests/verify_openai.py
+-rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.1.4/PKG-INFO
```

### Comparing `openai_messages_token_helper-0.1.3/.github/workflows/python.yaml` & `openai_messages_token_helper-0.1.4/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/.gitignore` & `openai_messages_token_helper-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/.vscode/launch.json` & `openai_messages_token_helper-0.1.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/CHANGELOG.md` & `openai_messages_token_helper-0.1.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.1.4] - May 14, 2024
+
+- Add support and tests for gpt-4o, which has a different tokenizer.
+
 ## [0.1.3] - May 2, 2024
 
 - Use openai type annotations for more precise type hints, and add a typing test.
 
 ## [0.1.2] - May 2, 2024
 
 - Add `py.typed` file so that mypy can find the type hints in this package.
```

### Comparing `openai_messages_token_helper-0.1.3/LICENSE` & `openai_messages_token_helper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/README.md` & `openai_messages_token_helper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/pyproject.toml` & `openai_messages_token_helper-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "openai-messages-token-helper"
 description = "A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API."
-version = "0.1.3"
+version = "0.1.4"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "openai",
     "tiktoken",
```

### Comparing `openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/function_format.py` & `openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/function_format.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/images_helper.py` & `openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/images_helper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/message_builder.py` & `openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/message_builder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/src/openai_messages_token_helper/model_helper.py` & `openai_messages_token_helper-0.1.4/src/openai_messages_token_helper/model_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "gpt-35-turbo": 4000,
     "gpt-3.5-turbo": 4000,
     "gpt-35-turbo-16k": 16000,
     "gpt-3.5-turbo-16k": 16000,
     "gpt-4": 8100,
     "gpt-4-32k": 32000,
     "gpt-4v": 128000,
+    "gpt-4o": 128000,
 }
 
 
 AOAI_2_OAI = {"gpt-35-turbo": "gpt-3.5-turbo", "gpt-35-turbo-16k": "gpt-3.5-turbo-16k", "gpt-4v": "gpt-4-turbo-vision"}
 
 logger = logging.getLogger("openai_messages_token_helper")
```

### Comparing `openai_messages_token_helper-0.1.3/tests/functions.py` & `openai_messages_token_helper-0.1.4/tests/functions.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/tests/image_large.png` & `openai_messages_token_helper-0.1.4/tests/image_large.png`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/tests/messages.py` & `openai_messages_token_helper-0.1.4/tests/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,122 @@
 system_message_short = {
     "message": {
         "role": "system",
         "content": "You are a bot.",
     },
     "count": 12,
+    "count_omni": 12,
 }
 
 system_message = {
     "message": {
         "role": "system",
         "content": "You are a helpful, pattern-following assistant that translates corporate jargon into plain English.",
     },
     "count": 25,
+    "count_omni": 24,
 }
 
 system_message_long = {
     "message": {
         "role": "system",
         "content": "Assistant helps the company employees with their healthcare plan questions, and questions about the employee handbook. Be brief in your answers.",
     },
     "count": 31,
+    "count_omni": 31,
 }
 
 system_message_unicode = {
     "message": {
         "role": "system",
         "content": "á",
     },
     "count": 8,
+    "count_omni": 8,
 }
 
 system_message_with_name = {
     "message": {
         "role": "system",
         "name": "example_user",
         "content": "New synergies will help drive top-line growth.",
     },
     "count": 20,  # Less tokens in older vision preview models
+    "count_omni": 20,
 }
 
 user_message = {
     "message": {
         "role": "user",
         "content": "Hello, how are you?",
     },
     "count": 13,
+    "count_omni": 13,
 }
 
 user_message_unicode = {
     "message": {
         "role": "user",
         "content": "á",
     },
     "count": 8,
+    "count_omni": 8,
 }
 
 user_message_perf = {
     "message": {
         "role": "user",
         "content": "What happens in a performance review?",
     },
     "count": 14,
+    "count_omni": 14,
 }
 
 assistant_message_perf = {
     "message": {
         "role": "assistant",
         "content": "During the performance review at Contoso Electronics, the supervisor will discuss the employee's performance over the past year and provide feedback on areas for improvement. They will also provide an opportunity for the employee to discuss their goals and objectives for the upcoming year. The review is a two-way dialogue between managers and employees, and employees will receive a written summary of their performance review which will include a rating of their performance, feedback, and goals and objectives for the upcoming year [employee_handbook-3.pdf].",
     },
     "count": 106,
+    "count_omni": 106,
 }
 
 assistant_message_perf_short = {
     "message": {
         "role": "assistant",
         "content": "The supervisor will discuss the employee's performance and provide feedback on areas for improvement. They will also provide an opportunity for the employee to discuss their goals and objectives for the upcoming year. The review is a two-way dialogue between managers and employees, and employees will receive a written summary of their performance review which will include a rating of their performance, feedback, and goals for the upcoming year [employee_handbook-3.pdf].",
     },
     "count": 91,
+    "count_omni": 91,
 }
 
 user_message_dresscode = {
     "message": {
         "role": "user",
         "content": "Is there a dress code?",
     },
     "count": 13,
+    "count_omni": 13,
 }
 
 assistant_message_dresscode = {
     "message": {
         "role": "assistant",
         "content": "Yes, there is a dress code at Contoso Electronics. Look sharp! [employee_handbook-1.pdf]",
     },
     "count": 30,
+    "count_omni": 30,
 }
 user_message_pm = {
     "message": {
         "role": "user",
         "content": "What does a Product Manager do?",
     },
     "count": 14,
+    "count_omni": 14,
 }
 text_and_image_message = {
     "message": {
         "role": "user",
         "content": [
             {"type": "text", "text": "Describe this picture:"},
             {
@@ -112,14 +125,15 @@
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mP8z/C/HgAGgwJ/lK3Q6wAAAABJRU5ErkJggg==",
                     "detail": "auto",
                 },
             },
         ],
     },
     "count": 266,
+    "count_omni": 266,
 }
 
 MESSAGE_COUNTS = [
     system_message,
     system_message_short,
     system_message_long,
     system_message_unicode,
```

### Comparing `openai_messages_token_helper-0.1.3/tests/test_imageshelper.py` & `openai_messages_token_helper-0.1.4/tests/test_imageshelper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/tests/test_messagebuilder.py` & `openai_messages_token_helper-0.1.4/tests/test_messagebuilder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/tests/test_modelhelper.py` & `openai_messages_token_helper-0.1.4/tests/test_modelhelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def test_get_token_limit():
     assert get_token_limit("gpt-35-turbo") == 4000
     assert get_token_limit("gpt-3.5-turbo") == 4000
     assert get_token_limit("gpt-35-turbo-16k") == 16000
     assert get_token_limit("gpt-3.5-turbo-16k") == 16000
     assert get_token_limit("gpt-4") == 8100
     assert get_token_limit("gpt-4-32k") == 32000
+    assert get_token_limit("gpt-4o") == 128000
 
 
 def test_get_token_limit_error():
     with pytest.raises(ValueError, match="Called with unknown model name: gpt-3"):
         get_token_limit("gpt-3")
 
 
@@ -23,40 +24,47 @@
     with caplog.at_level("WARNING"):
         assert get_token_limit("gpt-3", default_to_minimum=True) == 4000
         assert "Model gpt-3 not found, defaulting to minimum token limit 4000" in caplog.text
 
 
 # parameterize the model and the expected number of tokens
 @pytest.mark.parametrize(
-    "model",
+    "model, count_key",
     [
-        "gpt-35-turbo",
-        "gpt-3.5-turbo",
-        "gpt-35-turbo-16k",
-        "gpt-3.5-turbo-16k",
-        "gpt-4",
-        "gpt-4-32k",
-        "gpt-4v",
+        ("gpt-35-turbo", "count"),
+        ("gpt-3.5-turbo", "count"),
+        ("gpt-35-turbo-16k", "count"),
+        ("gpt-3.5-turbo-16k", "count"),
+        ("gpt-4", "count"),
+        ("gpt-4-32k", "count"),
+        ("gpt-4v", "count"),
+        ("gpt-4o", "count_omni"),
     ],
 )
 @pytest.mark.parametrize(
     "message",
     [
         user_message,
         system_message,
         system_message_with_name,
     ],
 )
-def test_count_tokens_for_message(model: str, message: dict):
-    assert count_tokens_for_message(model, message["message"]) == message["count"]
+def test_count_tokens_for_message(model, count_key, message):
+    assert count_tokens_for_message(model, message["message"]) == message[count_key]
 
 
-def test_count_tokens_for_message_list():
-    model = "gpt-4"
-    assert count_tokens_for_message(model, text_and_image_message["message"]) == text_and_image_message["count"]
+@pytest.mark.parametrize(
+    "model, count_key",
+    [
+        ("gpt-4", "count"),
+        ("gpt-4o", "count_omni"),
+    ],
+)
+def test_count_tokens_for_message_list(model, count_key):
+    assert count_tokens_for_message(model, text_and_image_message["message"]) == text_and_image_message[count_key]
 
 
 def test_count_tokens_for_message_error():
     message = {
         "role": "user",
         "content": {"key": "value"},
     }
```

### Comparing `openai_messages_token_helper-0.1.3/tests/verify_functions.py` & `openai_messages_token_helper-0.1.4/tests/verify_functions.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.3/tests/verify_openai.py` & `openai_messages_token_helper-0.1.4/tests/verify_openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,23 @@
     if (openai_model := os.getenv("OPENAI_MODEL")) is None:
         raise ValueError("Missing OpenAI model")
     client = openai.OpenAI(api_key=openai_key)
     MODEL_NAME = openai_model
 
 # Test the token count for each message
 for message_count_pair in MESSAGE_COUNTS:
-    response = client.chat.completions.create(
-        model=MODEL_NAME,
-        temperature=0.7,
-        n=1,
-        messages=[message_count_pair["message"]],  # type: ignore[list-item]
-    )
+    for model, expected_tokens in [
+        (MODEL_NAME, message_count_pair["count"]),
+        ("gpt-4o", message_count_pair["count_omni"]),
+    ]:
+        response = client.chat.completions.create(
+            model=model,
+            temperature=0.7,
+            n=1,
+            messages=[message_count_pair["message"]],  # type: ignore[list-item]
+        )
 
-    print(message_count_pair["message"])
-    expected_tokens = message_count_pair["count"]
-    assert response.usage is not None, "Expected usage to be present"
-    assert (
-        response.usage.prompt_tokens == expected_tokens
-    ), f"Expected {expected_tokens} tokens, got {response.usage.prompt_tokens}"
+        print(message_count_pair["message"])
+        assert response.usage is not None, "Expected usage to be present"
+        assert (
+            response.usage.prompt_tokens == expected_tokens
+        ), f"Expected {expected_tokens} tokens, got {response.usage.prompt_tokens} for model {model}"
```

### Comparing `openai_messages_token_helper-0.1.3/PKG-INFO` & `openai_messages_token_helper-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-messages-token-helper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API.
 Author: Pamela Fox
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

