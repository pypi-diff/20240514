# Comparing `tmp/touchbar_lyric-0.8.1.tar.gz` & `tmp/touchbar_lyric-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "touchbar_lyric-0.8.1.tar", max compression
+gzip compressed data, was "touchbar_lyric-0.8.2.tar", max compression
```

## Comparing `touchbar_lyric-0.8.1.tar` & `touchbar_lyric-0.8.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     3024 2023-01-23 19:28:58.514516 touchbar_lyric-0.8.1/README.md
--rw-r--r--   0        0        0      654 2023-02-15 01:24:02.059265 touchbar_lyric-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-01-23 19:28:59.423870 touchbar_lyric-0.8.1/touchbar_lyric/__init__.py
--rw-r--r--   0        0        0     1550 2022-10-14 02:53:32.936127 touchbar_lyric-0.8.1/touchbar_lyric/__main__.py
--rw-r--r--   0        0        0     2071 2023-01-23 19:28:59.422651 touchbar_lyric-0.8.1/touchbar_lyric/service/__init__.py
--rw-r--r--   0        0        0     7699 2023-02-15 01:24:17.484603 touchbar_lyric-0.8.1/touchbar_lyric/service/misc.py
--rw-r--r--   0        0        0     5350 2023-01-23 19:28:59.427127 touchbar_lyric-0.8.1/touchbar_lyric/service/netease.py
--rw-r--r--   0        0        0     1476 2023-01-23 18:35:42.988961 touchbar_lyric-0.8.1/touchbar_lyric/service/qq.py
--rw-r--r--   0        0        0     2619 2022-07-01 20:42:57.301030 touchbar_lyric-0.8.1/touchbar_lyric/utility/__init__.py
--rw-r--r--   0        0        0     4059 1970-01-01 00:00:00.000000 touchbar_lyric-0.8.1/setup.py
--rw-r--r--   0        0        0     4083 1970-01-01 00:00:00.000000 touchbar_lyric-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3024 2024-05-14 18:51:44.098795 touchbar_lyric-0.8.2/README.md
+-rw-r--r--   0        0        0      654 2024-05-14 19:27:12.764140 touchbar_lyric-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2086 2024-05-14 18:51:44.099595 touchbar_lyric-0.8.2/touchbar_lyric/__init__.py
+-rw-r--r--   0        0        0     1988 2024-05-14 19:25:26.382806 touchbar_lyric-0.8.2/touchbar_lyric/__main__.py
+-rw-r--r--   0        0        0     2075 2024-05-14 19:26:38.407582 touchbar_lyric-0.8.2/touchbar_lyric/service/__init__.py
+-rw-r--r--   0        0        0     7699 2024-05-14 18:51:44.099880 touchbar_lyric-0.8.2/touchbar_lyric/service/misc.py
+-rw-r--r--   0        0        0     5350 2024-05-14 18:51:44.099984 touchbar_lyric-0.8.2/touchbar_lyric/service/netease.py
+-rw-r--r--   0        0        0     1476 2024-05-14 18:51:44.100051 touchbar_lyric-0.8.2/touchbar_lyric/service/qq.py
+-rw-r--r--   0        0        0     2619 2024-05-14 18:51:44.100151 touchbar_lyric-0.8.2/touchbar_lyric/utility/__init__.py
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 touchbar_lyric-0.8.2/PKG-INFO
```

### Comparing `touchbar_lyric-0.8.1/README.md` & `touchbar_lyric-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `touchbar_lyric-0.8.1/pyproject.toml` & `touchbar_lyric-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "touchbar-lyric"
-version = "0.8.1"
+version = "0.8.2"
 description = "Display lyrics on your touchbar with BTT"
 authors = ["Chenghao Mou <mouchenghao@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `touchbar_lyric-0.8.1/touchbar_lyric/__init__.py` & `touchbar_lyric-0.8.2/touchbar_lyric/__init__.py`

 * *Files identical despite different names*

### Comparing `touchbar_lyric-0.8.1/touchbar_lyric/__main__.py` & `touchbar_lyric-0.8.2/touchbar_lyric/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Date    : 2021-03-14 15:29:12
 # @Author  : Chenghao Mou (chenghao@gmail.com)
-
+import hashlib
 import logging.config
+import os
+import time
+from pathlib import Path
 
 import typer
 from hanziconv import HanziConv
 from loguru import logger
 
