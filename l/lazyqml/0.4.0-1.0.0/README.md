# Comparing `tmp/lazyqml-0.4.0.tar.gz` & `tmp/lazyqml-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.4.0.tar", last modified: Fri May 10 09:57:56 2024, max compression
+gzip compressed data, was "lazyqml-1.0.0.tar", last modified: Tue May 14 11:04:06 2024, max compression
```

## Comparing `lazyqml-0.4.0.tar` & `lazyqml-1.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.269067 lazyqml-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.261067 lazyqml-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.265067 lazyqml-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.265067 lazyqml-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 09:57:45.000000 lazyqml-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 09:57:45.000000 lazyqml-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 09:57:45.000000 lazyqml-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 09:57:45.000000 lazyqml-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:57:56.269067 lazyqml-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 09:57:45.000000 lazyqml-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.265067 lazyqml-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.265067 lazyqml-0.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.269067 lazyqml-0.4.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 09:57:45.000000 lazyqml-0.4.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.269067 lazyqml-0.4.0/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 09:57:45.000000 lazyqml-0.4.0/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31488 2024-05-10 09:57:45.000000 lazyqml-0.4.0/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    41111 2024-05-10 09:57:45.000000 lazyqml-0.4.0/lazyqml/supervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.269067 lazyqml-0.4.0/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:57:56.000000 lazyqml-0.4.0/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 09:57:56.000000 lazyqml-0.4.0/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:57:56.000000 lazyqml-0.4.0/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 09:57:56.000000 lazyqml-0.4.0/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 09:57:56.000000 lazyqml-0.4.0/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:57:56.000000 lazyqml-0.4.0/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-10 09:57:45.000000 lazyqml-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 09:57:45.000000 lazyqml-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 09:57:45.000000 lazyqml-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:57:45.000000 lazyqml-0.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:57:56.269067 lazyqml-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:57:56.269067 lazyqml-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 09:57:45.000000 lazyqml-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 09:57:45.000000 lazyqml-0.4.0/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.386223 lazyqml-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.378223 lazyqml-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.382223 lazyqml-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.382223 lazyqml-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 11:03:52.000000 lazyqml-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-14 11:03:52.000000 lazyqml-1.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 11:03:52.000000 lazyqml-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 11:03:52.000000 lazyqml-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-14 11:04:06.386223 lazyqml-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 11:03:52.000000 lazyqml-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.382223 lazyqml-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.382223 lazyqml-1.0.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.382223 lazyqml-1.0.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-14 11:03:52.000000 lazyqml-1.0.0/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.382223 lazyqml-1.0.0/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-14 11:03:52.000000 lazyqml-1.0.0/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31697 2024-05-14 11:03:52.000000 lazyqml-1.0.0/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48360 2024-05-14 11:03:52.000000 lazyqml-1.0.0/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.386223 lazyqml-1.0.0/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-14 11:04:06.000000 lazyqml-1.0.0/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 11:04:06.000000 lazyqml-1.0.0/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:04:06.000000 lazyqml-1.0.0/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 11:04:06.000000 lazyqml-1.0.0/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-14 11:04:06.000000 lazyqml-1.0.0/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 11:04:06.000000 lazyqml-1.0.0/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-14 11:03:52.000000 lazyqml-1.0.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-14 11:03:52.000000 lazyqml-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-14 11:03:52.000000 lazyqml-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-14 11:03:52.000000 lazyqml-1.0.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:04:06.386223 lazyqml-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:04:06.386223 lazyqml-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 11:03:52.000000 lazyqml-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 11:03:52.000000 lazyqml-1.0.0/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.4.0/.github/workflows/docs-build.yml` & `lazyqml-1.0.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/.github/workflows/docs.yml` & `lazyqml-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/.github/workflows/installation.yml` & `lazyqml-1.0.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/.github/workflows/macos.yml` & `lazyqml-1.0.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/.github/workflows/pypi.yml` & `lazyqml-1.0.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/.github/workflows/ubuntu.yml` & `lazyqml-1.0.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/.github/workflows/windows.yml` & `lazyqml-1.0.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/.gitignore` & `lazyqml-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/LICENSE` & `lazyqml-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/PKG-INFO` & `lazyqml-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.4.0
+Version: 1.0.0
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.4.0/docs/contributing.md` & `lazyqml-1.0.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/docs/installation.md` & `lazyqml-1.0.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/docs/usage.md` & `lazyqml-1.0.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/lazyqml/common.py` & `lazyqml-1.0.0/lazyqml/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 import inspect
 import os
 from sklearn.metrics import mean_squared_error, accuracy_score, log_loss
 from sklearn.decomposition import PCA
 from sklearn.svm import SVC
 import datetime
 import time
