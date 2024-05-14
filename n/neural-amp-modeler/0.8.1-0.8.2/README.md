# Comparing `tmp/neural-amp-modeler-0.8.1.tar.gz` & `tmp/neural_amp_modeler-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-amp-modeler-0.8.1.tar", last modified: Sun Feb 11 16:25:01 2024, max compression
+gzip compressed data, was "neural_amp_modeler-0.8.2.tar", last modified: Tue May 14 05:40:19 2024, max compression
```

## Comparing `neural-amp-modeler-0.8.1.tar` & `neural_amp_modeler-0.8.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.587527 neural-amp-modeler-0.8.1/
--rw-r--r--   0 steve      (501) staff       (20)     1072 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural-amp-modeler-0.8.1/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)      575 2024-02-11 16:25:01.586794 neural-amp-modeler-0.8.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     6058 2024-02-11 15:53:26.000000 neural-amp-modeler-0.8.1/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.509327 neural-amp-modeler-0.8.1/nam/
--rw-r--r--   0 steve      (501) staff       (20)      729 2023-03-18 16:36:25.000000 neural-amp-modeler-0.8.1/nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural-amp-modeler-0.8.1/nam/_core.py
--rw-r--r--   0 steve      (501) staff       (20)       22 2024-02-11 16:22:42.000000 neural-amp-modeler-0.8.1/nam/_version.py
--rw-r--r--   0 steve      (501) staff       (20)    27295 2024-02-07 06:58:00.000000 neural-amp-modeler-0.8.1/nam/data.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.523670 neural-amp-modeler-0.8.1/nam/models/
--rw-r--r--   0 steve      (501) staff       (20)      372 2023-10-09 15:24:53.000000 neural-amp-modeler-0.8.1/nam/models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural-amp-modeler-0.8.1/nam/models/_activations.py
--rw-r--r--   0 steve      (501) staff       (20)     5892 2024-02-11 16:22:35.000000 neural-amp-modeler-0.8.1/nam/models/_base.py
--rw-r--r--   0 steve      (501) staff       (20)     4828 2024-01-13 20:55:59.000000 neural-amp-modeler-0.8.1/nam/models/_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/nam/models/_names.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.525035 neural-amp-modeler-0.8.1/nam/models/_resources/
--rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural-amp-modeler-0.8.1/nam/models/_resources/loudness_input.wav
--rw-r--r--   0 steve      (501) staff       (20)    14032 2024-02-11 16:22:35.000000 neural-amp-modeler-0.8.1/nam/models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     9259 2024-02-07 06:58:00.000000 neural-amp-modeler-0.8.1/nam/models/conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     2203 2023-10-09 15:24:53.000000 neural-amp-modeler-0.8.1/nam/models/linear.py
--rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural-amp-modeler-0.8.1/nam/models/losses.py
--rw-r--r--   0 steve      (501) staff       (20)     1215 2023-10-06 17:56:34.000000 neural-amp-modeler-0.8.1/nam/models/metadata.py
--rw-r--r--   0 steve      (501) staff       (20)    16557 2023-06-25 16:29:54.000000 neural-amp-modeler-0.8.1/nam/models/recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)    13969 2023-06-22 07:13:06.000000 neural-amp-modeler-0.8.1/nam/models/wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.532266 neural-amp-modeler-0.8.1/nam/train/
--rw-r--r--   0 steve      (501) staff       (20)      108 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/nam/train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      688 2024-02-10 19:50:23.000000 neural-amp-modeler-0.8.1/nam/train/_names.py
--rw-r--r--   0 steve      (501) staff       (20)      931 2024-02-10 19:50:23.000000 neural-amp-modeler-0.8.1/nam/train/_version.py
--rw-r--r--   0 steve      (501) staff       (20)     4095 2024-02-10 19:50:23.000000 neural-amp-modeler-0.8.1/nam/train/colab.py
--rw-r--r--   0 steve      (501) staff       (20)    43131 2024-02-10 19:50:23.000000 neural-amp-modeler-0.8.1/nam/train/core.py
--rw-r--r--   0 steve      (501) staff       (20)    21209 2023-11-07 01:38:12.000000 neural-amp-modeler-0.8.1/nam/train/gui.py
--rw-r--r--   0 steve      (501) staff       (20)     1075 2023-11-12 20:17:46.000000 neural-amp-modeler-0.8.1/nam/util.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.585944 neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      575 2024-02-11 16:25:01.000000 neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     1504 2024-02-11 16:25:01.000000 neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-02-11 16:25:01.000000 neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       42 2024-02-11 16:25:01.000000 neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      154 2024-02-11 16:25:01.000000 neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       10 2024-02-11 16:25:01.000000 neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-02-11 16:25:01.587706 neural-amp-modeler-0.8.1/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)     1451 2024-02-11 16:22:35.000000 neural-amp-modeler-0.8.1/setup.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.561618 neural-amp-modeler-0.8.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural-amp-modeler-0.8.1/tests/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.565228 neural-amp-modeler-0.8.1/tests/resources/
--rw-r--r--   0 steve      (501) staff       (20)     1021 2024-02-07 08:14:11.000000 neural-amp-modeler-0.8.1/tests/resources/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.566334 neural-amp-modeler-0.8.1/tests/test_bin/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.8.1/tests/test_bin/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.567508 neural-amp-modeler-0.8.1/tests/test_bin/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.8.1/tests/test_bin/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6568 2024-02-07 06:58:00.000000 neural-amp-modeler-0.8.1/tests/test_bin/test_train/test_main.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/tests/test_install.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.570448 neural-amp-modeler-0.8.1/tests/test_nam/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/tests/test_nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    14908 2024-02-07 06:58:00.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_data.py
--rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_importable.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.580909 neural-amp-modeler-0.8.1/tests/test_nam/test_models/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     4514 2024-01-13 03:07:09.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_base.py
--rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     4588 2023-04-25 01:51:12.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_losses.py
--rw-r--r--   0 steve      (501) staff       (20)     2360 2023-06-20 00:48:33.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-11 16:25:01.584663 neural-amp-modeler-0.8.1/tests/test_nam/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     8251 2024-02-07 08:14:11.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_train/test_core.py
--rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural-amp-modeler-0.8.1/tests/test_nam/test_train/test_version.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.812952 neural_amp_modeler-0.8.2/
+-rw-r--r--   0 steve      (501) staff       (20)     1072 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural_amp_modeler-0.8.2/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)      575 2024-05-14 05:40:19.812029 neural_amp_modeler-0.8.2/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      382 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.751000 neural_amp_modeler-0.8.2/nam/
+-rw-r--r--   0 steve      (501) staff       (20)      730 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural_amp_modeler-0.8.2/nam/_core.py
+-rw-r--r--   0 steve      (501) staff       (20)       22 2024-05-14 05:32:08.000000 neural_amp_modeler-0.8.2/nam/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)    27396 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/data.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.769847 neural_amp_modeler-0.8.2/nam/models/
+-rw-r--r--   0 steve      (501) staff       (20)      402 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural_amp_modeler-0.8.2/nam/models/_activations.py
+-rw-r--r--   0 steve      (501) staff       (20)     5891 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/models/_base.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/nam/models/_names.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.771322 neural_amp_modeler-0.8.2/nam/models/_resources/
+-rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural_amp_modeler-0.8.2/nam/models/_resources/loudness_input.wav
+-rw-r--r--   0 steve      (501) staff       (20)    14032 2024-02-11 16:22:35.000000 neural_amp_modeler-0.8.2/nam/models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     9259 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.2/nam/models/conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     4874 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/models/exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)     2203 2023-10-09 15:24:53.000000 neural_amp_modeler-0.8.2/nam/models/linear.py
+-rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural_amp_modeler-0.8.2/nam/models/losses.py
+-rw-r--r--   0 steve      (501) staff       (20)     1215 2023-10-06 17:56:34.000000 neural_amp_modeler-0.8.2/nam/models/metadata.py
+-rw-r--r--   0 steve      (501) staff       (20)    16557 2023-06-25 16:29:54.000000 neural_amp_modeler-0.8.2/nam/models/recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)    13969 2023-06-22 07:13:06.000000 neural_amp_modeler-0.8.2/nam/models/wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.781499 neural_amp_modeler-0.8.2/nam/train/
+-rw-r--r--   0 steve      (501) staff       (20)      251 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      693 2024-05-06 15:22:54.000000 neural_amp_modeler-0.8.2/nam/train/_names.py
+-rw-r--r--   0 steve      (501) staff       (20)      931 2024-02-10 19:50:23.000000 neural_amp_modeler-0.8.2/nam/train/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     4095 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/nam/train/colab.py
+-rw-r--r--   0 steve      (501) staff       (20)    45863 2024-05-13 15:33:11.000000 neural_amp_modeler-0.8.2/nam/train/core.py
+-rw-r--r--   0 steve      (501) staff       (20)    27403 2024-05-13 15:33:11.000000 neural_amp_modeler-0.8.2/nam/train/gui.py
+-rw-r--r--   0 steve      (501) staff       (20)     1075 2023-11-12 20:17:46.000000 neural_amp_modeler-0.8.2/nam/util.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.811092 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      575 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     1503 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       42 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      154 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       10 2024-05-14 05:40:19.000000 neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-14 05:40:19.813129 neural_amp_modeler-0.8.2/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)     1451 2024-02-11 16:22:35.000000 neural_amp_modeler-0.8.2/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.787523 neural_amp_modeler-0.8.2/tests/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural_amp_modeler-0.8.2/tests/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.788649 neural_amp_modeler-0.8.2/tests/resources/
+-rw-r--r--   0 steve      (501) staff       (20)     1021 2024-02-07 08:14:11.000000 neural_amp_modeler-0.8.2/tests/resources/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.790363 neural_amp_modeler-0.8.2/tests/test_bin/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural_amp_modeler-0.8.2/tests/test_bin/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.791346 neural_amp_modeler-0.8.2/tests/test_bin/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural_amp_modeler-0.8.2/tests/test_bin/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6568 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.2/tests/test_bin/test_train/test_main.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_install.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.795240 neural_amp_modeler-0.8.2/tests/test_nam/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    14908 2024-02-07 06:58:00.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_data.py
+-rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_importable.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.805601 neural_amp_modeler-0.8.2/tests/test_nam/test_models/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     4514 2024-01-13 03:07:09.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     4586 2024-05-13 06:04:29.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_losses.py
+-rw-r--r--   0 steve      (501) staff       (20)     2360 2023-06-20 00:48:33.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-14 05:40:19.809083 neural_amp_modeler-0.8.2/tests/test_nam/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     8251 2024-02-07 08:14:11.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_core.py
+-rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_version.py
```

### Comparing `neural-amp-modeler-0.8.1/LICENSE` & `neural_amp_modeler-0.8.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Steven Atkinson
+Copyright (c) 2024 Steven Atkinson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `neural-amp-modeler-0.8.1/PKG-INFO` & `neural_amp_modeler-0.8.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-amp-modeler
-Version: 0.8.1
+Version: 0.8.2
 Summary: Neural amp modeler
 Home-page: https://github.com/sdatkinson/
 Author: Steven Atkinson
 Author-email: steven@atkinson.mn
 License-File: LICENSE
 Requires-Dist: auraloss==0.3.0
 Requires-Dist: matplotlib
```

