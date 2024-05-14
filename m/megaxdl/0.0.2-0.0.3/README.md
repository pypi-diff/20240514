# Comparing `tmp/megaxdl-0.0.2.tar.gz` & `tmp/megaxdl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaxdl-0.0.2.tar", last modified: Tue May 14 10:42:26 2024, max compression
+gzip compressed data, was "megaxdl-0.0.3.tar", last modified: Tue May 14 10:47:34 2024, max compression
```

## Comparing `megaxdl-0.0.2.tar` & `megaxdl-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:42:26.084700 megaxdl-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 10:42:19.000000 megaxdl-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:42:26.080700 megaxdl-0.0.2/Megaxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38446 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:42:26.084700 megaxdl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 10:42:19.000000 megaxdl-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:42:26.084700 megaxdl-0.0.2/megaxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:42:26.084700 megaxdl-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 10:42:19.000000 megaxdl-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:34.335612 megaxdl-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 10:47:30.000000 megaxdl-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:34.335612 megaxdl-0.0.3/Megaxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38458 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:47:34.335612 megaxdl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 10:47:30.000000 megaxdl-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:34.335612 megaxdl-0.0.3/megaxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:47:34.335612 megaxdl-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 10:47:30.000000 megaxdl-0.0.3/setup.py
```

### Comparing `megaxdl-0.0.2/LICENSE` & `megaxdl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.2/Megaxdl/crypto.py` & `megaxdl-0.0.3/Megaxdl/crypto.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.2/Megaxdl/errors.py` & `megaxdl-0.0.3/Megaxdl/errors.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.2/Megaxdl/mega.py` & `megaxdl-0.0.3/Megaxdl/mega.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import os, re
+import os
+import re, time
 import math, tqdm
 import shutil, random
 import secrets, hashlib
 import logging, binascii
 import requests, tempfile
 
 from pathlib import Path
```

### Comparing `megaxdl-0.0.2/PKG-INFO` & `megaxdl-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.2
+Version: 0.0.3
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.2/README.md` & `megaxdl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.2/megaxdl.egg-info/PKG-INFO` & `megaxdl-0.0.3/megaxdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.2
+Version: 0.0.3
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.2/setup.py` & `megaxdl-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 install = ["tqdm>=4.64.1",
            "tenacity>=8.2.2",
            "requests>=2.27.1",
            "pycryptodome>=3.20.0,<4.0.0"]
 
 setup(name='megaxdl',
-      version='0.0.2',
+      version='0.0.3',
       python_requires='~=3.10',
       packages=find_packages(),
       long_description=readme,
       install_requires=install,
       include_package_data=True,
       long_description_content_type='text/markdown')
```

