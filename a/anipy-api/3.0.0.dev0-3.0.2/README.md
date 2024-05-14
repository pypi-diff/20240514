# Comparing `tmp/anipy_api-3.0.0.dev0.tar.gz` & `tmp/anipy_api-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_api-3.0.0.dev0.tar", max compression
+gzip compressed data, was "anipy_api-3.0.2.tar", max compression
```

## Comparing `anipy_api-3.0.0.dev0.tar` & `anipy_api-3.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      227 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/README.md
--rw-r--r--   0        0        0      852 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/pyproject.toml
--rw-r--r--   0        0        0       53 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/__init__.py
--rw-r--r--   0        0        0     5417 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/anime.py
--rw-r--r--   0        0        0    11323 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/download.py
--rw-r--r--   0        0        0     2765 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/error.py
--rw-r--r--   0        0        0     7953 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/locallist.py
--rw-r--r--   0        0        0    20790 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/mal.py
--rw-r--r--   0        0        0      132 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/base.py
--rw-r--r--   0        0        0     1692 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/player.py
--rw-r--r--   0        0        0      267 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/players/__init__.py
--rw-r--r--   0        0        0     1147 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/players/mpv.py
--rw-r--r--   0        0        0     2669 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/players/mpv_control.py
--rw-r--r--   0        0        0      941 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/players/syncplay.py
--rw-r--r--   0        0        0      918 2024-05-11 00:42:50.173161 anipy_api-3.0.0.dev0/src/anipy_api/player/players/vlc.py
--rw-r--r--   0        0        0      628 2024-05-11 00:42:50.177161 anipy_api-3.0.0.dev0/src/anipy_api/provider/__init__.py
--rw-r--r--   0        0        0     5321 2024-05-11 00:42:50.177161 anipy_api-3.0.0.dev0/src/anipy_api/provider/base.py
--rw-r--r--   0        0        0     3397 2024-05-11 00:42:50.177161 anipy_api-3.0.0.dev0/src/anipy_api/provider/filter.py
--rw-r--r--   0        0        0     1543 2024-05-11 00:42:50.177161 anipy_api-3.0.0.dev0/src/anipy_api/provider/provider.py
--rw-r--r--   0        0        0       96 2024-05-11 00:42:50.177161 anipy_api-3.0.0.dev0/src/anipy_api/provider/providers/__init__.py
--rw-r--r--   0        0        0    12230 2024-05-11 00:42:50.177161 anipy_api-3.0.0.dev0/src/anipy_api/provider/providers/gogo_provider.py
--rw-r--r--   0        0        0     1482 2024-05-11 00:42:50.177161 anipy_api-3.0.0.dev0/src/anipy_api/provider/utils.py
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 anipy_api-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-05-14 06:16:31.912194 anipy_api-3.0.2/README.md
+-rw-r--r--   0        0        0      847 2024-05-14 06:16:31.912194 anipy_api-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/__init__.py
+-rw-r--r--   0        0        0     5417 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/anime.py
+-rw-r--r--   0        0        0    11407 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/download.py
+-rw-r--r--   0        0        0     2765 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/error.py
+-rw-r--r--   0        0        0     7953 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/locallist.py
+-rw-r--r--   0        0        0    20790 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/mal.py
+-rw-r--r--   0        0        0      132 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/base.py
+-rw-r--r--   0        0        0     1692 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/player.py
+-rw-r--r--   0        0        0      267 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/players/__init__.py
+-rw-r--r--   0        0        0     1147 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/players/mpv.py
+-rw-r--r--   0        0        0     2669 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/players/mpv_control.py
+-rw-r--r--   0        0        0      941 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/players/syncplay.py
+-rw-r--r--   0        0        0      918 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/player/players/vlc.py
+-rw-r--r--   0        0        0      628 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/provider/__init__.py
+-rw-r--r--   0        0        0     5321 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/provider/base.py
+-rw-r--r--   0        0        0     3397 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/provider/filter.py
+-rw-r--r--   0        0        0     1543 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/provider/provider.py
+-rw-r--r--   0        0        0       96 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/provider/providers/__init__.py
+-rw-r--r--   0        0        0    12230 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/provider/providers/gogo_provider.py
+-rw-r--r--   0        0        0     1482 2024-05-14 06:16:31.912194 anipy_api-3.0.2/src/anipy_api/provider/utils.py
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.0.2/PKG-INFO
```

### Comparing `anipy_api-3.0.0.dev0/pyproject.toml` & `anipy_api-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-api"
-version = "3.0.0.dev0"
+version = "3.0.2"
 description = "api for anipy-cli"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-api"
 keywords = ["anime", "api"]
