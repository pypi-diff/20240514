# Comparing `tmp/testcontainers-4.4.0.tar.gz` & `tmp/testcontainers-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-4.4.0.tar", max compression
+gzip compressed data, was "testcontainers-4.4.1.tar", max compression
```

## Comparing `testcontainers-4.4.0.tar` & `testcontainers-4.4.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0    11328 2024-04-17 10:36:58.085342 testcontainers-4.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2042 2024-04-17 10:36:58.085342 testcontainers-4.4.0/README.md
--rw-r--r--   0        0        0      172 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/compose/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/compose/compose.py
--rw-r--r--   0        0        0        0 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/__init__.py
--rw-r--r--   0        0        0     2433 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/config.py
--rw-r--r--   0        0        0     8712 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/container.py
--rw-r--r--   0        0        0     6926 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/docker_client.py
--rw-r--r--   0        0        0      734 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/exceptions.py
--rw-r--r--   0        0        0     2418 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/generic.py
--rw-r--r--   0        0        0      978 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/labels.py
--rw-r--r--   0        0        0     1543 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/network.py
--rw-r--r--   0        0        0     2088 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/utils.py
--rw-r--r--   0        0        0     4069 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/waiting_utils.py
--rw-r--r--   0        0        0     3781 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/arangodb/testcontainers/arangodb/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/azurite/testcontainers/azurite/__init__.py
--rw-r--r--   0        0        0     2492 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/cassandra/testcontainers/cassandra/__init__.py
--rw-r--r--   0        0        0     2736 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/chroma/testcontainers/chroma/__init__.py
--rw-r--r--   0        0        0     3030 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/clickhouse/testcontainers/clickhouse/__init__.py
--rw-r--r--   0        0        0     3886 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
--rw-r--r--   0        0        0      106 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/google/testcontainers/google/__init__.py
--rw-r--r--   0        0        0     2709 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/google/testcontainers/google/datastore.py
--rw-r--r--   0        0        0     2952 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/google/testcontainers/google/pubsub.py
--rw-r--r--   0        0        0     3760 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb.py
--rw-r--r--   0        0        0     2387 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb1/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb2/__init__.py
--rw-r--r--   0        0        0     2694 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/k3s/testcontainers/k3s/__init__.py
--rw-r--r--   0        0        0     3592 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/kafka/testcontainers/kafka/__init__.py
--rw-r--r--   0        0        0     2727 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/kafka/testcontainers/kafka/_redpanda.py
--rw-r--r--   0        0        0     3313 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/keycloak/testcontainers/keycloak/__init__.py
--rw-r--r--   0        0        0     3222 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/localstack/testcontainers/localstack/__init__.py
--rw-r--r--   0        0        0     4116 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/minio/testcontainers/minio/__init__.py
--rw-r--r--   0        0        0     3017 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/mongodb/testcontainers/mongodb/__init__.py
--rw-r--r--   0        0        0     2202 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/mssql/testcontainers/mssql/__init__.py
--rw-r--r--   0        0        0     3535 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/mysql/testcontainers/mysql/__init__.py
--rw-r--r--   0        0        0     2811 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/nats/testcontainers/nats/__init__.py
--rw-r--r--   0        0        0     2782 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/neo4j/testcontainers/neo4j/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/nginx/testcontainers/nginx/__init__.py
--rw-r--r--   0        0        0     4109 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/opensearch/testcontainers/opensearch/__init__.py
--rw-r--r--   0        0        0     2960 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/oracle-free/testcontainers/oracle/__init__.py
--rw-r--r--   0        0        0     3984 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/postgres/testcontainers/postgres/__init__.py
--rw-r--r--   0        0        0     5209 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/qdrant/testcontainers/qdrant/__init__.py
--rw-r--r--   0        0        0     2967 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3144 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/redis/testcontainers/redis/__init__.py
--rw-r--r--   0        0        0     2761 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/registry/testcontainers/registry/__init__.py
--rw-r--r--   0        0        0     2722 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/selenium/testcontainers/selenium/__init__.py
--rw-r--r--   0        0        0     2519 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/vault/testcontainers/vault/__init__.py
--rw-r--r--   0        0        0     5588 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/weaviate/testcontainers/weaviate/__init__.py
--rw-r--r--   0        0        0     8755 2024-04-17 10:36:58.097342 testcontainers-4.4.0/pyproject.toml
--rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 testcontainers-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11328 2024-05-14 07:49:02.803210 testcontainers-4.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     2042 2024-05-14 07:49:02.803210 testcontainers-4.4.1/README.md
+-rw-r--r--   0        0        0      172 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/compose/__init__.py
+-rw-r--r--   0        0        0    13096 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/compose/compose.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/__init__.py
+-rw-r--r--   0        0        0     2433 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/config.py
+-rw-r--r--   0        0        0     8875 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/container.py
+-rw-r--r--   0        0        0     6926 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/docker_client.py
+-rw-r--r--   0        0        0      734 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/exceptions.py
+-rw-r--r--   0        0        0     2591 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/generic.py
+-rw-r--r--   0        0        0      978 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/labels.py
+-rw-r--r--   0        0        0     1543 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/network.py
+-rw-r--r--   0        0        0     2088 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/utils.py
+-rw-r--r--   0        0        0     4069 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/waiting_utils.py
+-rw-r--r--   0        0        0     3781 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/arangodb/testcontainers/arangodb/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/azurite/testcontainers/azurite/__init__.py
+-rw-r--r--   0        0        0     2492 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/cassandra/testcontainers/cassandra/__init__.py
+-rw-r--r--   0        0        0     2736 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/chroma/testcontainers/chroma/__init__.py
+-rw-r--r--   0        0        0     3030 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/clickhouse/testcontainers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     3886 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/google/testcontainers/google/__init__.py
+-rw-r--r--   0        0        0     2709 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/google/testcontainers/google/datastore.py
+-rw-r--r--   0        0        0     2952 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/google/testcontainers/google/pubsub.py
+-rw-r--r--   0        0        0     3760 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb.py
+-rw-r--r--   0        0        0     2387 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb1/__init__.py
+-rw-r--r--   0        0        0     4464 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb2/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/k3s/testcontainers/k3s/__init__.py
+-rw-r--r--   0        0        0     3592 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/kafka/testcontainers/kafka/__init__.py
+-rw-r--r--   0        0        0     2727 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/kafka/testcontainers/kafka/_redpanda.py
+-rw-r--r--   0        0        0     4249 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/keycloak/testcontainers/keycloak/__init__.py
+-rw-r--r--   0        0        0     3222 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/localstack/testcontainers/localstack/__init__.py
+-rw-r--r--   0        0        0     2042 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/memcached/testcontainers/memcached/__init__.py
+-rw-r--r--   0        0        0     4116 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/minio/testcontainers/minio/__init__.py
+-rw-r--r--   0        0        0     3017 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/mongodb/testcontainers/mongodb/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/mssql/testcontainers/mssql/__init__.py
+-rw-r--r--   0        0        0     4984 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/mysql/testcontainers/mysql/__init__.py
+-rw-r--r--   0        0        0     2811 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/nats/testcontainers/nats/__init__.py
+-rw-r--r--   0        0        0     2782 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/neo4j/testcontainers/neo4j/__init__.py
+-rw-r--r--   0        0        0     1596 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/nginx/testcontainers/nginx/__init__.py
+-rw-r--r--   0        0        0     4109 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/opensearch/testcontainers/opensearch/__init__.py
+-rw-r--r--   0        0        0     2960 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/oracle-free/testcontainers/oracle/__init__.py
+-rw-r--r--   0        0        0     3984 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/postgres/testcontainers/postgres/__init__.py
+-rw-r--r--   0        0        0     5209 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/qdrant/testcontainers/qdrant/__init__.py
+-rw-r--r--   0        0        0     2967 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3144 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/redis/testcontainers/redis/__init__.py
+-rw-r--r--   0        0        0     2761 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/registry/testcontainers/registry/__init__.py
+-rw-r--r--   0        0        0     4272 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/selenium/testcontainers/selenium/__init__.py
+-rw-r--r--   0        0        0     1432 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/selenium/testcontainers/selenium/video.py
+-rw-r--r--   0        0        0     2519 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/vault/testcontainers/vault/__init__.py
+-rw-r--r--   0        0        0     5588 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/weaviate/testcontainers/weaviate/__init__.py
+-rw-r--r--   0        0        0     8834 2024-05-14 07:49:02.815210 testcontainers-4.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5554 1970-01-01 00:00:00.000000 testcontainers-4.4.1/PKG-INFO
```

### Comparing `testcontainers-4.4.0/LICENSE.txt` & `testcontainers-4.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/README.md` & `testcontainers-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/compose/compose.py` & `testcontainers-4.4.1/core/testcontainers/compose/compose.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/core/config.py` & `testcontainers-4.4.1/core/testcontainers/core/config.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/core/container.py` & `testcontainers-4.4.1/core/testcontainers/core/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 
     def start(self) -> Self:
         if not c.ryuk_disabled and self.image != c.ryuk_image:
             logger.debug("Creating Ryuk container")
             Reaper.get_instance()
         logger.info("Pulling image %s", self.image)
         docker_client = self.get_docker_client()
