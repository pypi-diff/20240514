# Comparing `tmp/idemlib-0.1.5.tar.gz` & `tmp/idemlib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idemlib-0.1.5.tar", last modified: Fri Jul  7 18:52:16 2023, max compression
+gzip compressed data, was "idemlib-0.1.6.tar", last modified: Tue May 14 01:34:57 2024, max compression
```

## Comparing `idemlib-0.1.5.tar` & `idemlib-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leogao     (502) staff       (20)        0 2023-07-07 18:52:16.830124 idemlib-0.1.5/
--rw-r--r--   0 leogao     (502) staff       (20)       23 2023-05-25 22:17:10.000000 idemlib-0.1.5/.gitignore
--rw-r--r--   0 leogao     (502) staff       (20)      173 2023-07-07 18:52:16.829440 idemlib-0.1.5/PKG-INFO
-drwxr-xr-x   0 leogao     (502) staff       (20)        0 2023-07-07 18:52:16.813542 idemlib-0.1.5/idemlib/
--rw-r--r--   0 leogao     (502) staff       (20)    10834 2023-06-30 20:35:32.000000 idemlib-0.1.5/idemlib/__init__.py
--rw-r--r--   0 leogao     (502) staff       (20)    13950 2023-07-07 18:51:33.000000 idemlib-0.1.5/idemlib/hashers.py
-drwxr-xr-x   0 leogao     (502) staff       (20)        0 2023-07-07 18:52:16.826763 idemlib-0.1.5/idemlib.egg-info/
--rw-r--r--   0 leogao     (502) staff       (20)      173 2023-07-07 18:52:15.000000 idemlib-0.1.5/idemlib.egg-info/PKG-INFO
--rw-r--r--   0 leogao     (502) staff       (20)      232 2023-07-07 18:52:16.000000 idemlib-0.1.5/idemlib.egg-info/SOURCES.txt
--rw-r--r--   0 leogao     (502) staff       (20)        1 2023-07-07 18:52:15.000000 idemlib-0.1.5/idemlib.egg-info/dependency_links.txt
--rw-r--r--   0 leogao     (502) staff       (20)        9 2023-07-07 18:52:15.000000 idemlib-0.1.5/idemlib.egg-info/requires.txt
--rw-r--r--   0 leogao     (502) staff       (20)        8 2023-07-07 18:52:15.000000 idemlib-0.1.5/idemlib.egg-info/top_level.txt
--rw-r--r--   0 leogao     (502) staff       (20)       38 2023-07-07 18:52:16.830338 idemlib-0.1.5/setup.cfg
--rw-r--r--   0 leogao     (502) staff       (20)      358 2023-07-07 18:50:59.000000 idemlib-0.1.5/setup.py
-drwxr-xr-x   0 leogao     (502) staff       (20)        0 2023-07-07 18:52:16.827973 idemlib-0.1.5/tests/
--rw-r--r--   0 leogao     (502) staff       (20)     3677 2023-06-14 20:28:42.000000 idemlib-0.1.5/tests/test_cache.py
+drwxr-xr-x   0 leogao     (502) staff       (20)        0 2024-05-14 01:34:57.781713 idemlib-0.1.6/
+-rw-r--r--   0 leogao     (502) staff       (20)       23 2023-05-25 22:17:10.000000 idemlib-0.1.6/.gitignore
+-rw-r--r--   0 leogao     (502) staff       (20)      197 2024-05-14 01:34:57.779395 idemlib-0.1.6/PKG-INFO
+drwxr-xr-x   0 leogao     (502) staff       (20)        0 2024-05-14 01:34:57.740962 idemlib-0.1.6/idemlib/
+-rw-r--r--   0 leogao     (502) staff       (20)    13083 2024-05-14 01:32:19.000000 idemlib-0.1.6/idemlib/__init__.py
+-rw-r--r--   0 leogao     (502) staff       (20)    13950 2023-07-07 18:51:33.000000 idemlib-0.1.6/idemlib/hashers.py
+drwxr-xr-x   0 leogao     (502) staff       (20)        0 2024-05-14 01:34:57.776648 idemlib-0.1.6/idemlib.egg-info/
+-rw-r--r--   0 leogao     (502) staff       (20)      197 2024-05-14 01:34:57.000000 idemlib-0.1.6/idemlib.egg-info/PKG-INFO
+-rw-r--r--   0 leogao     (502) staff       (20)      232 2024-05-14 01:34:57.000000 idemlib-0.1.6/idemlib.egg-info/SOURCES.txt
+-rw-r--r--   0 leogao     (502) staff       (20)        1 2024-05-14 01:34:57.000000 idemlib-0.1.6/idemlib.egg-info/dependency_links.txt
+-rw-r--r--   0 leogao     (502) staff       (20)        9 2024-05-14 01:34:57.000000 idemlib-0.1.6/idemlib.egg-info/requires.txt
+-rw-r--r--   0 leogao     (502) staff       (20)        8 2024-05-14 01:34:57.000000 idemlib-0.1.6/idemlib.egg-info/top_level.txt
+-rw-r--r--   0 leogao     (502) staff       (20)       38 2024-05-14 01:34:57.781977 idemlib-0.1.6/setup.cfg
+-rw-r--r--   0 leogao     (502) staff       (20)      358 2024-05-14 01:32:26.000000 idemlib-0.1.6/setup.py
+drwxr-xr-x   0 leogao     (502) staff       (20)        0 2024-05-14 01:34:57.774459 idemlib-0.1.6/tests/
+-rw-r--r--   0 leogao     (502) staff       (20)     3677 2023-06-14 20:28:42.000000 idemlib-0.1.6/tests/test_cache.py
```

### Comparing `idemlib-0.1.5/idemlib/__init__.py` & `idemlib-0.1.6/idemlib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import idemlib.hashers as hashers
 
 T = TypeVar("T")
 
 # either callable or coroutine
 F = TypeVar("F", Callable[..., Any], Coroutine[Any, Any, Any], Awaitable[Any])
 
