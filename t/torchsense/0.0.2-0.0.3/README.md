# Comparing `tmp/torchsense-0.0.2.tar.gz` & `tmp/torchsense-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsense-0.0.2.tar", last modified: Sun May 12 15:21:14 2024, max compression
+gzip compressed data, was "torchsense-0.0.3.tar", last modified: Tue May 14 01:35:15 2024, max compression
```

## Comparing `torchsense-0.0.2.tar` & `torchsense-0.0.3.tar`

### file list

```diff
@@ -1,58 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.557749 torchsense-0.0.2/
--rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      311 2024-05-12 15:21:14.556746 torchsense-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2024-05-12 15:15:03.000000 torchsense-0.0.2/README.md
--rw-rw-rw-   0        0        0      529 2024-05-12 15:21:10.000000 torchsense-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 15:21:14.557749 torchsense-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.482028 torchsense-0.0.2/torchsense/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.495877 torchsense-0.0.2/torchsense/datasets/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.2/torchsense/datasets/__init__.py
--rw-rw-rw-   0        0        0     5075 2024-05-06 07:20:55.000000 torchsense-0.0.2/torchsense/datasets/dataset2.py
--rw-rw-rw-   0        0        0    13389 2024-05-12 14:40:19.000000 torchsense-0.0.2/torchsense/datasets/folder.py
--rw-rw-rw-   0        0        0     2502 2024-05-12 14:31:48.000000 torchsense-0.0.2/torchsense/datasets/utils.py
--rw-rw-rw-   0        0        0     4280 2024-05-06 06:45:31.000000 torchsense-0.0.2/torchsense/datasets/vision.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.551262 torchsense-0.0.2/torchsense/models/
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/Autoencode.py
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/Autoencoder.py
--rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/LSTM.py
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/__init__.py
--rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/alexnet.py
--rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/attention.py
--rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/cct.py
--rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/deeplab.py
--rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/deeplabv3p.py
--rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/densenet.py
--rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/googlenet.py
--rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/inceptionv3.py
--rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/inceptionv4.py
--rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenet.py
--rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenetv1.py
--rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenetv2.py
--rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenetv3.py
--rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/nasnet.py
--rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/preactresnet.py
--rw-rw-rw-   0        0        0     6759 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/resnet.py
--rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/resnext.py
--rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/rir.py
--rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/sealex.py
--rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/senet.py
--rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/shufflenet.py
--rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/shufflenetv2.py
--rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/simple_vit_1d.py
--rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/squeezenet.py
--rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/stochasticdepth.py
--rw-rw-rw-   0        0        0     4499 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/unet.py
--rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/vgg.py
--rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/vit.py
--rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/wideresidual.py
--rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/xception.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.553356 torchsense-0.0.2/torchsense/transforms/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.2/torchsense/transforms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.555742 torchsense-0.0.2/torchsense.egg-info/
--rw-rw-rw-   0        0        0      311 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1469 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.934951 torchsense-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      311 2024-05-14 01:35:15.934951 torchsense-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2839 2024-05-14 01:10:06.000000 torchsense-0.0.3/README.md
+-rw-rw-rw-   0        0        0      529 2024-05-14 01:35:07.000000 torchsense-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 01:35:15.934951 torchsense-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.740406 torchsense-0.0.3/torchsense/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.777057 torchsense-0.0.3/torchsense/datasets/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.3/torchsense/datasets/__init__.py
+-rw-rw-rw-   0        0        0     5076 2024-05-13 11:17:11.000000 torchsense-0.0.3/torchsense/datasets/dataset2.py
+-rw-rw-rw-   0        0        0    13392 2024-05-13 13:02:23.000000 torchsense-0.0.3/torchsense/datasets/folder.py
+-rw-rw-rw-   0        0        0     2505 2024-05-13 11:17:11.000000 torchsense-0.0.3/torchsense/datasets/utils.py
+-rw-rw-rw-   0        0        0     4281 2024-05-13 11:17:11.000000 torchsense-0.0.3/torchsense/datasets/vision.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.907626 torchsense-0.0.3/torchsense/models/
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/Autoencode.py
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/Autoencoder.py
+-rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/LSTM.py
+-rw-rw-rw-   0        0        0       41 2024-05-14 01:34:50.000000 torchsense-0.0.3/torchsense/models/__init__.py
+-rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/alexnet.py
+-rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/attention.py
+-rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/cct.py
+-rw-rw-rw-   0        0        0      938 2024-05-13 12:27:30.000000 torchsense-0.0.3/torchsense/models/cnn4.py
+-rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/deeplab.py
+-rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/deeplabv3p.py
+-rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/densenet.py
+-rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/googlenet.py
+-rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/inceptionv3.py
+-rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/inceptionv4.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.914693 torchsense-0.0.3/torchsense/models/lit_model/
+-rw-rw-rw-   0        0        0       59 2024-05-13 11:53:41.000000 torchsense-0.0.3/torchsense/models/lit_model/__init__.py
+-rw-rw-rw-   0        0        0      973 2024-05-13 12:49:15.000000 torchsense-0.0.3/torchsense/models/lit_model/litmodel.py
+-rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/mobilenet.py
+-rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/mobilenetv1.py
+-rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/mobilenetv2.py
+-rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/mobilenetv3.py
+-rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/nasnet.py
+-rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/preactresnet.py
+-rw-rw-rw-   0        0        0     6759 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/resnet.py
+-rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/resnext.py
+-rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/rir.py
+-rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/sealex.py
+-rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/senet.py
+-rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/shufflenet.py
+-rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/shufflenetv2.py
+-rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/simple_vit_1d.py
+-rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/squeezenet.py
+-rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/stochasticdepth.py
+-rw-rw-rw-   0        0        0     4170 2024-05-14 01:33:19.000000 torchsense-0.0.3/torchsense/models/unet.py
+-rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/vgg.py
+-rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/vit.py
+-rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/wideresidual.py
+-rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.3/torchsense/models/xception.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.920761 torchsense-0.0.3/torchsense/trainer/
+-rw-rw-rw-   0        0        0       48 2024-05-13 12:49:15.000000 torchsense-0.0.3/torchsense/trainer/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-05-13 12:40:00.000000 torchsense-0.0.3/torchsense/trainer/trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.922785 torchsense-0.0.3/torchsense/transforms/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.3/torchsense/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.927018 torchsense-0.0.3/torchsense/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:12:46.000000 torchsense-0.0.3/torchsense/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:35:15.930951 torchsense-0.0.3/torchsense.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-05-14 01:35:15.000000 torchsense-0.0.3/torchsense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2024-05-14 01:35:15.000000 torchsense-0.0.3/torchsense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 01:35:15.000000 torchsense-0.0.3/torchsense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 01:35:15.000000 torchsense-0.0.3/torchsense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 01:35:15.000000 torchsense-0.0.3/torchsense.egg-info/top_level.txt
```

### Comparing `torchsense-0.0.2/LICENSE` & `torchsense-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/README.md` & `torchsense-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #### Pip
 
 ```bash
 # clone project
 git clone https://github.com/xibrer/torchsense.git
 
 # pip install
-
 pip install torchsense
 ```
 
 ## Project Structure
 
 The directory structure of new project looks like this:
 