### Comparing `neural-amp-modeler-0.8.1/nam/__init__.py` & `neural_amp_modeler-0.8.2/nam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # File: __init__.py
 # File Created: Tuesday, 2nd February 2021 9:42:50 pm
 # Author: Steven Atkinson (steven@atkinson.mn)
 
+
 # Hack to recover graceful shutdowns in Windows.
 # This has to happen ASAP
 # See:
 # https://github.com/sdatkinson/neural-amp-modeler/issues/105
 # https://stackoverflow.com/a/44822794
 def _ensure_graceful_shutdowns():
     import os
```

### Comparing `neural-amp-modeler-0.8.1/nam/data.py` & `neural_amp_modeler-0.8.2/nam/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # File: data.py
 # Created Date: Saturday February 5th 2022
 # Author: Steven Atkinson (steven@atkinson.mn)
 
+"""
+Functions and classes for working with audio data with NAM
+"""
+
 import abc
 import logging
 from collections import namedtuple
 from copy import deepcopy
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
@@ -606,15 +610,19 @@
             msg = "Output clipped."
             if self._y_path is not None:
                 msg += f"Source is {self._y_path}"
             raise ValueError(msg)
 
     @classmethod
     def _validate_preceding_silence(
-        cls, x: torch.Tensor, start: Optional[int], silent_seconds: float, sample_rate: Optional[float]
+        cls,
+        x: torch.Tensor,
+        start: Optional[int],
+        silent_seconds: float,
+        sample_rate: Optional[float],
     ):
         """
         Make sure that the input is silent before the starting index.
         If it's not, then the output from that non-silent input will leak into the data
         set and couldn't be predicted!
 
         This assumes that silence is indeed required. If it's not, then don't call this!
```

### Comparing `neural-amp-modeler-0.8.1/nam/models/_base.py` & `neural_amp_modeler-0.8.2/nam/models/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from .._core import InitializableFromConfig
 from ..data import wav_to_tensor
-from ._exportable import Exportable
+from .exportable import Exportable
 
 
 class _Base(nn.Module, InitializableFromConfig, Exportable):
     def __init__(self, sample_rate: Optional[float] = None):
         super().__init__()
         self.register_buffer(
             "_has_sample_rate", torch.tensor(sample_rate is not None, dtype=torch.bool)
```

### Comparing `neural-amp-modeler-0.8.1/nam/models/_exportable.py` & `neural_amp_modeler-0.8.2/nam/models/exportable.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 
 class Exportable(abc.ABC):
     """
     Interface for my custon export format for use in the plugin.
     """
 
+    FILE_EXTENSION = ".nam"
+
     def export(
         self,
         outdir: Path,
         include_snapshot: bool = False,
         basename: str = "model",
         user_metadata: Optional[UserMetadata] = None,
     ):
@@ -62,15 +64,15 @@
         model_dict = self._get_export_dict()
         model_dict["metadata"].update(
             {} if user_metadata is None else _cast_enums(user_metadata.model_dump())
         )
 
         training = self.training
         self.eval()
-        with open(Path(outdir, f"{basename}.nam"), "w") as fp:
+        with open(Path(outdir, f"{basename}{self.FILE_EXTENSION}"), "w") as fp:
             json.dump(model_dict, fp)
         if include_snapshot:
             x, y = self._export_input_output()
             x_path = Path(outdir, "test_inputs.npy")
             y_path = Path(outdir, "test_outputs.npy")
             logger.debug(f"Saving snapshot input to {x_path}")
             np.save(x_path, x)
```

### Comparing `neural-amp-modeler-0.8.1/nam/models/_resources/loudness_input.wav` & `neural_amp_modeler-0.8.2/nam/models/_resources/loudness_input.wav`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/models/base.py` & `neural_amp_modeler-0.8.2/nam/models/base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/models/conv_net.py` & `neural_amp_modeler-0.8.2/nam/models/conv_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/models/linear.py` & `neural_amp_modeler-0.8.2/nam/models/linear.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/models/losses.py` & `neural_amp_modeler-0.8.2/nam/models/losses.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/models/metadata.py` & `neural_amp_modeler-0.8.2/nam/models/metadata.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/models/recurrent.py` & `neural_amp_modeler-0.8.2/nam/models/recurrent.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/models/wavenet.py` & `neural_amp_modeler-0.8.2/nam/models/wavenet.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/train/_names.py` & `neural_amp_modeler-0.8.2/nam/train/_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class VersionAndName(NamedTuple):
     version: Version
     name: str
 
 
-# From most the least recently-released
+# From most- to the least-recently-released:
 INPUT_BASENAMES = (
     VersionAndName(Version(3, 0, 0), "v3_0_0.wav"),
     VersionAndName(Version(2, 0, 0), "v2_0_0.wav"),
     VersionAndName(Version(1, 1, 1), "v1_1_1.wav"),
     VersionAndName(Version(1, 0, 0), "v1.wav"),
     VersionAndName(PROTEUS_VERSION, "Proteus_Capture.wav"),
 )
```

### Comparing `neural-amp-modeler-0.8.1/nam/train/_version.py` & `neural_amp_modeler-0.8.2/nam/train/_version.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/nam/train/colab.py` & `neural_amp_modeler-0.8.2/nam/train/colab.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     lr_decay: float = 0.007,
     seed: Optional[int] = 0,
     user_metadata: Optional[UserMetadata] = None,
     ignore_checks: bool = False,
     fit_cab: bool = False,
 ):
     """
