# Comparing `tmp/seedspark-0.1.7.tar.gz` & `tmp/seedspark-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedspark-0.1.7.tar", max compression
+gzip compressed data, was "seedspark-0.5.0.tar", max compression
```

## Comparing `seedspark-0.1.7.tar` & `seedspark-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     2621 2022-03-15 11:53:17.875443 seedspark-0.1.7/README.md
--rw-r--r--   0        0        0     3844 2022-03-15 14:08:44.852135 seedspark-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       46 2022-03-09 19:30:08.417780 seedspark-0.1.7/seedspark/__init__.py
--rw-r--r--   0        0        0       93 2022-03-09 19:56:17.611401 seedspark-0.1.7/seedspark/configs/__init__.py
--rw-r--r--   0        0        0     1173 2022-03-09 19:56:17.612094 seedspark-0.1.7/seedspark/configs/configs.py
--rw-r--r--   0        0        0      118 2022-03-09 19:59:04.777353 seedspark-0.1.7/seedspark/contrib/__init__.py
--rw-r--r--   0        0        0      212 2022-03-09 19:56:17.627892 seedspark-0.1.7/seedspark/contrib/test/__init__.py
--rw-r--r--   0        0        0     3361 2022-03-09 19:56:17.628283 seedspark-0.1.7/seedspark/contrib/test/base_airflow_test.py
--rw-r--r--   0        0        0     6639 2022-03-09 19:56:17.628663 seedspark-0.1.7/seedspark/contrib/test/base_spark_test.py
--rw-r--r--   0        0        0      110 2022-03-09 19:56:17.638675 seedspark-0.1.7/seedspark/dataquality/__init__.py
--rw-r--r--   0        0        0     1145 2022-03-09 19:56:17.638958 seedspark-0.1.7/seedspark/dataquality/ge.py
--rw-r--r--   0        0        0        0 2022-03-09 19:56:17.639246 seedspark-0.1.7/seedspark/dataquality/service.py
--rw-r--r--   0        0        0      215 2022-03-09 19:56:17.654600 seedspark-0.1.7/seedspark/spark/__init__.py
--rw-r--r--   0        0        0        0 2022-03-09 19:56:17.654927 seedspark-0.1.7/seedspark/spark/dataframe/__init__.py
--rw-r--r--   0        0        0        0 2022-03-09 19:56:17.655297 seedspark-0.1.7/seedspark/spark/dataframe/compare/__init__.py
--rw-r--r--   0        0        0    17096 2022-03-09 20:05:21.798404 seedspark-0.1.7/seedspark/spark/dataframe/compare/df_compare.py
--rw-r--r--   0        0        0     9456 2022-03-09 19:56:17.655912 seedspark-0.1.7/seedspark/spark/dataframe/compare/schema_comparer.py
--rw-r--r--   0        0        0     2351 2022-03-09 19:56:17.656256 seedspark-0.1.7/seedspark/spark/dataframe/utils.py
--rw-r--r--   0        0        0     7817 2022-03-09 19:56:17.656514 seedspark-0.1.7/seedspark/spark/sparkapp.py
--rw-r--r--   0        0        0      100 2022-03-09 19:56:17.665124 seedspark-0.1.7/seedspark/utils/__init__.py
--rw-r--r--   0        0        0     2989 2022-03-09 19:56:17.665383 seedspark-0.1.7/seedspark/utils/_datetime.py
--rw-r--r--   0        0        0     1719 2022-03-09 19:56:17.665642 seedspark-0.1.7/seedspark/utils/json.py
--rw-r--r--   0        0        0     3689 2022-03-15 14:09:08.163626 seedspark-0.1.7/setup.py
--rw-r--r--   0        0        0     4125 2022-03-15 14:09:08.163975 seedspark-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4265 2024-05-07 07:17:47.556809 seedspark-0.5.0/README.md
+-rw-r--r--   0        0        0     4011 2024-05-14 17:08:54.332671 seedspark-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-14 07:18:38.410729 seedspark-0.5.0/seedspark/__init__.py
+-rw-r--r--   0        0        0      107 2024-03-14 07:18:38.410888 seedspark-0.5.0/seedspark/apps/__init__.py
+-rw-r--r--   0        0        0     7017 2024-04-30 17:21:49.929613 seedspark-0.5.0/seedspark/apps/clickhouse_delta.py
+-rw-r--r--   0        0        0      184 2024-03-14 07:18:38.411243 seedspark-0.5.0/seedspark/configs/__init__.py
+-rw-r--r--   0        0        0     2050 2024-03-14 07:18:38.411343 seedspark-0.5.0/seedspark/configs/clickhouse.py
+-rw-r--r--   0        0        0     1848 2024-03-14 07:18:38.411438 seedspark-0.5.0/seedspark/configs/configs.py
+-rw-r--r--   0        0        0       82 2024-03-14 07:18:38.411587 seedspark-0.5.0/seedspark/connections/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-14 07:18:38.411689 seedspark-0.5.0/seedspark/connections/clickhouse.py
+-rw-r--r--   0        0        0      910 2024-03-14 07:18:38.411790 seedspark-0.5.0/seedspark/connections/clickhouse_dialect.py
+-rw-r--r--   0        0        0        0 2024-03-14 07:18:38.411889 seedspark-0.5.0/seedspark/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 07:18:38.412009 seedspark-0.5.0/seedspark/contrib/testing/__init__.py
+-rw-r--r--   0        0        0     2096 2024-05-02 19:20:00.182687 seedspark-0.5.0/seedspark/contrib/testing/spark.py
+-rw-r--r--   0        0        0     1170 2024-04-30 17:15:26.324874 seedspark-0.5.0/seedspark/decorators.py
+-rw-r--r--   0        0        0        0 2024-03-14 07:18:38.412344 seedspark-0.5.0/seedspark/examples/__init__.py
+-rw-r--r--   0        0        0     2401 2024-03-14 07:18:38.412469 seedspark-0.5.0/seedspark/examples/clichouse_taxi.py
+-rw-r--r--   0        0        0     2769 2024-05-01 18:39:47.879198 seedspark-0.5.0/seedspark/examples/music_sessions_explore.py
+-rw-r--r--   0        0        0     6182 2024-05-07 07:17:44.883533 seedspark-0.5.0/seedspark/examples/music_sessions_top_n.py
+-rw-r--r--   0        0        0     1158 2024-03-14 07:18:38.412573 seedspark-0.5.0/seedspark/examples/postgres.py
+-rw-r--r--   0        0        0     1827 2024-03-14 07:18:38.412736 seedspark-0.5.0/seedspark/examples/sql/weekend_trip_metrics.sql
+-rw-r--r--   0        0        0     2626 2024-03-14 07:18:38.412864 seedspark-0.5.0/seedspark/examples/weekend_fares_kpi.py
+-rw-r--r--   0        0        0     1402 2024-04-30 17:21:49.929421 seedspark-0.5.0/seedspark/examples/word_count.py
+-rw-r--r--   0        0        0     7524 2024-05-02 19:39:20.176920 seedspark-0.5.0/seedspark/sparkapp.py
+-rw-r--r--   0        0        0     4908 1970-01-01 00:00:00.000000 seedspark-0.5.0/PKG-INFO
```

