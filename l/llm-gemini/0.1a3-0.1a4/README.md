# Comparing `tmp/llm-gemini-0.1a3.tar.gz` & `tmp/llm_gemini-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-gemini-0.1a3.tar", last modified: Wed Apr 10 21:38:07 2024, max compression
+gzip compressed data, was "llm_gemini-0.1a4.tar", last modified: Tue May 14 19:59:52 2024, max compression
```

## Comparing `llm-gemini-0.1a3.tar` & `llm_gemini-0.1a4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:38:07.939016 llm-gemini-0.1a3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 21:37:57.000000 llm-gemini-0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-10 21:38:07.939016 llm-gemini-0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-10 21:37:57.000000 llm-gemini-0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:38:07.939016 llm-gemini-0.1a3/llm_gemini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-10 21:38:07.000000 llm-gemini-0.1a3/llm_gemini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 21:38:07.000000 llm-gemini-0.1a3/llm_gemini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:38:07.000000 llm-gemini-0.1a3/llm_gemini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 21:38:07.000000 llm-gemini-0.1a3/llm_gemini.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 21:38:07.000000 llm-gemini-0.1a3/llm_gemini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 21:38:07.000000 llm-gemini-0.1a3/llm_gemini.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-10 21:37:57.000000 llm-gemini-0.1a3/llm_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 21:37:57.000000 llm-gemini-0.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:38:07.939016 llm-gemini-0.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:38:07.939016 llm-gemini-0.1a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 21:37:57.000000 llm-gemini-0.1a3/tests/test_gemini.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:59:52.088758 llm_gemini-0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:59:43.000000 llm_gemini-0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-14 19:59:52.088758 llm_gemini-0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-14 19:59:43.000000 llm_gemini-0.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:59:52.088758 llm_gemini-0.1a4/llm_gemini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-14 19:59:52.000000 llm_gemini-0.1a4/llm_gemini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 19:59:52.000000 llm_gemini-0.1a4/llm_gemini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:59:52.000000 llm_gemini-0.1a4/llm_gemini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 19:59:52.000000 llm_gemini-0.1a4/llm_gemini.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 19:59:52.000000 llm_gemini-0.1a4/llm_gemini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:59:52.000000 llm_gemini-0.1a4/llm_gemini.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-14 19:59:43.000000 llm_gemini-0.1a4/llm_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-14 19:59:43.000000 llm_gemini-0.1a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:59:52.088758 llm_gemini-0.1a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:59:52.088758 llm_gemini-0.1a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 19:59:43.000000 llm_gemini-0.1a4/tests/test_gemini.py
```

### Comparing `llm-gemini-0.1a3/LICENSE` & `llm_gemini-0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-gemini-0.1a3/PKG-INFO` & `llm_gemini-0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-gemini
-Version: 0.1a3
+Version: 0.1a4
 Summary: LLM plugin to access Google's Gemini family of models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-gemini
 Project-URL: Changelog, https://github.com/simonw/llm-gemini/releases
 Project-URL: Issues, https://github.com/simonw/llm-gemini/issues
 Project-URL: CI, https://github.com/simonw/llm-gemini/actions
```

### Comparing `llm-gemini-0.1a3/README.md` & `llm_gemini-0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `llm-gemini-0.1a3/llm_gemini.egg-info/PKG-INFO` & `llm_gemini-0.1a4/llm_gemini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-gemini
-Version: 0.1a3
+Version: 0.1a4
 Summary: LLM plugin to access Google's Gemini family of models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-gemini
 Project-URL: Changelog, https://github.com/simonw/llm-gemini/releases
 Project-URL: Issues, https://github.com/simonw/llm-gemini/issues
 Project-URL: CI, https://github.com/simonw/llm-gemini/actions
```

### Comparing `llm-gemini-0.1a3/llm_gemini.py` & `llm_gemini-0.1a4/llm_gemini.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ]
 
 
 @llm.hookimpl
 def register_models(register):
     register(GeminiPro("gemini-pro"))
     register(GeminiPro("gemini-1.5-pro-latest"))
+    register(GeminiPro("gemini-1.5-flash-latest"))
 
 
 class GeminiPro(llm.Model):
     can_stream = True
 
     def __init__(self, model_id):
         self.model_id = model_id
```

### Comparing `llm-gemini-0.1a3/pyproject.toml` & `llm_gemini-0.1a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-gemini"
-version = "0.1a3"
+version = "0.1a4"
 description = "LLM plugin to access Google's Gemini family of models"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

