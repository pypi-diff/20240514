# Comparing `tmp/modelmerge-0.3.5.tar.gz` & `tmp/modelmerge-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.3.5.tar", last modified: Mon May 13 20:19:09 2024, max compression
+gzip compressed data, was "modelmerge-0.3.6.tar", last modified: Tue May 14 04:00:12 2024, max compression
```

## Comparing `modelmerge-0.3.5.tar` & `modelmerge-0.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.728814 modelmerge-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 20:19:01.000000 modelmerge-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-13 20:19:09.724814 modelmerge-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 20:19:01.000000 modelmerge-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:19:09.728814 modelmerge-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:19:01.000000 modelmerge-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.720814 modelmerge-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.720814 modelmerge-0.3.5/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30484 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 20:19:01.000000 modelmerge-0.3.5/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 20:19:01.000000 modelmerge-0.3.5/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 20:19:01.000000 modelmerge-0.3.5/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.641981 modelmerge-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 04:00:03.000000 modelmerge-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 04:00:12.637981 modelmerge-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-14 04:00:03.000000 modelmerge-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 04:00:12.641981 modelmerge-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 04:00:03.000000 modelmerge-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.633981 modelmerge-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.633981 modelmerge-0.3.6/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30625 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-14 04:00:03.000000 modelmerge-0.3.6/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 04:00:12.000000 modelmerge-0.3.6/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:00:12.637981 modelmerge-0.3.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 04:00:03.000000 modelmerge-0.3.6/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 04:00:03.000000 modelmerge-0.3.6/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 04:00:03.000000 modelmerge-0.3.6/test/test_google_search.py
```

### Comparing `modelmerge-0.3.5/LICENSE` & `modelmerge-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/PKG-INFO` & `modelmerge-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.5
+Version: 0.3.6
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
-Requires-Dist: execjs
+Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: duckduckgo-search==5.3.1
 Requires-Dist: google-api-python-client==2.128.0
```

### Comparing `modelmerge-0.3.5/README.md` & `modelmerge-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.3.6/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,28 +61,28 @@
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         super().__init__(api_key, engine, api_url, system_prompt, proxy, timeout, max_tokens, temperature, top_p, presence_penalty, frequency_penalty, reply_count, truncate_limit)
         self.max_tokens: int = max_tokens or (
             4096
-            if "gpt-4-1106-preview" in engine or "gpt-4-0125-preview" in engine or "gpt-4-turbo" in engine or "gpt-3.5-turbo-1106" in engine or "claude" in engine
+            if "gpt-4-1106-preview" in engine or "gpt-4-0125-preview" in engine or "gpt-4-turbo" in engine or "gpt-3.5-turbo-1106" in engine or "claude" in engine or "gpt-4o" in engine
             else 31000
             if "gpt-4-32k" in engine
             else 7000
             if "gpt-4" in engine
             else 16385
             if "gpt-3.5-turbo-16k" in engine
             # else 99000
             # if "claude-2.1" in engine
             else 4000
         )
         self.truncate_limit: int = truncate_limit or (
             127500
-            if "gpt-4-1106-preview" in engine or "gpt-4-0125-preview" in engine or "gpt-4-turbo" in engine
+            if "gpt-4-1106-preview" in engine or "gpt-4-0125-preview" in engine or "gpt-4-turbo" in engine or "gpt-4o" in engine
             else 30500
             if "gpt-4-32k" in engine
             else 6500
             if "gpt-4" in engine
             else 14500
             if "gpt-3.5-turbo-16k" in engine or "gpt-3.5-turbo-1106" in engine
             else 98500
@@ -285,14 +285,15 @@
             "n": kwargs.get("n", self.reply_count),
             "user": role,
         }
         json_post_body.update(copy.deepcopy(body))
         json_post_body.update(copy.deepcopy(function_call_list["base"]))
         for item in PLUGINS.keys():
             try:
+                # print(item, PLUGINS[item])
                 if PLUGINS[item]:
                     json_post_body["functions"].append(function_call_list[item])
             except:
                 pass
 
         return json_post_body
 
@@ -347,14 +348,15 @@
                 return
             except requests.exceptions.ReadTimeout:
                 print("请求超时，请检查网络连接或增加超时时间。{e}")
                 return
             except Exception as e:
                 print(f"发生了未预料的错误: {e}")
                 return
+            # print("response.text", response.text)
             if response.status_code == 400:
                 del json_post["function_call"]
                 del json_post["functions"]
                 continue
             if response.status_code == 200:
                 break
         if response.status_code != 200:
```

### Comparing `modelmerge-0.3.5/src/ModelMerge/models/claude.py` & `modelmerge-0.3.6/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/models/config.py` & `modelmerge-0.3.6/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/models/genimi.py` & `modelmerge-0.3.6/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/models/groq.py` & `modelmerge-0.3.6/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.3.6/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.3.6/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/tools/function_call.py` & `modelmerge-0.3.6/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/utils/prompt.py` & `modelmerge-0.3.6/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/ModelMerge/utils/scripts.py` & `modelmerge-0.3.6/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.3.6/src/modelmerge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.5
+Version: 0.3.6
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
-Requires-Dist: execjs
+Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: duckduckgo-search==5.3.1
 Requires-Dist: google-api-python-client==2.128.0
```

### Comparing `modelmerge-0.3.5/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.3.6/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.5/test/test_google_search.py` & `modelmerge-0.3.6/test/test_google_search.py`

 * *Files identical despite different names*

