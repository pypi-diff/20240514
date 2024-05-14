# Comparing `tmp/cloud-sql-python-connector-1.9.1.tar.gz` & `tmp/cloud-sql-python-connector-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-sql-python-connector-1.9.1.tar", last modified: Wed Apr 17 15:49:02 2024, max compression
+gzip compressed data, was "cloud-sql-python-connector-1.9.2.tar", last modified: Tue May 14 18:13:35 2024, max compression
```

## Comparing `cloud-sql-python-connector-1.9.1.tar` & `cloud-sql-python-connector-1.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/LICENSE
--rw-r--r--   0 root         (0)     1003    23771 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    22623 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.036124 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    23771 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      876 2024-04-17 15:49:02.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      164 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.032124 cloud-sql-python-connector-1.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.032124 cloud-sql-python-connector-1.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.032124 cloud-sql-python-connector-1.9.1/google/cloud/sql/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/
--rw-rw-r--   0 root         (0)     1003      883 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     1838 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/asyncpg.py
--rw-rw-r--   0 root         (0)     1003     8494 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/client.py
--rwxrwxr-x   0 root         (0)     1003    19188 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/connector.py
--rw-rw-r--   0 root         (0)     1003     1524 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003    14920 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     1814 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/py.typed
--rw-rw-r--   0 root         (0)     1003     2105 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pymysql.py
--rw-rw-r--   0 root         (0)     1003     2452 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pytds.py
--rw-rw-r--   0 root         (0)     1003     2993 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     3680 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/refresh_utils.py
--rwxrwxr-x   0 root         (0)     1003     3448 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/version.py
--rw-rw-r--   0 root         (0)     1003       67 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2905 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 18:13:35.828966 cloud-sql-python-connector-1.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/LICENSE
+-rw-r--r--   0 root         (0)     1003    23771 2024-05-14 18:13:35.828966 cloud-sql-python-connector-1.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    22623 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 18:13:35.824967 cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    23771 2024-05-14 18:13:35.000000 cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      876 2024-05-14 18:13:35.000000 cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-14 18:13:35.000000 cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-14 18:13:35.000000 cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      164 2024-05-14 18:13:35.000000 cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-14 18:13:35.000000 cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 18:13:35.824967 cloud-sql-python-connector-1.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 18:13:35.824967 cloud-sql-python-connector-1.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 18:13:35.824967 cloud-sql-python-connector-1.9.2/google/cloud/sql/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-14 18:13:35.828966 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/
+-rw-rw-r--   0 root         (0)     1003      883 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1838 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/asyncpg.py
+-rw-rw-r--   0 root         (0)     1003     8494 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/client.py
+-rwxrwxr-x   0 root         (0)     1003    19147 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003     1524 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    14966 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     1814 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/py.typed
+-rw-rw-r--   0 root         (0)     1003     2105 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/pymysql.py
+-rw-rw-r--   0 root         (0)     1003     2452 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/pytds.py
+-rw-rw-r--   0 root         (0)     1003     2993 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     3680 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/refresh_utils.py
+-rwxrwxr-x   0 root         (0)     1003     3448 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/version.py
+-rw-rw-r--   0 root         (0)     1003       67 2024-05-14 18:13:35.828966 cloud-sql-python-connector-1.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2905 2024-05-14 18:11:13.000000 cloud-sql-python-connector-1.9.2/setup.py
```

### Comparing `cloud-sql-python-connector-1.9.1/LICENSE` & `cloud-sql-python-connector-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/PKG-INFO` & `cloud-sql-python-connector-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.9.1
+Version: 1.9.2
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.1 Summary:
+Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.2 Summary:
 The Cloud SQL Python Connector is a library that can be used alongside a
 database driver to allow users with sufficient permissions to connect to a
 Cloud SQL database without having to manually allowlist IPs or manage SSL
 certificates. Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-
 python-connector Author: Google LLC Author-email: googleapis-
 packages@google.com License: Apache 2.0 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `cloud-sql-python-connector-1.9.1/README.md` & `cloud-sql-python-connector-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/PKG-INFO` & `cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.9.1
+Version: 1.9.2
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.1 Summary:
+Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.2 Summary:
 The Cloud SQL Python Connector is a library that can be used alongside a
 database driver to allow users with sufficient permissions to connect to a
 Cloud SQL database without having to manually allowlist IPs or manage SSL
 certificates. Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-
 python-connector Author: Google LLC Author-email: googleapis-
 packages@google.com License: Apache 2.0 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/SOURCES.txt` & `cloud-sql-python-connector-1.9.2/cloud_sql_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/__init__.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/asyncpg.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/client.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/client.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/connector.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from google.auth.credentials import Credentials
 from google.auth.credentials import with_scopes_if_required
 
 import google.cloud.sql.connector.asyncpg as asyncpg
 from google.cloud.sql.connector.client import CloudSQLClient
 from google.cloud.sql.connector.exceptions import ConnectorLoopError
 from google.cloud.sql.connector.exceptions import DnsNameResolutionError
-from google.cloud.sql.connector.instance import Instance
 from google.cloud.sql.connector.instance import IPTypes
+from google.cloud.sql.connector.instance import RefreshAheadCache
 import google.cloud.sql.connector.pg8000 as pg8000
 import google.cloud.sql.connector.pymysql as pymysql
 import google.cloud.sql.connector.pytds as pytds
 from google.cloud.sql.connector.utils import format_database_user
 from google.cloud.sql.connector.utils import generate_keys
 
 logger = logging.getLogger(name=__name__)
@@ -109,15 +109,15 @@
             self._loop = asyncio.new_event_loop()
             self._thread = Thread(target=self._loop.run_forever, daemon=True)
             self._thread.start()
             self._keys = asyncio.wrap_future(
                 asyncio.run_coroutine_threadsafe(generate_keys(), self._loop),
                 loop=self._loop,
             )
-        self._instances: Dict[str, Instance] = {}
+        self._cache: Dict[str, RefreshAheadCache] = {}
         self._client: Optional[CloudSQLClient] = None
 
         # initialize credentials
         scopes = ["https://www.googleapis.com/auth/sqlservice.admin"]
         if credentials:
             # verify custom credentials are proper type
             # and atleast base class of google.auth.credentials
@@ -251,31 +251,31 @@
                 self._sqladmin_api_endpoint,
                 self._quota_project,
                 self._credentials,
                 user_agent=self._user_agent,
                 driver=driver,
             )
         enable_iam_auth = kwargs.pop("enable_iam_auth", self._enable_iam_auth)
-        if instance_connection_string in self._instances:
-            instance = self._instances[instance_connection_string]
-            if enable_iam_auth != instance._enable_iam_auth:
+        if instance_connection_string in self._cache:
+            cache = self._cache[instance_connection_string]
+            if enable_iam_auth != cache._enable_iam_auth:
                 raise ValueError(
                     f"connect() called with 'enable_iam_auth={enable_iam_auth}', "
-                    f"but previously used 'enable_iam_auth={instance._enable_iam_auth}'. "
+                    f"but previously used 'enable_iam_auth={cache._enable_iam_auth}'. "
                     "If you require both for your use case, please use a new "
                     "connector.Connector object."
                 )
         else:
-            instance = Instance(
+            cache = RefreshAheadCache(
                 instance_connection_string,
                 self._client,
                 self._keys,
                 enable_iam_auth,
             )
-            self._instances[instance_connection_string] = instance
+            self._cache[instance_connection_string] = cache
 
         connect_func = {
             "pymysql": pymysql.connect,
             "pg8000": pg8000.connect,
             "asyncpg": asyncpg.connect,
             "pytds": pytds.connect,
         }
@@ -296,15 +296,15 @@
         # want the user to specify them.
         kwargs.pop("host", None)
         kwargs.pop("ssl", None)
         kwargs.pop("port", None)
 
         # attempt to make connection to Cloud SQL instance
         try:
-            instance_data, ip_address = await instance.connect_info(ip_type)
+            instance_data, ip_address = await cache.connect_info(ip_type)
             # resolve DNS name into IP address for PSC
             if ip_type.value == "PSC":
                 addr_info = await self._loop.getaddrinfo(
                     ip_address, None, family=socket.AF_INET, type=socket.SOCK_STREAM
                 )
                 # getaddrinfo returns a list of 5-tuples that contain socket
                 # connection info in the form
@@ -335,15 +335,15 @@
             connect_partial = partial(
                 connector, ip_address, instance_data.context, **kwargs
             )
             return await self._loop.run_in_executor(None, connect_partial)
 
         except Exception:
             # with any exception, we attempt a force refresh, then throw the error
-            await instance.force_refresh()
+            await cache.force_refresh()
             raise
 
     def __enter__(self) -> Any:
         """Enter context manager by returning Connector object"""
         return self
 
     def __exit__(
@@ -381,19 +381,17 @@
             if self._loop.is_running():
                 # stop event loop running in background thread
                 self._loop.call_soon_threadsafe(self._loop.stop)
             # wait for thread to finish closing (i.e. loop to stop)
             self._thread.join()
 
     async def close_async(self) -> None:
-        """Helper function to cancel Instances' tasks
+        """Helper function to cancel the cache's tasks
         and close aiohttp.ClientSession."""
-        await asyncio.gather(
-            *[instance.close() for instance in self._instances.values()]
-        )
+        await asyncio.gather(*[cache.close() for cache in self._cache.values()])
         if self._client:
             await self._client.close()
 
 
 async def create_async_connector(
     ip_type: str | IPTypes = IPTypes.PUBLIC,
     enable_iam_auth: bool = False,
```

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/exceptions.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/instance.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,64 +140,57 @@
             return self.ip_addrs[ip_type.value]
         raise CloudSQLIPTypeError(
             "Cloud SQL instance does not have any IP addresses matching "
             f"preference: {ip_type.value})"
         )
 
 
