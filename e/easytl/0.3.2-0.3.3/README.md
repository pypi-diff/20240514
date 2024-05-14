# Comparing `tmp/easytl-0.3.2.tar.gz` & `tmp/easytl-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.3.2.tar", last modified: Mon May 13 19:49:27 2024, max compression
+gzip compressed data, was "easytl-0.3.3.tar", last modified: Tue May 14 00:05:39 2024, max compression
```

## Comparing `easytl-0.3.2.tar` & `easytl-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.461073 easytl-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.461073 easytl-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-13 19:47:59.000000 easytl-0.3.2/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-13 19:47:59.000000 easytl-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-13 19:47:59.000000 easytl-0.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-13 19:49:27.465074 easytl-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-13 19:47:59.000000 easytl-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-13 19:47:59.000000 easytl-0.3.2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 19:47:59.000000 easytl-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:49:27.465074 easytl-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.461073 easytl-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    71506 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/googletl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    26492 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-13 19:47:59.000000 easytl-0.3.2/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-13 19:47:59.000000 easytl-0.3.2/tests/passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.431685 easytl-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.423685 easytl-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.427685 easytl-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-14 00:04:12.000000 easytl-0.3.3/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-14 00:04:12.000000 easytl-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 00:04:12.000000 easytl-0.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-14 00:05:39.431685 easytl-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-14 00:04:12.000000 easytl-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-14 00:04:12.000000 easytl-0.3.3/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 00:04:12.000000 easytl-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 00:05:39.431685 easytl-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.423685 easytl-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.427685 easytl-0.3.3/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16049 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/anthropic_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71506 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27077 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.431685 easytl-0.3.3/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.427685 easytl-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-14 00:04:12.000000 easytl-0.3.3/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-14 00:04:12.000000 easytl-0.3.3/tests/passing.py
```

### Comparing `easytl-0.3.2/.github/workflows/workflow.yml` & `easytl-0.3.3/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/.gitignore` & `easytl-0.3.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -162,7 +162,8 @@
 
 ## test files
 tests/gemini.txt
 tests/openai.txt
 tests/deepl.txt
 tests/easytl-log.txt
 tests/google_translate_key.json
+tests/anthropic.txt
```

### Comparing `easytl-0.3.2/LICENSE.md` & `easytl-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/PKG-INFO` & `easytl-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.2
+Version: 0.3.3
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.1
+Requires-Dist: google-generativeai==0.5.3
 Requires-Dist: deepl==1.16.1
-Requires-Dist: openai==1.13.3
+Requires-Dist: openai==1.29.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: google-cloud-translate==3.15.3
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
```

### Comparing `easytl-0.3.2/README.md` & `easytl-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/SECURITY.md` & `easytl-0.3.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/pyproject.toml` & `easytl-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     "tomli"
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [
-    "google-generativeai==0.5.1",
+    "google-generativeai==0.5.3",
     "deepl==1.16.1",
-    "openai==1.13.3",
+    "openai==1.29.0",
     "backoff==2.2.1",
     "tiktoken==0.6.0",
     "google-cloud-translate==3.15.3"
 ]
 
 name = "easytl"
-version = "v0.3.2"
+version = "v0.3.3"
 authors = [
   { name="Bikatr7", email="Bikatr7@proton.me" },
 ]
 description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `easytl-0.3.2/src/easytl/__init__.py` & `easytl-0.3.3/src/easytl/__init__.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/src/easytl/decorators.py` & `easytl-0.3.3/src/easytl/decorators.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/src/easytl/deepl_service.py` & `easytl-0.3.3/src/easytl/deepl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/src/easytl/easytl.py` & `easytl-0.3.3/src/easytl/easytl.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/src/easytl/exceptions.py` & `easytl-0.3.3/src/easytl/exceptions.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/src/easytl/gemini_service.py` & `easytl-0.3.3/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/src/easytl/googletl_service.py` & `easytl-0.3.3/src/easytl/googletl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/src/easytl/openai_service.py` & `easytl-0.3.3/src/easytl/openai_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ##-------------------start-of-set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _set_api_key(api_key:str) -> None:
 
         """
 
-        Sets the API key for the OpenAI client.
+        Sets the API key for the OpenAI clients.
 
         Parameters:
         api_key (string) : The API key to set.
 
         """
 
         OpenAIService._async_client.api_key = api_key
@@ -350,35 +350,21 @@
             _validity = True
 
             return _validity, None
 
         except Exception as _e:
 
             return _validity, _e
-        
-##-------------------start-of-get_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _get_decorator() -> typing.Union[typing.Callable, None]:
-
-        """
-
-        Returns the decorator to use for the OpenAI service.
 
-        Returns:
-        decorator (callable) : The decorator to use.
-
-        """
-
-        return OpenAIService._decorator_to_use
-    
 ##-------------------start-of-_calculate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
-    def _calculate_cost(text:str | typing.Iterable, translation_instructions:str | None, model:str | None) -> typing.Tuple[int, float, str]:
+    def _calculate_cost(text:str | ModelTranslationMessage | SystemTranslationMessage | typing.Iterable, 
+                        translation_instructions:str | None, 
+                        model:str | None) -> typing.Tuple[int, float, str]:
 
         """
 
         Calculates the cost of the translation.
 
         Parameters:
         text (string | iterable) : The text to translate.
```

