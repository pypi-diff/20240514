# Comparing `tmp/cms_pri_chmod-0.0.2.tar.gz` & `tmp/cms_pri_chmod-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cms_pri_chmod-0.0.2.tar", last modified: Tue May 14 09:28:56 2024, max compression
+gzip compressed data, was "cms_pri_chmod-0.0.3.tar", last modified: Tue May 14 09:38:41 2024, max compression
```

## Comparing `cms_pri_chmod-0.0.2.tar` & `cms_pri_chmod-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:28:56.380841 cms_pri_chmod-0.0.2/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2024-05-14 09:16:51.000000 cms_pri_chmod-0.0.2/LICENSE
--rw-r--r--   0 bytedance   (502) staff       (20)      527 2024-05-14 09:28:56.380309 cms_pri_chmod-0.0.2/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)       38 2024-05-14 09:16:39.000000 cms_pri_chmod-0.0.2/README.md
--rw-r--r--   0 bytedance   (502) staff       (20)      557 2024-05-14 09:25:22.000000 cms_pri_chmod-0.0.2/pyproject.toml
--rw-r--r--   0 bytedance   (502) staff       (20)       38 2024-05-14 09:28:56.381234 cms_pri_chmod-0.0.2/setup.cfg
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:28:56.376825 cms_pri_chmod-0.0.2/src/
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:28:56.377531 cms_pri_chmod-0.0.2/src/cms_pri_chmod/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2024-05-14 09:15:12.000000 cms_pri_chmod-0.0.2/src/cms_pri_chmod/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)       42 2024-05-14 09:15:40.000000 cms_pri_chmod-0.0.2/src/cms_pri_chmod/main.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:28:56.379535 cms_pri_chmod-0.0.2/src/cms_pri_chmod.egg-info/
--rw-r--r--   0 bytedance   (502) staff       (20)      527 2024-05-14 09:28:56.000000 cms_pri_chmod-0.0.2/src/cms_pri_chmod.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)      265 2024-05-14 09:28:56.000000 cms_pri_chmod-0.0.2/src/cms_pri_chmod.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2024-05-14 09:28:56.000000 cms_pri_chmod-0.0.2/src/cms_pri_chmod.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       20 2024-05-14 09:28:56.000000 cms_pri_chmod-0.0.2/src/cms_pri_chmod.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (502) staff       (20)      355 2024-05-14 09:28:33.000000 cms_pri_chmod-0.0.2/src/setup.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:38:41.328429 cms_pri_chmod-0.0.3/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2024-05-14 09:16:51.000000 cms_pri_chmod-0.0.3/LICENSE
+-rw-r--r--   0 bytedance   (502) staff       (20)      527 2024-05-14 09:38:41.327906 cms_pri_chmod-0.0.3/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)       38 2024-05-14 09:16:39.000000 cms_pri_chmod-0.0.3/README.md
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:38:41.327151 cms_pri_chmod-0.0.3/cms_pri_chmod.egg-info/
+-rw-r--r--   0 bytedance   (502) staff       (20)      527 2024-05-14 09:38:41.000000 cms_pri_chmod-0.0.3/cms_pri_chmod.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)      245 2024-05-14 09:38:41.000000 cms_pri_chmod-0.0.3/cms_pri_chmod.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        1 2024-05-14 09:38:41.000000 cms_pri_chmod-0.0.3/cms_pri_chmod.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       18 2024-05-14 09:38:41.000000 cms_pri_chmod-0.0.3/cms_pri_chmod.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)      557 2024-05-14 09:38:18.000000 cms_pri_chmod-0.0.3/pyproject.toml
+-rw-r--r--   0 bytedance   (502) staff       (20)       38 2024-05-14 09:38:41.328545 cms_pri_chmod-0.0.3/setup.cfg
+-rw-r--r--   0 bytedance   (502) staff       (20)      359 2024-05-14 09:38:36.000000 cms_pri_chmod-0.0.3/setup.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:38:41.322016 cms_pri_chmod-0.0.3/src/
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2024-05-14 09:38:41.325949 cms_pri_chmod-0.0.3/src/cms_pri_chmod/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2024-05-14 09:15:12.000000 cms_pri_chmod-0.0.3/src/cms_pri_chmod/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)       42 2024-05-14 09:15:40.000000 cms_pri_chmod-0.0.3/src/cms_pri_chmod/main.py
```

### Comparing `cms_pri_chmod-0.0.2/PKG-INFO` & `cms_pri_chmod-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cms_pri_chmod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: wkk <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cms_pri_chmod-0.0.2/pyproject.toml` & `cms_pri_chmod-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cms_pri_chmod"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="wkk", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cms_pri_chmod-0.0.2/src/cms_pri_chmod.egg-info/PKG-INFO` & `cms_pri_chmod-0.0.3/cms_pri_chmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cms_pri_chmod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: wkk <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

