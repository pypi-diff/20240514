# Comparing `tmp/repo_find_orphans-0.0.3.tar.gz` & `tmp/repo_find_orphans-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo_find_orphans-0.0.3.tar", max compression
+gzip compressed data, was "repo_find_orphans-0.0.4.tar", max compression
```

## Comparing `repo_find_orphans-0.0.3.tar` & `repo_find_orphans-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2024-05-06 21:12:33.300704 repo_find_orphans-0.0.3/LICENSE
--rw-r--r--   0        0        0     2336 2024-05-06 22:15:23.758657 repo_find_orphans-0.0.3/README.md
--rw-r--r--   0        0        0     5482 2024-05-06 22:15:09.989670 repo_find_orphans-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 21:12:33.301652 repo_find_orphans-0.0.3/src/repo_find_orphans/__init__.py
--rw-r--r--   0        0        0      642 2024-05-06 21:12:33.301793 repo_find_orphans-0.0.3/src/repo_find_orphans/cli.py
--rw-r--r--   0        0        0      806 2024-05-06 21:12:33.301920 repo_find_orphans-0.0.3/src/repo_find_orphans/parse.py
--rw-r--r--   0        0        0      991 2024-05-06 21:12:33.302033 repo_find_orphans-0.0.3/src/repo_find_orphans/scan.py
--rw-r--r--   0        0        0        0 2024-05-06 21:12:33.302072 repo_find_orphans-0.0.3/src/repo_find_orphans/types/__init__.py
--rw-r--r--   0        0        0      337 2024-05-06 21:12:33.302232 repo_find_orphans-0.0.3/src/repo_find_orphans/types/project.py
--rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 repo_find_orphans-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-06 21:12:33.300704 repo_find_orphans-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2336 2024-05-06 22:15:23.758657 repo_find_orphans-0.0.4/README.md
+-rw-r--r--   0        0        0     5483 2024-05-13 23:13:27.970927 repo_find_orphans-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 21:12:33.301652 repo_find_orphans-0.0.4/src/repo_find_orphans/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-06 21:12:33.301793 repo_find_orphans-0.0.4/src/repo_find_orphans/cli.py
+-rw-r--r--   0        0        0      806 2024-05-06 21:12:33.301920 repo_find_orphans-0.0.4/src/repo_find_orphans/parse.py
+-rw-r--r--   0        0        0      991 2024-05-06 21:12:33.302033 repo_find_orphans-0.0.4/src/repo_find_orphans/scan.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:12:33.302072 repo_find_orphans-0.0.4/src/repo_find_orphans/types/__init__.py
+-rw-r--r--   0        0        0      337 2024-05-06 21:12:33.302232 repo_find_orphans-0.0.4/src/repo_find_orphans/types/project.py
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 repo_find_orphans-0.0.4/PKG-INFO
```

### Comparing `repo_find_orphans-0.0.3/LICENSE` & `repo_find_orphans-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.3/README.md` & `repo_find_orphans-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.3/pyproject.toml` & `repo_find_orphans-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "repo-find-orphans"
 authors = ["Vlad <vlad@v-lad.org>"]
 description = "Supplements to the repo script"
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 
 packages = [
   { include = "repo_find_orphans", from = "src" }
 ]
 
 classifiers = [
@@ -25,15 +25,15 @@
 
 [project.urls]
 Homepage = "https://github.com/vladistan/repo-find-orphans"
 Issues = "https://github.com/vladistan/repo-find-orphans/issues"
 
 
 [tool.poetry.dependencies]
-python = "3.11.2"
+python = "^3.11.0"
 annotated-types = "^0.6.0"
 defusedxml = "^0.7.1"
 typer = "^0.12.3"
 
 [tool.poetry.scripts]
 repo-find-orphans = "repo_find_orphans.cli:app"
```

### Comparing `repo_find_orphans-0.0.3/src/repo_find_orphans/cli.py` & `repo_find_orphans-0.0.4/src/repo_find_orphans/cli.py`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.3/src/repo_find_orphans/parse.py` & `repo_find_orphans-0.0.4/src/repo_find_orphans/parse.py`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.3/src/repo_find_orphans/scan.py` & `repo_find_orphans-0.0.4/src/repo_find_orphans/scan.py`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.3/PKG-INFO` & `repo_find_orphans-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: repo-find-orphans
-Version: 0.0.3
+Version: 0.0.4
 Summary: Supplements to the repo script
 Author: Vlad
 Author-email: vlad@v-lad.org
-Requires-Python: ==3.11.2
+Requires-Python: >=3.11.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: annotated-types (>=0.6.0,<0.7.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
```

