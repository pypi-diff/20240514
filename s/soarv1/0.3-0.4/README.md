# Comparing `tmp/soarv1-0.3.tar.gz` & `tmp/soarv1-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soarv1-0.3.tar", last modified: Tue May 14 05:25:52 2024, max compression
+gzip compressed data, was "soarv1-0.4.tar", last modified: Tue May 14 09:07:39 2024, max compression
```

## Comparing `soarv1-0.3.tar` & `soarv1-0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.963667 soarv1-0.3/
--rw-rw-rw-   0        0        0      634 2024-05-14 05:25:52.963667 soarv1-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-14 05:25:52.963667 soarv1-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.938667 soarv1-0.3/soar/
--rw-rw-rw-   0        0        0      126 2024-05-14 05:24:44.000000 soarv1-0.3/soar/__init__.py
--rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.3/soar/config.py
--rw-rw-rw-   0        0        0     8008 2024-05-14 05:22:20.000000 soarv1-0.3/soar/context.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.943669 soarv1-0.3/soar/datasets/
--rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.3/soar/datasets/__init__.py
--rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.3/soar/datasets/augment.py
--rw-rw-rw-   0        0        0     1402 2024-05-10 06:09:42.000000 soarv1-0.3/soar/datasets/dataloader.py
--rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.3/soar/datasets/dataset.py
--rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.3/soar/datasets/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.947667 soarv1-0.3/soar/engine/
--rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.3/soar/engine/__init__.py
--rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.3/soar/engine/exporter.py
--rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.3/soar/engine/predictor.py
--rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.3/soar/engine/trainer.py
--rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.3/soar/engine/validator.py
--rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.3/soar/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.950668 soarv1-0.3/soar/models/
--rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.3/soar/models/__init__.py
--rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.3/soar/models/botnet.py
--rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.3/soar/models/model.py
--rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.3/soar/models/resnet.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.959668 soarv1-0.3/soar/utils/
--rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.3/soar/utils/__init__.py
--rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.3/soar/utils/crypt.py
--rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.3/soar/utils/ema.py
--rw-rw-rw-   0        0        0     3342 2024-05-14 05:10:54.000000 soarv1-0.3/soar/utils/event.py
--rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.3/soar/utils/logger.py
--rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.3/soar/utils/loss.py
--rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.3/soar/utils/metric.py
--rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.3/soar/utils/optimizer.py
--rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.3/soar/utils/parallel.py
--rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.3/soar/utils/scheduler.py
--rw-rw-rw-   0        0        0      757 2024-05-14 04:23:19.000000 soarv1-0.3/soar/utils/storager.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.960668 soarv1-0.3/soar/weights/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.3/soar/weights/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 05:25:52.962667 soarv1-0.3/soarv1.egg-info/
--rw-rw-rw-   0        0        0      634 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      820 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-14 05:25:52.000000 soarv1-0.3/soarv1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.395599 soarv1-0.4/
+-rw-rw-rw-   0        0        0      634 2024-05-14 09:07:39.395599 soarv1-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-14 09:07:39.395599 soarv1-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.373598 soarv1-0.4/soar/
+-rw-rw-rw-   0        0        0      126 2024-05-14 09:06:41.000000 soarv1-0.4/soar/__init__.py
+-rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.4/soar/config.py
+-rw-rw-rw-   0        0        0     8008 2024-05-14 07:19:56.000000 soarv1-0.4/soar/context.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.377600 soarv1-0.4/soar/datasets/
+-rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.4/soar/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.4/soar/datasets/augment.py
+-rw-rw-rw-   0        0        0     1402 2024-05-10 06:09:42.000000 soarv1-0.4/soar/datasets/dataloader.py
+-rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.4/soar/datasets/dataset.py
+-rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.4/soar/datasets/transform.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.380598 soarv1-0.4/soar/engine/
+-rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.4/soar/engine/__init__.py
+-rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.4/soar/engine/exporter.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.4/soar/engine/predictor.py
+-rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.4/soar/engine/trainer.py
+-rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.4/soar/engine/validator.py
+-rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.4/soar/main.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.382598 soarv1-0.4/soar/models/
+-rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.4/soar/models/__init__.py
+-rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.4/soar/models/botnet.py
+-rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.4/soar/models/model.py
+-rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.4/soar/models/resnet.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.390598 soarv1-0.4/soar/utils/
+-rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.4/soar/utils/__init__.py
+-rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.4/soar/utils/crypt.py
+-rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.4/soar/utils/ema.py
+-rw-rw-rw-   0        0        0     3533 2024-05-14 07:17:00.000000 soarv1-0.4/soar/utils/event.py
+-rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.4/soar/utils/logger.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.4/soar/utils/loss.py
+-rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.4/soar/utils/metric.py
+-rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.4/soar/utils/optimizer.py
+-rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.4/soar/utils/parallel.py
+-rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.4/soar/utils/scheduler.py
+-rw-rw-rw-   0        0        0     1443 2024-05-14 07:57:35.000000 soarv1-0.4/soar/utils/storager.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.390598 soarv1-0.4/soar/weights/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.4/soar/weights/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:07:39.394599 soarv1-0.4/soarv1.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-05-14 09:07:39.000000 soarv1-0.4/soarv1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2024-05-14 09:07:39.000000 soarv1-0.4/soarv1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 09:07:39.000000 soarv1-0.4/soarv1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2024-05-14 09:07:39.000000 soarv1-0.4/soarv1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-14 09:07:39.000000 soarv1-0.4/soarv1.egg-info/top_level.txt
```

### Comparing `soarv1-0.3/PKG-INFO` & `soarv1-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.3
+Version: 0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.3/setup.py` & `soarv1-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/config.py` & `soarv1-0.4/soar/config.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/context.py` & `soarv1-0.4/soar/context.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/datasets/augment.py` & `soarv1-0.4/soar/datasets/augment.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/datasets/dataloader.py` & `soarv1-0.4/soar/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/datasets/dataset.py` & `soarv1-0.4/soar/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/datasets/transform.py` & `soarv1-0.4/soar/datasets/transform.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/engine/exporter.py` & `soarv1-0.4/soar/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/engine/trainer.py` & `soarv1-0.4/soar/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/engine/validator.py` & `soarv1-0.4/soar/engine/validator.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/models/botnet.py` & `soarv1-0.4/soar/models/botnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/models/model.py` & `soarv1-0.4/soar/models/model.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/models/resnet.py` & `soarv1-0.4/soar/models/resnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/crypt.py` & `soarv1-0.4/soar/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/ema.py` & `soarv1-0.4/soar/utils/ema.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/event.py` & `soarv1-0.4/soar/utils/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,14 +57,19 @@
         return process
 
     def reload(self, result):
         metrics = result.to_dict()
         for key, value in metrics.items():
             self.metrics[key] = list(value.values())
 
+        epochs = metrics.pop("epoch")
+        for epoch in epochs:
+            for name, metric in metrics.items():
+                self.writer.add_scalar(name, metric[epoch-1], epoch)
+
         # concat tensorboard output
         # event_list = []
         # for event_name in os.listdir(self.storager.save_path):
         #     if event_name.startswith("events"):
         #         event_list.append(os.path.join(self.storager.save_path, event_name))
         # buffer = BytesIO()
         # for event_path in event_list:
```

### Comparing `soarv1-0.3/soar/utils/logger.py` & `soarv1-0.4/soar/utils/logger.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/loss.py` & `soarv1-0.4/soar/utils/loss.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/metric.py` & `soarv1-0.4/soar/utils/metric.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/optimizer.py` & `soarv1-0.4/soar/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/parallel.py` & `soarv1-0.4/soar/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soar/utils/scheduler.py` & `soarv1-0.4/soar/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.3/soarv1.egg-info/PKG-INFO` & `soarv1-0.4/soarv1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.3
+Version: 0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.3/soarv1.egg-info/SOURCES.txt` & `soarv1-0.4/soarv1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