@@ -39,31 +38,60 @@
         ├── nsdf3.ext
         └── ...
         └── asd932_.ext
 ```
 
 
 ## How to run
-
-Train model with default configuration
+torchsense provide two-way to run model
+### Train model with default configuration
 
 ```python 
 # ensure you already install torch and lightning
-from torchsense.datasets.folder import ImageFolder
+from torchsense.datasets.folder import SensorFolder
 from torch.utils.data import DataLoader
 
 # you need to input
 list1 = [key1,key2,key3] # example ["acc", "mix_mic", "mic"]
-root_data = "data" # data root path
+root_data = "data1" # data1 root path
 
 # as normal
 data = ImageFolder(root=root_data, params=list1)
 train_set, test_set = data.train_test_split(0.5)
 train_loader = DataLoader(train_set, batch_size=1, shuffle=True)
 test_loader = DataLoader(test_set, batch_size=1, shuffle=False)
 
 for i, batch in enumerate(train_loader):
     acc, mix, mic = batch[0]
     # ... train your self
 ```
 
 now model only support .mat file
+### Train model with custom configuration
+```python
+import torch
+from torchsense.trainer import Trainer
+from torchsense.models.cnn4 import CNN4
+
+
+def train():
+    from torchvision.datasets import MNIST
+    from torchvision.transforms import ToTensor
+
+    train_set = MNIST(root="./tmp/data1/MNIST", train=True, transform=ToTensor(), download=True)
+    val_set = MNIST(root="./tmp/data1/MNIST", train=False, transform=ToTensor(), download=False)
+
+    train_loader = torch.utils.data.DataLoader(
+        train_set, batch_size=64, shuffle=True, pin_memory=torch.cuda.is_available(), num_workers=0
+    )
+    val_loader = torch.utils.data.DataLoader(
+        val_set, batch_size=64, shuffle=False, pin_memory=torch.cuda.is_available(), num_workers=0
+    )
+
+    model = CNN4()
+    trainer = Trainer(model, max_epochs=5)
+    trainer.fit(train_loader, val_loader)
+```
+
+## Thanks
+
+u-net parts reference [milesial](https://github.com/milesial/Pytorch-UNet/tree/master)
```

