# Comparing `tmp/genai_apis-0.0.5-py3-none-any.whl.zip` & `tmp/genai_apis-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8849 bytes, number of entries: 11
--rw-r--r--  2.0 unx       91 b- defN 24-May-14 08:01 genai_apis/__init__.py
+Zip file size: 8856 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       91 b- defN 24-May-14 08:06 genai_apis/__init__.py
 -rw-r--r--  2.0 unx      265 b- defN 24-May-07 01:51 genai_apis/abstract.py
 -rw-r--r--  2.0 unx      819 b- defN 24-May-07 01:51 genai_apis/anthropic_api.py
 -rw-r--r--  2.0 unx     2905 b- defN 24-May-03 05:23 genai_apis/factory.py
--rw-r--r--  2.0 unx     1680 b- defN 24-May-14 08:01 genai_apis/gemini_api.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-14 08:06 genai_apis/gemini_api.py
 -rw-r--r--  2.0 unx      790 b- defN 24-May-07 01:51 genai_apis/openai_api.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1672 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      879 b- defN 24-May-14 08:02 genai_apis-0.0.5.dist-info/RECORD
-11 files, 20561 bytes uncompressed, 7363 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-14 08:06 genai_apis-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1672 b- defN 24-May-14 08:06 genai_apis-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 08:06 genai_apis-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-14 08:06 genai_apis-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      879 b- defN 24-May-14 08:06 genai_apis-0.0.6.dist-info/RECORD
+11 files, 20610 bytes uncompressed, 7370 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: genai_apis/gemini_api.py
 Comment: 
 
 Filename: genai_apis/openai_api.py
 Comment: 
 
-Filename: genai_apis-0.0.5.dist-info/LICENSE
+Filename: genai_apis-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: genai_apis-0.0.5.dist-info/METADATA
+Filename: genai_apis-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: genai_apis-0.0.5.dist-info/WHEEL
+Filename: genai_apis-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: genai_apis-0.0.5.dist-info/top_level.txt
+Filename: genai_apis-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: genai_apis-0.0.5.dist-info/RECORD
+Filename: genai_apis-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genai_apis/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 from genai_apis.factory import APIFactory
 
 __all__ = ["APIFactory"]
```

## genai_apis/gemini_api.py

```diff
@@ -33,16 +33,17 @@
         else:
             return response.text
 
 
 class GeminiVertexAPI(TextGenerationAPI):
     async def generate_text(self, model, prompt, system_instruction=None, **kwargs):
         from vertexai.generative_models import GenerativeModel
+        from vertexai import generative_models
 
-        generation_config = GenerativeModel.GenerationConfig(**kwargs)
+        generation_config = generative_models.GenerationConfig(**kwargs)
         model = GenerativeModel(model_name=model, system_instruction=system_instruction)
         response = await model.generate_content_async(
             [prompt], generation_config=generation_config
         )
 
         if "stream" in kwargs and kwargs["stream"] is True:
             return _get_stream_outputs(response)
```

## Comparing `genai_apis-0.0.5.dist-info/LICENSE` & `genai_apis-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genai_apis-0.0.5.dist-info/METADATA` & `genai_apis-0.0.6.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genai-apis
-Version: 0.0.5
+Version: 0.0.6
 Summary: GenAI APIs provides a unified API callers to Gemini API, OpenAI API, and Anthropic API.
 Home-page: https://github.com/deep-diver/genai-apis
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: genai
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `genai_apis-0.0.5.dist-info/RECORD` & `genai_apis-0.0.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-genai_apis/__init__.py,sha256=ZgkdS9YdryLVPxEvrXjx11dFxQEPWj4rVZabv8qrCZA,91
+genai_apis/__init__.py,sha256=Tx_HRvTUMjQdl9Nh0Dd_cpQOFO_xudGU4ztaiMQbsmc,91
 genai_apis/abstract.py,sha256=a54RxTFFfSWuoO2r8-rIjRpcXcD3LBmEchwPZNCzP7U,265
 genai_apis/anthropic_api.py,sha256=nprzpxgta3ubIY6eQuvaXEz8eA-9WoNxcZUFG17jGlQ,819
 genai_apis/factory.py,sha256=sJgX-cUGVb5c-i7bYjofYAVbEVXqWVnFflURO5C9PIA,2905
-genai_apis/gemini_api.py,sha256=LqejXTZAr0l6D7tiGAorCyxca4999LOqVNqHvyjj2Sk,1680
+genai_apis/gemini_api.py,sha256=1pkPPY0AGQtGrkZX9yTTE2Vt2ECCccX0FkdbZSekuU8,1729
 genai_apis/openai_api.py,sha256=Uu_i7Mo8KObH7PxkVDxSz5C9tKLhOuW5yMm1ShLTMVM,790
-genai_apis-0.0.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-genai_apis-0.0.5.dist-info/METADATA,sha256=v6l_QWfuRcGXSPA4yafMY3JGz3OuHf7OrgXZMxUmhkw,1672
-genai_apis-0.0.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-genai_apis-0.0.5.dist-info/top_level.txt,sha256=lxy-j5IOQHvkO1zMVLruWLnxQapKtnD_0P9_F_z8cKc,11
-genai_apis-0.0.5.dist-info/RECORD,,
+genai_apis-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+genai_apis-0.0.6.dist-info/METADATA,sha256=ZiNdbNsoJxxcCrr2d8D7cWy8uOETuYaUWqzh_V7BA8k,1672
+genai_apis-0.0.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+genai_apis-0.0.6.dist-info/top_level.txt,sha256=lxy-j5IOQHvkO1zMVLruWLnxQapKtnD_0P9_F_z8cKc,11
+genai_apis-0.0.6.dist-info/RECORD,,
```

