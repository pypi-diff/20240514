# Comparing `tmp/tulp-2.0.tar.gz` & `tmp/tulp-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulp-2.0.tar", last modified: Fri May  3 22:26:57 2024, max compression
+gzip compressed data, was "tulp-2.1.tar", last modified: Tue May 14 18:02:12 2024, max compression
```

## Comparing `tulp-2.0.tar` & `tulp-2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.607448 tulp-2.0/
--rw-rw-r--   0 fede      (1000) fede      (1000)      684 2024-02-14 15:35:47.000000 tulp-2.0/LICENSE
--rw-r--r--   0 fede      (1000) fede      (1000)    11330 2024-05-03 22:26:57.607448 tulp-2.0/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)    10567 2024-05-03 22:26:20.000000 tulp-2.0/README.md
--rw-rw-r--   0 fede      (1000) fede      (1000)      990 2024-05-03 22:26:57.611448 tulp-2.0/setup.cfg
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-02-14 15:35:47.000000 tulp-2.0/setup.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.595448 tulp-2.0/test/
--rw-rw-r--   0 fede      (1000) fede      (1000)     2847 2024-05-03 22:26:20.000000 tulp-2.0/test/test_filterMode_advanced.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3621 2024-02-14 15:35:47.000000 tulp-2.0/test/test_filterMode_basic.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1342 2024-02-14 15:35:47.000000 tulp-2.0/test/test_requestMode.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1066 2024-02-14 15:35:47.000000 tulp-2.0/test/test_slowtest.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.599448 tulp-2.0/tulp/
--rw-rw-r--   0 fede      (1000) fede      (1000)     1378 2024-05-02 13:40:36.000000 tulp-2.0/tulp/TulpOutputFileWriter.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      111 2024-02-14 15:35:47.000000 tulp-2.0/tulp/__init__.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1864 2024-02-14 15:35:47.000000 tulp-2.0/tulp/createFilteringProgramPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1443 2024-02-14 15:35:47.000000 tulp-2.0/tulp/createProgramPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      389 2024-02-14 15:35:47.000000 tulp-2.0/tulp/executePython.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     4939 2024-05-03 22:26:20.000000 tulp-2.0/tulp/filteringPrompt.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.607448 tulp-2.0/tulp/llms/
--rw-rw-r--   0 fede      (1000) fede      (1000)     3431 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmAnthropic.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3167 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmGemini.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3431 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmGroq.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3141 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmOllama.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     2061 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmOpenAI.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1616 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/__init__.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3678 2024-05-03 22:26:20.000000 tulp-2.0/tulp/requestPrompt.py
--rwxrwxr-x   0 fede      (1000) fede      (1000)    11917 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulp.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     2387 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulpargs.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1381 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulpconfig.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1935 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulplogger.py
--rw-rw-r--   0 fede      (1000) fede      (1000)       16 2024-05-03 22:26:20.000000 tulp-2.0/tulp/version.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.607448 tulp-2.0/tulp.egg-info/
--rw-r--r--   0 fede      (1000) fede      (1000)    11330 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)      740 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/SOURCES.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/dependency_links.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/entry_points.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       95 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/requires.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        5 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/top_level.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-02-14 15:41:21.000000 tulp-2.0/tulp.egg-info/zip-safe
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-14 18:02:12.216671 tulp-2.1/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      684 2024-02-14 15:35:47.000000 tulp-2.1/LICENSE
+-rw-r--r--   0 fede      (1000) fede      (1000)    11400 2024-05-14 18:02:12.216671 tulp-2.1/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)    10637 2024-05-14 18:01:54.000000 tulp-2.1/README.md
+-rw-rw-r--   0 fede      (1000) fede      (1000)      990 2024-05-14 18:02:12.216671 tulp-2.1/setup.cfg
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-02-14 15:35:47.000000 tulp-2.1/setup.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-14 18:02:12.208671 tulp-2.1/test/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2847 2024-05-03 22:26:20.000000 tulp-2.1/test/test_filterMode_advanced.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3621 2024-02-14 15:35:47.000000 tulp-2.1/test/test_filterMode_basic.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1342 2024-02-14 15:35:47.000000 tulp-2.1/test/test_requestMode.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1066 2024-02-14 15:35:47.000000 tulp-2.1/test/test_slowtest.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-14 18:02:12.212671 tulp-2.1/tulp/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1378 2024-05-02 13:40:36.000000 tulp-2.1/tulp/TulpOutputFileWriter.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      111 2024-02-14 15:35:47.000000 tulp-2.1/tulp/__init__.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1864 2024-02-14 15:35:47.000000 tulp-2.1/tulp/createFilteringProgramPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1443 2024-02-14 15:35:47.000000 tulp-2.1/tulp/createProgramPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      389 2024-02-14 15:35:47.000000 tulp-2.1/tulp/executePython.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     4939 2024-05-03 22:26:20.000000 tulp-2.1/tulp/filteringPrompt.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-14 18:02:12.216671 tulp-2.1/tulp/llms/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3431 2024-05-03 22:26:20.000000 tulp-2.1/tulp/llms/LlmAnthropic.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3859 2024-05-09 14:18:53.000000 tulp-2.1/tulp/llms/LlmGemini.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3431 2024-05-03 22:26:20.000000 tulp-2.1/tulp/llms/LlmGroq.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3141 2024-05-03 22:26:20.000000 tulp-2.1/tulp/llms/LlmOllama.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2061 2024-05-03 22:26:20.000000 tulp-2.1/tulp/llms/LlmOpenAI.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1616 2024-05-03 22:26:20.000000 tulp-2.1/tulp/llms/__init__.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3678 2024-05-03 22:26:20.000000 tulp-2.1/tulp/requestPrompt.py
+-rwxrwxr-x   0 fede      (1000) fede      (1000)    12013 2024-05-09 18:26:40.000000 tulp-2.1/tulp/tulp.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2387 2024-05-03 22:26:20.000000 tulp-2.1/tulp/tulpargs.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1376 2024-05-14 17:55:24.000000 tulp-2.1/tulp/tulpconfig.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1935 2024-05-03 22:26:20.000000 tulp-2.1/tulp/tulplogger.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)       16 2024-05-14 17:59:20.000000 tulp-2.1/tulp/version.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-14 18:02:12.216671 tulp-2.1/tulp.egg-info/
+-rw-r--r--   0 fede      (1000) fede      (1000)    11400 2024-05-14 18:02:12.000000 tulp-2.1/tulp.egg-info/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      740 2024-05-14 18:02:12.000000 tulp-2.1/tulp.egg-info/SOURCES.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-05-14 18:02:12.000000 tulp-2.1/tulp.egg-info/dependency_links.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-05-14 18:02:12.000000 tulp-2.1/tulp.egg-info/entry_points.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       95 2024-05-14 18:02:12.000000 tulp-2.1/tulp.egg-info/requires.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        5 2024-05-14 18:02:12.000000 tulp-2.1/tulp.egg-info/top_level.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-02-14 15:41:21.000000 tulp-2.1/tulp.egg-info/zip-safe
```

### Comparing `tulp-2.0/LICENSE` & `tulp-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tulp-2.0/PKG-INFO` & `tulp-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 2.0
+Version: 2.1
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 ```
 
 
 In both cases, TULP will write to the standard output the answers and will write any other information to the standard error. You can safely pipe the output to your file or next piping command and will still get all the information and errors on stderr.
 
 It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by the selected AI model in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
 
-By default, tulp uses **gpt-4-0125-preview**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
+By default, tulp uses **gpt-4o**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
 
 ### Options:
 ```
 usage: tulp [-h] [-x] [-w W] [--model MODEL] [--max-chars MAX_CHARS] [-v] [-q] [--groq_api_key GROQ_API_KEY] [--ollama_host OLLAMA_HOST] [--anthropic_api_key ANTHROPIC_API_KEY] [--openai_api_key OPENAI_API_KEY] [--openai_baseurl OPENAI_BASEURL] [--gemini_api_key GEMINI_API_KEY] ...
 
 TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with support for multiple AI APIs including groq, ollama, anthropic, and gemini.
 
