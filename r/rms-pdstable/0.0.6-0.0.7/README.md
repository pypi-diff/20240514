# Comparing `tmp/rms-pdstable-0.0.6.tar.gz` & `tmp/rms_pdstable-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-pdstable-0.0.6.tar", last modified: Wed Jan 24 23:32:21 2024, max compression
+gzip compressed data, was "rms_pdstable-0.0.7.tar", last modified: Tue May 14 19:17:52 2024, max compression
```

## Comparing `rms-pdstable-0.0.6.tar` & `rms_pdstable-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:21.829527 rms-pdstable-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:21.809527 rms-pdstable-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:21.809527 rms-pdstable-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-01-24 23:32:21.829527 rms-pdstable-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:21.809527 rms-pdstable-0.0.6/pdstable/
--rw-r--r--   0 runner    (1001) docker     (127)    48952 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/pdstable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:32:21.000000 rms-pdstable-0.0.6/pdstable/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:21.829527 rms-pdstable-0.0.6/rms_pdstable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-01-24 23:32:21.000000 rms-pdstable-0.0.6/rms_pdstable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-24 23:32:21.000000 rms-pdstable-0.0.6/rms_pdstable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:32:21.000000 rms-pdstable-0.0.6/rms_pdstable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-24 23:32:21.000000 rms-pdstable-0.0.6/rms_pdstable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-24 23:32:21.000000 rms-pdstable-0.0.6/rms_pdstable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-24 23:32:21.829527 rms-pdstable-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:21.829527 rms-pdstable-0.0.6/test_files/
--rwxr-xr-x   0 runner    (1001) docker     (127)    48138 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/test_files/cassini_iss_index.lbl
--rwxr-xr-x   0 runner    (1001) docker     (127) 13985775 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/test_files/cassini_iss_index.tab
--rwxr-xr-x   0 runner    (1001) docker     (127)    18752 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/test_files/cassini_iss_index_edited.lbl
--rwxr-xr-x   0 runner    (1001) docker     (127)   118100 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/test_files/cassini_iss_index_edited.tab
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:32:21.829527 rms-pdstable-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-01-24 23:31:57.000000 rms-pdstable-0.0.6/tests/test_pdstable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:52.103471 rms_pdstable-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:52.079470 rms_pdstable-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:52.083470 rms_pdstable-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-14 19:17:52.103471 rms_pdstable-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:52.083470 rms_pdstable-0.0.7/pdstable/
+-rw-r--r--   0 runner    (1001) docker     (127)    48953 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/pdstable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:17:51.000000 rms_pdstable-0.0.7/pdstable/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:52.099470 rms_pdstable-0.0.7/rms_pdstable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-14 19:17:52.000000 rms_pdstable-0.0.7/rms_pdstable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-14 19:17:52.000000 rms_pdstable-0.0.7/rms_pdstable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:17:52.000000 rms_pdstable-0.0.7/rms_pdstable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 19:17:52.000000 rms_pdstable-0.0.7/rms_pdstable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 19:17:52.000000 rms_pdstable-0.0.7/rms_pdstable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 19:17:52.103471 rms_pdstable-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:52.099470 rms_pdstable-0.0.7/test_files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48138 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/test_files/cassini_iss_index.lbl
+-rwxr-xr-x   0 runner    (1001) docker     (127) 13985775 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/test_files/cassini_iss_index.tab
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18752 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/test_files/cassini_iss_index_edited.lbl
+-rwxr-xr-x   0 runner    (1001) docker     (127)   118100 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/test_files/cassini_iss_index_edited.tab
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:52.099470 rms_pdstable-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-14 19:17:30.000000 rms_pdstable-0.0.7/tests/test_pdstable.py
```

### Comparing `rms-pdstable-0.0.6/.github/workflows/publish_to_pypi.yml` & `rms_pdstable-0.0.7/.github/workflows/publish_to_pypi.yml`

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

### Comparing `rms-pdstable-0.0.6/.github/workflows/publish_to_test_pypi.yml` & `rms_pdstable-0.0.7/.github/workflows/publish_to_test_pypi.yml`

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

### Comparing `rms-pdstable-0.0.6/.github/workflows/run-tests.yml` & `rms_pdstable-0.0.7/.github/workflows/run-tests.yml`

 * *Files 10% similar despite different names*

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

### Comparing `rms-pdstable-0.0.6/.gitignore` & `rms_pdstable-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-pdstable-0.0.6/LICENSE` & `rms_pdstable-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-pdstable-0.0.6/pdstable/__init__.py` & `rms_pdstable-0.0.7/pdstable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 import numpy as np
 import numbers
 
 import pdsparser
 import julian
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 # STR_DTYPE is 'S' for Python 2; 'U' for Python 3
 STR_DTYPE = np.array(['x']).dtype.kind
 PYTHON2 = (sys.version_info[0] == 2)
```

### Comparing `rms-pdstable-0.0.6/pyproject.toml` & `rms_pdstable-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-pdstable-0.0.6/rms_pdstable.egg-info/SOURCES.txt` & `rms_pdstable-0.0.7/rms_pdstable.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 .coveragerc
 .gitignore
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/publish_to_pypi.yml
 .github/workflows/publish_to_test_pypi.yml
```

### Comparing `rms-pdstable-0.0.6/test_files/cassini_iss_index.lbl` & `rms_pdstable-0.0.7/test_files/cassini_iss_index.lbl`

 * *Files identical despite different names*

### Comparing `rms-pdstable-0.0.6/test_files/cassini_iss_index.tab` & `rms_pdstable-0.0.7/test_files/cassini_iss_index.tab`

 * *Files identical despite different names*

### Comparing `rms-pdstable-0.0.6/test_files/cassini_iss_index_edited.lbl` & `rms_pdstable-0.0.7/test_files/cassini_iss_index_edited.lbl`

 * *Files identical despite different names*

### Comparing `rms-pdstable-0.0.6/test_files/cassini_iss_index_edited.tab` & `rms_pdstable-0.0.7/test_files/cassini_iss_index_edited.tab`

 * *Files identical despite different names*

### Comparing `rms-pdstable-0.0.6/tests/test_pdstable.py` & `rms_pdstable-0.0.7/tests/test_pdstable.py`

 * *Files identical despite different names*

