# Comparing `tmp/mixvideoconcat-1.1.0.tar.gz` & `tmp/mixvideoconcat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixvideoconcat-1.1.0.tar", last modified: Sun Apr 28 00:06:54 2024, max compression
+gzip compressed data, was "mixvideoconcat-1.2.0.tar", last modified: Tue May 14 20:58:07 2024, max compression
```

## Comparing `mixvideoconcat-1.1.0.tar` & `mixvideoconcat-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-04-23 19:28:35.000000 mixvideoconcat-1.1.0/LICENSE
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    43710 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1845 2024-04-23 21:17:06.000000 mixvideoconcat-1.1.0/README.md
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1481 2024-04-28 00:05:28.000000 mixvideoconcat-1.1.0/pyproject.toml
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/setup.cfg
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.935247 mixvideoconcat-1.1.0/src/
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.983247 mixvideoconcat-1.1.0/src/mixvideoconcat/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     3187 2024-04-26 18:47:18.000000 mixvideoconcat-1.1.0/src/mixvideoconcat/__init__.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     8475 2024-04-26 19:19:15.000000 mixvideoconcat-1.1.0/src/mixvideoconcat/concat.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-04-23 21:00:36.000000 mixvideoconcat-1.1.0/src/mixvideoconcat/log.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    43710 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      331 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/SOURCES.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/dependency_links.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       55 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/entry_points.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       15 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/top_level.txt
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 20:58:07.881780 mixvideoconcat-1.2.0/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-04-23 19:28:35.000000 mixvideoconcat-1.2.0/LICENSE
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    44182 2024-05-14 20:58:07.881780 mixvideoconcat-1.2.0/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2317 2024-05-14 20:48:51.000000 mixvideoconcat-1.2.0/README.md
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1481 2024-05-14 20:57:00.000000 mixvideoconcat-1.2.0/pyproject.toml
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-05-14 20:58:07.881780 mixvideoconcat-1.2.0/setup.cfg
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 20:58:07.881780 mixvideoconcat-1.2.0/src/
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 20:58:07.881780 mixvideoconcat-1.2.0/src/mixvideoconcat/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     3588 2024-05-14 20:39:28.000000 mixvideoconcat-1.2.0/src/mixvideoconcat/__init__.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     9594 2024-05-14 20:29:37.000000 mixvideoconcat-1.2.0/src/mixvideoconcat/concat.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-04-23 21:00:36.000000 mixvideoconcat-1.2.0/src/mixvideoconcat/log.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 20:58:07.881780 mixvideoconcat-1.2.0/src/mixvideoconcat.egg-info/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    44182 2024-05-14 20:58:07.000000 mixvideoconcat-1.2.0/src/mixvideoconcat.egg-info/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      331 2024-05-14 20:58:07.000000 mixvideoconcat-1.2.0/src/mixvideoconcat.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-05-14 20:58:07.000000 mixvideoconcat-1.2.0/src/mixvideoconcat.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       55 2024-05-14 20:58:07.000000 mixvideoconcat-1.2.0/src/mixvideoconcat.egg-info/entry_points.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       15 2024-05-14 20:58:07.000000 mixvideoconcat-1.2.0/src/mixvideoconcat.egg-info/top_level.txt
```

### Comparing `mixvideoconcat-1.1.0/LICENSE` & `mixvideoconcat-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mixvideoconcat-1.1.0/PKG-INFO` & `mixvideoconcat-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixvideoconcat
-Version: 1.1.0
+Version: 1.2.0
 Summary: Mixed videos concatenator
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -731,14 +731,18 @@
 options:
   -h, --help            show this help message and exit
   -t TMPDIR, --tmpdir TMPDIR
                         Directory for temprary files (they can be huge!)
   -l LOGFILE, --logfile LOGFILE
                         Log file
   -f, --force           Overwrite existing
+  --deinterlace {on,off,auto}
+                        Deinterlace mode (default: auto)
+  --stabilize {on,off}  Stabilize mode (default: on)
+  -v, --verbose         Print verbose information (ffmpeg output)
 ```
 
 ## Example
 
 Concatenate three video files (video1.mp4, video2.mov, video3.avi) into a single video file named output.mp4:
 
 ```bash
@@ -749,13 +753,19 @@
 
 ```python
 from mixvideoconcat import concat
 
 concat(['video1.mp4', 'video2.mov', 'video3.avi'], 'output.mp4')
 ```
 
+## Tune
+
+You can override the default constant rate factor (CRF) of 23 by setting the `FFMPEG_CRF` environment variable.
+The frame rate will be determined as the maximum frame rate among the source files.
+To override this, use the `FFMPEG_FR` environment variable.
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.
 
 ## Show your support
 Give a ⭐️ if this project helped you!
