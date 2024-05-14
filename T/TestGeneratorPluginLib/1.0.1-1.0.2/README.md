# Comparing `tmp/TestGeneratorPluginLib-1.0.1.tar.gz` & `tmp/TestGeneratorPluginLib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.0.1.tar", last modified: Tue May 14 16:12:12 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.0.2.tar", last modified: Tue May 14 17:41:50 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.0.1.tar` & `TestGeneratorPluginLib-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/
--rw-rw-rw-   0        0        0     1090 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 16:12:12.648520 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      191 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0      830 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0      965 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0     2728 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     3248 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:41:50.042178 TestGeneratorPluginLib-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-14 17:41:50.042178 TestGeneratorPluginLib-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 17:41:50.042178 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      191 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0      830 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0      965 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0     2760 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     3344 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:41:50.042178 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-14 17:41:49.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-05-14 17:41:50.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:41:49.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-14 17:41:49.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-14 17:41:49.000000 TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:41:50.042178 TestGeneratorPluginLib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-14 17:40:47.000000 TestGeneratorPluginLib-1.0.2/setup.py
```

### Comparing `TestGeneratorPluginLib-1.0.1/LICENSE` & `TestGeneratorPluginLib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.1/PKG-INFO` & `TestGeneratorPluginLib-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,31 +20,31 @@
                  platform_specific: bool = None,
                  dependencies: Iterable[str] = tuple(),
                  conflicts: Iterable[str] = tuple(),
 
                  directories: Iterable[str] = tuple(),
                  requirements: Iterable[str] = tuple(),
 
-                 main_tabs: Iterable[Callable[[BackendManager], MainTab]] = tuple(),
-                 side_tabs: Iterable[SideTab] = tuple(),
+                 main_tabs: dict[str: Callable[[BackendManager], MainTab]] = None,
+                 side_tabs: dict[str: Callable[[BackendManager], SideTab]] = None,
                  ):
         self.name = name
         self.description = description
         self.version = version
         self.author = author
         self.url = url
         self.platform_specific = bool(requirements) if platform_specific is None else platform_specific
         self.dependencies = list(dependencies)
         self.conflicts = list(conflicts)
 
         self._directories = list(directories)
         self._requirements = list(requirements)
 
-        self.main_tabs = list(main_tabs)
-        self.side_tabs = list(side_tabs)
+        self.main_tabs = main_tabs or dict()
+        self.side_tabs = side_tabs or dict()
 
         self._parse_args()
 
     def _parse_args(self):
         _parser = argparse.ArgumentParser()
         _parser.add_argument('-b', '--build', action='store_true')
         _parser.add_argument('-u', '--upload', action='store_true')
```

### Comparing `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib/_widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 from PyQt6.QtGui import QCursor
 from PyQtUIkit.widgets import KitVBoxLayout, KitHBoxLayout, KitIconButton, KitLabel, KitVSeparator
 
 from TestGeneratorPluginLib._managers import BackendManager
 
 
 class MainTab(KitVBoxLayout):
-    def __init__(self):
+    def __init__(self, name=''):
         super().__init__()
+        self.name = name
         self.need_project = False
 
     def command(self, *args, **kwargs):
         pass
 
 
 class SideTab(KitHBoxLayout):
     startResizing = pyqtSignal()
     resized = pyqtSignal(int)
 
-    def __init__(self, bm: BackendManager, name=''):
+    def __init__(self, bm: BackendManager, name='', icon=''):
         super().__init__()
         self.bm = bm
+        self.name = name
+        self.icon = icon
         self.side_panel_width = 300
 
         self.__layout = KitVBoxLayout()
         self.__layout.setContentsMargins(5, 5, 0, 5)
         self.__layout.setSpacing(5)
         self.addWidget(self.__layout)
```

### Comparing `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.0.2/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.1/setup.py` & `TestGeneratorPluginLib-1.0.2/setup.py`

 * *Files identical despite different names*