+        self._configure()
         self._container = docker_client.run(
             self.image,
             command=self._command,
             detach=True,
             environment=self.env,
             ports=self.ports,
             name=self._name,
@@ -172,14 +173,18 @@
         return self._container.logs(stderr=False), self._container.logs(stdout=False)
 
     def exec(self, command) -> tuple[int, str]:
         if not self._container:
             raise ContainerStartException("Container should be started before executing a command")
         return self._container.exec_run(command)
 
+    def _configure(self) -> None:
+        # placeholder if subclasses want to define this and use the default start method
+        pass
+
 
 class Reaper:
     _instance: "Optional[Reaper]" = None
     _container: Optional[DockerContainer] = None
     _socket: Optional[socket] = None
 
     @classmethod
```

### Comparing `testcontainers-4.4.0/core/testcontainers/core/docker_client.py` & `testcontainers-4.4.1/core/testcontainers/core/docker_client.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/core/exceptions.py` & `testcontainers-4.4.1/core/testcontainers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/core/generic.py` & `testcontainers-4.4.1/core/testcontainers/core/generic.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 from typing import Optional
+from urllib.parse import quote
 
 from testcontainers.core.container import DockerContainer
 from testcontainers.core.exceptions import ContainerStartException
 from testcontainers.core.utils import raise_for_deprecated_parameter
 from testcontainers.core.waiting_utils import wait_container_is_ready
 
 ADDITIONAL_TRANSIENT_ERRORS = []
@@ -56,20 +57,25 @@
     ) -> str:
         if raise_for_deprecated_parameter(kwargs, "db_name", "dbname"):
             raise ValueError(f"Unexpected arguments: {','.join(kwargs)}")
         if self._container is None:
             raise ContainerStartException("container has not been started")
         host = host or self.get_container_host_ip()
         port = self.get_exposed_port(port)
