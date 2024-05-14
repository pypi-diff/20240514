# Comparing `tmp/neural_amp_modeler-0.8.2.tar.gz` & `tmp/neural_amp_modeler-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_amp_modeler-0.8.2.tar", last modified: Tue May 14 05:40:19 2024, max compression
+gzip compressed data, was "neural_amp_modeler-0.8.3.tar", last modified: Tue May 14 07:12:04 2024, max compression
```

## Comparing `neural_amp_modeler-0.8.2.tar` & `neural_amp_modeler-0.8.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.812952 neural_amp_modeler-0.8.2/
--rw-r--r--   0 steve      (501) staff       (20)     1072 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural_amp_modeler-0.8.2/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)      575 2024-05-14 05:40:19.812029 neural_amp_modeler-0.8.2/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      382 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.751000 neural_amp_modeler-0.8.2/nam/
--rw-r--r--   0 steve      (501) staff       (20)      730 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural_amp_modeler-0.8.2/nam/_core.py
--rw-r--r--   0 steve      (501) staff       (20)       22 2024-05-14 05:32:08.000000 neural_amp_modeler-0.8.2/nam/_version.py
--rw-r--r--   0 steve      (501) staff       (20)    27396 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/data.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.769847 neural_amp_modeler-0.8.2/nam/models/
--rw-r--r--   0 steve      (501) staff       (20)      402 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural_amp_modeler-0.8.2/nam/models/_activations.py
--rw-r--r--   0 steve      (501) staff       (20)     5891 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/models/_base.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/nam/models/_names.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.771322 neural_amp_modeler-0.8.2/nam/models/_resources/
--rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural_amp_modeler-0.8.2/nam/models/_resources/loudness_input.wav
--rw-r--r--   0 steve      (501) staff       (20)    14032 2024-02-11 16:22:35.000000 neural_amp_modeler-0.8.2/nam/models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     9259 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.2/nam/models/conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     4874 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/models/exportable.py
--rw-r--r--   0 steve      (501) staff       (20)     2203 2023-10-09 15:24:53.000000 neural_amp_modeler-0.8.2/nam/models/linear.py
--rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural_amp_modeler-0.8.2/nam/models/losses.py
--rw-r--r--   0 steve      (501) staff       (20)     1215 2023-10-06 17:56:34.000000 neural_amp_modeler-0.8.2/nam/models/metadata.py
--rw-r--r--   0 steve      (501) staff       (20)    16557 2023-06-25 16:29:54.000000 neural_amp_modeler-0.8.2/nam/models/recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)    13969 2023-06-22 07:13:06.000000 neural_amp_modeler-0.8.2/nam/models/wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.781499 neural_amp_modeler-0.8.2/nam/train/
--rw-r--r--   0 steve      (501) staff       (20)      251 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      693 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/train/_names.py
--rw-r--r--   0 steve      (501) staff       (20)      931 2024-02-10 19:50:23.000000 neural_amp_modeler-0.8.2/nam/train/_version.py
--rw-r--r--   0 steve      (501) staff       (20)     4095 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/train/colab.py
--rw-r--r--   0 steve      (501) staff       (20)    45863 2024-05-13 15:33:11.000000 neural_amp_modeler-0.8.2/nam/train/core.py
--rw-r--r--   0 steve      (501) staff       (20)    27403 2024-05-13 15:33:11.000000 neural_amp_modeler-0.8.2/nam/train/gui.py
--rw-r--r--   0 steve      (501) staff       (20)     1075 2023-11-12 20:17:46.000000 neural_amp_modeler-0.8.2/nam/util.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.811092 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      575 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     1503 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       42 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      154 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       10 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-14 05:40:19.813129 neural_amp_modeler-0.8.2/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)     1451 2024-02-11 16:22:35.000000 neural_amp_modeler-0.8.2/setup.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.787523 neural_amp_modeler-0.8.2/tests/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural_amp_modeler-0.8.2/tests/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.788649 neural_amp_modeler-0.8.2/tests/resources/
--rw-r--r--   0 steve      (501) staff       (20)     1021 2024-02-07 08:14:11.000000 neural_amp_modeler-0.8.2/tests/resources/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.790363 neural_amp_modeler-0.8.2/tests/test_bin/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural_amp_modeler-0.8.2/tests/test_bin/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.791346 neural_amp_modeler-0.8.2/tests/test_bin/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural_amp_modeler-0.8.2/tests/test_bin/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6568 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.2/tests/test_bin/test_train/test_main.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_install.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.795240 neural_amp_modeler-0.8.2/tests/test_nam/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    14908 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_data.py
--rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_importable.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.805601 neural_amp_modeler-0.8.2/tests/test_nam/test_models/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     4514 2024-01-13 03:07:09.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_base.py
--rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     4586 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_losses.py
--rw-r--r--   0 steve      (501) staff       (20)     2360 2023-06-20 00:48:33.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.809083 neural_amp_modeler-0.8.2/tests/test_nam/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     8251 2024-02-07 08:14:11.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_core.py
--rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_version.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.889357 neural_amp_modeler-0.8.3/
+-rw-r--r--   0 steve      (501) staff       (20)     1072 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.3/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural_amp_modeler-0.8.3/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)      575 2024-05-14 07:12:04.888605 neural_amp_modeler-0.8.3/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      382 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.3/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.851263 neural_amp_modeler-0.8.3/nam/
+-rw-r--r--   0 steve      (501) staff       (20)      730 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.3/nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural_amp_modeler-0.8.3/nam/_core.py
+-rw-r--r--   0 steve      (501) staff       (20)       22 2024-05-14 07:11:21.000000 neural_amp_modeler-0.8.3/nam/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)    27396 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.3/nam/data.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.860459 neural_amp_modeler-0.8.3/nam/models/
+-rw-r--r--   0 steve      (501) staff       (20)      402 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.3/nam/models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural_amp_modeler-0.8.3/nam/models/_activations.py
+-rw-r--r--   0 steve      (501) staff       (20)     6291 2024-05-14 07:11:21.000000 neural_amp_modeler-0.8.3/nam/models/_base.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.3/nam/models/_names.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.861051 neural_amp_modeler-0.8.3/nam/models/_resources/
+-rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural_amp_modeler-0.8.3/nam/models/_resources/loudness_input.wav
+-rw-r--r--   0 steve      (501) staff       (20)    14032 2024-02-11 16:22:35.000000 neural_amp_modeler-0.8.3/nam/models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     9259 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.3/nam/models/conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     4874 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.3/nam/models/exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)     2203 2023-10-09 15:24:53.000000 neural_amp_modeler-0.8.3/nam/models/linear.py
+-rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural_amp_modeler-0.8.3/nam/models/losses.py
+-rw-r--r--   0 steve      (501) staff       (20)     1215 2023-10-06 17:56:34.000000 neural_amp_modeler-0.8.3/nam/models/metadata.py
+-rw-r--r--   0 steve      (501) staff       (20)    16557 2023-06-25 16:29:54.000000 neural_amp_modeler-0.8.3/nam/models/recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)    13975 2024-05-14 07:11:21.000000 neural_amp_modeler-0.8.3/nam/models/wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.868734 neural_amp_modeler-0.8.3/nam/train/
+-rw-r--r--   0 steve      (501) staff       (20)      251 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.3/nam/train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      693 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.3/nam/train/_names.py
+-rw-r--r--   0 steve      (501) staff       (20)      931 2024-02-10 19:50:23.000000 neural_amp_modeler-0.8.3/nam/train/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     4095 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.3/nam/train/colab.py
+-rw-r--r--   0 steve      (501) staff       (20)    45863 2024-05-13 15:33:11.000000 neural_amp_modeler-0.8.3/nam/train/core.py
+-rw-r--r--   0 steve      (501) staff       (20)    27403 2024-05-13 15:33:11.000000 neural_amp_modeler-0.8.3/nam/train/gui.py
+-rw-r--r--   0 steve      (501) staff       (20)     1075 2023-11-12 20:17:46.000000 neural_amp_modeler-0.8.3/nam/util.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.887907 neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      575 2024-05-14 07:12:04.000000 neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     1503 2024-05-14 07:12:04.000000 neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-14 07:12:04.000000 neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       42 2024-05-14 07:12:04.000000 neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      154 2024-05-14 07:12:04.000000 neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       10 2024-05-14 07:12:04.000000 neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-14 07:12:04.889548 neural_amp_modeler-0.8.3/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)     1451 2024-02-11 16:22:35.000000 neural_amp_modeler-0.8.3/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.872697 neural_amp_modeler-0.8.3/tests/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural_amp_modeler-0.8.3/tests/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.873608 neural_amp_modeler-0.8.3/tests/resources/
+-rw-r--r--   0 steve      (501) staff       (20)     1021 2024-02-07 08:14:11.000000 neural_amp_modeler-0.8.3/tests/resources/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.874471 neural_amp_modeler-0.8.3/tests/test_bin/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural_amp_modeler-0.8.3/tests/test_bin/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.875279 neural_amp_modeler-0.8.3/tests/test_bin/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural_amp_modeler-0.8.3/tests/test_bin/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6568 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.3/tests/test_bin/test_train/test_main.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.3/tests/test_install.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.877755 neural_amp_modeler-0.8.3/tests/test_nam/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.3/tests/test_nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    14908 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_data.py
+-rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_importable.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.884299 neural_amp_modeler-0.8.3/tests/test_nam/test_models/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     4514 2024-01-13 03:07:09.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     4586 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_losses.py
+-rw-r--r--   0 steve      (501) staff       (20)     2360 2023-06-20 00:48:33.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 07:12:04.886766 neural_amp_modeler-0.8.3/tests/test_nam/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     8251 2024-02-07 08:14:11.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_train/test_core.py
+-rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural_amp_modeler-0.8.3/tests/test_nam/test_train/test_version.py
```

### Comparing `neural_amp_modeler-0.8.2/LICENSE` & `neural_amp_modeler-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/PKG-INFO` & `neural_amp_modeler-0.8.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-amp-modeler
-Version: 0.8.2
+Version: 0.8.3
 Summary: Neural amp modeler
 Home-page: https://github.com/sdatkinson/
 Author: Steven Atkinson
 Author-email: steven@atkinson.mn
 License-File: LICENSE
 Requires-Dist: auraloss==0.3.0
 Requires-Dist: matplotlib
