# Comparing `tmp/zoobot-2.0.0.tar.gz` & `tmp/zoobot-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoobot-2.0.0.tar", last modified: Thu Apr  4 19:51:51 2024, max compression
+gzip compressed data, was "zoobot-2.0.1.tar", last modified: Tue May 14 20:07:45 2024, max compression
```

## Comparing `zoobot-2.0.0.tar` & `zoobot-2.0.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:51.006094 zoobot-2.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-04-04 19:51:42.000000 zoobot-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-04-04 19:51:51.006094 zoobot-2.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    12454 2024-04-04 19:51:42.000000 zoobot-2.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-04-04 19:51:42.000000 zoobot-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:51:51.010094 zoobot-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4602 2024-04-04 19:51:42.000000 zoobot-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.990094 zoobot-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-04 19:51:42.000000 zoobot-2.0.0/tests/test_from_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-04 19:51:42.000000 zoobot-2.0.0/tests/test_loss_equivalence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.990094 zoobot-2.0.0/zoobot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/datasets/webdatamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/datasets/webdataset_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/cuda_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22399 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3188 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/efficientnet_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/manchester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/predictions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/predictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/predictions/predict_on_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38788 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6800 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/representations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/tensorboard_writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19378 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/train_with_pytorch_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/shared/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/benchmark_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4437 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/compress_representations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/label_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/load_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/save_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12868 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/estimators/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2508 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/alexnet_baseline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1795 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/custom_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7227 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2300 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_custom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    84167 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_standard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/small_cnn_baseline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/predictions/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/predictions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3417 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/predictions/predict_on_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5239 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/stats/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14433 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/dirichlet_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3526 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/mixture_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:51.002094 zoobot-2.0.0/zoobot/tensorflow/training/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6865 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/train_with_keras.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6505 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/training_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:51.002094 zoobot-2.0.0/zoobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.504405 zoobot-2.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-14 20:07:34.000000 zoobot-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-05-14 20:07:45.504405 zoobot-2.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11796 2024-05-14 20:07:34.000000 zoobot-2.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-14 20:07:34.000000 zoobot-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:07:45.504405 zoobot-2.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4602 2024-05-14 20:07:34.000000 zoobot-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.488405 zoobot-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 20:07:34.000000 zoobot-2.0.1/tests/test_from_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-14 20:07:34.000000 zoobot-2.0.1/tests/test_loss_equivalence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.488405 zoobot-2.0.1/zoobot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.488405 zoobot-2.0.1/zoobot/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.492405 zoobot-2.0.1/zoobot/pytorch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/datasets/webdatamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/datasets/webdataset_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.492405 zoobot-2.0.1/zoobot/pytorch/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/estimators/cuda_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22399 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3188 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/estimators/efficientnet_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/manchester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.492405 zoobot-2.0.1/zoobot/pytorch/predictions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/predictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/predictions/predict_on_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.492405 zoobot-2.0.1/zoobot/pytorch/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39188 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6800 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/training/representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/training/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/training/tensorboard_writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19378 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/pytorch/training/train_with_pytorch_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.496405 zoobot-2.0.1/zoobot/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/benchmark_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4437 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/compress_representations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/label_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/load_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/save_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13065 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/shared/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.496405 zoobot-2.0.1/zoobot/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.496405 zoobot-2.0.1/zoobot/tensorflow/estimators/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2508 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/alexnet_baseline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1795 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/custom_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7227 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2300 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/efficientnet_custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    84167 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/efficientnet_standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/estimators/small_cnn_baseline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.496405 zoobot-2.0.1/zoobot/tensorflow/predictions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/predictions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3417 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/predictions/predict_on_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5239 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.496405 zoobot-2.0.1/zoobot/tensorflow/stats/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/stats/coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14433 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/stats/dirichlet_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3526 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/stats/mixture_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.500405 zoobot-2.0.1/zoobot/tensorflow/training/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/training/custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6865 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/training/train_with_keras.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6505 2024-05-14 20:07:34.000000 zoobot-2.0.1/zoobot/tensorflow/training/training_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:07:45.500405 zoobot-2.0.1/zoobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-05-14 20:07:45.000000 zoobot-2.0.1/zoobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-14 20:07:45.000000 zoobot-2.0.1/zoobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:07:45.000000 zoobot-2.0.1/zoobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-14 20:07:45.000000 zoobot-2.0.1/zoobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 20:07:45.000000 zoobot-2.0.1/zoobot.egg-info/top_level.txt
```

### Comparing `zoobot-2.0.0/LICENSE` & `zoobot-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/PKG-INFO` & `zoobot-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoobot
-Version: 2.0.0
+Version: 2.0.1
 Summary: Galaxy morphology classifiers
 Home-page: https://github.com/mwalmsley/zoobot
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Requires-Dist: scikit-learn>=1.0.2
 Requires-Dist: matplotlib
 Requires-Dist: pyarrow
 Requires-Dist: wandb
 Requires-Dist: webdataset
 Requires-Dist: huggingface_hub
 Requires-Dist: setuptools
-Requires-Dist: galaxy-datasets>=0.0.17
+Requires-Dist: galaxy-datasets>=0.0.18
 Provides-Extra: pytorch-cpu
 Requires-Dist: torch==2.1.0+cpu; extra == "pytorch-cpu"
 Requires-Dist: torchvision==0.16.0+cpu; extra == "pytorch-cpu"
 Requires-Dist: torchaudio>=2.1.0; extra == "pytorch-cpu"
 Requires-Dist: lightning>=2.0.0; extra == "pytorch-cpu"
 Requires-Dist: albumentations; extra == "pytorch-cpu"
 Requires-Dist: pyro-ppl>=1.8.6; extra == "pytorch-cpu"