+import sklearn
+from sklearn.model_selection import RepeatedStratifiedKFold, LeaveOneOut
 from sklearn.pipeline import Pipeline
 from sklearn.impute import SimpleImputer, MissingIndicator
 from sklearn.preprocessing import StandardScaler, OneHotEncoder, OrdinalEncoder
 from sklearn.compose import ColumnTransformer
 from sklearn.utils import all_estimators
 from sklearn.base import RegressorMixin
 from sklearn.base import ClassifierMixin
@@ -281,30 +283,30 @@
     Returns:
         None
     """
     N=len(wires)
     for i in range(N):
         qml.RY(theta[i], wires = i)
     for i in range(N - 1):
-            qml.CNOT(wires = [i, i + 1])
+        qml.CNOT(wires = [i, i + 1])
 
 def get_ansatz(ansatz, n_qubits):
     """Returns the ansatz function and the number of parameters based on the specified ansatz type.
 
     Args:
         ansatz (str): ansatz type ('hardware_efficient', 'tree_tensor', 'HPzRx', or 'two_local')
         n_qubits (int): number of qubits
 
     Returns:
         tuple: ansatz function and the number of parameters
     """
     if ansatz == 'hardware_efficient':
         return hardware_efficient_ansatz, 3 * n_qubits
     if ansatz == 'tree_tensor':
-        return tree_tensor_ansatz , 2**(n_qubits+1)-1
+        return tree_tensor_ansatz , 2**(n_qubits-1)-1
     if ansatz == 'HPzRx':
         return HPzRx , n_qubits
     if ansatz == 'two_local':
         return TwoLocal, n_qubits
 """
  Auxiliary Functions
 """    
@@ -553,15 +555,15 @@
             roc_auc = roc_auc_score(y_test, y_predict)
         except Exception as exception:
             roc_auc = None
             if ignore_warnings is False:
                 verboseprint("ROC AUC couldn't be calculated")
                 verboseprint(exception)
 
-        return predictions, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
+        return params_per_layer*layers*n_estimators,predictions, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
 
 def evaluate_bagging_predictor_binary(qnn, n_estimators, max_features, max_samples, optimizer, n_qubits, runs, epochs, layers, ansatz, X_train, X_test, y_train, y_test, seed, verboseprint,ignore_warnings=True):
     """Evaluates a binary classification bagging predictor composed of a quantum neural network (QNN) ensemble.
 
     Args:
         qnn (function): quantum neural network function
         n_estimators (int): number of estimators in the bagging predictor
@@ -683,15 +685,15 @@
             roc_auc = roc_auc_score(y_test, y_predict)
         except Exception as exception:
             roc_auc = None
             if ignore_warnings is False:
                 verboseprint("ROC AUC couldn't be calculated")
                 verboseprint(exception)
 
-        return y_predict, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
+        return params_per_layer*layers*n_estimators ,y_predict, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
 
 
 
 def evaluate_full_model_predictor(qnn, optimizer, n_qubits, runs, epochs, layers, ansatz, X_train, X_test, y_train, y_test, seed,verboseprint,ignore_warnings=True):
     """Evaluates a full model predictor composed of a quantum neural network (QNN).
 
     Args:
@@ -773,15 +775,15 @@
             roc_auc = roc_auc_score(y_test, y_predict)
         except Exception as exception:
             roc_auc = None
             if ignore_warnings is False:
                 verboseprint("ROC AUC couldn't be calculated")
                 verboseprint(exception)
 
-        return y_predict, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
+        return params_per_layer*layers, y_predict, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
 
 
 def evaluate_full_model_predictor_binary(qnn, optimizer, n_qubits,  epochs, layers, ansatz, X_train, X_test, y_train, y_test, runs, seed, verboseprint, ignore_warnings=True):
     """Evaluates a binary classification full model predictor composed of a quantum neural network (QNN).
 
     Args:
         qnn (function): quantum neural network function
