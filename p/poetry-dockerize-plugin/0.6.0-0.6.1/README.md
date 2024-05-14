# Comparing `tmp/poetry_dockerize_plugin-0.6.0.tar.gz` & `tmp/poetry_dockerize_plugin-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_dockerize_plugin-0.6.0.tar", max compression
+gzip compressed data, was "poetry_dockerize_plugin-0.6.1.tar", max compression
```

## Comparing `poetry_dockerize_plugin-0.6.0.tar` & `poetry_dockerize_plugin-0.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/LICENSE
--rw-r--r--   0        0        0     4471 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/__init__.py
--rw-r--r--   0        0        0    13459 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/builder.py
--rw-r--r--   0        0        0     1239 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/plugin.py
--rw-r--r--   0        0        0     1997 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4471 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/__init__.py
+-rw-r--r--   0        0        0    13196 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/builder.py
+-rw-r--r--   0        0        0     1239 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/plugin.py
+-rw-r--r--   0        0        0     1997 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-0.6.1/PKG-INFO
```

### Comparing `poetry_dockerize_plugin-0.6.0/LICENSE` & `poetry_dockerize_plugin-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-0.6.0/README.md` & `poetry_dockerize_plugin-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/builder.py` & `poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os.path
 import re
 import sys
 import tempfile
 import time
 from pathlib import Path
 from typing import List, Optional
@@ -187,17 +186,15 @@
      && apt-get update \
      && apt-get -y dist-upgrade \
      && apt-get -y install {apt_packages_str}"""
 
 
 def generate_add_project_toml_str(config: ProjectConfiguration, real_context_path: str) -> str:
     add_str = "RUN mkdir /app\n"
-    if os.path.exists(os.path.join(real_context_path, "poetry.lock")):
-        add_str += "COPY poetry.lock /app/poetry.lock\n"
-    add_str += "COPY pyproject.toml /app/pyproject.toml\n"
+    add_str += "COPY pyproject.toml poetry.lock* README* /app/\n"
     for package in list(set(config.deps_packages)):
         if os.path.exists(os.path.join(real_context_path, package)):
             add_str += f"COPY ./{package} /app/{package}\n"
         else:
             print(f"WARNING: {package} not found, skipping it")
     return add_str
 
@@ -215,27 +212,25 @@
     cmd_str = " ".join(config.entrypoint)
     envs_str = "\n".join([f"ENV {key}={value}" for key, value in config.envs.items()])
     labels_str = "\n".join([f"LABEL {key}={value}" for key, value in config.labels.items()])
     return f"""
 FROM {config.base_image} as builder
 RUN pip install poetry==1.7.1
 
-ENV POETRY_NO_INTERACTION=1
 ENV POETRY_VIRTUALENVS_IN_PROJECT=1
 ENV POETRY_VIRTUALENVS_CREATE=1
 ENV POETRY_CACHE_DIR=/tmp/poetry_cache
-RUN poetry config virtualenvs.create false && poetry config virtualenvs.in-project false
 
 {generate_apt_packages_str(config.build_apt_packages)}
 {generate_add_project_toml_str(config, real_context_path)}
 
 {generate_add_packages_str(config, real_context_path)}
 {generate_extra_instructions_str(config.extra_build_instructions)}
 
-RUN cd /app && poetry install --no-interaction --no-ansi --no-root
+RUN cd /app && poetry install --no-interaction --no-ansi
 
 FROM {config.base_image} as runtime
 {generate_apt_packages_str(config.runtime_apt_packages)}
 {labels_str}
 
 ENV PATH="/app/.venv/bin:$PATH"
 ENV PYTHONUNBUFFERED=1
```

### Comparing `poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/plugin.py` & `poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-0.6.0/pyproject.toml` & `poetry_dockerize_plugin-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dockerize-plugin"
-version = "0.6.0"
+version = "0.6.1"
 description = "Poetry application to Docker, automatically."
 authors = ["Nicolò Boschi <boschi1997@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["poetry", "packaging", "docker"]
 repository = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
 documentation = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
```

### Comparing `poetry_dockerize_plugin-0.6.0/PKG-INFO` & `poetry_dockerize_plugin-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-dockerize-plugin
-Version: 0.6.0
+Version: 0.6.1
 Summary: Poetry application to Docker, automatically.
 Home-page: https://github.com/nicoloboschi/poetry-dockerize-plugin
 License: MIT
 Keywords: poetry,packaging,docker
 Author: Nicolò Boschi
 Author-email: boschi1997@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 0.6.0 Summary:
+Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 0.6.1 Summary:
 Poetry application to Docker, automatically. Home-page: https://github.com/
 nicoloboschi/poetry-dockerize-plugin License: MIT Keywords:
 poetry,packaging,docker Author: NicolÃ² Boschi Author-email:
 boschi1997@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
```