-    :param epochs: How amny epochs we'll train for.
+    :param epochs: How many epochs we'll train for.
     :param delay: How far the output algs the input due to round-trip latency during
         reamping, in samples.
     :param stage_1_channels: The number of channels in the WaveNet's first stage.
     :param stage_2_channels: The number of channels in the WaveNet's second stage.
     :param lr: The initial learning rate
     :param lr_decay: The amount by which the learning rate decays each epoch
     :param seed: RNG seed for reproducibility.
```

### Comparing `neural-amp-modeler-0.8.1/nam/train/core.py` & `neural_amp_modeler-0.8.2/nam/train/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 """
 
 import hashlib
 import tkinter as tk
 from copy import deepcopy
 from enum import Enum
 from functools import partial
+from pathlib import Path
 from time import time
 from typing import Dict, Optional, Sequence, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from pydantic import BaseModel
 from pytorch_lightning.utilities.warnings import PossibleUserWarning
 from torch.utils.data import DataLoader
 
 from ..data import Split, init_dataset, wav_to_np, wav_to_tensor
 from ..models import Model
+from ..models.exportable import Exportable
 from ..models.losses import esr
+from ..models.metadata import UserMetadata
 from ..util import filter_warnings
 from ._version import PROTEUS_VERSION, Version
 
 __all__ = ["train"]
 
 # Training using the simplified trainers in NAM is done at 48k.
 STANDARD_SAMPLE_RATE = 48_000.0
@@ -1075,14 +1078,91 @@
         command=lambda: [modal.destroy(), root.quit()],
     )
     ok_button.pack()
     modal.grab_set()  # disable interaction with root window while modal is open
     modal.mainloop()
 
 
+class _ValidationStopping(pl.callbacks.EarlyStopping):
+    """
+    Callback to indicate to stop training if the validation metric is good enough,
+    without the other conditions that EarlyStopping usually forces like patience.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.patience = np.inf
+
+
+class _ModelCheckpoint(pl.callbacks.model_checkpoint.ModelCheckpoint):
+    """
+    Extension to model checkpoint to save a .nam file as well as the .ckpt file.
+    """
+
+    def __init__(self, *args, user_metadata: Optional[UserMetadata] = None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._user_metadata = user_metadata
+
+    _NAM_FILE_EXTENSION = Exportable.FILE_EXTENSION
+
+    @classmethod
+    def _get_nam_filepath(cls, filepath: str) -> Path:
+        """
+        Given a .ckpt filepath, figure out a .nam for it.
+        """
+        if not filepath.endswith(cls.FILE_EXTENSION):
+            raise ValueError(
+                f"Checkpoint filepath {filepath} doesn't end in expected extension "
+                f"{cls.FILE_EXTENSION}"
+            )
+        return Path(filepath[: -len(cls.FILE_EXTENSION)] + cls._NAM_FILE_EXTENSION)
+
+    def _save_checkpoint(self, trainer: pl.Trainer, filepath: str):
+        # Save the .ckpt:
+        super()._save_checkpoint(trainer, filepath)
+        # Save the .nam:
+        nam_filepath = self._get_nam_filepath(filepath)
+        pl_model: Model = trainer.model
+        nam_model = pl_model.net
+        outdir = nam_filepath.parent
+        # HACK: Assume the extension
+        basename = nam_filepath.name[: -len(self._NAM_FILE_EXTENSION)]
+        nam_model.export(outdir, basename=basename, user_metadata=self._user_metadata)
+
+    def _remove_checkpoint(self, trainer: pl.Trainer, filepath: str) -> None:
+        super()._remove_checkpoint(trainer, filepath)
+        nam_path = self._get_nam_filepath(filepath)
+        if nam_path.exists():
+            nam_path.unlink()
+
+
+def _get_callbacks(
+    threshold_esr: Optional[float], user_metadata: Optional[UserMetadata] = None
+):
+    callbacks = [
+        _ModelCheckpoint(
+            filename="checkpoint_best_{epoch:04d}_{step}_{ESR:.4g}_{MSE:.3e}",
+            save_top_k=3,
+            monitor="val_loss",
+            every_n_epochs=1,
+            user_metadata=user_metadata,
+        ),
+        _ModelCheckpoint(
+            filename="checkpoint_last_{epoch:04d}_{step}",
+            every_n_epochs=1,
+            user_metadata=user_metadata,
+        ),
+    ]
+    if threshold_esr is not None:
+        callbacks.append(
+            _ValidationStopping(monitor="ESR", stopping_threshold=threshold_esr)
+        )
+    return callbacks
+
+
 def train(
     input_path: str,
     output_path: str,
     train_path: str,
     input_version: Optional[Version] = None,
     epochs=100,
     delay=None,
@@ -1095,15 +1175,21 @@
     seed: Optional[int] = 0,
     save_plot: bool = False,
     silent: bool = False,
     modelname: str = "model",
     ignore_checks: bool = False,
     local: bool = False,
     fit_cab: bool = False,
+    threshold_esr: Optional[bool] = None,
+    user_metadata: Optional[UserMetadata] = None,
 ) -> Optional[Model]:
+    """
+    :param threshold_esr: Stop training if ESR is better than this. Ignore if `None`.
+    """
+
     if seed is not None:
         torch.manual_seed(seed)
 
     if input_version is None:
         input_version, strong_match = _detect_input_version(input_path)
 
     if delay is None:
@@ -1158,27 +1244,19 @@
     )
     if train_dataloader.dataset.sample_rate != val_dataloader.dataset.sample_rate:
         raise RuntimeError(
             "Train and validation data loaders have different data set sample rates: "
             f"{train_dataloader.dataset.sample_rate}, "
             f"{val_dataloader.dataset.sample_rate}"
         )
