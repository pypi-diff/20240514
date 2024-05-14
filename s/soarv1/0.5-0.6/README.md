# Comparing `tmp/soarv1-0.5.tar.gz` & `tmp/soarv1-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soarv1-0.5.tar", last modified: Tue May 14 09:47:25 2024, max compression
+gzip compressed data, was "soarv1-0.6.tar", last modified: Tue May 14 10:49:47 2024, max compression
```

## Comparing `soarv1-0.5.tar` & `soarv1-0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.236433 soarv1-0.5/
--rw-rw-rw-   0        0        0      634 2024-05-14 09:47:25.236433 soarv1-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-14 09:47:25.237432 soarv1-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.214434 soarv1-0.5/soar/
--rw-rw-rw-   0        0        0      126 2024-05-14 09:47:00.000000 soarv1-0.5/soar/__init__.py
--rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.5/soar/config.py
--rw-rw-rw-   0        0        0     8008 2024-05-14 07:19:56.000000 soarv1-0.5/soar/context.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.217433 soarv1-0.5/soar/datasets/
--rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.5/soar/datasets/__init__.py
--rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.5/soar/datasets/augment.py
--rw-rw-rw-   0        0        0     1402 2024-05-10 06:09:42.000000 soarv1-0.5/soar/datasets/dataloader.py
--rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.5/soar/datasets/dataset.py
--rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.5/soar/datasets/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.220432 soarv1-0.5/soar/engine/
--rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.5/soar/engine/__init__.py
--rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.5/soar/engine/exporter.py
--rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.5/soar/engine/predictor.py
--rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.5/soar/engine/trainer.py
--rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.5/soar/engine/validator.py
--rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.5/soar/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.222434 soarv1-0.5/soar/models/
--rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.5/soar/models/__init__.py
--rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.5/soar/models/botnet.py
--rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.5/soar/models/model.py
--rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.5/soar/models/resnet.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.231435 soarv1-0.5/soar/utils/
--rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.5/soar/utils/__init__.py
--rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.5/soar/utils/crypt.py
--rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.5/soar/utils/ema.py
--rw-rw-rw-   0        0        0     3534 2024-05-14 09:45:06.000000 soarv1-0.5/soar/utils/event.py
--rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.5/soar/utils/logger.py
--rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.5/soar/utils/loss.py
--rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.5/soar/utils/metric.py
--rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.5/soar/utils/optimizer.py
--rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.5/soar/utils/parallel.py
--rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.5/soar/utils/scheduler.py
--rw-rw-rw-   0        0        0     1443 2024-05-14 07:57:35.000000 soarv1-0.5/soar/utils/storager.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.232434 soarv1-0.5/soar/weights/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.5/soar/weights/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:47:25.235434 soarv1-0.5/soarv1.egg-info/
--rw-rw-rw-   0        0        0      634 2024-05-14 09:47:25.000000 soarv1-0.5/soarv1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      820 2024-05-14 09:47:25.000000 soarv1-0.5/soarv1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 09:47:25.000000 soarv1-0.5/soarv1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2024-05-14 09:47:25.000000 soarv1-0.5/soarv1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-14 09:47:25.000000 soarv1-0.5/soarv1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.526960 soarv1-0.6/
+-rw-rw-rw-   0        0        0      634 2024-05-14 10:49:47.525959 soarv1-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-14 10:49:47.526960 soarv1-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.504958 soarv1-0.6/soar/
+-rw-rw-rw-   0        0        0      126 2024-05-14 10:49:20.000000 soarv1-0.6/soar/__init__.py
+-rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.6/soar/config.py
+-rw-rw-rw-   0        0        0     8057 2024-05-14 10:49:07.000000 soarv1-0.6/soar/context.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.508960 soarv1-0.6/soar/datasets/
+-rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.6/soar/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.6/soar/datasets/augment.py
+-rw-rw-rw-   0        0        0     1402 2024-05-10 06:09:42.000000 soarv1-0.6/soar/datasets/dataloader.py
+-rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.6/soar/datasets/dataset.py
+-rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.6/soar/datasets/transform.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.511958 soarv1-0.6/soar/engine/
+-rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.6/soar/engine/__init__.py
+-rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.6/soar/engine/exporter.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.6/soar/engine/predictor.py
+-rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.6/soar/engine/trainer.py
+-rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.6/soar/engine/validator.py
+-rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.6/soar/main.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.513958 soarv1-0.6/soar/models/
+-rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.6/soar/models/__init__.py
+-rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.6/soar/models/botnet.py
+-rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.6/soar/models/model.py
+-rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.6/soar/models/resnet.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.520958 soarv1-0.6/soar/utils/
+-rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.6/soar/utils/__init__.py
+-rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.6/soar/utils/crypt.py
+-rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.6/soar/utils/ema.py
+-rw-rw-rw-   0        0        0     3534 2024-05-14 09:45:06.000000 soarv1-0.6/soar/utils/event.py
+-rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.6/soar/utils/logger.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.6/soar/utils/loss.py
+-rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.6/soar/utils/metric.py
+-rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.6/soar/utils/optimizer.py
+-rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.6/soar/utils/parallel.py
+-rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.6/soar/utils/scheduler.py
+-rw-rw-rw-   0        0        0     1443 2024-05-14 07:57:35.000000 soarv1-0.6/soar/utils/storager.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.521961 soarv1-0.6/soar/weights/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.6/soar/weights/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:49:47.525959 soarv1-0.6/soarv1.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-05-14 10:49:47.000000 soarv1-0.6/soarv1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2024-05-14 10:49:47.000000 soarv1-0.6/soarv1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 10:49:47.000000 soarv1-0.6/soarv1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2024-05-14 10:49:47.000000 soarv1-0.6/soarv1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-14 10:49:47.000000 soarv1-0.6/soarv1.egg-info/top_level.txt
```

### Comparing `soarv1-0.5/PKG-INFO` & `soarv1-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.5
+Version: 0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.5/setup.py` & `soarv1-0.6/setup.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/config.py` & `soarv1-0.6/soar/config.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/context.py` & `soarv1-0.6/soar/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,13 +184,14 @@
                     self.event.reload(result)
                 self.epoch = len(result)
 
                 pt_key = f"./weights/last.pt"
                 pt_byte = self.storager.read(pt_key)
                 pt_buffer = BytesIO(pt_byte)
                 weight = torch.load(pt_buffer)
