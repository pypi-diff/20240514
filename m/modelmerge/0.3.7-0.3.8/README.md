# Comparing `tmp/modelmerge-0.3.7.tar.gz` & `tmp/modelmerge-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.3.7.tar", last modified: Tue May 14 08:42:27 2024, max compression
+gzip compressed data, was "modelmerge-0.3.8.tar", last modified: Tue May 14 10:33:42 2024, max compression
```

## Comparing `modelmerge-0.3.7.tar` & `modelmerge-0.3.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.182336 modelmerge-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 08:42:17.000000 modelmerge-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 08:42:27.182336 modelmerge-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-14 08:42:17.000000 modelmerge-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:42:27.182336 modelmerge-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 08:42:17.000000 modelmerge-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.174337 modelmerge-0.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.174337 modelmerge-0.3.7/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.182336 modelmerge-0.3.7/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.182336 modelmerge-0.3.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.212249 modelmerge-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 10:33:34.000000 modelmerge-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 10:33:42.212249 modelmerge-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-14 10:33:34.000000 modelmerge-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:33:42.212249 modelmerge-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 10:33:34.000000 modelmerge-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.204249 modelmerge-0.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.204249 modelmerge-0.3.8/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.208249 modelmerge-0.3.8/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30404 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.208249 modelmerge-0.3.8/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.208249 modelmerge-0.3.8/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.208249 modelmerge-0.3.8/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-14 10:33:34.000000 modelmerge-0.3.8/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.212249 modelmerge-0.3.8/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 10:33:42.000000 modelmerge-0.3.8/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 10:33:42.000000 modelmerge-0.3.8/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:33:42.000000 modelmerge-0.3.8/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 10:33:42.000000 modelmerge-0.3.8/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 10:33:42.000000 modelmerge-0.3.8/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:33:42.212249 modelmerge-0.3.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 10:33:34.000000 modelmerge-0.3.8/test/test_whisper.py
```

### Comparing `modelmerge-0.3.7/LICENSE` & `modelmerge-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/PKG-INFO` & `modelmerge-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.7
+Version: 0.3.8
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.3.7/README.md` & `modelmerge-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.3.8/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,20 +429,23 @@
                     # self.add_to_conversation(user_prompt, "user", convo_id=convo_id)
                 if function_call_name == "get_url_content":
                     url = json.loads(function_full_response)["url"]
                     print("\n\nurl", url)
                     # function_response = jina_ai_Web_crawler(url)
                     function_response = Web_crawler(url)
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                    function_response = (
-                        "Here is the documentation, inside <document></document> XML tags:"
-                        "<document>"
-                        "{}"
-                        "</document>"
-                    ).format(function_response)
+                    if function_response:
+                        function_response = (
+                            "Here is the documentation, inside <document></document> XML tags:"
+                            "<document>"
+                            "{}"
+                            "</document>"
+                        ).format(function_response)
+                    else:
+                        function_response = "无法找到相关信息，停止使用 tools"
                 if function_call_name == "get_city_tarvel_info":
                     city = json.loads(function_full_response)["city"]
                     function_response = eval(function_call_name)(city)
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_date_time_weekday":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
```

### Comparing `modelmerge-0.3.7/src/ModelMerge/models/claude.py` & `modelmerge-0.3.8/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/models/config.py` & `modelmerge-0.3.8/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/models/genimi.py` & `modelmerge-0.3.8/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/models/groq.py` & `modelmerge-0.3.8/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.3.8/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.3.8/src/ModelMerge/plugins/websearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import re
 import datetime
 import requests
 import threading
 import time as record_time
+from itertools import islice
 from bs4 import BeautifulSoup
 from duckduckgo_search import DDGS
 from googleapiclient.discovery import build
 
 from ..models import chatgpt
 
 
@@ -94,24 +95,25 @@
         print("error", e)
         print('\033[0m')
     # print(result + "\n\n")
     return result
 
 def getddgsearchurl(query, max_results=4):
     try:
-        webresult = DDGS().text(query, max_results=max_results)
-        if webresult == None:
-            return []
-        urls = [result['href'] for result in webresult]
+        results = []
+        with DDGS() as ddgs:
+            ddgs_gen = ddgs.text(query, safesearch='Off', timelimit='y', backend="lite")
+            for r in islice(ddgs_gen, max_results):
+                results.append(r)
+        urls = [result['href'] for result in results]
     except Exception as e:
         print('\033[31m')
         print("duckduckgo error", e)
         print('\033[0m')
         urls = []
-    # print("ddg urls", urls)
     return urls
 
 def getgooglesearchurl(result, numresults=3):
     urls = []
     if os.environ.get('GOOGLE_API_KEY', None) == None and os.environ.get('GOOGLE_CSE_ID', None) == None:
         return urls
     try:
```

### Comparing `modelmerge-0.3.7/src/ModelMerge/tools/function_call.py` & `modelmerge-0.3.8/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/utils/prompt.py` & `modelmerge-0.3.8/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/ModelMerge/utils/scripts.py` & `modelmerge-0.3.8/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.3.8/src/modelmerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.7
+Version: 0.3.8
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.3.7/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.3.8/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_Web_crawler.py` & `modelmerge-0.3.8/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_claude_zh_char.py` & `modelmerge-0.3.8/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_download_pdf.py` & `modelmerge-0.3.8/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_google_search.py` & `modelmerge-0.3.8/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_jieba.py` & `modelmerge-0.3.8/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_json.py` & `modelmerge-0.3.8/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_langchain_search_old.py` & `modelmerge-0.3.8/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_logging.py` & `modelmerge-0.3.8/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_ollama.py` & `modelmerge-0.3.8/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_tikitoken.py` & `modelmerge-0.3.8/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_token.py` & `modelmerge-0.3.8/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.7/test/test_url.py` & `modelmerge-0.3.8/test/test_url.py`

 * *Files identical despite different names*