### Comparing `easytl-0.3.2/src/easytl/util.py` & `easytl-0.3.3/src/easytl/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
 ##-------------------start-of-_return_curated_gemini_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _validate_stop_sequences(stop_sequences:typing.List[str] | None) -> None:
 
     assert stop_sequences is None or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), InvalidEasyTLSettingsException("Invalid stop sequences. Must be a string or a list of strings.")
 
-
 ##-------------------start-of-_string_to_bool()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _string_to_bool(string:str) -> bool:
 
     return string.lower() in ['true', '1', 'yes', 'y', 't']
 
 ##-------------------start-of-_convert_iterable_to_str()-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
@@ -519,14 +518,26 @@
     "gemini-1.5-pro-latest",
   ##  "gemini-1.0-ultra-latest",
     "gemini-pro",
     "gemini-pro-vision",
   ##  "gemini-ultra"
 ]
 
+ALLOWED_ANTHROPIC_MODELS = [
+    "claude-3-opus-20240229",
+    "claude-3-sonnet-20240229",
+    "claude-3-haiku-20240307"
+]
+
+VALID_JSON_ANTHROPIC_MODELS = [
+    "claude-3-opus-20240229",
+    "claude-3-sonnet-20240229",
+    "claude-3-haiku-20240307"
+]
+
 ## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-05-13
 MODEL_COSTS = {
     # Grouping GPT-3.5 models together
     "gpt-3.5-turbo-0125": {"price_case": 7, "_input_cost": 0.0005, "_output_cost": 0.0015},
     "gpt-3.5-turbo-0301": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-0613": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-1106": {"price_case": 2, "_input_cost": 0.0010, "_output_cost": 0.0020},
@@ -553,8 +564,14 @@
     "gemini-1.0-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.0-pro-vision-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.5-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
  ##   "gemini-1.0-ultra-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-pro": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-pro-vision": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
  ##   "gemini-ultra": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0}
+
+    ## grouping anthropic models together
+    "claude-3-haiku-20240307": {"price_case": 11, "_input_cost": 0.00025, "_output_cost": 0.00125},
+    "claude-3-sonnet-20240229": {"price_case": 12, "_input_cost": 0.003, "_output_cost": 0.015},
+    "claude-3-opus-20240229": {"price_case": 13, "_input_cost": 0.015, "_output_cost": 0.075}
+
 }
```

### Comparing `easytl-0.3.2/src/easytl.egg-info/PKG-INFO` & `easytl-0.3.3/src/easytl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.2
+Version: 0.3.3
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.1
+Requires-Dist: google-generativeai==0.5.3
 Requires-Dist: deepl==1.16.1
-Requires-Dist: openai==1.13.3
+Requires-Dist: openai==1.29.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: google-cloud-translate==3.15.3
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
```

### Comparing `easytl-0.3.2/src/easytl.egg-info/SOURCES.txt` & `easytl-0.3.3/src/easytl.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 LICENSE.md
 README.md
 SECURITY.md
 pyproject.toml
 .github/workflows/workflow.yml
 src/easytl/__init__.py
+src/easytl/anthropic_service.py
 src/easytl/classes.py
 src/easytl/decorators.py
 src/easytl/deepl_service.py
 src/easytl/easytl.py
 src/easytl/exceptions.py
 src/easytl/gemini_service.py
 src/easytl/googletl_service.py
```

### Comparing `easytl-0.3.2/tests/issue_template.py` & `easytl-0.3.3/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.2/tests/passing.py` & `easytl-0.3.3/tests/passing.py`

 * *Files identical despite different names*

