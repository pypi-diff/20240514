# Comparing `tmp/yen-0.4.2.tar.gz` & `tmp/yen-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yen-0.4.2.tar", last modified: Wed May  8 21:41:19 2024, max compression
+gzip compressed data, was "yen-0.4.3.tar", last modified: Tue May 14 17:44:31 2024, max compression
```

## Comparing `yen-0.4.2.tar` & `yen-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.213081 yen-0.4.2/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-03-30 13:10:26.000000 yen-0.4.2/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2670 2024-05-08 21:41:19.213015 yen-0.4.2/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1533 2024-03-30 13:10:26.000000 yen-0.4.2/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1246 2024-05-08 21:41:19.213396 yen-0.4.2/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-03-30 13:10:26.000000 yen-0.4.2/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.207470 yen-0.4.2/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.211322 yen-0.4.2/src/yen/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3325 2024-05-08 21:39:24.000000 yen-0.4.2/src/yen/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      120 2024-03-30 13:10:26.000000 yen-0.4.2/src/yen/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1317 2024-05-08 21:39:29.000000 yen-0.4.2/src/yen/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1748 2024-05-08 21:39:33.000000 yen-0.4.2/src/yen/downloader.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)  1047789 2024-03-30 13:10:26.000000 yen-0.4.2/src/yen/fallback_release_data.json
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3848 2024-05-08 21:39:38.000000 yen-0.4.2/src/yen/github.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-03-30 13:10:26.000000 yen-0.4.2/src/yen/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.212508 yen-0.4.2/src/yen.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2670 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      371 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       36 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       73 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        4 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 17:44:31.564725 yen-0.4.3/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-03-30 13:10:26.000000 yen-0.4.3/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2670 2024-05-14 17:44:31.564658 yen-0.4.3/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1533 2024-03-30 13:10:26.000000 yen-0.4.3/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1246 2024-05-14 17:44:31.565034 yen-0.4.3/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-03-30 13:10:26.000000 yen-0.4.3/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 17:44:31.559424 yen-0.4.3/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 17:44:31.563076 yen-0.4.3/src/yen/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3133 2024-05-14 17:36:00.000000 yen-0.4.3/src/yen/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      120 2024-03-30 13:10:26.000000 yen-0.4.3/src/yen/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1825 2024-05-14 17:37:29.000000 yen-0.4.3/src/yen/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1748 2024-05-08 21:39:33.000000 yen-0.4.3/src/yen/downloader.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)  1047789 2024-03-30 13:10:26.000000 yen-0.4.3/src/yen/fallback_release_data.json
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3848 2024-05-08 21:39:38.000000 yen-0.4.3/src/yen/github.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-03-30 13:10:26.000000 yen-0.4.3/src/yen/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 17:44:31.564158 yen-0.4.3/src/yen.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2670 2024-05-14 17:44:31.000000 yen-0.4.3/src/yen.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      371 2024-05-14 17:44:31.000000 yen-0.4.3/src/yen.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-14 17:44:31.000000 yen-0.4.3/src/yen.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       36 2024-05-14 17:44:31.000000 yen-0.4.3/src/yen.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       73 2024-05-14 17:44:31.000000 yen-0.4.3/src/yen.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        4 2024-05-14 17:44:31.000000 yen-0.4.3/src/yen.egg-info/top_level.txt
```

### Comparing `yen-0.4.2/LICENSE` & `yen-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yen-0.4.2/PKG-INFO` & `yen-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yen
-Version: 0.4.2
+Version: 0.4.3
 Summary: Yet another Python environment manager.
 Home-page: https://github.com/tusharsadhwani/yen
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yen-0.4.2/README.md` & `yen-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `yen-0.4.2/setup.cfg` & `yen-0.4.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yen
-version = 0.4.2
+version = 0.4.3
 description = Yet another Python environment manager.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/yen
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
```

### Comparing `yen-0.4.2/src/yen/__init__.py` & `yen-0.4.3/src/yen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,15 @@
         )
 
 
 def ensure_python(python_version: str) -> tuple[str, str]:
     """Checks if given Python version exists locally. If not, downloads it."""
     os.makedirs(PYTHON_INSTALLS_PATH, exist_ok=True)
 
-    try:
-        python_version, download_link = resolve_python_version(python_version)
-    except NotAvailable:
-        print(
-            "Error: requested Python version is not available."
-            " Use 'yen list' to get list of available Pythons."
-        )
-
+    python_version, download_link = resolve_python_version(python_version)
     download_directory = os.path.join(PYTHON_INSTALLS_PATH, python_version)
 
     if os.name == "nt":
         python_bin_path = os.path.join(download_directory, "python/python.exe")
     else:
         python_bin_path = os.path.join(download_directory, "python/bin/python3")
     if os.path.exists(python_bin_path):
```

### Comparing `yen-0.4.2/src/yen/cli.py` & `yen-0.4.3/src/yen/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """CLI interface for yen."""
 
 from __future__ import annotations
 
 import argparse
 from typing import Literal
 
-from yen import create_symlink, ensure_python, create_venv
+from yen import NotAvailable, create_symlink, create_venv, ensure_python
 from yen.github import list_pythons
 
 
 class YenArgs:
     command: Literal["list", "create", "use"]
     python: str
     venv_path: str
 
 
-def cli() -> None:
+def cli() -> int:
     """CLI interface."""
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(dest="command", required=True)
 
     subparsers.add_parser("list")
 
     create_parser = subparsers.add_parser("create")
@@ -34,13 +34,30 @@
     if args.command == "list":
         versions = list(list_pythons())
         print("Available Pythons:")
         for version in versions:
             print(version)
 
     elif args.command == "create":
-        python_version, python_bin_path = ensure_python(args.python)
-        create_venv(python_version, python_bin_path, args.venv_path)
+        try:
+            python_version, python_bin_path = ensure_python(args.python)
+            create_venv(python_version, python_bin_path, args.venv_path)
+        except NotAvailable:
+            print(
+                "Error: requested Python version is not available."
+                " Use 'yen list' to get list of available Pythons."
+            )
+            return 1
+
 
     elif args.command == "use":
-        python_version, python_bin_path = ensure_python(args.python)
-        create_symlink(python_bin_path, python_version)
+        try:
+            python_version, python_bin_path = ensure_python(args.python)
+            create_symlink(python_bin_path, python_version)
+        except NotAvailable:
+            print(
+                "Error: requested Python version is not available."
+                " Use 'yen list' to get list of available Pythons."
+            )
+            return 1
+
+    return 0
```

### Comparing `yen-0.4.2/src/yen/downloader.py` & `yen-0.4.3/src/yen/downloader.py`

 * *Files identical despite different names*

### Comparing `yen-0.4.2/src/yen/fallback_release_data.json` & `yen-0.4.3/src/yen/fallback_release_data.json`

 * *Files identical despite different names*

### Comparing `yen-0.4.2/src/yen/github.py` & `yen-0.4.3/src/yen/github.py`

 * *Files identical despite different names*

### Comparing `yen-0.4.2/src/yen.egg-info/PKG-INFO` & `yen-0.4.3/src/yen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yen
-Version: 0.4.2
+Version: 0.4.3
 Summary: Yet another Python environment manager.
 Home-page: https://github.com/tusharsadhwani/yen
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