@@ -864,8 +866,8 @@
             roc_auc = roc_auc_score(y_test, y_predict)
         except Exception as exception:
             roc_auc = None
             if ignore_warnings is False:
                 verboseprint("ROC AUC couldn't be calculated")
                 verboseprint(exception)
 
-        return y_predict, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
+        return params_per_layer*layers, y_predict, accuracy_score(y_test,y_predict), balanced_accuracy_score(y_test, y_predict), f1_score(y_test, y_predict, average="weighted"), roc_auc
```

### Comparing `lazyqml-0.4.0/lazyqml/supervised.py` & `lazyqml-1.0.0/lazyqml/supervised.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,54 +7,89 @@
 """
 
 from .common import *
 import warnings
 warnings.filterwarnings("ignore")
 
 """
- Classifiers
+ Auxiliary functions
 """
+def adjust_nqubits(numClasses):
+    # Find the next power of 2 greater than numClasses
+    power = np.ceil(np.log2(numClasses))
+    nqubits = 2 ** power
+    
+    # Ensure nqubits is greater than numClasses
+    if nqubits <= numClasses:
+        nqubits *= 2
 
+    return int(nqubits)
 def _check_classifiers(array):
     allowed_keywords = {"all", "qsvm", "qnn", "qnn_bag"} 
     return all(keyword in allowed_keywords for keyword in array)
 def _check_embeddings(array):
     allowed_keywords = {"all", "amplitude_embedding", "ZZ_embedding", "rx_embedding", "rz_embedding", "ry_embedding"} 
     return all(keyword in allowed_keywords for keyword in array)
 def _check_ansatz(array):
     allowed_keywords = {"all", "HPzRx","hardware_efficient", "tree_tensor", "two_local"} 
     return all(keyword in allowed_keywords for keyword in array)
 def _check_features(array):
     return all((keyword > 0 and keyword <= 1) for keyword in array)
 
+def is_metric_function(func):
+    if func is None:
+        logging.warning("No custom Metric was passed.")
+        return False
+    # Step 1: Check if the function takes exactly two arguments
+    sig = inspect.signature(func)
+    if len(sig.parameters) != 2:
+        logging.warning("The custom metric does take only two parameters. It will not be used.")
+        return False
+
+    # Step 2: Check if the function can be called with sample input
+    y_true = np.array([1, 2, 3])
+    y_pred = np.array([1.1, 1.9, 3.2])
+    try:
+        result = func(y_pred, y_true)
+    except Exception as e:
+        logging.warning("The custom metric function does not behave as expected. No custom metric will be used")
+        return False
+    
+    # Step 3: Check if the output is a single numerical value
+    if not isinstance(result, (int, float, np.number)):
+        logging.warning("The custom metric function does not return a single numerical value. It will not be used.")
+        return False
+    
+    logging.warning("The custom metric is valid and will be used.")
+    return True
+
+
 def create_combinations(classifiers, embeddings, ansatzs, features):
-        combinations = []
-        features.append(None)
-        ansatzs.append(None)
-        if "all" in classifiers:
-            classifiers = ["qsvm", "qnn", "qnn_bag"]
-        if "all" in embeddings:
-            embeddings = ["amplitude_embedding", "rx_embedding", "rz_embedding", "ry_embedding","ZZ_embedding"]
-        if "all" in ansatzs:
-            ansatzs = ["HPzRx", "tree_tensor", "two_local", "hardware_efficient", None]
-
-        for classifier, embedding, ansatz, feature in product(classifiers, embeddings, ansatzs, features):
-            if classifier == "qsvm":
-                # For "qsvm", ansatz and feature should be None
-                if ansatz is None and feature is None:
-                    combinations.append((classifier, embedding, ansatz, feature))
-            elif classifier == "qnn":
-                # For "qnn", feature should be None and ansatz cannot be None
-                if feature is None and ansatz is not None:
-                    combinations.append((classifier, embedding, ansatz, feature))
-            elif classifier == "qnn_bag":
-                # For "qnn_bag", ansatz and feature cannot be None
-                if embedding is not None and ansatz is not None and feature is not None:
-                    combinations.append((classifier, embedding, ansatz, feature))
-        return combinations
+    combinations = []
+    if "all" in classifiers:
+        classifiers = ["qsvm", "qnn", "qnn_bag"]
+    if "all" in embeddings:
+        embeddings = ["amplitude_embedding", "rx_embedding", "rz_embedding", "ry_embedding","ZZ_embedding"]
+    if "all" in ansatzs:
+        ansatzs = ["HPzRx", "tree_tensor", "two_local", "hardware_efficient", None]
+
+    for classifier, embedding, ansatz, feature in product(classifiers, embeddings, ansatzs, features+[None]):
+        if classifier == "qsvm":
+            # For "qsvm", ansatz and feature should be None
+            if ansatz is None and feature is None:
+                combinations.append((classifier, embedding, ansatz, feature))
+        elif classifier == "qnn":
+            # For "qnn", feature should be None and ansatz cannot be None
+            if feature is None and ansatz is not None:
+                combinations.append((classifier, embedding, ansatz, feature))
+        elif classifier == "qnn_bag":
+            # For "qnn_bag", ansatz and feature cannot be None
+            if embedding is not None and ansatz is not None and feature is not None:
+                combinations.append((classifier, embedding, ansatz, feature))
+    return combinations
 
 """
  Quantum Classifier
 """
 
 class QuantumClassifier():
     """
