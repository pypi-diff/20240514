# Comparing `tmp/summarytools-0.2.3.tar.gz` & `tmp/summarytools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summarytools-0.2.3.tar", last modified: Mon Nov 21 10:10:25 2022, max compression
+gzip compressed data, was "summarytools-0.3.0.tar", last modified: Sun May 12 07:28:27 2024, max compression
```

## Comparing `summarytools-0.2.3.tar` & `summarytools-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-11-21 10:10:25.288657 summarytools-0.2.3/
--rw-rw-rw-   0        0        0     1091 2022-11-20 00:30:45.000000 summarytools-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2886 2022-11-21 10:10:25.289657 summarytools-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1896 2022-11-20 00:30:45.000000 summarytools-0.2.3/README.md
--rw-rw-rw-   0        0        0      198 2022-11-20 00:30:45.000000 summarytools-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       85 2022-11-21 10:10:25.290658 summarytools-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     8703 2022-11-21 10:07:03.000000 summarytools-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-21 10:10:25.256655 summarytools-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2022-11-21 10:10:25.268657 summarytools-0.2.3/src/summarytools/
--rw-rw-rw-   0        0        0      104 2022-11-21 10:06:52.000000 summarytools-0.2.3/src/summarytools/__init__.py
--rw-rw-rw-   0        0        0     7367 2022-11-21 10:06:06.000000 summarytools-0.2.3/src/summarytools/htmlwidgets.py
--rw-rw-rw-   0        0        0     8804 2022-11-20 07:16:36.000000 summarytools-0.2.3/src/summarytools/summarytools.py
-drwxrwxrwx   0        0        0        0 2022-11-21 10:10:25.288657 summarytools-0.2.3/src/summarytools.egg-info/
--rw-rw-rw-   0        0        0     2886 2022-11-21 10:10:25.000000 summarytools-0.2.3/src/summarytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2022-11-21 10:10:25.000000 summarytools-0.2.3/src/summarytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-21 10:10:25.000000 summarytools-0.2.3/src/summarytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2022-11-21 10:10:25.000000 summarytools-0.2.3/src/summarytools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-21 10:10:25.000000 summarytools-0.2.3/src/summarytools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 07:28:27.173959 summarytools-0.3.0/
+-rw-rw-rw-   0        0        0    11556 2023-04-17 02:58:14.000000 summarytools-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3347 2024-05-12 07:28:27.173959 summarytools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2357 2023-04-17 03:40:40.000000 summarytools-0.3.0/README.md
+-rw-rw-rw-   0        0        0      198 2023-04-15 01:51:35.000000 summarytools-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-05-12 07:28:27.174958 summarytools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     8703 2024-04-20 23:49:18.000000 summarytools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:28:27.158960 summarytools-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 07:28:27.165958 summarytools-0.3.0/src/summarytools/
+-rw-rw-rw-   0        0        0      170 2024-04-21 03:04:11.000000 summarytools-0.3.0/src/summarytools/__init__.py
+-rw-rw-rw-   0        0        0     7367 2023-04-15 01:51:35.000000 summarytools-0.3.0/src/summarytools/htmlwidgets.py
+-rw-rw-rw-   0        0        0     4305 2024-04-21 09:07:54.000000 summarytools-0.3.0/src/summarytools/summary.py
+-rw-rw-rw-   0        0        0     5858 2024-04-21 02:55:06.000000 summarytools-0.3.0/src/summarytools/summarytools.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:28:27.172960 summarytools-0.3.0/src/summarytools.egg-info/
+-rw-rw-rw-   0        0        0     3347 2024-05-12 07:28:27.000000 summarytools-0.3.0/src/summarytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-12 07:28:27.000000 summarytools-0.3.0/src/summarytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 07:28:27.000000 summarytools-0.3.0/src/summarytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-05-12 07:28:27.000000 summarytools-0.3.0/src/summarytools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 07:28:27.000000 summarytools-0.3.0/src/summarytools.egg-info/top_level.txt
```

### Comparing `summarytools-0.2.3/PKG-INFO` & `summarytools-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summarytools
-Version: 0.2.3
+Version: 0.3.0
 Summary: summarytools in jupyter notebook
 Home-page: https://github.com/6chaoran/jupyter-summarytools
 Author: Liu Chaoran
 Author-email: 6chaoran@gmail.com
 Project-URL: Bug Reports, https://github.com/6chaoran/jupyter-summarytools/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
