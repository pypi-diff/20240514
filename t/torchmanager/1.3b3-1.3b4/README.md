# Comparing `tmp/torchmanager-1.3b3.tar.gz` & `tmp/torchmanager-1.3b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.3b3.tar", max compression
+gzip compressed data, was "torchmanager-1.3b4.tar", max compression
```

## Comparing `torchmanager-1.3b3.tar` & `torchmanager-1.3b4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1318 2024-01-25 17:20:45.574938 torchmanager-1.3b3/LICENSE
--rw-r--r--   0        0        0     6845 2024-04-22 19:39:02.144750 torchmanager-1.3b3/README.md
--rwxr-xr-x   0        0        0      728 2024-04-22 19:39:34.990394 torchmanager-1.3b3/pyproject.toml
--rw-r--r--   0        0        0      283 2024-04-12 14:34:40.966040 torchmanager-1.3b3/torchmanager/__init__.py
--rw-r--r--   0        0        0    15405 2024-04-22 19:39:02.147028 torchmanager-1.3b3/torchmanager/basic.py
--rwxr-xr-x   0        0        0      788 2024-04-22 19:39:02.147628 torchmanager-1.3b3/torchmanager/callbacks/__init__.py
--rwxr-xr-x   0        0        0     6962 2024-04-22 19:39:02.148315 torchmanager-1.3b3/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     5489 2024-04-22 19:39:02.148716 torchmanager-1.3b3/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3522 2024-01-25 17:20:45.576291 torchmanager-1.3b3/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1971 2024-04-22 19:39:02.149083 torchmanager-1.3b3/torchmanager/callbacks/early_stop.py
--rwxr-xr-x   0        0        0     2953 2024-04-22 19:39:02.149643 torchmanager-1.3b3/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     4139 2024-04-22 19:39:02.150224 torchmanager-1.3b3/torchmanager/callbacks/functional.py
--rw-r--r--   0        0        0     2347 2024-04-22 19:39:02.150676 torchmanager-1.3b3/torchmanager/callbacks/lr.py
--rwxr-xr-x   0        0        0     2372 2024-04-22 19:39:02.151005 torchmanager-1.3b3/torchmanager/callbacks/progress.py
--rw-r--r--   0        0        0     2600 2024-04-22 19:39:02.151417 torchmanager-1.3b3/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      544 2024-01-25 17:20:45.576732 torchmanager-1.3b3/torchmanager/compatibility.py
--rw-r--r--   0        0        0      299 2024-04-22 19:39:02.151696 torchmanager-1.3b3/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     5540 2024-04-22 19:39:02.152151 torchmanager-1.3b3/torchmanager/configs/basic.py
--rw-r--r--   0        0        0     5512 2024-04-22 19:39:02.152465 torchmanager-1.3b3/torchmanager/configs/json.py
--rw-r--r--   0        0        0     5549 2024-04-22 19:39:02.152811 torchmanager-1.3b3/torchmanager/configs/yaml.py
--rw-r--r--   0        0        0      172 2024-04-12 14:34:40.967281 torchmanager-1.3b3/torchmanager/core.py
--rw-r--r--   0        0        0      132 2024-04-22 19:39:02.153050 torchmanager-1.3b3/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     8634 2024-04-22 19:39:02.153351 torchmanager-1.3b3/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     4213 2024-04-22 19:39:02.153778 torchmanager-1.3b3/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      180 2024-01-25 17:20:45.577468 torchmanager-1.3b3/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     8030 2024-04-22 19:39:34.991161 torchmanager-1.3b3/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     2486 2024-04-22 19:39:34.991601 torchmanager-1.3b3/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     6419 2024-04-22 19:39:34.992072 torchmanager-1.3b3/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3156 2024-01-25 17:20:45.577853 torchmanager-1.3b3/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      393 2024-04-22 19:39:02.155498 torchmanager-1.3b3/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     6310 2024-04-22 19:39:34.992544 torchmanager-1.3b3/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     7185 2024-04-22 19:39:39.179577 torchmanager-1.3b3/torchmanager/metrics/conf_mat.py
--rw-r--r--   0        0        0       68 2024-04-12 14:34:40.968627 torchmanager-1.3b3/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5697 2024-04-22 19:39:34.993377 torchmanager-1.3b3/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2920 2024-04-22 19:39:39.179993 torchmanager-1.3b3/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4630 2024-04-22 19:39:34.994160 torchmanager-1.3b3/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     3544 2024-04-22 19:39:34.994631 torchmanager-1.3b3/torchmanager/metrics/similarity.py
--rw-r--r--   0        0        0     8734 2024-04-22 19:39:34.995068 torchmanager-1.3b3/torchmanager/testing.py
--rw-r--r--   0        0        0      288 2024-04-22 19:39:02.159382 torchmanager-1.3b3/torchmanager/train/__init__.py
--rw-r--r--   0        0        0       43 2024-01-25 17:20:45.578906 torchmanager-1.3b3/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      763 2024-01-25 17:20:45.578987 torchmanager-1.3b3/torchmanager/train/learning_rate.py
--rwxr-xr-x   0        0        0    15102 2024-04-22 19:39:34.995599 torchmanager-1.3b3/torchmanager/training.py
--rwxr-xr-x   0        0        0      645 2024-04-22 19:39:02.160275 torchmanager-1.3b3/torchmanager_core/__init__.py
--rw-r--r--   0        0        0       46 2024-04-22 19:39:02.160532 torchmanager-1.3b3/torchmanager_core/backward/__init__.py
--rw-r--r--   0        0        0     2747 2024-04-22 19:39:02.160779 torchmanager-1.3b3/torchmanager_core/backward/hook.py
--rw-r--r--   0        0        0      134 2024-04-22 19:39:02.160882 torchmanager-1.3b3/torchmanager_core/backward/protocols.py
--rw-r--r--   0        0        0       52 2024-01-25 17:20:45.579434 torchmanager-1.3b3/torchmanager_core/checkpoint/__init__.py
--rw-r--r--   0        0        0     7689 2024-04-22 19:39:02.161113 torchmanager-1.3b3/torchmanager_core/checkpoint/ckpt.py
--rw-r--r--   0        0        0      109 2024-01-25 17:20:45.579655 torchmanager-1.3b3/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     6054 2024-04-22 19:39:02.161343 torchmanager-1.3b3/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      265 2024-01-25 17:22:35.173853 torchmanager-1.3b3/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      243 2024-04-22 19:39:02.161575 torchmanager-1.3b3/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      331 2024-04-22 19:39:02.161684 torchmanager-1.3b3/torchmanager_core/errors/configs.py
--rw-r--r--   0        0        0      535 2024-04-22 19:39:02.161868 torchmanager-1.3b3/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2024-01-25 17:20:45.580120 torchmanager-1.3b3/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0      292 2024-04-22 19:39:02.161991 torchmanager-1.3b3/torchmanager_core/errors/version.py
--rw-r--r--   0        0        0     3281 2024-04-22 19:39:02.162172 torchmanager-1.3b3/torchmanager_core/protocols.py
--rw-r--r--   0        0        0      157 2024-04-22 19:39:02.162340 torchmanager-1.3b3/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0      806 2024-04-22 19:39:02.162436 torchmanager-1.3b3/torchmanager_core/random/random.py
--rw-r--r--   0        0        0     1008 2024-01-25 17:22:35.174100 torchmanager-1.3b3/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2024-01-25 17:20:45.580473 torchmanager-1.3b3/torchmanager_core/typing.py
--rw-r--r--   0        0        0      157 2024-04-12 14:34:40.970072 torchmanager-1.3b3/torchmanager_core/version/__init__.py
--rw-r--r--   0        0        0     1307 2024-04-22 19:39:02.162624 torchmanager-1.3b3/torchmanager_core/version/deprecation.py
--rw-r--r--   0        0        0      138 2024-04-22 19:39:34.995984 torchmanager-1.3b3/torchmanager_core/version/details.py
--rw-r--r--   0        0        0      318 2024-04-12 14:34:40.970557 torchmanager-1.3b3/torchmanager_core/version/errors.py
--rw-r--r--   0        0        0     6575 2024-04-22 19:39:02.163346 torchmanager-1.3b3/torchmanager_core/version/version.py
--rw-r--r--   0        0        0      138 2024-01-25 17:22:35.175250 torchmanager-1.3b3/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      577 2024-04-22 19:39:02.163525 torchmanager-1.3b3/torchmanager_core/view/logging.py
--rw-r--r--   0        0        0      313 2024-01-25 17:20:45.581203 torchmanager-1.3b3/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0     7580 1970-01-01 00:00:00.000000 torchmanager-1.3b3/PKG-INFO
+-rw-r--r--   0        0        0     1318 2024-01-25 17:20:45.574938 torchmanager-1.3b4/LICENSE
+-rw-r--r--   0        0        0     6845 2024-05-14 19:07:33.491342 torchmanager-1.3b4/README.md
+-rwxr-xr-x   0        0        0      728 2024-05-14 19:09:11.319694 torchmanager-1.3b4/pyproject.toml
+-rw-r--r--   0        0        0      283 2024-04-12 14:34:40.966040 torchmanager-1.3b4/torchmanager/__init__.py
+-rw-r--r--   0        0        0    15405 2024-05-14 19:07:33.493044 torchmanager-1.3b4/torchmanager/basic.py
+-rwxr-xr-x   0        0        0      788 2024-05-14 19:07:33.493522 torchmanager-1.3b4/torchmanager/callbacks/__init__.py
+-rwxr-xr-x   0        0        0     6962 2024-05-14 19:07:33.493946 torchmanager-1.3b4/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     5489 2024-05-14 19:07:33.494198 torchmanager-1.3b4/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3522 2024-01-25 17:20:45.576291 torchmanager-1.3b4/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1971 2024-05-14 19:07:33.494402 torchmanager-1.3b4/torchmanager/callbacks/early_stop.py
+-rwxr-xr-x   0        0        0     2953 2024-05-14 19:07:33.494772 torchmanager-1.3b4/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     4139 2024-05-14 19:07:33.495163 torchmanager-1.3b4/torchmanager/callbacks/functional.py
+-rw-r--r--   0        0        0     2347 2024-05-14 19:07:33.495392 torchmanager-1.3b4/torchmanager/callbacks/lr.py
+-rwxr-xr-x   0        0        0     2372 2024-05-14 19:07:33.495601 torchmanager-1.3b4/torchmanager/callbacks/progress.py
+-rw-r--r--   0        0        0     2600 2024-05-14 19:07:33.495802 torchmanager-1.3b4/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      544 2024-01-25 17:20:45.576732 torchmanager-1.3b4/torchmanager/compatibility.py
+-rw-r--r--   0        0        0      299 2024-05-14 19:07:33.495981 torchmanager-1.3b4/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     5799 2024-05-14 19:07:33.496244 torchmanager-1.3b4/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0     5512 2024-05-14 19:07:33.496527 torchmanager-1.3b4/torchmanager/configs/json.py
+-rw-r--r--   0        0        0     5549 2024-05-14 19:07:33.496810 torchmanager-1.3b4/torchmanager/configs/yaml.py
+-rw-r--r--   0        0        0      172 2024-04-12 14:34:40.967281 torchmanager-1.3b4/torchmanager/core.py
+-rw-r--r--   0        0        0      132 2024-05-14 19:07:33.496979 torchmanager-1.3b4/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     8634 2024-05-14 19:07:33.497183 torchmanager-1.3b4/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     4213 2024-05-14 19:07:33.497455 torchmanager-1.3b4/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      180 2024-01-25 17:20:45.577468 torchmanager-1.3b4/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     8030 2024-05-14 19:07:33.497830 torchmanager-1.3b4/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     2486 2024-05-14 19:07:33.498177 torchmanager-1.3b4/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     6419 2024-05-14 19:07:33.498520 torchmanager-1.3b4/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3156 2024-01-25 17:20:45.577853 torchmanager-1.3b4/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      393 2024-05-14 19:07:33.498871 torchmanager-1.3b4/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     6356 2024-05-14 19:07:33.499140 torchmanager-1.3b4/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     7185 2024-05-14 19:07:33.499479 torchmanager-1.3b4/torchmanager/metrics/conf_mat.py
+-rw-r--r--   0        0        0       68 2024-04-12 14:34:40.968627 torchmanager-1.3b4/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5697 2024-05-14 19:07:33.499841 torchmanager-1.3b4/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2920 2024-05-14 19:07:33.500192 torchmanager-1.3b4/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4630 2024-05-14 19:07:33.500575 torchmanager-1.3b4/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     3544 2024-05-14 19:07:33.500970 torchmanager-1.3b4/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     8734 2024-05-14 19:07:33.501345 torchmanager-1.3b4/torchmanager/testing.py
+-rw-r--r--   0        0        0      288 2024-05-14 19:07:33.501519 torchmanager-1.3b4/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0       43 2024-01-25 17:20:45.578906 torchmanager-1.3b4/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      763 2024-01-25 17:20:45.578987 torchmanager-1.3b4/torchmanager/train/learning_rate.py
+-rwxr-xr-x   0        0        0    15159 2024-05-14 19:07:33.501938 torchmanager-1.3b4/torchmanager/training.py
+-rwxr-xr-x   0        0        0      645 2024-05-14 19:07:33.502288 torchmanager-1.3b4/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0       46 2024-05-14 19:07:33.502404 torchmanager-1.3b4/torchmanager_core/backward/__init__.py
+-rw-r--r--   0        0        0     2747 2024-05-14 19:07:33.502520 torchmanager-1.3b4/torchmanager_core/backward/hook.py
+-rw-r--r--   0        0        0      134 2024-05-14 19:07:33.502622 torchmanager-1.3b4/torchmanager_core/backward/protocols.py
+-rw-r--r--   0        0        0       52 2024-01-25 17:20:45.579434 torchmanager-1.3b4/torchmanager_core/checkpoint/__init__.py
+-rw-r--r--   0        0        0     7689 2024-05-14 19:07:33.502828 torchmanager-1.3b4/torchmanager_core/checkpoint/ckpt.py
+-rw-r--r--   0        0        0      109 2024-01-25 17:20:45.579655 torchmanager-1.3b4/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     6040 2024-05-14 19:08:51.900263 torchmanager-1.3b4/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      265 2024-01-25 17:22:35.173853 torchmanager-1.3b4/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      243 2024-05-14 19:07:33.503010 torchmanager-1.3b4/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-14 19:07:33.503114 torchmanager-1.3b4/torchmanager_core/errors/configs.py
+-rw-r--r--   0        0        0      535 2024-05-14 19:07:33.503272 torchmanager-1.3b4/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2024-01-25 17:20:45.580120 torchmanager-1.3b4/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0      292 2024-05-14 19:07:33.503371 torchmanager-1.3b4/torchmanager_core/errors/version.py
+-rw-r--r--   0        0        0     3281 2024-05-14 19:07:33.503543 torchmanager-1.3b4/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0      157 2024-05-14 19:07:33.503700 torchmanager-1.3b4/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-14 19:07:33.503810 torchmanager-1.3b4/torchmanager_core/random/random.py
+-rw-r--r--   0        0        0     1008 2024-01-25 17:22:35.174100 torchmanager-1.3b4/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2024-01-25 17:20:45.580473 torchmanager-1.3b4/torchmanager_core/typing.py
+-rw-r--r--   0        0        0      157 2024-04-12 14:34:40.970072 torchmanager-1.3b4/torchmanager_core/version/__init__.py
+-rw-r--r--   0        0        0     1307 2024-05-14 19:07:33.504030 torchmanager-1.3b4/torchmanager_core/version/deprecation.py
+-rw-r--r--   0        0        0      138 2024-05-14 19:09:05.466376 torchmanager-1.3b4/torchmanager_core/version/details.py
+-rw-r--r--   0        0        0      318 2024-04-12 14:34:40.970557 torchmanager-1.3b4/torchmanager_core/version/errors.py
+-rw-r--r--   0        0        0     6575 2024-05-14 19:07:33.504764 torchmanager-1.3b4/torchmanager_core/version/version.py
+-rw-r--r--   0        0        0      138 2024-01-25 17:22:35.175250 torchmanager-1.3b4/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      577 2024-05-14 19:07:33.504942 torchmanager-1.3b4/torchmanager_core/view/logging.py
+-rw-r--r--   0        0        0      313 2024-01-25 17:20:45.581203 torchmanager-1.3b4/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0     7580 1970-01-01 00:00:00.000000 torchmanager-1.3b4/PKG-INFO
```

### Comparing `torchmanager-1.3b3/LICENSE` & `torchmanager-1.3b4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/README.md` & `torchmanager-1.3b4/README.md`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/pyproject.toml` & `torchmanager-1.3b4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "torchmanager"
-version = "1.3b3"
-description = "PyTorch Training Manager v1.3 (Beta 3)"
+version = "1.3b4"
+description = "PyTorch Training Manager v1.3 (Beta 4)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
 readme = "README.md"
```

