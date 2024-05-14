# Comparing `tmp/dsi_cocoa-0.2.1.tar.gz` & `tmp/dsi_cocoa-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.2.1.tar", last modified: Tue May 14 15:49:39 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.2.2.tar", last modified: Tue May 14 16:07:18 2024, max compression
```

## Comparing `dsi_cocoa-0.2.1.tar` & `dsi_cocoa-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.087664 dsi_cocoa-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.087664 dsi_cocoa-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.087664 dsi_cocoa-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.599231 dsi_cocoa-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.603231 dsi_cocoa-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.603231 dsi_cocoa-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.603231 dsi_cocoa-0.2.2/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.2.1/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.2.2/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.2.2/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/.gitignore` & `dsi_cocoa-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/.pre-commit-config.yaml` & `dsi_cocoa-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/PKG-INFO` & `dsi_cocoa-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.2.1
+Version: 0.2.2
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.2.1/README.md` & `dsi_cocoa-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/pyproject.toml` & `dsi_cocoa-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.2.2/src/cocoa/evaluate_repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/src/cocoa/linting.py` & `dsi_cocoa-0.2.2/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/src/cocoa/notebooks.py` & `dsi_cocoa-0.2.2/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/src/cocoa/repo.py` & `dsi_cocoa-0.2.2/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/src/cocoa/spring2024.py` & `dsi_cocoa-0.2.2/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.2.1
+Version: 0.2.2
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

