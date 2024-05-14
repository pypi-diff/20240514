# Comparing `tmp/qtharmony-0.2.5.tar.gz` & `tmp/qtharmony-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.2.5.tar", max compression
+gzip compressed data, was "qtharmony-0.2.6.tar", max compression
```

## Comparing `qtharmony-0.2.5.tar` & `qtharmony-0.2.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.5/LICENSE
--rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.2.5/README.md
--rw-r--r--   0        0        0      609 2024-05-14 07:45:29.350356 qtharmony-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.5/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.5/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     4435 2024-05-14 07:15:03.814438 qtharmony-0.2.5/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.2.5/qtharmony/resources/themes/dark-green.json
--rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.5/qtharmony/resources/themes/light-green.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.5/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.5/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.5/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.5/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.5/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.5/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/src/core/sizes.py
--rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.5/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.5/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     2353 2024-05-14 07:15:03.814438 qtharmony-0.2.5/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2335 2024-05-14 07:45:16.057622 qtharmony-0.2.5/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2661 2024-05-14 07:44:47.268920 qtharmony-0.2.5/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2512 2024-05-14 07:44:19.826823 qtharmony-0.2.5/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3491 2024-05-14 07:43:58.894434 qtharmony-0.2.5/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2508 2024-05-14 07:43:32.785611 qtharmony-0.2.5/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0      852 2024-05-14 07:42:04.482929 qtharmony-0.2.5/qtharmony/widgets/basic/frame.py
--rw-r--r--   0        0        0     2729 2024-05-14 07:46:30.804254 qtharmony-0.2.5/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3190 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3789 2024-05-14 07:42:59.490446 qtharmony-0.2.5/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1941 2024-05-14 07:42:43.167850 qtharmony-0.2.5/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1994 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.5/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.5/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/styles/frame.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.5/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.5/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.5/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.5/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.5/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.5/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.5/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.5/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 qtharmony-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.2.6/README.md
+-rw-r--r--   0        0        0      609 2024-05-14 09:27:35.576459 qtharmony-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.6/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.6/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.6/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.6/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     4435 2024-05-14 07:15:03.814438 qtharmony-0.2.6/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.2.6/qtharmony/resources/themes/dark-green.json
+-rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.6/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.6/qtharmony/resources/themes/light-green.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.6/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.6/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.6/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.6/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.6/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.6/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.6/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.6/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.6/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.6/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.6/qtharmony/src/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.6/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.6/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.6/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     2353 2024-05-14 07:15:03.814438 qtharmony-0.2.6/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.6/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-14 09:27:26.290205 qtharmony-0.2.6/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2674 2024-05-14 09:27:22.960354 qtharmony-0.2.6/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2521 2024-05-14 09:27:17.723920 qtharmony-0.2.6/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3500 2024-05-14 09:27:12.880802 qtharmony-0.2.6/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2524 2024-05-14 09:27:08.247675 qtharmony-0.2.6/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0      868 2024-05-14 09:27:02.917913 qtharmony-0.2.6/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2742 2024-05-14 09:26:57.594816 qtharmony-0.2.6/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3206 2024-05-14 09:26:52.878359 qtharmony-0.2.6/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3801 2024-05-14 09:26:46.188657 qtharmony-0.2.6/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1951 2024-05-14 09:26:41.755521 qtharmony-0.2.6/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     2007 2024-05-14 09:26:31.902626 qtharmony-0.2.6/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.6/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.6/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.6/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.6/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.6/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.6/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.6/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.6/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.6/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.6/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.6/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.6/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.6/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.6/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.6/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.6/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 qtharmony-0.2.6/PKG-INFO
```

### Comparing `qtharmony-0.2.5/LICENSE` & `qtharmony-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/README.md` & `qtharmony-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/pyproject.toml` & `qtharmony-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.2.5"
+version = "0.2.6"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.2.5/qtharmony/constructor/initialize.py` & `qtharmony-0.2.6/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.2.6/qtharmony/resources/themes/dark-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/resources/themes/dark-green.json` & `qtharmony-0.2.6/qtharmony/resources/themes/dark-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/resources/themes/light-default.json` & `qtharmony-0.2.6/qtharmony/resources/themes/light-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/resources/themes/light-green.json` & `qtharmony-0.2.6/qtharmony/resources/themes/light-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/resources/ui/Icon.png` & `qtharmony-0.2.6/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/resources/ui/Logo.png` & `qtharmony-0.2.6/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.2.6/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/src/core/dialog.py` & `qtharmony-0.2.6/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/src/core/font.py` & `qtharmony-0.2.6/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/src/core/load.py` & `qtharmony-0.2.6/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/src/core/sizes.py` & `qtharmony-0.2.6/qtharmony/src/core/sizes.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/src/core/stylesheet.py` & `qtharmony-0.2.6/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.2.6/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.2.6/qtharmony/src/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/button.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if font is not None: self.setFont(font)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
-            name="PushButton", obj_name="QPushButton#button",
+            name=self.__class__.__name__, obj_name="QPushButton#button",
             stylesheet=stylesheet
         )
         
         self.setObjectName("button")
         if size is not None: self.setFixedSize(*size)
 
         if text is not None:
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/check_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 
         self.setObjectName("check-box")
         if text is not None:
             self.setText(text)
         
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/check_box.css", 
-            name="CheckBox", obj_name="CheckBox#check-box",
+            name=self.__class__.__name__, obj_name="CheckBox#check-box",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/digital_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
         if font is not None: self.setFont(font)
 
         self.setObjectName("digital-entry")
         self.setRange(*range)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/digital_entry.css", 
