# Comparing `tmp/bert_server_client-1.1.3.tar.gz` & `tmp/bert_server_client-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_server_client-1.1.3.tar", last modified: Fri Mar  8 09:49:38 2024, max compression
+gzip compressed data, was "bert_server_client-1.2.3.tar", last modified: Tue May 14 13:56:40 2024, max compression
```

## Comparing `bert_server_client-1.1.3.tar` & `bert_server_client-1.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:49:38.649698 bert_server_client-1.1.3/
--rw-r--r--   0 root         (0) root         (0)      320 2024-03-08 09:49:38.649698 bert_server_client-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6220 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:49:38.646698 bert_server_client-1.1.3/bert_server_client/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4077 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:49:38.648698 bert_server_client-1.1.3/bert_server_client/schema/
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4291 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/schema/embedding.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/schema/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/schema/zmq_message_header.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:49:38.649698 bert_server_client-1.1.3/bert_server_client/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/tests/client_integration_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/tests/test_msgpack.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/bert_server_client/tests/test_zmq_message_header.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:49:38.647698 bert_server_client-1.1.3/bert_server_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      320 2024-03-08 09:49:38.000000 bert_server_client-1.1.3/bert_server_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2024-03-08 09:49:38.000000 bert_server_client-1.1.3/bert_server_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 09:49:38.000000 bert_server_client-1.1.3/bert_server_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-03-08 09:49:38.000000 bert_server_client-1.1.3/bert_server_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-08 09:49:38.000000 bert_server_client-1.1.3/bert_server_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 09:49:38.649698 bert_server_client-1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      740 2024-03-08 09:49:35.000000 bert_server_client-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.411595 bert_server_client-1.2.3/bert_server_client/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5034 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.413595 bert_server_client-1.2.3/bert_server_client/schema/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4291 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/embedding.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/zmq_message_header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/bert_server_client/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/client_integration_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_msgpack.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_zmq_message_header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.412595 bert_server_client-1.2.3/bert_server_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/setup.py
```

### Comparing `bert_server_client-1.1.3/README.md` & `bert_server_client-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/bert_server_client/client.py` & `bert_server_client-1.2.3/bert_server_client/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import zmq
 
 from typing import Optional, List
 
 from bert_server_client.error import BertClientError
 from bert_server_client.schema.base import Base, T
-from bert_server_client.schema.embedding import Embedding, EmbeddingRequest, EmbeddingResponse
+from bert_server_client.schema.embedding import Embedding, EmbeddingRequest, EmbeddingResponse, EmbeddingQueryRequest, EmbeddingQueryResponse
 from bert_server_client.schema.health_check import HealthCheck
 from bert_server_client.schema.zmq_message_header import ZmqMessageHeader, create_message_header, ZmqMessageStatus, \
     ZmqMessageType
 
 
 class BertClient:
     def __init__(self, host: str):
@@ -98,14 +98,34 @@
         if not isinstance(request, EmbeddingRequest):
             raise ValueError("Invalid request type provided")
 
         if isinstance(request.input, str):
             request.input = [request.input]
 
         return self._send_request(ZmqMessageType.EMBEDDING, request)
+    
+    def send_embedding_query_request(self, request: EmbeddingQueryRequest) -> Optional[EmbeddingQueryResponse]:
+        """
+        Sends an embedding query request to the BERT server and waits for a response.
+
+        Args:
+            request (EmbeddingQueryRequest): The request object containing the query data for embedding.
+
+        Returns:
+            Optional[EmbeddingQueryResponse]: The chunks (list of strings) from the BERT server.
+            None if an exception occurs during the request.
+
+        Raises:
+            ValueError: If the provided request is not of type EmbeddingQueryRequest.
+            Exception: For any network-related errors or data packing/unpacking issues.
+        """
+        if not isinstance(request, EmbeddingQueryRequest):
+            raise ValueError("Invalid request type provided")
+
+        return self._send_request(ZmqMessageType.EMBEDDING_QUERY, request)
 
     def send_health_check_request(self) -> Optional[HealthCheck]:
         """
         Sends a HealthCheck request to the server and waits for a HealthCheck response.
 
         :return: A HealthCheck response or None
         """
```

### Comparing `bert_server_client-1.1.3/bert_server_client/error.py` & `bert_server_client-1.2.3/bert_server_client/error.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/bert_server_client/schema/base.py` & `bert_server_client-1.2.3/bert_server_client/schema/base.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/bert_server_client/schema/embedding.py` & `bert_server_client-1.2.3/bert_server_client/schema/embedding.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,19 +23,43 @@
     object: str
     data: List[Embedding]
     model: Optional[str] = field(default=None)
     usage: Optional[EmbeddingUsage] = field(default=None)
 
 
 @dataclass
+class EmbeddingQueryResponse(Base):
+    object: str
+    data: List[str]
+    model: Optional[str] = field(default=None)
+    usage: Optional[EmbeddingUsage] = field(default=None)
+
+
+@dataclass
 class EmbeddingRequest(Base):
     input: Union[str, List[str]]
     model: str
     encoding_format: Optional[str] = field(default="float")
     dimensions: Optional[int] = field(default=None)
     user: Optional[UUID] = field(default=None)
