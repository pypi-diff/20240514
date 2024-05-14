# Comparing `tmp/songs_to_youtube-0.12.8.tar.gz` & `tmp/songs_to_youtube-0.12.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songs_to_youtube-0.12.8.tar", max compression
+gzip compressed data, was "songs_to_youtube-0.12.9.tar", max compression
```

## Comparing `songs_to_youtube-0.12.8.tar` & `songs_to_youtube-0.12.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     4161 2023-12-19 01:00:20.619261 songs_to_youtube-0.12.8/README.md
--rw-r--r--   0        0        0      593 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/pyproject.toml
--rw-r--r--   0        0        0      111 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/commands/concat/concat.command
--rw-r--r--   0        0        0      429 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/commands/render/blurred background.command
--rw-r--r--   0        0        0      185 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/commands/render/no background.command
--rw-r--r--   0        0        0      324 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/commands/render/solid color background.command
--rw-r--r--   0        0        0      439 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/commands/render/vertical blurred background.command
--rw-r--r--   0        0        0     1301 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/config/default.ini
--rw-r--r--   0        0        0      484 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/const.py
--rw-r--r--   0        0        0     7782 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/field.py
--rw-r--r--   0        0        0     5773 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/image/default.jpg
--rw-r--r--   0        0        0    74285 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/image/icon.ico
--rw-r--r--   0        0        0     2426 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/image/multiple-values.png
--rw-r--r--   0        0        0     4243 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/log.py
--rw-r--r--   0        0        0     7106 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/main.py
--rw-r--r--   0        0        0     3039 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/metadata.py
--rw-r--r--   0        0        0      912 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/metadata_table_widget.py
--rw-r--r--   0        0        0     2718 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/progress_window.py
--rw-r--r--   0        0        0    11011 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/render.py
--rw-r--r--   0        0        0    11072 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/settings.py
--rw-r--r--   0        0        0     9075 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/song_settings_widget.py
--rw-r--r--   0        0        0    10782 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/song_tree_widget.py
--rw-r--r--   0        0        0    12297 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/song_tree_widget_item.py
--rw-r--r--   0        0        0     1577 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/template.py
--rw-r--r--   0        0        0     4414 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/ui/adduser.ui
--rw-r--r--   0        0        0     6725 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/ui/mainwindow.ui
--rw-r--r--   0        0        0     3391 2023-12-19 01:00:20.623261 songs_to_youtube-0.12.8/songs_to_youtube/ui/metadata.ui
--rw-r--r--   0        0        0    18470 2023-12-19 01:00:20.627261 songs_to_youtube-0.12.8/songs_to_youtube/ui/settingswindow.ui
--rw-r--r--   0        0        0    12376 2023-12-19 01:00:20.627261 songs_to_youtube-0.12.8/songs_to_youtube/ui/songsettingswindow.ui
--rw-r--r--   0        0        0    10736 2023-12-19 01:00:20.627261 songs_to_youtube-0.12.8/songs_to_youtube/upload.py
--rw-r--r--   0        0        0     5609 2023-12-19 01:00:20.627261 songs_to_youtube-0.12.8/songs_to_youtube/utils.py
--rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 songs_to_youtube-0.12.8/PKG-INFO
+-rw-r--r--   0        0        0     4161 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/README.md
+-rw-r--r--   0        0        0      593 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/commands/concat/concat.command
+-rw-r--r--   0        0        0      429 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/commands/render/blurred background.command
+-rw-r--r--   0        0        0      185 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/commands/render/no background.command
+-rw-r--r--   0        0        0      324 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/commands/render/solid color background.command
+-rw-r--r--   0        0        0      439 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/commands/render/vertical blurred background.command
+-rw-r--r--   0        0        0     1301 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/config/default.ini
+-rw-r--r--   0        0        0      484 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/const.py
+-rw-r--r--   0        0        0     7782 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/field.py
+-rw-r--r--   0        0        0     5773 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/image/default.jpg
+-rw-r--r--   0        0        0    74285 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/image/icon.ico
+-rw-r--r--   0        0        0     2426 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/image/multiple-values.png
+-rw-r--r--   0        0        0     4243 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/log.py
+-rw-r--r--   0        0        0     7106 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/main.py
+-rw-r--r--   0        0        0     3039 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/metadata.py
+-rw-r--r--   0        0        0      912 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/metadata_table_widget.py
+-rw-r--r--   0        0        0     2718 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/progress_window.py
+-rw-r--r--   0        0        0    11011 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/render.py
+-rw-r--r--   0        0        0    11072 2023-12-19 01:45:57.306546 songs_to_youtube-0.12.9/songs_to_youtube/settings.py
+-rw-r--r--   0        0        0     9075 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/song_settings_widget.py
+-rw-r--r--   0        0        0    10782 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/song_tree_widget.py
+-rw-r--r--   0        0        0    12297 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/song_tree_widget_item.py
+-rw-r--r--   0        0        0     1577 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/template.py
+-rw-r--r--   0        0        0     4414 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/ui/adduser.ui
+-rw-r--r--   0        0        0     6725 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/ui/mainwindow.ui
+-rw-r--r--   0        0        0     3391 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/ui/metadata.ui
+-rw-r--r--   0        0        0    18470 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/ui/settingswindow.ui
+-rw-r--r--   0        0        0    12376 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/ui/songsettingswindow.ui
+-rw-r--r--   0        0        0    10736 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/upload.py
+-rw-r--r--   0        0        0     5609 2023-12-19 01:45:57.310546 songs_to_youtube-0.12.9/songs_to_youtube/utils.py
+-rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 songs_to_youtube-0.12.9/PKG-INFO
```

### Comparing `songs_to_youtube-0.12.8/README.md` & `songs_to_youtube-0.12.9/README.md`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/pyproject.toml` & `songs_to_youtube-0.12.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "songs-to-youtube"
-version = "0.12.8"
+version = "0.12.9"
 description = "Application to upload songs to YouTube"
 authors = ["7x11x13 <x7x11x13@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 songs-to-youtube = "songs_to_youtube.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.8, <3.13"
 mutagen = "^1.47.0"
 pathvalidate = "^3.2.0"
 psutil = "^5.9.6"
 pyside6 = "^6.6.0"
-youtube-up = "^0.3.5"
+youtube-up = "^0.3.6"
 
 [tool.poetry.group.build]
 optional = true
 
 [tool.poetry.group.build.dependencies]
 pyinstaller = "^6.2.0"
```

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/config/default.ini` & `songs_to_youtube-0.12.9/songs_to_youtube/config/default.ini`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/field.py` & `songs_to_youtube-0.12.9/songs_to_youtube/field.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/image/default.jpg` & `songs_to_youtube-0.12.9/songs_to_youtube/image/default.jpg`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/image/icon.ico` & `songs_to_youtube-0.12.9/songs_to_youtube/image/icon.ico`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/image/multiple-values.png` & `songs_to_youtube-0.12.9/songs_to_youtube/image/multiple-values.png`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/log.py` & `songs_to_youtube-0.12.9/songs_to_youtube/log.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/main.py` & `songs_to_youtube-0.12.9/songs_to_youtube/main.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/metadata.py` & `songs_to_youtube-0.12.9/songs_to_youtube/metadata.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/metadata_table_widget.py` & `songs_to_youtube-0.12.9/songs_to_youtube/metadata_table_widget.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/progress_window.py` & `songs_to_youtube-0.12.9/songs_to_youtube/progress_window.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/render.py` & `songs_to_youtube-0.12.9/songs_to_youtube/render.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/settings.py` & `songs_to_youtube-0.12.9/songs_to_youtube/settings.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/song_settings_widget.py` & `songs_to_youtube-0.12.9/songs_to_youtube/song_settings_widget.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/song_tree_widget.py` & `songs_to_youtube-0.12.9/songs_to_youtube/song_tree_widget.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/song_tree_widget_item.py` & `songs_to_youtube-0.12.9/songs_to_youtube/song_tree_widget_item.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/template.py` & `songs_to_youtube-0.12.9/songs_to_youtube/template.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/ui/adduser.ui` & `songs_to_youtube-0.12.9/songs_to_youtube/ui/adduser.ui`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/ui/mainwindow.ui` & `songs_to_youtube-0.12.9/songs_to_youtube/ui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/ui/metadata.ui` & `songs_to_youtube-0.12.9/songs_to_youtube/ui/metadata.ui`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/ui/settingswindow.ui` & `songs_to_youtube-0.12.9/songs_to_youtube/ui/settingswindow.ui`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/ui/songsettingswindow.ui` & `songs_to_youtube-0.12.9/songs_to_youtube/ui/songsettingswindow.ui`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/upload.py` & `songs_to_youtube-0.12.9/songs_to_youtube/upload.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/songs_to_youtube/utils.py` & `songs_to_youtube-0.12.9/songs_to_youtube/utils.py`

 * *Files identical despite different names*

### Comparing `songs_to_youtube-0.12.8/PKG-INFO` & `songs_to_youtube-0.12.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: songs-to-youtube
-Version: 0.12.8
+Version: 0.12.9
 Summary: Application to upload songs to YouTube
 Author: 7x11x13
 Author-email: x7x11x13@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mutagen (>=1.47.0,<2.0.0)
 Requires-Dist: pathvalidate (>=3.2.0,<4.0.0)
 Requires-Dist: psutil (>=5.9.6,<6.0.0)
 Requires-Dist: pyside6 (>=6.6.0,<7.0.0)
-Requires-Dist: youtube-up (>=0.3.5,<0.4.0)
+Requires-Dist: youtube-up (>=0.3.6,<0.4.0)
 Description-Content-Type: text/markdown
 
 <img align="left" width="100" height="100" src="https://raw.githubusercontent.com/7x11x13/songs-to-youtube/master/songs_to_youtube/image/icon.ico" alt="icon">
 
 # songs-to-youtube
 
 Convert audio files to videos and upload them to YouTube automatically.
```

