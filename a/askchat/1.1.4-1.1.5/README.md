# Comparing `tmp/askchat-1.1.4.tar.gz` & `tmp/askchat-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askchat-1.1.4.tar", last modified: Mon Apr 29 16:06:11 2024, max compression
+gzip compressed data, was "askchat-1.1.5.tar", last modified: Tue May 14 16:02:49 2024, max compression
```

## Comparing `askchat-1.1.4.tar` & `askchat-1.1.5.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.824930 askchat-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 16:06:00.000000 askchat-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-29 16:06:00.000000 askchat-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-29 16:06:11.824930 askchat-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-29 16:06:00.000000 askchat-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.820930 askchat-1.1.4/askchat/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/askenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.820930 askchat-1.1.4/askchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 16:06:11.824930 askchat-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-29 16:06:00.000000 askchat-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.824930 askchat-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 16:06:00.000000 askchat-1.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-29 16:06:00.000000 askchat-1.1.4/tests/test_askchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-29 16:06:00.000000 askchat-1.1.4/tests/test_askenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.534645 askchat-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 16:02:41.000000 askchat-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-14 16:02:41.000000 askchat-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-14 16:02:49.534645 askchat-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-14 16:02:41.000000 askchat-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/askchat/
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/askenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/askchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   492951 2024-05-14 16:02:41.000000 askchat-1.1.5/docs/assets/askchat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 16:02:49.534645 askchat-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 16:02:41.000000 askchat-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.534645 askchat-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 16:02:41.000000 askchat-1.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-14 16:02:41.000000 askchat-1.1.5/tests/test_askchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-14 16:02:41.000000 askchat-1.1.5/tests/test_askenv.py
```

### Comparing `askchat-1.1.4/LICENSE` & `askchat-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `askchat-1.1.4/PKG-INFO` & `askchat-1.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.4
+Version: 1.1.5
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.4/askchat/__init__.py` & `askchat-1.1.5/askchat/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for askchat."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '1.1.4'
+__version__ = '1.1.5'
 
 import asyncio
 from pathlib import Path
 import click
 from dotenv import set_key
 import os
 
@@ -53,45 +53,45 @@
 
 # common functions
 async def show_resp(chat, **options):
     msg = ''
     async for char in chat.async_stream_responses(textonly=True, **options):
         print(char, end='', flush=True)
         msg += char
-        await asyncio.sleep(0.01)
+        # await asyncio.sleep(0.01)
     if not msg.endswith('\n'):
         print() # add a newline if the message doesn't end with one
     return msg
 
 def set_keys(config_file, keys):
     """Set multiple keys in the config file."""
     for key, value in keys.items():
         if value:
             set_key(config_file, key, value)
 
-def raw_config(config_file:str):
+def create_empty_config(config_file:str):
     """Empty config file."""
     if not CONFIG_PATH.exists():
         CONFIG_PATH.mkdir(parents=True)
     with open(config_file, "w") as f:
         f.write(raw_env_text)
 
-def init_config(config_file:str):
+def initialize_config(config_file:str):
     """Initialize the config file with the current environment variables."""
-    raw_config(config_file)
+    create_empty_config(config_file)
     set_keys(config_file, {
         "OPENAI_API_KEY": os.getenv("OPENAI_API_KEY"),
         "OPENAI_API_MODEL": os.getenv("OPENAI_API_MODEL"),
         "OPENAI_API_BASE_URL": os.getenv("OPENAI_API_BASE_URL"),
         "OPENAI_API_BASE": os.getenv("OPENAI_API_BASE"),
     })
 
 def write_config(config_file, api_key, model, base_url, api_base, overwrite=False):
     """Write the environment variables to a config file."""
     if overwrite or not config_file.exists():
-        raw_config(config_file)
+        create_empty_config(config_file)
     set_keys(config_file, {
         "OPENAI_API_KEY": api_key,
         "OPENAI_API_MODEL": model,
         "OPENAI_API_BASE_URL": base_url,
         "OPENAI_API_BASE": api_base,
     })
```

### Comparing `askchat-1.1.4/askchat/askenv.py` & `askchat-1.1.5/askchat/askenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 def config(name, api_key, base_url, api_base, model):
     """Update default .env values."""
     if not any([api_key, base_url, api_base, model]):
         click.echo("No updates made. Provide at least one option to update.")
         return
     config_path = ENV_PATH / f'{name}.env' if name else MAIN_ENV_PATH
     if not config_path.exists():
-        click.echo(f"Environment '{config_path}' not found." +\
+        click.echo(f"Environment '{config_path}' not found.\n" +\
                    "Use `askenv new` to create a new environment." )
         return
     write_config(config_path, api_key, model, base_url, api_base)
     click.echo(f"Environment {config_path} updated.")
 
 if __name__ == '__main__':
     cli()
```

### Comparing `askchat-1.1.4/askchat/cli.py` & `askchat-1.1.5/askchat/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from pprint import pprint
 from dotenv import load_dotenv
 import asyncio, os, shutil
 from chattool import Chat, debug_log
 from pathlib import Path
 from askchat import (
-      show_resp, write_config, init_config
+      show_resp, write_config, initialize_config
     , ENV_PATH, MAIN_ENV_PATH
     , CONFIG_PATH, CONFIG_FILE
     , EnvNameCompletionType, ChatFileCompletionType
 )
 
 # Version and Config Path
 VERSION = askchat.__version__
@@ -36,15 +36,15 @@
 # callback functions for general options
 def generate_config_callback(ctx, param, value):
     """Generate a configuration file by environment table."""
     if not value: return
     # save the config file
     if os.path.exists(CONFIG_FILE):
         click.confirm(f"Overwrite the existing configuration file {CONFIG_FILE}?", abort=True)
-    init_config(CONFIG_FILE)
+    initialize_config(CONFIG_FILE)
     print("Created config file at", CONFIG_FILE)
     ctx.exit()
 
 def debug_log_callback(ctx, param, value):
     if not value: return
     setup()
     debug_log()
```

### Comparing `askchat-1.1.4/askchat.egg-info/PKG-INFO` & `askchat-1.1.5/askchat.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.4
+Version: 1.1.5
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.4/setup.py` & `askchat-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 requirements = ['chattool>=3.1.4', "python-dotenv>=0.17.0", 'Click>=8.0']
 
 test_requirements = ['pytest>=3']
```

### Comparing `askchat-1.1.4/tests/test_askchat.py` & `askchat-1.1.5/tests/test_askchat.py`

 * *Files identical despite different names*

### Comparing `askchat-1.1.4/tests/test_askenv.py` & `askchat-1.1.5/tests/test_askenv.py`

 * *Files identical despite different names*

