# Comparing `tmp/m3u8-4.1.0.tar.gz` & `tmp/m3u8-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u8-4.1.0.tar", last modified: Mon Apr  1 17:41:15 2024, max compression
+gzip compressed data, was "m3u8-5.0.0.tar", last modified: Tue May 14 17:15:17 2024, max compression
```

## Comparing `m3u8-4.1.0.tar` & `m3u8-5.0.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.522981 m3u8-4.1.0/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1135 2022-12-29 01:47:32.000000 m3u8-4.1.0/LICENSE
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       59 2022-12-29 01:47:32.000000 m3u8-4.1.0/MANIFEST.in
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15662 2024-04-01 17:41:15.522656 m3u8-4.1.0/PKG-INFO
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15465 2023-07-25 22:57:47.000000 m3u8-4.1.0/README.rst
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.519748 m3u8-4.1.0/m3u8/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     2525 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/__init__.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1023 2023-05-11 22:24:51.000000 m3u8-4.1.0/m3u8/httpclient.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1369 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/mixins.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    53969 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/model.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    23156 2024-04-01 17:38:58.000000 m3u8-4.1.0/m3u8/parser.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1750 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/protocol.py
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.521018 m3u8-4.1.0/m3u8.egg-info/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15662 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/PKG-INFO
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)      441 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/SOURCES.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/dependency_links.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/not-zip-safe
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       61 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/requires.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        5 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/top_level.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       58 2023-12-12 23:06:49.000000 m3u8-4.1.0/requirements.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       38 2024-04-01 17:41:15.523083 m3u8-4.1.0/setup.cfg
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)      655 2024-04-01 17:39:10.000000 m3u8-4.1.0/setup.py
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.522344 m3u8-4.1.0/tests/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     6149 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_loader.py
--rwxr-xr-x   0 mauricio.antunes   (501) staff       (20)    49520 2024-04-01 17:38:58.000000 m3u8-4.1.0/tests/test_model.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    36766 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_parser.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1073 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_strict_validations.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    13995 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_variant_m3u8.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-05-14 17:15:17.028310 m3u8-5.0.0/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1135 2022-12-29 01:47:32.000000 m3u8-5.0.0/LICENSE
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       59 2024-05-13 15:13:30.000000 m3u8-5.0.0/MANIFEST.in
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     4837 2024-05-14 17:15:17.028171 m3u8-5.0.0/PKG-INFO
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     4600 2024-05-13 15:11:41.000000 m3u8-5.0.0/README.md
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-05-14 17:15:17.024361 m3u8-5.0.0/m3u8/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     2525 2023-12-12 23:06:49.000000 m3u8-5.0.0/m3u8/__init__.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1023 2023-05-11 22:24:51.000000 m3u8-5.0.0/m3u8/httpclient.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1369 2024-05-14 03:24:57.000000 m3u8-5.0.0/m3u8/mixins.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    54575 2024-05-14 13:12:29.000000 m3u8-5.0.0/m3u8/model.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    23552 2024-05-13 12:02:28.000000 m3u8-5.0.0/m3u8/parser.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1750 2023-12-12 23:06:49.000000 m3u8-5.0.0/m3u8/protocol.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1013 2024-05-13 12:02:28.000000 m3u8-5.0.0/m3u8/version_matching.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     3038 2024-05-13 12:02:28.000000 m3u8-5.0.0/m3u8/version_matching_rules.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-05-14 17:15:17.025726 m3u8-5.0.0/m3u8.egg-info/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     4837 2024-05-14 17:15:17.000000 m3u8-5.0.0/m3u8.egg-info/PKG-INFO
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)      575 2024-05-14 17:15:17.000000 m3u8-5.0.0/m3u8.egg-info/SOURCES.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2024-05-14 17:15:17.000000 m3u8-5.0.0/m3u8.egg-info/dependency_links.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2024-05-14 17:03:43.000000 m3u8-5.0.0/m3u8.egg-info/not-zip-safe
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       61 2024-05-14 17:15:17.000000 m3u8-5.0.0/m3u8.egg-info/requires.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        5 2024-05-14 17:15:17.000000 m3u8-5.0.0/m3u8.egg-info/top_level.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       58 2023-12-12 23:06:49.000000 m3u8-5.0.0/requirements.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       38 2024-05-14 17:15:17.028360 m3u8-5.0.0/setup.cfg
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)      704 2024-05-14 17:10:25.000000 m3u8-5.0.0/setup.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-05-14 17:15:17.027935 m3u8-5.0.0/tests/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)      924 2024-05-13 12:02:28.000000 m3u8-5.0.0/tests/test_invalid_versioned_playlists.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     6149 2023-12-12 23:06:49.000000 m3u8-5.0.0/tests/test_loader.py
+-rwxr-xr-x   0 mauricio.antunes   (501) staff       (20)    49747 2024-05-13 12:02:22.000000 m3u8-5.0.0/tests/test_model.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    36953 2024-05-14 13:12:29.000000 m3u8-5.0.0/tests/test_parser.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1248 2024-05-13 12:02:28.000000 m3u8-5.0.0/tests/test_strict_validations.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    13995 2023-12-12 23:06:49.000000 m3u8-5.0.0/tests/test_variant_m3u8.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     3700 2024-05-13 12:02:28.000000 m3u8-5.0.0/tests/test_version_matching_rules.py
```

### Comparing `m3u8-4.1.0/LICENSE` & `m3u8-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u8-4.1.0/m3u8/__init__.py` & `m3u8-5.0.0/m3u8/__init__.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.1.0/m3u8/httpclient.py` & `m3u8-5.0.0/m3u8/httpclient.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.1.0/m3u8/mixins.py` & `m3u8-5.0.0/m3u8/mixins.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.1.0/m3u8/model.py` & `m3u8-5.0.0/m3u8/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,23 +466,26 @@
       when EXT-X-PROGRAM-DATE-TIME is set or a calculated value based on previous
       segments' EXT-X-PROGRAM-DATE-TIME and EXTINF values
 
     `discontinuity`
       Returns a boolean indicating if a EXT-X-DISCONTINUITY tag exists
       http://tools.ietf.org/html/draft-pantos-http-live-streaming-13#section-3.4.11
 
