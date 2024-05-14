# Comparing `tmp/ralium-0.1.2.tar.gz` & `tmp/ralium-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-0.1.2.tar", last modified: Tue May 14 07:04:08 2024, max compression
+gzip compressed data, was "ralium-0.1.3.tar", last modified: Tue May 14 21:36:14 2024, max compression
```

## Comparing `ralium-0.1.2.tar` & `ralium-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 07:04:08.455328 ralium-0.1.2/
--rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-14 07:04:08.454159 ralium-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.1.2/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-14 07:02:56.000000 ralium-0.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-14 07:04:08.433828 ralium-0.1.2/ralium/
--rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.1.2/ralium/__init__.py
--rw-rw-rw-   0        0        0     1705 2024-05-13 23:26:15.000000 ralium-0.1.2/ralium/_util.py
--rw-rw-rw-   0        0        0      583 2024-05-14 05:14:09.000000 ralium-0.1.2/ralium/_util.pyi
--rw-rw-rw-   0        0        0     6366 2024-05-13 23:30:11.000000 ralium-0.1.2/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.1.2/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.1.2/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.1.2/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.1.2/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.1.2/ralium/config.pyi
--rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.1.2/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.1.2/ralium/element.pyi
--rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.1.2/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.1.2/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1040 2024-05-13 22:41:14.000000 ralium-0.1.2/ralium/errors.py
--rw-rw-rw-   0        0        0      733 2024-05-13 22:32:57.000000 ralium-0.1.2/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.1.2/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.1.2/ralium/setup.py
--rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.1.2/ralium/setup.pyi
--rw-rw-rw-   0        0        0     5747 2024-05-13 23:30:09.000000 ralium-0.1.2/ralium/webpage.py
--rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.1.2/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     5139 2024-05-14 07:02:07.000000 ralium-0.1.2/ralium/window.py
--rw-rw-rw-   0        0        0      613 2024-05-14 05:14:09.000000 ralium-0.1.2/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-14 07:04:08.451851 ralium-0.1.2/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-14 07:04:08.000000 ralium-0.1.2/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2024-05-14 07:04:08.000000 ralium-0.1.2/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 07:04:08.000000 ralium-0.1.2/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-14 07:04:08.000000 ralium-0.1.2/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 07:04:08.000000 ralium-0.1.2/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 07:04:08.455328 ralium-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 21:36:14.764676 ralium-0.1.3/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-14 21:36:14.763357 ralium-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1018 2024-05-14 21:34:14.000000 ralium-0.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-14 21:36:14.731844 ralium-0.1.3/ralium/
+-rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.1.3/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1796 2024-05-14 21:30:36.000000 ralium-0.1.3/ralium/_util.py
+-rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.1.3/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     6357 2024-05-14 21:33:41.000000 ralium-0.1.3/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.1.3/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.1.3/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.1.3/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.1.3/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.1.3/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.1.3/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.1.3/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.1.3/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.1.3/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1040 2024-05-13 22:41:14.000000 ralium-0.1.3/ralium/errors.py
+-rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.1.3/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.1.3/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.1.3/ralium/setup.py
+-rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.1.3/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.1.3/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.1.3/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     5139 2024-05-14 07:02:07.000000 ralium-0.1.3/ralium/window.py
+-rw-rw-rw-   0        0        0      613 2024-05-14 05:14:09.000000 ralium-0.1.3/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-14 21:36:14.761868 ralium-0.1.3/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-14 21:36:14.000000 ralium-0.1.3/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2024-05-14 21:36:14.000000 ralium-0.1.3/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:36:14.000000 ralium-0.1.3/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-14 21:36:14.000000 ralium-0.1.3/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 21:36:14.000000 ralium-0.1.3/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:36:14.764676 ralium-0.1.3/setup.cfg
```

### Comparing `ralium-0.1.2/LICENSE` & `ralium-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/PKG-INFO` & `ralium-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.1.2/pyproject.toml` & `ralium-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "0.1.2"
+version = "0.1.3"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-0.1.2/ralium/_util.py` & `ralium-0.1.3/ralium/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 import platform
 import ctypes
 import winreg
 import sys
 import os
 
-__all__ = ["BasicHTTPServer", "_get_path_limit", "_get_path", "_is_markup_filelike"]
+__all__ = ["BasicHTTPServer", "_norm_url", "_get_path_limit", "_get_path", "_is_markup_filelike"]
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
+def _norm_url(path):
+    return os.path.normpath(path).replace("\\", "/")
+
 def _get_path_limit_winreg():
     with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, r"SYSTEM\CurrentControlSet\Control\FileSystem") as key:
         max_path_length, _ = winreg.QueryValueEx(key, "LongPathsEnabled")
         return max_path_length
 
 def _get_path_limit():
     system = platform.system()
```

### Comparing `ralium-0.1.2/ralium/_util.pyi` & `ralium-0.1.3/ralium/_util.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import TypeAlias, TypeVar, Callable, Any, Self, Literal
 from types import FunctionType, ModuleType
 import http.server
 
