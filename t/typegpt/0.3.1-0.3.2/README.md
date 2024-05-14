# Comparing `tmp/typegpt-0.3.1.tar.gz` & `tmp/typegpt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegpt-0.3.1.tar", last modified: Wed Apr 17 09:42:28 2024, max compression
+gzip compressed data, was "typegpt-0.3.2.tar", last modified: Tue May 14 12:43:07 2024, max compression
```

## Comparing `typegpt-0.3.1.tar` & `typegpt-0.3.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-17 09:42:22.000000 typegpt-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-17 09:42:28.132899 typegpt-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-17 09:42:22.000000 typegpt-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:42:28.136899 typegpt-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 09:42:22.000000 typegpt-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.128899 typegpt-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_fewshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.128899 typegpt-0.3.1/typegpt/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/example_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/example_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/message_collection_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/openai/_async/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_async/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_async/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/openai/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_sync/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/base_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/prompt_definition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/few_shot_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/prompt_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/internal_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.710874 typegpt-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-14 12:43:01.000000 typegpt-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-05-14 12:43:07.706874 typegpt-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-05-14 12:43:01.000000 typegpt-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:43:07.710874 typegpt-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 12:43:01.000000 typegpt-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.702874 typegpt-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_fewshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22690 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-14 12:43:01.000000 typegpt-0.3.2/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.702874 typegpt-0.3.2/typegpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/example_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/example_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/message_collection_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.706874 typegpt-0.3.2/typegpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.706874 typegpt-0.3.2/typegpt/openai/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/_async/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/_async/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.706874 typegpt-0.3.2/typegpt/openai/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/_sync/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/base_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/openai/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/prompt_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.706874 typegpt-0.3.2/typegpt/prompt_definition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/prompt_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/prompt_definition/few_shot_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/prompt_definition/prompt_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/prompt_definition/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.706874 typegpt-0.3.2/typegpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/utils/internal_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/utils/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 12:43:01.000000 typegpt-0.3.2/typegpt/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:43:07.706874 typegpt-0.3.2/typegpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-05-14 12:43:07.000000 typegpt-0.3.2/typegpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-14 12:43:07.000000 typegpt-0.3.2/typegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:43:07.000000 typegpt-0.3.2/typegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 12:43:07.000000 typegpt-0.3.2/typegpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 12:43:07.000000 typegpt-0.3.2/typegpt.egg-info/top_level.txt
```

### Comparing `typegpt-0.3.1/LICENSE` & `typegpt-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/PKG-INFO` & `typegpt-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: typegpt
-Version: 0.3.1
+Version: 0.3.2
 Summary: TypeGPT - Make GPT safe for production
 Home-page: https://github.com/alexeichhorn/typegpt
 Author: Alexander Eichhorn
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.1.0
 Requires-Dist: inflect>=7.0.0
-Requires-Dist: tiktoken>=0.5.0
+Requires-Dist: tiktoken>=0.7.0
 Requires-Dist: openai>=1.1.0
 
 # TypeGPT - Making GPT Safe for Production
 
 It is inherently difficult to produce outputs from LLMs in a consistent structure. TypeGPT simplifies this process to be as easy as defining a class in Python.
 
 Powering our own projects, such as [Spexia](https://getspexia.com)
```

### Comparing `typegpt-0.3.1/README.md` & `typegpt-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/setup.py` & `typegpt-0.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="typegpt",
-    version="0.3.1",
+    version="0.3.2",
     author="Alexander Eichhorn",
     author_email="",
     description="TypeGPT - Make GPT safe for production",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alexeichhorn/typegpt",
     install_requires=[
         "typing_extensions>=4.1.0",
         "inflect>=7.0.0",
-        "tiktoken>=0.5.0",
+        "tiktoken>=0.7.0",
         "openai>=1.1.0",
     ],
     packages=setuptools.find_packages(),
     classifiers=["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"],
     python_requires=">=3.10",
 )
```

### Comparing `typegpt-0.3.1/tests/test_fewshot.py` & `typegpt-0.3.2/tests/test_fewshot.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/tests/test_fields.py` & `typegpt-0.3.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/tests/test_helpers.py` & `typegpt-0.3.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/tests/test_openai.py` & `typegpt-0.3.2/tests/test_openai.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 import pytest
 from openai import AsyncOpenAI
 from openai.types.chat import ChatCompletion
 from openai.types.chat.chat_completion import Choice
 from openai.types.chat.chat_completion_message import ChatCompletionMessage
 
 from typegpt import BaseLLMResponse, LLMArrayOutput, LLMOutput, PromptTemplate
