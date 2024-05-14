# Comparing `tmp/moovs_business-0.0.0.tar.gz` & `tmp/moovs_business-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moovs_business-0.0.0.tar", last modified: Sat May 11 17:57:34 2024, max compression
+gzip compressed data, was "moovs_business-0.0.1.tar", last modified: Tue May 14 14:51:51 2024, max compression
```

## Comparing `moovs_business-0.0.0.tar` & `moovs_business-0.0.1.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-11 17:57:34.396043 moovs_business-0.0.0/
--rw-rw-r--   0 rreis     (1003) rreis     (1003)     2595 2024-05-11 17:57:34.396043 moovs_business-0.0.0/PKG-INFO
--rw-rw-r--   0 rreis     (1003) rreis     (1003)     2131 2024-05-11 17:39:38.000000 moovs_business-0.0.0/README.md
-drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-11 17:57:34.396043 moovs_business-0.0.0/moovs_business/
--rw-rw-r--   0 rreis     (1003) rreis     (1003)      206 2024-05-11 17:40:17.000000 moovs_business-0.0.0/moovs_business/__init__.py
--rw-rw-r--   0 rreis     (1003) rreis     (1003)      314 2024-05-11 17:32:07.000000 moovs_business-0.0.0/moovs_business/constants.py
-drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-11 17:57:34.396043 moovs_business-0.0.0/moovs_business/flows/
--rw-rw-r--   0 rreis     (1003) rreis     (1003)       57 2024-05-11 17:32:07.000000 moovs_business-0.0.0/moovs_business/flows/__init__.py
--rw-rw-r--   0 rreis     (1003) rreis     (1003)     4475 2024-05-11 17:42:10.000000 moovs_business-0.0.0/moovs_business/flows/detection.py
--rw-rw-r--   0 rreis     (1003) rreis     (1003)     6583 2024-05-11 17:42:10.000000 moovs_business-0.0.0/moovs_business/flows/human_pose.py
--rw-rw-r--   0 rreis     (1003) rreis     (1003)     4148 2024-05-11 17:42:10.000000 moovs_business-0.0.0/moovs_business/flows/tracking.py
--rw-rw-r--   0 rreis     (1003) rreis     (1003)     4127 2024-05-11 17:40:17.000000 moovs_business-0.0.0/moovs_business/structs.py
-drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-11 17:57:34.396043 moovs_business-0.0.0/moovs_business/tracking/
--rw-rw-r--   0 rreis     (1003) rreis     (1003)        0 2024-05-11 17:32:07.000000 moovs_business-0.0.0/moovs_business/tracking/__init__.py
--rwxrwxr-x   0 rreis     (1003) rreis     (1003)     2845 2024-05-11 17:32:07.000000 moovs_business-0.0.0/moovs_business/tracking/iou_matching.py
--rwxrwxr-x   0 rreis     (1003) rreis     (1003)     8119 2024-05-11 17:32:07.000000 moovs_business-0.0.0/moovs_business/tracking/kalman_filter.py
--rwxrwxr-x   0 rreis     (1003) rreis     (1003)     9033 2024-05-11 17:32:07.000000 moovs_business-0.0.0/moovs_business/tracking/linear_assignment.py
--rw-rw-r--   0 rreis     (1003) rreis     (1003)     4870 2024-05-11 17:32:07.000000 moovs_business-0.0.0/moovs_business/tracking/moving_average.py
-drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-11 17:57:34.396043 moovs_business-0.0.0/moovs_business.egg-info/
--rw-r--r--   0 rreis     (1003) rreis     (1003)     2595 2024-05-11 17:57:34.000000 moovs_business-0.0.0/moovs_business.egg-info/PKG-INFO
--rw-rw-r--   0 rreis     (1003) rreis     (1003)      627 2024-05-11 17:57:34.000000 moovs_business-0.0.0/moovs_business.egg-info/SOURCES.txt
--rw-rw-r--   0 rreis     (1003) rreis     (1003)        1 2024-05-11 17:57:34.000000 moovs_business-0.0.0/moovs_business.egg-info/dependency_links.txt
--rw-rw-r--   0 rreis     (1003) rreis     (1003)       77 2024-05-11 17:57:34.000000 moovs_business-0.0.0/moovs_business.egg-info/requires.txt
--rw-rw-r--   0 rreis     (1003) rreis     (1003)       15 2024-05-11 17:57:34.000000 moovs_business-0.0.0/moovs_business.egg-info/top_level.txt
--rw-rw-r--   0 rreis     (1003) rreis     (1003)       38 2024-05-11 17:57:34.396043 moovs_business-0.0.0/setup.cfg
--rw-rw-r--   0 rreis     (1003) rreis     (1003)      818 2024-05-11 17:35:00.000000 moovs_business-0.0.0/setup.py
+drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-14 14:51:51.151856 moovs_business-0.0.1/
+-rw-r--r--   0 rreis     (1003) rreis     (1003)     2777 2024-05-14 14:51:51.151856 moovs_business-0.0.1/PKG-INFO
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     2131 2024-05-11 17:39:38.000000 moovs_business-0.0.1/README.md
+drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-14 14:51:51.147856 moovs_business-0.0.1/moovs_business/
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)      206 2024-05-11 17:40:17.000000 moovs_business-0.0.1/moovs_business/__init__.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)      314 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/constants.py
+drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-14 14:51:51.147856 moovs_business-0.0.1/moovs_business/flows/
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)       57 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/flows/__init__.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     4475 2024-05-11 17:42:10.000000 moovs_business-0.0.1/moovs_business/flows/detection.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     6583 2024-05-11 17:42:10.000000 moovs_business-0.0.1/moovs_business/flows/human_pose.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     4148 2024-05-11 17:42:10.000000 moovs_business-0.0.1/moovs_business/flows/tracking.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     4127 2024-05-11 17:40:17.000000 moovs_business-0.0.1/moovs_business/structs.py
+drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-14 14:51:51.147856 moovs_business-0.0.1/moovs_business/tracking/
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)        0 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/tracking/__init__.py
+-rwxrwxr-x   0 rreis     (1003) rreis     (1003)     2845 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/tracking/iou_matching.py
+-rwxrwxr-x   0 rreis     (1003) rreis     (1003)     8119 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/tracking/kalman_filter.py
+-rwxrwxr-x   0 rreis     (1003) rreis     (1003)     9033 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/tracking/linear_assignment.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     4870 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/tracking/moving_average.py
+drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-14 14:51:51.151856 moovs_business-0.0.1/moovs_business/utils/
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)        0 2024-05-14 14:50:54.000000 moovs_business-0.0.1/moovs_business/utils/__init__.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     8707 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/utils/helpers.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)    19554 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/utils/math.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)    11732 2024-05-11 17:42:10.000000 moovs_business-0.0.1/moovs_business/utils/pose.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     2490 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/utils/resize.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)     1176 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/utils/serialize.py
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)    25018 2024-05-11 17:32:07.000000 moovs_business-0.0.1/moovs_business/utils/tracks.py
+drwxrwxr-x   0 rreis     (1003) rreis     (1003)        0 2024-05-14 14:51:51.151856 moovs_business-0.0.1/moovs_business.egg-info/
+-rw-r--r--   0 rreis     (1003) rreis     (1003)     2777 2024-05-14 14:51:51.000000 moovs_business-0.0.1/moovs_business.egg-info/PKG-INFO
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)      846 2024-05-14 14:51:51.000000 moovs_business-0.0.1/moovs_business.egg-info/SOURCES.txt
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)        1 2024-05-14 14:51:51.000000 moovs_business-0.0.1/moovs_business.egg-info/dependency_links.txt
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)       77 2024-05-14 14:51:51.000000 moovs_business-0.0.1/moovs_business.egg-info/requires.txt
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)       15 2024-05-14 14:51:51.000000 moovs_business-0.0.1/moovs_business.egg-info/top_level.txt
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)       38 2024-05-14 14:51:51.151856 moovs_business-0.0.1/setup.cfg
+-rw-rw-r--   0 rreis     (1003) rreis     (1003)      818 2024-05-14 14:51:34.000000 moovs_business-0.0.1/setup.py
```

### Comparing `moovs_business-0.0.0/PKG-INFO` & `moovs_business-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
 Name: moovs_business
