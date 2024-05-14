# Comparing `tmp/mpd_now_playable-1.1.1.tar.gz` & `tmp/mpd_now_playable-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpd_now_playable-1.1.1.tar", last modified: Tue May 14 04:08:22 2024, max compression
+gzip compressed data, was "mpd_now_playable-1.1.2.tar", last modified: Tue May 14 06:09:26 2024, max compression
```

## Comparing `mpd_now_playable-1.1.1.tar` & `mpd_now_playable-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4223 2024-05-14 04:04:04.537115 mpd_now_playable-1.1.1/README.md
--rw-r--r--   0        0        0     1914 2024-05-14 04:08:22.717033 mpd_now_playable-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       87 2024-03-07 04:52:35.897735 mpd_now_playable-1.1.1/src/corefoundationasyncio/__init__.py
--rw-r--r--   0        0        0     7343 2024-03-07 04:52:35.897945 mpd_now_playable-1.1.1/src/corefoundationasyncio/eventloop.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898117 mpd_now_playable-1.1.1/src/mpd_now_playable/__init__.py
--rw-r--r--   0        0        0      483 2024-03-07 04:52:35.898278 mpd_now_playable-1.1.1/src/mpd_now_playable/async_tools.py
--rw-r--r--   0        0        0     1384 2024-05-14 04:06:47.011108 mpd_now_playable-1.1.1/src/mpd_now_playable/cache.py
--rw-r--r--   0        0        0      869 2024-05-09 02:51:47.711237 mpd_now_playable-1.1.1/src/mpd_now_playable/cli.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898623 mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/__init__.py
--rw-r--r--   0        0        0     6961 2024-05-14 03:11:01.951769 mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/now_playing.py
--rw-r--r--   0        0        0     1657 2024-05-13 05:11:01.883611 mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/persistent_id.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.899242 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/__init__.py
--rw-r--r--   0        0        0     1698 2024-05-14 03:07:23.846226 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/artwork_cache.py
--rw-r--r--   0        0        0     4155 2024-05-13 05:09:56.754721 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/listener.py
--rw-r--r--   0        0        0    27419 2024-03-07 04:52:35.899776 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/logo.svg
--rw-r--r--   0        0        0     2536 2024-03-07 04:52:35.900036 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/types.py
--rw-r--r--   0        0        0      433 2024-03-07 04:52:35.900181 mpd_now_playable-1.1.1/src/mpd_now_playable/player.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.900247 mpd_now_playable-1.1.1/src/mpd_now_playable/py.typed
--rw-r--r--   0        0        0      735 2024-05-13 05:09:17.349547 mpd_now_playable-1.1.1/src/mpd_now_playable/song.py
--rw-r--r--   0        0        0      234 2024-03-07 04:52:35.900786 mpd_now_playable-1.1.1/src/mpd_now_playable/type_tools.py
--rw-r--r--   0        0        0     5345 1970-01-01 00:00:00.000000 mpd_now_playable-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4223 2024-05-14 04:04:04.537115 mpd_now_playable-1.1.2/README.md
+-rw-r--r--   0        0        0     1914 2024-05-14 06:09:26.833017 mpd_now_playable-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-03-07 04:52:35.897735 mpd_now_playable-1.1.2/src/corefoundationasyncio/__init__.py
+-rw-r--r--   0        0        0     7343 2024-03-07 04:52:35.897945 mpd_now_playable-1.1.2/src/corefoundationasyncio/eventloop.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898117 mpd_now_playable-1.1.2/src/mpd_now_playable/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-07 04:52:35.898278 mpd_now_playable-1.1.2/src/mpd_now_playable/async_tools.py
+-rw-r--r--   0        0        0     1384 2024-05-14 04:06:47.011108 mpd_now_playable-1.1.2/src/mpd_now_playable/cache.py
+-rw-r--r--   0        0        0      869 2024-05-09 02:51:47.711237 mpd_now_playable-1.1.2/src/mpd_now_playable/cli.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898623 mpd_now_playable-1.1.2/src/mpd_now_playable/cocoa/__init__.py
+-rw-r--r--   0        0        0     6961 2024-05-14 03:11:01.951769 mpd_now_playable-1.1.2/src/mpd_now_playable/cocoa/now_playing.py
+-rw-r--r--   0        0        0     1657 2024-05-13 05:11:01.883611 mpd_now_playable-1.1.2/src/mpd_now_playable/cocoa/persistent_id.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.899242 mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/__init__.py
+-rw-r--r--   0        0        0     1733 2024-05-14 05:11:56.159374 mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/artwork_cache.py
+-rw-r--r--   0        0        0     4155 2024-05-13 05:09:56.754721 mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/listener.py
+-rw-r--r--   0        0        0    27419 2024-03-07 04:52:35.899776 mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/logo.svg
+-rw-r--r--   0        0        0     2536 2024-03-07 04:52:35.900036 mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/types.py
+-rw-r--r--   0        0        0      433 2024-03-07 04:52:35.900181 mpd_now_playable-1.1.2/src/mpd_now_playable/player.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.900247 mpd_now_playable-1.1.2/src/mpd_now_playable/py.typed
+-rw-r--r--   0        0        0      735 2024-05-13 05:09:17.349547 mpd_now_playable-1.1.2/src/mpd_now_playable/song.py
+-rw-r--r--   0        0        0      234 2024-03-07 04:52:35.900786 mpd_now_playable-1.1.2/src/mpd_now_playable/type_tools.py
+-rw-r--r--   0        0        0     5345 1970-01-01 00:00:00.000000 mpd_now_playable-1.1.2/PKG-INFO
```

### Comparing `mpd_now_playable-1.1.1/README.md` & `mpd_now_playable-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/pyproject.toml` & `mpd_now_playable-1.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 classifiers = [
     "Environment :: No Input/Output (Daemon)",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python :: 3.12",
     "Topic :: Multimedia :: Sound/Audio :: Players",
 ]