@@ -337,43 +372,50 @@
             # Check if the module belongs to sklearn.impute
             if module.__name__.startswith('sklearn.impute'):
                 logging.warn("The object belongs to the sklearn.impute module. Custom Numeric Imputer will be used.")
                 self.numeric_transformer = Pipeline(
                 steps=[("imputer",customImputerNum), ("scaler", StandardScaler())])
             else:
                 logging.warn("The object does not belong to the sklearn.impute module. Default Custom Numeric Imputer will be used.")
+                self.numeric_transformer = Pipeline(
+                steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())])
         else:
             self.numeric_transformer = Pipeline(
             steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())])
 
 
         if customImputerCat is not None:
-            module = inspect.getmodule(customImputerNum)
+            module = inspect.getmodule(customImputerCat)
             # Check if the module belongs to sklearn.impute
             if module.__name__.startswith('sklearn.impute'):
-                logging.warn("The object belongs to the sklearn.impute module. Custom Numeric Categorical will be used.")
+                logging.warn("The object belongs to the sklearn.impute module. Custom Categorical Imputer will be used.")
                 self.categorical_transformer = Pipeline(
                 steps=[("imputer",customImputerCat), ("scaler", StandardScaler())])
             else:
                 logging.warn("The object does not belong to the sklearn.impute module. Default Custom Categorical Imputer will be used.")
+                self.categorical_transformer = Pipeline(
+                steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())])
         else:    
             self.categorical_transformer = Pipeline(
             steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())])
         
-        self.customMetric = customMetric
+        if is_metric_function(customMetric):
+            self.customMetric = customMetric
+        else:
+            self.customMetric = None
 
         if errors > 0:
             for i in errormsg:
                 logging.error(i,exc_info=False)
             exit()
         print(tabulate([[self.learningRate,self.epochs,self.runs,self.classifiers,self.embeddings,self.ansatzs,self.features,self.nqubits,self.numLayers,self.numPredictors]], headers=['Learning Rate', 'Epochs', "# Runs","Classifiers","Embeddings","Ansatzs","Features","Qubits","Layers","Predictors"], tablefmt='orgtbl'))
 
 
     
-    def fit(self, X_train, X_test, y_train, y_test):
+    def fit(self, X_train, y_train, X_test, y_test,showTable=True):
         """
         Fit Classification algorithms to X_train and y_train, predict and score on X_test, y_test.
         If the dimensions of the training vectors are not compatible with the different models, a 
         PCA transformation will be used in order to reduce the dimensionality to a compatible space.
         All categories must be in the training data if there are new categories in the test date the
         function will not work. The objective variable must be in a numerical form like LabelEncoder or
         OrdinalEncoder. Onehot or strings won't work.
@@ -388,15 +430,16 @@
             and columns is the number of features.
         y_train : array-like,
             Training vectors, where rows is the number of samples
             and columns is the number of features.
         y_test : array-like,
             Testing vectors, where rows is the number of samples
             and columns is the number of features.
-        
+        showTable : bool, optional (default=True)
+            Parameter to allow the fit to show a markdown table of the models metrics.
         Returns
         -------
         scores : Pandas DataFrame
             Returns metrics of all the models in a Pandas DataFrame.
         predictions : Pandas DataFrame
             Returns predictions of all the models in a Pandas DataFrame.
         """
