# Comparing `tmp/local_tuya-2.4.0.tar.gz` & `tmp/local_tuya-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_tuya-2.4.0.tar", max compression
+gzip compressed data, was "local_tuya-3.0.0.tar", max compression
```

## Comparing `local_tuya-2.4.0.tar` & `local_tuya-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0     1070 2024-05-12 19:23:34.579978 local_tuya-2.4.0/LICENSE
--rw-r--r--   0        0        0     2510 2024-05-12 19:23:34.579978 local_tuya-2.4.0/README.md
--rw-r--r--   0        0        0      445 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/__init__.py
--rw-r--r--   0        0        0     1070 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/backoff.py
--rw-r--r--   0        0        0     1580 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/README.md
--rw-r--r--   0        0        0      213 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/__init__.py
--rw-r--r--   0        0        0     3341 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/buffer.py
--rw-r--r--   0        0        0      395 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/config.py
--rw-r--r--   0        0        0     1855 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/constraints.py
--rw-r--r--   0        0        0     2778 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/device.py
--rw-r--r--   0        0        0      786 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/enums.py
--rw-r--r--   0        0        0     1288 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/state.py
--rw-r--r--   0        0        0      541 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/errors.py
--rw-r--r--   0        0        0     1149 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/events.py
--rw-r--r--   0        0        0      943 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/protocol/README.md
--rw-r--r--   0        0        0      167 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/__init__.py
--rw-r--r--   0        0        0      898 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/config.py
--rw-r--r--   0        0        0      618 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/events.py
--rw-r--r--   0        0        0     1055 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/heartbeat.py
--rw-r--r--   0        0        0      321 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/__init__.py
--rw-r--r--   0        0        0      549 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/__init__.py
--rw-r--r--   0        0        0      827 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/crypto.py
--rw-r--r--   0        0        0      759 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/handler.py
--rw-r--r--   0        0        0     6480 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/v33.py
--rw-r--r--   0        0        0     1562 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/messages.py
--rw-r--r--   0        0        0     2668 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/protocol.py
--rw-r--r--   0        0        0     1717 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/receiver.py
--rw-r--r--   0        0        0     3459 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/sender.py
--rw-r--r--   0        0        0     2372 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/state.py
--rw-r--r--   0        0        0     5577 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/transport.py
--rw-r--r--   0        0        0        0 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/py.typed
--rw-r--r--   0        0        0      958 2024-05-12 19:23:34.583978 local_tuya-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 local_tuya-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-14 08:07:11.836604 local_tuya-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2510 2024-05-14 08:07:11.836604 local_tuya-3.0.0/README.md
+-rw-r--r--   0        0        0      445 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/backoff.py
+-rw-r--r--   0        0        0     1580 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/README.md
+-rw-r--r--   0        0        0      213 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/__init__.py
+-rw-r--r--   0        0        0     3339 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/buffer.py
+-rw-r--r--   0        0        0      395 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/config.py
+-rw-r--r--   0        0        0     1855 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/constraints.py
+-rw-r--r--   0        0        0      995 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/dependencies.py
+-rw-r--r--   0        0        0     2636 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/device.py
+-rw-r--r--   0        0        0      786 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/enums.py
+-rw-r--r--   0        0        0     1237 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/device/state.py
+-rw-r--r--   0        0        0      541 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/errors.py
+-rw-r--r--   0        0        0     1110 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/events.py
+-rw-r--r--   0        0        0      943 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/README.md
+-rw-r--r--   0        0        0      280 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/config.py
+-rw-r--r--   0        0        0     2319 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/dependencies.py
+-rw-r--r--   0        0        0      618 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/events.py
+-rw-r--r--   0        0        0     1055 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/heartbeat.py
+-rw-r--r--   0        0        0      321 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/message/__init__.py
+-rw-r--r--   0        0        0      533 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/message/handlers/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/message/handlers/crypto.py
+-rw-r--r--   0        0        0      759 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/message/handlers/handler.py
+-rw-r--r--   0        0        0     6480 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/message/handlers/v33.py
+-rw-r--r--   0        0        0     1562 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/message/messages.py
+-rw-r--r--   0        0        0      571 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/protocol.py
+-rw-r--r--   0        0        0     1717 2024-05-14 08:07:11.836604 local_tuya-3.0.0/local_tuya/protocol/receiver.py
+-rw-r--r--   0        0        0     3459 2024-05-14 08:07:11.840604 local_tuya-3.0.0/local_tuya/protocol/sender.py
+-rw-r--r--   0        0        0     2382 2024-05-14 08:07:11.840604 local_tuya-3.0.0/local_tuya/protocol/state.py
+-rw-r--r--   0        0        0     5783 2024-05-14 08:07:11.840604 local_tuya-3.0.0/local_tuya/protocol/transport.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:07:11.840604 local_tuya-3.0.0/local_tuya/py.typed
+-rw-r--r--   0        0        0      979 2024-05-14 08:07:11.840604 local_tuya-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 local_tuya-3.0.0/PKG-INFO
```

### Comparing `local_tuya-2.4.0/LICENSE` & `local_tuya-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/README.md` & `local_tuya-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/backoff.py` & `local_tuya-3.0.0/local_tuya/backoff.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/device/README.md` & `local_tuya-3.0.0/local_tuya/device/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/device/buffer.py` & `local_tuya-3.0.0/local_tuya/device/buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,12 +88,12 @@
         # Wait until we receive real confirmation of update via status.
         await asyncio.wait_for(
             self._state_handler.matches(values),
             self._confirm_timeout,
         )
 
     async def _filter(self, values: Values) -> Values:
-        state = await self._state_handler.state()
+        state = await self._state_handler.get()
         filtered = {k: v for k, v in values.items() if state[k] != v}
         if not self._constraints:
             return filtered
         return self._constraints.filter_values(filtered, state)
```

### Comparing `local_tuya-2.4.0/local_tuya/device/constraints.py` & `local_tuya-3.0.0/local_tuya/device/constraints.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/device/device.py` & `local_tuya-3.0.0/local_tuya/device/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,69 @@
+import asyncio
 import logging
 from contextlib import AsyncExitStack
-from typing import Any, Awaitable, Callable, Generic, Optional, TypeVar
-from warnings import warn
+from typing import AsyncIterator, Callable, Generic, Optional, TypeVar, cast
 
-from typing_extensions import deprecated
+from imbue import Container
 
 from local_tuya.device.buffer import UpdateBuffer
 from local_tuya.device.config import DeviceConfig
 from local_tuya.device.constraints import Constraints
+from local_tuya.device.dependencies import DevicePackage
 from local_tuya.device.enums import State
 from local_tuya.device.state import StateHandler
-from local_tuya.events import maybe_async
-from local_tuya.protocol import Protocol, Values
+from local_tuya.events import EventNotifier
+from local_tuya.protocol import Protocol, ProtocolPackage, StateUpdated, Values
 
 logger = logging.getLogger(__name__)
 T = TypeVar("T", bound=State)
 
 
 class Device(AsyncExitStack, Generic[T]):
     def __init__(
         self,
         config: DeviceConfig,
         load_state: Callable[[Values], T],
-        state_updated_callback: Optional[Callable[[T], Any]] = None,
-        connection_broken_callback: Optional[Callable[[], Any]] = None,
         constraints: Optional[Constraints] = None,
     ):
