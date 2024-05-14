# Comparing `tmp/simplerllm-0.2.1.tar.gz` & `tmp/simplerllm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplerllm-0.2.1.tar", last modified: Sat May  4 19:39:55 2024, max compression
+gzip compressed data, was "simplerllm-0.2.3.tar", last modified: Tue May 14 10:21:31 2024, max compression
```

## Comparing `simplerllm-0.2.1.tar` & `simplerllm-0.2.3.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.042584 simplerllm-0.2.1/
--rw-rw-rw-   0        0        0     6963 2024-05-04 19:39:55.040074 simplerllm-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:54.977519 simplerllm-0.2.1/SimplerLLM/
--rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/image/
--rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/image/__init__.py
--rw-rw-rw-   0        0        0     1227 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/image/img_helper_funcs.py
--rw-rw-rw-   0        0        0     2080 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/image/stability_ai.py
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/language/
--rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/__init__.py
--rw-rw-rw-   0        0        0     1851 2024-05-04 14:03:11.000000 simplerllm-0.2.1/SimplerLLM/language/embeddings.py
--rw-rw-rw-   0        0        0     6422 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm.py
--rw-rw-rw-   0        0        0     2922 2024-05-01 19:46:15.000000 simplerllm-0.2.1/SimplerLLM/language/llm_addons.py
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/language/llm_providers/
--rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     5361 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/anthropic_llm.py
--rw-rw-rw-   0        0        0     8566 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/gemini_llm.py
--rw-rw-rw-   0        0        0      341 2024-05-01 19:22:49.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/llm_response_models.py
--rw-rw-rw-   0        0        0     7871 2024-05-04 14:03:09.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/openai_llm.py
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/prompts/
--rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/prompts/__init__.py
--rw-rw-rw-   0        0        0     3132 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/prompts/prompt_builder.py
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.040074 simplerllm-0.2.1/SimplerLLM/tools/
--rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/__init__.py
--rw-rw-rw-   0        0        0      949 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/file_loader.py
--rw-rw-rw-   0        0        0     6006 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/generic_loader.py
--rw-rw-rw-   0        0        0     6064 2024-05-01 19:40:59.000000 simplerllm-0.2.1/SimplerLLM/tools/json_helpers.py
--rw-rw-rw-   0        0        0     4988 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/rapid_api.py
--rw-rw-rw-   0        0        0     7138 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/serp.py
--rw-rw-rw-   0        0        0     8693 2024-05-04 19:16:42.000000 simplerllm-0.2.1/SimplerLLM/tools/text_chunker.py
-drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.040074 simplerllm-0.2.1/SimplerLLM.egg-info/
--rw-rw-rw-   0        0        0     6963 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 19:39:55.042584 simplerllm-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1473 2024-05-04 13:44:30.000000 simplerllm-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.941261 simplerllm-0.2.3/
+-rw-rw-rw-   0        0        0     1095 2024-05-13 19:15:16.000000 simplerllm-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     7000 2024-05-14 10:21:31.941261 simplerllm-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.905892 simplerllm-0.2.3/SimplerLLM/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.931152 simplerllm-0.2.3/SimplerLLM/image/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/image/__init__.py
+-rw-rw-rw-   0        0        0     1227 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/image/img_helper_funcs.py
+-rw-rw-rw-   0        0        0     2080 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/image/stability_ai.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.933152 simplerllm-0.2.3/SimplerLLM/language/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/language/__init__.py
+-rw-rw-rw-   0        0        0     1851 2024-05-04 14:03:11.000000 simplerllm-0.2.3/SimplerLLM/language/embeddings.py
+-rw-rw-rw-   0        0        0     6426 2024-05-05 18:44:17.000000 simplerllm-0.2.3/SimplerLLM/language/llm.py
+-rw-rw-rw-   0        0        0     5208 2024-05-14 09:32:17.000000 simplerllm-0.2.3/SimplerLLM/language/llm_addons.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.935152 simplerllm-0.2.3/SimplerLLM/language/llm_providers/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/language/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     5357 2024-05-14 09:20:43.000000 simplerllm-0.2.3/SimplerLLM/language/llm_providers/anthropic_llm.py
+-rw-rw-rw-   0        0        0     8566 2024-05-14 09:22:56.000000 simplerllm-0.2.3/SimplerLLM/language/llm_providers/gemini_llm.py
+-rw-rw-rw-   0        0        0      341 2024-05-01 19:22:49.000000 simplerllm-0.2.3/SimplerLLM/language/llm_providers/llm_response_models.py
+-rw-rw-rw-   0        0        0     7871 2024-05-04 14:03:09.000000 simplerllm-0.2.3/SimplerLLM/language/llm_providers/openai_llm.py
+-rw-rw-rw-   0        0        0     2306 2024-05-05 18:44:09.000000 simplerllm-0.2.3/SimplerLLM/language/llm_providers/transformers_llm.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.936255 simplerllm-0.2.3/SimplerLLM/prompts/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3132 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/prompts/prompt_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.940261 simplerllm-0.2.3/SimplerLLM/tools/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/tools/__init__.py
+-rw-rw-rw-   0        0        0     1383 2024-05-13 19:19:25.000000 simplerllm-0.2.3/SimplerLLM/tools/file_functions.py
+-rw-rw-rw-   0        0        0      949 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/tools/file_loader.py
+-rw-rw-rw-   0        0        0     6006 2024-05-13 15:36:50.000000 simplerllm-0.2.3/SimplerLLM/tools/generic_loader.py
+-rw-rw-rw-   0        0        0     6025 2024-05-06 19:36:50.000000 simplerllm-0.2.3/SimplerLLM/tools/json_helpers.py
+-rw-rw-rw-   0        0        0     4988 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/tools/rapid_api.py
+-rw-rw-rw-   0        0        0     7138 2024-04-16 12:35:00.000000 simplerllm-0.2.3/SimplerLLM/tools/serp.py
+-rw-rw-rw-   0        0        0     8713 2024-05-14 10:14:29.000000 simplerllm-0.2.3/SimplerLLM/tools/text_chunker.py
+-rw-rw-rw-   0        0        0     1424 2024-05-06 20:07:45.000000 simplerllm-0.2.3/SimplerLLM/tools/web_crawler.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:31.940261 simplerllm-0.2.3/SimplerLLM.egg-info/
+-rw-rw-rw-   0        0        0     7000 2024-05-14 10:21:31.000000 simplerllm-0.2.3/SimplerLLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2024-05-14 10:21:31.000000 simplerllm-0.2.3/SimplerLLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 10:21:31.000000 simplerllm-0.2.3/SimplerLLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2024-05-14 10:21:31.000000 simplerllm-0.2.3/SimplerLLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 10:21:31.000000 simplerllm-0.2.3/SimplerLLM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 10:21:31.941261 simplerllm-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2024-05-14 10:20:37.000000 simplerllm-0.2.3/setup.py
```

### Comparing `simplerllm-0.2.1/PKG-INFO` & `simplerllm-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: SimplerLLM
-Version: 0.2.1
+Version: 0.2.3
 Summary: An easy-to-use Library for interacting with language models.
 Home-page: https://github.com/hassancs91/SimplerLLM
 Author: Hasan Aboul Hasan
 Author-email: hasan@learnwithhasan.com
