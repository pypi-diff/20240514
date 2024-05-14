# Comparing `tmp/python3-cyberfusion-common-2.10.11.1.tar.gz` & `tmp/python3-cyberfusion-common-2.10.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-cyberfusion-common-2.10.11.1.tar", last modified: Mon Sep  4 17:37:06 2023, max compression
+gzip compressed data, was "python3-cyberfusion-common-2.10.11.2.tar", last modified: Tue May 14 10:20:41 2024, max compression
```

## Comparing `python3-cyberfusion-common-2.10.11.1.tar` & `python3-cyberfusion-common-2.10.11.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1151 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-09-04 17:32:47.000000 python3-cyberfusion-common-2.10.11.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/Config.py
--rw-rw-rw-   0 root         (0) root         (0)     2237 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/Filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/FilesystemComparison.py
--rw-rw-rw-   0 root         (0) root         (0)     3633 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-09-04 17:16:07.000000 python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/exceptions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-04 17:37:06.168373 python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1151 2023-09-04 17:37:06.000000 python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2023-09-04 17:37:06.000000 python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-04 17:37:06.000000 python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-09-04 17:37:06.000000 python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-09-04 17:37:06.000000 python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2024-03-02 01:14:05.000000 python3-cyberfusion-common-2.10.11.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-03-02 01:14:05.000000 python3-cyberfusion-common-2.10.11.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-03-02 01:14:05.000000 python3-cyberfusion-common-2.10.11.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-14 10:11:03.000000 python3-cyberfusion-common-2.10.11.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2024-05-14 10:19:52.000000 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/Config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2237 2024-03-02 01:14:05.000000 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/Filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2024-03-02 01:14:05.000000 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/FilesystemComparison.py
+-rw-rw-rw-   0 root         (0) root         (0)     3633 2024-03-02 01:14:05.000000 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      171 2024-03-02 01:14:05.000000 python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 10:20:41.888253 python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-14 10:20:41.000000 python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-14 10:20:41.000000 python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 10:20:41.000000 python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-14 10:20:41.000000 python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-14 10:20:41.000000 python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/top_level.txt
```

### Comparing `python3-cyberfusion-common-2.10.11.1/LICENSE` & `python3-cyberfusion-common-2.10.11.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-common-2.10.11.1/PKG-INFO` & `python3-cyberfusion-common-2.10.11.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-cyberfusion-common
-Version: 2.10.11.1
+Version: 2.10.11.2
 Summary: Common utilities.
 Home-page: https://vcs.cyberfusion.nl/shared/python3-cyberfusion-common
 Author: William Edwards
 Author-email: wedwards@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,common
 Platform: linux
@@ -51,9 +51,7 @@
 # Tests
 
 Run tests with pytest:
 
     pytest tests/
 
 The tests must be run from the project root.
-
-
```

### Comparing `python3-cyberfusion-common-2.10.11.1/README.md` & `python3-cyberfusion-common-2.10.11.2/README.md`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-common-2.10.11.1/setup.py` & `python3-cyberfusion-common-2.10.11.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="python3-cyberfusion-common",
-    version="2.10.11.1",
+    version="2.10.11.2",
     description="Common utilities.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.9",
     author="William Edwards",
     author_email="wedwards@cyberfusion.nl",
     url="https://vcs.cyberfusion.nl/shared/python3-cyberfusion-common",
```

### Comparing `python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/Config.py` & `python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/Config.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         return self._path
 
     @cached_property
     def config(self) -> configparser.ConfigParser:
         """Read config."""
         config = configparser.ConfigParser()
 
-        config.read(self.path)
+        with open(self.path, "r") as f:
+            config.read_file(f)
 
         return config
 
     def get(self, section: str, key: str) -> str:
         """Retrieve config option."""
         return self.config.get(section, key)
```

### Comparing `python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/Filesystem.py` & `python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/Filesystem.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/FilesystemComparison.py` & `python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/FilesystemComparison.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-common-2.10.11.1/src/cyberfusion/Common/__init__.py` & `python3-cyberfusion-common-2.10.11.2/src/cyberfusion/Common/__init__.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/PKG-INFO` & `python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-cyberfusion-common
-Version: 2.10.11.1
+Version: 2.10.11.2
 Summary: Common utilities.
 Home-page: https://vcs.cyberfusion.nl/shared/python3-cyberfusion-common
 Author: William Edwards
 Author-email: wedwards@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,common
 Platform: linux
@@ -51,9 +51,7 @@
 # Tests
 
 Run tests with pytest:
 
     pytest tests/
 
 The tests must be run from the project root.
-
-
```

### Comparing `python3-cyberfusion-common-2.10.11.1/src/python3_cyberfusion_common.egg-info/SOURCES.txt` & `python3-cyberfusion-common-2.10.11.2/src/python3_cyberfusion_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

