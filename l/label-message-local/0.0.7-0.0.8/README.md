# Comparing `tmp/label_message_local-0.0.7.tar.gz` & `tmp/label_message_local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "label_message_local-0.0.7.tar", last modified: Mon May 13 20:57:04 2024, max compression
+gzip compressed data, was "label_message_local-0.0.8.tar", last modified: Tue May 14 14:35:40 2024, max compression
```

## Comparing `label_message_local-0.0.7.tar` & `label_message_local-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:57:04.094177 label_message_local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 20:57:04.094177 label_message_local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:56:48.000000 label_message_local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:57:04.094177 label_message_local-0.0.7/label_message_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:57:04.094177 label_message_local-0.0.7/label_message_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-13 20:56:48.000000 label_message_local-0.0.7/label_message_local/src/LabelConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-13 20:56:48.000000 label_message_local-0.0.7/label_message_local/src/LabelMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:56:48.000000 label_message_local-0.0.7/label_message_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:57:04.094177 label_message_local-0.0.7/label_message_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 20:57:04.000000 label_message_local-0.0.7/label_message_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-13 20:57:04.000000 label_message_local-0.0.7/label_message_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:57:04.000000 label_message_local-0.0.7/label_message_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 20:57:04.000000 label_message_local-0.0.7/label_message_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 20:57:04.000000 label_message_local-0.0.7/label_message_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 20:56:48.000000 label_message_local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:57:04.094177 label_message_local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-13 20:56:48.000000 label_message_local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:35:40.111106 label_message_local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 14:35:40.111106 label_message_local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:35:22.000000 label_message_local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:35:40.111106 label_message_local-0.0.8/label_message_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:35:40.111106 label_message_local-0.0.8/label_message_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-14 14:35:22.000000 label_message_local-0.0.8/label_message_local/src/LabelConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-14 14:35:22.000000 label_message_local-0.0.8/label_message_local/src/LabelMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:35:22.000000 label_message_local-0.0.8/label_message_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:35:40.111106 label_message_local-0.0.8/label_message_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 14:35:40.000000 label_message_local-0.0.8/label_message_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-14 14:35:40.000000 label_message_local-0.0.8/label_message_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:35:40.000000 label_message_local-0.0.8/label_message_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 14:35:40.000000 label_message_local-0.0.8/label_message_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 14:35:40.000000 label_message_local-0.0.8/label_message_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 14:35:22.000000 label_message_local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:35:40.111106 label_message_local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-14 14:35:22.000000 label_message_local-0.0.8/setup.py
```

### Comparing `label_message_local-0.0.7/PKG-INFO` & `label_message_local-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: label-message-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles label-message-local Python
 Home-page: https://github.com/circles-zone/label-message-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `label_message_local-0.0.7/label_message_local/src/LabelConstants.py` & `label_message_local-0.0.8/label_message_local/src/LabelConstants.py`

 * *Files identical despite different names*

### Comparing `label_message_local-0.0.7/label_message_local/src/LabelMessage.py` & `label_message_local-0.0.8/label_message_local/src/LabelMessage.py`

 * *Files identical despite different names*

### Comparing `label_message_local-0.0.7/label_message_local.egg-info/PKG-INFO` & `label_message_local-0.0.8/label_message_local.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: label-message-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles label-message-local Python
 Home-page: https://github.com/circles-zone/label-message-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `label_message_local-0.0.7/pyproject.toml` & `label_message_local-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `label_message_local-0.0.7/setup.py` & `label_message_local-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "label-message-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/label-message-local/
-    version='0.0.7',
+    version='0.0.8',
     author="Circles",
     author_email="info@circlez.ai",
     description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     # packages=setuptools.find_packages(),
```

