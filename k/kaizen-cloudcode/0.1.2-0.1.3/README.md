# Comparing `tmp/kaizen_cloudcode-0.1.2.tar.gz` & `tmp/kaizen_cloudcode-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.2.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.1.3.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.2.tar` & `kaizen_cloudcode-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-05-13 11:50:49.061935 kaizen_cloudcode-0.1.2/LICENSE
--rw-r--r--   0        0        0     4135 2024-05-13 11:50:49.061935 kaizen_cloudcode-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     3075 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1467 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/general.py
--rw-r--r--   0        0        0     3631 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7183 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     1900 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     2969 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1386 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     1677 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/utils/config.py
--rw-r--r--   0        0        0      776 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4135 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3449 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1463 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     3631 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7183 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     2217 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     3395 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     1528 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/utils/config.py
+-rw-r--r--   0        0        0      776 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.3/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.2/LICENSE` & `kaizen_cloudcode-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.2/README.md` & `kaizen_cloudcode-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.2/kaizen/generator/ui.py` & `kaizen_cloudcode-0.1.3/kaizen/generator/ui.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,35 +21,37 @@
         folder_path: Optional[str] = "",
     ):
         """
         This method generates UI tests with cypress code for a given web URL.
         """
         web_content = self.extract_webpage(web_url)
         test_modules = self.identify_modules(web_content)
-        ui_tests = self.generate_module_tests(web_content, test_modules, web_url)
+        ui_tests, usage = self.generate_module_tests(
+            web_content, test_modules["modules"], web_url
+        )
         self.store_tests_files(ui_tests, folder_path)
-
-        return ui_tests
+        total_usage = self.provider.update_usage(usage, test_modules["usage"])
+        return ui_tests, total_usage
 
     def extract_webpage(self, web_url: str):
         """
         This method extracts the code for a given web URL.
         """
 
         html = output.get_web_html(web_url)
         return html
 
     def identify_modules(self, web_content: str, user: Optional[str] = None):
         """
         This method identifies the different UI modules from a webpage.
         """
         prompt = UI_MODULES_PROMPT.format(WEB_CONTENT=web_content)
-        resp = self.provider.chat_completion(prompt, user=user)
+        resp, usage = self.provider.chat_completion(prompt, user=user)
         modules = parser.extract_multi_json(resp)
