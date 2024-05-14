# Comparing `tmp/prett6-1.0.tar.gz` & `tmp/prett6-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prett6-1.0.tar", last modified: Mon May 13 08:24:47 2024, max compression
+gzip compressed data, was "prett6-1.1.tar", last modified: Tue May 14 03:32:19 2024, max compression
```

## Comparing `prett6-1.0.tar` & `prett6-1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-13 08:24:47.059526 prett6-1.0/
--rw-r--r--   0 wangcong   (502) staff       (20)     1074 2024-05-13 02:54:26.000000 prett6-1.0/LICENSE
--rw-r--r--   0 wangcong   (502) staff       (20)       86 2024-05-13 02:54:26.000000 prett6-1.0/MANIFEST.in
--rw-r--r--   0 wangcong   (502) staff       (20)     2845 2024-05-13 08:24:47.058324 prett6-1.0/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)     2113 2024-05-13 08:13:53.000000 prett6-1.0/README.rst
--rw-r--r--   0 wangcong   (502) staff       (20)        4 2024-05-13 08:18:22.000000 prett6-1.0/RELEASE-VERSION
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-13 08:24:47.044185 prett6-1.0/prett/
--rw-r--r--   0 wangcong   (502) staff       (20)     1708 2024-05-13 02:54:26.000000 prett6-1.0/prett/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2222 2024-05-13 02:54:26.000000 prett6-1.0/prett/base.py
--rw-r--r--   0 wangcong   (502) staff       (20)     6181 2024-05-13 02:54:26.000000 prett6-1.0/prett/multi_types.py
--rw-r--r--   0 wangcong   (502) staff       (20)     5403 2024-05-13 02:54:26.000000 prett6-1.0/prett/project.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1915 2024-05-13 08:16:03.000000 prett6-1.0/prett/sender.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1263 2024-05-13 02:54:26.000000 prett6-1.0/prett/setting.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2418 2024-05-13 02:54:26.000000 prett6-1.0/prett/widget_interface.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-13 08:24:47.056886 prett6-1.0/prett6.egg-info/
--rw-r--r--   0 wangcong   (502) staff       (20)     2845 2024-05-13 08:24:46.000000 prett6-1.0/prett6.egg-info/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)      437 2024-05-13 08:24:46.000000 prett6-1.0/prett6.egg-info/SOURCES.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        1 2024-05-13 08:24:46.000000 prett6-1.0/prett6.egg-info/dependency_links.txt
--rw-r--r--   0 wangcong   (502) staff       (20)       15 2024-05-13 08:24:46.000000 prett6-1.0/prett6.egg-info/requires.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        6 2024-05-13 08:24:46.000000 prett6-1.0/prett6.egg-info/top_level.txt
--rw-r--r--   0 wangcong   (502) staff       (20)       15 2024-05-13 08:03:38.000000 prett6-1.0/requirements.txt
--rw-r--r--   0 wangcong   (502) staff       (20)       38 2024-05-13 08:24:47.059802 prett6-1.0/setup.cfg
--rw-r--r--   0 wangcong   (502) staff       (20)     1640 2024-05-13 08:13:53.000000 prett6-1.0/setup.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-13 08:24:47.054795 prett6-1.0/tests/
--rw-r--r--   0 wangcong   (502) staff       (20)     2223 2024-05-13 02:54:26.000000 prett6-1.0/tests/test_prett.py
--rw-r--r--   0 wangcong   (502) staff       (20)     3043 2024-05-13 02:54:26.000000 prett6-1.0/tests/test_signal_emit_condition.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2677 2024-05-13 02:54:26.000000 prett6-1.0/tests/test_types.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2174 2024-05-13 02:54:26.000000 prett6-1.0/version.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-14 03:32:19.004930 prett6-1.1/
+-rw-r--r--   0 wangcong   (502) staff       (20)     1074 2024-05-13 02:54:26.000000 prett6-1.1/LICENSE
+-rw-r--r--   0 wangcong   (502) staff       (20)       86 2024-05-13 02:54:26.000000 prett6-1.1/MANIFEST.in
+-rw-r--r--   0 wangcong   (502) staff       (20)     2845 2024-05-14 03:32:19.004310 prett6-1.1/PKG-INFO
+-rw-r--r--   0 wangcong   (502) staff       (20)     2113 2024-05-13 08:13:53.000000 prett6-1.1/README.rst
+-rw-r--r--   0 wangcong   (502) staff       (20)        4 2024-05-14 03:32:18.000000 prett6-1.1/RELEASE-VERSION
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-14 03:32:18.998313 prett6-1.1/prett6/
+-rw-r--r--   0 wangcong   (502) staff       (20)     1708 2024-05-13 02:54:26.000000 prett6-1.1/prett6/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2222 2024-05-13 02:54:26.000000 prett6-1.1/prett6/base.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     6181 2024-05-13 02:54:26.000000 prett6-1.1/prett6/multi_types.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     5403 2024-05-13 02:54:26.000000 prett6-1.1/prett6/project.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1915 2024-05-13 08:16:03.000000 prett6-1.1/prett6/sender.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1263 2024-05-13 02:54:26.000000 prett6-1.1/prett6/setting.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2418 2024-05-13 02:54:26.000000 prett6-1.1/prett6/widget_interface.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-14 03:32:19.003508 prett6-1.1/prett6.egg-info/
+-rw-r--r--   0 wangcong   (502) staff       (20)     2845 2024-05-14 03:32:18.000000 prett6-1.1/prett6.egg-info/PKG-INFO
+-rw-r--r--   0 wangcong   (502) staff       (20)      444 2024-05-14 03:32:18.000000 prett6-1.1/prett6.egg-info/SOURCES.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)        1 2024-05-14 03:32:18.000000 prett6-1.1/prett6.egg-info/dependency_links.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)       15 2024-05-14 03:32:18.000000 prett6-1.1/prett6.egg-info/requires.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)        7 2024-05-14 03:32:18.000000 prett6-1.1/prett6.egg-info/top_level.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)       15 2024-05-13 08:03:38.000000 prett6-1.1/requirements.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)       38 2024-05-14 03:32:19.005083 prett6-1.1/setup.cfg
+-rw-r--r--   0 wangcong   (502) staff       (20)     1640 2024-05-13 08:13:53.000000 prett6-1.1/setup.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-14 03:32:19.002979 prett6-1.1/tests/
+-rw-r--r--   0 wangcong   (502) staff       (20)     2231 2024-05-14 03:30:39.000000 prett6-1.1/tests/test_prett.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     3050 2024-05-14 03:30:39.000000 prett6-1.1/tests/test_signal_emit_condition.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2688 2024-05-14 03:30:39.000000 prett6-1.1/tests/test_types.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2174 2024-05-13 02:54:26.000000 prett6-1.1/version.py
```

### Comparing `prett6-1.0/LICENSE` & `prett6-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prett6-1.0/PKG-INFO` & `prett6-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prett6
-Version: 1.0
+Version: 1.1
 Summary: A Pretty Project Framework
 Home-page: https://github.com/KD-Group/prett
 Author: SF-Zhou
 Author-email: sfzhou.scut@gmail.com
 License: MIT
 Keywords: qt ui
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prett6-1.0/README.rst` & `prett6-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett/__init__.py` & `prett6-1.1/prett6/__init__.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett/base.py` & `prett6-1.1/prett6/base.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett/multi_types.py` & `prett6-1.1/prett6/multi_types.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett/project.py` & `prett6-1.1/prett6/project.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett/sender.py` & `prett6-1.1/prett6/sender.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett/setting.py` & `prett6-1.1/prett6/setting.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett/widget_interface.py` & `prett6-1.1/prett6/widget_interface.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/prett6.egg-info/PKG-INFO` & `prett6-1.1/prett6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prett6
-Version: 1.0
+Version: 1.1
 Summary: A Pretty Project Framework
 Home-page: https://github.com/KD-Group/prett
 Author: SF-Zhou
 Author-email: sfzhou.scut@gmail.com
 License: MIT
 Keywords: qt ui
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prett6-1.0/setup.py` & `prett6-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `prett6-1.0/tests/test_prett.py` & `prett6-1.1/tests/test_prett.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
-import prett
+import prett6
 import unittest
 
 
 class MyTestCase(unittest.TestCase):
     def test_project_storage_tree(self):
-        class ItemDemo(prett.IntProjectItem):
+        class ItemDemo(prett6.IntProjectItem):
             pass
 
-        class ProjectDemo(prett.AbstractProject):
+        class ProjectDemo(prett6.AbstractProject):
             def __init__(self):
                 self.width = ItemDemo(self)
                 self.height = ItemDemo(self)
 
         p = ProjectDemo()
         p.width.int.value = 16
         p.height.int.value = 20
@@ -24,26 +24,26 @@
         self.assertEqual(p.width.value, None)
 
         p.value = json.loads(json_string)
         self.assertEqual(p.width.string.value, '16')
         self.assertEqual(p.height.string.value, '20')
 
     def test_value_changed(self):
-        class ItemDemo(prett.IntProjectItem):
+        class ItemDemo(prett6.IntProjectItem):
             pass
 
-        class ProjectDemo(prett.AbstractProject):
+        class ProjectDemo(prett6.AbstractProject):
             def __init__(self):
                 self.width = ItemDemo(self)
                 self.height = ItemDemo(self)
 
         p = ProjectDemo()
         times = []
 
-        @prett.connect_with(p.width.int.changed)
+        @prett6.connect_with(p.width.int.changed)
         def width_changed(value: int):
             times.append(len(times))
 
             if len(times) == 1:
                 self.assertEqual(value, 16)
             elif len(times) == 2:
                 self.assertEqual(value, 20)
@@ -55,18 +55,18 @@
         p.width.string.value = '16'
         p.width.value = '20'
         p.width.int.value = 0
 
         self.assertEqual(len(times), 3)
 
     def test_setting_value(self):
-        class SettingItemDemo(prett.IntSettingItem):
+        class SettingItemDemo(prett6.IntSettingItem):
             pass
 
-        class SettingDemo(prett.AbstractSetting):
+        class SettingDemo(prett6.AbstractSetting):
             def __init__(self):
                 self.margin = SettingItemDemo(self, 5)
 
         s = SettingDemo()
         self.assertEqual(s.margin.int.value, 5)
         self.assertEqual(s.value, {})
```

