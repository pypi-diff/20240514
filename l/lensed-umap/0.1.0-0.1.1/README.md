# Comparing `tmp/lensed_umap-0.1.0.tar.gz` & `tmp/lensed_umap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lensed_umap-0.1.0.tar", last modified: Mon Apr  8 16:07:52 2024, max compression
+gzip compressed data, was "lensed_umap-0.1.1.tar", last modified: Tue May 14 16:35:24 2024, max compression
```

## Comparing `lensed_umap-0.1.0.tar` & `lensed_umap-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/_static/initial_umap.png
--rw-r--r--   0 runner    (1001) docker     (127)    14959 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/_static/lensed_umap.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/lensed_umap/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/lensed_umap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/lensed_umap/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/lensed_umap/fast_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/lensed_umap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/lensed_umap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-08 16:07:18.000000 lensed_umap-0.1.0/lensed_umap/tests/test_lenses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/lensed_umap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-08 16:07:52.000000 lensed_umap-0.1.0/lensed_umap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 16:07:52.000000 lensed_umap-0.1.0/lensed_umap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:07:52.000000 lensed_umap-0.1.0/lensed_umap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 16:07:52.000000 lensed_umap-0.1.0/lensed_umap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 16:07:52.000000 lensed_umap-0.1.0/lensed_umap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 16:07:19.000000 lensed_umap-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 16:07:19.000000 lensed_umap-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-08 16:07:52.483173 lensed_umap-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 16:34:43.000000 lensed_umap-0.1.1/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 16:34:43.000000 lensed_umap-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 16:34:43.000000 lensed_umap-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-14 16:34:43.000000 lensed_umap-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-14 16:34:43.000000 lensed_umap-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/_static/initial_umap.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14959 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/_static/lensed_umap.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/lensed_umap/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/lensed_umap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/lensed_umap/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/lensed_umap/fast_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/lensed_umap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/lensed_umap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-14 16:34:44.000000 lensed_umap-0.1.1/lensed_umap/tests/test_lenses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:35:24.932623 lensed_umap-0.1.1/lensed_umap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-14 16:35:24.000000 lensed_umap-0.1.1/lensed_umap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 16:35:24.000000 lensed_umap-0.1.1/lensed_umap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:35:24.000000 lensed_umap-0.1.1/lensed_umap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 16:35:24.000000 lensed_umap-0.1.1/lensed_umap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 16:35:24.000000 lensed_umap-0.1.1/lensed_umap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 16:34:45.000000 lensed_umap-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 16:34:45.000000 lensed_umap-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-14 16:35:24.936623 lensed_umap-0.1.1/setup.cfg
```

### Comparing `lensed_umap-0.1.0/LICENSE` & `lensed_umap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/PKG-INFO` & `lensed_umap-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensed_umap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Untangle UMAP with lenses.
 Home-page: https://github.com/vda-lab/lensed_umap
 Author: Jelmer Bot
 Author-email: jelmer.bot@uhasselt.be
 License: BSD-3-Clause license
 Project-URL: Code, https://github.com/vda-lab/lensed_umap
 Project-URL: Issue tracker, https://github.com/vda-lab/lensed_umap/issues
@@ -78,22 +78,25 @@
 ```
 
 ![Lensed model](docs/_static/lensed_umap.png)
 
 
 ## Example Notebooks
 
-A notebook demonstrating how the package works is available at
-[How lensed UMAP Works](https://nbviewer.org/github/vda-lab/lensed_umap/blob/master/notebooks/01_How_lensed_UMAP_works.ipynb). 
-The other notebooks demonstrate lenses on several data sets and 
-contain the analyses presented in our paper.
+A notebook demonstrating how the package works is available at 
+[How lensed UMAP Works](https://nbviewer.org/github/vda-lab/lensed_umap/blob/master/notebooks/01_How_lensed_UMAP_works.ipynb).
+The other notebooks demonstrate lenses on several data sets and contain the
+analyses presented in our paper. The datasets we used as input and the data
+generated by our notebooks are stored using [git lfs](https://git-lfs.com/),
+which turns the files in this repository into versioned links to the actual data
+files. Their documentation explains how to retrieve the actual data files.
 
 ## Installing
 
-`lensed_umap`` is available on PyPI:
+`lensed_umap` is available on PyPI:
 
 ```bash
 pip install lensed_umap
 ```
 
 ## Citing