+    sample_rate = train_dataloader.dataset.sample_rate
+    model.net.sample_rate = sample_rate
 
     trainer = pl.Trainer(
-        callbacks=[
-            pl.callbacks.model_checkpoint.ModelCheckpoint(
-                filename="checkpoint_best_{epoch:04d}_{step}_{ESR:.4g}_{MSE:.3e}",
-                save_top_k=3,
-                monitor="val_loss",
-                every_n_epochs=1,
-            ),
-            pl.callbacks.model_checkpoint.ModelCheckpoint(
-                filename="checkpoint_last_{epoch:04d}_{step}", every_n_epochs=1
-            ),
-        ],
+        callbacks=_get_callbacks(threshold_esr, user_metadata=user_metadata),
         default_root_dir=train_path,
         **learning_config["trainer"],
     )
     # Suppress the PossibleUserWarning about num_workers (Issue 345)
     with filter_warnings("ignore", category=PossibleUserWarning):
         trainer.fit(model, train_dataloader, val_dataloader)
 
@@ -1187,15 +1265,15 @@
     if best_checkpoint != "":
         model = Model.load_from_checkpoint(
             trainer.checkpoint_callback.best_model_path,
             **Model.parse_config(model_config),
         )
     model.cpu()
     model.eval()
-    model.net.sample_rate = train_dataloader.dataset.sample_rate
+    model.net.sample_rate = sample_rate  # Hack, part 2
 
     def window_kwargs(version: Version):
         if version.major == 1:
             return dict(
                 window_start=100_000,  # Start of the plotting window, in samples
                 window_end=101_000,  # End of the plotting window, in samples
             )
```

### Comparing `neural-amp-modeler-0.8.1/nam/train/gui.py` & `neural_amp_modeler-0.8.2/nam/train/gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
 
 
 _ensure_graceful_shutdowns()
 
 import re
 import tkinter as tk
+import webbrowser
 from dataclasses import dataclass
 from enum import Enum
 from functools import partial
 from pathlib import Path
 from tkinter import filedialog
 from typing import Callable, Dict, Optional, Sequence
 
@@ -38,15 +39,15 @@
     import torch
 
     from nam import __version__
     from nam.train import core
     from nam.models.metadata import GearType, UserMetadata, ToneType
 
     # Ok private access here--this is technically allowed access
-    from nam.train._names import LATEST_VERSION
+    from nam.train._names import INPUT_BASENAMES, LATEST_VERSION
 
     _install_is_valid = True
     _HAVE_ACCELERATOR = torch.cuda.is_available() or torch.backends.mps.is_available()
 except ImportError:
     _install_is_valid = False
     _HAVE_ACCELERATOR = False
 
