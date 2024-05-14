# Comparing `tmp/fresh_bakery-0.3.3.tar.gz` & `tmp/fresh_bakery-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fresh_bakery-0.3.3.tar", max compression
+gzip compressed data, was "fresh_bakery-0.3.5.tar", max compression
```

## Comparing `fresh_bakery-0.3.3.tar` & `fresh_bakery-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/LICENSE
--rw-r--r--   0        0        0     7945 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/README.md
--rw-r--r--   0        0        0      653 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/__init__.py
--rw-r--r--   0        0        0     4005 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/bakery.py
--rw-r--r--   0        0        0     8447 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/baking.py
--rw-r--r--   0        0        0     4965 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/cake.py
--rw-r--r--   0        0        0     2052 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/mypy.py
--rw-r--r--   0        0        0     2721 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/piece_of_cake.py
--rw-r--r--   0        0        0        0 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/py.typed
--rw-r--r--   0        0        0     3364 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/shape.py
--rw-r--r--   0        0        0     7962 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/stuff.py
--rw-r--r--   0        0        0     4994 2023-11-01 17:48:23.178041 fresh_bakery-0.3.3/bakery/testbakery.py
--rw-r--r--   0        0        0     4316 2023-11-01 17:48:23.186041 fresh_bakery-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     9048 1970-01-01 00:00:00.000000 fresh_bakery-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/LICENSE
+-rw-r--r--   0        0        0     7945 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/README.md
+-rw-r--r--   0        0        0      653 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/__init__.py
+-rw-r--r--   0        0        0     4005 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/bakery.py
+-rw-r--r--   0        0        0      470 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/bakery.pyi
+-rw-r--r--   0        0        0     8447 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/baking.py
+-rw-r--r--   0        0        0     4965 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/cake.py
+-rw-r--r--   0        0        0     2052 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/mypy.py
+-rw-r--r--   0        0        0     2721 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/piece_of_cake.py
+-rw-r--r--   0        0        0        0 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/py.typed
+-rw-r--r--   0        0        0     3364 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/shape.py
+-rw-r--r--   0        0        0     7962 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/stuff.py
+-rw-r--r--   0        0        0     4994 2024-05-14 06:28:53.904580 fresh_bakery-0.3.5/bakery/testbakery.py
+-rw-r--r--   0        0        0     4728 2024-05-14 06:28:53.912580 fresh_bakery-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     9048 1970-01-01 00:00:00.000000 fresh_bakery-0.3.5/PKG-INFO
```

### Comparing `fresh_bakery-0.3.3/LICENSE` & `fresh_bakery-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/README.md` & `fresh_bakery-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/__init__.py` & `fresh_bakery-0.3.5/bakery/__init__.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/bakery.py` & `fresh_bakery-0.3.5/bakery/bakery.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/baking.py` & `fresh_bakery-0.3.5/bakery/baking.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/cake.py` & `fresh_bakery-0.3.5/bakery/cake.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/mypy.py` & `fresh_bakery-0.3.5/bakery/mypy.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/piece_of_cake.py` & `fresh_bakery-0.3.5/bakery/piece_of_cake.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/shape.py` & `fresh_bakery-0.3.5/bakery/shape.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/stuff.py` & `fresh_bakery-0.3.5/bakery/stuff.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/bakery/testbakery.py` & `fresh_bakery-0.3.5/bakery/testbakery.py`

 * *Files identical despite different names*

### Comparing `fresh_bakery-0.3.3/pyproject.toml` & `fresh_bakery-0.3.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["poetry_core>=1.0.0"]
+requires = ["poetry_core>=1.1.0a6"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 99
 target-version = ["py310"]
 include = '\.pyi?$'
 skip-string-normalization = true
@@ -23,20 +23,21 @@
 known_third_party = [
     'pytest',
 ]
 known_local_folder = []
 multi_line_output = 3
 lines_after_imports = 2
 include_trailing_comma = true
-use_parentheses= true
+use_parentheses = true
+profile = "black"
 
 
 [tool.poetry]
 name = "fresh-bakery"
-version = "0.3.3"
+version = "0.3.5"
 description = "Bake your dependencies stupidly simple!"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -78,44 +79,56 @@
 
 [tool.pytest.ini_options]
 trio_mode = "true"
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<3.13"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "*"
 pydocstringformatter = [
     {version = "*", python = ">=3.8"},
 ]
 isort = "*"
-mypy = "^1.5.1"
+mypy = [
+    {version = "^1.10.0", python = ">=3.8"},
+    {version = ">1.0", python = "~3.7"},
+    {version = "0.971", python = "~3.6.2"}
+]
 pre-commit = "*"
-pylint = "^3.0.1"
+pylint = [
+    {version = "2.13.9", python = ">= 3.6.2, < 3.8"},
+    {version = "^3.1.0", python = ">= 3.8"},
+]
 pytest = "*"
 pytest-cov = "*"
 pytest-trio = "*"
 autoflake = "*"
 pytest-mock = "*"
 trio = "*"
 types-dataclasses = "*"
 sort-all = "*"
 tox = "*"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
 # documentation
 mkdocs = "^1.3.1"
 mkautodoc = "^0.2.0"
 pymdown-extensions = "^9.1"
 mkdocs-material = "^8.2.11"
 jinja2 = "^3.0.3"
 
 [tool.pylint]
 # https://pylint.pycqa.org/en/latest/user_guide/configuration/all-options.html
 [tool.pylint.master]
 jobs = 0
-disable = ["unnecessary-dunder-call", "duplicate-code"]
+disable = ["unnecessary-dunder-call", "duplicate-code", "missing-module-docstring", "missing-class-docstring", "missing-function-docstring"]
 ignore = ["CVS", "examples/"]
 [tool.pylint.messages_control]
 max-line-length = 120
 [tool.pylint.classes]
 exclude-protected = ['_asdict', '_fields', '_replace', '_source', '_make', "_name"]
 valid-classmethod-first-arg = "cls"
 [tool.pylint.design]
@@ -147,25 +160,25 @@
 envlist = py36,py37,py38,py39,py310,py311,py312
 
 [testenv]
 deps =
     black==22.8.0
     isort==5.10.1
     py{36,37}: pylint==2.13.9
-    py{38,39,310,311,312}: pylint==3.0.1
+    py{38,39,310,311,312}: pylint==3.1.0
 
     pytest==7.0.1
     pytest-mock==3.6.1
     typing_extensions==4.1.1
     pytest-trio==0.7.0
     types-dataclasses==0.6.6
 
     py36: mypy==0.971
     py37: mypy==1.4.1
-    py{38,39,310,311,312}: mypy==1.5.1
+    py{38,39,310,311,312}: mypy==1.10.0
 commands = 
     black --check bakery/ tests/
     isort --check bakery tests/
     pylint bakery/ tests/  --disable=no-self-use,R0801,cyclic-import,isinstance-second-argument-not-valid-type,invalid-name
     mypy bakery/ tests/ 
     pytest tests/ -x
 setenv =
```

### Comparing `fresh_bakery-0.3.3/PKG-INFO` & `fresh_bakery-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresh-bakery
-Version: 0.3.3
+Version: 0.3.5
 Summary: Bake your dependencies stupidly simple!
 License: MIT
 Keywords: Dependency Injection,Dependency Injection pattern,Constructor Injection,Inversion of Control,Inversion of Control Container,IoC
 Author: Dmitry Makarov
 Author-email: mit.makaroff@gmail.com
 Requires-Python: >=3.6.2,<3.13
 Classifier: Intended Audience :: Developers
```

