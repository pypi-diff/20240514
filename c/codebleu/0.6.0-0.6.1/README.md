# Comparing `tmp/codebleu-0.6.0.tar.gz` & `tmp/codebleu-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebleu-0.6.0.tar", last modified: Fri Mar  1 15:37:35 2024, max compression
+gzip compressed data, was "codebleu-0.6.1.tar", last modified: Tue May 14 20:48:54 2024, max compression
```

## Comparing `codebleu-0.6.0.tar` & `codebleu-0.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:35.176108 codebleu-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-03-01 15:37:02.000000 codebleu-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:02.000000 codebleu-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)   157835 2024-03-01 15:37:02.000000 codebleu-0.6.0/CodeBLEU.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-01 15:37:02.000000 codebleu-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-01 15:37:02.000000 codebleu-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-03-01 15:37:35.176108 codebleu-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-03-01 15:37:02.000000 codebleu-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 15:37:02.000000 codebleu-0.6.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:35.168108 codebleu-0.6.0/codebleu/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21713 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/codebleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/dataflow_match.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:35.172108 codebleu-0.6.0/codebleu/keywords/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/c.txt
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/c_sharp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/cpp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/go.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/java.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/javascript.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/php.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/ruby.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/keywords/rust.txt
--rwxr-xr-x   0 runner    (1001) docker     (127) 12698456 2024-03-01 15:37:35.000000 codebleu-0.6.0/codebleu/my-languages.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:35.172108 codebleu-0.6.0/codebleu/parser/
--rw-r--r--   0 runner    (1001) docker     (127)    62313 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/parser/DFG.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/syntax_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18970 2024-03-01 15:37:02.000000 codebleu-0.6.0/codebleu/weighted_ngram_match.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:35.172108 codebleu-0.6.0/codebleu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-03-01 15:37:35.000000 codebleu-0.6.0/codebleu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-01 15:37:35.000000 codebleu-0.6.0/codebleu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 15:37:35.000000 codebleu-0.6.0/codebleu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 15:37:35.000000 codebleu-0.6.0/codebleu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-01 15:37:35.000000 codebleu-0.6.0/codebleu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 15:37:35.000000 codebleu-0.6.0/codebleu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-01 15:37:02.000000 codebleu-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 15:37:35.176108 codebleu-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-01 15:37:02.000000 codebleu-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:37:35.172108 codebleu-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-03-01 15:37:02.000000 codebleu-0.6.0/tests/test_codebleu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-14 20:48:19.000000 codebleu-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:19.000000 codebleu-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)   157835 2024-05-14 20:48:19.000000 codebleu-0.6.1/CodeBLEU.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 20:48:19.000000 codebleu-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 20:48:19.000000 codebleu-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-14 20:48:54.146776 codebleu-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-14 20:48:19.000000 codebleu-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 20:48:19.000000 codebleu-0.6.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.142776 codebleu-0.6.1/codebleu/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21713 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/codebleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/dataflow_match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.142776 codebleu-0.6.1/codebleu/keywords/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/c_sharp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/cpp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/go.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/java.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/javascript.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/php.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/ruby.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/keywords/rust.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127) 12698456 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu/my-languages.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/codebleu/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    62313 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/parser/DFG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/syntax_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18970 2024-05-14 20:48:19.000000 codebleu-0.6.1/codebleu/weighted_ngram_match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/codebleu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 20:48:54.000000 codebleu-0.6.1/codebleu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-14 20:48:19.000000 codebleu-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:48:54.146776 codebleu-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-14 20:48:19.000000 codebleu-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:54.146776 codebleu-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-05-14 20:48:19.000000 codebleu-0.6.1/tests/test_codebleu.py
```

### Comparing `codebleu-0.6.0/.gitignore` & `codebleu-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/CodeBLEU.jpg` & `codebleu-0.6.1/CodeBLEU.jpg`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/LICENSE` & `codebleu-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/PKG-INFO` & `codebleu-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: codebleu
-Version: 0.6.0
+Version: 0.6.1
 Summary: Unofficial CodeBLEU implementation that supports Linux, MacOS and Windows available on PyPI.
 Author-email: Konstantin Chernyshev <kdchernyshev@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/k4black/codebleu
 Keywords: codebleu,code,bleu,nlp,natural language processing,programming,evaluate,evaluation,code generation,metrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tree-sitter<1.0.0,>=0.20.0
+Requires-Dist: tree-sitter<0.22.0,>=0.20.0
 Requires-Dist: setuptools>=61.0.0
 Provides-Extra: test
 Requires-Dist: pytest<9.0.0,>=7.0.0; extra == "test"
-Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "test"
+Requires-Dist: pytest-cov<6.0.0,>=4.0.0; extra == "test"
 Requires-Dist: pytest-mock<4.0.0,>=3.0.0; extra == "test"
 Requires-Dist: pytest-timeout<3.0.0,>=2.0.0; extra == "test"
-Requires-Dist: black==24.2.0; extra == "test"
+Requires-Dist: black==24.4.0; extra == "test"
 Requires-Dist: mypy<2.0.0,>=1.0.0; extra == "test"
 Requires-Dist: types-tree-sitter; extra == "test"
 Requires-Dist: flake8<8.0.0,>=6.0.0; extra == "test"
-Requires-Dist: ruff<0.3.0,>=0.0.275; extra == "test"
+Requires-Dist: ruff<0.5.0,>=0.0.275; extra == "test"
 Requires-Dist: isort<6.0.0,>=5.0.0; extra == "test"
 Requires-Dist: nltk<4.0.0,>=3.0.0; extra == "test"
 
 # CodeBLEU
 [![Publish](https://github.com/k4black/codebleu/actions/workflows/publish.yml/badge.svg)](https://github.com/k4black/codebleu/actions/workflows/publish.yml)
 [![Test](https://github.com/k4black/codebleu/actions/workflows/test.yml/badge.svg?event=push)](https://github.com/k4black/codebleu/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/k4black/codebleu/branch/main/graph/badge.svg?token=60BIFPWRCE)](https://codecov.io/gh/k4black/codebleu)
```

