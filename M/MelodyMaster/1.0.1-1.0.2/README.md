# Comparing `tmp/melodymaster-1.0.1.tar.gz` & `tmp/melodymaster-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melodymaster-1.0.1.tar", max compression
+gzip compressed data, was "melodymaster-1.0.2.tar", max compression
```

## Comparing `melodymaster-1.0.1.tar` & `melodymaster-1.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1062 2024-05-14 22:33:58.433222 melodymaster-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      564 2024-05-14 06:11:08.000000 melodymaster-1.0.1/MelodyMaster/__init__.py
--rw-r--r--   0        0        0    11260 2024-05-13 08:25:58.000000 melodymaster-1.0.1/MelodyMaster/algorithm.py
--rw-r--r--   0        0        0    21200 2024-05-13 11:35:13.000000 melodymaster-1.0.1/MelodyMaster/api.py
--rw-r--r--   0        0        0       36 2024-05-13 23:18:40.000000 melodymaster-1.0.1/MelodyMaster/cil/__init__.py
--rw-r--r--   0        0        0     3247 2024-05-15 04:03:32.365669 melodymaster-1.0.1/MelodyMaster/cil/_cil.py
--rw-r--r--   0        0        0     2263 2024-05-14 16:08:40.000000 melodymaster-1.0.1/MelodyMaster/client.py
--rw-r--r--   0        0        0     5185 2024-05-14 16:08:18.000000 melodymaster-1.0.1/MelodyMaster/converter.py
--rw-r--r--   0        0        0        0 2024-05-13 08:25:36.000000 melodymaster-1.0.1/MelodyMaster/deprecated/__init__.py
--rw-r--r--   0        0        0      712 2024-05-13 08:25:19.000000 melodymaster-1.0.1/MelodyMaster/deprecated/decorator.py
--rw-r--r--   0        0        0     1015 2024-05-13 08:25:32.000000 melodymaster-1.0.1/MelodyMaster/enums.py
--rw-r--r--   0        0        0      253 2024-05-13 08:25:31.000000 melodymaster-1.0.1/MelodyMaster/exceptions.py
--rw-r--r--   0        0        0     3458 2024-05-13 08:25:17.000000 melodymaster-1.0.1/MelodyMaster/factory.py
--rw-r--r--   0        0        0     1558 2024-05-14 16:08:30.000000 melodymaster-1.0.1/MelodyMaster/factory_misc.py
--rw-r--r--   0        0        0        0 2024-05-13 08:25:18.000000 melodymaster-1.0.1/MelodyMaster/interfaces/__init__.py
--rw-r--r--   0        0        0      318 2024-05-13 08:25:59.000000 melodymaster-1.0.1/MelodyMaster/interfaces/client.py
--rw-r--r--   0        0        0      109 2024-05-14 16:08:01.000000 melodymaster-1.0.1/MelodyMaster/loggers.py
--rw-r--r--   0        0        0     4097 2024-05-14 16:06:48.000000 melodymaster-1.0.1/MelodyMaster/MelodyMaster.py
--rw-r--r--   0        0        0     2695 2024-05-14 16:11:11.000000 melodymaster-1.0.1/MelodyMaster/misc.py
--rw-r--r--   0        0        0     4758 2024-05-13 08:25:12.000000 melodymaster-1.0.1/MelodyMaster/musix_match_api.py
--rw-r--r--   0        0        0     1417 2024-05-13 08:25:51.000000 melodymaster-1.0.1/MelodyMaster/Musix_spot.py
--rw-r--r--   0        0        0     7870 2024-05-14 08:20:51.000000 melodymaster-1.0.1/MelodyMaster/Muxis.py
--rw-r--r--   0        0        0        0 2024-05-13 08:25:21.000000 melodymaster-1.0.1/MelodyMaster/schemas/__init__.py
--rw-r--r--   0        0        0      830 2024-05-14 16:09:21.000000 melodymaster-1.0.1/MelodyMaster/schemas/album.py
--rw-r--r--   0        0        0        0 2024-05-13 08:25:16.000000 melodymaster-1.0.1/MelodyMaster/schemas/artist/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 08:26:04.000000 melodymaster-1.0.1/MelodyMaster/schemas/artist/views/__init__.py
--rw-r--r--   0        0        0     2107 2024-05-14 16:10:08.000000 melodymaster-1.0.1/MelodyMaster/schemas/artist/views/full_albums.py
--rw-r--r--   0        0        0     1510 2024-05-14 16:10:00.000000 melodymaster-1.0.1/MelodyMaster/schemas/artist/views/last_release.py
--rw-r--r--   0        0        0     1318 2024-05-14 16:10:24.000000 melodymaster-1.0.1/MelodyMaster/schemas/artist/views/simular_artists.py
--rw-r--r--   0        0        0     1429 2024-05-14 16:10:16.000000 melodymaster-1.0.1/MelodyMaster/schemas/artist/views/top_music.py
--rw-r--r--   0        0        0     1779 2024-05-14 16:09:52.000000 melodymaster-1.0.1/MelodyMaster/schemas/artist/views/top_song.py
--rw-r--r--   0        0        0     2746 2024-05-14 16:09:14.000000 melodymaster-1.0.1/MelodyMaster/schemas/artists.py
--rw-r--r--   0        0        0      345 2024-05-13 08:25:08.000000 melodymaster-1.0.1/MelodyMaster/schemas/attributes.py
--rw-r--r--   0        0        0      725 2024-05-13 08:25:32.000000 melodymaster-1.0.1/MelodyMaster/schemas/base.py
--rw-r--r--   0        0        0      279 2024-05-13 08:25:43.000000 melodymaster-1.0.1/MelodyMaster/schemas/content_version.py
--rw-r--r--   0        0        0      464 2024-05-13 08:25:20.000000 melodymaster-1.0.1/MelodyMaster/schemas/enums.py
--rw-r--r--   0        0        0      138 2024-05-13 08:25:34.000000 melodymaster-1.0.1/MelodyMaster/schemas/errors.py
--rw-r--r--   0        0        0     4122 2024-05-13 08:25:17.000000 melodymaster-1.0.1/MelodyMaster/schemas/models.py
--rw-r--r--   0        0        0      526 2024-05-13 08:25:41.000000 melodymaster-1.0.1/MelodyMaster/schemas/photos.py
--rw-r--r--   0        0        0       88 2024-05-13 08:25:24.000000 melodymaster-1.0.1/MelodyMaster/schemas/play_params.py
--rw-r--r--   0        0        0        0 2024-05-13 08:25:14.000000 melodymaster-1.0.1/MelodyMaster/schemas/playlist/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-14 16:09:33.000000 melodymaster-1.0.1/MelodyMaster/schemas/playlist/playlist.py
--rw-r--r--   0        0        0       71 2024-05-13 08:25:14.000000 melodymaster-1.0.1/MelodyMaster/schemas/urls.py
--rw-r--r--   0        0        0     1725 2024-05-14 16:11:26.000000 melodymaster-1.0.1/MelodyMaster/serializers.py
--rw-r--r--   0        0        0     8505 2024-05-13 08:25:28.000000 melodymaster-1.0.1/MelodyMaster/signature.py
--rw-r--r--   0        0        0      645 2024-05-13 08:25:09.000000 melodymaster-1.0.1/MelodyMaster/tok.py
--rw-r--r--   0        0        0      159 2024-05-13 08:25:47.000000 melodymaster-1.0.1/MelodyMaster/typehints.py
--rw-r--r--   0        0        0    59504 2024-05-13 08:25:42.000000 melodymaster-1.0.1/MelodyMaster/user_agent.py
--rw-r--r--   0        0        0     1784 2024-05-14 16:07:50.000000 melodymaster-1.0.1/MelodyMaster/utils.py
--rw-r--r--   0        0        0     1257 2024-05-15 04:27:43.492584 melodymaster-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    20849 2024-05-15 03:50:04.659487 melodymaster-1.0.1/README.md
--rw-r--r--   0        0        0    22073 1970-01-01 00:00:00.000000 melodymaster-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-14 22:33:58.433222 melodymaster-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      564 2024-05-14 06:11:08.000000 melodymaster-1.0.2/MelodyMaster/__init__.py
+-rw-r--r--   0        0        0    11260 2024-05-13 08:25:58.000000 melodymaster-1.0.2/MelodyMaster/algorithm.py
+-rw-r--r--   0        0        0    21200 2024-05-13 11:35:13.000000 melodymaster-1.0.2/MelodyMaster/api.py
+-rw-r--r--   0        0        0       36 2024-05-13 23:18:40.000000 melodymaster-1.0.2/MelodyMaster/cil/__init__.py
+-rw-r--r--   0        0        0     3247 2024-05-15 05:40:21.936663 melodymaster-1.0.2/MelodyMaster/cil/_cil.py
+-rw-r--r--   0        0        0     2263 2024-05-14 16:08:40.000000 melodymaster-1.0.2/MelodyMaster/client.py
+-rw-r--r--   0        0        0     5185 2024-05-14 16:08:18.000000 melodymaster-1.0.2/MelodyMaster/converter.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:25:36.000000 melodymaster-1.0.2/MelodyMaster/deprecated/__init__.py
+-rw-r--r--   0        0        0      712 2024-05-13 08:25:19.000000 melodymaster-1.0.2/MelodyMaster/deprecated/decorator.py
+-rw-r--r--   0        0        0     1015 2024-05-13 08:25:32.000000 melodymaster-1.0.2/MelodyMaster/enums.py
+-rw-r--r--   0        0        0      253 2024-05-13 08:25:31.000000 melodymaster-1.0.2/MelodyMaster/exceptions.py
+-rw-r--r--   0        0        0     3458 2024-05-13 08:25:17.000000 melodymaster-1.0.2/MelodyMaster/factory.py
+-rw-r--r--   0        0        0     1558 2024-05-14 16:08:30.000000 melodymaster-1.0.2/MelodyMaster/factory_misc.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:25:18.000000 melodymaster-1.0.2/MelodyMaster/interfaces/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-13 08:25:59.000000 melodymaster-1.0.2/MelodyMaster/interfaces/client.py
+-rw-r--r--   0        0        0      109 2024-05-14 16:08:01.000000 melodymaster-1.0.2/MelodyMaster/loggers.py
+-rw-r--r--   0        0        0     4097 2024-05-14 16:06:48.000000 melodymaster-1.0.2/MelodyMaster/MelodyMaster.py
+-rw-r--r--   0        0        0     2695 2024-05-14 16:11:11.000000 melodymaster-1.0.2/MelodyMaster/misc.py
+-rw-r--r--   0        0        0     4758 2024-05-13 08:25:12.000000 melodymaster-1.0.2/MelodyMaster/musix_match_api.py
+-rw-r--r--   0        0        0     1417 2024-05-13 08:25:51.000000 melodymaster-1.0.2/MelodyMaster/Musix_spot.py
+-rw-r--r--   0        0        0     7864 2024-05-15 05:46:34.046100 melodymaster-1.0.2/MelodyMaster/Muxis.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:25:21.000000 melodymaster-1.0.2/MelodyMaster/schemas/__init__.py
+-rw-r--r--   0        0        0      830 2024-05-14 16:09:21.000000 melodymaster-1.0.2/MelodyMaster/schemas/album.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:25:16.000000 melodymaster-1.0.2/MelodyMaster/schemas/artist/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:26:04.000000 melodymaster-1.0.2/MelodyMaster/schemas/artist/views/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-14 16:10:08.000000 melodymaster-1.0.2/MelodyMaster/schemas/artist/views/full_albums.py
+-rw-r--r--   0        0        0     1510 2024-05-14 16:10:00.000000 melodymaster-1.0.2/MelodyMaster/schemas/artist/views/last_release.py
+-rw-r--r--   0        0        0     1318 2024-05-14 16:10:24.000000 melodymaster-1.0.2/MelodyMaster/schemas/artist/views/simular_artists.py
+-rw-r--r--   0        0        0     1429 2024-05-14 16:10:16.000000 melodymaster-1.0.2/MelodyMaster/schemas/artist/views/top_music.py
+-rw-r--r--   0        0        0     1779 2024-05-14 16:09:52.000000 melodymaster-1.0.2/MelodyMaster/schemas/artist/views/top_song.py
+-rw-r--r--   0        0        0     2746 2024-05-14 16:09:14.000000 melodymaster-1.0.2/MelodyMaster/schemas/artists.py
+-rw-r--r--   0        0        0      345 2024-05-13 08:25:08.000000 melodymaster-1.0.2/MelodyMaster/schemas/attributes.py
+-rw-r--r--   0        0        0      725 2024-05-13 08:25:32.000000 melodymaster-1.0.2/MelodyMaster/schemas/base.py
+-rw-r--r--   0        0        0      279 2024-05-13 08:25:43.000000 melodymaster-1.0.2/MelodyMaster/schemas/content_version.py
+-rw-r--r--   0        0        0      464 2024-05-13 08:25:20.000000 melodymaster-1.0.2/MelodyMaster/schemas/enums.py
+-rw-r--r--   0        0        0      138 2024-05-13 08:25:34.000000 melodymaster-1.0.2/MelodyMaster/schemas/errors.py
+-rw-r--r--   0        0        0     4122 2024-05-13 08:25:17.000000 melodymaster-1.0.2/MelodyMaster/schemas/models.py
+-rw-r--r--   0        0        0      526 2024-05-13 08:25:41.000000 melodymaster-1.0.2/MelodyMaster/schemas/photos.py
+-rw-r--r--   0        0        0       88 2024-05-13 08:25:24.000000 melodymaster-1.0.2/MelodyMaster/schemas/play_params.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:25:14.000000 melodymaster-1.0.2/MelodyMaster/schemas/playlist/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-14 16:09:33.000000 melodymaster-1.0.2/MelodyMaster/schemas/playlist/playlist.py
+-rw-r--r--   0        0        0       71 2024-05-13 08:25:14.000000 melodymaster-1.0.2/MelodyMaster/schemas/urls.py
+-rw-r--r--   0        0        0     1725 2024-05-14 16:11:26.000000 melodymaster-1.0.2/MelodyMaster/serializers.py
+-rw-r--r--   0        0        0     8505 2024-05-13 08:25:28.000000 melodymaster-1.0.2/MelodyMaster/signature.py
+-rw-r--r--   0        0        0      645 2024-05-13 08:25:09.000000 melodymaster-1.0.2/MelodyMaster/tok.py
+-rw-r--r--   0        0        0      159 2024-05-13 08:25:47.000000 melodymaster-1.0.2/MelodyMaster/typehints.py
+-rw-r--r--   0        0        0    59504 2024-05-13 08:25:42.000000 melodymaster-1.0.2/MelodyMaster/user_agent.py
+-rw-r--r--   0        0        0     1784 2024-05-14 16:07:50.000000 melodymaster-1.0.2/MelodyMaster/utils.py
+-rw-r--r--   0        0        0     1257 2024-05-15 05:50:11.116864 melodymaster-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    20849 2024-05-15 05:38:13.181112 melodymaster-1.0.2/README.md
+-rw-r--r--   0        0        0    22073 1970-01-01 00:00:00.000000 melodymaster-1.0.2/PKG-INFO
```

### Comparing `melodymaster-1.0.1/LICENSE.txt` & `melodymaster-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/__init__.py` & `melodymaster-1.0.2/MelodyMaster/__init__.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/algorithm.py` & `melodymaster-1.0.2/MelodyMaster/algorithm.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/api.py` & `melodymaster-1.0.2/MelodyMaster/api.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/cil/_cil.py` & `melodymaster-1.0.2/MelodyMaster/cil/_cil.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         'search_album',
         'get_default_lyrics',
         'get_alternative_lyrics',
         'recognize_text'
         'help'
     ])
     parser.add_argument('--title', type=str, help='Song title or title and artist')