```

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/anime.py` & `anipy_api-3.0.2/src/anipy_api/anime.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/download.py` & `anipy_api-3.0.2/src/anipy_api/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,19 +61,20 @@
         adapter = HTTPAdapter(max_retries=Retry(connect=3, backoff_factor=0.5))
         self._session.mount("http://", adapter)
         self._session.mount("https://", adapter)
 
     @staticmethod
     def _get_valid_pathname(name: str):
         if sys.platform == "win32":
-            WIN_INVALID_CHARS = ["\\", "/", ":", "*", "?", "<", ">", "|", '"']
-            name = "".join(["" if x in WIN_INVALID_CHARS else x for x in name])
+            INVALID_CHARS = ["\\", "/", ":", "*", "?", "<", ">", "|", '"', "."]
+        else:
+            INVALID_CHARS = [".", "/"]
 
         name = "".join(
-            [i for i in name if i.isascii()]
+            [i for i in name if i.isascii() and not i in INVALID_CHARS]
         )  # Verify all chars are ascii (eject if not)
 
         return name
 
     def m3u8_download(self, stream: "ProviderStream", download_path: Path) -> Path:
         """Download a m3u8/hls stream to a specified download path in a ts container.
 
@@ -102,15 +103,16 @@
         assert m3u8_content.is_variant is False
 
         counter = 0
 
         def download_ts(segment: m3u8.Segment):
             nonlocal counter
             url = urljoin(segment.base_uri, segment.uri)
-            fname = temp_folder / self._get_valid_pathname(segment.uri)
+            segment_uri = Path(segment.uri)
+            fname = (temp_folder / self._get_valid_pathname(segment_uri.stem)).with_suffix(segment_uri.suffix)
             try:
                 res = self._session.get(str(url))
                 res.raise_for_status()
 
                 with fname.open("wb") as fout:
                     fout.write(res.content)
```

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/error.py` & `anipy_api-3.0.2/src/anipy_api/error.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/locallist.py` & `anipy_api-3.0.2/src/anipy_api/locallist.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/mal.py` & `anipy_api-3.0.2/src/anipy_api/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/player/base.py` & `anipy_api-3.0.2/src/anipy_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/player/player.py` & `anipy_api-3.0.2/src/anipy_api/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/player/players/mpv.py` & `anipy_api-3.0.2/src/anipy_api/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/player/players/mpv_control.py` & `anipy_api-3.0.2/src/anipy_api/player/players/mpv_control.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/player/players/syncplay.py` & `anipy_api-3.0.2/src/anipy_api/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/player/players/vlc.py` & `anipy_api-3.0.2/src/anipy_api/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/provider/__init__.py` & `anipy_api-3.0.2/src/anipy_api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/provider/base.py` & `anipy_api-3.0.2/src/anipy_api/provider/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/provider/filter.py` & `anipy_api-3.0.2/src/anipy_api/provider/filter.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/provider/provider.py` & `anipy_api-3.0.2/src/anipy_api/provider/provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/provider/providers/gogo_provider.py` & `anipy_api-3.0.2/src/anipy_api/provider/providers/gogo_provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/src/anipy_api/provider/utils.py` & `anipy_api-3.0.2/src/anipy_api/provider/utils.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.0.dev0/PKG-INFO` & `anipy_api-3.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-api
-Version: 3.0.0.dev0
+Version: 3.0.2
 Summary: api for anipy-cli
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,api
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
```

