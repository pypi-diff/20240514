# Comparing `tmp/skeletonkey-0.2.12.tar.gz` & `tmp/skeletonkey-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.2.12.tar", last modified: Tue Apr 30 18:37:28 2024, max compression
+gzip compressed data, was "skeletonkey-0.2.13.tar", last modified: Tue May 14 18:10:05 2024, max compression
```

## Comparing `skeletonkey-0.2.12.tar` & `skeletonkey-0.2.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:37:28.331837 skeletonkey-0.2.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-30 18:37:28.327837 skeletonkey-0.2.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:37:28.331837 skeletonkey-0.2.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:37:28.327837 skeletonkey-0.2.12/skeletonkey/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/instantiate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:37:28.327837 skeletonkey-0.2.12/skeletonkey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/skeletonkey/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16514 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/instantiate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/skeletonkey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.2.12/LICENSE` & `skeletonkey-0.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.12/PKG-INFO` & `skeletonkey-0.2.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.2.12
+Version: 0.2.13
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `skeletonkey-0.2.12/README.md` & `skeletonkey-0.2.13/README.md`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.12/setup.py` & `skeletonkey-0.2.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version='v0.2.12',
+    version='v0.2.13',
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.2.12/skeletonkey/__init__.py` & `skeletonkey-0.2.13/skeletonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.12/skeletonkey/config.py` & `skeletonkey-0.2.13/skeletonkey/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This code provides a set of utility functions to handle YAML configurations. 
 It facilitates the management of complex configurations for applications using YAML 
 files and enables the dynamic loading of classes and their arguments at runtime.
 """
 import yaml
 import argparse
 import os
-from typing import List, Tuple
+from typing import List, Tuple, Union
 
 from .instantiate import instantiate
 
 BASE_DEFAULT_KEYWORD: str = "defaults"
 BASE_COLLECTION_KEYWORD: str = "keyring"
 
 class Config():
@@ -35,15 +35,15 @@
         if len(args) == 1:
             if not isinstance(args[0], dict):
                 raise ValueError("Supplied arg must be a dictionary")
             self._init_from_dict(args[0])
         else:
             self._init_from_dict(kwargs)
 
-    def update(self, update_config: dict|'Config'):
+    def update(self, update_config: Union[dict, 'Config']):
         """
         Take a config in some format and place those values into the config.
         This will overwrite values if they are present or create them if they are not.
 
         Args:
             update_config (dict|Config): The keys/values to place into the config. If this is a dictionary,
             it is expected that the keys are in dot notation.
```

### Comparing `skeletonkey-0.2.12/skeletonkey/core.py` & `skeletonkey-0.2.13/skeletonkey/core.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.12/skeletonkey/instantiate.py` & `skeletonkey-0.2.13/skeletonkey/instantiate.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.12/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.2.13/skeletonkey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.2.12
+Version: 0.2.13
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

