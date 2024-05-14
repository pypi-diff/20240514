# Comparing `tmp/deepmodeling_sphinx-0.2.5.tar.gz` & `tmp/deepmodeling_sphinx-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmodeling_sphinx-0.2.5.tar", last modified: Sun Dec 17 21:16:36 2023, max compression
+gzip compressed data, was "deepmodeling_sphinx-0.2.6.tar", last modified: Tue May 14 20:14:16 2024, max compression
```

## Comparing `deepmodeling_sphinx-0.2.5.tar` & `deepmodeling_sphinx-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 21:16:36.092038 deepmodeling_sphinx-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 21:16:36.088038 deepmodeling_sphinx-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 21:16:36.088038 deepmodeling_sphinx-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2023-12-17 21:16:36.092038 deepmodeling_sphinx-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 21:16:36.092038 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/banner.css
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/banner.html
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/banner.js
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/dark_rtd.css
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/inject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 21:16:36.092038 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2023-12-17 21:16:36.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-17 21:16:36.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 21:16:36.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-17 21:16:36.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-17 21:16:36.000000 deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 21:16:36.092038 deepmodeling_sphinx-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-17 21:16:24.000000 deepmodeling_sphinx-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 21:16:36.092038 deepmodeling_sphinx-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.906937 deepmodeling_sphinx-0.2.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.906937 deepmodeling_sphinx-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.906937 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/dark_rtd.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/inject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/setup.cfg
```

### Comparing `deepmodeling_sphinx-0.2.5/.github/workflows/release.yml` & `deepmodeling_sphinx-0.2.6/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release-to-pypi:
     name: Release to pypi
     runs-on: ubuntu-latest
     permissions:
         # IMPORTANT: this permission is mandatory for trusted publishing
         id-token: write
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Setup python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.x
         architecture: x64
     - name: Install dependencies
       run: python -m pip install build
     - run: python -m build
     - name: Publish a Python distribution to PyPI
```

### Comparing `deepmodeling_sphinx-0.2.5/.gitignore` & `deepmodeling_sphinx-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.5/.readthedocs.yaml` & `deepmodeling_sphinx-0.2.6/.readthedocs.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 version: 2
 
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-22.04
   tools:
     python: "3.10"
-
+  jobs:
+    post_create_environment:
+      - pip install uv
+    post_install:
+      - VIRTUAL_ENV=$READTHEDOCS_VIRTUALENV_PATH uv pip install -r docs/requirements.txt
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
-   configuration: docs/conf.py
+  configuration: docs/conf.py
 
 # If using Sphinx, optionally build your docs in additional formats such as PDF
 formats: all
