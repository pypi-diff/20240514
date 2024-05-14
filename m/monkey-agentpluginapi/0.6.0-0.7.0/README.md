# Comparing `tmp/monkey_agentpluginapi-0.6.0.tar.gz` & `tmp/monkey_agentpluginapi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkey_agentpluginapi-0.6.0.tar", max compression
+gzip compressed data, was "monkey_agentpluginapi-0.7.0.tar", max compression
```

## Comparing `monkey_agentpluginapi-0.6.0.tar` & `monkey_agentpluginapi-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1019 2024-03-14 13:22:04.064038 monkey_agentpluginapi-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0    35255 2024-01-16 19:17:10.913816 monkey_agentpluginapi-0.6.0/LICENSE
--rw-r--r--   0        0        0      281 2024-01-16 19:51:25.073278 monkey_agentpluginapi-0.6.0/README.md
--rw-r--r--   0        0        0     1349 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.6.0/agentpluginapi/__init__.py
--rw-r--r--   0        0        0      593 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.6.0/agentpluginapi/agent_binary_request.py
--rw-r--r--   0        0        0      123 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.6.0/agentpluginapi/dropper_execution_mode.py
--rw-r--r--   0        0        0      264 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.6.0/agentpluginapi/exploiter_result.py
--rw-r--r--   0        0        0      278 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.6.0/agentpluginapi/fingerprint_data.py
--rw-r--r--   0        0        0     1393 2024-03-08 16:05:18.693955 monkey_agentpluginapi-0.6.0/agentpluginapi/i_agent_binary_repository.py
--rw-r--r--   0        0        0      774 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.6.0/agentpluginapi/i_agent_command_builder_factory.py
--rw-r--r--   0        0        0      368 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.6.0/agentpluginapi/i_agent_event_publishler.py
--rw-r--r--   0        0        0      546 2024-03-08 16:05:18.693955 monkey_agentpluginapi-0.6.0/agentpluginapi/i_agent_otp_provider.py
--rw-r--r--   0        0        0     1372 2024-03-08 16:05:18.693955 monkey_agentpluginapi-0.6.0/agentpluginapi/i_http_agent_binary_server_registrar.py
--rw-r--r--   0        0        0     1879 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.6.0/agentpluginapi/i_linux_agent_command_builder.py
--rw-r--r--   0        0        0      699 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.6.0/agentpluginapi/i_propagation_credentials_repository.py
--rw-r--r--   0        0        0     1166 2024-01-18 13:24:45.273537 monkey_agentpluginapi-0.6.0/agentpluginapi/i_tcp_port_selector.py
--rw-r--r--   0        0        0     2005 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.6.0/agentpluginapi/i_windows_agent_command_builder.py
--rw-r--r--   0        0        0     7090 2024-01-18 13:24:45.273537 monkey_agentpluginapi-0.6.0/agentpluginapi/local_machine_info.py
--rw-r--r--   0        0        0      122 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.6.0/agentpluginapi/payload_result.py
--rw-r--r--   0        0        0      254 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.6.0/agentpluginapi/ping_scan_data.py
--rw-r--r--   0        0        0      468 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.6.0/agentpluginapi/port_scan_data.py
--rw-r--r--   0        0        0        0 2024-01-16 19:42:05.151087 monkey_agentpluginapi-0.6.0/agentpluginapi/py.typed
--rw-r--r--   0        0        0     2313 2024-03-14 13:22:04.064038 monkey_agentpluginapi-0.6.0/agentpluginapi/target_host.py
--rw-r--r--   0        0        0     2033 2024-03-14 13:22:04.064038 monkey_agentpluginapi-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 monkey_agentpluginapi-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1195 2024-05-14 18:03:45.894751 monkey_agentpluginapi-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35255 2024-01-16 19:17:10.913816 monkey_agentpluginapi-0.7.0/LICENSE
+-rw-r--r--   0        0        0      281 2024-01-16 19:51:25.073278 monkey_agentpluginapi-0.7.0/README.md
+-rw-r--r--   0        0        0     1323 2024-05-14 18:03:45.894751 monkey_agentpluginapi-0.7.0/agentpluginapi/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-14 18:03:45.894751 monkey_agentpluginapi-0.7.0/agentpluginapi/agent_binary_request.py
+-rw-r--r--   0        0        0      123 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.7.0/agentpluginapi/dropper_execution_mode.py
+-rw-r--r--   0        0        0      264 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.7.0/agentpluginapi/exploiter_result.py
+-rw-r--r--   0        0        0      278 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.7.0/agentpluginapi/fingerprint_data.py
+-rw-r--r--   0        0        0     1393 2024-03-08 16:05:18.693955 monkey_agentpluginapi-0.7.0/agentpluginapi/i_agent_binary_repository.py
+-rw-r--r--   0        0        0      774 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.7.0/agentpluginapi/i_agent_command_builder_factory.py
+-rw-r--r--   0        0        0      368 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.7.0/agentpluginapi/i_agent_event_publishler.py
+-rw-r--r--   0        0        0      546 2024-03-08 16:05:18.693955 monkey_agentpluginapi-0.7.0/agentpluginapi/i_agent_otp_provider.py
+-rw-r--r--   0        0        0     1550 2024-05-14 18:03:45.894751 monkey_agentpluginapi-0.7.0/agentpluginapi/i_http_agent_binary_server_registrar.py
+-rw-r--r--   0        0        0     1879 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.7.0/agentpluginapi/i_linux_agent_command_builder.py
+-rw-r--r--   0        0        0      699 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.7.0/agentpluginapi/i_propagation_credentials_repository.py
+-rw-r--r--   0        0        0     1166 2024-01-18 13:24:45.273537 monkey_agentpluginapi-0.7.0/agentpluginapi/i_tcp_port_selector.py
+-rw-r--r--   0        0        0     2005 2024-03-08 16:04:53.057846 monkey_agentpluginapi-0.7.0/agentpluginapi/i_windows_agent_command_builder.py
+-rw-r--r--   0        0        0     7090 2024-01-18 13:24:45.273537 monkey_agentpluginapi-0.7.0/agentpluginapi/local_machine_info.py
+-rw-r--r--   0        0        0      122 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.7.0/agentpluginapi/payload_result.py
+-rw-r--r--   0        0        0      254 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.7.0/agentpluginapi/ping_scan_data.py
+-rw-r--r--   0        0        0      468 2024-01-16 19:17:10.833815 monkey_agentpluginapi-0.7.0/agentpluginapi/port_scan_data.py
+-rw-r--r--   0        0        0        0 2024-01-16 19:42:05.151087 monkey_agentpluginapi-0.7.0/agentpluginapi/py.typed
+-rw-r--r--   0        0        0     2313 2024-03-14 13:22:04.064038 monkey_agentpluginapi-0.7.0/agentpluginapi/target_host.py
+-rw-r--r--   0        0        0     2033 2024-05-14 18:03:45.894751 monkey_agentpluginapi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 monkey_agentpluginapi-0.7.0/PKG-INFO
```

### Comparing `monkey_agentpluginapi-0.6.0/CHANGELOG.md` & `monkey_agentpluginapi-0.7.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this
 file.
 
 The format is based on [Keep a
 Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
 the [PEP 440 version scheme](https://peps.python.org/pep-0440/#version-scheme).
 
+## [v0.7.0] - 2024-05-14
+### Changed
+- The `agent_binary_transform` parameter to `agent_binary_wrapper_template` in
+  `IHTTPAgentBinaryServerRegistrar.reserve_download()`. #8
+
 ## [v0.6.0] - 2024-03-14
 ### Fixed
 - An issue in TargetHost that caused ports_status to be shared amongst all
   TargetHosts. #7
 
 ## [v0.5.0] - 2024-03-08
 ### Added
```

### Comparing `monkey_agentpluginapi-0.6.0/LICENSE` & `monkey_agentpluginapi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/__init__.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from .agent_binary_request import (
     AgentBinaryDownloadReservation,
     AgentBinaryDownloadTicket,
-    AgentBinaryTransform,
     ReservationID,
 )
 from .dropper_execution_mode import DropperExecutionMode
 from .exploiter_result import ExploiterResult
 from .fingerprint_data import FingerprintData
 from .i_agent_binary_repository import IAgentBinaryRepository, RetrievalError
 from .i_agent_command_builder_factory import IAgentCommandBuilderFactory
```

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_agent_binary_repository.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_agent_binary_repository.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_agent_command_builder_factory.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_agent_command_builder_factory.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_agent_otp_provider.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_agent_otp_provider.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_http_agent_binary_server_registrar.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_http_agent_binary_server_registrar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import abc
 from ipaddress import IPv4Address
 
 from monkeytypes import OperatingSystem
 
-from .agent_binary_request import AgentBinaryDownloadTicket, AgentBinaryTransform, ReservationID
+from .agent_binary_request import AgentBinaryDownloadTicket, ReservationID
 
 
 class IHTTPAgentBinaryServerRegistrar(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def reserve_download(
         self,
         operating_system: OperatingSystem,
         requestor_ip: IPv4Address,
-        agent_binary_transform: AgentBinaryTransform,
+        agent_binary_wrapper_template: bytes | None,
     ) -> AgentBinaryDownloadTicket:
         """
         Register to download an Agent over HTTP
 
         :param operating_system: The operating system for the Agent binary to serve
         :param requestor_ip: The IP address of the client that will download the Agent binary
-        :param agent_binary_transform: A callable that transforms the Agent binary before serving.
-            This may be used to, e.g., convert the binary into a self-extracting shell script.
+        :param agent_binary_wrapper_template: A bytes template that the bytes from the Agent binary
+            will be inserted into. This may be used to, e.g., convert the Agent binary into a
+            self-extracting shell script. This template should include the string
+            "$(agent_binary)b", which will be replaced by the bytes of the Agent binary.
+            Defaults to None.
         :raises RuntimeError: If the binary could not be served
         :returns: A ticket to download the Agent binary
         """
 
     @abc.abstractmethod
     def clear_reservation(self, reservation_id: ReservationID):
         """
```

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_linux_agent_command_builder.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_linux_agent_command_builder.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_propagation_credentials_repository.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_propagation_credentials_repository.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_tcp_port_selector.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_tcp_port_selector.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/i_windows_agent_command_builder.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/i_windows_agent_command_builder.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/local_machine_info.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/local_machine_info.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/agentpluginapi/target_host.py` & `monkey_agentpluginapi-0.7.0/agentpluginapi/target_host.py`

 * *Files identical despite different names*

### Comparing `monkey_agentpluginapi-0.6.0/pyproject.toml` & `monkey_agentpluginapi-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 [tool.vulture]
 exclude=[]
 paths = ["agentpluginapi", "vulture_allowlist.py"]
 
 [tool.poetry]
 name = "monkey-agentpluginapi"
-version = "v0.6.0"
+version = "v0.7.0"
 description = "Interfaces and components that comprise the Infection Monkey Agent Plugin API"
 authors = [
     "Ilija Lazoroski <ilija.la@live.com>",
     "Kekoa Kaaikala <kekoa.kaaikala@gmail.com>",
     "Mike Salvatore <mike.s.salvatore@gmail.com>",
     "Shreya Malviya <shreya.malviya@gmail.com>",
     "vakarisz <vakarisz@yahoo.com>"
```

### Comparing `monkey_agentpluginapi-0.6.0/PKG-INFO` & `monkey_agentpluginapi-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: monkey-agentpluginapi
-Version: 0.6.0
+Version: 0.7.0
 Summary: Interfaces and components that comprise the Infection Monkey Agent Plugin API
 Home-page: https://github.com/guardicode/agentpluginapi
 License: GPLv3
 Author: Ilija Lazoroski
 Author-email: ilija.la@live.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: egg_timer (>=1.3.0,<2.0.0)
 Requires-Dist: monkey-types
 Requires-Dist: monkeyevents (>=0.4.0,<0.5.0)
 Requires-Dist: monkeytoolbox
 Project-URL: Repository, https://github.com/guardicode/agentpluginapi
 Description-Content-Type: text/markdown
```