#### html2text {}

```diff
@@ -4,16 +4,29 @@
 It provides I/O, signal and data processing functions, datasets, model
 implementations and application components. ## Installation #### Pip ```bash #
 clone project git clone https://github.com/xibrer/torchsense.git # pip install
 pip install torchsense ``` ## Project Structure The directory structure of new
 project looks like this: ``` data/ âââ class_x â âââ xxx.ext â
 âââ xxy.ext â âââ ... â âââ xxz.ext âââ class_y
 âââ 123.ext âââ nsdf3.ext âââ ... âââ asd932_.ext ```
-## How to run Train model with default configuration ```python # ensure you
-already install torch and lightning from torchsense.datasets.folder import
-ImageFolder from torch.utils.data import DataLoader # you need to input list1 =
-[key1,key2,key3] # example ["acc", "mix_mic", "mic"] root_data = "data" # data
-root path # as normal data = ImageFolder(root=root_data, params=list1)
-train_set, test_set = data.train_test_split(0.5) train_loader = DataLoader
-(train_set, batch_size=1, shuffle=True) test_loader = DataLoader(test_set,
-batch_size=1, shuffle=False) for i, batch in enumerate(train_loader): acc, mix,
-mic = batch[0] # ... train your self ``` now model only support .mat file
+## How to run torchsense provide two-way to run model ### Train model with
+default configuration ```python # ensure you already install torch and
+lightning from torchsense.datasets.folder import SensorFolder from
+torch.utils.data import DataLoader # you need to input list1 = [key1,key2,key3]
+# example ["acc", "mix_mic", "mic"] root_data = "data1" # data1 root path # as
+normal data = ImageFolder(root=root_data, params=list1) train_set, test_set =
+data.train_test_split(0.5) train_loader = DataLoader(train_set, batch_size=1,
+shuffle=True) test_loader = DataLoader(test_set, batch_size=1, shuffle=False)
+for i, batch in enumerate(train_loader): acc, mix, mic = batch[0] # ... train
+your self ``` now model only support .mat file ### Train model with custom
+configuration ```python import torch from torchsense.trainer import Trainer
+from torchsense.models.cnn4 import CNN4 def train(): from torchvision.datasets
+import MNIST from torchvision.transforms import ToTensor train_set = MNIST
+(root="./tmp/data1/MNIST", train=True, transform=ToTensor(), download=True)
+val_set = MNIST(root="./tmp/data1/MNIST", train=False, transform=ToTensor(),
+download=False) train_loader = torch.utils.data.DataLoader( train_set,
+batch_size=64, shuffle=True, pin_memory=torch.cuda.is_available(),
+num_workers=0 ) val_loader = torch.utils.data.DataLoader( val_set,
+batch_size=64, shuffle=False, pin_memory=torch.cuda.is_available(),
+num_workers=0 ) model = CNN4() trainer = Trainer(model, max_epochs=5)
+trainer.fit(train_loader, val_loader) ``` ## Thanks u-net parts reference
+[milesial](https://github.com/milesial/Pytorch-UNet/tree/master)
```

### Comparing `torchsense-0.0.2/pyproject.toml` & `torchsense-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchsense"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Xingwei Wang", email = "wxwjkl123@gmail.com"},
 ]
 description = "Torchsense is a library for sensor data processing with PyTorch"
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
```

### Comparing `torchsense-0.0.2/torchsense/datasets/dataset2.py` & `torchsense-0.0.3/torchsense/datasets/dataset2.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
 
     Args:
         root (str or ``pathlib.Path``): Root directory where the dataset's top level directory is found
         sessions (Tuple[int]): Tuple of sessions (1-5) to use. (Default: ``(1, 2, 3, 4, 5)``)
         utterance_type (str or None, optional): Which type(s) of utterances to include in the dataset.
             Options: ("scripted", "improvised", ``None``). If ``None``, both scripted and improvised