-version = "1.1.1"
+version = "1.1.2"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 redis = [
     "aiocache[redis]",
```

### Comparing `mpd_now_playable-1.1.1/src/corefoundationasyncio/eventloop.py` & `mpd_now_playable-1.1.2/src/corefoundationasyncio/eventloop.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/cache.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/cache.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/cli.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/cli.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/now_playing.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/cocoa/now_playing.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/persistent_id.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/cocoa/persistent_id.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/artwork_cache.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/artwork_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from typing import TypedDict
 
 from ..async_tools import run_background_task
 from ..cache import Cache, make_cache
 from .types import CurrentSongResponse, MpdStateHandler
 
-CACHE_TTL = 60 * 10  # ten minutes
+CACHE_TTL = 60 * 60 # seconds = 1 hour
 
 
 class ArtCacheEntry(TypedDict):
 	data: bytes | None
 
 
 def calc_album_key(song: CurrentSongResponse) -> str:
 	artist = song.get("albumartist", song.get("artist", "Unknown Artist"))
 	album = song.get("album", "Unknown Album")
-	return f"{artist}:-:-:{album}"
+	return ":".join(t.replace(":", "-") for t in (artist, album))
 
 
 def calc_track_key(song: CurrentSongResponse) -> str:
 	return song["file"]
 
 
 class MpdArtworkCache:
```

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/listener.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/listener.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/logo.svg` & `mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/logo.svg`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/types.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/mpd/types.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/src/mpd_now_playable/song.py` & `mpd_now_playable-1.1.2/src/mpd_now_playable/song.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.1/PKG-INFO` & `mpd_now_playable-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-now-playable
-Version: 1.1.1
+Version: 1.1.2
 Summary: Expose your MPD server as a 'now playable' app on MacOS
 Author-Email: Danielle McLean <dani@00dani.me>
 License: MIT
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.12
```

