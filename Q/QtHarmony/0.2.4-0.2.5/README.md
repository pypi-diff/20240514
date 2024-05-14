# Comparing `tmp/qtharmony-0.2.4.tar.gz` & `tmp/qtharmony-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.2.4.tar", max compression
+gzip compressed data, was "qtharmony-0.2.5.tar", max compression
```

## Comparing `qtharmony-0.2.4.tar` & `qtharmony-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.4/LICENSE
--rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.2.4/README.md
--rw-r--r--   0        0        0      609 2024-05-14 07:15:20.617023 qtharmony-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.4/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.4/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.4/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.4/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     4435 2024-05-14 07:15:03.814438 qtharmony-0.2.4/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.2.4/qtharmony/resources/themes/dark-green.json
--rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.4/qtharmony/resources/themes/light-green.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.4/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.4/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.4/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.4/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.4/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.4/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.4/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.4/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.4/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.4/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/src/core/sizes.py
--rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.4/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.4/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     2353 2024-05-14 07:15:03.814438 qtharmony-0.2.4/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2316 2024-05-12 10:49:33.152065 qtharmony-0.2.4/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2642 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2492 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3472 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2489 2024-05-12 10:24:10.276814 qtharmony-0.2.4/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0      815 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/basic/frame.py
--rw-r--r--   0        0        0     2704 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3190 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3784 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1922 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1994 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.4/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.4/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.4/qtharmony/widgets/basic/styles/frame.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.4/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.4/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.4/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.4/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.4/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.4/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.4/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.4/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.4/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 qtharmony-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.2.5/README.md
+-rw-r--r--   0        0        0      609 2024-05-14 07:45:29.350356 qtharmony-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.5/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.5/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     4435 2024-05-14 07:15:03.814438 qtharmony-0.2.5/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.2.5/qtharmony/resources/themes/dark-green.json
+-rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.5/qtharmony/resources/themes/light-green.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.5/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.5/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.5/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.5/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.5/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.5/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.5/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/src/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.5/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.5/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     2353 2024-05-14 07:15:03.814438 qtharmony-0.2.5/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2335 2024-05-14 07:45:16.057622 qtharmony-0.2.5/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2661 2024-05-14 07:44:47.268920 qtharmony-0.2.5/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2512 2024-05-14 07:44:19.826823 qtharmony-0.2.5/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3491 2024-05-14 07:43:58.894434 qtharmony-0.2.5/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2508 2024-05-14 07:43:32.785611 qtharmony-0.2.5/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0      852 2024-05-14 07:42:04.482929 qtharmony-0.2.5/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2729 2024-05-14 07:46:30.804254 qtharmony-0.2.5/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3190 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3789 2024-05-14 07:42:59.490446 qtharmony-0.2.5/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1941 2024-05-14 07:42:43.167850 qtharmony-0.2.5/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1994 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.5/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.5/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.5/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.5/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.5/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.5/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.5/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.5/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.5/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.5/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.5/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.5/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 qtharmony-0.2.5/PKG-INFO
```

### Comparing `qtharmony-0.2.4/LICENSE` & `qtharmony-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/README.md` & `qtharmony-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/pyproject.toml` & `qtharmony-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.2.4"
+version = "0.2.5"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.2.4/qtharmony/constructor/initialize.py` & `qtharmony-0.2.5/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.2.5/qtharmony/resources/themes/dark-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/resources/themes/dark-green.json` & `qtharmony-0.2.5/qtharmony/resources/themes/dark-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/resources/themes/light-default.json` & `qtharmony-0.2.5/qtharmony/resources/themes/light-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/resources/themes/light-green.json` & `qtharmony-0.2.5/qtharmony/resources/themes/light-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/resources/ui/Icon.png` & `qtharmony-0.2.5/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/resources/ui/Logo.png` & `qtharmony-0.2.5/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.2.5/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/src/core/dialog.py` & `qtharmony-0.2.5/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/src/core/font.py` & `qtharmony-0.2.5/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/src/core/load.py` & `qtharmony-0.2.5/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/src/core/sizes.py` & `qtharmony-0.2.5/qtharmony/src/core/sizes.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/src/core/stylesheet.py` & `qtharmony-0.2.5/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.2.5/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.2.5/qtharmony/src/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/button.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/button.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
               - Initializes the PushButton widget with optional text, size, font, and stylesheet.
 
     """
 
     def __init__(
             self, 
             text: Optional[str] = None,
-            size: tuple[int, int] = (100, 25),
+            size: Optional[tuple[int, int]] = None,
             font: Optional["QFont"] = None, 
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None, 
     ) -> None:
         """
         Initializes the PushButton widget with optional text, size, font, and stylesheet.
@@ -52,14 +52,14 @@
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
             name="PushButton", obj_name="QPushButton#button",
             stylesheet=stylesheet
         )
         
         self.setObjectName("button")
