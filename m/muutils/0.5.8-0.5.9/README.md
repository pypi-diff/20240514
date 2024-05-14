# Comparing `tmp/muutils-0.5.8.tar.gz` & `tmp/muutils-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muutils-0.5.8.tar", max compression
+gzip compressed data, was "muutils-0.5.9.tar", max compression
```

## Comparing `muutils-0.5.8.tar` & `muutils-0.5.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.5.8/LICENSE
--rw-r--r--   0        0        0        0 2023-09-04 07:57:55.210230 muutils-0.5.8/muutils/__init__.py
--rw-r--r--   0        0        0     4014 2023-06-14 07:24:44.650510 muutils-0.5.8/muutils/_wip/dataclass_validator.py
--rw-r--r--   0        0        0     4955 2024-02-15 08:20:16.828002 muutils-0.5.8/muutils/_wip/experiments.ipynb
--rw-r--r--   0        0        0     5834 2023-06-14 07:24:44.650510 muutils-0.5.8/muutils/_wip/gptdataset.py
--rw-r--r--   0        0        0    23255 2023-06-14 07:24:44.650510 muutils-0.5.8/muutils/_wip/json_serialize_old.py
--rw-r--r--   0        0        0     3281 2023-06-14 07:24:44.656519 muutils-0.5.8/muutils/_wip/lazy_externals.py
--rw-r--r--   0        0        0    10195 2023-06-14 07:24:44.656731 muutils-0.5.8/muutils/_wip/newargparser.py
--rw-r--r--   0        0        0     7415 2023-06-14 07:24:44.657732 muutils-0.5.8/muutils/_wip/torch_util_old.py
--rw-r--r--   0        0        0     8198 2024-02-15 07:41:47.478998 muutils-0.5.8/muutils/_wip/training_progress.py
--rw-r--r--   0        0        0    15724 2024-02-16 06:58:59.633973 muutils-0.5.8/muutils/dictmagic.py
--rw-r--r--   0        0        0     1950 2023-06-14 07:24:44.658733 muutils-0.5.8/muutils/group_equiv.py
--rw-r--r--   0        0        0      620 2023-07-17 04:40:48.621935 muutils-0.5.8/muutils/json_serialize/__init__.py
--rw-r--r--   0        0        0     6280 2024-01-29 20:08:47.419787 muutils-0.5.8/muutils/json_serialize/array.py
--rw-r--r--   0        0        0    11110 2024-02-15 07:41:47.353963 muutils-0.5.8/muutils/json_serialize/dataclass_factories.py
--rw-r--r--   0        0        0     9426 2024-02-23 22:05:45.594141 muutils-0.5.8/muutils/json_serialize/json_serialize.py
--rw-r--r--   0        0        0    16935 2024-01-29 20:08:47.566819 muutils-0.5.8/muutils/json_serialize/serializable_dataclass.py
--rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.5.8/muutils/json_serialize/util.py
--rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.5.8/muutils/jsonlines.py
--rw-r--r--   0        0        0     1225 2023-07-15 22:26:31.994739 muutils-0.5.8/muutils/kappa.py
--rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.5.8/muutils/logger/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.5.8/muutils/logger/exception_context.py
--rw-r--r--   0        0        0     1659 2024-02-15 07:41:47.251891 muutils-0.5.8/muutils/logger/headerfuncs.py
--rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.5.8/muutils/logger/log_util.py
--rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.5.8/muutils/logger/logger.py
--rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.5.8/muutils/logger/loggingstream.py
--rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.5.8/muutils/logger/simplelogger.py
--rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.5.8/muutils/logger/timing.py
--rw-r--r--   0        0        0     3337 2023-09-04 20:37:29.057158 muutils-0.5.8/muutils/misc.py
--rw-r--r--   0        0        0     4689 2023-12-05 08:52:36.674286 muutils-0.5.8/muutils/mlutils.py
--rw-r--r--   0        0        0       57 2024-02-23 22:06:26.579631 muutils-0.5.8/muutils/nbutils/__init__.py
--rw-r--r--   0        0        0     8233 2024-02-15 07:03:31.158334 muutils-0.5.8/muutils/nbutils/configure_notebook.py
--rw-r--r--   0        0        0    12697 2024-02-15 07:41:47.593001 muutils-0.5.8/muutils/nbutils/convert_ipynb_to_script.py
--rw-r--r--   0        0        0      500 2024-02-23 22:05:45.447024 muutils-0.5.8/muutils/nbutils/mermaid.py
--rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.5.8/muutils/nbutils/print_tex.py
--rw-r--r--   0        0        0     3896 2024-02-15 07:41:47.438999 muutils-0.5.8/muutils/nbutils/run_notebook_tests.py
--rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.5.8/muutils/py.typed
--rw-r--r--   0        0        0     6513 2023-07-22 03:22:18.640525 muutils-0.5.8/muutils/statcounter.py
--rw-r--r--   0        0        0     6376 2023-06-14 07:24:44.661730 muutils-0.5.8/muutils/sysinfo.py
--rw-r--r--   0        0        0    13111 2023-10-04 05:28:48.563912 muutils-0.5.8/muutils/tensor_utils.py
--rw-r--r--   0        0        0     1611 2024-02-23 22:05:10.038801 muutils-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3341 2023-08-29 21:00:08.608852 muutils-0.5.8/README.md
--rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 muutils-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.5.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-09-04 07:57:55.210230 muutils-0.5.9/muutils/__init__.py
+-rw-r--r--   0        0        0     4014 2023-06-14 07:24:44.650510 muutils-0.5.9/muutils/_wip/dataclass_validator.py
+-rw-r--r--   0        0        0     4955 2024-02-15 08:20:16.828002 muutils-0.5.9/muutils/_wip/experiments.ipynb
+-rw-r--r--   0        0        0     5834 2023-06-14 07:24:44.650510 muutils-0.5.9/muutils/_wip/gptdataset.py
+-rw-r--r--   0        0        0    23255 2023-06-14 07:24:44.650510 muutils-0.5.9/muutils/_wip/json_serialize_old.py
+-rw-r--r--   0        0        0     3281 2023-06-14 07:24:44.656519 muutils-0.5.9/muutils/_wip/lazy_externals.py
+-rw-r--r--   0        0        0    10195 2023-06-14 07:24:44.656731 muutils-0.5.9/muutils/_wip/newargparser.py
+-rw-r--r--   0        0        0     7415 2023-06-14 07:24:44.657732 muutils-0.5.9/muutils/_wip/torch_util_old.py
+-rw-r--r--   0        0        0     8198 2024-02-15 07:41:47.478998 muutils-0.5.9/muutils/_wip/training_progress.py
+-rw-r--r--   0        0        0    16735 2024-05-14 02:45:54.939597 muutils-0.5.9/muutils/dictmagic.py
+-rw-r--r--   0        0        0     1950 2023-06-14 07:24:44.658733 muutils-0.5.9/muutils/group_equiv.py
+-rw-r--r--   0        0        0      620 2023-07-17 04:40:48.621935 muutils-0.5.9/muutils/json_serialize/__init__.py
+-rw-r--r--   0        0        0     6280 2024-01-29 20:08:47.419787 muutils-0.5.9/muutils/json_serialize/array.py
+-rw-r--r--   0        0        0    11110 2024-02-15 07:41:47.353963 muutils-0.5.9/muutils/json_serialize/dataclass_factories.py
+-rw-r--r--   0        0        0     9426 2024-02-23 22:05:45.594141 muutils-0.5.9/muutils/json_serialize/json_serialize.py
+-rw-r--r--   0        0        0    16935 2024-01-29 20:08:47.566819 muutils-0.5.9/muutils/json_serialize/serializable_dataclass.py
+-rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.5.9/muutils/json_serialize/util.py
+-rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.5.9/muutils/jsonlines.py
+-rw-r--r--   0        0        0     1225 2023-07-15 22:26:31.994739 muutils-0.5.9/muutils/kappa.py
+-rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.5.9/muutils/logger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.5.9/muutils/logger/exception_context.py
+-rw-r--r--   0        0        0     1659 2024-02-15 07:41:47.251891 muutils-0.5.9/muutils/logger/headerfuncs.py
+-rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.5.9/muutils/logger/log_util.py
+-rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.5.9/muutils/logger/logger.py
+-rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.5.9/muutils/logger/loggingstream.py
+-rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.5.9/muutils/logger/simplelogger.py
+-rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.5.9/muutils/logger/timing.py
+-rw-r--r--   0        0        0     3337 2024-03-02 05:45:04.437857 muutils-0.5.9/muutils/misc.py
+-rw-r--r--   0        0        0     4689 2023-12-05 08:52:36.674286 muutils-0.5.9/muutils/mlutils.py
+-rw-r--r--   0        0        0       57 2024-02-23 22:06:26.579631 muutils-0.5.9/muutils/nbutils/__init__.py
+-rw-r--r--   0        0        0     8233 2024-02-15 07:03:31.158334 muutils-0.5.9/muutils/nbutils/configure_notebook.py
+-rw-r--r--   0        0        0    12697 2024-02-15 07:41:47.593001 muutils-0.5.9/muutils/nbutils/convert_ipynb_to_script.py
+-rw-r--r--   0        0        0      500 2024-02-23 22:05:45.447024 muutils-0.5.9/muutils/nbutils/mermaid.py
+-rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.5.9/muutils/nbutils/print_tex.py
+-rw-r--r--   0        0        0     3896 2024-02-15 07:41:47.438999 muutils-0.5.9/muutils/nbutils/run_notebook_tests.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.5.9/muutils/py.typed
+-rw-r--r--   0        0        0     6513 2023-07-22 03:22:18.640525 muutils-0.5.9/muutils/statcounter.py
+-rw-r--r--   0        0        0     6376 2023-06-14 07:24:44.661730 muutils-0.5.9/muutils/sysinfo.py
+-rw-r--r--   0        0        0    13111 2023-10-04 05:28:48.563912 muutils-0.5.9/muutils/tensor_utils.py
+-rw-r--r--   0        0        0     1611 2024-05-14 02:51:32.043871 muutils-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3341 2023-08-29 21:00:08.608852 muutils-0.5.9/README.md
+-rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 muutils-0.5.9/PKG-INFO
```

### Comparing `muutils-0.5.8/LICENSE` & `muutils-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/dataclass_validator.py` & `muutils-0.5.9/muutils/_wip/dataclass_validator.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/experiments.ipynb` & `muutils-0.5.9/muutils/_wip/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/gptdataset.py` & `muutils-0.5.9/muutils/_wip/gptdataset.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/json_serialize_old.py` & `muutils-0.5.9/muutils/_wip/json_serialize_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/lazy_externals.py` & `muutils-0.5.9/muutils/_wip/lazy_externals.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/newargparser.py` & `muutils-0.5.9/muutils/_wip/newargparser.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/torch_util_old.py` & `muutils-0.5.9/muutils/_wip/torch_util_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/_wip/training_progress.py` & `muutils-0.5.9/muutils/_wip/training_progress.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/dictmagic.py` & `muutils-0.5.9/muutils/dictmagic.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,47 @@
         # iterate over the keys except the last one
         for sub_key in keys[:-1]:
             current = current[sub_key]
         current[keys[-1]] = value
     return defaultdict_to_dict_recursive(nested_dict)
 
 
