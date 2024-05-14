# Comparing `tmp/livekit_plugins_silero-0.4.dev0.tar.gz` & `tmp/livekit_plugins_silero-0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_silero-0.4.dev0.tar", last modified: Wed May  1 00:22:47 2024, max compression
+gzip compressed data, was "livekit_plugins_silero-0.4.dev1.tar", last modified: Wed May  1 00:54:31 2024, max compression
```

## Comparing `livekit_plugins_silero-0.4.dev0.tar` & `livekit_plugins_silero-0.4.dev1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/log.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:31.274875 livekit_plugins_silero-0.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 00:54:31.274875 livekit_plugins_silero-0.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:31.270875 livekit_plugins_silero-0.4.dev1/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:31.270875 livekit_plugins_silero-0.4.dev1/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:31.270875 livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:31.274875 livekit_plugins_silero-0.4.dev1/livekit_plugins_silero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 00:54:31.000000 livekit_plugins_silero-0.4.dev1/livekit_plugins_silero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-01 00:54:31.000000 livekit_plugins_silero-0.4.dev1/livekit_plugins_silero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:54:31.000000 livekit_plugins_silero-0.4.dev1/livekit_plugins_silero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:54:31.000000 livekit_plugins_silero-0.4.dev1/livekit_plugins_silero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:54:31.000000 livekit_plugins_silero-0.4.dev1/livekit_plugins_silero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:54:31.274875 livekit_plugins_silero-0.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-01 00:54:24.000000 livekit_plugins_silero-0.4.dev1/setup.py
```

### Comparing `livekit_plugins_silero-0.4.dev0/PKG-INFO` & `livekit_plugins_silero-0.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-silero
-Version: 0.4.dev0
+Version: 0.4.dev1
 Summary: Agent Framework Plugin for Silero
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev0
+Requires-Dist: livekit-agents~=0.6.dev1
 Requires-Dist: torch<3,>=2
 Requires-Dist: torchaudio>=2
 Requires-Dist: numpy<2,>=1
 Requires-Dist: onnxruntime~=1.17.0
 
 # LiveKit Plugins Silero
```

### Comparing `livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/__init__.py` & `livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/vad.py` & `livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/vad.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/version.py` & `livekit_plugins_silero-0.4.dev1/livekit/plugins/silero/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.dev0"
+__version__ = "0.4.dev1"
```

### Comparing `livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/PKG-INFO` & `livekit_plugins_silero-0.4.dev1/livekit_plugins_silero.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-silero
-Version: 0.4.dev0
+Version: 0.4.dev1
 Summary: Agent Framework Plugin for Silero
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev0
+Requires-Dist: livekit-agents~=0.6.dev1
 Requires-Dist: torch<3,>=2
 Requires-Dist: torchaudio>=2
 Requires-Dist: numpy<2,>=1
 Requires-Dist: onnxruntime~=1.17.0
 
 # LiveKit Plugins Silero
```

### Comparing `livekit_plugins_silero-0.4.dev0/setup.py` & `livekit_plugins_silero-0.4.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.8.0",
     install_requires=[
         "livekit ~= 0.11",
-        "livekit-agents~=0.6.dev0",
+        "livekit-agents~=0.6.dev1",
         "torch >= 2, < 3",
         "torchaudio >= 2",
         "numpy >= 1, < 2",
         "onnxruntime~=1.17.0",
     ],
     package_data={"livekit.plugins.silero": ["files/silero_vad.jit"]},
     project_urls={
```
