# Comparing `tmp/asullmapi-1.1.1.tar.gz` & `tmp/asullmapi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asullmapi-1.1.1.tar", last modified: Mon May 13 18:57:10 2024, max compression
+gzip compressed data, was "asullmapi-1.1.3.tar", last modified: Mon May 13 22:18:20 2024, max compression
```

## Comparing `asullmapi-1.1.1.tar` & `asullmapi-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:57:10.614309 asullmapi-1.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:57:10.591463 asullmapi-1.1.1/ASUllmAPI/
--rw-rw-rw-   0        0        0      169 2024-05-08 21:25:24.000000 asullmapi-1.1.1/ASUllmAPI/__init__.py
--rw-rw-rw-   0        0        0     2980 2024-05-09 21:37:02.000000 asullmapi-1.1.1/ASUllmAPI/api.py
--rw-rw-rw-   0        0        0     2006 2024-05-09 21:37:02.000000 asullmapi-1.1.1/ASUllmAPI/model_config.py
--rw-rw-rw-   0        0        0     1670 2024-05-13 18:46:15.000000 asullmapi-1.1.1/ASUllmAPI/multithreading.py
--rw-rw-rw-   0        0        0      666 2024-05-08 21:25:24.000000 asullmapi-1.1.1/ASUllmAPI/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:57:10.608945 asullmapi-1.1.1/ASUllmAPI.egg-info/
--rw-rw-rw-   0        0        0     9860 2024-05-13 18:57:10.000000 asullmapi-1.1.1/ASUllmAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-05-13 18:57:10.000000 asullmapi-1.1.1/ASUllmAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:57:10.000000 asullmapi-1.1.1/ASUllmAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 18:57:10.000000 asullmapi-1.1.1/ASUllmAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-13 18:57:10.000000 asullmapi-1.1.1/ASUllmAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1124 2024-04-18 18:53:24.000000 asullmapi-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     9860 2024-05-13 18:57:10.610965 asullmapi-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9148 2024-05-09 21:37:02.000000 asullmapi-1.1.1/README.md
--rw-rw-rw-   0        0        0      724 2024-05-13 18:48:55.000000 asullmapi-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 18:57:10.614309 asullmapi-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 22:18:20.851169 asullmapi-1.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-13 22:18:20.823839 asullmapi-1.1.3/ASUllmAPI/
+-rw-rw-rw-   0        0        0      169 2024-05-08 21:25:24.000000 asullmapi-1.1.3/ASUllmAPI/__init__.py
+-rw-rw-rw-   0        0        0     2980 2024-05-09 21:37:02.000000 asullmapi-1.1.3/ASUllmAPI/api.py
+-rw-rw-rw-   0        0        0     2006 2024-05-09 21:37:02.000000 asullmapi-1.1.3/ASUllmAPI/model_config.py
+-rw-rw-rw-   0        0        0     1705 2024-05-13 19:58:06.000000 asullmapi-1.1.3/ASUllmAPI/multithreading.py
+-rw-rw-rw-   0        0        0      666 2024-05-08 21:25:24.000000 asullmapi-1.1.3/ASUllmAPI/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:18:20.846069 asullmapi-1.1.3/ASUllmAPI.egg-info/
+-rw-rw-rw-   0        0        0     1385 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1124 2024-04-18 18:53:24.000000 asullmapi-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1385 2024-05-13 22:18:20.848091 asullmapi-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2024-05-13 22:14:19.000000 asullmapi-1.1.3/README.md
+-rw-rw-rw-   0        0        0      724 2024-05-13 22:15:05.000000 asullmapi-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 22:18:20.851666 asullmapi-1.1.3/setup.cfg
```

### Comparing `asullmapi-1.1.1/ASUllmAPI/api.py` & `asullmapi-1.1.3/ASUllmAPI/api.py`

 * *Files identical despite different names*

### Comparing `asullmapi-1.1.1/ASUllmAPI/model_config.py` & `asullmapi-1.1.3/ASUllmAPI/model_config.py`

 * *Files identical despite different names*

### Comparing `asullmapi-1.1.1/ASUllmAPI/multithreading.py` & `asullmapi-1.1.3/ASUllmAPI/multithreading.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from typing import Dict
 
 from tqdm.auto import tqdm
 
 from .api import query_llm
 from .model_config import ModelConfig
 from .utils import time_api
 
 
 @time_api
-def batch_query_llm(model: ModelConfig, queries: dict, max_threads: int,
+def batch_query_llm(model: ModelConfig, queries: Dict[int, str], max_threads: int,
                     num_retry: int = 3, auto_increase_retry: bool = False,
-                    success_sleep: float = 0.0, fail_sleep: float = 1.0) -> dict[int, str]:
+                    success_sleep: float = 0.0, fail_sleep: float = 1.0) -> Dict[int, str]:
     with ThreadPoolExecutor(max_workers=max_threads) as executor:
         # Submit tasks to the executor - order of return will be asynchronous.
         # If `auto_increase_retry` enabled, then scaling API backoff is implemented.
         if auto_increase_retry:
             future_to_query = {executor.submit(query_llm, model, question,
                                                qid, success_sleep, fail_sleep): qid
                                for qid, question in queries.items()}
```

### Comparing `asullmapi-1.1.1/ASUllmAPI/utils.py` & `asullmapi-1.1.3/ASUllmAPI/utils.py`

 * *Files identical despite different names*

### Comparing `asullmapi-1.1.1/LICENSE` & `asullmapi-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asullmapi-1.1.1/pyproject.toml` & `asullmapi-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ASUllmAPI"
-version = "1.1.1"
+version = "1.1.3"
 authors = [
     { name="Stella Wenxing Liu", email="stellawenxingliu@gmail.com" },
     { name="Varun Shourie", email="svarun195@gmail.com" }
 ]
 description = "A simple python package to facilitate connection to ASU LLM API"
 readme = "README.md"
 requires-python = ">=3.8"
```

