# Comparing `tmp/segments-ai-1.8.0.tar.gz` & `tmp/segments-ai-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segments-ai-1.8.0.tar", last modified: Tue May  7 08:56:51 2024, max compression
+gzip compressed data, was "segments-ai-1.8.1.tar", last modified: Tue May 14 15:28:37 2024, max compression
```

## Comparing `segments-ai-1.8.0.tar` & `segments-ai-1.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.379060 segments-ai-1.8.0/
--rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.8.0/LICENSE.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.8.0/MANIFEST.in
--rw-rw-r--   0 bert      (1000) bert      (1000)     1179 2024-05-07 08:56:51.379060 segments-ai-1.8.0/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.8.0/README.md
--rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.8.0/pyproject.toml
--rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.8.0/requirements.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.8.0/requirements_dev.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.8.0/requirements_docs.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-05-07 08:56:51.379060 segments-ai-1.8.0/setup.cfg
--rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-05-07 08:55:36.000000 segments-ai-1.8.0/setup.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.371060 segments-ai-1.8.0/src/
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.375060 segments-ai-1.8.0/src/segments/
--rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.8.0/src/segments/__init__.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    87827 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/client.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.375060 segments-ai-1.8.0/src/segments/data/
--rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.8.0/src/segments/data/dataset_card_template.md
--rw-rw-r--   0 bert      (1000) bert      (1000)    14575 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.8.0/src/segments/exceptions.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    30466 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/export.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.8.0/src/segments/huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.8.0/src/segments/py.typed
--rw-rw-r--   0 bert      (1000) bert      (1000)    23071 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/typing.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    38454 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/utils.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.375060 segments-ai-1.8.0/src/segments_ai.egg-info/
--rw-r--r--   0 bert      (1000) bert      (1000)     1179 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/requires.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/top_level.txt
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.379060 segments-ai-1.8.0/tests/
--rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.8.0/tests/test_client.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.8.0/tests/test_dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.8.0/tests/test_huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.8.0/tests/test_random.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.8.0/tests/test_utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-14 15:28:37.108997 segments-ai-1.8.1/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.8.1/LICENSE.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.8.1/MANIFEST.in
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1179 2024-05-14 15:28:37.108997 segments-ai-1.8.1/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.8.1/README.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.8.1/pyproject.toml
+-rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.8.1/requirements.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.8.1/requirements_dev.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.8.1/requirements_docs.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-05-14 15:28:37.108997 segments-ai-1.8.1/setup.cfg
+-rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-05-14 15:27:42.000000 segments-ai-1.8.1/setup.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-14 15:28:37.104997 segments-ai-1.8.1/src/
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-14 15:28:37.108997 segments-ai-1.8.1/src/segments/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.8.1/src/segments/__init__.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    87827 2024-05-07 08:55:20.000000 segments-ai-1.8.1/src/segments/client.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-14 15:28:37.108997 segments-ai-1.8.1/src/segments/data/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.8.1/src/segments/data/dataset_card_template.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)    14575 2024-05-07 08:55:20.000000 segments-ai-1.8.1/src/segments/dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.8.1/src/segments/exceptions.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    30466 2024-05-07 08:55:20.000000 segments-ai-1.8.1/src/segments/export.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.8.1/src/segments/huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.8.1/src/segments/py.typed
+-rw-rw-r--   0 bert      (1000) bert      (1000)    22953 2024-05-14 15:26:53.000000 segments-ai-1.8.1/src/segments/typing.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    38454 2024-05-07 08:55:20.000000 segments-ai-1.8.1/src/segments/utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-14 15:28:37.108997 segments-ai-1.8.1/src/segments_ai.egg-info/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1179 2024-05-14 15:28:36.000000 segments-ai-1.8.1/src/segments_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-05-14 15:28:37.000000 segments-ai-1.8.1/src/segments_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-05-14 15:28:36.000000 segments-ai-1.8.1/src/segments_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-05-14 15:28:37.000000 segments-ai-1.8.1/src/segments_ai.egg-info/requires.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-05-14 15:28:37.000000 segments-ai-1.8.1/src/segments_ai.egg-info/top_level.txt
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-14 15:28:37.108997 segments-ai-1.8.1/tests/
+-rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.8.1/tests/test_client.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.8.1/tests/test_dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.8.1/tests/test_huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.8.1/tests/test_random.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.8.1/tests/test_utils.py
```

### Comparing `segments-ai-1.8.0/LICENSE.txt` & `segments-ai-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/PKG-INFO` & `segments-ai-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.8.0
+Version: 1.8.1
 Summary: UNKNOWN
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.8.0.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.8.1.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `segments-ai-1.8.0/README.md` & `segments-ai-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/pyproject.toml` & `segments-ai-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/setup.py` & `segments-ai-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from typing import List
 
 
 #############
 # Constants #
 #############
-MAJOR, MINOR, PATCH = 1, 8, 0
+MAJOR, MINOR, PATCH = 1, 8, 1
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 
 ####################
 # Helper functions #
 ####################
 # https://github.com/allenai/python-package-template
```

### Comparing `segments-ai-1.8.0/src/segments/client.py` & `segments-ai-1.8.1/src/segments/client.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/src/segments/dataset.py` & `segments-ai-1.8.1/src/segments/dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/src/segments/exceptions.py` & `segments-ai-1.8.1/src/segments/exceptions.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/src/segments/export.py` & `segments-ai-1.8.1/src/segments/export.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/src/segments/huggingface.py` & `segments-ai-1.8.1/src/segments/huggingface.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/src/segments/typing.py` & `segments-ai-1.8.1/src/segments/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,15 @@
     frames: List[ImageVectorFrame]
     format_version: Optional[FormatVersion] = None
 
 
 # Point cloud segmentation
 class PointcloudSegmentationLabelAttributes(BaseModel):
     annotations: List[Annotation]
-    point_annotations: Optional[List[int]] = None
+    point_annotations: List[int]
     format_version: Optional[FormatVersion] = None
 
 
 class XYZ(BaseModel):
     x: float
     y: float
     z: float
@@ -415,17 +415,15 @@
     track_id: int
     is_keyframe: bool = False
     attributes: Optional[ObjectAttributes] = None
 
 
 class PointcloudSegmentationFrame(PointcloudSegmentationLabelAttributes):
     annotations: List[PointcloudSequenceSegmentationAnnotation]
-    point_annotations: Optional[List[int]] = None
     timestamp: Optional[Timestamp] = None
-    format_version: Optional[FormatVersion] = None
 
 
 class PointcloudSequenceSegmentationLabelAttributes(BaseModel):
     frames: List[PointcloudSegmentationFrame]
     format_version: Optional[FormatVersion] = None
```

### Comparing `segments-ai-1.8.0/src/segments/utils.py` & `segments-ai-1.8.1/src/segments/utils.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/src/segments_ai.egg-info/PKG-INFO` & `segments-ai-1.8.1/src/segments_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.8.0
+Version: 1.8.1
 Summary: UNKNOWN
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.8.0.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.8.1.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `segments-ai-1.8.0/src/segments_ai.egg-info/SOURCES.txt` & `segments-ai-1.8.1/src/segments_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/tests/test_client.py` & `segments-ai-1.8.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/tests/test_dataset.py` & `segments-ai-1.8.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.8.0/tests/test_utils.py` & `segments-ai-1.8.1/tests/test_utils.py`

 * *Files identical despite different names*

