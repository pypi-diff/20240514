# Comparing `tmp/kuksa_client-0.4.3a1.tar.gz` & `tmp/kuksa_client-0.4.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuksa_client-0.4.3a1.tar", last modified: Fri May 10 09:26:27 2024, max compression
+gzip compressed data, was "kuksa_client-0.4.3a2.tar", last modified: Tue May 14 08:41:26 2024, max compression
```

## Comparing `kuksa_client-0.4.3a1.tar` & `kuksa_client-0.4.3a2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/
--rw-r--r--   0 erik      (1000) erik      (1000)    11357 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)       35 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)     4180 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     2941 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa/val/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa/val/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa/val/v1/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa/val/v1/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    10052 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)    13964 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2.pyi
--rw-r--r--   0 erik      (1000) erik      (1000)     1135 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2_grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4117 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4416 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2.pyi
--rw-r--r--   0 erik      (1000) erik      (1000)    10435 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2_grpc.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa_client/
--rw-r--r--   0 erik      (1000) erik      (1000)     4630 2024-04-29 12:30:35.000000 kuksa_client-0.4.3a1/kuksa_client/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    26983 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/__main__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1761 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/_metadata.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa_client/cli_backend/
--rw-r--r--   0 erik      (1000) erik      (1000)     2083 2024-05-07 11:27:06.000000 kuksa_client-0.4.3a1/kuksa_client/cli_backend/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    12316 2024-05-08 14:12:58.000000 kuksa_client-0.4.3a1/kuksa_client/cli_backend/grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)    12763 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/cli_backend/ws.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client/grpc/
--rw-r--r--   0 erik      (1000) erik      (1000)    42873 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/grpc/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    17846 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa_client/grpc/aio.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client/kuksa_logger/
--rw-r--r--   0 erik      (1000) erik      (1000)     4583 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/kuksa_logger/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      626 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa_client/logo
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client/ws/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa_client/ws/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     4180 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      931 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       60 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      162 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       25 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      661 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)     1221 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1768 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2545 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/conftest.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4157 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/test_basevssclient.py
--rw-r--r--   0 erik      (1000) erik      (1000)     7647 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/test_datapoint.py
--rw-r--r--   0 erik      (1000) erik      (1000)    67181 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/test_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/
+-rw-r--r--   0 erik      (1000) erik      (1000)    11357 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)       35 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)     4180 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     2941 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.000001 kuksa_client-0.4.3a2/kuksa/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/kuksa/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.000001 kuksa_client-0.4.3a2/kuksa/val/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/kuksa/val/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.004001 kuksa_client-0.4.3a2/kuksa/val/v1/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/kuksa/val/v1/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    10052 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa/val/v1/types_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    13964 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa/val/v1/types_pb2.pyi
+-rw-r--r--   0 erik      (1000) erik      (1000)     1135 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa/val/v1/types_pb2_grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4117 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa/val/v1/val_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4416 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa/val/v1/val_pb2.pyi
+-rw-r--r--   0 erik      (1000) erik      (1000)    10435 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa/val/v1/val_pb2_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.004001 kuksa_client-0.4.3a2/kuksa_client/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4630 2024-04-29 12:30:35.000000 kuksa_client-0.4.3a2/kuksa_client/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    26066 2024-05-10 12:00:35.000000 kuksa_client-0.4.3a2/kuksa_client/__main__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1761 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a2/kuksa_client/_metadata.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/kuksa_client/cli_backend/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1973 2024-05-10 12:00:45.000000 kuksa_client-0.4.3a2/kuksa_client/cli_backend/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    12028 2024-05-10 12:01:43.000000 kuksa_client-0.4.3a2/kuksa_client/cli_backend/grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    12661 2024-05-10 12:04:41.000000 kuksa_client-0.4.3a2/kuksa_client/cli_backend/ws.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/kuksa_client/grpc/
+-rw-r--r--   0 erik      (1000) erik      (1000)    42058 2024-05-10 12:02:29.000000 kuksa_client-0.4.3a2/kuksa_client/grpc/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    17846 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/kuksa_client/grpc/aio.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/kuksa_client/kuksa_logger/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4583 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a2/kuksa_client/kuksa_logger/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      626 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/kuksa_client/logo
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/kuksa_client/ws/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/kuksa_client/ws/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/kuksa_client.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4180 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa_client.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      931 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       60 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa_client.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      162 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa_client.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       25 2024-05-14 08:41:25.000000 kuksa_client-0.4.3a2/kuksa_client.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      661 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a2/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)     1221 2024-05-14 08:41:26.012001 kuksa_client-0.4.3a2/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1768 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-14 08:41:26.008001 kuksa_client-0.4.3a2/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/tests/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2546 2024-05-10 12:09:39.000000 kuksa_client-0.4.3a2/tests/conftest.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4157 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/tests/test_basevssclient.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     7647 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a2/tests/test_datapoint.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    67021 2024-05-10 12:04:17.000000 kuksa_client-0.4.3a2/tests/test_grpc.py
```

### Comparing `kuksa_client-0.4.3a1/LICENSE` & `kuksa_client-0.4.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/PKG-INFO` & `kuksa_client-0.4.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.4.3a1
+Version: 0.4.3a2
 Summary: KUKSA Python Client and SDK
 Home-page: https://github.com/eclipse-kuksa/kuksa-python-sdk
 Author: Eclipse KUKSA Project
 Author-email: kuksa-dev@eclipse.org
 Project-URL: Source, https://github.com/eclipse-kuksa/kuksa-python-sdk
 Project-URL: Bug Tracker, https://github.com/eclipse-kuksa/kuksa-python-sdk/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `kuksa_client-0.4.3a1/README.md` & `kuksa_client-0.4.3a2/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/__init__.py` & `kuksa_client-0.4.3a2/kuksa/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/__init__.py` & `kuksa_client-0.4.3a2/kuksa/val/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/v1/__init__.py` & `kuksa_client-0.4.3a2/kuksa/val/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2.py` & `kuksa_client-0.4.3a2/kuksa/val/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2.pyi` & `kuksa_client-0.4.3a2/kuksa/val/v1/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2_grpc.py` & `kuksa_client-0.4.3a2/kuksa/val/v1/types_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2.py` & `kuksa_client-0.4.3a2/kuksa/val/v1/val_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2.pyi` & `kuksa_client-0.4.3a2/kuksa/val/v1/val_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2_grpc.py` & `kuksa_client-0.4.3a2/kuksa/val/v1/val_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa_client/__init__.py` & `kuksa_client-0.4.3a2/kuksa_client/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa_client/__main__.py` & `kuksa_client-0.4.3a2/kuksa_client/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,14 @@
 from kuksa_client import _metadata
 from kuksa_client.kuksa_logger import KuksaLogger
 
 scriptDir = os.path.dirname(os.path.realpath(__file__))
 
 DEFAULT_KUKSA_ADDRESS = os.environ.get("KUKSA_ADDRESS", "grpc://127.0.0.1:55555")
 DEFAULT_TOKEN_OR_TOKENFILE = os.environ.get("TOKEN_OR_TOKENFILE", None)