-    `cue_out_start`
-      Returns a boolean indicating if a EXT-X-CUE-OUT tag exists
-
     `cue_out`
       Returns a boolean indicating if a EXT-X-CUE-OUT-CONT tag exists
       Note: for backwards compatibility, this will be True when cue_out_start
             is True, even though this tag did not exist in the input, and
             EXT-X-CUE-OUT-CONT will not exist in the output
 
+    `cue_out_start`
+      Returns a boolean indicating if a EXT-X-CUE-OUT tag exists
+
+    `cue_out_explicitly_duration`
+      Returns a boolean indicating if a EXT-X-CUE-OUT have the DURATION parameter when parsing
+
     `cue_in`
       Returns a boolean indicating if a EXT-X-CUE-IN tag exists
 
     `scte35`
       Base64 encoded SCTE35 metadata if available
 
     `scte35_duration`
@@ -524,14 +527,15 @@
         current_program_date_time=None,
         duration=None,
         title=None,
         bitrate=None,
         byterange=None,
         cue_out=False,
         cue_out_start=False,
+        cue_out_explicitly_duration=False,
         cue_in=False,
         discontinuity=False,
         key=None,
         scte35=None,
         oatcls_scte35=None,
         scte35_duration=None,
         scte35_elapsedtime=None,
@@ -551,14 +555,15 @@
         self._base_uri = base_uri
         self.bitrate = bitrate
         self.byterange = byterange
         self.program_date_time = program_date_time
         self.current_program_date_time = current_program_date_time
         self.discontinuity = discontinuity
         self.cue_out_start = cue_out_start
+        self.cue_out_explicitly_duration = cue_out_explicitly_duration
         self.cue_out = cue_out
         self.cue_in = cue_in
         self.scte35 = scte35
         self.oatcls_scte35 = oatcls_scte35
         self.scte35_duration = scte35_duration
         self.scte35_elapsedtime = scte35_elapsedtime
         self.asset_metadata = asset_metadata
@@ -623,19 +628,18 @@
 
             if self.asset_metadata:
                 asset_suffix = []
                 for metadata_key, metadata_value in self.asset_metadata.items():
                     asset_suffix.append(f"{metadata_key.upper()}={metadata_value}")
                 output.append(f"{ext_x_asset}:{','.join(asset_suffix)}\n")
 
