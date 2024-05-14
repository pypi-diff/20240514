# Comparing `tmp/eztils-0.4.93.tar.gz` & `tmp/eztils-0.4.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.93.tar", max compression
+gzip compressed data, was "eztils-0.4.94.tar", max compression
```

## Comparing `eztils-0.4.93.tar` & `eztils-0.4.94.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2024-03-29 03:11:19.401071 eztils-0.4.93/LICENSE
--rw-r--r--   0        0        0    12741 2024-03-29 03:11:19.401071 eztils-0.4.93/README.md
--rw-r--r--   0        0        0     5076 2024-03-29 03:11:19.401071 eztils-0.4.93/eztils/__init__.py
--rw-r--r--   0        0        0     5259 2024-03-29 03:11:19.401071 eztils-0.4.93/eztils/dict_operations.py
--rw-r--r--   0        0        0     2534 2024-03-29 03:11:19.401071 eztils-0.4.93/eztils/ezitertools.py
--rw-r--r--   0        0        0     3376 2024-03-29 03:11:19.401071 eztils-0.4.93/eztils/ezlogging.py
--rw-r--r--   0        0        0     2341 2024-03-29 03:11:19.401071 eztils-0.4.93/eztils/ezmath.py
--rw-r--r--   0        0        0     6073 2024-03-29 03:11:19.401071 eztils-0.4.93/eztils/git/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/persistence/__init__.py
--rw-r--r--   0        0        0      905 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/persistence/hf.py
--rw-r--r--   0        0        0     4594 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/run_parallel.py
--rw-r--r--   0        0        0     4394 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/serialization.py
--rw-r--r--   0        0        0     2758 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/structures.py
--rw-r--r--   0        0        0     3101 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/__init__.py
--rw-r--r--   0        0        0    15598 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/distributions.py
--rw-r--r--   0        0        0      307 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/lightning.py
--rw-r--r--   0        0        0      368 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/math.py
--rw-r--r--   0        0        0     3049 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/modules.py
--rw-r--r--   0        0        0     2120 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/parameters.py
--rw-r--r--   0        0        0     2617 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/tensor_creators.py
--rw-r--r--   0        0        0     4227 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/to.py
--rw-r--r--   0        0        0     2220 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/torch/wandb.py
--rw-r--r--   0        0        0      586 2024-03-29 03:11:19.405071 eztils-0.4.93/eztils/typer/__init__.py
--rw-r--r--   0        0        0     4069 2024-03-29 03:11:19.405071 eztils-0.4.93/pyproject.toml
--rw-r--r--   0        0        0    14281 1970-01-01 00:00:00.000000 eztils-0.4.93/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-30 15:35:27.736996 eztils-0.4.94/LICENSE
+-rw-r--r--   0        0        0    12741 2024-03-30 15:35:27.736996 eztils-0.4.94/README.md
+-rw-r--r--   0        0        0     5076 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/__init__.py
+-rw-r--r--   0        0        0    22127 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/argparser.py
+-rw-r--r--   0        0        0     5259 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/dict_operations.py
+-rw-r--r--   0        0        0     2534 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/ezitertools.py
+-rw-r--r--   0        0        0     3376 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/ezlogging.py
+-rw-r--r--   0        0        0     2341 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/ezmath.py
+-rw-r--r--   0        0        0     6073 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/git/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/persistence/__init__.py
+-rw-r--r--   0        0        0      905 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/persistence/hf.py
+-rw-r--r--   0        0        0     4594 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/run_parallel.py
+-rw-r--r--   0        0        0     4394 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/serialization.py
+-rw-r--r--   0        0        0     2758 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/structures.py
+-rw-r--r--   0        0        0     3115 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/__init__.py
+-rw-r--r--   0        0        0    15590 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/distributions.py
+-rw-r--r--   0        0        0      307 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      368 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/math.py
+-rw-r--r--   0        0        0     3049 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/modules.py
+-rw-r--r--   0        0        0     2120 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     2617 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/tensor_creators.py
+-rw-r--r--   0        0        0     4234 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/to.py
+-rw-r--r--   0        0        0     2220 2024-03-30 15:35:27.740996 eztils-0.4.94/eztils/torch/wandb.py
+-rw-r--r--   0        0        0     4069 2024-03-30 15:35:27.740996 eztils-0.4.94/pyproject.toml
+-rw-r--r--   0        0        0    14281 1970-01-01 00:00:00.000000 eztils-0.4.94/PKG-INFO
```

### Comparing `eztils-0.4.93/LICENSE` & `eztils-0.4.94/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/README.md` & `eztils-0.4.94/README.md`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/__init__.py` & `eztils-0.4.94/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/dict_operations.py` & `eztils-0.4.94/eztils/dict_operations.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/ezitertools.py` & `eztils-0.4.94/eztils/ezitertools.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/ezlogging.py` & `eztils-0.4.94/eztils/ezlogging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/ezmath.py` & `eztils-0.4.94/eztils/ezmath.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/git/__init__.py` & `eztils-0.4.94/eztils/git/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/persistence/hf.py` & `eztils-0.4.94/eztils/persistence/hf.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/run_parallel.py` & `eztils-0.4.94/eztils/run_parallel.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/serialization.py` & `eztils-0.4.94/eztils/serialization.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/structures.py` & `eztils-0.4.94/eztils/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/torch/__init__.py` & `eztils-0.4.94/eztils/torch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import random
 from functools import partial
 
 import numpy as np
 import torch
 
-from eztils import load, save
+from eztils.serialization import load, save
 
 """
 globals
 """
 USE_GPU = False
 DTYPE = torch.float
 GPU_ID = 0
```

### Comparing `eztils-0.4.93/eztils/torch/distributions.py` & `eztils-0.4.94/eztils/torch/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from torch.distributions import Beta as TorchBeta
 from torch.distributions import Distribution as TorchDistribution
 from torch.distributions import Independent as TorchIndependent
 from torch.distributions import Normal as TorchNormal
 from torch.distributions import kl_divergence
 from torch.distributions.utils import _sum_rightmost
 
-from eztils.default.ezmath import create_stats_ordered_dict
+from eztils.ezmath import create_stats_ordered_dict
 from eztils.torch.math import atanh
 from eztils.torch.tensor_creators import ones, tensor, zeros
 from eztils.torch.to import to_np
 
 
 class Distribution(TorchDistribution):
     def sample_and_logprob(self):
```

### Comparing `eztils-0.4.93/eztils/torch/modules.py` & `eztils-0.4.94/eztils/torch/modules.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/torch/parameters.py` & `eztils-0.4.94/eztils/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/torch/tensor_creators.py` & `eztils-0.4.94/eztils/torch/tensor_creators.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/eztils/torch/to.py` & `eztils-0.4.94/eztils/torch/to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Optional, Union
 
 import functools
 
 import numpy as np
 import torch
 
-from eztils import normalize
+from eztils.ezmath import normalize
 
 
 def to_np(x):
     """
     Convert a tensor to a numpy array.
 
     :param x: Input tensor.
```

### Comparing `eztils-0.4.93/eztils/torch/wandb.py` & `eztils-0.4.94/eztils/torch/wandb.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.93/pyproject.toml` & `eztils-0.4.94/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.93"
+version = "0.4.94"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `eztils-0.4.93/PKG-INFO` & `eztils-0.4.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.93
+Version: 0.4.94
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

