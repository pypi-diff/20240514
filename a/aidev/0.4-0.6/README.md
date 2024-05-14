# Comparing `tmp/aidev-0.4.tar.gz` & `tmp/aidev-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidev-0.4.tar", last modified: Mon May  8 07:09:47 2023, max compression
+gzip compressed data, was "aidev-0.6.tar", last modified: Tue May 14 18:22:26 2024, max compression
```

## Comparing `aidev-0.4.tar` & `aidev-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-05-08 07:09:47.022100 aidev-0.4/
--rw-r--r--   0 voidful    (501) staff       (20)      128 2023-05-08 07:09:47.021953 aidev-0.4/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)     4546 2023-05-08 05:26:48.000000 aidev-0.4/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-05-08 07:09:47.020904 aidev-0.4/aidev/
--rw-r--r--   0 voidful    (501) staff       (20)       23 2023-04-06 19:53:32.000000 aidev-0.4/aidev/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)     1869 2023-04-07 07:38:13.000000 aidev-0.4/aidev/config_manager.py
--rw-r--r--   0 voidful    (501) staff       (20)      472 2023-05-08 04:54:48.000000 aidev-0.4/aidev/config_utils.py
--rw-r--r--   0 voidful    (501) staff       (20)     6513 2023-05-08 06:12:19.000000 aidev-0.4/aidev/helpers.py
--rw-r--r--   0 voidful    (501) staff       (20)     4093 2023-05-08 05:57:55.000000 aidev-0.4/aidev/main.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-05-08 07:09:47.021766 aidev-0.4/aidev.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)      128 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      289 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)       88 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/entry_points.txt
--rw-r--r--   0 voidful    (501) staff       (20)       23 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        6 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/top_level.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-05-08 07:09:47.022157 aidev-0.4/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)      367 2023-05-08 07:09:44.000000 aidev-0.4/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-05-14 18:22:26.703661 aidev-0.6/
+-rw-r--r--   0 voidful    (501) staff       (20)       47 2024-05-14 18:22:26.703503 aidev-0.6/PKG-INFO
+-rw-------   0 voidful    (501) staff       (20)     4546 2023-05-08 05:26:48.000000 aidev-0.6/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-05-14 18:22:26.701672 aidev-0.6/aidev/
+-rw-------   0 voidful    (501) staff       (20)       23 2023-04-06 19:53:32.000000 aidev-0.6/aidev/__init__.py
+-rw-------   0 voidful    (501) staff       (20)     1869 2023-04-07 07:38:13.000000 aidev-0.6/aidev/config_manager.py
+-rw-------   0 voidful    (501) staff       (20)      472 2023-05-08 04:54:48.000000 aidev-0.6/aidev/config_utils.py
+-rw-------   0 voidful    (501) staff       (20)     6335 2024-05-14 18:19:11.000000 aidev-0.6/aidev/helpers.py
+-rw-------   0 voidful    (501) staff       (20)     4144 2023-08-01 23:27:14.000000 aidev-0.6/aidev/main.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-05-14 18:22:26.703269 aidev-0.6/aidev.egg-info/
+-rw-------   0 voidful    (501) staff       (20)       47 2024-05-14 18:22:24.000000 aidev-0.6/aidev.egg-info/PKG-INFO
+-rw-------   0 voidful    (501) staff       (20)      289 2024-05-14 18:22:26.000000 aidev-0.6/aidev.egg-info/SOURCES.txt
+-rw-------   0 voidful    (501) staff       (20)        1 2024-05-14 18:22:25.000000 aidev-0.6/aidev.egg-info/dependency_links.txt
+-rw-------   0 voidful    (501) staff       (20)       87 2024-05-14 18:22:25.000000 aidev-0.6/aidev.egg-info/entry_points.txt
+-rw-------   0 voidful    (501) staff       (20)       23 2024-05-14 18:22:25.000000 aidev-0.6/aidev.egg-info/requires.txt
+-rw-------   0 voidful    (501) staff       (20)        6 2024-05-14 18:22:25.000000 aidev-0.6/aidev.egg-info/top_level.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2024-05-14 18:22:26.703718 aidev-0.6/setup.cfg
+-rw-------   0 voidful    (501) staff       (20)      367 2024-05-14 18:19:11.000000 aidev-0.6/setup.py
```

### Comparing `aidev-0.4/README.md` & `aidev-0.6/README.md`

 * *Files identical despite different names*

### Comparing `aidev-0.4/aidev/config_manager.py` & `aidev-0.6/aidev/config_manager.py`

 * *Files identical despite different names*

### Comparing `aidev-0.4/aidev/helpers.py` & `aidev-0.6/aidev/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,23 +83,17 @@
         print(f"Warning: Code change is too extensive ({len(code)} characters) for AI to handle. \n"
               f"Please consider breaking your changes into smaller commits to less than {max_input_length} characters.")
         return False
     return True
 
 
 def get_ai_response(code: str, response_type: ResponseType, threshold: float, engine: str, language: str = "english",
-                    max_tokens: int = 300) -> str:
-    max_input_lengths = {
-        "gpt-3.5-turbo": 3796,
-        "gpt-4": 7892,
-        "gpt-4-32k": 32468,
-    }
-    max_input_length = max_input_lengths.get(engine, 3000)
+                    max_tokens: int = 8000) -> str:
 
-    if not input_length_validation(code, max_input_length):
+    if not input_length_validation(code, max_tokens):
         return ""
 
     prompt_template = build_prompt_template(response_type)
     prompt = prompt_template.format(code=code)
     response_queue = queue.Queue()
     api_call = threading.Thread(target=call_openai_api,
                                 args=(prompt, engine, threshold, language, max_tokens, response_queue))
```

### Comparing `aidev-0.4/aidev/main.py` & `aidev-0.6/aidev/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from bullet import Bullet
 
 from aidev.helpers import get_git_diff, get_ai_run_result, get_code_execution_test_detail, get_code_improvement_detail, \
     get_unit_tests_detail
 from .config_utils import read_config, store_config
 
 config = read_config() or {}
-detected_language = locale.getdefaultlocale()[0][:2]
+detected_language = 'en' if locale.getdefaultlocale()[0] is None else locale.getdefaultlocale()[0][:2]
 
 
 @click.command()
 @click.option('--threshold', default=config.get('threshold', 0.3), type=float,
               help='Confidence threshold for the AI generated result (0.0 to 1.0).')
 @click.option('--engine', default=config.get('engine', 'gpt-3.5-turbo'),
               help='The GPT engine to use (e.g., "gpt-3.5-turbo", "gpt-4", "gpt-4-32k").')
@@ -85,8 +85,8 @@
         elif action == "Give detailed Code Improvement":
             response_text = "Code Improvement\n"
             response_text += get_code_improvement_detail(diff, threshold, engine, language, max_tokens)
         elif action == "Create a unit test for this change":
             response_text = "Unit Test\n"
             response_text += get_unit_tests_detail(diff, threshold, engine, language, max_tokens)
         elif action == "Exit":
-            break
+            break
```

