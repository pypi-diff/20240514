# Comparing `tmp/fusion_engine_client-1.23.0.tar.gz` & `tmp/fusion_engine_client-1.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion_engine_client-1.23.0.tar", last modified: Fri May  3 21:02:55 2024, max compression
+gzip compressed data, was "fusion_engine_client-1.23.1.tar", last modified: Tue May 14 18:18:41 2024, max compression
```

## Comparing `fusion_engine_client-1.23.0.tar` & `fusion_engine_client-1.23.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.501875 fusion_engine_client-1.23.0/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.505875 fusion_engine_client-1.23.0/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   128047 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (127)    47884 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.505875 fusion_engine_client-1.23.0/fusion_engine_client/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/import_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      313 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_display.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6809 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_lband_extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16262 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.509875 fusion_engine_client-1.23.0/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62152 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    27163 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    29659 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/gnss_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    50308 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)    15264 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35603 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.509875 fusion_engine_client-1.23.0/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/fast_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24420 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.509875 fusion_engine_client-1.23.0/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24918 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 21:02:55.000000 fusion_engine_client-1.23.0/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:02:55.513875 fusion_engine_client-1.23.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-03 21:02:14.000000 fusion_engine_client-1.23.0/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.944756 fusion_engine_client-1.23.1/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.948756 fusion_engine_client-1.23.1/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   128072 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47575 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.948756 fusion_engine_client-1.23.1/fusion_engine_client/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/import_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      313 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_display.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6809 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_lband_extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16262 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.952756 fusion_engine_client-1.23.1/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62220 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29955 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50595 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35741 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.952756 fusion_engine_client-1.23.1/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/fast_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24420 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.952756 fusion_engine_client-1.23.1/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24918 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_time_range.py
```

### Comparing `fusion_engine_client-1.23.0/PKG-INFO` & `fusion_engine_client-1.23.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.23.0
+Version: 1.23.1
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
-Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.0.tar.gz
+Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.1.tar.gz
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -23,25 +23,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: construct>=2.10.0
 Requires-Dist: numpy>=1.16.0
-Requires-Dist: pymap3d>=2.4.3
-Requires-Dist: aenum>=3.1.1
 Requires-Dist: p1-gpstime>=0.6.3.dev1
+Requires-Dist: argparse-formatter>=1.4
 Requires-Dist: packaging>=21.0.0
+Requires-Dist: pymap3d>=2.4.3
+Requires-Dist: plotly>=4.0.0
+Requires-Dist: scipy>=1.5.0
 Requires-Dist: palettable>=3.3.0
 Requires-Dist: colorama>=0.4.4