-
-# Optionally declare the Python requirements required to build your docs
-python:
-   install:
-   - requirements: docs/requirements.txt
```

### Comparing `deepmodeling_sphinx-0.2.5/LICENSE` & `deepmodeling_sphinx-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.5/PKG-INFO` & `deepmodeling_sphinx-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepmodeling_sphinx
-Version: 0.2.5
+Version: 0.2.6
 Summary: Sphinx extension for DeepModeling projects.
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -174,15 +174,15 @@
 Project-URL: repository, https://github.com/deepmodeling/deepmodeling_sphinx
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sphinx
-Requires-Dist: htmlmin
+Requires-Dist: minify-html-onepass
 Requires-Dist: jsmin
 Requires-Dist: cssmin
 Requires-Dist: jinja2
 
 # deepmodeling_sphinx
 
 [![pip install](https://img.shields.io/pypi/dm/deepmodeling_sphinx?label=pip%20install&logo=pypi)](https://pypi.org/project/deepmodeling_sphinx)
```

### Comparing `deepmodeling_sphinx-0.2.5/README.md` & `deepmodeling_sphinx-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/authors.py` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/authors.py`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/banner.css` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,587 +1,585 @@
 /* The initial version is taken from
 https://github.com/pytorch/pytorch_sphinx_theme
 under MIT license
 */
 
 .header-container {
-    max-width: none;
-    margin-top: 4px;
+  max-width: none;
+  margin-top: 4px;
 }
 
 @media screen and (min-width: 1101px) {
-    .header-container {
-        margin-top: 0;
-    }
+  .header-container {
+    margin-top: 0;
+  }
 }
 
 @media screen and (min-width: 1600px) {
-    .header-container {
-        margin-top: 0;
-    }
+  .header-container {
+    margin-top: 0;
+  }
 }
 
 .container-fluid.header-holder {
-    padding-right: 0;
-    padding-left: 0;
-    /* pydata theme has z-index 1030; we should be the largest */
-    z-index: 2000;
+  padding-right: 0;
+  padding-left: 0;
+  /* pydata theme has z-index 1030; we should be the largest */
+  z-index: 2000;
 }
 
 .header-holder .container {
-    max-width: none;
-    padding-right: 1.875rem;
-    padding-left: 1.875rem;
+  max-width: none;
+  padding-right: 1.875rem;
+  padding-left: 1.875rem;
 }
 
 @media screen and (min-width: 1101px) {
-    .header-holder .container {
-        padding-right: 1.875rem;
-        padding-left: 1.875rem;
-    }
+  .header-holder .container {
+    padding-right: 1.875rem;
+    padding-left: 1.875rem;
+  }
 }
 
 .header-holder .main-menu {
-    -webkit-box-pack: unset;
-    -ms-flex-pack: unset;
-    justify-content: unset;
-    position: relative;
+  -webkit-box-pack: unset;
+  -ms-flex-pack: unset;
+  justify-content: unset;
+  position: relative;
 }
 
 @media screen and (min-width: 1101px) {
-    .header-holder .main-menu ul {
-        padding-left: 0;
-        margin-left: 26%;
-    }
+  .header-holder .main-menu ul {
+    padding-left: 0;
+    margin-left: 26%;
+  }
 }
 
 @media screen and (min-width: 1600px) {
-    .header-holder .main-menu ul {
-        padding-left: 38px;
-        margin-left: 310px;
-    }
+  .header-holder .main-menu ul {
+    padding-left: 38px;
+    margin-left: 310px;
+  }
 }
 
-
 .header-holder {
-    height: 68px;
-    -webkit-box-align: center;
-    -ms-flex-align: center;
-    align-items: center;
-    display: -webkit-box;
-    display: -ms-flexbox;
-    display: flex;
-    left: 0;
-    margin-left: auto;
-    margin-right: auto;
-    position: fixed;
-    right: 0;
-    top: 0;
-    width: 100%;
-    z-index: 9999;
-    background-color: #ffffff;
-    border-bottom: 1px solid #e2e2e2;
-}
-
-.wy-nav-side, .shift {
-    margin-top: 68px;
+  height: 68px;
+  -webkit-box-align: center;
+  -ms-flex-align: center;
+  align-items: center;
+  display: -webkit-box;
+  display: -ms-flexbox;
+  display: flex;
+  left: 0;
+  margin-left: auto;
+  margin-right: auto;
+  position: fixed;
+  right: 0;
+  top: 0;
+  width: 100%;
+  z-index: 9999;
+  background-color: #ffffff;
+  border-bottom: 1px solid #e2e2e2;
+}
+
+.wy-nav-side,
+.shift {
+  margin-top: 68px;
 }
 
 @media screen and (min-width: 1100px) {
+  .wy-nav-side {
+    margin-top: 90px;
+  }
 
-    .wy-nav-side {
-        margin-top: 90px;
-    }
-
-    .header-holder {
-        height: 90px;
-    }
+  .header-holder {
+    height: 90px;
+  }
 }
 
 .header-container {
-    position: relative;
-    display: -webkit-box;
-    display: -ms-flexbox;
-    display: flex;
-    -webkit-box-align: center;
-    -ms-flex-align: center;
-    align-items: center;
+  position: relative;
+  display: -webkit-box;
+  display: -ms-flexbox;
+  display: flex;
+  -webkit-box-align: center;
+  -ms-flex-align: center;
+  align-items: center;
 }
 
 .header-container:before,
 .header-container:after {
-    content: "";
-    display: table;
+  content: "";
+  display: table;
 }
 
 .header-container:after {
-    clear: both;
+  clear: both;
 }
 
 .header-container {
-    *zoom: 1;
+  *zoom: 1;
 }
 
 @media screen and (min-width: 1100px) {
-    .header-container {
-        display: block;
-    }
+  .header-container {
+    display: block;
+  }
 }
 
 .header-logo {
-    height: 50px;
-    width: 50px;
-    background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/logos/deepmodeling.svg");
-    background-repeat: no-repeat;
-    background-size: 50px 50px;
-    display: block;
-    float: left;
-    z-index: 10;
+  height: 50px;
+  width: 50px;
+  background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/logos/deepmodeling.svg");
+  background-repeat: no-repeat;
+  background-size: 50px 50px;
+  display: block;
+  float: left;
+  z-index: 10;
 }
 
 .header-logo::after {
-    content: "DeepModeling";
-    font-size: 1.375rem;
-    margin-left: 60px;
-    padding-top: 10px;
-    display: block;
-    color: #262626;
+  content: "DeepModeling";
+  font-size: 1.375rem;
+  margin-left: 60px;
+  padding-top: 10px;
+  display: block;
+  color: #262626;
 }
 
 .main-menu ul li a {
-    color: #262626;
+  color: #262626;
 }
 
 @media screen and (min-width: 1100px) {
-    /* only fix for read the docs theme */
-    .wy-body-for-nav .header-logo {
-        background-size: 50px 50px;
-        position: fixed;
-        height: 50px;
-        width: 50px;
-        top: -8px;
-        float: none;
-        margin-top: 25px;
-    }
+  /* only fix for read the docs theme */
+  .wy-body-for-nav .header-logo {
+    background-size: 50px 50px;
+    position: fixed;
+    height: 50px;
+    width: 50px;
+    top: -8px;
+    float: none;
+    margin-top: 25px;
+  }
 }
 
 @media screen and (min-width: 1100px) {
-    .main-menu-open-button {
-        display: none;
-    }
+  .main-menu-open-button {
+    display: none;
+  }
 }
 
 .header-holder .main-menu {
-    display: none;
+  display: none;
 }
 
 @media screen and (min-width: 1100px) {
-    .header-holder .main-menu {
-        display: -webkit-box;
-        display: -ms-flexbox;
-        display: flex;
-        -webkit-box-align: center;
-        -ms-flex-align: center;
-        align-items: center;
-        -webkit-box-pack: end;
-        -ms-flex-pack: end;
-    }
-}
-
-.header-holder .main-menu ul {
+  .header-holder .main-menu {
     display: -webkit-box;
     display: -ms-flexbox;
     display: flex;
     -webkit-box-align: center;
     -ms-flex-align: center;
     align-items: center;
+    -webkit-box-pack: end;
+    -ms-flex-pack: end;
+  }
+}
+
+.header-holder .main-menu ul {
+  display: -webkit-box;
+  display: -ms-flexbox;
+  display: flex;
+  -webkit-box-align: center;
+  -ms-flex-align: center;
+  align-items: center;
 }
 
 .header-holder .main-menu ul li {
-    display: inline-block;
-    margin-right: 40px;
-    position: relative;
+  display: inline-block;
+  margin-right: 40px;
+  position: relative;
 }
 
 .header-holder .main-menu ul li.active:after {
-    content: "•";
-    bottom: -24px;
-    color: #1E90FF;
-    font-size: 1.375rem;
-    left: 0;
-    position: absolute;
-    right: 0;
-    text-align: center;
+  content: "•";
+  bottom: -24px;
+  color: #1e90ff;
+  font-size: 1.375rem;
+  left: 0;
+  position: absolute;
+  right: 0;
+  text-align: center;
 }
 
 .header-holder .main-menu ul li.active a {
-    color: #1E90FF;
+  color: #1e90ff;
 }
 
 .header-holder .main-menu ul li.docs-active:after {
-    content: "•";
-    bottom: -24px;
-    color: #1E90FF;
-    font-size: 1.375rem;
-    left: -24px;
-    position: absolute;
-    right: 0;
-    text-align: center;
+  content: "•";
+  bottom: -24px;
+  color: #1e90ff;
+  font-size: 1.375rem;
+  left: -24px;
+  position: absolute;
+  right: 0;
+  text-align: center;
 }
 
 .header-holder .main-menu ul li:last-of-type {
-    margin-right: 0;
+  margin-right: 0;
 }
 
 .header-holder .main-menu ul li a {
-    color: #000000;
-    font-size: 1.3rem;
-    letter-spacing: 0;
-    line-height: 2.125rem;
-    text-align: center;
-    text-decoration: none;
+  color: #000000;
+  font-size: 1.3rem;
+  letter-spacing: 0;
+  line-height: 2.125rem;
+  text-align: center;
+  text-decoration: none;
 }
 
 @media screen and (min-width: 1100px) {
-    .header-holder .main-menu ul li a:hover {
-        color: #1E90FF;
-    }
+  .header-holder .main-menu ul li a:hover {
+    color: #1e90ff;
+  }
 }
 
 .mobile-main-menu {
-    display: none;
+  display: none;
 }
 
 .mobile-main-menu.open {
-    background-color: #262626;
-    display: block;
-    height: 100%;
-    left: 0;
-    margin-left: auto;
-    margin-right: auto;
-    min-height: 100%;
-    position: fixed;
-    right: 0;
-    top: 0;
-    width: 100%;
-    z-index: 99999;
+  background-color: #262626;
+  display: block;
+  height: 100%;
+  left: 0;
+  margin-left: auto;
+  margin-right: auto;
+  min-height: 100%;
+  position: fixed;
+  right: 0;
+  top: 0;
+  width: 100%;
+  z-index: 99999;
 }
 
 .mobile-main-menu .container-fluid {
-    -webkit-box-align: center;
-    -ms-flex-align: center;
-    align-items: center;
-    display: -webkit-box;
-    display: -ms-flexbox;
-    display: flex;
-    height: 68px;
-    position: relative;
+  -webkit-box-align: center;
+  -ms-flex-align: center;
+  align-items: center;
+  display: -webkit-box;
+  display: -ms-flexbox;
+  display: flex;
+  height: 68px;
+  position: relative;
 }
 
 .mobile-main-menu .container-fluid:before,
 .mobile-main-menu .container-fluid:after {
-    content: "";
-    display: table;
+  content: "";
+  display: table;
 }
 
 .mobile-main-menu .container-fluid:after {
-    clear: both;
+  clear: both;
 }
 
 .mobile-main-menu .container-fluid {
-    *zoom: 1;
+  *zoom: 1;
 }
 
 .mobile-main-menu.open ul {
-    list-style-type: none;
-    padding: 0;
+  list-style-type: none;
+  padding: 0;
 }
 
 .mobile-main-menu.open ul li a,
 .mobile-main-menu.open .resources-mobile-menu-title {
-    font-size: 2rem;
-    color: #ffffff;
-    letter-spacing: 0;
-    line-height: 4rem;
-    text-decoration: none;
+  font-size: 2rem;
+  color: #ffffff;
+  letter-spacing: 0;
+  line-height: 4rem;
+  text-decoration: none;
 }
 
 .mobile-main-menu.open ul li.active a {
-    color: #1E90FF;
+  color: #1e90ff;
 }
 
 .main-menu-close-button {
-    background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/icon-close-opt.svg");
-    background-position: center center;
-    background-repeat: no-repeat;
-    background-size: 24px 24px;
-    height: 24px;
-    position: absolute;
-    right: 0;
-    width: 24px;
-    top: -4px;
+  background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/icon-close-opt.svg");
+  background-position: center center;
+  background-repeat: no-repeat;
+  background-size: 24px 24px;
+  height: 24px;
+  position: absolute;
+  right: 0;
+  width: 24px;
+  top: -4px;
 }
 
 .mobile-main-menu-header-container {
-    position: relative;
+  position: relative;
 }
 
 .mobile-main-menu-links-container {
-    display: -webkit-box;
-    display: -ms-flexbox;
-    display: flex;
-    -webkit-box-align: center;
-    -ms-flex-align: center;
-    align-items: center;
-    padding-left: 2.8125rem;
-    height: 90vh;
-    margin-top: -25px;
-    padding-top: 50%;
-    overflow-y: scroll;
+  display: -webkit-box;
+  display: -ms-flexbox;
+  display: flex;
+  -webkit-box-align: center;
+  -ms-flex-align: center;
+  align-items: center;
+  padding-left: 2.8125rem;
+  height: 90vh;
+  margin-top: -25px;
+  padding-top: 50%;
+  overflow-y: scroll;
 }
 
 .mobile-main-menu-links-container .main-menu {
-    height: 100vh;
+  height: 100vh;
 }
 
 .mobile-main-menu-links-container ul.resources-mobile-menu-items li {
-    padding-left: 15px;
+  padding-left: 15px;
 }
 
 .main-menu ul li .resources-dropdown a {
-    cursor: pointer;
+  cursor: pointer;
 }
 
 .main-menu ul li .dropdown-menu {
-    border-radius: 0;
-    padding: 0;
+  border-radius: 0;
+  padding: 0;
 }
 
 .main-menu ul li .dropdown-menu .dropdown-item {
-    color: #6c6c6d;
-    border-bottom: 1px solid #e2e2e2;
+  color: #6c6c6d;
+  border-bottom: 1px solid #e2e2e2;
 }
 
 .main-menu ul li .dropdown-menu .dropdown-item:last-of-type {
-    border-bottom-color: transparent;
+  border-bottom-color: transparent;
 }
 
 .main-menu ul li .dropdown-menu .dropdown-item:hover {
-    background-color: #1E90FF;
+  background-color: #1e90ff;
 }
 
 .main-menu ul li .dropdown-menu .dropdown-item p {
-    font-size: 1rem;
-    color: #979797;
+  font-size: 1rem;
+  color: #979797;
 }
 
 .main-menu ul li .dropdown-menu a.dropdown-item:hover {
-    color: #ffffff;
+  color: #ffffff;
 }
 
 .main-menu ul li .dropdown-menu a.dropdown-item:hover p {
-    color: #ffffff;
+  color: #ffffff;
 }
 
 .resources-dropdown-menu {
-    left: -75px;
-    width: 226px;
-    display: none;
-    position: absolute;
-    z-index: 1000;
-    display: none;
-    float: left;
-    min-width: 10rem;
-    padding: 0.5rem 0;
-    font-size: 1rem;
-    color: #212529;
-    text-align: left;
-    list-style: none;
-    background-color: #ffffff;
-    background-clip: padding-box;
-    border: 1px solid rgba(0, 0, 0, 0.15);
-    border-radius: 0.25rem;
+  left: -75px;
+  width: 226px;
+  display: none;
+  position: absolute;
+  z-index: 1000;
+  display: none;
+  float: left;
+  min-width: 10rem;
+  padding: 0.5rem 0;
+  font-size: 1rem;
+  color: #212529;
+  text-align: left;
+  list-style: none;
+  background-color: #ffffff;
+  background-clip: padding-box;
+  border: 1px solid rgba(0, 0, 0, 0.15);
+  border-radius: 0.25rem;
 }
 
 .resources-dropdown:hover .resources-dropdown-menu {
-    display: block;
+  display: block;
 }
 
 .main-menu ul li .resources-dropdown-menu {
-    border-radius: 0;
-    padding: 0;
+  border-radius: 0;
+  padding: 0;
 }
 
 .main-menu ul li.active:hover .resources-dropdown-menu {
-    display: block;
+  display: block;
 }
 
 .main-menu ul li .resources-dropdown-menu .dropdown-item {
-    color: #6c6c6d;
-    border-bottom: 1px solid #e2e2e2;
+  color: #6c6c6d;
+  border-bottom: 1px solid #e2e2e2;
 }
 
 .resources-dropdown .with-down-orange-arrow {
-    padding-right: 2rem;
-    position: relative;
-    background: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/chevron-down-black-opt.svg");
-    background-size: 14px 18px;
-    background-position: top 7px right 10px;
-    background-repeat: no-repeat;
+  padding-right: 2rem;
+  position: relative;
+  background: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/chevron-down-black-opt.svg");
+  background-size: 14px 18px;
+  background-position: top 7px right 10px;
+  background-repeat: no-repeat;
 }
 
 .with-down-arrow {
-    padding-right: 2rem;
-    position: relative;
-    background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/chevron-down-black-opt.svg");
-    background-size: 14px 18px;
-    background-position: top 7px right 10px;
-    background-repeat: no-repeat;
+  padding-right: 2rem;
+  position: relative;
+  background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/chevron-down-black-opt.svg");
+  background-size: 14px 18px;
+  background-position: top 7px right 10px;
+  background-repeat: no-repeat;
 }
 
 .with-down-arrow:hover {
-    background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/chevron-down-black-opt.svg");
-    background-repeat: no-repeat;
+  background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/chevron-down-black-opt.svg");
+  background-repeat: no-repeat;
 }
 
 .header-holder .main-menu ul li .resources-dropdown .doc-dropdown-option {
-    padding-top: 1rem;
+  padding-top: 1rem;
 }
 
 .header-holder .main-menu ul li a.nav-dropdown-item {
-    display: block;
-    font-size: 1rem;
-    line-height: 1.3125rem;
-    width: 100%;
-    padding: 0.25rem 1.5rem;
-    clear: both;
-    font-weight: 400;
-    color: #979797;
-    text-align: center;
-    background-color: transparent;
-    border-bottom: 1px solid #e2e2e2;
+  display: block;
+  font-size: 1rem;
+  line-height: 1.3125rem;
+  width: 100%;
+  padding: 0.25rem 1.5rem;
+  clear: both;
+  font-weight: 400;
+  color: #979797;
+  text-align: center;
+  background-color: transparent;
+  border-bottom: 1px solid #e2e2e2;
 }
 
 .header-holder .main-menu ul li a.nav-dropdown-item:last-of-type {
-    border-bottom-color: transparent;
+  border-bottom-color: transparent;
 }
 
 .header-holder .main-menu ul li a.nav-dropdown-item:hover {
-    background-color: #1E90FF;
-    color: white;
+  background-color: #1e90ff;
+  color: white;
 }
 
 .header-holder .main-menu ul li a.nav-dropdown-item .dropdown-title {
-    font-size: 1.125rem;
-    color: #6c6c6d;
-    letter-spacing: 0;
-    line-height: 34px;
+  font-size: 1.125rem;
+  color: #6c6c6d;
+  letter-spacing: 0;
+  line-height: 34px;
 }
 
 .header-holder .main-menu ul li a.nav-dropdown-item:hover .dropdown-title {
-    background-color: #1E90FF;
-    color: white;
+  background-color: #1e90ff;
+  color: white;
 }
 
 .main-menu-open-button {
-    background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/icon-menu-dots-dark-opt.svg");
-    background-position: center center;
-    background-size: 25px 7px;
-    background-repeat: no-repeat;
-    width: 25px;
-    height: 17px;
-    position: absolute;
-    right: 0;
-    top: 14px;
+  background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/icon-menu-dots-dark-opt.svg");
+  background-position: center center;
+  background-size: 25px 7px;
+  background-repeat: no-repeat;
+  width: 25px;
+  height: 17px;
+  position: absolute;
+  right: 0;
+  top: 14px;
 }
 
 @media screen and (min-width: 1100px) {
-    .main-menu-open-button {
-        display: none;
-    }
+  .main-menu-open-button {
+    display: none;
+  }
 }
 
 .tutorials-header .main-menu-open-button {
-    background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/icon-menu-dots-dark-opt.svg");
+  background-image: url("https://unpkg.com/@njzjz/icons@0.0.5/deepmodeling/icon-menu-dots-dark-opt.svg");
 }
 
-
 .container {
-    width: 100%;
-    padding-right: 15px;
-    padding-left: 15px;
-    margin-right: auto;
-    margin-left: auto;
+  width: 100%;
+  padding-right: 15px;
+  padding-left: 15px;
+  margin-right: auto;
+  margin-left: auto;
 }
 
 @media (min-width: 576px) {
-    .container {
-        max-width: 540px;
-    }
+  .container {
+    max-width: 540px;
+  }
 }
 
 @media (min-width: 768px) {
-    .container {
-        max-width: 720px;
-    }
+  .container {
+    max-width: 720px;
+  }
 }
 
 @media (min-width: 992px) {
-    .container {
-        max-width: 960px;
-    }
+  .container {
+    max-width: 960px;
+  }
 }
 
 @media (min-width: 1200px) {
-    .container {
-        max-width: 1140px;
-    }
+  .container {
+    max-width: 1140px;
+  }
 }
 
 .container-fluid {
-    width: 100%;
-    padding-right: 15px;
-    padding-left: 15px;
-    margin-right: auto;
-    margin-left: auto;
+  width: 100%;
+  padding-right: 15px;
+  padding-left: 15px;
+  margin-right: auto;
+  margin-left: auto;
 }
 
 .header-holder {
-    position: relative;
-    z-index: 201;
-  }
+  position: relative;
+  z-index: 201;
+}
 
 .wy-side-scroll {
-  height: calc(100% - 68px)!important;
+  height: calc(100% - 68px) !important;
 }
 
 @media screen and (min-width: 1100px) {
-    .wy-side-scroll {
-      height: calc(100% - 90px)!important;
-    }
+  .wy-side-scroll {
+    height: calc(100% - 90px) !important;
+  }
 }
 
 @media (prefers-color-scheme: dark) {
-    /* Dark mode */
-    .header-holder {
-        background-color: #1E1E1E;
-    }
-    .header-logo::after {
-        color: #ffffff;
-    }
-    .header-holder .main-menu ul li a {
-        color: #ffffff;
-    }
-    .resources-dropdown-menu {
-        color: #ffffff;
-        background-color: #1E1E1E;
-    }
-    .header-holder .main-menu ul li a.nav-dropdown-item {
-        color: #ffffff;
-    }
-    .header-holder .main-menu ul li a.nav-dropdown-item .dropdown-title {
-        color: #ffffff;
-    }
-    .wy-body-for-nav {
-        background-color: #1E1E1E;
-    }
+  /* Dark mode */
+  .header-holder {
+    background-color: #1e1e1e;
+  }
+  .header-logo::after {
+    color: #ffffff;
+  }
+  .header-holder .main-menu ul li a {
+    color: #ffffff;
+  }
+  .resources-dropdown-menu {
+    color: #ffffff;
+    background-color: #1e1e1e;
+  }
+  .header-holder .main-menu ul li a.nav-dropdown-item {
+    color: #ffffff;
+  }
+  .header-holder .main-menu ul li a.nav-dropdown-item .dropdown-title {
+    color: #ffffff;
+  }
+  .wy-body-for-nav {
+    background-color: #1e1e1e;
+  }
 }
```

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/banner.html` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,94 @@
 <link rel="preconnect" href="https://unpkg.com/" />
-<link rel="icon" href="https://unpkg.com/@njzjz/icons@0.0.5/logos/deepmodeling.svg" type="image/png">
+<link
+  rel="icon"
+  href="https://unpkg.com/@njzjz/icons@0.0.5/logos/deepmodeling.svg"
+  type="image/png"
+/>
 <!-- The initial version is taken from
 https://github.com/pytorch/pytorch_sphinx_theme
 under MIT license
 -->
 <div class="container-fluid header-holder tutorials-header" id="header-holder">
-    <div class="container">
-        <div class="header-container">
-            <a class="header-logo" href="https://deepmodeling.com" aria-label="deepmodeling"></a>
+  <div class="container">
+    <div class="header-container">
+      <a
+        class="header-logo"
+        href="https://deepmodeling.com"
+        aria-label="deepmodeling"
+      ></a>
 
-            <div class="main-menu">
-                <ul>
-                    {% for item in items %}
-                    <li class="{{ item.class }}">
-                    {% if item.subitem %}
-                        <div id="resourcesDropdownButton" data-toggle="resources-dropdown" class="resources-dropdown">
-                            <a href="{{ item.url }}" class="resource-option with-down-orange-arrow">
-                                {{ item.title }}
-                            </a>
-                            <div class="resources-dropdown-menu">
-                                {% for subitem in item.subitem %}
-                                <a class="doc-dropdown-option nav-dropdown-item"
-                                    href="{{ subitem.url }}">
-                                    <span class="dropdown-title">{{ subitem.title }}</span>
-                                    <p></p>
-                                </a>
-                                {% endfor %}
-                            </div>
-                        </div>
-                    {% else %}
-                        <a href="{{ item.url }}">{{ item.title }}</a>
-                    {% endif %}
-                    </li>
-                    {% endfor %}
-                </ul>
+      <div class="main-menu">
+        <ul>
+          {% for item in items %}
+          <li class="{{ item.class }}">
+            {% if item.subitem %}
+            <div
+              id="resourcesDropdownButton"
+              data-toggle="resources-dropdown"
+              class="resources-dropdown"
+            >
+              <a
+                href="{{ item.url }}"
+                class="resource-option with-down-orange-arrow"
+              >
+                {{ item.title }}
+              </a>
+              <div class="resources-dropdown-menu">
+                {% for subitem in item.subitem %}
+                <a
+                  class="doc-dropdown-option nav-dropdown-item"
+                  href="{{ subitem.url }}"
+                >
+                  <span class="dropdown-title">{{ subitem.title }}</span>
+                  <p></p>
+                </a>
+                {% endfor %}
+              </div>
             </div>
+            {% else %}
+            <a href="{{ item.url }}">{{ item.title }}</a>
+            {% endif %}
+          </li>
+          {% endfor %}
+        </ul>
+      </div>
 
-            <a class="main-menu-open-button" href="#" data-behavior="open-mobile-menu"></a>
-        </div>
+      <a
+        class="main-menu-open-button"
+        href="#"
+        data-behavior="open-mobile-menu"
+      ></a>
     </div>
+  </div>
 </div>
 
 <div class="mobile-main-menu">
-    <div class="container-fluid">
-        <div class="container">
-            <div class="mobile-main-menu-header-container">
-                <a class="header-logo" href="https://deepmodeling.com" aria-label="deepmodeling"></a>
-                <a class="main-menu-close-button" href="#" data-behavior="close-mobile-menu"></a>
-            </div>
-        </div>
+  <div class="container-fluid">
+    <div class="container">
+      <div class="mobile-main-menu-header-container">
+        <a
+          class="header-logo"
+          href="https://deepmodeling.com"
+          aria-label="deepmodeling"
+        ></a>
+        <a
+          class="main-menu-close-button"
+          href="#"
+          data-behavior="close-mobile-menu"
+        ></a>
+      </div>
     </div>
+  </div>
 
-    <div class="mobile-main-menu-links-container">
-        <div class="main-menu">
-            <ul>
-                {% for item in items %}
-                <li>
-                    <a href="{{ item.url }}">{{ item.title }}</a>
-                </li>
-                {% endfor %}
-            </ul>
-        </div>
+  <div class="mobile-main-menu-links-container">
+    <div class="main-menu">
+      <ul>
+        {% for item in items %}
+        <li>
+          <a href="{{ item.url }}">{{ item.title }}</a>
+        </li>
+        {% endfor %}
+      </ul>
     </div>
+  </div>
 </div>
```

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/banner.js` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,37 +1,37 @@
 /* The initial version is taken from
 https://github.com/pytorch/pytorch_sphinx_theme
 under MIT license
 */
 window.mobileMenu = {
     bind: function() {
-        $("[data-behavior='open-mobile-menu']").on('click', function(e) {
+        $("[data-behavior='open-mobile-menu']").on("click", function(e) {
             e.preventDefault();
             $(".mobile-main-menu").addClass("open");
-            $("body").addClass('no-scroll');
+            $("body").addClass("no-scroll");
 
             mobileMenu.listenForResize();
         });
 
-        $("[data-behavior='close-mobile-menu']").on('click', function(e) {
+        $("[data-behavior='close-mobile-menu']").on("click", function(e) {
             e.preventDefault();
             mobileMenu.close();
         });
     },
 
     listenForResize: function() {
-        $(window).on('resize.ForMobileMenu', function() {
+        $(window).on("resize.ForMobileMenu", function() {
             if ($(this).width() > 768) {
                 mobileMenu.close();
             }
         });
     },
 
     close: function() {
         $(".mobile-main-menu").removeClass("open");
-        $("body").removeClass('no-scroll');
-        $(window).off('resize.ForMobileMenu');
-    }
+        $("body").removeClass("no-scroll");
+        $(window).off("resize.ForMobileMenu");
+    },
 };
 $(document).ready(function() {
     mobileMenu.bind();
 });
```

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/config.py` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/config.py`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx/inject.py` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/inject.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import types
 from pathlib import Path
 from typing import Any, Dict
 
-import htmlmin
+import minify_html_onepass
 from cssmin import cssmin
 from jinja2 import Template
 from jsmin import jsmin
 from sphinx.application import Sphinx
 from sphinx.util.fileutil import copy_asset_file
 
 from .config import active_class, icp_no, sitemap
@@ -116,15 +116,15 @@
 
 def minify_html_files(app, pagename, templatename, context, doctree):
     if not hasattr(app.builder.templates.render, "_deepmodeling_minified"):
         old_render = app.builder.templates.render
 
         def render(self, template, render_context):
             content = old_render(template, render_context)
-            return htmlmin.minify(content)
+            return minify_html_onepass.minify(content, minify_js=True)
 
         render.__dict__.update(old_render.__dict__)
         render._deepmodeling_minified = True
         app.builder.templates.render = types.MethodType(render, app.builder.templates)
 
 
 def minify_js_files(app, exception):
```

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/PKG-INFO` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: deepmodeling-sphinx
-Version: 0.2.5
+Name: deepmodeling_sphinx
+Version: 0.2.6
 Summary: Sphinx extension for DeepModeling projects.
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -174,15 +174,15 @@
 Project-URL: repository, https://github.com/deepmodeling/deepmodeling_sphinx
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sphinx
-Requires-Dist: htmlmin
+Requires-Dist: minify-html-onepass
 Requires-Dist: jsmin
 Requires-Dist: cssmin
 Requires-Dist: jinja2
 
 # deepmodeling_sphinx
 
 [![pip install](https://img.shields.io/pypi/dm/deepmodeling_sphinx?label=pip%20install&logo=pypi)](https://pypi.org/project/deepmodeling_sphinx)
```

### Comparing `deepmodeling_sphinx-0.2.5/deepmodeling_sphinx.egg-info/SOURCES.txt` & `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+.git_archival.txt
+.gitattributes
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
+.github/dependabot.yml
+.github/workflows/mirror_gitee.yml
 .github/workflows/release.yml
 deepmodeling_sphinx/__init__.py
 deepmodeling_sphinx/authors.py
 deepmodeling_sphinx/banner.css
 deepmodeling_sphinx/banner.html
 deepmodeling_sphinx/banner.js
 deepmodeling_sphinx/config.py
```

### Comparing `deepmodeling_sphinx-0.2.5/docs/conf.py` & `deepmodeling_sphinx-0.2.6/docs/conf.py`

 * *Files identical despite different names*

