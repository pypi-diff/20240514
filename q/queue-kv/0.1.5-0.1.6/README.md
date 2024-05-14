# Comparing `tmp/queue_kv-0.1.5.tar.gz` & `tmp/queue_kv-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_kv-0.1.5.tar", last modified: Thu May  2 10:20:04 2024, max compression
+gzip compressed data, was "queue_kv-0.1.6.tar", last modified: Tue May 14 11:41:34 2024, max compression
```

## Comparing `queue_kv-0.1.5.tar` & `queue_kv-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:20:04.369093 queue_kv-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      971 2024-05-02 10:20:04.369093 queue_kv-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-05-02 10:15:17.000000 queue_kv-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      628 2024-05-02 10:20:01.000000 queue_kv-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 10:20:04.369093 queue_kv-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:20:04.369093 queue_kv-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:20:04.369093 queue_kv-0.1.5/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:20:04.369093 queue_kv-0.1.5/src/q/kv/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-01 09:09:25.000000 queue_kv-0.1.5/src/q/kv/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-05-01 09:09:25.000000 queue_kv-0.1.5/src/q/kv/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2577 2024-05-02 10:05:20.000000 queue_kv-0.1.5/src/q/kv/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      961 2024-05-02 10:10:53.000000 queue_kv-0.1.5/src/q/kv/append.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:20:04.369093 queue_kv-0.1.5/src/queue_kv.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      971 2024-05-02 10:20:04.000000 queue_kv-0.1.5/src/queue_kv.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-05-02 10:20:04.000000 queue_kv-0.1.5/src/queue_kv.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-02 10:20:04.000000 queue_kv-0.1.5/src/queue_kv.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 10:20:04.000000 queue_kv-0.1.5/src/queue_kv.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-02 10:20:04.000000 queue_kv-0.1.5/src/queue_kv.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-14 11:41:34.801378 queue_kv-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      999 2024-05-14 11:41:34.801378 queue_kv-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      487 2024-05-02 10:24:44.000000 queue_kv-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      628 2024-05-14 11:41:30.000000 queue_kv-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-14 11:41:34.801378 queue_kv-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-14 11:41:34.781378 queue_kv-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-14 11:41:34.781378 queue_kv-0.1.6/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-14 11:41:34.791378 queue_kv-0.1.6/src/q/kv/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-01 09:09:25.000000 queue_kv-0.1.6/src/q/kv/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-05-01 09:09:25.000000 queue_kv-0.1.6/src/q/kv/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2605 2024-05-14 11:41:24.000000 queue_kv-0.1.6/src/q/kv/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      961 2024-05-02 10:10:53.000000 queue_kv-0.1.6/src/q/kv/append.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-14 11:41:34.801378 queue_kv-0.1.6/src/queue_kv.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      999 2024-05-14 11:41:34.000000 queue_kv-0.1.6/src/queue_kv.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-05-14 11:41:34.000000 queue_kv-0.1.6/src/queue_kv.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-14 11:41:34.000000 queue_kv-0.1.6/src/queue_kv.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-14 11:41:34.000000 queue_kv-0.1.6/src/queue_kv.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-14 11:41:34.000000 queue_kv-0.1.6/src/queue_kv.egg-info/top_level.txt
```

### Comparing `queue_kv-0.1.5/PKG-INFO` & `queue_kv-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-kv
-Version: 0.1.5
+Version: 0.1.6
 Summary: Queue implementation based on `kv.api`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
@@ -15,16 +15,18 @@
 Provides-Extra: sqlite
 Requires-Dist: kv-sqlite-sync; extra == "sqlite"
 
 # Queue: Key-Value
 
 > Queue implementation based on [`kv.api`](https://pypi.org/project/kv-api/)
 
-```bash
+```python
 pip install queue-kv
+
+from q.kv import QueueKV
 ```
 
 ## Usage
 
 - Use an arbitrary `KV` implementation:
 
 ```python
```

### Comparing `queue_kv-0.1.5/pyproject.toml` & `queue_kv-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-kv"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Queue implementation based on `kv.api`"
 dependencies = [
   "queue-api", "kv-api", "pydantic", "lazy-loader"
 ]
```

### Comparing `queue_kv-0.1.5/src/q/kv/api.py` & `queue_kv-0.1.6/src/q/kv/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing_extensions import AsyncIterable, Generic, Literal, TypeVar, overload
 import asyncio
+import os
 from datetime import timedelta
 from haskellian import either as E, AsyncIter, iter as I, Either, Left, IsLeft, Right
 from kv.api import KV, InexistentItem as KVInexistentItem
 from q.api import Queue, QueueError, ReadError, InexistentItem
 
 A = TypeVar('A')
 B = TypeVar('B')
@@ -27,15 +28,15 @@
   
   @classmethod
   def sqlite(cls, Type: type[B], path: str, table: str = 'queue') -> 'QueueKV[B]':
     try:
       from kv.sqlite import SQLiteKV
     except ImportError:
       raise ImportError('Install `kv-sqlite-sync` to run in local SQLite')
-    if len(path.split('.')) == 1:
+    if len(os.path.basename(path).split('.')) == 1:
       path += '.sqlite'
     return QueueKV(SQLiteKV.validated(Type, path, table))
   
   @classmethod
   @overload
   def at(cls, Type: type[B], path: str, protocol: Literal['fs']) -> 'QueueKV[B]': ...
   @classmethod
```

### Comparing `queue_kv-0.1.5/src/q/kv/append.py` & `queue_kv-0.1.6/src/q/kv/append.py`

 * *Files identical despite different names*

### Comparing `queue_kv-0.1.5/src/queue_kv.egg-info/PKG-INFO` & `queue_kv-0.1.6/src/queue_kv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-kv
-Version: 0.1.5
+Version: 0.1.6
 Summary: Queue implementation based on `kv.api`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
@@ -15,16 +15,18 @@
 Provides-Extra: sqlite
 Requires-Dist: kv-sqlite-sync; extra == "sqlite"
 
 # Queue: Key-Value
 
 > Queue implementation based on [`kv.api`](https://pypi.org/project/kv-api/)
 
-```bash
+```python
 pip install queue-kv
+
+from q.kv import QueueKV
 ```
 
 ## Usage
 
 - Use an arbitrary `KV` implementation:
 
 ```python
```

