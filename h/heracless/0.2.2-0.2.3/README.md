# Comparing `tmp/heracless-0.2.2.tar.gz` & `tmp/heracless-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heracless-0.2.2.tar", last modified: Mon Mar 18 10:13:17 2024, max compression
+gzip compressed data, was "heracless-0.2.3.tar", last modified: Tue May 14 08:19:06 2024, max compression
```

## Comparing `heracless-0.2.2.tar` & `heracless-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-18 10:13:17.981731 heracless-0.2.2/
--rw-rw-r--   0 felix     (1000) felix     (1000)     1066 2024-03-15 13:41:30.000000 heracless-0.2.2/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)     4071 2024-03-18 10:13:17.981731 heracless-0.2.2/PKG-INFO
--rw-rw-r--   0 felix     (1000) felix     (1000)     3373 2024-03-15 16:37:57.000000 heracless-0.2.2/README.md
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-18 10:13:17.977731 heracless-0.2.2/heracless/
--rw-rw-r--   0 felix     (1000) felix     (1000)     1450 2024-03-18 10:06:09.000000 heracless-0.2.2/heracless/__init__.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     2348 2024-03-15 16:24:09.000000 heracless-0.2.2/heracless/cli_tool.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     2021 2024-03-15 16:25:33.000000 heracless-0.2.2/heracless/decorator.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     2125 2024-03-15 13:41:30.000000 heracless-0.2.2/heracless/main.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-18 10:13:17.981731 heracless-0.2.2/heracless/tests/
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-18 10:13:17.981731 heracless-0.2.2/heracless/tests/config/
--rw-rw-r--   0 felix     (1000) felix     (1000)      698 2024-03-15 13:41:30.000000 heracless-0.2.2/heracless/tests/config/types.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      718 2024-03-18 10:09:09.000000 heracless-0.2.2/heracless/tests/conftest.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      983 2024-03-15 13:41:30.000000 heracless-0.2.2/heracless/tests/load.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      466 2024-03-18 10:06:51.000000 heracless-0.2.2/heracless/tests/quick_test.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      956 2024-03-15 14:22:13.000000 heracless-0.2.2/heracless/tests/test_end_to_end.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     1447 2024-03-15 15:46:56.000000 heracless-0.2.2/heracless/tests/test_units.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-18 10:13:17.981731 heracless-0.2.2/heracless/utils/
--rw-rw-r--   0 felix     (1000) felix     (1000)       72 2024-03-15 14:03:31.000000 heracless-0.2.2/heracless/utils/c_types.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     8003 2024-03-18 10:12:19.000000 heracless-0.2.2/heracless/utils/cfg_tree.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      538 2024-03-15 13:41:30.000000 heracless-0.2.2/heracless/utils/exceptions.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     1764 2024-03-15 16:26:15.000000 heracless-0.2.2/heracless/utils/helper.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-18 10:13:17.981731 heracless-0.2.2/heracless.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)     4071 2024-03-18 10:13:17.000000 heracless-0.2.2/heracless.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1000) felix     (1000)      571 2024-03-18 10:13:17.000000 heracless-0.2.2/heracless.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)        1 2024-03-18 10:13:17.000000 heracless-0.2.2/heracless.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)       49 2024-03-18 10:13:17.000000 heracless-0.2.2/heracless.egg-info/requires.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)       10 2024-03-18 10:13:17.000000 heracless-0.2.2/heracless.egg-info/top_level.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)      875 2024-03-18 10:13:11.000000 heracless-0.2.2/pyproject.toml
--rw-rw-r--   0 felix     (1000) felix     (1000)       38 2024-03-18 10:13:17.981731 heracless-0.2.2/setup.cfg
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-14 08:19:06.390042 heracless-0.2.3/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1066 2024-03-15 13:41:30.000000 heracless-0.2.3/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)     4046 2024-05-14 08:19:06.390042 heracless-0.2.3/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)     3373 2024-03-15 16:37:57.000000 heracless-0.2.3/README.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-14 08:19:06.390042 heracless-0.2.3/heracless/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1450 2024-03-18 10:06:09.000000 heracless-0.2.3/heracless/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2348 2024-03-15 16:24:09.000000 heracless-0.2.3/heracless/cli_tool.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2021 2024-03-15 16:25:33.000000 heracless-0.2.3/heracless/decorator.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2125 2024-03-15 13:41:30.000000 heracless-0.2.3/heracless/main.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-14 08:19:06.390042 heracless-0.2.3/heracless/tests/
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-14 08:19:06.390042 heracless-0.2.3/heracless/tests/config/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      698 2024-03-15 13:41:30.000000 heracless-0.2.3/heracless/tests/config/types.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      718 2024-03-18 10:09:09.000000 heracless-0.2.3/heracless/tests/conftest.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      983 2024-03-15 13:41:30.000000 heracless-0.2.3/heracless/tests/load.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      466 2024-03-18 10:06:51.000000 heracless-0.2.3/heracless/tests/quick_test.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      956 2024-03-15 14:22:13.000000 heracless-0.2.3/heracless/tests/test_end_to_end.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1447 2024-03-15 15:46:56.000000 heracless-0.2.3/heracless/tests/test_units.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-14 08:19:06.390042 heracless-0.2.3/heracless/utils/
+-rw-rw-r--   0 felix     (1000) felix     (1000)       72 2024-03-15 14:03:31.000000 heracless-0.2.3/heracless/utils/c_types.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     8003 2024-03-18 10:12:19.000000 heracless-0.2.3/heracless/utils/cfg_tree.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      538 2024-03-15 13:41:30.000000 heracless-0.2.3/heracless/utils/exceptions.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1764 2024-03-15 16:26:15.000000 heracless-0.2.3/heracless/utils/helper.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-14 08:19:06.390042 heracless-0.2.3/heracless.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     4046 2024-05-14 08:19:06.000000 heracless-0.2.3/heracless.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      571 2024-05-14 08:19:06.000000 heracless-0.2.3/heracless.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2024-05-14 08:19:06.000000 heracless-0.2.3/heracless.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       24 2024-05-14 08:19:06.000000 heracless-0.2.3/heracless.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       10 2024-05-14 08:19:06.000000 heracless-0.2.3/heracless.egg-info/top_level.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)      850 2024-05-14 08:17:56.000000 heracless-0.2.3/pyproject.toml
+-rw-rw-r--   0 felix     (1000) felix     (1000)       38 2024-05-14 08:19:06.390042 heracless-0.2.3/setup.cfg
```

### Comparing `heracless-0.2.2/LICENSE` & `heracless-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/PKG-INFO` & `heracless-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: heracless
-Version: 0.2.2
+Version: 0.2.3
 Summary: Yaml to Dataclass parser for Config files
 Author-email: Felix Schelling <felix.schelling@protonmail.com>
 Project-URL: Homepage, https://github.com/felixscode/heracless
 Keywords: YMAL,Dataclass,Config
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: black==23.1.0
-Requires-Dist: pytest==7.2.1
-Requires-Dist: PyYAML==6.0
-Requires-Dist: art==6.1
+Requires-Dist: black
+Requires-Dist: pytest
+Requires-Dist: PyYAML
+Requires-Dist: art
 
 # heracless
 
 Config Manager using yaml.
 
 # Description
