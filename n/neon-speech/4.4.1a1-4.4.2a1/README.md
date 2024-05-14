# Comparing `tmp/neon_speech-4.4.1a1.tar.gz` & `tmp/neon_speech-4.4.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_speech-4.4.1a1.tar", last modified: Thu Apr 25 23:02:18 2024, max compression
+gzip compressed data, was "neon_speech-4.4.2a1.tar", last modified: Tue May 14 17:07:20 2024, max compression
```

## Comparing `neon_speech-4.4.1a1.tar` & `neon_speech-4.4.2a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:02:18.420544 neon_speech-4.4.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-25 23:02:18.420544 neon_speech-4.4.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:02:18.416544 neon_speech-4.4.1a1/neon_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/neon_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/neon_speech/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/neon_speech/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/neon_speech/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/neon_speech/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/neon_speech/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/neon_speech/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:02:18.420544 neon_speech-4.4.1a1/neon_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-25 23:02:18.000000 neon_speech-4.4.1a1/neon_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 23:02:18.000000 neon_speech-4.4.1a1/neon_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 23:02:18.000000 neon_speech-4.4.1a1/neon_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 23:02:18.000000 neon_speech-4.4.1a1/neon_speech.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-25 23:02:18.000000 neon_speech-4.4.1a1/neon_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 23:02:18.000000 neon_speech-4.4.1a1/neon_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 23:02:18.420544 neon_speech-4.4.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-25 23:02:15.000000 neon_speech-4.4.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:07:20.964951 neon_speech-4.4.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-14 17:07:20.964951 neon_speech-4.4.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:07:20.964951 neon_speech-4.4.2a1/neon_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/neon_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/neon_speech/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/neon_speech/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27208 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/neon_speech/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/neon_speech/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/neon_speech/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/neon_speech/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:07:20.964951 neon_speech-4.4.2a1/neon_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-14 17:07:20.000000 neon_speech-4.4.2a1/neon_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-14 17:07:20.000000 neon_speech-4.4.2a1/neon_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:07:20.000000 neon_speech-4.4.2a1/neon_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 17:07:20.000000 neon_speech-4.4.2a1/neon_speech.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-14 17:07:20.000000 neon_speech-4.4.2a1/neon_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 17:07:20.000000 neon_speech-4.4.2a1/neon_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:07:20.964951 neon_speech-4.4.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-14 17:07:12.000000 neon_speech-4.4.2a1/setup.py
```

### Comparing `neon_speech-4.4.1a1/LICENSE.md` & `neon_speech-4.4.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/PKG-INFO` & `neon_speech-4.4.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_speech
-Version: 4.4.1a1
+Version: 4.4.2a1
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.4.1a1/README.md` & `neon_speech-4.4.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/neon_speech/__init__.py` & `neon_speech-4.4.2a1/neon_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/neon_speech/__main__.py` & `neon_speech-4.4.2a1/neon_speech/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/neon_speech/cli.py` & `neon_speech-4.4.2a1/neon_speech/cli.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/neon_speech/service.py` & `neon_speech-4.4.2a1/neon_speech/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from typing import Dict
 
 import ovos_dinkum_listener.plugins
 
 from tempfile import mkstemp
 from threading import Lock, Event
 from time import time
+
 from pydub import AudioSegment
 from speech_recognition import AudioData
 from neon_utils.file_utils import decode_base64_string_to_file
 from ovos_utils.log import LOG, log_deprecation
 from neon_utils.configuration_utils import get_neon_user_config
 from neon_utils.metrics_utils import Stopwatch
 from neon_utils.user_utils import apply_local_user_profile_updates
@@ -131,17 +132,17 @@
         if self.config.get('listener', {}).get('enable_stt_api', True):
             self.api_stt = STTFactory.create(config=self.config,
                                              results_event=None)
         else:
             LOG.info("Skipping api_stt init")
             self.api_stt = None
 
-    def _record_begin(self):
+    def _record_end_signal(self):
         self._stt_stopwatch.start()
-        OVOSDinkumVoiceService._record_begin(self)
+        OVOSDinkumVoiceService._record_end_signal(self)
 
     def _stt_text(self, text: str, stt_context: dict):
         self._stt_stopwatch.stop()
         stt_context.setdefault("timing", dict())
         stt_context["timing"]["get_stt"] = self._stt_stopwatch.time
 
         # This is where the first Message of the interaction is created
```

### Comparing `neon_speech-4.4.1a1/neon_speech/stt.py` & `neon_speech-4.4.2a1/neon_speech/stt.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/neon_speech/transformers.py` & `neon_speech-4.4.2a1/neon_speech/transformers.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/neon_speech/utils.py` & `neon_speech-4.4.2a1/neon_speech/utils.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.4.1a1/neon_speech.egg-info/PKG-INFO` & `neon_speech-4.4.2a1/neon_speech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 4.4.1a1
+Version: 4.4.2a1
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.4.1a1/setup.py` & `neon_speech-4.4.2a1/setup.py`

 * *Files identical despite different names*

