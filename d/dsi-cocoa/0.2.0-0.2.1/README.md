# Comparing `tmp/dsi_cocoa-0.2.0.tar.gz` & `tmp/dsi_cocoa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.2.0.tar", last modified: Thu May  9 20:51:07 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.2.1.tar", last modified: Tue May 14 15:49:39 2024, max compression
```

## Comparing `dsi_cocoa-0.2.0.tar` & `dsi_cocoa-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.747569 dsi_cocoa-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.751569 dsi_cocoa-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.751569 dsi_cocoa-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.751569 dsi_cocoa-0.2.0/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.087664 dsi_cocoa-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.087664 dsi_cocoa-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.087664 dsi_cocoa-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-14 15:49:35.000000 dsi_cocoa-0.2.1/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:49:39.091663 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 15:49:39.000000 dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.2.0/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.2.1/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.2.1/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/.gitignore` & `dsi_cocoa-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/.pre-commit-config.yaml` & `dsi_cocoa-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/PKG-INFO` & `dsi_cocoa-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.2.0
+Version: 0.2.1
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.2.0/README.md` & `dsi_cocoa-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/pyproject.toml` & `dsi_cocoa-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.2.1/src/cocoa/evaluate_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Main entry point for complete evaluation of a python codebase in git
 """
 
 import argparse
 import os
+import shutil
 
 from termcolor import cprint
 
 from cocoa.constants import (
     MAX_CELLS_PER_NOTEBOOK,
     MAX_FUNCTIONS_PER_NOTEBOOK,
     MAX_LINES_PER_CELL,
+    PREAMBLE_TEXT,
 )
 from cocoa.linting import (
     black_python_file,
     code_contains_subprocess,
     functions_without_docstrings,
     get_pylint_warnings,
     is_code_in_functions_or_main,
@@ -147,15 +149,15 @@
 
 def evaluate_repo(
     path_or_url, lint_flag, start_date=None, verbose=False, branchinfo=False
 ):
     """
     This is the entry point to running the automated code review.
     """
-
+    cprint(PREAMBLE_TEXT, color="green")
     if os.path.isdir(path_or_url):
         if not is_git_repo(path_or_url):
             print(f"Error: {path_or_url} is not a Git repository.")
             exit(1)
 
         check_branch_names(path_or_url)
         if branchinfo:
@@ -171,16 +173,19 @@
         repo_path = clone_repo(path_or_url)
         evaluate_repo(
             repo_path,
             lint_flag=lint_flag,
             start_date=start_date,
             verbose=verbose,
         )
+        shutil.rmtree(repo_path)
     else:
-        print(f"Error: {path_or_url} is not a Git repository URL.")
+        print(
+            f"Error: {path_or_url} is either private or not a git repository. 404."
+        )
         exit(1)
     return 0
 
 
 def main():
     parser = argparse.ArgumentParser(description="COCOA CLI")
```

### Comparing `dsi_cocoa-0.2.0/src/cocoa/linting.py` & `dsi_cocoa-0.2.1/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/src/cocoa/notebooks.py` & `dsi_cocoa-0.2.1/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/src/cocoa/repo.py` & `dsi_cocoa-0.2.1/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/src/cocoa/spring2024.py` & `dsi_cocoa-0.2.1/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.2.0
+Version: 0.2.1
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.2.1/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 README.md
-eval-repo.sh
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/main.workflow.yml
 .github/workflows/publish.workflow.yml
 src/cocoa/__init__.py
 src/cocoa/constants.py
```

