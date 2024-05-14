# Comparing `tmp/processing_pypelines-0.0.57.tar.gz` & `tmp/processing_pypelines-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing_pypelines-0.0.57.tar", last modified: Fri May  3 16:41:44 2024, max compression
+gzip compressed data, was "processing_pypelines-0.0.58.tar", last modified: Tue May 14 18:43:45 2024, max compression
```

## Comparing `processing_pypelines-0.0.57.tar` & `processing_pypelines-0.0.58.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2024-05-03 16:41:34.858793 processing_pypelines-0.0.57/LICENSE
--rw-r--r--   0        0        0      118 2024-05-03 16:41:34.858793 processing_pypelines-0.0.57/README.md
--rw-r--r--   0        0        0     1152 2024-05-03 16:41:44.130626 processing_pypelines-0.0.57/pyproject.toml
--rw-r--r--   0        0        0      367 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/__init__.py
--rw-r--r--   0        0        0     4483 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/accessors.py
--rw-r--r--   0        0        0     4633 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/arguments.py
--rw-r--r--   0        0        0    34226 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/celery_tasks.py
--rw-r--r--   0        0        0    11851 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/disk.py
--rw-r--r--   0        0        0     6647 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/examples.py
--rw-r--r--   0        0        0   352259 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/feature_test.ipynb
--rw-r--r--   0        0        0     7880 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/graphs.py
--rw-r--r--   0        0        0    17038 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/loggs.py
--rw-r--r--   0        0        0     5985 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/multisession.py
--rw-r--r--   0        0        0    18914 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/pickle_backend.py
--rw-r--r--   0        0        0     6559 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/pipelines.py
--rw-r--r--   0        0        0     9444 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/pipes.py
--rw-r--r--   0        0        0     3084 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/sessions.py
--rw-r--r--   0        0        0    37032 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/steps.py
--rw-r--r--   0        0        0     3915 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/tasks.py
--rw-r--r--   0        0        0     7360 2024-05-03 16:41:34.870793 processing_pypelines-0.0.57/src/pypelines/versions.py
--rw-r--r--   0        0        0        0 2024-05-03 16:41:34.918792 processing_pypelines-0.0.57/tests/__init__.py
--rw-r--r--   0        0        0      962 2024-05-03 16:41:34.870793 processing_pypelines-0.0.57/tests/tests.py
--rw-r--r--   0        0        0     1230 2024-05-03 16:41:34.870793 processing_pypelines-0.0.57/tests/versions_example.json
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.57/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/README.md
+-rw-r--r--   0        0        0     1152 2024-05-14 18:43:45.204755 processing_pypelines-0.0.58/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/__init__.py
+-rw-r--r--   0        0        0     4483 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/accessors.py
+-rw-r--r--   0        0        0     4633 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/arguments.py
+-rw-r--r--   0        0        0    34226 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/celery_tasks.py
+-rw-r--r--   0        0        0    11851 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/disk.py
+-rw-r--r--   0        0        0     6647 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/examples.py
+-rw-r--r--   0        0        0   352259 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/feature_test.ipynb
+-rw-r--r--   0        0        0     7880 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/graphs.py
+-rw-r--r--   0        0        0    17075 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/loggs.py
+-rw-r--r--   0        0        0     5985 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/multisession.py
+-rw-r--r--   0        0        0    18914 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/pickle_backend.py
+-rw-r--r--   0        0        0     6559 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/pipelines.py
+-rw-r--r--   0        0        0     9444 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/pipes.py
+-rw-r--r--   0        0        0     3084 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/sessions.py
+-rw-r--r--   0        0        0    37032 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/steps.py
+-rw-r--r--   0        0        0     3915 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/tasks.py
+-rw-r--r--   0        0        0     7360 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/versions.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:43:35.208877 processing_pypelines-0.0.58/tests/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/tests/tests.py
+-rw-r--r--   0        0        0     1230 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/tests/versions_example.json
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.58/PKG-INFO
```

### Comparing `processing_pypelines-0.0.57/LICENSE` & `processing_pypelines-0.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/pyproject.toml` & `processing_pypelines-0.0.58/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 maintainers = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 description = "Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = []
-version = "0.0.57"
+version = "0.0.58"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 celery = [
     "celery>=5.3.5",
```

### Comparing `processing_pypelines-0.0.57/src/pypelines/accessors.py` & `processing_pypelines-0.0.58/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/arguments.py` & `processing_pypelines-0.0.58/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/celery_tasks.py` & `processing_pypelines-0.0.58/src/pypelines/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/disk.py` & `processing_pypelines-0.0.58/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/examples.py` & `processing_pypelines-0.0.58/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/feature_test.ipynb` & `processing_pypelines-0.0.58/src/pypelines/feature_test.ipynb`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/graphs.py` & `processing_pypelines-0.0.58/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/loggs.py` & `processing_pypelines-0.0.58/src/pypelines/loggs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,17 @@
 
     logger = logging.getLogger()
 
     logger.setLevel(
         min(terminal_level, file_level)
     )  # set logger level to the lowest usefull, to be sure we can capture messages necessary in handlers
 
-    for handler in [fh, ch]:
+    for handler, level in zip([fh, ch], [file_level, terminal_level]):
 
-        handler.setLevel(file_level)
+        handler.setLevel(level)
         logger.addHandler(handler)
 
 
 class DynamicColoredFormatter(ColoredFormatter):
     """_summary_"""
 
     # note that only message, name, levelname, pathname, process, thread, lineno, levelno and filename can be dynamic.
```

### Comparing `processing_pypelines-0.0.57/src/pypelines/multisession.py` & `processing_pypelines-0.0.58/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/pickle_backend.py` & `processing_pypelines-0.0.58/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/pipelines.py` & `processing_pypelines-0.0.58/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/pipes.py` & `processing_pypelines-0.0.58/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/sessions.py` & `processing_pypelines-0.0.58/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/steps.py` & `processing_pypelines-0.0.58/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/tasks.py` & `processing_pypelines-0.0.58/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/src/pypelines/versions.py` & `processing_pypelines-0.0.58/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/tests/tests.py` & `processing_pypelines-0.0.58/tests/tests.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/tests/versions_example.json` & `processing_pypelines-0.0.58/tests/versions_example.json`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.57/PKG-INFO` & `processing_pypelines-0.0.58/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.57
+Version: 0.0.58
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Home-page: https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Author-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 Maintainer-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: Repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

