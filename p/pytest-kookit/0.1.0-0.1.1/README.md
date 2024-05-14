# Comparing `tmp/pytest_kookit-0.1.0.tar.gz` & `tmp/pytest_kookit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_kookit-0.1.0.tar", max compression
+gzip compressed data, was "pytest_kookit-0.1.1.tar", max compression
```

## Comparing `pytest_kookit-0.1.0.tar` & `pytest_kookit-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       54 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/README.md
--rw-r--r--   0        0        0       49 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/__init__.py
--rw-r--r--   0        0        0     1401 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/client_side.py
--rw-r--r--   0        0        0       44 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/__init__.py
--rw-r--r--   0        0        0      799 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/interfaces.py
--rw-r--r--   0        0        0     3669 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/kookit.py
--rw-r--r--   0        0        0      214 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/__init__.py
--rw-r--r--   0        0        0      772 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/json_request.py
--rw-r--r--   0        0        0      597 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/json_response.py
--rw-r--r--   0        0        0     1721 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/request.py
--rw-r--r--   0        0        0     2747 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/response.py
--rw-r--r--   0        0        0      710 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/xml_response.py
--rw-r--r--   0        0        0     4463 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/response_group.py
--rw-r--r--   0        0        0     1603 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/server.py
--rw-r--r--   0        0        0     8022 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/service.py
--rw-r--r--   0        0        0     1372 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/interfaces.py
--rw-r--r--   0        0        0     2772 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/kookit.py
--rw-r--r--   0        0        0      230 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/logging.py
--rw-r--r--   0        0        0        0 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/py.typed
--rw-r--r--   0        0        0     1319 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/utils.py
--rw-r--r--   0        0        0     3416 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/README.md
+-rw-r--r--   0        0        0       49 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/__init__.py
+-rw-r--r--   0        0        0     1401 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/client_side.py
+-rw-r--r--   0        0        0       44 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/__init__.py
+-rw-r--r--   0        0        0      823 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/interfaces.py
+-rw-r--r--   0        0        0     3669 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/kookit.py
+-rw-r--r--   0        0        0      214 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/json_request.py
+-rw-r--r--   0        0        0      597 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/json_response.py
+-rw-r--r--   0        0        0     1721 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/request.py
+-rw-r--r--   0        0        0     2747 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/response.py
+-rw-r--r--   0        0        0      710 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/xml_response.py
+-rw-r--r--   0        0        0     4463 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/response_group.py
+-rw-r--r--   0        0        0     1695 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/server.py
+-rw-r--r--   0        0        0     8096 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/service.py
+-rw-r--r--   0        0        0     1372 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/interfaces.py
+-rw-r--r--   0        0        0     2772 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/kookit.py
+-rw-r--r--   0        0        0      230 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/logging.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/py.typed
+-rw-r--r--   0        0        0     1392 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/utils.py
+-rw-r--r--   0        0        0     3416 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.1.1/PKG-INFO
```

### Comparing `pytest_kookit-0.1.0/kookit/client_side.py` & `pytest_kookit-0.1.1/kookit/client_side.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/interfaces.py` & `pytest_kookit-0.1.1/kookit/http_kookit/interfaces.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, Protocol
+from typing import TYPE_CHECKING, Any, Callable, Protocol
 
 
 if TYPE_CHECKING:
     from collections.abc import Iterable, Mapping
 
     from fastapi import APIRouter
     from httpx import URL
@@ -28,13 +28,13 @@
     def path_params(self) -> dict: ...
 
 
 class IServer(Protocol):
     def wait(self, timeout: float | None = None) -> Any: ...
     def run(
         self,
-        routers: Iterable[APIRouter],
+        routers: Iterable[Callable[[], APIRouter]],
         lifespans: Iterable[ILifespan],
     ) -> None: ...
 
     @property
     def url(self) -> str: ...