```

### Comparing `neural_amp_modeler-0.8.2/nam/__init__.py` & `neural_amp_modeler-0.8.3/nam/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/data.py` & `neural_amp_modeler-0.8.3/nam/data.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/_base.py` & `neural_amp_modeler-0.8.3/nam/models/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,26 @@
         return wav_to_tensor(
             pkg_resources.resource_filename(
                 "nam", "models/_resources/loudness_input.wav"
             )
         )
 
     @property
+    def device(self) -> Optional[torch.device]:
+        """
+        Helpful property, where the parameters of the model live.
+        """
+        # We can do this because the models are tiny and I don't expect a NAM to be on
+        # multiple devices
+        try:
+            return next(self.parameters()).device
+        except StopIteration:
+            return None
+
+    @property
     def sample_rate(self) -> Optional[float]:
         return self._sample_rate.item() if self._has_sample_rate else None
 
     @sample_rate.setter
     def sample_rate(self, val: Optional[float]):
         self._has_sample_rate = torch.tensor(val is not None, dtype=torch.bool)
         self._sample_rate = torch.tensor(0.0 if val is None else val)
@@ -77,15 +89,15 @@
     def _metadata_loudness(self, gain: float = 1.0, db: bool = True) -> float:
         """
         How loud is this model when given a standardized input?
         In dB
 
         :param gain: Multiplies input signal
         """
