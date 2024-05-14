# Comparing `tmp/google-cloud-alloydb-connector-1.1.0.tar.gz` & `tmp/google-cloud-alloydb-connector-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-alloydb-connector-1.1.0.tar", last modified: Tue Apr 16 15:32:14 2024, max compression
+gzip compressed data, was "google-cloud-alloydb-connector-1.1.1.tar", last modified: Tue May 14 20:27:17 2024, max compression
```

## Comparing `google-cloud-alloydb-connector-1.1.0.tar` & `google-cloud-alloydb-connector-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/
--rw-rw-r--   0 root         (0)     1003    11357 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/LICENSE
--rw-r--r--   0 root         (0)     1003    16779 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    15823 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/api/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/api/__init__.py
--rwxrwxr-x   0 root         (0)     1003     2620 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/api/field_behavior_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/
--rw-rw-r--   0 root         (0)     1003      903 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     7785 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/async_connector.py
--rw-rw-r--   0 root         (0)     1003     1841 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/asyncpg.py
--rw-rw-r--   0 root         (0)     1003     6956 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/client.py
--rw-rw-r--   0 root         (0)     1003    13812 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/connector.py
--rw-rw-r--   0 root         (0)     1003      665 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003     9804 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     1437 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/py.typed
--rw-rw-r--   0 root         (0)     1003     2764 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     4482 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/refresh.py
--rw-rw-r--   0 root         (0)     1003     2076 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/__init__.py
--rwxrwxr-x   0 root         (0)     1003     3962 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    16779 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1085 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      111 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2024-04-16 15:32:14.566715 google-cloud-alloydb-connector-1.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2673 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.456291 google-cloud-alloydb-connector-1.1.1/
+-rw-rw-r--   0 root         (0)     1003    11357 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/LICENSE
+-rw-r--r--   0 root         (0)     1003    16779 2024-05-14 20:27:17.456291 google-cloud-alloydb-connector-1.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    15823 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.452291 google-cloud-alloydb-connector-1.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.452291 google-cloud-alloydb-connector-1.1.1/google/api/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/api/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     2620 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/api/field_behavior_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.452291 google-cloud-alloydb-connector-1.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.452291 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.456291 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/
+-rw-rw-r--   0 root         (0)     1003      903 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7785 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/async_connector.py
+-rw-rw-r--   0 root         (0)     1003     1841 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/asyncpg.py
+-rw-rw-r--   0 root         (0)     1003     6956 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/client.py
+-rw-rw-r--   0 root         (0)     1003    13699 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003      665 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     9804 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     1437 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/py.typed
+-rw-rw-r--   0 root         (0)     1003     2764 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     4482 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/refresh.py
+-rw-rw-r--   0 root         (0)     1003     2076 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.452291 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb_connectors_v1/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.456291 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb_connectors_v1/proto/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb_connectors_v1/proto/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     3962 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 20:27:17.456291 google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    16779 2024-05-14 20:27:17.000000 google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1085 2024-05-14 20:27:17.000000 google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-14 20:27:17.000000 google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-14 20:27:17.000000 google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      111 2024-05-14 20:27:17.000000 google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-14 20:27:17.000000 google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2024-05-14 20:27:17.456291 google-cloud-alloydb-connector-1.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2673 2024-05-14 20:24:38.000000 google-cloud-alloydb-connector-1.1.1/setup.py
```

### Comparing `google-cloud-alloydb-connector-1.1.0/LICENSE` & `google-cloud-alloydb-connector-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/PKG-INFO` & `google-cloud-alloydb-connector-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-alloydb-connector-1.1.0/README.md` & `google-cloud-alloydb-connector-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/api/__init__.py` & `google-cloud-alloydb-connector-1.1.1/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/api/field_behavior_pb2.py` & `google-cloud-alloydb-connector-1.1.1/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/__init__.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/async_connector.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/async_connector.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/asyncpg.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/client.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/connector.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,11 +329,7 @@
         """Helper function to cancel Instances' tasks
         and close client."""
         await asyncio.gather(
             *[instance.close() for instance in self._instances.values()]
         )
         if self._client:
             await self._client.close()
-
-    def __del__(self) -> None:
-        """Close Connector as part of garbage collection"""
-        self.close()
```

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/exceptions.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/instance.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/pg8000.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/rate_limiter.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/refresh.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/refresh.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/utils.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/version.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb/connector/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/__init__.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb_connectors_v1/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py` & `google-cloud-alloydb-connector-1.1.1/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/PKG-INFO` & `google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/SOURCES.txt` & `google-cloud-alloydb-connector-1.1.1/google_cloud_alloydb_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.1.0/setup.py` & `google-cloud-alloydb-connector-1.1.1/setup.py`

 * *Files identical despite different names*