-DEFAULT_CERTIFICATE = os.environ.get("CERTIFICATE", None)
-DEFAULT_KEYFILE = os.environ.get("KEYFILE", None)
 DEFAULT_CACERTIFICATE = os.environ.get("CACERTIFICATE", None)
 DEFAULT_TLS_SERVER_NAME = os.environ.get("TLS_SERVER_NAME", None)
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -313,16 +311,14 @@
     )
 
     # Constructor, request names after protocol to avoid errors
     def __init__(
         self,
         server=None,
         token_or_tokenfile=None,
-        certificate=None,
-        keyfile=None,
         cacertificate=None,
         tls_server_name=None,
     ):
         shortcuts = constants.DEFAULT_SHORTCUTS
         shortcuts.update({"exit": "quit"})
         super().__init__(
             persistent_history_file=".vssclient_history",
@@ -336,16 +332,14 @@
         self.server = server or DEFAULT_KUKSA_ADDRESS
 
         self.metadata = {}
         self.pathCompletionItems = []
         self.subscribeIds = set()
         self.commThread = None
         self.token_or_tokenfile = token_or_tokenfile
-        self.certificate = certificate
-        self.keyfile = keyfile
         self.cacertificate = cacertificate
         self.tls_server_name = tls_server_name
 
         with (pathlib.Path(scriptDir) / "logo").open("r", encoding="utf-8") as f:
             logo = f.read()
             print(logo.replace("%ver%", str(_metadata.__version__)))
 
@@ -608,18 +602,14 @@
 using {'KUKSA GRPC' if config['protocol'] == 'grpc' else 'VISS' } protocol."
         )
         print(f"TLS will {'not be' if config['insecure'] else 'be'} used.")
 
         # Configs should only be added if they actually have a value
         if self.token_or_tokenfile is not None:
             config["token_or_tokenfile"] = self.token_or_tokenfile