### Comparing `torchmanager-1.3b3/torchmanager/basic.py` & `torchmanager-1.3b4/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/__init__.py` & `torchmanager-1.3b4/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/callback.py` & `torchmanager-1.3b4/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/ckpt.py` & `torchmanager-1.3b4/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/dynamic.py` & `torchmanager-1.3b4/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/early_stop.py` & `torchmanager-1.3b4/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/experiment.py` & `torchmanager-1.3b4/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/functional.py` & `torchmanager-1.3b4/torchmanager/callbacks/functional.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/lr.py` & `torchmanager-1.3b4/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/progress.py` & `torchmanager-1.3b4/torchmanager/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/callbacks/tensorboard.py` & `torchmanager-1.3b4/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/compatibility.py` & `torchmanager-1.3b4/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/configs/basic.py` & `torchmanager-1.3b4/torchmanager/configs/basic.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,14 +63,21 @@
         log_file = os.path.basename(configs.experiment.replace(".exp", ".log"))
         log_path = os.path.join(log_dir, log_file)
         view.set_log_path(log_path=log_path)
 
         # save configs
         configs.save()
 
+        # initialize console
+        formatter = view.logging.Formatter("%(message)s")
+        console = view.logging.StreamHandler()
+        console.setLevel(view.logging.INFO)
+        console.setFormatter(formatter)
+        view.logger.addHandler(console)
+
         # show configs summarize
         if show_summary:
             view.logger.info("------------Settings------------")
             view.logger.info(f"Experiment name: {configs.experiment}")
             configs.show_settings()
             view.logger.info("----------Environments----------")
             configs.show_environments()