-from touchbar_lyric.service import universal_search
+from touchbar_lyric.service import universal_search, CACHE
 from touchbar_lyric.utility import get_info
 
 logging.config.dictConfig(
     {
         "version": 1,
         "disable_existing_loggers": True,
     }
@@ -32,25 +35,32 @@
     ),
 ):  # pragma: no cover
     {True: logger.enable, False: logger.disable}[debug]("touchbar_lyric")
 
     if not debug:
         logger.disable("touchbar_lyric")
         logger.disable("__main__")
-
+    start_time = time.time()
     media_info = get_info(app)
     if media_info is None:
         return
 
+    hash = hashlib.md5(f"{media_info.name}{media_info.artists}".encode()).hexdigest()
+    if os.path.exists(Path(CACHE) / f"{hash}.lock"):
+        return []
+    # Create a manual lock to prevent multiple searches
+    open(Path(CACHE) / f"{hash}.lock", "w").close()
     songs = universal_search(media_info.name, media_info.artists)
+    os.remove(Path(CACHE) / f"{hash}.lock")
+
     logger.debug("|".join(song.title for song in songs))
     logger.debug("|".join(song.artists for song in songs))
     for song in songs:
         if song.anchor(media_info.position):
-            line: str = song.anchor(media_info.position)
+            line: str = song.anchor(media_info.position + int(time.time() - start_time))
             if traditional:
                 line = HanziConv.toTraditional(line)
             print(line)
             break
 
 
 if __name__ == "__main__":  # pragma: no cover
```

### Comparing `touchbar_lyric-0.8.1/touchbar_lyric/service/__init__.py` & `touchbar_lyric-0.8.2/touchbar_lyric/service/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Date    : 2021-03-14 15:54:40
 # @Author  : Chenghao Mou (mouchenghao@gmail.com)
-
 import logging.config
 import os
+from concurrent.futures import ThreadPoolExecutor
 from typing import List, Tuple
 
 from diskcache import FanoutCache
 from hanziconv import HanziConv
 from strsimpy.normalized_levenshtein import NormalizedLevenshtein
 
 from touchbar_lyric import Song
@@ -35,22 +35,31 @@
 cache = FanoutCache(CACHE, timeout=2)
 
 
 @cache.memoize(typed=True, expire=None, tag="lyric")
 def universal_search(title: str, artists: str) -> List[Song]:  # pragma: no cover
     songs: List[Tuple[int, Song]] = []
     title = HanziConv.toSimplified(title)