-Requires-Dist: scipy>=1.5.0
-Requires-Dist: construct>=2.10.0
-Requires-Dist: plotly>=4.0.0
-Requires-Dist: argparse-formatter>=1.4
+Requires-Dist: aenum>=3.1.1
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion_engine_client-1.23.0/README.md` & `fusion_engine_client-1.23.1/README.md`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/analysis/analyzer.py` & `fusion_engine_client-1.23.1/fusion_engine_client/analysis/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1804,15 +1804,15 @@
         fig.update_yaxes(
             ticktext=['%s (%d)' % (e.name, e.value) for e in SolutionType],
             tickvals=[e.value for e in SolutionType],
             title_text='Solution Type',
             row=3, col=1
         )
 
-        fig.update_layout(title='Heading Plots', legend_traceorder='normal')
+        fig.update_layout(title='Heading Plots', legend_traceorder='normal', modebar_add=['v1hovermode'])
 
 
         # Display the navigation engine's heading estimate, if available, for comparison with the heading sensor
         # measurement.
         if primary_pose_data is not None:
             invalid_idx = primary_pose_data.solution_type[primary_pose_data.solution_type != SolutionType.Invalid]
             yaw_deg = primary_pose_data.ypr_deg[0][invalid_idx]
@@ -2001,15 +2001,15 @@
                 go.Scatter(
                     x=heading_time,
                     y=heading_data.solution_type,
                     customdata=heading_data.p1_time,
                     marker={'color': 'green'},
                     hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
                                   '<br><b>Solution</b>: %{text}',
-                    text=[str(SolutionType(s)) for s in raw_heading_data.solution_type],
+                    text=[str(SolutionType(s)) for s in heading_data.solution_type],
                     name='Corrected Heading Solution Type'
                 ),
                 row=3, col=1
             )
 
         self._add_figure(name='heading_measurement', figure=fig, title='Measurements: Heading')
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/analysis/attitude.py` & `fusion_engine_client-1.23.1/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/analysis/data_loader.py` & `fusion_engine_client-1.23.1/fusion_engine_client/analysis/data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,23 +195,23 @@
             # If there are no messages in the index that have system time, disable the search below. Otherwise, continue
             # below to search for system t0.
             if not np.any(np.isin(self.reader.get_index().type, list(messages_with_system_time))):
                 self.logger.warning('Unable to set system t0 - no system timestamps found in index file.')
                 self._need_system_t0 = False
         else:
             self.read(require_p1_time=True, max_messages=1, max_bytes=1 * 1024 * 1024,
-                      disable_index_generation=True, ignore_cache=True, show_progress=False)
+                      ignore_cache=True, show_progress=False)
 
         # Similarly, we also set the system t0 based on the first system-stamped (typically POSIX) message to appear in
         # the log, if any (profiling data, etc.). Unlike P1 time, since the index file does not contain system
         # timestamps, we have to do a read() even if an index exists. read() will use the index to at least speed up the
         # read operation.
         if self._need_system_t0:
             self.read(require_system_time=True, max_messages=1, max_bytes=1 * 1024 * 1024,
-                      disable_index_generation=True, ignore_cache=True, show_progress=False)
+                      ignore_cache=True, show_progress=False)
 
     def close(self):
         """!
         @brief Close the file.
         """
         if self.reader is not None:
             self.reader = None
@@ -230,16 +230,14 @@
 
         @param message_types A list of one or more @ref fusion_engine_client.messages.defs.MessageType "MessageTypes" to
                be returned. If `None` or an empty list, read all available messages.
         @param time_range An optional @ref TimeRange object specifying desired start and end time bounds of the data to
                be read. See @ref TimeRange for more details.
 
         @param show_progress If `True`, print the read progress every 10 MB (useful for large files).
-        @param disable_index_generation If `True`, override the `save_index` argument provided to `open()` and do
-               not generate an index file during this call (intended for internal use only).
         @param ignore_cache If `True`, ignore any cached data from a previous @ref read() call, and reload the requested
                data from disk.
 
         @param max_messages If set, read up to the specified maximum number of messages. Applies across all message
                types. If negative, read the last N messages.
         @param max_bytes If set, read up to the specified maximum number of bytes.
         @param require_p1_time If `True`, omit messages that do not contain valid P1 timestamps.
@@ -273,15 +271,15 @@
         """
         return self._read(*args, **kwargs)
 
     def _read(self,
               message_types: Union[Iterable[MessageType], MessageType] = None,
               time_range: TimeRange = None,
               show_progress: bool = False,
-              ignore_cache: bool = False, disable_index_generation: bool = False,
+              ignore_cache: bool = False,
               max_messages: int = None, max_bytes: int = None,
               require_p1_time: bool = False, require_system_time: bool = False,
               return_in_order: bool = False, return_bytes: bool = False, return_message_index: bool = False,
               return_numpy: bool = False, keep_messages: bool = False, remove_nan_times: bool = True,
               time_align: TimeAlignmentMode = TimeAlignmentMode.NONE,
               aligned_message_types: Union[list, tuple, set] = None,
               quiet: bool = False) \
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/applications/import_utils.py` & `fusion_engine_client-1.23.1/fusion_engine_client/applications/import_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_extract.py` & `fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_extract.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_lband_extract.py` & `fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_lband_extract.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/applications/p1_print.py` & `fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_print.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/configuration.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1597,14 +1597,17 @@
         return len(self.pack())
 
 
 class DataVersion(NamedTuple):
     major: int
     minor: int
 
+    def __str__(self):
+        return f'{self.major}.{self.minor}'
+
 
 _DataVersionConstructRaw = Struct(
     Padding(1),
     "major" / Int8ul,
     "minor" / Int16ul,
 )
 _DataVersionConstruct = NamedTupleAdapter(DataVersion, _DataVersionConstructRaw)
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/control.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     def __init__(self):
         self.source_sequence_num = 0
         self.response = Response.OK
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         self._STRUCT.pack_into(buffer, offset, self.source_sequence_num, self.response)
         offset = self._STRUCT.size
 
         if return_buffer:
@@ -80,14 +81,15 @@
 
     def __init__(self, message_type: MessageType = MessageType.INVALID):
         self.message_type: MessageType = message_type
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         self._STRUCT.pack_into(buffer, offset, self.message_type.value)
         offset += self._STRUCT.size
 
         if return_buffer:
@@ -318,14 +320,15 @@
 
     def __init__(self, reset_mask: int = 0):
         self.reset_mask = reset_mask
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         self._STRUCT.pack_into(buffer, offset, self.reset_mask)
 
         if return_buffer:
             return buffer
         else:
             return self.calcsize()
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/defs.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import re
 import struct
 import sys
-from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Tuple, Type, Union
 from zlib import crc32
 
 import numpy as np
 
 from .measurement_details import *
 from .signal_defs import *
 from .timestamp import *
@@ -310,26 +310,28 @@
 
         if return_buffer:
             return buffer
         else:
             return self.calcsize()
 
     def unpack(self, buffer: bytes, offset: int = 0, validate_sync: bool = False, validate_crc: bool = False,
-               warn_on_unrecognized: bool = True) -> int:
+               warn_on_unrecognized: bool = True, return_sync_bytes: bool = False) -> \
+            Union[int, Tuple[int, bytes]]:
         """!
         @brief Deserialize a message header and validate its sync bytes and CRC.
 
         @note
         If CRC validation is enabled, the complete message payload is assumed to follow the header in `buffer`.
 
         @param buffer A byte buffer containing a serialized message.
         @param offset The offset into the buffer (in bytes) at which the message header begins.
         @param validate_sync If `True`, validate the sync bytes contained in the data buffer.
         @param validate_crc If `True`, validate the deserialized CRC against the data in the buffer.
         @param warn_on_unrecognized If `True`, print a warning if the message type is not listed in @ref MessageType.
+        @param return_sync_bytes If `True`, return the decoded sync bytes in addition to the header size.
 
         @return The size of the serialized header (in bytes).
         """
         (sync0, sync1, self.reserved,
          self.crc, self.protocol_version,
          self.message_version, message_type_int,
          self.sequence_number, self.payload_size_bytes, self.source_identifier) = \
@@ -346,15 +348,18 @@
             self.message_type = MessageType(message_type_int)
         except (ValueError, KeyError):
             if warn_on_unrecognized:
                 _logger.log(logging.WARNING if message_type_int < int(MessageType.RESERVED) else logging.DEBUG,
                             'Unrecognized message type %d.' % message_type_int)
             self.message_type = MessageType(message_type_int, raise_on_unrecognized=False)
 
-        return MessageHeader._SIZE
+        if return_sync_bytes:
+            return MessageHeader._SIZE, bytes((sync0, sync1))
+        else:
+            return MessageHeader._SIZE
 
     def get_message_size(self) -> int:
         """!
         @brief Calculate the total message size (header + payload).
 
         @return The message size (in bytes).
         """
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/device.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/fault_control.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/gnss_corrections.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/gnss_corrections.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/measurement_details.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/measurement_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         self.measurement_time_source = SystemTimeSource.INVALID
         self.data_source = SensorDataSource.UNKNOWN
         self.p1_time = Timestamp()
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.measurement_time.pack(buffer, offset, return_buffer=False)
         self._STRUCT.pack_into(buffer, offset, int(self.measurement_time_source), int(self.data_source))
         offset += self._STRUCT.size
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/measurements.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/measurements.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..utils.construct_utils import FixedPointAdapter, construct_message_to_string
 from ..utils.enum_utils import IntEnum
 
 ################################################################################
 # IMU Measurements
 ################################################################################
 
+
 class IMUInput(MessagePayload):
     """!
     @brief IMU sensor measurement input.
     """
     MESSAGE_TYPE = MessageType.IMU_INPUT
     MESSAGE_VERSION = 0
 
@@ -69,14 +70,15 @@
         else:
             return super().__getattr__(item)
 
     def __str__(self):
         return construct_message_to_string(message=self, construct=self.Construct, title='IMU Input',
                                            fields=['details', 'accel_mps2', 'gyro_rps', 'temperature_degc'])
 
+
 class IMUOutput(MessagePayload):
     """!
     @brief IMU sensor measurement data.
     """
     MESSAGE_TYPE = MessageType.IMU_OUTPUT
     MESSAGE_VERSION = 0
 
@@ -90,14 +92,15 @@
 
         self.gyro_rps = np.full((3,), np.nan)
         self.gyro_std_rps = np.full((3,), np.nan)
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
 
         offset += self.pack_values(
             self._STRUCT, buffer, offset,
@@ -781,14 +784,15 @@
         # Set to @ref GearType::FORWARD or @ref GearType::REVERSE where vehicle direction information is available
         # externally.
         self.gear = GearType.UNKNOWN
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.details.pack(buffer, offset, return_buffer=False)
 
         offset += self.pack_values(
             self._STRUCT, buffer, offset,
@@ -884,14 +888,15 @@
         # Set to @ref GearType::FORWARD or @ref GearType::REVERSE where vehicle direction information is available
         # externally.
         self.gear = GearType.UNKNOWN
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.details.pack(buffer, offset, return_buffer=False)
 
         offset += self.pack_values(
             self._STRUCT, buffer, offset,
@@ -995,14 +1000,15 @@
         # `true` if the wheel speeds are signed (positive forward, negative reverse), or `false` if the values are
         # unsigned (positive in both directions).
         self.is_signed = True
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.details.pack(buffer, offset, return_buffer=False)
 
         offset += self.pack_values(
             self._STRUCT, buffer, offset,
@@ -1099,14 +1105,15 @@
         # `true` if the wheel speeds are signed (positive forward, negative reverse), or `false` if the values are
         # unsigned (positive in both directions).
         self.is_signed = True
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.details.pack(buffer, offset, return_buffer=False)
 
         offset += self.pack_values(
             self._STRUCT, buffer, offset,
@@ -1160,48 +1167,51 @@
 ################################################################################
 # Heading Sensor Definitions
 ################################################################################
 
 
 class HeadingOutput(MessagePayload):
     """!
-     @brief Corrected heading sensor measurement output.
+    @brief Heading sensor measurement output with heading bias corrections applied.
     """
     MESSAGE_TYPE = MessageType.HEADING_OUTPUT
     MESSAGE_VERSION = 0
 
     _STRUCT = struct.Struct('<B3xL3ff')
 
     def __init__(self):
         ## Measurement timestamps, if available. See @ref measurement_messages.
         self.details = MeasurementDetails()
 
         ## Set to @ref SolutionType::RTKFixed when heading is available, or @ref SolutionType::Invalid otherwise.
         self.solution_type = SolutionType.Invalid
         ## A bitmask of flags associated with the solution
         self.flags = 0
-        ## The measured YPR vector (in degrees), resolved in the ENU frame.
+
+        ##
+        # The measured YPR vector (in degrees), resolved in the ENU frame, after applying horizontal (yaw) and vertical
+        # (pitch) bias corrections.
         self.ypr_deg = np.full((3,), np.nan)
 
         ##
-        # The corrected heading between the primary device antenna and the secondary (in degrees) with
-        # respect to true north.
+        # The heading angle (in degrees) with respect to true north, pointing from the primary antenna to the secondary
+        # antenna, after applying bias corrections.
         #
         # @note
         # Reported in the range [0, 360).
         self.heading_true_north_deg = np.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
-        buffer = self.details.pack(buffer)
-        offset += self.details.calcsize()
+        offset += self.details.pack(buffer, offset, return_buffer=False)
 
         self._STRUCT.pack_into(
             buffer, offset,
             int(self.solution_type),
             self.flags,
             self.ypr_deg[0],
             self.ypr_deg[1],
@@ -1220,54 +1230,53 @@
         offset += self.details.unpack(buffer, offset)
 
         (solution_type_int,
          self.flags,
          self.ypr_deg[0],
          self.ypr_deg[1],
          self.ypr_deg[2],
-         self.heading_true_north_deg) = self._STRUCT.unpack_from(buffer, offset)
+         self.heading_true_north_deg) = \
+            self._STRUCT.unpack_from(buffer, offset)
         offset += self._STRUCT.size
 
         self.solution_type = SolutionType(solution_type_int)
 
         return offset - initial_offset
 
     def __repr__(self):
         result = super().__repr__()[:-1]
-        ypr_str = ['%.1f' % v for v in self.ypr_deg]
-        result += f', solution_type={self.solution_type}, ypr=[{ypr_str}] deg]'
+        result += f', solution_type={self.solution_type}, heading={self.heading_true_north_deg:.1f} deg]'
         return result
 
     def __str__(self):
         return f"""\
 Heading Output @ {str(self.details.p1_time)}
   Solution Type: {self.solution_type}
   YPR (ENU) (deg): {self.ypr_deg[0]:.2f}, {self.ypr_deg[1]:.2f}, {self.ypr_deg[2]:.2f}
-  Heading (deg): {self.heading_true_north_deg:.2f}
-  """
+  Heading (deg): {self.heading_true_north_deg:.2f}"""
 
     @classmethod
     def calcsize(cls) -> int:
         return cls._STRUCT.size + MeasurementDetails.calcsize()
 
     @classmethod
     def to_numpy(cls, messages: Sequence['HeadingOutput']):
         result = {
             'solution_type': np.array([int(m.solution_type) for m in messages], dtype=int),
             'flags': np.array([int(m.flags) for m in messages], dtype=np.uint32),
             'ypr_deg': np.array([m.ypr_deg for m in messages]).T,
-            'heading_true_north_deg': np.array([m.heading_true_north_deg for m in messages], dtype=float).T,
+            'heading_true_north_deg': np.array([m.heading_true_north_deg for m in messages], dtype=float),
         }
         result.update(MeasurementDetails.to_numpy([m.details for m in messages]))
         return result
 
 
 class RawHeadingOutput(MessagePayload):
     """!
-     @brief Raw (uncorrected) heading sensor measurement output.
+    @brief Raw (uncorrected) heading sensor measurement output.
     """
     MESSAGE_TYPE = MessageType.RAW_HEADING_OUTPUT
     MESSAGE_VERSION = 0
 
     _STRUCT = struct.Struct('<B3xL3f3fff')
 
     def __init__(self):
@@ -1299,14 +1308,15 @@
         ##
         # The estimated distance between primary and secondary antennas (in meters).
         self.baseline_distance_m = np.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         buffer = self.details.pack(buffer)
         offset += self.details.calcsize()
 
         self._STRUCT.pack_into(
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/ros.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/ros.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         # The platform orientation, represented as a quaternion with the scalar
         # component last (x, y, z, w)
         self.orientation = np.full((4,), np.nan)
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
 
         struct.pack_into(ROSPoseMessage._FORMAT, buffer, offset,
                          self.position_rel_m[0], self.position_rel_m[1], self.position_rel_m[2],
@@ -156,14 +157,15 @@
         self.position_covariance_type = CovarianceType.COVARIANCE_TYPE_UNKNOWN
 
         self.reserved = np.full((3,), 0, np.uint8)
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
 
         struct.pack_into(ROSGPSFixMessage._FORMAT, buffer, offset,
                          self.latitude_deg,
@@ -284,14 +286,15 @@
         self.acceleration_mps2 = np.full((3,), 0.0)
         # Vehicle x/y/z acceleration covariance matrix. Set to -1 if not available
         self.acceleration_covariance = np.full((9,), -1.0)
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
 
         struct.pack_into(
             ROSIMUMessage._FORMAT, buffer, offset,
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/signal_defs.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/solution.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.aggregate_protection_level_m = np.nan
         self.horizontal_protection_level_m = np.nan
         self.vertical_protection_level_m = np.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
         offset += self.gps_time.pack(buffer, offset, return_buffer=False)
 
         if np.isnan(self.undulation_m):
@@ -184,14 +185,15 @@
 
         self.velocity_enu_mps = np.full((3,), np.nan)
         self.velocity_std_enu_mps = np.full((3,), np.nan)
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
 
         offset += self.pack_values(
             self._STRUCT, buffer, offset,
@@ -273,14 +275,15 @@
         self.vdop = np.nan
 
         self.gps_time_std_sec = np.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
         offset += self.gps_time.pack(buffer, offset, return_buffer=False)
 
         if np.isnan(self.corrections_age_sec):
@@ -414,14 +417,15 @@
         self.elevation_deg = np.nan
         ## The C/N0 of the L1 signal present on this satellite (in dB-Hz).
         self.cn0_dbhz = np.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         if np.isnan(self.cn0_dbhz):
             cn0_int = SatelliteInfo.INVALID_CN0
         else:
             cn0_int = round(self.cn0_dbhz / 0.25)
             if cn0_int > 255:
                 cn0_int = 255
@@ -472,14 +476,15 @@
         self.gps_time = Timestamp()
 
         self.svs: List[SatelliteInfo] = []
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
         offset += self.gps_time.pack(buffer, offset, return_buffer=False)
 
         self._STRUCT.pack_into(buffer, offset, len(self.svs))
@@ -676,14 +681,15 @@
         self.mounting_angle_max_std_dev_deg = np.full((3,), np.nan)
 
         ## @}
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         if buffer is None:
             buffer = bytearray(self.calcsize())
+            offset = 0
 
         initial_offset = offset
 
         offset += self.p1_time.pack(buffer, offset, return_buffer=False)
 
         self._STRUCT.pack_into(
             buffer, offset,
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/messages/timestamp.py` & `fusion_engine_client-1.23.1/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/parsers/decoder.py` & `fusion_engine_client-1.23.1/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/parsers/encoder.py` & `fusion_engine_client-1.23.1/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/parsers/fast_indexer.py` & `fusion_engine_client-1.23.1/fusion_engine_client/parsers/fast_indexer.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/parsers/file_index.py` & `fusion_engine_client-1.23.1/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion_engine_client-1.23.1/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/argument_parser.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,16 @@
         if not isinstance(values, list):
             values = [values]
 
         flattened_values = [v.strip() for entry in values for v in entry.split(',')]
         result = getattr(namespace, self.dest)
         if result is None:
             result = []
+        elif result is self.default:
+            result = []
         result.extend(flattened_values)
         setattr(namespace, self.dest, result)
 
 
 class TriStateBoolFormatter(argparse.HelpFormatter):
     def _format_action_invocation(self, action):
         if isinstance(action, TriStateBooleanAction):
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/bin_utils.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/construct_utils.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/enum_utils.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/log.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/numpy_utils.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/time_range.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client/utils/trace.py` & `fusion_engine_client-1.23.1/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client.egg-info/PKG-INFO` & `fusion_engine_client-1.23.1/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.23.0
+Version: 1.23.1
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
-Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.0.tar.gz
+Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.1.tar.gz
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -23,25 +23,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: construct>=2.10.0
 Requires-Dist: numpy>=1.16.0
-Requires-Dist: pymap3d>=2.4.3
-Requires-Dist: aenum>=3.1.1
 Requires-Dist: p1-gpstime>=0.6.3.dev1
+Requires-Dist: argparse-formatter>=1.4
 Requires-Dist: packaging>=21.0.0
+Requires-Dist: pymap3d>=2.4.3
+Requires-Dist: plotly>=4.0.0
+Requires-Dist: scipy>=1.5.0
 Requires-Dist: palettable>=3.3.0
 Requires-Dist: colorama>=0.4.4
-Requires-Dist: scipy>=1.5.0
-Requires-Dist: construct>=2.10.0
-Requires-Dist: plotly>=4.0.0
-Requires-Dist: argparse-formatter>=1.4
+Requires-Dist: aenum>=3.1.1
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion_engine_client-1.23.0/fusion_engine_client.egg-info/SOURCES.txt` & `fusion_engine_client-1.23.1/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/setup.py` & `fusion_engine_client-1.23.1/setup.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_config.py` & `fusion_engine_client-1.23.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_construct_utils.py` & `fusion_engine_client-1.23.1/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_data_loader.py` & `fusion_engine_client-1.23.1/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_decoder.py` & `fusion_engine_client-1.23.1/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_encoder.py` & `fusion_engine_client-1.23.1/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_enum_utils.py` & `fusion_engine_client-1.23.1/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_file_index.py` & `fusion_engine_client-1.23.1/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_message_defs.py` & `fusion_engine_client-1.23.1/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_mixed_log_reader.py` & `fusion_engine_client-1.23.1/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.0/tests/test_time_range.py` & `fusion_engine_client-1.23.1/tests/test_time_range.py`

 * *Files identical despite different names*

