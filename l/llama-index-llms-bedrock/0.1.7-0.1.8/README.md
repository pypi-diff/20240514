# Comparing `tmp/llama_index_llms_bedrock-0.1.7.tar.gz` & `tmp/llama_index_llms_bedrock-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_bedrock-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_llms_bedrock-0.1.8.tar", max compression
```

## Comparing `llama_index_llms_bedrock-0.1.7.tar` & `llama_index_llms_bedrock-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       39 2024-04-23 04:01:23.211103 llama_index_llms_bedrock-0.1.7/README.md
--rw-r--r--   0        0        0      216 2024-04-23 04:01:23.215103 llama_index_llms_bedrock-0.1.7/llama_index/llms/bedrock/__init__.py
--rw-r--r--   0        0        0    11896 2024-04-23 04:01:23.215103 llama_index_llms_bedrock-0.1.7/llama_index/llms/bedrock/base.py
--rw-r--r--   0        0        0     2248 2024-04-23 04:01:23.215103 llama_index_llms_bedrock-0.1.7/llama_index/llms/bedrock/llama_utils.py
--rw-r--r--   0        0        0     8407 2024-04-23 04:01:23.215103 llama_index_llms_bedrock-0.1.7/llama_index/llms/bedrock/utils.py
--rw-r--r--   0        0        0     1482 2024-04-23 04:01:23.215103 llama_index_llms_bedrock-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 llama_index_llms_bedrock-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-14 17:23:12.352822 llama_index_llms_bedrock-0.1.8/README.md
+-rw-r--r--   0        0        0      216 2024-05-14 17:23:12.352822 llama_index_llms_bedrock-0.1.8/llama_index/llms/bedrock/__init__.py
+-rw-r--r--   0        0        0    11896 2024-05-14 17:23:12.352822 llama_index_llms_bedrock-0.1.8/llama_index/llms/bedrock/base.py
+-rw-r--r--   0        0        0     2248 2024-05-14 17:23:12.352822 llama_index_llms_bedrock-0.1.8/llama_index/llms/bedrock/llama_utils.py
+-rw-r--r--   0        0        0     8407 2024-05-14 17:23:12.352822 llama_index_llms_bedrock-0.1.8/llama_index/llms/bedrock/utils.py
+-rw-r--r--   0        0        0     1482 2024-05-14 17:23:12.356822 llama_index_llms_bedrock-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 llama_index_llms_bedrock-0.1.8/PKG-INFO
```

### Comparing `llama_index_llms_bedrock-0.1.7/llama_index/llms/bedrock/base.py` & `llama_index_llms_bedrock-0.1.8/llama_index/llms/bedrock/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_bedrock-0.1.7/llama_index/llms/bedrock/llama_utils.py` & `llama_index_llms_bedrock-0.1.8/llama_index/llms/bedrock/llama_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_bedrock-0.1.7/llama_index/llms/bedrock/utils.py` & `llama_index_llms_bedrock-0.1.8/llama_index/llms/bedrock/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_bedrock-0.1.7/pyproject.toml` & `llama_index_llms_bedrock-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms bedrock integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-bedrock"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-anthropic = "^0.1.7"
 boto3 = "^1.34.26"
```

### Comparing `llama_index_llms_bedrock-0.1.7/PKG-INFO` & `llama_index_llms_bedrock-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-bedrock
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index llms bedrock integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