-    parser.add_argument('--str', type=str, help='Whether to treat the input as a string or not')
+    parser.add_argument('--srt', type=str, help='Whether to treat the input as a string or not')
     parser.add_argument('--duration', type=str, help='Song duration')
     parser.add_argument('--artist', type=str, help='Song artist')
     parser.add_argument('--file_path', type=str, help='Path to audio file')
     parser.add_argument('--album_id', type=int, help='Album id')
     parser.add_argument('--artist_id', type=int, help='Album id')
     parser.add_argument('--lang', type=int, help='lang')
 
@@ -52,24 +52,24 @@
 
     if args.command == 'get_default_lyrics':
         if args.title is None:
             print("Error: Missing song title.")
             print_help()
             return
 
-        asyncio.run(get_default_lyrics(args.title, args.str or "true"))
+        asyncio.run(get_default_lyrics(args.title, args.srt or "true"))
         return
 
     if args.command == 'get_alternative_lyrics':
         if args.title is None:
             print("Error: Missing song title.")
             print_help()
             return
 
-        asyncio.run(get_alternative_lyrics(args.title, args.artist or "", args.duration or "", args.str or "true"))
+        asyncio.run(get_alternative_lyrics(args.title, args.artist or "", args.duration or "", args.srt or "true"))
         return
 
     if args.command == 'recognize_text':
         if args.file_path is None:
             print("Error: Missing audio file_path.")
             print_help()
             return