### Comparing `prett6-1.0/tests/test_signal_emit_condition.py` & `prett6-1.1/tests/test_signal_emit_condition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import unittest
 
-import prett
+import prett6
 
 
 class MyTestCase(unittest.TestCase):
     def test_dict_item_emit_change_condition(self):
-        class ProjectDemo(prett.AbstractProject):
+        class ProjectDemo(prett6.AbstractProject):
             def __init__(self):
-                self.d = prett.DictProjectItem(self)
+                self.d = prett6.DictProjectItem(self)
 
         p = ProjectDemo()
         self.emit_value = None
 
-        @prett.connect_with(p.d.changed)
+        @prett6.connect_with(p.d.changed)
         def copy_value_from_dict_item(data: dict):
             self.emit_value = data.copy()
 
         # emit changed if use `=` operator
         p.d.dict.value = {1: 2, 3: 4}
         self.assertEqual(self.emit_value, {1: 2, 3: 4})
 
@@ -42,22 +42,22 @@
 
         # emit change if using DictProjectItem method
         p.d.dict.value = {1: 2, 3: 4}
         p.d.dict.pop(1)
         self.assertEqual(self.emit_value, {3: 4})
 
     def test_list_item_emit_change_condition(self):
-        class ProjectDemo(prett.AbstractProject):
+        class ProjectDemo(prett6.AbstractProject):
             def __init__(self):