```

### Comparing `mixvideoconcat-1.1.0/README.md` & `mixvideoconcat-1.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 options:
   -h, --help            show this help message and exit
   -t TMPDIR, --tmpdir TMPDIR
                         Directory for temprary files (they can be huge!)
   -l LOGFILE, --logfile LOGFILE
                         Log file
   -f, --force           Overwrite existing
+  --deinterlace {on,off,auto}
+                        Deinterlace mode (default: auto)
+  --stabilize {on,off}  Stabilize mode (default: on)
+  -v, --verbose         Print verbose information (ffmpeg output)
 ```
 
 ## Example
 
 Concatenate three video files (video1.mp4, video2.mov, video3.avi) into a single video file named output.mp4:
 
 ```bash
@@ -45,13 +49,19 @@
 
 ```python
 from mixvideoconcat import concat
 
 concat(['video1.mp4', 'video2.mov', 'video3.avi'], 'output.mp4')
 ```
 
+## Tune
+
+You can override the default constant rate factor (CRF) of 23 by setting the `FFMPEG_CRF` environment variable.
+The frame rate will be determined as the maximum frame rate among the source files.
+To override this, use the `FFMPEG_FR` environment variable.
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.
 
 ## Show your support
 Give a ⭐️ if this project helped you!
```

### Comparing `mixvideoconcat-1.1.0/pyproject.toml` & `mixvideoconcat-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mixvideoconcat"
-version = "1.1.0"
+version = "1.2.0"
 description = "Mixed videos concatenator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["video", "concatenate", "tool", "ffmpeg"]
 
 authors = [
```

### Comparing `mixvideoconcat-1.1.0/src/mixvideoconcat/__init__.py` & `mixvideoconcat-1.2.0/src/mixvideoconcat/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 # pylint: disable=broad-exception-caught
 
 """
 MixVideoConcat Script
 
 This script provides a command-line interface for concatenating video files into
 a single video file.
-
-Example:
-    Concatenate video files "video1.mp4", "video2.mov", "video3.avi"
-    into a single video file "output.mp4":
-    $ mixvideoconcat video1.mp4 video2.mov video3.avi output.mp4
 """
 
 import os
 import sys
 import logging
 import argparse
 import tempfile
 
 from .concat import *
 from .log import init_logger
 
 
+DESCRIPTION = """
+Concatenatenite video files into a single video file.
+
+Example:
+    Concatenate video files "video1.mp4", "video2.mov", "video3.avi"
+    into a single video file "output.mp4":
+    $ mixvideoconcat video1.mp4 video2.mov video3.avi output.mp4
+
+You can override the default constant rate factor (CRF) of 23 by setting the FFMPEG_CRF environment variable.
+The frame rate will be determined as the maximum frame rate among the source files.
+To override this, use the FFMPEG_FR environment variable.
+"""
+
+
 def __deinterlace_mode(value):
     if value == "on":
         return True
     if value == "off":
         return False
     if value == "auto":
         return None
@@ -38,26 +47,26 @@
         return True
     if value == "off":
         return False
     raise argparse.ArgumentTypeError(f"Invalid stabilize mode: {value}")
 
 
 def __args_parse():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        description=DESCRIPTION, formatter_class=argparse.RawTextHelpFormatter
+    )
     parser.add_argument("sources", nargs="+", help="Source files")
     parser.add_argument("destination", help="Destination file")
     parser.add_argument(
         "-t",
         "--tmpdir",
         help="Directory for temprary files (they can be huge!)",
     )
     parser.add_argument("-l", "--logfile", help="Log file", default=None)
-    parser.add_argument(
-        "-f", "--force", help="Overwrite existing", action="store_true"
-    )
+    parser.add_argument("-f", "--force", help="Overwrite existing", action="store_true")
     parser.add_argument(
         "--deinterlace",
         help="Deinterlace mode (default: auto)",
         choices=["on", "off", "auto"],
         default="auto",
     )
     parser.add_argument(
```

### Comparing `mixvideoconcat-1.1.0/src/mixvideoconcat/concat.py` & `mixvideoconcat-1.2.0/src/mixvideoconcat/concat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# pylint: disable=line-too-long,too-many-arguments,too-many-locals
+# pylint: disable=line-too-long,too-many-arguments,too-many-locals,eval-used
 """
 MixVideoConcat Module
 
 This module provides functions for manipulating and concatenating video files.
 """
 
 import os
 import logging
 import subprocess
 import json
 
-FFMPEG_BINARY = "ffmpeg"
-FFMPEG_CODEC = "libx264"
-REENCODE_FPS = "25"
+FFMPEG_BINARY = os.getenv("FFMPEG_BINARY", "ffmpeg")
+FFMPEG_CODEC = os.getenv("FFMPEG_CODEC", "libx264")
+FFMPEG_CRF = os.getenv("FFMPEG_CRF", "23")  # use 18 for visually lossless file (ffmpeg default: 23)
+FFMPEG_FR = os.getenv("FFMPEG_FR", "25")
 
 
 def __unlink(filename):
     try:
         os.unlink(filename)
     except FileNotFoundError:
         logging.exception("unlink failed")
@@ -32,53 +33,42 @@
         "error",
         "-show_format",
         "-show_streams",
         "-print_format",
         "json",
         filename,
     ]