```

### Comparing `melodymaster-1.0.1/MelodyMaster/client.py` & `melodymaster-1.0.2/MelodyMaster/client.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/converter.py` & `melodymaster-1.0.2/MelodyMaster/converter.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/deprecated/decorator.py` & `melodymaster-1.0.2/MelodyMaster/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/enums.py` & `melodymaster-1.0.2/MelodyMaster/enums.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/factory.py` & `melodymaster-1.0.2/MelodyMaster/factory.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/factory_misc.py` & `melodymaster-1.0.2/MelodyMaster/factory_misc.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/MelodyMaster.py` & `melodymaster-1.0.2/MelodyMaster/MelodyMaster.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/misc.py` & `melodymaster-1.0.2/MelodyMaster/misc.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/musix_match_api.py` & `melodymaster-1.0.2/MelodyMaster/musix_match_api.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/Musix_spot.py` & `melodymaster-1.0.2/MelodyMaster/Musix_spot.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/Muxis.py` & `melodymaster-1.0.2/MelodyMaster/Muxis.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from collections import OrderedDict
 import json
 import os
 import speech_recognition as sr
 from pydub import AudioSegment
 musix = Musix()
 black_space = ['"""""', '', '♪', ' """""']
-author = 'https://OverGroundOfWall.t.me'
+author = 'https://t.me/BDXBB.t.me'
 
 async def get_default_lyrics(query, srt):
     try: 
         dic = OrderedDict({'lyrics': ""})
         dic['info'] = {
-            'Dev': '~ ZHAN',
+            'Dev': 'SILVER',
             'my_account': f'{author}'  
         }
         track_id = musix.search_track(query)
         response = musix.get_lyrics(track_id)
         for line in response.strip().splitlines():
             match = re.findall(r'\[(.*?)\](.*?)$', line)
             time, content = match[0][0].split('.')[0], match[0][1]