@@ -60,26 +61,38 @@
     _DEFAULT_LR_DECAY = 0.05
 _BUTTON_WIDTH = 20
 _BUTTON_HEIGHT = 2
 _TEXT_WIDTH = 70
 
 _DEFAULT_DELAY = None
 _DEFAULT_IGNORE_CHECKS = False
+_DEFAULT_THRESHOLD_ESR = None
 
 _ADVANCED_OPTIONS_LEFT_WIDTH = 12
 _ADVANCED_OPTIONS_RIGHT_WIDTH = 12
 _METADATA_RIGHT_WIDTH = 60
 
 
 @dataclass
 class _AdvancedOptions(object):
+    """
+    :param architecture: Which architecture to use.
+    :param num_epochs: How many epochs to train for.
+    :param latency: Latency between the input and output audio, in samples.
+        None means we don't know and it has to be calibrated.
+    :param ignore_checks: Keep going even if a check says that something is wrong.
+    :param threshold_esr: Stop training if the ESR gets better than this. If None, don't
+        stop.
+    """
+
     architecture: core.Architecture
     num_epochs: int
-    delay: Optional[int]
+    latency: Optional[int]
     ignore_checks: bool
+    threshold_esr: Optional[float]
 
 
 class _PathType(Enum):
     FILE = "file"
     DIRECTORY = "directory"
     MULTIFILE = "multifile"
 
@@ -92,53 +105,75 @@
     def __init__(
         self,
         frame: tk.Frame,
         button_text: str,
         info_str: str,
         path_type: _PathType,
         hooks: Optional[Sequence[Callable[[], None]]] = None,
+        color_when_not_set: str = "#EF0000",  # Darker red
+        default: Optional[Path] = None,
     ):
+        """
+        :param hooks: Callables run at the end of setting the value.
+        """
         self._button_text = button_text
         self._info_str = info_str
-        self._path: Optional[Path] = None
+        self._path: Optional[Path] = default
         self._path_type = path_type