-        url = f"{dialect}://{username}:{password}@{host}:{port}"
+        quoted_password = quote(password, safe=" +")
+        url = f"{dialect}://{username}:{quoted_password}@{host}:{port}"
         if dbname:
             url = f"{url}/{dbname}"
         return url
 
     def start(self) -> "DbContainer":
         self._configure()
         super().start()
+        self._transfer_seed()
         self._connect()
         return self
 
     def _configure(self) -> None:
         raise NotImplementedError
+
+    def _transfer_seed(self) -> None:
+        pass
```

### Comparing `testcontainers-4.4.0/core/testcontainers/core/labels.py` & `testcontainers-4.4.1/core/testcontainers/core/labels.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/core/network.py` & `testcontainers-4.4.1/core/testcontainers/core/network.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/core/utils.py` & `testcontainers-4.4.1/core/testcontainers/core/utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/core/testcontainers/core/waiting_utils.py` & `testcontainers-4.4.1/core/testcontainers/core/waiting_utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/arangodb/testcontainers/arangodb/__init__.py` & `testcontainers-4.4.1/modules/arangodb/testcontainers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/azurite/testcontainers/azurite/__init__.py` & `testcontainers-4.4.1/modules/azurite/testcontainers/azurite/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/cassandra/testcontainers/cassandra/__init__.py` & `testcontainers-4.4.1/modules/cassandra/testcontainers/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/chroma/testcontainers/chroma/__init__.py` & `testcontainers-4.4.1/modules/chroma/testcontainers/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/clickhouse/testcontainers/clickhouse/__init__.py` & `testcontainers-4.4.1/modules/clickhouse/testcontainers/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py` & `testcontainers-4.4.1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/google/testcontainers/google/datastore.py` & `testcontainers-4.4.1/modules/google/testcontainers/google/datastore.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/google/testcontainers/google/pubsub.py` & `testcontainers-4.4.1/modules/google/testcontainers/google/pubsub.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb.py` & `testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb1/__init__.py` & `testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb1/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb2/__init__.py` & `testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/k3s/testcontainers/k3s/__init__.py` & `testcontainers-4.4.1/modules/k3s/testcontainers/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/kafka/testcontainers/kafka/__init__.py` & `testcontainers-4.4.1/modules/kafka/testcontainers/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/kafka/testcontainers/kafka/_redpanda.py` & `testcontainers-4.4.1/modules/kafka/testcontainers/kafka/_redpanda.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/keycloak/testcontainers/keycloak/__init__.py` & `testcontainers-4.4.1/modules/keycloak/testcontainers/keycloak/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_container_is_ready, wait_for_logs
 
 _DEFAULT_DEV_COMMAND = "start-dev"
 
 
 class KeycloakContainer(DockerContainer):