-        if self.certificate is not None:
-            config["certificate"] = self.certificate
-        if self.keyfile is not None:
-            config["keyfile"] = self.keyfile
         if self.cacertificate is not None:
             config["cacertificate"] = self.cacertificate
         if self.tls_server_name is not None:
             config["tls_server_name"] = self.tls_server_name
 
         self.commThread = KuksaClientThread(config)
         self.commThread.start()
@@ -680,25 +670,14 @@
     parser.add_argument(
         "--token_or_tokenfile",
         default=DEFAULT_TOKEN_OR_TOKENFILE,
         help="JWT token or path to a JWT token file (.token)",
     )
 
     # Add TLS arguments
-    # Note: Databroker does not yet support mutual authentication, so no need to use two first arguments
-    parser.add_argument(
-        "--certificate",
-        default=DEFAULT_CERTIFICATE,
-        help="Client cert file(.pem), only needed for mutual authentication",
-    )
-    parser.add_argument(
-        "--keyfile",
-        default=DEFAULT_KEYFILE,
-        help="Client private key file (.key), only needed for mutual authentication",
-    )
     parser.add_argument(
         "--cacertificate",
         default=DEFAULT_CACERTIFICATE,
         help="Client root cert file (.pem). \
         Needed for TLS enabled transports (grpcs, wss)",
     )
     # Observations for Python
@@ -712,16 +691,14 @@
     )
 
     args = parser.parse_args()
 
     clientApp = TestClient(
         args.server,
         token_or_tokenfile=args.token_or_tokenfile,
-        certificate=args.certificate,
-        keyfile=args.keyfile,
         cacertificate=args.cacertificate,
         tls_server_name=args.tls_server_name,
     )
     try:
         # We exit the loop when the user types "quit" or hits Ctrl-D.
         clientApp.cmdloop()
     finally:
```

### Comparing `kuksa_client-0.4.3a1/kuksa_client/_metadata.py` & `kuksa_client-0.4.3a2/kuksa_client/_metadata.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa_client/cli_backend/__init__.py` & `kuksa_client-0.4.3a2/kuksa_client/cli_backend/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,14 @@
             self.insecure = config.getboolean('insecure', False)
         except AttributeError:
             self.insecure = config.get('insecure', False)
         self.cacertificate = config.get('cacertificate', None)
         # If no CA Certificate is given we will use an insecure connection, requested or not
         if self.cacertificate is None:
             self.insecure = True
-        self.certificate = config.get('certificate', None)
-        self.keyfile = config.get('keyfile', None)
         self.tls_server_name = config.get('tls_server_name', "")
         self.token_or_tokenfile = config.get('token_or_tokenfile', None)
 
     @staticmethod
     def from_config(config):
         protocol = config.get('protocol', 'ws')
