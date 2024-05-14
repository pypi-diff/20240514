# Comparing `tmp/amiami-0.0.8.tar.gz` & `tmp/amiami-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amiami-0.0.8.tar", last modified: Mon Oct 31 15:33:34 2022, max compression
+gzip compressed data, was "amiami-0.0.9.tar", last modified: Tue Aug  1 06:19:55 2023, max compression
```

## Comparing `amiami-0.0.8.tar` & `amiami-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2022-10-31 15:33:34.815749 amiami-0.0.8/
--rw-r--r--   0 batmanuel   (501) staff       (20)     1066 2022-10-20 16:14:22.000000 amiami-0.0.8/LICENSE
--rw-r--r--   0 batmanuel   (501) staff       (20)       43 2022-10-21 03:31:24.000000 amiami-0.0.8/MANIFEST.in
--rw-r--r--   0 batmanuel   (501) staff       (20)      882 2022-10-31 15:33:34.815622 amiami-0.0.8/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)      545 2022-10-20 16:14:22.000000 amiami-0.0.8/README.md
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2022-10-31 15:33:34.814996 amiami-0.0.8/amiami/
--rw-r--r--   0 batmanuel   (501) staff       (20)       27 2022-10-20 16:14:22.000000 amiami-0.0.8/amiami/__init__.py
--rw-r--r--   0 batmanuel   (501) staff       (20)     4325 2022-10-31 15:32:40.000000 amiami-0.0.8/amiami/amiami.py
--rw-r--r--   0 batmanuel   (501) staff       (20)     3171 2022-10-31 15:17:43.000000 amiami-0.0.8/amiami/test.py
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2022-10-31 15:33:34.815480 amiami-0.0.8/amiami.egg-info/
--rw-r--r--   0 batmanuel   (501) staff       (20)      882 2022-10-31 15:33:34.000000 amiami-0.0.8/amiami.egg-info/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)      255 2022-10-31 15:33:34.000000 amiami-0.0.8/amiami.egg-info/SOURCES.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)        1 2022-10-31 15:33:34.000000 amiami-0.0.8/amiami.egg-info/dependency_links.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)      158 2022-10-31 15:33:34.000000 amiami-0.0.8/amiami.egg-info/requires.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)        7 2022-10-31 15:33:34.000000 amiami-0.0.8/amiami.egg-info/top_level.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)      158 2022-10-21 03:08:48.000000 amiami-0.0.8/requirements.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)       38 2022-10-31 15:33:34.815786 amiami-0.0.8/setup.cfg
--rw-r--r--   0 batmanuel   (501) staff       (20)      624 2022-10-31 15:32:59.000000 amiami-0.0.8/setup.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-08-01 06:19:55.864313 amiami-0.0.9/
+-rw-r--r--   0 batmanuel   (501) staff       (20)     1066 2022-10-20 16:14:22.000000 amiami-0.0.9/LICENSE
+-rw-r--r--   0 batmanuel   (501) staff       (20)       43 2022-10-21 03:31:24.000000 amiami-0.0.9/MANIFEST.in
+-rw-r--r--   0 batmanuel   (501) staff       (20)      884 2023-08-01 06:19:55.864200 amiami-0.0.9/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)      547 2023-08-01 06:16:26.000000 amiami-0.0.9/README.md
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-08-01 06:19:55.863245 amiami-0.0.9/amiami/
+-rw-r--r--   0 batmanuel   (501) staff       (20)       27 2022-10-20 16:14:22.000000 amiami-0.0.9/amiami/__init__.py
+-rw-r--r--   0 batmanuel   (501) staff       (20)     4577 2023-08-01 06:14:54.000000 amiami-0.0.9/amiami/amiami.py
+-rw-r--r--   0 batmanuel   (501) staff       (20)     3171 2022-10-31 15:17:43.000000 amiami-0.0.9/amiami/test.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-08-01 06:19:55.864048 amiami-0.0.9/amiami.egg-info/
+-rw-r--r--   0 batmanuel   (501) staff       (20)      884 2023-08-01 06:19:55.000000 amiami-0.0.9/amiami.egg-info/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)      255 2023-08-01 06:19:55.000000 amiami-0.0.9/amiami.egg-info/SOURCES.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)        1 2023-08-01 06:19:55.000000 amiami-0.0.9/amiami.egg-info/dependency_links.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       46 2023-08-01 06:19:55.000000 amiami-0.0.9/amiami.egg-info/requires.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)        7 2023-08-01 06:19:55.000000 amiami-0.0.9/amiami.egg-info/top_level.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       46 2023-08-01 06:16:04.000000 amiami-0.0.9/requirements.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       38 2023-08-01 06:19:55.864355 amiami-0.0.9/setup.cfg
+-rw-r--r--   0 batmanuel   (501) staff       (20)      624 2023-08-01 06:16:34.000000 amiami-0.0.9/setup.py
```

### Comparing `amiami-0.0.8/LICENSE` & `amiami-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amiami-0.0.8/PKG-INFO` & `amiami-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amiami
-Version: 0.0.8
+Version: 0.0.9
 Summary: amiami api wrapper
 Home-page: https://bitbucket.org/marvinody/amiami/
 Author: marvinody
 Author-email: manny@amiami.sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -18,14 +18,14 @@
 Simple usage can be something like
 
 ```python
 import amiami
 
 results = amiami.search("fumofumo plush")
 for item in results.items:
-  print("{}, {}".format(item.productName, item.productURL))
+  print("{}, {}".format(item.productName, item.availability))
 ```
 
 
 Sometimes items tend to result in an unknown status because the flag -> state parsing is a bit rough. These items will be added to the list with a status of `Unknown status?`. They will also print out a message with the flags and item code. Good to check your log and see what's going on.
