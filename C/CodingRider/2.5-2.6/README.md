# Comparing `tmp/codingrider-2.5.tar.gz` & `tmp/codingrider-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codingrider-2.5.tar", last modified: Tue May 14 03:20:55 2024, max compression
+gzip compressed data, was "codingrider-2.6.tar", last modified: Tue May 14 03:57:30 2024, max compression
```

## Comparing `codingrider-2.5.tar` & `codingrider-2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:20:55.731936 codingrider-2.5/
-drwxrwxrwx   0        0        0        0 2024-05-14 03:20:55.711162 codingrider-2.5/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/crc.py
--rw-rw-rw-   0        0        0    44020 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/drone.py
--rw-rw-rw-   0        0        0    73925 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1904 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10249 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:20:55.728933 codingrider-2.5/CodingRider/tools/
--rw-rw-rw-   0        0        0       33 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/tools/__init__.py
--rw-rw-rw-   0        0        0    31268 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/tools/parser.py
--rw-rw-rw-   0        0        0     9491 2024-05-14 03:14:00.000000 codingrider-2.5/CodingRider/tools/update.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:20:55.729932 codingrider-2.5/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      718 2024-05-14 03:20:55.000000 codingrider-2.5/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2024-05-14 03:20:55.000000 codingrider-2.5/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:20:55.000000 codingrider-2.5/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-14 03:20:55.000000 codingrider-2.5/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 03:20:55.000000 codingrider-2.5/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.5/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      718 2024-05-14 03:20:55.730936 codingrider-2.5/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 03:20:55.731936 codingrider-2.5/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-05-14 03:19:12.000000 codingrider-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.340740 codingrider-2.6/
+drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.331437 codingrider-2.6/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    44020 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    73925 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1904 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10251 2024-05-14 03:51:54.000000 codingrider-2.6/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.339231 codingrider-2.6/CodingRider/tools/
+-rw-rw-rw-   0        0        0       33 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/tools/__init__.py
+-rw-rw-rw-   0        0        0    31268 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/tools/parser.py
+-rw-rw-rw-   0        0        0     9491 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/tools/update.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.339735 codingrider-2.6/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      718 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.6/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      718 2024-05-14 03:57:30.340740 codingrider-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 03:57:30.341882 codingrider-2.6/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-05-14 03:55:16.000000 codingrider-2.6/setup.py
```

### Comparing `codingrider-2.5/CodingRider/crc.py` & `codingrider-2.6/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.5/CodingRider/drone.py` & `codingrider-2.6/CodingRider/drone.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.5/CodingRider/protocol.py` & `codingrider-2.6/CodingRider/protocol.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.5/CodingRider/receiver.py` & `codingrider-2.6/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.5/CodingRider/storage.py` & `codingrider-2.6/CodingRider/storage.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.5/CodingRider/system.py` & `codingrider-2.6/CodingRider/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,19 +81,20 @@
 
 
 
 class ModeSystem(Enum):
     
     None_               = 0x00
 
-    Boot                = 0x01
-    Start               = 0x02
-    Running             = 0x03
-    ReadyToReset        = 0x04
-    Error               = 0x05
+    Boot                = 0x10
+    Start               = 0x11
+    Running             = 0x12
+    ReadyToReset        = 0x13
+
+    Error               = 0xA0
 
     EndOfType           = 0x06
 
 
 
 class ModeControlFlight(Enum):
```

### Comparing `codingrider-2.5/CodingRider/tools/parser.py` & `codingrider-2.6/CodingRider/tools/parser.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.5/CodingRider/tools/update.py` & `codingrider-2.6/CodingRider/tools/update.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.5/CodingRider.egg-info/PKG-INFO` & `codingrider-2.6/CodingRider.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.5
+Version: 2.6
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.5/PKG-INFO` & `codingrider-2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.5
+Version: 2.6
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.5/setup.py` & `codingrider-2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "2.5",
+    version = "2.6",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
```

