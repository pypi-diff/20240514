# Comparing `tmp/seg_tgce-0.0.1.tar.gz` & `tmp/seg_tgce-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seg_tgce-0.0.1.tar", max compression
+gzip compressed data, was "seg_tgce-0.1.0.tar", max compression
```

## Comparing `seg_tgce-0.0.1.tar` & `seg_tgce-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/README.md
--rw-r--r--   0        0        0      992 2024-05-14 02:45:12.221779 seg_tgce-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 14:27:20.493094 seg_tgce-0.0.1/seg_tgce/data/crowd_seg/__init__.py
--rw-r--r--   0        0        0     4937 2024-05-07 10:46:36.549085 seg_tgce-0.0.1/seg_tgce/data/crowd_seg/generator.py
--rw-r--r--   0        0        0      475 2024-04-30 04:42:11.177868 seg_tgce-0.0.1/seg_tgce/data/crowd_seg/map.py
--rw-r--r--   0        0        0     2231 2024-05-06 04:51:09.581252 seg_tgce-0.0.1/seg_tgce/data/crowd_seg/visualizer.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/data/oxford_pet/__init__.py
--rw-r--r--   0        0        0     2465 2024-05-06 05:34:13.661853 seg_tgce-0.0.1/seg_tgce/data/oxford_pet/disturbance/model.py
--rw-r--r--   0        0        0     2711 2024-05-14 03:29:38.912294 seg_tgce-0.0.1/seg_tgce/data/oxford_pet/oxford_iiit_pet.py
--rw-r--r--   0        0        0      905 2024-05-06 04:41:48.714086 seg_tgce-0.0.1/seg_tgce/data/oxford_pet/oxford_pet.py
--rw-r--r--   0        0        0     2302 2024-05-06 04:49:22.008457 seg_tgce-0.0.1/seg_tgce/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/experiments/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/experiments/apr_14_2024/__init__.py
--rw-r--r--   0        0        0      856 2024-05-06 05:22:24.575116 seg_tgce-0.0.1/seg_tgce/experiments/apr_14_2024/experiment.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/loss/__init__.py
--rw-r--r--   0        0        0     3290 2024-05-06 04:49:42.271689 seg_tgce-0.0.1/seg_tgce/loss/tgce.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/metrics/__init__.py
--rw-r--r--   0        0        0     1225 2024-05-06 05:24:38.627838 seg_tgce-0.0.1/seg_tgce/metrics/dice_coefficient.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/models/__init__.py
--rw-r--r--   0        0        0      746 2024-05-06 05:22:57.754965 seg_tgce-0.0.1/seg_tgce/models/ma_model.py
--rw-r--r--   0        0        0     4618 2024-05-06 05:10:53.688560 seg_tgce-0.0.1/seg_tgce/models/unet.py
--rw-r--r--   0        0        0        0 2024-04-30 04:42:11.177868 seg_tgce-0.0.1/seg_tgce/py.typed
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/run/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 04:39:26.044844 seg_tgce-0.0.1/seg_tgce/run/oxford_ma_runner/__init__.py
--rw-r--r--   0        0        0      414 2024-05-06 05:13:40.777698 seg_tgce-0.0.1/seg_tgce/run/oxford_ma_runner/model_result.py
--rw-r--r--   0        0        0     2468 2024-05-06 05:24:38.624505 seg_tgce-0.0.1/seg_tgce/run/oxford_ma_runner/plotting.py
--rw-r--r--   0        0        0     7072 2024-05-07 11:10:44.874873 seg_tgce-0.0.1/seg_tgce/run/oxford_ma_runner/runner.py
--rw-r--r--   0        0        0      800 2024-04-16 19:11:40.745930 seg_tgce-0.0.1/seg_tgce/run/runner.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 seg_tgce-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      322 2024-05-14 04:12:07.157195 seg_tgce-0.1.0/README.md
+-rw-r--r--   0        0        0     1580 2024-05-14 04:12:07.157195 seg_tgce-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 14:27:20.493094 seg_tgce-0.1.0/seg_tgce/data/crowd_seg/__init__.py
+-rw-r--r--   0        0        0     4937 2024-05-07 10:46:36.549085 seg_tgce-0.1.0/seg_tgce/data/crowd_seg/generator.py
+-rw-r--r--   0        0        0      475 2024-04-30 04:42:11.177868 seg_tgce-0.1.0/seg_tgce/data/crowd_seg/map.py
+-rw-r--r--   0        0        0     2231 2024-05-06 04:51:09.581252 seg_tgce-0.1.0/seg_tgce/data/crowd_seg/visualizer.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/data/oxford_pet/__init__.py
+-rw-r--r--   0        0        0     2465 2024-05-06 05:34:13.661853 seg_tgce-0.1.0/seg_tgce/data/oxford_pet/disturbance/model.py
+-rw-r--r--   0        0        0     2711 2024-05-14 03:29:38.912294 seg_tgce-0.1.0/seg_tgce/data/oxford_pet/oxford_iiit_pet.py
+-rw-r--r--   0        0        0      876 2024-05-14 03:55:28.061819 seg_tgce-0.1.0/seg_tgce/data/oxford_pet/oxford_pet.py
+-rw-r--r--   0        0        0     2228 2024-05-14 03:55:28.058486 seg_tgce-0.1.0/seg_tgce/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/experiments/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/experiments/apr_14_2024/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-06 05:22:24.575116 seg_tgce-0.1.0/seg_tgce/experiments/apr_14_2024/experiment.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/loss/__init__.py
+-rw-r--r--   0        0        0     3290 2024-05-06 04:49:42.271689 seg_tgce-0.1.0/seg_tgce/loss/tgce.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/metrics/__init__.py
+-rw-r--r--   0        0        0     1225 2024-05-06 05:24:38.627838 seg_tgce-0.1.0/seg_tgce/metrics/dice_coefficient.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/models/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-06 05:22:57.754965 seg_tgce-0.1.0/seg_tgce/models/ma_model.py
+-rw-r--r--   0        0        0     4618 2024-05-06 05:10:53.688560 seg_tgce-0.1.0/seg_tgce/models/unet.py
+-rw-r--r--   0        0        0        0 2024-04-30 04:42:11.177868 seg_tgce-0.1.0/seg_tgce/py.typed
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/run/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 04:39:26.044844 seg_tgce-0.1.0/seg_tgce/run/oxford_ma_runner/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-06 05:13:40.777698 seg_tgce-0.1.0/seg_tgce/run/oxford_ma_runner/model_result.py
+-rw-r--r--   0        0        0     2468 2024-05-06 05:24:38.624505 seg_tgce-0.1.0/seg_tgce/run/oxford_ma_runner/plotting.py
+-rw-r--r--   0        0        0     7072 2024-05-07 11:10:44.874873 seg_tgce-0.1.0/seg_tgce/run/oxford_ma_runner/runner.py
+-rw-r--r--   0        0        0      800 2024-04-16 19:11:40.745930 seg_tgce-0.1.0/seg_tgce/run/runner.py
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 seg_tgce-0.1.0/PKG-INFO
```

### Comparing `seg_tgce-0.0.1/pyproject.toml` & `seg_tgce-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+[project]
+description = "Framework for handling image segmentation in the context of multiple annotators"
+name = "seg_tgce"
+version = "0.1.0"
+readme = "README.md"
+authors = [{ name = "Brandon Lotero", email = "blotero@gmail.com" }]
+maintainers = [{ name = "Brandon Lotero", email = "blotero@gmail.com" }]
+license = { file = "../LICENSE" }
+
+[project.urls]
+Homepage = "https://github.com/blotero/seg_tgce"
+Documentation = "https://seg-tgce.readthedocs.io/en/latest/"
+Repository = "https://github.com/blotero/seg_tgce"
+Issues = "https://github.com/blotero/seg_tgce/issues"
+
 [tool.poetry]
 name = "seg_tgce"
