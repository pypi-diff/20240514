# Comparing `tmp/ddeutil_io-0.1.1.tar.gz` & `tmp/ddeutil_io-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_io-0.1.1.tar", last modified: Mon May 13 11:55:53 2024, max compression
+gzip compressed data, was "ddeutil_io-0.1.2.tar", last modified: Tue May 14 15:55:47 2024, max compression
```

## Comparing `ddeutil_io-0.1.1.tar` & `ddeutil_io-0.1.2.tar`

### file list

```diff
@@ -1,61 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.281828 ddeutil_io-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-13 11:55:53.281828 ddeutil_io-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:55:53.281828 ddeutil_io-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.269828 ddeutil_io-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.269828 ddeutil_io-0.1.1/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.273828 ddeutil_io-0.1.1/src/ddeutil/io/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/__about__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.273828 ddeutil_io-0.1.1/src/ddeutil/io/__base/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/__base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/__base/__regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/__base/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/__base/pathutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/__base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18156 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.277828 ddeutil_io-0.1.1/src/ddeutil/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9315 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.277828 ddeutil_io-0.1.1/src/ddeutil/node/base/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/base/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/base/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/base/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/datasets_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.277828 ddeutil_io-0.1.1/src/ddeutil/node/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/vendors/boto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/vendors/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/src/ddeutil/node/vendors/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.281828 ddeutil_io-0.1.1/src/ddeutil_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-13 11:55:53.000000 ddeutil_io-0.1.1/src/ddeutil_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-13 11:55:53.000000 ddeutil_io-0.1.1/src/ddeutil_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:55:53.000000 ddeutil_io-0.1.1/src/ddeutil_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 11:55:53.000000 ddeutil_io-0.1.1/src/ddeutil_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 11:55:53.000000 ddeutil_io-0.1.1/src/ddeutil_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:53.281828 ddeutil_io-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_base_dir_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_base_file_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_base_file_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_base_file_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_config_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-13 11:55:48.000000 ddeutil_io-0.1.1/tests/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.179581 ddeutil_io-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.179581 ddeutil_io-0.1.2/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.179581 ddeutil_io-0.1.2/src/ddeutil/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__about__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.183581 ddeutil_io-0.1.2/src/ddeutil/io/__base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/__regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17049 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.183581 ddeutil_io-0.1.2/src/ddeutil/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9315 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.183581 ddeutil_io-0.1.2/src/ddeutil/node/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/datasets_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/src/ddeutil/node/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/boto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_file_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_config_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_register.py
```

### Comparing `ddeutil_io-0.1.1/LICENSE` & `ddeutil_io-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/PKG-INFO` & `ddeutil_io-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
@@ -60,17 +60,17 @@
 
 ### Config
 
 The **Config Object** is the file system handler object.
 
 ```python
 from pathlib import Path
-from ddeutil.io.config import ConfFile
+from ddeutil.io.config import ConfFl
 
-config: ConfFile = ConfFile(path=Path(), compress="gzip")
+config: ConfFl = ConfFl(path=Path('./file.gz.yaml'), compress="gzip")
 ```
 
 ### Register
 
 The **Register Object** is the metadata generator object for the config data.
 If you passing name and configs to this object, it will find the config name
 in any stage storage and generate its metadata to you.
@@ -83,14 +83,15 @@
     name='examples:conn_data_local_file',
     config=Params.model_validate({
         "stages": {
           "raw": {"format": "{naming:%s}.{timestamp:%Y%m%d_%H%M%S}"},
         },
     }),
 )
+registry.move(stage="raw")
 ```
 
 ### Link
 
 ```yaml
 connection_local_file_landing:
     type: "connection.LocalSystem"
```

### Comparing `ddeutil_io-0.1.1/README.md` & `ddeutil_io-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 ### Config
 
 The **Config Object** is the file system handler object.
 
 ```python
 from pathlib import Path
-from ddeutil.io.config import ConfFile
+from ddeutil.io.config import ConfFl
 
-config: ConfFile = ConfFile(path=Path(), compress="gzip")
+config: ConfFl = ConfFl(path=Path('./file.gz.yaml'), compress="gzip")
 ```
 
 ### Register
 
 The **Register Object** is the metadata generator object for the config data.
 If you passing name and configs to this object, it will find the config name
 in any stage storage and generate its metadata to you.
@@ -52,14 +52,15 @@
     name='examples:conn_data_local_file',
     config=Params.model_validate({
         "stages": {
           "raw": {"format": "{naming:%s}.{timestamp:%Y%m%d_%H%M%S}"},
         },
     }),
 )
+registry.move(stage="raw")
 ```
 
 ### Link
 
 ```yaml
 connection_local_file_landing:
     type: "connection.LocalSystem"
```

### Comparing `ddeutil_io-0.1.1/pyproject.toml` & `ddeutil_io-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 [[tool.mypy.overrides]]
 module = "tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.black]
 line-length = 80
+preview = true
 target-version = ['py39']
 exclude = """
 /(
     \\.git
     | \\.__pycache__
     | \\.idea
     | \\.ruff_cache
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/__base/__regex.py` & `ddeutil_io-0.1.2/src/ddeutil/io/__base/__regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MULTILINE,
     UNICODE,
     VERBOSE,
     Pattern,
 )
 
 
-class SettingRegex:
+class RegexConf:
     """Core Configuration Model"""
 
     # Normal regular expression for the secret value.
     # ---
     # [\"\']?                             # single or double quoted value
     # (?P<search>@secrets{                # search string for replacement
     #     (?P<braced>.*?)                 # value if use braced {}
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/__base/files.py` & `ddeutil_io-0.1.2/src/ddeutil/io/__base/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
 """
 This is then main function for open any files in local or remote space
 with the best python libraries and the best practice such as build-in
 ``io.open``, ``mmap.mmap``, etc.
