# Comparing `tmp/snek_sploit-0.5.0.tar.gz` & `tmp/snek_sploit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek_sploit-0.5.0.tar", max compression
+gzip compressed data, was "snek_sploit-0.6.0.tar", max compression
```

## Comparing `snek_sploit-0.5.0.tar` & `snek_sploit-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-05-10 12:23:03.555946 snek_sploit-0.5.0/LICENSE
--rw-r--r--   0        0        0     1420 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/README.md
--rw-r--r--   0        0        0      686 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1331 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/__init__.py
--rw-r--r--   0        0        0     4595 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/context.py
--rw-r--r--   0        0        0     3004 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/metasploit.py
--rw-r--r--   0        0        0        0 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/__init__.py
--rw-r--r--   0        0        0     3086 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/auth.py
--rw-r--r--   0        0        0    10952 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/consoles.py
--rw-r--r--   0        0        0     7892 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/core.py
--rw-r--r--   0        0        0    12331 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/db.py
--rw-r--r--   0        0        0      728 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/health.py
--rw-r--r--   0        0        0     2676 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/jobs.py
--rw-r--r--   0        0        0    19865 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/modules.py
--rw-r--r--   0        0        0     1629 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/plugins.py
--rw-r--r--   0        0        0    24221 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/sessions.py
--rw-r--r--   0        0        0        0 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/__init__.py
--rw-r--r--   0        0        0     1887 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/constants.py
--rw-r--r--   0        0        0      448 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/enums.py
--rw-r--r--   0        0        0      276 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/exceptions.py
--rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 snek_sploit-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1539 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/README.md
+-rw-r--r--   0        0        0      686 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1393 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/snek_sploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/snek_sploit/lib/__init__.py
+-rw-r--r--   0        0        0     4696 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/context.py
+-rw-r--r--   0        0        0     3004 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/metasploit.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/auth.py
+-rw-r--r--   0        0        0    10952 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/consoles.py
+-rw-r--r--   0        0        0     7892 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/core.py
+-rw-r--r--   0        0        0    12331 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/db.py
+-rw-r--r--   0        0        0      728 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/health.py
+-rw-r--r--   0        0        0     2676 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/jobs.py
+-rw-r--r--   0        0        0    19865 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/modules.py
+-rw-r--r--   0        0        0     1629 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/plugins.py
+-rw-r--r--   0        0        0    24221 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/sessions.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/constants.py
+-rw-r--r--   0        0        0      448 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/enums.py
+-rw-r--r--   0        0        0      276 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/exceptions.py
+-rw-r--r--   0        0        0      713 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/retry.py
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 snek_sploit-0.6.0/PKG-INFO
```

### Comparing `snek_sploit-0.5.0/LICENSE` & `snek_sploit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/README.md` & `snek_sploit-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 if __name__ == '__main__':
     client = MetasploitClient("msf", "root")
     print(client.core.rpc.version())
 
 ```
 
+Examples can be found in the *[examples](https://github.com/SadParad1se/snek-sploit/tree/master/examples)* directory.
+
 ## Starting MSF RPC server
 In Metasploit console:
 ```shell
 load msgrpc ServerHost=127.0.0.1 ServerPort=55553 User=msf Pass='root' SSL=true
 ```
 
 In shell:
```

### Comparing `snek_sploit-0.5.0/pyproject.toml` & `snek_sploit-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snek-sploit"
-version = "0.5.0"
+version = "0.6.0"
 description = "Python RPC client for Metasploit Framework"
 authors = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
 maintainers = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
```

### Comparing `snek_sploit-0.5.0/snek_sploit/__init__.py` & `snek_sploit-0.6.0/snek_sploit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,40 @@
     "ConsoleInfo",
     "ConsoleData",
     "ConsoleOptions",
     "ModuleStatistics",
     "VersionInformation",
     "FrameworkThread",
     "JobInformation",