@@ -37,29 +37,29 @@
 async def get_alternative_lyrics(title,artist,duration,srt):
     print(srt)
     if srt == 'false' or srt == None or srt == '' or srt == ' ':
         try:
             if duration or ':' in [duration]:
                 dic = OrderedDict({'lyrics':[]})
                 dic['info'] = {
-                    'Dev':'~ ZHAN',
+                    'Dev':'SILVER',
                     'my_account':f'{author}'  
                     }
                 lyrics = musix.get_lyrics_alternative(title, artist, convert_duration(duration))
                 for lyr in lyrics.strip().splitlines():
                     match = re.findall(r'\[(.*?)\](.*?)$', lyr)
                     time, content = match[0][0].split('.')[0], match[0][1]
                     time = time[-4:] if time[0] == '0' else time
                     if content not in black_space:
                         dic['lyrics'].append({time:content})
                 return print(dic)
             else:
                 dic = OrderedDict({'lyrics':[]})
                 dic['info'] = {
-                    'Dev':'~ ZHAN',
+                    'Dev':'SILVER',
                     'my_account':f'{author}'  
                     }
                 lyrics = musix.get_lyrics_alternative(title,artist)
                 for lyr in lyrics.strip().splitlines():
                     match = re.findall(r'\[(.*?)\](.*?)$', lyr)
                     time, content = match[0][0].split('.')[0], match[0][1]
                     time = time[-4:] if time[0] == '0' else time