+    has_realm_imports = False
+
     """
     Keycloak container.
 
     Example:
 
         .. doctest::
 
@@ -39,50 +41,70 @@
 
     def __init__(
         self,
         image="quay.io/keycloak/keycloak:latest",
         username: Optional[str] = None,
         password: Optional[str] = None,
         port: int = 8080,
+        cmd: Optional[str] = _DEFAULT_DEV_COMMAND,
     ) -> None:
         super().__init__(image=image)
         self.username = username or os.environ.get("KEYCLOAK_ADMIN", "test")
         self.password = password or os.environ.get("KEYCLOAK_ADMIN_PASSWORD", "test")
         self.port = port
         self.with_exposed_ports(self.port)
+        self.cmd = cmd
 
     def _configure(self) -> None:
         self.with_env("KEYCLOAK_ADMIN", self.username)
         self.with_env("KEYCLOAK_ADMIN_PASSWORD", self.password)
         # Enable health checks
         # see: https://www.keycloak.org/server/health#_relevant_options
         self.with_env("KC_HEALTH_ENABLED", "true")
-        # Starting Keycloak in development mode
+        # Start Keycloak in development mode
         # see: https://www.keycloak.org/server/configuration#_starting_keycloak_in_development_mode
-        self.with_command(_DEFAULT_DEV_COMMAND)
+        if self.has_realm_imports:
+            self.cmd += " --import-realm"
+        self.with_command(self.cmd)
 
     def get_url(self) -> str:
         host = self.get_container_host_ip()
         port = self.get_exposed_port(self.port)
         return f"http://{host}:{port}"
 
     @wait_container_is_ready(requests.exceptions.ConnectionError, requests.exceptions.ReadTimeout)
     def _readiness_probe(self) -> None:
-        # Keycloak provides an REST API endpoints for health checks: https://www.keycloak.org/server/health
+        # Keycloak provides REST API endpoints for health checks: https://www.keycloak.org/server/health
         response = requests.get(f"{self.get_url()}/health/ready", timeout=1)
         response.raise_for_status()
-        if self._command == _DEFAULT_DEV_COMMAND:
+        if _DEFAULT_DEV_COMMAND in self._command:
             wait_for_logs(self, "Added user .* to realm .*")
 
     def start(self) -> "KeycloakContainer":
         self._configure()
         super().start()
         self._readiness_probe()
         return self
 
+    def with_realm_import_file(self, realm_import_file: str) -> "KeycloakContainer":
+        file = os.path.abspath(realm_import_file)
+        if not os.path.exists(file):
+            raise FileNotFoundError(f"Realm file {file} does not exist")
+        self.with_volume_mapping(file, "/opt/keycloak/data/import/realm.json")
+        self.has_realm_imports = True
+        return self
+
+    def with_realm_import_folder(self, realm_import_folder: str) -> "KeycloakContainer":
+        folder = os.path.abspath(realm_import_folder)
+        if not os.path.exists(folder):
+            raise FileNotFoundError(f"Realm folder {folder} does not exist")
+        self.with_volume_mapping(folder, "/opt/keycloak/data/import/")
+        self.has_realm_imports = True
+        return self
+
     def get_client(self, **kwargs) -> KeycloakAdmin:
         default_kwargs = {
             "server_url": self.get_url(),
             "username": self.username,
             "password": self.password,
             "realm_name": "master",
             "verify": True,
```

### Comparing `testcontainers-4.4.0/modules/localstack/testcontainers/localstack/__init__.py` & `testcontainers-4.4.1/modules/localstack/testcontainers/localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/minio/testcontainers/minio/__init__.py` & `testcontainers-4.4.1/modules/minio/testcontainers/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/mongodb/testcontainers/mongodb/__init__.py` & `testcontainers-4.4.1/modules/mongodb/testcontainers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/mssql/testcontainers/mssql/__init__.py` & `testcontainers-4.4.1/modules/mssql/testcontainers/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/nats/testcontainers/nats/__init__.py` & `testcontainers-4.4.1/modules/nats/testcontainers/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/neo4j/testcontainers/neo4j/__init__.py` & `testcontainers-4.4.1/modules/neo4j/testcontainers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/nginx/testcontainers/nginx/__init__.py` & `testcontainers-4.4.1/modules/nginx/testcontainers/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/opensearch/testcontainers/opensearch/__init__.py` & `testcontainers-4.4.1/modules/opensearch/testcontainers/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/oracle-free/testcontainers/oracle/__init__.py` & `testcontainers-4.4.1/modules/oracle-free/testcontainers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/postgres/testcontainers/postgres/__init__.py` & `testcontainers-4.4.1/modules/postgres/testcontainers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/qdrant/testcontainers/qdrant/__init__.py` & `testcontainers-4.4.1/modules/qdrant/testcontainers/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py` & `testcontainers-4.4.1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/redis/testcontainers/redis/__init__.py` & `testcontainers-4.4.1/modules/redis/testcontainers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/registry/testcontainers/registry/__init__.py` & `testcontainers-4.4.1/modules/registry/testcontainers/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/selenium/testcontainers/selenium/__init__.py` & `testcontainers-4.4.1/modules/memcached/testcontainers/memcached/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,69 +6,54 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
+import socket
 
-from typing import Optional
-
-import urllib3
-
-from selenium import webdriver
-from selenium.webdriver.common.options import ArgOptions
 from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_container_is_ready
 
-IMAGES = {"firefox": "selenium/standalone-firefox-debug:latest", "chrome": "selenium/standalone-chrome-debug:latest"}
-
 
-def get_image_name(capabilities: str) -> str:
-    return IMAGES[capabilities["browserName"]]
+class MemcachedNotReady(Exception):
+    pass
 
 
-class BrowserWebDriverContainer(DockerContainer):
+class MemcachedContainer(DockerContainer):
     """
