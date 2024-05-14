# Comparing `tmp/delphai_utils-4.1.0.tar.gz` & `tmp/delphai_utils-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_utils-4.1.0.tar", max compression
+gzip compressed data, was "delphai_utils-4.1.1.tar", max compression
```

## Comparing `delphai_utils-4.1.0.tar` & `delphai_utils-4.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       22 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/__init__.py
--rw-r--r--   0        0        0      936 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/aio.py
--rw-r--r--   0        0        0     3842 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/authorization.py
--rw-r--r--   0        0        0      495 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/authorization_test.py
--rw-r--r--   0        0        0     2069 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/caching.py
--rw-r--r--   0        0        0     1313 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/config.py
--rw-r--r--   0        0        0    13924 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/constants/companies.py
--rw-r--r--   0        0        0     1389 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/db.py
--rw-r--r--   0        0        0      549 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/elasticsearch.py
--rw-r--r--   0        0        0     9347 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/faust.py
--rw-r--r--   0        0        0      481 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/formatting.py
--rw-r--r--   0        0        0     6728 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/gateway.py
--rw-r--r--   0        0        0     4796 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/grpc_client.py
--rw-r--r--   0        0        0     3687 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/grpc_server.py
--rw-r--r--   0        0        0     1532 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/interceptors/authentication.py
--rw-r--r--   0        0        0     5218 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/interceptors/metrics.py
--rw-r--r--   0        0        0     1482 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/keycloak.py
--rw-r--r--   0        0        0     1410 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/logging.py
--rw-r--r--   0        0        0     7182 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/monitoring.py
--rw-r--r--   0        0        0     2926 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/patches.py
--rw-r--r--   0        0        0      119 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/rpc/__init__.py
--rw-r--r--   0        0        0    10360 2024-05-13 08:20:31.567872 delphai_utils-4.1.0/delphai_utils/rpc/client.py
--rw-r--r--   0        0        0      393 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/rpc/errors.py
--rw-r--r--   0        0        0     4954 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/rpc/metrics.py
--rw-r--r--   0        0        0     2492 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/rpc/models.py
--rw-r--r--   0        0        0    10569 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/rpc/server.py
--rw-r--r--   0        0        0     2830 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/rpc/types.py
--rw-r--r--   0        0        0      693 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/rpc/utils.py
--rw-r--r--   0        0        0      582 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/strings/similarity.py
--rw-r--r--   0        0        0     4106 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/users.py
--rw-r--r--   0        0        0     2608 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/utils.py
--rw-r--r--   0        0        0      435 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/validation.py
--rw-r--r--   0        0        0    43882 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/delphai_utils/validator.py
--rw-r--r--   0        0        0     3196 2024-05-13 08:20:31.571872 delphai_utils-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 delphai_utils-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/__init__.py
+-rw-r--r--   0        0        0      936 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/aio.py
+-rw-r--r--   0        0        0     3842 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/authorization.py
+-rw-r--r--   0        0        0      495 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/authorization_test.py
+-rw-r--r--   0        0        0     2069 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/caching.py
+-rw-r--r--   0        0        0     1313 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/config.py
+-rw-r--r--   0        0        0    13924 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/constants/companies.py
+-rw-r--r--   0        0        0     1389 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/db.py
+-rw-r--r--   0        0        0      549 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/elasticsearch.py
+-rw-r--r--   0        0        0     9347 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/faust.py
+-rw-r--r--   0        0        0      481 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/formatting.py
+-rw-r--r--   0        0        0     6728 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/gateway.py
+-rw-r--r--   0        0        0     4796 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/grpc_client.py
+-rw-r--r--   0        0        0     3687 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/grpc_server.py
+-rw-r--r--   0        0        0     1532 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/interceptors/authentication.py
+-rw-r--r--   0        0        0     5218 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/interceptors/metrics.py
+-rw-r--r--   0        0        0     1482 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/keycloak.py
+-rw-r--r--   0        0        0     1410 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/logging.py
+-rw-r--r--   0        0        0     7182 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/monitoring.py
+-rw-r--r--   0        0        0     2926 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/patches.py
+-rw-r--r--   0        0        0      119 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/__init__.py
+-rw-r--r--   0        0        0    10360 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/client.py
+-rw-r--r--   0        0        0      393 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/errors.py
+-rw-r--r--   0        0        0     4954 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/metrics.py
+-rw-r--r--   0        0        0     2492 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/models.py
+-rw-r--r--   0        0        0    10649 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/server.py
+-rw-r--r--   0        0        0     2830 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/types.py
+-rw-r--r--   0        0        0      693 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/utils.py
+-rw-r--r--   0        0        0      582 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/strings/similarity.py
+-rw-r--r--   0        0        0     4106 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/users.py
+-rw-r--r--   0        0        0     2608 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/utils.py
+-rw-r--r--   0        0        0      435 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/validation.py
+-rw-r--r--   0        0        0    43882 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/validator.py
+-rw-r--r--   0        0        0     3196 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 delphai_utils-4.1.1/PKG-INFO
```

### Comparing `delphai_utils-4.1.0/delphai_utils/aio.py` & `delphai_utils-4.1.1/delphai_utils/aio.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/authorization.py` & `delphai_utils-4.1.1/delphai_utils/authorization.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/caching.py` & `delphai_utils-4.1.1/delphai_utils/caching.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/config.py` & `delphai_utils-4.1.1/delphai_utils/config.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/constants/companies.py` & `delphai_utils-4.1.1/delphai_utils/constants/companies.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/db.py` & `delphai_utils-4.1.1/delphai_utils/db.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/elasticsearch.py` & `delphai_utils-4.1.1/delphai_utils/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/faust.py` & `delphai_utils-4.1.1/delphai_utils/faust.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/gateway.py` & `delphai_utils-4.1.1/delphai_utils/gateway.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/grpc_client.py` & `delphai_utils-4.1.1/delphai_utils/grpc_client.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/grpc_server.py` & `delphai_utils-4.1.1/delphai_utils/grpc_server.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/interceptors/authentication.py` & `delphai_utils-4.1.1/delphai_utils/interceptors/authentication.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/interceptors/metrics.py` & `delphai_utils-4.1.1/delphai_utils/interceptors/metrics.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/keycloak.py` & `delphai_utils-4.1.1/delphai_utils/keycloak.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/logging.py` & `delphai_utils-4.1.1/delphai_utils/logging.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/monitoring.py` & `delphai_utils-4.1.1/delphai_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/patches.py` & `delphai_utils-4.1.1/delphai_utils/patches.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/rpc/client.py` & `delphai_utils-4.1.1/delphai_utils/rpc/client.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/rpc/metrics.py` & `delphai_utils-4.1.1/delphai_utils/rpc/metrics.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/rpc/models.py` & `delphai_utils-4.1.1/delphai_utils/rpc/models.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/rpc/server.py` & `delphai_utils-4.1.1/delphai_utils/rpc/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,22 +271,23 @@
             method=request.method_name,
             error=response.error,
             queued_for=queued_for,
             elapsed=elapsed,
         )
 
         logger.info(
-            "[MID:%s] Processed `%s` from `%s` service to method `%s`. In queue: %ims execution: %ims, success: %s ",
+            "[MID:%s] Processed `%s` from `%s` service to method `%s`. In queue: %ims, execution: %ims, success: %s%s",
             message.message_id,
             message.type,
             message.app_id or "unknown",
             request.method_name,
             max(queued_for * 1000, 0),
             elapsed * 1000,
             response.error is None,
+            (f", error: {response.error.message}" if response.error else ""),
         )
 
         return response
 
     @Response.wrap_errors
     async def _process_request(self, request) -> Response:
         handler = self._handlers.get(request.method_name)
```

### Comparing `delphai_utils-4.1.0/delphai_utils/rpc/types.py` & `delphai_utils-4.1.1/delphai_utils/rpc/types.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/rpc/utils.py` & `delphai_utils-4.1.1/delphai_utils/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/strings/similarity.py` & `delphai_utils-4.1.1/delphai_utils/strings/similarity.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/users.py` & `delphai_utils-4.1.1/delphai_utils/users.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/utils.py` & `delphai_utils-4.1.1/delphai_utils/utils.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/delphai_utils/validator.py` & `delphai_utils-4.1.1/delphai_utils/validator.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.0/pyproject.toml` & `delphai_utils-4.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delphai-utils"
-version = "4.1.0"
+version = "4.1.1"
 description = "delphai backend utilities"
 authors = ["Barath Kumar <barath@delphai.com>"]
 homepage = "https://github.com/delphai/delphai-utils"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiokafka = { version = "0.7.2", optional = true }
```

### Comparing `delphai_utils-4.1.0/PKG-INFO` & `delphai_utils-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-utils
-Version: 4.1.0
+Version: 4.1.1
 Summary: delphai backend utilities
 Home-page: https://github.com/delphai/delphai-utils
 Author: Barath Kumar
 Author-email: barath@delphai.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

