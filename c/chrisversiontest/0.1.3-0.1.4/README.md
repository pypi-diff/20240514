# Comparing `tmp/chrisversiontest-0.1.3.tar.gz` & `tmp/chrisversiontest-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisversiontest-0.1.3.tar", last modified: Tue May 14 16:16:09 2024, max compression
+gzip compressed data, was "chrisversiontest-0.1.4.tar", last modified: Tue May 14 16:23:14 2024, max compression
```

## Comparing `chrisversiontest-0.1.3.tar` & `chrisversiontest-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:09.399796 chrisversiontest-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:09.395796 chrisversiontest-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:09.399796 chrisversiontest-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 16:16:09.399796 chrisversiontest-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:09.399796 chrisversiontest-0.1.3/chrisversiontest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 16:16:09.000000 chrisversiontest-0.1.3/chrisversiontest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 16:16:09.000000 chrisversiontest-0.1.3/chrisversiontest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:16:09.000000 chrisversiontest-0.1.3/chrisversiontest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 16:16:09.000000 chrisversiontest-0.1.3/chrisversiontest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 16:16:09.000000 chrisversiontest-0.1.3/chrisversiontest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 16:16:09.000000 chrisversiontest-0.1.3/chrisversiontest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:16:09.399796 chrisversiontest-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:09.395796 chrisversiontest-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:09.399796 chrisversiontest-0.1.3/src/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/src/versioning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:16:09.399796 chrisversiontest-0.1.3/src/versioning/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/src/versioning/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/src/versioning/__pycache__/entrypoint.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 16:16:09.000000 chrisversiontest-0.1.3/src/versioning/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 16:16:05.000000 chrisversiontest-0.1.3/src/versioning/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:14.614839 chrisversiontest-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:14.606839 chrisversiontest-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:14.610839 chrisversiontest-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 16:23:14.610839 chrisversiontest-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:14.610839 chrisversiontest-0.1.4/chrisversiontest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 16:23:14.000000 chrisversiontest-0.1.4/chrisversiontest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 16:23:14.000000 chrisversiontest-0.1.4/chrisversiontest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:23:14.000000 chrisversiontest-0.1.4/chrisversiontest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 16:23:14.000000 chrisversiontest-0.1.4/chrisversiontest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 16:23:14.000000 chrisversiontest-0.1.4/chrisversiontest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 16:23:14.000000 chrisversiontest-0.1.4/chrisversiontest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:23:14.614839 chrisversiontest-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:14.610839 chrisversiontest-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:14.610839 chrisversiontest-0.1.4/src/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/src/versioning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:23:14.610839 chrisversiontest-0.1.4/src/versioning/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/src/versioning/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/src/versioning/__pycache__/entrypoint.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 16:23:14.000000 chrisversiontest-0.1.4/src/versioning/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-14 16:23:10.000000 chrisversiontest-0.1.4/src/versioning/entrypoint.py
```

### Comparing `chrisversiontest-0.1.3/.github/workflows/publish.yaml` & `chrisversiontest-0.1.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `chrisversiontest-0.1.3/LICENSE` & `chrisversiontest-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisversiontest-0.1.3/PKG-INFO` & `chrisversiontest-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisversiontest
-Version: 0.1.3
+Version: 0.1.4
 Summary: Testing some versioning stuff in isolation
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/chris11-taylor-nttd/py-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `chrisversiontest-0.1.3/chrisversiontest.egg-info/PKG-INFO` & `chrisversiontest-0.1.4/chrisversiontest.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisversiontest
-Version: 0.1.3
+Version: 0.1.4
 Summary: Testing some versioning stuff in isolation
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/chris11-taylor-nttd/py-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `chrisversiontest-0.1.3/pyproject.toml` & `chrisversiontest-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chrisversiontest-0.1.3/src/versioning/__pycache__/entrypoint.cpython-311.pyc` & `chrisversiontest-0.1.4/src/versioning/__pycache__/entrypoint.cpython-311.pyc`

 * *Files identical despite different names*

