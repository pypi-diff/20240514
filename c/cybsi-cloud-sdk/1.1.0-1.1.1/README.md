# Comparing `tmp/cybsi_cloud_sdk-1.1.0.tar.gz` & `tmp/cybsi_cloud_sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybsi_cloud_sdk-1.1.0.tar", max compression
+gzip compressed data, was "cybsi_cloud_sdk-1.1.1.tar", max compression
```

## Comparing `cybsi_cloud_sdk-1.1.0.tar` & `cybsi_cloud_sdk-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    10142 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/LICENSE
--rw-r--r--   0        0        0      626 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/README.md
--rw-r--r--   0        0        0      151 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/__init__.py
--rw-r--r--   0        0        0      195 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/__version__.py
--rw-r--r--   0        0        0      405 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/__init__.py
--rw-r--r--   0        0        0     1362 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/api.py
--rw-r--r--   0        0        0      539 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/__init__.py
--rw-r--r--   0        0        0      412 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/api.py
--rw-r--r--   0        0        0     8864 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/api_key.py
--rw-r--r--   0        0        0     1814 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/limits.py
--rw-r--r--   0        0        0     1551 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/permission.py
--rw-r--r--   0        0        0     2159 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/resource.py
--rw-r--r--   0        0        0      821 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/token.py
--rw-r--r--   0        0        0     4393 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/client.py
--rw-r--r--   0        0        0     5631 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/client_config.py
--rw-r--r--   0        0        0      829 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/enum.py
--rw-r--r--   0        0        0     9679 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/error.py
--rw-r--r--   0        0        0      306 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/files/__init__.py
--rw-r--r--   0        0        0    23274 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/files/files.py
--rw-r--r--   0        0        0      541 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/api.py
--rw-r--r--   0        0        0     8823 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/schemas.py
--rw-r--r--   0        0        0     7897 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/task_queue.py
--rw-r--r--   0        0        0     7492 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/tasks.py
--rw-r--r--   0        0        0      257 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/__init__.py
--rw-r--r--   0        0        0     2046 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/base.py
--rw-r--r--   0        0        0     8226 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/buffer.py
--rw-r--r--   0        0        0     7192 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/connector.py
--rw-r--r--   0        0        0     1755 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/multipart.py
--rw-r--r--   0        0        0      870 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/time.py
--rw-r--r--   0        0        0      595 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/__init__.py
--rw-r--r--   0        0        0     1200 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/api.py
--rw-r--r--   0        0        0     9771 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/collection.py
--rw-r--r--   0        0        0    15217 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/objects.py
--rw-r--r--   0        0        0     8513 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/schemas.py
--rw-r--r--   0        0        0     4302 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/pagination.py
--rw-r--r--   0        0        0      520 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/view.py
--rw-r--r--   0        0        0        0 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/py.typed
--rw-r--r--   0        0        0     1163 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 cybsi_cloud_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/LICENSE
+-rw-r--r--   0        0        0      626 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/README.md
+-rw-r--r--   0        0        0      151 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/__version__.py
+-rw-r--r--   0        0        0      405 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/__init__.py
+-rw-r--r--   0        0        0     1362 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/api.py
+-rw-r--r--   0        0        0      539 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/api.py
+-rw-r--r--   0        0        0     8864 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/api_key.py
+-rw-r--r--   0        0        0     1814 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/limits.py
+-rw-r--r--   0        0        0     1551 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/permission.py
+-rw-r--r--   0        0        0     2159 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/resource.py
+-rw-r--r--   0        0        0      821 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/token.py
+-rw-r--r--   0        0        0     4393 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/client.py
+-rw-r--r--   0        0        0     5631 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/client_config.py
+-rw-r--r--   0        0        0      829 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/enum.py
+-rw-r--r--   0        0        0     9679 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/error.py
+-rw-r--r--   0        0        0      306 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/files/__init__.py
+-rw-r--r--   0        0        0    23274 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/files/files.py
+-rw-r--r--   0        0        0      541 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/__init__.py
+-rw-r--r--   0        0        0     1178 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/api.py
+-rw-r--r--   0        0        0     8823 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/schemas.py
+-rw-r--r--   0        0        0     7897 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/task_queue.py
+-rw-r--r--   0        0        0     7637 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/tasks.py
+-rw-r--r--   0        0        0      257 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/__init__.py
+-rw-r--r--   0        0        0     2046 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/base.py
+-rw-r--r--   0        0        0     8226 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/buffer.py
+-rw-r--r--   0        0        0     7192 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/connector.py
+-rw-r--r--   0        0        0     1755 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/multipart.py
+-rw-r--r--   0        0        0      870 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/time.py
+-rw-r--r--   0        0        0      595 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/__init__.py
+-rw-r--r--   0        0        0     1200 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/api.py
+-rw-r--r--   0        0        0     9771 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/collection.py
+-rw-r--r--   0        0        0    15217 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/objects.py
+-rw-r--r--   0        0        0     8513 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/schemas.py
+-rw-r--r--   0        0        0     4302 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/pagination.py
+-rw-r--r--   0        0        0      520 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/view.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/py.typed
+-rw-r--r--   0        0        0     1163 2024-05-14 08:45:22.085479 cybsi_cloud_sdk-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 cybsi_cloud_sdk-1.1.1/PKG-INFO
```

### Comparing `cybsi_cloud_sdk-1.1.0/LICENSE` & `cybsi_cloud_sdk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/README.md` & `cybsi_cloud_sdk-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/api.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/__init__.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/api_key.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/api_key.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/limits.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/limits.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/permission.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/permission.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/resource.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/resource.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/token.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/token.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/client.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/client.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/client_config.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/client_config.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/enum.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/enum.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/error.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/error.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/files/files.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/files/files.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/__init__.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/api.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/schemas.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/schemas.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/task_queue.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/task_queue.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/tasks.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,30 +206,34 @@
 
     @property
     def state(self) -> TaskState:
         """Task state."""
         return TaskState(self._get("state"))
 
     @property