+
+NOTE:
+    - Add more compress type such as
+        - h5,hdf5(h5py)
+        - fits(astropy)
+        - rar(...)
 """
 from __future__ import annotations
 
 import abc
 import csv
 import io
 import json
+import logging
 import marshal
 import mmap
 import os
 import pickle
 from contextlib import contextmanager
 from pathlib import Path
 from typing import (
@@ -37,43 +44,66 @@
 import yaml
 
 try:
     from yaml import CSafeLoader as SafeLoader
 except ImportError:
     from yaml import SafeLoader
 
-from .__regex import SettingRegex
+from .__regex import RegexConf
 from .utils import search_env, search_env_replace
 
 FileCompressType = Literal["gzip", "gz", "xz", "bz2"]
-
-# NOTE:
-#   add more compress type such as
-#       - h5,hdf5(h5py)
-#       - fits(astropy)
-#       - rar(...)
 DirCompressType = Literal["zip", "rar", "tar", "h5", "hdf5", "fits"]
 
 
+def compress_lib(compress: str) -> CompressProtocol:
+    """Return Compress module that use to unpack data from the compressed file.
+
+    Note:
+        Now, it support for "gzip", "gz", "xz", "bz2"]
+    """
+    if not compress:
+        return io
+    elif compress in ("gzip", "gz"):
+        import gzip
+
+        return gzip
+    elif compress in ("bz2",):
+        import bz2
+
+        return bz2
+    elif compress in ("xz",):
+        import lzma as xz
+
+        return xz
+    raise NotImplementedError(f"Compress {compress} does not implement yet")
+
+
 class CompressProtocol(Protocol):
     def decompress(self, *args, **kwargs) -> AnyStr: ...
 
     def open(self, *args, **kwargs) -> IO: ...
 
 
-class OpenFileAbc(abc.ABC):
+class FlAbc(abc.ABC):
     @abc.abstractmethod
     def read(self, *args, **kwargs): ...
 
     @abc.abstractmethod
     def write(self, *args, **kwargs): ...
 
 
-class OpenFile(OpenFileAbc):
-    """Open File Object"""
+class Fl:
+    """Open File Object that use to open any simple or compression file from
+    local file system.
+
+    Examples:
+        >>> with Fl('./dwh/conf/params.gz.txt', compress='gzip').open() as f:
+        ...     data = f.readline()
+    """
 
     def __init__(
         self,
         path: Union[str, Path],
         *,
         encoding: Optional[str] = None,
         compress: Optional[FileCompressType] = None,
@@ -83,103 +113,94 @@
         self.compress: Optional[FileCompressType] = compress
 
         # Action anything after set up attributes.
         self.after_set_attrs()
 
     def after_set_attrs(self) -> None: ...
 
-    @property
-    def compress_lib(self) -> CompressProtocol:
-        """Return Compress package"""
-        if not self.compress:
-            return io
-        elif self.compress in ("gzip", "gz"):
-            import gzip
-
-            return gzip
-        elif self.compress in ("bz2",):
-            import bz2
-
-            return bz2
-        elif self.compress in ("xz",):
-            import lzma as xz
-
-            return xz
-        raise NotImplementedError(
-            f"Compress {self.compress} does not implement yet"
-        )
+    def __call__(self, *args, **kwargs) -> IO:
+        return self.open(*args, **kwargs)
 
     @property
-    def decompress(self) -> Callable:
+    def decompress(self) -> Callable[[...], AnyStr]:
         if self.compress and self.compress in get_args(FileCompressType):
-            return self.compress_lib.decompress
+            return compress_lib(self.compress).decompress
         raise NotImplementedError(
             "Does not implement decompress method for None compress value."
         )
 
     def convert_mode(
         self,
         mode: Optional[str] = None,
+        *,
         default: bool = True,
     ) -> dict[str, str]:
+        """Convert mode before passing to the main standard lib.
+
+        :param mode: a reading or writing mode for the open method.
+        :param default: a default flag for return reading mode if a mode does
+            not set.
+        :type default: bool(=True)
+
+        :return: A mapping of mode and other input parameters for standard libs.
+        """
         if not mode:
             if default:
                 return {"mode": "r"}
             raise ValueError("The mode value does not set.")
         byte_mode: bool = "b" in mode
         if self.compress is None:
             _mode: dict[str, str] = {"mode": mode}
             return _mode if byte_mode else {"encoding": self.encoding, **_mode}
         elif not byte_mode and self.compress in ("gzip", "gz", "xz", "bz2"):
             # NOTE:
             #   Add `t` in open file mode for force with text mode.
             return {"mode": f"{mode}t", "encoding": self.encoding}
         elif byte_mode and self.compress in ("gzip", "gz", "xz", "bz2"):
             return {"mode": mode}
+        return {"mode": mode}
 
     def open(self, *, mode: Optional[str] = None, **kwargs) -> IO:
-        return self.compress_lib.open(
+        return compress_lib(self.compress).open(
             self.path,
-            **self.convert_mode(mode),
-            **kwargs,
+            **(self.convert_mode(mode) | kwargs),
         )
 
     @contextmanager
     def mopen(self, *, mode: Optional[str] = None) -> IO:
-        _mode: str = mode or "r"
-        _f: IO = self.open(mode=mode)
-        _access = mmap.ACCESS_READ if ("r" in _mode) else mmap.ACCESS_WRITE
+        mode: str = mode or "r"
+        file: IO = self.open(mode=mode)
+        _access = mmap.ACCESS_READ if ("r" in mode) else mmap.ACCESS_WRITE
         try:
-            yield mmap.mmap(
-                _f.fileno(),
-                length=0,
-                access=_access,
-            )
-        except ValueError:
-            yield _f
+            yield mmap.mmap(file.fileno(), length=0, access=_access)
+        except ValueError as err:
+            if str(err) != "cannot mmap an empty file":
+                raise err
+            yield file
+            logging.error("Does not open file with memory mode")
         finally:
-            _f.close()
+            file.close()
 
     def read(self, *args, **kwargs):
         raise NotImplementedError
 
     def write(self, *args, **kwargs):
         raise NotImplementedError
 
 
-class OpenDir:
+class Dir:
     """Open File Object"""
 
     def __init__(
         self,
         path: Union[str, Path],
         *,
         compress: Optional[DirCompressType] = None,
     ):
-        self.path = path
+        self.path: Path = Path(path) if isinstance(path, str) else path
         self.compress = compress
         # Action anything after set up attributes.
         self.after_set_attrs()
 
     def after_set_attrs(self) -> None: ...
 
     def open(self, *, mode: str, **kwargs):
@@ -202,15 +223,15 @@
             return tarfile.open(
                 self.path,
                 mode=f"{mode}:gz",  # w:bz2
             )
         return NotImplementedError
 
 
-class Env(OpenFile):
+class EnvFl(Fl, FlAbc):
     """Env object which mapping search engine"""
 
     keep_newline: ClassVar[bool] = False
     default: ClassVar[str] = ""
 
     def read(self, *, update: bool = True) -> dict[str, str]:
         with self.open(mode="r") as _r:
@@ -224,15 +245,15 @@
                 os.environ.update(**_result)
             return _result
 
     def write(self, data: dict[str, Any]) -> None:
         raise NotImplementedError
 
 
-class Yaml(OpenFile):
+class YamlFl(Fl, FlAbc):
     """Yaml File Object
 
     .. noted::
         - The boolean value in the yaml file
             - true: Y, true, Yes, ON
             - false: n, false, No, off
     """
@@ -244,45 +265,45 @@
         return NotImplementedError
 
     def write(self, data: dict[str, Any]) -> None:
         with self.open(mode="w") as _w:
             yaml.dump(data, _w, default_flow_style=False)
 
 
-class YamlEnv(Yaml):
+class YamlEnvFl(YamlFl):
     """Yaml object which mapping search environment variable."""
 
     raise_if_not_default: ClassVar[bool] = False
-    default: ClassVar[str] = "N/A"
+    default: ClassVar[str] = "null"
     escape: ClassVar[str] = "ESC"
 
     @staticmethod
     def prepare(x: str) -> str:
         return x
 
     def read(self, safe: bool = True) -> dict[str, Any]:
         if safe:
             with self.open(mode="r") as _r:
                 _env_replace: str = search_env_replace(
-                    SettingRegex.RE_YAML_COMMENT.sub("", _r.read()),
+                    RegexConf.RE_YAML_COMMENT.sub("", _r.read()),
                     raise_if_default_not_exists=self.raise_if_not_default,
                     default=self.default,
                     escape=self.escape,
                     caller=self.prepare,
                 )
                 if _result := yaml.load(_env_replace, SafeLoader):
                     return _result
                 return {}
         return NotImplementedError
 
     def write(self, data: dict[str, Any]) -> None:
         raise NotImplementedError
 
 
-class CSV(OpenFile):
+class CsvFl(Fl, FlAbc):
     def read(self) -> list[str]:
         with self.open(mode="r") as _r:
             try:
                 dialect = csv.Sniffer().sniff(_r.read(128))
                 _r.seek(0)
                 return list(csv.DictReader(_r, dialect=dialect))
             except csv.Error:
@@ -323,15 +344,15 @@
         with self.open(mode="r") as _r:
             try:
                 return csv.Sniffer().has_header(_r.read(128))
             except csv.Error:
                 return False
 
 
-class CSVPipeDim(CSV):
+class CsvPipeFl(CsvFl):
     def after_set_attrs(self) -> None:
         csv.register_dialect(
             "pipe_delimiter", delimiter="|", quoting=csv.QUOTE_ALL
         )
 
     def read(self) -> list:
         with self.open(mode="r") as _r:
@@ -371,15 +392,15 @@
                     **kwargs,
                 )
                 if mode == "w" or not self.has_header:
                     writer.writeheader()
                 writer.writerows(data)
 
 
-class Json(OpenFile):
+class JsonFl(Fl, FlAbc):
     def read(self) -> Union[dict[Any, Any], list[Any]]:
         with self.open(mode="r") as _r:
             try:
                 return json.loads(_r.read())
             except json.decoder.JSONDecodeError:
                 return {}
 
@@ -393,15 +414,15 @@
         with self.open(mode="w") as _w:
             if self.compress:
                 _w.write(json.dumps(data))
             else:
                 json.dump(data, _w, indent=indent)
 
 
-class JsonEnv(Json):
+class JsonEnvFl(JsonFl):
     raise_if_not_default: bool = False
     default: str = "N/A"
     escape: str = "ESC"
 
     @staticmethod
     def prepare(x: str) -> str:
         return x
@@ -418,39 +439,39 @@
                 )
             )
 
     def write(self, data, *, indent: int = 4) -> None:
         raise NotImplementedError
 
 
-class Pickle(OpenFile):
+class PickleFl(Fl, FlAbc):
     def read(self):
         with self.open(mode="rb") as _r:
             return pickle.loads(_r.read())
 
     def write(self, data):
         with self.open(mode="wb") as _w:
             pickle.dump(data, _w)
 
 
-class Marshal(OpenFile):
+class MarshalFl(Fl, FlAbc):
     def read(self):
         with self.open(mode="rb") as _r:
             return marshal.loads(_r.read())
 
     def write(self, data):
         with self.open(mode="wb") as _w:
             marshal.dump(data, _w)
 
 
 __all__ = (
-    "OpenFile",
-    "Env",
-    "Json",
-    "JsonEnv",
-    "Yaml",
-    "YamlEnv",
-    "CSV",
-    "CSVPipeDim",
-    "Marshal",
-    "Pickle",
+    "Fl",
+    "EnvFl",
+    "JsonFl",
+    "JsonEnvFl",
+    "YamlFl",
+    "YamlEnvFl",
+    "CsvFl",
+    "CsvPipeFl",
+    "MarshalFl",
+    "PickleFl",
 )
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/__base/pathutils.py` & `ddeutil_io-0.1.2/src/ddeutil/io/__base/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-import datetime
+from __future__ import annotations
+
 import fnmatch
 import os
 import shutil
-from collections.abc import Iterator
 from pathlib import Path
 from typing import (
     Optional,
 )
 
-
-def replace_os(path: str) -> str:
-    return path.replace(os.sep, "/")
-
-
-def get_modification_time(path: str) -> datetime.datetime:
-    """Return datetime of modification of file."""
-    timestamp = os.path.getmtime(path)
-    return datetime.datetime.fromtimestamp(timestamp)
-
-
-def get_files(path: str, pattern: str) -> Iterator[Path]:
-    """Return path from glob method."""
-    yield from Path(path).glob(pattern)
+from .__regex import RegexConf
+from .files import (
+    CsvFl,
+    CsvPipeFl,
+    EnvFl,
+    Fl,
+    JsonEnvFl,
+    JsonFl,
+    MarshalFl,
+    PickleFl,
+    YamlEnvFl,
+    YamlFl,
+)
+from .utils import (
+    add_newline,
+    search_env_replace,
+)
 
 
 def rm(path: str, is_dir: bool = False) -> None:
-    """param <path> could either be relative or absolute."""
+    """Remove file or dir from a input path."""
     if os.path.isfile(path) or os.path.islink(path):
         os.remove(path)
     elif os.path.isdir(path) and is_dir:
         shutil.rmtree(path)
     else:
         raise ValueError(
             f"file {path!r} is not a file{' or dir' if is_dir else ''}."
         )
 
 
 def touch(filename: str, times=None) -> None:
+    """Touch file"""
     file_handle = open(filename, mode="a")
     try:
         os.utime(filename, times)
     finally:
         file_handle.close()
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/__base/utils.py` & `ddeutil_io-0.1.2/src/ddeutil/io/__base/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 import os
 from typing import (
     Callable,
     Optional,
 )
 
 try:
-    from .__regex import SettingRegex
+    from .__regex import RegexConf
 except ImportError:
-    from __regex import SettingRegex
+    from __regex import RegexConf
 
 
 def add_newline(text: str, newline: Optional[str] = None) -> str:
+    """Add newline to a text value."""
     nl: str = newline or "\n"
     return f"{text}{nl}" if not text.endswith(nl) else text
 
 
 def search_env_replace(
     contents: str,
     *,
     raise_if_default_not_exists: bool = False,
     default: str = "N/A",
     escape: str = "ESC",
     caller: Callable[[str], str] = (lambda x: x),
 ) -> str:
-    """Prepare content data before parse to any file loading method"""
+    """Prepare content data before parse to any file parsing object.
+
+    :param contents:
+    :param raise_if_default_not_exists:
+    :param default: a default value.
+    :param escape: a escape value that use for initial replace when found escape
+        char on searching.
+    :param caller: a prepare function.
+    """
     shifting: int = 0
     replaces: dict = {}
     replaces_esc: dict = {}
-    for content in SettingRegex.RE_ENV_SEARCH.finditer(contents):
+    for content in RegexConf.RE_ENV_SEARCH.finditer(contents):
         search: str = content.group(1)
         if not (_escaped := content.group("escaped")):
             var: str = content.group("braced")
             _braced_default: str = content.group("braced_default")
             if not _braced_default and raise_if_default_not_exists:
                 raise ValueError(
                     f"Could not find default value for {var} "
@@ -76,40 +85,40 @@
     :param default: a default value that use if it does not exists
 
     References:
         - python-dotenv (https://github.com/theskumar/python-dotenv)
     """
     _default: str = default or ""
     env: dict[str, str] = {}
