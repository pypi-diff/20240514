# Comparing `tmp/funkai-0.7.tar.gz` & `tmp/funkai-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funkai-0.7.tar", last modified: Wed Apr  3 18:31:54 2024, max compression
+gzip compressed data, was "funkai-0.8.tar", last modified: Tue May 14 06:00:52 2024, max compression
```

## Comparing `funkai-0.7.tar` & `funkai-0.8.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-04-03 18:31:54.716529 funkai-0.7/
--rw-r--r--   0 sameer     (502) staff       (20)     4876 2024-04-03 18:31:54.716286 funkai-0.7/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-04-03 18:27:26.000000 funkai-0.7/README.md
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-04-03 18:31:54.715002 funkai-0.7/funkai/
--rw-r--r--   0 sameer     (502) staff       (20)       36 2024-03-10 16:49:11.000000 funkai-0.7/funkai/__init__.py
--rw-r--r--   0 sameer     (502) staff       (20)     7408 2024-04-03 18:15:57.000000 funkai-0.7/funkai/core.py
--rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-0.7/funkai/examples.py
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-04-03 18:31:54.715911 funkai-0.7/funkai.egg-info/
--rw-r--r--   0 sameer     (502) staff       (20)     4876 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)      220 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/SOURCES.txt
--rw-r--r--   0 sameer     (502) staff       (20)        1 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/dependency_links.txt
--rw-r--r--   0 sameer     (502) staff       (20)       17 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/requires.txt
--rw-r--r--   0 sameer     (502) staff       (20)        7 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/top_level.txt
--rw-r--r--   0 sameer     (502) staff       (20)       38 2024-04-03 18:31:54.716589 funkai-0.7/setup.cfg
--rw-r--r--   0 sameer     (502) staff       (20)      557 2024-04-03 18:27:57.000000 funkai-0.7/setup.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-14 06:00:52.192613 funkai-0.8/
+-rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-14 06:00:52.192350 funkai-0.8/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-05-14 06:00:28.000000 funkai-0.8/README.md
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-14 06:00:52.190957 funkai-0.8/funkai/
+-rw-r--r--   0 sameer     (502) staff       (20)       61 2024-05-14 06:00:28.000000 funkai-0.8/funkai/__init__.py
+-rw-r--r--   0 sameer     (502) staff       (20)      199 2024-05-14 06:00:28.000000 funkai-0.8/funkai/claude.py
+-rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-0.8/funkai/examples.py
+-rw-r--r--   0 sameer     (502) staff       (20)     6471 2024-05-14 06:00:28.000000 funkai-0.8/funkai/funk.py
+-rw-r--r--   0 sameer     (502) staff       (20)     1639 2024-05-14 06:00:28.000000 funkai-0.8/funkai/manager.py
+-rw-r--r--   0 sameer     (502) staff       (20)      190 2024-05-14 06:00:28.000000 funkai-0.8/funkai/openai.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-14 06:00:52.191852 funkai-0.8/funkai.egg-info/
+-rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)      272 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        1 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       24 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/requires.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        7 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/top_level.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       38 2024-05-14 06:00:52.192664 funkai-0.8/setup.cfg
+-rw-r--r--   0 sameer     (502) staff       (20)      567 2024-05-14 06:00:28.000000 funkai-0.8/setup.py
```

### Comparing `funkai-0.7/PKG-INFO` & `funkai-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.7
+Version: 0.8
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
+Requires-Dist: claude
 
 # Funkai Library
 
 Funkai is a Python library that encapsulates linguistic operations and uses OpenAI to perform them based on user inputs.
 
 ## Features
```

### Comparing `funkai-0.7/README.md` & `funkai-0.8/README.md`

 * *Files identical despite different names*

### Comparing `funkai-0.7/funkai/core.py` & `funkai-0.8/funkai/funk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,56 @@
-import openai
-import ast
 import os
+import ast
+import openai
+import anthropic
 
 class Funk:
-    def __init__(self, name, operation, api_key, retry_count=0, input_dtype=str, output_dtype=str, model="gpt-3.5-turbo-16k"):
+    def __init__(self, provider, name, operation, api_key, model, options, retry_count=0, input_dtype=str, output_dtype=str):
         self.name = name
         self.operation = operation
         self.input_dtype = input_dtype
         self.output_dtype = output_dtype
         self.retry_count = retry_count
         self.model = model
         self.error = False
+        self.provider = provider
+        self.options = options
         self.set_api_key(api_key)
         self.restricted_models(model)
 
     def set_api_key(self, key):
