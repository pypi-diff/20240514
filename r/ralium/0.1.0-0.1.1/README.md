# Comparing `tmp/ralium-0.1.0.tar.gz` & `tmp/ralium-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-0.1.0.tar", last modified: Tue May 14 03:35:33 2024, max compression
+gzip compressed data, was "ralium-0.1.1.tar", last modified: Tue May 14 05:16:12 2024, max compression
```

## Comparing `ralium-0.1.0.tar` & `ralium-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:35:33.198647 ralium-0.1.0/
--rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-14 03:35:33.197643 ralium-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.1.0/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-14 03:33:08.000000 ralium-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-14 03:35:33.173797 ralium-0.1.0/ralium/
--rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.1.0/ralium/__init__.py
--rw-rw-rw-   0        0        0     1705 2024-05-13 23:26:15.000000 ralium-0.1.0/ralium/_util.py
--rw-rw-rw-   0        0        0      583 2024-05-14 03:28:18.000000 ralium-0.1.0/ralium/_util.pyi
--rw-rw-rw-   0        0        0     6366 2024-05-13 23:30:11.000000 ralium-0.1.0/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.1.0/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.1.0/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.1.0/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.1.0/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.1.0/ralium/config.pyi
--rw-rw-rw-   0        0        0     6270 2024-05-14 03:20:18.000000 ralium-0.1.0/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-14 03:29:32.000000 ralium-0.1.0/ralium/element.pyi
--rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.1.0/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.1.0/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1040 2024-05-13 22:41:14.000000 ralium-0.1.0/ralium/errors.py
--rw-rw-rw-   0        0        0      733 2024-05-13 22:32:57.000000 ralium-0.1.0/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.1.0/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.1.0/ralium/setup.py
--rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.1.0/ralium/setup.pyi
--rw-rw-rw-   0        0        0     5747 2024-05-13 23:30:09.000000 ralium-0.1.0/ralium/webpage.py
--rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.1.0/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     5129 2024-05-14 03:24:57.000000 ralium-0.1.0/ralium/window.py
--rw-rw-rw-   0        0        0      613 2024-05-14 03:24:04.000000 ralium-0.1.0/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-14 03:35:33.196224 ralium-0.1.0/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-14 03:35:33.000000 ralium-0.1.0/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2024-05-14 03:35:33.000000 ralium-0.1.0/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:35:33.000000 ralium-0.1.0/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-14 03:35:33.000000 ralium-0.1.0/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 03:35:33.000000 ralium-0.1.0/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 03:35:33.198647 ralium-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 05:16:12.620892 ralium-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-14 05:16:12.619888 ralium-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1018 2024-05-14 05:15:48.000000 ralium-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-14 05:16:12.599876 ralium-0.1.1/ralium/
+-rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.1.1/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1705 2024-05-13 23:26:15.000000 ralium-0.1.1/ralium/_util.py
+-rw-rw-rw-   0        0        0      583 2024-05-14 05:14:09.000000 ralium-0.1.1/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     6366 2024-05-13 23:30:11.000000 ralium-0.1.1/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.1.1/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.1.1/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.1.1/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.1.1/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.1.1/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.1.1/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.1.1/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.1.1/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.1.1/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1040 2024-05-13 22:41:14.000000 ralium-0.1.1/ralium/errors.py
+-rw-rw-rw-   0        0        0      733 2024-05-13 22:32:57.000000 ralium-0.1.1/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.1.1/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.1.1/ralium/setup.py
+-rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.1.1/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     5747 2024-05-13 23:30:09.000000 ralium-0.1.1/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.1.1/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     5129 2024-05-14 05:14:09.000000 ralium-0.1.1/ralium/window.py
+-rw-rw-rw-   0        0        0      613 2024-05-14 05:14:09.000000 ralium-0.1.1/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-14 05:16:12.618429 ralium-0.1.1/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-14 05:16:12.000000 ralium-0.1.1/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2024-05-14 05:16:12.000000 ralium-0.1.1/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 05:16:12.000000 ralium-0.1.1/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-14 05:16:12.000000 ralium-0.1.1/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 05:16:12.000000 ralium-0.1.1/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 05:16:12.620892 ralium-0.1.1/setup.cfg
```

### Comparing `ralium-0.1.0/LICENSE` & `ralium-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/PKG-INFO` & `ralium-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.1.0/pyproject.toml` & `ralium-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "0.1.0"
+version = "0.1.1"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-0.1.0/ralium/_util.py` & `ralium-0.1.1/ralium/_util.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/_util.pyi` & `ralium-0.1.1/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/api.py` & `ralium-0.1.1/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/api.pyi` & `ralium-0.1.1/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/builtins.py` & `ralium-0.1.1/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/builtins.pyi` & `ralium-0.1.1/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/config.py` & `ralium-0.1.1/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/element.py` & `ralium-0.1.1/ralium/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,14 @@
         return self._parse(self._eval(f"{self._as_js_str()}.{identifier}"))
     
     def __setattr__(self, identifier, value):
         if identifier in HTMLElementAttributes:
             return object.__setattr__(self, identifier, value)
 
         self._eval(f"{self._get_js_element()}.{identifier} = {value};")
-        print(identifier, self._eval(f"{self._as_js_str()}.{identifier}"))
     
     def _get_js_element(self):
         return f"document.getElementsByClassName('{self._ralium_id}')[0]"
     
     def _as_js_str(self):
         return f"'' + {self._get_js_element()}"
```

### Comparing `ralium-0.1.0/ralium/element.pyi` & `ralium-0.1.1/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/engine.py` & `ralium-0.1.1/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/engine.pyi` & `ralium-0.1.1/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/errors.py` & `ralium-0.1.1/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/navigation.py` & `ralium-0.1.1/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/setup.py` & `ralium-0.1.1/ralium/setup.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/setup.pyi` & `ralium-0.1.1/ralium/setup.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/webpage.py` & `ralium-0.1.1/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/webpage.pyi` & `ralium-0.1.1/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/window.py` & `ralium-0.1.1/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium/window.pyi` & `ralium-0.1.1/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.1.0/ralium.egg-info/PKG-INFO` & `ralium-0.1.1/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.1.0/ralium.egg-info/SOURCES.txt` & `ralium-0.1.1/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

