# Comparing `tmp/modelmerge-0.3.6.tar.gz` & `tmp/modelmerge-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.3.6.tar", last modified: Tue May 14 04:00:12 2024, max compression
+gzip compressed data, was "modelmerge-0.3.7.tar", last modified: Tue May 14 08:42:27 2024, max compression
```

## Comparing `modelmerge-0.3.6.tar` & `modelmerge-0.3.7.tar`

### file list

```diff
@@ -1,39 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.641981 modelmerge-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 04:00:03.000000 modelmerge-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 04:00:12.637981 modelmerge-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-14 04:00:03.000000 modelmerge-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 04:00:12.641981 modelmerge-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 04:00:03.000000 modelmerge-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.633981 modelmerge-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.633981 modelmerge-0.3.6/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30625 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 04:00:03.000000 modelmerge-0.3.6/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 04:00:03.000000 modelmerge-0.3.6/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 04:00:03.000000 modelmerge-0.3.6/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.182336 modelmerge-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 08:42:17.000000 modelmerge-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 08:42:27.182336 modelmerge-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-14 08:42:17.000000 modelmerge-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:42:27.182336 modelmerge-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 08:42:17.000000 modelmerge-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.174337 modelmerge-0.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.174337 modelmerge-0.3.7/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.178336 modelmerge-0.3.7/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-14 08:42:17.000000 modelmerge-0.3.7/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.182336 modelmerge-0.3.7/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:42:27.000000 modelmerge-0.3.7/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:42:27.182336 modelmerge-0.3.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 08:42:17.000000 modelmerge-0.3.7/test/test_whisper.py
```

### Comparing `modelmerge-0.3.6/LICENSE` & `modelmerge-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/PKG-INFO` & `modelmerge-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.6
+Version: 0.3.7
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.3.6/README.md` & `modelmerge-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.3.7/src/ModelMerge/models/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,21 +319,15 @@
         """
         # Make conversation if it doesn't exist
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id, system_prompt=self.system_prompt)
         self.add_to_conversation(prompt, role, convo_id=convo_id, function_name=function_name)
         json_post, message_token = self.truncate_conversation(prompt, role, convo_id, model, pass_history, **kwargs)
         # print(self.conversation[convo_id])
-
-        if self.engine == "gpt-4-1106-preview" or "gpt-4-0125-preview" in self.engine or "gpt-4-turbo" in self.engine or "claude" in self.engine:
-            model_max_tokens = kwargs.get("max_tokens", self.max_tokens)
-        elif self.engine == "gpt-3.5-turbo-1106":
-            model_max_tokens = min(kwargs.get("max_tokens", self.max_tokens), 16385 - message_token["total"])
-        else:
-            model_max_tokens = min(kwargs.get("max_tokens", self.max_tokens), self.max_tokens - message_token["total"])
+        model_max_tokens = kwargs.get("max_tokens", self.max_tokens)
         print("model_max_tokens", model_max_tokens)
         json_post["max_tokens"] = model_max_tokens
         print("api_url", self.api_url.chat_url)
         for _ in range(2):
             print(json.dumps(json_post, indent=4, ensure_ascii=False))
             try:
                 response = self.session.post(
@@ -402,14 +396,15 @@
                 function_full_response += function_call_content
                 if function_full_response.count("\\n") > 2 or "}" in function_full_response:
                     break
         if need_function_call:
             function_full_response = check_json(function_full_response)
             print("function_full_response", function_full_response)
             function_response = ""
+            # print(self.function_calls_counter)
             if not self.function_calls_counter.get(function_call_name):
                 self.function_calls_counter[function_call_name] = 1
             else:
                 self.function_calls_counter[function_call_name] += 1
             if self.function_calls_counter[function_call_name] <= self.function_call_max_loop:
                 function_call_max_tokens = self.truncate_limit - message_token["total"] - 1000
                 if function_call_max_tokens <= 0:
@@ -451,15 +446,15 @@
                 if function_call_name == "get_date_time_weekday":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_version_info":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
             else:
-                function_response = "抱歉，直接告诉用户，无法找到相关信息"
+                function_response = "无法找到相关信息，停止使用 tools"
             response_role = "function"
             # print(self.conversation[convo_id][-1])
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
                 # print("Truncate message:", mess)
             yield from self.ask_stream(function_response, response_role, convo_id=convo_id, function_name=function_call_name)
         else:
```

### Comparing `modelmerge-0.3.6/src/ModelMerge/models/claude.py` & `modelmerge-0.3.7/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/models/config.py` & `modelmerge-0.3.7/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/models/genimi.py` & `modelmerge-0.3.7/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/models/groq.py` & `modelmerge-0.3.7/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.3.7/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.3.7/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/tools/function_call.py` & `modelmerge-0.3.7/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/utils/prompt.py` & `modelmerge-0.3.7/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/ModelMerge/utils/scripts.py` & `modelmerge-0.3.7/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.6/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.3.7/src/modelmerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.6
+Version: 0.3.7
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.3.6/test/test_google_search.py` & `modelmerge-0.3.7/test/test_google_search.py`

 * *Files identical despite different names*

