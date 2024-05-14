# Comparing `tmp/dataprep_ml-24.5.1.0.tar.gz` & `tmp/dataprep_ml-24.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataprep_ml-24.5.1.0.tar", max compression
+gzip compressed data, was "dataprep_ml-24.5.1.1.tar", max compression
```

## Comparing `dataprep_ml-24.5.1.0.tar` & `dataprep_ml-24.5.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35104 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/LICENSE
--rw-r--r--   0        0        0     1762 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/README.md
--rw-r--r--   0        0        0      193 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/__init__.py
--rw-r--r--   0        0        0     1984 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/base.py
--rw-r--r--   0        0        0    18873 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/cleaners.py
--rw-r--r--   0        0        0     1197 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/helpers.py
--rw-r--r--   0        0        0     3342 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/imputers.py
--rw-r--r--   0        0        0     9314 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/insights.py
--rw-r--r--   0        0        0     4615 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/recommenders.py
--rw-r--r--   0        0        0     6633 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/splitters.py
--rw-r--r--   0        0        0      626 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/pyproject.toml
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 dataprep_ml-24.5.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35104 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/LICENSE
+-rw-r--r--   0        0        0     1762 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/README.md
+-rw-r--r--   0        0        0      193 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/__init__.py
+-rw-r--r--   0        0        0     1984 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/base.py
+-rw-r--r--   0        0        0    18873 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/cleaners.py
+-rw-r--r--   0        0        0     1197 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/helpers.py
+-rw-r--r--   0        0        0     3342 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/imputers.py
+-rw-r--r--   0        0        0     9314 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/insights.py
+-rw-r--r--   0        0        0     4615 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/recommenders.py
+-rw-r--r--   0        0        0     6711 2024-05-14 17:09:52.512891 dataprep_ml-24.5.1.1/dataprep_ml/splitters.py
+-rw-r--r--   0        0        0      626 2024-05-14 17:09:52.516891 dataprep_ml-24.5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 dataprep_ml-24.5.1.1/PKG-INFO
```

### Comparing `dataprep_ml-24.5.1.0/LICENSE` & `dataprep_ml-24.5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/README.md` & `dataprep_ml-24.5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/dataprep_ml/base.py` & `dataprep_ml-24.5.1.1/dataprep_ml/base.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/dataprep_ml/cleaners.py` & `dataprep_ml-24.5.1.1/dataprep_ml/cleaners.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/dataprep_ml/helpers.py` & `dataprep_ml-24.5.1.1/dataprep_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/dataprep_ml/imputers.py` & `dataprep_ml-24.5.1.1/dataprep_ml/imputers.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/dataprep_ml/insights.py` & `dataprep_ml-24.5.1.1/dataprep_ml/insights.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/dataprep_ml/recommenders.py` & `dataprep_ml-24.5.1.1/dataprep_ml/recommenders.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-24.5.1.0/dataprep_ml/splitters.py` & `dataprep_ml-24.5.1.1/dataprep_ml/splitters.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,19 +54,22 @@
     if stratify_on:
         reshuffle = not tss.get('is_timeseries', False)
         train, dev, test = stratify(data, pct_train, pct_dev, pct_test, stratify_on, seed, reshuffle)
     else:
         train, dev, test = simple_split(data, pct_train, pct_dev, pct_test)
 
     # Final assertions for time series
-    if min(len(train), len(dev)) < tss.get('window', 1):
-        raise Exception(f"Dataset size is too small for the specified window size ({tss.get('window', 1)})")
+    window = tss.get('window', 1) if tss.get('window', 1) else 1
+    horizon = tss.get('horizon', 1) if tss.get('horizon', 1) else 1
 
-    if min(len(train), len(dev), len(test)) < tss.get('horizon', 1):
-        raise Exception(f"Dataset size is too small for the specified horizon size ({tss.get('horizon', 1)})")
+    if min(len(train), len(dev)) < window:
+        raise Exception(f"Dataset size is too small for the specified window size ({window})")
+
+    if min(len(train), len(dev), len(test)) < horizon:
+        raise Exception(f"Dataset size is too small for the specified horizon size ({horizon})")
 
     return {"train": train, "test": test, "dev": dev, "stratified_on": stratify_on}
 
 
 def simple_split(data: pd.DataFrame,
                  pct_train: float,
                  pct_dev: float,
```

### Comparing `dataprep_ml-24.5.1.0/pyproject.toml` & `dataprep_ml-24.5.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataprep-ml"
-version = "24.5.1.0"
+version = "24.5.1.1"
 description = "Automated dataframe analysis for Machine Learning pipelines."
 authors = ["MindsDB Inc. <hello@mindsdb.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "dataprep_ml"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dataprep_ml-24.5.1.0/PKG-INFO` & `dataprep_ml-24.5.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataprep-ml
-Version: 24.5.1.0
+Version: 24.5.1.1
 Summary: Automated dataframe analysis for Machine Learning pipelines.
 License: GPL-3.0
 Author: MindsDB Inc.
 Author-email: hello@mindsdb.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dataprep-ml Version: 24.5.1.0 Summary: Automated
+Metadata-Version: 2.1 Name: dataprep-ml Version: 24.5.1.1 Summary: Automated
 dataframe analysis for Machine Learning pipelines. License: GPL-3.0 Author:
 MindsDB Inc. Author-email: hello@mindsdb.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: colorlog (>=6.5.0,<7.0.0) Requires-
```