```

### Comparing `kuksa_client-0.4.3a1/kuksa_client/cli_backend/grpc.py` & `kuksa_client-0.4.3a2/kuksa_client/cli_backend/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,14 @@
 
 
 class Backend(cli_backend.Backend):
     def __init__(self, config):
         super().__init__(config)
         if self.cacertificate is not None:
             self.cacertificate = pathlib.Path(self.cacertificate)
-        if self.keyfile is not None:
-            self.keyfile = pathlib.Path(self.keyfile)
-        if self.certificate is not None:
-            self.certificate = pathlib.Path(self.certificate)
         if self.token_or_tokenfile is not None:
             if os.path.isfile(self.token_or_tokenfile):
                 self.token_or_tokenfile = pathlib.Path(self.token_or_tokenfile)
                 self.token = self.token_or_tokenfile.expanduser(
                 ).read_text(encoding='utf-8').rstrip('\n')
             else:
                 self.token = str(self.token_or_tokenfile)
@@ -281,14 +277,12 @@
                 logger.info("gRPC channel connected.")
                 await self._grpcHandler(vss_client)
         else:
             async with kuksa_client.grpc.aio.VSSClient(
                 self.serverIP,
                 self.serverPort,
                 root_certificates=self.cacertificate,
-                private_key=self.keyfile,
-                certificate_chain=self.certificate,
                 tls_server_name=self.tls_server_name,
                 token=self.token
             ) as vss_client:
                 logger.info("Secure gRPC channel connected.")
                 await self._grpcHandler(vss_client)
