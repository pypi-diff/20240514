# Comparing `tmp/evervault-4.2.0.tar.gz` & `tmp/evervault-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evervault-4.2.0.tar", max compression
+gzip compressed data, was "evervault-4.3.0.tar", max compression
```

## Comparing `evervault-4.2.0.tar` & `evervault-4.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1109 2024-03-12 18:32:47.238152 evervault-4.2.0/LICENSE
--rw-r--r--   0        0        0      642 2024-03-12 18:32:47.238152 evervault-4.2.0/README.md
--rw-r--r--   0        0        0     5175 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/__init__.py
--rw-r--r--   0        0        0     3472 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/cages_v2.py
--rw-r--r--   0        0        0     5020 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/client.py
--rw-r--r--   0        0        0       55 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/crypto/__init__.py
--rw-r--r--   0        0        0    11722 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/crypto/client.py
--rw-r--r--   0        0        0       58 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/crypto/curves/__init__.py
--rw-r--r--   0        0        0     3486 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/crypto/curves/base.py
--rw-r--r--   0        0        0      744 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/crypto/curves/koblitz.py
--rw-r--r--   0        0        0      779 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/crypto/curves/p256.py
--rw-r--r--   0        0        0      136 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/crypto/version.py
--rw-r--r--   0        0        0      115 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/datatypes/__init__.py
--rw-r--r--   0        0        0      223 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/datatypes/map.py
--rw-r--r--   0        0        0     3492 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/enclaves.py
--rw-r--r--   0        0        0       43 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/errors/__init__.py
--rw-r--r--   0        0        0     2939 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/errors/error_handler.py
--rw-r--r--   0        0        0      563 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/errors/evervault_errors.py
--rw-r--r--   0        0        0       37 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/http/__init__.py
--rw-r--r--   0        0        0     2061 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/http/attestationdoc.py
--rw-r--r--   0        0        0     2260 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/http/outboundrelayconfig.py
--rw-r--r--   0        0        0     3950 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/http/pcrManager.py
--rw-r--r--   0        0        0     4315 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/http/request.py
--rw-r--r--   0        0        0     1207 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/http/requesthandler.py
--rw-r--r--   0        0        0     7820 2024-03-12 18:32:47.238152 evervault-4.2.0/evervault/http/requestintercept.py
--rw-r--r--   0        0        0       73 2024-03-12 18:32:47.242152 evervault-4.2.0/evervault/models/__init__.py
--rw-r--r--   0        0        0      217 2024-03-12 18:32:47.242152 evervault-4.2.0/evervault/models/cage.py
--rw-r--r--   0        0        0        0 2024-03-12 18:32:47.242152 evervault-4.2.0/evervault/services/__init__.py
--rw-r--r--   0        0        0      136 2024-03-12 18:32:47.242152 evervault-4.2.0/evervault/services/timeservice.py
--rw-r--r--   0        0        0     1143 2024-03-12 18:32:47.242152 evervault-4.2.0/evervault/threading/repeatedtimer.py
--rw-r--r--   0        0        0      901 2024-03-12 18:32:47.242152 evervault-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 evervault-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-04-19 16:34:19.093217 evervault-4.3.0/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-19 16:34:19.093217 evervault-4.3.0/README.md
+-rw-r--r--   0        0        0     5271 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/__init__.py
+-rw-r--r--   0        0        0     3472 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/cages_v2.py
+-rw-r--r--   0        0        0     5020 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/client.py
+-rw-r--r--   0        0        0       55 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/crypto/__init__.py
+-rw-r--r--   0        0        0    11724 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/crypto/client.py
+-rw-r--r--   0        0        0       58 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/crypto/curves/__init__.py
+-rw-r--r--   0        0        0     3486 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/crypto/curves/base.py
+-rw-r--r--   0        0        0      744 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/crypto/curves/koblitz.py
+-rw-r--r--   0        0        0      779 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/crypto/curves/p256.py
+-rw-r--r--   0        0        0      136 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/crypto/version.py
+-rw-r--r--   0        0        0      115 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/datatypes/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/datatypes/map.py
+-rw-r--r--   0        0        0     3492 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/enclaves.py
+-rw-r--r--   0        0        0       43 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/errors/__init__.py
+-rw-r--r--   0        0        0     2939 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/errors/error_handler.py
+-rw-r--r--   0        0        0      563 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/errors/evervault_errors.py
+-rw-r--r--   0        0        0       37 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/http/__init__.py
+-rw-r--r--   0        0        0     2061 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/http/attestationdoc.py
+-rw-r--r--   0        0        0     2260 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/http/outboundrelayconfig.py
+-rw-r--r--   0        0        0     3950 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/http/pcrManager.py
+-rw-r--r--   0        0        0     4315 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/http/request.py
+-rw-r--r--   0        0        0     1207 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/http/requesthandler.py
+-rw-r--r--   0        0        0     7820 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/http/requestintercept.py
+-rw-r--r--   0        0        0       73 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/models/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/models/cage.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/services/__init__.py
+-rw-r--r--   0        0        0      136 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/services/timeservice.py
+-rw-r--r--   0        0        0     1143 2024-04-19 16:34:19.097217 evervault-4.3.0/evervault/threading/repeatedtimer.py
+-rw-r--r--   0        0        0      901 2024-04-19 16:34:19.097217 evervault-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 evervault-4.3.0/PKG-INFO
```

### Comparing `evervault-4.2.0/LICENSE` & `evervault-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/README.md` & `evervault-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/__init__.py` & `evervault-4.3.0/evervault/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Package for the evervault SDK"""
+
 from evervault.enclaves import EnclaveRequestsSession
 from .client import Client
 from .errors.evervault_errors import EvervaultError
 from .cages_v2 import CageRequestsSession
 import os
 import sys
 from warnings import warn
@@ -12,15 +13,15 @@
 from importlib import metadata
 
 __version__ = metadata.version(__package__ or __name__)
 
 ev_client = None
 _app_uuid = None
 _api_key = None
-request_timeout = 30
+_request_timeout = None
 _retry = False
 _curve = None
 
 BASE_URL_DEFAULT = "https://api.evervault.com/"
 RELAY_URL_DEFAULT = "https://relay.evervault.com:443"
 CA_HOST_DEFAULT = "https://ca.evervault.com"
 CAGES_HOST_DEFAULT = "cage.evervault.com"
@@ -40,24 +41,27 @@
     app_id,
     api_key,
     decryption_domains=[],
     retry=False,
     curve=Curves.SECP256K1,
     debug_requests=False,
     enable_outbound_relay=False,
+    request_timeout=30,
 ):
     global _app_uuid
     global _api_key
     global _retry
     global _curve
+    global _request_timeout
 
     _app_uuid = app_id
     _api_key = api_key
     _retry = retry
     _curve = curve
+    _request_timeout = request_timeout
 
     if len(decryption_domains) > 0:
         __client().enable_outbound_relay(
             debug_requests, decryption_domains=decryption_domains
         )
     elif enable_outbound_relay:
         __client().enable_outbound_relay(
@@ -154,15 +158,15 @@
     if not ev_client:
         max_file_size_in_mb = int(
             os.environ.get("EV_MAX_FILE_SIZE_IN_MB", MAX_FILE_SIZE_IN_MB_DEFAULT)
         )
         ev_client = Client(
             api_key=_api_key,
             app_uuid=_app_uuid,
-            request_timeout=request_timeout,
+            request_timeout=_request_timeout,
             base_url=os.environ.get("EV_API_URL", BASE_URL_DEFAULT),
             relay_url=os.environ.get("EV_TUNNEL_HOSTNAME", RELAY_URL_DEFAULT),
             ca_host=os.environ.get("EV_CERT_HOSTNAME", CA_HOST_DEFAULT),
             retry=_retry,
             curve=_curve,
             max_file_size_in_mb=max_file_size_in_mb,
         )
```

### Comparing `evervault-4.2.0/evervault/cages_v2.py` & `evervault-4.3.0/evervault/cages_v2.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/client.py` & `evervault-4.3.0/evervault/client.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/crypto/client.py` & `evervault-4.3.0/evervault/crypto/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             time_diff = now - self.start_time
             if time_diff > KEY_INTERVAL:
                 self.start_time = now
                 return self.__generate_shared_key(has_role)
             return self.shared_key
 
     def __generate_shared_key(self, has_role):
-        generated_key = ec.generate_private_key(CURVES[self.curve])
+        generated_key = ec.generate_private_key(CURVES[self.curve]())
         public_key = generated_key.public_key()
         self.compressed_public_key = public_key.public_bytes(
             Encoding.X962, PublicFormat.CompressedPoint
         )
         self.uncompressed_public_key = public_key.public_bytes(
             Encoding.X962, PublicFormat.UncompressedPoint
         )
```

### Comparing `evervault-4.2.0/evervault/crypto/curves/base.py` & `evervault-4.3.0/evervault/crypto/curves/base.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/crypto/curves/koblitz.py` & `evervault-4.3.0/evervault/crypto/curves/koblitz.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/crypto/curves/p256.py` & `evervault-4.3.0/evervault/crypto/curves/p256.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/enclaves.py` & `evervault-4.3.0/evervault/enclaves.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/errors/error_handler.py` & `evervault-4.3.0/evervault/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/errors/evervault_errors.py` & `evervault-4.3.0/evervault/errors/evervault_errors.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/http/attestationdoc.py` & `evervault-4.3.0/evervault/http/attestationdoc.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/http/outboundrelayconfig.py` & `evervault-4.3.0/evervault/http/outboundrelayconfig.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/http/pcrManager.py` & `evervault-4.3.0/evervault/http/pcrManager.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/http/request.py` & `evervault-4.3.0/evervault/http/request.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/http/requesthandler.py` & `evervault-4.3.0/evervault/http/requesthandler.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/http/requestintercept.py` & `evervault-4.3.0/evervault/http/requestintercept.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/evervault/threading/repeatedtimer.py` & `evervault-4.3.0/evervault/threading/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `evervault-4.2.0/pyproject.toml` & `evervault-4.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "evervault"
-version = "4.2.0"
+version = "4.3.0"
 description = "Evervault SDK"
 authors = ["Evervault <engineering@evervault.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://evervault.com"
 repository = "https://github.com/evervault/evervault-python"
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.0"
 requests = "^2.24.0"
 cryptography = "^42.0.0"
 certifi = "*"
 pycryptodome = "^3.10.1"
 pyasn1 = "^0.4.8"
 evervault-attestation-bindings = "0.3.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-socket = "^0.4.1"
 requests-mock = "^1.9.3"
 flake8 = "^5.0.4"
-black = "^22.3.0"
+black = "^24.3.0"
 parameterized = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 responses = "^0.23.3"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `evervault-4.2.0/PKG-INFO` & `evervault-4.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: evervault
-Version: 4.2.0
+Version: 4.3.0
 Summary: Evervault SDK
 Home-page: https://evervault.com
 License: MIT
 Author: Evervault
 Author-email: engineering@evervault.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi
 Requires-Dist: cryptography (>=42.0.0,<43.0.0)
 Requires-Dist: evervault-attestation-bindings (==0.3.3)
```