-        os.environ['OPENAI_API_KEY'] = key
-        openai.api_key = key
-        self.check_api_key()
-
-    def restricted_models(self, value):
-        restricted_values = ['gpt-3.5-turbo-16k', 'gpt-3.5-turbo-1106', 'gpt-3.5-turbo-16k-0613',
-                             'gpt-3.5-turbo', 'gpt-3.5-turbo-0125', 'gpt-4-0613', 'gpt-3.5-turbo-0301', 
-                             'gpt-3.5-turbo-0613', 'gpt-3.5-turbo-instruct-0914', 'gpt-4', 
-                             'gpt-3.5-turbo-instruct', 'gpt-4-1106-preview', 'gpt-4-vision-preview',
-                             'gpt-4-0125-preview', 'gpt-4-turbo-preview']
-        
-        if value not in restricted_values:
-            self.error = True
-            print("Model value is not allowed. Please choose from:", restricted_values)
-  
-    def check_api_key(self):
-        if not openai.api_key and 'OPENAI_API_KEY' not in os.environ:
-            self.error = True
+        if not key:
             raise ValueError("OpenAI API Key not set. Set the key using Funk.set_api_key('YOUR_API_KEY').")
-        elif 'LLMONITOR_APP_ID' in os.environ:
+        
+        if self.provider == 'openai':
+            openai.api_key = key
+        else:
+            self.api_key = key
+
+        if 'LLMONITOR_APP_ID' in os.environ:
             try:
                 from llmonitor import monitor
                 monitor(openai)
             except ImportError:
                 self.error = True
                 print("LLMONITOR_APP_ID is set but llmonitor is not installed. Install llmonitor and rerun.")
 
+    def restricted_models(self, value):
+        if self.provider == 'openai':
+            restricted_values = ['gpt-3.5-turbo-16k', 'gpt-3.5-turbo-1106', 'gpt-3.5-turbo-16k-0613',
+                                'gpt-3.5-turbo', 'gpt-3.5-turbo-0125', 'gpt-4-0613', 'gpt-3.5-turbo-0301', 
+                                'gpt-3.5-turbo-0613', 'gpt-3.5-turbo-instruct-0914', 'gpt-4', 
+                                'gpt-3.5-turbo-instruct', 'gpt-4-1106-preview', 'gpt-4-vision-preview',
+                                'gpt-4-0125-preview', 'gpt-4-turbo-preview']
+        else: 
+            restricted_values = ['claude-3-opus-20240229', 'claude-3-sonnet-20240229', 'claude-3-haiku-20240307']
+
+        if value not in restricted_values:
+            print("Model value is not allowed. Please choose from:", restricted_values)
+  
     def _prepare_messages(self, sys_cont, examples, input_content):
         user_messages = [
             {"role": "user", "content": f"Operation: {self.operation}\nInput: {str(ex)}\nOutput data type: {self.output_dtype}"}
             for ex in examples
         ]
         user_messages.append({"role": "user", "content": f"Operation: {self.operation}\nInput: {input_content}\nOutput data type: {self.output_dtype}"})
         assistant_messages = [
@@ -54,62 +59,79 @@
         ]
         return [{"role": "system", "content": sys_cont}] + user_messages + assistant_messages
 
     def _funkai_main(self, sys_cont, examples, input_content):
         messages = self._prepare_messages(sys_cont, examples, input_content)
         max_tokens = 1000 if len(messages) > 1 else 500
 
-        gpt_response = False
-
         try:
-            gpt_response = openai.chat.completions.create(
-                model=self.model,
-                messages=messages,
-                temperature=0.7,
-                max_tokens=max_tokens
-            )
+            options = {
+                'temperature': self.options.get('temperature', 0.7),
+                'max_tokens': self.options.get('max_tokens', max_tokens),
+            }
+
+            if self.provider == 'openai':
+                response = openai.chat.completions.create(
+                    model=self.model,
+                    messages=messages,
+                    **options
+                )
+            else:
+                system = messages[0]['content']
+                del messages[0]
 
-            return gpt_response
-        
-        except openai.OpenAIError:
+                client = anthropic.Anthropic(api_key=self.api_key)
+                response = client.messages.create(
+                    model=self.model,
+                    messages=messages,
+                    system=str(system),
+                    **options
+                )
+
+            return response
+
+        except (openai.OpenAIError, Exception) as e:
             if self.retry_count > 0:
                 self.retry_count -= 1
                 return self._funkai_main(sys_cont, examples, input_content)
             else:
-                return openai.APIError
-
+                raise e
 
     def run(self, input_content, examples=None, full_resp=False):
         if not isinstance(input_content, self.input_dtype):
             raise TypeError(f"Expected input of type {self.input_dtype}, but got {type(input_content)}")
 
         system_content = """Act as a python program. Process the input based on the operation provided and produce an output. 
         Ensure the output matches the specified Python data type because the result will be interpreted as a Python literal. 
         The output must only be the response with no explanation."""
 
         examples = examples or {}
 
         raw_output = self._funkai_main(system_content, examples, str(input_content))
         raw_output_str = Funk._clean_gpt_response(raw_output)
 
-        if full_resp:
-            try:
-                return Funk._convert_output(raw_output_str, self.output_dtype), raw_output
-            except ValueError:
-                raise TypeError(f"Failed to convert output to {self.output_dtype}. Raw output: {raw_output_str}")
-        else:
-            try:
-                return Funk._convert_output(raw_output_str, self.output_dtype)
-            except ValueError:
-                raise TypeError(f"Failed to convert output to {self.output_dtype}. Raw output: {raw_output_str}")
-                
+        try:
+            converted_output = Funk._convert_output(raw_output_str, self.output_dtype)
+            if full_resp:
+                return converted_output, raw_output
+            else:
+                return converted_output
+        except ValueError as ve:
+            self.error = True
+            raise TypeError(f"Failed to convert output to {self.output_dtype}. Raw output: {raw_output_str}. Error: {ve}")
+
 
     @staticmethod
     def _clean_gpt_response(response):
-        return response.choices[0].message.content
+        if hasattr(response, 'content') and response.content:
+            return response.content[0].text
+        elif hasattr(response, 'choices') and response.choices:
+            return response.choices[0].message.content
+        else:
+            return None 
 
     @staticmethod
     def _convert_output(output_str, target_dtype):
         def _convert(eval_func, err_message):
             try:
                 return eval_func(output_str)
             except (ValueError, SyntaxError):
@@ -123,57 +145,7 @@
             return _convert(lambda x: target_dtype(ast.literal_eval(x)), "invalid syntax")
         elif target_dtype == range:
             return _convert(lambda x: range(*ast.literal_eval(x)) if isinstance(ast.literal_eval(x), (list, tuple)) and len(ast.literal_eval(x)) in [1, 2, 3] else ValueError, "invalid range syntax")
         elif target_dtype == str:
             return output_str
         else:
             return _convert(target_dtype, "conversion error")
-
-class FunkManager:
-    def __init__(self, api_key, model="gpt-3.5-turbo"):
-        self.api_key = api_key
-        self.model = model
-        self.funks = {}
-
-    def add(self, name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str):
-        if api_key is None:
-            api_key = self.api_key
-        if model is None:
-            model = self.model
-
-        if name in self.funks:
-            raise ValueError(f"A Funk with name '{name}' already exists.")
-        new_funk = Funk(name, operation, api_key, retry_count, input_dtype, output_dtype, model)
-        if new_funk.error:
-            raise ValueError("Invalid Funk Parameters.")
-        else:
-            self.funks[name] = new_funk
-
-    def update(self, name, **kwargs):
-        funk = self._get(name)
-        if not funk:
-            raise ValueError(f"No Funk with name '{name}' found.")
-        
-        for key, value in kwargs.items():
-            if hasattr(funk, key):
-                setattr(funk, key, value)
-            else:
-                raise ValueError(f"Invalid parameter '{key}' for Funk instance.")
-
-        self.funks[name] = funk
-        
-    def _get(self, name):
-        return self.funks.get(name, None)
-
-    def remove(self, name):
-        if name not in self.funks:
-            raise ValueError(f"No Funk with name '{name}' found.")
-        del self.funks[name]
-
-    def run(self, name, input_content, examples=None, full_resp=False):
-        funk = self._get(name)
-        if not funk:
-            raise ValueError(f"No Funk with name '{name}' found.")
-        return funk.run(input_content, examples, full_resp)
-
-    def show(self):
-        return list(self.funks.keys())
```

### Comparing `funkai-0.7/funkai/examples.py` & `funkai-0.8/funkai/examples.py`

 * *Files identical despite different names*

### Comparing `funkai-0.7/funkai.egg-info/PKG-INFO` & `funkai-0.8/funkai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.7
+Version: 0.8
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
+Requires-Dist: claude
 
 # Funkai Library
 
 Funkai is a Python library that encapsulates linguistic operations and uses OpenAI to perform them based on user inputs.
 
 ## Features
```

### Comparing `funkai-0.7/setup.py` & `funkai-0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="funkai",
-    version="0.7",
+    version="0.8",
     packages=find_packages(),
     install_requires=[
-        "openai",  'llmonitor'
+        "openai",  'llmonitor', 'claude'
     ],
     author="Ciara Adkins",
     author_email="adkins.ciara@gmail.com.com",
     description="Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/ciaraadkins/funkai",
```