-    for content in SettingRegex.RE_DOTENV.finditer(contents):
+    for content in RegexConf.RE_DOTENV.finditer(contents):
         name: str = content.group("name")
 
         # Remove leading/trailing whitespace
         _value: str = (content.group("value") or "").strip()
 
         if not _value:
             raise ValueError(
                 f"Value {name:!r} in `.env` file does not set value "
                 f"of variable"
             )
         value: str = _value if keep_newline else "".join(_value.splitlines())
         quoted: Optional[str] = None
 
         # Remove surrounding quotes
-        if m2 := SettingRegex.RE_ENV_VALUE_QUOTED.match(value):
+        if m2 := RegexConf.RE_ENV_VALUE_QUOTED.match(value):
             quoted: str = m2.group("quoted")
             value: str = m2.group("value")
 
         if quoted == "'":
             env[name] = value
             continue
         elif quoted == '"':
             # Unescape all chars except $ so variables
             # can be escaped properly
-            value: str = SettingRegex.RE_ENV_ESCAPE.sub(r"\1", value)
+            value: str = RegexConf.RE_ENV_ESCAPE.sub(r"\1", value)
 
         # Substitute variables in a value
         env[name] = __search_var(value, env, default=_default)
     return env
 
 
 def __search_var(
@@ -133,15 +142,15 @@
         'Test bar'
         >>> import os
         >>> os.environ["VAR2"] = "baz"
         >>> __search_var("Test ${VAR2}", {"VAR": "foo"}, default="bar")
         'Test baz'
     """
     _default: str = default or ""
-    for sub_content in SettingRegex.RE_DOTENV_VAR.findall(value):
+    for sub_content in RegexConf.RE_DOTENV_VAR.findall(value):
         replace: str = "".join(sub_content[1:-1])
         if sub_content[0] != "\\":
             # Replace it with the value from the environment
             replace: str = env.get(
                 sub_content[-1],
                 os.environ.get(sub_content[-1], _default),
             )
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/config.py` & `ddeutil_io-0.1.2/src/ddeutil/io/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 from typing import (
     Any,
     Optional,
     Union,
 )
 
 from .__base import (
-    Json,
-    OpenFile,
-    YamlEnv,
+    Fl,
+    JsonFl,
+    PathSearch,
+    YamlEnvFl,
+    rm,
 )
-from .__base.pathutils import PathSearch, rm
 from .exceptions import ConfigArgumentError
 
 
 class ConfABC(abc.ABC):
     """Config Adapter abstract object."""
 
     @abc.abstractmethod
@@ -47,30 +48,30 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def create(self, name: str, **kwargs) -> None:
         raise NotImplementedError
 
 
-class BaseConfFile:
+class BaseConfFl:
     """Base Config File object for getting data with `.yaml` format and mapping
     environment variables to the content data.
     """
 
     def __init__(
         self,
         path: Union[str, Path],
         *,
         compress: Optional[str] = None,
-        open_file: Optional[type[OpenFile]] = None,
+        open_file: Optional[type[Fl]] = None,
         excluded_fmt: Optional[tuple[str]] = None,
     ):
         self.path: Path = Path(path) if isinstance(path, str) else path
         self.compress: Optional[str] = compress
-        self.open_file: type[OpenFile] = open_file or YamlEnv
+        self.open_file: type[Fl] = open_file or YamlEnvFl
         self.excluded_fmt: tuple[str] = excluded_fmt or (".json", ".toml")
         if not self.path.exists():
             self.path.mkdir(parents=True)
 
     def load(
         self,
         name: str,
@@ -138,39 +139,39 @@
     ) -> None:
         """Copy filename to destination path."""
         if auto_create:
             destination.mkdir(parents=True, exist_ok=True)
         shutil.copy(self.path / path, destination)
 
 
-class ConfFile(BaseConfFile, ConfABC):
+class ConfFl(BaseConfFl, ConfABC):
     """Config File Loading Object for get data from configuration and stage."""
 
     def __init__(
         self,
         path: Union[str, Path],
         *,
         compress: Optional[str] = None,
-        open_file: Optional[type[OpenFile]] = None,
+        open_file: Optional[type[Fl]] = None,
         excluded_fmt: Optional[list[str]] = None,
-        open_file_stg: Optional[type[OpenFile]] = None,
+        open_file_stg: Optional[type[Fl]] = None,
     ):
         """Main initialize of config file loading object.
 
         :param path: A path of files to action.
         :type path: Union[str, Path]
         :param compress: Optional[str] : A compress type of action file.
         """
         super().__init__(
             path,
             compress=compress,
             open_file=open_file,
             excluded_fmt=excluded_fmt,
         )
-        self.open_file_stg: type[OpenFile] = open_file_stg or Json
+        self.open_file_stg: type[Fl] = open_file_stg or JsonFl
 
     def load_stage(
         self,
         path: Union[str, Path],
         *,
         default: Optional[Any] = None,
     ) -> Union[dict[Any, Any], list[Any]]:
@@ -192,14 +193,15 @@
     ) -> None:
         """Write content data to file with filename. If merge is true, it will
         load current data from file and merge the data content together
         before write.
         """
         if not merge:
             self.open_file_stg(path, compress=self.compress).write(data)
+            print(f"Start writing data to {path}")
             return
         elif merge and (
             "mode"
             in inspect.getfullargspec(self.open_file_stg.write).annotations
         ):
             self.open_file_stg(path, compress=self.compress).write(
                 **{
@@ -400,11 +402,11 @@
         _results: dict = data.copy()
         _results[_key] = json.loads(data[_key])
         return _results
 
 
 __all__ = (
     "ConfABC",
-    "ConfFile",
+    "ConfFl",
     "ConfSQLite",
-    "OpenFile",
+    "Fl",
 )
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/exceptions.py` & `ddeutil_io-0.1.2/src/ddeutil/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/models.py` & `ddeutil_io-0.1.2/src/ddeutil/io/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
 from __future__ import annotations
 
-import datetime
-import pathlib
 import re
+from pathlib import Path
 from typing import (
     Any,
     Optional,
     Union,
 )
 
-from ddeutil.io.__base import YamlEnv
-from ddeutil.io.exceptions import ConfigArgumentError
 from pydantic import (
     BaseModel,
     Field,
     ValidationInfo,
-    field_validator,
 )
+from pydantic.functional_validators import field_validator
+
+from .__base import YamlEnvFl
+from .exceptions import ConfigArgumentError
 
 FMT_NAMES: tuple[str, ...] = (
     "naming",
     "domain",
     "environ",
     "timestamp",
     "version",
@@ -49,15 +49,14 @@
             },
             "excluded": [],
             "compress": None,
         }
     """
 
     timestamp: Optional[dict[str, int]] = Field(default_factory=dict)
-
     version: Optional[str] = Field(default=None)
     excluded: Optional[list[str]] = Field(default_factory=list)
     compress: Optional[str] = Field(default=None)
 
 
 class StageData(BaseModel):
     """
@@ -117,43 +116,36 @@
                         f"a `{validator}` format name in the format."
                     ),
                 )
         return value
 
 
 class PathData(BaseModel):
-    root: Union[str, pathlib.Path] = Field(default_factory=pathlib.Path)
-    data: pathlib.Path = Field(default="data", validate_default=True)
-    conf: pathlib.Path = Field(default="conf", validate_default=True)
-    archive: pathlib.Path = Field(default=".archive", validate_default=True)
+    root: Path = Field(default_factory=Path)
+    data: Path = Field(default="data", validate_default=True)
+    conf: Path = Field(default="conf", validate_default=True)
+    archive: Path = Field(default=".archive", validate_default=True)
 
     @field_validator("root", mode="before")
-    def prepare_root(cls, v):
-        if isinstance(v, str):
-            return pathlib.Path(v)
-        return v
+    def prepare_root(cls, v: Union[str, Path]) -> Path:
+        return Path(v) if isinstance(v, str) else v
 
     @field_validator("data", "conf", "archive", mode="before")
-    def prepare_path_from_str(
-        cls,
-        v,
-        info: ValidationInfo,
-    ) -> pathlib.Path:
-        _root: pathlib.Path = info.data["root"]
-        return v if isinstance(v, pathlib.Path) else (_root / v)
+    def prepare_path_from_str(cls, v, info: ValidationInfo) -> Path:
+        return v if isinstance(v, Path) else (info.data["root"] / v)
 
 
 class FlagData(BaseModel):
     archive: bool = Field(default=False)
     auto_update: bool = Field(default=False)
 
 
 class ValueData(BaseModel):
-    datetime_fmt: str = Field(default="%Y-%m-%d %H:%M:%S")
-    excluded_keys: tuple[str, ...] = Field(
+    dt_fmt: str = Field(default="%Y-%m-%d %H:%M:%S")
+    excluded: tuple[str, ...] = Field(
         default=(
             "version",
             "updt",
         )
     )
 
 
@@ -164,17 +156,17 @@
 
 
 class Params(BaseModel, validate_assignment=True):
     stages: dict[str, StageData] = Field(default_factory=dict)
     engine: EngineData = Field(default_factory=EngineData)
 
     @classmethod
-    def from_file(cls, path: Union[str, pathlib.Path]):
+    def from_file(cls, path: Union[str, Path]):
         cls._origin_path = path
-        return cls.model_validate(YamlEnv(path).read())
+        return cls.model_validate(YamlEnvFl(path).read())
 
     @field_validator("stages", mode="before")
     def order_layer(cls, value: dict[str, dict[Any, Any]]):
         for i, k in enumerate(value, start=1):
             value[k] = value[k].copy() | {"layer": i, "alias": k}
         return value
 
@@ -182,15 +174,15 @@
     def stage_final(self) -> str:
         return max(self.stages.items(), key=lambda i: i[1].layer)[0]
 
     @property
     def stage_first(self) -> str:
         return min(self.stages.items(), key=lambda i: i[1].layer)[0]
 
-    def get_stage(self, name: str):
+    def get_stage(self, name: str) -> StageData:
         if name == "base":
             return StageData.model_validate(
                 {
                     "format": "{naming}_{timestamp}",
                     "layer": 0,
                     "alias": "base",
                 }
@@ -205,27 +197,7 @@
             )
         return self.stages[name].model_copy()
 
     def refresh(self, path: Optional[str] = None) -> Params:
         _origin_path = path or self._origin_path
         self.__dict__.update(self.from_file(path=_origin_path).__dict__)
         return self
-
-
-def gt(self: StageData, other: StageData):
-    return self.layer > other.layer
-
-
-class RegisterConfData(BaseModel):
-    author: str = Field(default="unknown")
-    auto_update: bool = Field(default=True)
-    force_exists: bool = Field(default=False)
-
-
-class RegisterMetaData(BaseModel, validate_assignment=True):
-    name: str
-    shortname: str
-    fullname: str
-    data: dict[str, Any]
-    updt: datetime.datetime
-    rtdt: datetime.datetime
-    author: str
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/register.py` & `ddeutil_io-0.1.2/src/ddeutil/io/register.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
 from __future__ import annotations
 
-import datetime
+import logging
 import os
+from datetime import datetime
 from typing import (
     Any,
     Optional,
     TypedDict,
 )
 
 from dateutil.relativedelta import relativedelta
@@ -31,20 +32,25 @@
     Naming,
     VerPackage,
     Version,
     make_const,
     make_group,
 )
 
-from .__base.pathutils import rm
-from .config import ConfFile, OpenFile
+from .__base import rm
+from .config import ConfFl, Fl
 from .exceptions import ConfigArgumentError, ConfigNotFound
 from .models import Params
 
-METADATA: dict[Any, Any] = {}
+METADATA: dict[str, Any] = {}
+
+
+class StageFiles(TypedDict):
+    parse: FormatterGroup
+    file: str
 
 
 CompressConst: ConstantType = make_const(
     name="CompressConst",
     formatter={
         "%g": "gzip",
         "%-g": "gz",
@@ -68,30 +74,26 @@
 
 class BaseRegister:
     """Base Register Object"""
 
     def __init__(
         self,
         name: str,
+        *,
         domain: Optional[str] = None,
-    ):
-        self.name = name
-        self.domain: str = domain or ""
-        self.updt: datetime.datetime = get_date("datetime")
-
-        if domain:
-            self.domain = (
-                domain.replace(os.sep, "/").rstrip("/").lstrip("/").lower()
-            )
-        if any(sep in self.name for sep in {",", "."}):
-            # Raise if name of configuration contain comma (`,`)
-            # or dot (`.`) characters.
+    ) -> None:
+        self.name: str = name
+        self.updt: datetime = get_date("datetime")
+        self.domain: str = (
+            domain.replace(os.sep, "/").strip("/").lower() if domain else ""
+        )
+        if any(sep in self.name for sep in (",", ".")):
             raise ConfigArgumentError(
                 "name",
-                "the name of config should not contain comma or dot characters",
+                "Config name should not contain `,` or `.` char",
             )
 
     @property
     def fullname(self) -> str:
         """Return a configuration fullname, which join `name` and `domain`
         together with domain partition string.
         """
@@ -117,182 +119,149 @@
                 "extension": FileExtensionConst,
                 "version": Version,
                 "timestamp": Datetime,
             }
         )
 
 
-class StageFiles(TypedDict):
-    parse: FormatterGroup
-    file: str
-
-
 class Register(BaseRegister):
     """Register Object that contain configuration loading methods and metadata
     management. This object work with stage input argument, that set all
     properties in the `parameter.yaml` file.
     """
 
     @classmethod
     def reset(
         cls,
         name: str,
-        config: Params,
+        params: Params,
     ) -> Register:
         """Reset all configuration data files that exists in any stage but
         does not do anything in the base stage. This method will use when the
         config name of data was changed and does not use the old name. If the
         name was changed and that config data does not reset,
         the configuration files of this data will exist in any moved stage.
 
-        :param name: str : The fullname of configuration.
-        :param config:
-        :type config: Params
+        :param name: The fullname of configuration.
+        :type name: str
+        :param params:
+        :type params: Params
         """
-
-        # Delete all config file from any stage.
-        for stage in config.stages:
+        for stage in params.stages:
             try:
-                cls(
-                    name,
-                    stage=stage,
-                    config=config,
-                ).remove()
+                cls(name, stage=stage, params=params).remove()
             except ConfigNotFound:
                 continue
-
-        # # Delete data form metadata.
-        # ConfMetadata(
-        #     params.engine.path.metadata,
-        #     name=_name,
-        #     environ=Env(config=params).name,
-        # ).remove()
-        return cls(name, config=config)
+        return cls(name, params=params)
 
     def __init__(
         self,
         name: str,
         stage: Optional[str] = None,
         *,
-        config: Optional[Params] = None,
-        loader: Optional[type[OpenFile]] = None,
+        params: Optional[Params] = None,
+        loader: Optional[type[Fl]] = None,
     ):
         _domain, _name = must_rsplit(concat(name.split()), ":", maxsplit=1)
         super().__init__(name=_name, domain=_domain)
+        if not params:
+            raise NotImplementedError(
+                "This register instance can not do any actions because config "
+                "param does not set."
+            )
         self.stage: str = stage or "base"
-        self.config = config
-        self.loader = loader
+        self.loader: Optional[type[Fl]] = loader
+        self.params: Optional[Params] = params
 
         # Load latest version of data from data lake or data store of
         # configuration files
         self.__data: dict[str, Any] = self.pick(stage=self.stage)
         if not self.__data:
-            _domain_stm: str = (
-                f"with domain {self.domain!r}" if self.domain else ""
-            )
             raise ConfigNotFound(
-                f"Configuration {self.name!r} {_domain_stm} "
-                f"does not found in the {self.stage!r} data lake or data store."
+                f"Config {self.name!r} "
+                f"{f'in domain {self.domain!r} ' if self.domain else ' '}"
+                f"does not exist in stage {self.stage!r}."
             )
 
-        # TODO: Implement meta object
-        self.meta = METADATA
+        self.meta: dict[str, Any] = METADATA
 
-        # Compare data from current stage and latest version in metadata.
+        # NOTE:
+        #   Compare data from current stage and latest version in metadata.
         self.changed: int = self.compare_data(
             target=self.meta.get(self.stage, {})
         )
 
-        # Update metadata if the configuration data does not exist, or
-        # it has any changes.
+        # NOTE:
+        #   Update metadata if the configuration data does not exist, or
+        #   it has any changes.
         if not self.params.engine.flags.auto_update:
-            print("Skip update metadata table/file ...")
+            logging.info("Skip update metadata table/file ...")
         elif self.changed == 99:
-            print(
+            logging.info(
                 f"Configuration data with stage: {self.stage!r} does not "
                 f"exists in metadata ..."
             )
         elif self.changed > 0:
-            print(
+            logging.info(
                 f"Should update metadata because diff level is {self.changed}."
             )
-            _version_stm: str = f"v{str(self.version((self.stage != 'base')))}"
 
     def __hash__(self):
         return hash(
             self.fullname
             + self.stage
-            + f"{self.timestamp:{self.params.engine.values.datetime_fmt}}"
+            + f"{self.timestamp:{self.params.engine.values.dt_fmt}}"
         )
 
     def __str__(self) -> str:
         return f"({self.fullname}, {self.stage})"
 
     def __repr__(self) -> str:
-        _params: list = [f"name={self.fullname!r}"]
-        if self.stage != "base":
-            _params.append(f"stage={self.stage!r}")
-        return f"<{self.__class__.__name__}({', '.join(_params)})>"
+        return (
+            f"<{self.__class__.__name__}(name={self.fullname!r}"
+            f"{f'stage={self.stage!r}' if self.stage != 'base' else ''})>"
+        )
 
     def __eq__(self, other: Register) -> bool:
         if isinstance(other, self.__class__):
             return (
                 self.fullname == other.fullname
                 and self.stage == other.stage
                 and self.timestamp == other.timestamp
             )
         return NotImplemented
 
     def data(self, hashing: bool = False) -> dict[str, Any]:
         """Return the data with the configuration name."""
         _data = self.__data
-        if (self.stage is None) or (self.stage == "base"):
-            _data = merge_dict(
-                {
-                    k: v
-                    for k, v in (self.meta.get(self.stage, {}).items())
-                    if k in self.params.engine.values.excluded_keys
-                },
-                self.__data,
-            )
+        if not self.stage or (self.stage == "base"):
+            _data = {
+                k: v
+                for k, v in (self.meta.get(self.stage, {}).items())
+                if k in self.params.engine.values.excluded
+            } | self.__data
         return (
-            hash_all(
-                _data,
-                exclude=set(self.params.engine.values.excluded_keys),
-            )
+            hash_all(_data, exclude=set(self.params.engine.values.excluded))
             if hashing
             else _data
         )
 
     @property
-    def params(self) -> Params:
-        if self.config is None:
-            raise NotImplementedError(
-                "This register instance can not do any actions because config "
-                "param does not set."
-            )
-        return self.config
-
-    @params.setter
-    def params(self, config: Params) -> None:
-        self.config = config
-
-    @property
-    def timestamp(self) -> datetime.datetime:
+    def timestamp(self) -> datetime:
         """Return the current timestamp value of config data. If timestamp value
         does not exist. this property will return timestamp of initialize.
 
         :return: datetime
         """
         if self.changed > 0:
             return self.updt
         elif _dt := self.data().get("updt"):
-            return datetime.datetime.strptime(
+            return datetime.strptime(
                 _dt,
-                self.params.engine.values.datetime_fmt,
+                self.params.engine.values.dt_fmt,
             )
         return self.updt
 
     def version(self, _next: bool = False) -> VerPackage:
         """Generate version value from the pick method. If version value does
         not exist from configuration data, this property will return the
         default, `v0.0.1`. If the initialization process tracking some change
@@ -306,15 +275,15 @@
             return _vs
         elif self.changed >= 3:
             return _vs.bump_major()
         elif self.changed == 2:
             return _vs.bump_minor()
         return _vs.bump_patch()
 
-    def fmt(self, update: Optional[dict[str, Any]] = None):
+    def fmt(self, update: Optional[dict[str, Any]] = None) -> FormatterGroup:
         return self.fmt_group(
             {
                 "timestamp": self.timestamp,
                 "version": self.version(),
                 **(update or {}),
             }
         )
@@ -333,16 +302,15 @@
             return 99
 
         results = DeepDiff(
             self.data(hashing=True),
             target,
             ignore_order=True,
             exclude_paths={
-                f"root[{key!r}]"
-                for key in self.params.engine.values.excluded_keys
+                f"root[{key!r}]" for key in self.params.engine.values.excluded
             },
         )
         if any(
             _ in results
             for _ in (
                 "dictionary_item_added",
                 "dictionary_item_removed",
@@ -360,15 +328,15 @@
         ):
             return 1
         return 0
 
     def __stage_files(
         self,
         stage: str,
-        loading: ConfFile,
+        loading: ConfFl,
     ) -> dict[int, StageFiles]:
         """Return mapping of StageFiles data."""
         results: dict[int, StageFiles] = {}
         for index, file in enumerate(
             (_f.name for _f in loading.files()),
             start=1,
         ):
@@ -386,23 +354,22 @@
 
     def pick(
         self,
         stage: Optional[str] = None,
         *,
         order: Optional[int] = 1,
         reverse: bool = False,
-    ):
-        # Load data from source
+    ) -> dict[str, Any]:
         if (stage is None) or (stage == "base"):
-            return ConfFile(
+            return ConfFl(
                 path=(self.params.engine.paths.conf / self.domain),
                 open_file=self.loader,
             ).load(name=self.name, order=order)
 
-        loading = ConfFile(
+        loading = ConfFl(
             path=self.params.engine.paths.data / stage,
             compress=self.params.get_stage(stage).rules.compress,
             open_file=self.loader,
         )
 
         if results := self.__stage_files(stage, loading):
             max_data: list = sorted(
@@ -418,97 +385,92 @@
     def move(
         self,
         stage: str,
         *,
         force: bool = False,
         retention: bool = True,
     ) -> Register:
-        """"""
-        loading = ConfFile(
+        """Move file to the target stage."""
+        loading: ConfFl = ConfFl(
             path=self.params.engine.paths.data / stage,
             compress=self.params.get_stage(stage).rules.compress,
             open_file=self.loader,
         )
         if (
             self.compare_data(
                 hash_all(
                     self.pick(stage=stage),
-                    exclude=set(self.params.engine.values.excluded_keys),
+                    exclude=set(self.params.engine.values.excluded),
                 )
             )
             > 0
             or force
         ):
             _filename: str = self.fmt().format(
                 f"{self.params.get_stage(name=stage).format}.json",
             )
-            if os.path.exists(loading.path / _filename):
+            if (loading.path / _filename).exists():
                 # TODO: generate serial number if file exists
-                print(
-                    f"file {_filename!r} already exists in the "
-                    f"{stage!r} stage.",
+                logging.warning(
+                    f"File {_filename!r} already exists in {stage!r} stage."
                 )
-            _dt_fmt: str = self.params.engine.values.datetime_fmt
+            _dt_fmt: str = self.params.engine.values.dt_fmt
             loading.save_stage(
                 path=(loading.path / _filename),
                 data=merge_dict(
                     self.data(),
                     {
                         "updt": f"{self.timestamp:{_dt_fmt}}",
                         "version": f"v{str(self.version())}",
                     },
                 ),
             )
-            # Retention process after move data to the stage successful
+            # NOTE:
+            #   Retention process after move data to the stage successful
             if retention:
                 self.purge(stage=stage)
         else:
-            print(
-                f"Config {self.name!r} can not move {self.stage!r} -> "
-                f"{stage!r} because config data does not any change or "
-                f"does not force moving."
+            logging.warning(
+                f"Config {self.name!r} cannot move {self.stage!r} -> "
+                f"{stage!r} cause the data does not has any change or "
+                f"force moving flag does not set."
             )
         return self.switch(stage=stage)
 
     def switch(self, stage: str) -> Register:
         """Switch instance from old stage to new stage with input argument."""
         return self.__class__(
             name=self.fullname,
             stage=stage,
-            config=self.params,
+            params=self.params,
         )
 
     def purge(self, stage: Optional[str] = None) -> None:
         """Purge configuration files that match with any rules in the stage
         setting.
         """
         _stage: str = stage or self.stage
         if not (_rules := self.params.get_stage(_stage).rules):
             return
-        loading = ConfFile(
+        loading = ConfFl(
             path=self.params.engine.paths.data / stage,
             compress=_rules.compress,
             open_file=self.loader,
         )
         results: dict = self.__stage_files(_stage, loading)
         max_file: FormatterGroup = max(
             results.items(),
             key=lambda x: (x[1]["parse"],),
         )[1]["parse"]
 
         upper_bound: Optional[FormatterGroup] = None
         if _rtt_ts := _rules.timestamp:
-            _metric: Optional[str] = _rules.timestamp_metric
             upper_bound = max_file.adjust(
                 {"timestamp": relativedelta(**_rtt_ts)}
             )
-        # elif _rtt_value := _rules.version:
-        #     upper_bound = max_file.adjust(
-        #         {'version': _rtt_value}
-        #     )
 
         if upper_bound is not None:
             for _, data in filter(
                 lambda x: x[1]["parse"] < upper_bound,
                 results.items(),
             ):
                 _file: str = data["file"]
@@ -539,22 +501,22 @@
             if _stop and (stage == _stop):
                 break
         return _base
 
     def remove(self, stage: Optional[str] = None) -> None:
         """Remove config file from the stage storage.
 
-        :param stage:
+        :param stage: a stage value that want to remove.
         :type stage: Optional[str]
         """
         _stage: str = stage or self.stage
         assert (
             _stage != "base"
         ), "The remove method can not process on the 'base' stage."
-        loading = ConfFile(
+        loading = ConfFl(
             path=self.params.engine.paths.data / _stage,
             open_file=self.loader,
         )
 
         # Remove all files from the stage.
         for _, data in self.__stage_files(_stage, loading).items():
             _file: str = data["file"]
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/io/utils.py` & `ddeutil_io-0.1.2/src/ddeutil/io/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Any,
     Callable,
     Union,
 )
 
 from ddeutil.core import import_string, str2args
 
-from .__base import SettingRegex
+from .__base import RegexConf
 from .exceptions import ConfigArgumentError
 
 
 def map_secret(
     value: Any,
     secrets: dict[str, Any],
 ) -> Union[dict, str, Any]:
@@ -28,15 +28,15 @@
     """
     if isinstance(value, dict):
         return {k: map_secret(value[k], secrets) for k in value}
     elif isinstance(value, (list, tuple)):
         return type(value)([map_secret(i, secrets) for i in value])
     elif not isinstance(value, str):
         return value
-    for search in SettingRegex.RE_SECRETS.finditer(value):
+    for search in RegexConf.RE_SECRETS.finditer(value):
         searches: dict = search.groupdict()
         if "." in (br := searches["braced"]):
             raise ConfigArgumentError(
                 "secrets",
                 f", value {br!r},  should not contain dot ('.') in get value.",
             )
         value: str = value.replace(
@@ -50,15 +50,15 @@
     """Map the function result to configuration data."""
     if isinstance(value, dict):
         return {k: map_function(value[k]) for k in value}
     elif isinstance(value, (list, tuple)):
         return type(value)([map_function(i) for i in value])
     elif not isinstance(value, str):
         return value
-    for search in SettingRegex.RE_FUNCTION.finditer(value):
+    for search in RegexConf.RE_FUNCTION.finditer(value):
         searches: dict = search.groupdict()
         if not callable(_fn := import_string(searches["function"])):
             raise ConfigArgumentError(
                 "@function",
                 f'from function {searches["function"]!r} is not callable.',
             )
         args, kwargs = str2args(searches["arguments"])
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/action.py` & `ddeutil_io-0.1.2/src/ddeutil/node/action.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/apps.py` & `ddeutil_io-0.1.2/src/ddeutil/node/apps.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/base/converter.py` & `ddeutil_io-0.1.2/src/ddeutil/node/base/converter.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/base/loader.py` & `ddeutil_io-0.1.2/src/ddeutil/node/base/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     clear_cache,
     getdot,
     hasdot,
     import_string,
     setdot,
 )
 from ddeutil.io import Params, Register
-from ddeutil.io.__base import YamlEnv
+from ddeutil.io.__base import YamlEnvFl
 from ddeutil.io.utils import map_func_to_str
 from fmtutil import Datetime
 
 from ..exceptions import ConfigArgumentError, ConfigNotFound
 
-YamlEnvQuote = YamlEnv
+YamlEnvQuote = YamlEnvFl
 YamlEnvQuote.prepare = staticmethod(lambda x: urllib.parse.quote_plus(str(x)))
 
 
 class LoaderData(TypedDict):
     name: str
     fullname: str
     data: dict[str, Any]
@@ -71,29 +71,29 @@
             base and auto deploy to `cls.load_stage` again if it set be True.
         :type refresh: bool
         :param params:
         """
         if refresh:
             _regis: Register = Register(
                 name=name,
-                config=config,
+                params=config,
                 loader=YamlEnvQuote,
             ).deploy(stop=config.stage_final)
         else:
             try:
                 _regis: Register = Register(
                     name=name,
                     stage=config.stage_final,
-                    config=config,
+                    params=config,
                     loader=YamlEnvQuote,
                 )
             except ConfigNotFound:
                 _regis: Register = Register(
                     name=name,
-                    config=config,
+                    params=config,
                     loader=YamlEnvQuote,
                 ).deploy(stop=config.stage_final)
 
         return cls(
             data={
                 "name": _regis.name,
                 "fullname": _regis.fullname,
@@ -136,26 +136,14 @@
                 (
                     f"{self.name!r} does not starts with the "
                     f"{self.__class__.__name__} prefix value "
                     f"{self.load_prefixes!r}."
                 ),
             )
 
-    # @cached_property
-    # def type(self) -> ObjectType:
-    #     """Return object type which implement in `config_object` key."""
-    #     if (_typ := self._ld_regis["data"].get("type")) is None:
-    #         logger.warning(
-    #             f"the 'type' value: {_typ} does not exists in config data."
-    #         )
-    #         # TODO: add default type from prefix name.
-    #         raise ValueError
-    #     _obj_prefix: str = params.engine.path.object
-    #     return import_string(f"{_obj_prefix}.{_typ}")
-
     @cached_property
     def __map_data(self) -> dict[str, Any]:
         """Return configuration data without key in the excluded key set."""
         _data: dict[str, Any] = self.__data["data"].copy()
         _results: dict[str, Any] = {
             k: _data[k] for k in _data if k not in self.data_excluded
         }
@@ -212,14 +200,13 @@
             f"This {self.__class__.__name__} object does not pass data from "
             f"catalog that support refresh method."
         )
 
     @cached_property
     def type(self):
         """Return object type which implement in `config_object` key."""
-        if (_typ := self.data.get("type")) is None:
-            # TODO: add default type from prefix name.
+        if not (_typ := self.data.get("type")):
             raise ValueError(
                 f"the 'type' value: {_typ} does not exists in config data."
             )
         _obj_prefix: str = "ddeutil.node"
         return import_string(f"{_obj_prefix}.{_typ}")
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/base/models.py` & `ddeutil_io-0.1.2/src/ddeutil/node/base/models.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/connection.py` & `ddeutil_io-0.1.2/src/ddeutil/node/connection.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/datasets_legacy.py` & `ddeutil_io-0.1.2/src/ddeutil/node/datasets_legacy.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/exceptions.py` & `ddeutil_io-0.1.2/src/ddeutil/node/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/loader.py` & `ddeutil_io-0.1.2/src/ddeutil/node/loader.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/node.py` & `ddeutil_io-0.1.2/src/ddeutil/node/node.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/schedule.py` & `ddeutil_io-0.1.2/src/ddeutil/node/schedule.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/vendors/boto.py` & `ddeutil_io-0.1.2/src/ddeutil/node/vendors/boto.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil/node/vendors/sftp.py` & `ddeutil_io-0.1.2/src/ddeutil/node/vendors/sftp.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.1/src/ddeutil_io.egg-info/PKG-INFO` & `ddeutil_io-0.1.2/src/ddeutil_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
@@ -60,17 +60,17 @@
 
 ### Config
 
 The **Config Object** is the file system handler object.
 
 ```python
 from pathlib import Path
-from ddeutil.io.config import ConfFile
+from ddeutil.io.config import ConfFl
 
-config: ConfFile = ConfFile(path=Path(), compress="gzip")
+config: ConfFl = ConfFl(path=Path('./file.gz.yaml'), compress="gzip")
 ```
 
 ### Register
 
 The **Register Object** is the metadata generator object for the config data.
 If you passing name and configs to this object, it will find the config name
 in any stage storage and generate its metadata to you.
@@ -83,14 +83,15 @@
     name='examples:conn_data_local_file',
     config=Params.model_validate({
         "stages": {
           "raw": {"format": "{naming:%s}.{timestamp:%Y%m%d_%H%M%S}"},
         },
     }),
 )
+registry.move(stage="raw")
 ```
 
 ### Link
 
 ```yaml
 connection_local_file_landing:
     type: "connection.LocalSystem"
```

### Comparing `ddeutil_io-0.1.1/src/ddeutil_io.egg-info/SOURCES.txt` & `ddeutil_io-0.1.2/src/ddeutil_io.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 pyproject.toml
 src/ddeutil/io/__about__.py
 src/ddeutil/io/__init__.py
 src/ddeutil/io/config.py
 src/ddeutil/io/exceptions.py
 src/ddeutil/io/models.py
 src/ddeutil/io/register.py
-src/ddeutil/io/tracking.py
 src/ddeutil/io/utils.py
 src/ddeutil/io/__base/__init__.py
 src/ddeutil/io/__base/__regex.py
 src/ddeutil/io/__base/files.py
-src/ddeutil/io/__base/pathutils.py
 src/ddeutil/io/__base/utils.py
 src/ddeutil/node/__init__.py
 src/ddeutil/node/action.py
 src/ddeutil/node/apps.py
 src/ddeutil/node/connection.py
 src/ddeutil/node/datasets.py
 src/ddeutil/node/datasets_legacy.py
@@ -34,16 +32,16 @@
 src/ddeutil/node/vendors/sftp.py
 src/ddeutil/node/vendors/vpn.py
 src/ddeutil_io.egg-info/PKG-INFO
 src/ddeutil_io.egg-info/SOURCES.txt
 src/ddeutil_io.egg-info/dependency_links.txt
 src/ddeutil_io.egg-info/requires.txt
 src/ddeutil_io.egg-info/top_level.txt
-tests/test_base_dir_open.py
+tests/test_base_csv.py
+tests/test_base_dir.py
 tests/test_base_env.py
-tests/test_base_file_csv.py
-tests/test_base_file_open.py
+tests/test_base_file.py
 tests/test_base_file_yaml.py
 tests/test_config_file.py
 tests/test_config_sqlite.py
 tests/test_models.py
 tests/test_register.py
```

### Comparing `ddeutil_io-0.1.1/tests/test_base_dir_open.py` & `ddeutil_io-0.1.2/tests/test_base_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 
     def setUp(self) -> None:
         self.encoding = "utf-8"
 
     def test_open_dir_common_zip(self):
         data_dir = pathlib.Path(self.data_path)
 
-        opd = fl.OpenDir(
+        opd = fl.Dir(
             path=pathlib.Path(f"{self.root_path}/test_common_dir.zip"),
             compress="zip",
         )
         with opd.open(mode="w") as d:
             for data in data_dir.rglob("*"):
                 d.write(filename=data, arcname=data.relative_to(data_dir))
 
     def test_open_dir_common_tar(self):
         data_dir = pathlib.Path(self.data_path)
 
-        opd = fl.OpenDir(
+        opd = fl.Dir(
             path=pathlib.Path(f"{self.root_path}/test_common_dir.tar.gz"),
             compress="tar",
         )
         with opd.open(mode="w") as d:
             for data in data_dir.rglob("*"):
                 d.add(name=data, arcname=data.relative_to(data_dir))
```

### Comparing `ddeutil_io-0.1.1/tests/test_base_env.py` & `ddeutil_io-0.1.2/tests/test_base_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,45 @@
-import os
 import shutil
-import unittest
+from collections.abc import Generator
+from pathlib import Path
 from textwrap import dedent
 
 import ddeutil.io.__base as bfl
+import pytest
 
 
-class EnvTestCase(unittest.TestCase):
-    root_path: str
-
-    @classmethod
-    def setUpClass(cls) -> None:
-        _root_path: str = os.path.dirname(os.path.abspath(__file__)).replace(
-            os.sep, "/"
+@pytest.fixture(scope="module")
+def env_path(test_path) -> Generator[Path, None, None]:
+    this_path: Path = test_path / "env"
+    this_path.mkdir(parents=True, exist_ok=True)
+
+    yield this_path
+
+    shutil.rmtree(this_path)
+
+
+def test_env(env_path):
+    env_path: Path = env_path / ".env"
+
+    with open(env_path, mode="w", encoding="utf-8") as f:
+        f.write(
+            dedent(
+                """
+    TEST=This is common value test
+    # Comment this line ...
+    COMMENT_TEST='This is common value test'  # This is inline comment
+    QUOTE='single quote'
+    DOUBLE_QUOTE="double quote"
+    PASSING=${DOUBLE_QUOTE}
+    UN_PASSING='${DOUBLE_QUOTE}'
+    """
+            ).strip()
         )
-        os.makedirs(f"{_root_path}/env", exist_ok=True)
-
-        cls.root_path: str = f"{_root_path}/env"
 
-    def setUp(self) -> None:
-        self.maxDiff = None
-        self.env_str = dedent(
-            """
-        TEST=This is common value test
-        # Comment this line ...
-        COMMENT_TEST='This is common value test'  # This is inline comment
-        QUOTE='single quote'
-        DOUBLE_QUOTE="double quote"
-        PASSING=${DOUBLE_QUOTE}
-        UN_PASSING='${DOUBLE_QUOTE}'
-        """
-        ).strip()
-
-        self.env_data = {
-            "TEST": "This is common value test",
-            "COMMENT_TEST": "This is common value test",
-            "QUOTE": "single quote",
-            "DOUBLE_QUOTE": "double quote",
-            "PASSING": "double quote",
-            "UN_PASSING": "${DOUBLE_QUOTE}",
-        }
-
-    def test_env(self):
-        env_path: str = f"{self.root_path}/.env"
-
-        with open(env_path, mode="w", encoding="utf-8") as f:
-            f.write(self.env_str)
-
-        data = bfl.Env(path=env_path).read(update=False)
-
-        self.assertDictEqual(self.env_data, data)
-
-    @classmethod
-    def tearDownClass(cls) -> None:
-        shutil.rmtree(cls.root_path)
+    assert {
+        "TEST": "This is common value test",
+        "COMMENT_TEST": "This is common value test",
+        "QUOTE": "single quote",
+        "DOUBLE_QUOTE": "double quote",
+        "PASSING": "double quote",
+        "UN_PASSING": "${DOUBLE_QUOTE}",
+    } == bfl.EnvFl(path=env_path).read(update=False)
```

### Comparing `ddeutil_io-0.1.1/tests/test_base_file_open.py` & `ddeutil_io-0.1.2/tests/test_base_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,246 +1,233 @@
-import os
-import pathlib
 import shutil
-import unittest
+from collections.abc import Generator
+from pathlib import Path
 
 import ddeutil.io.__base.files as fl
 import ddeutil.io.__base.utils as utils
+import pytest
 
 
-class OpenFileTestCase(unittest.TestCase):
-    root_path: str
+@pytest.fixture(scope="module")
+def openfile_path(test_path) -> Generator[Path, None, None]:
+    this_path: Path = test_path / "open_file"
+    this_path.mkdir(parents=True, exist_ok=True)
 
-    @classmethod
-    def setUpClass(cls) -> None:
-        _root_path: str = os.path.dirname(os.path.abspath(__file__)).replace(
-            os.sep, "/"
-        )
-        os.makedirs(f"{_root_path}/open_file", exist_ok=True)
+    yield this_path
 
-        cls.root_path: str = f"{_root_path}/open_file"
+    shutil.rmtree(this_path)
 
-    def setUp(self) -> None:
-        self.encoding = "utf-8"
 
-    def test_open_file_common(self):
-        opf = fl.OpenFile(
-            path=pathlib.Path(f"{self.root_path}/test_common_file.text"),
-            encoding="utf-8",
-        )
-        with opf.open(mode="w") as f:
-            f.write("Write data with common file in normal mode")
+@pytest.fixture(scope="module")
+def encoding() -> str:
+    return "utf-8"
 
-        with opf.open(mode="r") as f:
-            rs = f.read()
 
-        self.assertEqual("Write data with common file in normal mode", rs)
+def test_open_file_common(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_common_file.text",
+        encoding=encoding,
+    )
+    with opf.open(mode="w") as f:
+        f.write("Write data with common file in normal mode")
 
-    def test_open_file_common_append(self):
-        opf = fl.OpenFile(
-            path=pathlib.Path(f"{self.root_path}/test_common_file_append.text"),
-            encoding="utf-8",
-        )
-        with opf.open(mode="w") as f:
-            f.write(
-                utils.add_newline(
-                    "Write data with common file append in normal mode",
-                )
-            )
+    with opf.open(mode="r") as f:
+        rs = f.read()
 
-        with opf.open(mode="a", newline="\n") as f:
-            f.write("Write another line in the same file")
+    assert "Write data with common file in normal mode" == rs
 
-        with opf.open(mode="r") as f:
-            rs = f.read()
 
-        self.assertEqual(
-            (
-                "Write data with common file append in normal mode\n"
-                "Write another line in the same file"
-            ),
-            rs,
+def test_open_file_common_append(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_common_file_append.text",
+        encoding=encoding,
+    )
+    with opf.open(mode="w") as f:
+        f.write(
+            utils.add_newline(
+                "Write data with common file append in normal mode",
+            )
         )
 
-    def test_open_file_common_gzip(self):
-        opf = fl.OpenFile(
-            path=pathlib.Path(f"{self.root_path}/test_common_file.gz.text"),
-            encoding="utf-8",
-            compress="gzip",
-        )
-        with opf.open(mode="w") as f:
-            f.write("Write data with common file in gzip mode")
+    with opf.open(mode="a", newline="\n") as f:
+        f.write("Write another line in the same file")
 
-        with opf.open(mode="r") as f:
-            rs = f.read()
+    with opf.open(mode="r") as f:
+        rs = f.read()
 
-        self.assertEqual("Write data with common file in gzip mode", rs)
+    assert (
+        "Write data with common file append in normal mode\n"
+        "Write another line in the same file"
+    ) == rs
 
-    def test_open_file_common_xz(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_common_file.xz.text",
-            encoding="utf-8",
-            compress="xz",
-        )
-        with opf.open(mode="w") as f:
-            f.write("Write data with common file in xz mode")
 
-        with opf.open(mode="r") as f:
-            rs = f.read()
+def test_open_file_common_gzip(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_common_file.gz.text",
+        encoding=encoding,
+        compress="gzip",
+    )
+    with opf.open(mode="w") as f:
+        f.write("Write data with common file in gzip mode")
 
-        self.assertEqual("Write data with common file in xz mode", rs)
+    with opf.open(mode="r") as f:
+        rs = f.read()
 
-    def test_open_file_common_bz2(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_common_file.bz2.text",
-            encoding="utf-8",
-            compress="bz2",
-        )
-        with opf.open(mode="w") as f:
-            f.write("Write data with common file in bz2 mode")
+    assert "Write data with common file in gzip mode" == rs
 
-        with opf.open(mode="r") as f:
-            rs = f.read()
 
-        self.assertEqual("Write data with common file in bz2 mode", rs)
+def test_open_file_common_xz(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_common_file.xz.text",
+        encoding=encoding,
+        compress="xz",
+    )
+    with opf.open(mode="w") as f:
+        f.write("Write data with common file in xz mode")
 
-    def test_open_file_binary(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_binary_file.text",
-            encoding="utf-8",
-        )
-        with opf.open(mode="wb") as f:
-            f.write(b"Write data with binary file in normal mode")
+    with opf.open(mode="r") as f:
+        rs = f.read()
 
-        with opf.open(mode="rb") as f:
-            rs = f.read()
+    assert "Write data with common file in xz mode" == rs
 
-        self.assertEqual(b"Write data with binary file in normal mode", rs)
 
-    def test_open_file_binary_gzip(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_binary_file.gz.text",
-            encoding="utf-8",
-            compress="gzip",
-        )
-        with opf.open(mode="wb") as f:
-            f.write(b"Write data with binary file in gzip mode")
+def test_open_file_common_bz2(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_common_file.bz2.text",
+        encoding=encoding,
+        compress="bz2",
+    )
+    with opf.open(mode="w") as f:
+        f.write("Write data with common file in bz2 mode")
 
-        with opf.open(mode="rb") as f:
-            rs = f.read()
+    with opf.open(mode="r") as f:
+        rs = f.read()
 
-        self.assertEqual(b"Write data with binary file in gzip mode", rs)
+    assert "Write data with common file in bz2 mode" == rs
 
-    def test_open_file_binary_xz(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_binary_file.xz.text",
-            encoding="utf-8",
-            compress="xz",
-        )
-        with opf.open(mode="wb") as f:
-            f.write(b"Write data with binary file in xz mode")
 
-        with opf.open(mode="rb") as f:
-            rs = f.read()
+def test_open_file_binary(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_binary_file.text",
+        encoding=encoding,
+    )
+    with opf.open(mode="wb") as f:
+        f.write(b"Write data with binary file in normal mode")
 
-        self.assertEqual(b"Write data with binary file in xz mode", rs)
+    with opf.open(mode="rb") as f:
+        rs = f.read()
 
-    def test_open_file_binary_bz2(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_binary_file.bz2.text",
-            encoding="utf-8",
-            compress="bz2",
-        )
-        with opf.open(mode="wb") as f:
-            f.write(b"Write data with binary file in bz2 mode")
+    assert b"Write data with binary file in normal mode" == rs
 
-        with opf.open(mode="rb") as f:
-            rs = f.read()
 
-        self.assertEqual(b"Write data with binary file in bz2 mode", rs)
+def test_open_file_binary_gzip(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_binary_file.gz.text",
+        encoding=encoding,
+        compress="gzip",
+    )
+    with opf.open(mode="wb") as f:
+        f.write(b"Write data with binary file in gzip mode")
 
-    @classmethod
-    def tearDownClass(cls) -> None:
-        shutil.rmtree(cls.root_path)
+    with opf.open(mode="rb") as f:
+        rs = f.read()
 
+    assert b"Write data with binary file in gzip mode" == rs
 
-class OpenFileMemoryTestCase(unittest.TestCase):
-    root_path: str
 
-    @classmethod
-    def setUpClass(cls) -> None:
-        _root_path: str = os.path.dirname(os.path.abspath(__file__)).replace(
-            os.sep, "/"
-        )
-        os.makedirs(f"{_root_path}/open_file_mem", exist_ok=True)
+def test_open_file_binary_xz(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_binary_file.xz.text",
+        encoding=encoding,
+        compress="xz",
+    )
+    with opf.open(mode="wb") as f:
+        f.write(b"Write data with binary file in xz mode")
 
-        cls.root_path: str = f"{_root_path}/open_file_mem"
+    with opf.open(mode="rb") as f:
+        rs = f.read()
 
-    def setUp(self) -> None:
-        self.encoding = "utf-8"
+    assert b"Write data with binary file in xz mode" == rs
 
-    def test_open_file_mem_common(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_common_mem_file.text",
-            encoding="utf-8",
-        )
-        with opf.mopen(mode="w") as f:
-            f.write("Write data with common file in normal mode on memory")
 
-        with opf.mopen(mode="r") as f:
-            rs = f.read()
+def test_open_file_binary_bz2(openfile_path, encoding):
+    opf = fl.Fl(
+        path=openfile_path / "test_binary_file.bz2.text",
+        encoding=encoding,
+        compress="bz2",
+    )
+    with opf.open(mode="wb") as f:
+        f.write(b"Write data with binary file in bz2 mode")
 
-        self.assertEqual(
-            b"Write data with common file in normal mode on memory", rs
-        )
+    with opf.open(mode="rb") as f:
+        rs = f.read()
 
-    def test_open_file_mem_common_gzip(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_common_mem_file.gz.text",
-            encoding="utf-8",
-            compress="gzip",
-        )
-        with opf.mopen(mode="w") as f:
-            f.write("Write data with common file in gzip mode on memory")
+    assert b"Write data with binary file in bz2 mode" == rs
 
-        with opf.mopen(mode="r") as f:
-            rs = opf.compress_lib.decompress(f.read())
 
-        self.assertEqual(
-            b"Write data with common file in gzip mode on memory", rs
-        )
+@pytest.fixture(scope="module")
+def openfile_mem_path(test_path) -> Generator[Path, None, None]:
+    this_path: Path = test_path / "open_file_mem"
+    this_path.mkdir(parents=True, exist_ok=True)
 
-    def test_open_file_mem_common_xz(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_common_mem_file.xz.text",
-            encoding="utf-8",
-            compress="xz",
-        )
-        with opf.mopen(mode="w") as f:
-            f.write("Write data with common file in xz mode on memory")
+    yield this_path
 
-        with opf.mopen(mode="r") as f:
-            rs = opf.compress_lib.decompress(f.read())
+    shutil.rmtree(this_path)
 
-        self.assertEqual(
-            b"Write data with common file in xz mode on memory", rs
-        )
 
-    def test_open_file_mem_common_bz2(self):
-        opf = fl.OpenFile(
-            path=f"{self.root_path}/test_common_mem_file.bz2.text",
-            encoding="utf-8",
-            compress="bz2",
-        )
-        with opf.mopen(mode="w") as f:
-            f.write("Write data with common file in bz2 mode on memory")
+def test_open_file_mem_common(openfile_mem_path, encoding):
+    opf = fl.Fl(
+        path=openfile_mem_path / "test_common_mem_file.text",
+        encoding=encoding,
+    )
+    with opf.mopen(mode="w") as f:
+        f.write("Write data with common file in normal mode on memory")
 
-        with opf.mopen(mode="r") as f:
-            rs = opf.compress_lib.decompress(f.read())
+    with opf.mopen(mode="r") as f:
+        rs = f.read()
 
-        self.assertEqual(
-            b"Write data with common file in bz2 mode on memory", rs
-        )
+    assert b"Write data with common file in normal mode on memory" == rs
+
+
+def test_open_file_mem_common_gzip(openfile_mem_path, encoding):
+    opf = fl.Fl(
+        path=openfile_mem_path / "test_common_mem_file.gz.text",
+        encoding=encoding,
+        compress="gzip",
+    )
+    with opf.mopen(mode="w") as f:
+        f.write("Write data with common file in gzip mode on memory")
+
+    with opf.mopen(mode="r") as f:
+        rs = fl.compress_lib("gzip").decompress(f.read())
+
+    assert b"Write data with common file in gzip mode on memory" == rs
+
+
+def test_open_file_mem_common_xz(openfile_mem_path, encoding):
+    opf = fl.Fl(
+        path=openfile_mem_path / "test_common_mem_file.xz.text",
+        encoding=encoding,
+        compress="xz",
+    )
+    with opf.mopen(mode="w") as f:
+        f.write("Write data with common file in xz mode on memory")
+
+    with opf.mopen(mode="r") as f:
+        rs = fl.compress_lib("xz").decompress(f.read())
+
+    assert b"Write data with common file in xz mode on memory" == rs
+
+
+def test_open_file_mem_common_bz2(openfile_mem_path, encoding):
+    opf = fl.Fl(
+        path=openfile_mem_path / "test_common_mem_file.bz2.text",
+        encoding=encoding,
+        compress="bz2",
+    )
+    with opf.mopen(mode="w") as f:
+        f.write("Write data with common file in bz2 mode on memory")
+
+    with opf.mopen(mode="r") as f:
+        rs = fl.compress_lib("bz2").decompress(f.read())
 
-    @classmethod
-    def tearDownClass(cls) -> None:
-        shutil.rmtree(cls.root_path)
+    assert b"Write data with common file in bz2 mode on memory" == rs
```

### Comparing `ddeutil_io-0.1.1/tests/test_base_file_yaml.py` & `ddeutil_io-0.1.2/tests/test_base_file_yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,27 @@
                 }
             }
         }
 
     def test_write_yaml_file_with_safe_mode(self):
         yaml_path: str = f"{self.root_path}/test_write_file.yaml"
 
-        fl.Yaml(path=yaml_path).write(self.yaml_data)
+        fl.YamlFl(path=yaml_path).write(self.yaml_data)
 
         self.assertTrue(os.path.exists(yaml_path))
 
         os.remove(yaml_path)
 
     def test_read_yaml_file_with_safe_mode(self):
         yaml_path: str = f"{self.root_path}/test_read_file.yaml"
 
         with open(yaml_path, mode="w", encoding="utf-8") as f:
             yaml.dump(yaml.safe_load(self.yaml_str), f)
 
-        data = fl.Yaml(path=yaml_path).read()
+        data = fl.YamlFl(path=yaml_path).read()
         self.assertDictEqual(self.yaml_data, data)
 
         os.remove(yaml_path)
 
 
 class YamlEnvFileTestCase(unittest.TestCase):
     @classmethod
@@ -97,28 +97,28 @@
         yaml_path: str = f"{self.root_path}/test_read_file_env.yaml"
 
         with open(yaml_path, mode="w", encoding="utf-8") as f:
             yaml.dump(yaml.safe_load(self.yaml_str), f)
 
         os.environ["DEMO_ENV_VALUE"] = "demo"
 
-        data = fl.YamlEnv(path=yaml_path).read()
+        data = fl.YamlEnvFl(path=yaml_path).read()
         self.assertDictEqual(self.yaml_data, data)
 
         os.remove(yaml_path)
 
     def test_read_yaml_file_with_safe_mode_and_prepare(self):
         yaml_path: str = f"{self.root_path}/test_read_file_env_prepare.yaml"
 
         with open(yaml_path, mode="w", encoding="utf-8") as f:
             yaml.dump(yaml.safe_load(self.yaml_str), f)
 
         os.environ["DEMO_ENV_VALUE"] = "demo"
 
-        yml_loader = fl.YamlEnv(path=yaml_path)
+        yml_loader = fl.YamlEnvFl(path=yaml_path)
         yml_loader.prepare = lambda x: f"{x}!!"
         data = yml_loader.read()
         self.assertDictEqual(
             {
                 "main_key": {
                     "sub_key": {
                         "key01": "test demo!! value",
@@ -141,15 +141,15 @@
         with open(yaml_path, mode="w", encoding="utf-8") as f:
             yaml.dump(yaml.safe_load(self.yaml_str), f)
 
         os.environ["DEMO_ENV_VALUE"] = "P@ssW0rd"
 
         import urllib.parse
 
-        yml_loader = fl.YamlEnv
+        yml_loader = fl.YamlEnvFl
         yml_loader.prepare = staticmethod(
             lambda x: urllib.parse.quote_plus(str(x))
         )
         data = yml_loader(path=yaml_path).read()
         self.assertDictEqual(
             {
                 "main_key": {
```

### Comparing `ddeutil_io-0.1.1/tests/test_config_file.py` & `ddeutil_io-0.1.2/tests/test_config_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,62 +6,57 @@
 
 
 @pytest.fixture(scope="module")
 def target_path(test_path) -> Path:
     return test_path / "conf_file_temp"
 
 
-@pytest.fixture(scope="module")
-def demo_path(test_path) -> Path:
-    return test_path / "examples" / "conf" / "demo"
-
-
 def test_base_conf_read_file(demo_path, target_path):
-    bcf = conf.BaseConfFile(demo_path)
+    bcf = conf.BaseConfFl(demo_path)
 
     assert {
         "alias": "conn_local_file",
-        "endpoint": "file:///N%2FA/tests/examples/dummy",
+        "endpoint": "file:///null/tests/examples/dummy",
         "type": "connection.LocalFileStorage",
     } == bcf.load(name="conn_local_file")
 
     bcf.move(
         "demo_01_connections.yaml",
         destination=target_path / "demo_01_connections.yaml",
     )
 
-    bcf_temp = conf.BaseConfFile(target_path)
+    bcf_temp = conf.BaseConfFl(target_path)
     assert {
         "alias": "conn_local_file",
-        "endpoint": "file:///N%2FA/tests/examples/dummy",
+        "endpoint": "file:///null/tests/examples/dummy",
         "type": "connection.LocalFileStorage",
     } == bcf_temp.load(name="conn_local_file")
 
     assert (target_path / "demo_01_connections.yaml").exists()
 
     if target_path.exists():
         shutil.rmtree(target_path)
 
 
 def test_conf_read_file(demo_path, target_path):
-    cf = conf.ConfFile(demo_path)
+    cf = conf.ConfFl(demo_path)
     cf.move(
         path="demo_01_connections.yaml",
         destination=target_path / "demo_01_connections.yaml",
     )
 
     _stage_path = target_path / "demo_01_connections_stage.json"
 
     cf.create(path=_stage_path)
     assert _stage_path.exists()
     cf.save_stage(path=_stage_path, data=cf.load("conn_local_file"))
 
     assert {
         "alias": "conn_local_file",
-        "endpoint": "file:///N%2FA/tests/examples/dummy",
+        "endpoint": "file:///null/tests/examples/dummy",
         "type": "connection.LocalFileStorage",
     } == cf.load_stage(path=_stage_path)
 
     cf.save_stage(
         path=_stage_path,
         data={"temp_additional": cf.load("conn_local_file")},
         merge=True,
@@ -70,13 +65,13 @@
     cf.remove_stage(
         path=_stage_path,
         name="temp_additional",
     )
 
     assert {
         "alias": "conn_local_file",
-        "endpoint": "file:///N%2FA/tests/examples/dummy",
+        "endpoint": "file:///null/tests/examples/dummy",
         "type": "connection.LocalFileStorage",
     } == cf.load_stage(path=_stage_path)
 
     if target_path.exists():
         shutil.rmtree(target_path)
```

### Comparing `ddeutil_io-0.1.1/tests/test_config_sqlite.py` & `ddeutil_io-0.1.2/tests/test_config_sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 from pathlib import Path
 
 import ddeutil.io.config as conf
 import pytest
 
 
 @pytest.fixture(scope="module")
-def target_path(test_path) -> Path:
+def sqlite_path(test_path) -> Path:
     return test_path / "conf_sqlite_temp"
 
 
 @pytest.fixture(scope="module")
 def demo_path(test_path) -> Path:
     return test_path / "examples" / "conf" / "demo"
 
 
-def test_base_conf_read_file(demo_path, target_path):
+def test_base_conf_read_file(demo_path, sqlite_path):
     _schemas: dict[str, str] = {
         "name": "varchar(256) primary key",
         "shortname": "varchar(64) not null",
         "fullname": "varchar(256) not null",
         "data": "json not null",
         "updt": "datetime not null",
         "rtdt": "datetime not null",
         "author": "varchar(512) not null",
     }
 
-    bc_sql = conf.ConfSQLite(target_path)
+    bc_sql = conf.ConfSQLite(sqlite_path)
     bc_sql.create(table="demo.db/temp_table", schemas=_schemas)
 
-    assert (target_path / "demo.db").exists()
+    assert (sqlite_path / "demo.db").exists()
 
     _data = {
         "conn_local_data_landing": {
             "name": "conn_local_data_landing",
             "shortname": "cldl",
             "fullname": "conn_local_data_landing",
             "data": {"first_row": {"key": "value"}},
@@ -42,9 +42,9 @@
             "author": "unknown",
         },
     }
 
     bc_sql.save_stage(table="demo.db/temp_table", data=_data)
 
     assert _data == bc_sql.load_stage(table="demo.db/temp_table")
-    if target_path.exists():
-        shutil.rmtree(target_path)
+    if sqlite_path.exists():
+        shutil.rmtree(sqlite_path)
```

### Comparing `ddeutil_io-0.1.1/tests/test_register.py` & `ddeutil_io-0.1.2/tests/test_register.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,15 @@
 
 @pytest.fixture(scope="module")
 def target_path(test_path) -> Path:
     return test_path / "conf_file_temp"
 
 
 @pytest.fixture(scope="module")
-def root_path(test_path) -> Path:
-    return test_path.parent.parent
-
-
-@pytest.fixture(scope="module")
-def param_config(test_path, root_path) -> Params:
+def params(test_path, root_path) -> Params:
     return Params.model_validate(
         {
             "engine": {
                 "paths": {
                     "conf": test_path / "examples/conf",
                     "data": root_path / "data",
                     "archive": root_path / "/data/.archive",
@@ -31,52 +26,50 @@
                 "raw": {"format": "{naming:%s}.{timestamp:%Y%m%d_%H%M%S}"},
                 "persisted": {"format": "{naming:%s}.{version:v%m.%n.%c}"},
             },
         }
     )
 
 
-def test_register_init(param_config):
-    register = rgt.Register(
-        name="demo:conn_local_file",
-        config=param_config,
-    )
+def test_register_init(params: Params):
+    register = rgt.Register(name="demo:conn_local_file", params=params)
 
     assert "base" == register.stage
     assert {
         "alias": "conn_local_file",
         "type": "connection.LocalFileStorage",
-        "endpoint": "file:///N%2FA/tests/examples/dummy",
+        "endpoint": "file:///null/tests/examples/dummy",
     } == register.data()
-
     assert {
         "alias": "62d877a16819c672578d7bded7f5903c",
         "type": "cece9f1b3f4791a04ec3d695cb5ba1a9",
-        "endpoint": "853dd5b0a2a4c58d8be2babdff0d7da8",
+        "endpoint": "0d1db48bb2425db014fc66734508098f",
     } == register.data(hashing=True)
 
     print("\nChange compare from metadata:", register.changed)
+    assert register.changed == 99
 
     rsg_raw = register.move(stage="raw")
 
-    assert "base" == register.stage
-    assert "raw" == rsg_raw.stage
-
+    assert register.stage != rsg_raw.stage
     assert (
         "62d877a16819c672578d7bded7f5903c"
         == rsg_raw.data(hashing=True)["alias"]
     )
 
-    rgt.Register.reset(
-        name="demo:conn_local_file",
-        config=param_config,
+    rsg_persisted = rsg_raw.move(stage="persisted")
+    assert rsg_raw.stage != rsg_persisted.stage
+    assert (
+        "62d877a16819c672578d7bded7f5903c"
+        == rsg_persisted.data(hashing=True)["alias"]
     )
+    rgt.Register.reset(name="demo:conn_local_file", params=params)
 
 
-def test_register_without_config():
+def test_register_without_params():
     try:
         rgt.Register(name="demo:conn_local_file")
     except NotImplementedError as err:
         assert (
             "This register instance can not do any actions because config "
             "param does not set."
         ) == str(err)
```