@@ -410,19 +453,24 @@
         F1 = []
         TIME = []
         PARAMETERS = []
 
         predictions = {}
         
         models = []
-        
+        scores = None
 
         numClasses = len(np.unique(y_train))
         binary = numClasses == 2 
 
+        if (numClasses > 2**math.floor(math.log2(self.nqubits))):
+            logging.warning("The number of qubits must exceed the number of classes and be a power of 2 to execute all circuits successfully. \nEnsure that nqubits > #classes and that 2^floor(log2(nqubits)) > #classes.\nThe number of qubits will be changed to a valid one, this change will affect the QuantumClassifier object.")
+            self.nqubits = adjust_nqubits(numClasses)
+            logging.warning(f"New number of qubits:\t{self.nqubits}")
+
 
         if self.customMetric is not None:
             customMetric = []
 
         if isinstance(X_train, np.ndarray):
             X_train = pd.DataFrame(X_train)
             X_test = pd.DataFrame(X_test)
@@ -462,15 +510,15 @@
         X_test = pca.transform(X_test) if self.nqubits <= X_test.shape[1] else X_test
         
         
         one = OneHotEncoder(sparse_output=False)
 
         # Creates tuple of (model_name, embedding, ansatz, features)
         models = create_combinations(self.classifiers,self.embeddings,self.ansatzs,self.features)
-
+        
 
         for model in models:
             
             name, embedding, ansatz, feature = model
             
             name = name if feature==None else name + f"_{feature}"
             self.verboseprint(name,embedding,ansatz)
@@ -479,21 +527,24 @@
                 start = time.time()
                 qsvm = SVC(kernel= qkernel(embedding, n_qubits=self.nqubits))
                 qsvm.fit(X=X_train if embedding != "amplitude_embedding" else X_train_amp,y=y_train)
                 y_pred = qsvm.predict(X=X_test if embedding != "amplitude_embedding" else X_test_amp)
                 accuracy = accuracy_score(y_test, y_pred, normalize=True)
                 b_accuracy = balanced_accuracy_score(y_test, y_pred)
                 f1 = f1_score(y_test, y_pred, average="weighted")
+                trainable = "~"
                 try:
                     roc_auc = roc_auc_score(y_test, y_pred)
                 except Exception as exception:
                     roc_auc = None
                     if self.ignoreWarnings is False:
                         self.verboseprint("ROC AUC couldn't be calculated for " + name)
                         self.verboseprint(exception)
+                if self.predictions:
+                    predictions[f"{name}_{embedding}"] = y_pred
                
             elif name == "qnn":
                 if binary:
                     start = time.time()
                     qnn_tmp = create_circuit_binary(n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits, layers=self.numLayers, ansatz=ansatz,embedding=embedding)
                     # apply vmap on x (first circuit param)
                     qnn_batched = jax.vmap(qnn_tmp, (0, None))
@@ -511,17 +562,17 @@
                         if ansatz == "tree_tensor":
                             auxTrain = X_train_tree
                             auxTest = X_test_tree
                         else:
                             auxTrain = X_train
                             auxTest = X_test
 
-                    preds, accuracy, b_accuracy, f1, roc_auc = evaluate_full_model_predictor_binary(qnn=qnn,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train,y_test=y_test,runs=self.runs,seed=self.randomstate,verboseprint=self.verboseprint)
+                    trainable, preds, accuracy, b_accuracy, f1, roc_auc = evaluate_full_model_predictor_binary(qnn=qnn,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train,y_test=y_test,runs=self.runs,seed=self.randomstate,verboseprint=self.verboseprint)
                     if self.predictions:
-                        predictions.append(preds)
+                        predictions[f"{name}_{embedding}_{ansatz}"] = preds
                 else:
                     y_train_o = one.fit_transform(y_train.reshape(-1,1))
                     y_test_o = one.transform(y_test.reshape(-1,1))
                     start = time.time()
                     qnn_tmp = create_circuit(n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits, layers=self.numLayers, ansatz=ansatz, n_class=numClasses,embedding=embedding)
                     # apply vmap on x (first circuit param)
                     qnn_batched = jax.vmap(qnn_tmp, (0, None))
@@ -539,17 +590,17 @@
                         if ansatz == "tree_tensor":
                             auxTrain = X_train_tree
                             auxTest = X_test_tree
                         else:
                             auxTrain = X_train
                             auxTest = X_test
 
-                    preds, accuracy, b_accuracy, f1, roc_auc = evaluate_full_model_predictor(qnn=qnn,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train_o,y_test=y_test_o,seed=self.randomstate,runs=self.runs,verboseprint=self.verboseprint)
+                    trainable, preds, accuracy, b_accuracy, f1, roc_auc = evaluate_full_model_predictor(qnn=qnn,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train_o,y_test=y_test_o,seed=self.randomstate,runs=self.runs,verboseprint=self.verboseprint)
                     if self.predictions:
-                        predictions.append(preds)
+                        predictions[f"{name}_{embedding}_{ansatz}"] = preds
             elif "qnn_bag" in name:
                 if binary:
                     start = time.time()
                     qnn_tmp_bag = create_circuit_binary(n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,embedding=embedding)
                     # apply vmap on x (first circuit param)
                     qnn_batched_bag = jax.vmap(qnn_tmp_bag, (0, None))
                     # Jit for faster execution
@@ -566,17 +617,17 @@
                         if ansatz == "tree_tensor":
                             auxTrain = X_train_tree
                             auxTest = X_test_tree
                         else:
                             auxTrain = X_train
                             auxTest = X_test
                     
-                    preds, accuracy, b_accuracy, f1, roc_auc = evaluate_bagging_predictor_binary(qnn=qnn_bag,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train,y_test=y_test,seed=self.randomstate,runs=self.runs,n_estimators=self.numPredictors,max_features=feature,max_samples=self.maxSamples,verboseprint=self.verboseprint)
+                    trainable, preds, accuracy, b_accuracy, f1, roc_auc = evaluate_bagging_predictor_binary(qnn=qnn_bag,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train,y_test=y_test,seed=self.randomstate,runs=self.runs,n_estimators=self.numPredictors,max_features=feature,max_samples=self.maxSamples,verboseprint=self.verboseprint)
                     if self.predictions:
-                        predictions.append(preds)
+                        predictions[f"{name}_{embedding}_{ansatz}_{feature}"] = preds
                 else:
                     start = time.time()
                     y_train_o =one.fit_transform(y_train.reshape(-1,1))
                     y_test_o = one.transform(y_test.reshape(-1,1))
                     qnn_tmp_bag = create_circuit(n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,n_class=numClasses,embedding=embedding)
                     # apply vmap on x (first circuit param)
                     qnn_batched_bag = jax.vmap(qnn_tmp_bag, (0, None))
@@ -593,53 +644,59 @@
                     else:
                         if ansatz == "tree_tensor":
                             auxTrain = X_train_tree
                             auxTest = X_test_tree
                         else:
                             auxTrain = X_train
                             auxTest = X_test
-                    preds, accuracy, b_accuracy, f1, roc_auc = evaluate_bagging_predictor(qnn=qnn_bag,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train_o,y_test=y_test_o,seed=self.randomstate,runs=self.runs,n_estimators=self.numPredictors,max_features=feature,max_samples=self.maxSamples,verboseprint=self.verboseprint)
+                    trainable, preds, accuracy, b_accuracy, f1, roc_auc = evaluate_bagging_predictor(qnn=qnn_bag,optimizer=self.optimizer,epochs=self.epochs,n_qubits= 2**math.floor(math.log2(self.nqubits))if ansatz=="tree_tensor" else self.nqubits,layers=self.numLayers,ansatz=ansatz,X_train=auxTrain,X_test=auxTest,y_train=y_train_o,y_test=y_test_o,seed=self.randomstate,runs=self.runs,n_estimators=self.numPredictors,max_features=feature,max_samples=self.maxSamples,verboseprint=self.verboseprint)
                     if self.predictions:
-                        predictions.append(preds)
+                        predictions[f"{name}_{embedding}_{ansatz}_{feature}"] = preds
 
             NAMES.append(name)
             ANSATZ.append(ansatz)
             ACCURACY.append(accuracy)
             B_ACCURACY.append(b_accuracy)
             ROC_AUC.append(roc_auc)
             EMBEDDINGS.append(embedding)
             F1.append(f1)
             TIME.append(time.time() - start)
+            PARAMETERS.append(trainable)
+
+            predictions = {}
 
             if self.customMetric is not None:
-                customMetric = self.customMetric(y_test, y_pred)
-                customMetric.append(customMetric)
+                customMetricV = self.customMetric(y_test, y_pred)
+                customMetric.append(customMetricV)
+
                 self.verboseprint(
                     {
                         "Model": NAMES[-1],
                         "Embedding": EMBEDDINGS[-1],
                         "Ansatz": ANSATZ[-1],
                         "Accuracy": ACCURACY[-1],
                         "Balanced Accuracy": B_ACCURACY[-1],
                         "ROC AUC": ROC_AUC[-1],
                         "F1 Score": F1[-1],
                         self.customMetric.__name__: customMetric,
+                        "Trainable Parameters": PARAMETERS[-1],
                         "Time taken": TIME[-1],
                     }
                 )
             else:
                 self.verboseprint(
                     {
                         "Model": NAMES[-1],
                         "Embedding": EMBEDDINGS[-1],
                         "Ansatz": ANSATZ[-1],
                         "Accuracy": ACCURACY[-1],
                         "Balanced Accuracy": B_ACCURACY[-1],
                         "ROC AUC": ROC_AUC[-1],
                         "F1 Score": F1[-1],
+                        "Trainable Parameters": PARAMETERS[-1],
                         "Time taken": TIME[-1],
                     }
                 )
         
             
         if self.customMetric is None:
            
@@ -648,32 +705,142 @@
                     "Model": NAMES,
                     "Embedding": EMBEDDINGS,
                     "Ansatz": ANSATZ,
                     "Accuracy": ACCURACY,
                     "Balanced Accuracy": B_ACCURACY,
                     "ROC AUC": ROC_AUC,
                     "F1 Score": F1,
+                    "Trainable Parameters": PARAMETERS,
                     "Time taken": TIME,
                 }
             )
         else:
             scores = pd.DataFrame(
                 {
                     "Model": NAMES,
                     "Embedding": EMBEDDINGS,
                     "Ansatz": ANSATZ,
                     "Accuracy": ACCURACY,
                     "Balanced Accuracy": B_ACCURACY,
                     "ROC AUC": ROC_AUC,
                     "F1 Score": F1,
                     self.customMetric.__name__: customMetric,
+                    "Trainable Parameters": PARAMETERS,
                     "Time taken": TIME,
                 }
             )
-        scores = scores.sort_values(by="Balanced Accuracy", ascending=False).set_index(
-            "Model"
-        )
+        scores = scores.sort_values(by="Balanced Accuracy", ascending=False)
         if self.predictions:
             predictions_df = pd.DataFrame.from_dict(predictions)
         