@@ -19,38 +19,42 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
+![GitHub](https://img.shields.io/github/license/6chaoran/jupyter-summarytools) 
+
+![PyPI](https://img.shields.io/pypi/v/summarytools?color=blue) ![PyPI - Status](https://img.shields.io/pypi/status/summarytools?color=blue) ![PyPI - Downloads](https://img.shields.io/pypi/dm/summarytools?color=blue) ![GitHub last commit](https://img.shields.io/github/last-commit/6chaoran/jupyter-summarytools?color=blue)
+
 # DataFrame Summary Tools in Jupyter Notebook
 
 This is python version of `summarytools`, which is used to generate standardized and comprehensive summary of dataframe in Jupyter Notebooks.
 
 The idea is originated from the `summarytools` R package (https://github.com/dcomtois/summarytools).
 
 * Only `dfSummary` function is made available for now
 * Added two html widgets to avoid displaying lengthy content
     + [collapsible summary](#collapsible-summary) 
     + [tabbed summary](#tabbed-summary)
 
 # Installation
 
 ```
-pip install jupyter-summarytools
+pip install summarytools
 ```
 
 ## Dependencies
 1. python 3.6+
 2. pandas >= 1.4.0
 
 # Quick Start
 
-the quick-start notebook is available in [here](quick-start.ipynb)
+the quick-start notebook is available in [here](https://github.com/6chaoran/jupyter-summarytools/blob/master/quick-start.ipynb)
 
 out-of-box `dfSummary` function will generate a HTML based data frame summary.
 
 ```py
 import pandas as pd
 from summarytools import dfSummary
 titanic = pd.read_csv('./data/titanic.csv')
```

### Comparing `summarytools-0.2.3/README.md` & `summarytools-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+![GitHub](https://img.shields.io/github/license/6chaoran/jupyter-summarytools) 
+
+![PyPI](https://img.shields.io/pypi/v/summarytools?color=blue) ![PyPI - Status](https://img.shields.io/pypi/status/summarytools?color=blue) ![PyPI - Downloads](https://img.shields.io/pypi/dm/summarytools?color=blue) ![GitHub last commit](https://img.shields.io/github/last-commit/6chaoran/jupyter-summarytools?color=blue)
+
 # DataFrame Summary Tools in Jupyter Notebook
 
 This is python version of `summarytools`, which is used to generate standardized and comprehensive summary of dataframe in Jupyter Notebooks.
 
 The idea is originated from the `summarytools` R package (https://github.com/dcomtois/summarytools).
 
 * Only `dfSummary` function is made available for now
 * Added two html widgets to avoid displaying lengthy content
     + [collapsible summary](#collapsible-summary) 
     + [tabbed summary](#tabbed-summary)
 
 # Installation
 
 ```
-pip install jupyter-summarytools
+pip install summarytools
 ```
 
 ## Dependencies
 1. python 3.6+
 2. pandas >= 1.4.0
 
 # Quick Start
 
-the quick-start notebook is available in [here](quick-start.ipynb)
+the quick-start notebook is available in [here](https://github.com/6chaoran/jupyter-summarytools/blob/master/quick-start.ipynb)
 
 out-of-box `dfSummary` function will generate a HTML based data frame summary.
 
 ```py
 import pandas as pd
 from summarytools import dfSummary
 titanic = pd.read_csv('./data/titanic.csv')
```

### Comparing `summarytools-0.2.3/setup.py` & `summarytools-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="summarytools",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.2.3",  # Required
+    version="0.3.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="summarytools in jupyter notebook",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `summarytools-0.2.3/src/summarytools/htmlwidgets.py` & `summarytools-0.3.0/src/summarytools/htmlwidgets.py`

 * *Files identical despite different names*

### Comparing `summarytools-0.2.3/src/summarytools.egg-info/PKG-INFO` & `summarytools-0.3.0/src/summarytools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summarytools
-Version: 0.2.3
+Version: 0.3.0
 Summary: summarytools in jupyter notebook
 Home-page: https://github.com/6chaoran/jupyter-summarytools
 Author: Liu Chaoran
 Author-email: 6chaoran@gmail.com
 Project-URL: Bug Reports, https://github.com/6chaoran/jupyter-summarytools/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
@@ -19,38 +19,42 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
+![GitHub](https://img.shields.io/github/license/6chaoran/jupyter-summarytools) 
+
+![PyPI](https://img.shields.io/pypi/v/summarytools?color=blue) ![PyPI - Status](https://img.shields.io/pypi/status/summarytools?color=blue) ![PyPI - Downloads](https://img.shields.io/pypi/dm/summarytools?color=blue) ![GitHub last commit](https://img.shields.io/github/last-commit/6chaoran/jupyter-summarytools?color=blue)
+
 # DataFrame Summary Tools in Jupyter Notebook
 
 This is python version of `summarytools`, which is used to generate standardized and comprehensive summary of dataframe in Jupyter Notebooks.
 
 The idea is originated from the `summarytools` R package (https://github.com/dcomtois/summarytools).
 
 * Only `dfSummary` function is made available for now
 * Added two html widgets to avoid displaying lengthy content
     + [collapsible summary](#collapsible-summary) 
     + [tabbed summary](#tabbed-summary)
 
 # Installation
 
 ```
-pip install jupyter-summarytools
+pip install summarytools
 ```
 
 ## Dependencies
 1. python 3.6+
 2. pandas >= 1.4.0
 
 # Quick Start
 
-the quick-start notebook is available in [here](quick-start.ipynb)
+the quick-start notebook is available in [here](https://github.com/6chaoran/jupyter-summarytools/blob/master/quick-start.ipynb)
 
 out-of-box `dfSummary` function will generate a HTML based data frame summary.
 
 ```py
 import pandas as pd
 from summarytools import dfSummary
 titanic = pd.read_csv('./data/titanic.csv')
```