+def nested_dict_to_dotlist(
+    nested_dict: dict[str, Any],
+    sep: str = ".",
+    allow_lists: bool = False,
+) -> dict[str, Any]:
+    def _recurse(current: Any, parent_key: str = "") -> dict[str, Any]:
+        items: dict = dict()
+
+        new_key: str
+        if isinstance(current, dict):
+            # dict case
+            if not current and parent_key:
+                items[parent_key] = current
+            else:
+                for k, v in current.items():
+                    new_key = f"{parent_key}{sep}{k}" if parent_key else k
+                    items.update(_recurse(v, new_key))
+
+        elif allow_lists and isinstance(current, list):
+            # list case
+            for i, item in enumerate(current):
+                new_key = f"{parent_key}{sep}{i}" if parent_key else str(i)
+                items.update(_recurse(item, new_key))
+
+        else:
+            # anything else (write value)
+            items[parent_key] = current
+
+        return items
+
+    return _recurse(nested_dict)
+
+
 def update_with_nested_dict(
     original: dict[str, Any],
     update: dict[str, Any],
 ) -> dict[str, Any]:
     """Update a dict with a nested dict
 
     Example:
```

### Comparing `muutils-0.5.8/muutils/group_equiv.py` & `muutils-0.5.9/muutils/group_equiv.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/json_serialize/__init__.py` & `muutils-0.5.9/muutils/json_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/json_serialize/array.py` & `muutils-0.5.9/muutils/json_serialize/array.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/json_serialize/dataclass_factories.py` & `muutils-0.5.9/muutils/json_serialize/dataclass_factories.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/json_serialize/json_serialize.py` & `muutils-0.5.9/muutils/json_serialize/json_serialize.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/json_serialize/serializable_dataclass.py` & `muutils-0.5.9/muutils/json_serialize/serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/json_serialize/util.py` & `muutils-0.5.9/muutils/json_serialize/util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/jsonlines.py` & `muutils-0.5.9/muutils/jsonlines.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/kappa.py` & `muutils-0.5.9/muutils/kappa.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/logger/exception_context.py` & `muutils-0.5.9/muutils/logger/exception_context.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/logger/headerfuncs.py` & `muutils-0.5.9/muutils/logger/headerfuncs.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/logger/log_util.py` & `muutils-0.5.9/muutils/logger/log_util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/logger/logger.py` & `muutils-0.5.9/muutils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/logger/loggingstream.py` & `muutils-0.5.9/muutils/logger/loggingstream.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/logger/simplelogger.py` & `muutils-0.5.9/muutils/logger/simplelogger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/logger/timing.py` & `muutils-0.5.9/muutils/logger/timing.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/misc.py` & `muutils-0.5.9/muutils/misc.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/mlutils.py` & `muutils-0.5.9/muutils/mlutils.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/nbutils/configure_notebook.py` & `muutils-0.5.9/muutils/nbutils/configure_notebook.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/nbutils/convert_ipynb_to_script.py` & `muutils-0.5.9/muutils/nbutils/convert_ipynb_to_script.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/nbutils/run_notebook_tests.py` & `muutils-0.5.9/muutils/nbutils/run_notebook_tests.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/statcounter.py` & `muutils-0.5.9/muutils/statcounter.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/sysinfo.py` & `muutils-0.5.9/muutils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/muutils/tensor_utils.py` & `muutils-0.5.9/muutils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/pyproject.toml` & `muutils-0.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muutils"
-version = "0.5.8"
+version = "0.5.9"
 description = "A collection of miscellaneous python utilities"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `muutils-0.5.8/README.md` & `muutils-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `muutils-0.5.8/PKG-INFO` & `muutils-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muutils
-Version: 0.5.8
+Version: 0.5.9
 Summary: A collection of miscellaneous python utilities
 Home-page: https://github.com/mivanit/muutils
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