```

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/album.py` & `melodymaster-1.0.2/MelodyMaster/schemas/album.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/artist/views/full_albums.py` & `melodymaster-1.0.2/MelodyMaster/schemas/artist/views/full_albums.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/artist/views/last_release.py` & `melodymaster-1.0.2/MelodyMaster/schemas/artist/views/last_release.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/artist/views/simular_artists.py` & `melodymaster-1.0.2/MelodyMaster/schemas/artist/views/simular_artists.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/artist/views/top_music.py` & `melodymaster-1.0.2/MelodyMaster/schemas/artist/views/top_music.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/artist/views/top_song.py` & `melodymaster-1.0.2/MelodyMaster/schemas/artist/views/top_song.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/artists.py` & `melodymaster-1.0.2/MelodyMaster/schemas/artists.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/base.py` & `melodymaster-1.0.2/MelodyMaster/schemas/base.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/models.py` & `melodymaster-1.0.2/MelodyMaster/schemas/models.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/photos.py` & `melodymaster-1.0.2/MelodyMaster/schemas/photos.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/schemas/playlist/playlist.py` & `melodymaster-1.0.2/MelodyMaster/schemas/playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/serializers.py` & `melodymaster-1.0.2/MelodyMaster/serializers.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/signature.py` & `melodymaster-1.0.2/MelodyMaster/signature.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/tok.py` & `melodymaster-1.0.2/MelodyMaster/tok.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/user_agent.py` & `melodymaster-1.0.2/MelodyMaster/user_agent.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/MelodyMaster/utils.py` & `melodymaster-1.0.2/MelodyMaster/utils.py`

 * *Files identical despite different names*

