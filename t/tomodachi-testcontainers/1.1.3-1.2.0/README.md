# Comparing `tmp/tomodachi_testcontainers-1.1.3.tar.gz` & `tmp/tomodachi_testcontainers-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-1.1.3.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-1.2.0.tar", max compression
```

## Comparing `tomodachi_testcontainers-1.1.3.tar` & `tomodachi_testcontainers-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-1.1.3/LICENSE
--rw-r--r--   0        0        0     5348 2024-03-09 08:39:31.463310 tomodachi_testcontainers-1.1.3/README.md
--rw-r--r--   0        0        0     5797 2024-05-06 11:04:23.840534 tomodachi_testcontainers-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1276 2024-01-20 12:02:32.093321 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0     1874 2024-01-20 12:02:32.093525 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/assertions.py
--rw-r--r--   0        0        0     2630 2024-02-10 12:31:41.559539 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/async_probes.py
--rw-r--r--   0        0        0      162 2024-02-10 12:31:41.538492 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0    10112 2024-02-29 12:23:35.986712 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/clients/snssqs.py
--rw-r--r--   0        0        0     1069 2024-01-20 12:02:32.094393 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0      352 2024-01-20 12:02:32.094662 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/__init__.py
--rw-r--r--   0        0        0     5436 2024-05-06 11:02:27.200947 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/container.py
--rw-r--r--   0        0        0     2471 2024-03-07 14:43:49.403638 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/database.py
--rw-r--r--   0        0        0     2879 2024-01-08 19:54:00.254890 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/image.py
--rw-r--r--   0        0        0     2082 2024-03-07 14:43:49.404544 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/web.py
--rw-r--r--   0        0        0     1519 2024-01-20 12:02:32.095426 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/dynamodb_admin.py
--rw-r--r--   0        0        0     2290 2024-01-20 12:02:32.095615 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2597 2024-03-07 14:43:49.405277 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/minio.py
--rw-r--r--   0        0        0     2487 2024-01-20 12:02:32.095997 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     2144 2024-02-10 12:31:41.557850 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/mysql.py
--rw-r--r--   0        0        0     1837 2024-02-29 12:23:35.987113 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/postgres.py
--rw-r--r--   0        0        0     3511 2024-03-07 14:43:49.408064 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0     2561 2024-01-20 12:02:32.096696 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0     2820 2024-02-10 12:31:41.571774 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/wiremock.py
--rw-r--r--   0        0        0     1996 2024-03-13 08:33:53.123090 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/__init__.py
--rw-r--r--   0        0        0     2166 2024-01-20 12:02:32.097410 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/containers.py
--rw-r--r--   0        0        0     3252 2024-03-13 08:36:44.293036 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/localstack.py
--rw-r--r--   0        0        0      722 2024-03-09 08:38:21.893971 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/minio.py
--rw-r--r--   0        0        0     3037 2024-03-13 08:36:04.781801 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/moto.py
--rw-r--r--   0        0        0      336 2024-03-09 08:38:04.306148 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/mysql.py
--rw-r--r--   0        0        0      393 2024-03-09 08:35:49.808543 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/postgres.py
--rw-r--r--   0        0        0     1542 2024-03-09 08:35:23.475100 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/sftp.py
--rw-r--r--   0        0        0      915 2024-03-13 08:36:50.873024 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/wiremock.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     2788 2024-03-07 14:43:49.412303 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0     7188 1970-01-01 00:00:00.000000 tomodachi_testcontainers-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5348 2024-03-09 08:39:31.463310 tomodachi_testcontainers-1.2.0/README.md
+-rw-r--r--   0        0        0     5975 2024-05-14 13:44:28.267957 tomodachi_testcontainers-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1276 2024-01-20 12:02:32.093321 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0     1874 2024-01-20 12:02:32.093525 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/assertions.py
+-rw-r--r--   0        0        0     2630 2024-02-10 12:31:41.559539 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/async_probes.py
+-rw-r--r--   0        0        0      162 2024-02-10 12:31:41.538492 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0    10112 2024-02-29 12:23:35.986712 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/clients/snssqs.py
+-rw-r--r--   0        0        0     1069 2024-01-20 12:02:32.094393 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0      352 2024-01-20 12:02:32.094662 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/__init__.py
+-rw-r--r--   0        0        0     5560 2024-05-14 13:53:54.645693 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/container.py
+-rw-r--r--   0        0        0     2543 2024-05-14 13:34:50.731465 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/database.py
+-rw-r--r--   0        0        0     2879 2024-01-08 19:54:00.254890 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/image.py
+-rw-r--r--   0        0        0     2154 2024-05-14 13:34:50.731933 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/web.py
+-rw-r--r--   0        0        0     1603 2024-05-14 13:34:50.732546 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/dynamodb_admin.py
+-rw-r--r--   0        0        0     2374 2024-05-14 13:34:50.732936 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2681 2024-05-14 13:34:50.733197 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/minio.py
+-rw-r--r--   0        0        0     2571 2024-05-14 13:34:50.733643 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     2228 2024-05-14 13:34:50.734002 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/mysql.py
+-rw-r--r--   0        0        0     1921 2024-05-14 13:34:50.734320 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/postgres.py
+-rw-r--r--   0        0        0     3583 2024-05-14 13:34:50.734742 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0     2645 2024-05-14 13:34:50.735157 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0     2904 2024-05-14 13:34:50.735724 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/wiremock.py
+-rw-r--r--   0        0        0     1996 2024-03-13 08:33:53.123090 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/__init__.py
+-rw-r--r--   0        0        0     2166 2024-01-20 12:02:32.097410 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/containers.py
+-rw-r--r--   0        0        0     3377 2024-05-14 13:34:50.736372 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/localstack.py
+-rw-r--r--   0        0        0      842 2024-05-14 13:34:50.737037 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/minio.py
+-rw-r--r--   0        0        0     3156 2024-05-14 13:34:50.737452 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/moto.py
+-rw-r--r--   0        0        0      456 2024-05-14 13:34:50.737937 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/mysql.py
+-rw-r--r--   0        0        0      516 2024-05-14 13:34:50.738312 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/postgres.py
+-rw-r--r--   0        0        0     1661 2024-05-14 13:34:50.738775 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/sftp.py
+-rw-r--r--   0        0        0     1038 2024-05-14 13:34:50.739351 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/wiremock.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     2788 2024-05-14 12:22:05.269656 tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0     7188 1970-01-01 00:00:00.000000 tomodachi_testcontainers-1.2.0/PKG-INFO
```

### Comparing `tomodachi_testcontainers-1.1.3/LICENSE` & `tomodachi_testcontainers-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/README.md` & `tomodachi_testcontainers-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/pyproject.toml` & `tomodachi_testcontainers-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "1.1.3"
+version = "1.2.0"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
@@ -210,14 +210,18 @@
     "AWS_SESSION_TOKEN=testing",
     # Testcontainers configuration
     "DOCKER_BUILDKIT=1",
     "TESTCONTAINER_DOCKER_NETWORK=tomodachi-testcontainers",
     "TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile",
     "TESTCONTAINER_DOCKER_BUILD_CONTEXT=examples",
     "TESTCONTAINER_DOCKER_BUILD_TARGET=test",
