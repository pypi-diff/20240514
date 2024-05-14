# Comparing `tmp/laff-0.9.8.tar.gz` & `tmp/laff-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laff-0.9.8.tar", max compression
+gzip compressed data, was "laff-0.9.9.tar", max compression
```

## Comparing `laff-0.9.8.tar` & `laff-0.9.9.tar`

### file list

```diff
@@ -1,27 +1,13 @@
--rw-r--r--   0        0        0     2642 2023-08-23 16:25:59.728263 laff-0.9.8/README.md
--rw-r--r--   0        0        0     8196 2023-09-28 14:34:54.160596 laff-0.9.8/laff/.DS_Store
--rw-r--r--   0        0        0      172 2024-01-25 13:38:15.058200 laff-0.9.8/laff/__init__.py
--rw-r--r--   0        0        0       47 2024-01-25 13:38:15.058837 laff-0.9.8/laff/flarefinding/__init__.py
--rw-r--r--   0        0        0      206 2024-01-25 13:49:56.422467 laff-0.9.8/laff/flarefinding/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      204 2023-10-04 17:07:31.137248 laff-0.9.8/laff/flarefinding/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5666 2024-01-26 13:42:51.984110 laff-0.9.8/laff/flarefinding/__pycache__/flarefinding.cpython-310.pyc
--rw-r--r--   0        0        0     5668 2023-10-05 15:55:51.687151 laff-0.9.8/laff/flarefinding/__pycache__/flarefinding.cpython-38.pyc
--rw-r--r--   0        0        0     5708 2023-10-04 09:23:53.443878 laff-0.9.8/laff/flarefinding/__pycache__/sequential_flarefinding.cpython-38.pyc
--rw-r--r--   0        0        0     7495 2024-01-26 13:30:26.120682 laff-0.9.8/laff/flarefinding/flarefinding.py
--rw-r--r--   0        0        0    10942 2024-01-30 14:53:41.024069 laff-0.9.8/laff/laff.py
--rw-r--r--   0        0        0     2809 2024-01-30 14:48:17.108498 laff-0.9.8/laff/lightcurve_import.py
--rw-r--r--   0        0        0      171 2024-01-26 13:30:26.122602 laff-0.9.8/laff/modelling/__init__.py
--rw-r--r--   0        0        0      348 2024-01-26 13:42:51.989788 laff-0.9.8/laff/modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6166 2024-01-25 13:49:56.475026 laff-0.9.8/laff/modelling/__pycache__/fit_continuum.cpython-310.pyc
--rw-r--r--   0        0        0     8136 2024-01-26 16:00:03.151990 laff-0.9.8/laff/modelling/__pycache__/fit_flare.cpython-310.pyc
--rw-r--r--   0        0        0     7060 2024-01-25 13:38:15.063790 laff-0.9.8/laff/modelling/fit_continuum.py
--rw-r--r--   0        0        0    10592 2024-01-26 15:59:44.873046 laff-0.9.8/laff/modelling/fit_flare.py
--rw-r--r--   0        0        0      162 2024-01-26 13:24:30.560039 laff-0.9.8/laff/utility/__init__.py
--rw-r--r--   0        0        0      353 2024-01-26 13:42:51.999072 laff-0.9.8/laff/utility/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      351 2023-10-05 10:37:10.223761 laff-0.9.8/laff/utility/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      773 2023-11-20 17:09:13.079262 laff-0.9.8/laff/utility/__pycache__/errors.cpython-310.pyc
--rw-r--r--   0        0        0     1871 2024-01-26 13:42:52.007265 laff-0.9.8/laff/utility/__pycache__/utility.cpython-310.pyc
--rw-r--r--   0        0        0     1880 2023-10-10 15:29:05.729179 laff-0.9.8/laff/utility/__pycache__/utility.cpython-38.pyc
--rw-r--r--   0        0        0     1922 2024-01-30 14:52:49.999241 laff-0.9.8/laff/utility/utility.py
--rw-r--r--   0        0        0      524 2024-01-30 14:54:27.521717 laff-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 laff-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     2642 2023-08-23 16:25:59.728263 laff-0.9.9/README.md
+-rw-r--r--   0        0        0      172 2024-01-25 13:38:15.058200 laff-0.9.9/laff/__init__.py
+-rw-r--r--   0        0        0       47 2024-01-25 13:38:15.058837 laff-0.9.9/laff/flarefinding/__init__.py
+-rw-r--r--   0        0        0     7494 2024-01-30 15:22:47.763104 laff-0.9.9/laff/flarefinding/flarefinding.py
+-rw-r--r--   0        0        0    10942 2024-01-30 14:53:41.024069 laff-0.9.9/laff/laff.py
+-rw-r--r--   0        0        0     2809 2024-01-30 14:48:17.108498 laff-0.9.9/laff/lightcurve_import.py
+-rw-r--r--   0        0        0      171 2024-01-26 13:30:26.122602 laff-0.9.9/laff/modelling/__init__.py
+-rw-r--r--   0        0        0     7060 2024-01-25 13:38:15.063790 laff-0.9.9/laff/modelling/fit_continuum.py
+-rw-r--r--   0        0        0    10592 2024-01-26 15:59:44.873046 laff-0.9.9/laff/modelling/fit_flare.py
+-rw-r--r--   0        0        0      162 2024-01-26 13:24:30.560039 laff-0.9.9/laff/utility/__init__.py
+-rw-r--r--   0        0        0     1966 2024-01-30 15:22:01.723234 laff-0.9.9/laff/utility/utility.py
+-rw-r--r--   0        0        0      524 2024-01-30 15:39:11.494765 laff-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 laff-0.9.9/PKG-INFO
```

### Comparing `laff-0.9.8/README.md` & `laff-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `laff-0.9.8/laff/flarefinding/flarefinding.py` & `laff-0.9.9/laff/flarefinding/flarefinding.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
         n += 1
 
     return FLARES
 
 def find_start(data: pd.DataFrame, start: int, prev_decay: int) -> int:
     """Return flare start by looking for local minima."""
-
     if start < 3:
         points = data.iloc[0:3]
     else:
         points = data.iloc[start-3:start+1]
     minimum = data[data.flux == min(points.flux)].index.values[0]
     minimum = (minimum + 1) if (minimum <= prev_decay) else minimum
     logger.debug(f"Flare start found at {minimum}")
```