```

### Comparing `lensed_umap-0.1.0/README.md` & `lensed_umap-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -51,22 +51,25 @@
 ```
 
 ![Lensed model](docs/_static/lensed_umap.png)
 
 
 ## Example Notebooks
 
-A notebook demonstrating how the package works is available at
-[How lensed UMAP Works](https://nbviewer.org/github/vda-lab/lensed_umap/blob/master/notebooks/01_How_lensed_UMAP_works.ipynb). 
-The other notebooks demonstrate lenses on several data sets and 
-contain the analyses presented in our paper.
+A notebook demonstrating how the package works is available at 
+[How lensed UMAP Works](https://nbviewer.org/github/vda-lab/lensed_umap/blob/master/notebooks/01_How_lensed_UMAP_works.ipynb).
+The other notebooks demonstrate lenses on several data sets and contain the
+analyses presented in our paper. The datasets we used as input and the data
+generated by our notebooks are stored using [git lfs](https://git-lfs.com/),
+which turns the files in this repository into versioned links to the actual data
+files. Their documentation explains how to retrieve the actual data files.
 
 ## Installing
 
-`lensed_umap`` is available on PyPI:
+`lensed_umap` is available on PyPI:
 
 ```bash
 pip install lensed_umap
 ```
 
 ## Citing
```

### Comparing `lensed_umap-0.1.0/docs/Makefile` & `lensed_umap-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/docs/_static/initial_umap.png` & `lensed_umap-0.1.1/docs/_static/initial_umap.png`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/docs/_static/lensed_umap.png` & `lensed_umap-0.1.1/docs/_static/lensed_umap.png`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/docs/_templates/layout.html` & `lensed_umap-0.1.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/docs/conf.py` & `lensed_umap-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/docs/index.rst` & `lensed_umap-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/docs/make.bat` & `lensed_umap-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/lensed_umap/api.py` & `lensed_umap-0.1.1/lensed_umap/api.py`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/lensed_umap/fast_impl.py` & `lensed_umap-0.1.1/lensed_umap/fast_impl.py`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/lensed_umap/tests/test_lenses.py` & `lensed_umap-0.1.1/lensed_umap/tests/test_lenses.py`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/lensed_umap.egg-info/PKG-INFO` & `lensed_umap-0.1.1/lensed_umap.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensed_umap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Untangle UMAP with lenses.
 Home-page: https://github.com/vda-lab/lensed_umap
 Author: Jelmer Bot
 Author-email: jelmer.bot@uhasselt.be
 License: BSD-3-Clause license
 Project-URL: Code, https://github.com/vda-lab/lensed_umap
 Project-URL: Issue tracker, https://github.com/vda-lab/lensed_umap/issues
@@ -78,22 +78,25 @@
 ```
 
 ![Lensed model](docs/_static/lensed_umap.png)
 
 
 ## Example Notebooks
 
-A notebook demonstrating how the package works is available at
-[How lensed UMAP Works](https://nbviewer.org/github/vda-lab/lensed_umap/blob/master/notebooks/01_How_lensed_UMAP_works.ipynb). 
-The other notebooks demonstrate lenses on several data sets and 
-contain the analyses presented in our paper.
+A notebook demonstrating how the package works is available at 
+[How lensed UMAP Works](https://nbviewer.org/github/vda-lab/lensed_umap/blob/master/notebooks/01_How_lensed_UMAP_works.ipynb).
+The other notebooks demonstrate lenses on several data sets and contain the
+analyses presented in our paper. The datasets we used as input and the data
+generated by our notebooks are stored using [git lfs](https://git-lfs.com/),
+which turns the files in this repository into versioned links to the actual data
+files. Their documentation explains how to retrieve the actual data files.
 
 ## Installing
 
-`lensed_umap`` is available on PyPI:
+`lensed_umap` is available on PyPI:
 
 ```bash
 pip install lensed_umap
 ```
 
 ## Citing
```

### Comparing `lensed_umap-0.1.0/lensed_umap.egg-info/SOURCES.txt` & `lensed_umap-0.1.1/lensed_umap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lensed_umap-0.1.0/setup.cfg` & `lensed_umap-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lensed_umap
-version = 0.1.0
+version = 0.1.1
 description = Untangle UMAP with lenses.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause license
 author = Jelmer Bot
 author_email = jelmer.bot@uhasselt.be
 url = https://github.com/vda-lab/lensed_umap
```

