# Comparing `tmp/rai-sdk-0.7.4.tar.gz` & `tmp/rai_sdk-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai-sdk-0.7.4.tar", last modified: Thu Apr  4 22:07:06 2024, max compression
+gzip compressed data, was "rai_sdk-0.7.5.tar", last modified: Tue May 14 10:07:08 2024, max compression
```

## Comparing `rai-sdk-0.7.4.tar` & `rai_sdk-0.7.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/rai_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.508692 rai-sdk-0.7.4/railib/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29256 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/railib/pb/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/pb/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/pb/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/show.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:07:08.796263 rai_sdk-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-14 10:07:08.796263 rai_sdk-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:07:08.796263 rai_sdk-0.7.5/rai_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-14 10:07:08.000000 rai_sdk-0.7.5/rai_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 10:07:08.000000 rai_sdk-0.7.5/rai_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:07:08.000000 rai_sdk-0.7.5/rai_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 10:07:08.000000 rai_sdk-0.7.5/rai_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 10:07:08.000000 rai_sdk-0.7.5/rai_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:07:08.792263 rai_sdk-0.7.5/railib/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29366 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:07:08.792263 rai_sdk-0.7.5/railib/pb/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/pb/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/pb/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/railib/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:07:08.796263 rai_sdk-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:07:08.796263 rai_sdk-0.7.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-14 10:07:03.000000 rai_sdk-0.7.5/test/test_unit.py
```

### Comparing `rai-sdk-0.7.4/LICENSE` & `rai_sdk-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/PKG-INFO` & `rai_sdk-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-sdk
-Version: 0.7.4
+Version: 0.7.5
 Summary: The RelationalAI Software Development Kit for Python
 Home-page: http://github.com/RelationalAI/rai-sdk-python
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-sdk-0.7.4/README.md` & `rai_sdk-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/rai_sdk.egg-info/PKG-INFO` & `rai_sdk-0.7.5/rai_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-sdk
-Version: 0.7.4
+Version: 0.7.5
 Summary: The RelationalAI Software Development Kit for Python
 Home-page: http://github.com/RelationalAI/rai-sdk-python
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-sdk-0.7.4/railib/__init__.py` & `rai_sdk-0.7.5/railib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version_info__ = (0, 7, 4)
+__version_info__ = (0, 7, 5)
 __version__ = ".".join(map(str, __version_info__))
```

### Comparing `rai-sdk-0.7.4/railib/api.py` & `rai_sdk-0.7.5/railib/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,35 +327,40 @@
     f,
     overhead_rate: float,
     start_time: float = None,
     timeout: int = None,
     max_tries: int = None,
     max_delay: int = 120,
 ):
+    if overhead_rate < 0:
+        raise ValueError("overhead_rate must be non-negative")
+
     if start_time is None:
         start_time = time.time()
+    
     tries = 0
     max_time = time.time() + timeout if timeout else None
 
     while True:
         if f():
             break
 
+        current_time = time.time()
+        
         if max_tries is not None and tries >= max_tries:
             raise Exception(f'max tries {max_tries} exhausted')
 
-        if max_time is not None and time.time() >= max_time:
+        if max_time is not None and current_time >= max_time:
             raise Exception(f'timed out after {timeout} seconds')
 
+        duration = (current_time - start_time) * overhead_rate
+        duration = min(duration, max_delay)
+        
+        time.sleep(duration) 
         tries += 1
-        duration = min((time.time() - start_time) * overhead_rate, max_delay)
-        if tries == 1:
-            time.sleep(0.5)
-        else:
-            time.sleep(duration)
 
 
 def is_engine_term_state(state: str) -> bool:
     return state == "PROVISIONED" or ("FAILED" in state)
 
 
 def create_engine(ctx: Context, engine: str, size: str = "XS", **kwargs):
```

### Comparing `rai-sdk-0.7.4/railib/config.py` & `rai_sdk-0.7.5/railib/config.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/railib/credentials.py` & `rai_sdk-0.7.5/railib/credentials.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/railib/pb/message_pb2.py` & `rai_sdk-0.7.5/railib/pb/message_pb2.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/railib/pb/schema_pb2.py` & `rai_sdk-0.7.5/railib/pb/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/railib/rest.py` & `rai_sdk-0.7.5/railib/rest.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/railib/show.py` & `rai_sdk-0.7.5/railib/show.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/setup.py` & `rai_sdk-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/test/test_integration.py` & `rai_sdk-0.7.5/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.4/test/test_unit.py` & `rai_sdk-0.7.5/test/test_unit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+import time
 import unittest
 from unittest.mock import patch, MagicMock
 from urllib.error import URLError
 from urllib.request import Request
 
 from railib import api
 from railib.rest import _urlopen_with_retry
@@ -23,14 +24,56 @@
 
     def test_validation(self):
         api.poll_with_specified_overhead(lambda: True, overhead_rate=0.1)
         api.poll_with_specified_overhead(lambda: True, overhead_rate=0.1, timeout=1)
         api.poll_with_specified_overhead(lambda: True, overhead_rate=0.1, max_tries=1)
         api.poll_with_specified_overhead(lambda: True, overhead_rate=0.1, timeout=1, max_tries=1)
 
+    @patch('time.sleep', return_value=None)
+    @patch('time.time')
+    def test_initial_delay(self, mock_time, mock_sleep):
+        start_time = 100  # Fixed start time
+        increment_time = 0.0001
+        mock_time.side_effect = [start_time, start_time + increment_time]  # Simulate time progression
+
+        try:
+            api.poll_with_specified_overhead(lambda: False, overhead_rate=0.1, max_tries=2)
+        except Exception as e:
+            pass  # Ignore the exception for this test
+
+        expected_sleep_time = (start_time + increment_time - start_time) * 0.1
+        mock_sleep.assert_called_with(expected_sleep_time)
+    
+    def test_max_delay_cap(self):
+        with patch('time.sleep') as mock_sleep:
+            try:
+                api.poll_with_specified_overhead(lambda: False, overhead_rate=1, max_tries=2, start_time=time.time() - 200)
+            except Exception:
+                pass
+            # Ensure that the maximum delay of 120 seconds is not exceeded
+            mock_sleep.assert_called_with(120)
+
+    def test_polling_success(self):
+        with patch('time.sleep', return_value=None) as mock_sleep:
+            api.poll_with_specified_overhead(lambda: True, overhead_rate=0.1)
+            mock_sleep.assert_not_called()
+
+    def test_negative_overhead_rate(self):
+        with self.assertRaises(ValueError):
+            api.poll_with_specified_overhead(lambda: True, overhead_rate=-0.1)
+
+    def test_realistic_scenario(self):
+        responses = [False, False, True]
+        def side_effect():
+            return responses.pop(0)
+
+        with patch('time.sleep') as mock_sleep:
+            api.poll_with_specified_overhead(side_effect, overhead_rate=0.1, max_tries=3)
+            # Ensure that `time.sleep` was called twice (for two false returns)
+            self.assertEqual(mock_sleep.call_count, 2)
 
 @patch('railib.rest.urlopen')
 class TestURLOpenWithRetry(unittest.TestCase):
 
     WARNING_LOG_PREFIX = "URL/Connection error occured"
     ERROR_LOG_PREFIX = "Failed to connect to"
```