-            output.append(
-                "#EXT-X-CUE-OUT{}\n".format(
-                    (":" + self.scte35_duration) if self.scte35_duration else ""
-                )
-            )
+            prefix = ":DURATION=" if self.cue_out_explicitly_duration else ":"
+            cue_info = f"{prefix}{self.scte35_duration}" if self.scte35_duration else ""
+            output.append(f"#EXT-X-CUE-OUT{cue_info}\n")
+
         elif self.cue_out:
             cue_out_cont_suffix = []
             if self.scte35_elapsedtime:
                 cue_out_cont_suffix.append(f"ElapsedTime={self.scte35_elapsedtime}")
             if self.scte35_duration:
                 cue_out_cont_suffix.append(f"Duration={self.scte35_duration}")
             if self.scte35:
@@ -974,14 +978,15 @@
             resolution=resolution_pair,
             codecs=stream_info.get("codecs"),
             frame_rate=stream_info.get("frame_rate"),
             video_range=stream_info.get("video_range"),
             hdcp_level=stream_info.get("hdcp_level"),
             pathway_id=stream_info.get("pathway_id"),
             stable_variant_id=stream_info.get("stable_variant_id"),
+            req_video_layout=stream_info.get("req_video_layout"),
         )
         self.media = []
         for media_type in ("audio", "video", "subtitles"):
             group_id = stream_info.get(media_type)
             if not group_id:
                 continue
 
@@ -1039,14 +1044,15 @@
             resolution=resolution_pair,
             codecs=iframe_stream_info.get("codecs"),
             video_range=iframe_stream_info.get("video_range"),
             hdcp_level=iframe_stream_info.get("hdcp_level"),
             frame_rate=None,
             pathway_id=iframe_stream_info.get("pathway_id"),
             stable_variant_id=iframe_stream_info.get("stable_variant_id"),
