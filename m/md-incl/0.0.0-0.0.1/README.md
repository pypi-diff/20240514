# Comparing `tmp/md_incl-0.0.0.tar.gz` & `tmp/md_incl-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_incl-0.0.0.tar", last modified: Mon May 13 22:57:59 2024, max compression
+gzip compressed data, was "md_incl-0.0.1.tar", last modified: Mon May 13 23:08:42 2024, max compression
```

## Comparing `md_incl-0.0.0.tar` & `md_incl-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 22:57:59.572279 md_incl-0.0.0/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     1065 2024-05-09 21:05:58.000000 md_incl-0.0.0/LICENSE
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     2462 2024-05-13 22:57:59.572044 md_incl-0.0.0/PKG-INFO
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     1952 2024-05-13 22:55:36.000000 md_incl-0.0.0/README.md
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      714 2024-05-13 22:56:21.000000 md_incl-0.0.0/pyproject.toml
--rw-r--r--   0 xiaotianhan   (501) staff       (20)       38 2024-05-13 22:57:59.572335 md_incl-0.0.0/setup.cfg
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 22:57:59.567213 md_incl-0.0.0/src/
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 22:57:59.570338 md_incl-0.0.0/src/markdown_include/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)        0 2024-05-09 22:19:18.000000 md_incl-0.0.0/src/markdown_include/__init__.py
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      407 2024-05-09 22:20:43.000000 md_incl-0.0.0/src/markdown_include/__main__.py
--rwxr-xr-x   0 xiaotianhan   (501) staff       (20)     1386 2024-05-09 23:13:13.000000 md_incl-0.0.0/src/markdown_include/markdown_include.py
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 22:57:59.571778 md_incl-0.0.0/src/md_incl.egg-info/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)     2462 2024-05-13 22:57:59.000000 md_incl-0.0.0/src/md_incl.egg-info/PKG-INFO
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      348 2024-05-13 22:57:59.000000 md_incl-0.0.0/src/md_incl.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotianhan   (501) staff       (20)        1 2024-05-13 22:57:59.000000 md_incl-0.0.0/src/md_incl.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotianhan   (501) staff       (20)       59 2024-05-13 22:57:59.000000 md_incl-0.0.0/src/md_incl.egg-info/entry_points.txt
--rw-r--r--   0 xiaotianhan   (501) staff       (20)       17 2024-05-13 22:57:59.000000 md_incl-0.0.0/src/md_incl.egg-info/top_level.txt
-drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 22:57:59.571418 md_incl-0.0.0/tests/
--rw-r--r--   0 xiaotianhan   (501) staff       (20)      356 2024-05-13 20:53:52.000000 md_incl-0.0.0/tests/test_markdown_include.py
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:08:42.066486 md_incl-0.0.1/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     1065 2024-05-09 21:05:58.000000 md_incl-0.0.1/LICENSE
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     2390 2024-05-13 23:08:42.066250 md_incl-0.0.1/PKG-INFO
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     1880 2024-05-13 23:08:09.000000 md_incl-0.0.1/README.md
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      714 2024-05-13 22:58:45.000000 md_incl-0.0.1/pyproject.toml
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)       38 2024-05-13 23:08:42.066689 md_incl-0.0.1/setup.cfg
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:08:42.063296 md_incl-0.0.1/src/
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:08:42.064578 md_incl-0.0.1/src/markdown_include/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)        0 2024-05-09 22:19:18.000000 md_incl-0.0.1/src/markdown_include/__init__.py
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      407 2024-05-09 22:20:43.000000 md_incl-0.0.1/src/markdown_include/__main__.py
+-rwxr-xr-x   0 xiaotianhan   (501) staff       (20)     1386 2024-05-09 23:13:13.000000 md_incl-0.0.1/src/markdown_include/markdown_include.py
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:08:42.065983 md_incl-0.0.1/src/md_incl.egg-info/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)     2390 2024-05-13 23:08:42.000000 md_incl-0.0.1/src/md_incl.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      348 2024-05-13 23:08:42.000000 md_incl-0.0.1/src/md_incl.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)        1 2024-05-13 23:08:42.000000 md_incl-0.0.1/src/md_incl.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)       59 2024-05-13 23:08:42.000000 md_incl-0.0.1/src/md_incl.egg-info/entry_points.txt
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)       17 2024-05-13 23:08:42.000000 md_incl-0.0.1/src/md_incl.egg-info/top_level.txt
+drwxr-xr-x   0 xiaotianhan   (501) staff       (20)        0 2024-05-13 23:08:42.065644 md_incl-0.0.1/tests/
+-rw-r--r--   0 xiaotianhan   (501) staff       (20)      356 2024-05-13 20:53:52.000000 md_incl-0.0.1/tests/test_markdown_include.py
```

### Comparing `md_incl-0.0.0/LICENSE` & `md_incl-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `md_incl-0.0.0/PKG-INFO` & `md_incl-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md_incl
-Version: 0.0.0
+Version: 0.0.1
 Summary: processes a Markdown file by including the contents of other Markdown files
 Author-email: Sean Han <xiaotian.han91@gmail.com>
 Project-URL: Homepage, https://github.com/hxtmike/markdown_include
 Project-URL: Issues, https://github.com/hxtmike/markdown_include/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
@@ -13,42 +13,44 @@
 
 # markdown_include
 
 This is a simple Python script that processes Markdown files by including the contents of other Markdown files.
 
 The script takes in a Markdown file as input, looks for lines that are similar to `<!-- include (filename) -->` (Parentheses are necessary to identify the path) and treats them as include directives. For each include directive, the script reads the specified file and writes its contents to the output file. The result is a new Markdown file that includes the contents of all included files.
 
+## Github
+
+<https://github.com/hxtmike/markdown_include>
+
 ## Usage
 
 To use the script, simply pass the input file name and the output file name as command-line arguments. The script will process the input file, generate the output file, and exit. Here's an example of how to run the script:
 
 ```shell
 md_incl input_file.md output_file.md
 ```
 
-This script will be added as a command to the `$PATH` for direct invocation
+This script will be added as a command after installation
 
 ## Features
 
 + Processes Markdown files by including the contents of other Markdown files
 + Supports include directives in the format of `<!-- include (filename) -->` (Parentheses are necessary to identify the path)
 + Outputs a new Markdown file that includes the contents of the included files
 + Takes in input and output file names as command-line arguments
 
 ## Requirements
 
-+ `>Python 3.5`
++ `>Python 3.8`
 + A text editor to modify the input and included files
 
 ## Installation
 
-To use this script, simply download the file and save it to your computer. You can use `pip` to install the command
-
 ```shell
