# Comparing `tmp/aioairq-0.3.2.tar.gz` & `tmp/aioairq-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairq-0.3.2.tar", last modified: Sat Dec 23 20:41:08 2023, max compression
+gzip compressed data, was "aioairq-0.4.2.tar", last modified: Tue May 14 17:09:56 2024, max compression
```

## Comparing `aioairq-0.3.2.tar` & `aioairq-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2023-12-23 20:41:08.602202 aioairq-0.3.2/
--rw-r--r--   0 renat     (1000) renat     (1001)    10173 2023-11-28 18:02:04.000000 aioairq-0.3.2/LICENSE
--rw-r--r--   0 renat     (1000) renat     (1001)     1841 2023-12-23 20:41:08.602202 aioairq-0.3.2/PKG-INFO
--rw-r--r--   0 renat     (1000) renat     (1001)      848 2023-11-28 18:02:04.000000 aioairq-0.3.2/README.md
-drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2023-12-23 20:41:08.598868 aioairq-0.3.2/aioairq/
--rw-r--r--   0 renat     (1000) renat     (1001)      387 2023-12-23 20:33:05.000000 aioairq-0.3.2/aioairq/__init__.py
--rw-r--r--   0 renat     (1000) renat     (1001)     5602 2023-12-23 20:33:05.000000 aioairq-0.3.2/aioairq/core.py
--rw-r--r--   0 renat     (1000) renat     (1001)     1837 2023-11-28 18:02:04.000000 aioairq-0.3.2/aioairq/encrypt.py
--rw-r--r--   0 renat     (1000) renat     (1001)      201 2023-12-23 20:33:05.000000 aioairq-0.3.2/aioairq/exceptions.py
-drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2023-12-23 20:41:08.598868 aioairq-0.3.2/aioairq.egg-info/
--rw-r--r--   0 renat     (1000) renat     (1001)     1841 2023-12-23 20:41:08.000000 aioairq-0.3.2/aioairq.egg-info/PKG-INFO
--rw-r--r--   0 renat     (1000) renat     (1001)      312 2023-12-23 20:41:08.000000 aioairq-0.3.2/aioairq.egg-info/SOURCES.txt
--rw-r--r--   0 renat     (1000) renat     (1001)        1 2023-12-23 20:41:08.000000 aioairq-0.3.2/aioairq.egg-info/dependency_links.txt
--rw-r--r--   0 renat     (1000) renat     (1001)       52 2023-12-23 20:41:08.000000 aioairq-0.3.2/aioairq.egg-info/requires.txt
--rw-r--r--   0 renat     (1000) renat     (1001)        8 2023-12-23 20:41:08.000000 aioairq-0.3.2/aioairq.egg-info/top_level.txt
--rw-r--r--   0 renat     (1000) renat     (1001)     1101 2023-11-28 18:02:04.000000 aioairq-0.3.2/pyproject.toml
--rw-r--r--   0 renat     (1000) renat     (1001)       38 2023-12-23 20:41:08.602202 aioairq-0.3.2/setup.cfg
--rw-r--r--   0 renat     (1000) renat     (1001)      101 2023-11-28 18:02:04.000000 aioairq-0.3.2/setup.py
-drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2023-12-23 20:41:08.598868 aioairq-0.3.2/tests/
--rw-r--r--   0 renat     (1000) renat     (1001)      917 2023-12-23 20:33:05.000000 aioairq-0.3.2/tests/test_access.py
--rw-r--r--   0 renat     (1000) renat     (1001)      719 2023-12-23 20:39:55.000000 aioairq-0.3.2/tests/test_core.py
+drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2024-05-14 17:09:56.298769 aioairq-0.4.2/
+-rw-r--r--   0 renat     (1000) renat     (1001)    10173 2023-11-28 18:02:04.000000 aioairq-0.4.2/LICENSE
+-rw-r--r--   0 renat     (1000) renat     (1001)     4390 2024-05-14 17:09:56.298769 aioairq-0.4.2/PKG-INFO
+-rw-r--r--   0 renat     (1000) renat     (1001)     3223 2024-05-07 17:39:35.000000 aioairq-0.4.2/README.md
+drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2024-05-14 17:09:56.298769 aioairq-0.4.2/aioairq/
+-rw-r--r--   0 renat     (1000) renat     (1001)      588 2024-05-14 16:54:45.000000 aioairq-0.4.2/aioairq/__init__.py
+-rw-r--r--   0 renat     (1000) renat     (1001)    16974 2024-05-14 16:54:45.000000 aioairq-0.4.2/aioairq/core.py
+-rw-r--r--   0 renat     (1000) renat     (1001)     2368 2024-05-07 17:39:35.000000 aioairq-0.4.2/aioairq/encrypt.py
+-rw-r--r--   0 renat     (1000) renat     (1001)      535 2024-05-14 16:54:45.000000 aioairq-0.4.2/aioairq/exceptions.py
+-rw-r--r--   0 renat     (1000) renat     (1001)      251 2024-05-07 17:39:35.000000 aioairq-0.4.2/aioairq/utils.py
+drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2024-05-14 17:09:56.298769 aioairq-0.4.2/aioairq.egg-info/
+-rw-r--r--   0 renat     (1000) renat     (1001)     4390 2024-05-14 17:09:56.000000 aioairq-0.4.2/aioairq.egg-info/PKG-INFO
+-rw-r--r--   0 renat     (1000) renat     (1001)      375 2024-05-14 17:09:56.000000 aioairq-0.4.2/aioairq.egg-info/SOURCES.txt
+-rw-r--r--   0 renat     (1000) renat     (1001)        1 2024-05-14 17:09:56.000000 aioairq-0.4.2/aioairq.egg-info/dependency_links.txt
+-rw-r--r--   0 renat     (1000) renat     (1001)       66 2024-05-14 17:09:56.000000 aioairq-0.4.2/aioairq.egg-info/requires.txt
+-rw-r--r--   0 renat     (1000) renat     (1001)        8 2024-05-14 17:09:56.000000 aioairq-0.4.2/aioairq.egg-info/top_level.txt
+-rw-r--r--   0 renat     (1000) renat     (1001)     1209 2024-05-07 17:39:35.000000 aioairq-0.4.2/pyproject.toml
+-rw-r--r--   0 renat     (1000) renat     (1001)       38 2024-05-14 17:09:56.298769 aioairq-0.4.2/setup.cfg
+-rw-r--r--   0 renat     (1000) renat     (1001)      101 2023-11-28 18:02:04.000000 aioairq-0.4.2/setup.py
+drwxr-xr-x   0 renat     (1000) renat     (1001)        0 2024-05-14 17:09:56.298769 aioairq-0.4.2/tests/
+-rw-r--r--   0 renat     (1000) renat     (1001)      613 2024-05-07 17:39:35.000000 aioairq-0.4.2/tests/test_aes.py
+-rw-r--r--   0 renat     (1000) renat     (1001)      719 2024-02-28 14:25:46.000000 aioairq-0.4.2/tests/test_core.py
+-rw-r--r--   0 renat     (1000) renat     (1001)     7252 2024-05-14 16:54:45.000000 aioairq-0.4.2/tests/test_core_on_device.py
+-rw-r--r--   0 renat     (1000) renat     (1001)      815 2024-05-07 17:39:35.000000 aioairq-0.4.2/tests/test_utils.py
```

### Comparing `aioairq-0.3.2/LICENSE` & `aioairq-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairq-0.3.2/aioairq/encrypt.py` & `aioairq-0.4.2/aioairq/encrypt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 """Module concerned with encryption of the data"""
 import base64
 
 from Crypto.Cipher import AES
