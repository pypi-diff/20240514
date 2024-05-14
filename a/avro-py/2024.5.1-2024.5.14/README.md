# Comparing `tmp/avro_py-2024.5.1.tar.gz` & `tmp/avro_py-2024.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro_py-2024.5.1.tar", max compression
+gzip compressed data, was "avro_py-2024.5.14.tar", max compression
```

## Comparing `avro_py-2024.5.1.tar` & `avro_py-2024.5.14.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-01 12:02:57.923729 avro_py-2024.5.1/LICENSE
--rw-r--r--   0        0        0     6156 2024-05-01 12:02:57.923729 avro_py-2024.5.1/README.md
--rwxr-xr-x   0        0        0       77 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/__init__.py
--rw-r--r--   0        0        0     2883 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/cli.py
--rwxr-xr-x   0        0        0      799 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/config.py
--rwxr-xr-x   0        0        0    12937 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/main.py
--rw-r--r--   0        0        0       83 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/resources/__init__.py
--rw-r--r--   0        0        0    39017 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/resources/dictionary.py
--rw-r--r--   0        0        0       31 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/utils/__init__.py
--rwxr-xr-x   0        0        0      472 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/utils/count.py
--rwxr-xr-x   0        0        0     2311 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/utils/validate.py
--rw-r--r--   0        0        0     1746 2024-05-01 12:02:57.927729 avro_py-2024.5.1/pyproject.toml
--rw-r--r--   0        0        0     7357 1970-01-01 00:00:00.000000 avro_py-2024.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-14 10:03:13.402338 avro_py-2024.5.14/LICENSE
+-rw-r--r--   0        0        0     6276 2024-05-14 10:03:13.402338 avro_py-2024.5.14/README.md
+-rwxr-xr-x   0        0        0       77 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/__init__.py
+-rw-r--r--   0        0        0     2885 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/cli.py
+-rwxr-xr-x   0        0        0      799 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/config.py
+-rwxr-xr-x   0        0        0    13003 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/main.py
+-rw-r--r--   0        0        0       83 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/resources/__init__.py
+-rw-r--r--   0        0        0    39017 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/resources/dictionary.py
+-rw-r--r--   0        0        0       31 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/utils/__init__.py
+-rwxr-xr-x   0        0        0      472 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/utils/count.py
+-rwxr-xr-x   0        0        0     2311 2024-05-14 10:03:13.402338 avro_py-2024.5.14/avro/utils/validate.py
+-rw-r--r--   0        0        0     1827 2024-05-14 10:03:13.406338 avro_py-2024.5.14/pyproject.toml
+-rw-r--r--   0        0        0     7478 1970-01-01 00:00:00.000000 avro_py-2024.5.14/PKG-INFO
```

### Comparing `avro_py-2024.5.1/LICENSE` & `avro_py-2024.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `avro_py-2024.5.1/README.md` & `avro_py-2024.5.14/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -130,20 +130,29 @@
 
 ```sh
 # Set up virtual environment and activate it.
 $ python3 -m venv venv && source venv/bin/activate
 
 # Install required first-party dependencies and Poetry for dependency management.
 # (Note: Skip this step if Poetry is globally installed and added to PATH.)
-$ pip install -U pip setuptools && pip install poetry
+$ pip install -U pip setuptools
 
 # Setup project using Poetry.
 $ poetry install --all-extras
 ```
 
+Later, you can run the tests provided with the project using the following command:
+
+```sh
+# Run unit tests.
+$ poetry run pytest .
+```
+
+<br>
+
 ### 🐛 We're looking for bug hunters, by the way!
 
 If you come across any kind of bug or wanna request a feature, please let us know by opening an issue [here](https://github.com/hitblast/avro.py/issues). We do need more ideas to keep the project alive and running, don't we? :P
 
 ---
 
 <br>
```

### Comparing `avro_py-2024.5.1/avro/cli.py` & `avro_py-2024.5.14/avro/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         output = avro.reverse(text)
     else:
         output = avro.parse(text) if not bijoy else avro.parse(text, bijoy=True)
 
     if output == text:
         return _print_err("No changes in output.")
 
-    console.print(f"\n[bold green]Output[/bold green]\n {text}\n")
+    console.print(f"\n[bold green]Output[/bold green]\n {output}\n")
 
     if copy_on_success:
         pyclip.copy(text)
         console.print("[bold yellow](copied to clipboard)[/bold yellow]\n")
 
 
 # usage: avro parse <text> [--bijoy] [--from-clip] [--copy]
```

### Comparing `avro_py-2024.5.1/avro/config.py` & `avro_py-2024.5.14/avro/config.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.5.1/avro/main.py` & `avro_py-2024.5.14/avro/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: MIT
 
 
 # Import first-party Python libraries.
