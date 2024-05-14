# Comparing `tmp/pyrippleapi-2024.5.1.tar.gz` & `tmp/pyrippleapi-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrippleapi-2024.5.1.tar", last modified: Mon May 13 13:47:27 2024, max compression
+gzip compressed data, was "pyrippleapi-2024.5.2.tar", last modified: Mon May 13 14:18:53 2024, max compression
```

## Comparing `pyrippleapi-2024.5.1.tar` & `pyrippleapi-2024.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.746620 pyrippleapi-2024.5.1/
--rw-rw-rw-   0        0        0      418 2024-05-13 13:47:27.747619 pyrippleapi-2024.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2024.5.1/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2024.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       85 2024-05-13 13:47:27.756622 pyrippleapi-2024.5.1/setup.cfg
--rw-rw-rw-   0        0        0      817 2024-05-13 13:47:20.000000 pyrippleapi-2024.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.697619 pyrippleapi-2024.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.714630 pyrippleapi-2024.5.1/src/pyrippleapi/
--rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2024.5.1/src/pyrippleapi/__init__.py
--rw-rw-rw-   0        0        0     3287 2024-02-29 13:52:45.000000 pyrippleapi-2024.5.1/src/pyrippleapi/api.py
--rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2024.5.1/src/pyrippleapi/exceptions.py
--rw-rw-rw-   0        0        0     5909 2024-05-13 13:46:46.000000 pyrippleapi-2024.5.1/src/pyrippleapi/generation_asset.py
-drwxrwxrwx   0        0        0        0 2024-05-13 13:47:27.744620 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 13:47:27.000000 pyrippleapi-2024.5.1/src/pyrippleapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:18:53.426630 pyrippleapi-2024.5.2/
+-rw-rw-rw-   0        0        0      418 2024-05-13 14:18:53.427630 pyrippleapi-2024.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2024.5.2/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2024.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-05-13 14:18:53.434932 pyrippleapi-2024.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      817 2024-05-13 14:18:45.000000 pyrippleapi-2024.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:18:53.370956 pyrippleapi-2024.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:18:53.391032 pyrippleapi-2024.5.2/src/pyrippleapi/
+-rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2024.5.2/src/pyrippleapi/__init__.py
+-rw-rw-rw-   0        0        0     3341 2024-05-13 14:17:35.000000 pyrippleapi-2024.5.2/src/pyrippleapi/api.py
+-rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2024.5.2/src/pyrippleapi/exceptions.py
+-rw-rw-rw-   0        0        0     5909 2024-05-13 13:46:46.000000 pyrippleapi-2024.5.2/src/pyrippleapi/generation_asset.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:18:53.424630 pyrippleapi-2024.5.2/src/pyrippleapi.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-13 14:18:53.000000 pyrippleapi-2024.5.2/src/pyrippleapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-13 14:18:53.000000 pyrippleapi-2024.5.2/src/pyrippleapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:18:53.000000 pyrippleapi-2024.5.2/src/pyrippleapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 14:18:53.000000 pyrippleapi-2024.5.2/src/pyrippleapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 14:18:53.000000 pyrippleapi-2024.5.2/src/pyrippleapi.egg-info/top_level.txt
```

### Comparing `pyrippleapi-2024.5.1/setup.py` & `pyrippleapi-2024.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pyrippleapi",
-    version="2024.5.1",
+    version="2024.5.2",
     description="Ripple energy api wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ryanbdclark/pyrippleapi",
     author="Ryan Clark",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyrippleapi-2024.5.1/src/pyrippleapi/api.py` & `pyrippleapi-2024.5.2/src/pyrippleapi/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,27 +73,29 @@
 
         headers = {
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.67",
         }
-
         async with self.session.request(
             "GET", self._api_url + self._auth_token, headers=headers
         ) as response:
             if response.status != 200:
                 raise RippleConnectionError("Error sending request")
 
             response = await response.json()
 
             if "error" in response:
                 raise RippleAuthenticationError("Invalid API Key")
 
             if len(response["generation_assets"]) < 1:
                 raise RippleDevicesError("No generation assets found")
+        
+            new_assets = []
+            for asset in response["generation_assets"]:
+                if asset["name"] in assets:
+                    new_assets.append(asset)
 
-            for asset in enumerate(response["generation_assets"]):
-                if asset[1]["name"] not in assets:
-                    del response["generation_assets"][asset[0]]
+            response["generation_assets"]=new_assets
 
             return response
```

### Comparing `pyrippleapi-2024.5.1/src/pyrippleapi/generation_asset.py` & `pyrippleapi-2024.5.2/src/pyrippleapi/generation_asset.py`

 * *Files identical despite different names*