### Comparing `laff-0.9.8/laff/laff.py` & `laff-0.9.9/laff/laff.py`

 * *Files identical despite different names*

### Comparing `laff-0.9.8/laff/lightcurve_import.py` & `laff-0.9.9/laff/lightcurve_import.py`

 * *Files identical despite different names*

### Comparing `laff-0.9.8/laff/modelling/fit_continuum.py` & `laff-0.9.9/laff/modelling/fit_continuum.py`

 * *Files identical despite different names*

### Comparing `laff-0.9.8/laff/modelling/fit_flare.py` & `laff-0.9.9/laff/modelling/fit_flare.py`

 * *Files identical despite different names*

### Comparing `laff-0.9.8/laff/utility/utility.py` & `laff-0.9.9/laff/utility/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         data['time_nerr'] = data['time_perr']
         data['flux_nerr'] = data['flux_perr']
         data.columns = expected_columns
     elif data.shape[1] == 6:
         data.columns = expected_columns
     else:
         raise ValueError(f"Expected dataframe with 4 or 6 columns - got {data.shape[1]}.")
+    
+    data = data.reset_index(drop=True)
 
     logger.debug('Data input is good.')
 
     return data
 
 def calculate_fluence(model, params, start, stop, count_flux_ratio):
     """Given some model and range, calculate the fluence. Optional count/flux ratio, default 1."""
```

### Comparing `laff-0.9.8/pyproject.toml` & `laff-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "laff"
-version = "0.9.8"
+version = "0.9.9"
 description = "GRB lightcurve flare and continuum fitter."
 authors = ["Adam Hennessy <ah724@leicester.ac.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 numpy = "^1.24.3"
```

### Comparing `laff-0.9.8/PKG-INFO` & `laff-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laff
-Version: 0.9.8
+Version: 0.9.9
 Summary: GRB lightcurve flare and continuum fitter.
 Author: Adam Hennessy
 Author-email: ah724@leicester.ac.uk
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