-    def result(self) -> JsonObject:
+    def result(self) -> Optional[JsonObject]:
         """Task result.
 
         Note:
             This value is present if task state is :attr:`~.TaskState.Completed`
         """
-        return cast(JsonObject, self._get("result"))
+        if result := self._data.get("result", None):
+            return cast(JsonObject, result)
+        return None
 
     @property
-    def error(self) -> TaskErrorView:
+    def error(self) -> Optional[TaskErrorView]:
         """Task error.
 
         Note:
             This value is present if task state is :attr:`~.TaskState.Failed`
         """
-        return TaskErrorView(self._get("result"))
+        if error := self._data.get("error", None):
+            return TaskErrorView(error)
+        return None
 
 
 class ObjectKeyForm(JsonObjectForm):
     """Object key form."""
 
     def __init__(self, key_type: ObjectKeyType, value: str):
         super().__init__()
```

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/base.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/base.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/buffer.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/buffer.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/connector.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/connector.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/multipart.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/multipart.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/time.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/time.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/__init__.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/api.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/collection.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/collection.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/objects.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/objects.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/schemas.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/schemas.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/pagination.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/pagination.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/cybsi/cloud/view.py` & `cybsi_cloud_sdk-1.1.1/cybsi/cloud/view.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.0/pyproject.toml` & `cybsi_cloud_sdk-1.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cybsi-cloud-sdk"
-version = "1.1.0"
+version = "1.1.1"
 description = "Cybsi Cloud development kit"
 authors = ["Cybsi Cloud developers"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "cybsi" },
 ]
@@ -32,15 +32,15 @@
 [tool.isort]
 profile = "black"
 extend_skip = ["__init__.py"]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "1.1.0"
+current = "1.1.1"
 
 regex = '''
   ^
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
```

### Comparing `cybsi_cloud_sdk-1.1.0/PKG-INFO` & `cybsi_cloud_sdk-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybsi-cloud-sdk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Cybsi Cloud development kit
 License: Apache-2.0
 Author: Cybsi Cloud developers
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

