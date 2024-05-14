# Comparing `tmp/modelmimic-0.0.1.tar.gz` & `tmp/modelmimic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmimic-0.0.1.tar", last modified: Thu May  2 16:41:08 2024, max compression
+gzip compressed data, was "modelmimic-0.0.2.tar", last modified: Tue May 14 18:23:05 2024, max compression
```

## Comparing `modelmimic-0.0.1.tar` & `modelmimic-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:41:08.078519 modelmimic-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:41:08.070519 modelmimic-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:41:08.074519 modelmimic-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 16:41:03.000000 modelmimic-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 16:41:03.000000 modelmimic-0.0.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-02 16:41:03.000000 modelmimic-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 16:41:03.000000 modelmimic-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-02 16:41:03.000000 modelmimic-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-02 16:41:03.000000 modelmimic-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-02 16:41:03.000000 modelmimic-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 16:41:08.078519 modelmimic-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 16:41:03.000000 modelmimic-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:41:08.074519 modelmimic-0.0.1/modelmimic/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-02 16:41:03.000000 modelmimic-0.0.1/modelmimic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:41:08.074519 modelmimic-0.0.1/modelmimic/config/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-02 16:41:03.000000 modelmimic-0.0.1/modelmimic/config/MVK.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-02 16:41:03.000000 modelmimic-0.0.1/modelmimic/config/TSC.toml
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-02 16:41:03.000000 modelmimic-0.0.1/modelmimic/mimic.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-02 16:41:03.000000 modelmimic-0.0.1/modelmimic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:41:08.074519 modelmimic-0.0.1/modelmimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 16:41:08.000000 modelmimic-0.0.1/modelmimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 16:41:08.000000 modelmimic-0.0.1/modelmimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:41:08.000000 modelmimic-0.0.1/modelmimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 16:41:08.000000 modelmimic-0.0.1/modelmimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 16:41:08.000000 modelmimic-0.0.1/modelmimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 16:41:03.000000 modelmimic-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:41:08.078519 modelmimic-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:41:08.074519 modelmimic-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-02 16:41:03.000000 modelmimic-0.0.1/tests/test_numerics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-02 16:41:03.000000 modelmimic-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:05.612039 modelmimic-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:05.608039 modelmimic-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:05.608039 modelmimic-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-14 18:22:58.000000 modelmimic-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-14 18:22:58.000000 modelmimic-0.0.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-14 18:22:58.000000 modelmimic-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-14 18:22:58.000000 modelmimic-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-14 18:22:58.000000 modelmimic-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-14 18:22:58.000000 modelmimic-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-14 18:22:58.000000 modelmimic-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-14 18:23:05.612039 modelmimic-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-14 18:22:58.000000 modelmimic-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:05.608039 modelmimic-0.0.2/modelmimic/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-14 18:22:58.000000 modelmimic-0.0.2/modelmimic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:05.612039 modelmimic-0.0.2/modelmimic/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-14 18:22:58.000000 modelmimic-0.0.2/modelmimic/config/MVK.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 18:22:58.000000 modelmimic-0.0.2/modelmimic/config/TSC.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-14 18:22:58.000000 modelmimic-0.0.2/modelmimic/mimic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 18:22:58.000000 modelmimic-0.0.2/modelmimic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:05.612039 modelmimic-0.0.2/modelmimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-14 18:23:05.000000 modelmimic-0.0.2/modelmimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 18:23:05.000000 modelmimic-0.0.2/modelmimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:23:05.000000 modelmimic-0.0.2/modelmimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 18:23:05.000000 modelmimic-0.0.2/modelmimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 18:23:05.000000 modelmimic-0.0.2/modelmimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-14 18:22:58.000000 modelmimic-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:23:05.612039 modelmimic-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:05.612039 modelmimic-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-14 18:22:58.000000 modelmimic-0.0.2/tests/test_numerics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-14 18:22:58.000000 modelmimic-0.0.2/tests/test_utils.py
```

### Comparing `modelmimic-0.0.1/.github/workflows/docs.yml` & `modelmimic-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/.github/workflows/pre-commit.yml` & `modelmimic-0.0.2/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/.github/workflows/python-package.yml` & `modelmimic-0.0.2/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `modelmimic-0.0.1/.github/workflows/python-publish.yml` & `modelmimic-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/.gitignore` & `modelmimic-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/LICENSE` & `modelmimic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/PKG-INFO` & `modelmimic-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: modelmimic
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate model-like data, _mimic_ the output of various CIME tests.
 Author-email: Michael Kelleher <kelleherme@ornl.gov>
 License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/LIVVkit/modelmimic/
+Project-URL: Documentation, https://livvkit.github.io/modelmimic/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: netCDF4
 Requires-Dist: pandas
 Requires-Dist: toml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # Model Mimic
+[![Python package](https://github.com/LIVVkit/modelmimic/actions/workflows/python-package.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/LIVVkit/modelmimic/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/python-publish.yml)
+[![Docs](https://github.com/LIVVkit/modelmimic/actions/workflows/docs.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/docs.yml)
+[![Pre-Commit](https://github.com/LIVVkit/modelmimic/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/pre-commit.yml)
+
 ## Generate testing data for [EVV4ESM](https://github.com/LIVVkit/evv4esm)
 This package mimics an Earth System Model run output data so that each type
 of evv4esm test can be checked systematically
```

