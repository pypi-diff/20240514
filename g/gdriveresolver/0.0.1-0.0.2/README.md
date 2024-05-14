# Comparing `tmp/gdriveresolver-0.0.1.tar.gz` & `tmp/gdriveresolver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdriveresolver-0.0.1.tar", last modified: Tue May 14 20:49:26 2024, max compression
+gzip compressed data, was "gdriveresolver-0.0.2.tar", last modified: Tue May 14 20:58:48 2024, max compression
```

## Comparing `gdriveresolver-0.0.1.tar` & `gdriveresolver-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:49:26.400982 gdriveresolver-0.0.1/
--rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.1/LICENSE
--rw-r--r--   0 harman     (501) staff       (20)     1848 2024-05-14 20:49:26.400823 gdriveresolver-0.0.1/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)     1219 2024-05-14 20:23:11.000000 gdriveresolver-0.0.1/README.md
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:49:26.400673 gdriveresolver-0.0.1/gdriveresolver.egg-info/
--rw-r--r--   0 harman     (501) staff       (20)     1848 2024-05-14 20:49:26.000000 gdriveresolver-0.0.1/gdriveresolver.egg-info/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      335 2024-05-14 20:49:26.000000 gdriveresolver-0.0.1/gdriveresolver.egg-info/SOURCES.txt
--rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-14 20:49:26.000000 gdriveresolver-0.0.1/gdriveresolver.egg-info/dependency_links.txt
--rw-r--r--   0 harman     (501) staff       (20)       10 2024-05-14 20:49:26.000000 gdriveresolver-0.0.1/gdriveresolver.egg-info/top_level.txt
--rw-r--r--   0 harman     (501) staff       (20)      591 2024-05-14 20:49:17.000000 gdriveresolver-0.0.1/pyproject.toml
--rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-14 20:49:26.401023 gdriveresolver-0.0.1/setup.cfg
--rw-r--r--   0 harman     (501) staff       (20)      448 2024-05-14 19:57:18.000000 gdriveresolver-0.0.1/setup.py
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:49:26.400087 gdriveresolver-0.0.1/src/
--rw-r--r--   0 harman     (501) staff       (20)       42 2024-05-14 19:54:16.000000 gdriveresolver-0.0.1/src/__init__.py
--rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.1/src/exceptions.py
--rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-14 18:17:17.000000 gdriveresolver-0.0.1/src/model.py
--rw-r--r--   0 harman     (501) staff       (20)      862 2024-05-14 19:55:10.000000 gdriveresolver-0.0.1/src/resolver.py
--rw-r--r--   0 harman     (501) staff       (20)     2805 2024-05-14 19:26:42.000000 gdriveresolver-0.0.1/src/system_operations.py
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:49:26.400405 gdriveresolver-0.0.1/tests/
--rw-r--r--   0 harman     (501) staff       (20)        0 2024-05-14 18:28:00.000000 gdriveresolver-0.0.1/tests/__init__.py
--rw-r--r--   0 harman     (501) staff       (20)     3968 2024-05-14 19:51:42.000000 gdriveresolver-0.0.1/tests/test_google_drive_resolver.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:58:48.424729 gdriveresolver-0.0.2/
+-rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.2/LICENSE
+-rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 20:58:48.424551 gdriveresolver-0.0.2/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      992 2024-05-14 20:57:44.000000 gdriveresolver-0.0.2/README.md
+-rw-r--r--   0 harman     (501) staff       (20)      591 2024-05-14 20:58:45.000000 gdriveresolver-0.0.2/pyproject.toml
+-rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-14 20:58:48.424771 gdriveresolver-0.0.2/setup.cfg
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:58:48.423655 gdriveresolver-0.0.2/src/
+-rw-r--r--   0 harman     (501) staff       (20)       42 2024-05-14 19:54:16.000000 gdriveresolver-0.0.2/src/__init__.py
+-rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.2/src/exceptions.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:58:48.424380 gdriveresolver-0.0.2/src/gdriveresolver.egg-info/
+-rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 20:58:48.000000 gdriveresolver-0.0.2/src/gdriveresolver.egg-info/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      324 2024-05-14 20:58:48.000000 gdriveresolver-0.0.2/src/gdriveresolver.egg-info/SOURCES.txt
+-rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-14 20:58:48.000000 gdriveresolver-0.0.2/src/gdriveresolver.egg-info/dependency_links.txt
+-rw-r--r--   0 harman     (501) staff       (20)       53 2024-05-14 20:58:48.000000 gdriveresolver-0.0.2/src/gdriveresolver.egg-info/top_level.txt
+-rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-14 18:17:17.000000 gdriveresolver-0.0.2/src/model.py
+-rw-r--r--   0 harman     (501) staff       (20)      862 2024-05-14 19:55:10.000000 gdriveresolver-0.0.2/src/resolver.py
+-rw-r--r--   0 harman     (501) staff       (20)     2805 2024-05-14 19:26:42.000000 gdriveresolver-0.0.2/src/system_operations.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 20:58:48.424202 gdriveresolver-0.0.2/tests/
+-rw-r--r--   0 harman     (501) staff       (20)     3968 2024-05-14 19:51:42.000000 gdriveresolver-0.0.2/tests/test_google_drive_resolver.py
```

### Comparing `gdriveresolver-0.0.1/LICENSE` & `gdriveresolver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.1/PKG-INFO` & `gdriveresolver-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,40 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
-Author: Your Name
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gdrive_resolver
 Different systems may mount Google Drive to different locations. 
 This package automatically finds the mounted Google Drive directory so that it can resolve Google Drive relative
 paths to absolute system paths.
 
 Example Usage:
 
 ```python
-from src import GoogleDriveResolver
+from gdriveresolver import GoogleDriveResolver
 
 gdrive_resolver = GoogleDriveResolver()
-absolute_path = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
-print(absolute_path)
-```
-```output
-"/path/to/mounted/google/drive/my/path/in/google/drive/myfile.txt"
-```
-
-## Development
-```bash
-git clone
-cd src
-# Create a virtual environment, then:
-pip install -r requirements.txt
-```
-
-## Testing
-```bash
-pytest tests
+absolute_path: str = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
 ```
 
 ## Troubleshooting
 If GoogleDriveResolver cannot resolve your Google Drive path, it may not be searching at a sufficient depth.
 You can increase the depth by passing the `max_depth` parameter to the constructor.
 
 ```python
-from src import GoogleDriveResolver
+from gdriveresolver import GoogleDriveResolver
 
 absolute_path = GoogleDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
 print(absolute_path)
 ```
 If it still cannot resolve your path, please ensure that your Google Drive is mounted, accessible,
 and that it is called "Google Drive" or "GoogleDrive" in your system.