-        print(scores.to_markdown())
-        return scores, predictions_df if self.predictions is True else scores
+        if showTable:
+            print(scores.to_markdown())
+        return scores, predictions_df if self.predictions is True else None
+    
+    def repeated_cross_validation(self, X, y, n_splits=5, n_repeats=10, showTable=True):
+        """x
+        Perform repeated cross-validation on the given dataset and model.
+
+        This method splits the dataset into multiple train-test splits using RepeatedStratifiedKFold,
+        fits the model on the training set, evaluates it on the validation set, and aggregates the results.
+
+        Parameters:
+        -----------
+        X : array-like
+            The input features for the dataset.
+        y : array-like
+            The target labels for the dataset.
+        n_splits : int, optional (default=5)
+            Number of folds in each repetition of the cross-validation.
+        n_repeats : int, optional (default=10)
+            Number of times cross-validation needs to be repeated.
+        showTable : bool, optional (default=True)
+            If True, prints the aggregated results in a tabular format.
+
+        Returns:
+        --------
+        mean_scores : pandas.DataFrame
+            A DataFrame containing the mean scores of each fold, grouped by 'Model', 'Embedding', and 'Ansatz'.
+        
+        Raises:
+        -------
+        ValueError
+            If X or y is None.
+        """
+        # Check if X and y are not None
+        if X is None or y is None:
+            raise ValueError("Input features X and target y must not be None")
+
+        # Ensure X and y are array-like
+        X = np.array(X)
+        y = np.array(y)
+    
+        # Initialize RepeatedStratifiedKFold
+        rkf = RepeatedStratifiedKFold(n_splits=n_splits, n_repeats=n_repeats, random_state=self.randomstate)
+        all_scores = []
+
+        # Split the data and perform cross-validation
+        for train_index, val_index in rkf.split(X, y):
+            X_train, X_val = X[train_index], X[val_index]
+            y_train, y_val = y[train_index], y[val_index]
+
+            # Fit the model and get the scores for the current fold
+            scores, preds = self.fit(X_train=X_train, y_train=y_train, X_test=X_val, y_test=y_val,showTable=False)
+            all_scores.append(scores)
+
+        # Aggregate results by taking the mean of each score
+        mean_scores = pd.concat(all_scores).groupby(['Model', 'Embedding', 'Ansatz'], as_index=False).mean()
+        if showTable:
+            print(mean_scores.to_markdown())
+        return mean_scores
+    def leave_one_out(self, X, y, showTable=True):
+        """
+        Perform leave-one-out cross-validation on the given dataset and model.
+
+        This method splits the dataset into multiple train-test splits using LeaveOneOut,
+        fits the model on the training set, evaluates it on the validation set, and aggregates the results.
+
+        Parameters:
+        -----------
+        X : array-like
+            The input features for the dataset.
+        y : array-like
+            The target labels for the dataset.
+        showTable : bool, optional (default=True)
+            If True, prints the aggregated results in a tabular format.
+
+        Returns:
+        --------
+        mean_scores : pandas.DataFrame
+            A DataFrame containing the mean scores of each fold, grouped by 'Model', 'Embedding', and 'Ansatz'.
+        
+        Raises:
+        -------
+        ValueError
+            If X or y is None.
+        """
+        # Check if X and y are not None
+        if X is None or y is None:
+            raise ValueError("Input features X and target y must not be None")
+
+        # Ensure X and y are array-like
+        X = np.array(X)
+        y = np.array(y)
+
+        # Initialize LeaveOneOut
+        loo = LeaveOneOut()
+        all_scores = []
+
+        # Split the data and perform cross-validation
+        for train_index, val_index in loo.split(X):
+            X_train, X_val = X[train_index], X[val_index]
+            y_train, y_val = y[train_index], y[val_index]
+
+            # Fit the model and get the scores for the current fold
+            scores, preds = self.fit(X_train=X_train, y_train=y_train, X_test=X_val, y_test=y_val, showTable=False)
+            all_scores.append(scores)
+
+        # Aggregate results by taking the mean of each score
+        mean_scores = pd.concat(all_scores).groupby(['Model', 'Embedding', 'Ansatz'], as_index=False).mean()
+        if showTable:
+            print(mean_scores.to_markdown())
+        return mean_scores
```

### Comparing `lazyqml-0.4.0/lazyqml.egg-info/PKG-INFO` & `lazyqml-1.0.0/lazyqml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.4.0
+Version: 1.0.0
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.4.0/lazyqml.egg-info/SOURCES.txt` & `lazyqml-1.0.0/lazyqml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/mkdocs.yml` & `lazyqml-1.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/pyproject.toml` & `lazyqml-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lazyqml"
-version = "0.4.0"
+version = "1.0.0"
 dynamic = [
     "dependencies",
 ]
 description = "LazyQML benchmarking utility to test quantum machine learning models."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -46,15 +46,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.4.0"
+current_version = "1.0.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.4.0/requirements.txt` & `lazyqml-1.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/requirements_dev.txt` & `lazyqml-1.0.0/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.4.0/tests/test_lazyqml.py` & `lazyqml-1.0.0/tests/test_lazyqml.py`

 * *Files identical despite different names*