-__all__ = ["BasicHTTPServer", "_get_path_limit", "_get_path", "_is_markup_filelike"]
+__all__ = ["BasicHTTPServer", "_norm_url", "_get_path_limit", "_get_path", "_is_markup_filelike"]
 
 _RT = TypeVar("_RT") # Return Type
 ClassType: TypeAlias = object
 DirPathStr: TypeAlias = str
 FilePathStr: TypeAlias = str
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler): ...
 
+def _norm_url(path: str) -> str: ...
 def _get_path_limit_winreg() -> int: ...
 def _get_path_limit() -> int: ...
 def _get_path(path: str) -> str: ...
 def _is_markup_filelike(markup: str) -> bool: ...
```

### Comparing `ralium-0.1.2/ralium/api.py` & `ralium-0.1.3/ralium/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ralium.webpage import WebHook, WebHookNamespace
 from ralium.config import WindowConfig
 from ralium.window import Window
 from ralium.errors import *
-from ralium._util import _get_path
+from ralium._util import _get_path, _norm_url
 
 from types import FunctionType, MethodType
 
 import inspect
 import os
 
 RALIUM_API_REGISTRY_IDENTIFIER = "__ralium_registry__"
@@ -46,15 +46,15 @@
 
 def _collect_webhooks(webfolder, webroutes):
     webhooks = []
     global_css = _collect_global_css_files(webfolder)
     root_split_string = os.path.join(os.path.basename(webfolder), "routes")
 
     for root, _, files in os.walk(webroutes):
-        url = f"/{root.split(root_split_string)[-1].strip("\\").replace("\\", "/")}"
+        url = _norm_url(f"/{root.split(root_split_string)[-1]}")
 
         if not files: 
             continue
 
         css = [*global_css]
         html = None
         functions = []
```

### Comparing `ralium-0.1.2/ralium/api.pyi` & `ralium-0.1.3/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/builtins.py` & `ralium-0.1.3/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/builtins.pyi` & `ralium-0.1.3/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/config.py` & `ralium-0.1.3/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/element.py` & `ralium-0.1.3/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/element.pyi` & `ralium-0.1.3/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/engine.py` & `ralium-0.1.3/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/engine.pyi` & `ralium-0.1.3/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/errors.py` & `ralium-0.1.3/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/navigation.py` & `ralium-0.1.3/ralium/navigation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from ralium._util import _norm_url
+
 class WindowNavigation:
     """
     The Window Navigation Manager.
 
     :param current_url: The url to initially display.
     """
 
     def __init__(self, current_url = "/"):
         self.__homepage = None
         self.__previous = None
-        self.__location = current_url
+        self.__location = _norm_url(current_url)
 
     def setdefault(self, url):
         """Sets the homepage."""
-        self.__homepage = url
+        self.__homepage = _norm_url(url)
     
     @property
     def homepage(self):
         return self.__homepage
 
     @property
     def previous(self):
@@ -25,8 +27,8 @@
     @property
     def location(self):
         return self.__location
 
     @location.setter
     def location(self, new_url):
         self.__previous = None
-        self.__location = new_url
+        self.__location = _norm_url(new_url)
```

### Comparing `ralium-0.1.2/ralium/setup.py` & `ralium-0.1.3/ralium/setup.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/setup.pyi` & `ralium-0.1.3/ralium/setup.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/webpage.py` & `ralium-0.1.3/ralium/webpage.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     :param encoding: The file encoding of the HTML and CSS files.
 
     :raises FileNotFoundWarning: Displays a warning if a file doesn't exist. (Only if warnings are enabled.)
     :raises FilePathLimitError: If a path exceeds the system limit for path lengths.
     """
 
     def __init__(self, url, html, css = None, functions = None, namespaces = None, homepage = False, encoding = "UTF-8"):
-        self.url = url
+        self.url = _norm_url(url)
         self.css = css or ""
         self.html = html
         self.window = None
         self.elements = []
         self.homepage = homepage
         self.encoding = encoding
         self.functions = functions
@@ -140,17 +140,15 @@
             return
         
         for namespace in self.namespaces:
             for key in namespace.keys():
                 namespace[key] = WebHookFunction(namespace[key], self.window)
 
     def set_window(self, window):
-        """
-        Sets the window of the WebHook.
-        """
+        """Sets the window of the WebHook."""
         self.window = window
 
 class WebHookDict(dict):
     def __init__(self, webhooks):
         for webhook in webhooks:
             self[webhook.url] = webhook
```

### Comparing `ralium-0.1.2/ralium/webpage.pyi` & `ralium-0.1.3/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/window.py` & `ralium-0.1.3/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium/window.pyi` & `ralium-0.1.3/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.2/ralium.egg-info/PKG-INFO` & `ralium-0.1.3/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.1.2/ralium.egg-info/SOURCES.txt` & `ralium-0.1.3/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

