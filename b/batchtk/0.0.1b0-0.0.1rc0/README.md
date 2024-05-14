# Comparing `tmp/batchtk-0.0.1b0.tar.gz` & `tmp/batchtk-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchtk-0.0.1b0.tar", last modified: Wed Apr 24 03:29:18 2024, max compression
+gzip compressed data, was "batchtk-0.0.1rc0.tar", last modified: Tue May 14 21:17:46 2024, max compression
```

## Comparing `batchtk-0.0.1b0.tar` & `batchtk-0.0.1rc0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:18.328970 batchtk-0.0.1b0/batchtk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/batchtk/raytk/
--rwxr-xr-x   0 runner    (1001) docker     (127)       58 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/raytk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/raytk/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/batchtk/runtk/
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/runtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/runtk/dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/runtk/header.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11721 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/runtk/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/runtk/sockets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/runtk/submits.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4159 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/runtk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/batchtk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/batchtk/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/batchtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-24 03:29:18.000000 batchtk-0.0.1b0/batchtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 03:29:18.000000 batchtk-0.0.1b0/batchtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:29:18.000000 batchtk-0.0.1b0/batchtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 03:29:18.000000 batchtk-0.0.1b0/batchtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 03:29:18.000000 batchtk-0.0.1b0/batchtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:18.332970 batchtk-0.0.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/tests/test_sh.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-24 03:29:12.000000 batchtk-0.0.1b0/tests/test_submit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:17:46.085571 batchtk-0.0.1rc0/batchtk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/batchtk/raytk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       58 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/raytk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/raytk/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/batchtk/runtk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/runtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/runtk/dispatchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/runtk/header.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11885 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/runtk/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/runtk/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/runtk/submits.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4159 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/runtk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/batchtk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/batchtk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/batchtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-14 21:17:46.000000 batchtk-0.0.1rc0/batchtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 21:17:46.000000 batchtk-0.0.1rc0/batchtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:17:46.000000 batchtk-0.0.1rc0/batchtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 21:17:46.000000 batchtk-0.0.1rc0/batchtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 21:17:46.000000 batchtk-0.0.1rc0/batchtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:17:46.089571 batchtk-0.0.1rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/tests/test_sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-14 21:17:42.000000 batchtk-0.0.1rc0/tests/test_submit.py
```

### Comparing `batchtk-0.0.1b0/LICENSE.md` & `batchtk-0.0.1rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/PKG-INFO` & `batchtk-0.0.1rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchtk
-Version: 0.0.1b0
+Version: 0.0.1rc0
 Summary: Batch submission toolkit for Python
 Author-email: James Chen <jchen.6727@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: importlib-metadata; python_version > "3"
 
 # batchtk
@@ -26,17 +26,17 @@
 │   │   └── utils.py
 │   └── utils <- utilities used by rest of the package
 │       ├── __init__.py
 │       └── utils.py
 ├── examples
 │   └── colab <- examples of package usage
 │       ├── basic_runner.py
-│       ├── pubtk0.ipynb
-│       ├── pubtk1.ipynb
-│       ├── pubtk2.ipynb
+│       ├── batchtk0.ipynb
+│       ├── batchtk1.ipynb
+│       ├── batchtk2.ipynb
 │       └── socket_runner.py
 ├── LICENSE.md
 ├── pyproject.toml
 ├── README.md
 └── tests <- pytest checks
     ├── cleanup.zsh
     ├── runner_scripts
```

### Comparing `batchtk-0.0.1b0/README.md` & `batchtk-0.0.1rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 │   │   └── utils.py
 │   └── utils <- utilities used by rest of the package
 │       ├── __init__.py
 │       └── utils.py
 ├── examples
 │   └── colab <- examples of package usage
 │       ├── basic_runner.py
-│       ├── pubtk0.ipynb
-│       ├── pubtk1.ipynb
-│       ├── pubtk2.ipynb
+│       ├── batchtk0.ipynb
+│       ├── batchtk1.ipynb
+│       ├── batchtk2.ipynb
 │       └── socket_runner.py
 ├── LICENSE.md
 ├── pyproject.toml
 ├── README.md
 └── tests <- pytest checks
     ├── cleanup.zsh
     ├── runner_scripts
