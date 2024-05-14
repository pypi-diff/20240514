# Comparing `tmp/dagster-toolbox-0.0.8.tar.gz` & `tmp/dagster-toolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-toolbox-0.0.8.tar", last modified: Wed Oct 11 16:12:40 2023, max compression
+gzip compressed data, was "dagster-toolbox-0.0.9.tar", last modified: Wed Oct 11 20:36:54 2023, max compression
```

## Comparing `dagster-toolbox-0.0.8.tar` & `dagster-toolbox-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.983200 dagster-toolbox-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-10-11 16:12:40.983200 dagster-toolbox-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.975200 dagster-toolbox-0.0.8/dagster_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.975200 dagster-toolbox-0.0.8/dagster_toolbox/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/functions/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/functions/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/functions/google_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/functions/partitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/functions/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/functions/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.979200 dagster-toolbox-0.0.8/dagster_toolbox/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/csv_partitioned_io_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/json_partitioned_io_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/postgres_io_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/postgres_partitioned_io_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/resources/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.979200 dagster-toolbox-0.0.8/dagster_toolbox/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.979200 dagster-toolbox-0.0.8/dagster_toolbox/types/common/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/common/cities.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/common/continents.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/common/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/common/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/common/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/common/subregions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.979200 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/container_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/continent_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/country_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/currency_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/language_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/subdivision_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/units_of_measure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.979200 dagster-toolbox-0.0.8/dagster_toolbox/types/geonames/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/geonames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/geonames/postal_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.983200 dagster-toolbox-0.0.8/dagster_toolbox/types/google_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/google_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/google_analytics/google_analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.983200 dagster-toolbox-0.0.8/dagster_toolbox/types/open_data_fr/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/open_data_fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/dagster_toolbox/types/open_data_fr/agriculture_ministry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 16:12:40.975200 dagster-toolbox-0.0.8/dagster_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-10-11 16:12:40.000000 dagster-toolbox-0.0.8/dagster_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-10-11 16:12:40.000000 dagster-toolbox-0.0.8/dagster_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 16:12:40.000000 dagster-toolbox-0.0.8/dagster_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-11 16:12:40.000000 dagster-toolbox-0.0.8/dagster_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-11 16:12:40.000000 dagster-toolbox-0.0.8/dagster_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 16:12:40.983200 dagster-toolbox-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-11 16:12:29.000000 dagster-toolbox-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.336891 dagster-toolbox-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-10-11 20:36:54.336891 dagster-toolbox-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.328891 dagster-toolbox-0.0.9/dagster_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.332891 dagster-toolbox-0.0.9/dagster_toolbox/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/functions/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/functions/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/functions/google_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/functions/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/functions/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/functions/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.332891 dagster-toolbox-0.0.9/dagster_toolbox/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/csv_partitioned_io_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/json_partitioned_io_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/postgres_io_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/postgres_partitioned_io_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/resources/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.332891 dagster-toolbox-0.0.9/dagster_toolbox/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.332891 dagster-toolbox-0.0.9/dagster_toolbox/types/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/common/cities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/common/continents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/common/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/common/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/common/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/common/subregions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.336891 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/container_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/continent_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/country_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/currency_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/language_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/subdivision_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/units_of_measure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.336891 dagster-toolbox-0.0.9/dagster_toolbox/types/geonames/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/geonames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/geonames/postal_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.336891 dagster-toolbox-0.0.9/dagster_toolbox/types/google_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/google_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/google_analytics/google_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.336891 dagster-toolbox-0.0.9/dagster_toolbox/types/open_data_fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/open_data_fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/dagster_toolbox/types/open_data_fr/agriculture_ministry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:36:54.328891 dagster-toolbox-0.0.9/dagster_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-10-11 20:36:54.000000 dagster-toolbox-0.0.9/dagster_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-10-11 20:36:54.000000 dagster-toolbox-0.0.9/dagster_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 20:36:54.000000 dagster-toolbox-0.0.9/dagster_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-11 20:36:54.000000 dagster-toolbox-0.0.9/dagster_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-11 20:36:54.000000 dagster-toolbox-0.0.9/dagster_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 20:36:54.336891 dagster-toolbox-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-11 20:36:42.000000 dagster-toolbox-0.0.9/setup.py
```

### Comparing `dagster-toolbox-0.0.8/LICENSE` & `dagster-toolbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/PKG-INFO` & `dagster-toolbox-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A set of tools to ease Dagster usage
 Home-page: https://github.com/nicolasramy/dagster-toolbox
 Author: Nicolas RAMY
 Author-email: nicolas.ramy@darkelda.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/functions/dataframe.py` & `dagster-toolbox-0.0.9/dagster_toolbox/functions/dataframe.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/functions/ftp.py` & `dagster-toolbox-0.0.9/dagster_toolbox/functions/ftp.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/functions/google_analytics.py` & `dagster-toolbox-0.0.9/dagster_toolbox/functions/google_analytics.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/functions/sftp.py` & `dagster-toolbox-0.0.9/dagster_toolbox/functions/sftp.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/functions/text.py` & `dagster-toolbox-0.0.9/dagster_toolbox/functions/text.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/__init__.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from .csv_partitioned_io_manager import csv_partitioned_io_manager
 from .json_partitioned_io_manager import json_partitioned_io_manager
 from .postgres_partitioned_io_manager import postgres_partitioned_io_manager
 from .postgres_io_manager import postgres_io_manager
 from .object_storage import (
     analytics_objects,
+    connecting_objects,
     customers_objects,
     datalake_objects,
     datawarehouse_objects,
     experiments_objects,
     external_sources_objects,
     legacy_objects,
     logs_objects,
     miscellaneous_objects,
-    saas_objects,
     test_objects,
 )
 from .vault import vault
 
 
 __all__ = [
     # IO Managers
     "csv_partitioned_io_manager",
     "json_partitioned_io_manager",
     "postgres_partitioned_io_manager",
     "postgres_io_manager",
     # ObjectStorage
     "analytics_objects",
+    "connecting_objects",
     "customers_objects",
     "datalake_objects",
     "datawarehouse_objects",
     "experiments_objects",
     "external_sources_objects",
     "legacy_objects",
     "logs_objects",
     "miscellaneous_objects",
-    "saas_objects",
     "test_objects",
     "vault",
 ]