-# TODO: hierarchical cache
+
 class CacheHelper:
     """
     CacheHelper helps cache the return values of function calls based on their
     arguments. It is useful for caching the results of expensive computations
     or API calls.
 
     CacheHelper hashes the arguments to a function and the cache key defined in
@@ -28,39 +28,73 @@
     function without invalidating the cache. When the implementation of the
     function changes in ways that affect the output, the user is responsible for
     changing the cache key.
 
     By convention, the cache key is a random hex string, with a version number
     at the end (such as "976d37ab_0"). This is to avoid collisions and ensure
     that old names are not left in strings, causing confusion. The version
-    number makes it easy to invalidate the cache.
+    number makes it easy to invalidate the cache. This is just a convention and
+    there is no special handling of the version number.
 
     CacheHelper should "just work" for async functions.
 
     For custom classes, CacheHelper will error by default to be safe -- to add
     support for custom classes, add a function to `special_hashing` that takes
     the object and returns a hashable object. If the custom class has attributes
     that could themselves not be hashable, the function should recursively call
     `cache._prepare_for_hash` on those attributes.
 
-    Usage:
+    Basic usage:
 
     ```
     cache = CacheHelper("az://my/container")
 
     @cache("976d37ab_0")
     def myfunc(x, y):
         print("running myfunc")
         return x + y
 
 
     myfunc(1, 2) # prints "running myfunc" and returns 3
     myfunc(1, 2) # prints nothing and returns 3
     myfunc(1, 2, cache_version=1) # prints "running myfunc" and returns 3
     ```
+
+    Some notes:
+    - It’s good practice to make sure your function is deterministic (or if 
+    full determinism is unachievable, for different possible return values to be 
+    interchangeable downstream), and not to rely on the caching for determinism.
+    For example, if your function splits a dataset into train and test, you should
+    seed the random number generator.
+    - If working on multiple branches, bumping the version number may lead to
+    collisions between branches. In such cases, a convention is to also include
+    the branch name or some other identifier in the cache key. For example, 
+    `976d37ab_2` can be bumped to `976d37ab_2_myfeature_0` and then
+    `976d37ab_2_myfeature_1`. Then, after `myfeature` is merged to master, if
+    the version needs to be bumped again, it can be bumped to `976d37ab_3`.
+
+    Some rough edges:
+    - Currently, args and kwargs get hashed separately. Therefore, if you have
+    a function `f(x)` and you call with `f(1)` and `f(x=1)`, the hash will
+    be different and will result in two cache entries. This is planned to be
+    fixed in the future.
+    - The return value is saved as a pickle. This inherits all the limitations
+    of pickle, including that some objects cannot be pickled, and that if
+    classes change or are renamed, the pickle may not be loadable. In the
+    future, we plan to add support for other serialization formats.
+    - If two calls with the same cache key and arguments run in parallel,
+    rather than locking the cache, the function will be run twice, and the
+    second call will overwrite the first. The plan is to add a locking mechanism
+    in the future.
+    - The cache is not automatically invalidated when the function implementation
+    changes. Therefore, if you modify the function substantively without changing 
+    the cache key, (1) your function will continue to return the old value, and
+    (2) if you call the function with new arguments, it will run the new version
+    of the function and cache the result under the same key. Automatic invalidation 
+    is semantically ambiguous, so it is not possible to fix this problem in generality.
     """
 
     def __init__(self, save_location: Optional[str], object_hasher=None):
         if save_location is None:
             self.save_location = None
             # memory
             self._cache = {}
@@ -75,15 +109,15 @@
 
     def _get_kv(self, key: str):
         if self.save_location is None:
             return self._cache[key]
 
         try:
             return pickle.load(bf.BlobFile(self.save_location + "/" + key, "rb"))
-        except (FileNotFoundError, EOFError):
+        except (FileNotFoundError, EOFError, pickle.UnpicklingError):
             raise KeyError(key)
 
     def _set_kv(self, key: str, value):
         if self.save_location is None:
             self._cache[key] = value
             return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idemlib-0.1.5/idemlib/hashers.py` & `idemlib-0.1.6/idemlib/hashers.py`

 * *Files identical despite different names*

### Comparing `idemlib-0.1.5/tests/test_cache.py` & `idemlib-0.1.6/tests/test_cache.py`

 * *Files identical despite different names*

