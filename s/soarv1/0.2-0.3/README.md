# Comparing `tmp/soarv1-0.2.tar.gz` & `tmp/soarv1-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soarv1-0.2.tar", last modified: Fri May 10 05:24:26 2024, max compression
+gzip compressed data, was "soarv1-0.3.tar", last modified: Tue May 14 05:25:52 2024, max compression
```

## Comparing `soarv1-0.2.tar` & `soarv1-0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.357558 soarv1-0.2/
--rw-rw-rw-   0        0        0      634 2024-05-10 05:24:26.357558 soarv1-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 05:24:26.357558 soarv1-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.330557 soarv1-0.2/soar/
--rw-rw-rw-   0        0        0      126 2024-05-10 05:23:35.000000 soarv1-0.2/soar/__init__.py
--rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.2/soar/config.py
--rw-rw-rw-   0        0        0     7894 2024-04-25 01:42:25.000000 soarv1-0.2/soar/context.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.334558 soarv1-0.2/soar/datasets/
--rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.2/soar/datasets/__init__.py
--rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.2/soar/datasets/augment.py
--rw-rw-rw-   0        0        0     1288 2024-04-19 11:58:52.000000 soarv1-0.2/soar/datasets/dataloader.py
--rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.2/soar/datasets/dataset.py
--rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.2/soar/datasets/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.338557 soarv1-0.2/soar/engine/
--rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.2/soar/engine/__init__.py
--rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.2/soar/engine/exporter.py
--rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.2/soar/engine/predictor.py
--rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.2/soar/engine/trainer.py
--rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.2/soar/engine/validator.py
--rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.2/soar/main.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.341557 soarv1-0.2/soar/models/
--rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.2/soar/models/__init__.py
--rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.2/soar/models/botnet.py
--rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.2/soar/models/model.py
--rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.2/soar/models/resnet.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.352559 soarv1-0.2/soar/utils/
--rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.2/soar/utils/__init__.py
--rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.2/soar/utils/crypt.py
--rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.2/soar/utils/ema.py
--rw-rw-rw-   0        0        0     3214 2024-04-12 08:05:27.000000 soarv1-0.2/soar/utils/event.py
--rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.2/soar/utils/logger.py
--rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.2/soar/utils/loss.py
--rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.2/soar/utils/metric.py
--rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.2/soar/utils/optimizer.py
--rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.2/soar/utils/parallel.py
--rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.2/soar/utils/scheduler.py
--rw-rw-rw-   0        0        0      628 2024-04-24 15:15:31.000000 soarv1-0.2/soar/utils/storager.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.353558 soarv1-0.2/soar/weights/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.2/soar/weights/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:24:26.356558 soarv1-0.2/soarv1.egg-info/
--rw-rw-rw-   0        0        0      634 2024-05-10 05:24:26.000000 soarv1-0.2/soarv1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      820 2024-05-10 05:24:26.000000 soarv1-0.2/soarv1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:24:26.000000 soarv1-0.2/soarv1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2024-05-10 05:24:26.000000 soarv1-0.2/soarv1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-10 05:24:26.000000 soarv1-0.2/soarv1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.963667 soarv1-0.3/
+-rw-rw-rw-   0        0        0      634 2024-05-14 05:25:52.963667 soarv1-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-14 05:25:52.963667 soarv1-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.938667 soarv1-0.3/soar/
+-rw-rw-rw-   0        0        0      126 2024-05-14 05:24:44.000000 soarv1-0.3/soar/__init__.py
+-rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.3/soar/config.py
+-rw-rw-rw-   0        0        0     8008 2024-05-14 05:22:20.000000 soarv1-0.3/soar/context.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.943669 soarv1-0.3/soar/datasets/
+-rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.3/soar/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.3/soar/datasets/augment.py
+-rw-rw-rw-   0        0        0     1402 2024-05-10 06:09:42.000000 soarv1-0.3/soar/datasets/dataloader.py
+-rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.3/soar/datasets/dataset.py
+-rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.3/soar/datasets/transform.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.947667 soarv1-0.3/soar/engine/
+-rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.3/soar/engine/__init__.py
+-rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.3/soar/engine/exporter.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.3/soar/engine/predictor.py
+-rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.3/soar/engine/trainer.py
+-rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.3/soar/engine/validator.py
+-rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.3/soar/main.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.950668 soarv1-0.3/soar/models/
+-rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.3/soar/models/__init__.py
+-rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.3/soar/models/botnet.py
+-rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.3/soar/models/model.py
+-rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.3/soar/models/resnet.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.959668 soarv1-0.3/soar/utils/
+-rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.3/soar/utils/__init__.py
+-rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.3/soar/utils/crypt.py
+-rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.3/soar/utils/ema.py
+-rw-rw-rw-   0        0        0     3342 2024-05-14 05:10:54.000000 soarv1-0.3/soar/utils/event.py
+-rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.3/soar/utils/logger.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.3/soar/utils/loss.py
+-rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.3/soar/utils/metric.py
+-rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.3/soar/utils/optimizer.py
+-rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.3/soar/utils/parallel.py
+-rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.3/soar/utils/scheduler.py
+-rw-rw-rw-   0        0        0      757 2024-05-14 04:23:19.000000 soarv1-0.3/soar/utils/storager.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.960668 soarv1-0.3/soar/weights/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.3/soar/weights/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.962667 soarv1-0.3/soarv1.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/top_level.txt
```

### Comparing `soarv1-0.2/PKG-INFO` & `soarv1-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.2
+Version: 0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.2/setup.py` & `soarv1-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/config.py` & `soarv1-0.3/soar/config.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/context.py` & `soarv1-0.3/soar/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,20 @@
             valid_result = self.validator(
                 epoch=self.epoch,
                 logger=self.logger,
                 header=["", ""],
                 master=self.master_process,
                 world_size=self.world_size)
             if self.master_process:
-                self.save_model()
                 lr = self.scheduler.get_last_lr()[0]
                 self.event(epoch=self.epoch,
                            learning_rate=lr,
                            train_result=train_result,
                            valid_result=valid_result)
+                self.save_model()
         self.epoch = 0
 
     def setup_ddp(self):
         os.environ["MASTER_ADDR"] = self.addr
         os.environ["MASTER_PORT"] = self.port
         backend = 'nccl' if dist.is_nccl_available() else 'gloo'
         dist.init_process_group(backend=backend, rank=self.rank,
@@ -135,26 +135,29 @@
             event = None
         else:
             storager, event = None, None
         return storager, event
 
     def save_model(self):
         """Save model checkpoints based on various conditions."""
+        buffer = BytesIO()
+        ckpt = {
+            'epoch': self.epoch,
+            'model': de_parallel(copy.deepcopy(self.model)),
+            'ema': de_parallel(copy.deepcopy(self.ema.shadow)),
+            'optimizer': pickle.dumps(self.optimizer.state_dict()),
+            'scheduler': pickle.dumps(self.scheduler.state_dict()),
+            'config': self.config,
+            'version': __version__
+        }
+        torch.save(ckpt, buffer, pickle_module=pickle)
+        self.storager.write(f"./weights/last.pt", buffer)
+        if self.epoch == self.event.best_epoch:
+            self.storager.write(f"./weights/best.pt", buffer)
         if self.epoch % self.save_period == 0:
-            buffer = BytesIO()
-            ckpt = {
-                'epoch': self.epoch,
-                'model': de_parallel(copy.deepcopy(self.model)),
-                'ema': de_parallel(copy.deepcopy(self.ema.shadow)),
-                'optimizer': pickle.dumps(self.optimizer.state_dict()),
-                'scheduler': pickle.dumps(self.scheduler.state_dict()),
-                'config': self.config,
-                'version': __version__
-            }
-            torch.save(ckpt, buffer, pickle_module=pickle)
             model_path = f"./weights/epoch{self.epoch}.pt"
             self.storager.write(model_path, buffer)
 
     def check_storage_path(self):
         current_id = 0
         if not os.path.exists(self.save_dir):
             os.makedirs(self.save_dir)
@@ -177,15 +180,15 @@
             if csv_byte is not None:
                 csv_buffer = BytesIO(csv_byte)
                 result = pd.read_csv(csv_buffer)
                 if self.master_process:
                     self.event.reload(result)
                 self.epoch = len(result)
 
-                pt_key = f"./weights/epoch{self.epoch}.pt"
+                pt_key = f"./weights/last.pt"
                 pt_byte = self.storager.read(pt_key)
                 pt_buffer = BytesIO(pt_byte)
                 weight = torch.load(pt_buffer)
 
                 state_dict = weight["model"].state_dict()
                 self.model.load_state_dict(state_dict)
                 self.optimizer.load_state_dict(pickle.loads(weight["optimizer"]))
```

### Comparing `soarv1-0.2/soar/datasets/augment.py` & `soarv1-0.3/soar/datasets/augment.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/datasets/dataloader.py` & `soarv1-0.3/soar/datasets/dataloader.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from torch.utils.data import DistributedSampler
 
 
 class LMDBDataLoader(DataLoader):
     def __init__(self, config, dataset, mode, *args, **kwargs):
         self.mode = mode
         self.config = config[mode]
-        self.world_size = config["world_size"]
+        self.world_size = config["world_size"] if "world_size" in config.keys() else 1
         self.batch_size = self.config["batch_size"] // self.world_size
         self.num_workers = self.config["num_workers"] // self.world_size
         self.drop_last = self.config["drop_last"]
         self.sampler = LMDBDataSampler(config, dataset, mode)
         super(LMDBDataLoader, self).__init__(
             dataset=dataset,
             batch_size=self.batch_size,
@@ -18,16 +18,16 @@
             sampler=self.sampler,
             drop_last=self.drop_last,
             *args, **kwargs)
 
 
 class LMDBDataSampler(DistributedSampler):
     def __init__(self, config, dataset, mode):
-        self.rank = config["rank"]
-        self.world_size = config["world_size"]
+        self.rank = config["rank"] if "rank" in config.keys() else 0
+        self.world_size = config["world_size"] if "world_size" in config.keys() else 1
         self.config = config[mode]
         self.shuffle = self.config["shuffle"]
         super(LMDBDataSampler, self).__init__(
             dataset=dataset,
             num_replicas=self.world_size,
             rank=self.rank,
             shuffle=self.shuffle)
```

### Comparing `soarv1-0.2/soar/datasets/dataset.py` & `soarv1-0.3/soar/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/datasets/transform.py` & `soarv1-0.3/soar/datasets/transform.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/engine/exporter.py` & `soarv1-0.3/soar/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/engine/trainer.py` & `soarv1-0.3/soar/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/engine/validator.py` & `soarv1-0.3/soar/engine/validator.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/models/botnet.py` & `soarv1-0.3/soar/models/botnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/models/model.py` & `soarv1-0.3/soar/models/model.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/models/resnet.py` & `soarv1-0.3/soar/models/resnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/crypt.py` & `soarv1-0.3/soar/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/ema.py` & `soarv1-0.3/soar/utils/ema.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/event.py` & `soarv1-0.3/soar/utils/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,29 @@
             "recall/valid": [],
             "f1/train": [],
             "f1/valid": [],
             "loss/train": [],
             "loss/valid": [],
             "learning_rate": []
         }