-class Instance:
-    """A class to manage the details of the connection to a Cloud SQL
-    instance, including refreshing the credentials.
-
-    :param instance_connection_string:
-        The Google Cloud SQL Instance's connection
-        string.
-    :type instance_connection_string: str
-
-    :param enable_iam_auth
-        Enables automatic IAM database authentication for Postgres or MySQL
-        instances.
-    :type enable_iam_auth: bool
-    """
+class RefreshAheadCache:
+    """Cache that refreshes connection info in the background prior to expiration.
 
-    _enable_iam_auth: bool
-    _keys: asyncio.Future
-    _instance_connection_string: str
-    _instance: str
-    _project: str
-    _region: str
-
-    _refresh_rate_limiter: AsyncRateLimiter
-    _refresh_in_progress: asyncio.locks.Event
-    _current: asyncio.Task  # task wraps coroutine that returns ConnectionInfo
-    _next: asyncio.Task  # task wraps coroutine that returns another task
+    Background tasks are used to schedule refresh attempts to get a new
+    ephemeral certificate and Cloud SQL metadata (IP addresses, etc.) ahead of
+    expiration.
+    """
 
     def __init__(
         self,
         instance_connection_string: str,
         client: CloudSQLClient,
         keys: asyncio.Future,
         enable_iam_auth: bool = False,
     ) -> None:
+        """Initializes a RefreshAheadCache instance.
+
+        Args:
+            instance_connection_string (str): The Cloud SQL Instance's
+                connection string (also known as an instance connection name).
+            client (CloudSQLClient): The Cloud SQL Client instance.
+            keys (asyncio.Future): A future to the client's public-private key
+                pair.
+            enable_iam_auth (bool): Enables automatic IAM database authentication
+                (Postgres and MySQL) as the default authentication method for all
+                connections.
+        """
         # validate and parse instance connection name
         self._project, self._region, self._instance = _parse_instance_connection_name(
             instance_connection_string
         )
         self._instance_connection_string = instance_connection_string
 
         self._enable_iam_auth = enable_iam_auth
         self._keys = keys
         self._client = client
         self._refresh_rate_limiter = AsyncRateLimiter(
             max_capacity=2,
             rate=1 / 30,
         )
         self._refresh_in_progress = asyncio.locks.Event()
-        self._current = self._schedule_refresh(0)
-        self._next = self._current
+        self._current: asyncio.Task = self._schedule_refresh(0)
+        self._next: asyncio.Task = self._current
 
     async def force_refresh(self) -> None:
         """
         Forces a new refresh attempt immediately to be used for future connection attempts.
         """
         # if next refresh is not already in progress, cancel it and schedule new one immediately
         if not self._refresh_in_progress.is_set():
