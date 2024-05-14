# Comparing `tmp/paradi-0.1.3.tar.gz` & `tmp/paradi-0.1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradi-0.1.3.tar", last modified: Tue May 14 07:41:45 2024, max compression
+gzip compressed data, was "paradi-0.1.3.post1.tar", last modified: Tue May 14 07:46:49 2024, max compression
```

## Comparing `paradi-0.1.3.tar` & `paradi-0.1.3.post1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 07:41:39.000000 paradi-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 07:41:45.873882 paradi-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-14 07:41:39.000000 paradi-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/paradi/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-14 07:41:39.000000 paradi-0.1.3/paradi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-14 07:41:39.000000 paradi-0.1.3/paradi/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-14 07:41:39.000000 paradi-0.1.3/paradi/paradi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/paradi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 07:41:45.000000 paradi-0.1.3/paradi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 07:41:39.000000 paradi-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:41:45.873882 paradi-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 07:41:39.000000 paradi-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:41:45.873882 paradi-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-14 07:41:39.000000 paradi-0.1.3/tests/test_paradi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:46:49.904896 paradi-0.1.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-14 07:46:49.904896 paradi-0.1.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:46:49.904896 paradi-0.1.3.post1/paradi/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/paradi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/paradi/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/paradi/paradi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:46:49.904896 paradi-0.1.3.post1/paradi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-14 07:46:49.000000 paradi-0.1.3.post1/paradi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 07:46:49.000000 paradi-0.1.3.post1/paradi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:46:49.000000 paradi-0.1.3.post1/paradi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 07:46:49.000000 paradi-0.1.3.post1/paradi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:46:49.904896 paradi-0.1.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:46:49.904896 paradi-0.1.3.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-14 07:46:45.000000 paradi-0.1.3.post1/tests/test_paradi.py
```

### Comparing `paradi-0.1.3/LICENSE` & `paradi-0.1.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `paradi-0.1.3/PKG-INFO` & `paradi-0.1.3.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradi
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
 Author: Julien Crambes
 Author-email: Julien Crambes <julien.crambes@gmail.com>
 Project-URL: Homepage, https://github.com/Elektriman/paradi
 Project-URL: Issues, https://github.com/Elektriman/paradi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paradi-0.1.3/README.md` & `paradi-0.1.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `paradi-0.1.3/paradi/logging_config.py` & `paradi-0.1.3.post1/paradi/logging_config.py`

 * *Files identical despite different names*

### Comparing `paradi-0.1.3/paradi/paradi.py` & `paradi-0.1.3.post1/paradi/paradi.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,11 +171,7 @@
                    ):
         """
         This method should save any information needed to make a request to the API after the first authentication
 
         :param response: the response object from the call of the login endpoint
         """
         ...
-
-
-if __name__ == "__main__":
-    raise NotImplementedError("Cannot invoke package as `__main__`, use `import`")
```

### Comparing `paradi-0.1.3/paradi.egg-info/PKG-INFO` & `paradi-0.1.3.post1/paradi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradi
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities.
 Author: Julien Crambes
 Author-email: Julien Crambes <julien.crambes@gmail.com>
 Project-URL: Homepage, https://github.com/Elektriman/paradi
 Project-URL: Issues, https://github.com/Elektriman/paradi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paradi-0.1.3/pyproject.toml` & `paradi-0.1.3.post1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "paradi"
-version = "0.1.3"
+version = "0.1.3.post1"
 authors = [
     { name="Julien Crambes", email="julien.crambes@gmail.com" },
 ]
 description = "This is an abstract class which purpose is to interface any Rest API using python's standard functionnalities."
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `paradi-0.1.3/tests/test_paradi.py` & `paradi-0.1.3.post1/tests/test_paradi.py`

 * *Files identical despite different names*