-Version: 0.0.0
+Version: 0.0.1
 Summary: Empower your software with advanced object detection, human pose estimation, and real-time multi-object tracking to revolutionize how you interact with the physical world.
 Home-page: https://github.com/dotmoovs/moovs-business
 Author: Guilherme Viveiros, Rui Reis.
 Author-email: guilherme.viveiros@dotmoovs.com, rui.reis@dotmoovs.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: numpy==1.24.4
+Requires-Dist: vidgear==0.3.2
+Requires-Dist: pyqflow==1.1.1
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: pydantic
+Requires-Dist: scipy
 
 # moovs-business
 
 `moovs-business` is a powerful Python package that empowers software with advanced capabilities in object detection, human pose estimation, and real-time multi-object tracking. This package is designed to revolutionize how applications interact with the physical world by providing easy-to-integrate tools for analyzing video content.
 
 ## Features
```

### Comparing `moovs_business-0.0.0/README.md` & `moovs_business-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/flows/detection.py` & `moovs_business-0.0.1/moovs_business/flows/detection.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/flows/human_pose.py` & `moovs_business-0.0.1/moovs_business/flows/human_pose.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/flows/tracking.py` & `moovs_business-0.0.1/moovs_business/flows/tracking.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/structs.py` & `moovs_business-0.0.1/moovs_business/structs.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/tracking/iou_matching.py` & `moovs_business-0.0.1/moovs_business/tracking/iou_matching.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/tracking/kalman_filter.py` & `moovs_business-0.0.1/moovs_business/tracking/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/tracking/linear_assignment.py` & `moovs_business-0.0.1/moovs_business/tracking/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business/tracking/moving_average.py` & `moovs_business-0.0.1/moovs_business/tracking/moving_average.py`

 * *Files identical despite different names*

### Comparing `moovs_business-0.0.0/moovs_business.egg-info/PKG-INFO` & `moovs_business-0.0.1/moovs_business.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
-Name: moovs-business
-Version: 0.0.0
+Name: moovs_business
+Version: 0.0.1
 Summary: Empower your software with advanced object detection, human pose estimation, and real-time multi-object tracking to revolutionize how you interact with the physical world.
 Home-page: https://github.com/dotmoovs/moovs-business
 Author: Guilherme Viveiros, Rui Reis.
 Author-email: guilherme.viveiros@dotmoovs.com, rui.reis@dotmoovs.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: numpy==1.24.4
+Requires-Dist: vidgear==0.3.2
+Requires-Dist: pyqflow==1.1.1
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: pydantic
+Requires-Dist: scipy
 
 # moovs-business
 
 `moovs-business` is a powerful Python package that empowers software with advanced capabilities in object detection, human pose estimation, and real-time multi-object tracking. This package is designed to revolutionize how applications interact with the physical world by providing easy-to-integrate tools for analyzing video content.
 
 ## Features
```

### Comparing `moovs_business-0.0.0/setup.py` & `moovs_business-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fr:
     installation_requirements = fr.readlines()
 
 setuptools.setup(
     name="moovs_business",
-    version="0.0.0",
+    version="0.0.1",
     author="Guilherme Viveiros, Rui Reis.",
     author_email="guilherme.viveiros@dotmoovs.com, rui.reis@dotmoovs.com",
     description="Empower your software with advanced object detection, human pose estimation, and real-time multi-object tracking to revolutionize how you interact with the physical world.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dotmoovs/moovs-business",
     packages=setuptools.find_packages(),
```