```

### Comparing `batchtk-0.0.1b0/batchtk/raytk/search.py` & `batchtk-0.0.1rc0/batchtk/raytk/search.py`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/batchtk/runtk/dispatchers.py` & `batchtk-0.0.1rc0/batchtk/runtk/dispatchers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import json
 import subprocess
 import hashlib
 from batchtk import runtk
 from batchtk.runtk.submits import Submit
 from batchtk.runtk.sockets import INETSocket, UNIXSocket
 from batchtk.utils import create_path
 import socket
@@ -24,16 +25,22 @@
     returns:
         {'INTRUNTK0': 'foo=1', 'FLOATRUNTK1': 'bar=2.0', 'STRRUNTK2': 'baz=three'}
 
     with runtk.GREPSTR being defined in as 'RUNTK' (see ./header.py)
     """
     cl = len(dictionary)
     get_type = staticmethod(lambda x: type(x).__name__)
+
+    def serialize(key, value): #what if someone creates a dictionary #TODO official global serialize, deserialize functions
+        if type(value) == dict:
+            return "{}={}".format(key, json.dumps(value))
+        else:
+            return "{}={}".format(key, value)
     return {"{}{}{}".format(value_type or get_type(value).upper(), runtk.GREPSTR, cl + i):
-                "{}={}".format(key, value) for i, (key, value) in enumerate(dictionary.items())}
+            serialize(key, value) for i, (key, value) in enumerate(dictionary.items())}
 
     # convert dictionary to proper elements
 class Dispatcher(object):
     """
     base class for all Dispatcher classes
     Handles parsing and injection of passed variables (env) to Runner script, submitting the script to a Runner
     and retrieving outputs
```

### Comparing `batchtk-0.0.1b0/batchtk/runtk/header.py` & `batchtk-0.0.1rc0/batchtk/runtk/header.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
+import ast
 from collections import namedtuple
-
+import numpy
 
 GREPSTR = 'RUNTK'
 SUBMIT = 'submit'
 STDOUT = 'stdout'
 
 #NOTE: changing the second value will change the environment variable name and is SAFE(?)
 # changing the 1st value will require a code refactor since it is referenced codewise in getattribute
@@ -16,20 +17,24 @@
 
 HANDLES = {SUBMIT: 'runtk.SUBMIT',
            STDOUT: 'runtk.STDOUT',
            MSGOUT: 'runtk.MSGOUT',
            SGLOUT: 'runtk.SGLOUT',
            SOCKET: 'runtk.SOCKET'}
 