```

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/abstract.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/abstract.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/csv_partitioned_io_manager.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/json_partitioned_io_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 from io import BytesIO
 
 import pandas
-from slugify import slugify
 
 from dagster import (
     MemoizableIOManager,
     io_manager,
     MetadataValue,
     Field,
     StringSource,
     get_dagster_logger,
 )
 
 from dagster import _check as check
 
 
-class CSVPartitionedIOManager(MemoizableIOManager):
+class JsonPartitionedIOManager(MemoizableIOManager):
     def __init__(
         self,
         s3_bucket,
         s3_session,
         s3_prefix=None,
     ):
         self.logger = get_dagster_logger()
 
         self.bucket = check.str_param(s3_bucket, "s3_bucket")
         self.s3_prefix = check.opt_str_param(s3_prefix, "s3_prefix")
         self.s3 = s3_session
         self.s3.list_objects(Bucket=self.bucket, MaxKeys=1)
 
     def _get_path(self, context) -> str:
-        context.log.debug(context.get_asset_identifier())
-
         if context.has_asset_key:
             path = context.get_asset_identifier()
             try:
                 del path[path.index(self.bucket)]
 
             except ValueError:
                 bucket_key = self.bucket.replace("-", "_")
                 del path[path.index(bucket_key)]
 
         else:
             path = ["storage", *context.get_identifier()]
 
-        new_path = list(map(slugify, path[:-1]))
-        new_path.append(slugify(path[-1]))
-
-        return "/".join(new_path) + ".csv"
+        return "/".join(path) + ".json"
 
     def has_output(self, context):
         key = self._get_path(context)
         return self._has_object(key)
 
     def _rm_object(self, key):
         check.str_param(key, "key")
@@ -86,32 +80,22 @@
                 f"Object not found from {self._uri_for_key(key)}"
             )
             return None
 
         context.log.debug(f"Loading S3 object from: {self._uri_for_key(key)}")
 
         stream_bytes = BytesIO(
-            self.s3.get_object(
-                bucket_name=self.bucket,
-                object_name=key
-            )["Body"].read()
+            self.s3.get_object(Bucket=self.bucket, Key=key)["Body"].read()
         )
 
-        try:
-            obj = pandas.read_csv(
-                stream_bytes,
-                encoding="utf-8",
-                parse_dates=["partition_key"],
-                dayfirst=False,
-            )
-        except ValueError:
-            obj = pandas.read_csv(
-                stream_bytes,
-                encoding="utf-8",
-            )
+        obj = pandas.read_json(
+            stream_bytes,
+            orient="records",
+            encoding="utf-8",
+        )
 
         return obj
 
     def handle_output(self, context, obj):
         if isinstance(context.dagster_type.typing_type, type(None)):
             check.invariant(
                 obj is None,
@@ -126,18 +110,19 @@
         context.log.debug(f"Writing S3 object at: {path}")
 
         if self._has_object(key):
             context.log.warning(f"Removing existing S3 key: {key}")
             self._rm_object(key)
 
         if obj is not None:
-            pickled_obj = obj.to_csv(
-                encoding="utf_8",
-                index=False,
+            pickled_obj = obj.to_json(
+                orient="records",
+                date_format="iso",
             )
+
             pickled_obj_bytes = BytesIO(bytes(pickled_obj, "utf-8"))
             self.s3.upload_fileobj(pickled_obj_bytes, self.bucket, key)
             context.add_output_metadata(
                 {"uri": MetadataValue.path(path)} | context.metadata
             )
 
         else:
@@ -149,16 +134,16 @@
 @io_manager(
     config_schema={
         "s3_bucket": Field(StringSource),
         "s3_prefix": Field(StringSource, is_required=False, default_value=""),
     },
     required_resource_keys={"s3"},
 )
-def csv_partitioned_io_manager(init_context):
+def json_partitioned_io_manager(init_context):
     s3_session = init_context.resources.s3
     s3_bucket = init_context.resource_config.get("s3_bucket")
     s3_prefix = init_context.resource_config.get("s3_prefix")
 
-    _csv_partitioned_io_manager = CSVPartitionedIOManager(
+    _json_partitioned_io_manager = JsonPartitionedIOManager(
         s3_bucket, s3_session, s3_prefix=s3_prefix
     )
-    return _csv_partitioned_io_manager
+    return _json_partitioned_io_manager
```

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/json_partitioned_io_manager.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/csv_partitioned_io_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 from io import BytesIO
 
 import pandas
