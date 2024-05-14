# Comparing `tmp/torchret-0.0.3.tar.gz` & `tmp/torchret-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchret-0.0.3.tar", last modified: Tue May 14 04:01:58 2024, max compression
+gzip compressed data, was "torchret-0.0.4.tar", last modified: Tue May 14 17:33:15 2024, max compression
```

## Comparing `torchret-0.0.3.tar` & `torchret-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 04:01:58.589247 torchret-0.0.3/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 04:01:58.589092 torchret-0.0.3/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-14 04:01:58.589310 torchret-0.0.3/setup.cfg
--rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-14 03:59:43.000000 torchret-0.0.3/setup.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 04:01:58.587944 torchret-0.0.3/torchret/
--rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.0.3/torchret/__init__.py
--rw-r--r--   0 parth      (501) staff       (20)    13676 2024-05-14 03:46:01.000000 torchret-0.0.3/torchret/model.py
--rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.0.3/torchret/utils.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 04:01:58.588858 torchret-0.0.3/torchret.egg-info/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 04:01:58.000000 torchret-0.0.3/torchret.egg-info/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-14 04:01:58.000000 torchret-0.0.3/torchret.egg-info/SOURCES.txt
--rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-14 04:01:58.000000 torchret-0.0.3/torchret.egg-info/dependency_links.txt
--rw-r--r--   0 parth      (501) staff       (20)      142 2024-05-14 04:01:58.000000 torchret-0.0.3/torchret.egg-info/requires.txt
--rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-14 04:01:58.000000 torchret-0.0.3/torchret.egg-info/top_level.txt
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 17:33:15.688963 torchret-0.0.4/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 17:33:15.688808 torchret-0.0.4/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-14 17:33:15.689021 torchret-0.0.4/setup.cfg
+-rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-14 17:33:14.000000 torchret-0.0.4/setup.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 17:33:15.687447 torchret-0.0.4/torchret/
+-rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.0.4/torchret/__init__.py
+-rw-r--r--   0 parth      (501) staff       (20)    13800 2024-05-14 17:24:11.000000 torchret-0.0.4/torchret/model.py
+-rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.0.4/torchret/utils.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 17:33:15.688363 torchret-0.0.4/torchret.egg-info/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/SOURCES.txt
+-rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/dependency_links.txt
+-rw-r--r--   0 parth      (501) staff       (20)       13 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/requires.txt
+-rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-14 17:33:15.000000 torchret-0.0.4/torchret.egg-info/top_level.txt
```

### Comparing `torchret-0.0.3/setup.py` & `torchret-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().splitlines()
 
 
 setup(
     name="torchret",
     description="",
     long_description="",
-    version = '0.0.3',
+    version = '0.0.4',
     long_description_content_type="text/markdown",
     author="Parth Dhameliya",
     url="https://github.com/parthdhameliya7",
     license="Apache License 2.0",
     packages=find_packages(),
     include_package_data=True,
     platforms=["linux", "unix"],
```

### Comparing `torchret-0.0.3/torchret/model.py` & `torchret-0.0.4/torchret/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,34 +328,35 @@
         
         if self.fp16:
             self.scaler = torch.cuda.amp.GradScaler()
 
         self.optimizer = self.fetch_optimizer()
         self.scheduler = self.fetch_scheduler()
         self.current_epoch += 1
-        self.best_loss = np.Inf
+        self.best_loss = 1000
         self.best_score = 0.0
 
 
         for _ in range(epochs):
             self.train_loss, self.train_metrics = self.train_one_epoch(self.trainloader)
             if self.validloader is not None:
                 self.valid_loss, self.valid_metrics = self.valid_one_epoch(self.validloader)
             self.current_epoch += 1
 
             if self.save_best_model is not None:
                 if self.save_best_model == 'on_eval_loss':
                     if self.valid_loss < self.best_loss:
                         self.save(f'{self.metric_path}_{self.model_path}', self.weights_only)
                         print(f'Model was saved based {self.save_best_model} with {self.valid_loss} loss')
+                        self.best_loss = self.valid_loss
                 elif self.save_best_model == 'on_eval_metric':
                     if self.save_on_metric in self.train_metrics:
                         if self.valid_metrics[self.save_on_metric] > self.best_score:
                             self.save(f'{self.metric_path}_{self.model_path}', self.weights_only)
                             print(f'Model was saved based {self.save_best_model} with {self.valid_metrics[self.save_on_metric]} {self.save_on_metric}')
-                
+                            self.best_score = self.valid_metrics[self.save_on_metric]
             if self.save_model_at_every_epoch is not None:
                 self.save(self.model_path, self.weights_only)
```

### Comparing `torchret-0.0.3/torchret/utils.py` & `torchret-0.0.4/torchret/utils.py`

 * *Files identical despite different names*