-    Selenium browser container for Chrome or Firefox.
+    Test container for Memcached. The example below spins up a Memcached server
 
     Example:
 
         .. doctest::
 
-            >>> from testcontainers.selenium import BrowserWebDriverContainer
-            >>> from selenium.webdriver import DesiredCapabilities
+            >>> from testcontainers.memcached import MemcachedContainer
 
-            >>> with BrowserWebDriverContainer(DesiredCapabilities.CHROME) as chrome:
-            ...    webdriver = chrome.get_driver()
-
-        You can easily change browser by passing :code:`DesiredCapabilities.FIREFOX` instead.
+            >>> with MemcachedContainer() as memcached_container:
+            ...    host, port = memcached_container.get_host_and_port()
     """
 
-    def __init__(
-        self, capabilities: str, image: Optional[str] = None, port: int = 4444, vnc_port: int = 5900, **kwargs
-    ) -> None:
-        self.capabilities = capabilities
-        self.image = image or get_image_name(capabilities)
-        self.port = port
-        self.vnc_port = vnc_port
-        super().__init__(image=self.image, **kwargs)
-        self.with_exposed_ports(self.port, self.vnc_port)
-
-    def _configure(self) -> None:
-        self.with_env("no_proxy", "localhost")
-        self.with_env("HUB_ENV_no_proxy", "localhost")
-
-    @wait_container_is_ready(urllib3.exceptions.HTTPError)
-    def _connect(self) -> webdriver.Remote:
-        options = ArgOptions()
-        for key, value in self.capabilities.items():
-            options.set_capability(key, value)
-        return webdriver.Remote(command_executor=(self.get_connection_url()), options=options)
-
-    def get_driver(self) -> webdriver.Remote:
-        return self._connect()
-
-    def get_connection_url(self) -> str:
-        ip = self.get_container_host_ip()
-        port = self.get_exposed_port(self.port)
-        return f"http://{ip}:{port}/wd/hub"
+    def __init__(self, image="memcached:1", port_to_expose=11211, **kwargs):
+        super().__init__(image, **kwargs)
+        self.port_to_expose = port_to_expose
+        self.with_exposed_ports(port_to_expose)
+
+    @wait_container_is_ready(MemcachedNotReady)
+    def _connect(self):
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+            host = self.get_container_host_ip()
+            port = int(self.get_exposed_port(self.port_to_expose))
+            s.connect((host, port))
+            s.sendall(b"stats\n\r")
+            data = s.recv(1024)
+            if len(data) == 0:
+                raise MemcachedNotReady("Memcached not ready yet")
+
+    def start(self):
+        super().start()
+        self._connect()
+        return self
+
+    def get_host_and_port(self):
+        return self.get_container_host_ip(), int(self.get_exposed_port(self.port_to_expose))
```

### Comparing `testcontainers-4.4.0/modules/vault/testcontainers/vault/__init__.py` & `testcontainers-4.4.1/modules/vault/testcontainers/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/modules/weaviate/testcontainers/weaviate/__init__.py` & `testcontainers-4.4.1/modules/weaviate/testcontainers/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.0/pyproject.toml` & `testcontainers-4.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testcontainers"
-version = "4.4.0"  # auto-incremented by release-please
+version = "4.4.1"  # auto-incremented by release-please
 description = "Python library for throwaway instances of anything that can run in a Docker container"
 authors = ["Sergey Pirogov <automationremarks@gmail.com>"]
 maintainers = [
     "Balint Bartha <totallyzen@users.noreply.github.com>",
     "David Ankin <daveankin@gmail.com>",
     "Vemund Santi <vemund@santi.no>"
 ]
@@ -36,14 +36,15 @@
     { include = "testcontainers", from = "modules/elasticsearch" },
     { include = "testcontainers", from = "modules/google" },
     { include = "testcontainers", from = "modules/influxdb" },
     { include = "testcontainers", from = "modules/k3s" },
     { include = "testcontainers", from = "modules/kafka" },
     { include = "testcontainers", from = "modules/keycloak" },
     { include = "testcontainers", from = "modules/localstack" },
+    { include = "testcontainers", from = "modules/memcached" },
     { include = "testcontainers", from = "modules/minio" },
     { include = "testcontainers", from = "modules/mongodb" },
     { include = "testcontainers", from = "modules/mssql" },
     { include = "testcontainers", from = "modules/mysql" },
     { include = "testcontainers", from = "modules/nats" },
     { include = "testcontainers", from = "modules/neo4j" },
     { include = "testcontainers", from = "modules/nginx" },
@@ -107,14 +108,15 @@
 elasticsearch = []
 google = ["google-cloud-pubsub", "google-cloud-datastore"]
 influxdb = ["influxdb", "influxdb-client"]
 k3s = ["kubernetes", "pyyaml"]
 kafka = []
 keycloak = ["python-keycloak"]
 localstack = ["boto3"]
+memcached = []
 minio = ["minio"]
 mongodb = ["pymongo"]
 mssql = ["sqlalchemy", "pymssql"]
 mysql = ["sqlalchemy", "pymysql"]
 nats = ["nats-py"]
 neo4j = ["neo4j"]
 nginx = []
```

### Comparing `testcontainers-4.4.0/PKG-INFO` & `testcontainers-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers
-Version: 4.4.0
+Version: 4.4.1
 Summary: Python library for throwaway instances of anything that can run in a Docker container
 Keywords: testing,logging,docker,test automation
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Maintainer: Balint Bartha
 Maintainer-email: totallyzen@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -29,14 +29,15 @@
 Provides-Extra: elasticsearch
 Provides-Extra: google
 Provides-Extra: influxdb
 Provides-Extra: k3s
 Provides-Extra: kafka
 Provides-Extra: keycloak
 Provides-Extra: localstack
+Provides-Extra: memcached
 Provides-Extra: minio
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: nats
 Provides-Extra: neo4j
 Provides-Extra: nginx
```

