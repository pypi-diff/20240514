# Comparing `tmp/tarsier-0.5.94.tar.gz` & `tmp/tarsier-0.5.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarsier-0.5.94.tar", max compression
+gzip compressed data, was "tarsier-0.5.941.tar", max compression
```

## Comparing `tarsier-0.5.94.tar` & `tarsier-0.5.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-11 23:43:10.265367 tarsier-0.5.94/LICENSE
--rw-r--r--   0        0        0     5763 2024-04-11 23:43:10.265367 tarsier-0.5.94/README.md
--rw-r--r--   0        0        0     1392 2024-04-11 23:43:10.269367 tarsier-0.5.94/pyproject.toml
--rw-r--r--   0        0        0      115 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/__init__.py
--rw-r--r--   0        0        0     1575 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/__main__.py
--rw-r--r--   0        0        0      348 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/_utils.py
--rw-r--r--   0        0        0     1029 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/adapter/__init__.py
--rw-r--r--   0        0        0      488 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/adapter/_base.py
--rw-r--r--   0        0        0     2154 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/adapter/playwright.py
--rw-r--r--   0        0        0      941 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/adapter/selenium.py
--rw-r--r--   0        0        0      334 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/adapter/types.py
--rw-r--r--   0        0        0     2780 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/core.py
--rw-r--r--   0        0        0      180 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/ocr/__init__.py
--rw-r--r--   0        0        0     2617 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/ocr/ocr_service.py
--rw-r--r--   0        0        0      490 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/ocr/types.py
--rw-r--r--   0        0        0        0 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/py.typed
--rw-r--r--   0        0        0     5723 2024-04-11 23:43:18.213367 tarsier-0.5.94/tarsier/tag_utils.min.js
--rw-r--r--   0        0        0     8688 2024-04-11 23:43:11.693366 tarsier-0.5.94/tarsier/text_format.py
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 tarsier-0.5.94/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-14 05:19:45.094610 tarsier-0.5.941/LICENSE
+-rw-r--r--   0        0        0     5763 2024-05-14 05:19:45.094610 tarsier-0.5.941/README.md
+-rw-r--r--   0        0        0     1393 2024-05-14 05:19:45.098610 tarsier-0.5.941/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/__init__.py
+-rw-r--r--   0        0        0     1575 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/__main__.py
+-rw-r--r--   0        0        0      348 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/_utils.py
+-rw-r--r--   0        0        0     1029 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/adapter/__init__.py
+-rw-r--r--   0        0        0      488 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/adapter/_base.py
+-rw-r--r--   0        0        0     2154 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/adapter/playwright.py
+-rw-r--r--   0        0        0      941 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/adapter/selenium.py
+-rw-r--r--   0        0        0      334 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/adapter/types.py
+-rw-r--r--   0        0        0     2780 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/core.py
+-rw-r--r--   0        0        0      180 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/ocr/__init__.py
+-rw-r--r--   0        0        0     2617 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/ocr/ocr_service.py
+-rw-r--r--   0        0        0      490 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/ocr/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/py.typed
+-rw-r--r--   0        0        0     5699 2024-05-14 05:19:51.158609 tarsier-0.5.941/tarsier/tag_utils.min.js
+-rw-r--r--   0        0        0     8688 2024-05-14 05:19:46.510610 tarsier-0.5.941/tarsier/text_format.py
+-rw-r--r--   0        0        0     6249 1970-01-01 00:00:00.000000 tarsier-0.5.941/PKG-INFO
```

### Comparing `tarsier-0.5.94/LICENSE` & `tarsier-0.5.941/LICENSE`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/README.md` & `tarsier-0.5.941/README.md`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/pyproject.toml` & `tarsier-0.5.941/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tarsier"
-version = "0.5.94"
+version = "0.5.941"
 description = "Vision utilities for web interaction agents"
 authors = ["Rohan Pandey", "Adam Watkins", "Asim Shrestha"]
 readme = "README.md"
 include = ["tarsier/**/*.min.js"]
 exclude = ["tarsier/**/*.ts", "tarsier_snapshots", "tarsier_snapshots/*"]
```

### Comparing `tarsier-0.5.94/tarsier/__main__.py` & `tarsier-0.5.941/tarsier/__main__.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/tarsier/adapter/__init__.py` & `tarsier-0.5.941/tarsier/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/tarsier/adapter/playwright.py` & `tarsier-0.5.941/tarsier/adapter/playwright.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/tarsier/adapter/selenium.py` & `tarsier-0.5.941/tarsier/adapter/selenium.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/tarsier/core.py` & `tarsier-0.5.941/tarsier/core.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/tarsier/ocr/ocr_service.py` & `tarsier-0.5.941/tarsier/ocr/ocr_service.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/tarsier/tag_utils.min.js` & `tarsier-0.5.941/tarsier/tag_utils.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -63,15 +63,15 @@
     return n + "//" + i.join("/")
 }
 
 function create_tagged_span(t, i) {
     let n;
     isInteractable(i) ? isTextInsertable(i) ? n = `[#${t}]` : i.tagName.toLowerCase() == "a" ? n = `[@${t}]` : n = `[$${t}]` : n = `[${t}]`;
     let e = document.createElement("span");
-    return e.id = tarsierId, e.style.position = "relative", e.style.display = "inline", e.style.color = "white", e.style.backgroundColor = "red", e.style.padding = "1.5px", e.style.borderRadius = "3px", e.style.fontWeight = "bold", e.style.fontSize = "15px", e.style.fontFamily = "Arial", e.style.margin = "1px", e.style.lineHeight = "1.25", e.style.letterSpacing = "2px", e.style.zIndex = "2140000046", e.style.clip = "auto", e.style.height = "fit-content", e.style.width = "fit-content", e.style.minHeight = "fit-content", e.style.minWidth = "fit-content", e.style.maxHeight = "unset", e.style.maxWidth = "unset", e.textContent = n, e.style.webkitTextFillColor = "white", e.style.textShadow = "", e.style.textDecoration = "none", e
+    return e.id = tarsierId, e.style.position = "relative", e.style.display = "inline", e.style.color = "white", e.style.backgroundColor = "red", e.style.padding = "1.5px", e.style.borderRadius = "3px", e.style.fontWeight = "bold", e.style.fontFamily = "Arial", e.style.margin = "1px", e.style.lineHeight = "1.25", e.style.letterSpacing = "2px", e.style.zIndex = "2140000046", e.style.clip = "auto", e.style.height = "fit-content", e.style.width = "fit-content", e.style.minHeight = "fit-content", e.style.minWidth = "fit-content", e.style.maxHeight = "unset", e.style.maxWidth = "unset", e.textContent = n, e.style.webkitTextFillColor = "white", e.style.textShadow = "", e.style.textDecoration = "none", e
 }
 window.tagifyWebpage = (t = !1) => {
     window.removeTags(), hideMapElements();
     let i = 0,
         n = {},
         e = [...document.body.querySelectorAll("*")];
     const s = document.getElementsByTagName("iframe");
```

### Comparing `tarsier-0.5.94/tarsier/text_format.py` & `tarsier-0.5.941/tarsier/text_format.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.94/PKG-INFO` & `tarsier-0.5.941/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarsier
-Version: 0.5.94
+Version: 0.5.941
 Summary: Vision utilities for web interaction agents
 Author: Rohan Pandey
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: google-cloud-vision (>=3.4.5,<4.0.0)
```