+    # LocalStack Testcontainer configuration
+    "LOCALSTACK_TESTCONTAINER_DISABLE_LOGGING=1",
+    # Moto Testcontainer configuration
+    "MOTO_TESTCONTAINER_DISABLE_LOGGING=1",
     # WireMock Testcontainer configuration
     "WIREMOCK_TESTCONTAINER_MAPPING_STUBS=tests/containers/test-wiremock-container/mappings",
     "WIREMOCK_TESTCONTAINER_MAPPING_FILES=tests/containers/test-wiremock-container/files",
     "WIREMOCK_TESTCONTAINER_VERBOSE=1",
 ]
 
 [tool.coverage.run]
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/__init__.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/assertions.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/assertions.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/async_probes.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/async_probes.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/clients/snssqs.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/clients/snssqs.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/container.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,33 +21,38 @@
 class DockerContainer(testcontainers.core.container.DockerContainer, abc.ABC):
     """Abstract class for generic Docker containers."""
 
     _container: Optional[Container]
     _name: str
     _logger: logging.Logger
 
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
+    def __init__(self, *args: Any, disable_logging: bool = False, **kwargs: Any) -> None:
         self._set_container_network()
+
         super().__init__(*args, **kwargs, network=self.network)
+
         self._set_default_container_name()
 