+        self.best_epoch = 0
 
     def __call__(self, epoch, learning_rate, train_result, valid_result):
         self.metrics["epoch"].append(epoch)
         self.metrics["learning_rate"].append(learning_rate)
         self.metrics["loss/train"].append(train_result[0])
         self.metrics["loss/valid"].append(valid_result[0])
         self.metrics["precision/train"].append(train_result[1])
         self.metrics["precision/valid"].append(valid_result[1])
         self.metrics["recall/train"].append(train_result[2])
         self.metrics["recall/valid"].append(valid_result[2])
         self.metrics["f1/train"].append(train_result[3])
         self.metrics["f1/valid"].append(valid_result[3])
+        if valid_result[3] == max(self.metrics["f1/valid"]):
+            self.best_epoch = epoch
         self.write_csv()
         self.write_summary()
 
     def __del__(self):
         self.writer.close()
         self.process.terminate()
```

### Comparing `soarv1-0.2/soar/utils/logger.py` & `soarv1-0.3/soar/utils/logger.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/loss.py` & `soarv1-0.3/soar/utils/loss.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/metric.py` & `soarv1-0.3/soar/utils/metric.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/optimizer.py` & `soarv1-0.3/soar/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/parallel.py` & `soarv1-0.3/soar/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/scheduler.py` & `soarv1-0.3/soar/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.2/soar/utils/storager.py` & `soarv1-0.3/soar/utils/storager.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,13 +10,15 @@
         self.crypt = Crypt(key)
 
     def __del__(self):
         self.lmdbFile.close()
 
     def read(self, key):
         with self.lmdbFile.begin() as context:
-            buffer = context.get(self.crypt.encode(key))
+            # buffer = context.get(self.crypt.encode(key))
+            buffer = self.crypt.decode(context.get(key))
         return buffer
 
     def write(self, key, value):
         with self.lmdbFile.begin(write=True) as context:
-            context.put(self.crypt.encode(key), value.getvalue())
+            # context.put(self.crypt.encode(key), value.getvalue())
+            context.put(key, self.crypt.encode(value.getvalue()))
```

### Comparing `soarv1-0.2/soarv1.egg-info/PKG-INFO` & `soarv1-0.3/soarv1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.2
+Version: 0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.2/soarv1.egg-info/SOURCES.txt` & `soarv1-0.3/soarv1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