### Comparing `codebleu-0.6.0/README.md` & `codebleu-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/__main__.py` & `codebleu-0.6.1/codebleu/__main__.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/bleu.py` & `codebleu-0.6.1/codebleu/bleu.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/codebleu.py` & `codebleu-0.6.1/codebleu/codebleu.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/dataflow_match.py` & `codebleu-0.6.1/codebleu/dataflow_match.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/keywords/c_sharp.txt` & `codebleu-0.6.1/codebleu/keywords/c_sharp.txt`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/keywords/cpp.txt` & `codebleu-0.6.1/codebleu/keywords/cpp.txt`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/my-languages.so` & `codebleu-0.6.1/codebleu/my-languages.so`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/parser/DFG.py` & `codebleu-0.6.1/codebleu/parser/DFG.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/parser/__init__.py` & `codebleu-0.6.1/codebleu/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/parser/utils.py` & `codebleu-0.6.1/codebleu/parser/utils.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/syntax_match.py` & `codebleu-0.6.1/codebleu/syntax_match.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/utils.py` & `codebleu-0.6.1/codebleu/utils.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu/weighted_ngram_match.py` & `codebleu-0.6.1/codebleu/weighted_ngram_match.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/codebleu.egg-info/PKG-INFO` & `codebleu-0.6.1/codebleu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: codebleu
-Version: 0.6.0
+Version: 0.6.1
 Summary: Unofficial CodeBLEU implementation that supports Linux, MacOS and Windows available on PyPI.
 Author-email: Konstantin Chernyshev <kdchernyshev@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/k4black/codebleu
 Keywords: codebleu,code,bleu,nlp,natural language processing,programming,evaluate,evaluation,code generation,metrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tree-sitter<1.0.0,>=0.20.0