```

### Comparing `gdriveresolver-0.0.1/README.md` & `gdriveresolver-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,42 +2,25 @@
 Different systems may mount Google Drive to different locations. 
 This package automatically finds the mounted Google Drive directory so that it can resolve Google Drive relative
 paths to absolute system paths.
 
 Example Usage:
 
 ```python
-from src import GoogleDriveResolver
+from gdriveresolver import GoogleDriveResolver
 
 gdrive_resolver = GoogleDriveResolver()
-absolute_path = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
-print(absolute_path)
-```
-```output
-"/path/to/mounted/google/drive/my/path/in/google/drive/myfile.txt"
-```
-
-## Development
-```bash
-git clone
-cd src
-# Create a virtual environment, then:
-pip install -r requirements.txt
-```
-
-## Testing
-```bash
-pytest tests
+absolute_path: str = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
 ```
 
 ## Troubleshooting
 If GoogleDriveResolver cannot resolve your Google Drive path, it may not be searching at a sufficient depth.
 You can increase the depth by passing the `max_depth` parameter to the constructor.
 
 ```python
-from src import GoogleDriveResolver
+from gdriveresolver import GoogleDriveResolver
 
 absolute_path = GoogleDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
 print(absolute_path)
 ```
 If it still cannot resolve your path, please ensure that your Google Drive is mounted, accessible,
 and that it is called "Google Drive" or "GoogleDrive" in your system.
```

### Comparing `gdriveresolver-0.0.1/gdriveresolver.egg-info/PKG-INFO` & `gdriveresolver-0.0.2/src/gdriveresolver.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,40 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
-Author: Your Name
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gdrive_resolver
 Different systems may mount Google Drive to different locations. 
 This package automatically finds the mounted Google Drive directory so that it can resolve Google Drive relative
 paths to absolute system paths.
 
 Example Usage:
 
 ```python
-from src import GoogleDriveResolver
+from gdriveresolver import GoogleDriveResolver
 
 gdrive_resolver = GoogleDriveResolver()
-absolute_path = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
-print(absolute_path)
-```
-```output
-"/path/to/mounted/google/drive/my/path/in/google/drive/myfile.txt"
-```
-
-## Development
-```bash
-git clone
-cd src
-# Create a virtual environment, then:
-pip install -r requirements.txt
-```
-
-## Testing
-```bash
-pytest tests
+absolute_path: str = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
 ```
 
 ## Troubleshooting
 If GoogleDriveResolver cannot resolve your Google Drive path, it may not be searching at a sufficient depth.
 You can increase the depth by passing the `max_depth` parameter to the constructor.
 
 ```python
-from src import GoogleDriveResolver
+from gdriveresolver import GoogleDriveResolver
 
 absolute_path = GoogleDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
 print(absolute_path)
 ```
 If it still cannot resolve your path, please ensure that your Google Drive is mounted, accessible,
 and that it is called "Google Drive" or "GoogleDrive" in your system.
```

### Comparing `gdriveresolver-0.0.1/pyproject.toml` & `gdriveresolver-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gdriveresolver"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="C Harman", email="charman@netrias.com" },
 ]
 description = "A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gdriveresolver-0.0.1/src/model.py` & `gdriveresolver-0.0.2/src/model.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.1/src/resolver.py` & `gdriveresolver-0.0.2/src/resolver.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.1/src/system_operations.py` & `gdriveresolver-0.0.2/src/system_operations.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.1/tests/test_google_drive_resolver.py` & `gdriveresolver-0.0.2/tests/test_google_drive_resolver.py`

 * *Files identical despite different names*

