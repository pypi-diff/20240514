# Comparing `tmp/adb_tool_py-0.0.2.tar.gz` & `tmp/adb_tool_py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb_tool_py-0.0.2.tar", last modified: Mon May 13 12:22:31 2024, max compression
+gzip compressed data, was "adb_tool_py-0.0.3.tar", last modified: Mon May 13 14:07:07 2024, max compression
```

## Comparing `adb_tool_py-0.0.2.tar` & `adb_tool_py-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 12:22:31.054522 adb_tool_py-0.0.2/
--rw-r--r--   0 iuchi      (501) staff       (20)     1059 2024-05-12 12:33:16.000000 adb_tool_py-0.0.2/LICENSE
--rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-12 13:08:55.000000 adb_tool_py-0.0.2/MANIFEST.in
--rw-r--r--   0 iuchi      (501) staff       (20)      446 2024-05-13 12:22:31.054397 adb_tool_py-0.0.2/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)       14 2024-05-12 13:37:06.000000 adb_tool_py-0.0.2/README.md
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 12:22:31.053732 adb_tool_py-0.0.2/adb_tool_py/
--rw-r--r--   0 iuchi      (501) staff       (20)        0 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/__init__.py
--rw-r--r--   0 iuchi      (501) staff       (20)     1820 2024-05-12 13:37:06.000000 adb_tool_py-0.0.2/adb_tool_py/adb_command.py
--rw-r--r--   0 iuchi      (501) staff       (20)       84 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/adb_device.py
--rw-r--r--   0 iuchi      (501) staff       (20)     2605 2024-05-12 13:46:35.000000 adb_tool_py-0.0.2/adb_tool_py/adb_tool.py
--rw-r--r--   0 iuchi      (501) staff       (20)     4360 2024-05-12 13:37:06.000000 adb_tool_py-0.0.2/adb_tool_py/adb_view_tree.py
--rw-r--r--   0 iuchi      (501) staff       (20)      468 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/command.py
--rw-r--r--   0 iuchi      (501) staff       (20)     2436 2024-05-12 12:33:36.000000 adb_tool_py-0.0.2/adb_tool_py/ui_node.py
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 12:22:31.054249 adb_tool_py-0.0.2/adb_tool_py.egg-info/
--rw-r--r--   0 iuchi      (501) staff       (20)      446 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)      388 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/SOURCES.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/dependency_links.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        8 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/requires.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-13 12:22:31.000000 adb_tool_py-0.0.2/adb_tool_py.egg-info/top_level.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-13 12:22:31.054562 adb_tool_py-0.0.2/setup.cfg
--rw-r--r--   0 iuchi      (501) staff       (20)      756 2024-05-13 12:20:55.000000 adb_tool_py-0.0.2/setup.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 14:07:07.445670 adb_tool_py-0.0.3/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1059 2024-05-12 12:33:16.000000 adb_tool_py-0.0.3/LICENSE
+-rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-12 13:08:55.000000 adb_tool_py-0.0.3/MANIFEST.in
+-rw-r--r--   0 iuchi      (501) staff       (20)     1276 2024-05-13 14:07:07.445558 adb_tool_py-0.0.3/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      844 2024-05-13 14:06:36.000000 adb_tool_py-0.0.3/README.md
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 14:07:07.444868 adb_tool_py-0.0.3/adb_tool_py/
+-rw-r--r--   0 iuchi      (501) staff       (20)      175 2024-05-13 13:35:05.000000 adb_tool_py-0.0.3/adb_tool_py/__init__.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     1936 2024-05-13 13:42:45.000000 adb_tool_py-0.0.3/adb_tool_py/adb_command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)       91 2024-05-13 13:07:27.000000 adb_tool_py-0.0.3/adb_tool_py/adb_device.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     2691 2024-05-13 13:56:34.000000 adb_tool_py-0.0.3/adb_tool_py/adb_tool.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     4339 2024-05-13 13:42:36.000000 adb_tool_py-0.0.3/adb_tool_py/adb_view_tree.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      468 2024-05-12 12:33:36.000000 adb_tool_py-0.0.3/adb_tool_py/command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     2436 2024-05-12 12:33:36.000000 adb_tool_py-0.0.3/adb_tool_py/ui_node.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-13 14:07:07.445407 adb_tool_py-0.0.3/adb_tool_py.egg-info/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1276 2024-05-13 14:07:07.000000 adb_tool_py-0.0.3/adb_tool_py.egg-info/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      388 2024-05-13 14:07:07.000000 adb_tool_py-0.0.3/adb_tool_py.egg-info/SOURCES.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-13 14:07:07.000000 adb_tool_py-0.0.3/adb_tool_py.egg-info/dependency_links.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        8 2024-05-13 14:07:07.000000 adb_tool_py-0.0.3/adb_tool_py.egg-info/requires.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-13 14:07:07.000000 adb_tool_py-0.0.3/adb_tool_py.egg-info/top_level.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-13 14:07:07.445711 adb_tool_py-0.0.3/setup.cfg
+-rw-r--r--   0 iuchi      (501) staff       (20)      756 2024-05-13 14:06:47.000000 adb_tool_py-0.0.3/setup.py
```

### Comparing `adb_tool_py-0.0.2/LICENSE` & `adb_tool_py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adb_tool_py-0.0.2/adb_tool_py/adb_command.py` & `adb_tool_py-0.0.3/adb_tool_py/adb_command.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import subprocess
 from functools import singledispatchmethod