+Requires-Dist: tree-sitter<0.22.0,>=0.20.0
 Requires-Dist: setuptools>=61.0.0
 Provides-Extra: test
 Requires-Dist: pytest<9.0.0,>=7.0.0; extra == "test"
-Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "test"
+Requires-Dist: pytest-cov<6.0.0,>=4.0.0; extra == "test"
 Requires-Dist: pytest-mock<4.0.0,>=3.0.0; extra == "test"
 Requires-Dist: pytest-timeout<3.0.0,>=2.0.0; extra == "test"
-Requires-Dist: black==24.2.0; extra == "test"
+Requires-Dist: black==24.4.0; extra == "test"
 Requires-Dist: mypy<2.0.0,>=1.0.0; extra == "test"
 Requires-Dist: types-tree-sitter; extra == "test"
 Requires-Dist: flake8<8.0.0,>=6.0.0; extra == "test"
-Requires-Dist: ruff<0.3.0,>=0.0.275; extra == "test"
+Requires-Dist: ruff<0.5.0,>=0.0.275; extra == "test"
 Requires-Dist: isort<6.0.0,>=5.0.0; extra == "test"
 Requires-Dist: nltk<4.0.0,>=3.0.0; extra == "test"
 
 # CodeBLEU
 [![Publish](https://github.com/k4black/codebleu/actions/workflows/publish.yml/badge.svg)](https://github.com/k4black/codebleu/actions/workflows/publish.yml)
 [![Test](https://github.com/k4black/codebleu/actions/workflows/test.yml/badge.svg?event=push)](https://github.com/k4black/codebleu/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/k4black/codebleu/branch/main/graph/badge.svg?token=60BIFPWRCE)](https://codecov.io/gh/k4black/codebleu)
```

### Comparing `codebleu-0.6.0/codebleu.egg-info/SOURCES.txt` & `codebleu-0.6.1/codebleu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/pyproject.toml` & `codebleu-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel", "tree-sitter>=0.20.0,<1.0.0", "requests>=2.0.0,<3.0.0"]
+requires = ["setuptools>=61.0.0", "wheel", "tree-sitter>=0.20.0,<0.22.0", "requests>=2.0.0,<3.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "codebleu"
 description = "Unofficial CodeBLEU implementation that supports Linux, MacOS and Windows available on PyPI."
 readme = "README.md"
@@ -19,15 +19,15 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Typing :: Typed"
 ]
 
 dependencies = [
-    "tree-sitter >=0.20.0,<1.0.0",
+    "tree-sitter >=0.20.0,<0.22.0",
     "setuptools >=61.0.0",  # distutils removed in 3.12, but distutils.ccompiler used in tree-sitter
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
@@ -45,22 +45,22 @@
 
 [project.urls]
 homepage = "https://github.com/k4black/codebleu"
 
 [project.optional-dependencies]
 test = [
     "pytest >=7.0.0,<9.0.0",
-    "pytest-cov >=4.0.0,<5.0.0",
+    "pytest-cov >=4.0.0,<6.0.0",
     "pytest-mock >=3.0.0,<4.0.0",
     "pytest-timeout >=2.0.0,<3.0.0",
-    "black ==24.2.0",
+    "black ==24.4.0",
     "mypy >=1.0.0,<2.0.0",
     "types-tree-sitter",
     "flake8 >=6.0.0,<8.0.0",
-    "ruff >=0.0.275,<0.3.0",
+    "ruff >=0.0.275,<0.5.0",
     "isort >=5.0.0,<6.0.0",
     "nltk >=3.0.0,<4.0.0",
 ]
 
 [tool.setuptools.dynamic]
 version = {file = "VERSION"}
```

### Comparing `codebleu-0.6.0/setup.py` & `codebleu-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `codebleu-0.6.0/tests/test_codebleu.py` & `codebleu-0.6.1/tests/test_codebleu.py`

 * *Files identical despite different names*