-        x = self._metadata_loudness_x()
+        x = self._metadata_loudness_x().to(self.device)
         y = self._at_nominal_settings(gain * x)
         loudness = torch.sqrt(torch.mean(torch.square(y)))
         if db:
             loudness = 20.0 * torch.log10(loudness)
         return loudness.item()
 
     def _metadata_gain(self) -> float:
```

### Comparing `neural_amp_modeler-0.8.2/nam/models/_resources/loudness_input.wav` & `neural_amp_modeler-0.8.3/nam/models/_resources/loudness_input.wav`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/base.py` & `neural_amp_modeler-0.8.3/nam/models/base.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/conv_net.py` & `neural_amp_modeler-0.8.3/nam/models/conv_net.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/exportable.py` & `neural_amp_modeler-0.8.3/nam/models/exportable.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/linear.py` & `neural_amp_modeler-0.8.3/nam/models/linear.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/losses.py` & `neural_amp_modeler-0.8.3/nam/models/losses.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/metadata.py` & `neural_amp_modeler-0.8.3/nam/models/metadata.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/recurrent.py` & `neural_amp_modeler-0.8.3/nam/models/recurrent.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/models/wavenet.py` & `neural_amp_modeler-0.8.3/nam/models/wavenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     def export_weights(self) -> np.ndarray:
         """
         :return: 1D array
         """
         weights = torch.cat([layer.export_weights() for layer in self._layers])
         if self._head is not None:
             weights = torch.cat([weights, self._head.export_weights()])
-        weights = torch.cat([weights, torch.Tensor([self._head_scale])])
+        weights = torch.cat([weights.cpu(), torch.Tensor([self._head_scale])])
         return weights.detach().cpu().numpy()
 
     def import_weights(self, weights: torch.Tensor):
         i = 0
         for layer in self._layers:
             i = layer.import_weights(weights, i)
```

