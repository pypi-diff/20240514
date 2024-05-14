# Comparing `tmp/pysortlib-0.5.0.tar.gz` & `tmp/pysortlib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysortlib-0.5.0.tar", max compression
+gzip compressed data, was "pysortlib-0.5.1.tar", max compression
```

## Comparing `pysortlib-0.5.0.tar` & `pysortlib-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-01-23 11:39:22.589926 pysortlib-0.5.0/LICENSE
--rw-r--r--   0        0        0     1416 2024-01-23 11:39:22.589926 pysortlib-0.5.0/README.md
--rw-r--r--   0        0        0     1851 2024-01-23 11:39:22.589926 pysortlib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      261 2024-01-23 11:39:22.589926 pysortlib-0.5.0/pysortlib/__init__.py
--rw-r--r--   0        0        0     7817 2024-01-23 11:39:22.589926 pysortlib-0.5.0/pysortlib/sorting.py
--rw-r--r--   0        0        0     3117 2024-01-23 11:39:22.589926 pysortlib-0.5.0/pysortlib/sorting_extra.py
--rw-r--r--   0        0        0      470 2024-01-23 11:39:22.589926 pysortlib-0.5.0/pysortlib/utils.py
--rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 pysortlib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-14 09:34:21.836525 pysortlib-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1397 2024-05-14 09:34:21.836525 pysortlib-0.5.1/README.md
+-rw-r--r--   0        0        0     1848 2024-05-14 09:34:21.836525 pysortlib-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      261 2024-05-14 09:34:21.836525 pysortlib-0.5.1/pysortlib/__init__.py
+-rw-r--r--   0        0        0     7817 2024-05-14 09:34:21.836525 pysortlib-0.5.1/pysortlib/sorting.py
+-rw-r--r--   0        0        0     3117 2024-05-14 09:34:21.836525 pysortlib-0.5.1/pysortlib/sorting_extra.py
+-rw-r--r--   0        0        0      470 2024-05-14 09:34:21.836525 pysortlib-0.5.1/pysortlib/utils.py
+-rw-r--r--   0        0        0     2182 1970-01-01 00:00:00.000000 pysortlib-0.5.1/PKG-INFO
```

### Comparing `pysortlib-0.5.0/LICENSE` & `pysortlib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysortlib-0.5.0/README.md` & `pysortlib-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Python Sorting Library
 
 [![PyPI](https://img.shields.io/pypi/v/pysortlib)](https://pypi.org/project/pysortlib)
 [![Downloads](https://static.pepy.tech/badge/pysortlib)](https://pepy.tech/project/pysortlib)
-[![Coverage](https://coveralls.io/repos/github/slimreaper35/pysortlib/badge.svg?branch=main)](https://coveralls.io/github/slimreaper35/pysortlib?branch=main)
+[![Coverage](https://codecov.io/gh/slimreaper35/pysortlib/graph/badge.svg?token=S24DIT654W)](https://codecov.io/gh/slimreaper35/pysortlib)
 
 Library of sorting algorithms with precise implementation and documentation.
 
 ## Algorithms
 
 - Bubble sort
 - Counting sort
```

### Comparing `pysortlib-0.5.0/pyproject.toml` & `pysortlib-0.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,36 @@
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = [
+  "poetry-core",
+]
+
 [tool.poetry]
 name = "pysortlib"
-version = "0.5.0"
+version = "0.5.1"
 description = "Python Sorting Library"
 license = "MIT"
-authors = ["Michal Šoltis <msoltis@redhat.com>"]
+authors = [
+  "Michal Šoltis <msoltis@redhat.com>",
+]
 readme = "README.md"
 repository = "https://github.com/slimreaper35/pysortlib"
-keywords = ["sorting", "algorithms", "data structures"]
+keywords = [
+  "sorting",
+  "algorithms",
+  "data structures",
+]
 classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Education",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Education",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.dev-dependencies]
 black = "*"
@@ -29,18 +41,33 @@
 pytest = "*"
 pytest-cov = "*"
 pytest-rich = "*"
 ruff = "*"
 tox = "*"
 tox-ini-fmt = "*"
 
-[build-system]
-build-backend = "poetry.core.masonry.api"
-requires = [
-    "poetry-core",
+[tool.ruff.lint]
+select = [
+  "ALL",
+]
+ignore = [
+  "D100", # Missing docstring in public module
+  "D203", # 1 blank line required before class docstring
+  "D212", # Multi-line docstring summary should start at the first line
+]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = [
+  "F401", # {name} imported but unused
+]
+"tests/*" = [
+  "D103",  # Missing docstring in public function
+  "D104",  # Missing docstring in public package
+  "PT011", # pytest.raises({exception}) is too broad, set the match parameter or use a more specific exception
+  "S101",  # Use of assert detected
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
@@ -48,26 +75,7 @@
 disallow_untyped_decorators = true
 strict = true
 strict_equality = true
 
 [[tool.mypy.overrides]]
 module = "tests/*"
 disallow_untyped_decorators = false
-
-[tool.ruff]
-select = ["ALL"]
-ignore = [
-    "D100", # Missing docstring in public module
-    "D203", # 1 blank line required before class docstring
-    "D212", # Multi-line docstring summary should start at the first line
-]
-
-[tool.ruff.per-file-ignores]
-"__init__.py" = [
-    "F401", # {name} imported but unused
-]
-"tests/*" = [
-    "D103",  # Missing docstring in public function
-    "D104",  # Missing docstring in public package
-    "PT011", # pytest.raises({exception}) is too broad, set the match parameter or use a more specific exception
-    "S101",  # Use of assert detected
-]
```

### Comparing `pysortlib-0.5.0/pysortlib/sorting.py` & `pysortlib-0.5.1/pysortlib/sorting.py`

 * *Files identical despite different names*

### Comparing `pysortlib-0.5.0/pysortlib/sorting_extra.py` & `pysortlib-0.5.1/pysortlib/sorting_extra.py`

 * *Files identical despite different names*

### Comparing `pysortlib-0.5.0/PKG-INFO` & `pysortlib-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysortlib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Sorting Library
 Home-page: https://github.com/slimreaper35/pysortlib
 License: MIT
 Keywords: sorting,algorithms,data structures
 Author: Michal Šoltis
 Author-email: msoltis@redhat.com
 Requires-Python: >=3.11,<4.0
@@ -19,15 +19,15 @@
 Project-URL: Repository, https://github.com/slimreaper35/pysortlib
 Description-Content-Type: text/markdown
 
 # Python Sorting Library
 
 [![PyPI](https://img.shields.io/pypi/v/pysortlib)](https://pypi.org/project/pysortlib)
 [![Downloads](https://static.pepy.tech/badge/pysortlib)](https://pepy.tech/project/pysortlib)
-[![Coverage](https://coveralls.io/repos/github/slimreaper35/pysortlib/badge.svg?branch=main)](https://coveralls.io/github/slimreaper35/pysortlib?branch=main)
+[![Coverage](https://codecov.io/gh/slimreaper35/pysortlib/graph/badge.svg?token=S24DIT654W)](https://codecov.io/gh/slimreaper35/pysortlib)
 
 Library of sorting algorithms with precise implementation and documentation.
 
 ## Algorithms
 
 - Bubble sort
 - Counting sort
```

