# Comparing `tmp/py-ai-cli-0.5.1.tar.gz` & `tmp/py-ai-cli-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ai-cli-0.5.1.tar", last modified: Thu Feb 22 13:51:22 2024, max compression
+gzip compressed data, was "py-ai-cli-0.5.3.tar", last modified: Tue May 14 05:34:36 2024, max compression
```

## Comparing `py-ai-cli-0.5.1.tar` & `py-ai-cli-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2280 2024-02-22 13:51:01.010938 py-ai-cli-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1092 2024-02-22 13:51:01.010938 py-ai-cli-0.5.1/LICENSE
--rw-r--r--   0        0        0     4027 2024-02-22 13:51:01.010938 py-ai-cli-0.5.1/README.md
--rw-r--r--   0        0        0     4504 2024-02-22 13:51:01.010938 py-ai-cli-0.5.1/README_ja.md
--rw-r--r--   0        0        0     3270 2024-02-22 13:51:01.010938 py-ai-cli-0.5.1/README_zh.md
--rw-r--r--   0        0        0     2078 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      995 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/__init__.py
--rw-r--r--   0        0        0     8759 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/bot/__init__.py
--rw-r--r--   0        0        0     1099 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/bot/bard.py
--rw-r--r--   0        0        0     3126 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/bot/bing.py
--rw-r--r--   0        0        0     2266 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/bot/gemini.py
--rw-r--r--   0        0        0      195 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/bot/token.py
--rwxr-xr-x   0        0        0    13293 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/cli.py
--rw-r--r--   0        0        0     5567 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/git.py
--rw-r--r--   0        0        0     4820 2024-02-22 13:51:01.322939 py-ai-cli-0.5.1/src/ai_cli/setting.py
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 py-ai-cli-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2488 2024-05-14 05:34:12.662739 py-ai-cli-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1092 2024-05-14 05:34:12.662739 py-ai-cli-0.5.3/LICENSE
+-rw-r--r--   0        0        0     4027 2024-05-14 05:34:12.662739 py-ai-cli-0.5.3/README.md
+-rw-r--r--   0        0        0     4504 2024-05-14 05:34:12.662739 py-ai-cli-0.5.3/README_ja.md
+-rw-r--r--   0        0        0     3270 2024-05-14 05:34:12.662739 py-ai-cli-0.5.3/README_zh.md
+-rw-r--r--   0        0        0     2078 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      995 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/__init__.py
+-rw-r--r--   0        0        0     8759 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/bot/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/bot/bard.py
+-rw-r--r--   0        0        0     3126 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/bot/bing.py
+-rw-r--r--   0        0        0     2302 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/bot/gemini.py
+-rw-r--r--   0        0        0      195 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/bot/token.py
+-rwxr-xr-x   0        0        0    13293 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/cli.py
+-rw-r--r--   0        0        0     5567 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/git.py
+-rw-r--r--   0        0        0     4807 2024-05-14 05:34:12.982739 py-ai-cli-0.5.3/src/ai_cli/setting.py
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 py-ai-cli-0.5.3/PKG-INFO
```

### Comparing `py-ai-cli-0.5.1/CHANGELOG.md` & `py-ai-cli-0.5.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Release v0.5.3
+---------------------------
+
+- feat: support gpt-4o, and default to it
+
+Release v0.5.2
+---------------------------
+
+- feat: support Gemini 1.5 pro, use `gemini-1.5-pro-latest` to switch to it
+
 Release v0.5.0
 ---------------------------
 
 - feat: now support Google Gemini Model. You can use `ai setting --edit bot=GeminiBot` to switch to it
 
 Release v0.4.0
 ---------------------------