@@ -207,18 +200,19 @@
         if not await _is_valid(self._current):
             self._current = self._next
 
     async def _perform_refresh(self) -> ConnectionInfo:
         """Retrieves instance metadata and ephemeral certificate from the
         Cloud SQL Instance.
 
-        :rtype: ConnectionInfo
-        :returns: A dataclass containing a string representing the ephemeral certificate, a dict
-            containing the instances IP adresses, a string representing a PEM-encoded private key
-            and a string representing a PEM-encoded certificate authority.
+        Returns:
+            A ConnectionInfo instance containing a string representing the
+            ephemeral certificate, a dict containing the instances IP adresses,
+            a string representing a PEM-encoded private key and a string
+            representing a PEM-encoded certificate authority.
         """
         self._refresh_in_progress.set()
         logger.debug(
             f"['{self._instance_connection_string}']: Entered _perform_refresh"
         )
 
         try:
@@ -286,23 +280,22 @@
             self._enable_iam_auth,
         )
 
     def _schedule_refresh(self, delay: int) -> asyncio.Task:
         """
         Schedule task to sleep and then perform refresh to get ConnectionInfo.
 
-        :type delay: int
-        :param delay
-            Time in seconds to sleep before running _perform_refresh.
+        Args:
+            delay (int): Time in seconds to sleep before performing a refresh.
 
-        :rtype: asyncio.Task
-        :returns: A Task representing the scheduled _perform_refresh.
+        Returns:
+            An asyncio.Task representing the scheduled refresh.
         """
 
-        async def _refresh_task(self: Instance, delay: int) -> ConnectionInfo:
+        async def _refresh_task(self: RefreshAheadCache, delay: int) -> ConnectionInfo:
             """
             A coroutine that sleeps for the specified amount of time before
             running _perform_refresh.
             """
             refresh_task: asyncio.Task
             try:
                 logger.debug(f"['{self._instance_connection_string}']: Entering sleep")
@@ -345,24 +338,22 @@
     async def connect_info(
         self,
         ip_type: IPTypes,
     ) -> Tuple[ConnectionInfo, str]:
         """Retrieve instance metadata and ip address required
         for making connection to Cloud SQL instance.
 
-        :type ip_type: IPTypes
-        :param ip_type: Enum specifying whether to look for public
-            or private IP address.
-
-        :rtype instance_data: ConnectionInfo
-        :returns: Instance metadata for Cloud SQL instance.
-
-        :rtype ip_address: str
-        :returns: A string representing the IP address of
-            the given Cloud SQL instance.
+        Args:
+            ip_type (IPTypes): Enum specifying type of IP address to lookup and
+                use for connection.
+
+        Returns:
+            A tuple with the first item being the ConnectionInfo instance for
+            establishing the connection, and the second item being the IP
+            address of the Cloud SQL instance matching the specified IP type.
         """
         logger.debug(
             f"['{self._instance_connection_string}']: Entered connect_info method"
         )
 
         instance_data: ConnectionInfo
```

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pg8000.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pymysql.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/pymysql.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pytds.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/pytds.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/rate_limiter.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/refresh_utils.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/refresh_utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/utils.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/version.py` & `cloud-sql-python-connector-1.9.2/google/cloud/sql/connector/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.9.1"
+__version__ = "1.9.2"
```

### Comparing `cloud-sql-python-connector-1.9.1/setup.py` & `cloud-sql-python-connector-1.9.2/setup.py`

 * *Files identical despite different names*

