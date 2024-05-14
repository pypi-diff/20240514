# Comparing `tmp/packaged-0.3.0.tar.gz` & `tmp/packaged-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.3.0.tar", last modified: Sun May 12 06:38:20 2024, max compression
+gzip compressed data, was "packaged-0.3.1.tar", last modified: Tue May 14 12:31:39 2024, max compression
```

## Comparing `packaged-0.3.0.tar` & `packaged-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-12 06:38:20.473306 packaged-0.3.0/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.3.0/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3769 2024-05-12 06:38:20.473235 packaged-0.3.0/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2557 2024-05-12 06:38:05.000000 packaged-0.3.0/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1270 2024-05-12 06:38:20.473653 packaged-0.3.0/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.3.0/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-12 06:38:20.469479 packaged-0.3.0/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-12 06:38:20.471046 packaged-0.3.0/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4507 2024-05-11 20:09:56.000000 packaged-0.3.0/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.3.0/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2416 2024-05-12 06:38:05.000000 packaged-0.3.0/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1457 2024-05-12 06:38:05.000000 packaged-0.3.0/src/packaged/config.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.3.0/src/packaged/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-12 06:38:20.472500 packaged-0.3.0/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3769 2024-05-12 06:38:20.000000 packaged-0.3.0/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      369 2024-05-12 06:38:20.000000 packaged-0.3.0/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-12 06:38:20.000000 packaged-0.3.0/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-12 06:38:20.000000 packaged-0.3.0/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      105 2024-05-12 06:38:20.000000 packaged-0.3.0/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-12 06:38:20.000000 packaged-0.3.0/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.856349 packaged-0.3.1/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.3.1/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4287 2024-05-14 12:31:39.856269 packaged-0.3.1/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3036 2024-05-14 12:26:43.000000 packaged-0.3.1/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1342 2024-05-14 12:31:39.856662 packaged-0.3.1/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.3.1/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.851889 packaged-0.3.1/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.854610 packaged-0.3.1/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3778 2024-05-14 12:13:43.000000 packaged-0.3.1/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.3.1/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2377 2024-05-14 12:08:44.000000 packaged-0.3.1/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1457 2024-05-12 06:38:05.000000 packaged-0.3.1/src/packaged/config.py
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.3.1/src/packaged/makeself-header.sh
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.3.1/src/packaged/makeself.sh
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.3.1/src/packaged/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.855753 packaged-0.3.1/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4287 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      105 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.3.0/PKG-INFO` & `packaged-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.3.0
+Version: 0.3.1
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+License: GPL-2.0-or-later
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -99,23 +99,23 @@
 
 ```bash
 packaged './textualdemo.bin' 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
-### Chimp game (pygame)
+### Aliens (pygame)
 
-Pygame ships with various games as well, `pygame.examples.chimp` is one of them:
+Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
-packaged './chimp' 'pip install pygame' 'python -m pygame.examples.chimp'
+packaged './aliens' 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
-Another fun game that you can try out are `pygame.examples.aliens`.
+Another one that you can try out is `pygame.examples.chimp`.
 
 ## Local Development / Testing
 
 To test and modify the package locally:
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
@@ -138,7 +138,18 @@
 ```
 
 Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation):
 
 ```bash
 twine upload dist/*
 ```
+
+## License
+
+The package is Licensed under GNU General Public License v2 (GPLv2). However,
+note that **the packages created with `packaged` are NOT licensed under GPL**.
+This is because the archives created are just data for the package, and
+`packaged` is not a part of the archives created.
+
+That means that you can freely use `packaged` for commercial use.
+
+Read the [License section for Makeself](https://github.com/megastep/makeself?tab=readme-ov-file#license) for more information.
```

### Comparing `packaged-0.3.0/README.md` & `packaged-0.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -67,23 +67,23 @@
 
 ```bash
 packaged './textualdemo.bin' 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
-### Chimp game (pygame)
+### Aliens (pygame)
 
-Pygame ships with various games as well, `pygame.examples.chimp` is one of them:
+Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
-packaged './chimp' 'pip install pygame' 'python -m pygame.examples.chimp'
+packaged './aliens' 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
-Another fun game that you can try out are `pygame.examples.aliens`.
+Another one that you can try out is `pygame.examples.chimp`.
 
 ## Local Development / Testing
 
 To test and modify the package locally:
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
@@ -106,7 +106,18 @@
 ```
 
 Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation):
 
 ```bash
 twine upload dist/*
 ```