-        self._button = tk.Button(
-            frame,
+        self._frame = frame
+        self._widgets = {}
+        self._widgets["button"] = tk.Button(
+            self._frame,
             text=button_text,
             width=_BUTTON_WIDTH,
             height=_BUTTON_HEIGHT,
             fg="black",
             command=self._set_val,
         )
-        self._button.pack(side=tk.LEFT)
-        self._label = tk.Label(
-            frame,
+        self._widgets["button"].pack(side=tk.LEFT)
+        self._widgets["label"] = tk.Label(
+            self._frame,
             width=_TEXT_WIDTH,
             height=_BUTTON_HEIGHT,
             fg="black",
             bg=None,
             anchor="w",
         )
-        self._label.pack(side=tk.RIGHT)
+        self._widgets["label"].pack(side=tk.LEFT)
         self._hooks = hooks
+        self._color_when_not_set = color_when_not_set
         self._set_text()
 
+    def __setitem__(self, key, val):
+        """
+        Implement tk-style setter for state
+        """
+        if key == "state":
+            for widget in self._widgets.values():
+                widget["state"] = val
+        else:
+            raise RuntimeError(
+                f"{self.__class__.__name__} instance does not support item assignment for non-state key {key}!"
+            )
+
     @property
     def val(self) -> Optional[Path]:
         return self._path
 
     def _set_text(self):
         if self._path is None:
-            self._label["fg"] = "red"
-            self._label["text"] = self._info_str
+            self._widgets["label"]["fg"] = self._color_when_not_set
+            self._widgets["label"]["text"] = self._info_str
         else:
             val = self.val
             val = val[0] if isinstance(val, tuple) and len(val) == 1 else val
-            self._label["fg"] = "black"
-            self._label["text"] = f"{self._button_text.capitalize()} set to {val}"
+            self._widgets["label"]["fg"] = "black"
+            self._widgets["label"][
+                "text"
+            ] = f"{self._button_text.capitalize()} set to {val}"
 
     def _set_val(self):
         res = {
             _PathType.FILE: filedialog.askopenfilename,
             _PathType.DIRECTORY: filedialog.askdirectory,
             _PathType.MULTIFILE: filedialog.askopenfilenames,
         }[self._path_type]()
@@ -147,131 +182,231 @@
         self._set_text()
 
         if self._hooks is not None:
             for h in self._hooks:
                 h()
 
 
+class _InputPathButton(_PathButton):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # Download the training file!
+        self._widgets["button_download_input"] = tk.Button(
+            self._frame,
+            text="Download input file",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._download_input_file,
+        )
+        self._widgets["button_download_input"].pack(side=tk.RIGHT)
+
+    @classmethod
+    def _download_input_file(cls):
+        file_urls = {
+            "v3_0_0.wav": "https://drive.google.com/file/d/1Pgf8PdE0rKB1TD4TRPKbpNo1ByR3IOm9/view?usp=drive_link",
+            "v2_0_0.wav": "https://drive.google.com/file/d/1xnyJP_IZ7NuyDSTJfn-Jmc5lw0IE7nfu/view?usp=drive_link",
+            "v1_1_1.wav": "",
+            "v1.wav": "",
+        }
+        # Pick the most recent file.
+        for input_basename in INPUT_BASENAMES:
+            name = input_basename.name
+            url = file_urls.get(name)
+            if url:
+                if name != LATEST_VERSION.name:
+                    print(
+                        f"WARNING: File {name} is out of date. "
+                        "This needs to be updated!"
+                    )
+                webbrowser.open(url)
+                return
+
+
+class _ClearablePathButton(_PathButton):
+    """
+    Can clear a path
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, color_when_not_set="black", **kwargs)
+        # Download the training file!
+        self._widgets["button_clear"] = tk.Button(
+            self._frame,
+            text="Clear",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._clear_path,
+        )
+        self._widgets["button_clear"].pack(side=tk.RIGHT)
+
+    def _clear_path(self):
+        self._path = None
+        self._set_text()
+
+
 class _CheckboxKeys(Enum):
     """
     Keys for checkboxes
     """
 
     FIT_CAB = "fit_cab"
     SILENT_TRAINING = "silent_training"
     SAVE_PLOT = "save_plot"
     IGNORE_DATA_CHECKS = "ignore_data_checks"
 
 
+class _BasicModal(object):
+    """
+    Message and OK button
+    """
+
+    def __init__(self, resume_main, msg: str):
+        self._root = tk.Toplevel()
+        self._text = tk.Label(self._root, text=msg)
+        self._text.pack()
+        self._ok = tk.Button(
+            self._root,
+            text="Ok",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._close,
+        )
+        self._ok.pack()
+        self._resume_main = resume_main
+
+    def _close(self):
+        self._root.destroy()
+        self._resume_main()
+
+
+class _GUIWidgets(Enum):
+    INPUT_PATH = "input_path"
+    OUTPUT_PATH = "output_path"
+    TRAINING_DESTINATION = "training_destination"
+    METADATA = "metadata"
+    ADVANCED_OPTIONS = "advanced_options"
+    TRAIN = "train"
+
+
 class _GUI(object):
     def __init__(self):
         self._root = tk.Tk()
         self._root.title(f"NAM Trainer - v{__version__}")
+        self._widgets = {}
 
         # Buttons for paths:
-        self._frame_input_path = tk.Frame(self._root)
-        self._frame_input_path.pack()
-        self._path_button_input = _PathButton(
-            self._frame_input_path,
+        self._frame_input = tk.Frame(self._root)
+        self._frame_input.pack(anchor="w")
+        self._widgets[_GUIWidgets.INPUT_PATH] = _InputPathButton(
+            self._frame_input,
             "Input Audio",
-            f"Select input DI file (e.g. {LATEST_VERSION.name})",
+            f"Select input (DI) file (e.g. {LATEST_VERSION.name})",
             _PathType.FILE,
             hooks=[self._check_button_states],
         )
 
         self._frame_output_path = tk.Frame(self._root)
-        self._frame_output_path.pack()
-        self._path_button_output = _PathButton(
+        self._frame_output_path.pack(anchor="w")
+        self._widgets[_GUIWidgets.OUTPUT_PATH] = _PathButton(
             self._frame_output_path,
             "Output Audio",
-            "Select output (reamped) audio - choose multiple files to enable batch training",
+            "Select output (reamped) file - (Choose MULTIPLE FILES to enable BATCH TRAINING)",
             _PathType.MULTIFILE,
             hooks=[self._check_button_states],
         )
 
         self._frame_train_destination = tk.Frame(self._root)
-        self._frame_train_destination.pack()
-        self._path_button_train_destination = _PathButton(
+        self._frame_train_destination.pack(anchor="w")
+        self._widgets[_GUIWidgets.TRAINING_DESTINATION] = _PathButton(
             self._frame_train_destination,
             "Train Destination",
             "Select training output directory",
             _PathType.DIRECTORY,
             hooks=[self._check_button_states],
         )
 
         # Metadata
         self.user_metadata = UserMetadata()
         self._frame_metadata = tk.Frame(self._root)
-        self._frame_metadata.pack()
-        self._button_metadata = tk.Button(
+        self._frame_metadata.pack(anchor="w")
+        self._widgets["metadata"] = tk.Button(
             self._frame_metadata,
             text="Metadata...",
             width=_BUTTON_WIDTH,
             height=_BUTTON_HEIGHT,
             fg="black",
             command=self._open_metadata,
         )
-        self._button_metadata.pack()
+        self._widgets["metadata"].pack()
         self.user_metadata_flag = False
 
         # This should probably be to the right somewhere
         self._get_additional_options_frame()
 
+        # Last frames: avdanced options & train in the SE corner:
+        self._frame_advanced_options = tk.Frame(self._root)
+        self._frame_train = tk.Frame(self._root)
+        # Pack train first so that it's on bottom.
+        self._frame_train.pack(side=tk.BOTTOM, anchor="e")
+        self._frame_advanced_options.pack(side=tk.BOTTOM, anchor="e")
+
         # Advanced options for training
         default_architecture = core.Architecture.STANDARD
         self.advanced_options = _AdvancedOptions(
             default_architecture,
             _DEFAULT_NUM_EPOCHS,
             _DEFAULT_DELAY,
             _DEFAULT_IGNORE_CHECKS,
+            _DEFAULT_THRESHOLD_ESR,
         )
         # Window to edit them:
-        self._frame_advanced_options = tk.Frame(self._root)
-        self._frame_advanced_options.pack()
-        self._button_advanced_options = tk.Button(
+
+        self._widgets[_GUIWidgets.ADVANCED_OPTIONS] = tk.Button(
             self._frame_advanced_options,
             text="Advanced options...",
             width=_BUTTON_WIDTH,
             height=_BUTTON_HEIGHT,
             fg="black",
             command=self._open_advanced_options,
         )
-        self._button_advanced_options.pack()
+        self._widgets[_GUIWidgets.ADVANCED_OPTIONS].pack()
 
         # Train button
-        self._frame_train = tk.Frame(self._root)
-        self._frame_train.pack()
-        self._button_train = tk.Button(
+
+        self._widgets[_GUIWidgets.TRAIN] = tk.Button(
             self._frame_train,
             text="Train",
             width=_BUTTON_WIDTH,
             height=_BUTTON_HEIGHT,
             fg="black",
             command=self._train,
         )
-        self._button_train.pack()
+        self._widgets[_GUIWidgets.TRAIN].pack()
 
         self._check_button_states()
 
     def _check_button_states(self):
         """
         Determine if any buttons should be disabled
         """
         # Train button is disabled unless all paths are set
         if any(
             pb.val is None
             for pb in (
-                self._path_button_input,
-                self._path_button_output,
-                self._path_button_train_destination,
+                self._widgets[_GUIWidgets.INPUT_PATH],
+                self._widgets[_GUIWidgets.OUTPUT_PATH],
+                self._widgets[_GUIWidgets.TRAINING_DESTINATION],
             )
         ):
-            self._button_train["state"] = tk.DISABLED
+            self._widgets[_GUIWidgets.TRAIN]["state"] = tk.DISABLED
             return
-        self._button_train["state"] = tk.NORMAL
+        self._widgets[_GUIWidgets.TRAIN]["state"] = tk.NORMAL
 
     def _get_additional_options_frame(self):
         # Checkboxes
         # TODO get these definitions into __init__()
         self._frame_checkboxes = tk.Frame(self._root)
         self._frame_checkboxes.pack(side=tk.LEFT)
         row = 1
@@ -286,14 +421,15 @@
         ) -> Checkbox:
             variable = tk.BooleanVar()
             variable.set(default_value)
             check_button = tk.Checkbutton(
                 self._frame_checkboxes, text=text, variable=variable
             )
             self._checkboxes[key] = Checkbox(variable, check_button)
+            self._widgets[key] = check_button  # For tracking in set-all-widgets ops
 
         self._checkboxes: Dict[_CheckboxKeys, Checkbox] = dict()
         make_checkbox(_CheckboxKeys.FIT_CAB, "Cab modeling", False)
         make_checkbox(
             _CheckboxKeys.SILENT_TRAINING,
             "Silent run (suggested for batch training)",
             False,
@@ -310,55 +446,67 @@
         for v in self._checkboxes.values():
             v.check_button.grid(row=row, column=1, sticky="W")
             row += 1
 
     def mainloop(self):
         self._root.mainloop()
 
+    def _disable(self):
+        self._set_all_widget_states_to(tk.DISABLED)
+
     def _open_advanced_options(self):
         """
-        Open advanced options
+        Open window for advanced options
         """
-        ao = _AdvancedOptionsGUI(self)
-        # I should probably disable the main GUI...
-        ao.mainloop()
-        # ...and then re-enable it once it gets closed.
+
+        self._wait_while_func(lambda resume: _AdvancedOptionsGUI(resume, self))
 
     def _open_metadata(self):
         """
-        Open dialog for metadata
+        Open window for metadata
         """
-        mdata = _UserMetadataGUI(self)
-        # I should probably disable the main GUI...
-        mdata.mainloop()
+
+        self._wait_while_func(lambda resume: _UserMetadataGUI(resume, self))
+
+    def _resume(self):
+        self._set_all_widget_states_to(tk.NORMAL)
+        self._check_button_states()
+
+    def _set_all_widget_states_to(self, state):
+        for widget in self._widgets.values():
+            widget["state"] = state
 
     def _train(self):
         # Advanced options:
         num_epochs = self.advanced_options.num_epochs
         architecture = self.advanced_options.architecture
-        delay = self.advanced_options.delay
-        file_list = self._path_button_output.val
+        delay = self.advanced_options.latency
+        file_list = self._widgets[_GUIWidgets.OUTPUT_PATH].val
+        threshold_esr = self.advanced_options.threshold_esr
 
         # Advanced-er options
         # If you're poking around looking for these, then maybe it's time to learn to
         # use the command-line scripts ;)
         lr = 0.004
         lr_decay = _DEFAULT_LR_DECAY
         batch_size = _DEFAULT_BATCH_SIZE
         seed = 0
 
         # Run it
         for file in file_list:
             print("Now training {}".format(file))
             basename = re.sub(r"\.wav$", "", file.split("/")[-1])
+            user_metadata = (
+                self.user_metadata if self.user_metadata_flag else UserMetadata()
+            )
 
             trained_model = core.train(
-                self._path_button_input.val,
+                self._widgets[_GUIWidgets.INPUT_PATH].val,
                 file,
-                self._path_button_train_destination.val,
+                self._widgets[_GUIWidgets.TRAINING_DESTINATION].val,
                 epochs=num_epochs,
                 delay=delay,
                 architecture=architecture,
                 batch_size=batch_size,
                 lr=lr,
                 lr_decay=lr_decay,
                 seed=seed,
@@ -366,52 +514,64 @@
                 save_plot=self._checkboxes[_CheckboxKeys.SAVE_PLOT].variable.get(),
                 modelname=basename,
                 ignore_checks=self._checkboxes[
                     _CheckboxKeys.IGNORE_DATA_CHECKS
                 ].variable.get(),
                 local=True,
                 fit_cab=self._checkboxes[_CheckboxKeys.FIT_CAB].variable.get(),
+                threshold_esr=threshold_esr,
+                user_metadata=user_metadata,
             )
+
             if trained_model is None:
                 print("Model training failed! Skip exporting...")
                 continue
             print("Model training complete!")
             print("Exporting...")
-            outdir = self._path_button_train_destination.val
+            outdir = self._widgets[_GUIWidgets.TRAINING_DESTINATION].val
             print(f"Exporting trained model to {outdir}...")
             trained_model.net.export(
-                outdir,
-                basename=basename,
-                user_metadata=self.user_metadata
-                if self.user_metadata_flag
-                else UserMetadata(),
+                outdir, basename=basename, user_metadata=user_metadata
             )
             print("Done!")
 
         # Metadata was only valid for 1 run, so make sure it's not used again unless
         # the user re-visits the window and clicks "ok"
         self.user_metadata_flag = False
 
+    def _wait_while_func(self, func, *args, **kwargs):
+        """
+        Disable this GUI while something happens.
+        That function _needs_ to call the provided self._resume when it's ready to
+        release me!
+        """
+        self._disable()
+        func(self._resume, *args, **kwargs)
+
 
 # some typing functions
 def _non_negative_int(val):
     val = int(val)
     if val < 0:
         val = 0
     return val
 
 
-def _int_or_null(val):
+def _type_or_null(T, val):
     val = val.rstrip()
     if val == "null":
         return val
-    return int(val)
+    return T(val)
+
+
+_int_or_null = partial(_type_or_null, int)
+_float_or_null = partial(_type_or_null, float)
 
 
-def _int_or_null_inv(val):
+def _type_or_null_inv(val):
     return "null" if val is None else str(val)
 
 
 def _rstripped_str(val):
     return str(val).rstrip()
 
 
@@ -528,17 +688,18 @@
 
 
 class _AdvancedOptionsGUI(object):
     """
     A window to hold advanced options (Architecture and number of epochs)
     """
 
-    def __init__(self, parent: _GUI):
+    def __init__(self, resume_main, parent: _GUI):
+        self._resume_main = resume_main
         self._parent = parent
-        self._root = tk.Tk()
+        self._root = tk.Toplevel()
         self._root.title("Advanced Options")
 
         # Architecture: radio buttons
         self._frame_architecture = tk.Frame(self._root)
         self._frame_architecture.pack()
         self._architecture = _LabeledOptionMenu(
             self._frame_architecture,
@@ -555,60 +716,76 @@
             self._frame_epochs,
             "Epochs",
             default=str(self._parent.advanced_options.num_epochs),
             type=_non_negative_int,
         )
 
         # Delay: text box
-        self._frame_delay = tk.Frame(self._root)
-        self._frame_delay.pack()
+        self._frame_latency = tk.Frame(self._root)
+        self._frame_latency.pack()
 
-        self._delay = _LabeledText(
-            self._frame_delay,
-            "Delay",
-            default=_int_or_null_inv(self._parent.advanced_options.delay),
+        self._latency = _LabeledText(
+            self._frame_latency,
+            "Reamp latency",
+            default=_type_or_null_inv(self._parent.advanced_options.latency),
             type=_int_or_null,
         )
 
+        # Threshold ESR
+        self._frame_threshold_esr = tk.Frame(self._root)
+        self._frame_threshold_esr.pack()
+        self._threshold_esr = _LabeledText(
+            self._frame_threshold_esr,
+            "Threshold ESR",
+            default=_type_or_null_inv(self._parent.advanced_options.threshold_esr),
+            type=_float_or_null,
+        )
+
         # "Ok": apply and destory
         self._frame_ok = tk.Frame(self._root)
         self._frame_ok.pack()
         self._button_ok = tk.Button(
             self._frame_ok,
             text="Ok",
             width=_BUTTON_WIDTH,
             height=_BUTTON_HEIGHT,
             fg="black",
             command=self._apply_and_destroy,
         )
         self._button_ok.pack()
 
-    def mainloop(self):
-        self._root.mainloop()
-
     def _apply_and_destroy(self):
         """
         Set values to parent and destroy this object
         """
         self._parent.advanced_options.architecture = self._architecture.get()
         epochs = self._epochs.get()
         if epochs is not None:
             self._parent.advanced_options.num_epochs = epochs
-        delay = self._delay.get()
+        latency = self._latency.get()
         # Value None is returned as "null" to disambiguate from non-set.
-        if delay is not None:
-            self._parent.advanced_options.delay = None if delay == "null" else delay
+        if latency is not None:
+            self._parent.advanced_options.latency = (
+                None if latency == "null" else latency
+            )
+        threshold_esr = self._threshold_esr.get()
+        if threshold_esr is not None:
+            self._parent.advanced_options.threshold_esr = (
+                None if threshold_esr == "null" else threshold_esr
+            )
         self._root.destroy()
+        self._resume_main()
 
 
 class _UserMetadataGUI(object):
     # Things that are auto-filled:
     # Model date
     # gain
-    def __init__(self, parent: _GUI):
+    def __init__(self, resume_main, parent: _GUI):
+        self._resume_main = resume_main
         self._parent = parent
         self._root = tk.Tk()
         self._root.title("Metadata")
 
         LabeledText = partial(_LabeledText, right_width=_METADATA_RIGHT_WIDTH)
 
         # Name
@@ -675,30 +852,28 @@
             width=_BUTTON_WIDTH,
             height=_BUTTON_HEIGHT,
             fg="black",
             command=self._apply_and_destroy,
         )
         self._button_ok.pack()
 
-    def mainloop(self):
-        self._root.mainloop()
-
     def _apply_and_destroy(self):
         """
         Set values to parent and destroy this object
         """
         self._parent.user_metadata.name = self._name.get()
         self._parent.user_metadata.modeled_by = self._modeled_by.get()
         self._parent.user_metadata.gear_make = self._gear_make.get()
         self._parent.user_metadata.gear_model = self._gear_model.get()
         self._parent.user_metadata.gear_type = self._gear_type.get()
         self._parent.user_metadata.tone_type = self._tone_type.get()
         self._parent.user_metadata_flag = True
 
         self._root.destroy()
+        self._resume_main()
 
 
 def _install_error():
     window = tk.Tk()
     window.title("ERROR")
     label = tk.Label(
         window,
```

### Comparing `neural-amp-modeler-0.8.1/nam/util.py` & `neural_amp_modeler-0.8.2/nam/util.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/PKG-INFO` & `neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-amp-modeler
-Version: 0.8.1
+Version: 0.8.2
 Summary: Neural amp modeler
 Home-page: https://github.com/sdatkinson/
 Author: Steven Atkinson
 Author-email: steven@atkinson.mn
 License-File: LICENSE
 Requires-Dist: auraloss==0.3.0
 Requires-Dist: matplotlib
```

### Comparing `neural-amp-modeler-0.8.1/neural_amp_modeler.egg-info/SOURCES.txt` & `neural_amp_modeler-0.8.2/neural_amp_modeler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 nam/_core.py
 nam/_version.py
 nam/data.py
 nam/util.py
 nam/models/__init__.py
 nam/models/_activations.py
 nam/models/_base.py
-nam/models/_exportable.py
 nam/models/_names.py
 nam/models/base.py
 nam/models/conv_net.py
+nam/models/exportable.py
 nam/models/linear.py
 nam/models/losses.py
 nam/models/metadata.py
 nam/models/recurrent.py
 nam/models/wavenet.py
 nam/models/_resources/loudness_input.wav
 nam/train/__init__.py
```

### Comparing `neural-amp-modeler-0.8.1/setup.py` & `neural_amp_modeler-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/resources/__init__.py` & `neural_amp_modeler-0.8.2/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_bin/test_train/test_main.py` & `neural_amp_modeler-0.8.2/tests/test_bin/test_train/test_main.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_data.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_data.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_models/base.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_models/base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_base.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_conv_net.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_conv_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_exportable.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_exportable.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from typing import Optional, Tuple
 
 import numpy as np
 import pytest
 import torch
 import torch.nn as nn
 
-from nam.models import _exportable
+from nam.models import exportable
 from nam.models import metadata
 
 
 class TestExportable(object):
     def test_export(self):
         """
         Does it work?
@@ -101,15 +101,15 @@
                 assert preds == pytest.approx(y)
             else:
                 assert not input_path.exists()
                 assert not output_path.exists()
 
     @classmethod
     def _get_model(cls):
-        class Model(nn.Module, _exportable.Exportable):
+        class Model(nn.Module, exportable.Exportable):
             def __init__(self):
                 super().__init__()
                 self._scale = nn.Parameter(torch.tensor(0.0))
                 self._bias = nn.Parameter(torch.tensor(0.0))
 
             def forward(self, x: torch.Tensor):
                 return self._scale * x + self._bias
```

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_losses.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_losses.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_recurrent.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_recurrent.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_models/test_wavenet.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_models/test_wavenet.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_train/test_core.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_core.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.8.1/tests/test_nam/test_train/test_version.py` & `neural_amp_modeler-0.8.2/tests/test_nam/test_train/test_version.py`

 * *Files identical despite different names*