+from slugify import slugify
 
 from dagster import (
     MemoizableIOManager,
     io_manager,
     MetadataValue,
     Field,
     StringSource,
     get_dagster_logger,
 )
 
 from dagster import _check as check
 
 
-class JsonPartitionedIOManager(MemoizableIOManager):
+class CSVPartitionedIOManager(MemoizableIOManager):
     def __init__(
         self,
         s3_bucket,
         s3_session,
         s3_prefix=None,
     ):
         self.logger = get_dagster_logger()
 
         self.bucket = check.str_param(s3_bucket, "s3_bucket")
         self.s3_prefix = check.opt_str_param(s3_prefix, "s3_prefix")
         self.s3 = s3_session
         self.s3.list_objects(Bucket=self.bucket, MaxKeys=1)
 
     def _get_path(self, context) -> str:
+        context.log.debug(context.get_asset_identifier())
+
         if context.has_asset_key:
             path = context.get_asset_identifier()
             try:
                 del path[path.index(self.bucket)]
 
             except ValueError:
                 bucket_key = self.bucket.replace("-", "_")
                 del path[path.index(bucket_key)]
 
         else:
             path = ["storage", *context.get_identifier()]
 
-        return "/".join(path) + ".json"
+        new_path = list(map(slugify, path[:-1]))
+        new_path.append(slugify(path[-1]))
+
+        return "/".join(new_path) + ".csv"
 
     def has_output(self, context):
         key = self._get_path(context)
         return self._has_object(key)
 
     def _rm_object(self, key):
         check.str_param(key, "key")
@@ -80,25 +86,18 @@
                 f"Object not found from {self._uri_for_key(key)}"
             )
             return None
 
         context.log.debug(f"Loading S3 object from: {self._uri_for_key(key)}")
 
         stream_bytes = BytesIO(
-            self.s3.get_object(
-                bucket_name=self.bucket,
-                object_name=key
-            )["Body"].read()
+            self.s3.get_object(Bucket=self.bucket, Key=key)["Body"].read()
         )
 
