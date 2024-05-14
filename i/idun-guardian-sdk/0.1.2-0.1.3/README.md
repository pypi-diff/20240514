# Comparing `tmp/idun_guardian_sdk-0.1.2.tar.gz` & `tmp/idun_guardian_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_sdk-0.1.2.tar", max compression
+gzip compressed data, was "idun_guardian_sdk-0.1.3.tar", max compression
```

## Comparing `idun_guardian_sdk-0.1.2.tar` & `idun_guardian_sdk-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,18 @@
--rw-r--r--   0        0        0       38 2024-02-12 13:03:08.116868 idun_guardian_sdk-0.1.2/idun_guardian_sdk/__init__.py
--rw-r--r--   0        0        0    10813 2024-02-20 10:22:14.612116 idun_guardian_sdk-0.1.2/idun_guardian_sdk/api.py
--rw-r--r--   0        0        0     9285 2024-02-14 17:33:55.028675 idun_guardian_sdk-0.1.2/idun_guardian_sdk/ble.py
--rw-r--r--   0        0        0      666 2024-02-20 10:22:21.984390 idun_guardian_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      100 2024-02-12 13:03:08.102671 idun_guardian_sdk-0.1.2/README.md
--rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 idun_guardian_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-05-14 11:39:35.656492 idun_guardian_sdk-0.1.3/idun_guardian_sdk/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-07 14:27:29.482099 idun_guardian_sdk-0.1.3/idun_guardian_sdk/constants.py
+-rw-r--r--   0        0        0    12324 2024-05-14 11:39:35.657490 idun_guardian_sdk-0.1.3/idun_guardian_sdk/debug_logs.py
+-rw-r--r--   0        0        0       54 2024-05-07 14:27:29.482099 idun_guardian_sdk-0.1.3/idun_guardian_sdk/event.py
+-rw-r--r--   0        0        0      605 2024-05-07 14:27:29.483095 idun_guardian_sdk-0.1.3/idun_guardian_sdk/event_handlers.py
+-rw-r--r--   0        0        0      428 2024-05-07 14:27:29.483095 idun_guardian_sdk-0.1.3/idun_guardian_sdk/exceptions.py
+-rw-r--r--   0        0        0    30788 2024-05-14 11:39:35.658487 idun_guardian_sdk-0.1.3/idun_guardian_sdk/guardian_ble.py
+-rw-r--r--   0        0        0    13399 2024-05-14 11:39:35.658487 idun_guardian_sdk-0.1.3/idun_guardian_sdk/guardian_client.py
+-rw-r--r--   0        0        0     8797 2024-05-14 11:39:35.659484 idun_guardian_sdk-0.1.3/idun_guardian_sdk/guardian_http_api.py
+-rw-r--r--   0        0        0    14999 2024-05-14 11:39:35.660481 idun_guardian_sdk-0.1.3/idun_guardian_sdk/guardian_recording.py
+-rw-r--r--   0        0        0      430 2024-05-07 14:27:29.485090 idun_guardian_sdk-0.1.3/idun_guardian_sdk/polling_service.py
+-rw-r--r--   0        0        0      117 2024-05-07 14:27:29.485090 idun_guardian_sdk-0.1.3/idun_guardian_sdk/types.py
+-rw-r--r--   0        0        0     1963 2024-05-14 11:39:35.660481 idun_guardian_sdk-0.1.3/idun_guardian_sdk/utils.py
+-rw-r--r--   0        0        0     4714 2024-05-07 14:27:29.486087 idun_guardian_sdk-0.1.3/idun_guardian_sdk/websocket_messages.py
+-rw-r--r--   0        0        0      665 2024-05-07 14:27:29.486087 idun_guardian_sdk-0.1.3/idun_guardian_sdk/ws_msg_handler.py
+-rw-r--r--   0        0        0      687 2024-05-14 11:41:35.221309 idun_guardian_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8625 2024-05-07 14:27:29.477112 idun_guardian_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0     9151 1970-01-01 00:00:00.000000 idun_guardian_sdk-0.1.3/PKG-INFO
```

### Comparing `idun_guardian_sdk-0.1.2/pyproject.toml` & `idun_guardian_sdk-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "idun-guardian-sdk"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["IDUN Technologies AG <support@iduntechnologies.com>"]
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "idun_guardian_sdk"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-simplepyble = "^0.6.1"
+python = ">=3.9,<3.13"
 requests = "^2.31.0"
 urllib3 = "<2.0"
-websocket-client = "^1.7.0"
 python-dotenv = "^1.0.1"
 certifi = "^2024.2.2"
+pycryptodome = "^3.20.0"
+bleak = "^0.21.1"
+websockets = "^12.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.1.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
```

