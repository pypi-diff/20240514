# Comparing `tmp/sortipy-0.0.3.tar.gz` & `tmp/sortipy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortipy-0.0.3.tar", last modified: Tue May 14 21:11:44 2024, max compression
+gzip compressed data, was "sortipy-0.0.4.tar", last modified: Tue May 14 21:18:18 2024, max compression
```

## Comparing `sortipy-0.0.3.tar` & `sortipy-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.226017 sortipy-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3198 2024-05-14 21:11:44.221491 sortipy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2801 2024-05-14 21:07:55.000000 sortipy-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 21:11:44.226017 sortipy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      551 2024-05-14 21:09:49.000000 sortipy-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.146071 sortipy-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.174396 sortipy-0.0.3/src/sortipy/
--rw-rw-rw-   0        0        0        0 2024-05-14 10:25:51.000000 sortipy-0.0.3/src/sortipy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.195730 sortipy-0.0.3/src/sortipy/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-14 12:17:07.000000 sortipy-0.0.3/src/sortipy/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1546 2024-05-14 18:48:33.000000 sortipy-0.0.3/src/sortipy/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.206055 sortipy-0.0.3/src/sortipy/models/
--rw-rw-rw-   0        0        0     1710 2024-05-14 20:28:27.000000 sortipy-0.0.3/src/sortipy/models/Directory.py
--rw-rw-rw-   0        0        0     2050 2024-05-14 19:05:49.000000 sortipy-0.0.3/src/sortipy/models/File.py
--rw-rw-rw-   0        0        0        0 2024-05-14 12:14:42.000000 sortipy-0.0.3/src/sortipy/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.213951 sortipy-0.0.3/src/sortipy/sorters/
--rw-rw-rw-   0        0        0     1458 2024-05-14 20:43:39.000000 sortipy-0.0.3/src/sortipy/sorters/DefaultSorter.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:53:00.000000 sortipy-0.0.3/src/sortipy/sorters/__init__.py
--rw-rw-rw-   0        0        0     1125 2024-05-14 21:10:53.000000 sortipy-0.0.3/src/sortipy/sortipy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.215938 sortipy-0.0.3/src/sortipy.egg-info/
--rw-rw-rw-   0        0        0     3198 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.535372 sortipy-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3198 2024-05-14 21:18:18.535372 sortipy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2801 2024-05-14 21:17:57.000000 sortipy-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:18:18.535372 sortipy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      551 2024-05-14 21:17:52.000000 sortipy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.455435 sortipy-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.475577 sortipy-0.0.4/src/sortipy/
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:25:51.000000 sortipy-0.0.4/src/sortipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.516987 sortipy-0.0.4/src/sortipy/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-14 12:17:07.000000 sortipy-0.0.4/src/sortipy/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1546 2024-05-14 18:48:33.000000 sortipy-0.0.4/src/sortipy/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.526970 sortipy-0.0.4/src/sortipy/models/
+-rw-rw-rw-   0        0        0     1726 2024-05-14 21:16:43.000000 sortipy-0.0.4/src/sortipy/models/Directory.py
+-rw-rw-rw-   0        0        0     2058 2024-05-14 21:16:47.000000 sortipy-0.0.4/src/sortipy/models/File.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 12:14:42.000000 sortipy-0.0.4/src/sortipy/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.530863 sortipy-0.0.4/src/sortipy/sorters/
+-rw-rw-rw-   0        0        0     1466 2024-05-14 21:17:07.000000 sortipy-0.0.4/src/sortipy/sorters/DefaultSorter.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:53:00.000000 sortipy-0.0.4/src/sortipy/sorters/__init__.py
+-rw-rw-rw-   0        0        0     1141 2024-05-14 21:16:36.000000 sortipy-0.0.4/src/sortipy/sortipy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.533805 sortipy-0.0.4/src/sortipy.egg-info/
+-rw-rw-rw-   0        0        0     3198 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/top_level.txt
```

### Comparing `sortipy-0.0.3/LICENSE` & `sortipy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.3/LICENSE.txt` & `sortipy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.3/PKG-INFO` & `sortipy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sortipy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sortipy is designed to help you organize files in a directory by sorting them based on their file extensions.
 Home-page: https://github.com/pzzzl/sortipy
 Author: Bruno Peselli
 Author-email: brunopeselli@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 <h1 align="center">Sortipy</h1>
 
 <p align="center">