```

### Comparing `amiami-0.0.8/README.md` & `amiami-0.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 Simple usage can be something like
 
 ```python
 import amiami
 
 results = amiami.search("fumofumo plush")
 for item in results.items:
-  print("{}, {}".format(item.productName, item.productURL))
+  print("{}, {}".format(item.productName, item.availability))
 ```
 
 
 Sometimes items tend to result in an unknown status because the flag -> state parsing is a bit rough. These items will be added to the list with a status of `Unknown status?`. They will also print out a message with the flags and item code. Good to check your log and see what's going on.
```

### Comparing `amiami-0.0.8/amiami/amiami.py` & `amiami-0.0.9/amiami/amiami.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import httpx
 from math import ceil
+# import logging
+from curl_cffi import requests
+
 
 rootURL = "https://api.amiami.com/api/v1.0/items"
 PER_PAGE = 30
 
 class Item:
     def __init__(self, *args, **kwargs):
         self.productURL = kwargs['productURL']
@@ -96,28 +98,34 @@
             self.init = True
         for productInfo in obj['items']:
             self.add(productInfo)
             self._itemCount += 1
 
         return self._itemCount == self.maxItems
 
+# leaving this here because I need it every time some shit breaks and don't wanna dig it up
+# logging.basicConfig(
+#     format="%(levelname)s [%(asctime)s] %(name)s - %(message)s",
+#     datefmt="%Y-%m-%d %H:%M:%S",
+#     level=logging.DEBUG
+# )
+
 def search(keywords):
     data = {
         "s_keywords": keywords,
         "pagecnt": 1,
         "pagemax": PER_PAGE,
         "lang": "eng",
     }
     headers = {
         "X-User-Key": "amiami_dev",
         "User-Agent": "python-amiami_dev",
     }
 
-    with httpx.Client() as client:
-        rs = ResultSet()
-        hasMore = True
-        while hasMore:
-            resp = client.get(rootURL, params=data, headers=headers)
-            hasMore = not rs.parse(resp.json())
-            data['pagecnt'] += 1
+    rs = ResultSet()
+    hasMore = True
+    while hasMore:
+        resp = requests.get(rootURL, params=data, headers=headers, impersonate="chrome110")
+        hasMore = not rs.parse(resp.json())
+        data['pagecnt'] += 1
 
     return rs
```

### Comparing `amiami-0.0.8/amiami/test.py` & `amiami-0.0.9/amiami/test.py`

 * *Files identical despite different names*

### Comparing `amiami-0.0.8/amiami.egg-info/PKG-INFO` & `amiami-0.0.9/amiami.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amiami
-Version: 0.0.8
+Version: 0.0.9
 Summary: amiami api wrapper
 Home-page: https://bitbucket.org/marvinody/amiami/
 Author: marvinody
 Author-email: manny@amiami.sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -18,14 +18,14 @@
 Simple usage can be something like
 
 ```python
 import amiami
 
 results = amiami.search("fumofumo plush")
 for item in results.items:
-  print("{}, {}".format(item.productName, item.productURL))
+  print("{}, {}".format(item.productName, item.availability))
 ```
 
 
 Sometimes items tend to result in an unknown status because the flag -> state parsing is a bit rough. These items will be added to the list with a status of `Unknown status?`. They will also print out a message with the flags and item code. Good to check your log and see what's going on.
```

### Comparing `amiami-0.0.8/setup.py` & `amiami-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='amiami',
-    version='0.0.8',
+    version='0.0.9',
     author='marvinody',
     author_email='manny@amiami.sadpanda.moe',
     description='amiami api wrapper',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/marvinody/amiami/',
     packages=setuptools.find_packages(),
```