-from typegpt.exceptions import LLMTokenLimitExceeded
+from typegpt.exceptions import LLMOutputFieldWrongType, LLMTokenLimitExceeded
 from typegpt.openai import AsyncTypeAzureOpenAI, AsyncTypeOpenAI, OpenAIChatModel, TypeAzureOpenAI, TypeOpenAI
 
 
 class TestOpenAIChatCompletion:
     def test_token_counter(self):
         test_messages = [
             {"role": "system", "content": "This is a system message"},
             {"role": "user", "content": "This is a user message 🧑🏾"},
         ]
 
         # check if test covers all models (increase if new models are added)
-        assert len(OpenAIChatModel.__args__) == 19  #  type: ignore
+        assert len(OpenAIChatModel.__args__) == 21  #  type: ignore
 
         client = AsyncTypeOpenAI(api_key="mock")
 
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo-0301") == 29
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo-0613") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo-1106") == 27
@@ -45,22 +45,24 @@
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-32k-0613") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-turbo-preview") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-1106-preview") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-0125-preview") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-vision-preview") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-turbo") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-turbo-2024-04-09") == 27
+        assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4o") == 26
+        assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4o-2024-05-13") == 26
 
     def test_max_token_counter(self):
         # check if test covers all models (increase if new models are added)
-        assert len(OpenAIChatModel.__args__) == 19  #  type: ignore
+        assert len(OpenAIChatModel.__args__) == 21  #  type: ignore
 
         client = AsyncTypeOpenAI(api_key="mock")
 
-        assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo") == 4096
+        assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo") == 16384
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-0301") == 4096
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-0613") == 4096
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-1106") == 16384
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-0125") == 16384
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-16k") == 16384
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-16k-0613") == 16384
         assert client.chat.completions.max_tokens_of_model("gpt-4") == 8192
@@ -71,14 +73,16 @@
         assert client.chat.completions.max_tokens_of_model("gpt-4-32k-0613") == 32768
         assert client.chat.completions.max_tokens_of_model("gpt-4-turbo-preview") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-1106-preview") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-0125-preview") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-vision-preview") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-turbo") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-turbo-2024-04-09") == 128_000
