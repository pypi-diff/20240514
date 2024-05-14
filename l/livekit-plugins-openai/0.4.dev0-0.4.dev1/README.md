# Comparing `tmp/livekit_plugins_openai-0.4.dev0.tar.gz` & `tmp/livekit_plugins_openai-0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_openai-0.4.dev0.tar", last modified: Wed May  1 00:22:29 2024, max compression
+gzip compressed data, was "livekit_plugins_openai-0.4.dev1.tar", last modified: Wed May  1 00:54:27 2024, max compression
```

## Comparing `livekit_plugins_openai-0.4.dev0.tar` & `livekit_plugins_openai-0.4.dev1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.637794 livekit_plugins_openai-0.4.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.637794 livekit_plugins_openai-0.4.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.593602 livekit_plugins_openai-0.4.dev1/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.593602 livekit_plugins_openai-0.4.dev1/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/setup.py
```

### Comparing `livekit_plugins_openai-0.4.dev0/PKG-INFO` & `livekit_plugins_openai-0.4.dev1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.4.dev0
+Version: 0.4.dev1
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev0
+Requires-Dist: livekit-agents~=0.6.dev1
 Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
```

### Comparing `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/__init__.py` & `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/llm.py` & `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/llm.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/models.py` & `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/models.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/stt.py` & `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/stt.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/tts.py` & `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/tts.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/version.py` & `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/version.py`

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

### Comparing `livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/PKG-INFO` & `livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.4.dev0
+Version: 0.4.dev1
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev0
+Requires-Dist: livekit-agents~=0.6.dev1
 Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
```

### Comparing `livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/SOURCES.txt` & `livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev0/setup.py` & `livekit_plugins_openai-0.4.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "livekit ~= 0.11",
-        "livekit-agents~=0.6.dev0",
+        "livekit-agents~=0.6.dev1",
         "openai >= 1.0.0",
         "requests >= 2, < 3",
     ],
     package_data={
         "livekit.plugins.openai": ["py.typed"],
     },
     project_urls={
```