```

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/kookit.py` & `pytest_kookit-0.1.1/kookit/http_kookit/kookit.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/models/json_request.py` & `pytest_kookit-0.1.1/kookit/http_kookit/models/json_request.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/models/json_response.py` & `pytest_kookit-0.1.1/kookit/http_kookit/models/json_response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/models/request.py` & `pytest_kookit-0.1.1/kookit/http_kookit/models/request.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/models/response.py` & `pytest_kookit-0.1.1/kookit/http_kookit/models/response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/models/xml_response.py` & `pytest_kookit-0.1.1/kookit/http_kookit/models/xml_response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/response_group.py` & `pytest_kookit-0.1.1/kookit/http_kookit/response_group.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/server.py` & `pytest_kookit-0.1.1/kookit/http_kookit/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 from contextlib import asynccontextmanager
-from typing import Any, AsyncIterator, Final, Iterable
+from typing import TYPE_CHECKING, Any, Final
 
 import uvicorn
 from fastapi import APIRouter, FastAPI
 from multiprocess import Queue
 
 from kookit.logging import logger
 from kookit.utils import ILifespan, Lifespans
 
 
+if TYPE_CHECKING:
+    from collections.abc import AsyncIterator, Callable, Iterable
+
+
 class KookitHTTPServer:
     def __init__(self, port: int, *, host: str = "127.0.0.1") -> None:
         self.queue: Final = Queue()
         self.host: Final[str] = host
         self.port: Final[int] = port
         self.url: Final[str] = f"http://{host}:{port}"
 
@@ -21,29 +25,29 @@
         return "[KookitHTTPServer]"
 
     def wait(self, timeout: float | None = None) -> Any:
         return self.queue.get(timeout=timeout)
 
     def run(
         self,
-        routers: Iterable[APIRouter],
+        routers: Iterable[Callable[[], APIRouter]],
         lifespans: Iterable[ILifespan],
     ) -> None:
         @asynccontextmanager
         # ruff: noqa: ARG001
         async def notify_lifespan(app: FastAPI) -> AsyncIterator:
             # ruff: noqa: FBT003
             self.queue.put(True)
             yield
             self.queue.put(False)
 
         @asynccontextmanager
         async def routers_lifespan(app: FastAPI) -> AsyncIterator:
             for router in routers:
-                app.include_router(router)
+                app.include_router(router())
             yield
 
         app: FastAPI = FastAPI(
             lifespan=Lifespans(
                 *lifespans,
                 routers_lifespan,
                 notify_lifespan,
```

### Comparing `pytest_kookit-0.1.0/kookit/http_kookit/service.py` & `pytest_kookit-0.1.1/kookit/http_kookit/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,27 +103,28 @@
 
     def add_lifespans(self, *lifespans: ILifespan) -> None:
         self.lifespans.extend(lifespans)
 
     def add_routers(self, *routers: APIRouter) -> None:
         self.routers.extend(routers)
 
-    @property
     def router(self) -> APIRouter:
         router = APIRouter()
         for r in self.routers:
             router.include_router(r)
 
         for group in self._response_groups:
             if group.response:
                 router.add_api_route(
                     group.path,
                     self.__call__,
                     methods=[group.method],
                 )
+
+        logger.trace(f"{self}: routes: {chr(10).join(str(r) for r in router.routes)}")
         return router
 
     @property
     def lifespan(self) -> ILifespan:
         return Lifespans(*self.lifespans)
 
     def start(self, *, wait_for_start_timeout: float | None = None) -> None:
```

### Comparing `pytest_kookit-0.1.0/kookit/interfaces.py` & `pytest_kookit-0.1.1/kookit/interfaces.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/kookit.py` & `pytest_kookit-0.1.1/kookit/kookit.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.0/kookit/utils.py` & `pytest_kookit-0.1.1/kookit/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 import contextlib
 import json
+import sys
 from contextlib import AbstractAsyncContextManager, asynccontextmanager
 from traceback import extract_stack
-from typing import TYPE_CHECKING, Any, Protocol
+from typing import TYPE_CHECKING, Any, Callable
 from uuid import UUID
 
 
 if TYPE_CHECKING:
     from collections.abc import AsyncIterator
 
-
-class ILifespan(Protocol):
-    def __call__(self, app: Any) -> AbstractAsyncContextManager[None]: ...
+if sys.version_info >= (3, 9):
+    ILifespan = Callable[[Any], AbstractAsyncContextManager[None]]
+else:
+    ILifespan = Callable[[Any], AbstractAsyncContextManager]
 
 
 class Lifespans:
     def __init__(
         self,
         *lifespans: ILifespan,
     ) -> None:
```

### Comparing `pytest_kookit-0.1.0/pyproject.toml` & `pytest_kookit-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "pytest-kookit"
-version = "0.1.0"
+version = "0.1.1"
 description = "Your simple but kooky integration testing with pytest"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pytest_kookit-0.1.0/PKG-INFO` & `pytest_kookit-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-kookit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Your simple but kooky integration testing with pytest
 License: MIT
 Keywords: Integration Testing,External Services' mocks
 Author: Dmitry Makarov
 Author-email: mit.makaroff@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Intended Audience :: Developers
```

