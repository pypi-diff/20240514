# Comparing `tmp/chrisversiontest-0.1.1.tar.gz` & `tmp/chrisversiontest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisversiontest-0.1.1.tar", last modified: Tue May 14 15:52:48 2024, max compression
+gzip compressed data, was "chrisversiontest-0.1.2.tar", last modified: Tue May 14 16:11:12 2024, max compression
```

## Comparing `chrisversiontest-0.1.1.tar` & `chrisversiontest-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:48.543618 chrisversiontest-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:48.539618 chrisversiontest-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:48.539618 chrisversiontest-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 15:52:48.543618 chrisversiontest-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:48.539618 chrisversiontest-0.1.1/chrisversiontest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 15:52:48.000000 chrisversiontest-0.1.1/chrisversiontest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-14 15:52:48.000000 chrisversiontest-0.1.1/chrisversiontest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:52:48.000000 chrisversiontest-0.1.1/chrisversiontest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 15:52:48.000000 chrisversiontest-0.1.1/chrisversiontest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 15:52:48.000000 chrisversiontest-0.1.1/chrisversiontest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 15:52:48.000000 chrisversiontest-0.1.1/chrisversiontest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:52:48.543618 chrisversiontest-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:48.539618 chrisversiontest-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:48.539618 chrisversiontest-0.1.1/src/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/src/versioning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:52:48.539618 chrisversiontest-0.1.1/src/versioning/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/src/versioning/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/src/versioning/__pycache__/entrypoint.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 15:52:39.000000 chrisversiontest-0.1.1/src/versioning/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:12.020779 chrisversiontest-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:12.016779 chrisversiontest-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:12.020779 chrisversiontest-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 16:11:12.020779 chrisversiontest-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:12.020779 chrisversiontest-0.1.2/chrisversiontest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 16:11:11.000000 chrisversiontest-0.1.2/chrisversiontest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-14 16:11:12.000000 chrisversiontest-0.1.2/chrisversiontest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:11:12.000000 chrisversiontest-0.1.2/chrisversiontest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 16:11:12.000000 chrisversiontest-0.1.2/chrisversiontest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 16:11:12.000000 chrisversiontest-0.1.2/chrisversiontest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 16:11:12.000000 chrisversiontest-0.1.2/chrisversiontest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:11:12.020779 chrisversiontest-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:12.016779 chrisversiontest-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:12.020779 chrisversiontest-0.1.2/src/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/src/versioning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:12.020779 chrisversiontest-0.1.2/src/versioning/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/src/versioning/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/src/versioning/__pycache__/entrypoint.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 16:11:08.000000 chrisversiontest-0.1.2/src/versioning/entrypoint.py
```

### Comparing `chrisversiontest-0.1.1/.github/workflows/publish.yaml` & `chrisversiontest-0.1.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `chrisversiontest-0.1.1/LICENSE` & `chrisversiontest-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisversiontest-0.1.1/PKG-INFO` & `chrisversiontest-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisversiontest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Testing some versioning stuff in isolation
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/chris11-taylor-nttd/py-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `chrisversiontest-0.1.1/chrisversiontest.egg-info/PKG-INFO` & `chrisversiontest-0.1.2/chrisversiontest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisversiontest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Testing some versioning stuff in isolation
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/chris11-taylor-nttd/py-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `chrisversiontest-0.1.1/pyproject.toml` & `chrisversiontest-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -37,7 +37,8 @@
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 version_scheme = "only-version"
 local_scheme = "no-local-version"
+version_file = "__version__.py"
```

### Comparing `chrisversiontest-0.1.1/src/versioning/__pycache__/entrypoint.cpython-311.pyc` & `chrisversiontest-0.1.2/src/versioning/__pycache__/entrypoint.cpython-311.pyc`

 * *Files identical despite different names*