### Comparing `melodymaster-1.0.1/pyproject.toml` & `melodymaster-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MelodyMaster"
-version = "1.0.1"
+version = "1.0.2"
 description = "Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp."
 authors = ["BKXBB"]
 license = "MIT License"
 keywords = ["python", "shazam", "music", "recognize", "api", "async", "asyncio", "aiohttp", "identification"]
 readme = "README.md"
 homepage = "https://github.com/BDXBB/MelodyMaster"
 repository = "https://github.com/BDXBB/MelodyMaster"
```

### Comparing `melodymaster-1.0.1/README.md` & `melodymaster-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
    ```
    This example means you want to get the lyrics of the song titled "Song Title" and --srt if true give you lyrics with time if --srt false just lyrics
    
 6 .**get_alternative_lyrics**: Used to get alternative lyrics of a song.
 
    Example:
    ```
-   MelodyMaster get_alternative_lyrics --title "Song Title" --artist "Artist Name" --duration "Duration" --str "true"
+   MelodyMaster get_alternative_lyrics --title "Song Title" --artist "Artist Name" --duration "Duration" --srt "true"
    ```
    This example means you want to get the alternative lyrics of the song titled "Song Title" by the artist "Artist Name" with duration "Duration". duration and Artist name optional
 
  7. **recognize_text**: Used to recognize text from an audio file.
 
    Example:
    ```