-version = "0.0.1"
+version = "0.1.0"
 authors = ["Brandon Lotero <blotero@gmail.com>"]
 description = "A package for the SEG TGCE project"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
@@ -16,14 +31,15 @@
 python = ">=3.11,<3.12"
 numpy = "^1.26.4"
 keras = "2.15.0"
 tensorflow = "2.15.1"
 matplotlib = "^3.8.4"
 opencv-python = "^4.9.0.80"
 tensorflow-datasets = "^4.9.4"
+gdown = "^5.2.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `seg_tgce-0.0.1/seg_tgce/data/crowd_seg/generator.py` & `seg_tgce-0.1.0/seg_tgce/data/crowd_seg/generator.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/data/crowd_seg/visualizer.py` & `seg_tgce-0.1.0/seg_tgce/data/crowd_seg/visualizer.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/data/oxford_pet/disturbance/model.py` & `seg_tgce-0.1.0/seg_tgce/data/oxford_pet/disturbance/model.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/data/oxford_pet/oxford_iiit_pet.py` & `seg_tgce-0.1.0/seg_tgce/data/oxford_pet/oxford_iiit_pet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/data/oxford_pet/oxford_pet.py` & `seg_tgce-0.1.0/seg_tgce/data/oxford_pet/oxford_pet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tensorflow as tf
-from gcpds.image_segmentation.datasets.segmentation import OxfordIiitPet
 from keras.models import Model
 
 from seg_tgce.data.utils import map_dataset_multiple_annotators
 
