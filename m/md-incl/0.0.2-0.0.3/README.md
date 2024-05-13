# Comparing `tmp/md_incl-0.0.2.tar.gz` & `tmp/md_incl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_incl-0.0.2.tar", last modified: Mon May 13 23:22:29 2024, max compression
+gzip compressed data, was "md_incl-0.0.3.tar", last modified: Mon May 13 23:24:57 2024, max compression
```

## Comparing `md_incl-0.0.2.tar` & `md_incl-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:22:29.314485 md_incl-0.0.2/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     1065 2024-05-09 21:05:58.000000 md_incl-0.0.2/LICENSE
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     2130 2024-05-13 23:22:29.314227 md_incl-0.0.2/PKG-INFO
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     1620 2024-05-13 23:20:11.000000 md_incl-0.0.2/README.md
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      714 2024-05-13 23:21:43.000000 md_incl-0.0.2/pyproject.toml
--rw-r--r--   0 xiaotianhan   (501) staff       (20)       38 2024-05-13 23:22:29.314547 md_incl-0.0.2/setup.cfg
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:22:29.311800 md_incl-0.0.2/src/
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:22:29.312902 md_incl-0.0.2/src/markdown_include/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)        0 2024-05-09 22:19:18.000000 md_incl-0.0.2/src/markdown_include/__init__.py
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      407 2024-05-09 22:20:43.000000 md_incl-0.0.2/src/markdown_include/__main__.py
--rwxr-xr-x   0 xiaotianhan   (501) staff       (20)     1386 2024-05-09 23:13:13.000000 md_incl-0.0.2/src/markdown_include/markdown_include.py
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:22:29.313961 md_incl-0.0.2/src/md_incl.egg-info/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     2130 2024-05-13 23:22:29.000000 md_incl-0.0.2/src/md_incl.egg-info/PKG-INFO
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      348 2024-05-13 23:22:29.000000 md_incl-0.0.2/src/md_incl.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotianhan   (501) staff       (20)        1 2024-05-13 23:22:29.000000 md_incl-0.0.2/src/md_incl.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotianhan   (501) staff       (20)       59 2024-05-13 23:22:29.000000 md_incl-0.0.2/src/md_incl.egg-info/entry_points.txt
--rw-r--r--   0 xiaotianhan   (501) staff       (20)       17 2024-05-13 23:22:29.000000 md_incl-0.0.2/src/md_incl.egg-info/top_level.txt
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:22:29.313747 md_incl-0.0.2/tests/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      356 2024-05-13 20:53:52.000000 md_incl-0.0.2/tests/test_markdown_include.py
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:24:57.595548 md_incl-0.0.3/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     1065 2024-05-09 21:05:58.000000 md_incl-0.0.3/LICENSE
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     2072 2024-05-13 23:24:57.595274 md_incl-0.0.3/PKG-INFO
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     1562 2024-05-13 23:24:03.000000 md_incl-0.0.3/README.md
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      714 2024-05-13 23:24:48.000000 md_incl-0.0.3/pyproject.toml
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)       38 2024-05-13 23:24:57.595614 md_incl-0.0.3/setup.cfg
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:24:57.592455 md_incl-0.0.3/src/
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:24:57.593598 md_incl-0.0.3/src/markdown_include/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)        0 2024-05-09 22:19:18.000000 md_incl-0.0.3/src/markdown_include/__init__.py
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      407 2024-05-09 22:20:43.000000 md_incl-0.0.3/src/markdown_include/__main__.py
+-rwxr-xr-x   0 xiaotianhan   (501) staff       (20)     1386 2024-05-09 23:13:13.000000 md_incl-0.0.3/src/markdown_include/markdown_include.py
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:24:57.594997 md_incl-0.0.3/src/md_incl.egg-info/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     2072 2024-05-13 23:24:57.000000 md_incl-0.0.3/src/md_incl.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      348 2024-05-13 23:24:57.000000 md_incl-0.0.3/src/md_incl.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)        1 2024-05-13 23:24:57.000000 md_incl-0.0.3/src/md_incl.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)       59 2024-05-13 23:24:57.000000 md_incl-0.0.3/src/md_incl.egg-info/entry_points.txt
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)       17 2024-05-13 23:24:57.000000 md_incl-0.0.3/src/md_incl.egg-info/top_level.txt
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:24:57.594606 md_incl-0.0.3/tests/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      356 2024-05-13 20:53:52.000000 md_incl-0.0.3/tests/test_markdown_include.py
```

### Comparing `md_incl-0.0.2/LICENSE` & `md_incl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `md_incl-0.0.2/PKG-INFO` & `md_incl-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md_incl
-Version: 0.0.2
+Version: 0.0.3
 Summary: processes a Markdown file by including the contents of other Markdown files
 Author-email: Sean Han <xiaotian.han91@gmail.com>
 Project-URL: Homepage, https://github.com/hxtmike/markdown_include
 Project-URL: Issues, https://github.com/hxtmike/markdown_include/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
@@ -38,18 +38,14 @@
 ```
 
 ## Requirements
 
 + `>Python 3.8`
 + A text editor to modify the input and included files
 
-## Github
-
-<https://github.com/hxtmike/markdown_include>
-
 ## Contributions
 
 If you'd like to contribute to the development of this script, feel free to fork the repository and submit a pull request. I'll be happy to review your changes and merge them into the main codebase.
 
 ## License
 
 This script is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `md_incl-0.0.2/README.md` & `md_incl-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,18 +25,14 @@
 ```
 
 ## Requirements
 
 + `>Python 3.8`
 + A text editor to modify the input and included files
 
-## Github
-
-<https://github.com/hxtmike/markdown_include>
-
 ## Contributions
 
 If you'd like to contribute to the development of this script, feel free to fork the repository and submit a pull request. I'll be happy to review your changes and merge them into the main codebase.
 
 ## License
 
 This script is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `md_incl-0.0.2/pyproject.toml` & `md_incl-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'md_incl'
-version = '0.0.2'
+version = '0.0.3'
 authors = [{ name = "Sean Han", email = "xiaotian.han91@gmail.com" }]
 description = "processes a Markdown file by including the contents of other Markdown files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `md_incl-0.0.2/src/markdown_include/markdown_include.py` & `md_incl-0.0.3/src/markdown_include/markdown_include.py`

 * *Files identical despite different names*

### Comparing `md_incl-0.0.2/src/md_incl.egg-info/PKG-INFO` & `md_incl-0.0.3/src/md_incl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md_incl
-Version: 0.0.2
+Version: 0.0.3
 Summary: processes a Markdown file by including the contents of other Markdown files
 Author-email: Sean Han <xiaotian.han91@gmail.com>
 Project-URL: Homepage, https://github.com/hxtmike/markdown_include
 Project-URL: Issues, https://github.com/hxtmike/markdown_include/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
@@ -38,18 +38,14 @@
 ```
 
 ## Requirements
 
 + `>Python 3.8`
 + A text editor to modify the input and included files
 
-## Github
-
-<https://github.com/hxtmike/markdown_include>
-
 ## Contributions
 
 If you'd like to contribute to the development of this script, feel free to fork the repository and submit a pull request. I'll be happy to review your changes and merge them into the main codebase.
 
 ## License
 
 This script is licensed under the MIT License. See the LICENSE file for details.
```