+License: MIT
 Keywords: text generation,openai,LLM,RAG
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -16,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp==3.9.4
 Requires-Dist: duckduckgo_search==5.3.0
 Requires-Dist: newspaper3k==0.2.8
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openai==1.25.0
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: PyPDF2==3.0.1
```

### Comparing `simplerllm-0.2.1/SimplerLLM/image/img_helper_funcs.py` & `simplerllm-0.2.3/SimplerLLM/image/img_helper_funcs.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/image/stability_ai.py` & `simplerllm-0.2.3/SimplerLLM/image/stability_ai.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/language/embeddings.py` & `simplerllm-0.2.3/SimplerLLM/language/embeddings.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/language/llm.py` & `simplerllm-0.2.3/SimplerLLM/language/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,7 +200,9 @@
                 "messages": messages,
                 "system_prompt": system_prompt,
                 "max_tokens": max_tokens,
                 "full_response": full_response,
             }
         )
         return await anthropic_llm.generate_response_async(**params)
+
+
```

### Comparing `simplerllm-0.2.1/SimplerLLM/language/llm_providers/anthropic_llm.py` & `simplerllm-0.2.3/SimplerLLM/language/llm_providers/anthropic_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import requests
 from .llm_response_models import LLMFullResponse
 
 # Load environment variables
 load_dotenv()
 
 # Constants
