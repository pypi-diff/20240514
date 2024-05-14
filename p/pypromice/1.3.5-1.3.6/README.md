# Comparing `tmp/pypromice-1.3.5.tar.gz` & `tmp/pypromice-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypromice-1.3.5.tar", last modified: Thu Apr 25 06:17:06 2024, max compression
+gzip compressed data, was "pypromice-1.3.6.tar", last modified: Tue May 14 05:10:54 2024, max compression
```

## Comparing `pypromice-1.3.5.tar` & `pypromice-1.3.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.272019 pypromice-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-25 06:17:02.000000 pypromice-1.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 06:17:02.000000 pypromice-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-25 06:17:06.272019 pypromice-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-25 06:17:02.000000 pypromice-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:17:06.272019 pypromice-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-25 06:17:02.000000 pypromice-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.248018 pypromice-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.252018 pypromice-1.3.5/src/pypromice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.252018 pypromice-1.3.5/src/pypromice/get/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/get/get.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/get/get_promice_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.256018 pypromice-1.3.5/src/pypromice/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/bufr_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/bufr_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/get_bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/positions_seed.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/real_time_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/station_configurations.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.256018 pypromice-1.3.5/src/pypromice/process/
--rw-r--r--   0 runner    (1001) docker     (127)    22818 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/L0toL1.py
--rw-r--r--   0 runner    (1001) docker     (127)    25577 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/L1toL2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18238 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/L2toL3.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29844 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/aws.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/get_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/join_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/value_clipping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.260018 pypromice-1.3.5/src/pypromice/qc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/github_data_issues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.260018 pypromice-1.3.5/src/pypromice/qc/percentiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/compute_thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/outlier_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/thresholds.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/persistence_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.268018 pypromice-1.3.5/src/pypromice/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_config1.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_config2.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_email
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_percentile.py
--rw-r--r--   0 runner    (1001) docker     (127)  1626942 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw1.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3337781 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_DataTable2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   348047 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_SlimTableMem1.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1993699 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_transmitted1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_transmitted2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.272019 pypromice-1.3.5/src/pypromice/tx/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/get_l0tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/get_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/get_watsontx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.272019 pypromice-1.3.5/src/pypromice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.517717 pypromice-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 05:10:50.000000 pypromice-1.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 05:10:50.000000 pypromice-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-14 05:10:54.517717 pypromice-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-14 05:10:50.000000 pypromice-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 05:10:54.517717 pypromice-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-14 05:10:50.000000 pypromice-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.497717 pypromice-1.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.501716 pypromice-1.3.6/src/pypromice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.501716 pypromice-1.3.6/src/pypromice/get/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/get/get.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/get/get_promice_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.501716 pypromice-1.3.6/src/pypromice/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/postprocess/bufr_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/postprocess/bufr_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/postprocess/get_bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/postprocess/positions_seed.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/postprocess/real_time_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/postprocess/station_configurations.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.505717 pypromice-1.3.6/src/pypromice/process/
+-rw-r--r--   0 runner    (1001) docker     (127)    22818 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/L0toL1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28532 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/L1toL2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18311 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/L2toL3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32195 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/aws.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/get_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/join_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/value_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13313 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/process/variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.505717 pypromice-1.3.6/src/pypromice/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/github_data_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.505717 pypromice-1.3.6/src/pypromice/qc/percentiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/percentiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/percentiles/compute_thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/percentiles/outlier_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/percentiles/thresholds.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/qc/persistence_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.517717 pypromice-1.3.6/src/pypromice/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_config1.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_config2.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_email
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1626942 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_raw1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3337781 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_raw_DataTable2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   348047 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_raw_SlimTableMem1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1993699 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_raw_transmitted1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/test/test_raw_transmitted2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.517717 pypromice-1.3.6/src/pypromice/tx/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/tx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/tx/get_l0tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/tx/get_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/tx/get_watsontx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/tx/payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/tx/payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-05-14 05:10:50.000000 pypromice-1.3.6/src/pypromice/tx/tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:10:54.517717 pypromice-1.3.6/src/pypromice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-14 05:10:54.000000 pypromice-1.3.6/src/pypromice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-14 05:10:54.000000 pypromice-1.3.6/src/pypromice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 05:10:54.000000 pypromice-1.3.6/src/pypromice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 05:10:54.000000 pypromice-1.3.6/src/pypromice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 05:10:54.000000 pypromice-1.3.6/src/pypromice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 05:10:54.000000 pypromice-1.3.6/src/pypromice.egg-info/top_level.txt
```

### Comparing `pypromice-1.3.5/LICENSE.txt` & `pypromice-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/PKG-INFO` & `pypromice-1.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.3.5
+Version: 1.3.6
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
@@ -19,19 +19,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: xarray>=2022.6.0
 Requires-Dist: toml
 Requires-Dist: scipy>=1.9.0
-Requires-Dist: scikit-learn>=1.1.0
 Requires-Dist: Bottleneck
 Requires-Dist: netcdf4
 Requires-Dist: pyDataverse
 Requires-Dist: eccodes
