# Comparing `tmp/simple-openai-3.4.1.tar.gz` & `tmp/simple_openai-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-openai-3.4.1.tar", last modified: Sun Mar 31 12:33:13 2024, max compression
+gzip compressed data, was "simple_openai-3.4.2.tar", last modified: Tue May 14 20:31:59 2024, max compression
```

## Comparing `simple-openai-3.4.1.tar` & `simple_openai-3.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-31 12:33:13.771035 simple-openai-3.4.1/
--rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-3.4.1/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)    17943 2024-03-31 12:33:13.770587 simple-openai-3.4.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     3795 2023-08-20 13:57:08.000000 simple-openai-3.4.1/README.md
--rw-r--r--   0 steve      (501) staff       (20)     1179 2024-03-31 12:27:08.000000 simple-openai-3.4.1/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-03-31 12:33:13.771084 simple-openai-3.4.1/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-31 12:33:13.766951 simple-openai-3.4.1/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-31 12:33:13.768557 simple-openai-3.4.1/src/simple_openai/
--rw-r--r--   0 steve      (501) staff       (20)      223 2023-06-17 09:54:32.000000 simple-openai-3.4.1/src/simple_openai/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    11031 2023-08-20 14:02:35.000000 simple-openai-3.4.1/src/simple_openai/async_simple_openai.py
--rw-r--r--   0 steve      (501) staff       (20)     4604 2023-08-20 10:51:23.000000 simple-openai-3.4.1/src/simple_openai/chat_manager.py
--rw-r--r--   0 steve      (501) staff       (20)      351 2023-08-20 11:24:55.000000 simple-openai-3.4.1/src/simple_openai/constants.py
--rw-r--r--   0 steve      (501) staff       (20)     3782 2023-08-20 13:38:19.000000 simple-openai-3.4.1/src/simple_openai/function_manager.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-31 12:33:13.769605 simple-openai-3.4.1/src/simple_openai/models/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-08-20 13:26:57.000000 simple-openai-3.4.1/src/simple_openai/models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     2735 2024-03-31 12:25:45.000000 simple-openai-3.4.1/src/simple_openai/models/open_ai_models.py
--rw-r--r--   0 steve      (501) staff       (20)      678 2023-08-20 13:49:58.000000 simple-openai-3.4.1/src/simple_openai/responses.py
--rw-r--r--   0 steve      (501) staff       (20)     9882 2023-08-20 11:18:24.000000 simple-openai-3.4.1/src/simple_openai/simple_openai.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-31 12:33:13.770130 simple-openai-3.4.1/src/simple_openai.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    17943 2024-03-31 12:33:13.000000 simple-openai-3.4.1/src/simple_openai.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      615 2024-03-31 12:33:13.000000 simple-openai-3.4.1/src/simple_openai.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-03-31 12:33:13.000000 simple-openai-3.4.1/src/simple_openai.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       89 2024-03-31 12:33:13.000000 simple-openai-3.4.1/src/simple_openai.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       14 2024-03-31 12:33:13.000000 simple-openai-3.4.1/src/simple_openai.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-31 12:33:13.769928 simple-openai-3.4.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)     6191 2023-08-20 11:25:31.000000 simple-openai-3.4.1/tests/test_AsyncSimpleOpenai.py
--rw-r--r--   0 steve      (501) staff       (20)     5665 2023-08-20 11:29:36.000000 simple-openai-3.4.1/tests/test_SimpleOpenai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 20:31:59.417156 simple_openai-3.4.2/
+-rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple_openai-3.4.2/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)    17943 2024-05-14 20:31:59.416753 simple_openai-3.4.2/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     3795 2023-08-20 13:57:08.000000 simple_openai-3.4.2/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     1179 2024-05-14 20:24:15.000000 simple_openai-3.4.2/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-14 20:31:59.417206 simple_openai-3.4.2/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 20:31:59.409705 simple_openai-3.4.2/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 20:31:59.412791 simple_openai-3.4.2/src/simple_openai/
+-rw-r--r--   0 steve      (501) staff       (20)      223 2023-06-17 09:54:32.000000 simple_openai-3.4.2/src/simple_openai/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    11031 2023-08-20 14:02:35.000000 simple_openai-3.4.2/src/simple_openai/async_simple_openai.py
+-rw-r--r--   0 steve      (501) staff       (20)     4604 2023-08-20 10:51:23.000000 simple_openai-3.4.2/src/simple_openai/chat_manager.py
+-rw-r--r--   0 steve      (501) staff       (20)      351 2023-08-20 11:24:55.000000 simple_openai-3.4.2/src/simple_openai/constants.py
+-rw-r--r--   0 steve      (501) staff       (20)     3782 2023-08-20 13:38:19.000000 simple_openai-3.4.2/src/simple_openai/function_manager.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 20:31:59.414260 simple_openai-3.4.2/src/simple_openai/models/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-08-20 13:26:57.000000 simple_openai-3.4.2/src/simple_openai/models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     2736 2024-05-14 20:29:19.000000 simple_openai-3.4.2/src/simple_openai/models/open_ai_models.py
+-rw-r--r--   0 steve      (501) staff       (20)      678 2023-08-20 13:49:58.000000 simple_openai-3.4.2/src/simple_openai/responses.py
+-rw-r--r--   0 steve      (501) staff       (20)     9882 2023-08-20 11:18:24.000000 simple_openai-3.4.2/src/simple_openai/simple_openai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 20:31:59.416125 simple_openai-3.4.2/src/simple_openai.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    17943 2024-05-14 20:31:59.000000 simple_openai-3.4.2/src/simple_openai.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      615 2024-05-14 20:31:59.000000 simple_openai-3.4.2/src/simple_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-14 20:31:59.000000 simple_openai-3.4.2/src/simple_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       89 2024-05-14 20:31:59.000000 simple_openai-3.4.2/src/simple_openai.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       14 2024-05-14 20:31:59.000000 simple_openai-3.4.2/src/simple_openai.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 20:31:59.415496 simple_openai-3.4.2/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     6191 2023-08-20 11:25:31.000000 simple_openai-3.4.2/tests/test_AsyncSimpleOpenai.py
+-rw-r--r--   0 steve      (501) staff       (20)     5665 2023-08-20 11:29:36.000000 simple_openai-3.4.2/tests/test_SimpleOpenai.py
```

### Comparing `simple-openai-3.4.1/LICENSE` & `simple_openai-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/PKG-INFO` & `simple_openai-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 3.4.1
+Version: 3.4.2
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple-openai-3.4.1/README.md` & `simple_openai-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/pyproject.toml` & `simple_openai-3.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-openai"
-version = "3.4.1"
+version = "3.4.2"
 description = "Simple OpenAI API wrapper"
 readme = "README.md"
 authors = [{ name = "Stephen Schleising", email = "stephen@schleising.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `simple-openai-3.4.1/src/simple_openai/async_simple_openai.py` & `simple_openai-3.4.2/src/simple_openai/async_simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/src/simple_openai/chat_manager.py` & `simple_openai-3.4.2/src/simple_openai/chat_manager.py`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/src/simple_openai/function_manager.py` & `simple_openai-3.4.2/src/simple_openai/function_manager.py`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/src/simple_openai/models/open_ai_models.py` & `simple_openai-3.4.2/src/simple_openai/models/open_ai_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 class Chat(BaseModel):
     messages: list[ChatMessage]
 
 class ChatRequest(Chat):
     functions: list[OpenAIFunction] | None = None
     function_call: str
-    model: str = 'gpt-4'
+    model: str = 'gpt-4o'
 
 class ResponseMessage(BaseModel):
     role: str
     content: str | None
     function_call: FunctionCall | None = None
 
 class Choice(BaseModel):
```

### Comparing `simple-openai-3.4.1/src/simple_openai/responses.py` & `simple_openai-3.4.2/src/simple_openai/responses.py`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/src/simple_openai/simple_openai.py` & `simple_openai-3.4.2/src/simple_openai/simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/src/simple_openai.egg-info/PKG-INFO` & `simple_openai-3.4.2/src/simple_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 3.4.1
+Version: 3.4.2
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple-openai-3.4.1/src/simple_openai.egg-info/SOURCES.txt` & `simple_openai-3.4.2/src/simple_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/tests/test_AsyncSimpleOpenai.py` & `simple_openai-3.4.2/tests/test_AsyncSimpleOpenai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-3.4.1/tests/test_SimpleOpenai.py` & `simple_openai-3.4.2/tests/test_SimpleOpenai.py`

 * *Files identical despite different names*