+    doc_id: Optional[str] = field(default=None) # Currently mocked not derived from URL
+
+    @classmethod
+    def decode_map(cls) -> Dict[str, Any]:
+        return {
+            "user": UUID,
+        }
+    
+
+@dataclass
+class EmbeddingQueryRequest(Base):
+    input: str
+    model: str
+    encoding_format: Optional[str] = field(default="float")
+    dimensions: Optional[int] = field(default=None)
+    user: Optional[UUID] = field(default=None)
 
     @classmethod
     def decode_map(cls) -> Dict[str, Any]:
         return {
             "user": UUID,
         }
```

### Comparing `bert_server_client-1.1.3/bert_server_client/schema/zmq_message_header.py` & `bert_server_client-1.2.3/bert_server_client/schema/zmq_message_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import Optional, Dict, Any
 from uuid import UUID
 
 from bert_server_client.schema.base import Base
-from bert_server_client.schema.embedding import EmbeddingResponse
+from bert_server_client.schema.embedding import EmbeddingResponse, EmbeddingQueryResponse
 from bert_server_client.schema.health_check import HealthCheck
 
 
 class ZmqMessageType(Enum):
     """
     ZmqMessageType defines the types of messages used in a ZeroMQ messaging system.
     Each type is associated with a specific class for handling its data.
     """
     EMBEDDING = 1
-    HEALTH_CHECK = 2
-    UNKNOWN = 3
+    EMBEDDING_QUERY = 2
+    HEALTH_CHECK = 3
+    UNKNOWN = 4
 
     @property
     def get_associated_class(self):
         return {
             ZmqMessageType.EMBEDDING: EmbeddingResponse,
+            ZmqMessageType.EMBEDDING_QUERY: EmbeddingQueryResponse,
             ZmqMessageType.HEALTH_CHECK: HealthCheck,
             ZmqMessageType.UNKNOWN: lambda x: None,
         }.get(self, lambda x: None)
 
 
 class ZmqMessageStatus(Enum):
     """
```

### Comparing `bert_server_client-1.1.3/bert_server_client/tests/test_base.py` & `bert_server_client-1.2.3/bert_server_client/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/bert_server_client/tests/test_client.py` & `bert_server_client-1.2.3/bert_server_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/bert_server_client/tests/test_msgpack.py` & `bert_server_client-1.2.3/bert_server_client/tests/test_msgpack.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from uuid import UUID, uuid4
 from dataclasses import dataclass
 from typing import Optional, Dict, Any
 
 from polyfactory.factories import DataclassFactory
 
 from bert_server_client.schema.base import Base
-from bert_server_client.schema.embedding import EmbeddingRequest, EmbeddingResponse
+from bert_server_client.schema.embedding import EmbeddingRequest, EmbeddingResponse, EmbeddingQueryRequest, EmbeddingQueryResponse
 
 
 @dataclass
 class MyMapClass(Base):
     dummy: str
     key_values: Optional[Dict[str, Any]] = None  # Optional key_values for advanced options
 
@@ -79,7 +79,40 @@
     packed = embedding_response.msgpack_pack()
 
     unpacked = embedding_response.msgpack_unpack(packed)
 
     print(unpacked.to_json_str())
 
     assert embedding_response == unpacked
+
+
+# Duplicate for EmbeddingQuery
+
+
+class EmbeddingQueryRequestFactory(DataclassFactory[EmbeddingQueryRequest]):
+    __model__ = EmbeddingQueryRequest
+
+
+def test_embedding_query_request_factory():
+    """
+    Test if the datetime encoding and decoding works correctly.
+    """
+    query_request = EmbeddingQueryRequestFactory.build()
+    print(query_request.to_json_str())
+    packed_request = query_request.msgpack_pack()
+    unpacked_request = EmbeddingQueryRequest.msgpack_unpack(packed_request)
+    assert query_request == unpacked_request
+
+
+class EmbeddingQueryResponseFactory(DataclassFactory[EmbeddingQueryResponse]):
+    __model__ = EmbeddingQueryResponse
+
+
+def test_embedding_query_response_factory():
+    """
+    Test if the datetime encoding and decoding works correctly.
+    """
+    query_response = EmbeddingQueryResponseFactory.build()
+    print(query_response.to_json_str())
+    packed_response = query_response.msgpack_pack()
+    unpacked_response = EmbeddingQueryResponse.msgpack_unpack(packed_response)
+    assert query_response == unpacked_response
```

### Comparing `bert_server_client-1.1.3/bert_server_client/tests/test_zmq_message_header.py` & `bert_server_client-1.2.3/bert_server_client/tests/test_zmq_message_header.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/bert_server_client.egg-info/SOURCES.txt` & `bert_server_client-1.2.3/bert_server_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/pyproject.toml` & `bert_server_client-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.1.3/setup.py` & `bert_server_client-1.2.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert_server_client",
-    version="1.1.3",
+    version="1.2.3",
     packages=find_packages(),
     package_data={'bert_server_client': ['schema/*']},
     author="Anil Aydiner",
     author_email="a.aydiner@qimia.de",
     description="A ZMQ client interface for Bert server",
     long_description="A ZMQ client interface for Bert server",
     url="https://gitlab.com/qimiaio/qimia-ai-dev/bert-server-client",
```