+from .oxford_iiit_pet import OxfordIiitPet
+
 MODEL_ORIGINAL_SHAPE = (256, 256)
 
 
 def get_data_multiple_annotators(
     annotation_models: list[Model],
     target_shape: tuple[int, int] = (256, 256),
     batch_size: int = 32,
```

### Comparing `seg_tgce-0.0.1/seg_tgce/data/utils.py` & `seg_tgce-0.1.0/seg_tgce/data/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from typing import Tuple
 
 import tensorflow as tf
-from gcpds.image_segmentation.datasets.segmentation import OxfordIiitPet
 from keras.models import Model
+from tensorflow import Tensor
 
 
 def disturb_mask(
     model: Model,
-    image: tf.Tensor,
+    image: Tensor,
     model_shape: Tuple[int, int],
     target_shape: Tuple[int, int],
-) -> tf.Tensor:
+) -> Tensor:
     return tf.image.resize(model(tf.image.resize(image, model_shape)), target_shape)
 
 
-def mix_channels(mask: tf.Tensor) -> tf.Tensor:
+def mix_channels(mask: Tensor) -> Tensor:
     return tf.stack([mask, 1 - mask], axis=-2)
 
 
 def add_noisy_annotators(
-    img: tf.Tensor,
-    models: list[tf.Tensor],
+    img: Tensor,
+    models: list[Tensor],
     model_shape: Tuple[int, int],
     target_shape: Tuple[int, int],
-) -> tf.Tensor:
+) -> Tensor:
     return tf.transpose(
         [
             disturb_mask(model, img, model_shape=model_shape, target_shape=target_shape)
             for model in models
         ],
         [2, 3, 1, 4, 0],
     )
 
 
 def map_dataset_multiple_annotators(
-    dataset: OxfordIiitPet,
+    dataset: Tensor,
     target_shape: tuple[int, int],
     model_shape: tuple[int, int],
     batch_size: int,
     disturbance_models: list[Model],
-) -> tf.Tensor:
+) -> Tensor:
     dataset_ = dataset.map(
         lambda img, mask, label, id_img: (img, mask),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
 
     dataset_ = dataset_.map(
         lambda img, mask: (
```

### Comparing `seg_tgce-0.0.1/seg_tgce/experiments/apr_14_2024/experiment.py` & `seg_tgce-0.1.0/seg_tgce/experiments/apr_14_2024/experiment.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/loss/tgce.py` & `seg_tgce-0.1.0/seg_tgce/loss/tgce.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/metrics/dice_coefficient.py` & `seg_tgce-0.1.0/seg_tgce/metrics/dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/models/ma_model.py` & `seg_tgce-0.1.0/seg_tgce/models/ma_model.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/models/unet.py` & `seg_tgce-0.1.0/seg_tgce/models/unet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/run/oxford_ma_runner/plotting.py` & `seg_tgce-0.1.0/seg_tgce/run/oxford_ma_runner/plotting.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/run/oxford_ma_runner/runner.py` & `seg_tgce-0.1.0/seg_tgce/run/oxford_ma_runner/runner.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.0.1/seg_tgce/run/runner.py` & `seg_tgce-0.1.0/seg_tgce/run/runner.py`

 * *Files identical despite different names*

