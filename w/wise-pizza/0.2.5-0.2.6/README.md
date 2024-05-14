# Comparing `tmp/wise-pizza-0.2.5.tar.gz` & `tmp/wise-pizza-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.2.5.tar", last modified: Mon May 13 16:03:35 2024, max compression
+gzip compressed data, was "wise-pizza-0.2.6.tar", last modified: Tue May 14 09:49:58 2024, max compression
```

## Comparing `wise-pizza-0.2.5.tar` & `wise-pizza-0.2.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:35.012511 wise-pizza-0.2.5/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-05-13 16:03:35.011797 wise-pizza-0.2.5/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7149 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/README.md
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2024-05-13 16:03:35.012586 wise-pizza-0.2.5/setup.cfg
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1415 2024-05-13 16:01:29.000000 wise-pizza-0.2.5/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:34.985835 wise-pizza-0.2.5/tests/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9754 2024-05-13 15:24:20.000000 wise-pizza-0.2.5/tests/test_fit.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:34.994538 wise-pizza-0.2.5/wise_pizza/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      142 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/__init__.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3869 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/cluster.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    23347 2024-05-13 15:23:28.000000 wise-pizza-0.2.5/wise_pizza/explain.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9193 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/make_matrix.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    12938 2024-05-13 14:44:18.000000 wise-pizza-0.2.5/wise_pizza/plotting.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    13313 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/plotting_time.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3788 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/preselect.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      329 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/run_streamlit_app_entry_point.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      553 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/segment_data.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    17785 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/slicer.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7503 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/slicer_facades.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      983 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/slicer_plotting.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:35.010944 wise-pizza-0.2.5/wise_pizza/solve/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/__init__.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7430 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/find_alpha.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1080 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/fitter.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4435 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/solver.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6415 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/tree.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      697 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/weighted_quantiles.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    12152 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/streamlit_app.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3700 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/time.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3554 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/transform.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11210 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:35.008402 wise-pizza-0.2.5/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      853 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       91 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/entry_points.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      150 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-14 09:49:58.083706 wise-pizza-0.2.6/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-05-14 09:49:58.082692 wise-pizza-0.2.6/PKG-INFO
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7149 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/README.md
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2024-05-14 09:49:58.083795 wise-pizza-0.2.6/setup.cfg
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1415 2024-05-14 09:48:19.000000 wise-pizza-0.2.6/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-14 09:49:58.061808 wise-pizza-0.2.6/tests/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     9754 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/tests/test_fit.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-14 09:49:58.068493 wise-pizza-0.2.6/wise_pizza/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      142 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/__init__.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3869 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/cluster.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    23358 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/explain.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     9193 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/make_matrix.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    12938 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/plotting.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    13313 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/plotting_time.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3788 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/preselect.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      329 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/run_streamlit_app_entry_point.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      553 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/segment_data.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    17815 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/slicer.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7503 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/slicer_facades.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      983 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/slicer_plotting.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-14 09:49:58.080304 wise-pizza-0.2.6/wise_pizza/solve/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)        0 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/solve/__init__.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7000 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/solve/find_alpha.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1080 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/solve/fitter.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4435 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/solve/solver.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     6415 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/solve/tree.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      697 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/solve/weighted_quantiles.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    12152 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/streamlit_app.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3700 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/time.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3554 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/transform.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    12004 2024-05-14 09:43:49.000000 wise-pizza-0.2.6/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-14 09:49:58.077002 wise-pizza-0.2.6/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-05-14 09:49:58.000000 wise-pizza-0.2.6/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      853 2024-05-14 09:49:58.000000 wise-pizza-0.2.6/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2024-05-14 09:49:58.000000 wise-pizza-0.2.6/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       91 2024-05-14 09:49:58.000000 wise-pizza-0.2.6/wise_pizza.egg-info/entry_points.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      150 2024-05-14 09:49:58.000000 wise-pizza-0.2.6/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2024-05-14 09:49:58.000000 wise-pizza-0.2.6/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.2.5/LICENSE` & `wise-pizza-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/PKG-INFO` & `wise-pizza-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.2.5/README.md` & `wise-pizza-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/setup.py` & `wise-pizza-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.2.5",
+    version="0.2.6",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `wise-pizza-0.2.5/tests/test_fit.py` & `wise-pizza-0.2.6/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/cluster.py` & `wise-pizza-0.2.6/wise_pizza/cluster.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/explain.py` & `wise-pizza-0.2.6/wise_pizza/explain.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def explain_changes_in_average(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     dims: List[str],
     total_name: str,
     size_name: str,
     min_segments: Optional[int] = None,
-    max_segments: int = 5,
+    max_segments: int = None,
     min_depth: int = 1,
     max_depth: int = 2,
     solver: str = "lasso",
     how: str = "totals",
     force_add_up: bool = False,
     constrain_signs: bool = True,
     cluster_values: bool = False,
@@ -120,15 +120,15 @@
 def explain_changes_in_totals(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     dims: List[str],
     total_name: str,
     size_name: str,
     min_segments: Optional[int] = None,
-    max_segments: int = 5,
+    max_segments: int = None,
     min_depth: int = 1,
     max_depth: int = 2,
     solver: str = "lasso",
     how: str = "totals",
     force_add_up: bool = False,
     constrain_signs: bool = True,
     cluster_values: bool = False,
@@ -267,15 +267,15 @@
 
 def explain_levels(
     df: pd.DataFrame,
     dims: List[str],
     total_name: str,
     size_name: Optional[str] = None,
     min_segments: int = None,
-    max_segments: int = 10,
+    max_segments: int = None,
     min_depth: int = 1,
     max_depth: int = 2,
     solver="lasso",
     verbose=0,
     force_add_up: bool = False,
     constrain_signs: bool = True,
     cluster_values: bool = False,
@@ -349,15 +349,15 @@
 def explain_timeseries(
     df: pd.DataFrame,
     dims: List[str],
     total_name: str,
     time_name: str,
     size_name: Optional[str] = None,
     min_segments: int = None,
-    max_segments: int = 5,
+    max_segments: int = None,
     min_depth: int = 1,
     max_depth: int = 2,
     solver: str = "omp",
     verbose: bool = False,
     constrain_signs: bool = False,
     cluster_values: bool = False,
     time_basis: Optional[pd.DataFrame] = None,
```

