# Comparing `tmp/pleonasty-0.0.5.tar.gz` & `tmp/pleonasty-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pleonasty-0.0.5.tar", last modified: Thu Apr 25 19:23:07 2024, max compression
+gzip compressed data, was "pleonasty-0.0.6.tar", last modified: Tue May 14 11:47:53 2024, max compression
```

## Comparing `pleonasty-0.0.5.tar` & `pleonasty-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 19:23:07.203661 pleonasty-0.0.5/
--rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1385 2024-04-25 19:23:07.202661 pleonasty-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.5/README.MD
--rw-rw-rw-   0        0        0      830 2024-04-25 19:22:09.000000 pleonasty-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 19:23:07.204659 pleonasty-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 19:23:07.166143 pleonasty-0.0.5/src/
--rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 19:23:07.196658 pleonasty-0.0.5/src/pleonasty.egg-info/
--rw-rw-rw-   0        0        0     1385 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14643 2024-04-25 19:21:42.000000 pleonasty-0.0.5/src/pleonasty.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:47:53.641718 pleonasty-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1385 2024-05-14 11:47:53.640718 pleonasty-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.6/README.MD
+-rw-rw-rw-   0        0        0      830 2024-05-14 11:47:31.000000 pleonasty-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 11:47:53.641718 pleonasty-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 11:47:53.634718 pleonasty-0.0.6/src/
+-rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:47:53.640718 pleonasty-0.0.6/src/pleonasty.egg-info/
+-rw-rw-rw-   0        0        0     1385 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14839 2024-05-14 11:15:26.000000 pleonasty-0.0.6/src/pleonasty.py
```

### Comparing `pleonasty-0.0.5/LICENSE` & `pleonasty-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.5/PKG-INFO` & `pleonasty-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.5
+Version: 0.0.6
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.5/README.MD` & `pleonasty-0.0.6/README.MD`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.5/pyproject.toml` & `pleonasty-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 
 name = "pleonasty"
 
-version = "0.0.5"
+version = "0.0.6"
 
 authors = [
   { name="Ryan L. Boyd", email="ryan@ryanboyd.io" },
 ]
 
 description = "A very simple abstraction for LLMs to get single responses to a given input."
```

### Comparing `pleonasty-0.0.5/src/pleonasty.egg-info/PKG-INFO` & `pleonasty-0.0.6/src/pleonasty.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.5
+Version: 0.0.6
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.5/src/pleonasty.py` & `pleonasty-0.0.6/src/pleonasty.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,17 @@
         sequences = self.pipeline(
             prompt_messages,
             do_sample=True,
             temperature=temperature,
             top_k=top_k,
             num_return_sequences=1,
             eos_token_id=self.tokenizer.eos_token_id,
-            max_length=max_seq_length)
+            pad_token_id=self.tokenizer.eos_token_id,
+            max_length=max_seq_length,
+        )
 
         return sequences
 
     def analyze_text(self,
                      input_text: str,
                      max_seq_length: int = 4096,
                      temperature: float = 0.3,
@@ -330,15 +332,17 @@
             raise MessageContextException("It appears that your prompt set is not a list of dictionaries.")
 
         for item in prompt_messages:
             if not isinstance(item, dict):
                 raise MessageContextException("""Your prompt set need to be contained in dictionaries.
                          Each dictionary must have both a "role" and "content" key.""")
 
-        return self.tokenizer.apply_chat_template(prompt_messages,  tokenize=False)
+        return self.tokenizer.apply_chat_template(prompt_messages, 
+                                                  tokenize=False,
+                                                  add_generation_prompt=True)
 
 
 
 # some potential stuff for parsing jsons
 #import ast
 #import json
 #from pprint import pprint
```