```

### Comparing `torchmanager-1.3b3/torchmanager/configs/json.py` & `torchmanager-1.3b4/torchmanager/configs/json.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/configs/yaml.py` & `torchmanager-1.3b4/torchmanager/configs/yaml.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/data/dataset.py` & `torchmanager-1.3b4/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/data/sliding.py` & `torchmanager-1.3b4/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/losses/cross_entropy.py` & `torchmanager-1.3b4/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/losses/dice.py` & `torchmanager-1.3b4/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/losses/loss.py` & `torchmanager-1.3b4/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/losses/mse.py` & `torchmanager-1.3b4/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/metrics/accuracy.py` & `torchmanager-1.3b4/torchmanager/metrics/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def convert(self, from_version: Version) -> None:
         super().convert(from_version)
         if from_version < Version("v1.3"):
             self.dim = self._dim
 
     @torch.no_grad()
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        input = input.argmax(dim=self.dim)
+        input = input.argmax(dim=self._dim) if input.shape[self._dim] > 1 else input > 0
         return super().forward(input, target)
 
 
 class CategoricalAccuracy(SparseCategoricalAccuracy):
     """
     The accuracy metric for categorical labels
```

### Comparing `torchmanager-1.3b3/torchmanager/metrics/conf_mat.py` & `torchmanager-1.3b4/torchmanager/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/metrics/extractor.py` & `torchmanager-1.3b4/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/metrics/iou.py` & `torchmanager-1.3b4/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/metrics/metric.py` & `torchmanager-1.3b4/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/metrics/similarity.py` & `torchmanager-1.3b4/torchmanager/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/testing.py` & `torchmanager-1.3b4/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/train/learning_rate.py` & `torchmanager-1.3b4/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager/training.py` & `torchmanager-1.3b4/torchmanager/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,18 +64,18 @@
             - iterations: An optional `int` of total training iterations, must be smaller than the size of dataset
             - device: A `torch.device` where the data is moved to, should be same as the model
             - use_multi_gpus: A `bool` flag of if using multi gpus
             - callbacks_list: A `list` of callbacks in `Callback`
         - Returns: A summary of `dict` with keys as `str` and values as `float`
         """
         # initialize status