-import adb_tool_py.adb_device as adb_device
+import adb_tool_py as adb_tool
 import adb_tool_py.command as command
 
 
 class AdbCommand:
-    device: adb_device.AdbDevice = None
+    device: adb_tool.AdbDevice = None
 
-    def __init__(self, adb: str = "adb"):
+    def __init__(self, adb: str = "adb", device: adb_tool.AdbDevice = None):
         self.adb = adb
+        self.set_device(device)
+
+    def set_device(self, device: adb_tool.AdbDevice) -> 'AdbCommand':
+        self.device = device
+        return self
 
     def _base_cmd(self) -> list:
-        if self.device is None:
+        if self.device is None or self.device.serial is None:
             return [self.adb]
         else:
             return [self.adb, '-s', self.device.serial]
 
-    def set_device(self, device: adb_device.AdbDevice):
-        self.device = device
-
     @singledispatchmethod
     def query(self, cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE) -> subprocess.CompletedProcess:
         raise NotImplementedError("Unsupported type")
 
     @query.register
     def _(self, cmd: str, stdout=subprocess.PIPE, stderr=subprocess.PIPE) -> subprocess.CompletedProcess:
         return self.query(cmd.split(' '), stdout, stderr)
```

### Comparing `adb_tool_py-0.0.2/adb_tool_py/adb_tool.py` & `adb_tool_py-0.0.3/adb_tool_py/adb_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 import io
 import subprocess
 import tempfile
-import adb_tool_py.adb_command as adb_command
-import adb_tool_py.adb_view_tree as adb_view_tree
+import adb_tool_py as adb_tool
 import adb_tool_py.ui_node as ui_node
 
 
 class AdbTool:
-    def __init__(self, adb: adb_command.AdbCommand = adb_command.AdbCommand()):
-        self.adb = adb
-        self.adbv = adb_view_tree.AdbViewTree(adb)
+    def __init__(self, adb_command: adb_tool.AdbCommand):
+        self.adb = adb_command
+        self.avt = adb_tool.AdbViewTree(adb_command)
+
+    def __init__(self, adb: str = "adb", serial: str = None):
+        self.adb = adb_tool.AdbCommand(adb, adb_tool.AdbDevice(serial))
+        self.avt = adb_tool.AdbViewTree(self.adb)
 
-    def adb(self, cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE) -> str:
+    def query(self, cmd: str, stdout=subprocess.PIPE, stderr=subprocess.PIPE) -> subprocess.Popen:
         return self.adb.query(cmd, stdout, stderr)
 
-    def adb_async(self, cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE) -> subprocess.Popen:
+    def query_async(self, cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE) -> subprocess.Popen:
         return self.adb.query_async(cmd, stdout, stderr)
 
     def logcat(self, output_file=None, cmd: str = '') -> tuple[subprocess.Popen, io.TextIOWrapper]:
         if output_file is None:
             output_file = tempfile.NamedTemporaryFile(delete=False)
