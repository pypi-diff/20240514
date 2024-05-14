# Comparing `tmp/finml_utils-2.2.1.tar.gz` & `tmp/finml_utils-2.2.2.tar.gz`

## Comparing `finml_utils-2.2.1.tar` & `finml_utils-2.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finml_utils-2.2.1/codecov.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/__init__.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/dataframes.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/enums.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/files.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/introspection.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/list.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/parallel.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/returns.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/s3_store.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/shuffle.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/stats.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 finml_utils-2.2.1/src/finml_utils/transformations.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 finml_utils-2.2.1/.gitignore
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 finml_utils-2.2.1/README.md
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 finml_utils-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 finml_utils-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finml_utils-2.2.2/codecov.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/__init__.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/dataframes.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/enums.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/files.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/introspection.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/list.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/parallel.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/returns.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/s3_store.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/shuffle.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/stats.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 finml_utils-2.2.2/src/finml_utils/transformations.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 finml_utils-2.2.2/.gitignore
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 finml_utils-2.2.2/README.md
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 finml_utils-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 finml_utils-2.2.2/PKG-INFO
```

### Comparing `finml_utils-2.2.1/src/finml_utils/dataframes.py` & `finml_utils-2.2.2/src/finml_utils/dataframes.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/src/finml_utils/list.py` & `finml_utils-2.2.2/src/finml_utils/list.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/src/finml_utils/parallel.py` & `finml_utils-2.2.2/src/finml_utils/parallel.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/src/finml_utils/returns.py` & `finml_utils-2.2.2/src/finml_utils/returns.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def __apply_clip(data: T, clip: float | None) -> T:
     if clip is not None:
         return data.clip(lower=-clip, upper=clip)
     return data
 
 
 def to_log_returns(data: T, clip: float | None) -> T:
-    return __apply_clip(np.log1p(to_returns(data)), clip)
+    return __apply_clip(np.log1p(to_returns(data, clip=None)), clip)
 
 
 def to_returns(data: T, clip: float | None) -> T:
     if isinstance(data, pd.DataFrame):
         return data.apply(to_returns)
     if data.min() < 0:
         return __apply_clip(
```

### Comparing `finml_utils-2.2.1/src/finml_utils/s3_store.py` & `finml_utils-2.2.2/src/finml_utils/s3_store.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/src/finml_utils/shuffle.py` & `finml_utils-2.2.2/src/finml_utils/shuffle.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/src/finml_utils/stats.py` & `finml_utils-2.2.2/src/finml_utils/stats.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/src/finml_utils/transformations.py` & `finml_utils-2.2.2/src/finml_utils/transformations.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/.gitignore` & `finml_utils-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `finml_utils-2.2.1/pyproject.toml` & `finml_utils-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "finml-utils"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -50,15 +50,15 @@
   "pytest~=7.1.2",
   "pytest-cov>=4.0",
 ]
 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "2.2.1"
+current_version = "2.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `finml_utils-2.2.1/PKG-INFO` & `finml_utils-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: finml-utils
-Version: 2.2.1
+Version: 2.2.2
 Project-URL: Issues, https://github.com/dream-faster/finml-utils/issues
 Project-URL: Source, https://github.com/dream-faster/finml-utils
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License-Expression: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