+                weight = weight.to(self.device)
 
                 state_dict = weight["model"].state_dict()
                 self.model.load_state_dict(state_dict)
                 self.optimizer.load_state_dict(pickle.loads(weight["optimizer"]))
                 self.scheduler.load_state_dict(pickle.loads(weight["scheduler"]))
                 self.ema.shadow = weight["ema"].copy()
```

### Comparing `soarv1-0.5/soar/datasets/augment.py` & `soarv1-0.6/soar/datasets/augment.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/datasets/dataloader.py` & `soarv1-0.6/soar/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/datasets/dataset.py` & `soarv1-0.6/soar/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/datasets/transform.py` & `soarv1-0.6/soar/datasets/transform.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/engine/exporter.py` & `soarv1-0.6/soar/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/engine/trainer.py` & `soarv1-0.6/soar/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/engine/validator.py` & `soarv1-0.6/soar/engine/validator.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/models/botnet.py` & `soarv1-0.6/soar/models/botnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/models/model.py` & `soarv1-0.6/soar/models/model.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/models/resnet.py` & `soarv1-0.6/soar/models/resnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/crypt.py` & `soarv1-0.6/soar/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/ema.py` & `soarv1-0.6/soar/utils/ema.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/event.py` & `soarv1-0.6/soar/utils/event.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/logger.py` & `soarv1-0.6/soar/utils/logger.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/loss.py` & `soarv1-0.6/soar/utils/loss.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/metric.py` & `soarv1-0.6/soar/utils/metric.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/optimizer.py` & `soarv1-0.6/soar/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/parallel.py` & `soarv1-0.6/soar/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/scheduler.py` & `soarv1-0.6/soar/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soar/utils/storager.py` & `soarv1-0.6/soar/utils/storager.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.5/soarv1.egg-info/PKG-INFO` & `soarv1-0.6/soarv1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.5
+Version: 0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.5/soarv1.egg-info/SOURCES.txt` & `soarv1-0.6/soarv1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