+        assert client.chat.completions.max_tokens_of_model("gpt-4o") == 128_000
+        assert client.chat.completions.max_tokens_of_model("gpt-4o-2024-05-13") == 128_000
 
     # -
 
     @pytest.fixture
     def mock_openai_completion(self, mocker):
         async def async_mock(*args, **kwargs):
             return ChatCompletion(
@@ -372,15 +376,15 @@
                 title: str
                 items: list[str] = LLMArrayOutput((1, 2), instruction=lambda _: "Put the items here")
                 count: int
 
         client = AsyncTypeOpenAI(api_key="mock")
 
         result = await client.chat.completions.generate_output(
-            model="gpt-3.5-turbo", prompt=FullExamplePrompt(), max_output_tokens=100, retry_on_parse_error=5
+            model="gpt-3.5-turbo-0613", prompt=FullExamplePrompt(), max_output_tokens=100, retry_on_parse_error=5
         )
 
         assert isinstance(result, FullExamplePrompt.Output)
         assert result.title == "Some title n"
         assert result.items == ["abc"]
         assert result.count == 42
 
@@ -400,28 +404,31 @@
                 lines: list[str]
 
         non_reducing_prompt_100 = NonAutomaticReducingPrompt(100)
 
         client = AsyncTypeOpenAI(api_key="mock")
 
         result = await client.chat.completions.generate_output(
-            model="gpt-3.5-turbo",
+            model="gpt-3.5-turbo-0613",
             prompt=non_reducing_prompt_100,
             max_output_tokens=100,
         )
 
         non_reducing_prompt_1000 = NonAutomaticReducingPrompt(1000)
 
-        with pytest.raises(LLMTokenLimitExceeded):
+        with pytest.raises(LLMTokenLimitExceeded) as exc:
             result = await client.chat.completions.generate_output(
-                model="gpt-3.5-turbo",
+                model="gpt-3.5-turbo-0613",
                 prompt=non_reducing_prompt_1000,
                 max_output_tokens=100,
             )
 
+        assert exc.value.system_prompt == "This is a random system prompt"
+        assert exc.value.raw_completion is None
+
         class ReducingTestPrompt(PromptTemplate):
             def __init__(self, number: int):
                 self.lines = [f"This is line {i}" for i in range(number)]
 
             def system_prompt(self) -> str:
                 return "This is a random system prompt"
 
@@ -437,25 +444,25 @@
                     self.lines = self.lines[:-10]
                     return True
                 return False
 
         reducing_prompt_100 = ReducingTestPrompt(100)
 
         result = await client.chat.completions.generate_output(
-            model="gpt-3.5-turbo",
+            model="gpt-3.5-turbo-0613",
             prompt=reducing_prompt_100,
             max_output_tokens=100,
         )
 
         assert len(reducing_prompt_100.lines) == 100
 
         reducing_prompt_1000 = ReducingTestPrompt(1000)
 
         result = await client.chat.completions.generate_output(
-            model="gpt-3.5-turbo",
+            model="gpt-3.5-turbo-0613",
             prompt=reducing_prompt_1000,
             max_output_tokens=100,
         )
 
     # -
 
     def test_dynamic_output_type(self, mock_openai_completion_sync):
@@ -478,15 +485,89 @@
                 return Output
 
         client = TypeOpenAI(api_key="mock")
 
         prompt = FullExamplePrompt("test")
 
         result = client.chat.completions.generate_output(
-            model="gpt-3.5-turbo",
+            model="gpt-3.5-turbo-0613",
             prompt=prompt,
             output_type=prompt.Output,
             max_output_tokens=100,
         )
 
         assert result.title == "This is a test completion"
         assert result.count == 9
+
+    # region: - Exceptions
+
+    def test_exception_injection_sync(self, mock_openai_completion_sync):
+        class ExamplePrompt(PromptTemplate):
+            class Output(BaseLLMResponse):
+                title: int  # wrong type
+                count: int
+
+            def system_prompt(self) -> str:
+                return "This is a random system prompt"
+
+            def user_prompt(self) -> str:
+                return "This is a random user prompt"
+
+        client = TypeOpenAI(api_key="mock")
+
+        with pytest.raises(LLMOutputFieldWrongType) as exc:
+            result = client.chat.completions.generate_output(
+                model="gpt-3.5-turbo-0613",
+                prompt=ExamplePrompt(),
+                output_type=ExamplePrompt.Output,
+                max_output_tokens=100,
+            )
+
+        assert exc.value.system_prompt and exc.value.system_prompt.startswith("This is a random system prompt")  # + format instruction
+        assert exc.value.user_prompt == "This is a random user prompt"
+        assert exc.value.raw_completion == "TITLE: This is a test completion\nCOUNT: 09"
+
+    @pytest.mark.asyncio
+    async def test_exception_injection_async(self, mock_openai_completion):
+        class ExamplePrompt(PromptTemplate):
+            class Output(BaseLLMResponse):
+                title: int  # wrong type
+                count: int
+
+            def system_prompt(self) -> str:
+                return "This is a random system prompt"
+
+            def user_prompt(self) -> str:
+                return "This is a random user prompt"
+
+        client = AsyncTypeOpenAI(api_key="mock")
+
+        with pytest.raises(LLMOutputFieldWrongType) as exc:
+            result = await client.chat.completions.generate_output(
+                model="gpt-3.5-turbo-0613",
+                prompt=ExamplePrompt(),
+                output_type=ExamplePrompt.Output,
+                max_output_tokens=100,
+            )
+
+        assert exc.value.system_prompt and exc.value.system_prompt.startswith("This is a random system prompt")  # + format instruction
+        assert exc.value.user_prompt == "This is a random user prompt"
+        assert exc.value.raw_completion == "TITLE: This is a test completion\nCOUNT: 09"
+
+        # - Azure
+
+        azure_client = AsyncTypeAzureOpenAI(api_key="mock", azure_endpoint="mock", api_version="mock")
+
+        with pytest.raises(LLMOutputFieldWrongType) as exc2:
+            result = await azure_client.chat.completions.generate_output(
+                model="gpt-3.5-turbo-0613",
+                prompt=ExamplePrompt(),
+                output_type=ExamplePrompt.Output,
+                max_output_tokens=100,
+            )
+
+        assert exc.value.system_prompt and exc.value.system_prompt.startswith("This is a random system prompt")  # + format instruction
+        assert exc2.value.user_prompt == "This is a random user prompt"
+        assert exc2.value.raw_completion == "TITLE: This is a test completion\nCOUNT: 09"
+
+
+# endregion: - Exceptions
```

### Comparing `typegpt-0.3.1/tests/test_parser.py` & `typegpt-0.3.2/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,25 +140,33 @@
         with pytest.raises(LLMOutputFieldMissing):
             self.MultilineMultipleTestOutput.parse_response(completion_output_3)
 
         completion_output_4 = """
 TEXT: L1
 """
 
-        with pytest.raises(LLMOutputFieldMissing):
+        with pytest.raises(LLMOutputFieldMissing) as exc1:
             self.MultilineMultipleTestOutput.parse_response(completion_output_4)
 
+        assert exc1.value.system_prompt is None
+        assert exc1.value.user_prompt is None
+        assert exc1.value.raw_completion == completion_output_4
+
         completion_output = """
 TEXT: L1
 VALUE: 8xz
 """
 
-        with pytest.raises(LLMOutputFieldWrongType):
+        with pytest.raises(LLMOutputFieldWrongType) as exc2:
             self.MultilineMultipleTestOutput.parse_response(completion_output)
 
+        assert exc2.value.system_prompt is None
+        assert exc2.value.user_prompt is None
+        assert exc2.value.raw_completion == completion_output
+
     # endregion
     # region - 4
 
     class LimitedArrayTestOutput(BaseLLMResponse):
         geese: list[str] = LLMArrayOutput((2, 3), lambda _: "test")
 
     # endregion
@@ -178,17 +186,21 @@
         parsed_output = self.MultilineArrayTestOutput.parse_response(completion_output)
         assert parsed_output.apples == ["L1\nL2", "L3\nL4"]
 
         completion_output_2 = """
 APPLE 1: L1
 """
 
-        with pytest.raises(LLMOutputFieldInvalidLength):
+        with pytest.raises(LLMOutputFieldInvalidLength) as exc:
             self.MultilineArrayTestOutput.parse_response(completion_output_2)
 
+        assert exc.value.system_prompt is None
+        assert exc.value.user_prompt is None
+        assert exc.value.raw_completion == completion_output_2
+
         completion_output_3 = """
 APPLE 1: L1
 APPLE 2: L2
 APPLE 3: L3
 """
 
         parsed_output_3 = self.MultilineArrayTestOutput.parse_response(completion_output_3)
```

### Comparing `typegpt-0.3.1/tests/test_prompt.py` & `typegpt-0.3.2/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/tests/test_response_object.py` & `typegpt-0.3.2/tests/test_response_object.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/tests/test_settings.py` & `typegpt-0.3.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/base.py` & `typegpt-0.3.2/typegpt/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TYPE_CHECKING, Any, ClassVar, TypeVar
 
-from .exceptions import LLMOutputFieldInvalidLength, LLMOutputFieldMissing, LLMOutputFieldWrongType
+from .exceptions import LLMException, LLMOutputFieldInvalidLength, LLMOutputFieldMissing, LLMOutputFieldWrongType
 from .fields import ClassPlaceholder, LLMArrayElementOutputInfo, LLMArrayOutputInfo, LLMFieldInfo, LLMOutputInfo
 from .meta import LLMArrayElementMeta, LLMBaseMeta
 from .parser import Parser
 
 if TYPE_CHECKING:
     from inspect import Signature
 
@@ -159,15 +159,19 @@
 
     # - Parsing
 
     _Self = TypeVar("_Self", bound="BaseLLMResponse")  # backward compatibility for pre-Python 3.12
 
     @classmethod
     def parse_response(cls: type[_Self], response: str) -> _Self:
-        return Parser(cls).parse(response)
+        try:
+            return Parser(cls).parse(response)
+        except LLMException as e:
+            e.raw_completion = response
+            raise e
 
 
 # -
 
 
 class BaseLLMArrayElement(_InternalBaseLLMResponse, metaclass=LLMArrayElementMeta):
     if TYPE_CHECKING:
```

### Comparing `typegpt-0.3.1/typegpt/example_builder.py` & `typegpt-0.3.2/typegpt/example_builder.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/example_formatter.py` & `typegpt-0.3.2/typegpt/example_formatter.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/fields.py` & `typegpt-0.3.2/typegpt/fields.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/helper.py` & `typegpt-0.3.2/typegpt/helper.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/message_collection_builder.py` & `typegpt-0.3.2/typegpt/message_collection_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,12 +67,16 @@
             generated_messages = self._generate_messages_from_prompt(prompt)
 
             num_tokens = self.token_counter(generated_messages)
             if num_tokens <= token_limit:
                 self.prompt = prompt  # update the prompt if successful
                 return generated_messages
 
-        raise LLMTokenLimitExceeded(f"Prompt can't be reduced to fit within the token limit ({token_limit})")
+        raise LLMTokenLimitExceeded(
+            f"Prompt can't be reduced to fit within the token limit ({token_limit})",
+            system_prompt=prompt.system_prompt(),
+            user_prompt=prompt.user_prompt(),
+        )
 
 
 if TYPE_CHECKING:
     from .prompt_definition.prompt_template import PromptTemplate
```

### Comparing `typegpt-0.3.1/typegpt/meta.py` & `typegpt-0.3.2/typegpt/meta.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/openai/_async/chat_completion.py` & `typegpt-0.3.2/typegpt/openai/_async/chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ChatCompletionMessageParam,
     ChatCompletionToolChoiceOptionParam,
     ChatCompletionToolParam,
     completion_create_params,
 )
 
 from ...base import BaseLLMResponse