-        return self.adb_async(['logcat', *(cmd.split(' '))], stdout=output_file), output_file
+        return self.query_async(['logcat', *(cmd.split(' '))], stdout=output_file), output_file
 
     def logcat_clear(self, cmd: str = '') -> str:
-        return self.adb(['logcat', '-c', *(cmd.split(' '))])
+        return self.query(['logcat', '-c', *(cmd.split(' '))])
 
     def logcat_dump(self, cmd: str = '') -> str:
-        return self.adb(['logcat', '-d', *(cmd.split(' '))])
+        return self.query(['logcat', '-d', *(cmd.split(' '))])
 
     def capture(self) -> None:
-        self.adbv.capture()
+        self.avt.capture()
 
-    def content_tree(self) -> adb_view_tree.ui_node.UINode:
-        return self.adbv.content_tree
+    def content_tree(self) -> ui_node.UINode:
+        return self.avt.content_tree
 
-    def find_text(self, text: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> adb_view_tree.ui_node.UINode:
-        return self.adbv.find_text(text, index, root_node, is_capture)
+    def find_text(self, text: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> ui_node.UINode:
+        return self.avt.find_text(text, index, root_node, is_capture)
 
-    def find_resource_id(self, resource_id: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> adb_view_tree.ui_node.UINode:
-        return self.adbv.find_resource_id(resource_id, index, root_node, is_capture)
+    def find_resource_id(self, resource_id: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> ui_node.UINode:
+        return self.avt.find_resource_id(resource_id, index, root_node, is_capture)
 
     def check_text(self, text: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> bool:
-        return self.adbv.check_text(text, index, root_node, is_capture)
+        return self.avt.check_text(text, index, root_node, is_capture)
 
     def check_resource_id(self, resource_id: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> bool:
-        return self.adbv.check_resource_id(resource_id, index, root_node, is_capture)
+        return self.avt.check_resource_id(resource_id, index, root_node, is_capture)
 
     def touch_text(self, text: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> bool:
-        return self.adbv.touch_text(text, index, root_node, is_capture)
+        return self.avt.touch_text(text, index, root_node, is_capture)
 
     def touch_resource_id(self, resource_id: str, index: int = 0, root_node: ui_node.UINode = None, is_capture: bool = False) -> bool:
-        return self.adbv.touch_resource_id(resource_id, index, root_node, is_capture)
+        return self.avt.touch_resource_id(resource_id, index, root_node, is_capture)
```

### Comparing `adb_tool_py-0.0.2/adb_tool_py/adb_view_tree.py` & `adb_tool_py-0.0.3/adb_tool_py/adb_view_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import chardet
 import os
 import tempfile
 import xml.etree.ElementTree as ET
-import adb_tool_py.adb_command as adb_command
+import adb_tool_py as adb_tool
 import adb_tool_py.ui_node as ui_node
 
 
 DEVICE_FILE_PATH = '/sdcard/window_dump.xml'
 
 
 def _parse_uiautomator_tree(content: str) -> ui_node.UINode:
@@ -24,15 +24,15 @@
             _build_tree(child_element, child_node)
 
 
 class AdbViewTree:
     content: str = None
     content_tree: ui_node.UINode = None
 
-    def __init__(self, adb: adb_command.AdbCommand = adb_command.AdbCommand()):
+    def __init__(self, adb: adb_tool.AdbCommand = adb_tool.AdbCommand()):
         self.adb = adb
 
     def capture(self) -> None:
         # capture
         ret = self.adb.query(f'shell uiautomator dump {DEVICE_FILE_PATH}')
         if ret.returncode != 0:
             raise Exception(f"Error: {ret.stderr}")
```

### Comparing `adb_tool_py-0.0.2/adb_tool_py/ui_node.py` & `adb_tool_py-0.0.3/adb_tool_py/ui_node.py`

 * *Files identical despite different names*

### Comparing `adb_tool_py-0.0.2/setup.py` & `adb_tool_py-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='adb_tool_py',
-    version='0.0.2',
+    version='0.0.3',
     author='Shota Iuchi',
     author_email='shotaiuchi.develop@gmail.com',
     description='adb_tool_py is a tool for Android Debug Bridge (adb).',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ShotaIuchi/adb-tool-py',
     license='MIT',
```

