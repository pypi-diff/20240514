# Comparing `tmp/njab-0.0.5.tar.gz` & `tmp/njab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "njab-0.0.5.tar", last modified: Thu May  2 14:22:22 2024, max compression
+gzip compressed data, was "njab-0.0.6.tar", last modified: Tue May 14 14:47:44 2024, max compression
```

## Comparing `njab-0.0.5.tar` & `njab-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 14:22:18.000000 njab-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-02 14:22:22.475694 njab-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-02 14:22:18.000000 njab-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 14:22:18.000000 njab-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-02 14:22:22.479694 njab-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 14:22:18.000000 njab-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/njab/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/njab/io/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/njab/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/km.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/lifelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/pca.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/stats/ancova.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/stats/groups_comparision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-02 14:22:18.000000 njab-0.0.5/test/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 14:22:18.000000 njab-0.0.5/test/test_pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 14:22:18.000000 njab-0.0.5/test/test_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-14 14:47:40.000000 njab-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-14 14:47:44.309849 njab-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-14 14:47:40.000000 njab-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 14:47:40.000000 njab-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-14 14:47:44.309849 njab-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 14:47:40.000000 njab-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/njab/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/njab/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/njab/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/km.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/stats/ancova.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/stats/groups_comparision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 14:47:40.000000 njab-0.0.6/test/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 14:47:40.000000 njab-0.0.6/test/test_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 14:47:40.000000 njab-0.0.6/test/test_scoring.py
```

### Comparing `njab-0.0.5/LICENSE` & `njab-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/PKG-INFO` & `njab-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: njab
-Version: 0.0.5
+Version: 0.0.6
 Summary: not Just Another Biomarker
 Author: Henry Webel
 Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
```

### Comparing `njab-0.0.5/README.md` & `njab-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/setup.cfg` & `njab-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = njab
-version = 0.0.5
+version = 0.0.6
 description = not Just Another Biomarker
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Henry Webel
 author_email = "Henry Webel" <henry.webel@cpr.ku.dk>
 license = MIT
 license_files = LICENSE
```

### Comparing `njab-0.0.5/src/njab/pandas/__init__.py` & `njab-0.0.6/src/njab/pandas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -116,14 +116,12 @@
         Exclude NA values from counting, by default True
 
     Returns
     -------
     pandas.DataFrame
         DataFrame of combined value counts.
     """
-    """
-    """
-    _df = pd.DataFrame()
+    freq_targets = list()
     for col in X.columns:
-        _df = _df.join(X[col].value_counts(dropna=dropna), how='outer')
-    freq_targets = _df.sort_index()
+        freq_targets.append(X[col].value_counts(dropna=dropna).rename(col))
+    freq_targets = pd.concat(freq_targets, axis=1, sort=True)
     return freq_targets
```

### Comparing `njab-0.0.5/src/njab/plotting/__init__.py` & `njab-0.0.6/src/njab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/plotting/km.py` & `njab-0.0.6/src/njab/plotting/km.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/plotting/lifelines.py` & `njab-0.0.6/src/njab/plotting/lifelines.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/plotting/metrics.py` & `njab-0.0.6/src/njab/plotting/metrics.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/sklearn/__init__.py` & `njab-0.0.6/src/njab/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/sklearn/pca.py` & `njab-0.0.6/src/njab/sklearn/pca.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/sklearn/preprocessing.py` & `njab-0.0.6/src/njab/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/sklearn/scoring.py` & `njab-0.0.6/src/njab/sklearn/scoring.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/sklearn/types.py` & `njab-0.0.6/src/njab/sklearn/types.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/stats/ancova.py` & `njab-0.0.6/src/njab/stats/ancova.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab/stats/groups_comparision.py` & `njab-0.0.6/src/njab/stats/groups_comparision.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.5/src/njab.egg-info/PKG-INFO` & `njab-0.0.6/src/njab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: njab
-Version: 0.0.5
+Version: 0.0.6
 Summary: not Just Another Biomarker
 Author: Henry Webel
 Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
```

### Comparing `njab-0.0.5/src/njab.egg-info/SOURCES.txt` & `njab-0.0.6/src/njab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