-SUPPORTS = {
+SUPPORTS = { #TODO numpy handling? or binary serialization?
     'INT': int,
     'FLOAT': float,
     'JSON': json.loads,
     'DICT': json.loads,
     'STR': staticmethod(lambda val: val),
+    'LIST': ast.literal_eval, #TODO ast.literal_eval for each entry?
+    'TUPLE': ast.literal_eval,
+    'FLOAT64': float, #TODO what method encapsulate all other data type, 
+    'INT64': int,
 }
 
 SOCKET_ALIASES = {SOCKET: SOCKET_ENV,
                   JOBID: JOBID_ENV}
 FILE_ALIASES = {SGLOUT: SGLOUT_ENV,
                 MSGOUT: MSGOUT_ENV,
                 JOBID : JOBID_ENV}
```

### Comparing `batchtk-0.0.1b0/batchtk/runtk/runners.py` & `batchtk-0.0.1rc0/batchtk/runtk/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from batchtk.runtk.utils import convert, set_map
 from batchtk import runtk
 from batchtk.runtk.sockets import INETSocket, UNIXSocket
 import socket
 import logging
 import time
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+import ast
 
 class Runner(object):
     """
     base class for all Runner classes
     Handles parsing and injection of passed variables (env) into the python script's namespace. This serves as a base
     class for all runners.
 
@@ -91,15 +92,15 @@
 
     def __getitem__(self, k):
         try:
             return object.__getattribute__(self, k)
         except:
             raise KeyError(k)
 
-    def convert(self, _type: str, val: object):
+    def convert(self, _type: str, val: object):#TODO fix nomenclature for convert
         """
         Internal function called during initialization for converting environment values to the appropriate type
         (see runtk.SUPPORTS)
         Returns
         -------
         self.supports[_type](val)
         """
@@ -107,14 +108,18 @@
             return self.supports[_type](val)
         if _type == '':
             for _type in self.supports:
                 try:
                     return self.supports[_type](val)
                 except:
                     pass
+                try:
+                    return ast.literal_eval(val)
+                except:
+                    pass
         raise KeyError(_type)
 
     def connect(self, **kwargs):
         """
         Method for connecting to the host (dispatcher) if bidirectional communication is implemented
         (see runtk.SocketRunner)
         If it is implemented, it will be a blocking call.
```

### Comparing `batchtk-0.0.1b0/batchtk/runtk/sockets.py` & `batchtk-0.0.1rc0/batchtk/runtk/sockets.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,17 @@
         return self.name
 
     def accept(self):
         self.connection, self.peer_address = self.socket.accept()
         self.connection.settimeout(self.timeout)
         return self.connection, self.peer_address
 
-    def connect(self):
+    def connect(self, socket_name=None):
+        if socket_name:
+            self.name = socket_name
         self.peer_address = self.name
         self.connection = socket.socket(self.type, socket.SOCK_STREAM)
         self.connection.settimeout(self.timeout)
         self.connection.connect(self.name)
 
 
     #def send(self, message):
```

### Comparing `batchtk-0.0.1b0/batchtk/runtk/submits.py` & `batchtk-0.0.1rc0/batchtk/runtk/submits.py`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/batchtk/runtk/utils.py` & `batchtk-0.0.1rc0/batchtk/runtk/utils.py`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/batchtk/utils/utils.py` & `batchtk-0.0.1rc0/batchtk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/batchtk.egg-info/PKG-INFO` & `batchtk-0.0.1rc0/batchtk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchtk
-Version: 0.0.1b0
+Version: 0.0.1rc0
 Summary: Batch submission toolkit for Python
 Author-email: James Chen <jchen.6727@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: importlib-metadata; python_version > "3"
 
 # batchtk
@@ -26,17 +26,17 @@
 │   │   └── utils.py
 │   └── utils <- utilities used by rest of the package
 │       ├── __init__.py
 │       └── utils.py
 ├── examples
 │   └── colab <- examples of package usage
 │       ├── basic_runner.py
-│       ├── pubtk0.ipynb
-│       ├── pubtk1.ipynb
-│       ├── pubtk2.ipynb
+│       ├── batchtk0.ipynb
+│       ├── batchtk1.ipynb
+│       ├── batchtk2.ipynb
 │       └── socket_runner.py
 ├── LICENSE.md
 ├── pyproject.toml
 ├── README.md
 └── tests <- pytest checks
     ├── cleanup.zsh
     ├── runner_scripts
```

### Comparing `batchtk-0.0.1b0/batchtk.egg-info/SOURCES.txt` & `batchtk-0.0.1rc0/batchtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/tests/test_dispatcher.py` & `batchtk-0.0.1rc0/tests/test_dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 from collections import namedtuple
 from batchtk.runtk.dispatchers import Dispatcher, INETDispatcher, UNIXDispatcher
 from batchtk import runtk
-from batchtk.runtk.submits import ZSHSubmit, ZSHSubmitSOCK, ZSHSubmitSFS
+from batchtk.runtk.submits import SHSubmit, SHSubmitSOCK, SHSubmitSFS
 
 class TestDispatcher:
     @pytest.fixture
     def setup(self):
         dispatcher = Dispatcher(env={'type': 'base'}, gid='dispatcher_base')
         return dispatcher
 
@@ -19,16 +19,16 @@
     def test_update_env(self, setup):
         dispatcher = setup
         dispatcher.update_env({'new_var': 'new_value'}, value_type='STR')
         assert 'new_var=new_value' in dispatcher.env.values()
 
 Job = namedtuple('Job', ['Dispatcher', 'Submit'])
 JOBS = [
-        Job(INETDispatcher, ZSHSubmitSOCK),
-        Job(UNIXDispatcher, ZSHSubmitSOCK)
+        Job(INETDispatcher, SHSubmitSOCK),
+        Job(UNIXDispatcher, SHSubmitSOCK)
         ]
 
 class TestJOBS:
     @pytest.fixture(params=JOBS)
     def setup(self, request):
         Submit = request.param.Submit
         submit = Submit()
```

### Comparing `batchtk-0.0.1b0/tests/test_job.py` & `batchtk-0.0.1rc0/tests/test_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 test_job.py
 this file runs a simple test between a dispatcher<->runner pair
 it does not start a subprocess but validates that the file is appropriate and the runner has imported the correct values
 to start bidirectional communication
-the created environment. for subprocess testing, use test_zsh.py.
+the created environment. for subprocess testing, use test_sh.py.
 """
 
 import pytest
 import os
 from batchtk import runtk
 from batchtk.runtk.dispatchers import INETDispatcher, UNIXDispatcher
-from batchtk.runtk.submits import ZSHSubmitSOCK
+from batchtk.runtk.submits import SHSubmitSOCK
 from batchtk.runtk.runners import SocketRunner
 from batchtk.utils import get_exports#TODO implement a more universal get_port_info
 import logging
 import json
 from collections import namedtuple
+from header import TEST_ENVIRONMENT
 
 
 Job = namedtuple('Job', ['Dispatcher', 'Submit'])
 JOBS = [
-        Job(INETDispatcher, ZSHSubmitSOCK),
-        Job(UNIXDispatcher, ZSHSubmitSOCK)
+        Job(INETDispatcher, SHSubmitSOCK),
+        Job(UNIXDispatcher, SHSubmitSOCK)
         ]
 
 logger = logging.getLogger('test')
 logger.setLevel(logging.INFO)
 handler = logging.FileHandler('test_job.log')
 
 formatter = logging.Formatter('>>> %(asctime)s --- %(funcName)s --- %(levelname)s >>>\n%(message)s <<<\n')
@@ -37,17 +38,15 @@
     @pytest.fixture(params=JOBS)
     def setup(self, request):
         Submit = request.param.Submit
         Dispatcher = request.param.Dispatcher
         dispatcher = Dispatcher(project_path=os.getcwd(),
                                      submit=Submit(),
                                      gid='test' + Dispatcher.__name__ + Submit.__name__)
-        dispatcher.update_env({'strvalue': '1',
-                               'intvalue': 2,
-                               'fltvalue': 3.0})
+        dispatcher.update_env(TEST_ENVIRONMENT)
         dispatcher.submit.update_templates(command='python test.py')
         return dispatcher
 
     def test_job(self, setup):
         dispatcher = setup
         dispatcher.create_job()
         assert os.path.exists(dispatcher.handles[runtk.SUBMIT])
@@ -60,15 +59,15 @@
         logger.info("script:\n{}".format(script))
         #logger.info("port info (dispatcher listen):\n{}".format(get_port_info(dispatcher.socket.name[1])))
         assert 'python test.py' in script
         env = get_exports(dispatcher.handles[runtk.SUBMIT])
 
         logger.info(env)
         runner = SocketRunner(env=env)
-        logger.info("runner.socketname:\n{}".format(runner.socketname))
+        logger.info("runner.socket_name:\n{}".format(runner.socket_name))
         runner.connect()
         connection, peer_address = dispatcher.accept()
         #logger.info("port info (runner connect):\n{}".format(get_port_info(dispatcher.socket.name[1])))
         logger.info("runner.host_socket:\n{}".format(runner.host_socket))
         test_message = 'runner -> dispatcher message'
         runner.send(test_message)
         recv_message = dispatcher.recv()
@@ -85,11 +84,10 @@
 dispatcher sent              ---> runner recv
 {} ---> {}""".format(test_message, recv_message))
         assert test_message == recv_message
         runner.close()
         #logger.info("port info (runner close):\n{}".format(get_port_info(dispatcher.socket.name[1])))
         dispatcher.clean()
         logger.info("runner.mappings:\n{}".format(json.dumps(runner.mappings)))
-        assert runner.mappings['strvalue'] == '1'
-        assert runner.mappings['intvalue'] == 2
-        assert runner.mappings['fltvalue'] == 3.0
+        for key, value in TEST_ENVIRONMENT.items():
+            assert runner.mappings[key] == value
         #logger.info("port info (dispatcher clean):\n{}".format(get_port_info(dispatcher.socket.name[1])))
```

### Comparing `batchtk-0.0.1b0/tests/test_sh.py` & `batchtk-0.0.1rc0/tests/test_sh.py`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/tests/test_socket.py` & `batchtk-0.0.1rc0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `batchtk-0.0.1b0/tests/test_submit.py` & `batchtk-0.0.1rc0/tests/test_submit.py`

 * *Files identical despite different names*