### Comparing `neural_amp_modeler-0.8.2/nam/train/_names.py` & `neural_amp_modeler-0.8.3/nam/train/_names.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/train/_version.py` & `neural_amp_modeler-0.8.3/nam/train/_version.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/train/colab.py` & `neural_amp_modeler-0.8.3/nam/train/colab.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/train/core.py` & `neural_amp_modeler-0.8.3/nam/train/core.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/train/gui.py` & `neural_amp_modeler-0.8.3/nam/train/gui.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/nam/util.py` & `neural_amp_modeler-0.8.3/nam/util.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/PKG-INFO` & `neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-amp-modeler
-Version: 0.8.2
+Version: 0.8.3
 Summary: Neural amp modeler
 Home-page: https://github.com/sdatkinson/
 Author: Steven Atkinson
 Author-email: steven@atkinson.mn
 License-File: LICENSE
 Requires-Dist: auraloss==0.3.0
 Requires-Dist: matplotlib
```

### Comparing `neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/SOURCES.txt` & `neural_amp_modeler-0.8.3/neural_amp_modeler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/setup.py` & `neural_amp_modeler-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/resources/__init__.py` & `neural_amp_modeler-0.8.3/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_bin/test_train/test_main.py` & `neural_amp_modeler-0.8.3/tests/test_bin/test_train/test_main.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_data.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_data.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_models/base.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_models/base.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_base.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_base.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_conv_net.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_conv_net.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_exportable.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_exportable.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_losses.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_losses.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_recurrent.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_recurrent.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_wavenet.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_models/test_wavenet.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_core.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_train/test_core.py`

 * *Files identical despite different names*

### Comparing `neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_version.py` & `neural_amp_modeler-0.8.3/tests/test_nam/test_train/test_version.py`

 * *Files identical despite different names*

