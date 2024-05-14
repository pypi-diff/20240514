# Comparing `tmp/rms-pdstemplate-0.0.4.tar.gz` & `tmp/rms_pdstemplate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-pdstemplate-0.0.4.tar", last modified: Wed Jan 24 23:32:40 2024, max compression
+gzip compressed data, was "rms_pdstemplate-0.0.5.tar", last modified: Tue May 14 19:17:54 2024, max compression
```

## Comparing `rms-pdstemplate-0.0.4.tar` & `rms_pdstemplate-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:40.154103 rms-pdstemplate-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:40.150103 rms-pdstemplate-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:40.150103 rms-pdstemplate-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-01-24 23:32:40.154103 rms-pdstemplate-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:40.150103 rms-pdstemplate-0.0.4/pdstemplate/
--rw-r--r--   0 runner    (1001) docker     (127)    56080 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/pdstemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:32:40.000000 rms-pdstemplate-0.0.4/pdstemplate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:40.154103 rms-pdstemplate-0.0.4/rms_pdstemplate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-01-24 23:32:40.000000 rms-pdstemplate-0.0.4/rms_pdstemplate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-24 23:32:40.000000 rms-pdstemplate-0.0.4/rms_pdstemplate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:32:40.000000 rms-pdstemplate-0.0.4/rms_pdstemplate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-24 23:32:40.000000 rms-pdstemplate-0.0.4/rms_pdstemplate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-24 23:32:40.000000 rms-pdstemplate-0.0.4/rms_pdstemplate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-24 23:32:40.154103 rms-pdstemplate-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:40.154103 rms-pdstemplate-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21793 2024-01-24 23:32:26.000000 rms-pdstemplate-0.0.4/tests/test_pdstemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:54.020988 rms_pdstemplate-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:54.016988 rms_pdstemplate-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:54.020988 rms_pdstemplate-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-14 19:17:54.020988 rms_pdstemplate-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:54.020988 rms_pdstemplate-0.0.5/pdstemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)    56081 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/pdstemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:17:53.000000 rms_pdstemplate-0.0.5/pdstemplate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:54.020988 rms_pdstemplate-0.0.5/rms_pdstemplate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-14 19:17:53.000000 rms_pdstemplate-0.0.5/rms_pdstemplate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 19:17:54.000000 rms_pdstemplate-0.0.5/rms_pdstemplate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:17:53.000000 rms_pdstemplate-0.0.5/rms_pdstemplate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 19:17:53.000000 rms_pdstemplate-0.0.5/rms_pdstemplate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 19:17:53.000000 rms_pdstemplate-0.0.5/rms_pdstemplate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 19:17:54.020988 rms_pdstemplate-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:54.020988 rms_pdstemplate-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21793 2024-05-14 19:17:44.000000 rms_pdstemplate-0.0.5/tests/test_pdstemplate.py
```

### Comparing `rms-pdstemplate-0.0.4/.github/workflows/publish_to_pypi.yml` & `rms_pdstemplate-0.0.5/.github/workflows/publish_to_pypi.yml`

 * *Files 16% similar despite different names*

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

### Comparing `rms-pdstemplate-0.0.4/.github/workflows/publish_to_test_pypi.yml` & `rms_pdstemplate-0.0.5/.github/workflows/publish_to_test_pypi.yml`

 * *Files 20% similar despite different names*

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

### Comparing `rms-pdstemplate-0.0.4/.github/workflows/run-tests.yml` & `rms_pdstemplate-0.0.5/.github/workflows/run-tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Run Tests
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   pull_request:
     branches: [ main ]
   push:
     branches: [ main ]
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
+
+      - name: Print coverage report
+        run: |
           coverage report -m
 
       - name: Upload coverage report to codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-pdstemplate-0.0.4/.gitignore` & `rms_pdstemplate-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-pdstemplate-0.0.4/LICENSE` & `rms_pdstemplate-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-pdstemplate-0.0.4/README.md` & `rms_pdstemplate-0.0.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,29 @@
-| PyPI Release | Test Status | Code Coverage |
-| ------------ | ----------- | ------------- |
-| [![PyPI version](https://badge.fury.io/py/rms-pdstemplate.svg)](https://badge.fury.io/py/rms-pdstemplate) | [![Build status](https://img.shields.io/github/actions/workflow/status/SETI/rms-pdstemplate/run-tests.yml?branch=main)](https://github.com/SETI/rms-pdstemplate/actions) | [![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-pdstemplate/main?logo=codecov)](https://codecov.io/gh/SETI/rms-pdstemplate) |
+[![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/releases)
+[![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/releases)
+[![Test Status](https://img.shields.io/github/actions/workflow/status/SETI/rms-pdstemplate/run-tests.yml?branch=main)](https://github.com/SETI/rms-pdstemplate/actions)
+[![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-pdstemplate/main?logo=codecov)](https://codecov.io/gh/SETI/rms-pdstemplate)
+<br />
+[![PyPI - Version](https://img.shields.io/pypi/v/rms-pdstemplate)](https://pypi.org/project/rms-pdstemplate)
+[![PyPI - Format](https://img.shields.io/pypi/format/rms-pdstemplate)](https://pypi.org/project/rms-pdstemplate)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/rms-pdstemplate)](https://pypi.org/project/rms-pdstemplate)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rms-pdstemplate)](https://pypi.org/project/rms-pdstemplate)
+<br />
+[![GitHub commits since latest release](https://img.shields.io/github/commits-since/SETI/rms-pdstemplate/latest)](https://github.com/SETI/rms-pdstemplate/commits/main/)
+[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/commits/main/)
+[![GitHub last commit](https://img.shields.io/github/last-commit/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/commits/main/)
+<br />
+[![Number of GitHub open issues](https://img.shields.io/github/issues-raw/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/issues)
+[![Number of GitHub closed issues](https://img.shields.io/github/issues-closed-raw/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/issues)
+[![Number of GitHub open pull requests](https://img.shields.io/github/issues-pr-raw/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/pulls)
+[![Number of GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed-raw/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/pulls)
+<br />
+![GitHub License](https://img.shields.io/github/license/SETI/rms-pdstemplate)
+[![Number of GitHub stars](https://img.shields.io/github/stars/SETI/rms-pdstemplate)](https://github.com/SETI/rms-pdstemplate/stargazers)
+![GitHub forks](https://img.shields.io/github/forks/SETI/rms-pdstemplate)
 
 # rms-pdstemplate
 
 PDS Ring-Moon Systems Node, SETI Institute
 
 Supported versions: Python >= 3.8
```

### Comparing `rms-pdstemplate-0.0.4/pdstemplate/__init__.py` & `rms_pdstemplate-0.0.5/pdstemplate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from collections import deque, namedtuple
 from xml.sax.saxutils import escape
 
 import julian
 import pdslogger
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 ##########################################################################################
 # IMPORTANT: Update the PDSTEMPLATE_VERSION_ID below whenever the behavior of this module
 # is changed!
```

### Comparing `rms-pdstemplate-0.0.4/pyproject.toml` & `rms_pdstemplate-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-pdstemplate-0.0.4/tests/test_pdstemplate.py` & `rms_pdstemplate-0.0.5/tests/test_pdstemplate.py`

 * *Files identical despite different names*