+
+## License
+
+The package is Licensed under GNU General Public License v2 (GPLv2). However,
+note that **the packages created with `packaged` are NOT licensed under GPL**.
+This is because the archives created are just data for the package, and
+`packaged` is not a part of the archives created.
+
+That means that you can freely use `packaged` for commercial use.
+
+Read the [License section for Makeself](https://github.com/megastep/makeself?tab=readme-ov-file#license) for more information.
```

### Comparing `packaged-0.3.0/setup.cfg` & `packaged-0.3.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = packaged
-version = 0.3.0
+version = 0.3.1
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
-license = MIT
+license = GPL-2.0-or-later
 license_file = LICENSE
 classifiers = 
-	License :: OSI Approved :: MIT License
+	License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
@@ -45,14 +45,16 @@
 	pytest-cov
 	pytest-xdist
 	tox
 
 [options.package_data]
 packaged = 
 	py.typed
+	makeself.sh
+	makeself-header.sh
 
 [tool:pytest]
 addopts = --cov --cov-report=term-missing -nauto
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `packaged-0.3.0/src/packaged/cli.py` & `packaged-0.3.1/src/packaged/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import argparse
 import os.path
 import platform
 import sys
 
-from packaged import SourceDirectoryNotFound, ensure_makeself, create_package
+from packaged import SourceDirectoryNotFound, create_package
 from packaged.config import (
     Config,
     ConfigValidationError,
     config_file_exists,
     parse_config,
 )
 
@@ -68,14 +68,13 @@
         source_directory, output_path, build_command, startup_command = (
             args.source_directory,
             args.output_path,
             args.build_command,
             args.startup_command,
         )
 
-    ensure_makeself()
     try:
         create_package(source_directory, output_path, build_command, startup_command)
     except SourceDirectoryNotFound as exc:
         error(f"Folder {exc.directory_path!r} does not exist.")
 
     return 0
```

### Comparing `packaged-0.3.0/src/packaged/config.py` & `packaged-0.3.1/src/packaged/config.py`

 * *Files identical despite different names*

### Comparing `packaged-0.3.0/src/packaged.egg-info/PKG-INFO` & `packaged-0.3.1/src/packaged.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.3.0
+Version: 0.3.1
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+License: GPL-2.0-or-later
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -99,23 +99,23 @@
 
 ```bash
 packaged './textualdemo.bin' 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
-### Chimp game (pygame)
+### Aliens (pygame)
 
-Pygame ships with various games as well, `pygame.examples.chimp` is one of them:
+Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
-packaged './chimp' 'pip install pygame' 'python -m pygame.examples.chimp'
+packaged './aliens' 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
-Another fun game that you can try out are `pygame.examples.aliens`.
+Another one that you can try out is `pygame.examples.chimp`.
 
 ## Local Development / Testing
 
 To test and modify the package locally:
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
@@ -138,7 +138,18 @@
 ```
 
 Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation):
 
 ```bash
 twine upload dist/*
 ```
+
+## License
+
+The package is Licensed under GNU General Public License v2 (GPLv2). However,
+note that **the packages created with `packaged` are NOT licensed under GPL**.
+This is because the archives created are just data for the package, and
+`packaged` is not a part of the archives created.
+
+That means that you can freely use `packaged` for commercial use.
+
+Read the [License section for Makeself](https://github.com/megastep/makeself?tab=readme-ov-file#license) for more information.
```

