# Comparing `tmp/rms-tabulation-0.0.3.tar.gz` & `tmp/rms_tabulation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-tabulation-0.0.3.tar", last modified: Wed Jan 24 22:15:17 2024, max compression
+gzip compressed data, was "rms_tabulation-0.0.4.tar", last modified: Tue May 14 19:02:57 2024, max compression
```

## Comparing `rms-tabulation-0.0.3.tar` & `rms_tabulation-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 22:15:17.298370 rms-tabulation-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 22:15:17.294370 rms-tabulation-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 22:15:17.294370 rms-tabulation-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-24 22:15:17.298370 rms-tabulation-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 22:15:17.298370 rms-tabulation-0.0.3/rms_tabulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-24 22:15:17.000000 rms-tabulation-0.0.3/rms_tabulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-24 22:15:17.000000 rms-tabulation-0.0.3/rms_tabulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 22:15:17.000000 rms-tabulation-0.0.3/rms_tabulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-24 22:15:17.000000 rms-tabulation-0.0.3/rms_tabulation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-24 22:15:17.000000 rms-tabulation-0.0.3/rms_tabulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-24 22:15:17.298370 rms-tabulation-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 22:15:17.294370 rms-tabulation-0.0.3/tabulation/
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/tabulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 22:15:17.000000 rms-tabulation-0.0.3/tabulation/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 22:15:17.298370 rms-tabulation-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-01-24 22:14:59.000000 rms-tabulation-0.0.3/tests/test_tabulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.662304 rms_tabulation-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.662304 rms_tabulation-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/rms_tabulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/tabulation/
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/tabulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/tabulation/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/tests/test_tabulation.py
```

### Comparing `rms-tabulation-0.0.3/.github/workflows/publish_to_pypi.yml` & `rms_tabulation-0.0.4/.github/workflows/publish_to_pypi.yml`

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

### Comparing `rms-tabulation-0.0.3/.github/workflows/publish_to_test_pypi.yml` & `rms_tabulation-0.0.4/.github/workflows/publish_to_test_pypi.yml`

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

### Comparing `rms-tabulation-0.0.3/.github/workflows/run-tests.yml` & `rms_tabulation-0.0.4/.github/workflows/run-tests.yml`

 * *Files 12% similar despite different names*

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
@@ -13,34 +13,38 @@
 jobs:
   test:
     name: Test tabulation
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

### Comparing `rms-tabulation-0.0.3/.gitignore` & `rms_tabulation-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-tabulation-0.0.3/LICENSE` & `rms_tabulation-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-tabulation-0.0.3/pyproject.toml` & `rms_tabulation-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-tabulation-0.0.3/tabulation/__init__.py` & `rms_tabulation-0.0.4/tabulation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from __future__ import division
 
 import numpy as np
 from scipy.interpolate import interp1d
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 class Tabulation(object):
     """A class that represents a function by a sequence of linear interpolations
     between points defined by arrays of x and y coordinates. The function is
@@ -158,43 +158,43 @@
         if type(other) == type(self):
             new_x = Tabulation._xoverlap(self.x, other.x)
             return Tabulation(new_x, self(new_x) * other(new_x))._trim()
 
         # Otherwise just scale the y-values
         elif np.shape(other) == ():
             return Tabulation(self.x, self.y * other)
-        
+
         raise ValueError("Cannot multiply Tabulation by given value")
 
     def __truediv__(self, other):
 
         # Division of two Tabulations
         # Note: the new domain is the intersection of the given domains
         if type(other) == type(self):
             new_x = Tabulation._xoverlap(self.x, other.x)
             return Tabulation(new_x, self(new_x) / other(new_x))._trim()
 
         # Otherwise just scale the y-values
         elif np.shape(other) == ():
             return Tabulation(self.x, self.y / other)
-        
+
         raise ValueError("Cannot divide Tabulation by given value")
 
     def __add__(self, other):
 
         # Addition of two Tabulations
         # Note: the new domain is the union of the given domains
         if type(other) == type(self):
             new_x = Tabulation._xmerge(self.x, other.x)
             return Tabulation(new_x, self(new_x) + other(new_x))
 
         # Otherwise just shift the y-values
         elif np.shape(other) == ():
             return Tabulation(self.x, self.y + other)
-        
+
         raise ValueError("Cannot add Tabulation by given value")
 
         # Note that a constant added to a Tabulation will still return zero
         # outside the domain.
 
     def __sub__(self, other):
 
@@ -203,15 +203,15 @@
         if type(other) == type(self):
             new_x = Tabulation._xmerge(self.x, other.x)
             return Tabulation(new_x, self(new_x) - other(new_x))
 
         # Otherwise just shift the y-values
         elif np.shape(other) == ():
             return Tabulation(self.x, self.y - other)
-        
+
         raise ValueError("Cannot subtract Tabulation by given value")
 
         # Note that a constant subtracted from a Tabulation will still return
         # zero outside the domain.
 
     def __imul__(self, other):
 
@@ -219,28 +219,28 @@
         if type(other) == type(self):
             new_x = Tabulation._xoverlap(self.x, other.x)
             return self._update(new_x, self(new_x) * other(new_x))._trim()
 
         # Otherwise just scale the y-values
         elif np.shape(other) == ():
             return self._update_y(self.y * other)
-        
+
         raise ValueError("Cannot multiply Tabulation in-place by given value")
 
     def __itruediv__(self, other):
 
         # In-place division of two Tabulations
         if type(other) == type(self):
             new_x = Tabulation._xoverlap(self.x, other.x)
             return self._update(new_x, self(new_x) / other(new_x))._trim()
 
         # Otherwise just scale the y-values
         elif np.shape(other) == ():
             return self._update_y(self.y / other)
-        
+
         raise ValueError("Cannot divide Tabulation in-place by given value")
 
     def __iadd__(self, other):
 
         # In-place addition of two Tabulations
         if type(other) == type(self):
             new_x = Tabulation._xmerge(self.x, other.x)
```

### Comparing `rms-tabulation-0.0.3/tests/test_tabulation.py` & `rms_tabulation-0.0.4/tests/test_tabulation.py`

 * *Files identical despite different names*