+            req_video_layout=None,
         )
 
     def __str__(self):
         iframe_stream_inf = []
         if self.iframe_stream_info.program_id:
             iframe_stream_inf.append(
                 "PROGRAM-ID=%d" % self.iframe_stream_info.program_id
@@ -1099,14 +1105,15 @@
     video = None
     subtitles = None
     frame_rate = None
     video_range = None
     hdcp_level = None
     pathway_id = None
     stable_variant_id = None
+    req_video_layout = None
 
     def __init__(self, **kwargs):
         self.bandwidth = kwargs.get("bandwidth")
         self.closed_captions = kwargs.get("closed_captions")
         self.average_bandwidth = kwargs.get("average_bandwidth")
         self.program_id = kwargs.get("program_id")
         self.resolution = kwargs.get("resolution")
@@ -1115,14 +1122,15 @@
         self.video = kwargs.get("video")
         self.subtitles = kwargs.get("subtitles")
         self.frame_rate = kwargs.get("frame_rate")
         self.video_range = kwargs.get("video_range")
         self.hdcp_level = kwargs.get("hdcp_level")
         self.pathway_id = kwargs.get("pathway_id")
         self.stable_variant_id = kwargs.get("stable_variant_id")
+        self.req_video_layout = kwargs.get("req_video_layout")
 
     def __str__(self):
         stream_inf = []
         if self.program_id is not None:
             stream_inf.append("PROGRAM-ID=%d" % self.program_id)
         if self.closed_captions is not None:
             stream_inf.append("CLOSED-CAPTIONS=%s" % self.closed_captions)
@@ -1144,14 +1152,16 @@
             stream_inf.append("VIDEO-RANGE=%s" % self.video_range)
         if self.hdcp_level is not None:
             stream_inf.append("HDCP-LEVEL=%s" % self.hdcp_level)
         if self.pathway_id is not None:
             stream_inf.append("PATHWAY-ID=" + quoted(self.pathway_id))
         if self.stable_variant_id is not None:
             stream_inf.append("STABLE-VARIANT-ID=" + quoted(self.stable_variant_id))
+        if self.req_video_layout is not None:
+            stream_inf.append("REQ-VIDEO_LAYOUT=" + quoted(self.req_video_layout))
         return ",".join(stream_inf)
 
 
 class Media(BasePathMixin):
     """
     A media object from a M3U8 playlist
     https://tools.ietf.org/html/draft-pantos-http-live-streaming-16#section-4.3.4.1
```

### Comparing `m3u8-4.1.0/m3u8/parser.py` & `m3u8-5.0.0/m3u8/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from backports.datetime_fromisoformat import MonkeyPatch
 
     MonkeyPatch.patch_fromisoformat()
 except ImportError:
     pass
 
 
-from m3u8 import protocol
+from m3u8 import protocol, version_matching
 
 """
 http://tools.ietf.org/html/draft-pantos-http-live-streaming-08#section-3.2
 http://stackoverflow.com/questions/2785755/how-to-split-but-ignore-separators-in-quoted-strings-in-python
 """
 ATTRIBUTELISTPATTERN = re.compile(r"""((?:[^,"']|"[^"]*"|'[^']*')+)""")
 
@@ -70,16 +70,23 @@
     state = {
         "expect_segment": False,
         "expect_playlist": False,
         "current_key": None,
         "current_segment_map": None,
     }
 
+    lines = string_to_lines(content)
+    if strict:
+        found_errors = version_matching.validate(lines)
+
+        if len(found_errors) > 0:
+            raise Exception(found_errors)
+
     lineno = 0
-    for line in string_to_lines(content):
+    for line in lines:
         lineno += 1
         line = line.strip()
 
         # Call custom parser if needed
         if line.startswith("#") and callable(custom_tags_parser):
             go_to_next_line = custom_tags_parser(line, lineno, data, state)
 
@@ -120,14 +127,16 @@
             _parse_cueout_cont(line, state)
             state["cue_out"] = True
 
         elif line.startswith(protocol.ext_x_cue_out):
             _parse_cueout(line, state)
             state["cue_out_start"] = True
             state["cue_out"] = True
+            if "DURATION" in line.upper():
+                state["cue_out_explicitly_duration"] = True
 
         elif line.startswith(f"{protocol.ext_oatcls_scte35}:"):
             _parse_oatcls_scte35(line, state)
 
         elif line.startswith(f"{protocol.ext_x_asset}:"):
             _parse_asset(line, state)
 
@@ -292,14 +301,17 @@
     if state.get("current_program_date_time"):
         segment["current_program_date_time"] = state["current_program_date_time"]
         state["current_program_date_time"] += timedelta(seconds=segment["duration"])
     segment["uri"] = line
     segment["cue_in"] = state.pop("cue_in", False)
     segment["cue_out"] = state.pop("cue_out", False)
     segment["cue_out_start"] = state.pop("cue_out_start", False)
+    segment["cue_out_explicitly_duration"] = state.pop(
+        "cue_out_explicitly_duration", False
+    )
     scte_op = state.pop if segment["cue_in"] else state.get
     segment["scte35"] = scte_op("current_cue_out_scte35", None)
     segment["oatcls_scte35"] = scte_op("current_cue_out_oatcls_scte35", None)
     segment["scte35_duration"] = scte_op("current_cue_out_duration", None)
     segment["scte35_elapsedtime"] = scte_op("current_cue_out_elapsedtime", None)
     segment["asset_metadata"] = scte_op("asset_metadata", None)
     segment["discontinuity"] = state.pop("discontinuity", False)
@@ -463,15 +475,15 @@
     elements = line.split(":", 1)
     if len(elements) != 2:
         return
 
     # EXT-X-CUE-OUT-CONT:2.436/120 style
     res = re.match(
         r"^[-+]?([0-9]+(\.[0-9]+)?|\.[0-9]+)/[-+]?([0-9]+(\.[0-9]+)?|\.[0-9]+)$",
-        elements[1]
+        elements[1],
     )
     if res:
         state["current_cue_out_elapsedtime"] = res.group(1)
         state["current_cue_out_duration"] = res.group(3)
         return
 
     # EXT-X-CUE-OUT-CONT:ElapsedTime=10,Duration=60,SCTE35=... style
```

### Comparing `m3u8-4.1.0/m3u8/protocol.py` & `m3u8-5.0.0/m3u8/protocol.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.1.0/setup.py` & `m3u8-5.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from os.path import abspath, dirname, exists, join
 
 from setuptools import setup
 
 long_description = None
-if exists("README.rst"):
-    with open("README.rst") as file:
+if exists("README.md"):
+    with open("README.md") as file:
         long_description = file.read()
 
 install_reqs = [
     req for req in open(abspath(join(dirname(__file__), "requirements.txt")))
 ]
 
 setup(
     name="m3u8",
     author="Globo.com",
-    version="4.1.0",
+    version="5.0.0",
     license="MIT",
     zip_safe=False,
     include_package_data=True,
     install_requires=install_reqs,
     packages=["m3u8"],
     url="https://github.com/globocom/m3u8",
     description="Python m3u8 parser",
     long_description=long_description,
+    long_description_content_type="text/markdown",
     python_requires=">=3.7",
 )
```

### Comparing `m3u8-4.1.0/tests/test_loader.py` & `m3u8-5.0.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.1.0/tests/test_model.py` & `m3u8-5.0.0/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,22 @@
     obj = m3u8.M3U8(playlists.CUE_OUT_WITH_DURATION_PLAYLIST)
 
     result = obj.dumps()
     expected = "#EXT-X-CUE-OUT:11.52\n"
     assert expected in result
 
 
+def test_segment_cue_out_start_explicit_dumps():
+    obj = m3u8.M3U8(playlists.CUE_OUT_WITH_EXPLICIT_DURATION_PLAYLIST)
+
+    result = obj.dumps()
+    expected = "#EXT-X-CUE-OUT:DURATION=11.52\n"
+    assert expected in result
+
+
 def test_segment_cue_out_start_no_duration_dumps():
     obj = m3u8.M3U8(playlists.CUE_OUT_NO_DURATION_PLAYLIST)
 
     result = obj.dumps()
     expected = "#EXT-X-CUE-OUT\n"
     assert expected in result
 
@@ -225,22 +233,22 @@
     )
 
 
 def test_segment_cue_out_cont_alt():
     obj = m3u8.M3U8(playlists.CUE_OUT_CONT_ALT_PLAYLIST)
     segments = obj.segments
 
-    assert segments[1].scte35_elapsedtime == '2'
-    assert segments[1].scte35_duration == '120'
+    assert segments[1].scte35_elapsedtime == "2"
+    assert segments[1].scte35_duration == "120"
 
-    assert segments[2].scte35_elapsedtime == '8'
-    assert segments[2].scte35_duration == '120.0'
+    assert segments[2].scte35_elapsedtime == "8"
+    assert segments[2].scte35_duration == "120.0"
 
-    assert segments[3].scte35_elapsedtime == '14.001'
-    assert segments[3].scte35_duration == '120.0'
+    assert segments[3].scte35_elapsedtime == "14.001"
+    assert segments[3].scte35_duration == "120.0"
 
 
 def test_segment_envivio_scte35_attribute():
     obj = m3u8.M3U8(playlists.CUE_OUT_ENVIVIO_PLAYLIST)
     segments = obj.segments
     assert segments[3].cue_out is True
     assert (
```

### Comparing `m3u8-4.1.0/tests/test_parser.py` & `m3u8-5.0.0/tests/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,7 +901,12 @@
 
 def test_media_with_stable_rendition_id():
     data = m3u8.parse(playlists.VARIANT_PLAYLIST_WITH_STABLE_RENDITION_ID)
     assert (
         data["media"][0]["stable_rendition_id"]
         == "a8213e27c12a158ea8660e0fe8bdcac6072ca26d984e7e8603652bc61fdceffa"
     )
+
+
+def test_req_video_layout():
+    data = m3u8.parse(playlists.VARIANT_PLAYLIST_WITH_REQ_VIDEO_LAYOUT)
+    assert data["playlists"][0]["stream_info"]["req_video_layout"] == '"CH-STEREO"'
```

### Comparing `m3u8-4.1.0/tests/test_strict_validations.py` & `m3u8-5.0.0/tests/test_strict_validations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Copyright 2014 Globo.com Player authors. All rights reserved.
 # Use of this source code is governed by a MIT License
 # license that can be found in the LICENSE file.
 
+import invalid_versioned_playlists
 import pytest
 
+import m3u8
+import m3u8.version_matching_rules
+
 
 @pytest.mark.xfail
 def test_should_fail_if_first_line_not_EXTM3U():
     assert 0
 
 
 @pytest.mark.xfail
@@ -26,17 +30,19 @@
 
 
 @pytest.mark.xfail
 def test_should_fail_if_EXT_X_MEDIA_SEQUENCE_is_not_a_number():
     assert 0
 
 
-@pytest.mark.xfail
 def test_should_validate_supported_EXT_X_VERSION():
-    assert 0
+    with pytest.raises(
+        Exception,
+    ):
+        m3u8.parse(invalid_versioned_playlists.M3U8_RULE_IV, strict=True)
 
 
 @pytest.mark.xfail
 def test_should_fail_if_any_EXTINF_duration_is_greater_than_TARGET_DURATION():
     assert 0
```

### Comparing `m3u8-4.1.0/tests/test_variant_m3u8.py` & `m3u8-5.0.0/tests/test_variant_m3u8.py`

 * *Files identical despite different names*

