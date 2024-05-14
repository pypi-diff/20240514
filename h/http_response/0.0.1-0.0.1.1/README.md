# Comparing `tmp/http_response-0.0.1.tar.gz` & `tmp/http_response-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_response-0.0.1.tar", max compression
+gzip compressed data, was "http_response-0.0.1.1.tar", max compression
```

## Comparing `http_response-0.0.1.tar` & `http_response-0.0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 http_response-0.0.1/LICENSE
--rw-r--r--   0        0        0     3214 2024-05-02 13:48:22.655187 http_response-0.0.1/http_response/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 http_response-0.0.1/http_response/py.typed
--rw-r--r--   0        0        0     1153 2024-05-02 13:47:38.312653 http_response-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-02 13:46:45.898090 http_response-0.0.1/readme.md
--rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 http_response-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 http_response-0.0.1.1/LICENSE
+-rw-r--r--   0        0        0     3304 2024-05-14 13:52:22.523060 http_response-0.0.1.1/http_response/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 http_response-0.0.1.1/http_response/py.typed
+-rw-r--r--   0        0        0     1155 2024-05-14 13:53:46.121878 http_response-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-02 13:46:45.898090 http_response-0.0.1.1/readme.md
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 http_response-0.0.1.1/PKG-INFO
```

### Comparing `http_response-0.0.1/LICENSE` & `http_response-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `http_response-0.0.1/http_response/__init__.py` & `http_response-0.0.1.1/http_response/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     if hdr_cd and hdr_cd.startswith("attachment; filename="):
         filename = hdr_cd[21:]
         if filename.startswith(("'", '"')):
             filename = filename[1:-1]
         elif filename.startswith(" "):
             filename = filename[1:]
         return unquote(filename)
-    urlp = urlsplit(response.url)
+    url = response.url
+    if not isinstance(url, (bytearray, bytes, str)):
+        url = str(url)
+    urlp = urlsplit(url)
     filename = basename(unquote(urlp.path)) or default
     if filename:
         if guess_type(filename)[0]:
             return filename
         try:
             hdr_ct = response.headers["content-type"]
         except KeyError:
```

### Comparing `http_response-0.0.1/pyproject.toml` & `http_response-0.0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "http_response"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Python http response utils."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/http_response"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/http_response"
 keywords = ["http", "response"]
```

### Comparing `http_response-0.0.1/PKG-INFO` & `http_response-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http_response
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Python http response utils.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/http_response
 License: MIT
 Keywords: http,response
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