-        self.setFixedSize(QSize(*size))
+        if size is not None: self.setFixedSize(*size)
 
         if text is not None:
             self.setText(text)
         
         if stylesheet is not None:
             self.setStyleSheet(self.styleSheet() + stylesheet)
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/check_box.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
               *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
               - Initializes the CheckBox widget with optional text, size, checkability, checked state, disabled state, and stylesheet.
     """
 
     def __init__(
             self,
             text: Optional[str] = None,
-            size: tuple[int, int] = (150, 30),
+            size: Optional[tuple[int, int]] = None,
             is_checkable: bool = True,
             is_checked: bool = False,
             is_disabled: bool = False,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
@@ -43,15 +43,15 @@
             stylesheet (Optional[str], optional): Custom stylesheet for the checkbox widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the checkbox. Defaults to None.
         """
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        self.setFixedSize(QSize(*size))
+        if size is not None: self.setFixedSize(*size)
         self.setChecked(is_checked)
         self.setCheckable(is_checkable)
         self.setDisabled(is_disabled)
 
         self.setObjectName("check-box")
         if text is not None:
             self.setText(text)
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/digital_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
               *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
               - Initializes the DigitalEntry widget with optional range, size, font, button inclusion, and stylesheet.
     """
 
     def __init__(
             self, 
             range: tuple[int, int] = (0, 100), 
-            size: tuple[int, int] = (40, 30), 
+            size: Optional[tuple[int, int]] = None, 
             font: Optional["QFont"] = None, 
             include_buttons: bool = False,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
@@ -42,15 +42,15 @@
             stylesheet (Optional[str], optional): Custom stylesheet for the spin box widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the spin box. Defaults to None.
         """
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        self.setFixedSize(QSize(*size))
+        if size is not None: self.setFixedSize(*size)
         if not include_buttons: self.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
         if font is not None: self.setFont(font)
 
         self.setObjectName("digital-entry")
         self.setRange(*range)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     - set_items(*__values: str) -> None
               - Sets the items in the drop-down menu with the provided values.
     """
 
     def __init__(
             self, 
             values: Optional[list[str]] = None, 
-            size: tuple[int, int] = (200, 30),
+            size: Optional[tuple[int, int]] = None,
             font: Optional["QFont"] = None, 
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the DropDownMenu widget with optional values, size, font, and stylesheet.
@@ -46,15 +46,15 @@
             stylesheet (Optional[str], optional): Custom stylesheet for the drop-down menu widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the drop-down menu. Defaults to None.
         """
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        self.setFixedSize(QSize(*size))
+        if size is not None: self.setFixedSize(*size)
         self.view().setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         self.__values = []
 
         if values is not None: self.__values = [*values]
         self.addItems(self.__values)
         self.setObjectName("drop-down-menu")
         if font is not None: self.setFont(font)
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/entry.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
               - Initializes the Entry widget with optional text, placeholder, size, font, and stylesheet.
     """
 
     def __init__(
             self, 
             placed: Optional[str] = None, 
             placeholder: Optional[str] = None,
-            size: tuple[int, int] = (200, 30), 
+            size: Optional[tuple[int, int]] = None, 
             font: Optional["QFont"] = None, 
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the Entry widget with optional text, placeholder, size, font, and stylesheet.
@@ -44,16 +44,16 @@
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if placed is not None: self.setText(placed)
         if placeholder is not None: self.setPlaceholderText(placeholder)
         if font is not None: self.setFont(font)
+        if size is not None: self.setFixedSize(*size)
 
-        self.setFixedSize(QSize(*size))
         self.setObjectName("entry")
         self.setFocusPolicy(Qt.FocusPolicy.WheelFocus)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/entry.css", 
             name="Entry", obj_name="QLineEdit#entry",
             stylesheet=stylesheet
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/frame.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/frame.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,24 +9,25 @@
     from PySide6.QtWidgets import QWidget
 
 
 class Frame(QFrame):
 
     def __init__(
             self,
-            size: tuple[int, int] = (600, 400),
+            size: Optional[tuple[int, int]] = None,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
             name="Frame", obj_name="QFrame#frame",
             stylesheet=stylesheet
         )
         self.setObjectName("frame")
 
-        self.setFixedSize(*size)
+        if size is not None:
+            self.setFixedSize(*size)
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/groups.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     - __init__(title: Optional[str] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
               - Initializes the GroupBox widget with optional title and stylesheet.
     """
 
     def __init__(
             self,
             title: Optional[str] = None,
-            size: tuple[int, int] = (400, 200),
+            size: Optional[tuple[int, int]] = None,
             orientation: str = "vertical",
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the GroupBox widget with optional title and stylesheet.
@@ -59,15 +59,15 @@
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/group_box.css", 
             name="GroupBox", obj_name="QGroupBox#group-box",
             stylesheet=stylesheet
         )
 
         if title is not None: self.setTitle(title)
-        self.setFixedSize(*size)
+        if size is not None: self.setFixedSize(*size)
 
         if orientation == "vertical": self.mainLayout = QVBoxLayout()
         elif orientation == "horizontal": self.mainLayout = QHBoxLayout()
         else: raise ValueError("Invalid orientation. should be use 'vertical' or 'horizontal'.")
 
         self.setLayout(self.mainLayout)
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/label.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/path_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
               - Returns the Entry widget used for path input.
     """
 
     def __init__(
             self, 
             placed: Optional[str] = None, 
             placeholder: Optional[str] = None,
-            size: tuple[int, int] = (200, 30), 
+            size: Optional[tuple[int, int]] = None, 
             font: Optional["QFont"] = None, 
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the PathEntry widget with path input functionality.
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/radio_button.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
               *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
               - Initializes the RadioButton widget with optional text, size, and stylesheet.
     """
 
     def __init__(
             self,
             text: Optional[str] = None,
-            size: tuple[int, int] = (200, 30),
+            size: Optional[tuple[int, int]] = None,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the RadioButton widget with optional text, size, and stylesheet.
 
@@ -37,15 +37,15 @@
             parent (Optional["QWidget"], optional): Parent widget of the radio button. Defaults to None.
         """ 
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if text is not None: self.setText(text)
-        self.setFixedSize(QSize(*size))
+        if size is not None: self.setFixedSize(*size)
 
         self.setObjectName("radio-button")
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/radio_button.css", 
             name="RadioButton", obj_name="QRadioButton#radio-button",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.2.5/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/qtharmony/windows/main_window.py` & `qtharmony-0.2.5/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.4/PKG-INFO` & `qtharmony-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.2.4
+Version: 0.2.5
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

