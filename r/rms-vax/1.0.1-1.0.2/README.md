# Comparing `tmp/rms-vax-1.0.1.tar.gz` & `tmp/rms_vax-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-vax-1.0.1.tar", last modified: Wed Jan 24 23:40:56 2024, max compression
+gzip compressed data, was "rms_vax-1.0.2.tar", last modified: Tue May 14 19:06:23 2024, max compression
```

## Comparing `rms-vax-1.0.1.tar` & `rms_vax-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:40:56.097606 rms-vax-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:40:40.000000 rms-vax-1.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-24 23:40:40.000000 rms-vax-1.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:40:56.093606 rms-vax-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:40:56.097606 rms-vax-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:40:40.000000 rms-vax-1.0.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:40:40.000000 rms-vax-1.0.1/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-01-24 23:40:40.000000 rms-vax-1.0.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:40:40.000000 rms-vax-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:40:40.000000 rms-vax-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-24 23:40:56.097606 rms-vax-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-24 23:40:40.000000 rms-vax-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-24 23:40:40.000000 rms-vax-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-24 23:40:40.000000 rms-vax-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:40:56.097606 rms-vax-1.0.1/rms_vax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-24 23:40:56.000000 rms-vax-1.0.1/rms_vax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-24 23:40:56.000000 rms-vax-1.0.1/rms_vax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:40:56.000000 rms-vax-1.0.1/rms_vax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-24 23:40:56.000000 rms-vax-1.0.1/rms_vax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-24 23:40:56.000000 rms-vax-1.0.1/rms_vax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-24 23:40:56.097606 rms-vax-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:40:56.097606 rms-vax-1.0.1/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-01-24 23:40:40.000000 rms-vax-1.0.1/test_files/C3490702_GEOMA.DAT
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-01-24 23:40:40.000000 rms-vax-1.0.1/test_files/C3490702_GEOMA.LBL
--rw-r--r--   0 runner    (1001) docker     (127)    20424 2024-01-24 23:40:40.000000 rms-vax-1.0.1/test_files/C3490702_GEOMA.TAB
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:40:56.097606 rms-vax-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-01-24 23:40:40.000000 rms-vax-1.0.1/tests/test_vax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:40:56.097606 rms-vax-1.0.1/vax/
--rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-01-24 23:40:40.000000 rms-vax-1.0.1/vax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:40:56.000000 rms-vax-1.0.1/vax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.083470 rms_vax-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.083470 rms_vax-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:06:13.000000 rms_vax-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-14 19:06:13.000000 rms_vax-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:06:13.000000 rms_vax-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-14 19:06:23.087470 rms_vax-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-14 19:06:13.000000 rms_vax-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-14 19:06:13.000000 rms_vax-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 19:06:13.000000 rms_vax-1.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/rms_vax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 19:06:23.087470 rms_vax-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.083470 rms_vax-1.0.2/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-05-14 19:06:13.000000 rms_vax-1.0.2/test_files/C3490702_GEOMA.DAT
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-14 19:06:13.000000 rms_vax-1.0.2/test_files/C3490702_GEOMA.LBL
+-rw-r--r--   0 runner    (1001) docker     (127)    20424 2024-05-14 19:06:13.000000 rms_vax-1.0.2/test_files/C3490702_GEOMA.TAB
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-05-14 19:06:13.000000 rms_vax-1.0.2/tests/test_vax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/vax/
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-14 19:06:13.000000 rms_vax-1.0.2/vax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:06:22.000000 rms_vax-1.0.2/vax/_version.py
```

### Comparing `rms-vax-1.0.1/.github/workflows/publish_to_pypi.yml` & `rms_vax-1.0.2/.github/workflows/publish_to_pypi.yml`

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

### Comparing `rms-vax-1.0.1/.github/workflows/publish_to_test_pypi.yml` & `rms_vax-1.0.2/.github/workflows/publish_to_test_pypi.yml`

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

### Comparing `rms-vax-1.0.1/.github/workflows/run-tests.yml` & `rms_vax-1.0.2/.github/workflows/run-tests.yml`

 * *Files 14% similar despite different names*

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
@@ -13,35 +13,38 @@
 jobs:
   test:
     name: Test vax
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [ '3.7', '3.8', '3.9', '3.10', '3.11', '3.12' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
       fail-fast: false
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
-        env:
-          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
+          token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-vax-1.0.1/.gitignore` & `rms_vax-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-vax-1.0.1/LICENSE` & `rms_vax-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-vax-1.0.1/PKG-INFO` & `rms_vax-1.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1
-Name: rms-vax
-Version: 1.0.1
-Summary: Routines for converting to and from vax single-precision floating-point values
-Maintainer-email: "Robert S. French" <rfrench@seti.org>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/SETI/rms-vax
-Project-URL: Repository, https://github.com/SETI/rms-vax
-Project-URL: Source, https://github.com/SETI/rms-vax
-Project-URL: Issues, https://github.com/SETI/rms-vax/issues
-Keywords: vax
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-
-| PyPI Release | Test Status | Code Coverage |
-| ------------ | ----------- | ------------- |
-| [![PyPI version](https://badge.fury.io/py/rms-vax.svg)](https://badge.fury.io/py/rms-vax) | [![Build status](https://img.shields.io/github/actions/workflow/status/SETI/rms-vax/run-tests.yml?branch=main)](https://github.com/SETI/rms-vax/actions) | [![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-vax/main?logo=codecov)](https://codecov.io/gh/SETI/rms-vax) |
-
-# rms-vax
-
-PDS Ring-Moon Systems Node, SETI Institute
-
-Supported versions: Python >= 3.7
-
-Conversions between Vax floats and IEEE floats.
-
-Conversions to/from Vax single precision are supported. However, only conversions
-from Vax doubles to IEEE doubles is supported, not the reverse.
-
+[build-system]
+requires = ["setuptools", "setuptools_scm[toml]"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "rms-vax"
+dynamic = ["version"]
+description = "Routines for converting to and from vax single-precision floating-point values"
+readme = "README.md"
+requires-python = ">=3.7"
+dependencies = [
+    "numpy"
+]
+license = {text = "Apache-2.0"}
+maintainers = [
+  {name = "Robert S. French", email = "rfrench@seti.org"}
+]
+keywords = ["vax"]
+classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Natural Language :: English",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Astronomy",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Utilities",
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Operating System :: MacOS :: MacOS X",
+  "Operating System :: POSIX :: Linux",
+  "Operating System :: Microsoft :: Windows"
+]
+
+[project.urls]
+Homepage = "https://github.com/SETI/rms-vax"
+Repository = "https://github.com/SETI/rms-vax"
+Source = "https://github.com/SETI/rms-vax"
+Issues = "https://github.com/SETI/rms-vax/issues"
+
+[tool.setuptools]
+packages = ["vax"]
+
+[tool.setuptools_scm]
+local_scheme = "no-local-version"
+write_to = "vax/_version.py"
```

### Comparing `rms-vax-1.0.1/test_files/C3490702_GEOMA.DAT` & `rms_vax-1.0.2/test_files/C3490702_GEOMA.DAT`

 * *Files identical despite different names*

### Comparing `rms-vax-1.0.1/test_files/C3490702_GEOMA.LBL` & `rms_vax-1.0.2/test_files/C3490702_GEOMA.LBL`

 * *Files identical despite different names*

### Comparing `rms-vax-1.0.1/test_files/C3490702_GEOMA.TAB` & `rms_vax-1.0.2/test_files/C3490702_GEOMA.TAB`

 * *Files identical despite different names*

### Comparing `rms-vax-1.0.1/tests/test_vax.py` & `rms_vax-1.0.2/tests/test_vax.py`

 * *Files identical despite different names*

### Comparing `rms-vax-1.0.1/vax/__init__.py` & `rms_vax-1.0.2/vax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from Vax doubles to IEEE doubles are supported, not the reverse.
 """
 
 import numpy as np
 import sys
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 _PYTHON2 = sys.version_info.major <= 2
 
 
 def from_vax32(data):
```