-    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.3_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
+    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.4_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
 </p>
 
 <p align="center"><b><i>Sortipy</i></b> is a Python package designed to help you organize files in a directory by sorting them based on their file extensions.</p>
 
 ## Summary
 
 - [Summary](#summary)
```

### Comparing `sortipy-0.0.3/README.md` & `sortipy-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">Sortipy</h1>
 
 <p align="center">
-    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.3_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
+    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.4_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
 </p>
 
 <p align="center"><b><i>Sortipy</i></b> is a Python package designed to help you organize files in a directory by sorting them based on their file extensions.</p>
 
 ## Summary
 
 - [Summary](#summary)
```

### Comparing `sortipy-0.0.3/setup.py` & `sortipy-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sortipy',
-    version='0.0.3',
+    version='0.0.4',
     author='Bruno Peselli',
     author_email='brunopeselli@gmail.com',
     description='Sortipy is designed to help you organize files in a directory by sorting them based on their file extensions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/pzzzl/sortipy',
     packages=find_packages(where='src'),
```

### Comparing `sortipy-0.0.3/src/sortipy/exceptions/exceptions.py` & `sortipy-0.0.4/src/sortipy/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.3/src/sortipy/models/Directory.py` & `sortipy-0.0.4/src/sortipy/models/Directory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from exceptions.exceptions import DirectoryNotFoundError, EmptyDirectoryError, ExtensionNotAllowedError
-from models.File import File
+from sortipy.exceptions.exceptions import DirectoryNotFoundError, EmptyDirectoryError, ExtensionNotAllowedError
+from sortipy.models.File import File
 from typing import List
 
 class Directory:
     """
     Represents a directory containing files with specified extensions.
 
     Attributes:
```

### Comparing `sortipy-0.0.3/src/sortipy/models/File.py` & `sortipy-0.0.4/src/sortipy/models/File.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from exceptions.exceptions import ExtensionNotAllowedError
+from sortipy.exceptions.exceptions import ExtensionNotAllowedError
 from typing import List
 
 class File:
     """
     Represents a file with specified extensions.
 
     Attributes:
```

### Comparing `sortipy-0.0.3/src/sortipy/sorters/DefaultSorter.py` & `sortipy-0.0.4/src/sortipy/sorters/DefaultSorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from models.File import File
+from sortipy.models.File import File
 from typing import List, Dict
 import os
 
 class DefaultSorter:
     """
     A class to sort files based on their extensions.
```

### Comparing `sortipy-0.0.3/src/sortipy/sortipy.py` & `sortipy-0.0.4/src/sortipy/sortipy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
-from models.Directory import Directory
-from sorters.DefaultSorter import DefaultSorter
+from sortipy.models.Directory import Directory
+from sortipy.sorters.DefaultSorter import DefaultSorter
 
 def sort(path: str, extensions: List[str] = []) -> Dict[str, List[str]]:
     """
     Sorts files in a directory based on their extensions.
 
     Args:
         path (str): The path to the directory containing files to be sorted.
```

### Comparing `sortipy-0.0.3/src/sortipy.egg-info/PKG-INFO` & `sortipy-0.0.4/src/sortipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sortipy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sortipy is designed to help you organize files in a directory by sorting them based on their file extensions.
 Home-page: https://github.com/pzzzl/sortipy
 Author: Bruno Peselli
 Author-email: brunopeselli@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 <h1 align="center">Sortipy</h1>
 
 <p align="center">
-    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.3_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
+    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.4_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
 </p>
 
 <p align="center"><b><i>Sortipy</i></b> is a Python package designed to help you organize files in a directory by sorting them based on their file extensions.</p>
 
 ## Summary
 
 - [Summary](#summary)
```

