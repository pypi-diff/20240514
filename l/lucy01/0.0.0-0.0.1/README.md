# Comparing `tmp/lucy01-0.0.0.tar.gz` & `tmp/lucy01-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucy01-0.0.0.tar", last modified: Tue May 14 08:41:07 2024, max compression
+gzip compressed data, was "lucy01-0.0.1.tar", last modified: Tue May 14 09:07:59 2024, max compression
```

## Comparing `lucy01-0.0.0.tar` & `lucy01-0.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:41:07.716579 lucy01-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-14 08:41:07.716579 lucy01-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-14 08:41:03.000000 lucy01-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:41:07.712579 lucy01-0.0.0/lucy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:41:07.712579 lucy01-0.0.0/lucy/parser_/
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/parser_/atcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/parser_/contest.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/parser_/parser_.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/update_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-14 08:41:03.000000 lucy01-0.0.0/lucy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:41:07.716579 lucy01-0.0.0/lucy01.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-14 08:41:07.000000 lucy01-0.0.0/lucy01.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 08:41:07.000000 lucy01-0.0.0/lucy01.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:41:07.000000 lucy01-0.0.0/lucy01.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 08:41:07.000000 lucy01-0.0.0/lucy01.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 08:41:07.000000 lucy01-0.0.0/lucy01.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 08:41:07.000000 lucy01-0.0.0/lucy01.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-14 08:41:03.000000 lucy01-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:41:07.716579 lucy01-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:07:59.625811 lucy01-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-14 09:07:59.625811 lucy01-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-14 09:07:55.000000 lucy01-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:07:59.625811 lucy01-0.0.1/lucy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:07:59.625811 lucy01-0.0.1/lucy/parser_/
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/parser_/atcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/parser_/contest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/parser_/parser_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/update_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-14 09:07:55.000000 lucy01-0.0.1/lucy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:07:59.625811 lucy01-0.0.1/lucy01.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-14 09:07:59.000000 lucy01-0.0.1/lucy01.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 09:07:59.000000 lucy01-0.0.1/lucy01.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:07:59.000000 lucy01-0.0.1/lucy01.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 09:07:59.000000 lucy01-0.0.1/lucy01.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 09:07:59.000000 lucy01-0.0.1/lucy01.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 09:07:59.000000 lucy01-0.0.1/lucy01.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 09:07:55.000000 lucy01-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:07:59.625811 lucy01-0.0.1/setup.cfg
```

### Comparing `lucy01-0.0.0/PKG-INFO` & `lucy01-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lucy01
-Version: 0.0.0
-Summary: CLI helper for CP contests.
+Version: 0.0.1
+Summary: CLI companion for CP.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: requests
 Requires-Dist: selenium
@@ -36,15 +36,15 @@
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
 
 ## Getting Started
-1. Set the environment variable `$LUCY_HOME` as preferred.
+1. Set the environment variable `$LUCY_HOME` as preferred. By default, it uses the `~/.lucy`.
 2. Get help!
     ```
     lucy --help
     ```
 
 ## Directory Structure
 ```
```

### Comparing `lucy01-0.0.0/README.md` & `lucy01-0.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
 
 ## Getting Started
-1. Set the environment variable `$LUCY_HOME` as preferred.
+1. Set the environment variable `$LUCY_HOME` as preferred. By default, it uses the `~/.lucy`.
 2. Get help!
     ```
     lucy --help
     ```
 
 ## Directory Structure
 ```
```

### Comparing `lucy01-0.0.0/lucy/config.py` & `lucy01-0.0.1/lucy/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,29 +27,28 @@
         return self.name.lower()
 
 
 @dataclass
 class Config:
     WEBSITE_HOST = {Website.ATCODER: 'https://atcoder.jp'}
 
-    LUCY_HOME = os.getenv('LUCY_HOME')
-    if not LUCY_HOME:
-        raise ValueError('`$LUCY_HOME` not set!')
+    LUCY_HOME = os.getenv('LUCY_HOME') or f'{os.getenv("HOME")}/.lucy'
     LUCY_HOME = os.path.abspath(LUCY_HOME)
     os.makedirs(LUCY_HOME, exist_ok=True)
 
     SNIPPETS_DIR = f'{LUCY_HOME}/.vscode'
     os.makedirs(SNIPPETS_DIR, exist_ok=True)
     SNIPPETS_PATH = os.path.abspath(f'{SNIPPETS_DIR}/cp.code-snippets')
 
     COMMONS_PATH = os.path.abspath(f'{LUCY_HOME}/common')
     os.makedirs(COMMONS_PATH, exist_ok=True)
 
     TEMPLATE_PATH = f'{COMMONS_PATH}/base.cpp'
-    os.makedirs(COMMONS_PATH, exist_ok=True)
+    with open(TEMPLATE_PATH, 'w+', encoding='utf-8'):
+        pass
 
     CLI_WEBSITE_CHOICE = click.Choice(['atcoder'])
 
     IMPL_MAIN = 'main.cpp'
     IMPL_BIN = 'main'
 
     SAMPLES_DIR = 'tests'
```

### Comparing `lucy01-0.0.0/lucy/main.py` & `lucy01-0.0.1/lucy/main.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.0/lucy/parser_/atcoder.py` & `lucy01-0.0.1/lucy/parser_/atcoder.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.0/lucy/scraper.py` & `lucy01-0.0.1/lucy/scraper.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.0/lucy/tester.py` & `lucy01-0.0.1/lucy/tester.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.0/lucy/update_snippets.py` & `lucy01-0.0.1/lucy/update_snippets.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.0/lucy/utils.py` & `lucy01-0.0.1/lucy/utils.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.0/lucy01.egg-info/PKG-INFO` & `lucy01-0.0.1/lucy01.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lucy01
-Version: 0.0.0
-Summary: CLI helper for CP contests.
+Version: 0.0.1
+Summary: CLI companion for CP.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: requests
 Requires-Dist: selenium
@@ -36,15 +36,15 @@
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
 
 ## Getting Started
-1. Set the environment variable `$LUCY_HOME` as preferred.
+1. Set the environment variable `$LUCY_HOME` as preferred. By default, it uses the `~/.lucy`.
 2. Get help!
     ```
     lucy --help
     ```
 
 ## Directory Structure
 ```
```

### Comparing `lucy01-0.0.0/pyproject.toml` & `lucy01-0.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lucy01"
-version = "0.0.0"
-description = "CLI helper for CP contests."
+version = "0.0.1"
+description = "CLI companion for CP."
 readme = "README.md"
 dependencies = [
     "bs4",
     "click",
     "lxml",
     "requests",
     "selenium",
```