```

### Comparing `py-ai-cli-0.5.1/LICENSE` & `py-ai-cli-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/README.md` & `py-ai-cli-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/README_ja.md` & `py-ai-cli-0.5.3/README_ja.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/README_zh.md` & `py-ai-cli-0.5.3/README_zh.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/pyproject.toml` & `py-ai-cli-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -96,21 +96,21 @@
 ]
 dependencies = [
     "rich>=13.3.1",
     "openai>=1.10.0",
     "pysocks>=1.7.1",
     "pyperclip>=1.8.2",
     "EdgeGPT>=0.1.22.1",
-    "tiktoken>=0.5.1",
+    "tiktoken>=0.7.0",
     "BardApi>=0.1.38",
     "google-generativeai>=0.3.2",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
-version = "0.5.1"
+version = "0.5.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/yufeikang/ai-cli"
 Documentation = "https://github.com/yufeikang/ai-cli/blob/main/README.md"
```

### Comparing `py-ai-cli-0.5.1/src/ai_cli/__init__.py` & `py-ai-cli-0.5.3/src/ai_cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.1"
+__version__ = "0.5.3"
 
 import logging
 import re
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 
 HOME = Path.home()
```

### Comparing `py-ai-cli-0.5.1/src/ai_cli/bot/__init__.py` & `py-ai-cli-0.5.3/src/ai_cli/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/src/ai_cli/bot/bard.py` & `py-ai-cli-0.5.3/src/ai_cli/bot/bard.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/src/ai_cli/bot/bing.py` & `py-ai-cli-0.5.3/src/ai_cli/bot/bing.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/src/ai_cli/bot/gemini.py` & `py-ai-cli-0.5.3/src/ai_cli/bot/gemini.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 class GeminiBot(Bot):
     def __init__(self, setting: Setting, args, **kwargs):
         super().__init__(setting, args, **kwargs)
         logger.info(f"Init GeminiBot with setting: {setting}")
         api_key = setting.google_api_key.get_value() or os.environ.get("GOOGLE_API_KEY")
         genai.configure(api_key=api_key)
-        self.model = args.model or setting.model.get_value() or "gemini-pro"
+        self.model = args.model or setting.model.get_value() or "gemini-1.5-pro-latest"
         if self.model not in self.available_models:
             raise ValueError(f"Model {self.model} is not supported. Supported models: {self.available_models}")
         self.bot: GenerativeModel = genai.GenerativeModel(model_name=self.model)
 
     @property
     def available_models(self):
-        return ["gemini-1.0-pro", "gemini-pro"]
+        return ["gemini-1.5-pro-latest", "gemini-1.0-pro", "gemini-pro"]
 
     def get_messages(self):
         prompt_added = False
         for m in self.history:
             parts = []
             if prompt_added is False and self.prompt:
                 parts.append(self.prompt)
```

### Comparing `py-ai-cli-0.5.1/src/ai_cli/cli.py` & `py-ai-cli-0.5.3/src/ai_cli/cli.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/src/ai_cli/git.py` & `py-ai-cli-0.5.3/src/ai_cli/git.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.5.1/src/ai_cli/setting.py` & `py-ai-cli-0.5.3/src/ai_cli/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     )
     google_api_key = SettingField(
         "Google API Key", description="You can get it from https://aistudio.google.com/app/apikey"
     )
     endpoint = SettingField("OpenAI API Endpoint", description="default is https://api.openai.com")
     model = SettingField(
         "Model",
-        default="gpt-4-turbo-preview",
+        default="gpt-4o",
         description="default is openai model, if you use other LLM, please change it",
     )
     no_stream = SettingField("Disable stream mode", default=False, type=bool)
     bot = SettingField("Bot Type", default="GPTBot", description="Supported: GPTBot, BingBot, BardBot, GeminiBot")
     raw = SettingField("Raw mode", default=False, type=bool, description="no render content by rich")
     log_level = SettingField("Log level", default="INFO")
     debug = SettingField("Debug mode", default=False, type=bool)
```

### Comparing `py-ai-cli-0.5.1/PKG-INFO` & `py-ai-cli-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ai_cli
-Version: 0.5.1
+Version: 0.5.3
 Summary: This CLI tool allows you to easily chat with chatGPT in the command line. You can chat with it, ask questions, and even translate text. It also
 License: MIT
 Author-email: Yufei Kang <kou.uhi.x@gmail.com>
 Requires-Python: >=3.9
 Project-URL: Documentation, https://github.com/yufeikang/ai-cli/blob/main/README.md
 Project-URL: Repository, https://github.com/yufeikang/ai-cli
 Description-Content-Type: text/markdown
```