-    result = subprocess.run(
-        command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False
-    )
+    result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False)
     if result.returncode != 0:
         error_msg = result.stderr.decode("utf-8").strip()
         raise SystemError(error_msg)
 
     output = result.stdout.decode("utf-8")
     data = json.loads(output)
 
     video_stream = next(
-        (
-            stream
-            for stream in data["streams"]
-            if stream["codec_type"] == "video"
-        ),
+        (stream for stream in data["streams"] if stream["codec_type"] == "video"),
         None,
     )
     if video_stream is None:
         raise RuntimeWarning("File has no video steam")
 
     info = {
         "width": int(video_stream.get("width", 0)),
         "height": int(video_stream.get("height", 0)),
+        "frame_rate": video_stream.get("r_frame_rate", 0),
         "duration": float(data["format"]["duration"]),
-        "orientation": int(
-            video_stream.get("side_data_list", [{}])[0].get("rotation", 0)
-        ),
-        "interlaced": (
-            video_stream.get("field_order", "unknown") != "progressive"
-        ),
+        "orientation": int(video_stream.get("side_data_list", [{}])[0].get("rotation", 0)),
+        "interlaced": (video_stream.get("field_order", "unknown") != "progressive"),
     }
     logging.info("%s: %s", filename, info)
     return info
 
 
-def apply_video_filters(
-    in_file, out_file, filters, add_params=None, verbose=False
-):
+def apply_video_filters(in_file, out_file, filters, add_params=None, verbose=False):
     """
     Apply filters to a video file.
     """
     cmd = [FFMPEG_BINARY, "-y"]  # overwrite existing
     cmd += ("-i", in_file)  # input file
     cmd += ("-vf", ",".join(filters))  # filters
     if out_file is None:
@@ -129,24 +119,26 @@
         ]
         logging.info("start stab")
         apply_video_filters(in_file, out_file, filters, None, verbose)
     finally:
         __unlink(trffile)
 
 
-def resize_and_resample(in_file, out_file, w, h, verbose):
+def resize_and_resample(in_file, out_file, w, h, frame_rate, verbose):
     """
     Resize and resample a video file.
     """
+    if not frame_rate:
+        frame_rate = FFMPEG_FR
     filters = [
         "format=yuv420p",
         f"scale=w='if(gt(a,{w}/{h}),{w},trunc(oh*a/2)*2)':h='if(gt(a,{w}/{h}),trunc(ow/a/2)*2,{h})'",  # noqa
         f"pad={w}:{h}:(ow-iw)/2:(oh-ih)/2:black",
     ]
