# Comparing `tmp/modelmerge-0.3.4.tar.gz` & `tmp/modelmerge-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.3.4.tar", last modified: Mon May 13 08:38:25 2024, max compression
+gzip compressed data, was "modelmerge-0.3.5.tar", last modified: Mon May 13 20:19:09 2024, max compression
```

## Comparing `modelmerge-0.3.4.tar` & `modelmerge-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.441986 modelmerge-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 08:38:14.000000 modelmerge-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 08:38:25.441986 modelmerge-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 08:38:14.000000 modelmerge-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:38:25.441986 modelmerge-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 08:38:14.000000 modelmerge-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.433986 modelmerge-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.433986 modelmerge-0.3.4/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.441986 modelmerge-0.3.4/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 08:38:14.000000 modelmerge-0.3.4/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 08:38:14.000000 modelmerge-0.3.4/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 08:38:14.000000 modelmerge-0.3.4/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.728814 modelmerge-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 20:19:01.000000 modelmerge-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-13 20:19:09.724814 modelmerge-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 20:19:01.000000 modelmerge-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:19:09.728814 modelmerge-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:19:01.000000 modelmerge-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.720814 modelmerge-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.720814 modelmerge-0.3.5/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30484 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-13 20:19:01.000000 modelmerge-0.3.5/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 20:19:09.000000 modelmerge-0.3.5/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:09.724814 modelmerge-0.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 20:19:01.000000 modelmerge-0.3.5/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 20:19:01.000000 modelmerge-0.3.5/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 20:19:01.000000 modelmerge-0.3.5/test/test_google_search.py
```

### Comparing `modelmerge-0.3.4/LICENSE` & `modelmerge-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/PKG-INFO` & `modelmerge-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.4
+Version: 0.3.5
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
+Requires-Dist: execjs
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: duckduckgo-search==5.3.1
 Requires-Dist: google-api-python-client==2.128.0
```

### Comparing `modelmerge-0.3.4/README.md` & `modelmerge-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.3.5/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import tiktoken
 
 # import config
 from ..utils.scripts import check_json, cut_message
 from ..utils.prompt import search_key_word_prompt
 from ..tools.function_call import function_call_list
 from ..plugins.websearch import Web_crawler, get_search_results
+from ..plugins.tarvel import get_city_tarvel_info
 
 def get_filtered_keys_from_object(obj: object, *keys: str) -> Set[str]:
     """
     Get filtered list of object variable names.
     :param keys: List of keys to include. If the first key is "not", the remaining keys will be removed from the class keys.
     :return: List of class keys.
     """
@@ -362,14 +363,15 @@
         full_response: str = ""
         function_full_response: str = ""
         function_call_name: str = ""
         need_function_call: bool = False
         for line in response.iter_lines():
             if not line or line.decode("utf-8").startswith(':'):
                 continue
+            # print("line.decode('utf-8')", line.decode("utf-8"))
             if line.decode("utf-8").startswith('data:'):
                 line = line.decode("utf-8")[6:]
             else:
                 print("line", line.decode("utf-8"))
                 full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
                 yield full_response
                 break
@@ -436,14 +438,18 @@
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                     function_response = (
                         "Here is the documentation, inside <document></document> XML tags:"
                         "<document>"
                         "{}"
                         "</document>"
                     ).format(function_response)
+                if function_call_name == "get_city_tarvel_info":
+                    city = json.loads(function_full_response)["city"]
+                    function_response = eval(function_call_name)(city)
+                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_date_time_weekday":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_version_info":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
             else:
```

### Comparing `modelmerge-0.3.4/src/ModelMerge/models/claude.py` & `modelmerge-0.3.5/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/src/ModelMerge/models/config.py` & `modelmerge-0.3.5/src/ModelMerge/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ..utils import prompt
 
 PLUGINS = {
     "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
     "URL": True,
     "DATE": False,
     "VERSION": False,
+    "TARVEL": False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
 
 class BaseAPI:
     def __init__(
         self,
```

### Comparing `modelmerge-0.3.4/src/ModelMerge/models/genimi.py` & `modelmerge-0.3.5/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/src/ModelMerge/models/groq.py` & `modelmerge-0.3.5/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.3.5/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/src/ModelMerge/tools/function_call.py` & `modelmerge-0.3.5/src/ModelMerge/tools/function_call.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,14 +71,30 @@
         "name": "get_version_info",
         "description": "Get version information",
         "parameters": {
             "type": "object",
             "properties": {}
         }
     },
+    "TARVEL": {
+        "name": "get_city_tarvel_info",
+        "description": "Get the city's travel plan by city name.",
+        "parameters": {
+            "type": "object",
+            "properties": {
+                "city": {
+                    "type": "string",
+                    "description": "the city to search"
+                }
+            },
+            "required": [
+                "city"
+            ]
+        }
+    },
 }
 def gpt2claude_tools_json(json_dict):
     import copy
     json_dict = copy.deepcopy(json_dict)
     keys_to_change = {
         "parameters": "input_schema",
         "functions": "tools",
```

### Comparing `modelmerge-0.3.4/src/ModelMerge/utils/prompt.py` & `modelmerge-0.3.5/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/src/ModelMerge/utils/scripts.py` & `modelmerge-0.3.5/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.4/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.3.5/src/modelmerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.4
+Version: 0.3.5
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
+Requires-Dist: execjs
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: duckduckgo-search==5.3.1
 Requires-Dist: google-api-python-client==2.128.0
```

### Comparing `modelmerge-0.3.4/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.3.5/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/ModelMerge/models/__init__.py
 src/ModelMerge/models/chatgpt.py
 src/ModelMerge/models/claude.py
 src/ModelMerge/models/config.py
 src/ModelMerge/models/genimi.py
 src/ModelMerge/models/groq.py
 src/ModelMerge/plugins/__init__.py
+src/ModelMerge/plugins/tarvel.py
 src/ModelMerge/plugins/today.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
 src/ModelMerge/tools/function_call.py
 src/ModelMerge/utils/__init__.py
 src/ModelMerge/utils/prompt.py
```

### Comparing `modelmerge-0.3.4/test/test_google_search.py` & `modelmerge-0.3.5/test/test_google_search.py`

 * *Files identical despite different names*