@@ -91,28 +91,28 @@
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. 
 
 The following are the parameters that can be configured:
 - **LOG_LEVEL**: The log level of Tulp. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
 - **API_KEYS**: The API keys for the supported AI models (OpenAI, GROQ, Ollama, Anthropic, Gemini). The default value is an empty string for each.
 - **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 40000.
-- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4-0125-preview, but other models are also available.
+- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4o but other models are also available.
 
 All these settings could be overridden by an environment variable using the prefix TULP\_ or by the different command line arguments described above. 
 As environment variables, they will become: TULP_LOG_LEVEL, TULP_API_KEYS, TULP_MAX_CHARS, or TULP_MODEL.
 Command line arguments will override environmental variables and the configuration file.
 
 
 Here is an example configuration file with the default values:
 ```INI
 [DEFAULT]
 LOG_LEVEL = INFO
 ${MODEL}_API_KEYS = <<<YOUR API KEYS FOR GROQ, OLLAMA, ANTHROPIC, OPENAI, GEMINI>>>
 MAX_CHARS = 40000
-MODEL = gpt-4-0125-preview
+MODEL = gpt-4o
 ```
 
 
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspiration:
 
 ### Random
@@ -259,14 +259,18 @@
 ```
 
 # Why?
 
 I am a heavy user of Unix tooling (e.g: awk, jq, sed, grep, and so on), I have been using them since my early days and I used to think that I couldn't survive without them. But then, ChatGPT appeared, and I started to use more and more GPT for things that I used to use Unix tooling for. Somehow I feel the pain of cut & paste, and I was missing a way to do it faster and from within the terminal itself, so I came up with `tulp`.
 
 # Changelog
+## v2.1 | 2024-05-14
+- Improves formating of messages for gemini
+- Changed to use gpt-4o model by default
+
 ## v2.0 | 2024-05-04
 - Added support for groq, ollama, anthropic, and gemini AI models.
 - Changed to use gpt-4-turbo model by default
 
 ## v1.0 | 2024-02-14
 - Changed to use gpt-4-0125-preview model by default
 - Updated to use openapi v1.0
```