@@ -94,25 +94,30 @@
 ![build](https://github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg)
 ![publish](https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://badge.fury.io/py/zoobot)
 [![DOI](https://zenodo.org/badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617)
 [![status](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f)
 <a href="https://ascl.net/2203.027"><img src="https://img.shields.io/badge/ascl-2203.027-blue.svg?colorB=262255" alt="ascl:2203.027" /></a>
 
+---
+### :tada: Zoobot 2.0 is now available. Bigger and better models with streamlined finetuning. [Blog](https://walmsley.dev/posts/zoobot-scaling-laws), [paper](https://arxiv.org/abs/2404.02973) :tada:
+---
+
 Zoobot classifies galaxy morphology with deep learning.
 <!-- At Galaxy Zoo, we use Zoobot to help our volunteers classify the galaxies in all our recent catalogues: GZ DECaLS, GZ DESI, GZ Rings and GZ Cosmic Dawn. -->
 
 Zoobot is trained using millions of answers by Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately solve your own prediction task.
 
 - [Install](#installation)
 - [Quickstart](#quickstart)
 - [Worked Examples](#worked-examples)
 - [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/pretrained_models.html)
 - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
 - [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
+- [Mailing List](https://groups.google.com/g/zoobot) (for updates)
 
 ## Installation
 
 <a name="installation"></a>
 
 You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing). To install locally, keep reading.
 
@@ -140,52 +145,51 @@
 
 <a name="quickstart"></a>
 
 The [Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
 
 Let's say you want to find ringed galaxies and you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find rings like so:
 
-    ```python
-
-    import pandas as pd
-    from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
-    from zoobot.pytorch.training import finetune
-
-    # csv with 'ring' column (0 or 1) and 'file_loc' column (path to image)
-    labelled_df = pd.read_csv('/your/path/some_labelled_galaxies.csv')
-
-    datamodule = GalaxyDataModule(
-      label_cols=['ring'],
-      catalog=labelled_df,
-      batch_size=32
-    )
-
-    # load trained Zoobot model
-    model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2)  
-    
-    # retrain to find rings
-    trainer = finetune.get_trainer(save_dir)
-    trainer.fit(model, datamodule)
-    ```
+```python
+import pandas as pd
+from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
+from zoobot.pytorch.training import finetune
+
+# csv with 'ring' column (0 or 1) and 'file_loc' column (path to image)
+labelled_df = pd.read_csv('/your/path/some_labelled_galaxies.csv')
+
+datamodule = GalaxyDataModule(
+    label_cols=['ring'],
+    catalog=labelled_df,
+    batch_size=32
+)
+
+# load trained Zoobot model
+model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2)  
+
+# retrain to find rings
+trainer = finetune.get_trainer(save_dir)
+trainer.fit(model, datamodule)
+```
 
 Then you can make predict if new galaxies have rings:
 
-    ```python
-    from zoobot.pytorch.predictions import predict_on_catalog
+```python
+from zoobot.pytorch.predictions import predict_on_catalog
 
-    # csv with 'file_loc' column (path to image). Zoobot will predict the labels.
-    unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
+# csv with 'file_loc' column (path to image). Zoobot will predict the labels.
+unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 
-    predict_on_catalog.predict(
-      unlabelled_df,
-      model,
-      label_cols=['ring'],  # only used for 
-      save_loc='/your/path/finetuned_predictions.csv'
-    )
-    ```
+predict_on_catalog.predict(
+    unlabelled_df,
+    model,
+    label_cols=['ring'],  # only used for 
+    save_loc='/your/path/finetuned_predictions.csv'
+)
+```
 
 Zoobot includes many guides and working examples - see the [Getting Started](#getting-started) section below.
 
 ## Getting Started
 
 <a name="getting_started"></a>
 
@@ -195,44 +199,39 @@
 
 Pretrained models are listed [here](https://zoobot.readthedocs.io/en/latest/pretrained_models.html) and available on [HuggingFace](https://huggingface.co/collections/mwalmsley/zoobot-encoders-65fa14ae92911b173712b874)
 
 ### Worked Examples
 
 <a name="worked_examples"></a>
 
-PyTorch (recommended):
-
 - [pytorch/examples/finetuning/finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py)
 - [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py)
 - [pytorch/examples/representations/get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/representations/get_representations.py)
 - [pytorch/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/train_model_on_catalog.py) (only necessary to train from scratch)
 
 There is more explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
 
-I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
-
-When trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer labels of varying confidence and predict posteriors for what the typical volunteer might say. Specifically, this Zoobot mode predicts the parameters for distributions, not simple class labels! For a demonstration of how to interpret these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb).
-
 
 ### (Optional) Install PyTorch with CUDA
 
 <a name="install_cuda"></a>
 
 *If you're not using a GPU, skip this step. Use the pytorch-cpu option in the section below.*
 
-Install PyTorch 2.1.0 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
+Install PyTorch 2.1.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
 
 CUDA 12.1 for PyTorch 2.1.0:
 
     conda create --name zoobot39_torch python==3.9
     conda activate zoobot39_torch
     conda install -c conda-forge cudatoolkit=12.1
 
 ### Recent release features (v2.0.0)
 
+- **New in 2.0.1** Add greyscale encoders. Use `hf_hub:mwalmsley/zoobot-encoder-greyscale-convnext_nano` or [similar](https://huggingface.co/collections/mwalmsley/zoobot-encoders-greyscale-66427c51133285ca01b490c6).
 - New pretrained architectures: ConvNeXT, EfficientNetV2, MaxViT, and more. Each in several sizes.
 - Reworked finetuning procedure. All these architectures are finetuneable through a common method.
 - Reworked finetuning options. Batch norm finetuning removed. Cosine schedule option added.
 - Reworked finetuning saving/loading. Auto-downloads encoder from HuggingFace.
 - Now supports regression finetuning (as well as multi-class and binary). See `pytorch/examples/finetuning`
 - Updated `timm` to 0.9.10, allowing latest model architectures. Previously downloaded checkpoints may not load correctly!
 - (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC H2O). Significant performance improvement on HSC finetuning. Also now includes GZ UKIDSS (dragged from our archives).
@@ -242,19 +241,19 @@
 - Added option to compile encoder for max speed (not recommended for finetuning, only for pretraining).
 - Deprecates TensorFlow. The CS research community focuses on PyTorch and new frameworks like JAX.
 
 Contributions are very welcome and will be credited in any future work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) for more.
 
 ### Benchmarks and Replication - Training from Scratch
 
-The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot from scratch. We use these scripts to make sure new code versions work well, and that TensorFlow and PyTorch achieve similar performance.
+The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot 1.0 from scratch. 
 
 Training Zoobot using the GZ DECaLS dataset option will create models very similar to those used for the GZ DECaLS catalogue and shared with the early versions of this repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2).
 
-**Pretraining is becoming increasingly complex and is now partially refactored out to a separate repository. We are gradually migrating this `zoobot` repository to focus on finetuning.**
+*Pretraining is becoming increasingly complex and is now partially refactored out to a separate repository. We are gradually migrating this `zoobot` repository to focus on finetuning.*
 
 ### Citing
 
 If you use this software, or otherwise wish to cite Zoobot as a software package, please use the [JOSS paper](https://doi.org/10.21105/joss.05312):
 
     @article{Walmsley2023, doi = {10.21105/joss.05312}, url = {https://doi.org/10.21105/joss.05312}, year = {2023}, publisher = {The Open Journal}, volume = {8}, number = {85}, pages = {5312}, author = {Mike Walmsley and Campbell Allen and Ben Aussel and Micah Bowles and Kasia Gregorowicz and Inigo Val Slijepcevic and Chris J. Lintott and Anna M. m. Scaife and Maja Jabłońska and Kosio Karchev and Denise Lanzieri and Devina Mohan and David O’Ryan and Bharath Saiguhan and Crisel Suárez and Nicolás Guerra-Varas and Renuka Velu}, title = {Zoobot: Adaptable Deep Learning Models for Galaxy Morphology}, journal = {Journal of Open Source Software} }
```

### Comparing `zoobot-2.0.0/README.md` & `zoobot-2.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 ![build](https://github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg)
 ![publish](https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://badge.fury.io/py/zoobot)
 [![DOI](https://zenodo.org/badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617)
 [![status](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f)
 <a href="https://ascl.net/2203.027"><img src="https://img.shields.io/badge/ascl-2203.027-blue.svg?colorB=262255" alt="ascl:2203.027" /></a>
 
+---
+### :tada: Zoobot 2.0 is now available. Bigger and better models with streamlined finetuning. [Blog](https://walmsley.dev/posts/zoobot-scaling-laws), [paper](https://arxiv.org/abs/2404.02973) :tada:
+---
+
 Zoobot classifies galaxy morphology with deep learning.
 <!-- At Galaxy Zoo, we use Zoobot to help our volunteers classify the galaxies in all our recent catalogues: GZ DECaLS, GZ DESI, GZ Rings and GZ Cosmic Dawn. -->
 
 Zoobot is trained using millions of answers by Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately solve your own prediction task.
 
 - [Install](#installation)
 - [Quickstart](#quickstart)
 - [Worked Examples](#worked-examples)
 - [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/pretrained_models.html)
 - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
 - [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
+- [Mailing List](https://groups.google.com/g/zoobot) (for updates)
 
 ## Installation
 
 <a name="installation"></a>
 
 You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing). To install locally, keep reading.
 
@@ -51,52 +56,51 @@
 
 <a name="quickstart"></a>
 
 The [Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
 
 Let's say you want to find ringed galaxies and you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find rings like so:
 
-    ```python
-
-    import pandas as pd
-    from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
-    from zoobot.pytorch.training import finetune
-
-    # csv with 'ring' column (0 or 1) and 'file_loc' column (path to image)
-    labelled_df = pd.read_csv('/your/path/some_labelled_galaxies.csv')
-
-    datamodule = GalaxyDataModule(
-      label_cols=['ring'],
-      catalog=labelled_df,
-      batch_size=32
-    )
-
-    # load trained Zoobot model
-    model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2)  
-    
-    # retrain to find rings
-    trainer = finetune.get_trainer(save_dir)
-    trainer.fit(model, datamodule)
-    ```
+```python
+import pandas as pd
+from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
+from zoobot.pytorch.training import finetune
+
+# csv with 'ring' column (0 or 1) and 'file_loc' column (path to image)
+labelled_df = pd.read_csv('/your/path/some_labelled_galaxies.csv')
+
+datamodule = GalaxyDataModule(
+    label_cols=['ring'],
+    catalog=labelled_df,
+    batch_size=32
+)
+
+# load trained Zoobot model
+model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2)  
+
+# retrain to find rings
+trainer = finetune.get_trainer(save_dir)
+trainer.fit(model, datamodule)
+```
 
 Then you can make predict if new galaxies have rings:
 
-    ```python
-    from zoobot.pytorch.predictions import predict_on_catalog
+```python
+from zoobot.pytorch.predictions import predict_on_catalog
 
-    # csv with 'file_loc' column (path to image). Zoobot will predict the labels.
-    unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
+# csv with 'file_loc' column (path to image). Zoobot will predict the labels.
+unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 
-    predict_on_catalog.predict(
-      unlabelled_df,
-      model,
-      label_cols=['ring'],  # only used for 
-      save_loc='/your/path/finetuned_predictions.csv'
-    )
-    ```
+predict_on_catalog.predict(
+    unlabelled_df,
+    model,
+    label_cols=['ring'],  # only used for 
+    save_loc='/your/path/finetuned_predictions.csv'
+)
+```
 
 Zoobot includes many guides and working examples - see the [Getting Started](#getting-started) section below.
 
 ## Getting Started
 
 <a name="getting_started"></a>
 
@@ -106,44 +110,39 @@
 
 Pretrained models are listed [here](https://zoobot.readthedocs.io/en/latest/pretrained_models.html) and available on [HuggingFace](https://huggingface.co/collections/mwalmsley/zoobot-encoders-65fa14ae92911b173712b874)
 
 ### Worked Examples
 
 <a name="worked_examples"></a>
 
-PyTorch (recommended):
-
 - [pytorch/examples/finetuning/finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py)
 - [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py)
 - [pytorch/examples/representations/get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/representations/get_representations.py)
 - [pytorch/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/train_model_on_catalog.py) (only necessary to train from scratch)
 
 There is more explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
 
-I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
-
-When trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer labels of varying confidence and predict posteriors for what the typical volunteer might say. Specifically, this Zoobot mode predicts the parameters for distributions, not simple class labels! For a demonstration of how to interpret these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb).
-
 
 ### (Optional) Install PyTorch with CUDA
 
 <a name="install_cuda"></a>
 
 *If you're not using a GPU, skip this step. Use the pytorch-cpu option in the section below.*
 
-Install PyTorch 2.1.0 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
+Install PyTorch 2.1.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
 
 CUDA 12.1 for PyTorch 2.1.0:
 
     conda create --name zoobot39_torch python==3.9
     conda activate zoobot39_torch
     conda install -c conda-forge cudatoolkit=12.1
 
 ### Recent release features (v2.0.0)
 
+- **New in 2.0.1** Add greyscale encoders. Use `hf_hub:mwalmsley/zoobot-encoder-greyscale-convnext_nano` or [similar](https://huggingface.co/collections/mwalmsley/zoobot-encoders-greyscale-66427c51133285ca01b490c6).
 - New pretrained architectures: ConvNeXT, EfficientNetV2, MaxViT, and more. Each in several sizes.
 - Reworked finetuning procedure. All these architectures are finetuneable through a common method.
 - Reworked finetuning options. Batch norm finetuning removed. Cosine schedule option added.
 - Reworked finetuning saving/loading. Auto-downloads encoder from HuggingFace.
 - Now supports regression finetuning (as well as multi-class and binary). See `pytorch/examples/finetuning`
 - Updated `timm` to 0.9.10, allowing latest model architectures. Previously downloaded checkpoints may not load correctly!
 - (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC H2O). Significant performance improvement on HSC finetuning. Also now includes GZ UKIDSS (dragged from our archives).
@@ -153,19 +152,19 @@
 - Added option to compile encoder for max speed (not recommended for finetuning, only for pretraining).
 - Deprecates TensorFlow. The CS research community focuses on PyTorch and new frameworks like JAX.
 
 Contributions are very welcome and will be credited in any future work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) for more.
 
 ### Benchmarks and Replication - Training from Scratch
 
-The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot from scratch. We use these scripts to make sure new code versions work well, and that TensorFlow and PyTorch achieve similar performance.
+The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot 1.0 from scratch. 
 
 Training Zoobot using the GZ DECaLS dataset option will create models very similar to those used for the GZ DECaLS catalogue and shared with the early versions of this repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2).
 
-**Pretraining is becoming increasingly complex and is now partially refactored out to a separate repository. We are gradually migrating this `zoobot` repository to focus on finetuning.**
+*Pretraining is becoming increasingly complex and is now partially refactored out to a separate repository. We are gradually migrating this `zoobot` repository to focus on finetuning.*
 
 ### Citing
 
 If you use this software, or otherwise wish to cite Zoobot as a software package, please use the [JOSS paper](https://doi.org/10.21105/joss.05312):
 
     @article{Walmsley2023, doi = {10.21105/joss.05312}, url = {https://doi.org/10.21105/joss.05312}, year = {2023}, publisher = {The Open Journal}, volume = {8}, number = {85}, pages = {5312}, author = {Mike Walmsley and Campbell Allen and Ben Aussel and Micah Bowles and Kasia Gregorowicz and Inigo Val Slijepcevic and Chris J. Lintott and Anna M. m. Scaife and Maja Jabłońska and Kosio Karchev and Denise Lanzieri and Devina Mohan and David O’Ryan and Bharath Saiguhan and Crisel Suárez and Nicolás Guerra-Varas and Renuka Velu}, title = {Zoobot: Adaptable Deep Learning Models for Galaxy Morphology}, journal = {Journal of Open Source Software} }
```

#### html2text {}

```diff
@@ -3,41 +3,44 @@
 zoobot/badge/?version=latest)](https://zoobot.readthedocs.io/) ![build](https:/
 /github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg) ![publish]
 (https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/
 badge.svg) [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://
 badge.fury.io/py/zoobot) [![DOI](https://zenodo.org/badge/343787617.svg)]
 (https://zenodo.org/badge/latestdoi/343787617) [![status](https://
 joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://
-joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f) _[_a_s_c_l_:_2_2_0_3_._0_2_7_]Zoobot
-classifies galaxy morphology with deep learning. Zoobot is trained using
-millions of answers by Galaxy Zoo volunteers. This code will let you
-**retrain** Zoobot to accurately solve your own prediction task. - [Install]
-(#installation) - [Quickstart](#quickstart) - [Worked Examples](#worked-
-examples) - [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/
-pretrained_models.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-
-datasets) - [Documentation](https://zoobot.readthedocs.io/) (for understanding/
-reference) ## Installation You can retrain Zoobot in the cloud with a free GPU
-using this [Google Colab notebook](https://colab.research.google.com/drive/1A_-
-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing). To install locally, keep reading.
-Download the code using git: git clone git@github.com:mwalmsley/zoobot.git And
-then pick one of the three commands below to install Zoobot and PyTorch: #
-Zoobot with PyTorch and a GPU. Requires CUDA 12.1 (or CUDA 11.8, if you use
-`_cu118` instead) pip install -e "zoobot[pytorch-cu121]" --extra-index-url
-https://download.pytorch.org/whl/cu121 # OR Zoobot with PyTorch and no GPU pip
-install -e "zoobot[pytorch-cpu]" --extra-index-url https://
-download.pytorch.org/whl/cpu # OR Zoobot with PyTorch on Mac with M1 chip pip
-install -e "zoobot[pytorch-m1]" This installs the downloaded Zoobot code using
-pip [editable mode](https://pip.pypa.io/en/stable/topics/local-project-
-installs/#editable-installs) so you can easily change the code locally. Zoobot
-is also available directly from pip (`pip install zoobot[option]`). Only use
-this if you are sure you won't be making changes to Zoobot itself. For Google
-Colab, use `pip install zoobot[pytorch_colab]` To use a GPU, you must *already*
-have CUDA installed and matching the versions above. I share my install steps
-[here](#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU,
-just slower. ## Quickstart The [Colab notebook](https://
+joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f) _[_a_s_c_l_:_2_2_0_3_._0_2_7_]--- ###
+:tada: Zoobot 2.0 is now available. Bigger and better models with streamlined
+finetuning. [Blog](https://walmsley.dev/posts/zoobot-scaling-laws), [paper]
+(https://arxiv.org/abs/2404.02973) :tada: --- Zoobot classifies galaxy
+morphology with deep learning. Zoobot is trained using millions of answers by
+Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately
+solve your own prediction task. - [Install](#installation) - [Quickstart]
+(#quickstart) - [Worked Examples](#worked-examples) - [Pretrained Weights]
+(https://zoobot.readthedocs.io/en/latest/pretrained_models.html) - [Datasets]
+(https://www.github.com/mwalmsley/galaxy-datasets) - [Documentation](https://
+zoobot.readthedocs.io/) (for understanding/reference) - [Mailing List](https://
+groups.google.com/g/zoobot) (for updates) ## Installation You can retrain
+Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://
+colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing).
+To install locally, keep reading. Download the code using git: git clone
+git@github.com:mwalmsley/zoobot.git And then pick one of the three commands
+below to install Zoobot and PyTorch: # Zoobot with PyTorch and a GPU. Requires
+CUDA 12.1 (or CUDA 11.8, if you use `_cu118` instead) pip install -e "zoobot
+[pytorch-cu121]" --extra-index-url https://download.pytorch.org/whl/cu121 # OR
+Zoobot with PyTorch and no GPU pip install -e "zoobot[pytorch-cpu]" --extra-
+index-url https://download.pytorch.org/whl/cpu # OR Zoobot with PyTorch on Mac
+with M1 chip pip install -e "zoobot[pytorch-m1]" This installs the downloaded
+Zoobot code using pip [editable mode](https://pip.pypa.io/en/stable/topics/
+local-project-installs/#editable-installs) so you can easily change the code
+locally. Zoobot is also available directly from pip (`pip install zoobot
+[option]`). Only use this if you are sure you won't be making changes to Zoobot
+itself. For Google Colab, use `pip install zoobot[pytorch_colab]` To use a GPU,
+you must *already* have CUDA installed and matching the versions above. I share
+my install steps [here](#install_cuda). GPUs are optional - Zoobot will run
+retrain fine on CPU, just slower. ## Quickstart The [Colab notebook](https://
 colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing)
 is the quickest way to get started. Alternatively, the minimal example below
 illustrates how Zoobot works. Let's say you want to find ringed galaxies and
 you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can
 retrain Zoobot to find rings like so: ```python import pandas as pd from
 galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule from
 zoobot.pytorch.training import finetune # csv with 'ring' column (0 or 1) and
@@ -56,102 +59,91 @@
 section below. ## Getting Started I suggest starting with the [Colab notebook]
 (https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-
 g_Zi0RMGz5?usp=sharing) or the worked examples below, which you can copy and
 adapt. For context and explanation, see the [documentation](https://
 zoobot.readthedocs.io/). Pretrained models are listed [here](https://
 zoobot.readthedocs.io/en/latest/pretrained_models.html) and available on
 [HuggingFace](https://huggingface.co/collections/mwalmsley/zoobot-encoders-
-65fa14ae92911b173712b874) ### Worked Examples PyTorch (recommended): -
-[pytorch/examples/finetuning/finetune_binary_classification.py](https://
-github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/
-finetune_binary_classification.py) - [pytorch/examples/finetuning/
-finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/
-zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py) - [pytorch/
-examples/representations/get_representations.py](https://github.com/mwalmsley/
-zoobot/blob/main/zoobot/pytorch/examples/representations/
-get_representations.py) - [pytorch/examples/train_model_on_catalog.py](https://
-github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/
-train_model_on_catalog.py) (only necessary to train from scratch) There is more
-explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
-I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the
-scripts used to create and benchmark our pretrained models. Many pretrained
-models are available [already](https://zoobot.readthedocs.io/en/latest/
-data_notes.html), but if you need one trained on e.g. different input image
-sizes or with a specific architecture, I can probably make it for you. When
-trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot
-can learn from volunteer labels of varying confidence and predict posteriors
-for what the typical volunteer might say. Specifically, this Zoobot mode
-predicts the parameters for distributions, not simple class labels! For a
-demonstration of how to interpret these predictions, see the
-[gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/
-zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb). ### (Optional)
-Install PyTorch with CUDA *If you're not using a GPU, skip this step. Use the
-pytorch-cpu option in the section below.* Install PyTorch 2.1.0 or Tensorflow
-2.10.0 and compatible CUDA drivers. I highly recommend using [conda](https://
-docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both
-creating a new virtual environment (`conda create`) and installing CUDA
-(`cudatoolkit`, `cudnn`) CUDA 12.1 for PyTorch 2.1.0: conda create --name
-zoobot39_torch python==3.9 conda activate zoobot39_torch conda install -
-c conda-forge cudatoolkit=12.1 ### Recent release features (v2.0.0) - New
-pretrained architectures: ConvNeXT, EfficientNetV2, MaxViT, and more. Each in
-several sizes. - Reworked finetuning procedure. All these architectures are
-finetuneable through a common method. - Reworked finetuning options. Batch norm
-finetuning removed. Cosine schedule option added. - Reworked finetuning saving/
-loading. Auto-downloads encoder from HuggingFace. - Now supports regression
-finetuning (as well as multi-class and binary). See `pytorch/examples/
-finetuning` - Updated `timm` to 0.9.10, allowing latest model architectures.
-Previously downloaded checkpoints may not load correctly! - (internal until
-published) GZ Evo v2 now includes Cosmic Dawn (HSC H2O). Significant
-performance improvement on HSC finetuning. Also now includes GZ UKIDSS (dragged
-from our archives). - Updated `pytorch` to `2.1.0` - Added support for
-webdatasets (only recommended for large-scale distributed training) - Improved
-per-question logging when training from scratch - Added option to compile
-encoder for max speed (not recommended for finetuning, only for pretraining). -
-Deprecates TensorFlow. The CS research community focuses on PyTorch and new
-frameworks like JAX. Contributions are very welcome and will be credited in any
-future work. Please get in touch! See [CONTRIBUTING.md](https://github.com/
-mwalmsley/zoobot/blob/main/benchmarks) for more. ### Benchmarks and Replication
-- Training from Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/
-blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot
-from scratch. We use these scripts to make sure new code versions work well,
-and that TensorFlow and PyTorch achieve similar performance. Training Zoobot
-using the GZ DECaLS dataset option will create models very similar to those
-used for the GZ DECaLS catalogue and shared with the early versions of this
-repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as
-the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). **Pretraining is
-becoming increasingly complex and is now partially refactored out to a separate
-repository. We are gradually migrating this `zoobot` repository to focus on
-finetuning.** ### Citing If you use this software, or otherwise wish to cite
-Zoobot as a software package, please use the [JOSS paper](https://doi.org/
-10.21105/joss.05312): @article{Walmsley2023, doi = {10.21105/joss.05312}, url =
-{https://doi.org/10.21105/joss.05312}, year = {2023}, publisher = {The Open
-Journal}, volume = {8}, number = {85}, pages = {5312}, author = {Mike Walmsley
-and Campbell Allen and Ben Aussel and Micah Bowles and Kasia Gregorowicz and
-Inigo Val Slijepcevic and Chris J. Lintott and Anna M. m. Scaife and Maja
-JabÅoÅska and Kosio Karchev and Denise Lanzieri and Devina Mohan and David
-OâRyan and Bharath Saiguhan and Crisel SuÃ¡rez and NicolÃ¡s Guerra-Varas and
-Renuka Velu}, title = {Zoobot: Adaptable Deep Learning Models for Galaxy
-Morphology}, journal = {Journal of Open Source Software} } You might be
-interested in reading papers using Zoobot: - [Galaxy Zoo DECaLS: Detailed
-visual morphology measurements from volunteers and deep learning for 314,000
-galaxies](https://arxiv.org/abs/2102.08414) (2022) - [A Comparison of Deep
-Learning Architectures for Optical Galaxy Morphology Classification](https://
-arxiv.org/abs/2111.04353) (2022) - [Practical Galaxy Morphology Tools from Deep
-Supervised Representation Learning](https://arxiv.org/abs/2110.12735) (2022) -
-[Towards Foundation Models for Galaxy Morphology](https://arxiv.org/abs/
-2206.11927) (2022) - [Harnessing the Hubble Space Telescope Archives: A
-Catalogue of 21,926 Interacting Galaxies](https://arxiv.org/abs/2303.00366)
-(2023) - [Galaxy Zoo DESI: Detailed morphology measurements for 8.7M galaxies
-in the DESI Legacy Imaging Surveys](https://academic.oup.com/mnras/advance-
-article/doi/10.1093/mnras/stad2919/7283169?login=false) (2023) - [Galaxy
-mergers in Subaru HSC-SSP: A deep representation learning approach for
-identification, and the role of environment on merger incidence](https://
-doi.org/10.1051/0004-6361/202346743) (2023) - [Astronomaly at Scale: Searching
-for Anomalies Amongst 4 Million Galaxies](https://arxiv.org/abs/2309.08660)
-(2023, submitted) - [Transfer learning for galaxy feature detection: Finding
-Giant Star-forming Clumps in low redshift galaxies using Faster R-CNN](https://
-arxiv.org/abs/2312.03503) (2023) - [Euclid preparation. Measuring detailed
-galaxy morphologies for Euclid with Machine Learning](https://arxiv.org/abs/
-2402.10187) (2024, submitted) Many other works use Zoobot indirectly via the
-[Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog (and now via the
-new [Galaxy Zoo DESI](https://academic.oup.com/mnras/advance-article/doi/
-10.1093/mnras/stad2919/7283169?login=false) catalog).
+65fa14ae92911b173712b874) ### Worked Examples - [pytorch/examples/finetuning/
+finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
+main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
+[pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
+mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/
+finetune_counts_full_tree.py) - [pytorch/examples/representations/
+get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
+pytorch/examples/representations/get_representations.py) - [pytorch/examples/
+train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/
+zoobot/pytorch/examples/train_model_on_catalog.py) (only necessary to train
+from scratch) There is more explanation and an API reference on the [docs]
+(https://zoobot.readthedocs.io/). ### (Optional) Install PyTorch with CUDA *If
+you're not using a GPU, skip this step. Use the pytorch-cpu option in the
+section below.* Install PyTorch 2.1.0 and compatible CUDA drivers. I highly
+recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do
+this. Conda will handle both creating a new virtual environment (`conda
+create`) and installing CUDA (`cudatoolkit`, `cudnn`) CUDA 12.1 for PyTorch
+2.1.0: conda create --name zoobot39_torch python==3.9 conda activate
+zoobot39_torch conda install -c conda-forge cudatoolkit=12.1 ### Recent release
+features (v2.0.0) - **New in 2.0.1** Add greyscale encoders. Use `hf_hub:
+mwalmsley/zoobot-encoder-greyscale-convnext_nano` or [similar](https://
+huggingface.co/collections/mwalmsley/zoobot-encoders-greyscale-
+66427c51133285ca01b490c6). - New pretrained architectures: ConvNeXT,
+EfficientNetV2, MaxViT, and more. Each in several sizes. - Reworked finetuning
+procedure. All these architectures are finetuneable through a common method. -
+Reworked finetuning options. Batch norm finetuning removed. Cosine schedule
+option added. - Reworked finetuning saving/loading. Auto-downloads encoder from
+HuggingFace. - Now supports regression finetuning (as well as multi-class and
+binary). See `pytorch/examples/finetuning` - Updated `timm` to 0.9.10, allowing
+latest model architectures. Previously downloaded checkpoints may not load
+correctly! - (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC
+H2O). Significant performance improvement on HSC finetuning. Also now includes
+GZ UKIDSS (dragged from our archives). - Updated `pytorch` to `2.1.0` - Added
+support for webdatasets (only recommended for large-scale distributed training)
+- Improved per-question logging when training from scratch - Added option to
+compile encoder for max speed (not recommended for finetuning, only for
+pretraining). - Deprecates TensorFlow. The CS research community focuses on
+PyTorch and new frameworks like JAX. Contributions are very welcome and will be
+credited in any future work. Please get in touch! See [CONTRIBUTING.md](https:/
+/github.com/mwalmsley/zoobot/blob/main/benchmarks) for more. ### Benchmarks and
+Replication - Training from Scratch The [benchmarks](https://github.com/
+mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts
+to train Zoobot 1.0 from scratch. Training Zoobot using the GZ DECaLS dataset
+option will create models very similar to those used for the GZ DECaLS
+catalogue and shared with the early versions of this repo. The GZ DESI Zoobot
+model is trained on additional data (GZD-1, GZD-2), as the GZ Evo Zoobot model
+(GZD-1/2/5, Hubble, Candels, GZ2). *Pretraining is becoming increasingly
+complex and is now partially refactored out to a separate repository. We are
+gradually migrating this `zoobot` repository to focus on finetuning.* ###
+Citing If you use this software, or otherwise wish to cite Zoobot as a software
+package, please use the [JOSS paper](https://doi.org/10.21105/joss.05312):
+@article{Walmsley2023, doi = {10.21105/joss.05312}, url = {https://doi.org/
+10.21105/joss.05312}, year = {2023}, publisher = {The Open Journal}, volume =
+{8}, number = {85}, pages = {5312}, author = {Mike Walmsley and Campbell Allen
+and Ben Aussel and Micah Bowles and Kasia Gregorowicz and Inigo Val Slijepcevic
+and Chris J. Lintott and Anna M. m. Scaife and Maja JabÅoÅska and Kosio
+Karchev and Denise Lanzieri and Devina Mohan and David OâRyan and Bharath
+Saiguhan and Crisel SuÃ¡rez and NicolÃ¡s Guerra-Varas and Renuka Velu}, title =
+{Zoobot: Adaptable Deep Learning Models for Galaxy Morphology}, journal =
+{Journal of Open Source Software} } You might be interested in reading papers
+using Zoobot: - [Galaxy Zoo DECaLS: Detailed visual morphology measurements
+from volunteers and deep learning for 314,000 galaxies](https://arxiv.org/abs/
+2102.08414) (2022) - [A Comparison of Deep Learning Architectures for Optical
+Galaxy Morphology Classification](https://arxiv.org/abs/2111.04353) (2022) -
+[Practical Galaxy Morphology Tools from Deep Supervised Representation
+Learning](https://arxiv.org/abs/2110.12735) (2022) - [Towards Foundation Models
+for Galaxy Morphology](https://arxiv.org/abs/2206.11927) (2022) - [Harnessing
+the Hubble Space Telescope Archives: A Catalogue of 21,926 Interacting
+Galaxies](https://arxiv.org/abs/2303.00366) (2023) - [Galaxy Zoo DESI: Detailed
+morphology measurements for 8.7M galaxies in the DESI Legacy Imaging Surveys]
+(https://academic.oup.com/mnras/advance-article/doi/10.1093/mnras/stad2919/
+7283169?login=false) (2023) - [Galaxy mergers in Subaru HSC-SSP: A deep
+representation learning approach for identification, and the role of
+environment on merger incidence](https://doi.org/10.1051/0004-6361/202346743)
+(2023) - [Astronomaly at Scale: Searching for Anomalies Amongst 4 Million
+Galaxies](https://arxiv.org/abs/2309.08660) (2023, submitted) - [Transfer
+learning for galaxy feature detection: Finding Giant Star-forming Clumps in low
+redshift galaxies using Faster R-CNN](https://arxiv.org/abs/2312.03503) (2023)
+- [Euclid preparation. Measuring detailed galaxy morphologies for Euclid with
+Machine Learning](https://arxiv.org/abs/2402.10187) (2024, submitted) Many
+other works use Zoobot indirectly via the [Galaxy Zoo DECaLS](https://
+arxiv.org/abs/2102.08414) catalog (and now via the new [Galaxy Zoo DESI](https:
+//academic.oup.com/mnras/advance-article/doi/10.1093/mnras/stad2919/
+7283169?login=false) catalog).
```

### Comparing `zoobot-2.0.0/setup.py` & `zoobot-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zoobot",
-    version="2.0.0",
+    version="2.0.1",
     author="Mike Walmsley",
     author_email="walmsleymk1@gmail.com",
     description="Galaxy morphology classifiers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mwalmsley/zoobot",
     classifiers=[
@@ -113,10 +113,10 @@
         'matplotlib',
         'pyarrow',  # to read parquet, which is very handy for big datasets
         # for saving metrics to weights&biases (cloud service, free within limits)
         'wandb',
         'webdataset',  # for reading webdataset files
         'huggingface_hub',  # login may be required
         'setuptools',  # no longer pinned
-        'galaxy-datasets>=0.0.17'  # for dataset loading in both TF and Torch (see github/mwalmsley/galaxy-datasets)
+        'galaxy-datasets>=0.0.18'  # for dataset loading in both TF and Torch (see github/mwalmsley/galaxy-datasets)
     ]
 )
```

### Comparing `zoobot-2.0.0/tests/test_from_hub.py` & `zoobot-2.0.1/tests/test_from_hub.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/tests/test_loss_equivalence.py` & `zoobot-2.0.1/tests/test_loss_equivalence.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/datasets/webdatamodule.py` & `zoobot-2.0.1/zoobot/pytorch/datasets/webdatamodule.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/datasets/webdataset_utils.py` & `zoobot-2.0.1/zoobot/pytorch/datasets/webdataset_utils.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/estimators/custom_layers.py` & `zoobot-2.0.1/zoobot/pytorch/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/estimators/define_model.py` & `zoobot-2.0.1/zoobot/pytorch/estimators/define_model.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/estimators/efficientnet_custom.py` & `zoobot-2.0.1/zoobot/pytorch/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/manchester.py` & `zoobot-2.0.1/zoobot/pytorch/manchester.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/predictions/predict_on_catalog.py` & `zoobot-2.0.1/zoobot/pytorch/predictions/predict_on_catalog.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/training/finetune.py` & `zoobot-2.0.1/zoobot/pytorch/training/finetune.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,22 @@
             # therefore ignore the warning
         self.save_hyperparameters(ignore=['encoder']) # never serialise the encoder, way too heavy
             # if you need the encoder to recreate, pass when loading checkpoint e.g. 
             # FinetuneableZoobotTree.load_from_checkpoint(loc, encoder=encoder)
         
         if name is not None:
             assert encoder is None, 'Cannot pass both name and encoder to use'
-            self.encoder = timm.create_model(name, num_classes=0, pretrained=True)
+            if 'greyscale' in name:
+                # I'm not sure why timm is happy to convert color model stem to greyscale 
+                # but doesn't correctly load greyscale model without this hack
+                logging.info('Loading greyscale model (auto-detected from name)')
+                timm_kwargs = {'in_chans': 1}
+            else:
+                timm_kwargs = {}
+            self.encoder = timm.create_model(name, num_classes=0, pretrained=True, **timm_kwargs)
             self.encoder_dim = self.encoder.num_features
 
         elif zoobot_checkpoint_loc is not None:
             assert encoder is None, 'Cannot pass both checkpoint to load and encoder to use'
             self.encoder = load_pretrained_zoobot(zoobot_checkpoint_loc)  # extracts the timm encoder
             self.encoder_dim = self.encoder.num_features
         else:
```

### Comparing `zoobot-2.0.0/zoobot/pytorch/training/losses.py` & `zoobot-2.0.1/zoobot/pytorch/training/losses.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/training/representations.py` & `zoobot-2.0.1/zoobot/pytorch/training/representations.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/training/schedulers.py` & `zoobot-2.0.1/zoobot/pytorch/training/schedulers.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/training/tensorboard_writers.py` & `zoobot-2.0.1/zoobot/pytorch/training/tensorboard_writers.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/pytorch/training/train_with_pytorch_lightning.py` & `zoobot-2.0.1/zoobot/pytorch/training/train_with_pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/shared/benchmark_datasets.py` & `zoobot-2.0.1/zoobot/shared/benchmark_datasets.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/shared/compress_representations.py` & `zoobot-2.0.1/zoobot/shared/compress_representations.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/shared/label_metadata.py` & `zoobot-2.0.1/zoobot/shared/label_metadata.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/shared/load_predictions.py` & `zoobot-2.0.1/zoobot/shared/load_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/shared/save_predictions.py` & `zoobot-2.0.1/zoobot/shared/save_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/shared/schemas.py` & `zoobot-2.0.1/zoobot/shared/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -295,7 +295,10 @@
 # trigger basicConfig() and prevent user setting their own logging.
 # so don't log anything during Schema.__init__!
 
 gz_evo_v1_schema = Schema(label_metadata.gz_evo_v1_pairs, label_metadata.gz_evo_v1_dependencies)
 
 gz_ukidss_schema = Schema(label_metadata.ukidss_ortho_pairs, label_metadata.ukidss_ortho_dependencies)
 gz_jwst_schema = Schema(label_metadata.jwst_ortho_pairs, label_metadata.jwst_ortho_dependencies)
+
+euclid_ortho_schema = Schema(label_metadata.euclid_ortho_pairs , label_metadata.euclid_ortho_dependencies)
+euclid_schema = Schema(label_metadata.euclid_pairs , label_metadata.euclid_dependencies)
```

### Comparing `zoobot-2.0.0/zoobot/shared/stats.py` & `zoobot-2.0.1/zoobot/shared/stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/estimators/alexnet_baseline.py` & `zoobot-2.0.1/zoobot/tensorflow/estimators/alexnet_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/estimators/custom_callbacks.py` & `zoobot-2.0.1/zoobot/tensorflow/estimators/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/estimators/custom_layers.py` & `zoobot-2.0.1/zoobot/tensorflow/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/estimators/define_model.py` & `zoobot-2.0.1/zoobot/tensorflow/estimators/define_model.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_custom.py` & `zoobot-2.0.1/zoobot/tensorflow/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_standard.py` & `zoobot-2.0.1/zoobot/tensorflow/estimators/efficientnet_standard.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/estimators/small_cnn_baseline.py` & `zoobot-2.0.1/zoobot/tensorflow/estimators/small_cnn_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/predictions/predict_on_dataset.py` & `zoobot-2.0.1/zoobot/tensorflow/predictions/predict_on_dataset.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py` & `zoobot-2.0.1/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/stats/coverage.py` & `zoobot-2.0.1/zoobot/tensorflow/stats/coverage.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/stats/dirichlet_stats.py` & `zoobot-2.0.1/zoobot/tensorflow/stats/dirichlet_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/stats/mixture_stats.py` & `zoobot-2.0.1/zoobot/tensorflow/stats/mixture_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/training/custom_metrics.py` & `zoobot-2.0.1/zoobot/tensorflow/training/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/training/finetune.py` & `zoobot-2.0.1/zoobot/tensorflow/training/finetune.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/training/losses.py` & `zoobot-2.0.1/zoobot/tensorflow/training/losses.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/training/train_with_keras.py` & `zoobot-2.0.1/zoobot/tensorflow/training/train_with_keras.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot/tensorflow/training/training_config.py` & `zoobot-2.0.1/zoobot/tensorflow/training/training_config.py`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot.egg-info/PKG-INFO` & `zoobot-2.0.1/zoobot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoobot
-Version: 2.0.0
+Version: 2.0.1
 Summary: Galaxy morphology classifiers
 Home-page: https://github.com/mwalmsley/zoobot
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Requires-Dist: scikit-learn>=1.0.2
 Requires-Dist: matplotlib
 Requires-Dist: pyarrow
 Requires-Dist: wandb
 Requires-Dist: webdataset
 Requires-Dist: huggingface_hub
 Requires-Dist: setuptools
-Requires-Dist: galaxy-datasets>=0.0.17
+Requires-Dist: galaxy-datasets>=0.0.18
 Provides-Extra: pytorch-cpu
 Requires-Dist: torch==2.1.0+cpu; extra == "pytorch-cpu"
 Requires-Dist: torchvision==0.16.0+cpu; extra == "pytorch-cpu"
 Requires-Dist: torchaudio>=2.1.0; extra == "pytorch-cpu"
 Requires-Dist: lightning>=2.0.0; extra == "pytorch-cpu"
 Requires-Dist: albumentations; extra == "pytorch-cpu"
 Requires-Dist: pyro-ppl>=1.8.6; extra == "pytorch-cpu"
@@ -94,25 +94,30 @@
 ![build](https://github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg)
 ![publish](https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://badge.fury.io/py/zoobot)
 [![DOI](https://zenodo.org/badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617)
 [![status](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f)
 <a href="https://ascl.net/2203.027"><img src="https://img.shields.io/badge/ascl-2203.027-blue.svg?colorB=262255" alt="ascl:2203.027" /></a>
 
+---
+### :tada: Zoobot 2.0 is now available. Bigger and better models with streamlined finetuning. [Blog](https://walmsley.dev/posts/zoobot-scaling-laws), [paper](https://arxiv.org/abs/2404.02973) :tada:
+---
+
 Zoobot classifies galaxy morphology with deep learning.
 <!-- At Galaxy Zoo, we use Zoobot to help our volunteers classify the galaxies in all our recent catalogues: GZ DECaLS, GZ DESI, GZ Rings and GZ Cosmic Dawn. -->
 
 Zoobot is trained using millions of answers by Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately solve your own prediction task.
 
 - [Install](#installation)
 - [Quickstart](#quickstart)
 - [Worked Examples](#worked-examples)
 - [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/pretrained_models.html)
 - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
 - [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
+- [Mailing List](https://groups.google.com/g/zoobot) (for updates)
 
 ## Installation
 
 <a name="installation"></a>
 
 You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing). To install locally, keep reading.
 
@@ -140,52 +145,51 @@
 
 <a name="quickstart"></a>
 
 The [Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
 
 Let's say you want to find ringed galaxies and you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find rings like so:
 
-    ```python
-
-    import pandas as pd
-    from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
-    from zoobot.pytorch.training import finetune
-
-    # csv with 'ring' column (0 or 1) and 'file_loc' column (path to image)
-    labelled_df = pd.read_csv('/your/path/some_labelled_galaxies.csv')
-
-    datamodule = GalaxyDataModule(
-      label_cols=['ring'],
-      catalog=labelled_df,
-      batch_size=32
-    )
-
-    # load trained Zoobot model
-    model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2)  
-    
-    # retrain to find rings
-    trainer = finetune.get_trainer(save_dir)
-    trainer.fit(model, datamodule)
-    ```
+```python
+import pandas as pd
+from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
+from zoobot.pytorch.training import finetune
+
+# csv with 'ring' column (0 or 1) and 'file_loc' column (path to image)
+labelled_df = pd.read_csv('/your/path/some_labelled_galaxies.csv')
+
+datamodule = GalaxyDataModule(
+    label_cols=['ring'],
+    catalog=labelled_df,
+    batch_size=32
+)
+
+# load trained Zoobot model
+model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2)  
+
+# retrain to find rings
+trainer = finetune.get_trainer(save_dir)
+trainer.fit(model, datamodule)
+```
 
 Then you can make predict if new galaxies have rings:
 
-    ```python
-    from zoobot.pytorch.predictions import predict_on_catalog
+```python
+from zoobot.pytorch.predictions import predict_on_catalog
 
-    # csv with 'file_loc' column (path to image). Zoobot will predict the labels.
-    unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
+# csv with 'file_loc' column (path to image). Zoobot will predict the labels.
+unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 
-    predict_on_catalog.predict(
-      unlabelled_df,
-      model,
-      label_cols=['ring'],  # only used for 
-      save_loc='/your/path/finetuned_predictions.csv'
-    )
-    ```
+predict_on_catalog.predict(
+    unlabelled_df,
+    model,
+    label_cols=['ring'],  # only used for 
+    save_loc='/your/path/finetuned_predictions.csv'
+)
+```
 
 Zoobot includes many guides and working examples - see the [Getting Started](#getting-started) section below.
 
 ## Getting Started
 
 <a name="getting_started"></a>
 
@@ -195,44 +199,39 @@
 
 Pretrained models are listed [here](https://zoobot.readthedocs.io/en/latest/pretrained_models.html) and available on [HuggingFace](https://huggingface.co/collections/mwalmsley/zoobot-encoders-65fa14ae92911b173712b874)
 
 ### Worked Examples
 
 <a name="worked_examples"></a>
 
-PyTorch (recommended):
-
 - [pytorch/examples/finetuning/finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py)
 - [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py)
 - [pytorch/examples/representations/get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/representations/get_representations.py)
 - [pytorch/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/train_model_on_catalog.py) (only necessary to train from scratch)
 
 There is more explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
 
-I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
-
-When trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer labels of varying confidence and predict posteriors for what the typical volunteer might say. Specifically, this Zoobot mode predicts the parameters for distributions, not simple class labels! For a demonstration of how to interpret these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb).
-
 
 ### (Optional) Install PyTorch with CUDA
 
 <a name="install_cuda"></a>
 
 *If you're not using a GPU, skip this step. Use the pytorch-cpu option in the section below.*
 
-Install PyTorch 2.1.0 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
+Install PyTorch 2.1.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
 
 CUDA 12.1 for PyTorch 2.1.0:
 
     conda create --name zoobot39_torch python==3.9
     conda activate zoobot39_torch
     conda install -c conda-forge cudatoolkit=12.1
 
 ### Recent release features (v2.0.0)
 
+- **New in 2.0.1** Add greyscale encoders. Use `hf_hub:mwalmsley/zoobot-encoder-greyscale-convnext_nano` or [similar](https://huggingface.co/collections/mwalmsley/zoobot-encoders-greyscale-66427c51133285ca01b490c6).
 - New pretrained architectures: ConvNeXT, EfficientNetV2, MaxViT, and more. Each in several sizes.
 - Reworked finetuning procedure. All these architectures are finetuneable through a common method.
 - Reworked finetuning options. Batch norm finetuning removed. Cosine schedule option added.
 - Reworked finetuning saving/loading. Auto-downloads encoder from HuggingFace.
 - Now supports regression finetuning (as well as multi-class and binary). See `pytorch/examples/finetuning`
 - Updated `timm` to 0.9.10, allowing latest model architectures. Previously downloaded checkpoints may not load correctly!
 - (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC H2O). Significant performance improvement on HSC finetuning. Also now includes GZ UKIDSS (dragged from our archives).
@@ -242,19 +241,19 @@
 - Added option to compile encoder for max speed (not recommended for finetuning, only for pretraining).
 - Deprecates TensorFlow. The CS research community focuses on PyTorch and new frameworks like JAX.
 
 Contributions are very welcome and will be credited in any future work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) for more.
 
 ### Benchmarks and Replication - Training from Scratch
 
-The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot from scratch. We use these scripts to make sure new code versions work well, and that TensorFlow and PyTorch achieve similar performance.
+The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot 1.0 from scratch. 
 
 Training Zoobot using the GZ DECaLS dataset option will create models very similar to those used for the GZ DECaLS catalogue and shared with the early versions of this repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2).
 
-**Pretraining is becoming increasingly complex and is now partially refactored out to a separate repository. We are gradually migrating this `zoobot` repository to focus on finetuning.**
+*Pretraining is becoming increasingly complex and is now partially refactored out to a separate repository. We are gradually migrating this `zoobot` repository to focus on finetuning.*
 
 ### Citing
 
 If you use this software, or otherwise wish to cite Zoobot as a software package, please use the [JOSS paper](https://doi.org/10.21105/joss.05312):
 
     @article{Walmsley2023, doi = {10.21105/joss.05312}, url = {https://doi.org/10.21105/joss.05312}, year = {2023}, publisher = {The Open Journal}, volume = {8}, number = {85}, pages = {5312}, author = {Mike Walmsley and Campbell Allen and Ben Aussel and Micah Bowles and Kasia Gregorowicz and Inigo Val Slijepcevic and Chris J. Lintott and Anna M. m. Scaife and Maja Jabłońska and Kosio Karchev and Denise Lanzieri and Devina Mohan and David O’Ryan and Bharath Saiguhan and Crisel Suárez and Nicolás Guerra-Varas and Renuka Velu}, title = {Zoobot: Adaptable Deep Learning Models for Galaxy Morphology}, journal = {Journal of Open Source Software} }
```

### Comparing `zoobot-2.0.0/zoobot.egg-info/SOURCES.txt` & `zoobot-2.0.1/zoobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zoobot-2.0.0/zoobot.egg-info/requires.txt` & `zoobot-2.0.1/zoobot.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 scikit-learn>=1.0.2
 matplotlib
 pyarrow
 wandb
 webdataset
 huggingface_hub
 setuptools
-galaxy-datasets>=0.0.17
+galaxy-datasets>=0.0.18
 
 [docs]
 Sphinx
 sphinxcontrib-napoleon
 furo
 docutils<0.18
 sphinxemoji
```

