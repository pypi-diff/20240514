# Comparing `tmp/pyDuotecno-2024.3.2.tar.gz` & `tmp/pyduotecno-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDuotecno-2024.3.2.tar", last modified: Wed Mar 27 17:43:31 2024, max compression
+gzip compressed data, was "pyduotecno-2024.5.0.tar", last modified: Tue May 14 16:43:28 2024, max compression
```

## Comparing `pyDuotecno-2024.3.2.tar` & `pyduotecno-2024.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:43:31.905314 pyDuotecno-2024.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-27 17:43:31.905314 pyDuotecno-2024.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:43:31.905314 pyDuotecno-2024.3.2/duotecno/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/duotecno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/duotecno/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/duotecno/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/duotecno/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/duotecno/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/duotecno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/duotecno/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:43:31.905314 pyDuotecno-2024.3.2/pyDuotecno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-27 17:43:31.000000 pyDuotecno-2024.3.2/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-27 17:43:31.000000 pyDuotecno-2024.3.2/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:43:31.000000 pyDuotecno-2024.3.2/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:43:31.000000 pyDuotecno-2024.3.2/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-27 17:43:31.000000 pyDuotecno-2024.3.2/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 17:43:31.905314 pyDuotecno-2024.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-27 17:43:27.000000 pyDuotecno-2024.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:28.925104 pyduotecno-2024.5.0/duotecno/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/pyDuotecno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/setup.py
```

### Comparing `pyDuotecno-2024.3.2/LICENSE` & `pyduotecno-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2024.3.2/PKG-INFO` & `pyduotecno-2024.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2024.3.2
+Version: 2024.5.0
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2024.3.2/duotecno/controller.py` & `pyduotecno-2024.5.0/duotecno/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from __future__ import annotations
 import asyncio
 import logging
 from collections import deque
 from duotecno.exceptions import LoadFailure, InvalidPassword
 from duotecno.protocol import (
     Packet,
-    EV_CLIENTCONNECTSET_3,
     EV_NODEDATABASEINFO_0,
     EV_NODEDATABASEINFO_1,
     EV_HEARTBEATSTATUS_1,
 )
 from duotecno.node import Node
 from duotecno.unit import BaseUnit
 