+from Crypto import Random
 
 from aioairq.exceptions import InvalidAuth
 
 
 class AESCipher:
     _bs = AES.block_size  # 16
 
     def __init__(self, passw: str):
         """Class responsible for decryption of AirQ responses
 
-        Main idea of the class is to expose a convenience method
-        ``decode`` while the decryption key is stored as an attribute,
+        Main idea of the class is to expose convenience methods
+        ``encode`` and ``decode`` while the key is stored as a private attribute,
         conveniently computed from the password upon initialisation
         of the class' instance
 
         Parameters
         ----------
         passw : str
             Device's password
         """
-        self.key = self._pass2aes(passw)
+        self._key = self._pass2aes(passw)
 
-    def decode(self, encrypted: bytes) -> str:
+    def encode(self, data: str) -> str:
+        iv = Random.new().read(AES.block_size)
+        cipher = AES.new(self._key, AES.MODE_CBC, iv)
+
+        encoded = data.encode("utf-8")
+        encrypted = iv + cipher.encrypt(self._pad(encoded))
+
+        return base64.b64encode(encrypted).decode("utf-8")
+
+    def decode(self, encrypted: str) -> str:
         decoded = base64.b64decode(encrypted)
         iv = decoded[: self._bs]
-        cipher = AES.new(self.key, AES.MODE_CBC, iv)
+        cipher = AES.new(self._key, AES.MODE_CBC, iv)
         decrypted = cipher.decrypt(decoded[self._bs :])
         try:
             # Currently the device does not support proper authentication.
             # The success or failure of the authentication based on the ability
             # to decode the response from the device.
             decoded = decrypted.decode("utf-8")
         except UnicodeDecodeError:
-            raise InvalidAuth("Failed to decode a message. Incorrect password")
+            raise InvalidAuth(
+                "Failed to decode a message. Incorrect password"
+            ) from None
         return self._unpad(decoded)
 
     @staticmethod
+    def _pad(data: bytes) -> bytes:
+        length = 16 - (len(data) % 16)
+        return data + bytes(chr(length) * length, "utf-8")
+
+    @staticmethod
     def _unpad(data: str) -> str:
         return data[: -ord(data[-1])]
 
     @staticmethod
     def _pass2aes(passw: str) -> str:
         """Derive the key for AES256 from the device password
```

### Comparing `aioairq-0.3.2/pyproject.toml` & `aioairq-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 [project.optional-dependencies]
-tests = ["pytest", "pytest-asyncio"]
+dev = ["ruff", "pre-commit", "pytest", "pytest-asyncio"]
 
 
 [tool.setuptools.dynamic]
 version = { attr = "aioairq.__version__" }
 
 [project.urls]
 "Homepage" = "https://github.com/CorantGmbH/aioairq"
```

### Comparing `aioairq-0.3.2/tests/test_core.py` & `aioairq-0.4.2/tests/test_core.py`

 * *Files identical despite different names*

