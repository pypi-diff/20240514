# Comparing `tmp/qtharmony-0.2.7.tar.gz` & `tmp/qtharmony-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.2.7.tar", max compression
+gzip compressed data, was "qtharmony-0.2.8.tar", max compression
```

## Comparing `qtharmony-0.2.7.tar` & `qtharmony-0.2.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.7/LICENSE
--rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.2.7/README.md
--rw-r--r--   0        0        0      609 2024-05-14 09:59:02.138730 qtharmony-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.7/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.7/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.7/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.7/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     4435 2024-05-14 07:15:03.814438 qtharmony-0.2.7/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.2.7/qtharmony/resources/themes/dark-green.json
--rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.7/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.7/qtharmony/resources/themes/light-green.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.7/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.7/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.7/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.7/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.7/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.7/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.7/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.7/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.7/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.7/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.7/qtharmony/src/core/sizes.py
--rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.7/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.7/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.7/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     2353 2024-05-14 07:15:03.814438 qtharmony-0.2.7/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.7/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2360 2024-05-14 09:57:46.458842 qtharmony-0.2.7/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2685 2024-05-14 09:57:33.139448 qtharmony-0.2.7/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2528 2024-05-14 09:58:01.104841 qtharmony-0.2.7/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3506 2024-05-14 09:58:08.501171 qtharmony-0.2.7/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2539 2024-05-14 09:58:14.124249 qtharmony-0.2.7/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0      883 2024-05-14 09:58:20.743947 qtharmony-0.2.7/qtharmony/widgets/basic/frame.py
--rw-r--r--   0        0        0     2753 2024-05-14 09:58:26.717009 qtharmony-0.2.7/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3221 2024-05-14 09:58:31.116809 qtharmony-0.2.7/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3811 2024-05-14 09:58:37.846502 qtharmony-0.2.7/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1959 2024-05-14 09:58:45.422824 qtharmony-0.2.7/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     2019 2024-05-14 09:58:50.315935 qtharmony-0.2.7/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.7/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.7/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.7/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.7/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.7/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.7/qtharmony/widgets/basic/styles/frame.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.7/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.7/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.7/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.7/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.7/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.7/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.7/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.7/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.7/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.7/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 qtharmony-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.2.8/README.md
+-rw-r--r--   0        0        0      609 2024-05-14 14:57:06.668881 qtharmony-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.8/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.8/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.8/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.8/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     4435 2024-05-14 07:15:03.814438 qtharmony-0.2.8/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.2.8/qtharmony/resources/themes/dark-green.json
+-rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.8/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.8/qtharmony/resources/themes/light-green.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.8/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.8/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.8/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.8/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.8/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.8/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.8/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.8/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.8/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.8/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.8/qtharmony/src/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.8/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.8/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.8/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     2353 2024-05-14 07:15:03.814438 qtharmony-0.2.8/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.8/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2404 2024-05-14 14:57:06.668881 qtharmony-0.2.8/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2729 2024-05-14 14:57:06.668881 qtharmony-0.2.8/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2572 2024-05-14 14:57:06.668881 qtharmony-0.2.8/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3550 2024-05-14 14:57:06.668881 qtharmony-0.2.8/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2583 2024-05-14 14:57:06.668881 qtharmony-0.2.8/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0      927 2024-05-14 14:57:06.668881 qtharmony-0.2.8/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2797 2024-05-14 14:57:06.672214 qtharmony-0.2.8/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3265 2024-05-14 14:57:06.672214 qtharmony-0.2.8/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3855 2024-05-14 14:57:06.672214 qtharmony-0.2.8/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     2003 2024-05-14 14:57:06.672214 qtharmony-0.2.8/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     2063 2024-05-14 14:57:06.672214 qtharmony-0.2.8/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.8/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.8/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.8/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.8/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.8/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.8/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.8/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.8/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.8/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.8/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.8/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.8/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.8/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.8/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.8/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.8/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 qtharmony-0.2.8/PKG-INFO
```

### Comparing `qtharmony-0.2.7/LICENSE` & `qtharmony-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/README.md` & `qtharmony-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/pyproject.toml` & `qtharmony-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.2.7"
+version = "0.2.8"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.2.7/qtharmony/constructor/initialize.py` & `qtharmony-0.2.8/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.2.8/qtharmony/resources/themes/dark-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/resources/themes/dark-green.json` & `qtharmony-0.2.8/qtharmony/resources/themes/dark-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/resources/themes/light-default.json` & `qtharmony-0.2.8/qtharmony/resources/themes/light-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/resources/themes/light-green.json` & `qtharmony-0.2.8/qtharmony/resources/themes/light-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/resources/ui/Icon.png` & `qtharmony-0.2.8/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/resources/ui/Logo.png` & `qtharmony-0.2.8/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.2.8/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/src/core/dialog.py` & `qtharmony-0.2.8/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/src/core/font.py` & `qtharmony-0.2.8/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/src/core/load.py` & `qtharmony-0.2.8/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/src/core/sizes.py` & `qtharmony-0.2.8/qtharmony/src/core/sizes.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/src/core/stylesheet.py` & `qtharmony-0.2.8/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.2.8/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.2.8/qtharmony/src/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/button.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/button.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     def __init__(
             self, 
             text: Optional[str] = None,
             size: Optional[tuple[int, int]] = None,
             font: Optional["QFont"] = None, 
             *,
+            object_name: str = "button",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None, 
     ) -> None:
         """
         Initializes the PushButton widget with optional text, size, font, and stylesheet.
 
         Args:
@@ -45,15 +46,15 @@
 
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if font is not None: self.setFont(font)
 
-        self.setObjectName("button")
+        self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
             name=self.__class__.__name__, obj_name=f"QPushButton#{self.objectName()}",
             stylesheet=stylesheet
         )
         
         if size is not None: self.setFixedSize(*size)
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/check_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             self,
             text: Optional[str] = None,
             size: Optional[tuple[int, int]] = None,
             is_checkable: bool = True,
             is_checked: bool = False,
             is_disabled: bool = False,
             *,
+            object_name: str = "check-box",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the CheckBox widget with optional text, size, checkability, checked state, disabled state, and stylesheet.
 
         Args:
@@ -48,15 +49,15 @@
         ThemeManager.add_widgets(self)
 
         if size is not None: self.setFixedSize(*size)
         self.setChecked(is_checked)
         self.setCheckable(is_checkable)
         self.setDisabled(is_disabled)
 
-        self.setObjectName("check-box")
+        self.setObjectName(object_name)
         if text is not None:
             self.setText(text)
         
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/check_box.css", 
             name=self.__class__.__name__, obj_name=f"CheckBox#{self.objectName()}",
             stylesheet=stylesheet
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/digital_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     def __init__(
             self, 
             range: tuple[int, int] = (0, 100), 
             size: Optional[tuple[int, int]] = None, 
             font: Optional["QFont"] = None, 
             include_buttons: bool = False,
             *,
+            object_name: str = "digital-entry",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the DigitalEntry widget with optional range, size, font, button inclusion, and stylesheet.
 
         Args:
@@ -46,15 +47,15 @@
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if size is not None: self.setFixedSize(*size)
         if not include_buttons: self.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
         if font is not None: self.setFont(font)
 
-        self.setObjectName("digital-entry")
+        self.setObjectName(object_name)
         self.setRange(*range)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/digital_entry.css", 
             name=self.__class__.__name__, obj_name=f"QSpinBox#{self.objectName()}",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     def __init__(
             self, 
             values: Optional[list[str]] = None, 
             size: Optional[tuple[int, int]] = None,
             font: Optional["QFont"] = None, 
             *,
+            object_name: str = "drop-down-menu",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the DropDownMenu widget with optional values, size, font, and stylesheet.
 
         Args:
@@ -52,15 +53,15 @@
 
         if size is not None: self.setFixedSize(*size)
         self.view().setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         self.__values = []
 
         if values is not None: self.__values = [*values]
         self.addItems(self.__values)
-        self.setObjectName("drop-down-menu")
+        self.setObjectName(object_name)
         if font is not None: self.setFont(font)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/drop_down_menu.css", 
             name=self.__class__.__name__, obj_name=f"QComboBox#{self.objectName()}",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/entry.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     def __init__(
             self, 
             placed: Optional[str] = None, 
             placeholder: Optional[str] = None,
             size: Optional[tuple[int, int]] = None, 
             font: Optional["QFont"] = None, 
             *,
+            object_name: str = "entry",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the Entry widget with optional text, placeholder, size, font, and stylesheet.
 
         Args:
@@ -46,15 +47,15 @@
         ThemeManager.add_widgets(self)
 
         if placed is not None: self.setText(placed)
         if placeholder is not None: self.setPlaceholderText(placeholder)
         if font is not None: self.setFont(font)
         if size is not None: self.setFixedSize(*size)
 
-        self.setObjectName("entry")
+        self.setObjectName(object_name)
         self.setFocusPolicy(Qt.FocusPolicy.WheelFocus)
 
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/entry.css", 
             name=self.__class__.__name__, obj_name=f"QLineEdit#{self.objectName()}",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/frame.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 
 class Frame(QFrame):
 
     def __init__(
             self,
             size: Optional[tuple[int, int]] = None,
             *,
+            object_name: str = "frame",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        self.setObjectName("frame")
+        self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
             name=self.__class__.__name__, obj_name=f"QFrame#{self.objectName()}",
             stylesheet=stylesheet
         )
 
         if size is not None:
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/groups.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     def __init__(
             self,
             title: Optional[str] = None,
             size: Optional[tuple[int, int]] = None,
             orientation: str = "vertical",
             *,
+            object_name: str = "group-box",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the GroupBox widget with optional title and stylesheet.
 
         Args:
@@ -51,15 +52,15 @@
             stylesheet (Optional[str], optional): Custom stylesheet for the group box widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the group box. Defaults to None.
         """
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        self.setObjectName("group-box")
+        self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/group_box.css", 
             name=self.__class__.__name__, obj_name=f"QGroupBox#{self.objectName()}",
             stylesheet=stylesheet
         )
 
         if title is not None: self.setTitle(title)
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/label.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             font_family: str, 
             font_size: int,
             bold: bool = False,
             italic: bool = False,
             color: Optional[str] = None,
             word_wrap: bool = False,
             *,
