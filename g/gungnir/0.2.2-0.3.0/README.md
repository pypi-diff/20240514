# Comparing `tmp/gungnir-0.2.2.tar.gz` & `tmp/gungnir-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gungnir-0.2.2.tar", last modified: Mon Jul 31 20:21:34 2023, max compression
+gzip compressed data, was "gungnir-0.3.0.tar", last modified: Tue May 14 09:05:15 2024, max compression
```

## Comparing `gungnir-0.2.2.tar` & `gungnir-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.709061 gungnir-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 20:21:06.000000 gungnir-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-31 20:21:34.709061 gungnir-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-31 20:21:06.000000 gungnir-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.705062 gungnir-0.2.2/gungnir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.705062 gungnir-0.2.2/gungnir/dependencytrack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:06.000000 gungnir-0.2.2/gungnir/dependencytrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-31 20:21:06.000000 gungnir-0.2.2/gungnir/dependencytrack/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-31 20:21:06.000000 gungnir-0.2.2/gungnir/dependencytrack/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.709061 gungnir-0.2.2/gungnir/gungnir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-31 20:21:06.000000 gungnir-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:21:34.709061 gungnir-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.709061 gungnir-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 20:21:06.000000 gungnir-0.2.2/tests/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:05:15.951288 gungnir-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 09:04:49.000000 gungnir-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-14 09:05:15.951288 gungnir-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 09:04:49.000000 gungnir-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:05:15.947288 gungnir-0.3.0/gungnir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:05:15.947288 gungnir-0.3.0/gungnir/dependencytrack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:04:49.000000 gungnir-0.3.0/gungnir/dependencytrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-14 09:04:49.000000 gungnir-0.3.0/gungnir/dependencytrack/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-14 09:04:49.000000 gungnir-0.3.0/gungnir/dependencytrack/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:05:15.947288 gungnir-0.3.0/gungnir/gungnir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-14 09:05:15.000000 gungnir-0.3.0/gungnir/gungnir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 09:05:15.000000 gungnir-0.3.0/gungnir/gungnir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:05:15.000000 gungnir-0.3.0/gungnir/gungnir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 09:05:15.000000 gungnir-0.3.0/gungnir/gungnir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 09:05:15.000000 gungnir-0.3.0/gungnir/gungnir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 09:04:49.000000 gungnir-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:05:15.951288 gungnir-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:05:15.947288 gungnir-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 09:04:49.000000 gungnir-0.3.0/tests/test_project.py
```

### Comparing `gungnir-0.2.2/LICENSE` & `gungnir-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gungnir-0.2.2/PKG-INFO` & `gungnir-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: gungnir
-Version: 0.2.2
+Version: 0.3.0
 Summary: Homelab Automation Bot to Guard your very own Asgard
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/gungnir
 Project-URL: Bug Tracker, https://github.com/GeekMasher/gungnir/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: docker==7.0.0
+Requires-Dist: idna==3.7
+Requires-Dist: packaging==24.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: urllib3==2.2.1
+Requires-Dist: websocket-client==1.8.0
 
 # gungnir
 
 <div align="center">
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GeekMasher/gungnir)
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/geekmasher/gungnir/python-package.yml?style=for-the-badge)](https://github.com/GeekMasher/gungnir/actions/workflows/python-package.yml?query=branch%3Amain)
```

### Comparing `gungnir-0.2.2/README.md` & `gungnir-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gungnir-0.2.2/gungnir/dependencytrack/api.py` & `gungnir-0.3.0/gungnir/dependencytrack/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dependency Track module."""
+
 import logging
 from typing import Dict, List
 from requests import Session, Response
 
 
 logger = logging.getLogger("gungnir.dependencytrack")
```

### Comparing `gungnir-0.2.2/gungnir/dependencytrack/project.py` & `gungnir-0.3.0/gungnir/dependencytrack/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dependency Track Project."""
+
 import json
 import base64
 import logging
 
 from gungnir.dependencytrack.api import DependencyTrack, checkResponse
 from gungnir.project import Container, OperatingSystem
```

### Comparing `gungnir-0.2.2/gungnir/gungnir.egg-info/PKG-INFO` & `gungnir-0.3.0/gungnir/gungnir.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: gungnir
-Version: 0.2.2
+Version: 0.3.0
 Summary: Homelab Automation Bot to Guard your very own Asgard
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/gungnir
 Project-URL: Bug Tracker, https://github.com/GeekMasher/gungnir/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: docker==7.0.0
+Requires-Dist: idna==3.7
+Requires-Dist: packaging==24.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: urllib3==2.2.1
+Requires-Dist: websocket-client==1.8.0
 
 # gungnir
 
 <div align="center">
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GeekMasher/gungnir)
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/geekmasher/gungnir/python-package.yml?style=for-the-badge)](https://github.com/GeekMasher/gungnir/actions/workflows/python-package.yml?query=branch%3Amain)
```

### Comparing `gungnir-0.2.2/pyproject.toml` & `gungnir-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [project]
 name = "gungnir"
-version = "0.2.2"
+version = "0.3.0"
 authors = [{ name = "GeekMasher" }]
 description = "Homelab Automation Bot to Guard your very own Asgard"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "certifi==2023.7.22",
-    "charset-normalizer==3.2.0",
-    "docker==6.1.3",
-    "idna==3.4",
-    "packaging==23.1",
+    "certifi==2024.2.2",
+    "charset-normalizer==3.3.2",
+    "docker==7.0.0",
+    "idna==3.7",
+    "packaging==24.0",
     "requests==2.31.0",
-    "urllib3==2.0.4",
-    "websocket-client==1.6.1",
+    "urllib3==2.2.1",
+    "websocket-client==1.8.0",
 ]
 
 [tool.setuptools.packages.find]
 where = ["gungnir"]
 
 [project.urls]
 "Homepage" = "https://github.com/GeekMasher/gungnir"
```