```

### Comparing `kuksa_client-0.4.3a1/kuksa_client/cli_backend/ws.py` & `kuksa_client-0.4.3a2/kuksa_client/cli_backend/ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,16 +293,14 @@
         """
         return self.ws_connection_established
 
     async def connect(self, _=None):
         subprotocols = ["VISSv2"]
         if not self.insecure:
             context = ssl.create_default_context()
-            context.load_cert_chain(
-                certfile=self.certificate, keyfile=self.keyfile)
             context.load_verify_locations(cafile=self.cacertificate)
             # We want host name to match
             # For example certificates we use subjectAltName to make it match for Server, localahost and 127.0.0.1
             # If using your own certificates make sure that name is included or use tls_server_name work-around
             context.check_hostname = True
             try:
                 logger.info("connect to wss://"+self.serverIP+":"+str(self.serverPort))
```

### Comparing `kuksa_client-0.4.3a1/kuksa_client/grpc/__init__.py` & `kuksa_client-0.4.3a2/kuksa_client/grpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -555,44 +555,32 @@
 class BaseVSSClient:
     def __init__(
         self,
         host: str,
         port: int,
         token: Optional[str] = None,
         root_certificates: Optional[Path] = None,
-        private_key: Optional[Path] = None,
-        certificate_chain: Optional[Path] = None,
         ensure_startup_connection: bool = True,
         connected: bool = False,
         tls_server_name: Optional[str] = None
     ):
 
         self.authorization_header = self.get_authorization_header(token)
         self.target_host = f'{host}:{port}'
         self.root_certificates = root_certificates
-        self.private_key = private_key
-        self.certificate_chain = certificate_chain
         self.tls_server_name = tls_server_name
         self.ensure_startup_connection = ensure_startup_connection
         self.connected = connected
         self.client_stub = None
 
     def _load_creds(self) -> Optional[grpc.ChannelCredentials]:
         if self.root_certificates:
             logger.info(f"Using TLS with Root CA from {self.root_certificates}")
             root_certificates = self.root_certificates.read_bytes()
-            if self.private_key and self.certificate_chain:
-                private_key = self.private_key.read_bytes()
-                certificate_chain = self.certificate_chain.read_bytes()
-                # As of today there is no option in KUKSA.val Databroker to require client authentication
-                logger.info("Using client private key and certificates, mutual TLS supported if supported by server")
-                return grpc.ssl_channel_credentials(root_certificates, private_key, certificate_chain)
-            else:
-                logger.info("No client certificates provided, mutual TLS not supported!")
-                return grpc.ssl_channel_credentials(root_certificates)
+            return grpc.ssl_channel_credentials(root_certificates)
         logger.info("No Root CA present, it will not be possible to use a secure connection!")
         return None
 
     def _prepare_get_request(self, entries: Iterable[EntryRequest]) -> val_pb2.GetRequest:
         req = val_pb2.GetRequest(entries=[])
         for entry in entries:
             entry_request = val_pb2.EntryRequest(
```

### Comparing `kuksa_client-0.4.3a1/kuksa_client/grpc/aio.py` & `kuksa_client-0.4.3a2/kuksa_client/grpc/aio.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa_client/kuksa_logger/__init__.py` & `kuksa_client-0.4.3a2/kuksa_client/kuksa_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa_client/logo` & `kuksa_client-0.4.3a2/kuksa_client/logo`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa_client/ws/__init__.py` & `kuksa_client-0.4.3a2/kuksa_client/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/kuksa_client.egg-info/PKG-INFO` & `kuksa_client-0.4.3a2/kuksa_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.4.3a1
+Version: 0.4.3a2
 Summary: KUKSA Python Client and SDK
 Home-page: https://github.com/eclipse-kuksa/kuksa-python-sdk
 Author: Eclipse KUKSA Project
 Author-email: kuksa-dev@eclipse.org
 Project-URL: Source, https://github.com/eclipse-kuksa/kuksa-python-sdk
 Project-URL: Bug Tracker, https://github.com/eclipse-kuksa/kuksa-python-sdk/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `kuksa_client-0.4.3a1/kuksa_client.egg-info/SOURCES.txt` & `kuksa_client-0.4.3a2/kuksa_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/pyproject.toml` & `kuksa_client-0.4.3a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/setup.cfg` & `kuksa_client-0.4.3a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/setup.py` & `kuksa_client-0.4.3a2/setup.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/tests/__init__.py` & `kuksa_client-0.4.3a2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/tests/conftest.py` & `kuksa_client-0.4.3a2/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,14 @@
     val_pb2_grpc.add_VALServicer_to_server(val_servicer, server)
     server.add_secure_port(f'localhost:{unused_tcp_port}', grpc.ssl_server_credentials(
         private_key_certificate_chain_pairs=[(
             (resources_path / 'test-server.key').read_bytes(),
             (resources_path / 'test-server.pem').read_bytes(),
         )],
         root_certificates=(resources_path / 'test-ca.pem').read_bytes(),
-        require_client_auth=True,
+        require_client_auth=False,
     ))
     await server.start()
     try:
         yield server
     finally:
         await server.stop(grace=2.0)
```

### Comparing `kuksa_client-0.4.3a1/tests/test_basevssclient.py` & `kuksa_client-0.4.3a2/tests/test_basevssclient.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/tests/test_datapoint.py` & `kuksa_client-0.4.3a2/tests/test_datapoint.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.3a1/tests/test_grpc.py` & `kuksa_client-0.4.3a2/tests/test_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,16 +402,14 @@
 class TestVSSClient:
     @pytest.mark.usefixtures('secure_val_server')
     async def test_secure_connection(self, unused_tcp_port, resources_path, val_servicer):
         val_servicer.GetServerInfo.return_value = val_pb2.GetServerInfoResponse(
             name='test_server', version='1.2.3')
         async with VSSClient('localhost', unused_tcp_port,
                              root_certificates=resources_path / 'test-ca.pem',
-                             private_key=resources_path / 'test-client.key',
-                             certificate_chain=resources_path / 'test-client.pem',
                              ensure_startup_connection=True
                              ):
             assert val_servicer.GetServerInfo.call_count == 1
 
     async def test_get_current_values(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
         client.connected = True  # To bypass connection test
```