-        self.model.train()
-        self.compiled_losses.train()
-        for m in self.compiled_metrics.values():
-            m.train()
+        self.model = self.model.train()
+        self.loss_fn = self.compiled_losses.train()
+        for k, m in self.compiled_metrics.items():
+            self.compiled_metrics[k] = m.train()
 
         # reset loss and metrics
         self.compiled_losses.reset()
         for m in self.metric_fns.values():
             m.reset()
 
         # initialize iterations
```

### Comparing `torchmanager-1.3b3/torchmanager_core/__init__.py` & `torchmanager-1.3b4/torchmanager_core/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/backward/hook.py` & `torchmanager-1.3b4/torchmanager_core/backward/hook.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/checkpoint/ckpt.py` & `torchmanager-1.3b4/torchmanager_core/checkpoint/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/devices/device.py` & `torchmanager-1.3b4/torchmanager_core/devices/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,36 +23,37 @@
     '''The list of available CUDA devices'''
 except:
     DEFAULT = CPU
     GPU = NotImplemented
     GPUS: list[torch.device] = []
 
 Module = TypeVar('Module', bound=torch.nn.Module)
+P = TypeVar('P', bound=torch.nn.parallel.DataParallel)
 
 
 @overload
-def data_parallel(raw_model: torch.nn.DataParallel[Module], /, devices: list[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.DataParallel[Module]) -> tuple[torch.nn.DataParallel[Module], bool]:
+def data_parallel(raw_model: torch.nn.parallel.DataParallel, /, devices: list[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type[P] = torch.nn.parallel.DataParallel) -> tuple[P, bool]:
     ...
 
 
 @overload
-def data_parallel(raw_model: Module, /, devices: list[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.DataParallel[Module]) -> tuple[Union[Module, torch.nn.DataParallel[Module]], bool]:
+def data_parallel(raw_model: Module, /, devices: list[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type[P] = torch.nn.parallel.DataParallel) -> tuple[Union[Module, P], bool]:
     ...
 
 
-def data_parallel(raw_model: Module, /, devices: list[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.DataParallel[Module]) -> tuple[Union[Module, torch.nn.DataParallel[Module]], bool]:
+def data_parallel(raw_model: Module, /, devices: list[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type[P] = torch.nn.parallel.DataParallel) -> tuple[Union[Module, P], bool]:
     """
     Make a `torch.nn.Module` data parallel
 
     - Parameters:
         - raw_model: A target `torch.nn.Module`
         - devices: A `list` of target `torch.device`
         - output_device: An optional `torch.device` of the target output device for the paralleled model
-        - parallel_type: A `type` of `torch.nn.DataParallel[Module]`
-    - Returns: A `tuple` of either data paralleled `torch.nn.DataParallel[Module]` model if CUDA is available or a raw model if not, and a `bool` flag of if the model data paralleled successfuly.
+        - parallel_type: A `type` of `torch.nn.parallel.DataParallel`
+    - Returns: A `tuple` of either data paralleled `torch.nn.parallel.DataParallel` model if CUDA is available or a raw model if not, and a `bool` flag of if the model data paralleled successfuly.
     """
     if isinstance(raw_model, parallel_type):
         return raw_model, True
     elif GPU is not NotImplemented:
         device_ids = [d.index for d in devices]
         model = parallel_type(raw_model, device_ids=device_ids, output_device=output_device)
         return model, True
```

### Comparing `torchmanager-1.3b3/torchmanager_core/errors/runtime.py` & `torchmanager-1.3b4/torchmanager_core/errors/runtime.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/errors/train.py` & `torchmanager-1.3b4/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/protocols.py` & `torchmanager-1.3b4/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/random/random.py` & `torchmanager-1.3b4/torchmanager_core/random/random.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/random/seed.py` & `torchmanager-1.3b4/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/version/deprecation.py` & `torchmanager-1.3b4/torchmanager_core/version/deprecation.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/version/version.py` & `torchmanager-1.3b4/torchmanager_core/version/version.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/torchmanager_core/view/logging.py` & `torchmanager-1.3b4/torchmanager_core/view/logging.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.3b3/PKG-INFO` & `torchmanager-1.3b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager
-Version: 1.3b3
-Summary: PyTorch Training Manager v1.3 (Beta 3)
+Version: 1.3b4
+Summary: PyTorch Training Manager v1.3 (Beta 4)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

