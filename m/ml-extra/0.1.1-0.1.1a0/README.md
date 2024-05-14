# Comparing `tmp/ml_extra-0.1.1.tar.gz` & `tmp/ml_extra-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_extra-0.1.1.tar", max compression
+gzip compressed data, was "ml_extra-0.1.1a0.tar", max compression
```

## Comparing `ml_extra-0.1.1.tar` & `ml_extra-0.1.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/calculations/classification_metrics.py
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/calculations/regression_metrics.py
--rw-r--r--   0        0        0      775 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/experiments/utils.py
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/artifacts/classfication.py
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/artifacts/regression.py
--rw-r--r--   0        0        0     3012 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/decorators/code.py
--rw-r--r--   0        0        0     1257 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/decorators/metrics.py
--rw-r--r--   0        0        0      673 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/decorators/params.py
--rw-r--r--   0        0        0     4392 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/decorators/utils.py
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/metrics/classification.py
--rw-r--r--   0        0        0        0 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/loggers/metrics/regression.py
--rw-r--r--   0        0        0      665 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/tests/inner_test/dummy_module.py
--rw-r--r--   0        0        0     4648 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/tests/logging_metrics.py
--rw-r--r--   0        0        0      428 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/tests/testing_classes.py
--rw-r--r--   0        0        0      387 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/tests/testing_functions.py
--rw-r--r--   0        0        0      157 2024-05-14 01:42:29.854099 ml_extra-0.1.1/ml_extra/utils/utils.py
--rw-r--r--   0        0        0      477 2024-05-14 01:42:29.854099 ml_extra-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 ml_extra-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.739048 ml_extra-0.1.1a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.739048 ml_extra-0.1.1a0/ml_extra/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.739048 ml_extra-0.1.1a0/ml_extra/calculations/classification_metrics.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.739048 ml_extra-0.1.1a0/ml_extra/calculations/regression_metrics.py
+-rw-r--r--   0        0        0      775 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/experiments/utils.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/artifacts/classfication.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/artifacts/regression.py
+-rw-r--r--   0        0        0     3012 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/decorators/code.py
+-rw-r--r--   0        0        0     1257 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/decorators/metrics.py
+-rw-r--r--   0        0        0      673 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/decorators/params.py
+-rw-r--r--   0        0        0     4392 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/decorators/utils.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/metrics/classification.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/loggers/metrics/regression.py
+-rw-r--r--   0        0        0      665 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/tests/inner_test/dummy_module.py
+-rw-r--r--   0        0        0     4648 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/tests/logging_metrics.py
+-rw-r--r--   0        0        0      428 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/tests/testing_classes.py
+-rw-r--r--   0        0        0      387 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/tests/testing_functions.py
+-rw-r--r--   0        0        0      157 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/ml_extra/utils/utils.py
+-rw-r--r--   0        0        0      479 2024-05-14 01:23:54.743048 ml_extra-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 ml_extra-0.1.1a0/PKG-INFO
```

### Comparing `ml_extra-0.1.1/ml_extra/experiments/utils.py` & `ml_extra-0.1.1a0/ml_extra/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.1/ml_extra/loggers/decorators/code.py` & `ml_extra-0.1.1a0/ml_extra/loggers/decorators/code.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.1/ml_extra/loggers/decorators/metrics.py` & `ml_extra-0.1.1a0/ml_extra/loggers/decorators/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.1/ml_extra/loggers/decorators/params.py` & `ml_extra-0.1.1a0/ml_extra/loggers/decorators/params.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.1/ml_extra/loggers/decorators/utils.py` & `ml_extra-0.1.1a0/ml_extra/loggers/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.1/ml_extra/tests/inner_test/dummy_module.py` & `ml_extra-0.1.1a0/ml_extra/tests/inner_test/dummy_module.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.1/ml_extra/tests/logging_metrics.py` & `ml_extra-0.1.1a0/ml_extra/tests/logging_metrics.py`

 * *Files identical despite different names*

### Comparing `ml_extra-0.1.1/PKG-INFO` & `ml_extra-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-extra
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: 
 Author: Manuel Gil
 Author-email: manuelgilsitio@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

