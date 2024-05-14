# Comparing `tmp/genai_apis-0.0.4-py3-none-any.whl.zip` & `tmp/genai_apis-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8809 bytes, number of entries: 11
--rw-r--r--  2.0 unx       91 b- defN 24-May-07 06:15 genai_apis/__init__.py
+Zip file size: 8849 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       91 b- defN 24-May-14 08:01 genai_apis/__init__.py
 -rw-r--r--  2.0 unx      265 b- defN 24-May-07 01:51 genai_apis/abstract.py
 -rw-r--r--  2.0 unx      819 b- defN 24-May-07 01:51 genai_apis/anthropic_api.py
 -rw-r--r--  2.0 unx     2905 b- defN 24-May-03 05:23 genai_apis/factory.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-07 01:51 genai_apis/gemini_api.py
+-rw-r--r--  2.0 unx     1680 b- defN 24-May-14 08:01 genai_apis/gemini_api.py
 -rw-r--r--  2.0 unx      790 b- defN 24-May-07 01:51 genai_apis/openai_api.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1672 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      879 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/RECORD
-11 files, 20324 bytes uncompressed, 7323 bytes compressed:  64.0%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1672 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      879 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/RECORD
+11 files, 20561 bytes uncompressed, 7363 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: genai_apis/gemini_api.py
 Comment: 
 
 Filename: genai_apis/openai_api.py
 Comment: 
 
-Filename: genai_apis-0.0.4.dist-info/LICENSE
+Filename: genai_apis-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: genai_apis-0.0.4.dist-info/METADATA
+Filename: genai_apis-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: genai_apis-0.0.4.dist-info/WHEEL
+Filename: genai_apis-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: genai_apis-0.0.4.dist-info/top_level.txt
+Filename: genai_apis-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: genai_apis-0.0.4.dist-info/RECORD
+Filename: genai_apis-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genai_apis/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 from genai_apis.factory import APIFactory
 
 __all__ = ["APIFactory"]
```

## genai_apis/gemini_api.py

```diff
@@ -15,29 +15,36 @@
             yield word
 
 
 class GeminiAPI(TextGenerationAPI):
     async def generate_text(self, model, prompt, system_instruction=None, **kwargs):
         import google.generativeai as genai
 
+        generation_config = genai.types.GenerationConfig(**kwargs)
+
         model = genai.GenerativeModel(
             model_name=model, system_instruction=system_instruction
         )
-        response = await model.generate_content_async([prompt], **kwargs)
+        response = await model.generate_content_async(
+            [prompt], generation_config=generation_config
+        )
 
         if "stream" in kwargs and kwargs["stream"] is True:
             return _get_stream_outputs(response)
         else:
             return response.text
 
 
 class GeminiVertexAPI(TextGenerationAPI):
     async def generate_text(self, model, prompt, system_instruction=None, **kwargs):
         from vertexai.generative_models import GenerativeModel
 
+        generation_config = GenerativeModel.GenerationConfig(**kwargs)
         model = GenerativeModel(model_name=model, system_instruction=system_instruction)
-        response = await model.generate_content_async([prompt], **kwargs)
+        response = await model.generate_content_async(
+            [prompt], generation_config=generation_config
+        )
 
         if "stream" in kwargs and kwargs["stream"] is True:
             return _get_stream_outputs(response)
         else:
             return response.text
```

## Comparing `genai_apis-0.0.4.dist-info/LICENSE` & `genai_apis-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genai_apis-0.0.4.dist-info/METADATA` & `genai_apis-0.0.5.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genai-apis
-Version: 0.0.4
+Version: 0.0.5
 Summary: GenAI APIs provides a unified API callers to Gemini API, OpenAI API, and Anthropic API.
 Home-page: https://github.com/deep-diver/genai-apis
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: genai
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

