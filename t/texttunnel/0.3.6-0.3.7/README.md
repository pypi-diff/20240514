# Comparing `tmp/texttunnel-0.3.6.tar.gz` & `tmp/texttunnel-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texttunnel-0.3.6.tar", max compression
+gzip compressed data, was "texttunnel-0.3.7.tar", max compression
```

## Comparing `texttunnel-0.3.6.tar` & `texttunnel-0.3.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-08-03 06:33:05.395777 texttunnel-0.3.6/LICENSE
--rw-r--r--   0        0        0     3572 2023-11-15 11:20:19.907850 texttunnel-0.3.6/README.md
--rw-r--r--   0        0        0      776 2024-01-15 11:04:56.702322 texttunnel-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-17 08:59:43.751438 texttunnel-0.3.6/texttunnel/__init__.py
--rw-r--r--   0        0        0    14951 2023-11-30 13:58:15.928114 texttunnel-0.3.6/texttunnel/chat.py
--rw-r--r--   0        0        0     6978 2023-11-15 11:20:19.908304 texttunnel-0.3.6/texttunnel/models.py
--rw-r--r--   0        0        0    35186 2024-01-15 11:04:56.703821 texttunnel-0.3.6/texttunnel/processor.py
--rw-r--r--   0        0        0     8755 2023-08-21 13:34:04.402374 texttunnel-0.3.6/texttunnel/utils.py
--rw-r--r--   0        0        0     4308 1970-01-01 00:00:00.000000 texttunnel-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-08-03 06:33:05.395777 texttunnel-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4072 2024-05-14 06:35:08.067833 texttunnel-0.3.7/README.md
+-rw-r--r--   0        0        0      776 2024-05-14 06:54:02.700955 texttunnel-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-17 08:59:43.751438 texttunnel-0.3.7/texttunnel/__init__.py
+-rw-r--r--   0        0        0    14951 2023-11-30 13:58:15.928114 texttunnel-0.3.7/texttunnel/chat.py
+-rw-r--r--   0        0        0     7465 2024-05-14 06:53:22.353265 texttunnel-0.3.7/texttunnel/models.py
+-rw-r--r--   0        0        0    35186 2024-01-15 11:04:56.703821 texttunnel-0.3.7/texttunnel/processor.py
+-rw-r--r--   0        0        0     8755 2023-08-21 13:34:04.402374 texttunnel-0.3.7/texttunnel/utils.py
+-rw-r--r--   0        0        0     4808 1970-01-01 00:00:00.000000 texttunnel-0.3.7/PKG-INFO
```

### Comparing `texttunnel-0.3.6/LICENSE` & `texttunnel-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `texttunnel-0.3.6/README.md` & `texttunnel-0.3.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,29 @@
   <img src="https://github.com/qagentur/texttunnel/assets/25177095/411ad918-d054-4d19-aef5-1dba9136db33" width="65%" />
 </div>
 
 This package offers a straightforward interface for integrating the GPT-3.5 and GPT-4 models into your natural language processing pipelines. It is optimally designed for the following scenario:
 
 Suppose you possess a corpus of text data that you want to analyze using the GPT-3.5 or GPT-4 models. The goal is to perform extractive NLP tasks such as classification, named entity recognition, translation, summarization, question answering, or sentiment analysis. In this context, the package prioritizes efficiency and tidiness to provide you streamlined results.
 
-🚧 When updating the package please check the [changelog](/CHANGELOG.md) for breaking changes. 🚧
-
 Features:
 
 - 📄 Output Schema: Utilizes [JSON Schema](https://json-schema.org) alongside OpenAI's function calling schema to define the output data structure.
 - ✔️ Input Validation: Ensures well-structured and error-free API requests by validating input data.
 - ✅ Output Validation: Checks the response data from OpenAI's API against the expected schema to maintain data integrity.
+- 🚦 Asynchronous Requests: Facilitates speedy data processing by sending simultaneous requests to OpenAI's API, while staying within API rate limits.
 - 🚀 Efficient Batching: Supports bulk processing by packing multiple input texts into a single request for the OpenAI's API.
-- 🚦 Asynchronous Requests: Facilitates speedy data processing by sending simultaneous requests to OpenAI's API, while maintaining API rate limits.
 - 💰 Cost Estimation: Aims for transparency in API utilization cost by providing cost estimates before sending API requests.
 - 💾 Caching: Uses [aiohttp_client_cache](https://github.com/requests-cache/aiohttp-client-cache) to avoid redundant requests and reduce cost by caching previous requests. Supports SQLite, MongoDB, DynamoDB and Redis cache backends.
 - 📝 Request Logging: Implements Python's native [logging](https://docs.python.org/3/library/logging.html) framework for tracking and logging all API requests.
 
+Note that this package only works with [function calling](https://platform.openai.com/docs/guides/function-calling) and only with the OpenAI API. If you're looking for a more flexible solution, consider [instructor](https://github.com/jxnl/instructor) and [litellm](https://github.com/BerriAI/litellm). You might also consider using the [OpenAI Batch API](https://platform.openai.com/docs/api-reference/batch) as it offers savings compared to synchronous API calls.
+
+⚠️ **Maintenance mode**: At this time no new features or enhancements are being developed. Only critical bugfixes will be made.
+
 ## Installation
 
 The package is available on [PyPI](https://pypi.org/project/texttunnel/). To install it, run:
   
 ```bash
 pip install texttunnel
 ```
```