### Comparing `wise-pizza-0.2.5/wise_pizza/make_matrix.py` & `wise-pizza-0.2.6/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/plotting.py` & `wise-pizza-0.2.6/wise_pizza/plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/plotting_time.py` & `wise-pizza-0.2.6/wise_pizza/plotting_time.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/preselect.py` & `wise-pizza-0.2.6/wise_pizza/preselect.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/segment_data.py` & `wise-pizza-0.2.6/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/slicer.py` & `wise-pizza-0.2.6/wise_pizza/slicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing import Optional, Union, List, Dict, Sequence
 from collections import defaultdict
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csc_matrix, diags
 
-from wise_pizza.solve.find_alpha import clean_up_min_max, find_alpha
+from wise_pizza.solve.find_alpha import find_alpha
+from wise_pizza.utils import clean_up_min_max
 from wise_pizza.make_matrix import sparse_dummy_matrix
 from wise_pizza.cluster import make_clusters
 from wise_pizza.preselect import HeuristicSelector
 from wise_pizza.time import extend_dataframe
 from wise_pizza.slicer_facades import SliceFinderPredictFacade
 from wise_pizza.solve.tree import tree_solver
 from wise_pizza.solve.solver import solve_lasso
@@ -94,15 +95,15 @@
     def fit(
         self,
         dim_df: pd.DataFrame,
         totals: pd.Series,
         weights: pd.Series = None,
         time_col: pd.Series = None,
         time_basis: pd.DataFrame = None,
-        min_segments: int = 10,
+        min_segments: int = None,
         max_segments: int = None,
         min_depth: int = 1,
         max_depth: int = 3,
         solver: str = "lp",
         verbose: Union[bool, None] = None,
         force_dim: Optional[str] = None,
         force_add_up: bool = False,
```

### Comparing `wise-pizza-0.2.5/wise_pizza/slicer_facades.py` & `wise-pizza-0.2.6/wise_pizza/slicer_facades.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/slicer_plotting.py` & `wise-pizza-0.2.6/wise_pizza/slicer_plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/solve/find_alpha.py` & `wise-pizza-0.2.6/wise_pizza/solve/find_alpha.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pandas as pd
 from scipy.sparse import vstack, csr_array, issparse
 from scipy.linalg import svd
 
 from wise_pizza.solve.solver import solve_lasso, solve_lp, solve_omp
+from wise_pizza.utils import clean_up_min_max
 
 
 def find_alpha(
     X,
     y_,
     max_nonzeros=None,
     min_nonzeros=None,
@@ -215,23 +216,7 @@
         1e-3 * min(alpha, 1.0),
         constrain_signs=constrain_signs,
         verbose=verbose,
         drop_last_row=adding_up_regularizer,
         # fit_intercept=not use_proj
     )
     return reg, nonzeros
-
-
-def clean_up_min_max(min_nonzeros: int = None, max_nonzeros: int = None):
-    assert min_nonzeros is not None or max_nonzeros is not None
-    if max_nonzeros is None:
-        if min_nonzeros is None:
-            max_nonzeros = 5
-            min_nonzeros = 5
-        else:
-            max_nonzeros = min_nonzeros
-    else:
-        if min_nonzeros is None:
-            min_nonzeros = max_nonzeros
-
-    assert min_nonzeros <= max_nonzeros
-    return min_nonzeros, max_nonzeros
```

### Comparing `wise-pizza-0.2.5/wise_pizza/solve/fitter.py` & `wise-pizza-0.2.6/wise_pizza/solve/fitter.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/solve/solver.py` & `wise-pizza-0.2.6/wise_pizza/solve/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/solve/tree.py` & `wise-pizza-0.2.6/wise_pizza/solve/tree.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/solve/weighted_quantiles.py` & `wise-pizza-0.2.6/wise_pizza/solve/weighted_quantiles.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/streamlit_app.py` & `wise-pizza-0.2.6/wise_pizza/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/time.py` & `wise-pizza-0.2.6/wise_pizza/time.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/transform.py` & `wise-pizza-0.2.6/wise_pizza/transform.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.5/wise_pizza/utils.py` & `wise-pizza-0.2.6/wise_pizza/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 
 from wise_pizza.segment_data import SegmentData
 
@@ -116,15 +117,17 @@
 
         c2 = combined.copy()
         c2["Change in totals"] = change_from_avg * avg_weights
         c2[weights] = 1.0  # avg_weights
 
         if return_multiple:
             sd_size = SegmentData(
-                combined.rename(columns={"Change in totals": "Change from segment size"}),
+                combined.rename(
+                    columns={"Change in totals": "Change from segment size"}
+                ),
                 dimensions=dims,
                 segment_total="Change from segment size",
                 segment_size=weights,
             )
             sd_avg = SegmentData(
                 c2.rename(columns={"Change in totals": "Change from segment average"}),
                 dimensions=dims,
@@ -133,15 +136,17 @@
             )
             return sd_size, sd_avg
 
         else:
             combined["Change from"] = "Segment size"
             c2["Change from"] = "Segment average"
 
-            df = pd.concat([combined, c2])[dims + [weights, "Change in totals", "Change from"]]
+            df = pd.concat([combined, c2])[
+                dims + [weights, "Change in totals", "Change from"]
+            ]
             df_change_in_totals = np.array(df["Change in totals"], dtype=np.longdouble)
             combined_dtotals = np.array(combined["dtotals"], dtype=np.longdouble)
             df_change_in_totals_sum = np.nansum(df_change_in_totals)
             combined_dtotals_sum = np.nansum(combined_dtotals)
             # if combined_dtotals_sum > 1e-31:
             #     assert rel_error(df_change_in_totals_sum, combined_dtotals_sum) < eps
 
@@ -156,15 +161,17 @@
         combined["Change in totals"] = combined[totals + "_y"] - combined[totals + "_x"]
 
         # TODO: why does taking prev period as baseline make the fit so slow?
         # baseline hypothesis is proportional increase from first period
         combined[weights] = 1.0  # combined[totals + "_x"]
         combined[weights] = np.maximum(1.0, combined[weights])
         cols = (
-            dims + ["Change in totals", totals + "_x", totals + "_y"] + [c for c in combined.columns if "baseline" in c]
+            dims
+            + ["Change in totals", totals + "_x", totals + "_y"]
+            + [c for c in combined.columns if "baseline" in c]
         )
 
         return SegmentData(
             combined[cols + [weights]],
             dimensions=dims,
             segment_total="Change in totals",
             segment_size=weights,
@@ -201,24 +208,34 @@
         # If weights are zero, totals must be zero in the same row
         new_df.loc[new_df[size_name] == 0, total_name] = 0
     else:
         new_df[[total_name]] = new_df[[total_name]].fillna(0)
 
     # replace NaN values in categorical columns with the column name + "_unknown"
     object_columns = list(new_df[dims].select_dtypes("object").columns)
-    new_df[object_columns] = new_df[object_columns].fillna(new_df[object_columns].apply(lambda x: x.name + "_unknown"))
+    new_df[object_columns] = new_df[object_columns].fillna(
+        new_df[object_columns].apply(lambda x: x.name + "_unknown")
+    )
     new_df[object_columns] = new_df[object_columns].astype(str)
 
     # Groupby all relevant dims to decrease the dataframe size, if possible
     group_dims = dims if time_name is None else dims + [time_name]
 
     if size_name is not None:
-        new_df = new_df.groupby(by=group_dims, observed=True)[[total_name, size_name]].sum().reset_index()
+        new_df = (
+            new_df.groupby(by=group_dims, observed=True)[[total_name, size_name]]
+            .sum()
+            .reset_index()
+        )
     else:
-        new_df = new_df.groupby(by=group_dims, observed=True)[[total_name]].sum().reset_index()
+        new_df = (
+            new_df.groupby(by=group_dims, observed=True)[[total_name]]
+            .sum()
+            .reset_index()
+        )
 
     return new_df
 
 
 #
 # def prepare_time_df(
 #     df: pd.DataFrame,
@@ -276,9 +293,28 @@
 #         new_df = new_df.groupby(by=dims, observed=True)[[total_name, size_name]].sum().reset_index()
 #     else:
 #         new_df = new_df.groupby(by=dims, observed=True)[[total_name]].sum().reset_index()
 #
 #     new_df[object_columns] = new_df[object_columns].astype(str)
 #
 #     return new_df
-def almost_equals(x1, x2, eps: float=1e-6) -> bool:
-    return np.sum(np.abs(x1-x2))/np.mean(np.abs(x1+x2)) < eps
+def almost_equals(x1, x2, eps: float = 1e-6) -> bool:
+    return np.sum(np.abs(x1 - x2)) / np.mean(np.abs(x1 + x2)) < eps
+
+
+def clean_up_min_max(min_nonzeros: int = None, max_nonzeros: int = None):
+    if min_nonzeros is not None:
+        logging.warning(
+            "min_segments parameter is deprecated, please use max_nonzeros instead."
+        )
+    if max_nonzeros is None:
+        if min_nonzeros is None:
+            max_nonzeros = 5
+            min_nonzeros = 5
+        else:
+            max_nonzeros = min_nonzeros
+    else:
+        if min_nonzeros is None:
+            min_nonzeros = max_nonzeros
+
+    assert min_nonzeros <= max_nonzeros
+    return min_nonzeros, max_nonzeros
```

### Comparing `wise-pizza-0.2.5/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.2.6/wise_pizza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.2.5/wise_pizza.egg-info/SOURCES.txt` & `wise-pizza-0.2.6/wise_pizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