-                self.ls = prett.ListProjectItem(self)
+                self.ls = prett6.ListProjectItem(self)
 
         p = ProjectDemo()
         self.emit_value = None
 
-        @prett.connect_with(p.ls.changed)
+        @prett6.connect_with(p.ls.changed)
         def copy_value_from_dict_item(data: list):
             self.emit_value = data.copy()
 
         # emit changed if use `=` operator
         p.ls.list.value = [1, 2, 3, 4]
         self.assertEqual(self.emit_value, [1, 2, 3, 4])
```

### Comparing `prett6-1.0/tests/test_types.py` & `prett6-1.1/tests/test_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import unittest
 
-import prett
+import prett6
 
 
 class MyTestCase(unittest.TestCase):
     def test_project_storage_tree(self):
-        class ItemDemo(prett.IntProjectItem):
+        class ItemDemo(prett6.IntProjectItem):
             pass
 
-        class ProjectDemo(prett.AbstractProject):
+        class ProjectDemo(prett6.AbstractProject):
             def __init__(self):
                 self.width = ItemDemo(self)
                 self.height = ItemDemo(self)
 
         p = ProjectDemo()
         p.width.int.value = 16
         p.height.int.value = 20
@@ -25,26 +25,26 @@
         self.assertEqual(p.width.value, None)
 
         p.value = json.loads(json_string)
         self.assertEqual(p.width.string.value, '16')
         self.assertEqual(p.height.string.value, '20')
 
     def test_value_changed(self):
