# Comparing `tmp/proq-0.0.3.tar.gz` & `tmp/proq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proq-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "proq-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `proq-0.0.3.tar` & `proq-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1012 2024-04-13 10:26:32.651677 proq-0.0.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1024 2024-04-13 10:26:32.651677 proq-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3097 2024-04-13 10:26:32.651677 proq-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2024-04-13 10:26:32.651677 proq-0.0.3/LICENSE
--rw-r--r--   0        0        0     1214 2024-04-13 10:26:32.651677 proq-0.0.3/README.md
--rw-r--r--   0        0        0      803 2024-04-13 10:26:32.651677 proq-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       64 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/__init__.py
--rw-r--r--   0        0        0      423 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/collectible.py
--rw-r--r--   0        0        0       62 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/common.py
--rw-r--r--   0        0        0     1682 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/proq.py
--rw-r--r--   0        0        0     1726 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/transform.py
--rw-r--r--   0        0        0     1800 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/transform_parallel.py
--rw-r--r--   0        0        0     3245 2024-04-13 10:26:32.651677 proq-0.0.3/tests/test_proq.py
--rw-r--r--   0        0        0     1142 2024-04-13 10:26:32.651677 proq-0.0.3/tests/test_transform.py
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 proq-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1012 2024-05-14 12:59:42.680688 proq-0.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1024 2024-05-14 12:59:42.680688 proq-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3097 2024-05-14 12:59:42.680688 proq-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2024-05-14 12:59:42.680688 proq-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1214 2024-05-14 12:59:42.680688 proq-0.0.4/README.md
+-rw-r--r--   0        0        0      803 2024-05-14 12:59:42.680688 proq-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-05-14 12:59:42.680688 proq-0.0.4/src/proq/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-14 12:59:42.680688 proq-0.0.4/src/proq/collectible.py
+-rw-r--r--   0        0        0       62 2024-05-14 12:59:42.680688 proq-0.0.4/src/proq/common.py
+-rw-r--r--   0        0        0     1723 2024-05-14 12:59:42.680688 proq-0.0.4/src/proq/proq.py
+-rw-r--r--   0        0        0     1726 2024-05-14 12:59:42.680688 proq-0.0.4/src/proq/transform.py
+-rw-r--r--   0        0        0     1709 2024-05-14 12:59:42.680688 proq-0.0.4/src/proq/transform_parallel.py
+-rw-r--r--   0        0        0     3245 2024-05-14 12:59:42.680688 proq-0.0.4/tests/test_proq.py
+-rw-r--r--   0        0        0     1142 2024-05-14 12:59:42.680688 proq-0.0.4/tests/test_transform.py
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 proq-0.0.4/PKG-INFO
```

### Comparing `proq-0.0.3/.github/workflows/python-package.yml` & `proq-0.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/.github/workflows/python-publish.yml` & `proq-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/.gitignore` & `proq-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/LICENSE` & `proq-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/README.md` & `proq-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/pyproject.toml` & `proq-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/src/proq/proq.py` & `proq-0.0.4/src/proq/proq.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,9 +46,9 @@
         if initial is None:
             return Proq(transform.Reduce(f, self))
         return Proq(transform.ReduceInitial(f, self, initial))
 
     def tee(self, n: int = 2) -> tuple[Proq[T], ...]:
         return tuple(Proq(iterator) for iterator in itertools.tee(self, n))
 
-    def par_map(self, f: Callable[[T], U]) -> Proq[U]:
-        return Proq(transform_parallel.ParallelMap(f, self))
+    def par_map(self, f: Callable[[T], U], max_tasks: int | None = None) -> Proq[U]:
+        return Proq(transform_parallel.ParallelMap(f, self, max_tasks))
```

### Comparing `proq-0.0.3/src/proq/transform.py` & `proq-0.0.4/src/proq/transform.py`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/src/proq/transform_parallel.py` & `proq-0.0.4/src/proq/transform_parallel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from __future__ import annotations
 
 import collections
-import concurrent.futures
+import os
 import pickle
+from concurrent import futures
 from typing import Any, Callable, Generic, Iterable, Iterator
 
 import dill  # type: ignore
 
 from . import collectible
 from .common import T, U
 
 
 class ParallelMap(collectible.Collectible[U]):
-    def __init__(self, f: Callable[[T], U], items: Iterable[T], max_tasks: int = 10):
-        self.f = SerializableCallable(f)
+    def __init__(
+        self, f: Callable[[T], U], items: Iterable[T], parallelism: int | None = None
+    ):
+        self.f: SerializableCallable = SerializableCallable(f)
         self.items = items
-        self.max_tasks = max_tasks
-        self.pool = concurrent.futures.ProcessPoolExecutor(max_workers=max_tasks)
-        self.tasks: collections.deque = collections.deque()
+        self.parallelism = parallelism or os.cpu_count() or 2
         super().__init__(self._get_iterator())
 
     def _get_iterator(self) -> Iterator[U]:
-        for i, item in enumerate(self.items):
-            self.tasks.append(self.pool.submit(self.f, item))
-            # until the queue fills up - submit 2 jobs and fetch 1
-            if i % 2 == 1 or len(self.tasks) >= self.max_tasks and i % 2 == 0:
-                task = self.tasks.popleft()
-                yield task.result()
+        tasks: collections.deque = collections.deque()
+        with futures.ProcessPoolExecutor(max_workers=self.parallelism) as pool:
+            for item in self.items:
+                tasks.append(pool.submit(self.f, item))
+                if len(tasks) > self.parallelism:
+                    yield tasks.popleft().result()
 
-        for task in self.tasks:
-            yield task.result()
-
-        self.pool.shutdown()
+            while tasks:
+                yield tasks.popleft().result()
 
 
 #
 # Serialization functions:
 #
 class SerializableCallable(Generic[T]):
-    def __init__(self, f: Callable[[Any], T]):
+    def __init__(self, f: Callable):
         self.f = self._dumps_if_needed(f)
 
     def __call__(self, *args: Any) -> T:
         return self._loads_if_needed(self.f)(*args)
 
     @staticmethod
     def _dumps_if_needed(obj: Callable) -> Callable | bytes:
```

### Comparing `proq-0.0.3/tests/test_proq.py` & `proq-0.0.4/tests/test_proq.py`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/tests/test_transform.py` & `proq-0.0.4/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `proq-0.0.3/PKG-INFO` & `proq-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proq
-Version: 0.0.3
+Version: 0.0.4
 Summary: Process Queue
 Author-email: Roi Gabay <roigby@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