-        obj = pandas.read_json(
-            stream_bytes,
-            orient="records",
-            encoding="utf-8",
-        )
+        obj = pandas.read_csv(stream_bytes, encoding="utf-8")
 
         return obj
 
     def handle_output(self, context, obj):
         if isinstance(context.dagster_type.typing_type, type(None)):
             check.invariant(
                 obj is None,
@@ -113,19 +112,18 @@
         context.log.debug(f"Writing S3 object at: {path}")
 
         if self._has_object(key):
             context.log.warning(f"Removing existing S3 key: {key}")
             self._rm_object(key)
 
         if obj is not None:
-            pickled_obj = obj.to_json(
-                orient="records",
-                date_format="iso",
+            pickled_obj = obj.to_csv(
+                encoding="utf_8",
+                index=False,
             )
-
             pickled_obj_bytes = BytesIO(bytes(pickled_obj, "utf-8"))
             self.s3.upload_fileobj(pickled_obj_bytes, self.bucket, key)
             context.add_output_metadata(
                 {"uri": MetadataValue.path(path)} | context.metadata
             )
 
         else:
@@ -137,16 +135,16 @@
 @io_manager(
     config_schema={
         "s3_bucket": Field(StringSource),
         "s3_prefix": Field(StringSource, is_required=False, default_value=""),
     },
     required_resource_keys={"s3"},
 )
-def json_partitioned_io_manager(init_context):
+def csv_partitioned_io_manager(init_context):
     s3_session = init_context.resources.s3
     s3_bucket = init_context.resource_config.get("s3_bucket")
     s3_prefix = init_context.resource_config.get("s3_prefix")
 
-    _json_partitioned_io_manager = JsonPartitionedIOManager(
+    _csv_partitioned_io_manager = CSVPartitionedIOManager(
         s3_bucket, s3_session, s3_prefix=s3_prefix
     )
-    return _json_partitioned_io_manager
+    return _csv_partitioned_io_manager
```

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/object_storage.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/object_storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 
 
 @resource
 def analytics_objects(init_context):
     return Analytics()
 
 
+class Connecting(ObjectStorage):
+    bucket = "connecting"
+
+
+@resource
+def connecting_objects(init_context):
+    return Connecting()
+
+
 class Customers(ObjectStorage):
     bucket = "customers"
 
 
 @resource
 def customers_objects(init_context):
     return Customers()
@@ -79,23 +88,14 @@
 
 
 @resource
 def miscellaneous_objects(init_context):
     return Miscellaneous()
 
 
-class SaaS(ObjectStorage):
-    bucket = "saas"
-
-
-@resource
-def saas_objects(init_context):
-    return SaaS()
-
-
 class Test(ObjectStorage):
     bucket = "test"
 
 
 @resource
 def test_objects(init_context):
     return Test()
```

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/postgres_io_manager.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/postgres_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/postgres_partitioned_io_manager.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/postgres_partitioned_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/resources/vault.py` & `dagster-toolbox-0.0.9/dagster_toolbox/resources/vault.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/__init__.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/common/cities.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/common/cities.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/common/countries.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/common/countries.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/common/postcodes.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/common/postcodes.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/common/regions.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/common/regions.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/common/subregions.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/common/subregions.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/__init__.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/container_codes.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/container_codes.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/country_codes.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/country_codes.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/currency_codes.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/currency_codes.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/language_codes.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/language_codes.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/subdivision_codes.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/subdivision_codes.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/datahub/units_of_measure.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/datahub/units_of_measure.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/geonames/postal_codes.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/geonames/postal_codes.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/google_analytics/google_analytics.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/google_analytics/google_analytics.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox/types/open_data_fr/agriculture_ministry.py` & `dagster-toolbox-0.0.9/dagster_toolbox/types/open_data_fr/agriculture_ministry.py`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox.egg-info/PKG-INFO` & `dagster-toolbox-0.0.9/dagster_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A set of tools to ease Dagster usage
 Home-page: https://github.com/nicolasramy/dagster-toolbox
 Author: Nicolas RAMY
 Author-email: nicolas.ramy@darkelda.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dagster-toolbox-0.0.8/dagster_toolbox.egg-info/SOURCES.txt` & `dagster-toolbox-0.0.9/dagster_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-toolbox-0.0.8/setup.py` & `dagster-toolbox-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dagster-toolbox",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     author="Nicolas RAMY",
     author_email="nicolas.ramy@darkelda.com",
     license="MIT",
     description="A set of tools to ease Dagster usage",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

