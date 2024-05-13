# Comparing `tmp/repo_find_orphans-0.0.4.tar.gz` & `tmp/repo_find_orphans-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo_find_orphans-0.0.4.tar", max compression
+gzip compressed data, was "repo_find_orphans-0.0.5.tar", max compression
```

## Comparing `repo_find_orphans-0.0.4.tar` & `repo_find_orphans-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2024-05-06 21:12:33.300704 repo_find_orphans-0.0.4/LICENSE
--rw-r--r--   0        0        0     2336 2024-05-06 22:15:23.758657 repo_find_orphans-0.0.4/README.md
--rw-r--r--   0        0        0     5483 2024-05-13 23:13:27.970927 repo_find_orphans-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 21:12:33.301652 repo_find_orphans-0.0.4/src/repo_find_orphans/__init__.py
--rw-r--r--   0        0        0      642 2024-05-06 21:12:33.301793 repo_find_orphans-0.0.4/src/repo_find_orphans/cli.py
--rw-r--r--   0        0        0      806 2024-05-06 21:12:33.301920 repo_find_orphans-0.0.4/src/repo_find_orphans/parse.py
--rw-r--r--   0        0        0      991 2024-05-06 21:12:33.302033 repo_find_orphans-0.0.4/src/repo_find_orphans/scan.py
--rw-r--r--   0        0        0        0 2024-05-06 21:12:33.302072 repo_find_orphans-0.0.4/src/repo_find_orphans/types/__init__.py
--rw-r--r--   0        0        0      337 2024-05-06 21:12:33.302232 repo_find_orphans-0.0.4/src/repo_find_orphans/types/project.py
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 repo_find_orphans-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-06 21:12:33.300704 repo_find_orphans-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2336 2024-05-06 22:15:23.758657 repo_find_orphans-0.0.5/README.md
+-rw-r--r--   0        0        0     5483 2024-05-13 23:32:59.799120 repo_find_orphans-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 21:12:33.301652 repo_find_orphans-0.0.5/src/repo_find_orphans/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-06 21:12:33.301793 repo_find_orphans-0.0.5/src/repo_find_orphans/cli.py
+-rw-r--r--   0        0        0      806 2024-05-06 21:12:33.301920 repo_find_orphans-0.0.5/src/repo_find_orphans/parse.py
+-rw-r--r--   0        0        0     1012 2024-05-13 23:34:17.459613 repo_find_orphans-0.0.5/src/repo_find_orphans/scan.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:12:33.302072 repo_find_orphans-0.0.5/src/repo_find_orphans/types/__init__.py
+-rw-r--r--   0        0        0      337 2024-05-06 21:12:33.302232 repo_find_orphans-0.0.5/src/repo_find_orphans/types/project.py
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 repo_find_orphans-0.0.5/PKG-INFO
```

### Comparing `repo_find_orphans-0.0.4/LICENSE` & `repo_find_orphans-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.4/README.md` & `repo_find_orphans-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.4/pyproject.toml` & `repo_find_orphans-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "repo-find-orphans"
 authors = ["Vlad <vlad@v-lad.org>"]
 description = "Supplements to the repo script"
-version = "0.0.4"
+version = "0.0.5"
 readme = "README.md"
 
 packages = [
   { include = "repo_find_orphans", from = "src" }
 ]
 
 classifiers = [
```

### Comparing `repo_find_orphans-0.0.4/src/repo_find_orphans/cli.py` & `repo_find_orphans-0.0.5/src/repo_find_orphans/cli.py`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.4/src/repo_find_orphans/parse.py` & `repo_find_orphans-0.0.5/src/repo_find_orphans/parse.py`

 * *Files identical despite different names*

### Comparing `repo_find_orphans-0.0.4/src/repo_find_orphans/scan.py` & `repo_find_orphans-0.0.5/src/repo_find_orphans/scan.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if gpath.is_dir():
             continue
         if gpath.name in ignored_files:
             continue
 
         clean_path = gpath.relative_to(Path(path))
 
-        if any(str(clean_path).startswith(str(proj_path)) for proj_path in project_paths):
+        if any((str(clean_path.parent) + "/").startswith(str(proj_path) + "/") for proj_path in project_paths):
             continue
         if any(str(clean_path).startswith(str(proj_path)) for proj_path in dirs):
             continue
 
         dirs.add(clean_path.parent)
 
     return dirs
```

### Comparing `repo_find_orphans-0.0.4/PKG-INFO` & `repo_find_orphans-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-find-orphans
-Version: 0.0.4
+Version: 0.0.5
 Summary: Supplements to the repo script
 Author: Vlad
 Author-email: vlad@v-lad.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

