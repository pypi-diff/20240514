# Comparing `tmp/edubot-0.7.5.tar.gz` & `tmp/edubot-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edubot-0.7.5.tar", max compression
+gzip compressed data, was "edubot-0.7.6.tar", max compression
```

## Comparing `edubot-0.7.5.tar` & `edubot-0.7.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.7.5/LICENSE
--rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.7.5/README.md
--rw-r--r--   0        0        0     1108 2023-09-02 16:08:01.187468 edubot-0.7.5/edubot/__init__.py
--rw-r--r--   0        0        0    23027 2023-09-21 13:45:03.358509 edubot-0.7.5/edubot/bot.py
--rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.7.5/edubot/sql.py
--rw-r--r--   0        0        0      695 2023-09-02 15:44:13.063018 edubot-0.7.5/edubot/types.py
--rw-r--r--   0        0        0      667 2023-09-21 13:48:55.181553 edubot-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 edubot-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-08 03:58:01.782760 edubot-0.7.6/LICENSE
+-rw-r--r--   0        0        0     1400 2024-03-08 03:58:01.782898 edubot-0.7.6/README.md
+-rw-r--r--   0        0        0     1108 2024-03-08 03:58:01.783742 edubot-0.7.6/edubot/__init__.py
+-rw-r--r--   0        0        0    23030 2024-05-14 07:48:51.873499 edubot-0.7.6/edubot/bot.py
+-rw-r--r--   0        0        0     2950 2024-03-08 03:58:01.784082 edubot-0.7.6/edubot/sql.py
+-rw-r--r--   0        0        0      695 2024-03-08 03:58:01.784170 edubot-0.7.6/edubot/types.py
+-rw-r--r--   0        0        0      686 2024-05-14 07:54:54.551710 edubot-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 edubot-0.7.6/PKG-INFO
```

### Comparing `edubot-0.7.5/LICENSE` & `edubot-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edubot-0.7.5/README.md` & `edubot-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `edubot-0.7.5/edubot/__init__.py` & `edubot-0.7.6/edubot/__init__.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.5/edubot/bot.py` & `edubot-0.7.6/edubot/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 from stability_sdk.utils import generation
 
 from edubot import DREAMSTUDIO_KEY, REPLICATE_KEY
 from edubot.sql import Bot, Completion, Message, Session, Thread
 from edubot.types import CompletionInfo, ImageInfo, MessageInfo
 
 # The limit for GPT-4 is 8192 tokens.
-MAX_GPT_TOKENS = 8192
+MAX_GPT_TOKENS = 128000
 # The maximum number of GPT tokens that chat context can be.
 MAX_PROMPT_TOKENS = MAX_GPT_TOKENS - 1192
 # The maximum number of GPT tokens that can be used for completion.
 MAX_COMPLETION_TOKENS = MAX_GPT_TOKENS - MAX_PROMPT_TOKENS
 
 # Settings for GPT completion generation
 GPT_SETTINGS = {
-    "model": "gpt-4",
+    "model": "gpt-4o",
     "temperature": 0.3,
     "max_tokens": MAX_COMPLETION_TOKENS,
 }
 
 LLM = ChatOpenAI(**GPT_SETTINGS)
 
 # The maximum allowed size of images in megabytes
```

### Comparing `edubot-0.7.5/edubot/sql.py` & `edubot-0.7.6/edubot/sql.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.5/edubot/types.py` & `edubot-0.7.6/edubot/types.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.5/pyproject.toml` & `edubot-0.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "edubot"
-version = "0.7.5"
-description = ""
+version = "0.7.6"
+description = "Basic Edubot module"
 authors = ["exciteabletom <tom@digitalnook.net>", "moodler <martin@moodle.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sqlalchemy = {version = "^2.0.14", extras = ["mypy"]}
```

### Comparing `edubot-0.7.5/PKG-INFO` & `edubot-0.7.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: edubot
-Version: 0.7.5
-Summary: 
+Version: 0.7.6
+Summary: Basic Edubot module
 License: GPLv3
 Author: exciteabletom
 Author-email: tom@digitalnook.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: langchain (>=0.0.279,<0.0.280)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: replicate (>=0.8.1,<0.9.0)
 Requires-Dist: sqlalchemy[mypy] (>=2.0.14,<3.0.0)
 Requires-Dist: stability-sdk (>=0.8.1,<0.9.0)
```