### Comparing `modelmimic-0.0.1/modelmimic/__init__.py` & `modelmimic-0.0.2/modelmimic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version_info__ = (0, 0, 1)
+__version_info__ = (0, 0, 2)
 __version__ = ".".join(str(_vi) for _vi in __version_info__)
 logo = r"""
 |-------------------------------------------------|
 |    __  __    ____    _____    ______   _        |
 |   |  \/  |  / __ \  |  __ \  |  ____| | |       |
 |   | \  / | | |  | | | |  | | | |__    | |       |
 |   | |\/| | | |  | | | |  | | |  __|   | |       |
```

### Comparing `modelmimic-0.0.1/modelmimic/config/MVK.toml` & `modelmimic-0.0.2/modelmimic/config/MVK.toml`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/modelmimic/config/TSC.toml` & `modelmimic-0.0.2/modelmimic/config/TSC.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [pass_b4b]
 ntimes = 61
 ninst = 12
-size = [4, 6]
+size = [3, 5]
 variables = [
     "T",
     "Q",
     "V",
     "CLDLIQ",
     "CLDICE",
     "NUMLIQ",
@@ -32,15 +32,15 @@
 ensemble = { seed = true }
 to_nc = { out_path = "./data/pass_b4b/tsc_pass_b4b_test", file_suffix = "DT0002", timestep = "sec", step_mult = 10 }
 name = "tsc_pass_b4b_test"
 
 [pass_nb4b]
 ntimes = 61
 ninst = 12
-size = [4, 6]
+size = [3, 5]
 variables = [
     "T",
     "Q",
     "V",
     "CLDLIQ",
     "CLDICE",
     "NUMLIQ",
@@ -67,15 +67,15 @@
 to_nc = { out_path = "./data/pass_nb4b/tsc_pass_nb4b_test", file_suffix = "DT0002", timestep = "sec", step_mult = 10 }
 name = "tsc_pass_nb4b_test"
 
 
 [fail]
 ntimes = 61
 ninst = 12
-size = [4, 6]
+size = [3, 5]
 variables = [
     "T",
     "Q",
     "V",
     "CLDLIQ",
     "CLDICE",
     "NUMLIQ",
```

### Comparing `modelmimic-0.0.1/modelmimic/mimic.py` & `modelmimic-0.0.2/modelmimic/mimic.py`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/modelmimic.egg-info/PKG-INFO` & `modelmimic-0.0.2/modelmimic.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: modelmimic
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate model-like data, _mimic_ the output of various CIME tests.
 Author-email: Michael Kelleher <kelleherme@ornl.gov>
 License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/LIVVkit/modelmimic/
+Project-URL: Documentation, https://livvkit.github.io/modelmimic/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: netCDF4
 Requires-Dist: pandas
 Requires-Dist: toml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # Model Mimic
+[![Python package](https://github.com/LIVVkit/modelmimic/actions/workflows/python-package.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/LIVVkit/modelmimic/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/python-publish.yml)
+[![Docs](https://github.com/LIVVkit/modelmimic/actions/workflows/docs.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/docs.yml)
+[![Pre-Commit](https://github.com/LIVVkit/modelmimic/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/LIVVkit/modelmimic/actions/workflows/pre-commit.yml)
+
 ## Generate testing data for [EVV4ESM](https://github.com/LIVVkit/evv4esm)
 This package mimics an Earth System Model run output data so that each type
 of evv4esm test can be checked systematically
```

### Comparing `modelmimic-0.0.1/modelmimic.egg-info/SOURCES.txt` & `modelmimic-0.0.2/modelmimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/pyproject.toml` & `modelmimic-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modelmimic"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 authors = [{ name = "Michael Kelleher", email = "kelleherme@ornl.gov" }]
 description = "Generate model-like data, _mimic_ the output of various CIME tests."
 readme = "README.md"
 license = { text = "BSD-3-Clause" }
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["numpy", "xarray", "netCDF4", "pandas", "toml"]
 dynamic = ["version"]
 
+[project.urls]
+Homepage = "https://github.com/LIVVkit/modelmimic/"
+Documentation = "https://livvkit.github.io/modelmimic/"
+
 [project.optional-dependencies]
-dev = ["ruff", "isort", "black"]
+dev = ["ruff", "isort", "black", "pytest"]
 
 [tool.setuptools.dynamic]
 version = { attr = "modelmimic.__version__" }
 
 [tool.pydoctor]
 project-name = "ModelMimic"
 make-html = true
```

### Comparing `modelmimic-0.0.1/tests/test_numerics.py` & `modelmimic-0.0.2/tests/test_numerics.py`

 * *Files identical despite different names*

### Comparing `modelmimic-0.0.1/tests/test_utils.py` & `modelmimic-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