-        if connection_broken_callback is not None:
-            warn(
-                "Parameter `connection_broken_callback` of local_tuya.Device will be removed.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
         super().__init__()
         self._load_state = load_state
-        self._state_updated_callback_func: Optional[Callable[[T], Awaitable]] = (
-            maybe_async(state_updated_callback) if state_updated_callback else None
-        )
-        self._state_handler = StateHandler(self._state_updated_callback)
-        self._protocol = Protocol(
-            config.protocol,
-            self._state_handler.updated,
-        )
-        self._buffer = UpdateBuffer(
-            delay=config.debounce_updates,
-            confirm_timeout=config.confirm_timeout,
-            protocol=self._protocol,
-            state_handler=self._state_handler,
-            constraints=constraints,
-        )
+        self._container = Container(
+            DevicePackage(config, constraints),
+            ProtocolPackage(config.protocol),
+        ).application_context()
+        self._state_handler: Optional[StateHandler] = None
+        self._buffer: Optional[UpdateBuffer] = None
+        self._last_state: Optional[T] = None
+        self._state_updated = asyncio.Event()
 
     async def __aenter__(self):
-        await self.enter_async_context(self._protocol)
-        self.enter_context(self._buffer)
+        await self.enter_async_context(self._container)
+        self._state_handler = await self._container.get(StateHandler)
+        self._buffer = await self._container.get(UpdateBuffer)
+        event_notifier = await self._container.get(EventNotifier)
+        event_notifier.register(StateUpdated, self._update_last_state)
+        (await self._container.get(Protocol)).connect()
         return self
 
-    @deprecated(
-        "Method local_tuya.Device.set_state_updated_callback will be removed.",
-        stacklevel=2,
-    )
-    def set_state_updated_callback(self, callback: Callable[[T], Any]) -> None:
-        self._state_updated_callback_func = maybe_async(callback)
+    async def state(self) -> AsyncIterator[T]:
+        if self._last_state:
+            yield self._last_state
+        while True:
+            await self._state_updated.wait()
+            self._state_updated.clear()
+            yield cast(T, self._last_state)
+
+    def _update_last_state(self, event: StateUpdated) -> None:
+        self._last_state = self._load_state(event.values)
+        logger.debug("received new device state: %s", self._last_state)
+        self._state_updated.set()
 
     async def _state(self) -> T:
-        return self._load_state(await self._state_handler.state())
+        if not self._state_handler:
+            raise RuntimeError(f"{self:r} context has not been entered")
+        return self._load_state(await self._state_handler.get())
 
     async def _update(self, values: Values) -> None:
+        if not self._buffer:
+            raise RuntimeError(f"{self:r} context has not been entered")
         await self._buffer.update(values)
-
-    async def _state_updated_callback(self, values: Values) -> None:
-        state = self._load_state(values)
-        logger.debug("received new device state: %s", state)
-        if self._state_updated_callback_func:
-            await self._state_updated_callback_func(state)
```

### Comparing `local_tuya-2.4.0/local_tuya/device/enums.py` & `local_tuya-3.0.0/local_tuya/device/enums.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/errors.py` & `local_tuya-3.0.0/local_tuya/errors.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/events.py` & `local_tuya-3.0.0/local_tuya/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import inspect
-from abc import ABC
 from collections import defaultdict
 from typing import Any, Awaitable, Callable, DefaultDict, List, Type, TypeVar, cast
 
 from typing_extensions import ParamSpec
 
 
-class Event(ABC):  # noqa: B024
+class Event:
     """Base event class"""
 
 
 T = TypeVar("T", bound=Event)
 
 
 class EventNotifier:
@@ -19,26 +18,26 @@
             Type[Event], List[Callable[[Event], Awaitable[None]]]
         ] = defaultdict(list)
 
     def register(self, event_class: Type[T], listener: Callable[[T], Any]) -> None:
         self._listeners[event_class].append(
             cast(
                 Callable[[Event], Awaitable[None]],
-                maybe_async(listener),
+                _make_async(listener),
             )
         )
 
     async def emit(self, event: Event) -> None:
         for listener in self._listeners[type(event)]:
             await listener(event)
 
 
 P = ParamSpec("P")
 
 
-def maybe_async(func: Callable[P, Any]) -> Callable[P, Awaitable[None]]:
+def _make_async(func: Callable[P, Any]) -> Callable[P, Awaitable[None]]:
     async def _wrapper(*args: P.args, **kwargs: P.kwargs) -> None:
         res = func(*args, **kwargs)
         if inspect.iscoroutine(res):
             await res
 
     return _wrapper
```

### Comparing `local_tuya-2.4.0/local_tuya/protocol/README.md` & `local_tuya-3.0.0/local_tuya/protocol/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/config.py` & `local_tuya-3.0.0/local_tuya/protocol/config.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/events.py` & `local_tuya-3.0.0/local_tuya/protocol/events.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/heartbeat.py` & `local_tuya-3.0.0/local_tuya/protocol/heartbeat.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/message/handlers/__init__.py` & `local_tuya-3.0.0/local_tuya/protocol/message/handlers/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,11 +7,10 @@
 HANDLERS: List[Type[MessageHandler]] = [
     V33MessageHandler,
 ]
 
 
 def get_handler(config: ProtocolConfig) -> MessageHandler:
     for handler_class in HANDLERS:
-        handler_ = handler_class.from_config(config)
-        if handler_:
+        if handler_ := handler_class.from_config(config):
             return handler_
     raise ValueError(f"unsupported device: {config!r}")
```

### Comparing `local_tuya-2.4.0/local_tuya/protocol/message/handlers/crypto.py` & `local_tuya-3.0.0/local_tuya/protocol/message/handlers/crypto.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/message/handlers/handler.py` & `local_tuya-3.0.0/local_tuya/protocol/message/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/message/handlers/v33.py` & `local_tuya-3.0.0/local_tuya/protocol/message/handlers/v33.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/message/messages.py` & `local_tuya-3.0.0/local_tuya/protocol/message/messages.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/protocol.py` & `local_tuya-3.0.0/local_tuya/protocol/dependencies.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,74 @@
-import asyncio
-from contextlib import AsyncExitStack
-from typing import Awaitable, Callable, Optional
+from typing import AsyncIterator
+
+from imbue import ContextualizedDependency, Package, auto_context
 
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.config import ProtocolConfig
-from local_tuya.protocol.events import CommandSent, StateUpdated
 from local_tuya.protocol.heartbeat import Heartbeat
 from local_tuya.protocol.message import (
     MessageHandler,
-    UpdateCommand,
-    Values,
     get_handler,
 )
