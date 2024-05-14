# Comparing `tmp/gr1336_toolbox-0.1.0.tar.gz` & `tmp/gr1336_toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gr1336_toolbox-0.1.0.tar", last modified: Sun May  5 01:14:30 2024, max compression
+gzip compressed data, was "gr1336_toolbox-0.1.1.tar", last modified: Tue May 14 01:50:01 2024, max compression
```

## Comparing `gr1336_toolbox-0.1.0.tar` & `gr1336_toolbox-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:14:30.670767 gr1336_toolbox-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-05 01:14:30.670767 gr1336_toolbox-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:14:30.670767 gr1336_toolbox-0.1.0/gr1336_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/misc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/txt_split_fnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/gr1336_toolbox/types_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:14:30.670767 gr1336_toolbox-0.1.0/gr1336_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-05 01:14:30.000000 gr1336_toolbox-0.1.0/gr1336_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-05 01:14:30.000000 gr1336_toolbox-0.1.0/gr1336_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 01:14:30.000000 gr1336_toolbox-0.1.0/gr1336_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 01:14:30.000000 gr1336_toolbox-0.1.0/gr1336_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 01:14:30.000000 gr1336_toolbox-0.1.0/gr1336_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 01:14:30.670767 gr1336_toolbox-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-05 01:14:24.000000 gr1336_toolbox-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:50:01.226949 gr1336_toolbox-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-14 01:50:01.226949 gr1336_toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:50:01.226949 gr1336_toolbox-0.1.1/gr1336_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/gr1336_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/gr1336_toolbox/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/gr1336_toolbox/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/gr1336_toolbox/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/gr1336_toolbox/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/gr1336_toolbox/txt_split_fnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/gr1336_toolbox/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:50:01.226949 gr1336_toolbox-0.1.1/gr1336_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-14 01:50:01.000000 gr1336_toolbox-0.1.1/gr1336_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-14 01:50:01.000000 gr1336_toolbox-0.1.1/gr1336_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:50:01.000000 gr1336_toolbox-0.1.1/gr1336_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 01:50:01.000000 gr1336_toolbox-0.1.1/gr1336_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:50:01.000000 gr1336_toolbox-0.1.1/gr1336_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:50:01.226949 gr1336_toolbox-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-14 01:49:57.000000 gr1336_toolbox-0.1.1/setup.py
```

### Comparing `gr1336_toolbox-0.1.0/LICENSE` & `gr1336_toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.1.0/PKG-INFO` & `gr1336_toolbox-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License: MIT License (MIT)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `gr1336_toolbox-0.1.0/gr1336_toolbox/file_manager.py` & `gr1336_toolbox-0.1.1/gr1336_toolbox/file_manager.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.1.0/gr1336_toolbox/files.py` & `gr1336_toolbox-0.1.1/gr1336_toolbox/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,16 +123,16 @@
     unsafe_loader=False,
 ) -> None | list[Any] | dict[Any, Any]:
     """Load YAML content from a file."""
     if not _path(path):
         return None
     with open(path, "r", encoding=encoding) as file:
         if not unsafe_loader:
-            return yaml.safe_load(file, Loader=yaml.FullLoader)
-        return yaml.unsafe_load(file, Loader=yaml.FullLoader)
+            return yaml.safe_load(file)
+        return yaml.unsafe_load(file)
 
 
 def save_yaml(
     path: Path | str,
     content: list | tuple | dict,
     encoding: str = "utf-8",
     safe_dump: bool = False,
```

### Comparing `gr1336_toolbox-0.1.0/gr1336_toolbox/misc.py` & `gr1336_toolbox-0.1.1/gr1336_toolbox/misc.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.1.0/gr1336_toolbox/text.py` & `gr1336_toolbox-0.1.1/gr1336_toolbox/text.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.1.0/gr1336_toolbox/txt_split_fnc.py` & `gr1336_toolbox-0.1.1/gr1336_toolbox/txt_split_fnc.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.1.0/gr1336_toolbox/types.py` & `gr1336_toolbox-0.1.1/gr1336_toolbox/types.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.1.0/gr1336_toolbox.egg-info/PKG-INFO` & `gr1336_toolbox-0.1.1/gr1336_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License: MIT License (MIT)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `gr1336_toolbox-0.1.0/setup.py` & `gr1336_toolbox-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    version="0.1.0",
+    version="0.1.1",
     name="gr1336_toolbox",
     description="Personal collection of reusable tools in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gr1336/gr1336_toolbox/",
     install_requires=[
         "markdownify==0.12.1",
```