+Requires-Dist: scikit-learn>=1.1.0
 
 # pypromice
 [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://badge.fury.io/py/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/version.svg)](https://anaconda.org/conda-forge/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/platforms.svg)](https://anaconda.org/conda-forge/pypromice) [![](<https://img.shields.io/badge/Dataverse DOI-10.22008/FK2/3TSBF0-orange>)](https://www.doi.org/10.22008/FK2/3TSBF0) [![DOI](https://joss.theoj.org/papers/10.21105/joss.05298/status.svg)](https://doi.org/10.21105/joss.05298) [![Documentation Status](https://readthedocs.org/projects/pypromice/badge/?version=latest)](https://pypromice.readthedocs.io/en/latest/?badge=latest)
  
 pypromice is designed for processing and handling [PROMICE](https://promice.org) automated weather station (AWS) data.
 
 It is envisioned for pypromice to be the go-to toolbox for handling and processing [PROMICE](https://promice.dk) and [GC-Net](http://cires1.colorado.edu/steffen/gcnet/) datasets. New releases of pypromice are uploaded alongside PROMICE AWS data releases to our [Dataverse](https://dataverse.geus.dk/dataverse/PROMICE) for transparency purposes and to encourage collaboration on improving our data. Please visit the pypromice [readthedocs](https://pypromice.readthedocs.io/en/latest/?badge=latest) for more information. 
@@ -54,15 +54,22 @@
 $ conda install pypromice -c conda-forge
 ```
 
 ```
 $ pip install pypromice
 ```
 
-For the most up-to-date version, pypromice can be installed directly from the repo: 
+The [eccodes](https://confluence.ecmwf.int/display/ECC/ecCodes+installation) package for pypromice's post-processing functionality needs to be installed specifically in the pip distribution:
+
+```
+$ conda install eccodes -c conda-forge
+$ pip install pypromice
+```
+
+And for the most up-to-date version of pypromice, the package can be cloned and installed directly from the repo: 
 
 ```
 $ pip install --upgrade git+http://github.com/GEUS-Glaciology-and-Climate/pypromice.git
 ```
 
 ### Developer install
 	
@@ -72,23 +79,7 @@
 $ conda create --name pypromice python=3.8
 $ conda activate pypromice
 $ git clone git@github.com:GEUS-Glaciology-and-Climate/pypromice.git
 $ cd pypromice/
 $ pip install .
 ```
 
-### Additional dependencies
-
-Additional packages are required if you wish to use pypromice's post-processing functionality. 
-
-[eccodes](https://confluence.ecmwf.int/display/ECC/ecCodes+installation) is the official package for BUFR encoding and decoding. Try firstly to install with conda-forge like so:
-
-```
-$ conda install -c conda-forge eccodes
-```
-
-If the environment cannot resolve the eccodes installation then follow the steps documented [here](https://gist.github.com/MHBalsmeier/a01ad4e07ecf467c90fad2ac7719844a) to download eccodes and then install eccodes' python bindings using pip.
-
-```
-$ pip3 install eccodes-python
-```
-
```

### Comparing `pypromice-1.3.5/README.md` & `pypromice-1.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,22 @@
 $ conda install pypromice -c conda-forge
 ```
 
 ```
 $ pip install pypromice
 ```
 
-For the most up-to-date version, pypromice can be installed directly from the repo: 
+The [eccodes](https://confluence.ecmwf.int/display/ECC/ecCodes+installation) package for pypromice's post-processing functionality needs to be installed specifically in the pip distribution:
+
+```
+$ conda install eccodes -c conda-forge
+$ pip install pypromice
+```
+
+And for the most up-to-date version of pypromice, the package can be cloned and installed directly from the repo: 
 
 ```
 $ pip install --upgrade git+http://github.com/GEUS-Glaciology-and-Climate/pypromice.git
 ```
 
 ### Developer install
 	
@@ -41,23 +48,7 @@
 $ conda create --name pypromice python=3.8
 $ conda activate pypromice
 $ git clone git@github.com:GEUS-Glaciology-and-Climate/pypromice.git
 $ cd pypromice/
 $ pip install .
 ```
 
-### Additional dependencies
-
-Additional packages are required if you wish to use pypromice's post-processing functionality. 
-
-[eccodes](https://confluence.ecmwf.int/display/ECC/ecCodes+installation) is the official package for BUFR encoding and decoding. Try firstly to install with conda-forge like so:
-
-```
-$ conda install -c conda-forge eccodes
-```
-
-If the environment cannot resolve the eccodes installation then follow the steps documented [here](https://gist.github.com/MHBalsmeier/a01ad4e07ecf467c90fad2ac7719844a) to download eccodes and then install eccodes' python bindings using pip.
-
-```
-$ pip3 install eccodes-python
-```
-
```

### Comparing `pypromice-1.3.5/setup.py` & `pypromice-1.3.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypromice",
-    version="1.3.5",
+    version="1.3.6",
     author="GEUS Glaciology and Climate",
     description="PROMICE/GC-Net data processing toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GEUS-Glaciology-and-Climate/pypromice",
     project_urls={
         "Bug Tracker": "https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues",
@@ -27,18 +27,21 @@
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     include_package_data = True,
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.8",
     package_data={
+    	"pypromice.process": ["metadata.csv", "variables.csv"],
+    	"pypromice.tx": ["payload_formats.csv", "payload_types.csv"],
         "pypromice.qc.percentiles": ["thresholds.csv"],
         "pypromice.postprocess": ["station_configurations.toml", "positions_seed.csv"],
     },
-    install_requires=['numpy>=1.23.0', 'pandas>=1.5.0', 'xarray>=2022.6.0', 'toml', 'scipy>=1.9.0', 'scikit-learn>=1.1.0', 'Bottleneck', 'netcdf4', 'pyDataverse', 'eccodes'],
+    install_requires=['numpy>=1.23.0', 'pandas>=1.5.0', 'xarray>=2022.6.0', 'toml', 'scipy>=1.9.0', 'Bottleneck', 'netcdf4', 'pyDataverse', 'eccodes','scikit-learn>=1.1.0'],
+#    extras_require={'postprocess': ['eccodes','scikit-learn>=1.1.0']},
     entry_points={
     'console_scripts': [
         'get_promice_data = pypromice.get.get_promice_data:get_promice_data',
         'get_l0tx = pypromice.tx.get_l0tx:get_l0tx',
         'get_l3 = pypromice.process.get_l3:get_l3',
         'join_l3 = pypromice.process.join_l3:join_l3',
         'get_watsontx = pypromice.tx.get_watsontx:get_watsontx',
```

### Comparing `pypromice-1.3.5/src/pypromice/get/get.py` & `pypromice-1.3.6/src/pypromice/get/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,34 +177,34 @@
         
 class TestGet(unittest.TestCase): 
     def testURL(self):
         '''Test URL retrieval'''
         l = lookup_table(['doi:10.22008/FK2/IW73UU'])
         self.assertTrue('10.22008/FK2' in list(l.values())[0])
     
-    def testAWSname(self):  
-        '''Test AWS names retrieval'''
-        n = aws_names()
-        self.assertIsInstance(n, list)
-        self.assertTrue('nuk_k_hour.csv' in n)
+#    def testAWSname(self):  
+#        '''Test AWS names retrieval'''
+#        n = aws_names()
+#        self.assertIsInstance(n, list)
+#        self.assertTrue('nuk_k_hour.csv' in n)
     
-    def testAWScsv(self):
-        '''Test AWS data retrieval'''
-        kan_b = aws_data('kan_b_hour.csv')
-        self.assertIsInstance(kan_b, pd.DataFrame)
+#    def testAWScsv(self):
+#        '''Test AWS data retrieval'''
+#        kan_b = aws_data('kan_b_hour.csv')
+#        self.assertIsInstance(kan_b, pd.DataFrame)
         
-    def testWatsonHour(self):
-        '''Test Wason River discharge hourly data retrieval'''
-        wh = watson_discharge()
-        self.assertTrue(wh['Q']['2021-10-27 23:00:00']==5.48)
+#    def testWatsonHour(self):
+#        '''Test Wason River discharge hourly data retrieval'''
+#        wh = watson_discharge()
+#        self.assertTrue(wh['Q']['2021-10-27 23:00:00']==5.48)
         
-    def testWatsonDaily(self):
-        '''Test Wason River discharge daily data retrieval'''
-        wd = watson_discharge(t='day')
-        self.assertTrue(wd['Q']['2009-09-04 00:00:00']==4.72)
+#    def testWatsonDaily(self):
+#        '''Test Wason River discharge daily data retrieval'''
+#        wd = watson_discharge(t='day')
+#        self.assertTrue(wd['Q']['2009-09-04 00:00:00']==4.72)
 
     def testGetCLI(self):
         '''Test get_promice_data'''
         exit_status = os.system('get_promice_data -h')
         self.assertEqual(exit_status, 0)
             
 if __name__ == "__main__":
```

### Comparing `pypromice-1.3.5/src/pypromice/get/get_promice_data.py` & `pypromice-1.3.6/src/pypromice/get/get_promice_data.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/postprocess/bufr_utilities.py` & `pypromice-1.3.6/src/pypromice/postprocess/bufr_utilities.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/postprocess/get_bufr.py` & `pypromice-1.3.6/src/pypromice/postprocess/get_bufr.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/postprocess/real_time_utilities.py` & `pypromice-1.3.6/src/pypromice/postprocess/real_time_utilities.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/postprocess/station_configurations.toml` & `pypromice-1.3.6/src/pypromice/postprocess/station_configurations.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/process/L0toL1.py` & `pypromice-1.3.6/src/pypromice/process/L0toL1.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/process/L1toL2.py` & `pypromice-1.3.6/src/pypromice/process/L1toL2.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,33 +62,42 @@
     try:
         ds = adjustTime(ds)                                                    # Adjust time after a user-defined csv files
         ds = flagNAN(ds)                                                       # Flag NaNs after a user-defined csv files
         ds = adjustData(ds)                                                    # Adjust data after a user-defined csv files
     except Exception:
         logger.exception('Flagging and fixing failed:')
 
-    if ds.attrs['format'] == 'TX':
-        ds = persistence_qc(ds)                                               # Flag and remove persistence outliers
-        # TODO: The configuration should be provided explicitly
-        outlier_detector = ThresholdBasedOutlierDetector.default()
-        ds = outlier_detector.filter_data(ds)                                 # Flag and remove percentile outliers
+    ds = persistence_qc(ds)                                               # Flag and remove persistence outliers
+    # if ds.attrs['format'] == 'TX':
+    #     # TODO: The configuration should be provided explicitly
+    #     outlier_detector = ThresholdBasedOutlierDetector.default()
+    #     ds = outlier_detector.filter_data(ds)                                 # Flag and remove percentile outliers
+
+    # filtering gps_lat, gps_lon and gps_alt based on the difference to a baseline elevation
+    # right now baseline elevation is gapfilled monthly median elevation
+    baseline_elevation = (ds.gps_alt.to_series().resample('M').median()
+                          .reindex(ds.time.to_series().index, method='nearest')
+                          .ffill().bfill())
+    mask = (np.abs(ds.gps_alt - baseline_elevation) < 100) & ds.gps_alt.notnull()
+    ds[['gps_alt','gps_lon', 'gps_lat']] = ds[['gps_alt','gps_lon', 'gps_lat']].where(mask)
+    
+    # removing dlr and ulr that are missing t_rad
+    # this is done now becasue t_rad can be filtered either manually or with persistence
+    ds['dlr'] = ds.dlr.where(ds.t_rad.notnull())
+    ds['ulr'] = ds.ulr.where(ds.t_rad.notnull())
 
     T_100 = _getTempK(T_0)
     ds['rh_u_cor'] = correctHumidity(ds['rh_u'], ds['t_u'],
                                      T_0, T_100, ews, ei0)
 
     # Determiune cloud cover for on-ice stations
-    if not ds.attrs['bedrock']:
-        cc = calcCloudCoverage(ds['t_u'], T_0, eps_overcast, eps_clear,        # Calculate cloud coverage
-                               ds['dlr'], ds.attrs['station_id'])
-        ds['cc'] = (('time'), cc.data)
-    else:
-        # Default cloud cover for bedrock station for which tilt should be 0 anyway.
-        cc = 0.8
-
+    cc = calcCloudCoverage(ds['t_u'], T_0, eps_overcast, eps_clear,        # Calculate cloud coverage
+                           ds['dlr'], ds.attrs['station_id'])
+    ds['cc'] = (('time'), cc.data)
+    
     # Determine surface temperature
     ds['t_surf'] = calcSurfaceTemperature(T_0, ds['ulr'], ds['dlr'],           # Calculate surface temperature
                                           emissivity)
     if not ds.attrs['bedrock']:
         ds['t_surf'] = xr.where(ds['t_surf'] > 0, 0, ds['t_surf'])
 
     # Determine station position relative to sun
@@ -98,31 +107,38 @@
 
     if hasattr(ds, 'latitude') and hasattr(ds, 'longitude'):
         lat = ds.attrs['latitude']                                             # TODO Why is mean GPS lat lon not preferred for calcs?
         lon = ds.attrs['longitude']
     else:
         lat = ds['gps_lat'].mean()
         lon = ds['gps_lon'].mean()
+    
+    # smoothing tilt and rot
+    ds['tilt_x'] = smoothTilt(ds['tilt_x'])
+    ds['tilt_y'] = smoothTilt(ds['tilt_y'])
+    ds['rot'] = smoothRot(ds['rot'])
 
     deg2rad, rad2deg = _getRotation()                                          # Get degree-radian conversions
     phi_sensor_rad, theta_sensor_rad = calcTilt(ds['tilt_x'], ds['tilt_y'],    # Calculate station tilt
                                                 deg2rad)
 
     Declination_rad = calcDeclination(doy, hour, minute)                       # Calculate declination
     HourAngle_rad = calcHourAngle(hour, minute, lon)                           # Calculate hour angle
     ZenithAngle_rad, ZenithAngle_deg = calcZenith(lat, Declination_rad,        # Calculate zenith
                                                   HourAngle_rad, deg2rad,
                                                   rad2deg)
-
+    
+    
     # Correct Downwelling shortwave radiation
     DifFrac = 0.2 + 0.8 * cc
     CorFac_all = calcCorrectionFactor(Declination_rad, phi_sensor_rad,         # Calculate correction
                                       theta_sensor_rad, HourAngle_rad,
                                       ZenithAngle_rad, ZenithAngle_deg,
                                       lat, DifFrac, deg2rad)
+    CorFac_all = xr.where(ds['cc'].notnull(), CorFac_all, 1)
     ds['dsr_cor'] = ds['dsr'].copy(deep=True) * CorFac_all                     # Apply correction
 
     AngleDif_deg = calcAngleDiff(ZenithAngle_rad, HourAngle_rad,               # Calculate angle between sun and sensor
                                  phi_sensor_rad, theta_sensor_rad)
 
     ds['albedo'], OKalbedos = calcAlbedo(ds['usr'], ds['dsr_cor'],             # Determine albedo
                               AngleDif_deg, ZenithAngle_deg)
@@ -141,17 +157,17 @@
     ds['albedo'] = ds['albedo'].where(OKalbedos)                               #TODO remove?
 
     # Remove data where TOA shortwave radiation invalid
     isr_toa = calcTOA(ZenithAngle_deg, ZenithAngle_rad)                        # Calculate TOA shortwave radiation
     TOA_crit_nopass = (ds['dsr_cor'] > (0.9 * isr_toa + 10))                   # Determine filter
     ds['dsr_cor'][TOA_crit_nopass] = np.nan                                    # Apply filter and interpolate
     ds['usr_cor'][TOA_crit_nopass] = np.nan
-    ds['dsr_cor'] = ds['dsr_cor'].interpolate_na(dim='time', use_coordinate=False)
-    ds['usr_cor'] = ds['usr_cor'].interpolate_na(dim='time', use_coordinate=False)
-
+    
+    ds['dsr_cor'] = ds.dsr_cor.where(ds.dsr.notnull())  
+    ds['usr_cor'] = ds.usr_cor.where(ds.usr.notnull())  
     # # Check sun position
     # sundown = ZenithAngle_deg >= 90
     # _checkSunPos(ds, OKalbedos, sundown, sunonlowerdome, TOA_crit_nopass)
 
     if hasattr(ds, 'correct_precip'):                                          # Correct precipitation
         precip_flag=ds.attrs['correct_precip']
     else:
@@ -237,14 +253,73 @@
     xarray.DataArray
         Calculated surface temperature
     '''
     t_surf = ((ulr - (1 - emissivity) * dlr) / emissivity / 5.67e-8)**0.25 - T_0
     return t_surf
 
 
+def smoothTilt(da: xr.DataArray, threshold=0.2):
+    '''Smooth the station tilt
+
+    Parameters
+    ----------
+    da : xarray.DataArray
+        either X or Y tilt inclinometer measurements
+    threshold : float
+        threshold used in a standrad.-deviation based filter
+
+    Returns
+    -------
+    xarray.DataArray
+        either X or Y smoothed tilt inclinometer measurements
+    '''
+    # we calculate the moving standard deviation over a 3-day sliding window
+    # hourly resampling is necessary to make sure the same threshold can be used 
+    # for 10 min and hourly data
+    moving_std_gap_filled = da.to_series().resample('H').median().rolling(
+                    3*24, center=True, min_periods=2
+                    ).std().reindex(da.time, method='bfill').values
+    # we select the good timestamps and gapfill assuming that
+    # - when tilt goes missing the last available value is used
+    # - when tilt is not available for the very first time steps, the first
+    #   good value is used for backfill
+    return da.where(
+                moving_std_gap_filled < threshold
+                ).ffill(dim='time').bfill(dim='time')
+
+
+def smoothRot(da: xr.DataArray, threshold=4):
+    '''Smooth the station rotation
+
+    Parameters
+    ----------
+    da : xarray.DataArray
+        rotation measurements from inclinometer
+    threshold : float
+        threshold used in a standrad-deviation based filter
+
+    Returns
+    -------
+    xarray.DataArray
+        smoothed rotation measurements from inclinometer
+    '''
+    moving_std_gap_filled = da.to_series().resample('H').median().rolling(
+                    3*24, center=True, min_periods=2
+                    ).std().reindex(da.time, method='bfill').values
+    # same as for tilt with, in addition:
+    #     - a resampling to daily values
+    #     - a two week median smoothing
+    #     - a resampling from these daily values to the original temporal resolution
+    return ('time', (da.where(moving_std_gap_filled <4).ffill(dim='time')
+            .to_series().resample('D').median()
+            .rolling(7*2,center=True,min_periods=2).median()
+            .reindex(da.time, method='bfill').values
+            ))
+
+
 def calcTilt(tilt_x, tilt_y, deg2rad):
     '''Calculate station tilt
 
     Parameters
     ----------
     tilt_x : xarray.DataArray
         X tilt inclinometer measurements
@@ -319,15 +394,14 @@
                    + np.log10(ei0))
 
     # Define freezing point. Why > -100?
     freezing = (T < 0) & (T > -100).values
 
     # Set to Groff & Gratch values when freezing, otherwise just rh
     rh_cor = rh.where(~freezing, other = rh*(e_s_wtr / e_s_ice))
-    rh_cor = rh_cor.where(T.notnull())
     return rh_cor
 
 
 def correctPrecip(precip, wspd):
     '''Correct precipitation with the undercatch correction method used in
     Yang et al. (1999) and Box et al. (2022), based on Goodison et al. (1998)
```

### Comparing `pypromice-1.3.5/src/pypromice/process/L2toL3.py` & `pypromice-1.3.6/src/pypromice/process/L2toL3.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         Aerodynamic surface roughness length for momention, assumed constant 
         for all ice/snow surfaces. Default is 0.001.
     g : int 
         Gravitational acceleration (m/s2). Default is 9.82.        
     es_0 : int 
         Saturation vapour pressure at the melting point (hPa). Default is 6.1071.        
     eps : int 
-        Default is 0.622.
+        Ratio of molar masses of vapor and dry air (0.622).
     gamma : int
         Flux profile correction (Paulson & Dyer). Default is 16..
     L_sub : int  
         Latent heat of sublimation (J/kg). Default is 2.83e6.
     L_dif_max : int 
         Default is 0.01.     
     c_pd : int
@@ -309,15 +309,15 @@
     T_0 : float 
         Steam point temperature. Default is 273.15.
     T_100 : float
         Steam point temperature in Kelvin
     T_h : xarray.DataArray
         Air temperature
     eps : int 
-        DESCRIPTION
+        ratio of molar masses of vapor and dry air (0.622)
     es_0 : float
         Saturation vapour pressure at the melting point (hPa)
     es_100 : float
         Saturation vapour pressure at steam point temperature (hPa)
     p_h : xarray.DataArray
         Air pressure
     RH_cor_h : xarray.DataArray
```

### Comparing `pypromice-1.3.5/src/pypromice/process/aws.py` & `pypromice-1.3.6/src/pypromice/process/aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         for k in self.config.keys():
             target = self.config[k]
             try:
                 ds_list.append(self.readL0file(target))
 
             except pd.errors.ParserError as e:
                 # ParserError: Too many columns specified: expected 40 and found 38
-                logger.info(f'-----> No msg_lat or msg_lon for {k}')
+                # logger.info(f'-----> No msg_lat or msg_lon for {k}')
                 for item in ['msg_lat', 'msg_lon']:
                     target['columns'].remove(item)                           # Also removes from self.config
                 ds_list.append(self.readL0file(target))
             logger.info(f'L0 data successfully loaded from {k}')
         return ds_list
 
     def readL0file(self, conf):
@@ -719,39 +719,96 @@
     ~2-3 minutes per operation: ds_d = ds_h.resample({'time':"1D"}).mean()
     This has now been fixed, so needs implementing:
     https://github.com/pydata/xarray/issues/4498#event-6610799698
 
     Parameters
     ----------
     ds_h : xarray.Dataset
-        L3 AWS daily dataset
+        L3 AWS dataset either at 10 min (for raw data) or hourly (for tx data)
     t : str
         Resample factor, same variable definition as in
         pandas.DataFrame.resample()
 
     Returns
     -------
     ds_d : xarray.Dataset
-        L3 AWS hourly dataset
+        L3 AWS dataset resampled to the frequency defined by t
     '''
     df_d = ds_h.to_dataframe().resample(t).mean()
+    
     # recalculating wind direction from averaged directional wind speeds
     for var in ['wdir_u','wdir_l','wdir_i']:
         if var in df_d.columns:
             if ('wspd_x_'+var.split('_')[1] in df_d.columns) & ('wspd_x_'+var.split('_')[1] in df_d.columns):
                 df_d[var] = _calcWindDir(df_d['wspd_x_'+var.split('_')[1]],
                                    df_d['wspd_y_'+var.split('_')[1]])
             else:
                 logger.info(var,'in dataframe but not','wspd_x_'+var.split('_')[1],'wspd_x_'+var.split('_')[1])
+    
+    # recalculating relative humidity from average vapour pressure and average
+    # saturation vapor pressure
+    for var in ['rh_u','rh_l']:
+        lvl = var.split('_')[1]
+        if var in df_d.columns:
+            if ('t_'+lvl in ds_h.keys()):
+                es_wtr, es_cor = calculateSaturationVaporPressure(ds_h['t_'+lvl])
+                p_vap = ds_h[var] / 100 * es_wtr
+                
+                df_d[var] = (p_vap.to_series().resample(t).mean() \
+                           / es_wtr.to_series().resample(t).mean())*100
+                df_d[var+'_cor'] = (p_vap.to_series().resample(t).mean() \
+                           / es_cor.to_series().resample(t).mean())*100
+            
     vals = [xr.DataArray(data=df_d[c], dims=['time'],
            coords={'time':df_d.index}, attrs=ds_h[c].attrs) for c in df_d.columns]
     ds_d = xr.Dataset(dict(zip(df_d.columns,vals)), attrs=ds_h.attrs)
     return ds_d
 
 
+def calculateSaturationVaporPressure(t, T_0=273.15, T_100=373.15, es_0=6.1071,
+                                     es_100=1013.246, eps=0.622):            
+    '''Calculate specific humidity
+    
+    Parameters
+    ----------
+    T_0 : float 
+        Steam point temperature. Default is 273.15.
+    T_100 : float
+        Steam point temperature in Kelvin
+    t : xarray.DataArray
+        Air temperature
+    es_0 : float
+        Saturation vapour pressure at the melting point (hPa)
+    es_100 : float
+        Saturation vapour pressure at steam point temperature (hPa)
+    
+    Returns
+    -------
+    xarray.DataArray
+        Saturation vapour pressure with regard to water above 0 C (hPa)
+    xarray.DataArray
+        Saturation vapour pressure where subfreezing timestamps are with regards to ice (hPa)
+    '''                                                         
+    # Saturation vapour pressure above 0 C (hPa)
+    es_wtr = 10**(-7.90298 * (T_100 / (t + T_0) - 1) + 5.02808 * np.log10(T_100 / (t + T_0))
+                  - 1.3816E-7 * (10**(11.344 * (1 - (t + T_0) / T_100)) - 1)
+                  + 8.1328E-3 * (10**(-3.49149 * (T_100 / (t + T_0) -1)) - 1) + np.log10(es_100))
+
+    # Saturation vapour pressure below 0 C (hPa)
+    es_ice = 10**(-9.09718 * (T_0 / (t + T_0) - 1) - 3.56654
+                  * np.log10(T_0 / (t + T_0)) + 0.876793
+                  * (1 - (t + T_0) / T_0)
+                  + np.log10(es_0)) 
+    
+    # Saturation vapour pressure (hPa)
+    es_cor = xr.where(t < 0, es_ice, es_wtr)
+    
+    return es_wtr, es_cor
+
+
 def _calcWindDir(wspd_x, wspd_y):
     '''Calculate wind direction in degrees
 
     Parameters
     ----------
     wspd_x : xarray.DataArray
         Wind speed in X direction
```

### Comparing `pypromice-1.3.5/src/pypromice/process/get_l3.py` & `pypromice-1.3.6/src/pypromice/process/get_l3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/process/join_l3.py` & `pypromice-1.3.6/src/pypromice/process/join_l3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/process/metadata.csv` & `pypromice-1.3.6/src/pypromice/process/metadata.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/process/value_clipping.py` & `pypromice-1.3.6/src/pypromice/process/value_clipping.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/process/variables.csv` & `pypromice-1.3.6/src/pypromice/process/variables.csv`

 * *Files 0% similar despite different names*

```diff
@@ -85,8 +85,8 @@
 t_i,air_temperature,Air temperature (instantaneous),degrees_C,-80,40,,all,all,4,physicalMeasurement,time lat lon alt,True,"PT100 temperature at boom, for meteorological observations"
 rh_i,relative_humidity,Relative humidity (instantaneous),%,0,150,rh_i_cor,all,all,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
 rh_i_cor,relative_humidity_corrected,Relative humidity (instantaneous) – corrected,%,0,100,,all,all,4,modelResult,time lat lon alt,True,For meteorological observations
 wspd_i,wind_speed,Wind speed (instantaneous),m s-1,0,100,wdir_i wspd_x_i wspd_y_i,all,all,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
 wdir_i,wind_from_direction,Wind from direction (instantaneous),degrees,1,360,wspd_x_i wspd_y_i,all,all,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
 wspd_x_i,wind_speed_from_x_direction,Wind speed from x direction (instantaneous),m s-1,-100,100,wdir_i wspd_i,all,all,4,modelResult,time lat lon alt,True,For meteorological observations
 wspd_y_i,wind_speed_from_y_direction,Wind speed from y direction (instantaneous),m s-1,-100,100,wdir_i wspd_i,all,all,4,modelResult,time lat lon alt,True,For meteorological observations
-msg_i,message,Message string (instantaneous),-,,,,all,all,,qualityInformation,time lat lon alt,True,For meteorological observations
+msg_i,message,Message string (instantaneous),-,,,,all,,,qualityInformation,time lat lon alt,True,L0 only
```

### Comparing `pypromice-1.3.5/src/pypromice/qc/github_data_issues.py` & `pypromice-1.3.6/src/pypromice/qc/github_data_issues.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/qc/percentiles/compute_thresholds.py` & `pypromice-1.3.6/src/pypromice/qc/percentiles/compute_thresholds.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/qc/percentiles/outlier_detector.py` & `pypromice-1.3.6/src/pypromice/qc/percentiles/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/qc/percentiles/thresholds.csv` & `pypromice-1.3.6/src/pypromice/qc/percentiles/thresholds.csv`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,16 @@
 NAU,t_[uli],-49.70,1.50,spring
 NAU,t_[uli],-34.79,7.90,summer
 NAU,t_[uli],-55.70,9.50,fall
 JAR,p_[ul],881.00,929.00,
 JAR,p_i,-119.00,-71.00,
 JAR,wspd_[uli],-11.62,29.82,
 JAR,t_[uli],-14.60,13.30,summer
-FRE,p_[ul],638.31,799.82,
-FRE,p_i,-361.69,-200.18,
+FRE,p_[ul],800,1000,
+FRE,p_i,-200,0,
 FRE,wspd_[uli],-12.00,22.62,
 FRE,t_[uli],-38.20,10.02,winter
 FRE,t_[uli],-36.55,18.07,spring
 FRE,t_[uli],-12.61,22.82,summer
 FRE,t_[uli],-33.93,17.69,fall
 CP1,p_[ul],747.90,826.00,
 CP1,p_i,-252.10,-174.00,
```

### Comparing `pypromice-1.3.5/src/pypromice/qc/persistence.py` & `pypromice-1.3.6/src/pypromice/qc/persistence.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,23 @@
     "find_persistent_regions",
     "count_consecutive_persistent_values",
     "count_consecutive_true",
 ]
 
 logger = logging.getLogger(__name__)
 
+# period is given in hours, 2 persistent 10 min values will be flagged if period < 0.333
 DEFAULT_VARIABLE_THRESHOLDS = {
     "t": {"max_diff": 0.0001, "period": 2},
     "p": {"max_diff": 0.0001, "period": 2},
-    # Relative humidity can be very stable around 100%.
-    #"rh": {"max_diff": 0.0001, "period": 2},
+    'gps_lat_lon':{"max_diff": 0.000001, "period": 6}, # gets special handling to remove simultaneously constant gps_lat and gps_lon
+    'gps_alt':{"max_diff": 0.0001, "period": 6},
+    't_rad':{"max_diff": 0.0001, "period": 2},
+    "rh": {"max_diff": 0.0001, "period": 2}, # gets special handling to allow constant 100%
+    "wspd": {"max_diff": 0.0001, "period": 6},
 }
 
 
 def persistence_qc(
     ds: xr.Dataset,
     variable_thresholds: Optional[Mapping] = None,
 ) -> xr.Dataset:
@@ -54,35 +58,54 @@
     # Plots will be shown before and after flag removal for each var
 
     df = ds.to_dataframe()  # Switch to pandas
 
     if variable_thresholds is None:
         variable_thresholds = DEFAULT_VARIABLE_THRESHOLDS
 
-    logger.debug(f"Running persistence_qc using {variable_thresholds}")
+    logger.info(f"Running persistence_qc using {variable_thresholds}")
 
     for k in variable_thresholds.keys():
-        var_all = [
-            k + "_u",
-            k + "_l",
-            k + "_i",
-        ]  # apply to upper, lower boom, and instant
+        if k in ['t','p','rh','wspd','wdir', 'z_boom']:
+            var_all = [
+                k + "_u",
+                k + "_l",
+                k + "_i",
+            ]  # apply to upper, lower boom, and instant
+        else:
+            var_all = [k]
         max_diff = variable_thresholds[k]["max_diff"]  # loading persistent limit
         period = variable_thresholds[k]["period"]  # loading diff period
 
         for v in var_all:
             if v in df:
                 mask = find_persistent_regions(df[v], period, max_diff)
+                if 'rh' in v:
+                    mask = mask & (df[v]<99)
                 n_masked = mask.sum()
                 n_samples = len(mask)
-                logger.debug(
+                logger.info(
                     f"Applying persistent QC in {v}. Filtering {n_masked}/{n_samples} samples"
                 )
                 # setting outliers to NaN
                 df.loc[mask, v] = np.nan
+            elif v == 'gps_lat_lon':
+                mask = (
+                    find_persistent_regions(df['gps_lon'], period, max_diff)
+                    & find_persistent_regions(df['gps_lat'], period, max_diff) 
+                )
+
+                n_masked = mask.sum()
+                n_samples = len(mask)
+                logger.info(
+                    f"Applying persistent QC in {v}. Filtering {n_masked}/{n_samples} samples"
+                )
+                # setting outliers to NaN
+                df.loc[mask, 'gps_lon'] = np.nan
+                df.loc[mask, 'gps_lat'] = np.nan
 
     # Back to xarray, and re-assign the original attrs
     ds_out = df.to_xarray()
     ds_out = ds_out.assign_attrs(ds.attrs)  # Dataset attrs
     for x in ds_out.data_vars:  # variable-specific attrs
         ds_out[x].attrs = ds[x].attrs
 
@@ -106,37 +129,38 @@
 
 def count_consecutive_persistent_values(
     data: pd.Series,
     max_diff: float,
 ) -> pd.Series:
     diff = data.ffill().diff().abs()  # forward filling all NaNs!
     mask: pd.Series = diff < max_diff
-    return count_consecutive_true(mask)
+    return duration_consecutive_true(mask)
 
 
-def count_consecutive_true(
-    series: Union[pd.Series, pd.DataFrame]
-) -> Union[pd.Series, pd.DataFrame]:
+def duration_consecutive_true(
+    series: pd.Series,
+) -> pd.Series:
     """
-    Convert boolean series to integer series where the values represent the number of connective true values.
+    From a boolean series, calculates the duration, in hours, of the periods with connective true values.
 
     Examples
     --------
-    >>> count_consecutive_true(pd.Series([False, True, False, False, True, True, True, False, True]))
+    >>> duration_consecutive_true(pd.Series([False, True, False, False, True, True, True, False, True]))
     pd.Series([0, 1, 0, 0, 1, 2, 3, 0, 1])
 
     Parameters
     ----------
-    series
+    pd.Series
         Boolean pandas Series or DataFrame
 
     Returns
     -------
-    consecutive_true_count
+    pd.Series
         Integer pandas Series or DataFrame with values representing the number of connective true values.
 
     """
     # assert series.dtype == bool
-    cumsum = series.cumsum()
+    cumsum = ((series.index - series.index[0]).total_seconds()/3600).to_series(index=series.index)
     is_first = series.astype("int").diff() == 1
     offset = (is_first * cumsum).replace(0, np.nan).fillna(method="ffill").fillna(0)
-    return ((cumsum - offset + 1) * series).astype("int")
+
+    return (cumsum - offset) * series
```

### Comparing `pypromice-1.3.5/src/pypromice/qc/persistence_test.py` & `pypromice-1.3.6/src/pypromice/qc/persistence_test.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_config1.toml` & `pypromice-1.3.6/src/pypromice/test/test_config1.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_config2.toml` & `pypromice-1.3.6/src/pypromice/test/test_config2.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_email` & `pypromice-1.3.6/src/pypromice/test/test_email`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_percentile.py` & `pypromice-1.3.6/src/pypromice/test/test_percentile.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_raw1.txt` & `pypromice-1.3.6/src/pypromice/test/test_raw1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_raw_DataTable2.txt` & `pypromice-1.3.6/src/pypromice/test/test_raw_DataTable2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_raw_SlimTableMem1.txt` & `pypromice-1.3.6/src/pypromice/test/test_raw_SlimTableMem1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_raw_transmitted1.txt` & `pypromice-1.3.6/src/pypromice/test/test_raw_transmitted1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/test/test_raw_transmitted2.txt` & `pypromice-1.3.6/src/pypromice/test/test_raw_transmitted2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/tx/get_l0tx.py` & `pypromice-1.3.6/src/pypromice/tx/get_l0tx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/tx/get_msg.py` & `pypromice-1.3.6/src/pypromice/tx/get_msg.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/tx/get_watsontx.py` & `pypromice-1.3.6/src/pypromice/tx/get_watsontx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/tx/payload_formats.csv` & `pypromice-1.3.6/src/pypromice/tx/payload_formats.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice/tx/tx.py` & `pypromice-1.3.6/src/pypromice/tx/tx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.5/src/pypromice.egg-info/PKG-INFO` & `pypromice-1.3.6/src/pypromice.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.3.5
+Version: 1.3.6
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
@@ -19,19 +19,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: xarray>=2022.6.0
 Requires-Dist: toml
 Requires-Dist: scipy>=1.9.0
-Requires-Dist: scikit-learn>=1.1.0
 Requires-Dist: Bottleneck
 Requires-Dist: netcdf4
 Requires-Dist: pyDataverse
 Requires-Dist: eccodes
+Requires-Dist: scikit-learn>=1.1.0
 
 # pypromice
 [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://badge.fury.io/py/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/version.svg)](https://anaconda.org/conda-forge/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/platforms.svg)](https://anaconda.org/conda-forge/pypromice) [![](<https://img.shields.io/badge/Dataverse DOI-10.22008/FK2/3TSBF0-orange>)](https://www.doi.org/10.22008/FK2/3TSBF0) [![DOI](https://joss.theoj.org/papers/10.21105/joss.05298/status.svg)](https://doi.org/10.21105/joss.05298) [![Documentation Status](https://readthedocs.org/projects/pypromice/badge/?version=latest)](https://pypromice.readthedocs.io/en/latest/?badge=latest)
  
 pypromice is designed for processing and handling [PROMICE](https://promice.org) automated weather station (AWS) data.
 
 It is envisioned for pypromice to be the go-to toolbox for handling and processing [PROMICE](https://promice.dk) and [GC-Net](http://cires1.colorado.edu/steffen/gcnet/) datasets. New releases of pypromice are uploaded alongside PROMICE AWS data releases to our [Dataverse](https://dataverse.geus.dk/dataverse/PROMICE) for transparency purposes and to encourage collaboration on improving our data. Please visit the pypromice [readthedocs](https://pypromice.readthedocs.io/en/latest/?badge=latest) for more information. 
@@ -54,15 +54,22 @@
 $ conda install pypromice -c conda-forge
 ```
 
 ```
 $ pip install pypromice
 ```
 
-For the most up-to-date version, pypromice can be installed directly from the repo: 
+The [eccodes](https://confluence.ecmwf.int/display/ECC/ecCodes+installation) package for pypromice's post-processing functionality needs to be installed specifically in the pip distribution:
+
+```
+$ conda install eccodes -c conda-forge
+$ pip install pypromice
+```
+
+And for the most up-to-date version of pypromice, the package can be cloned and installed directly from the repo: 
 
 ```
 $ pip install --upgrade git+http://github.com/GEUS-Glaciology-and-Climate/pypromice.git
 ```
 
 ### Developer install
 	
@@ -72,23 +79,7 @@
 $ conda create --name pypromice python=3.8
 $ conda activate pypromice
 $ git clone git@github.com:GEUS-Glaciology-and-Climate/pypromice.git
 $ cd pypromice/
 $ pip install .
 ```
 
-### Additional dependencies
-
-Additional packages are required if you wish to use pypromice's post-processing functionality. 
-
-[eccodes](https://confluence.ecmwf.int/display/ECC/ecCodes+installation) is the official package for BUFR encoding and decoding. Try firstly to install with conda-forge like so:
-
-```
-$ conda install -c conda-forge eccodes
-```
-
-If the environment cannot resolve the eccodes installation then follow the steps documented [here](https://gist.github.com/MHBalsmeier/a01ad4e07ecf467c90fad2ac7719844a) to download eccodes and then install eccodes' python bindings using pip.
-
-```
-$ pip3 install eccodes-python
-```
-
```

### Comparing `pypromice-1.3.5/src/pypromice.egg-info/SOURCES.txt` & `pypromice-1.3.6/src/pypromice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