+from local_tuya.protocol.protocol import Protocol
 from local_tuya.protocol.receiver import Receiver
 from local_tuya.protocol.sender import Sender
 from local_tuya.protocol.state import State
 from local_tuya.protocol.transport import Transport
 
 
-def _state_updated_callback(
-    func: Callable[[Values], Awaitable],
-) -> Callable[[StateUpdated], Awaitable]:
-    async def _wrapper(event: StateUpdated) -> None:
-        await func(event.values)
-
-    return _wrapper
-
+class ProtocolPackage(Package):
+    EXTRA_DEPENDENCIES = (
+        ContextualizedDependency(Receiver, eager=True),
+        Protocol,
+    )
+
+    def __init__(self, config: ProtocolConfig):
+        self._cfg = config
+
+    @auto_context
+    def event_notifier(self) -> EventNotifier:
+        return EventNotifier()
+
+    @auto_context
+    def message_handler(self) -> MessageHandler:
+        return get_handler(self._cfg)
+
+    @auto_context(eager=True)
+    async def transport(self, notifier: EventNotifier) -> AsyncIterator[Transport]:
+        async with Transport(
+            address=self._cfg.address,
+            port=self._cfg.port,
+            backoff=self._cfg.connection_backoff,
+            timeout=self._cfg.timeout,
+            event_notifier=notifier,
+        ) as transport:
+            yield transport
 
-class Protocol(asyncio.Protocol, AsyncExitStack):
-    def __init__(
+    @auto_context(eager=True)
+    async def sender(
         self,
-        config: ProtocolConfig,
-        state_updated_callback: Optional[Callable[[Values], Awaitable]] = None,
-    ):
-        super().__init__()
-        self._config = config
-        self._event_notifier = EventNotifier()
-        if state_updated_callback:
-            self._event_notifier.register(
-                StateUpdated,
-                _state_updated_callback(state_updated_callback),
-            )
-        message_handler: MessageHandler = get_handler(config)
-        self._transport = Transport(
-            address=config.address,
-            port=config.port,
-            backoff=config.connection_backoff,
-            timeout=config.timeout,
-            event_notifier=self._event_notifier,
-        )
-        self._sender = Sender(
-            message_handler=message_handler,
-            event_notifier=self._event_notifier,
-            timeout=config.timeout,
-        )
-        self._receiver = Receiver(
-            message_handler=message_handler,
-            event_notifier=self._event_notifier,
-        )
-        self._heartbeat = Heartbeat(
-            interval=config.heartbeat_interval,
-            event_notifier=self._event_notifier,
-        )
-        self._state_keeper = State(
-            refresh_interval=config.state_refresh_interval,
-            event_notifier=self._event_notifier,
-        )
-
-    async def __aenter__(self):
-        await self.enter_async_context(self._transport)
-        await self.enter_async_context(self._sender)
-        self.enter_context(self._heartbeat)
-        self.enter_context(self._state_keeper)
-        return self
-
-    async def update(self, values: Values) -> None:
-        """Update the device."""
-        await self._event_notifier.emit(CommandSent(UpdateCommand(values)))
+        notifier: EventNotifier,
+        msg_handler: MessageHandler,
+    ) -> AsyncIterator[Sender]:
+        async with Sender(
+            message_handler=msg_handler,
+            event_notifier=notifier,
+            timeout=self._cfg.timeout,
+        ) as sender:
+            yield sender
+
+    @auto_context(eager=True)
+    async def heartbeat(self, notifier: EventNotifier) -> AsyncIterator[Heartbeat]:
+        with Heartbeat(
+            interval=self._cfg.heartbeat_interval,
+            event_notifier=notifier,
+        ) as heartbeat:
+            yield heartbeat
+
+    @auto_context(eager=True)
+    async def state_keeper(self, notifier: EventNotifier) -> AsyncIterator[State]:
+        with State(
+            refresh_interval=self._cfg.state_refresh_interval,
+            event_notifier=notifier,
+        ) as state_keeper:
+            yield state_keeper
```

### Comparing `local_tuya-2.4.0/local_tuya/protocol/receiver.py` & `local_tuya-3.0.0/local_tuya/protocol/receiver.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/sender.py` & `local_tuya-3.0.0/local_tuya/protocol/sender.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.4.0/local_tuya/protocol/state.py` & `local_tuya-3.0.0/local_tuya/protocol/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,18 @@
         if event.response.error:
             pass
         elif isinstance(event.response, StateResponse):
             new_state = event.response.values
             if self._state != new_state:
                 logger.debug("received new device state: %s", new_state)
                 self._state = new_state