-from ...exceptions import LLMParseException
+from ...exceptions import LLMException, LLMParseException
 from ...prompt_definition.prompt_template import PromptTemplate
 from ...utils.internal_types import _UseDefault, _UseDefaultType
 from ..base_chat_completion import BaseChatCompletions
 from ..exceptions import AzureContentFilterException
 from ..views import AzureChatModel, OpenAIChatModel
 
 # Prompt = TypeVar("Prompt", bound=PromptTemplate)
@@ -103,16 +103,15 @@
         n: int | None | NotGiven = NOT_GIVEN,
         presence_penalty: float | None | NotGiven = NOT_GIVEN,  # [-2, 2]
         temperature: float | NotGiven = NOT_GIVEN,
         seed: int | None | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         timeout: float | None | NotGiven = NOT_GIVEN,
         retry_on_parse_error: int = 0,
-    ) -> _Output:
-        ...
+    ) -> _Output: ...
 
     @overload
     async def generate_output(
         self,
         model: OpenAIChatModel | AzureChatModel,
         prompt: PromptTemplate,
         max_output_tokens: int,
@@ -122,16 +121,15 @@
         n: int | None | NotGiven = NOT_GIVEN,
         presence_penalty: float | None | NotGiven = NOT_GIVEN,  # [-2, 2]
         temperature: float | NotGiven = NOT_GIVEN,
         seed: int | None | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         timeout: float | None | NotGiven = NOT_GIVEN,
         retry_on_parse_error: int = 0,
-    ) -> BaseLLMResponse:
-        ...
+    ) -> BaseLLMResponse: ...
 
     async def generate_output(
         self,
         model: OpenAIChatModel | AzureChatModel,
         prompt: PromptTemplate,
         max_output_tokens: int,
         output_type: type[_Output] | _UseDefaultType = _UseDefault,
@@ -204,8 +202,13 @@
                     temperature=temperature,
                     seed=seed,
                     top_p=top_p,
                     timeout=timeout,
                     retry_on_parse_error=retry_on_parse_error - 1,
                 )
             else:
+                self._inject_exception_details(e, messages, completion)
                 raise e
+
+        except LLMException as e:
+            self._inject_exception_details(e, messages, completion)
+            raise e
```

### Comparing `typegpt-0.3.1/typegpt/openai/_async/client.py` & `typegpt-0.3.2/typegpt/openai/_async/client.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/openai/_sync/chat_completion.py` & `typegpt-0.3.2/typegpt/openai/_sync/chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ChatCompletionMessageParam,
     ChatCompletionToolChoiceOptionParam,
     ChatCompletionToolParam,
     completion_create_params,
 )
 
 from ...base import BaseLLMResponse
-from ...exceptions import LLMParseException
+from ...exceptions import LLMException, LLMParseException
 from ...prompt_definition.prompt_template import PromptTemplate
 from ...utils.internal_types import _UseDefault, _UseDefaultType
 from ..base_chat_completion import BaseChatCompletions
 from ..exceptions import AzureContentFilterException
 from ..views import AzureChatModel, OpenAIChatModel
 
 _Output = TypeVar("_Output", bound=BaseLLMResponse)
@@ -102,16 +102,15 @@
         n: int | None | NotGiven = NOT_GIVEN,
         presence_penalty: float | None | NotGiven = NOT_GIVEN,  # [-2, 2]
         temperature: float | NotGiven = NOT_GIVEN,
         seed: int | None | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         timeout: float | None | NotGiven = NOT_GIVEN,
         retry_on_parse_error: int = 0,
