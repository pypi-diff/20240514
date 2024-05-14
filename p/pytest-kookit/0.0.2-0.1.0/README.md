# Comparing `tmp/pytest_kookit-0.0.2.tar.gz` & `tmp/pytest_kookit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_kookit-0.0.2.tar", max compression
+gzip compressed data, was "pytest_kookit-0.1.0.tar", max compression
```

## Comparing `pytest_kookit-0.0.2.tar` & `pytest_kookit-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,22 @@
--rw-r--r--   0        0        0       54 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/README.md
--rw-r--r--   0        0        0       75 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/__init__.py
--rw-r--r--   0        0        0      214 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/__init__.py
--rw-r--r--   0        0        0      703 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/json_request.py
--rw-r--r--   0        0        0      575 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/json_response.py
--rw-r--r--   0        0        0     1508 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/request.py
--rw-r--r--   0        0        0     2381 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/response.py
--rw-r--r--   0        0        0      688 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/xml_response.py
--rw-r--r--   0        0        0      241 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/__init__.py
--rw-r--r--   0        0        0     1624 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/actions_parser.py
--rw-r--r--   0        0        0     3514 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/http_handler.py
--rw-r--r--   0        0        0     1216 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/interfaces.py
--rw-r--r--   0        0        0     2472 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/request_runner.py
--rw-r--r--   0        0        0     1329 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/requests_diff.py
--rw-r--r--   0        0        0     3244 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/service.py
--rw-r--r--   0        0        0      230 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/logging.py
--rw-r--r--   0        0        0       62 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/__init__.py
--rw-r--r--   0        0        0     1542 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/client_side.py
--rw-r--r--   0        0        0       68 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/__init__.py
--rw-r--r--   0        0        0      572 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/interfaces.py
--rw-r--r--   0        0        0     3416 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/kookit.py
--rw-r--r--   0        0        0      945 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/server.py
--rw-r--r--   0        0        0      435 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/interfaces.py
--rw-r--r--   0        0        0     2146 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/kookit.py
--rw-r--r--   0        0        0        0 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/py.typed
--rw-r--r--   0        0        0     3492 2024-05-06 14:56:54.694275 pytest_kookit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/README.md
+-rw-r--r--   0        0        0       49 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/__init__.py
+-rw-r--r--   0        0        0     1401 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/client_side.py
+-rw-r--r--   0        0        0       44 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/interfaces.py
+-rw-r--r--   0        0        0     3669 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/kookit.py
+-rw-r--r--   0        0        0      214 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/json_request.py
+-rw-r--r--   0        0        0      597 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/json_response.py
+-rw-r--r--   0        0        0     1721 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/request.py
+-rw-r--r--   0        0        0     2747 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/response.py
+-rw-r--r--   0        0        0      710 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/models/xml_response.py
+-rw-r--r--   0        0        0     4463 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/response_group.py
+-rw-r--r--   0        0        0     1603 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/server.py
+-rw-r--r--   0        0        0     8022 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/http_kookit/service.py
+-rw-r--r--   0        0        0     1372 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/interfaces.py
+-rw-r--r--   0        0        0     2772 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/kookit.py
+-rw-r--r--   0        0        0      230 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/logging.py
+-rw-r--r--   0        0        0        0 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/py.typed
+-rw-r--r--   0        0        0     1319 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/kookit/utils.py
+-rw-r--r--   0        0        0     3416 2024-05-14 06:40:30.182574 pytest_kookit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.1.0/PKG-INFO
```

### Comparing `pytest_kookit-0.0.2/kookit/http_models/json_response.py` & `pytest_kookit-0.1.0/kookit/http_kookit/models/json_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import Any, Mapping, Optional
+from __future__ import annotations
+from typing import Any, Mapping
 
 from .response import KookitHTTPResponse
 
 
 class KookitJSONResponse(KookitHTTPResponse):
     def __init__(
         self,
         json: Any,
         *,
         url: str = "/",
         method: str = "GET",
         status_code: int = 200,
-        headers: Optional[Mapping] = None,
+        headers: Mapping | None = None,
         **request_matchers: Any,
     ) -> None:
         super().__init__(
             json=json,
             status_code=status_code,
             method=method,
             headers=headers,
```

### Comparing `pytest_kookit-0.0.2/kookit/http_models/request.py` & `pytest_kookit-0.1.0/kookit/http_kookit/models/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,57 @@
-from typing import Any, Final, Mapping, Optional, Protocol, Union
+from __future__ import annotations
+from json import dumps as json_dumps
+from json import loads as json_loads
+from typing import TYPE_CHECKING, Any, Final, Mapping, Protocol
 
 from httpx import URL, Request
-from httpx._types import HeaderTypes, QueryParamTypes, RequestContent, RequestData, RequestFiles
+
+from kookit.utils import UUIDEncoder
+
+
+if TYPE_CHECKING:
+    from httpx._types import (
+        HeaderTypes,
+        QueryParamTypes,
+        RequestContent,
+        RequestData,
+        RequestFiles,
+    )
 
 
 class IKookitService(Protocol):
     @property
-    def service_url(self) -> str:
-        ...
+    def url(self) -> str: ...
 
 
 class KookitHTTPRequest:
     def __init__(
         self,
         service: IKookitService,
         *,
-        url: Union[URL, str],
-        method: Union[str, bytes],
-        params: Optional[QueryParamTypes] = None,
-        headers: Optional[HeaderTypes] = None,
-        content: Optional[RequestContent] = None,
-        data: Optional[RequestData] = None,
-        files: Optional[RequestFiles] = None,
-        json: Optional[Any] = None,
+        url: URL | str,
+        method: str | bytes,
+        params: QueryParamTypes | None = None,
+        headers: HeaderTypes | None = None,
+        content: RequestContent | None = None,
+        data: RequestData | None = None,
+        files: RequestFiles | None = None,
+        json: Any | None = None,
         request_delay: float = 0.0,
     ) -> None:
         self.service: Final[IKookitService] = service
         request: Request = Request(
             url=url,
             method=method,
             params=params,
             headers=headers,
             content=content,
             data=data,
             files=files,
-            json=json,
+            json=json_loads(json_dumps(json, cls=UUIDEncoder)),
         )
         self.url: Final[URL] = request.url
         self.method: Final[str] = request.method
         self.content: Final[bytes] = request.content
         self.headers: Mapping[str, str] = request.headers
         self.request_delay: Final[float] = request_delay
```

### Comparing `pytest_kookit-0.0.2/kookit/http_models/response.py` & `pytest_kookit-0.1.0/kookit/http_kookit/models/response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,85 @@
+from __future__ import annotations
 from dataclasses import dataclass
-from typing import Any, Final, Mapping, Optional, Union
+from json import dumps as json_dumps
+from json import loads as json_loads
+from typing import TYPE_CHECKING, Any, Final, Mapping
 
 from httpx import URL, Request, Response
-from httpx._types import HeaderTypes, QueryParamTypes, RequestContent, RequestData, RequestFiles
+
+from kookit.utils import UUIDEncoder
+
+
+if TYPE_CHECKING:
+    from httpx._types import (
+        HeaderTypes,
+        QueryParamTypes,
+        RequestContent,
+        RequestData,
+        RequestFiles,
+    )
 
 
 @dataclass
 class KookitResponseRequest:
     content: bytes
-    headers: Optional[Mapping[str, str]]
+    headers: Mapping[str, str] | None
     url: URL
     method: str
 
 
 class KookitHTTPResponse:
     def __init__(
         self,
-        url: Union[URL, str],
-        method: Union[str, bytes],
+        url: URL | str,
+        method: str | bytes,
         *,
         status_code: int = 200,
         http_version: str = "HTTP/1.1",
-        headers: Optional[Mapping] = None,
-        content: Optional[bytes] = None,
-        text: Optional[str] = None,
-        html: Optional[str] = None,
+        headers: Mapping | None = None,
+        content: bytes | None = None,
+        text: str | None = None,
+        html: str | None = None,
         json: Any = None,
         stream: Any = None,
         # Request matchers here
-        request_params: Optional[QueryParamTypes] = None,
-        request_headers: Optional[HeaderTypes] = None,
-        request_content: Optional[RequestContent] = None,
-        request_data: Optional[RequestData] = None,
-        request_files: Optional[RequestFiles] = None,
-        request_json: Optional[Any] = None,
+        request_params: QueryParamTypes | None = None,
+        request_headers: HeaderTypes | None = None,
+        request_content: RequestContent | None = None,
+        request_data: RequestData | None = None,
+        request_files: RequestFiles | None = None,
+        request_json: Any | None = None,
     ) -> None:
         request = Request(
             url=url,
             method=method,
             params=request_params,
             headers=request_headers,
             content=request_content,
             data=request_data,
             files=request_files,
-            json=request_json,
+            json=json_loads(json_dumps(request_json, cls=UUIDEncoder)),
         )
+        if request_headers:
+            request_headers = request.headers  # lowercase headers' keys
         response: Response = Response(
             status_code=status_code,
             extensions={"http_version": http_version.encode("ascii")},
             headers=headers,
-            json=json,
+            json=json_loads(json_dumps(json, cls=UUIDEncoder)),
             content=content,
             text=text,
             html=html,
             stream=stream,
             request=request,
         )
 
         self.request: Final[KookitResponseRequest] = KookitResponseRequest(
             content=request.content,
-            headers=request_headers,  # type: ignore
+            headers=request_headers,  # type: ignore[arg-type]
             url=request.url,
             method=request.method,
         )
 
         self.content: Final[bytes] = response.content
         self.headers: Final[Mapping[str, str]] = response.headers
         self.status_code: Final[int] = response.status_code
```

### Comparing `pytest_kookit-0.0.2/kookit/http_models/xml_response.py` & `pytest_kookit-0.1.0/kookit/http_kookit/models/xml_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import Any, Mapping, Optional
+from __future__ import annotations
+from typing import Any, Mapping
 
 from .response import KookitHTTPResponse
 
 
 class KookitXMLResponse(KookitHTTPResponse):
     def __init__(
         self,
         xml: Any,
         *,
         url: str = "/",
         method: str = "GET",
         status_code: int = 200,
-        headers: Optional[Mapping] = None,
+        headers: Mapping | None = None,
         **request_matchers: Any,
     ) -> None:
         headers = headers or {}
         headers = dict(headers)
         headers["content-type"] = "application/xml"
         super().__init__(
             text=xml,
```

### Comparing `pytest_kookit-0.0.2/kookit/main/client_side.py` & `pytest_kookit-0.1.0/kookit/client_side.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from typing import Any, Protocol
 
-from httpx import AsyncClient, Response
+from httpx import Client, Response
 
 
 class IKookitService(Protocol):
     @property
-    def service_url(self) -> str:
-        ...
+    def url(self) -> str: ...
 
 
-class KookitHTTPAsyncClient:
-    async def request(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        async with AsyncClient(base_url=service.service_url) as client:
-            return await client.request(*args, **kwargs)
+class KookitHTTPClient:
+    def request(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        with Client(base_url=service.url) as client:
+            return client.request(*args, **kwargs)
 
-    async def get(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        return await self.request(service, "GET", *args, **kwargs)
+    def get(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        return self.request(service, "GET", *args, **kwargs)
 
-    async def post(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        return await self.request(service, "POST", *args, **kwargs)
+    def post(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        return self.request(service, "POST", *args, **kwargs)
 
-    async def put(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        return await self.request(service, "PUT", *args, **kwargs)
+    def put(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        return self.request(service, "PUT", *args, **kwargs)
 
-    async def delete(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        return await self.request(service, "DELETE", *args, **kwargs)
+    def delete(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        return self.request(service, "DELETE", *args, **kwargs)
 
-    async def options(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        return await self.request(service, "OPTIONS", *args, **kwargs)
+    def options(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        return self.request(service, "OPTIONS", *args, **kwargs)
 
-    async def patch(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        return await self.request(service, "PATCH", *args, **kwargs)
+    def patch(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        return self.request(service, "PATCH", *args, **kwargs)
 
-    async def head(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
-        return await self.request(service, "HEAD", *args, **kwargs)
+    def head(self, service: IKookitService, *args: Any, **kwargs: Any) -> Response:
+        return self.request(service, "HEAD", *args, **kwargs)
```

### Comparing `pytest_kookit-0.0.2/kookit/main/http_kookit/kookit.py` & `pytest_kookit-0.1.0/kookit/http_kookit/kookit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,122 @@
+from __future__ import annotations
 import os
 import queue
+import time
 from contextlib import suppress
 from itertools import cycle
-from typing import Any, Final, List, Optional
+from typing import TYPE_CHECKING, Final, Iterable
 
-from multiprocess import Process, Queue
-from pytest_mock import MockerFixture
+from multiprocess import Process
+from typing_extensions import Self
 
 from kookit.logging import logger
-from .interfaces import IKookitHTTPService, http_service
 from .server import KookitHTTPServer
+from .service import KookitHTTPService
+
+
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from fastapi import APIRouter
+    from pytest_mock import MockerFixture
+
+    from kookit.utils import ILifespan
+    from .models import KookitHTTPRequest, KookitHTTPResponse
+
+
+__all__ = ["HTTPKookit"]
 
 
 class HTTPKookit:
     server_port: Final[cycle] = cycle(i for i in range(29000, 30000))
 
     def __init__(self, mocker: MockerFixture) -> None:
         self.mocker: Final[MockerFixture] = mocker
-        self.server_queue: Final[Queue] = Queue()
-        self.server: Final[KookitHTTPServer] = KookitHTTPServer(
-            self.server_queue,
-            port=next(self.server_port),
-        )
-        self.services: Final[List[IKookitHTTPService]] = []
-        self.server_process: Optional[Process] = None
-        super().__init__()
+        self.server: Final[KookitHTTPServer] = KookitHTTPServer(next(self.server_port))
+        self.services: Final[list[KookitHTTPService]] = []
+        self.server_process: Process | None = None
 
     def __str__(self) -> str:
         return "[HTTPKookit]"
 
-    async def prepare_services(self, *services: Any) -> List[Any]:
-        assert not self.services, "You can only add services once"
-        logger.trace(f"{self}: preparing {len(services)} services: {services}")
-        self.services.extend((service for service in services if http_service(service)))
-        for service in self.services:
-            if not service.service_url:
-                service.service_url = self.server.url
-
-        envs = {**os.environ}
-        envs.update({s.url_env_var: s.service_url for s in services if s.url_env_var})
-        envs.update()
-        self.mocker.patch.dict(os.environ, envs)
-        return [service for service in services if not http_service(service)]
-
-    async def start_services(
+    def new_service(
         self,
-        **kwargs: Any,
-    ) -> None:
-        assert not self.server_process
-        self.server_process = Process(
-            target=self.server.run,
-            args=(self.services,),
+        env_var: str,
+        *,
+        unique_url: bool,
+        actions: Iterable[KookitHTTPRequest | KookitHTTPResponse] = (),
+        routers: Iterable[APIRouter] = (),
+        lifespans: Iterable[ILifespan] = (),
+        name: str = "",
+    ) -> KookitHTTPService:
+        server = self.server
+        if unique_url:
+            server = KookitHTTPServer(
+                next(self.server_port),
+            )
+
+        if env_var:
+            self.mocker.patch.dict(os.environ, {env_var: server.url})
+        service = KookitHTTPService(
+            server=server,
+            actions=actions,
+            routers=routers,
+            lifespans=lifespans,
+            unique_url=unique_url,
+            name=name,
         )
-        logger.trace(f"{self}: starting server process")
-        self.server_process.start()
+        self.services.append(service)
+        return service
 
-        wait_for_server_launch: Optional[float] = kwargs.get("http_wait_for_server_launch")
-        with suppress(queue.Empty):
-            assert self.server_queue.get(timeout=wait_for_server_launch)
+    def __enter__(self) -> Self:
+        # 1. start global server
+        # 2. start all other services' servers.
+        not_unique = [s for s in self.services if not s.unique_url]
+
+        if not_unique and not self.server_process:
+            self.server_process = Process(
+                target=self.server.run,
+                args=(
+                    [s.router for s in not_unique],
+                    [s.lifespan for s in not_unique],
+                ),
+            )
+            self.server_process.start()
+            time.sleep(0.01)
+
+            with suppress(queue.Empty):
+                is_started = self.server.wait()
+                if not is_started:
+                    msg = f"{self}: bad value received from server while starting"
+                    raise ValueError(msg)
 
-        logger.trace(f"{self}: running services")
         for service in self.services:
-            await service.run()
+            service.__enter__()
+
+        return self
 
-    async def stop_services(self, **kwargs: Any) -> None:
-        logger.trace(f"{self}: stopping services")
+    def __exit__(
+        self,
+        typ: type[BaseException] | None,
+        exc: BaseException | None,
+        tb: TracebackType | None,
+    ) -> None:
+        # 1. stop global service
+        # 2. stop all other services' servers
         if self.server_process:
+            logger.trace(f"{self}: stop server process ({self.server.url})")
             self.server_process.terminate()
+            time.sleep(0.01)
+
             self.server_process = None
 
-        try:
-            await self.assert_completed(self.services, local_url=self.server.url)
-        finally:
-            self.services.clear()
-
-        wait_for_server_stop: Optional[float] = kwargs.get("http_wait_for_server_stop")
-        with suppress(queue.Empty):
-            assert not self.server_queue.get(timeout=wait_for_server_stop)
-
-    @staticmethod
-    async def assert_completed(
-        services: List[IKookitHTTPService],
-        local_url: str,
-    ) -> None:
-        service_unused_responses: dict = {
-            service: service.unused_responses() for service in services
-        }
-        logger.debug(f"[kookit]: services' unused responses: {service_unused_responses}")
-        assert not any(
-            responses
-            for service, responses in service_unused_responses.items()
-            if service.service_url == local_url
-        ), service_unused_responses
+            with suppress(queue.Empty):
+                is_started: bool = self.server.wait()
+                if is_started:
+                    msg = f"{self}: bad value received from server while stopping"
+                    raise ValueError(msg)
+        else:
+            logger.trace(f"{self}: server process already stopped")
+
+        for service in self.services:
+            service.__exit__(typ, exc, tb)
```

### Comparing `pytest_kookit-0.0.2/pyproject.toml` & `pytest_kookit-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-target-version = ["py310"]
-include = '\.pyi?$'
-skip-string-normalization = true
-exclude = '''
-(
-  /(
-    | \.git
-    | \.mypy_cache
-  )/
-)
-'''
-
-[tool.isort]
-line_length = 99
-sections = ['FUTURE', 'STDLIB', 'THIRDPARTY', 'FIRSTPARTY', 'LOCALFOLDER']
-no_lines_before = ['STDLIB', 'LOCALFOLDER']
-known_third_party = [
-    'pytest',
-]
-known_local_folder = []
-multi_line_output = 3
-lines_after_imports = 2
-include_trailing_comma = true
-use_parentheses= true
-
 
 [tool.poetry]
 name = "pytest-kookit"
-version = "0.0.2"
+version = "0.1.0"
 description = "Your simple but kooky integration testing with pytest"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -62,96 +35,132 @@
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/Mityuha/pytest-kookit/releases"
 "Source" = "https://github.com/Mityuha/pytest-kookit"
 "Tracker" = "https://github.com/Mityuha/pytest-kookit/issues"
 
 [tool.poetry.plugins."pytest11"]
-"kookit" = "kookit.main"
+"kookit" = "kookit"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 multiprocess = "*"
 fastapi = ">=0.69.0"
 uvicorn = "*"
 httpx = "*"
 pytest-mock = "*"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
-ruff = "^0.1.4"
-black = "^23.10.1"
-pydocstringformatter = [
-    {version = "^0.7.3", python = ">=3.8"},
-]
-isort = "^5.12.0"
-mypy = "^1.5.1"
-pre-commit = "^3.5.0"
-pytest-cov = "^4.1.0"
-pytest-asyncio = "^0.21.1"
-autoflake = "^2.2.1"
-types-dataclasses = "^0.6.6"
-sort-all = "^1.2.0"
-tox = "^4.11.3"
-faker = "^19.13.0"
-requests = "^2.31.0"
-pytest-httpx = "0.22.0"
+pytest = "*"
+ruff = "*"
+mypy = "*"
+pre-commit = "*"
+pytest-cov = "*"
+pytest-asyncio = "*"
+autoflake = "*"
+types-dataclasses = "*"
+sort-all = "*"
+tox = "*"
+faker = "*"
+requests = "*"
+pytest-httpx = "*"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 xfail_strict = "true"
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/stable/config_file.html
 python_version = "3.10"
 exclude = []
 warn_unused_configs = true
 ignore_missing_imports = true
 disallow_incomplete_defs = true
 
 [tool.ruff]
+exclude = [
+    ".git", 
+    ".mypy_cache",
+    ".pytest_cache",
+]
 line-length = 99
+fix = true
+unsafe-fixes = true
+show-fixes = true
+
+[tool.ruff.lint]
+ignore = [
+    "D100",
+    "D101",
+    "D102",
+    "D103",
+    "D104",
+    "D105",
+    "D107",
+    "ANN101",
+    "ANN401",
+    "PLR0913",
+    "ISC001",
+    "D203",
+    "D213",
+    "COM812",
+]
+select = ["ALL"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
-
+"tests/*py" = [
+    "ANN001",
+    "ANN002",
+    "ANN003",
+    "ANN401",
+    "PLR2004",
+    "S101",
+    "S311",
+    "FBT001",
+]
+
+[tool.ruff.format]
+docstring-code-format = true
+
+[tool.ruff.lint.isort]
+no-lines-before = ["standard-library", "local-folder"]
+known-third-party = ["pytest"]
+known-local-folder = []
+lines-after-imports = 2
 
 [tool.coverage]
 [tool.coverage.run]
 omit = [
     '__init__.py',
 ]
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
 envlist = py38,py39,py310,py311,py312
 
 [testenv]
 deps =
-    black==22.8.0
-    isort==5.10.1
-    mypy==1.5.1
-    ruff==0.1.4
+    mypy==1.10.0
+    ruff==0.4.4
 
-    multiprocess==0.70.15
+    multiprocess==0.70.16
     fastapi==0.98.0
     uvicorn==0.23.2
     httpx==0.24.1
     pytest==7.4.3
     pytest-mock==3.12.0
     requests==2.31.0
     faker==19.13.0
     pytest-httpx==0.22.0
     pytest-asyncio==0.21.1
 
 commands = 
-    black --check kookit/ tests/
-    isort --check kookit tests/
-    ruff check kookit/ tests/
+    ruff check --no-fix kookit/ tests/ 
     mypy kookit/ tests/ 
     pytest tests/ -x
 setenv =
     PIP_INDEX_URL = {env:PIP_INDEX_URL:https://pypi.org/simple/}
 
 [gh-actions]
 python =
```

### Comparing `pytest_kookit-0.0.2/PKG-INFO` & `pytest_kookit-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-kookit
-Version: 0.0.2
+Version: 0.1.0
 Summary: Your simple but kooky integration testing with pytest
 License: MIT
 Keywords: Integration Testing,External Services' mocks
 Author: Dmitry Makarov
 Author-email: mit.makaroff@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Intended Audience :: Developers
```