-            data are used.
+            data1 are used.
     """
 
     def __init__(
             self,
             root: Union[str, Path],
             sessions: Tuple[str] = (1, 2, 3, 4, 5),
             utterance_type: Optional[str] = None,
```

### Comparing `torchsense-0.0.2/torchsense/datasets/folder.py` & `torchsense-0.0.3/torchsense/datasets/folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             msg += f"Supported extensions are: {extensions if isinstance(extensions, str) else ', '.join(extensions)}"
         raise FileNotFoundError(msg)
 
     return instances
 
 
 class DatasetFolder(VisionDataset):
-    """A generic data loader.
+    """A generic data1 loader.
 
     This default directory structure can be customized by overriding the
     :meth:`find_classes` method.
 
     Args:
         root (str or ``pathlib.Path``): Root directory path.
         loader (callable): A function to load a sample given its path.
@@ -252,25 +252,36 @@
         if len(sample) == 1:
             sample = sample[0]
         return sample, target
 
     def __len__(self) -> int:
         return len(self.samples)
 
+    def train_test_split(self, val_ratio):
+        """
+        划分训练集和验证集的函数，接收一个参数：`val_ratio`（验证集的比例）。
+        这个函数会返回划分好的训练集和验证集。
+        """
+        val_size = int(val_ratio * len(self))
+        train_size = len(self) - val_size
+        train_set, val_set = random_split(self, [train_size, val_size])
+
+        return train_set, val_set
+
 
 IMG_EXTENSIONS = (".mat", ".jpeg", ".npz")
 
 
 # TODO: specify the return type
 def default_loader(path: str, params: list) -> Any:
     return load_file(path, params)
 
 
-class ImageFolder(DatasetFolder):
-    """A generic data loader where the images are arranged in this way by default: ::
+class SensorFolder(DatasetFolder):
+    """A generic data1 loader where the images are arranged in this way by default: ::
 
         root/dog/xxx.png
         root/dog/xxy.png
         root/dog/[...]/xxz.png
 
         root/cat/123.png
         root/cat/nsdf3.png
@@ -314,18 +325,7 @@
             IMG_EXTENSIONS if is_valid_file is None else None,
             transform=transform,
             target_transform=target_transform,
             is_valid_file=is_valid_file,
             allow_empty=allow_empty,
         )
         self.imgs = self.samples
-
-    def train_test_split(self, val_ratio):
-        """
-        划分训练集和验证集的函数，接收一个参数：`val_ratio`（验证集的比例）。
-        这个函数会返回划分好的训练集和验证集。
-        """
-        val_size = int(val_ratio * len(self))
-        train_size = len(self) - val_size
-        train_set, val_set = random_split(self, [train_size, val_size])
-
-        return train_set, val_set
```

### Comparing `torchsense-0.0.2/torchsense/datasets/utils.py` & `torchsense-0.0.3/torchsense/datasets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     except NotImplementedError:
         all_mat_data = File(path)
         return get_meta_data(all_mat_data, list_j)
 
 
 def get_meta_data(raw_data: Union[Dict[str, Any], File], keys: List[str] = None) -> Tuple:
     if keys is None:
-        # If list_j is empty, return all values in data as a tuple
+        # If list_j is empty, return all values in data1 as a tuple
         # Remove meta info
         if '__header__' in raw_data:
             del raw_data['__header__']
         if '__version__' in raw_data:
             del raw_data['__version__']
         if '__globals__' in raw_data:
             del raw_data['__globals__']
@@ -78,9 +78,9 @@
 
 def load_npz_file(path, keys):
     npz_data = np.load(path)
     return tuple(npz_data[key] for key in keys if key in npz_data)
 
 # 使用示例
 # file_path = 'example.txt'
-# data = load_file(file_path)
-# print(data)
+# data1 = load_file(file_path)
+# print(data1)
```

### Comparing `torchsense-0.0.2/torchsense/datasets/vision.py` & `torchsense-0.0.3/torchsense/datasets/vision.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def __getitem__(self, index: int) -> Any:
         """
         Args:
             index (int): Index
 
         Returns:
-            (Any): Sample and meta data, optionally transformed by the respective transforms.
+            (Any): Sample and meta data1, optionally transformed by the respective transforms.
         """
         raise NotImplementedError
 
     def __len__(self) -> int:
         raise NotImplementedError
 
     def __repr__(self) -> str:
```

### Comparing `torchsense-0.0.2/torchsense/models/Autoencode.py` & `torchsense-0.0.3/torchsense/models/Autoencode.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/Autoencoder.py` & `torchsense-0.0.3/torchsense/models/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/LSTM.py` & `torchsense-0.0.3/torchsense/models/LSTM.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/alexnet.py` & `torchsense-0.0.3/torchsense/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/attention.py` & `torchsense-0.0.3/torchsense/models/attention.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/cct.py` & `torchsense-0.0.3/torchsense/models/cct.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/deeplab.py` & `torchsense-0.0.3/torchsense/models/deeplab.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/deeplabv3p.py` & `torchsense-0.0.3/torchsense/models/deeplabv3p.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/densenet.py` & `torchsense-0.0.3/torchsense/models/densenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/googlenet.py` & `torchsense-0.0.3/torchsense/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/inceptionv3.py` & `torchsense-0.0.3/torchsense/models/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/inceptionv4.py` & `torchsense-0.0.3/torchsense/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/mobilenet.py` & `torchsense-0.0.3/torchsense/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/mobilenetv1.py` & `torchsense-0.0.3/torchsense/models/mobilenetv1.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/mobilenetv2.py` & `torchsense-0.0.3/torchsense/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/mobilenetv3.py` & `torchsense-0.0.3/torchsense/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/nasnet.py` & `torchsense-0.0.3/torchsense/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/preactresnet.py` & `torchsense-0.0.3/torchsense/models/preactresnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/resnet.py` & `torchsense-0.0.3/torchsense/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/resnext.py` & `torchsense-0.0.3/torchsense/models/resnext.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/rir.py` & `torchsense-0.0.3/torchsense/models/rir.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/rnn.py` & `torchsense-0.0.3/torchsense/models/rnn.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/senet.py` & `torchsense-0.0.3/torchsense/models/senet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/shufflenet.py` & `torchsense-0.0.3/torchsense/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/shufflenetv2.py` & `torchsense-0.0.3/torchsense/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/simple_vit_1d.py` & `torchsense-0.0.3/torchsense/models/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/squeezenet.py` & `torchsense-0.0.3/torchsense/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/stochasticdepth.py` & `torchsense-0.0.3/torchsense/models/stochasticdepth.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/vgg.py` & `torchsense-0.0.3/torchsense/models/vgg.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/vit.py` & `torchsense-0.0.3/torchsense/models/vit.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/wideresidual.py` & `torchsense-0.0.3/torchsense/models/wideresidual.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense/models/xception.py` & `torchsense-0.0.3/torchsense/models/xception.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.2/torchsense.egg-info/SOURCES.txt` & `torchsense-0.0.3/torchsense.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 torchsense/models/Autoencode.py
 torchsense/models/Autoencoder.py
 torchsense/models/LSTM.py
 torchsense/models/__init__.py
 torchsense/models/alexnet.py
 torchsense/models/attention.py
 torchsense/models/cct.py
+torchsense/models/cnn4.py
 torchsense/models/deeplab.py
 torchsense/models/deeplabv3p.py
 torchsense/models/densenet.py
 torchsense/models/googlenet.py
 torchsense/models/inceptionv3.py
 torchsense/models/inceptionv4.py
 torchsense/models/mobilenet.py
@@ -43,8 +44,13 @@
 torchsense/models/squeezenet.py
 torchsense/models/stochasticdepth.py
 torchsense/models/unet.py
 torchsense/models/vgg.py
 torchsense/models/vit.py
 torchsense/models/wideresidual.py
 torchsense/models/xception.py
-torchsense/transforms/__init__.py
+torchsense/models/lit_model/__init__.py
+torchsense/models/lit_model/litmodel.py
+torchsense/trainer/__init__.py
+torchsense/trainer/trainer.py
+torchsense/transforms/__init__.py
+torchsense/utils/__init__.py
```