-    ) -> _Output:
-        ...
+    ) -> _Output: ...
 
     @overload
     def generate_output(
         self,
         model: OpenAIChatModel | AzureChatModel,
         prompt: PromptTemplate,
         max_output_tokens: int,
@@ -121,16 +120,15 @@
         n: int | None | NotGiven = NOT_GIVEN,
         presence_penalty: float | None | NotGiven = NOT_GIVEN,  # [-2, 2]
         temperature: float | NotGiven = NOT_GIVEN,
         seed: int | None | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         timeout: float | None | NotGiven = NOT_GIVEN,
         retry_on_parse_error: int = 0,
-    ) -> BaseLLMResponse:
-        ...
+    ) -> BaseLLMResponse: ...
 
     def generate_output(
         self,
         model: OpenAIChatModel | AzureChatModel,
         prompt: PromptTemplate,
         max_output_tokens: int,
         output_type: type[_Output] | _UseDefaultType = _UseDefault,
@@ -203,8 +201,13 @@
                     temperature=temperature,
                     seed=seed,
                     top_p=top_p,
                     timeout=timeout,
                     retry_on_parse_error=retry_on_parse_error - 1,
                 )
             else:
+                self._inject_exception_details(e, messages, completion)
                 raise e
+
+        except LLMException as e:
+            self._inject_exception_details(e, messages, completion)
+            raise e
```

### Comparing `typegpt-0.3.1/typegpt/openai/_sync/client.py` & `typegpt-0.3.2/typegpt/openai/_sync/client.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/openai/views.py` & `typegpt-0.3.2/typegpt/openai/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     "gpt-4-32k-0613",
     "gpt-4-turbo",  # gpt-4 turbo
     "gpt-4-turbo-2024-04-09",
     "gpt-4-turbo-preview",  # gpt-4 turbo (preview)
     "gpt-4-1106-preview",
     "gpt-4-0125-preview",
     "gpt-4-vision-preview",  # gpt-4 vision (preview)
+    "gpt-4o",  # gpt-4o
+    "gpt-4o-2024-05-13",
 ]
 
 
 @dataclass
 class AzureChatModel:
     deployment_id: str
     base_model: OpenAIChatModel  # only used for token counting
```

### Comparing `typegpt-0.3.1/typegpt/parser.py` & `typegpt-0.3.2/typegpt/parser.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/prompt_builder.py` & `typegpt-0.3.2/typegpt/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/prompt_definition/prompt_template.py` & `typegpt-0.3.2/typegpt/prompt_definition/prompt_template.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/utils/type_checker.py` & `typegpt-0.3.2/typegpt/utils/type_checker.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt/utils/utils.py` & `typegpt-0.3.2/typegpt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.1/typegpt.egg-info/PKG-INFO` & `typegpt-0.3.2/typegpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: typegpt
-Version: 0.3.1
+Version: 0.3.2
 Summary: TypeGPT - Make GPT safe for production
 Home-page: https://github.com/alexeichhorn/typegpt
 Author: Alexander Eichhorn
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.1.0
 Requires-Dist: inflect>=7.0.0
-Requires-Dist: tiktoken>=0.5.0
+Requires-Dist: tiktoken>=0.7.0
 Requires-Dist: openai>=1.1.0
 
 # TypeGPT - Making GPT Safe for Production
 
 It is inherently difficult to produce outputs from LLMs in a consistent structure. TypeGPT simplifies this process to be as easy as defining a class in Python.
 
 Powering our own projects, such as [Spexia](https://getspexia.com)
```

### Comparing `typegpt-0.3.1/typegpt.egg-info/SOURCES.txt` & `typegpt-0.3.2/typegpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

