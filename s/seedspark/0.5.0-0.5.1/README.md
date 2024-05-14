# Comparing `tmp/seedspark-0.5.0.tar.gz` & `tmp/seedspark-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedspark-0.5.0.tar", max compression
+gzip compressed data, was "seedspark-0.5.1.tar", max compression
```

## Comparing `seedspark-0.5.0.tar` & `seedspark-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4265 2024-05-07 07:17:47.556809 seedspark-0.5.0/README.md
--rw-r--r--   0        0        0     4011 2024-05-14 17:08:54.332671 seedspark-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-14 07:18:38.410729 seedspark-0.5.0/seedspark/__init__.py
--rw-r--r--   0        0        0      107 2024-03-14 07:18:38.410888 seedspark-0.5.0/seedspark/apps/__init__.py
--rw-r--r--   0        0        0     7017 2024-04-30 17:21:49.929613 seedspark-0.5.0/seedspark/apps/clickhouse_delta.py
--rw-r--r--   0        0        0      184 2024-03-14 07:18:38.411243 seedspark-0.5.0/seedspark/configs/__init__.py
--rw-r--r--   0        0        0     2050 2024-03-14 07:18:38.411343 seedspark-0.5.0/seedspark/configs/clickhouse.py
--rw-r--r--   0        0        0     1848 2024-03-14 07:18:38.411438 seedspark-0.5.0/seedspark/configs/configs.py
--rw-r--r--   0        0        0       82 2024-03-14 07:18:38.411587 seedspark-0.5.0/seedspark/connections/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-14 07:18:38.411689 seedspark-0.5.0/seedspark/connections/clickhouse.py
--rw-r--r--   0        0        0      910 2024-03-14 07:18:38.411790 seedspark-0.5.0/seedspark/connections/clickhouse_dialect.py
--rw-r--r--   0        0        0        0 2024-03-14 07:18:38.411889 seedspark-0.5.0/seedspark/contrib/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 07:18:38.412009 seedspark-0.5.0/seedspark/contrib/testing/__init__.py
--rw-r--r--   0        0        0     2096 2024-05-02 19:20:00.182687 seedspark-0.5.0/seedspark/contrib/testing/spark.py
--rw-r--r--   0        0        0     1170 2024-04-30 17:15:26.324874 seedspark-0.5.0/seedspark/decorators.py
--rw-r--r--   0        0        0        0 2024-03-14 07:18:38.412344 seedspark-0.5.0/seedspark/examples/__init__.py
--rw-r--r--   0        0        0     2401 2024-03-14 07:18:38.412469 seedspark-0.5.0/seedspark/examples/clichouse_taxi.py
--rw-r--r--   0        0        0     2769 2024-05-01 18:39:47.879198 seedspark-0.5.0/seedspark/examples/music_sessions_explore.py
--rw-r--r--   0        0        0     6182 2024-05-07 07:17:44.883533 seedspark-0.5.0/seedspark/examples/music_sessions_top_n.py
--rw-r--r--   0        0        0     1158 2024-03-14 07:18:38.412573 seedspark-0.5.0/seedspark/examples/postgres.py
--rw-r--r--   0        0        0     1827 2024-03-14 07:18:38.412736 seedspark-0.5.0/seedspark/examples/sql/weekend_trip_metrics.sql
--rw-r--r--   0        0        0     2626 2024-03-14 07:18:38.412864 seedspark-0.5.0/seedspark/examples/weekend_fares_kpi.py
--rw-r--r--   0        0        0     1402 2024-04-30 17:21:49.929421 seedspark-0.5.0/seedspark/examples/word_count.py
--rw-r--r--   0        0        0     7524 2024-05-02 19:39:20.176920 seedspark-0.5.0/seedspark/sparkapp.py
--rw-r--r--   0        0        0     4908 1970-01-01 00:00:00.000000 seedspark-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4265 2024-05-07 07:17:47.556809 seedspark-0.5.1/README.md
+-rw-r--r--   0        0        0     4037 2024-05-14 17:24:29.031882 seedspark-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-14 07:18:38.410729 seedspark-0.5.1/seedspark/__init__.py
+-rw-r--r--   0        0        0      107 2024-03-14 07:18:38.410888 seedspark-0.5.1/seedspark/apps/__init__.py
+-rw-r--r--   0        0        0     7017 2024-04-30 17:21:49.929613 seedspark-0.5.1/seedspark/apps/clickhouse_delta.py
+-rw-r--r--   0        0        0      184 2024-03-14 07:18:38.411243 seedspark-0.5.1/seedspark/configs/__init__.py
+-rw-r--r--   0        0        0     2050 2024-03-14 07:18:38.411343 seedspark-0.5.1/seedspark/configs/clickhouse.py
+-rw-r--r--   0        0        0     1848 2024-03-14 07:18:38.411438 seedspark-0.5.1/seedspark/configs/configs.py
+-rw-r--r--   0        0        0       82 2024-03-14 07:18:38.411587 seedspark-0.5.1/seedspark/connections/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-14 07:18:38.411689 seedspark-0.5.1/seedspark/connections/clickhouse.py
+-rw-r--r--   0        0        0      910 2024-03-14 07:18:38.411790 seedspark-0.5.1/seedspark/connections/clickhouse_dialect.py
+-rw-r--r--   0        0        0        0 2024-03-14 07:18:38.411889 seedspark-0.5.1/seedspark/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 07:18:38.412009 seedspark-0.5.1/seedspark/contrib/testing/__init__.py
+-rw-r--r--   0        0        0     2096 2024-05-02 19:20:00.182687 seedspark-0.5.1/seedspark/contrib/testing/spark.py
+-rw-r--r--   0        0        0     1170 2024-04-30 17:15:26.324874 seedspark-0.5.1/seedspark/decorators.py
+-rw-r--r--   0        0        0        0 2024-03-14 07:18:38.412344 seedspark-0.5.1/seedspark/examples/__init__.py
+-rw-r--r--   0        0        0     2401 2024-03-14 07:18:38.412469 seedspark-0.5.1/seedspark/examples/clichouse_taxi.py
+-rw-r--r--   0        0        0     2769 2024-05-01 18:39:47.879198 seedspark-0.5.1/seedspark/examples/music_sessions_explore.py
+-rw-r--r--   0        0        0     6182 2024-05-07 07:17:44.883533 seedspark-0.5.1/seedspark/examples/music_sessions_top_n.py
+-rw-r--r--   0        0        0     1158 2024-03-14 07:18:38.412573 seedspark-0.5.1/seedspark/examples/postgres.py
+-rw-r--r--   0        0        0     1827 2024-03-14 07:18:38.412736 seedspark-0.5.1/seedspark/examples/sql/weekend_trip_metrics.sql
+-rw-r--r--   0        0        0     2626 2024-03-14 07:18:38.412864 seedspark-0.5.1/seedspark/examples/weekend_fares_kpi.py
+-rw-r--r--   0        0        0     1402 2024-04-30 17:21:49.929421 seedspark-0.5.1/seedspark/examples/word_count.py
+-rw-r--r--   0        0        0     7524 2024-05-02 19:39:20.176920 seedspark-0.5.1/seedspark/sparkapp.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 seedspark-0.5.1/PKG-INFO
```

### Comparing `seedspark-0.5.0/README.md` & `seedspark-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/pyproject.toml` & `seedspark-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "seedspark"
-version = "0.5.0"
-description = ""
+version = "0.5.1"
+description = "Spark ETL Utility Framework"
 authors = ["ChethanUK <chethanuk@outlook.com>"]
 readme = "README.md"
 
 ###########################################################################
 #                         MAIN DEPENDENCIES
 ###########################################################################
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pyspark = {extras = ["connect", "sql"], version = "^3.5.0"}
 sqlglot = "^20.11.0"
 loguru = "^0.7.2"
 onetl = "^0.10.1"
 delta-spark = "3.1.0"
 requests = "^2.31.0"