```

### Comparing `heracless-0.2.2/README.md` & `heracless-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/__init__.py` & `heracless-0.2.3/heracless/__init__.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/cli_tool.py` & `heracless-0.2.3/heracless/cli_tool.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/decorator.py` & `heracless-0.2.3/heracless/decorator.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/main.py` & `heracless-0.2.3/heracless/main.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/tests/config/types.py` & `heracless-0.2.3/heracless/tests/config/types.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/tests/conftest.py` & `heracless-0.2.3/heracless/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/tests/load.py` & `heracless-0.2.3/heracless/tests/load.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/tests/test_end_to_end.py` & `heracless-0.2.3/heracless/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/tests/test_units.py` & `heracless-0.2.3/heracless/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/utils/cfg_tree.py` & `heracless-0.2.3/heracless/utils/cfg_tree.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/utils/exceptions.py` & `heracless-0.2.3/heracless/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless/utils/helper.py` & `heracless-0.2.3/heracless/utils/helper.py`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/heracless.egg-info/PKG-INFO` & `heracless-0.2.3/heracless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: heracless
-Version: 0.2.2
+Version: 0.2.3
 Summary: Yaml to Dataclass parser for Config files
 Author-email: Felix Schelling <felix.schelling@protonmail.com>
 Project-URL: Homepage, https://github.com/felixscode/heracless
 Keywords: YMAL,Dataclass,Config
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: black==23.1.0
-Requires-Dist: pytest==7.2.1
-Requires-Dist: PyYAML==6.0
-Requires-Dist: art==6.1
+Requires-Dist: black
+Requires-Dist: pytest
+Requires-Dist: PyYAML
+Requires-Dist: art
 
 # heracless
 
 Config Manager using yaml.
 
 # Description
```

### Comparing `heracless-0.2.2/heracless.egg-info/SOURCES.txt` & `heracless-0.2.3/heracless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heracless-0.2.2/pyproject.toml` & `heracless-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 line-length = 120
 target-version = ['py311']
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "heracless"
-version = "0.2.2"
+version = "0.2.3"
 description = "Yaml to Dataclass parser for Config files"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{ name = "Felix Schelling", email = "felix.schelling@protonmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["YMAL", "Dataclass", "Config"]
 dependencies = [
-    "black==23.1.0",
-    "pytest==7.2.1",
-    "PyYAML==6.0",
-    "art==6.1",
+    "black",
+    "pytest",
+    "PyYAML",
+    "art",
 ]
 requires-python = ">=3.10"
 
 [project.urls]
 "Homepage" = "https://github.com/felixscode/heracless"
```

