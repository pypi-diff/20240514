# Comparing `tmp/biomedisa-2024.5.17.tar.gz` & `tmp/biomedisa-2024.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedisa-2024.5.17.tar", last modified: Tue May 14 05:10:14 2024, max compression
+gzip compressed data, was "biomedisa-2024.5.18.tar", last modified: Tue May 14 05:14:07 2024, max compression
```

## Comparing `biomedisa-2024.5.17.tar` & `biomedisa-2024.5.18.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:10:14.023391 biomedisa-2024.5.17/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/LICENSE
--rw-r--r--   0 philipp   (1000) philipp   (1000)    11677 2024-05-14 05:10:14.023391 biomedisa-2024.5.17/PKG-INFO
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11069 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/README.md
--rw-rw-r--   0 philipp   (1000) philipp   (1000)      664 2024-05-14 05:10:04.000000 biomedisa-2024.5.17/pyproject.toml
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-14 05:10:14.023391 biomedisa-2024.5.17/setup.cfg
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:10:14.019391 biomedisa-2024.5.17/src/
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:10:14.019391 biomedisa-2024.5.17/src/biomedisa/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1690 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/__main__.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:10:14.023391 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/DataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-02-14 23:44:22.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/DataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/PredictDataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2023-12-07 02:51:22.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18131 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/active_contour.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:10:14.023391 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/assd.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32401 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/biomedisa_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13329 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/create_slices.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    23894 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/crop_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/curvop_numba.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     8989 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/django_env.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50343 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/keras_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/nc_reader.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2528 2024-01-22 02:42:52.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/pid.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    11159 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/process_image.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3274 2023-12-07 02:51:22.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/pycuda_test.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:10:14.023391 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7190 2023-12-07 02:51:22.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2023-12-07 02:51:22.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2023-12-07 02:51:22.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2023-12-07 02:51:22.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19805 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/rw_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14881 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/rw_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16801 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/remove_outlier.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12394 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/biomedisa_features/split_volume.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27063 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/deeplearning.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17335 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/interpolation.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15920 2024-05-08 09:06:16.000000 biomedisa-2024.5.17/src/biomedisa/mesh.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:10:14.023391 biomedisa-2024.5.17/src/biomedisa.egg-info/
--rw-r--r--   0 philipp   (1000) philipp   (1000)    11677 2024-05-14 05:10:14.000000 biomedisa-2024.5.17/src/biomedisa.egg-info/PKG-INFO
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2172 2024-05-14 05:10:14.000000 biomedisa-2024.5.17/src/biomedisa.egg-info/SOURCES.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-14 05:10:14.000000 biomedisa-2024.5.17/src/biomedisa.egg-info/dependency_links.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-14 05:10:14.000000 biomedisa-2024.5.17/src/biomedisa.egg-info/top_level.txt
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/LICENSE
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    10748 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/PKG-INFO
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    10140 2024-05-14 05:13:31.000000 biomedisa-2024.5.18/README.md
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)      664 2024-05-14 05:13:42.000000 biomedisa-2024.5.18/pyproject.toml
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/setup.cfg
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/src/
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/src/biomedisa/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1690 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/__main__.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/DataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-02-14 23:44:22.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/DataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/PredictDataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2023-12-07 02:51:22.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18131 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/active_contour.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/assd.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32401 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/biomedisa_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13329 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/create_slices.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    23894 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/crop_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/curvop_numba.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     8989 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/django_env.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50343 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/keras_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/nc_reader.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2528 2024-01-22 02:42:52.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/pid.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    11159 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/process_image.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3274 2023-12-07 02:51:22.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/pycuda_test.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7190 2023-12-07 02:51:22.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2023-12-07 02:51:22.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2023-12-07 02:51:22.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2023-12-07 02:51:22.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19805 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/rw_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14881 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/rw_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16801 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/remove_outlier.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12394 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/biomedisa_features/split_volume.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27063 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/deeplearning.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17335 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/interpolation.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15920 2024-05-08 09:06:16.000000 biomedisa-2024.5.18/src/biomedisa/mesh.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-14 05:14:07.913074 biomedisa-2024.5.18/src/biomedisa.egg-info/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    10748 2024-05-14 05:14:07.000000 biomedisa-2024.5.18/src/biomedisa.egg-info/PKG-INFO
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2172 2024-05-14 05:14:07.000000 biomedisa-2024.5.18/src/biomedisa.egg-info/SOURCES.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-14 05:14:07.000000 biomedisa-2024.5.18/src/biomedisa.egg-info/dependency_links.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-14 05:14:07.000000 biomedisa-2024.5.18/src/biomedisa.egg-info/top_level.txt
```

### Comparing `biomedisa-2024.5.17/LICENSE` & `biomedisa-2024.5.18/LICENSE`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/PKG-INFO` & `biomedisa-2024.5.18/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: biomedisa
-Version: 2024.5.17
-Summary: Segmentation of 3D volumetric image data
-Author: Philipp Lösel
-Author-email: philipp.loesel@anu.edu.au
-Project-URL: Homepage, https://biomedisa.info
-Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
-Project-URL: GitHub, https://github.com/biomedisa/biomedisa
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![biomedisa](biomedisa_app/static/biomedisa_logo.svg)](https://biomedisa.info)
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
@@ -51,21 +35,16 @@
 + Download the data from our [gallery](https://biomedisa.info/gallery/)
 
 # Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.biomedisa_interpolation import smart_interpolation
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.interpolation import smart_interpolation
 
 # load data
 img, _ = load_data('Downloads/trigonopterus.tif')
 labels, header = load_data('Downloads/labels.trigonopterus_smart.am')
 
 # run smart interpolation with optional smoothing result
 results = smart_interpolation(img, labels, smooth=100)
@@ -77,34 +56,24 @@
 # save results
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
-# start smart interpolation
-python biomedisa_interpolation.py C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
+python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
 ```
 
 # Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-# load libraries
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data
-from biomedisa_features.biomedisa_deeplearning import deep_learning
+from biomedisa.biomedisa_features.biomedisa_helper import load_data
+from biomedisa.deeplearning import deep_learning
 
 # load image data
 img1, _ = load_data('Head1.am')
 img2, _ = load_data('Head2.am')
 img_data = [img1, img2]
 
 # load label data and header information to be stored in the network file (optional)