-        return modules
+        return {"modules": modules, "usage": usage}
 
     def generate_playwright_code(
         self,
         web_content: str,
         test_description: str,
         web_url: str,
         user: Optional[str] = None,
@@ -57,36 +59,40 @@
         """
         This method generates playwright code for a particular UI test.
         """
         prompt = PLAYWRIGHT_CODE_PROMPT.format(
             WEB_CONTENT=web_content, TEST_DESCRIPTION=test_description, URL=web_url
         )
 
-        resp = self.provider.chat_completion(prompt, user=user)
+        resp, usage = self.provider.chat_completion(prompt, user=user)
 
-        return resp
+        return {"code": resp, "usage": usage}
 
     def generate_module_tests(self, web_content: str, test_modules: dict, web_url: str):
         """
         This method generates UI testing points for all modules.
         """
         ui_tests = test_modules
+        total_usage = None
         for module in ui_tests:
             for test in module["tests"]:
                 test_description = test["test_description"]
                 playwright_code = self.generate_playwright_code(
                     web_content, test_description, web_url
                 )
-                test["code"] = playwright_code
+                test["code"] = playwright_code["code"]
                 test["status"] = "Not run"
+                total_usage = self.provider.update_usage(
+                    total_usage, playwright_code["usage"]
+                )
 
-        return ui_tests
+        return ui_tests, total_usage
 
     def store_tests_files(self, json_tests: list, folder_path: str = ""):
-        
+
         if not folder_path:
             folder_path = output.get_parent_folder()
 
         folder_path = os.path.join(folder_path, ".kaizen/tests")
         output.create_folder(folder_path)
         output.create_test_files(json_tests, folder_path)
```

### Comparing `kaizen_cloudcode-0.1.2/kaizen/helpers/general.py` & `kaizen_cloudcode-0.1.3/kaizen/helpers/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 
 
 def run_test(code):
 
     # TODO: Update logic for pytest runner
-    
+
     pass
 
 
 def clean_python_code(code):
     match = re.search(r"```(?:python)?\n(.*)\n```", code, re.DOTALL)
     if match:
         return match.group(1)
```

### Comparing `kaizen_cloudcode-0.1.2/kaizen/helpers/output.py` & `kaizen_cloudcode-0.1.3/kaizen/helpers/output.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.2/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.1.3/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.2/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.1.3/kaizen/llms/prompts.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.2/kaizen/llms/provider.py` & `kaizen_cloudcode-0.1.3/kaizen/llms/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         response = litellm.completion(
             model=self.model,
             messages=messages,
             max_tokens=self.max_tokens,
             temperature=self.temperature,
             user=user,
         )
-        return response["choices"][0]["message"]["content"]
+        return response["choices"][0]["message"]["content"], response["usage"]
 
     def is_inside_token_limit(self, PROMPT, percentage=0.7):
         messages = [{"user": "role", "content": PROMPT}]
         if (
             litellm.token_counter(model=self.model, messages=messages)
             > litellm.get_max_tokens(self.model) * percentage
         ):
@@ -52,7 +52,16 @@
     def available_tokens(self, message, percentage=0.8):
         return litellm.get_max_tokens(self.model) * percentage - litellm.token_counter(
             self.model, message
         )
 
     def get_token_count(self, message):
         return litellm.token_counter(self.model, message)
+
+    def update_usage(self, total_usage, current_usage):
+        if total_usage is not None:
+            total_usage = {
+                key: total_usage[key] + current_usage[key] for key in total_usage
+            }
+        else:
+            total_usage = current_usage
+        return total_usage
```

### Comparing `kaizen_cloudcode-0.1.2/kaizen/reviewer/code_review.py` & `kaizen_cloudcode-0.1.3/kaizen/reviewer/code_review.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,40 +26,43 @@
 
         # If diff_text is smaller than 70% of model token
         prompt = CODE_REVIEW_PROMPT.format(
             PULL_REQUEST_TITLE=pull_request_title,
             PULL_REQUEST_DESC=pull_request_desc,
             CODE_DIFF=diff_text,
         )
-
+        total_usage = None
         if self.provider.is_inside_token_limit(PROMPT=prompt):
             self.logger.debug("Processing Directly from Diff")
-            resp = self.provider.chat_completion(prompt, user=user)
+            resp, usage = self.provider.chat_completion(prompt, user=user)
             review_json = parser.extract_json(resp)
             reviews = review_json["review"]
+            total_usage = self.provider.update_usage(total_usage, usage)
         else:
             self.logger.debug("Processing Based on files")
             # We recurrsively get feedback for files and then get basic summary
             reviews = []
             for file in pull_request_files:
                 patch_details = file["patch"]
                 filename = file["filename"]
                 if filename.split(".")[-1] not in parser.EXCLUDED_FILETYPES:
                     prompt = FILE_CODE_REVIEW_PROMPT.format(
                         PULL_REQUEST_TITLE=pull_request_title,
                         PULL_REQUEST_DESC=pull_request_desc,
                         FILE_PATCH=patch_details,
                     )
-                    resp = self.provider.chat_completion(prompt, user=user)
+                    resp, usage = self.provider.chat_completion(prompt, user=user)
+                    total_usage = self.provider.update_usage(total_usage, usage)
                     review_json = parser.extract_json(resp)
                     reviews.extend(review_json["review"])
         body = output.create_pr_review_from_json(reviews)
         self.logger.debug(f"Generated Review:\n {body}")
         # Share the review on pull request
-        return body
+
+        return {"review": body, "usage": total_usage}
 
     def generate_pull_request_desc(
         self,
         diff_text: str,
         pull_request_title: str,
         pull_request_desc: str,
         user: Optional[str] = None,
@@ -69,13 +72,16 @@
         """
         prompt = PR_DESCRIPTION_PROMPT.format(
             PULL_REQUEST_TITLE=pull_request_title,
             PULL_REQUEST_DESC=pull_request_desc,
             CODE_DIFF=diff_text,
         )
 
-        resp = self.provider.chat_completion(prompt, user=user)
+        # TODO: split the diff if alot of files and contents.
+        resp, usage = self.provider.chat_completion(prompt, user=user)
+        total_usage = None
         self.logger.debug(f"PROMPT Generate PR Desc RESP: {resp}")
         body = output.create_pr_description(
             parser.extract_json(resp), pull_request_desc
         )
-        return body
+        total_usage = self.provider.update_usage(total_usage, usage)
+        return {"desc": body, "usage": total_usage}
```

### Comparing `kaizen_cloudcode-0.1.2/kaizen/utils/config.py` & `kaizen_cloudcode-0.1.3/kaizen/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     if Path(config_file).is_file():
         with open(config_file, "r") as f:
             config_data = json.loads(f.read())
     else:
         config_data = {
             "language_model": {
                 "provider": "litellm",
-                "enable_observability_logging": False
+                "enable_observability_logging": False,
             },
             "github_app": {
                 "check_signature": False,
                 "auto_pr_review": False,
-                "edit_pr_desc": False
-            }
+                "edit_pr_desc": False,
+            },
         }
     return config_data
 
 
 def validate_config_settings(config):
     "Make sure relvant enviorment variables are set"
     if config.get("github_app", {}).get("check_signature", False):
```

### Comparing `kaizen_cloudcode-0.1.2/pyproject.toml` & `kaizen_cloudcode-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.2"
+version = "0.1.3"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
```

### Comparing `kaizen_cloudcode-0.1.2/PKG-INFO` & `kaizen_cloudcode-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.2
+Version: 0.1.3
 Summary: An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly.
 License: Apache2.0
 Author: Saurav Panda
 Author-email: saurav.panda@cloudcode.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.2 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.3 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