+import contextlib
 import re
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from functools import lru_cache
 from itertools import chain
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 # Import local modules.
@@ -51,15 +52,15 @@
     print(parsed)
     ```
     """
 
     # Compiled regular expression for UTF-8 validation
     utf8_regex = re.compile(r"\A[\x00-\x7F]*\Z")
 
-    @lru_cache
+    @lru_cache(maxsize=128)
     def _parse_backend(text: str) -> str:
         fixed_text = validate.fix_string_case(text)  # Sanitize input text.
         cur_end = 0  # Cursor end point.
 
         def output_generator() -> Generator[str, None, None]:
             nonlocal cur_end
 
@@ -122,15 +123,15 @@
     import avro
 
     converted = avro.to_bijoy('আমার সোনার বাংলা')
     print(converted)
     ```
     """
 
-    @lru_cache
+    @lru_cache(maxsize=128)
     def _convert_backend(text: str) -> str:
         text = _rearrange_unicode_text(re.sub("ৌ", "ৌ", re.sub("ো", "ো", text)))
 
         for unic in config.BIJOY_MAP:
             text = re.sub(unic, config.BIJOY_MAP[unic], text)
 
         return text.strip()
@@ -155,15 +156,15 @@
 
     reversed = avro.reverse('আমার সোনার বাংলা')
     print(reversed)
     ```
     """
 
     # Internal function for multiple reverses.
-    @lru_cache
+    @lru_cache(maxsize=128)
     def _reverse_backend(text: str) -> str:
         output = []  # The output list of strings.
 
         # Iterate through input text.
         for cur, i in enumerate(text):
             try:
                 i.encode("utf-8")
@@ -179,15 +180,15 @@
 
         return "".join(output)
 
     # Split using regex to remove noise.
     compiled_regex = re.compile("(\\s|\\.|,|\\?|\\।|\\-|;|')", re.UNICODE)
 
     # Extension for the _reverse_backend() function.
-    @lru_cache
+    @lru_cache(maxsize=128)
     def _reverse_backend_ext(text: str) -> str:
         exceptions = config.AVRO_EXCEPTIONS.get(text, None)
 
         if not exceptions:
             separated_texts = compiled_regex.split(text)
             text_segments = [_reverse_backend(separated_text) for separated_text in separated_texts]
             return "".join(text_segments)
@@ -323,23 +324,20 @@
         fixed_text[cursor] in config.AVRO_KAR
         or fixed_text[cursor] in config.AVRO_SHORBORNO
         or fixed_text[cursor] in config.AVRO_IGNORE
         or len(fixed_text) == cursor + 1
     ):
         added_suffix = "o"
 
-    try:
+    with contextlib.suppress(IndexError):
         if (fixed_text[cursor + 1] in config.AVRO_KAR) or (
             fixed_text[cursor + 2] in config.AVRO_KAR and not cursor == 0
         ):
             added_suffix = ""
 
-    except IndexError:
-        pass
-
     return text_reversed if not text_reversed else text_reversed + added_suffix
 
 
 def _process_rules(rules: Dict[str, Any], fixed_text: str, cur: int = 0, cur_end: int = 1) -> Optional[str]:
     """
     Process rules matched in pattern and returns suitable replacement.
```

### Comparing `avro_py-2024.5.1/avro/resources/dictionary.py` & `avro_py-2024.5.14/avro/resources/dictionary.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.5.1/avro/utils/validate.py` & `avro_py-2024.5.14/avro/utils/validate.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.5.1/pyproject.toml` & `avro_py-2024.5.14/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 "avro/__init__.py" = ["F403"]
 "avro/resources/__init__.py" = ["F403"]
 "avro/resources/dictionary.py" = ["F601"]
 "tests/test_main.py" = ["F601"]
 
 [tool.poetry]
 name = "avro-py"
-version = "2024.5.1"
+version = "2024.5.14"
 description = "A modern Pythonic implementation of Avro Phonetic."
 authors = ["HitBlast <hitblastlive@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "avro"}]
 homepage = "https://pypi.org/project/avro-py"
 repository = "https://github.com/hitblast/avro.py"
@@ -53,14 +53,18 @@
 click = { version="^8", optional = true }
 rich = { version="^13", optional = true }
 pyclip = { version="^0.7.0", optional = true }
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.1"
 
+[tool.poetry.group.docs.dependencies]
+setuptools = "^69.0.0"
+pdoc3 = "^0.10.0"
+
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.2"
 
 [tool.poetry.extras]
 cli = ["click", "rich", "pyclip"]
 
 [build-system]
```

### Comparing `avro_py-2024.5.1/PKG-INFO` & `avro_py-2024.5.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro-py
-Version: 2024.5.1
+Version: 2024.5.14
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://pypi.org/project/avro-py
 License: MIT
 Keywords: python,phonetics,avro,avro phonetic,bangla,bengali,bengali phonetics,transliteration
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -158,20 +158,29 @@
 
 ```sh
 # Set up virtual environment and activate it.
 $ python3 -m venv venv && source venv/bin/activate
 
 # Install required first-party dependencies and Poetry for dependency management.
 # (Note: Skip this step if Poetry is globally installed and added to PATH.)
-$ pip install -U pip setuptools && pip install poetry
+$ pip install -U pip setuptools
 
 # Setup project using Poetry.
 $ poetry install --all-extras
 ```
 
+Later, you can run the tests provided with the project using the following command:
+
+```sh
+# Run unit tests.
+$ poetry run pytest .
+```
+
+<br>
+
 ### 🐛 We're looking for bug hunters, by the way!
 
 If you come across any kind of bug or wanna request a feature, please let us know by opening an issue [here](https://github.com/hitblast/avro.py/issues). We do need more ideas to keep the project alive and running, don't we? :P
 
 ---
 
 <br>
```