### Comparing `tulp-2.0/README.md` & `tulp-2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```
 
 
 In both cases, TULP will write to the standard output the answers and will write any other information to the standard error. You can safely pipe the output to your file or next piping command and will still get all the information and errors on stderr.
 
 It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by the selected AI model in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
 
-By default, tulp uses **gpt-4-0125-preview**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
+By default, tulp uses **gpt-4o**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
 
 ### Options:
 ```
 usage: tulp [-h] [-x] [-w W] [--model MODEL] [--max-chars MAX_CHARS] [-v] [-q] [--groq_api_key GROQ_API_KEY] [--ollama_host OLLAMA_HOST] [--anthropic_api_key ANTHROPIC_API_KEY] [--openai_api_key OPENAI_API_KEY] [--openai_baseurl OPENAI_BASEURL] [--gemini_api_key GEMINI_API_KEY] ...
 
 TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with support for multiple AI APIs including groq, ollama, anthropic, and gemini.
 
@@ -72,28 +72,28 @@
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. 
 
 The following are the parameters that can be configured:
 - **LOG_LEVEL**: The log level of Tulp. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
 - **API_KEYS**: The API keys for the supported AI models (OpenAI, GROQ, Ollama, Anthropic, Gemini). The default value is an empty string for each.
 - **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 40000.
-- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4-0125-preview, but other models are also available.
+- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4o but other models are also available.
 
 All these settings could be overridden by an environment variable using the prefix TULP\_ or by the different command line arguments described above. 
 As environment variables, they will become: TULP_LOG_LEVEL, TULP_API_KEYS, TULP_MAX_CHARS, or TULP_MODEL.
 Command line arguments will override environmental variables and the configuration file.
 
 
 Here is an example configuration file with the default values:
 ```INI
 [DEFAULT]
 LOG_LEVEL = INFO
 ${MODEL}_API_KEYS = <<<YOUR API KEYS FOR GROQ, OLLAMA, ANTHROPIC, OPENAI, GEMINI>>>
 MAX_CHARS = 40000
-MODEL = gpt-4-0125-preview
+MODEL = gpt-4o
 ```
 
 
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspiration:
 
 ### Random
@@ -240,14 +240,18 @@
 ```
 
 # Why?
 
 I am a heavy user of Unix tooling (e.g: awk, jq, sed, grep, and so on), I have been using them since my early days and I used to think that I couldn't survive without them. But then, ChatGPT appeared, and I started to use more and more GPT for things that I used to use Unix tooling for. Somehow I feel the pain of cut & paste, and I was missing a way to do it faster and from within the terminal itself, so I came up with `tulp`.
 
 # Changelog
+## v2.1 | 2024-05-14
+- Improves formating of messages for gemini
+- Changed to use gpt-4o model by default
+
 ## v2.0 | 2024-05-04
 - Added support for groq, ollama, anthropic, and gemini AI models.
 - Changed to use gpt-4-turbo model by default
 
 ## v1.0 | 2024-02-14
 - Changed to use gpt-4-0125-preview model by default
 - Updated to use openapi v1.0
