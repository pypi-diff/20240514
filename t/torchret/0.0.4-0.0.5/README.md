# Comparing `tmp/torchret-0.0.4.tar.gz` & `tmp/torchret-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchret-0.0.4.tar", last modified: Tue May 14 17:33:15 2024, max compression
+gzip compressed data, was "torchret-0.0.5.tar", last modified: Tue May 14 18:03:38 2024, max compression
```

## Comparing `torchret-0.0.4.tar` & `torchret-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 17:33:15.688963 torchret-0.0.4/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 17:33:15.688808 torchret-0.0.4/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-14 17:33:15.689021 torchret-0.0.4/setup.cfg
--rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-14 17:33:14.000000 torchret-0.0.4/setup.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 17:33:15.687447 torchret-0.0.4/torchret/
--rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.0.4/torchret/__init__.py
--rw-r--r--   0 parth      (501) staff       (20)    13800 2024-05-14 17:24:11.000000 torchret-0.0.4/torchret/model.py
--rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.0.4/torchret/utils.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 17:33:15.688363 torchret-0.0.4/torchret.egg-info/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/SOURCES.txt
--rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/dependency_links.txt
--rw-r--r--   0 parth      (501) staff       (20)       13 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/requires.txt
--rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/top_level.txt
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 18:03:38.941500 torchret-0.0.5/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 18:03:38.941336 torchret-0.0.5/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-14 18:03:38.941579 torchret-0.0.5/setup.cfg
+-rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-14 18:02:11.000000 torchret-0.0.5/setup.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 18:03:38.940129 torchret-0.0.5/torchret/
+-rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.0.5/torchret/__init__.py
+-rw-r--r--   0 parth      (501) staff       (20)    13592 2024-05-14 17:59:57.000000 torchret-0.0.5/torchret/model.py
+-rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.0.5/torchret/utils.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 18:03:38.941102 torchret-0.0.5/torchret.egg-info/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 18:03:38.000000 torchret-0.0.5/torchret.egg-info/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-14 18:03:38.000000 torchret-0.0.5/torchret.egg-info/SOURCES.txt
+-rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-14 18:03:38.000000 torchret-0.0.5/torchret.egg-info/dependency_links.txt
+-rw-r--r--   0 parth      (501) staff       (20)       13 2024-05-14 18:03:38.000000 torchret-0.0.5/torchret.egg-info/requires.txt
+-rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-14 18:03:38.000000 torchret-0.0.5/torchret.egg-info/top_level.txt
```

### Comparing `torchret-0.0.4/setup.py` & `torchret-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().splitlines()
 
 
 setup(
     name="torchret",
     description="",
     long_description="",
-    version = '0.0.4',
+    version = '0.0.5',
     long_description_content_type="text/markdown",
     author="Parth Dhameliya",
     url="https://github.com/parthdhameliya7",
     license="Apache License 2.0",
     packages=find_packages(),
     include_package_data=True,
     platforms=["linux", "unix"],
```

### Comparing `torchret-0.0.4/torchret/model.py` & `torchret-0.0.5/torchret/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,14 @@
     
     def fetch_optimizer(self, *args, **kwargs):
         """
         Method to fetch the optimizer for training.
         """
         return 
     
-    def fetch_scheduler(self, *args, **kwargs):
-        """
-        Method to fetch the scheduler for adjusting learning rate during training.
-        """
-        return 
-    
     def get_mixup(self, *args, **kwargs):
         """
         Method to apply mixup augmentation to the data.
         """
         return 
     
     def get_cutmix(self, *args, **kwargs):
@@ -325,16 +319,15 @@
             )
         if next(self.parameters()).device != self.device:
             self.to(self.device)
         
         if self.fp16:
             self.scaler = torch.cuda.amp.GradScaler()
 
-        self.optimizer = self.fetch_optimizer()
-        self.scheduler = self.fetch_scheduler()
+        self.optimizer, self.scheduler = self.fetch_optimizer()
         self.current_epoch += 1
         self.best_loss = 1000
         self.best_score = 0.0
 
 
         for _ in range(epochs):
             self.train_loss, self.train_metrics = self.train_one_epoch(self.trainloader)
```

### Comparing `torchret-0.0.4/torchret/utils.py` & `torchret-0.0.5/torchret/utils.py`

 * *Files identical despite different names*