@@ -125,79 +94,63 @@
 deep_learning(img_data, label_data, train=True, batch_size=12,
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
 # start training with a batch size of 12
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
 
 # validation (optional)
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
 ```
 If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
 
 #### Python example (prediction)
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-# load libraries
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.biomedisa_deeplearning import deep_learning
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.deeplearning import deep_learning
 
 # load data
 img, _ = load_data('Head5.am')
 
 # deep learning
 results = deep_learning(img, predict=True,
         path_to_model='honeybees.h5', batch_size=6)
 
 # save result
 save_data('final.Head5.am', results['regular'], results['header'])
 ```
 
 #### Command-line based (prediction)
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
 # start prediction with a batch size of 6
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p -bs 6
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p -bs 6
 ```
 
 # Biomedisa Features
 
 #### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
 ```python
-import sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
 
 # load data as numpy array
 # for DICOM, PNG files, or similar formats, 'path_to_data' must reference
 # either a directory or a ZIP file containing the image slices
 data, header = load_data(path_to_data)
 
 # save data (for TIFF, header=None)
 save_data(path_to_data, data, header)
 ```
 
 #### Create STL mesh from segmentation (label values are saved as attributes)
 ```python
-import os, sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.create_mesh import get_voxel_spacing, save_mesh
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.mesh import get_voxel_spacing, save_mesh
 
 # load segmentation
 data, header, extension = load_data(path_to_data, return_extension=True)
 
 # get voxel spacing
 x_res, y_res, z_res = get_voxel_spacing(header, data, extension)
 print(f'Voxel spacing: x_spacing, y_spacing, z_spacing = {x_res}, {y_res}, {z_res}')
@@ -205,15 +158,15 @@
 # save stl file
 path_to_data = path_to_data.replace(os.path.splitext(path_to_data)[1],'.stl')
 save_mesh(path_to_data, data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
 ```
 
 #### Create mesh directly
 ```
-python git/biomedisa/biomedisa_features/create_mesh.py <path_to_data>
+python -m biomedisa.mesh <path_to_data>
 ```
 
 #### Options
 `--poly_reduction` or `-pr`: Reduce number of polygons by this factor (default: 0.9)
 
 `--smoothing_iterations` or `-s`: Iteration steps for smoothing (default: 15)
 
@@ -221,58 +174,60 @@
 
 `--y_res` or `-yres`: Voxel spacing/resolution y-axis (default: None)
 
 `--z_res` or `-zres`: Voxel spacing/resolution z-axis (default: None)
 
 #### Resize data
 ```python
-import os, sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import img_resize
+from biomedisa.biomedisa_features.biomedisa_helper import img_resize
 
 # resize image data
 zsh, ysh, xsh = data.shape
 new_zsh, new_ysh, new_xsh = zsh//2, ysh//2, xsh//2
 data = img_resize(data, new_zsh, new_ysh, new_xsh)
 
 # resize label data
 label_data = img_resize(label_data, new_zsh, new_ysh, new_xsh, labels=True)
 ```
 
 #### Remove outliers and fill holes
 ```python
-from biomedisa_features.biomedisa_helper import clean, fill
+from biomedisa.biomedisa_features.biomedisa_helper import clean, fill
 
 # delete outliers smaller than 90% of the segment
 label_data = clean(label_data, 0.9)
 
 # fill holes
 label_data = fill(label_data, 0.9)
 ```
 
 #### Accuracy assessment
 ```python
-from biomedisa_features.biomedisa_helper import Dice_score, ASSD
+from biomedisa.biomedisa_features.biomedisa_helper import Dice_score, ASSD
 dice = Dice_score(ground_truth, result)
 assd = ASSD(ground_truth, result)
 ```
 
 # Update Biomedisa
-If you have used `git clone`, change to the Biomedisa directory and make a pull request.
+If you installed Biomedisa via Pip.
+```
+pip install --upgrade biomedisa
+```
+If you used `git clone`, change to the Biomedisa directory and make a pull request.
 ```
 cd git/biomedisa
 git pull
 ```
 
-If you have installed the browser based version of Biomedisa (including MySQL database), you also need to update the database.
+If you installed the browser based version of Biomedisa (including MySQL database), you also need to update the database.
 ```
 python manage.py migrate
 ```
 
-If you have installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server.
+If you installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server.
 ```
 sudo service apache2 restart
 ```
 
 # Releases
 
 For the versions available, see the [list of releases](https://github.com/biomedisa/biomedisa/releases).
```

### Comparing `biomedisa-2024.5.17/README.md` & `biomedisa-2024.5.18/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: biomedisa
+Version: 2024.5.18
+Summary: Segmentation of 3D volumetric image data
+Author: Philipp Lösel
+Author-email: philipp.loesel@anu.edu.au
+Project-URL: Homepage, https://biomedisa.info
+Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
+Project-URL: GitHub, https://github.com/biomedisa/biomedisa
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![biomedisa](biomedisa_app/static/biomedisa_logo.svg)](https://biomedisa.info)
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
@@ -35,21 +51,16 @@
 + Download the data from our [gallery](https://biomedisa.info/gallery/)
 
 # Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.biomedisa_interpolation import smart_interpolation
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.interpolation import smart_interpolation
 
 # load data
 img, _ = load_data('Downloads/trigonopterus.tif')
 labels, header = load_data('Downloads/labels.trigonopterus_smart.am')
 
 # run smart interpolation with optional smoothing result
 results = smart_interpolation(img, labels, smooth=100)
@@ -61,34 +72,24 @@
 # save results
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
-# start smart interpolation
-python biomedisa_interpolation.py C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
+python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
 ```
 
 # Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-# load libraries
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data
-from biomedisa_features.biomedisa_deeplearning import deep_learning
+from biomedisa.biomedisa_features.biomedisa_helper import load_data
+from biomedisa.deeplearning import deep_learning
 
 # load image data
 img1, _ = load_data('Head1.am')
 img2, _ = load_data('Head2.am')
 img_data = [img1, img2]
 
 # load label data and header information to be stored in the network file (optional)
@@ -109,79 +110,63 @@
 deep_learning(img_data, label_data, train=True, batch_size=12,
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
 # start training with a batch size of 12
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
 
 # validation (optional)
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
 ```
 If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
 
 #### Python example (prediction)
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-# load libraries
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.biomedisa_deeplearning import deep_learning
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.deeplearning import deep_learning
 
 # load data
 img, _ = load_data('Head5.am')
 
 # deep learning
 results = deep_learning(img, predict=True,
         path_to_model='honeybees.h5', batch_size=6)
 
 # save result
 save_data('final.Head5.am', results['regular'], results['header'])
 ```
 
 #### Command-line based (prediction)
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
 # start prediction with a batch size of 6
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p -bs 6
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p -bs 6
 ```
 
 # Biomedisa Features
 
 #### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
 ```python
-import sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
 
 # load data as numpy array
 # for DICOM, PNG files, or similar formats, 'path_to_data' must reference
 # either a directory or a ZIP file containing the image slices
 data, header = load_data(path_to_data)
 
 # save data (for TIFF, header=None)
 save_data(path_to_data, data, header)
 ```
 
 #### Create STL mesh from segmentation (label values are saved as attributes)
 ```python
-import os, sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.create_mesh import get_voxel_spacing, save_mesh
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.mesh import get_voxel_spacing, save_mesh
 
 # load segmentation
 data, header, extension = load_data(path_to_data, return_extension=True)
 
 # get voxel spacing
 x_res, y_res, z_res = get_voxel_spacing(header, data, extension)
 print(f'Voxel spacing: x_spacing, y_spacing, z_spacing = {x_res}, {y_res}, {z_res}')
@@ -189,15 +174,15 @@
 # save stl file
 path_to_data = path_to_data.replace(os.path.splitext(path_to_data)[1],'.stl')
 save_mesh(path_to_data, data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
 ```
 
 #### Create mesh directly
 ```
-python git/biomedisa/biomedisa_features/create_mesh.py <path_to_data>
+python -m biomedisa.mesh <path_to_data>
 ```
 
 #### Options
 `--poly_reduction` or `-pr`: Reduce number of polygons by this factor (default: 0.9)
 
 `--smoothing_iterations` or `-s`: Iteration steps for smoothing (default: 15)
 
@@ -205,58 +190,60 @@
 
 `--y_res` or `-yres`: Voxel spacing/resolution y-axis (default: None)
 
 `--z_res` or `-zres`: Voxel spacing/resolution z-axis (default: None)
 
 #### Resize data
 ```python
-import os, sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import img_resize
+from biomedisa.biomedisa_features.biomedisa_helper import img_resize
 
 # resize image data
 zsh, ysh, xsh = data.shape
 new_zsh, new_ysh, new_xsh = zsh//2, ysh//2, xsh//2
 data = img_resize(data, new_zsh, new_ysh, new_xsh)
 
 # resize label data
 label_data = img_resize(label_data, new_zsh, new_ysh, new_xsh, labels=True)
 ```
 
 #### Remove outliers and fill holes
 ```python
-from biomedisa_features.biomedisa_helper import clean, fill
+from biomedisa.biomedisa_features.biomedisa_helper import clean, fill
 
 # delete outliers smaller than 90% of the segment
 label_data = clean(label_data, 0.9)
 
 # fill holes
 label_data = fill(label_data, 0.9)
 ```
 
 #### Accuracy assessment
 ```python
-from biomedisa_features.biomedisa_helper import Dice_score, ASSD
+from biomedisa.biomedisa_features.biomedisa_helper import Dice_score, ASSD
 dice = Dice_score(ground_truth, result)
 assd = ASSD(ground_truth, result)
 ```
 
 # Update Biomedisa
-If you have used `git clone`, change to the Biomedisa directory and make a pull request.
+If you installed Biomedisa via Pip.
+```
+pip install --upgrade biomedisa
+```
+If you used `git clone`, change to the Biomedisa directory and make a pull request.
 ```
 cd git/biomedisa
 git pull
 ```
 
-If you have installed the browser based version of Biomedisa (including MySQL database), you also need to update the database.
+If you installed the browser based version of Biomedisa (including MySQL database), you also need to update the database.
 ```
 python manage.py migrate
 ```
 
-If you have installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server.
+If you installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server.
 ```
 sudo service apache2 restart
 ```
 
 # Releases
 
 For the versions available, see the [list of releases](https://github.com/biomedisa/biomedisa/releases).
```

### Comparing `biomedisa-2024.5.17/pyproject.toml` & `biomedisa-2024.5.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biomedisa"
-version = "2024.5.17"
+version = "2024.5.18"
 authors = [
   { name="Philipp Lösel"}, {email="philipp.loesel@anu.edu.au" },
 ]
 description = "Segmentation of 3D volumetric image data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `biomedisa-2024.5.17/src/biomedisa/__init__.py` & `biomedisa-2024.5.18/src/biomedisa/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/__main__.py` & `biomedisa-2024.5.18/src/biomedisa/__main__.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/DataGenerator.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/DataGeneratorCrop.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/DataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/PredictDataGenerator.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/PredictDataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/active_contour.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/active_contour.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/assd.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/assd.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/biomedisa_helper.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/biomedisa_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/create_slices.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/create_slices.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/crop_helper.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/crop_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/curvop_numba.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/curvop_numba.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/django_env.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/django_env.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/keras_helper.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/keras_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/nc_reader.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/nc_reader.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/pid.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/pid.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/process_image.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/process_image.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/pycuda_test.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/pycuda_test.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/rw_large.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/rw_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/random_walk/rw_small.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/random_walk/rw_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/remove_outlier.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/remove_outlier.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/biomedisa_features/split_volume.py` & `biomedisa-2024.5.18/src/biomedisa/biomedisa_features/split_volume.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/deeplearning.py` & `biomedisa-2024.5.18/src/biomedisa/deeplearning.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/interpolation.py` & `biomedisa-2024.5.18/src/biomedisa/interpolation.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa/mesh.py` & `biomedisa-2024.5.18/src/biomedisa/mesh.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.17/src/biomedisa.egg-info/PKG-INFO` & `biomedisa-2024.5.18/src/biomedisa.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedisa
-Version: 2024.5.17
+Version: 2024.5.18
 Summary: Segmentation of 3D volumetric image data
 Author: Philipp Lösel
 Author-email: philipp.loesel@anu.edu.au
 Project-URL: Homepage, https://biomedisa.info
 Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
 Project-URL: GitHub, https://github.com/biomedisa/biomedisa
 Classifier: Programming Language :: Python :: 3
@@ -51,21 +51,16 @@
 + Download the data from our [gallery](https://biomedisa.info/gallery/)
 
 # Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.biomedisa_interpolation import smart_interpolation
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.interpolation import smart_interpolation
 
 # load data
 img, _ = load_data('Downloads/trigonopterus.tif')
 labels, header = load_data('Downloads/labels.trigonopterus_smart.am')
 
 # run smart interpolation with optional smoothing result
 results = smart_interpolation(img, labels, smooth=100)
@@ -77,34 +72,24 @@
 # save results
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
-# start smart interpolation
-python biomedisa_interpolation.py C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
+python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
 ```
 
 # Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-# load libraries
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data
-from biomedisa_features.biomedisa_deeplearning import deep_learning
+from biomedisa.biomedisa_features.biomedisa_helper import load_data
+from biomedisa.deeplearning import deep_learning
 
 # load image data
 img1, _ = load_data('Head1.am')
 img2, _ = load_data('Head2.am')
 img_data = [img1, img2]
 
 # load label data and header information to be stored in the network file (optional)
@@ -125,79 +110,63 @@
 deep_learning(img_data, label_data, train=True, batch_size=12,
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
 # start training with a batch size of 12
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
 
 # validation (optional)
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
 ```
 If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
 
 #### Python example (prediction)
 ```python
-# change this line to your biomedisa directory
-path_to_biomedisa = '/home/<user>/git/biomedisa'
-
-# load libraries
-import sys
-sys.path.append(path_to_biomedisa)
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.biomedisa_deeplearning import deep_learning
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.deeplearning import deep_learning
 
 # load data
 img, _ = load_data('Head5.am')
 
 # deep learning
 results = deep_learning(img, predict=True,
         path_to_model='honeybees.h5', batch_size=6)
 
 # save result
 save_data('final.Head5.am', results['regular'], results['header'])
 ```
 
 #### Command-line based (prediction)
 ```
-# change to the features directory
-cd git/biomedisa/biomedisa_features/
-
 # start prediction with a batch size of 6
-python biomedisa_deeplearning.py C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p -bs 6
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p -bs 6
 ```
 
 # Biomedisa Features
 
 #### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
 ```python
-import sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
 
 # load data as numpy array
 # for DICOM, PNG files, or similar formats, 'path_to_data' must reference
 # either a directory or a ZIP file containing the image slices
 data, header = load_data(path_to_data)
 
 # save data (for TIFF, header=None)
 save_data(path_to_data, data, header)
 ```
 
 #### Create STL mesh from segmentation (label values are saved as attributes)
 ```python
-import os, sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import load_data, save_data
-from biomedisa_features.create_mesh import get_voxel_spacing, save_mesh
+from biomedisa.biomedisa_features.biomedisa_helper import load_data, save_data
+from biomedisa.mesh import get_voxel_spacing, save_mesh
 
 # load segmentation
 data, header, extension = load_data(path_to_data, return_extension=True)
 
 # get voxel spacing
 x_res, y_res, z_res = get_voxel_spacing(header, data, extension)
 print(f'Voxel spacing: x_spacing, y_spacing, z_spacing = {x_res}, {y_res}, {z_res}')
@@ -205,15 +174,15 @@
 # save stl file
 path_to_data = path_to_data.replace(os.path.splitext(path_to_data)[1],'.stl')
 save_mesh(path_to_data, data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
 ```
 
 #### Create mesh directly
 ```
-python git/biomedisa/biomedisa_features/create_mesh.py <path_to_data>
+python -m biomedisa.mesh <path_to_data>
 ```
 
 #### Options
 `--poly_reduction` or `-pr`: Reduce number of polygons by this factor (default: 0.9)
 
 `--smoothing_iterations` or `-s`: Iteration steps for smoothing (default: 15)
 
@@ -221,58 +190,60 @@
 
 `--y_res` or `-yres`: Voxel spacing/resolution y-axis (default: None)
 
 `--z_res` or `-zres`: Voxel spacing/resolution z-axis (default: None)
 
 #### Resize data
 ```python
-import os, sys
-sys.path.append(path_to_biomedisa)  # e.g. '/home/<user>/git/biomedisa'
-from biomedisa_features.biomedisa_helper import img_resize
+from biomedisa.biomedisa_features.biomedisa_helper import img_resize
 
 # resize image data
 zsh, ysh, xsh = data.shape
 new_zsh, new_ysh, new_xsh = zsh//2, ysh//2, xsh//2
 data = img_resize(data, new_zsh, new_ysh, new_xsh)
 
 # resize label data
 label_data = img_resize(label_data, new_zsh, new_ysh, new_xsh, labels=True)
 ```
 
 #### Remove outliers and fill holes
 ```python
-from biomedisa_features.biomedisa_helper import clean, fill
+from biomedisa.biomedisa_features.biomedisa_helper import clean, fill
 
 # delete outliers smaller than 90% of the segment
 label_data = clean(label_data, 0.9)
 
 # fill holes
 label_data = fill(label_data, 0.9)
 ```
 
 #### Accuracy assessment
 ```python
-from biomedisa_features.biomedisa_helper import Dice_score, ASSD
+from biomedisa.biomedisa_features.biomedisa_helper import Dice_score, ASSD
 dice = Dice_score(ground_truth, result)
 assd = ASSD(ground_truth, result)
 ```
 
 # Update Biomedisa
-If you have used `git clone`, change to the Biomedisa directory and make a pull request.
+If you installed Biomedisa via Pip.
+```
+pip install --upgrade biomedisa
+```
+If you used `git clone`, change to the Biomedisa directory and make a pull request.
 ```
 cd git/biomedisa
 git pull
 ```
 
-If you have installed the browser based version of Biomedisa (including MySQL database), you also need to update the database.
+If you installed the browser based version of Biomedisa (including MySQL database), you also need to update the database.
 ```
 python manage.py migrate
 ```
 
-If you have installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server.
+If you installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server.
 ```
 sudo service apache2 restart
 ```
 
 # Releases
 
 For the versions available, see the [list of releases](https://github.com/biomedisa/biomedisa/releases).
```

### Comparing `biomedisa-2024.5.17/src/biomedisa.egg-info/SOURCES.txt` & `biomedisa-2024.5.18/src/biomedisa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