-                await self._notifier.emit(StateUpdated(self._state))
+                await self._notifier.emit(StateUpdated(new_state.copy()))
         elif isinstance(event.response, StatusResponse):
             if self._state is None:
                 # We have not yet received the initial state.
                 # Better discard this as the state might be newer.
                 return
             new_state = {**self._state, **event.response.values}
             if self._state != new_state:
                 logger.debug("received device state update: %s", event.response.values)
                 self._state = new_state
-                await self._notifier.emit(StateUpdated(self._state))
+                await self._notifier.emit(StateUpdated(new_state.copy()))
```

### Comparing `local_tuya-2.4.0/local_tuya/protocol/transport.py` & `local_tuya-3.0.0/local_tuya/protocol/transport.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import logging
 import re
-from typing import Optional, cast
+from contextlib import AbstractAsyncContextManager
+from typing import Awaitable, Optional, cast
 
 from concurrent_tasks import BackgroundTask
 
 from local_tuya.backoff import Backoff
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.events import (
     ConnectionClosed,
@@ -14,15 +15,15 @@
     DataSent,
     ResponseReceived,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class Transport(asyncio.Protocol):
+class Transport(AbstractAsyncContextManager, asyncio.Protocol):
     def __init__(
         self,
         address: str,
         port: int,
         backoff: Backoff,
         timeout: float,
         event_notifier: EventNotifier,
@@ -42,26 +43,28 @@
         self._close_exc: Optional[Exception] = None
         self._connected = asyncio.Event()
         self._connect_task = BackgroundTask(self._connect)
         self._receive_task = BackgroundTask(self._receive)
         # We need a queue as `data_received` is not async.
         self._received_bytes: asyncio.Queue[bytes] = asyncio.Queue()
 
-    async def __aenter__(self):
+    def connect(self) -> Awaitable[None]:
         self._closed.clear()
-        self._connect_task.create()
-        return self
+        return self._connect_task.create()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         self._closing = True
         self._connect_task.cancel()
         self._receive_task.cancel()
+        self._received_bytes = asyncio.Queue()
         if self._transport:
             await self._notifier.emit(ConnectionClosed(None))
             self._transport.close()
+            self._transport = None
+            self._connected.clear()
             # Wait until `connection_lost` was called.
             try:
                 await asyncio.wait_for(self._closed.wait(), timeout=self._timeout)
             except asyncio.TimeoutError:
                 logger.error("timeout waiting for transport to close")
 
     async def _connect(self) -> None:
```

### Comparing `local_tuya-2.4.0/pyproject.toml` & `local_tuya-3.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "local_tuya"
-version = "2.4.0"
+version = "3.0.0"
 description = "Interface to Tuya devices over LAN."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/local-tuya"
 include = ["local_tuya/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
-pycryptodomex = ">=3,<4"
 concurrent-tasks = ">=1.6,<2"
+imbue = ">=2.1.1,<3"
+pycryptodomex = ">=3,<4"
 typing-extensions = ">=4.10"
 
 [tool.poetry.group.test.dependencies]
 pytest = "==8.1.1"
 pytest-asyncio = "==0.21.1"
 pytest-mock = "==3.14.0"
 ruff = "==0.4.4"
```

### Comparing `local_tuya-2.4.0/PKG-INFO` & `local_tuya-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: local_tuya
-Version: 2.4.0
+Version: 3.0.0
 Summary: Interface to Tuya devices over LAN.
 Home-page: https://github.com/gpajot/local-tuya
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: concurrent-tasks (>=1.6,<2)
+Requires-Dist: imbue (>=2.1.1,<3)
 Requires-Dist: pycryptodomex (>=3,<4)
 Requires-Dist: typing-extensions (>=4.10)
 Project-URL: Repository, https://github.com/gpajot/local-tuya
 Description-Content-Type: text/markdown
 
 # local-tuya
```