-    songs.extend((-i, s) for i, s in enumerate(netease_music_search(title, artists)))
-    songs.extend((-i, s) for i, s in enumerate(qq_music_search(title, artists)))
-    songs.extend((-i, s)
-                 for i, s in enumerate(rentanadviser_music_search(title, artists)))
-    songs.extend((-i, s) for i, s in enumerate(megalobiz_music_search(title, artists)))
-    songs.extend((-i, s) for i, s in enumerate(lyricsify_music_search(title, artists)))
-    songs.extend((-i, s)
-                 for i, s in enumerate(rclyricsband_music_search(title, artists)))
+
+    # Multithreaded search
+    with ThreadPoolExecutor() as executor:
+        results = list(executor.map(
+            lambda f: f(title, artists),
+            [
+                netease_music_search,
+                qq_music_search,
+                rentanadviser_music_search,
+                megalobiz_music_search,
+                lyricsify_music_search,
+                rclyricsband_music_search,
+            ],
+        ))
+
+    for result in results:
+        songs.extend((-i, s) for i, s in enumerate(result))
 
     return [s[1] for s in sorted(
         songs,
         key=lambda s: (
             NormalizedLevenshtein().similarity(s[1].title, s[1].target_title)
             + NormalizedLevenshtein().similarity(s[1].artists, s[1].target_artists),
             s[0],
```

### Comparing `touchbar_lyric-0.8.1/touchbar_lyric/service/misc.py` & `touchbar_lyric-0.8.2/touchbar_lyric/service/misc.py`

 * *Files identical despite different names*

### Comparing `touchbar_lyric-0.8.1/touchbar_lyric/service/netease.py` & `touchbar_lyric-0.8.2/touchbar_lyric/service/netease.py`

 * *Files identical despite different names*

### Comparing `touchbar_lyric-0.8.1/touchbar_lyric/service/qq.py` & `touchbar_lyric-0.8.2/touchbar_lyric/service/qq.py`

 * *Files identical despite different names*

### Comparing `touchbar_lyric-0.8.1/touchbar_lyric/utility/__init__.py` & `touchbar_lyric-0.8.2/touchbar_lyric/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `touchbar_lyric-0.8.1/setup.py` & `touchbar_lyric-0.8.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,89 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: touchbar-lyric
+Version: 0.8.2
+Summary: Display lyrics on your touchbar with BTT
+License: MIT
+Author: Chenghao Mou
+Author-email: mouchenghao@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: applescript (>=2021.2.9,<2022.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: coverage (>=5.5,<6.0)
+Requires-Dist: diskcache (>=5.2.1,<6.0.0)
+Requires-Dist: hanziconv (>=0.3.2,<0.4.0)
+Requires-Dist: loguru (>=0.5.3,<0.6.0)
+Requires-Dist: pyaes (>=1.6.1,<2.0.0)
+Requires-Dist: qqmusic-api (>=0.1,<0.2)
+Requires-Dist: regex (>=2021.3.17,<2022.0.0)
+Requires-Dist: strsimpy (>=0.2.0,<0.3.0)
+Requires-Dist: typer (>=0.3.2,<0.4.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['touchbar_lyric', 'touchbar_lyric.service', 'touchbar_lyric.utility']
+<center><h1>Synced Lyric on TouchBar</h1></center>
 
-package_data = \
-{'': ['*']}
+:warning: I no longer have a macbook with TouchBar, so I won't be able to update this project as often.
 
-install_requires = \
-['applescript>=2021.2.9,<2022.0.0',
- 'beautifulsoup4>=4.11.1,<5.0.0',
- 'coverage>=5.5,<6.0',
- 'diskcache>=5.2.1,<6.0.0',
- 'hanziconv>=0.3.2,<0.4.0',
- 'loguru>=0.5.3,<0.6.0',
- 'pyaes>=1.6.1,<2.0.0',
- 'qqmusic-api>=0.1,<0.2',
- 'regex>=2021.3.17,<2022.0.0',
- 'strsimpy>=0.2.0,<0.3.0',
- 'typer>=0.3.2,<0.4.0']
-
-setup_kwargs = {
-    'name': 'touchbar-lyric',
-    'version': '0.8.1',
-    'description': 'Display lyrics on your touchbar with BTT',
-    'long_description': "<center><h1>Synced Lyric on TouchBar</h1></center>\n\n:warning: I no longer have a macbook with TouchBar, so I won't be able to update this project as often.\n\n[![Codacy Badge](https://api.codacy.com/project/badge/Grade/77de523131f9441997db18c608b3c54e)](https://app.codacy.com/manual/mouchenghao/touchbar-lyric?utm_source=github.com&utm_medium=referral&utm_content=ChenghaoMou/touchbar-lyric&utm_campaign=Badge_Grade_Dashboard) [![Build Status](https://travis-ci.com/ChenghaoMou/touchbar-lyric.svg?branch=master)](https://travis-ci.com/ChenghaoMou/touchbar-lyric) [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/aadeca6117a14aa6b655e21d5bbc09ea)](https://www.codacy.com/manual/mouchenghao/touchbar-lyric?utm_source=github.com&utm_medium=referral&utm_content=ChenghaoMou/touchbar-lyric&utm_campaign=Badge_Coverage) [![PyPI version](https://badge.fury.io/py/touchbar-lyric.svg)](https://badge.fury.io/py/touchbar-lyric)\n\nShow synced lyric in the touch-bar with BetterTouchTool and NetEase/QQ Music APIs. Based on the idea of [Kashi](https://community.folivora.ai/t/kashi-show-current-song-lyrics-on-touch-bar-spotify-itunes-youtube/6301).\n\n![Preview](./lyric_chinese.png)\n![Preview](./lyric_english.png)\n\n## Features\n\n-   **Synced lyrics** from QQ Music and NetEase Music APIs;\n-   Support **Spotify** (Recommended) & **Music** (Only songs in your playlists);\n-   Support for **English/Spanish/Chinese(Simplified/Traditional)/Japanese** and more;\n\n## Instruction\n\n**If you are not familiar with command line, python ecosystem or having problems understanding this tutorial, find a friend to help you. Issues/DMs are not actively monitored for this project.**\n\n### 1. Installation\n```shell\npip3 install touchbar_lyric --upgrade\n```\n\n### 2. Configuration in BetterTouchTool\n\nSame as Kashi:\n\n1.  Copy&paste the content in `lyric.json` in _Meun Bar > Touch Bar_;\n2.  Change the python path `$PYTHONPATH` to your own python path in the script area;\n\n```shell\n$PYTHONPATH -m touchbar_lyric --app Music\n```\n\nor use Spotify(default)\n\n```shell\n$PYTHONPATH -m touchbar_lyric --app Spotify\n```\n\nShow Traditional Chinese lyrics\n\n```shell\n$PYTHONPATH -m touchbar_lyric --app Spotify --traditional\n```\n\n**Be careful with typing double hyphens in BTT. It automatically change it to an em slash. Use copy & paste instead!**\n\n## Acknowledgement\n\n1. Inspired by [Kashi](https://community.folivora.ai/t/kashi-show-current-song-lyrics-on-touch-bar-spotify-itunes-youtube/6301) by [Jim Ho](https://github.com/jimu-gh).\n2. Supported by wonderful projects like [qq-music-api](https://github.com/Rain120/qq-music-api) by [Rain120](https://github.com/Rain120) and [spotifylyrics](https://github.com/SimonIT/spotifylyrics) by [SimonIT](https://github.com/SimonIT).\n\n## Disclaimer\n\nThis project is not affiliated with Apple, Spotify, QQ Music, NetEase Music, BetterTouchTool or any other third party. This project is not intended to violate any terms of service of the aforementioned parties. This project is for educational purposes only.\n",
-    'author': 'Chenghao Mou',
-    'author_email': 'mouchenghao@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/77de523131f9441997db18c608b3c54e)](https://app.codacy.com/manual/mouchenghao/touchbar-lyric?utm_source=github.com&utm_medium=referral&utm_content=ChenghaoMou/touchbar-lyric&utm_campaign=Badge_Grade_Dashboard) [![Build Status](https://travis-ci.com/ChenghaoMou/touchbar-lyric.svg?branch=master)](https://travis-ci.com/ChenghaoMou/touchbar-lyric) [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/aadeca6117a14aa6b655e21d5bbc09ea)](https://www.codacy.com/manual/mouchenghao/touchbar-lyric?utm_source=github.com&utm_medium=referral&utm_content=ChenghaoMou/touchbar-lyric&utm_campaign=Badge_Coverage) [![PyPI version](https://badge.fury.io/py/touchbar-lyric.svg)](https://badge.fury.io/py/touchbar-lyric)
 
+Show synced lyric in the touch-bar with BetterTouchTool and NetEase/QQ Music APIs. Based on the idea of [Kashi](https://community.folivora.ai/t/kashi-show-current-song-lyrics-on-touch-bar-spotify-itunes-youtube/6301).
+
+![Preview](./lyric_chinese.png)
+![Preview](./lyric_english.png)
+
+## Features
+
+-   **Synced lyrics** from QQ Music and NetEase Music APIs;
+-   Support **Spotify** (Recommended) & **Music** (Only songs in your playlists);
+-   Support for **English/Spanish/Chinese(Simplified/Traditional)/Japanese** and more;
+
+## Instruction
+
+**If you are not familiar with command line, python ecosystem or having problems understanding this tutorial, find a friend to help you. Issues/DMs are not actively monitored for this project.**
+
+### 1. Installation
+```shell
+pip3 install touchbar_lyric --upgrade
+```
+
+### 2. Configuration in BetterTouchTool
+
+Same as Kashi:
+
+1.  Copy&paste the content in `lyric.json` in _Meun Bar > Touch Bar_;
+2.  Change the python path `$PYTHONPATH` to your own python path in the script area;
+
+```shell
+$PYTHONPATH -m touchbar_lyric --app Music
+```
+
+or use Spotify(default)
+
+```shell
+$PYTHONPATH -m touchbar_lyric --app Spotify
+```
+
+Show Traditional Chinese lyrics
+
+```shell
+$PYTHONPATH -m touchbar_lyric --app Spotify --traditional
+```
+
+**Be careful with typing double hyphens in BTT. It automatically change it to an em slash. Use copy & paste instead!**
+
+## Acknowledgement
+
+1. Inspired by [Kashi](https://community.folivora.ai/t/kashi-show-current-song-lyrics-on-touch-bar-spotify-itunes-youtube/6301) by [Jim Ho](https://github.com/jimu-gh).
+2. Supported by wonderful projects like [qq-music-api](https://github.com/Rain120/qq-music-api) by [Rain120](https://github.com/Rain120) and [spotifylyrics](https://github.com/SimonIT/spotifylyrics) by [SimonIT](https://github.com/SimonIT).
+
+## Disclaimer
+
+This project is not affiliated with Apple, Spotify, QQ Music, NetEase Music, BetterTouchTool or any other third party. This project is not intended to violate any terms of service of the aforementioned parties. This project is for educational purposes only.
 
-setup(**setup_kwargs)
```