-CLAUDE_API_KEY = os.getenv("CLAUDE_API_KEY", "")
+ANTHROPIC_API_KEY = os.getenv("ANTHROPIC_API_KEY", "")
 MAX_RETRIES = int(os.getenv("MAX_RETRIES", 3))
 RETRY_DELAY = int(os.getenv("RETRY_DELAY", 2))
 
 
 def generate_response(
     model_name: str,
     prompt: Optional[str] = None,
@@ -42,15 +42,15 @@
         if prompt is not None:
             raise ValueError("Only one of 'prompt' or 'messages' should be provided.")
         messages = messages
 
     # Define the URL and headers
     url = "https://api.anthropic.com/v1/messages"
     headers = {
-        "x-api-key": CLAUDE_API_KEY,
+        "x-api-key": ANTHROPIC_API_KEY,
         "anthropic-version": "2023-06-01",
         "content-type": "application/json",
     }
 
     # Create the data payload
     payload = {
         "model": model_name,
@@ -73,15 +73,15 @@
                     process_time=time.time() - start_time,
                     llm_provider_response=response.json(),
                 )
 
             else:
                 return response.json()["content"][0]["text"]
 
-        except requests.RequestException as e:
+        except Exception as e:
             print(f"Attempt {attempt + 1} failed: {e}")
             time.sleep(retry_delay)
             retry_delay *= 2  # Double the delay each retry
 
     print("All retry attempts failed.")
     return None
 
@@ -112,15 +112,15 @@
         if prompt is not None:
             raise ValueError("Only one of 'prompt' or 'messages' should be provided.")
         messages = messages
 
     # Define the URL and headers
     url = "https://api.anthropic.com/v1/messages"
     headers = {
-        "x-api-key": CLAUDE_API_KEY,
+        "x-api-key": ANTHROPIC_API_KEY,
         "anthropic-version": "2023-06-01",
         "content-type": "application/json",
     }
 
     # Create the data payload
     payload = {
         "model": model_name,
```

### Comparing `simplerllm-0.2.1/SimplerLLM/language/llm_providers/gemini_llm.py` & `simplerllm-0.2.3/SimplerLLM/language/llm_providers/gemini_llm.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/language/llm_providers/openai_llm.py` & `simplerllm-0.2.3/SimplerLLM/language/llm_providers/openai_llm.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/prompts/prompt_builder.py` & `simplerllm-0.2.3/SimplerLLM/prompts/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/tools/file_loader.py` & `simplerllm-0.2.3/SimplerLLM/tools/file_loader.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/tools/generic_loader.py` & `simplerllm-0.2.3/SimplerLLM/tools/generic_loader.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/tools/json_helpers.py` & `simplerllm-0.2.3/SimplerLLM/tools/json_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 
 
 def convert_json_to_pydantic_model(model_class, json_data):
     try:
         model_instance = model_class(**json_data)
         return model_instance
     except ValidationError as e:
-        print("Validation error:", e)
         return None
 
 
 # Define a function to provide example values based on type
 def example_value_for_type(field_type: Type):
     origin = get_origin(field_type)
     if origin is None:  # Not a generic type
```

### Comparing `simplerllm-0.2.1/SimplerLLM/tools/rapid_api.py` & `simplerllm-0.2.3/SimplerLLM/tools/rapid_api.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/tools/serp.py` & `simplerllm-0.2.3/SimplerLLM/tools/serp.py`

 * *Files identical despite different names*

### Comparing `simplerllm-0.2.1/SimplerLLM/tools/text_chunker.py` & `simplerllm-0.2.3/SimplerLLM/tools/text_chunker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     text: str
     num_characters: int = Field(description="Number of characters in the chunk")
     num_words: int = Field(description="Number of words in the chunk")
 
 
 class TextChunks(BaseModel):
     num_chunks: int = Field(description="Total number of chunks")
-    chunks: List[ChunkInfo]
+    chunk_list: List[ChunkInfo]
 
 
 def chunk_by_max_chunk_size(
     text: str, max_chunk_size: int, preserve_sentence_structure: bool = False
 ) -> TextChunks:
     """
     Split the given text into chunks based on the maximum chunk size trying to reserve sentence endings if preserve_sentence_structure is enabled
@@ -72,15 +72,15 @@
         chunks.append(current_chunk.strip())
 
     chunk_infos = [
         ChunkInfo(text=chunk, num_characters=len(chunk), num_words=len(chunk.split()))
         for chunk in chunks
     ]
 
-    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
+    return TextChunks(num_chunks=len(chunk_infos), chunk_list=chunk_infos)
 
 
 def chunk_by_sentences(text: str) -> TextChunks:
     # Regular expression for splitting by sentence
     sentences = re.split(r"(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|\!)\s", text)
 
     chunk_infos = []
@@ -90,15 +90,15 @@
             chunk_info = ChunkInfo(
                 text=sentence,
                 num_characters=len(sentence),
                 num_words=len(sentence.split()),
             )
             chunk_infos.append(chunk_info)
 
-    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
+    return TextChunks(num_chunks=len(chunk_infos), chunk_list=chunk_infos)
 
 
 def chunk_by_paragraphs(text: str) -> TextChunks:
     # Splitting the text into paragraphs
     paragraphs = re.split(r"(?<=\n)(?=[A-Z0-9])", text)
 
     chunk_infos = [
@@ -107,15 +107,15 @@
             num_characters=len(paragraph.strip()),
             num_words=len(paragraph.strip().split()),
         )
         for paragraph in paragraphs
         if paragraph.strip()  # This condition filters out empty or whitespace-only paragraphs
     ]
 
-    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
+    return TextChunks(num_chunks=len(chunk_infos), chunk_list=chunk_infos)
 
 
 def chunk_by_semantics(text: str,  llm_embeddings_instance: llm_embeddings_instance, threshold_percentage=90) -> TextChunks:
 
     # Split the input text into individual sentences.
     single_sentences_list = __split_sentences(text)
 
@@ -163,15 +163,15 @@
             num_words=len(chunk.strip().split()),
         )
         for chunk in chunks
         if chunk.strip()  # This condition filters out empty or whitespace-only paragraphs
     ]
 
     # Return the list of text chunks.
-    return TextChunks(num_chunks=len(chunks), chunks=chunk_infos)
+    return TextChunks(num_chunks=len(chunks), chunk_list=chunk_infos)
 
 
 
 
 def __split_sentences(text):
     # Use regular expressions to split the text into sentences based on punctuation followed by whitespace.
     sentences = re.split(r"(?<=[.?!])\s+", text)
```

### Comparing `simplerllm-0.2.1/SimplerLLM.egg-info/PKG-INFO` & `simplerllm-0.2.3/SimplerLLM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: SimplerLLM
-Version: 0.2.1
+Version: 0.2.3
 Summary: An easy-to-use Library for interacting with language models.
 Home-page: https://github.com/hassancs91/SimplerLLM
 Author: Hasan Aboul Hasan
 Author-email: hasan@learnwithhasan.com
+License: MIT
 Keywords: text generation,openai,LLM,RAG
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -16,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp==3.9.4
 Requires-Dist: duckduckgo_search==5.3.0
 Requires-Dist: newspaper3k==0.2.8
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openai==1.25.0
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: PyPDF2==3.0.1
```

### Comparing `simplerllm-0.2.1/SimplerLLM.egg-info/SOURCES.txt` & `simplerllm-0.2.3/SimplerLLM.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 setup.py
 SimplerLLM/__init__.py
 SimplerLLM.egg-info/PKG-INFO
 SimplerLLM.egg-info/SOURCES.txt
 SimplerLLM.egg-info/dependency_links.txt
 SimplerLLM.egg-info/requires.txt
 SimplerLLM.egg-info/top_level.txt
@@ -13,16 +14,19 @@
 SimplerLLM/language/llm.py
 SimplerLLM/language/llm_addons.py
 SimplerLLM/language/llm_providers/__init__.py
 SimplerLLM/language/llm_providers/anthropic_llm.py
 SimplerLLM/language/llm_providers/gemini_llm.py
 SimplerLLM/language/llm_providers/llm_response_models.py
 SimplerLLM/language/llm_providers/openai_llm.py
+SimplerLLM/language/llm_providers/transformers_llm.py
 SimplerLLM/prompts/__init__.py
 SimplerLLM/prompts/prompt_builder.py
 SimplerLLM/tools/__init__.py
+SimplerLLM/tools/file_functions.py
 SimplerLLM/tools/file_loader.py
 SimplerLLM/tools/generic_loader.py
 SimplerLLM/tools/json_helpers.py
 SimplerLLM/tools/rapid_api.py
 SimplerLLM/tools/serp.py
-SimplerLLM/tools/text_chunker.py
+SimplerLLM/tools/text_chunker.py
+SimplerLLM/tools/web_crawler.py
```

### Comparing `simplerllm-0.2.1/setup.py` & `simplerllm-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from setuptools import setup, find_packages
 
+
 # Read requirements
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 # Read the long description from the README file
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SimplerLLM",
-    version="0.2.1",
+    version="0.2.3",
     author="Hasan Aboul Hasan",
     author_email="hasan@learnwithhasan.com",
     description="An easy-to-use Library for interacting with language models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hassancs91/SimplerLLM",
     packages=find_packages(),
     install_requires=requirements,
     python_requires=">=3.6",
+    license='MIT',
     keywords="text generation, openai, LLM, RAG",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
@@ -31,9 +33,11 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+
+
     # Add additional fields as necessary
 )
```

