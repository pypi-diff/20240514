# Comparing `tmp/rms-solar-1.0.1.tar.gz` & `tmp/rms_solar-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-solar-1.0.1.tar", last modified: Wed Jan 24 23:34:58 2024, max compression
+gzip compressed data, was "rms_solar-1.0.2.tar", last modified: Tue May 14 19:18:42 2024, max compression
```

## Comparing `rms-solar-1.0.1.tar` & `rms_solar-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:58.205535 rms-solar-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:34:35.000000 rms-solar-1.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:58.197535 rms-solar-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:58.201535 rms-solar-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:34:35.000000 rms-solar-1.0.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:34:35.000000 rms-solar-1.0.1/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-01-24 23:34:35.000000 rms-solar-1.0.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:34:35.000000 rms-solar-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:34:35.000000 rms-solar-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-01-24 23:34:58.205535 rms-solar-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-24 23:34:35.000000 rms-solar-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-01-24 23:34:35.000000 rms-solar-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-24 23:34:35.000000 rms-solar-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:58.205535 rms-solar-1.0.1/rms_solar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-01-24 23:34:58.000000 rms-solar-1.0.1/rms_solar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-24 23:34:58.000000 rms-solar-1.0.1/rms_solar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:34:58.000000 rms-solar-1.0.1/rms_solar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-24 23:34:58.000000 rms-solar-1.0.1/rms_solar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-24 23:34:58.000000 rms-solar-1.0.1/rms_solar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-24 23:34:58.205535 rms-solar-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:58.201535 rms-solar-1.0.1/solar/
--rw-r--r--   0 runner    (1001) docker     (127)    13394 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:34:58.000000 rms-solar-1.0.1/solar/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    36381 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/colina.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:58.205535 rms-solar-1.0.1/solar/data_files/
--rw-r--r--   0 runner    (1001) docker     (127)  1155314 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/data_files/kurucz-fsunallp.2000resam125.txt
--rw-r--r--   0 runner    (1001) docker     (127)   118080 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/data_files/rieke-solar_spec.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37440 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/data_files/stis-sun_reference_stis_002.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/kurucz.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/rieke.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/stis.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/stis_rieke.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-01-24 23:34:35.000000 rms-solar-1.0.1/solar/test_solar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:41.998263 rms_solar-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:41.998263 rms_solar-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:18:23.000000 rms_solar-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-14 19:18:23.000000 rms_solar-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:18:23.000000 rms_solar-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-14 19:18:42.002262 rms_solar-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-14 19:18:23.000000 rms_solar-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-14 19:18:23.000000 rms_solar-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 19:18:23.000000 rms_solar-1.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/rms_solar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 19:18:42.006262 rms_solar-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/solar/
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:18:41.000000 rms_solar-1.0.2/solar/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36381 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/colina.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/solar/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)  1155314 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/data_files/kurucz-fsunallp.2000resam125.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   118080 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/data_files/rieke-solar_spec.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37440 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/data_files/stis-sun_reference_stis_002.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/kurucz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/rieke.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/stis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/stis_rieke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/test_solar.py
```

### Comparing `rms-solar-1.0.1/.github/workflows/publish_to_pypi.yml` & `rms_solar-1.0.2/.github/workflows/publish_to_pypi.yml`

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

### Comparing `rms-solar-1.0.1/.github/workflows/publish_to_test_pypi.yml` & `rms_solar-1.0.2/.github/workflows/publish_to_test_pypi.yml`

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

### Comparing `rms-solar-1.0.1/.github/workflows/run-tests.yml` & `rms_solar-1.0.2/.github/workflows/run-tests.yml`

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
@@ -22,26 +22,29 @@
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

### Comparing `rms-solar-1.0.1/.gitignore` & `rms_solar-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/LICENSE` & `rms_solar-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/pyproject.toml` & `rms_solar-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/__init__.py` & `rms_solar-1.0.2/solar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import functools
 import importlib
 import numpy as np
 import tabulation as tab
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 # Class constants to be used externally as needed
 AU = 149597870.7    # km
 C = 299792.458      # km/sec
```

### Comparing `rms-solar-1.0.1/solar/colina.py` & `rms_solar-1.0.2/solar/colina.py`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/data_files/kurucz-fsunallp.2000resam125.txt` & `rms_solar-1.0.2/solar/data_files/kurucz-fsunallp.2000resam125.txt`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/data_files/rieke-solar_spec.fits` & `rms_solar-1.0.2/solar/data_files/rieke-solar_spec.fits`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/data_files/stis-sun_reference_stis_002.fits` & `rms_solar-1.0.2/solar/data_files/stis-sun_reference_stis_002.fits`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/kurucz.py` & `rms_solar-1.0.2/solar/kurucz.py`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/rieke.py` & `rms_solar-1.0.2/solar/rieke.py`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/stis.py` & `rms_solar-1.0.2/solar/stis.py`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/stis_rieke.py` & `rms_solar-1.0.2/solar/stis_rieke.py`

 * *Files identical despite different names*

### Comparing `rms-solar-1.0.1/solar/test_solar.py` & `rms_solar-1.0.2/solar/test_solar.py`

 * *Files identical despite different names*