```

### Comparing `tulp-2.0/setup.cfg` & `tulp-2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tulp-2.0/test/test_filterMode_advanced.py` & `tulp-2.1/test/test_filterMode_advanced.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/test/test_filterMode_basic.py` & `tulp-2.1/test/test_filterMode_basic.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/test/test_requestMode.py` & `tulp-2.1/test/test_requestMode.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/test/test_slowtest.py` & `tulp-2.1/test/test_slowtest.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/TulpOutputFileWriter.py` & `tulp-2.1/tulp/TulpOutputFileWriter.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/createFilteringProgramPrompt.py` & `tulp-2.1/tulp/createFilteringProgramPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/createProgramPrompt.py` & `tulp-2.1/tulp/createProgramPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/filteringPrompt.py` & `tulp-2.1/tulp/filteringPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/llms/LlmAnthropic.py` & `tulp-2.1/tulp/llms/LlmAnthropic.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/llms/LlmGemini.py` & `tulp-2.1/tulp/llms/LlmGemini.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     def __init__(self,config):
         self.config = config
         key = config.gemini_api_key
         if not key:
             log.error(f'Gemini API key not found. Please set the TULP_GEMINI_API_KEY environment variable or add it to {tulpconfig.CONFIG_FILE}')
             sys.exit(1)
         genai.configure(api_key=key)
-        self.model = genai.GenerativeModel('gemini-pro')
 
         # Safety config
         self.safety_settings={
         HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_NONE,
         HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_NONE,
     }
 
@@ -31,15 +30,22 @@
 
 
     def convertMessagesFromOpenAIToGemini(self, messages):
         gmessages = []
         pRole = None
         pParts = None
         for msg in messages:
-            cRole = (msg['role'] == "assistant" and "model" or "user")
+            mRole = msg['role']
+            if mRole == "assistant":
+              cRole = "model"
+            elif mRole == "system" and (pRole == "system" or pRole==None): 
+              # system is only accepted as the first system_instruction, any other message will be converted to user
+              cRole = "system"
+            else:
+              cRole = "user"
             if pRole and cRole != pRole:
                gmessages.append( {'role': pRole , 'parts': pParts } )
                pRole = None
             if not pRole:
                 pRole = cRole
                 pParts = [msg['content']]
             else:
@@ -63,22 +69,32 @@
 
     def generate(self, messages):
         """
         Writes the given content to the given file name. If the file already exists, it will rename it to a new file on the same folder, appending to the file name a counter (like -1) and keeping the same extension. It will continually increase the counter until it finds a free object.
 
         :param file_name: The name of the file to write to.
         """
+
         gmessages = self.convertMessagesFromOpenAIToGemini(messages)
+        if gmessages[0]['role'] == "system":
+            self.model = genai.GenerativeModel(self.config.model, system_instruction="\n".join(gmessages[0]['parts']))
+            log.debug(f"Adding system message!")
+            gmessages = gmessages[1:]
+        else:
+            self.model = genai.GenerativeModel(self.config.model)
+
+
         for req in gmessages:
             log.debug(f"REQ: {req}")
         log.debug(f"Sending the request to llm...")
         response = self.model.generate_content(gmessages,
-                    safety_settings=self.safety_settings)
+                    safety_settings=self.safety_settings,  request_options={"timeout": 600})
 
 
         cand = response.candidates[0]
         log.debug(f"ANS: {cand.content}")
         log.debug(f"ANS: finish: {cand.finish_reason}")
+        # https://ai.google.dev/api/rest/v1/GenerateContentResponse#FinishReason
         return { 
                 "response_text": cand.content.parts[0].text,
                 "finish_reason": cand.finish_reason
                }
```

### Comparing `tulp-2.0/tulp/llms/LlmGroq.py` & `tulp-2.1/tulp/llms/LlmGroq.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/llms/LlmOllama.py` & `tulp-2.1/tulp/llms/LlmOllama.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/llms/LlmOpenAI.py` & `tulp-2.1/tulp/llms/LlmOpenAI.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/llms/__init__.py` & `tulp-2.1/tulp/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/requestPrompt.py` & `tulp-2.1/tulp/requestPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/tulp.py` & `tulp-2.1/tulp/tulp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/python3
 
 import sys
 import os
+import re
 import math
 from . import tulpargs
 from . import tulplogger
 from . import tulpconfig
 from . import version
 from . import TulpOutputFileWriter
 
@@ -16,16 +17,18 @@
 llmclient: object  # will be defined in main
 
 # Helper functions
 
 ## cleanup_output: clenaup output, removing artifacts
 def cleanup_output(output):
     olines = output.strip().splitlines()
+
+    blockRe = re.compile(r'^```',re.MULTILINE)
     # gpt-3.5 usually adds unneeded markdown codeblock wrappers, try to remove them
