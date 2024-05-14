# Comparing `tmp/git_alert-0.3.1.tar.gz` & `tmp/git_alert-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_alert-0.3.1.tar", max compression
+gzip compressed data, was "git_alert-0.3.2.tar", max compression
```

## Comparing `git_alert-0.3.1.tar` & `git_alert-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2024-05-02 06:12:04.421961 git_alert-0.3.1/LICENSE
--rw-r--r--   0        0        0     4908 2024-05-02 06:12:04.421961 git_alert-0.3.1/README.md
--rw-r--r--   0        0        0      142 2024-05-02 06:12:04.421961 git_alert-0.3.1/git_alert/__init__.py
--rw-r--r--   0        0        0      883 2024-05-02 06:12:04.421961 git_alert-0.3.1/git_alert/__main__.py
--rw-r--r--   0        0        0     1348 2024-05-02 06:12:04.421961 git_alert-0.3.1/git_alert/argument_parser.py
--rw-r--r--   0        0        0     1395 2024-05-02 06:12:04.421961 git_alert-0.3.1/git_alert/configuration.py
--rw-r--r--   0        0        0     1285 2024-05-02 06:12:04.421961 git_alert-0.3.1/git_alert/repositories.py
--rw-r--r--   0        0        0      983 2024-05-02 06:12:04.421961 git_alert-0.3.1/git_alert/scripts/git_alert.py
--rw-r--r--   0        0        0     1552 2024-05-02 06:12:04.421961 git_alert-0.3.1/git_alert/traverse.py
--rw-r--r--   0        0        0      658 2024-05-02 06:12:04.421961 git_alert-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 git_alert-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-14 10:21:51.084584 git_alert-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4908 2024-05-14 10:21:51.084584 git_alert-0.3.2/README.md
+-rw-r--r--   0        0        0      142 2024-05-14 10:21:51.084584 git_alert-0.3.2/git_alert/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-14 10:21:51.084584 git_alert-0.3.2/git_alert/__main__.py
+-rw-r--r--   0        0        0     1348 2024-05-14 10:21:51.084584 git_alert-0.3.2/git_alert/argument_parser.py
+-rw-r--r--   0        0        0     1619 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/configuration.py
+-rw-r--r--   0        0        0     1285 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/repositories.py
+-rw-r--r--   0        0        0      983 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/scripts/git_alert.py
+-rw-r--r--   0        0        0     1552 2024-05-14 10:21:51.088584 git_alert-0.3.2/git_alert/traverse.py
+-rw-r--r--   0        0        0      658 2024-05-14 10:21:51.088584 git_alert-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 git_alert-0.3.2/PKG-INFO
```

### Comparing `git_alert-0.3.1/LICENSE` & `git_alert-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.1/README.md` & `git_alert-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.1/git_alert/__main__.py` & `git_alert-0.3.2/git_alert/__main__.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.1/git_alert/argument_parser.py` & `git_alert-0.3.2/git_alert/argument_parser.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.1/git_alert/configuration.py` & `git_alert-0.3.2/git_alert/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 import tomllib
 from pathlib import Path
 
 
 class System:
     def __init__(self):
         self.user = os.environ.get("USER")
+        self.platform = sys.platform
 
     @property
     def config_root(self):
-        return Path("/home") / str(self.user) / ".config/git_alert"
+        if self.platform == "darwin":
+            return Path("/Users") / str(self.user) / ".config/git_alert"
+        elif self.platform == "linux":
+            return Path("/home") / str(self.user) / ".config/git_alert"
 
     @property
     def config_file(self):
-        return self.config_root / "config.toml"
+        if self.config_root:
+            return self.config_root / "config.toml"
 
 
 class ReadConfig:
 
     def __init__(self, system: System, config=None):
         if config:
             self.CONFIG_FILE = config
```

### Comparing `git_alert-0.3.1/git_alert/repositories.py` & `git_alert-0.3.2/git_alert/repositories.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.1/git_alert/scripts/git_alert.py` & `git_alert-0.3.2/git_alert/scripts/git_alert.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.1/git_alert/traverse.py` & `git_alert-0.3.2/git_alert/traverse.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.3.1/pyproject.toml` & `git_alert-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git_alert"
-version = "0.3.1"
+version = "0.3.2"
 
 description = "Checks a given path and its sub-directories for dirty git repositories."
 authors = ["Simon Antonius Lauer <simon.lauer@posteo.de>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "git_alert"}]
```

### Comparing `git_alert-0.3.1/PKG-INFO` & `git_alert-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_alert
-Version: 0.3.1
+Version: 0.3.2
 Summary: Checks a given path and its sub-directories for dirty git repositories.
 License: MIT
 Author: Simon Antonius Lauer
 Author-email: simon.lauer@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