-    "ModuleType",
     "EncodingOptions",
     "ModuleShortInfo",
     "ModuleExecutionInfo",
     "ModuleRunningStatistics",
     "SessionInformation",
     "MeterpreterSessionTransportOptions",
     "SessionShell",
     "SessionMeterpreter",
     "SessionRing",
     "Error",
     "InputError",
     "RPCError",
+    "SessionType",
+    "ModuleType",
 ]
 
 from snek_sploit.lib.metasploit import MetasploitClient
 
 # from snek_sploit.lib.rpc.auth import
 from snek_sploit.lib.rpc.consoles import ConsoleInfo, ConsoleData, ConsoleOptions
 from snek_sploit.lib.rpc.core import ModuleStatistics, VersionInformation, FrameworkThread
 
 # from snek_sploit.lib.rpc.db import
 # from snek_sploit.lib.rpc.health import
 from snek_sploit.lib.rpc.jobs import JobInformation
 from snek_sploit.lib.rpc.modules import (
-    ModuleType,
     EncodingOptions,
     ModuleShortInfo,
     ModuleExecutionInfo,
     ModuleRunningStatistics,
 )
 
 # from snek_sploit.lib.rpc.plugins import
@@ -44,7 +44,8 @@
     SessionInformation,
     MeterpreterSessionTransportOptions,
     SessionShell,
     SessionMeterpreter,
     SessionRing,
 )
 from snek_sploit.util.exceptions import Error, InputError, RPCError
+from snek_sploit.util.enums import SessionType, ModuleType
```

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/context.py` & `snek_sploit-0.6.0/snek_sploit/lib/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 import msgpack
 from abc import ABC
 from typing import Union, List, Dict
 
 from snek_sploit.util import constants, exceptions
+from snek_sploit.util.retry import retry
 
 
 ResponseDict = Dict[Union[int, str, bytes], Union[int, str, bytes, list, dict, bool]]
 ResponseList = List[Union[str, bytes, dict]]
 RPCResponse = Union[ResponseDict, str, ResponseList]
 
 
@@ -59,14 +60,15 @@
         arguments = [self.token] if use_token else []
 
         if call_arguments is not None:
             arguments += call_arguments
 
         return arguments
 
+    @retry(tries=3, on_errors=(requests.RequestException,))
     def call(
         self, endpoint: str, arguments: list = None, use_token: bool = True, timeout: Union[float, tuple] = None
     ) -> RPCResponse:
         """
         Create a call to an endpoint.
         :param endpoint: Endpoint name
         :param arguments: Arguments that will be processed and passed to the endpoint
```

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/metasploit.py` & `snek_sploit-0.6.0/snek_sploit/lib/metasploit.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/auth.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/consoles.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/consoles.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/core.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/core.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/db.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/db.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/health.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/health.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/jobs.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/jobs.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/modules.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/plugins.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/plugins.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/lib/rpc/sessions.py` & `snek_sploit-0.6.0/snek_sploit/lib/rpc/sessions.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/snek_sploit/util/constants.py` & `snek_sploit-0.6.0/snek_sploit/util/constants.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.5.0/PKG-INFO` & `snek_sploit-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek-sploit
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python RPC client for Metasploit Framework
 Home-page: https://github.com/SadParad1se/snek-sploit
 License: MIT
 Keywords: metasploit,msf,rpc,client
 Author: Jiří Rája
 Author-email: jiri.raja@gmail.com
 Maintainer: Jiří Rája
@@ -41,14 +41,16 @@
 
 if __name__ == '__main__':
     client = MetasploitClient("msf", "root")
     print(client.core.rpc.version())
 
 ```
 
+Examples can be found in the *[examples](https://github.com/SadParad1se/snek-sploit/tree/master/examples)* directory.
+
 ## Starting MSF RPC server
 In Metasploit console:
 ```shell
 load msgrpc ServerHost=127.0.0.1 ServerPort=55553 User=msf Pass='root' SSL=true
 ```
 
 In shell:
```

