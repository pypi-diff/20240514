# Comparing `tmp/promptlayer-1.0.0.tar.gz` & `tmp/promptlayer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlayer-1.0.0.tar", max compression
+gzip compressed data, was "promptlayer-1.0.1.tar", max compression
```

## Comparing `promptlayer-1.0.0.tar` & `promptlayer-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-05-10 19:19:57.139462 promptlayer-1.0.0/LICENSE
--rw-r--r--   0        0        0     3870 2024-05-10 19:19:57.139462 promptlayer-1.0.0/README.md
--rw-r--r--   0        0        0     1565 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/__init__.py
--rw-r--r--   0        0        0      224 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/groups/__init__.py
--rw-r--r--   0        0        0      165 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/groups/groups.py
--rw-r--r--   0        0        0     4035 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/promptlayer.py
--rw-r--r--   0        0        0      717 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/templates.py
--rw-r--r--   0        0        0      945 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/track/__init__.py
--rw-r--r--   0        0        0     1610 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/track/track.py
--rw-r--r--   0        0        0       61 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/types/__init__.py
--rw-r--r--   0        0        0     3813 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/types/prompt_template.py
--rw-r--r--   0        0        0    21130 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/utils.py
--rw-r--r--   0        0        0      571 2024-05-10 19:19:57.143462 promptlayer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 promptlayer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 15:09:50.781215 promptlayer-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3870 2024-05-14 15:09:50.781215 promptlayer-1.0.1/README.md
+-rw-r--r--   0        0        0     1565 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/groups/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/groups/groups.py
+-rw-r--r--   0        0        0     4035 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/promptlayer.py
+-rw-r--r--   0        0        0      717 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/templates.py
+-rw-r--r--   0        0        0      945 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/track/__init__.py
+-rw-r--r--   0        0        0     1610 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/track/track.py
+-rw-r--r--   0        0        0       61 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/types/__init__.py
+-rw-r--r--   0        0        0     3813 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/types/prompt_template.py
+-rw-r--r--   0        0        0    21130 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/utils.py
+-rw-r--r--   0        0        0      571 2024-05-14 15:09:50.785215 promptlayer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 promptlayer-1.0.1/PKG-INFO
```

### Comparing `promptlayer-1.0.0/LICENSE` & `promptlayer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/README.md` & `promptlayer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/promptlayer/__init__.py` & `promptlayer-1.0.1/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/promptlayer/promptlayer.py` & `promptlayer-1.0.1/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/promptlayer/templates.py` & `promptlayer-1.0.1/promptlayer/templates.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/promptlayer/track/__init__.py` & `promptlayer-1.0.1/promptlayer/track/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/promptlayer/track/track.py` & `promptlayer-1.0.1/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/promptlayer/types/prompt_template.py` & `promptlayer-1.0.1/promptlayer/types/prompt_template.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/promptlayer/utils.py` & `promptlayer-1.0.1/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.0/pyproject.toml` & `promptlayer-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "promptlayer"
-version = "1.0.0"
+version = "1.0.1"
 description = "PromptLayer is a platform for prompt engineering and tracks your LLM requests."
 authors = ["Magniv <hello@magniv.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2.31.0"
-pytest = "^8.2.0"
 openai = "^1.26.0"
 anyio = "^4.3.0"
-pytest-asyncio = "^0.23.6"
 anthropic = "^0.25.8"
 
 [tool.poetry.group.dev.dependencies]
 langchain = "^0.0.260"
 behave = "^1.2.6"
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `promptlayer-1.0.0/PKG-INFO` & `promptlayer-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 1.0.0
+Version: 1.0.1
 Summary: PromptLayer is a platform for prompt engineering and tracks your LLM requests.
 License: Apache-2.0
 Author: Magniv
 Author-email: hello@magniv.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.25.8,<0.26.0)
 Requires-Dist: anyio (>=4.3.0,<5.0.0)
 Requires-Dist: openai (>=1.26.0,<2.0.0)
-Requires-Dist: pytest (>=8.2.0,<9.0.0)
-Requires-Dist: pytest-asyncio (>=0.23.6,<0.24.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # 🍰 PromptLayer
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 1.0.0 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 1.0.1 Summary: PromptLayer is
 a platform for prompt engineering and tracks your LLM requests. License:
 Apache-2.0 Author: Magniv Author-email: hello@magniv.io Requires-Python:
 >=3.8.1,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: anthropic (>=0.25.8,<0.26.0)
 Requires-Dist: anyio (>=4.3.0,<5.0.0) Requires-Dist: openai (>=1.26.0,<2.0.0)
-Requires-Dist: pytest (>=8.2.0,<9.0.0) Requires-Dist: pytest-asyncio
-(>=0.23.6,<0.24.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Description-
-Content-Type: text/markdown
+Requires-Dist: requests (>=2.31.0,<3.0.0) Description-Content-Type: text/
+markdown
  # ð° PromptLayer **The first platform built for prompt engineers** _[_P_y_t_h_o_n_]
                            _[_D_o_c_s_]_[_D_e_m_o_ _w_i_t_h_ _L_o_o_m_]---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
 to track, manage, and share your GPT prompt engineering. PromptLayer acts a
 middleware between your code and OpenAIâs python library. PromptLayer records
 all your OpenAI API requests, allowing you to search and explore request
 history in the PromptLayer dashboard. This repo contains the Python wrapper
```