-pip3 install .
+pip install md-incl
 ```
 
 It could be used in some building system like `Makefile`, which allows for the automatic assembly of large and complex reports and papers.
 
 ## Contributions
 
 If you'd like to contribute to the development of this script, feel free to fork the repository and submit a pull request. I'll be happy to review your changes and merge them into the main codebase.
```

### Comparing `md_incl-0.0.0/README.md` & `md_incl-0.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # markdown_include
 
 This is a simple Python script that processes Markdown files by including the contents of other Markdown files.
 
 The script takes in a Markdown file as input, looks for lines that are similar to `<!-- include (filename) -->` (Parentheses are necessary to identify the path) and treats them as include directives. For each include directive, the script reads the specified file and writes its contents to the output file. The result is a new Markdown file that includes the contents of all included files.
 
+## Github
+
+<https://github.com/hxtmike/markdown_include>
+
 ## Usage
 
 To use the script, simply pass the input file name and the output file name as command-line arguments. The script will process the input file, generate the output file, and exit. Here's an example of how to run the script:
 
 ```shell
 md_incl input_file.md output_file.md
 ```
 
-This script will be added as a command to the `$PATH` for direct invocation
+This script will be added as a command after installation
 
 ## Features
 
 + Processes Markdown files by including the contents of other Markdown files
 + Supports include directives in the format of `<!-- include (filename) -->` (Parentheses are necessary to identify the path)
 + Outputs a new Markdown file that includes the contents of the included files
 + Takes in input and output file names as command-line arguments
 
 ## Requirements
 
-+ `>Python 3.5`
++ `>Python 3.8`
 + A text editor to modify the input and included files
 
 ## Installation
 
-To use this script, simply download the file and save it to your computer. You can use `pip` to install the command
-
 ```shell
-pip3 install .
+pip install md-incl
 ```
 
 It could be used in some building system like `Makefile`, which allows for the automatic assembly of large and complex reports and papers.
 
 ## Contributions
 
 If you'd like to contribute to the development of this script, feel free to fork the repository and submit a pull request. I'll be happy to review your changes and merge them into the main codebase.
```

### Comparing `md_incl-0.0.0/pyproject.toml` & `md_incl-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'md_incl'
-version = '0.0.0'
+version = '0.0.1'
 authors = [{ name = "Sean Han", email = "xiaotian.han91@gmail.com" }]
 description = "processes a Markdown file by including the contents of other Markdown files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `md_incl-0.0.0/src/markdown_include/markdown_include.py` & `md_incl-0.0.1/src/markdown_include/markdown_include.py`

 * *Files identical despite different names*

### Comparing `md_incl-0.0.0/src/md_incl.egg-info/PKG-INFO` & `md_incl-0.0.1/src/md_incl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md_incl
-Version: 0.0.0
+Version: 0.0.1
 Summary: processes a Markdown file by including the contents of other Markdown files
 Author-email: Sean Han <xiaotian.han91@gmail.com>
 Project-URL: Homepage, https://github.com/hxtmike/markdown_include
 Project-URL: Issues, https://github.com/hxtmike/markdown_include/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
@@ -13,42 +13,44 @@
 
 # markdown_include
 
 This is a simple Python script that processes Markdown files by including the contents of other Markdown files.
 
 The script takes in a Markdown file as input, looks for lines that are similar to `<!-- include (filename) -->` (Parentheses are necessary to identify the path) and treats them as include directives. For each include directive, the script reads the specified file and writes its contents to the output file. The result is a new Markdown file that includes the contents of all included files.
 
+## Github
+
+<https://github.com/hxtmike/markdown_include>
+
 ## Usage
 
 To use the script, simply pass the input file name and the output file name as command-line arguments. The script will process the input file, generate the output file, and exit. Here's an example of how to run the script:
 
 ```shell
 md_incl input_file.md output_file.md
 ```
 
-This script will be added as a command to the `$PATH` for direct invocation
+This script will be added as a command after installation
 
 ## Features
 
 + Processes Markdown files by including the contents of other Markdown files
 + Supports include directives in the format of `<!-- include (filename) -->` (Parentheses are necessary to identify the path)
 + Outputs a new Markdown file that includes the contents of the included files
 + Takes in input and output file names as command-line arguments
 
 ## Requirements
 
-+ `>Python 3.5`
++ `>Python 3.8`
 + A text editor to modify the input and included files
 
 ## Installation
 
-To use this script, simply download the file and save it to your computer. You can use `pip` to install the command
-
 ```shell
-pip3 install .
+pip install md-incl
 ```
 
 It could be used in some building system like `Makefile`, which allows for the automatic assembly of large and complex reports and papers.
 
 ## Contributions
 
 If you'd like to contribute to the development of this script, feel free to fork the repository and submit a pull request. I'll be happy to review your changes and merge them into the main codebase.
```