```

### Comparing `seedspark-0.5.0/seedspark/apps/clickhouse_delta.py` & `seedspark-0.5.1/seedspark/apps/clickhouse_delta.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/configs/clickhouse.py` & `seedspark-0.5.1/seedspark/configs/clickhouse.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/configs/configs.py` & `seedspark-0.5.1/seedspark/configs/configs.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/connections/clickhouse.py` & `seedspark-0.5.1/seedspark/connections/clickhouse.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/connections/clickhouse_dialect.py` & `seedspark-0.5.1/seedspark/connections/clickhouse_dialect.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/contrib/testing/spark.py` & `seedspark-0.5.1/seedspark/contrib/testing/spark.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/decorators.py` & `seedspark-0.5.1/seedspark/decorators.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/examples/clichouse_taxi.py` & `seedspark-0.5.1/seedspark/examples/clichouse_taxi.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/examples/music_sessions_explore.py` & `seedspark-0.5.1/seedspark/examples/music_sessions_explore.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/examples/music_sessions_top_n.py` & `seedspark-0.5.1/seedspark/examples/music_sessions_top_n.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/examples/postgres.py` & `seedspark-0.5.1/seedspark/examples/postgres.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/examples/sql/weekend_trip_metrics.sql` & `seedspark-0.5.1/seedspark/examples/sql/weekend_trip_metrics.sql`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/examples/weekend_fares_kpi.py` & `seedspark-0.5.1/seedspark/examples/weekend_fares_kpi.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/examples/word_count.py` & `seedspark-0.5.1/seedspark/examples/word_count.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/seedspark/sparkapp.py` & `seedspark-0.5.1/seedspark/sparkapp.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.5.0/PKG-INFO` & `seedspark-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: seedspark
-Version: 0.5.0
-Summary: 
+Version: 0.5.1
+Summary: Spark ETL Utility Framework
 Author: ChethanUK
 Author-email: chethanuk@outlook.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: delta-spark (==3.1.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: onetl (>=0.10.1,<0.11.0)
 Requires-Dist: pyspark[connect,sql] (>=3.5.0,<4.0.0)
```