### Comparing `texttunnel-0.3.6/texttunnel/chat.py` & `texttunnel-0.3.7/texttunnel/chat.py`

 * *Files identical despite different names*

### Comparing `texttunnel-0.3.6/texttunnel/models.py` & `texttunnel-0.3.7/texttunnel/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,37 @@
             "tokens_per_minute",
             "requests_per_minute",
         ]:
             if getattr(self, arg) < 0:
                 raise ValueError(f"{arg} must be positive")
 
 
-# Look up information on models, pricing and rate limits:
+# Look up information on models, pricing and rate limits
+# Note that tokens_per_minute and requests_per_minute differ by usage tier
 # https://platform.openai.com/docs/models/overview
 # https://openai.com/pricing
-# https://platform.openai.com/account/rate-limits
+# https://platform.openai.com/docs/guides/rate-limits/usage-tiers
+
+GPT_4o = Model(
+    name="gpt-4o",
+    context_size=128000,
+    input_token_price_per_1k=0.005,
+    output_token_price_per_1k=0.0015,
+    tokens_per_minute=30000,
+    requests_per_minute=500,
+)
+
+GPT_4_TURBO = Model(
+    name="gpt-4-turbo",
+    context_size=128000,
+    input_token_price_per_1k=0.01,
+    output_token_price_per_1k=0.03,
+    tokens_per_minute=30000,
+    requests_per_minute=500,
+)
 
 GPT_4 = Model(
     name="gpt-4",
     context_size=8192,
     input_token_price_per_1k=0.03,
     output_token_price_per_1k=0.06,
     tokens_per_minute=10000,
```

### Comparing `texttunnel-0.3.6/texttunnel/processor.py` & `texttunnel-0.3.7/texttunnel/processor.py`

 * *Files identical despite different names*

### Comparing `texttunnel-0.3.6/texttunnel/utils.py` & `texttunnel-0.3.7/texttunnel/utils.py`

 * *Files identical despite different names*

### Comparing `texttunnel-0.3.6/PKG-INFO` & `texttunnel-0.3.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texttunnel
-Version: 0.3.6
+Version: 0.3.7
 Summary: Efficient text processing with the OpenAI API
 Home-page: https://github.com/qagentur/texttunnel
 License: MIT
 Author: Q Agentur für Forschung GmbH
 Author-email: info@teamq.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -24,27 +24,29 @@
   <img src="https://github.com/qagentur/texttunnel/assets/25177095/411ad918-d054-4d19-aef5-1dba9136db33" width="65%" />
 </div>
 
 This package offers a straightforward interface for integrating the GPT-3.5 and GPT-4 models into your natural language processing pipelines. It is optimally designed for the following scenario:
 
 Suppose you possess a corpus of text data that you want to analyze using the GPT-3.5 or GPT-4 models. The goal is to perform extractive NLP tasks such as classification, named entity recognition, translation, summarization, question answering, or sentiment analysis. In this context, the package prioritizes efficiency and tidiness to provide you streamlined results.
 
-🚧 When updating the package please check the [changelog](/CHANGELOG.md) for breaking changes. 🚧
-
 Features:
 
 - 📄 Output Schema: Utilizes [JSON Schema](https://json-schema.org) alongside OpenAI's function calling schema to define the output data structure.
 - ✔️ Input Validation: Ensures well-structured and error-free API requests by validating input data.
 - ✅ Output Validation: Checks the response data from OpenAI's API against the expected schema to maintain data integrity.
+- 🚦 Asynchronous Requests: Facilitates speedy data processing by sending simultaneous requests to OpenAI's API, while staying within API rate limits.
 - 🚀 Efficient Batching: Supports bulk processing by packing multiple input texts into a single request for the OpenAI's API.
-- 🚦 Asynchronous Requests: Facilitates speedy data processing by sending simultaneous requests to OpenAI's API, while maintaining API rate limits.
 - 💰 Cost Estimation: Aims for transparency in API utilization cost by providing cost estimates before sending API requests.
 - 💾 Caching: Uses [aiohttp_client_cache](https://github.com/requests-cache/aiohttp-client-cache) to avoid redundant requests and reduce cost by caching previous requests. Supports SQLite, MongoDB, DynamoDB and Redis cache backends.
 - 📝 Request Logging: Implements Python's native [logging](https://docs.python.org/3/library/logging.html) framework for tracking and logging all API requests.
 
+Note that this package only works with [function calling](https://platform.openai.com/docs/guides/function-calling) and only with the OpenAI API. If you're looking for a more flexible solution, consider [instructor](https://github.com/jxnl/instructor) and [litellm](https://github.com/BerriAI/litellm). You might also consider using the [OpenAI Batch API](https://platform.openai.com/docs/api-reference/batch) as it offers savings compared to synchronous API calls.
+
+⚠️ **Maintenance mode**: At this time no new features or enhancements are being developed. Only critical bugfixes will be made.
+
 ## Installation
 
 The package is available on [PyPI](https://pypi.org/project/texttunnel/). To install it, run:
   
 ```bash
 pip install texttunnel
 ```
```