-        class ItemDemo(prett.IntProjectItem):
+        class ItemDemo(prett6.IntProjectItem):
             pass
 
-        class ProjectDemo(prett.AbstractProject):
+        class ProjectDemo(prett6.AbstractProject):
             def __init__(self):
                 self.width = ItemDemo(self)
                 self.height = ItemDemo(self)
 
         p = ProjectDemo()
         times = []
 
-        @prett.connect_with(p.width.int.changed)
+        @prett6.connect_with(p.width.int.changed)
         def width_changed(value: int):
             times.append(len(times))
 
             if len(times) == 1:
                 self.assertEqual(value, 16)
             elif len(times) == 2:
                 self.assertEqual(value, 20)
@@ -56,37 +56,37 @@
         p.width.string.value = '16'
         p.width.value = '20'
         p.width.int.value = 0
 
         self.assertEqual(len(times), 3)
 
     def test_setting_value(self):
-        class SettingItemDemo(prett.IntSettingItem):
+        class SettingItemDemo(prett6.IntSettingItem):
             pass
 
-        class SettingDemo(prett.AbstractSetting):
+        class SettingDemo(prett6.AbstractSetting):
             def __init__(self):
                 self.margin = SettingItemDemo(self, 5)
 
         s = SettingDemo()
         self.assertEqual(s.margin.int.value, 5)
         self.assertEqual(s.value, {})
 
         s.margin.int.value = 20
         self.assertEqual(s.margin.int.value, 20)
         self.assertEqual(s.value, {'margin': '20'})
 
     def test_emun_item(self):
-        class Fruit(prett.Enum):
+        class Fruit(prett6.Enum):
             APPLE = "苹果"
             BANANA = "香蕉"
 
-        class ProjectDemo(prett.AbstractProject):
+        class ProjectDemo(prett6.AbstractProject):
             def __init__(self):
-                self.fruit = prett.EnumItem(self, Fruit)
+                self.fruit = prett6.EnumItem(self, Fruit)
 
         p = ProjectDemo()
         p.fruit.type.value = Fruit.BANANA
 
         self.assertEqual(p.fruit.type.value.value, "香蕉")
         self.assertEqual(p.fruit.type.value, Fruit.BANANA)
```

### Comparing `prett6-1.0/version.py` & `prett6-1.1/version.py`

 * *Files identical despite different names*