-            name="DigitalEntry", obj_name="QSpinBox#digital-entry",
+            name=self.__class__.__name__, obj_name="QSpinBox#digital-entry",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         if values is not None: self.__values = [*values]
         self.addItems(self.__values)
         self.setObjectName("drop-down-menu")
         if font is not None: self.setFont(font)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/drop_down_menu.css", 
-            name="DropDownMenu", obj_name="QComboBox#drop-down-menu",
+            name=self.__class__.__name__, obj_name="QComboBox#drop-down-menu",
             stylesheet=stylesheet
         )
 
         self.__load_down_arrow_style()
     
     def __load_down_arrow_style(self) -> None:
         """
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/entry.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,10 +51,10 @@
         if size is not None: self.setFixedSize(*size)
 
         self.setObjectName("entry")
         self.setFocusPolicy(Qt.FocusPolicy.WheelFocus)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/entry.css", 
-            name="Entry", obj_name="QLineEdit#entry",
+            name=self.__class__.__name__, obj_name="QLineEdit#entry",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/frame.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/frame.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             parent: Optional["QWidget"] = None
     ) -> None:
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
-            name="Frame", obj_name="QFrame#frame",
+            name=self.__class__.__name__, obj_name="QFrame#frame",
             stylesheet=stylesheet
         )
         self.setObjectName("frame")
 
         if size is not None:
             self.setFixedSize(*size)
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/groups.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         self.setObjectName("group-box")
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/group_box.css", 
-            name="GroupBox", obj_name="QGroupBox#group-box",
+            name=self.__class__.__name__, obj_name="QGroupBox#group-box",
             stylesheet=stylesheet
         )
 
         if title is not None: self.setTitle(title)
         if size is not None: self.setFixedSize(*size)
 
         if orientation == "vertical": self.mainLayout = QVBoxLayout()
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/label.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/label.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         self.setObjectName("label")
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/label.css", 
-            name="Label", obj_name="QLabel#label",
+            name=self.__class__.__name__, obj_name="QLabel#label",
             stylesheet=stylesheet
         )
 
         self.setText(text)
         if color is not None: self.set_color(color)
         
         self.setWordWrap(word_wrap)
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/path_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         super().__init__(parent)
 
         self.setObjectName("path-entry")
         if font is not None: self.setFont(font)
 
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/path_entry.css", 
-            name="PathEntry", obj_name="QWidget#path-entry",
+            name=self.__class__.__name__, obj_name="QWidget#path-entry",
             stylesheet=stylesheet
         ))
 
         print(self.styleSheet())
 
         self.mainLayout = QHBoxLayout()
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/radio_button.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,10 +42,10 @@
 
         if text is not None: self.setText(text)
         if size is not None: self.setFixedSize(*size)
 
         self.setObjectName("radio-button")
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/radio_button.css", 
-            name="RadioButton", obj_name="QRadioButton#radio-button",
+            name=self.__class__.__name__, obj_name="QRadioButton#radio-button",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/splitter.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         elif __orientation == "vertical": super().__init__(Qt.Orientation.Vertical, parent)
 
         ThemeManager.add_widgets(self)
 
         self.setObjectName("splitter")
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/splitter.css", 
-            name="Splitter", obj_name="QSplitter#splitter",
+            name=self.__class__.__name__, obj_name="QSplitter#splitter",
             stylesheet=stylesheet
         )
 
     def addWidget(self, widget):
         """
         Adds a widget to the splitter and sets it as non-collapsible.
```

### Comparing `qtharmony-0.2.5/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.2.6/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/qtharmony/windows/main_window.py` & `qtharmony-0.2.6/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.5/PKG-INFO` & `qtharmony-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.2.5
+Version: 0.2.6
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

