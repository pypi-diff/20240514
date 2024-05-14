# Comparing `tmp/virtual_camera-0.0.1.tar.gz` & `tmp/virtual_camera-0.0.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtual_camera-0.0.1.tar", last modified: Tue May 14 08:56:39 2024, max compression
+gzip compressed data, was "virtual_camera-0.0.2.post0.tar", last modified: Tue May 14 11:39:19 2024, max compression
```

## Comparing `virtual_camera-0.0.1.tar` & `virtual_camera-0.0.2.post0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 08:56:39.803976 virtual_camera-0.0.1/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)     1952 2024-05-14 08:56:39.803976 virtual_camera-0.0.1/PKG-INFO
--rw-rw-r--   0 alpha     (1000) alpha     (1000)       38 2024-05-14 08:56:39.803976 virtual_camera-0.0.1/setup.cfg
--rw-rw-r--   0 alpha     (1000) alpha     (1000)      434 2024-05-14 08:56:32.000000 virtual_camera-0.0.1/setup.py
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 08:56:39.803976 virtual_camera-0.0.1/virtual_camera/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)       28 2024-05-14 08:50:36.000000 virtual_camera-0.0.1/virtual_camera/__init__.py
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 08:56:39.803976 virtual_camera-0.0.1/virtual_camera/data/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)      537 2024-05-14 07:58:20.000000 virtual_camera-0.0.1/virtual_camera/data/calibration.yml
--rw-rw-r--   0 alpha     (1000) alpha     (1000)    55776 2024-05-14 07:56:45.000000 virtual_camera-0.0.1/virtual_camera/data/dst_image.jpg
--rw-rw-r--   0 alpha     (1000) alpha     (1000)    14224 2024-05-14 07:56:45.000000 virtual_camera-0.0.1/virtual_camera/data/mask.png
--rw-rw-r--   0 alpha     (1000) alpha     (1000)   135901 2024-05-14 07:56:44.000000 virtual_camera-0.0.1/virtual_camera/data/src_image.jpg
--rw-rw-r--   0 alpha     (1000) alpha     (1000)    14124 2024-05-14 07:53:55.000000 virtual_camera-0.0.1/virtual_camera/virtual_camera.py
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 08:56:39.803976 virtual_camera-0.0.1/virtual_camera.egg-info/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)     1952 2024-05-14 08:56:39.000000 virtual_camera-0.0.1/virtual_camera.egg-info/PKG-INFO
--rw-rw-r--   0 alpha     (1000) alpha     (1000)      390 2024-05-14 08:56:39.000000 virtual_camera-0.0.1/virtual_camera.egg-info/SOURCES.txt
--rw-rw-r--   0 alpha     (1000) alpha     (1000)        1 2024-05-14 08:56:39.000000 virtual_camera-0.0.1/virtual_camera.egg-info/dependency_links.txt
--rw-rw-r--   0 alpha     (1000) alpha     (1000)       12 2024-05-14 08:56:39.000000 virtual_camera-0.0.1/virtual_camera.egg-info/requires.txt
--rw-rw-r--   0 alpha     (1000) alpha     (1000)       15 2024-05-14 08:56:39.000000 virtual_camera-0.0.1/virtual_camera.egg-info/top_level.txt
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:39:19.281994 virtual_camera-0.0.2.post0/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)     1958 2024-05-14 11:39:19.281994 virtual_camera-0.0.2.post0/PKG-INFO
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)       38 2024-05-14 11:39:19.281994 virtual_camera-0.0.2.post0/setup.cfg
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)      439 2024-05-14 11:39:07.000000 virtual_camera-0.0.2.post0/setup.py
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:39:19.277994 virtual_camera-0.0.2.post0/virtual_camera/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)      712 2024-05-14 11:30:52.000000 virtual_camera-0.0.2.post0/virtual_camera/__init__.py
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:39:19.281994 virtual_camera-0.0.2.post0/virtual_camera/data/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)      537 2024-05-14 07:58:20.000000 virtual_camera-0.0.2.post0/virtual_camera/data/calibration.yml
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)    55776 2024-05-14 07:56:45.000000 virtual_camera-0.0.2.post0/virtual_camera/data/dst_image.jpg
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)    14224 2024-05-14 07:56:45.000000 virtual_camera-0.0.2.post0/virtual_camera/data/mask.png
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)   135901 2024-05-14 07:56:44.000000 virtual_camera-0.0.2.post0/virtual_camera/data/src_image.jpg
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)    14124 2024-05-14 11:29:49.000000 virtual_camera-0.0.2.post0/virtual_camera/virtual_camera.py
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:39:19.277994 virtual_camera-0.0.2.post0/virtual_camera.egg-info/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)     1958 2024-05-14 11:39:19.000000 virtual_camera-0.0.2.post0/virtual_camera.egg-info/PKG-INFO
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)      390 2024-05-14 11:39:19.000000 virtual_camera-0.0.2.post0/virtual_camera.egg-info/SOURCES.txt
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)        1 2024-05-14 11:39:19.000000 virtual_camera-0.0.2.post0/virtual_camera.egg-info/dependency_links.txt
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)       12 2024-05-14 11:39:19.000000 virtual_camera-0.0.2.post0/virtual_camera.egg-info/requires.txt
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)       15 2024-05-14 11:39:19.000000 virtual_camera-0.0.2.post0/virtual_camera.egg-info/top_level.txt
```

### Comparing `virtual_camera-0.0.1/PKG-INFO` & `virtual_camera-0.0.2.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtual_camera
-Version: 0.0.1
+Version: 0.0.2.post0
 Summary: Virtual Camera
 Author: AlphaLFC
 Author-email: 
 Description-Content-Type: text/markdown
 
 # Virtual Camera
```

### Comparing `virtual_camera-0.0.1/virtual_camera/data/calibration.yml` & `virtual_camera-0.0.2.post0/virtual_camera/data/calibration.yml`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.1/virtual_camera/data/dst_image.jpg` & `virtual_camera-0.0.2.post0/virtual_camera/data/dst_image.jpg`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.1/virtual_camera/data/mask.png` & `virtual_camera-0.0.2.post0/virtual_camera/data/mask.png`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.1/virtual_camera/data/src_image.jpg` & `virtual_camera-0.0.2.post0/virtual_camera/data/src_image.jpg`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.1/virtual_camera/virtual_camera.py` & `virtual_camera-0.0.2.post0/virtual_camera/virtual_camera.py`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.1/virtual_camera.egg-info/PKG-INFO` & `virtual_camera-0.0.2.post0/virtual_camera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtual-camera
-Version: 0.0.1
+Version: 0.0.2.post0
 Summary: Virtual Camera
 Author: AlphaLFC
 Author-email: 
 Description-Content-Type: text/markdown
 
 # Virtual Camera
```