+            object_name: str = "label",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the Label widget with optional text, font family, font size, bold, italic, color, word wrap, and stylesheet.
 
         Args:
@@ -50,15 +51,15 @@
             stylesheet (Optional[str], optional): Custom stylesheet for the label widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the label. Defaults to None.
         """
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        self.setObjectName("label")
+        self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/label.css", 
             name=self.__class__.__name__, obj_name=f"QLabel#{self.objectName()}",
             stylesheet=stylesheet
         )
 
         self.setText(text)
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/path_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     def __init__(
             self, 
             placed: Optional[str] = None, 
             placeholder: Optional[str] = None,
             size: Optional[tuple[int, int]] = None, 
             font: Optional["QFont"] = None, 
             *,
+            object_name: str = "path-entry",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the PathEntry widget with path input functionality.
 
         Args:
@@ -49,15 +50,15 @@
             font (Optional["QFont"], optional): The font to be used for text input. Defaults to None.
             stylesheet (Optional[str], optional): Custom stylesheet for the path entry widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the path entry. Defaults to None.
         """        
 
         super().__init__(parent)
 
-        self.setObjectName("path-entry")
+        self.setObjectName(object_name)
         if font is not None: self.setFont(font)
 
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/path_entry.css", 
             name=self.__class__.__name__, obj_name=f"QWidget#{self.objectName()}",
             stylesheet=stylesheet
         ))
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/radio_button.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     """
 
     def __init__(
             self,
             text: Optional[str] = None,
             size: Optional[tuple[int, int]] = None,
             *,
+            object_name: str = "radio-button",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the RadioButton widget with optional text, size, and stylesheet.
 
         Args:
@@ -39,13 +40,13 @@
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if text is not None: self.setText(text)
         if size is not None: self.setFixedSize(*size)
 
-        self.setObjectName("radio-button")
+        self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/radio_button.css", 
             name=self.__class__.__name__, obj_name=f"QRadioButton#{self.objectName()}",
             stylesheet=stylesheet
         )
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/splitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     - addWidget(widget): None - Adds a widget to the splitter and sets it as non-collapsible.
     """
 
     def __init__(
             self, 
             __orientation: str,
             *,
+            object_name: str = "splitter",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the Splitter instance with the specified orientation.
 
         Args:
@@ -35,15 +36,15 @@
         """
 
         if __orientation == "horizontal": super().__init__(Qt.Orientation.Horizontal, parent)
         elif __orientation == "vertical": super().__init__(Qt.Orientation.Vertical, parent)
 
         ThemeManager.add_widgets(self)
 
-        self.setObjectName("splitter")
+        self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/splitter.css", 
             name=self.__class__.__name__, obj_name=f"QSplitter#{self.objectName()}",
             stylesheet=stylesheet
         )
 
     def addWidget(self, widget):
```

### Comparing `qtharmony-0.2.7/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.2.8/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/qtharmony/windows/main_window.py` & `qtharmony-0.2.8/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.7/PKG-INFO` & `qtharmony-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.2.7
+Version: 0.2.8
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

