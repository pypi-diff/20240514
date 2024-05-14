# Comparing `tmp/cli-FSD-1.0.5.tar.gz` & `tmp/cli-FSD-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-FSD-1.0.5.tar", last modified: Sun Apr 21 18:17:10 2024, max compression
+gzip compressed data, was "cli-FSD-1.0.7.tar", last modified: Tue May 14 03:04:51 2024, max compression
```

## Comparing `cli-FSD-1.0.5.tar` & `cli-FSD-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 18:17:10.931190 cli-FSD-1.0.5/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    35149 2024-04-19 17:06:09.000000 cli-FSD-1.0.5/LICENSE
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 18:17:10.929175 cli-FSD-1.0.5/PKG-INFO
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     4672 2024-04-19 17:19:52.000000 cli-FSD-1.0.5/README.md
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 18:17:10.585634 cli-FSD-1.0.5/cli_FSD/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      694 2024-04-19 17:06:10.000000 cli-FSD-1.0.5/cli_FSD/__init__.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5806 2024-04-19 17:06:10.000000 cli-FSD-1.0.5/cli_FSD/engine.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    49029 2024-04-21 17:55:11.000000 cli-FSD-1.0.5/cli_FSD/main.py
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 18:17:10.906191 cli-FSD-1.0.5/cli_FSD/resources/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:06:10.000000 cli-FSD-1.0.5/cli_FSD/resources/__init__.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5753 2024-04-19 17:06:10.000000 cli-FSD-1.0.5/cli_FSD/resources/assembler.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      790 2024-04-19 17:08:03.000000 cli-FSD-1.0.5/cli_FSD/resources/test-ollama.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    46728 2024-04-19 17:08:01.000000 cli-FSD-1.0.5/cli_FSD/resources/v0.94.py
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 18:17:10.764380 cli-FSD-1.0.5/cli_FSD.egg-info/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 18:17:10.000000 cli-FSD-1.0.5/cli_FSD.egg-info/PKG-INFO
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      389 2024-04-21 18:17:10.000000 cli-FSD-1.0.5/cli_FSD.egg-info/SOURCES.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        1 2024-04-21 18:17:10.000000 cli-FSD-1.0.5/cli_FSD.egg-info/dependency_links.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       41 2024-04-21 18:17:10.000000 cli-FSD-1.0.5/cli_FSD.egg-info/entry_points.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       52 2024-04-21 18:17:10.000000 cli-FSD-1.0.5/cli_FSD.egg-info/requires.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        8 2024-04-21 18:17:10.000000 cli-FSD-1.0.5/cli_FSD.egg-info/top_level.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       38 2024-04-21 18:17:10.932175 cli-FSD-1.0.5/setup.cfg
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      848 2024-04-21 18:13:40.000000 cli-FSD-1.0.5/setup.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-05-14 03:04:51.498093 cli-FSD-1.0.7/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    35149 2024-04-19 17:06:09.000000 cli-FSD-1.0.7/LICENSE
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-05-14 03:04:51.491861 cli-FSD-1.0.7/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     4672 2024-04-19 17:19:52.000000 cli-FSD-1.0.7/README.md
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-05-14 03:04:51.009810 cli-FSD-1.0.7/cli_FSD/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      694 2024-04-19 17:06:10.000000 cli-FSD-1.0.7/cli_FSD/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5806 2024-04-19 17:06:10.000000 cli-FSD-1.0.7/cli_FSD/engine.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    49061 2024-05-14 03:01:00.000000 cli-FSD-1.0.7/cli_FSD/main.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-05-14 03:04:51.447150 cli-FSD-1.0.7/cli_FSD/resources/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:06:10.000000 cli-FSD-1.0.7/cli_FSD/resources/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5753 2024-04-19 17:06:10.000000 cli-FSD-1.0.7/cli_FSD/resources/assembler.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      790 2024-04-19 17:08:03.000000 cli-FSD-1.0.7/cli_FSD/resources/test-ollama.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    46728 2024-04-19 17:08:01.000000 cli-FSD-1.0.7/cli_FSD/resources/v0.94.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-05-14 03:04:51.231638 cli-FSD-1.0.7/cli_FSD.egg-info/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-05-14 03:04:50.000000 cli-FSD-1.0.7/cli_FSD.egg-info/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      389 2024-05-14 03:04:50.000000 cli-FSD-1.0.7/cli_FSD.egg-info/SOURCES.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        1 2024-05-14 03:04:50.000000 cli-FSD-1.0.7/cli_FSD.egg-info/dependency_links.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       41 2024-05-14 03:04:50.000000 cli-FSD-1.0.7/cli_FSD.egg-info/entry_points.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       52 2024-05-14 03:04:50.000000 cli-FSD-1.0.7/cli_FSD.egg-info/requires.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        8 2024-05-14 03:04:50.000000 cli-FSD-1.0.7/cli_FSD.egg-info/top_level.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       38 2024-05-14 03:04:51.501466 cli-FSD-1.0.7/setup.cfg
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      848 2024-05-14 03:02:12.000000 cli-FSD-1.0.7/setup.py
```

### Comparing `cli-FSD-1.0.5/LICENSE` & `cli-FSD-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.5/PKG-INFO` & `cli-FSD-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-FSD
-Version: 1.0.5
+Version: 1.0.7
 Summary: LLM-enabled companion utility for your terminal.
 Home-page: https://github.com/wazacraft/cli-FSD
 Author: JG
 Author-email: wazacraftRFID@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cli-FSD-1.0.5/README.md` & `cli-FSD-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.5/cli_FSD/__init__.py` & `cli-FSD-1.0.7/cli_FSD/__init__.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.5/cli_FSD/engine.py` & `cli-FSD-1.0.7/cli_FSD/engine.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.5/cli_FSD/main.py` & `cli-FSD-1.0.7/cli_FSD/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#0.9.4d