-    add_params = ["-r", REENCODE_FPS]
+    add_params = ["-r", frame_rate]
     logging.info("start resize")
     apply_video_filters(in_file, out_file, filters, add_params, verbose)
 
 
 def concat_uniform(filenames, out_file, tmpdirname, verbose):
     """
     Concatenate video files with uniform properties into a single video file.
@@ -160,15 +152,15 @@
             f.write(f"file '{fname}'\n")
 
     cmd = [FFMPEG_BINARY, "-y"]  # overwrite existing
     cmd += ("-f", "concat")
     cmd += ("-safe", "0")
     cmd += ("-i", listfile)
     cmd += ("-c:v", FFMPEG_CODEC)
-    cmd += ("-crf", "17")  # produce a visually lossless file.
+    cmd += ("-crf", FFMPEG_CRF)
     cmd += ("-bf", "2")  # limit consecutive B-frames to 2
     cmd += ("-use_editlist", "0")  # avoids writing edit lists
     # places moov atom/box at front of the output file.
     cmd += ("-movflags", "+faststart")
     # use the native encoder to produce an AAC audio stream.
     cmd += ("-c:a", "aac")
     cmd += ("-q:a", "1")  # sets the highest quality for the audio.
@@ -188,30 +180,52 @@
     finally:
         __unlink(listfile)
 
 
 def __get_info_and_size(filenames):
     max_height = 0
     max_width = 0
+    max_frame_rate = 0
+    max_frame_rate_str = ""
     fileinfos = []
     for f in filenames:
         info = get_video_info(f)
         w = info["width"]
         h = info["height"]
         if info["orientation"] not in (0, 180, -180):
             w, h = h, w
         if w > max_width:
             max_width = w
             max_height = h
+        frame_rate = eval(info["frame_rate"])
+        if frame_rate > max_frame_rate:
+            max_frame_rate = frame_rate
+            max_frame_rate_str = info["frame_rate"]
         info["name"] = f
         fileinfos.append(info)
 
     logging.info("Result video: width=%s, height=%s", max_width, max_height)
 
-    return fileinfos, max_width, max_height
+    return fileinfos, max_width, max_height, max_frame_rate_str
+
+
+def __check_is_uniform(fileinfos):
+    if len(fileinfos) == 0:
+        return True
+    finfo0 = fileinfos[0]
+    for finfo in fileinfos[1:]:
+        if (
+            finfo0["height"] != finfo["height"]
+            or finfo0["width"] != finfo["width"]
+            or finfo0["frame_rate"] != finfo["frame_rate"]
+            or finfo0["orientation"] != finfo["orientation"]
+            or finfo0["interlaced"] != finfo["interlaced"]
+        ):
+            return False
+    return True
 
 
 def concat(
     filenames,
     outputfile,
     tmpdirname="/tmp",
     deinterlace_mode=None,
@@ -232,19 +246,21 @@
         verbose (bool, optional): Enable ffmpeg output.
         dry_run (bool, optional): If True, performs a dry run without actually
             concatenating the videos. Defaults to False.
 
     Returns:
         list: Information about the concatenated video files.
     """
-    fileinfos, max_width, max_height = __get_info_and_size(filenames)
+    fileinfos, max_width, max_height, max_frame_rate_str = __get_info_and_size(filenames)
 
     if dry_run:
         return fileinfos
 
+    resize = not __check_is_uniform(fileinfos)
+
     tmpfilenames = []
 
     try:
         for i, finfo in enumerate(fileinfos):
             fname = os.path.join(tmpdirname, f"{i}.mp4")
             tfname = os.path.join(tmpdirname, f"{i}_tmp.mp4")
             src_name = finfo["name"]
@@ -259,21 +275,24 @@
                 src_name = fname
 
             if stabilize_mode:
                 stabilize(src_name, tfname, tmpdirname, verbose)
                 os.rename(tfname, fname)
                 src_name = fname
 
-            resize_and_resample(
-                src_name, tfname, max_width, max_height, verbose
-            )
-            os.rename(tfname, fname)
+            if resize:
+                resize_and_resample(
+                    src_name, tfname, max_width, max_height, max_frame_rate_str, verbose
+                )
+                os.rename(tfname, fname)
+                src_name = fname
 
-            tmpfilenames.append(fname)
+            tmpfilenames.append(src_name)
 
         concat_uniform(tmpfilenames, outputfile, tmpdirname, verbose)
 
     finally:
         for f in tmpfilenames:
-            __unlink(f)
+            if os.path.split(f)[0] == tmpdirname:
+                __unlink(f)
 
     return fileinfos
```

### Comparing `mixvideoconcat-1.1.0/src/mixvideoconcat/log.py` & `mixvideoconcat-1.2.0/src/mixvideoconcat/log.py`

 * *Files identical despite different names*

### Comparing `mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/PKG-INFO` & `mixvideoconcat-1.2.0/src/mixvideoconcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixvideoconcat
-Version: 1.1.0
+Version: 1.2.0
 Summary: Mixed videos concatenator
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -731,14 +731,18 @@
 options:
   -h, --help            show this help message and exit
   -t TMPDIR, --tmpdir TMPDIR
                         Directory for temprary files (they can be huge!)
   -l LOGFILE, --logfile LOGFILE
                         Log file
   -f, --force           Overwrite existing
+  --deinterlace {on,off,auto}
+                        Deinterlace mode (default: auto)
+  --stabilize {on,off}  Stabilize mode (default: on)
+  -v, --verbose         Print verbose information (ffmpeg output)
 ```
 
 ## Example
 
 Concatenate three video files (video1.mp4, video2.mov, video3.avi) into a single video file named output.mp4:
 
 ```bash
@@ -749,13 +753,19 @@
 
 ```python
 from mixvideoconcat import concat
 
 concat(['video1.mp4', 'video2.mov', 'video3.avi'], 'output.mp4')
 ```
 
+## Tune
+
+You can override the default constant rate factor (CRF) of 23 by setting the `FFMPEG_CRF` environment variable.
+The frame rate will be determined as the maximum frame rate among the source files.
+To override this, use the `FFMPEG_FR` environment variable.
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.
 
 ## Show your support
 Give a ⭐️ if this project helped you!
```

