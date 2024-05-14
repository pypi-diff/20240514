# Comparing `tmp/pyvhl-0.1.2.tar.gz` & `tmp/pyvhl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvhl-0.1.2.tar", max compression
+gzip compressed data, was "pyvhl-0.1.3.tar", max compression
```

## Comparing `pyvhl-0.1.2.tar` & `pyvhl-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       78 2024-05-01 05:33:54.771494 pyvhl-0.1.2/README.md
--rw-r--r--   0        0        0      465 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    15513 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/mirror_clients.py
--rw-r--r--   0        0        0        0 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/model/__init__.py
--rw-r--r--   0        0        0      523 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/model/_model.py
--rw-r--r--   0        0        0     5672 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/pyvhl.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 pyvhl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       78 2024-05-14 05:24:13.036501 pyvhl-0.1.3/README.md
+-rw-r--r--   0        0        0      518 2024-05-14 05:24:13.036501 pyvhl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    15472 2024-05-14 05:24:13.040501 pyvhl-0.1.3/pyvhl/mirror_clients.py
+-rw-r--r--   0        0        0        0 2024-05-14 05:24:13.040501 pyvhl-0.1.3/pyvhl/model/__init__.py
+-rw-r--r--   0        0        0      403 2024-05-14 05:24:13.040501 pyvhl-0.1.3/pyvhl/model/_model.py
+-rw-r--r--   0        0        0     6254 2024-05-14 05:24:13.040501 pyvhl-0.1.3/pyvhl/pyvhl.py
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 pyvhl-0.1.3/PKG-INFO
```

### Comparing `pyvhl-0.1.2/pyvhl/mirror_clients.py` & `pyvhl-0.1.3/pyvhl/mirror_clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from datetime import datetime, timezone
 from hashlib import sha256
 from hmac import new as hmac_new
 from io import BytesIO, IOBase, SEEK_END, SEEK_SET
-from mimetypes import guess_type
 from pathlib import Path
-from typing import Dict, Literal, Union
+from typing import Dict, Literal
 from urllib.parse import urlencode, urlparse
 
 from bs4 import BeautifulSoup
 from bs4.element import Tag
 from requests import Session
 from requests.structures import CaseInsensitiveDict
 from requests.utils import default_user_agent as requests_user_agent
@@ -409,15 +408,15 @@
         res = self.__transcode_uploaded_video(
             shortcode,
             transcoder_token,
             video_sz,
         )
         res.raise_for_status()
 
-        return StreamableVideo(shortcode=shortcode)
+        return StreamableVideo(shortcode=shortcode, url=f"{_StreamableClient.base_url}/{shortcode}")
 
 
 class _CatboxClient:
     api_url = "https://catbox.moe/user/api.php"
     file_base_url = "https://files.catbox.moe"
 
     def __init__(self, session: Session) -> None:
@@ -504,10 +503,7 @@
     def streamable(self):
         return self.__streamable
 
     @property
     def catbox(self):
         return self.__catbox
 
-
-if __name__ == "__main__":
-    client = Client()
```

### Comparing `pyvhl-0.1.2/pyvhl/pyvhl.py` & `pyvhl-0.1.3/pyvhl/pyvhl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import random
 
 from requests import Session
 from retry import retry
-from pyvhl.mirror_clients import Client
+from pyVHL.mirror_clients import Client
 from youtube_dl import YoutubeDL
 from loguru import logger
 
+from pyVHL.model._model import VideoClient
+
 
 class pyvhl:
     """
     Handles proccessing of mirroring videos from Reddit and Twitter.
     """
 
     def __init__(self) -> None:
@@ -39,41 +41,44 @@
         }
         with YoutubeDL(youtube_dl_opts) as ydl:
             info_dict = ydl.extract_info(video_url, download=download)
 
         # get size of file downloaded
         if download:
             file_size = os.stat(info_dict["id"] + "." + info_dict["ext"]).st_size
+        else:
+            file_size = 0
 
         if info_dict["extractor"] == "twitch:clips":
             clip_title = info_dict["title"]
             clip_url = info_dict["formats"][-1]["url"]
             clip_id = info_dict["id"]
             clip_streamer = info_dict["creator"]
             clip_date = info_dict["upload_date"]
             extractor = info_dict["extractor"]
             return {
+                "filename": info_dict["id"] + "." + info_dict["ext"],  # "filename": "clip.mp4
                 "title": clip_title,
                 "url": clip_url,
                 "id": clip_id,
                 "streamer": clip_streamer,
                 "date": clip_date,
                 "extractor": extractor,
                 "file_size": file_size,
             }
-            # return clip_title, clip_url, clip_id, clip_streamer
 
         elif info_dict["extractor"] == "youtube":
             clip_title = info_dict["title"]
             clip_url = info_dict["webpage_url"]
             clip_id = info_dict["id"]
             clip_streamer = video_url.split("/")[3]
             clip_date = info_dict["upload_date"]
             extractor = info_dict["extractor"]
             return {
+                "filename": info_dict["id"] + "." + info_dict["ext"],  # "filename": "clip.mp4
                 "title": clip_title,
                 "url": clip_url,
                 "id": clip_id,
                 "streamer": clip_streamer,
                 "date": clip_date,
                 "extractor": extractor,
                 "file_size": file_size,
@@ -130,37 +135,44 @@
             }
 
         else:
             logger.error(f"Clip URL: {video_url} | Clip not available")
             return {"title": None, "url": None, "id": None, "streamer": None, "date": None, "file_size": None}
 
     @retry(tries=10, delay=5)
-    def upload_video(self, clip_title: str, id: int, host: str = "") -> dict:
+    def upload_video(self, clip_title: str, filename: str, host: str = "", delete_file=False) -> VideoClient:
         """Uploads clip to one of the mirror clients
 
         Args:
             clip_title (str): Clip title
-            id (int): Clip id
-
+            filename (str): Clip filename
+            host (str): Mirror host. Defaults to random host. Must be either 'streamable' or 'catbox'
+            delete_file (bool): Delete file after upload. Defaults to False
         Returns:
-            str: Mirror url
+            dict: Contains mirror url and host
         """
-        if host not in ["streamable", "catbox"]:
+        if host not in ["streamable", "catbox", ""]:
             raise ValueError("Invalid host, must be either 'streamable' or 'catbox'")
         if host:
+            client_name = host
             client = self.clients[host]
         else:
             client_name = random.choice(list(self.clients.keys()))
             client = self.clients[client_name]
-        for file in os.listdir("./"):
-            if file.endswith(".mp4"):
-                if file.startswith(str(id)):
-                    clip_file = file
-                    break
+
+        clip_file = None
+        if os.path.exists(filename):
+            clip_file = filename
+        else:
+            raise FileNotFoundError("Clip file not found")
+
         try:
             with open(clip_file, "rb") as f:
                 mirror = client.upload_video(f, f"{id}.mp4")
-        finally:
+        except Exception as e:
+            logger.error(f"Error uploading video: {e}")
+            return {"url": mirror.url, "host": client_name}
+        if delete_file:
             # remove file
             os.remove(clip_file)
 
-        return {"mirror_url": mirror.url, "host": client_name}
+        return mirror
```

### Comparing `pyvhl-0.1.2/PKG-INFO` & `pyvhl-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVHL
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: problemxl
 Author-email: email@github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

