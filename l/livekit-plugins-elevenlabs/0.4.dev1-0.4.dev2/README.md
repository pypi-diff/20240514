# Comparing `tmp/livekit_plugins_elevenlabs-0.4.dev1.tar.gz` & `tmp/livekit_plugins_elevenlabs-0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_elevenlabs-0.4.dev1.tar", last modified: Wed May  1 00:54:11 2024, max compression
+gzip compressed data, was "livekit_plugins_elevenlabs-0.4.dev2.tar", last modified: Sun May  5 16:56:20 2024, max compression
```

## Comparing `livekit_plugins_elevenlabs-0.4.dev1.tar` & `livekit_plugins_elevenlabs-0.4.dev2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:11.096774 livekit_plugins_elevenlabs-0.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-01 00:54:11.096774 livekit_plugins_elevenlabs-0.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:11.092774 livekit_plugins_elevenlabs-0.4.dev1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:11.092774 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:11.096774 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:11.096774 livekit_plugins_elevenlabs-0.4.dev1/livekit_plugins_elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-01 00:54:11.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit_plugins_elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-01 00:54:11.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:54:11.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 00:54:11.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit_plugins_elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:54:11.000000 livekit_plugins_elevenlabs-0.4.dev1/livekit_plugins_elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:54:11.096774 livekit_plugins_elevenlabs-0.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-01 00:54:06.000000 livekit_plugins_elevenlabs-0.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.061905 livekit_plugins_elevenlabs-0.4.dev2/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.061905 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.061905 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/setup.py
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev1/PKG-INFO` & `livekit_plugins_elevenlabs-0.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.4.dev1
+Version: 0.4.dev2
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/__init__.py` & `livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/tts.py` & `livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/tts.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
             )
             await ws.send_str(json.dumps(init_pkt))
 
             while True:
                 data = await data_rx.recv()
                 data_pkt = dict(
                     text=data,
-                    try_trigger_generation=False,
+                    try_trigger_generation=True,
                 )
                 if data == SynthesizeStream._STREAM_EOS:
                     closing_ws = True
 
                 await ws.send_str(json.dumps(data_pkt))
 
                 if closing_ws:
@@ -346,15 +346,15 @@
                 data: dict = json.loads(msg.data)
                 if data.get("audio"):
                     b64data = base64.b64decode(data["audio"])
                     frame = rtc.AudioFrame(
                         data=b64data,
                         sample_rate=self._opts.sample_rate,
                         num_channels=1,
-                        samples_per_channel=len(data) // 2,
+                        samples_per_channel=len(b64data) // 2,
                     )
                     self._event_queue.put_nowait(
                         tts.SynthesisEvent(
                             type=tts.SynthesisEventType.AUDIO,
                             audio=tts.SynthesizedAudio(text="", data=frame),
                         )
                     )
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev1/livekit/plugins/elevenlabs/version.py` & `livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.dev1"
+__version__ = "0.4.dev2"
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev1/livekit_plugins_elevenlabs.egg-info/PKG-INFO` & `livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.4.dev1
+Version: 0.4.dev2
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev1/setup.py` & `livekit_plugins_elevenlabs-0.4.dev2/setup.py`

 * *Files identical despite different names*