-# adding Ollama support
+#1.3
+# added gpt-4o as default model
 
 # Added claude-3-opus mode and flag (-c)
 # added foundation for OpenAI assistants api routing but it's not working yet 
    
 #to-do: resolve response threadID error, fix flag for assistants api (ci) reimplement replicate flow, robust CMD mode and help log           
 
 import os
@@ -28,14 +28,16 @@
 import shlex
 import queue
 import ollama
 from ollama import Client
 import httpx
 import urllib.parse
 from groq import Groq as GroqClient
+import base64
+
 
 
 
 global llm_suggestions 
 global replicate_suggestions  # This will store suggestions from Replicate
 replicate_suggestions = ""
 global groq_client
@@ -68,28 +70,29 @@
 
 
 
 dotenv_path = Path('.env')
 load_dotenv(dotenv_path=dotenv_path)
 
 models = {
+    "gpt-4o": "gpt-4o",
     "gpt4": "gpt-4",
     "gpt40613": "gpt-4-0613",
     "gpt432k0613": "gpt-4-32k-0613",
     "35turbo": "gpt-3.5-turbo",
     "gpt-3.5-turbo-0125": "gpt-3.5-turbo-0125",
     "gpt-4-32k-0613	": "gpt-4-32k-0613",
     "gpt-4-turbo-preview": "gpt-4-turbo-preview",
     "gpt-4-vision-preview": "gpt-4-vision-preview",
     "dall-e-3":"dall-e-3",
     
 }
 
 
-current_model = os.getenv("DEFAULT_MODEL", "gpt-4-turbo-preview")
+current_model = os.getenv("DEFAULT_MODEL", "gpt-4o")
 api_key = os.getenv("OPENAI_API_KEY")
 if not api_key:
     api_key = input("Please enter your OpenAI API key: ")
     dotenv_path.touch(exist_ok=True)
     set_key(dotenv_path, "OPENAI_API_KEY", api_key)
 
 
@@ -1021,8 +1024,8 @@
 
 
     print("Operation completed.")
     stop_event.set()
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `cli-FSD-1.0.5/cli_FSD/resources/assembler.py` & `cli-FSD-1.0.7/cli_FSD/resources/assembler.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.5/cli_FSD/resources/test-ollama.py` & `cli-FSD-1.0.7/cli_FSD/resources/test-ollama.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.5/cli_FSD/resources/v0.94.py` & `cli-FSD-1.0.7/cli_FSD/resources/v0.94.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.5/cli_FSD.egg-info/PKG-INFO` & `cli-FSD-1.0.7/cli_FSD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-FSD
-Version: 1.0.5
+Version: 1.0.7
 Summary: LLM-enabled companion utility for your terminal.
 Home-page: https://github.com/wazacraft/cli-FSD
 Author: JG
 Author-email: wazacraftRFID@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cli-FSD-1.0.5/setup.py` & `cli-FSD-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-FSD',
-    version='1.0.5',
+    version='1.0.7',
     author='JG',
     author_email='wazacraftRFID@gmail.com',
     description='LLM-enabled companion utility for your terminal.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/wazacraft/cli-FSD',
     packages=find_packages(),
```

