# Comparing `tmp/shipyard_api-0.2.0a1.tar.gz` & `tmp/shipyard_api-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_api-0.2.0a1.tar", max compression
+gzip compressed data, was "shipyard_api-0.2.0a2.tar", max compression
```

## Comparing `shipyard_api-0.2.0a1.tar` & `shipyard_api-0.2.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-18 20:05:24.210595 shipyard_api-0.2.0a1/README.md
--rw-r--r--   0        0        0      538 2024-05-14 13:28:05.884166 shipyard_api-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-18 20:05:24.211332 shipyard_api-0.2.0a1/shipyard_api/__init__.py
--rw-r--r--   0        0        0      695 2024-05-06 20:06:59.600682 shipyard_api-0.2.0a1/shipyard_api/cli/authtest.py
--rw-r--r--   0        0        0     1443 2024-04-18 20:05:24.211506 shipyard_api-0.2.0a1/shipyard_api/cli/get_logs.py
--rw-r--r--   0        0        0     2397 2024-05-13 18:01:57.037107 shipyard_api-0.2.0a1/shipyard_api/cli/trigger_fleet.py
--rw-r--r--   0        0        0    10181 2024-05-14 13:27:41.985398 shipyard_api-0.2.0a1/shipyard_api/client.py
--rw-r--r--   0        0        0     1064 2024-05-13 21:35:11.173671 shipyard_api-0.2.0a1/shipyard_api/errors.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 shipyard_api-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 20:05:24.210595 shipyard_api-0.2.0a2/README.md
+-rw-r--r--   0        0        0      538 2024-05-14 13:34:40.631138 shipyard_api-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-18 20:05:24.211332 shipyard_api-0.2.0a2/shipyard_api/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-06 20:06:59.600682 shipyard_api-0.2.0a2/shipyard_api/cli/authtest.py
+-rw-r--r--   0        0        0     1443 2024-04-18 20:05:24.211506 shipyard_api-0.2.0a2/shipyard_api/cli/get_logs.py
+-rw-r--r--   0        0        0     2397 2024-05-13 18:01:57.037107 shipyard_api-0.2.0a2/shipyard_api/cli/trigger_fleet.py
+-rw-r--r--   0        0        0    10366 2024-05-14 13:34:40.623911 shipyard_api-0.2.0a2/shipyard_api/client.py
+-rw-r--r--   0        0        0     1099 2024-05-14 13:34:40.615839 shipyard_api-0.2.0a2/shipyard_api/errors.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 shipyard_api-0.2.0a2/PKG-INFO
```

### Comparing `shipyard_api-0.2.0a1/pyproject.toml` & `shipyard_api-0.2.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-api"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = ""
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
```

### Comparing `shipyard_api-0.2.0a1/shipyard_api/cli/authtest.py` & `shipyard_api-0.2.0a2/shipyard_api/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a1/shipyard_api/cli/get_logs.py` & `shipyard_api-0.2.0a2/shipyard_api/cli/get_logs.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a1/shipyard_api/cli/trigger_fleet.py` & `shipyard_api-0.2.0a2/shipyard_api/cli/trigger_fleet.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a1/shipyard_api/client.py` & `shipyard_api-0.2.0a2/shipyard_api/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -242,30 +242,35 @@
 
         Returns:
             requests.Response: The response from the API.
 
         Raises:
             ExitCodeException: If an exit code exception occurs.
         """
+        try:
+            response = self._request(method="PUT",
+                                     url=f"{self.base_url}/projects/{self.project_id}/fleets",
+                                     headers={
+                                         "accept": "application/json",
+                                         "content-type": "application/json",
+                                         "X-Shipyard-API-Key": self.api_key
+                                     },
+                                     data=yaml.dump(fleet_yaml)
+                                     )
+            logger.info("Successfully upserted fleet")
+            return response
+
+        except ExitCodeException:
+            raise
+        except Exception as e:
+            raise ExitCodeException(
+                f"Error upserting fleet: {e}",
+                exit_code=EXIT_CODE_UNKNOWN_ERROR,
+            ) from e
 
-        response = self._request(method="PUT",
-                                 url=f"{self.base_url}/projects/{self.project_id}/fleets",
-                                 headers={
-                                     "accept": "application/json",
-                                     "content-type": "application/json",
-                                     "X-Shipyard-API-Key": self.api_key
-                                 },
-                                 data=yaml.dump(fleet_yaml)
-                                 )
-        if response.ok:
-            logger.info("Fleet upserted successfully")
-        else:
-            logger.error(f"Fleet upsert failed: {response.content}")
-
-        return response
 
     def get_run_status(self, fleet_id: str, run_id: str):
         """
         Get the status of a fleet run.
 
         Args:
             fleet_id (str): The ID of the fleet.
```

### Comparing `shipyard_api-0.2.0a1/shipyard_api/errors.py` & `shipyard_api-0.2.0a2/shipyard_api/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 EXIT_CODE_UNAUTHORIZED_ACCESS = 103
 EXIT_CODE_LIST_FLEET_RUNS_ERROR = 104
 EXIT_CODE_LIST_VOYAGES_ERROR = 105
 EXIT_CODE_VOYAGE_EXPORT_ERROR = 106
 EXIT_CODE_TRIGGER_FLEET_ERROR = 107
 EXIT_CODE_ARTIFACTS_ERROR = 108
 EXIT_CODE_FLEET_FINAL_STATE_ERROR = 109
+EXIT_CODE_FLEET_UPSERT_ERROR = 110
 EXIT_CODE_UNKNOWN_ERROR = 249
 
 
 class MissingProjectID(ExitCodeException):
     def __init__(self):
         self.message = "Project ID is required in order to perform this operation"
         self.exit_code = EXIT_CODE_MISSING_PROJECT_ID
```

### Comparing `shipyard_api-0.2.0a1/PKG-INFO` & `shipyard_api-0.2.0a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-api
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