```

#### html2text {}

```diff
@@ -123,15 +123,15 @@
 ID. Example: ``` MelodyMaster search_album --album_id 123 ``` This example
 searches for the album with the ID 123. 5 .**get_default_lyrics**: Used to get
 the default lyrics of a song. Example: ``` MelodyMaster get_default_lyrics --
 title "Song Title" --srt "true" ``` This example means you want to get the
 lyrics of the song titled "Song Title" and --srt if true give you lyrics with
 time if --srt false just lyrics 6 .**get_alternative_lyrics**: Used to get
 alternative lyrics of a song. Example: ``` MelodyMaster get_alternative_lyrics
---title "Song Title" --artist "Artist Name" --duration "Duration" --str "true"
+--title "Song Title" --artist "Artist Name" --duration "Duration" --srt "true"
 ``` This example means you want to get the alternative lyrics of the song
 titled "Song Title" by the artist "Artist Name" with duration "Duration".
 duration and Artist name optional 7. **recognize_text**: Used to recognize text
 from an audio file. Example: ``` MelodyMaster recognize_text --file_path "path/
 to/audio_file" --lang "en-GB" ``` This example means you want to recognize the
 text from the audio file located at "path/to/audio_file" the lang for language
 you can find it . here Afrikaans (South Africa) : af-ZA Albanian (Albania) :
```

### Comparing `melodymaster-1.0.1/PKG-INFO` & `melodymaster-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MelodyMaster
-Version: 1.0.1
+Version: 1.0.2
 Summary: Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp.
 Home-page: https://github.com/BDXBB/MelodyMaster
 License: MIT
 Keywords: python,shazam,music,recognize,api,async,asyncio,aiohttp,identification
 Author: BKXBB
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -487,15 +487,15 @@
    ```
    This example means you want to get the lyrics of the song titled "Song Title" and --srt if true give you lyrics with time if --srt false just lyrics
    
 6 .**get_alternative_lyrics**: Used to get alternative lyrics of a song.
 
    Example:
    ```
-   MelodyMaster get_alternative_lyrics --title "Song Title" --artist "Artist Name" --duration "Duration" --str "true"
+   MelodyMaster get_alternative_lyrics --title "Song Title" --artist "Artist Name" --duration "Duration" --srt "true"
    ```
    This example means you want to get the alternative lyrics of the song titled "Song Title" by the artist "Artist Name" with duration "Duration". duration and Artist name optional
 
  7. **recognize_text**: Used to recognize text from an audio file.
 
    Example:
    ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MelodyMaster Version: 1.0.1 Summary: Is a
+Metadata-Version: 2.1 Name: MelodyMaster Version: 1.0.2 Summary: Is a
 asynchronous framework from reverse engineered Shazam API written in Python
 3.8+ with asyncio and aiohttp. Home-page: https://github.com/BDXBB/MelodyMaster
 License: MIT Keywords:
 python,shazam,music,recognize,api,async,asyncio,aiohttp,identification Author:
 BKXBB Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -140,15 +140,15 @@
 ID. Example: ``` MelodyMaster search_album --album_id 123 ``` This example
 searches for the album with the ID 123. 5 .**get_default_lyrics**: Used to get
 the default lyrics of a song. Example: ``` MelodyMaster get_default_lyrics --
 title "Song Title" --srt "true" ``` This example means you want to get the
 lyrics of the song titled "Song Title" and --srt if true give you lyrics with
 time if --srt false just lyrics 6 .**get_alternative_lyrics**: Used to get
 alternative lyrics of a song. Example: ``` MelodyMaster get_alternative_lyrics
---title "Song Title" --artist "Artist Name" --duration "Duration" --str "true"
+--title "Song Title" --artist "Artist Name" --duration "Duration" --srt "true"
 ``` This example means you want to get the alternative lyrics of the song
 titled "Song Title" by the artist "Artist Name" with duration "Duration".
 duration and Artist name optional 7. **recognize_text**: Used to recognize text
 from an audio file. Example: ``` MelodyMaster recognize_text --file_path "path/
 to/audio_file" --lang "en-GB" ``` This example means you want to recognize the
 text from the audio file located at "path/to/audio_file" the lang for language
 you can find it . here Afrikaans (South Africa) : af-ZA Albanian (Albania) :
```

