# Comparing `tmp/messages_local-0.0.55.tar.gz` & `tmp/messages_local-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages_local-0.0.55.tar", last modified: Tue May 14 08:27:58 2024, max compression
+gzip compressed data, was "messages_local-0.0.56.tar", last modified: Tue May 14 08:43:55 2024, max compression
```

## Comparing `messages_local-0.0.55.tar` & `messages_local-0.0.56.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:27:58.504678 messages_local-0.0.55/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 08:27:58.504678 messages_local-0.0.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-14 08:27:23.000000 messages_local-0.0.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:27:58.500678 messages_local-0.0.55/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:27:58.500678 messages_local-0.0.55/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-14 08:27:23.000000 messages_local-0.0.55/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:27:23.000000 messages_local-0.0.55/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:27:58.500678 messages_local-0.0.55/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 08:27:58.000000 messages_local-0.0.55/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 08:27:58.000000 messages_local-0.0.55/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:27:58.000000 messages_local-0.0.55/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 08:27:58.000000 messages_local-0.0.55/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 08:27:58.000000 messages_local-0.0.55/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-14 08:27:23.000000 messages_local-0.0.55/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:27:58.504678 messages_local-0.0.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-14 08:27:23.000000 messages_local-0.0.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:43:55.834952 messages_local-0.0.56/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 08:43:55.830952 messages_local-0.0.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-14 08:43:23.000000 messages_local-0.0.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:43:55.830952 messages_local-0.0.56/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:43:55.830952 messages_local-0.0.56/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-14 08:43:23.000000 messages_local-0.0.56/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:43:23.000000 messages_local-0.0.56/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:43:55.830952 messages_local-0.0.56/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 08:43:55.000000 messages_local-0.0.56/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 08:43:55.000000 messages_local-0.0.56/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:43:55.000000 messages_local-0.0.56/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 08:43:55.000000 messages_local-0.0.56/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 08:43:55.000000 messages_local-0.0.56/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-14 08:43:23.000000 messages_local-0.0.56/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:43:55.834952 messages_local-0.0.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-14 08:43:23.000000 messages_local-0.0.56/setup.py
```

### Comparing `messages_local-0.0.55/PKG-INFO` & `messages_local-0.0.56/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.55
+Version: 0.0.56
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages_local-0.0.55/README.md` & `messages_local-0.0.56/README.md`

 * *Files identical despite different names*

### Comparing `messages_local-0.0.55/messages_local/src/MessagesLocal.py` & `messages_local-0.0.56/messages_local/src/MessagesLocal.py`

 * *Files identical despite different names*

### Comparing `messages_local-0.0.55/messages_local.egg-info/PKG-INFO` & `messages_local-0.0.56/messages_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.55
+Version: 0.0.56
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages_local-0.0.55/setup.py` & `messages_local-0.0.56/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.55',  # https://pypi.org/project/messages-local
+    version='0.0.56',  # https://pypi.org/project/messages-local
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
```

