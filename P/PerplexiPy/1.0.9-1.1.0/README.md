# Comparing `tmp/PerplexiPy-1.0.9-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13233 bytes, number of entries: 10
--rw-r--r--  2.0 unx     9961 b- defN 24-May-10 05:58 perplexipy/__init__.py
--rw-r--r--  2.0 unx    15810 b- defN 24-May-10 06:04 perplexipy/codex.py
+Zip file size: 13195 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9671 b- defN 24-May-14 03:42 perplexipy/__init__.py
+-rw-r--r--  2.0 unx    15907 b- defN 24-May-14 03:42 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-May-10 06:07 PerplexiPy-1.0.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6968 b- defN 24-May-10 06:07 PerplexiPy-1.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 06:07 PerplexiPy-1.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-May-10 06:07 PerplexiPy-1.0.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-May-10 06:07 PerplexiPy-1.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      814 b- defN 24-May-10 06:07 PerplexiPy-1.0.9.dist-info/RECORD
-10 files, 36186 bytes uncompressed, 11841 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-14 03:43 PerplexiPy-1.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6968 b- defN 24-May-14 03:43 PerplexiPy-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 03:43 PerplexiPy-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-14 03:43 PerplexiPy-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-14 03:43 PerplexiPy-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      814 b- defN 24-May-14 03:43 PerplexiPy-1.1.0.dist-info/RECORD
+10 files, 35993 bytes uncompressed, 11803 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.9.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.9.dist-info/METADATA
+Filename: PerplexiPy-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.9.dist-info/WHEEL
+Filename: PerplexiPy-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.9.dist-info/entry_points.txt
+Filename: PerplexiPy-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.9.dist-info/top_level.txt
+Filename: PerplexiPy-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.9.dist-info/RECORD
+Filename: PerplexiPy-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/__init__.py

```diff
@@ -251,23 +251,20 @@
 
         - `parameterCount`
         - `contextLength`
         - `modelType`
         - `availability`
         """
         supportedModels = OrderedDict({
-            'codellama-70b-instruct': ModelInfo('70B', 16384, 'chat completion', 'open source',),
             'llama-3-70b-instruct': ModelInfo('70B', 8192, 'chat completion', 'open source'),
             'llama-3-8b-instruct': ModelInfo('8B', 8192, 'chat completion', 'open source'),
             'llama-3-sonar-large-32k-chat': ModelInfo('8x7B', 32768, 'chat completion', 'Perplexity',),
             'llama-3-sonar-large-32k-online': ModelInfo('8x7B', 32768, 'chat completion', 'Perplexity',),
             'llama-3-sonar-small-32k-chat': ModelInfo('7B', 32768, 'chat completion', 'Perplexity',),
             'llama-3-sonar-small-32k-online': ModelInfo('7B', 32768, 'chat completion', 'Perplexity',),
-            'mistral-7b-instruct': ModelInfo('7B', 16384, 'chat completion', 'open source',),
-            'mixtral-8x7b-instruct': ModelInfo('8x7B', 16384, 'chat completion', 'open source',),
         })
 
         return supportedModels
 
 
     @property
     def model(self) -> str:
```

## perplexipy/codex.py

```diff
@@ -3,14 +3,15 @@
 
 from appdirs import AppDirs
 from prompt_toolkit import HTML
 from prompt_toolkit import PromptSession
 from prompt_toolkit import print_formatted_text as printF
 from prompt_toolkit.enums import EditingMode
 
+from perplexipy import PERPLEXITY_DEFAULT_MODEL
 from perplexipy import PerplexityClient
 from perplexipy import __VERSION__
 
 import os
 import select
 import sys
 
@@ -30,15 +31,19 @@
 @private
 """
 CONFIG_FILE_NAME = os.path.join(CONFIG_PATH, 'codex-repl.yaml')
 """
 @private
 """
 
-DEFAULT_MODEL_NAME = 'mixtral-8x7b-instruct'
+DEFAULT_MODEL_NAME = PERPLEXITY_DEFAULT_MODEL
+"""
+@public
+Codex Playground default model.
+"""
 DEFAULT_VIM_EDIT_MODE = True
 """
 @private
 """
 
 QUERY_CRISP = 'Concise, code only reply to this prompt: '
 """
```

## Comparing `PerplexiPy-1.0.9.dist-info/LICENSE.txt` & `PerplexiPy-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.9.dist-info/METADATA` & `PerplexiPy-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.9
+Version: 1.1.0
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.9 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.1.0 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.9 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.1.0 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.9 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.1.0 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
```

## Comparing `PerplexiPy-1.0.9.dist-info/RECORD` & `PerplexiPy-1.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perplexipy/__init__.py,sha256=Kw2CPH3DHV8ukgVaWXOLjPWQe8Y0KOJIC0abJCU7oo8,9961
-perplexipy/codex.py,sha256=7HM4Q5iZaL35uN1N0uW2MiD7eH3mNYq9vki4Jbt_atE,15810
+perplexipy/__init__.py,sha256=6VBMWJybFtuVrt6ffrnJSekTPDFacjFfqwOR3zz4GXc,9671
+perplexipy/codex.py,sha256=30bl8lst6HinWgN6o_W-CyGyqs0lKcDbhuE90Rv2sus,15907
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-1.0.9.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-1.0.9.dist-info/METADATA,sha256=FXuxdO5tw2QJO9TgY2UePfV9gEDA9IqGrfBihzglvMM,6968
-PerplexiPy-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-1.0.9.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-1.0.9.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-1.0.9.dist-info/RECORD,,
+PerplexiPy-1.1.0.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.1.0.dist-info/METADATA,sha256=8NXcQXrXmYCeUGU8x6v-Jtin08Y4las7pMDwBenIQCI,6968
+PerplexiPy-1.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.1.0.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.1.0.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.1.0.dist-info/RECORD,,
```