@@ -23,17 +22,21 @@
     - open and close the connection
     """
 
     writer: asyncio.StreamWriter | None = None
     reader: asyncio.StreamReader | None = None
     readerTask: asyncio.Task[None]
     hbTask: asyncio.Task[None]
-    loginOK: asyncio.Event
+    handleTask: asyncio.Task[None]
+    receiveQueue: asyncio.Queue
+    sendQueue: asyncio.Queue
     connectionOK: asyncio.Event
     heartbeatReceived: asyncio.Event
+    packetToWaitFor: str | None = None
+    packetWaiter: asyncio.Event
     nodes: dict[int, Node] = {}
     host: str
     port: int
     password: str
 
     def get_units(self, unit_type: list[str] | str) -> list[BaseUnit]:
         res = []
@@ -51,15 +54,14 @@
         self._log.debug("Disable all Units on all nodes")
         for node in self.nodes.values():
             await node.disable()
 
     async def disconnect(self) -> None:
         self._log.debug("Disconnecting")
         self.connectionOK.clear()
-        self.loginOK.clear()
 
         self.readerTask.cancel()
         if self.writer:
             self.writer.close()
             self._log.debug("Waiting to finish disconnecting")
             await self.writer.wait_closed()
         self._log.debug("Disconnecting Finished")
@@ -88,30 +90,32 @@
             self.reader, self.writer = await asyncio.open_connection(
                 self.host, self.port
             )
         except (ConnectionError, TimeoutError):
             raise
         # events
         self.connectionOK = asyncio.Event()
-        self.loginOK = asyncio.Event()
         self.heartbeatReceived = asyncio.Event()
+        self.packetWaiter = asyncio.Event()
         # at this point the connection should be ok
         self._log.debug("Connection established")
         self.connectionOK.set()
-        self.loginOK.clear()
         self.heartbeatReceived.clear()
         # start the bus reading task
+        self.sendTask = asyncio.Task(self.sendTask())
         self.readerTask = asyncio.Task(self.readTask())
+        self.handleTask = asyncio.Task(self.handleTask())
+        self.receiveQueue = asyncio.Queue()
+        self.sendQueue = asyncio.Queue()
         # send login info
         passw = [str(ord(i)) for i in self.password]
         await self.write(f"[214,3,{len(passw)},{','.join(passw)}]")
         # wait for the login to be ok
         try:
-            await asyncio.wait_for(self.loginOK.wait(), timeout=5.0)
-            await self.loginOK.wait()
+            await asyncio.wait_for(self.waitForPacket("67,3,1"), timeout=5.0)
         except TimeoutError:
             await self.disconnect()
             raise InvalidPassword()
         # if we are not testing the connection, start scanning
         if testOnly:
             return
         # do we need to reload the modules?
@@ -136,22 +140,29 @@
     async def write(self, msg: str) -> None:
         """Send a message."""
         if not self.writer:
             return
         if self.writer.transport.is_closing():
             await self._reconnect()
             return
-        self._log.debug(f"Send: {msg}")
-        msg = f"{msg}{chr(10)}"
-        try:
-            self.writer.write(msg.encode())
-            await self.writer.drain()
-        except ConnectionError:
-            await self.reconnect()
-            return
+        # self._log.debug(f"Send: {msg}")
+        await self.sendQueue.put(msg)
+
+    async def sendTask(self) -> None:
+        """Send task."""
+        while self.connectionOK.is_set() and self.reader:
+            msg = await self.sendQueue.get()
+            self._log.debug(f"Transmitting: {msg}")
+            msg = f"{msg}{chr(10)}"
+            try:
+                self.writer.write(msg.encode())
+                await self.writer.drain()
+            except ConnectionError:
+                await self.reconnect()
+                return
 
     async def _loadTask(self) -> None:
         while len(self.nodes) < 1:
             await asyncio.sleep(3)
         while True:
             c = 0
             for n in self.nodes.values():
@@ -222,49 +233,72 @@
                 tmp = tmp.lstrip("[")
             tmp = tmp.replace("\x00", "")
             # self._log.debug(f'Receive: "{tmp}"')
             tmp = tmp[1:-1]
             if tmp == "":
                 return
             self._log.debug(f'Receive: "{tmp}"')
+            await self._comparePacket(tmp)
             p = tmp.split(",")
             try:
                 pc = Packet(int(p[0]), int(p[1]), deque([int(_i) for _i in p[2:]]))
-                await self._handlePacket(pc)
+                await self.receiveQueue.put(pc)
             except Exception as e:
                 self._log.error(e)
                 self._log.error(tmp)
-            if not self.loginOK.is_set():
-                self._log.error("Login failed")
-                self.connectionOK.clear()
+
+    async def _comparePacket(self, rpck: str) -> None:
+        if not self.packetToWaitFor:
+            return
+        self._log.debug(f"COMPARE received packet {rpck} with {self.packetToWaitFor}")
+        if rpck.startswith(self.packetToWaitFor):
+            self.packetWaiter.set()
+
+    async def waitForPacket(self, pstr: str) -> None:
+        """Wait for a certain packet.
+
+        will clear an event and then wait for the event to be set again
+        """
+        self.packetWaiter.clear()
+        self.packetToWaitFor = pstr
+        await self.packetWaiter.wait()
+        self.packetToWaitFor = None
+
+    async def handleTask(self) -> None:
+        """handler task."""
+        while self.connectionOK.is_set() and self.receiveQueue:
+            try:
+                pc = await self.receiveQueue.get()
+                self._log.debug(f"Handle: {pc}")
+                await self._handlePacket(pc)
+            except Exception as e:
+                self._log.error(e)
 
     async def _handlePacket(self, packet: Packet) -> None:
         if packet.cls is None:
             self._log.debug(f"Ignoring packet: {packet}")
             return
         if isinstance(packet.cls, EV_HEARTBEATSTATUS_1):
             self.heartbeatReceived.set()
             return
-        if isinstance(packet.cls, EV_CLIENTCONNECTSET_3):
-            if packet.cls.loginOK == 1:
-                self.loginOK.set()
-                return
         if isinstance(packet.cls, EV_NODEDATABASEINFO_0):
             for i in range(packet.cls.numNode):
                 await self.write(f"[209,1,{i}]")
+                await self.waitForPacket(f"64,1,{i}")
             return
         if isinstance(packet.cls, EV_NODEDATABASEINFO_1):
             if packet.cls.address not in self.nodes:
                 self.nodes[packet.cls.address] = Node(
                     name=packet.cls.nodeName,
                     address=packet.cls.address,
                     index=packet.cls.index,
                     nodeType=packet.cls.nodeType,
                     numUnits=packet.cls.numUnits,
                     writer=self.write,
+                    pwaiter=self.waitForPacket,
                 )
                 await self.nodes[packet.cls.address].load()
             return
         if hasattr(packet.cls, "address") and packet.cls.address in self.nodes:
             await self.nodes[packet.cls.address].handlePacket(packet.cls)
             return
         self._log.debug(f"Ignoring packet: {packet}")
```

### Comparing `pyDuotecno-2024.3.2/duotecno/node.py` & `pyduotecno-2024.5.0/duotecno/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,24 @@
         self,
         name: str,
         address: int,
         index: int,
         nodeType: NodeType,
         numUnits: int,
         writer: Callable[[str], Awaitable[None]],
+        pwaiter: Callable[[str], Awaitable[None]],
     ) -> None:
         self._log = logging.getLogger("pyduotecno-node")
         self.name = name
         self.address = address
         self.index = index
         self.numUnits = numUnits
         self.nodeType = nodeType
         self.writer = writer
+        self.pwaiter = pwaiter
         self.isLoaded = asyncio.Event()
         self.isLoaded.clear()
         self.units = {}
         self._log.debug(f"New node found: {self.name}")
 
     async def enable(self) -> None:
         for unit in self.units.values():
@@ -82,14 +84,15 @@
                     res.append(unit)
         return res
 
     async def load(self) -> None:
         self._log.debug(f"Node {self.name}: Requesting units")
         for i in range(self.numUnits):
             await self.writer(f"[209,2,{self.address},{i}]")
+            await self.pwaiter(f"64,2,{self.address},{i}")
 
     async def handlePacket(self, packet: BaseMessage) -> None:
         if isinstance(packet, EV_NODEDATABASEINFO_2):
             if packet.unit not in self.units:
                 u = BaseUnit
                 if packet.unitTypeName == "SWITCH":
                     u = SwitchUnit
```

### Comparing `pyDuotecno-2024.3.2/duotecno/protocol.py` & `pyduotecno-2024.5.0/duotecno/protocol.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2024.3.2/duotecno/unit.py` & `pyduotecno-2024.5.0/duotecno/unit.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2024.3.2/pyDuotecno.egg-info/PKG-INFO` & `pyduotecno-2024.5.0/pyDuotecno.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2024.3.2
+Version: 2024.5.0
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2024.3.2/pyproject.toml` & `pyduotecno-2024.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "pyDuotecno"
 license = {text = "Apache"}
-version = "2024.3.2"
+version = "2024.5.0"
 description = "Open-source home automation platform running on Python 3."
 readme = "README.md"
 authors = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords = ["home", "duotecno", "automation"]
 classifiers = [
@@ -37,15 +37,15 @@
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*", "examples", "examples/*"]
 
 [tool.bumpver]
-current_version = "2024.3.2"
+current_version = "2024.5.0"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

