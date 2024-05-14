# Comparing `tmp/shipyard_api-0.2.0a0.tar.gz` & `tmp/shipyard_api-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_api-0.2.0a0.tar", max compression
+gzip compressed data, was "shipyard_api-0.2.0a1.tar", max compression
```

## Comparing `shipyard_api-0.2.0a0.tar` & `shipyard_api-0.2.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-18 20:05:24.210595 shipyard_api-0.2.0a0/README.md
--rw-r--r--   0        0        0      538 2024-05-13 21:31:06.669868 shipyard_api-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-18 20:05:24.211332 shipyard_api-0.2.0a0/shipyard_api/__init__.py
--rw-r--r--   0        0        0      695 2024-05-06 20:06:59.600682 shipyard_api-0.2.0a0/shipyard_api/cli/authtest.py
--rw-r--r--   0        0        0     1443 2024-04-18 20:05:24.211506 shipyard_api-0.2.0a0/shipyard_api/cli/get_logs.py
--rw-r--r--   0        0        0     2397 2024-05-13 18:01:57.037107 shipyard_api-0.2.0a0/shipyard_api/cli/trigger_fleet.py
--rw-r--r--   0        0        0     9521 2024-05-13 21:31:06.670566 shipyard_api-0.2.0a0/shipyard_api/client.py
--rw-r--r--   0        0        0     1064 2024-05-13 21:31:06.671101 shipyard_api-0.2.0a0/shipyard_api/errors.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 shipyard_api-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 20:05:24.210595 shipyard_api-0.2.0a1/README.md
+-rw-r--r--   0        0        0      538 2024-05-14 13:28:05.884166 shipyard_api-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-18 20:05:24.211332 shipyard_api-0.2.0a1/shipyard_api/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-06 20:06:59.600682 shipyard_api-0.2.0a1/shipyard_api/cli/authtest.py
+-rw-r--r--   0        0        0     1443 2024-04-18 20:05:24.211506 shipyard_api-0.2.0a1/shipyard_api/cli/get_logs.py
+-rw-r--r--   0        0        0     2397 2024-05-13 18:01:57.037107 shipyard_api-0.2.0a1/shipyard_api/cli/trigger_fleet.py
+-rw-r--r--   0        0        0    10181 2024-05-14 13:27:41.985398 shipyard_api-0.2.0a1/shipyard_api/client.py
+-rw-r--r--   0        0        0     1064 2024-05-13 21:35:11.173671 shipyard_api-0.2.0a1/shipyard_api/errors.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 shipyard_api-0.2.0a1/PKG-INFO
```

### Comparing `shipyard_api-0.2.0a0/pyproject.toml` & `shipyard_api-0.2.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-api"
-version = "0.2.0a0"
+version = "0.2.0a1"
 description = ""
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
```

### Comparing `shipyard_api-0.2.0a0/shipyard_api/cli/authtest.py` & `shipyard_api-0.2.0a1/shipyard_api/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a0/shipyard_api/cli/get_logs.py` & `shipyard_api-0.2.0a1/shipyard_api/cli/get_logs.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a0/shipyard_api/cli/trigger_fleet.py` & `shipyard_api-0.2.0a1/shipyard_api/cli/trigger_fleet.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a0/shipyard_api/client.py` & `shipyard_api-0.2.0a1/shipyard_api/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,32 @@
     def __init__(self, org_id: str, api_key: str, project_id: Optional[str] = None):
         self.org_id = org_id
         self.api_key = api_key
         self.base_url = f"https://api.app.shipyardapp.com/orgs/{org_id}"
         self.headers = {"X-Shipyard-API-Key": self.api_key}
         self.project_id = project_id
 
-    def _request(self, method: str, url: str, data: Optional[Dict[str, Any]] = None, headers=None):
+    def _request(self, method: str, url: str, data: Optional[Dict[str, Any]] = None,
+                 headers: Optional[Dict[str, Any]] = None):
+        """
+        A helper method to make requests to the Shipyard API.
+
+        Args:
+            method (str): The HTTP method to use.
+            url (str): The URL to make the request to.
+            data (Optional[Dict[str, Any]]): The data to send with the request.
+            headers (Optional[Dict[str, Any]]): The headers to send with the request.
+
+        Returns:
+            requests.Response: The response object from the request.
+
+        Raises:
+            ExitCodeException: If an error occurs during the request.
+            UnauthorizedAccess: If the API returns a 401 status code.
+        """
         if headers is None:
             headers = self.headers
 
         request_args = {
             "method": method,
             "url": url,
             "headers": headers
@@ -239,17 +256,18 @@
                                  },
                                  data=yaml.dump(fleet_yaml)
                                  )
         if response.ok:
             logger.info("Fleet upserted successfully")
         else:
             logger.error(f"Fleet upsert failed: {response.content}")
-            return response
 
-    def get_run_status(self, fleet_id:str, run_id:str):
+        return response
+
+    def get_run_status(self, fleet_id: str, run_id: str):
         """
         Get the status of a fleet run.
 
         Args:
             fleet_id (str): The ID of the fleet.
             run_id (str): The ID of the run.
```

### Comparing `shipyard_api-0.2.0a0/shipyard_api/errors.py` & `shipyard_api-0.2.0a1/shipyard_api/errors.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a0/PKG-INFO` & `shipyard_api-0.2.0a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-api
-Version: 0.2.0a0
+Version: 0.2.0a1
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

