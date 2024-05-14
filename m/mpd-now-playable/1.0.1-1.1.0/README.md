# Comparing `tmp/mpd_now_playable-1.0.1.tar.gz` & `tmp/mpd_now_playable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpd_now_playable-1.0.1.tar", last modified: Wed Dec  6 03:39:36 2023, max compression
+gzip compressed data, was "mpd_now_playable-1.1.0.tar", last modified: Tue May 14 03:48:19 2024, max compression
```

## Comparing `mpd_now_playable-1.0.1.tar` & `mpd_now_playable-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     3122 2023-12-06 03:33:21.981236 mpd_now_playable-1.0.1/README.md
--rw-r--r--   0        0        0     1706 2023-12-06 03:39:36.044605 mpd_now_playable-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-11-26 22:48:15.174900 mpd_now_playable-1.0.1/src/corefoundationasyncio/__init__.py
--rw-r--r--   0        0        0     7343 2023-11-26 22:51:45.459175 mpd_now_playable-1.0.1/src/corefoundationasyncio/eventloop.py
--rw-r--r--   0        0        0        0 2023-11-26 13:16:43.358326 mpd_now_playable-1.0.1/src/mpd_now_playable/__init__.py
--rw-r--r--   0        0        0      483 2023-11-27 03:36:30.554220 mpd_now_playable-1.0.1/src/mpd_now_playable/async_tools.py
--rw-r--r--   0        0        0      817 2023-12-06 01:23:49.997803 mpd_now_playable-1.0.1/src/mpd_now_playable/cli.py
--rw-r--r--   0        0        0        0 2023-12-06 01:22:25.846711 mpd_now_playable-1.0.1/src/mpd_now_playable/cocoa/__init__.py
--rw-r--r--   0        0        0     6956 2023-12-06 03:38:52.497451 mpd_now_playable-1.0.1/src/mpd_now_playable/cocoa/now_playing.py
--rw-r--r--   0        0        0     1310 2023-12-06 01:26:20.071075 mpd_now_playable-1.0.1/src/mpd_now_playable/cocoa/persistent_id.py
--rw-r--r--   0        0        0        0 2023-11-27 02:46:22.178138 mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/__init__.py
--rw-r--r--   0        0        0     1458 2023-12-02 03:46:55.647885 mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/artwork_cache.py
--rw-r--r--   0        0        0     3969 2023-12-06 02:01:57.318726 mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/listener.py
--rw-r--r--   0        0        0    27419 2023-11-27 02:46:02.157056 mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/logo.svg
--rw-r--r--   0        0        0     2536 2023-12-05 22:59:39.962128 mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/types.py
--rw-r--r--   0        0        0      433 2023-12-06 01:42:37.348622 mpd_now_playable-1.0.1/src/mpd_now_playable/player.py
--rw-r--r--   0        0        0        0 2023-11-26 13:15:13.611579 mpd_now_playable-1.0.1/src/mpd_now_playable/py.typed
--rw-r--r--   0        0        0      694 2023-12-05 23:22:40.307826 mpd_now_playable-1.0.1/src/mpd_now_playable/song.py
--rw-r--r--   0        0        0      234 2023-12-05 23:24:17.862146 mpd_now_playable-1.0.1/src/mpd_now_playable/type_tools.py
--rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 mpd_now_playable-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3230 2024-03-07 04:52:56.592214 mpd_now_playable-1.1.0/README.md
+-rw-r--r--   0        0        0     1914 2024-05-14 03:48:19.943338 mpd_now_playable-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-03-07 04:52:35.897735 mpd_now_playable-1.1.0/src/corefoundationasyncio/__init__.py
+-rw-r--r--   0        0        0     7343 2024-03-07 04:52:35.897945 mpd_now_playable-1.1.0/src/corefoundationasyncio/eventloop.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898117 mpd_now_playable-1.1.0/src/mpd_now_playable/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-07 04:52:35.898278 mpd_now_playable-1.1.0/src/mpd_now_playable/async_tools.py
+-rw-r--r--   0        0        0     1405 2024-05-14 03:07:09.976223 mpd_now_playable-1.1.0/src/mpd_now_playable/cache.py
+-rw-r--r--   0        0        0      869 2024-05-09 02:51:47.711237 mpd_now_playable-1.1.0/src/mpd_now_playable/cli.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898623 mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/__init__.py
+-rw-r--r--   0        0        0     6961 2024-05-14 03:11:01.951769 mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/now_playing.py
+-rw-r--r--   0        0        0     1657 2024-05-13 05:11:01.883611 mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/persistent_id.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.899242 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/__init__.py
+-rw-r--r--   0        0        0     1698 2024-05-14 03:07:23.846226 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/artwork_cache.py
+-rw-r--r--   0        0        0     4155 2024-05-13 05:09:56.754721 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/listener.py
+-rw-r--r--   0        0        0    27419 2024-03-07 04:52:35.899776 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/logo.svg
+-rw-r--r--   0        0        0     2536 2024-03-07 04:52:35.900036 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/types.py
+-rw-r--r--   0        0        0      433 2024-03-07 04:52:35.900181 mpd_now_playable-1.1.0/src/mpd_now_playable/player.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.900247 mpd_now_playable-1.1.0/src/mpd_now_playable/py.typed
+-rw-r--r--   0        0        0      735 2024-05-13 05:09:17.349547 mpd_now_playable-1.1.0/src/mpd_now_playable/song.py
+-rw-r--r--   0        0        0      234 2024-03-07 04:52:35.900786 mpd_now_playable-1.1.0/src/mpd_now_playable/type_tools.py
+-rw-r--r--   0        0        0     4352 1970-01-01 00:00:00.000000 mpd_now_playable-1.1.0/PKG-INFO
```

### Comparing `mpd_now_playable-1.0.1/README.md` & `mpd_now_playable-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mpd-now-playable
+# mpd-now-playable [![PyPI version](https://badge.fury.io/py/mpd-now-playable.svg)](https://badge.fury.io/py/mpd-now-playable)
 
 This little Python program turns your MPD server into a [now playable app](https://developer.apple.com/documentation/mediaplayer/becoming_a_now_playable_app) on MacOS.
 This enables your keyboard's standard media keys to control MPD, as well as more esoteric music control methods like the buttons on your Bluetooth headphones.
 
 ## Installation
 
 The recommended way to install mpd-now-playable and its dependencies is with [pipx](https://pypa.github.io/pipx/):
```

### Comparing `mpd_now_playable-1.0.1/pyproject.toml` & `mpd_now_playable-1.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -16,19 +16,33 @@
 classifiers = [
     "Environment :: No Input/Output (Daemon)",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python :: 3.12",
     "Topic :: Multimedia :: Sound/Audio :: Players",
 ]
-version = "1.0.1"
+version = "1.1.0"
 
 [project.license]
 text = "MIT"
 
+[project.optional-dependencies]
+redis = [
+    "aiocache[redis]",
+]
+memcached = [
+    "aiocache[memcached]",
+]
+msgpack = [
+    "ormsgpack>=1.5.0",
+]
+all = [
+    "mpd-now-playable[redis,memcached,msgpack]",
+]
+
 [project.urls]
 Homepage = "https://git.00dani.me/00dani/mpd-now-playable"
 Issues = "https://git.00dani.me/00dani/mpd-now-playable/issues"
 
 [project.scripts]
 mpd-now-playable = "mpd_now_playable.cli:main"
```

### Comparing `mpd_now_playable-1.0.1/src/corefoundationasyncio/eventloop.py` & `mpd_now_playable-1.1.0/src/corefoundationasyncio/eventloop.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/cli.py` & `mpd_now_playable-1.1.0/src/mpd_now_playable/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from .mpd.listener import MpdStateListener
 
 
 async def listen() -> None:
 	port = int(environ.get("MPD_PORT", "6600"))
 	host = environ.get("MPD_HOST", "localhost")
 	password = environ.get("MPD_PASSWORD")
+	cache = environ.get("MPD_NOW_PLAYABLE_CACHE")
 	if password is None and "@" in host:
 		password, host = host.split("@", maxsplit=1)
 
-	listener = MpdStateListener()
+	listener = MpdStateListener(cache)
 	now_playing = CocoaNowPlaying(listener)
 	await listener.start(host=host, port=port, password=password)
 	await listener.loop(now_playing)
 
 
 def make_loop() -> CoreFoundationEventLoop:
 	return CoreFoundationEventLoop(console_app=True)
```

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/cocoa/now_playing.py` & `mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/now_playing.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 	return mapping[state]
 
 
 def song_to_media_item(song: Song) -> NSMutableDictionary:
 	nowplaying_info = nothing_to_media_item()
 	nowplaying_info[MPNowPlayingInfoPropertyMediaType] = MPNowPlayingInfoMediaTypeAudio
 	nowplaying_info[MPNowPlayingInfoPropertyElapsedPlaybackTime] = song.elapsed
-	nowplaying_info[MPNowPlayingInfoPropertyExternalContentIdentifier] = song.file
+	nowplaying_info[MPNowPlayingInfoPropertyExternalContentIdentifier] = str(song.file)
 	nowplaying_info[MPNowPlayingInfoPropertyPlaybackQueueCount] = song.queue_length
 	nowplaying_info[MPNowPlayingInfoPropertyPlaybackQueueIndex] = song.queue_index
 	nowplaying_info[MPMediaItemPropertyPersistentID] = song_to_persistent_id(song)
 
 	nowplaying_info[MPMediaItemPropertyTitle] = song.title
 	nowplaying_info[MPMediaItemPropertyArtist] = song.artist
 	nowplaying_info[MPMediaItemPropertyAlbumTitle] = song.album
```

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/cocoa/persistent_id.py` & `mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/persistent_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,36 +4,47 @@
 from uuid import UUID
 
 from ..song import Song
 
 # The maximum size for a BLAKE2b "person" value is sixteen bytes, so we need to be concise.
 HASH_PERSON_PREFIX: Final = b"mnp.mac."
 TRACKID_HASH_PERSON: Final = HASH_PERSON_PREFIX + b"mb_tid"
+RELEASETRACKID_HASH_PERSON: Final = HASH_PERSON_PREFIX + b"mb_rtid"
 FILE_HASH_PERSON: Final = HASH_PERSON_PREFIX + b"f"
 
 PERSISTENT_ID_BITS: Final = 64
 PERSISTENT_ID_BYTES: Final = PERSISTENT_ID_BITS // 8
 
 
 def digest_trackid(trackid: UUID) -> bytes:
 	return blake2b(
 		trackid.bytes, digest_size=PERSISTENT_ID_BYTES, person=TRACKID_HASH_PERSON
 	).digest()
 
 
+def digest_releasetrackid(trackid: UUID) -> bytes:
+	return blake2b(
+		trackid.bytes,
+		digest_size=PERSISTENT_ID_BYTES,
+		person=RELEASETRACKID_HASH_PERSON,
+	).digest()
+
+
 def digest_file_uri(file: Path) -> bytes:
 	return blake2b(
 		bytes(file), digest_size=PERSISTENT_ID_BYTES, person=FILE_HASH_PERSON
 	).digest()
 
 
 # The MPMediaItemPropertyPersistentID is only 64 bits, while a UUID is 128
 # bits and not all tracks will even have their MusicBrainz track ID included.
 # To work around this, we compute a BLAKE2 hash from the UUID, or failing
 # that from the file URI. BLAKE2 can be customised to different digest sizes,
 # making it perfect for this problem.
 def song_to_persistent_id(song: Song) -> int:
 	if song.musicbrainz_trackid:
 		hashed_id = digest_trackid(song.musicbrainz_trackid)
+	elif song.musicbrainz_releasetrackid:
+		hashed_id = digest_releasetrackid(song.musicbrainz_releasetrackid)
 	else:
 		hashed_id = digest_file_uri(song.file)
 	return int.from_bytes(hashed_id)
```

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/artwork_cache.py` & `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/artwork_cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-from aiocache import Cache
+from __future__ import annotations
+
+from typing import TypedDict
 
 from ..async_tools import run_background_task
+from ..cache import Cache, make_cache
 from .types import CurrentSongResponse, MpdStateHandler
 
 CACHE_TTL = 60 * 10  # ten minutes
 
 
+class ArtCacheEntry(TypedDict):
+	data: bytes | None
+
+
 def calc_album_key(song: CurrentSongResponse) -> str:
 	artist = song.get("albumartist", song.get("artist", "Unknown Artist"))
 	album = song.get("album", "Unknown Album")
 	return f"{artist}:-:-:{album}"
 
 
 def calc_track_key(song: CurrentSongResponse) -> str:
 	return song["file"]
 
 
 class MpdArtworkCache:
 	mpd: MpdStateHandler
-	album_cache: "Cache[bytes | None]"
-	track_cache: "Cache[bytes | None]"
+	album_cache: Cache[ArtCacheEntry]
+	track_cache: Cache[ArtCacheEntry]
 
-	def __init__(self, mpd: MpdStateHandler):
+	def __init__(self, mpd: MpdStateHandler, cache_url: str = "memory://"):
 		self.mpd = mpd
-		self.album_cache = Cache()
-		self.track_cache = Cache()
+		self.album_cache = make_cache(cache_url, "album")
+		self.track_cache = make_cache(cache_url, "track")
 
 	async def get_cached_artwork(self, song: CurrentSongResponse) -> bytes | None:
 		art = await self.track_cache.get(calc_track_key(song))
 		if art:
-			return art
+			return art["data"]
 
 		# If we don't have track artwork cached, go find some.
 		run_background_task(self.cache_artwork(song))
 
 		# Even if we don't have cached track art, we can try looking for cached album art.
 		art = await self.album_cache.get(calc_album_key(song))
 		if art:
-			return art
+			return art["data"]
 
 		return None
 
 	async def cache_artwork(self, song: CurrentSongResponse) -> None:
-		art = await self.mpd.readpicture(song["file"])
+		art = ArtCacheEntry(data=await self.mpd.readpicture(song["file"]))
 		try:
 			await self.album_cache.add(calc_album_key(song), art, ttl=CACHE_TTL)
 		except ValueError:
 			pass
 		await self.track_cache.set(calc_track_key(song), art, ttl=CACHE_TTL)
 		await self.mpd.refresh()
```

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/listener.py` & `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 ) -> Song:
 	return Song(
 		state=PlaybackState(status["state"]),
 		queue_index=int(current["pos"]),
 		queue_length=int(status["playlistlength"]),
 		file=Path(current["file"]),
 		musicbrainz_trackid=convert_if_exists(current.get("musicbrainz_trackid"), UUID),
+		musicbrainz_releasetrackid=convert_if_exists(
+			current.get("musicbrainz_releasetrackid"), UUID
+		),
 		title=current.get("title"),
 		artist=current.get("artist"),
 		album=current.get("album"),
 		album_artist=current.get("albumartist"),
 		composer=current.get("composer"),
 		genre=current.get("genre"),
 		track=convert_if_exists(current.get("track"), int),
@@ -37,17 +40,19 @@
 
 class MpdStateListener(Player):
 	client: MPDClient
 	listener: SongListener
 	art_cache: MpdArtworkCache
 	idle_count = 0
 
-	def __init__(self) -> None:
+	def __init__(self, cache: str | None = None) -> None:
 		self.client = MPDClient()
-		self.art_cache = MpdArtworkCache(self)
+		self.art_cache = (
+			MpdArtworkCache(self, cache) if cache else MpdArtworkCache(self)
+		)
 
 	async def start(
 		self, host: str = "localhost", port: int = 6600, password: str | None = None
 	) -> None:
 		print(f"Connecting to MPD server {host}:{port}...")
 		await self.client.connect(host, port)
 		if password is not None:
@@ -89,15 +94,15 @@
 		song = mpd_current_to_song(status, current, art)
 		print(song)
 		listener.update(song)
 
 	async def readpicture(self, file: str) -> bytes | None:
 		try:
 			readpic = await self.client.readpicture(file)
-			return readpic["binary"]
+			return readpic.get("binary")
 		except CommandError:
 			return None
 
 	async def on_play_pause(self) -> PlaybackState:
 		# python-mpd2 has direct support for toggling the play/pause state by
 		# calling MPDClient.pause(None), but it doesn't tell you the final
 		# state, and we also want to support playing from stopped, so we need
```

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/logo.svg` & `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/logo.svg`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/mpd/types.py` & `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/types.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.0.1/src/mpd_now_playable/song.py` & `mpd_now_playable-1.1.0/src/mpd_now_playable/song.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @define
 class Song:
 	state: PlaybackState
 	queue_index: int
 	queue_length: int
 	file: Path
 	musicbrainz_trackid: UUID | None
+	musicbrainz_releasetrackid: UUID | None
 	title: str | None
 	artist: str | None
 	composer: str | None
 	album: str | None
 	album_artist: str | None
 	track: int | None
 	disc: int | None
```

### Comparing `mpd_now_playable-1.0.1/PKG-INFO` & `mpd_now_playable-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-now-playable
-Version: 1.0.1
+Version: 1.1.0
 Summary: Expose your MPD server as a 'now playable' app on MacOS
 Author-Email: Danielle McLean <dani@00dani.me>
 License: MIT
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.12
@@ -12,17 +12,25 @@
 Project-URL: Homepage, https://git.00dani.me/00dani/mpd-now-playable
 Project-URL: Issues, https://git.00dani.me/00dani/mpd-now-playable/issues
 Requires-Python: >=3.12
 Requires-Dist: aiocache>=0.12.2
 Requires-Dist: attrs>=23.1.0
 Requires-Dist: pyobjc-framework-MediaPlayer>=10.0
 Requires-Dist: python-mpd2>=3.1.0
+Requires-Dist: aiocache[redis]; extra == "redis"
+Requires-Dist: aiocache[memcached]; extra == "memcached"
+Requires-Dist: ormsgpack>=1.5.0; extra == "msgpack"
+Requires-Dist: mpd-now-playable[memcached,msgpack,redis]; extra == "all"
+Provides-Extra: redis
+Provides-Extra: memcached
+Provides-Extra: msgpack
+Provides-Extra: all
 Description-Content-Type: text/markdown
 
-# mpd-now-playable
+# mpd-now-playable [![PyPI version](https://badge.fury.io/py/mpd-now-playable.svg)](https://badge.fury.io/py/mpd-now-playable)
 
 This little Python program turns your MPD server into a [now playable app](https://developer.apple.com/documentation/mediaplayer/becoming_a_now_playable_app) on MacOS.
 This enables your keyboard's standard media keys to control MPD, as well as more esoteric music control methods like the buttons on your Bluetooth headphones.
 
 ## Installation
 
 The recommended way to install mpd-now-playable and its dependencies is with [pipx](https://pypa.github.io/pipx/):
```