+        self._disable_logging = disable_logging
+
     def __enter__(self) -> "DockerContainer":
         try:
             return self.start()
         except ContainerWithSameNameAlreadyExistsError:
             raise
         except Exception:
             self._forward_container_logs_to_logger()
             self.stop()
             raise
 
     def __exit__(
         self, exc_type: Optional[Type[BaseException]], exc_val: Optional[BaseException], exc_tb: Optional[TracebackType]
     ) -> None:
-        self._forward_container_logs_to_logger()
+        if not self._disable_logging:
+            self._forward_container_logs_to_logger()
         self.stop()
 
     @abc.abstractmethod
     def log_message_on_container_start(self) -> str:
         """Returns a message that will be logged when the container starts."""
 
     def with_env(self, key: str, value: str) -> "DockerContainer":
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/database.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,17 +39,18 @@
     database: str
 
     def __init__(
         self,
         image: str,
         internal_port: int,
         edge_port: Optional[int] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
-        super().__init__(image, **kwargs)
+        super().__init__(image, disable_logging=disable_logging, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port or get_available_port()
         self.with_bind_ports(internal_port, self.edge_port)
 
     def get_internal_url(self) -> DatabaseURL:
         return DatabaseURL(
             drivername=self.drivername,
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/image.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/image.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/web.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/common/web.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 
     def __init__(
         self,
         image: str,
         internal_port: int,
         edge_port: Optional[int] = None,
         http_healthcheck_path: Optional[str] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
-        super().__init__(image, **kwargs)
+        super().__init__(image, disable_logging=disable_logging, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port or get_available_port()
         self.http_healthcheck_path = http_healthcheck_path
         self.with_bind_ports(internal_port, self.edge_port)
 
     def get_internal_url(self) -> str:
         ip = self.get_container_internal_ip()
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/dynamodb_admin.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/dynamodb_admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,23 @@
     def __init__(
         self,
         dynamo_endpoint: str,
         image: str = "aaronshaf/dynamodb-admin:latest",
         internal_port: int = 8001,
         edge_port: Optional[int] = None,
         region_name: Optional[str] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image=image,
             internal_port=internal_port,
             edge_port=edge_port,
             http_healthcheck_path="/",
+            disable_logging=disable_logging,
             **kwargs,
         )
 
         self.region_name = region_name or os.getenv("AWS_REGION") or os.getenv("AWS_DEFAULT_REGION") or "us-east-1"
         self.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
         self.aws_secret_access_key = os.getenv("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 
     def __init__(
         self,
         image: str = "localstack/localstack:3",
         internal_port: int = 4566,
         edge_port: Optional[int] = None,
         region_name: Optional[str] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image,
             internal_port=internal_port,
             edge_port=edge_port,
             http_healthcheck_path="/_localstack/health",
+            disable_logging=disable_logging,
             **kwargs,
         )
 
         self.region_name = region_name or os.getenv("AWS_REGION") or os.getenv("AWS_DEFAULT_REGION") or "us-east-1"
         self.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
         self.aws_secret_access_key = os.getenv("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/minio.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/minio.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,23 @@
         self,
         image: str = "minio/minio:latest",
         s3_api_internal_port: int = 9000,
         s3_api_edge_port: Optional[int] = None,
         console_internal_port: int = 9001,
         console_edge_port: Optional[int] = None,
         region_name: Optional[str] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image,
             internal_port=s3_api_internal_port,
             edge_port=s3_api_edge_port,
             http_healthcheck_path="/minio/health/live",
+            disable_logging=disable_logging,
             **kwargs,
         )
         self.s3_api_internal_port = s3_api_internal_port
         self.s3_api_edge_port = self.edge_port
         self.console_internal_port = console_internal_port
         self.console_edge_port = console_edge_port or get_available_port()
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/moto.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 
     def __init__(
         self,
         image: str = "motoserver/moto:latest",
         internal_port: int = 5000,
         edge_port: Optional[int] = None,
         region_name: Optional[str] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image,
             internal_port=internal_port,
             edge_port=edge_port,
             http_healthcheck_path="/moto-api/data.json",
+            disable_logging=disable_logging,
             **kwargs,
         )
 
         self.region_name = region_name or os.getenv("AWS_REGION") or os.getenv("AWS_DEFAULT_REGION") or "us-east-1"
         self.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
         self.aws_secret_access_key = os.getenv("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/mysql.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/mysql.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,20 +27,22 @@
         internal_port: int = 3306,
         edge_port: Optional[int] = None,
         drivername: Optional[str] = None,
         username: Optional[str] = None,
         root_password: Optional[str] = None,
         password: Optional[str] = None,
         database: Optional[str] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image,
             internal_port=internal_port,
             edge_port=edge_port,
+            disable_logging=disable_logging,
             **kwargs,
         )
 
         self.drivername = drivername or os.getenv("MYSQL_DRIVERNAME") or "mysql+pymysql"
         self.username = username or os.getenv("MYSQL_USER") or "username"
         self.root_password = root_password or os.getenv("MYSQL_ROOT_PASSWORD") or "root"
         self.password = password or os.getenv("MYSQL_PASSWORD") or "password"
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/postgres.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/postgres.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,20 +25,22 @@
         image: str = "postgres:16",
         internal_port: int = 5432,
         edge_port: Optional[int] = None,
         drivername: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
         database: Optional[str] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image,
             internal_port=internal_port,
             edge_port=edge_port,
+            disable_logging=disable_logging,
             **kwargs,
         )
 
         self.drivername = drivername or os.getenv("POSTGRES_DRIVERNAME") or "postgresql+psycopg"
         self.username = username or os.getenv("POSTGRES_USER") or "username"
         self.password = password or os.getenv("POSTGRES_PASSWORD") or "password"
         self.database = database or os.getenv("POSTGRES_DB") or "db"
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 class SFTPContainer(DockerContainer):
     def __init__(
         self,
         image: str = "atmoz/sftp:latest",
         internal_port: int = 22,
         edge_port: Optional[int] = None,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
-        super().__init__(image, **kwargs)
+        super().__init__(image, disable_logging=disable_logging, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port or get_available_port()
         self.with_bind_ports(self.internal_port, self.edge_port)
 
         self.with_command("userpass:pass:1001 userssh::1002")
 
         self.authorized_private_key = asyncssh.generate_private_key("ssh-ed25519")
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,23 @@
         self,
         image: str,
         internal_port: int = 9700,
         edge_port: Optional[int] = None,
         http_healthcheck_path: Optional[str] = None,
         *,
         export_coverage: bool = False,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image=image,
             internal_port=internal_port,
             edge_port=edge_port,
             http_healthcheck_path=http_healthcheck_path,
+            disable_logging=disable_logging,
             **kwargs,
         )
         self._export_coverage = export_coverage or bool(os.getenv("TOMODACHI_TESTCONTAINER_EXPORT_COVERAGE"))
         if self._export_coverage:
             self._configure_coverage_export()
 
     def log_message_on_container_start(self) -> str:
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/wiremock.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/containers/wiremock.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,22 @@
         image: str = "wiremock/wiremock:latest",
         internal_port: int = 8080,
         edge_port: Optional[int] = None,
         mapping_stubs: Optional[Path] = None,
         mapping_files: Optional[Path] = None,
         *,
         verbose: bool = False,
+        disable_logging: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             image,
             internal_port=internal_port,
             edge_port=edge_port,
+            disable_logging=disable_logging,
             **kwargs,
         )
 
         mapping_stubs_env = os.getenv("WIREMOCK_TESTCONTAINER_MAPPING_STUBS")
         mapping_files_env = os.getenv("WIREMOCK_TESTCONTAINER_MAPPING_FILES")
 
         self.mapping_stubs = mapping_stubs or (Path(mapping_stubs_env) if mapping_stubs_env else None)
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/__init__.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/containers.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/containers.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/localstack.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/localstack.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from .. import DockerContainer, LocalStackContainer
 from ..clients.snssqs import SNSSQSTestClient
 
 
 @pytest.fixture(scope="session")
 def localstack_container() -> Generator[DockerContainer, None, None]:
     image = os.getenv("LOCALSTACK_TESTCONTAINER_IMAGE_ID", "localstack/localstack:3")
-    with LocalStackContainer(image) as container:
+    disable_logging = bool(os.getenv("LOCALSTACK_TESTCONTAINER_DISABLE_LOGGING")) or False
+
+    with LocalStackContainer(image, disable_logging=disable_logging) as container:
         yield container
 
 
 @pytest.fixture()
 def restart_localstack_container_on_teardown(  # noqa: PT004
     localstack_container: LocalStackContainer,
 ) -> Generator[None, None, None]:
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/minio.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/minio.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 from .. import DockerContainer, MinioContainer
 
 
 @pytest.fixture(scope="session")
 def minio_container() -> Generator[DockerContainer, None, None]:
     image = os.getenv("MINIO_TESTCONTAINER_IMAGE_ID", "minio/minio:latest")
-    with MinioContainer(image) as container:
+    disable_logging = bool(os.getenv("MINIO_TESTCONTAINER_DISABLE_LOGGING")) or False
+
+    with MinioContainer(image, disable_logging=disable_logging) as container:
         yield container
 
 
 @pytest_asyncio.fixture(scope="session")
 async def minio_s3_client(minio_container: MinioContainer) -> AsyncGenerator[S3Client, None]:
     async with get_session().create_client("s3", **minio_container.get_aws_client_config()) as c:
         yield c
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/moto.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/moto.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from .. import DockerContainer, MotoContainer
 from ..clients.snssqs import SNSSQSTestClient
 
 
 @pytest.fixture(scope="session")
 def moto_container() -> Generator[DockerContainer, None, None]:
     image = os.getenv("MOTO_TESTCONTAINER_IMAGE_ID", "motoserver/moto:latest")
-    with MotoContainer(image) as container:
+    disable_logging = bool(os.getenv("MOTO_TESTCONTAINER_DISABLE_LOGGING")) or False
+
+    with MotoContainer(image, disable_logging=disable_logging) as container:
         yield container
 
 
 @pytest.fixture()
 def reset_moto_container_on_teardown(moto_container: MotoContainer) -> Generator[None, None, None]:  # noqa: PT004
     """Removes all mocked resources from Moto after each test without restarting the container."""
     yield
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/sftp.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/sftp.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 from .. import SFTPContainer
 
 
 @pytest.fixture(scope="session")
 def sftp_container() -> Generator[DockerContainer, None, None]:
     image = os.getenv("SFTP_TESTCONTAINER_IMAGE_ID", "atmoz/sftp:latest")
-    with SFTPContainer(image) as container:
+    disable_logging = bool(os.getenv("SFTP_TESTCONTAINER_DISABLE_LOGGING")) or False
+
+    with SFTPContainer(image, disable_logging=disable_logging) as container:
         yield container
 
 
 @pytest_asyncio.fixture(scope="session")
 async def userpass_sftp_client(sftp_container: SFTPContainer) -> AsyncGenerator[asyncssh.SFTPClient, None]:
     conn_details = sftp_container.get_external_conn_details()
     async with asyncssh.connect(
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/wiremock.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/fixtures/wiremock.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 except ImportError:
     WireMockConfig = None
 
 
 @pytest.fixture(scope="session")
 def wiremock_container() -> Generator[WireMockContainer, None, None]:
     image = os.getenv("WIREMOCK_TESTCONTAINER_IMAGE_ID", "wiremock/wiremock:latest")
-    with WireMockContainer(image) as container:
+    disable_logging = bool(os.getenv("WIREMOCK_TESTCONTAINER_DISABLE_LOGGING")) or False
+
+    with WireMockContainer(image, disable_logging=disable_logging) as container:
         container = cast(WireMockContainer, container)
         if WireMockConfig is not None:
             WireMockConfig.base_url = f"{container.get_external_url()}/__admin/"
         yield container
 
 
 @pytest.fixture()
```

### Comparing `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/utils.py` & `tomodachi_testcontainers-1.2.0/src/tomodachi_testcontainers/utils.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.3/PKG-INFO` & `tomodachi_testcontainers-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 1.1.3
+Version: 1.2.0
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