-    if len(olines) > 2:
+    if len(blockRe.findall(output)) == 2 and len(olines) > 2:
         if olines[0].startswith("```") and olines[-1] == "```":
             log.info("markdown codeblock wrapping detected and stripped!")
             return "\n".join(olines[1:-1])
     return output
 
 
 ## block_exists(blocks_dict, key):  test if a KEY exist and is not empty
```

### Comparing `tulp-2.0/tulp/tulpargs.py` & `tulp-2.1/tulp/tulpargs.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp/tulpconfig.py` & `tulp-2.1/tulp/tulpconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,13 +28,13 @@
             cls._instance.config = configparser.ConfigParser()
             cls._instance.config.read(CONFIG_FILE)
 
 
             cls._instance.log_level = (args.v and "DEBUG") or (args.q and "ERROR")  or cls._instance.getValue("LOG_LEVEL", "INFO")
             tulplogger.setLogLevel(cls._instance.log_level)
             cls._instance.max_chars = int(args.max_chars or cls._instance.getValue("MAX_CHARS", "40000"))
-            cls._instance.model = args.model or cls._instance.getValue("MODEL", "gpt-4-turbo")
+            cls._instance.model = args.model or cls._instance.getValue("MODEL", "gpt-4o")
             cls._instance.loadLlmsArguments(args)
 
         return cls._instance
```

### Comparing `tulp-2.0/tulp/tulplogger.py` & `tulp-2.1/tulp/tulplogger.py`

 * *Files identical despite different names*

### Comparing `tulp-2.0/tulp.egg-info/PKG-INFO` & `tulp-2.1/tulp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 2.0
+Version: 2.1
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 ```
 
 
 In both cases, TULP will write to the standard output the answers and will write any other information to the standard error. You can safely pipe the output to your file or next piping command and will still get all the information and errors on stderr.
 
 It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by the selected AI model in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
 
-By default, tulp uses **gpt-4-0125-preview**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
+By default, tulp uses **gpt-4o**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
 
 ### Options:
 ```
 usage: tulp [-h] [-x] [-w W] [--model MODEL] [--max-chars MAX_CHARS] [-v] [-q] [--groq_api_key GROQ_API_KEY] [--ollama_host OLLAMA_HOST] [--anthropic_api_key ANTHROPIC_API_KEY] [--openai_api_key OPENAI_API_KEY] [--openai_baseurl OPENAI_BASEURL] [--gemini_api_key GEMINI_API_KEY] ...
 
 TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with support for multiple AI APIs including groq, ollama, anthropic, and gemini.
 
@@ -91,28 +91,28 @@
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. 
 
 The following are the parameters that can be configured:
 - **LOG_LEVEL**: The log level of Tulp. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
 - **API_KEYS**: The API keys for the supported AI models (OpenAI, GROQ, Ollama, Anthropic, Gemini). The default value is an empty string for each.
 - **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 40000.
-- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4-0125-preview, but other models are also available.
+- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4o but other models are also available.
 
 All these settings could be overridden by an environment variable using the prefix TULP\_ or by the different command line arguments described above. 
 As environment variables, they will become: TULP_LOG_LEVEL, TULP_API_KEYS, TULP_MAX_CHARS, or TULP_MODEL.
 Command line arguments will override environmental variables and the configuration file.
 
 
 Here is an example configuration file with the default values:
 ```INI
 [DEFAULT]
 LOG_LEVEL = INFO
 ${MODEL}_API_KEYS = <<<YOUR API KEYS FOR GROQ, OLLAMA, ANTHROPIC, OPENAI, GEMINI>>>
 MAX_CHARS = 40000
-MODEL = gpt-4-0125-preview
+MODEL = gpt-4o
 ```
 
 
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspiration:
 
 ### Random
@@ -259,14 +259,18 @@
 ```
 
 # Why?
 
 I am a heavy user of Unix tooling (e.g: awk, jq, sed, grep, and so on), I have been using them since my early days and I used to think that I couldn't survive without them. But then, ChatGPT appeared, and I started to use more and more GPT for things that I used to use Unix tooling for. Somehow I feel the pain of cut & paste, and I was missing a way to do it faster and from within the terminal itself, so I came up with `tulp`.
 
 # Changelog
+## v2.1 | 2024-05-14
+- Improves formating of messages for gemini
+- Changed to use gpt-4o model by default
+
 ## v2.0 | 2024-05-04
 - Added support for groq, ollama, anthropic, and gemini AI models.
 - Changed to use gpt-4-turbo model by default
 
 ## v1.0 | 2024-02-14
 - Changed to use gpt-4-0125-preview model by default
 - Updated to use openapi v1.0
```

### Comparing `tulp-2.0/tulp.egg-info/SOURCES.txt` & `tulp-2.1/tulp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

