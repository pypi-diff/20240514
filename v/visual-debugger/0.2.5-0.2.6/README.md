# Comparing `tmp/visual_debugger-0.2.5.tar.gz` & `tmp/visual_debugger-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual_debugger-0.2.5.tar", last modified: Tue May 14 02:00:47 2024, max compression
+gzip compressed data, was "visual_debugger-0.2.6.tar", last modified: Tue May 14 04:29:09 2024, max compression
```

## Comparing `visual_debugger-0.2.5.tar` & `visual_debugger-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:00:47.356798 visual_debugger-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-14 02:00:47.356798 visual_debugger-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-14 02:00:43.000000 visual_debugger-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:00:47.356798 visual_debugger-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-14 02:00:43.000000 visual_debugger-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:00:47.352798 visual_debugger-0.2.5/visual_debugger/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 02:00:43.000000 visual_debugger-0.2.5/visual_debugger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-05-14 02:00:43.000000 visual_debugger-0.2.5/visual_debugger/visual_debugger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:00:47.356798 visual_debugger-0.2.5/visual_debugger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-14 02:00:47.000000 visual_debugger-0.2.5/visual_debugger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 02:00:47.000000 visual_debugger-0.2.5/visual_debugger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:00:47.000000 visual_debugger-0.2.5/visual_debugger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 02:00:47.000000 visual_debugger-0.2.5/visual_debugger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 02:00:47.000000 visual_debugger-0.2.5/visual_debugger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:29:09.821136 visual_debugger-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-14 04:29:09.821136 visual_debugger-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-14 04:29:05.000000 visual_debugger-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 04:29:09.821136 visual_debugger-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-14 04:29:05.000000 visual_debugger-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:29:09.817136 visual_debugger-0.2.6/visual_debugger/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 04:29:05.000000 visual_debugger-0.2.6/visual_debugger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-14 04:29:05.000000 visual_debugger-0.2.6/visual_debugger/visual_debugger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:29:09.821136 visual_debugger-0.2.6/visual_debugger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-14 04:29:09.000000 visual_debugger-0.2.6/visual_debugger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 04:29:09.000000 visual_debugger-0.2.6/visual_debugger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:29:09.000000 visual_debugger-0.2.6/visual_debugger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 04:29:09.000000 visual_debugger-0.2.6/visual_debugger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 04:29:09.000000 visual_debugger-0.2.6/visual_debugger.egg-info/top_level.txt
```

### Comparing `visual_debugger-0.2.5/PKG-INFO` & `visual_debugger-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual_debugger
-Version: 0.2.5
+Version: 0.2.6
 Summary: A module to help debugging visual workflows
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `visual_debugger-0.2.5/README.md` & `visual_debugger-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `visual_debugger-0.2.5/setup.py` & `visual_debugger-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import setuptools
 import subprocess
 import os
 
 setup(
     name='visual_debugger',  # Package name
-    version='0.2.5',  # Version of your package
+    version='0.2.6',  # Version of your package
     author='Enes Kuzucu',  # Your name
 
     description='A module to help debugging visual workflows',  # Short description
     long_description=open('README.md').read(),  # Long description from a README file
     long_description_content_type='text/markdown',  # Type of the long description
 #     url='https://github.com/karaposu/image-input-handler',  # URL to the repository
     packages=find_packages(),  # Automatically find packages in the directory
```

### Comparing `visual_debugger-0.2.5/visual_debugger/visual_debugger.py` & `visual_debugger-0.2.6/visual_debugger/visual_debugger.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,22 +177,24 @@
             p, y, r = annotation.orientation
             image = self.draw_orientation(image, y, p, r)
 
 
 def main():
     img_input = "sample_image.jpg"
     uiih = UniversalImageInputHandler(img_input, debug=False)
+    img=uiih.img
 
-    debug_folder_path = "./"
-    visdebugger = VisualDebugger(tag="HS", debug_folder_path=debug_folder_path, active=True, output='return')
+    vd = VisualDebugger(tag="visuals", debug_folder_path="./", active=True)
+    # vd = VisualDebugger(tag="visuals", debug_folder_path=debug_folder_path, active=True, output='return')
+    # annotations = [Annotation(type=AnnotationType.POINTS, coordinates=result["landmark_list"], color=(0, 255, 0))]
     annotations = [Annotation(type=AnnotationType.PITCH_YAW_ROLL, coordinates=(320, 240), orientation=(0.5, 0.5, 0.5))]
+    vd.visual_debug(img, annotations, process_step="head_orientation")
 
-    img = visdebugger.visual_debug(uiih.img, annotations, process_step="cropped_headselection_mask", condition="", mask=False)
-
-    if img is not None:
-        cv2.imshow("Debug Image", img)
-        cv2.waitKey(0)
-        cv2.destroyAllWindows()
+    # img = vd.visual_debug(uiih.img, annotations, process_step="cropped_headselection_mask", condition="", mask=False)
+    # if img is not None:
+    #     cv2.imshow("Debug Image", img)
+    #     cv2.waitKey(0)
+    #     cv2.destroyAllWindows()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `visual_debugger-0.2.5/visual_debugger.egg-info/PKG-INFO` & `visual_debugger-0.2.6/visual_debugger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual_debugger
-Version: 0.2.5
+Version: 0.2.6
 Summary: A module to help debugging visual workflows
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

