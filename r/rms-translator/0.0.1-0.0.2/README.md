# Comparing `tmp/rms-translator-0.0.1.tar.gz` & `tmp/rms_translator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-translator-0.0.1.tar", last modified: Wed Jan  3 20:17:01 2024, max compression
+gzip compressed data, was "rms_translator-0.0.2.tar", last modified: Tue May 14 19:19:03 2024, max compression
```

## Comparing `rms-translator-0.0.1.tar` & `rms_translator-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:17:01.479217 rms-translator-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-03 20:16:48.000000 rms-translator-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:17:01.479217 rms-translator-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:17:01.479217 rms-translator-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-03 20:16:48.000000 rms-translator-0.0.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-03 20:16:48.000000 rms-translator-0.0.1/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-03 20:16:48.000000 rms-translator-0.0.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-03 20:16:48.000000 rms-translator-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-03 20:16:48.000000 rms-translator-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-01-03 20:17:01.479217 rms-translator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-03 20:16:48.000000 rms-translator-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-01-03 20:16:48.000000 rms-translator-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-03 20:16:48.000000 rms-translator-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:17:01.479217 rms-translator-0.0.1/rms_translator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-01-03 20:17:01.000000 rms-translator-0.0.1/rms_translator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-03 20:17:01.000000 rms-translator-0.0.1/rms_translator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 20:17:01.000000 rms-translator-0.0.1/rms_translator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-03 20:17:01.000000 rms-translator-0.0.1/rms_translator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-03 20:17:01.483217 rms-translator-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:17:01.479217 rms-translator-0.0.1/translator/
--rwxr-xr-x   0 runner    (1001) docker     (127)    20347 2024-01-03 20:16:48.000000 rms-translator-0.0.1/translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-03 20:17:01.000000 rms-translator-0.0.1/translator/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:03.655893 rms_translator-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:18:57.000000 rms_translator-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:03.651893 rms_translator-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:03.651893 rms_translator-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 19:18:57.000000 rms_translator-0.0.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-14 19:18:57.000000 rms_translator-0.0.2/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-14 19:18:57.000000 rms_translator-0.0.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:18:57.000000 rms_translator-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:18:57.000000 rms_translator-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-14 19:18:57.000000 rms_translator-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:18:57.000000 rms_translator-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-14 19:19:03.655893 rms_translator-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-14 19:18:57.000000 rms_translator-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-14 19:18:57.000000 rms_translator-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 19:18:57.000000 rms_translator-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:03.655893 rms_translator-0.0.2/rms_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-14 19:19:03.000000 rms_translator-0.0.2/rms_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 19:19:03.000000 rms_translator-0.0.2/rms_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:19:03.000000 rms_translator-0.0.2/rms_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:19:03.000000 rms_translator-0.0.2/rms_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 19:19:03.655893 rms_translator-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:03.655893 rms_translator-0.0.2/translator/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20348 2024-05-14 19:18:57.000000 rms_translator-0.0.2/translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:19:03.000000 rms_translator-0.0.2/translator/_version.py
```

### Comparing `rms-translator-0.0.1/.github/workflows/publish_to_pypi.yml` & `rms_translator-0.0.2/.github/workflows/publish_to_pypi.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Publish to PyPI
-run-name: Publish to PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   release:
     types: [published]
 
 jobs:
   upload_pypi:
@@ -11,15 +11,15 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-translator-0.0.1/.github/workflows/publish_to_test_pypi.yml` & `rms_translator-0.0.2/.github/workflows/publish_to_test_pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Publish to Test PyPI
-run-name: Publish to Test PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to Test PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   workflow_dispatch:
 
 jobs:
   upload_pypi:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-translator-0.0.1/.github/workflows/run-tests.yml` & `rms_translator-0.0.2/.github/workflows/run-tests.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Run Tests
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   # pull_request:
   #   branches: [ main ]
   # push:
   #   branches: [ main ]
@@ -22,25 +22,29 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
 
       - name: Test with coverage
         run: |
           coverage run -m pytest
 
+      - name: Print coverage report
+        run: |
+          coverage report -m
+
       - name: Upload coverage report to codecov
-        uses: codecov/codecov-action@v3
-        env:
-          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
+          token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-translator-0.0.1/.gitignore` & `rms_translator-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-translator-0.0.1/LICENSE` & `rms_translator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-translator-0.0.1/pyproject.toml` & `rms_translator-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-translator-0.0.1/translator/__init__.py` & `rms_translator-0.0.2/translator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # other information. It is implemented in several ways including Python
 # dictionaries and regular expression/substitution pairs.
 ################################################################################
 
 import re
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 class Translator(object):
     """Abstract class to define translators from a set of strings (such as file
     paths) to associated information.
```

