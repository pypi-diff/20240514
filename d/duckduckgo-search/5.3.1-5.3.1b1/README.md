# Comparing `tmp/duckduckgo_search-5.3.1.tar.gz` & `tmp/duckduckgo_search-5.3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-5.3.1.tar", last modified: Wed May  8 21:44:30 2024, max compression
+gzip compressed data, was "duckduckgo_search-5.3.1b1.tar", last modified: Wed May  8 22:26:37 2024, max compression
```

## Comparing `duckduckgo_search-5.3.1.tar` & `duckduckgo_search-5.3.1b1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:44:30.138342 duckduckgo_search-5.3.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-05-08 21:44:30.138342 duckduckgo_search-5.3.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    16861 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:44:30.134341 duckduckgo_search-5.3.1/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16588 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    42719 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:44:30.138342 duckduckgo_search-5.3.1/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-05-08 21:44:30.000000 duckduckgo_search-5.3.1/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-08 21:44:30.000000 duckduckgo_search-5.3.1/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:44:30.000000 duckduckgo_search-5.3.1/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 21:44:30.000000 duckduckgo_search-5.3.1/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 21:44:30.000000 duckduckgo_search-5.3.1/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 21:44:30.000000 duckduckgo_search-5.3.1/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 21:44:30.138342 duckduckgo_search-5.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:44:30.138342 duckduckgo_search-5.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-08 21:44:19.000000 duckduckgo_search-5.3.1/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.980471 duckduckgo_search-5.3.1b1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-05-08 22:26:37.980471 duckduckgo_search-5.3.1b1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.976471 duckduckgo_search-5.3.1b1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      765 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42757 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13366 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.976471 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:26:37.980471 duckduckgo_search-5.3.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.976471 duckduckgo_search-5.3.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-5.3.1/LICENSE.md` & `duckduckgo_search-5.3.1b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.1/PKG-INFO` & `duckduckgo_search-5.3.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.1
+Version: 5.3.1b1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -19,18 +19,19 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.7.0b4
-Requires-Dist: orjson>=3.10.3
+Requires-Dist: httpx[brotli,http2,socks]>=0.27.0
 Provides-Extra: lxml
 Requires-Dist: lxml>=5.2.1; extra == "lxml"
+Provides-Extra: orjson
+Requires-Dist: orjson>=3.10.3; extra == "orjson"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: ruff>=0.4.3; extra == "dev"
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search)](https://pepy.tech/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search/week)](https://pepy.tech/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
@@ -57,18 +58,14 @@
 * [7. translate() - translation](#7-translate---translation-by-duckduckgocom)
 * [8. suggestions() - suggestions](#8-suggestions---suggestions-by-duckduckgocom)
 
 ## Install
 ```python
 pip install -U duckduckgo_search
 ```
-There is also a beta release that uses the `httpx` library:
-```python
-pip install -U duckduckgo_search==5.3.0b4
-```
 > [!NOTE]
 > you can install lxml to use the `text` function with `backend='html'` or `backend='lite'` (size ≈ 12Mb)</br>
 > `pip install -U duckduckgo_search[lxml]`
 
 ## CLI version
 
 ```python3
```

### Comparing `duckduckgo_search-5.3.1/README.md` & `duckduckgo_search-5.3.1b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,14 @@
 * [7. translate() - translation](#7-translate---translation-by-duckduckgocom)
 * [8. suggestions() - suggestions](#8-suggestions---suggestions-by-duckduckgocom)
 
 ## Install
 ```python
 pip install -U duckduckgo_search
 ```
-There is also a beta release that uses the `httpx` library:
-```python
-pip install -U duckduckgo_search==5.3.0b4
-```
 > [!NOTE]
 > you can install lxml to use the `text` function with `backend='html'` or `backend='lite'` (size ≈ 12Mb)</br>
 > `pip install -U duckduckgo_search[lxml]`
 
 ## CLI version
 
 ```python3
```

### Comparing `duckduckgo_search-5.3.1/duckduckgo_search/cli.py` & `duckduckgo_search-5.3.1b1/duckduckgo_search/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from urllib.parse import unquote
 
 import click
-from curl_cffi import requests
+import httpx
 
 from .duckduckgo_search import DDGS
-from .utils import json_dumps
+from .utils import _get_ssl_context, json_dumps
 from .version import __version__
 
 logger = logging.getLogger(__name__)
 
 COLORS = {
     0: "black",
     1: "red",
@@ -77,20 +77,20 @@
         .replace(" ", "")
     )
     return keywords
 
 
 def _download_file(url, dir_path, filename, proxy):
     try:
-        resp = requests.get(url, proxy=proxy, impersonate="chrome", timeout=10)
+        resp = httpx.get(url, proxy=proxy, timeout=10, follow_redirects=True, verify=_get_ssl_context())
         resp.raise_for_status()
         with open(os.path.join(dir_path, filename[:200]), "wb") as file:
             file.write(resp.content)
     except Exception as ex:
-        logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
+        logger.info(f"download_file url={url} {type(ex).__name__} {ex}")
 
 
 def _download_results(keywords, results, images=False, proxy=None, threads=None):
     path_type = "images" if images else "text"
     path = f"{path_type}_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     os.makedirs(path, exist_ok=True)
```

### Comparing `duckduckgo_search-5.3.1/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-5.3.1b1/duckduckgo_search/duckduckgo_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Awaitable, Dict, Optional, Type, Union
 
 from .duckduckgo_search_async import AsyncDDGS
 
 
 class DDGS(AsyncDDGS):
     _loop: asyncio.AbstractEventLoop = asyncio.new_event_loop()
-    Thread(target=_loop.run_forever, daemon=True).start()  # Start the event loop run in a separate thread.
+    Thread(target=_loop.run_forever, daemon=True).start()  # Start the event loop in a separate thread.
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         proxy: Optional[str] = None,
         proxies: Union[Dict[str, str], str, None] = None,  # deprecated
         timeout: Optional[int] = 10,
@@ -40,16 +40,16 @@
         self._close_session()
 
     def __del__(self) -> None:
         self._close_session()
 
     def _close_session(self) -> None:
         """Close the curl-cffi async session."""
-        if hasattr(self, "_asession") and self._asession._closed is False:
-            self._run_async_in_thread(self._asession.close())  # type: ignore
+        if hasattr(self, "_aclient") and self._aclient.is_closed is False:
+            self._run_async_in_thread(self._aclient.aclose())
 
     def _run_async_in_thread(self, coro: Awaitable[Any]) -> Any:
         """Runs an async coroutine in a separate thread."""
         future: Future[Any] = asyncio.run_coroutine_threadsafe(coro, self._loop)
         result = future.result()
         return result
```

### Comparing `duckduckgo_search-5.3.1/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-5.3.1b1/duckduckgo_search/duckduckgo_search_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import suppress
 from datetime import datetime, timezone
 from decimal import Decimal
 from functools import cached_property, partial
 from itertools import cycle, islice
 from types import TracebackType
-from typing import Dict, List, Optional, Tuple, Type, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
-from curl_cffi import requests
+import httpx
 
 try:
+    from lxml.html import Element, document_fromstring
     from lxml.html import HTMLParser as LHTMLParser
-    from lxml.html import document_fromstring
 
     LXML_AVAILABLE = True
 except ImportError:
     LXML_AVAILABLE = False
 
 from .exceptions import DuckDuckGoSearchException, RatelimitException, TimeoutException
 from .utils import (
     _calculate_distance,
     _extract_vqd,
+    _get_headers,
+    _get_ssl_context,
     _normalize,
     _normalize_url,
     _text_extract_json,
     json_loads,
 )
 
 logger = logging.getLogger("duckduckgo_search.AsyncDDGS")
@@ -54,75 +56,77 @@
             timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
         """
         self.proxy: Optional[str] = proxy
         assert self.proxy is None or isinstance(self.proxy, str), "proxy must be a str"
         if not proxy and proxies:
             warnings.warn("'proxies' is deprecated, use 'proxy' instead.", stacklevel=1)
             self.proxy = proxies.get("http") or proxies.get("https") if isinstance(proxies, dict) else proxies
-        self._asession = requests.AsyncSession(
-            headers=headers,
+        self._aclient = httpx.AsyncClient(
+            headers=_get_headers() if headers is None else headers,
             proxy=self.proxy,
             timeout=timeout,
-            impersonate="chrome",
-            allow_redirects=False,
+            follow_redirects=False,
+            http2=True,
+            verify=_get_ssl_context(),
         )
-        self._asession.headers["Referer"] = "https://duckduckgo.com/"
+        self._aclient.headers["Referer"] = "https://duckduckgo.com/"
         self._exception_event = asyncio.Event()
 
     async def __aenter__(self) -> "AsyncDDGS":
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        await self._asession.__aexit__(exc_type, exc_val, exc_tb)  # type: ignore
+        await self._aclient.__aexit__(exc_type, exc_val, exc_tb)
 
     def __del__(self) -> None:
-        if hasattr(self, "_asession") and self._asession._closed is False:
+        if hasattr(self, "_aclient") and self._aclient.is_closed is False:
             with suppress(RuntimeError, RuntimeWarning):
-                asyncio.create_task(self._asession.close())  # type: ignore
+                asyncio.create_task(self._aclient.aclose())
 
     @cached_property
-    def parser(self) -> Optional["LHTMLParser"]:
+    def parser(self) -> "LHTMLParser":
         """Get HTML parser."""
         return LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
 
     @classmethod
     def _get_executor(cls, max_workers: int = 1) -> ThreadPoolExecutor:
         """Get ThreadPoolExecutor. Default max_workers=1, because >=2 leads to a big overhead"""
         if cls._executor is None:
             cls._executor = ThreadPoolExecutor(max_workers=max_workers)
         return cls._executor
 
     @property
-    def executor(cls) -> Optional[ThreadPoolExecutor]:
+    def executor(cls) -> ThreadPoolExecutor:
         return cls._get_executor()
 
     async def _aget_url(
         self,
         method: str,
         url: str,
-        data: Optional[Union[Dict[str, str], bytes]] = None,
+        content: Optional[Union[str, bytes]] = None,
+        data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, str]] = None,
     ) -> bytes:
         if self._exception_event.is_set():
             raise DuckDuckGoSearchException("Exception occurred in previous call.")
         try:
-            resp = await self._asession.request(method, url, data=data, params=params)
+            resp = await self._aclient.request(method, url, content=content, data=data, params=params)
+        except httpx.TimeoutException as ex:
+            self._exception_event.set()
+            raise TimeoutException(f"{url} {type(ex).__name__}: {ex}") from ex
         except Exception as ex:
             self._exception_event.set()
-            if "time" in str(ex).lower():
-                raise TimeoutException(f"{url} {type(ex).__name__}: {ex}") from ex
             raise DuckDuckGoSearchException(f"{url} {type(ex).__name__}: {ex}") from ex
-        logger.debug(f"_aget_url() {resp.url} {resp.status_code} {resp.elapsed:.2f} {len(resp.content)}")
         if resp.status_code == 200:
-            return cast(bytes, resp.content)
+            return resp.content
         self._exception_event.set()
         if resp.status_code in (202, 301, 403):
             raise RatelimitException(f"{resp.url} {resp.status_code} Ratelimit")
         raise DuckDuckGoSearchException(f"{resp.url} return None. {params=} {data=}")
 
     async def _aget_vqd(self, keywords: str) -> str:
         """Get vqd value for a search query."""
@@ -282,15 +286,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._asession.headers["Referer"] = "https://html.duckduckgo.com/"
+        self._aclient.headers["Referer"] = "https://html.duckduckgo.com/"
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         payload = {
             "q": keywords,
             "kl": region,
             "p": safesearch_base[safesearch.lower()],
             "o": "json",
             "api": "d.js",
@@ -307,15 +311,15 @@
         async def _text_html_page(s: int, page: int) -> None:
             priority = page * 100
             payload["s"] = f"{s}"
             resp_content = await self._aget_url("POST", "https://html.duckduckgo.com/html", data=payload)
             if b"No  results." in resp_content:
                 return
 
-            tree = await self._asession.loop.run_in_executor(
+            tree: Element = await asyncio.get_running_loop().run_in_executor(
                 self.executor, partial(document_fromstring, resp_content, self.parser)
             )
 
             for e in tree.xpath("//div[h2]"):
                 href = e.xpath("./a/@href")
                 href = href[0] if href else None
                 if (
@@ -374,15 +378,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._asession.headers["Referer"] = "https://lite.duckduckgo.com/"
+        self._aclient.headers["Referer"] = "https://lite.duckduckgo.com/"
         payload = {
             "q": keywords,
             "o": "json",
             "api": "d.js",
             "kl": region,
         }
         if timelimit:
@@ -394,15 +398,15 @@
         async def _text_lite_page(s: int, page: int) -> None:
             priority = page * 100
             payload["s"] = f"{s}"
             resp_content = await self._aget_url("POST", "https://lite.duckduckgo.com/lite/", data=payload)
             if b"No more results." in resp_content:
                 return
 
-            tree = await self._asession.loop.run_in_executor(
+            tree: Element = await asyncio.get_running_loop().run_in_executor(
                 self.executor, partial(document_fromstring, resp_content, self.parser)
             )
 
             data = zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr"))
             for i, e in data:
                 if i == 1:
                     href = e.xpath(".//a//@href")
@@ -898,15 +902,15 @@
             lat_b, lon_r = Decimal(coordinates[0]), Decimal(coordinates[3])
 
         # if a radius is specified, expand the search square
         lat_t += Decimal(radius) * Decimal(0.008983)
         lat_b -= Decimal(radius) * Decimal(0.008983)
         lon_l -= Decimal(radius) * Decimal(0.008983)
         lon_r += Decimal(radius) * Decimal(0.008983)
-        logger.debug(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
+        logger.info(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
 
         cache = set()
         results: List[Dict[str, str]] = []
 
         async def _maps_page(
             bbox: Tuple[Decimal, Decimal, Decimal, Decimal],
         ) -> Optional[List[Dict[str, str]]]:
@@ -1025,15 +1029,15 @@
         results = []
 
         async def _translate_keyword(keyword: str) -> None:
             resp_content = await self._aget_url(
                 "POST",
                 "https://duckduckgo.com/translation.js",
                 params=payload,
-                data=keyword.encode(),
+                content=keyword,
             )
             page_data = json_loads(resp_content)
             page_data["original"] = keyword
             results.append(page_data)
 
         if isinstance(keywords, str):
             keywords = [keywords]
```

### Comparing `duckduckgo_search-5.3.1/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.1
+Version: 5.3.1b1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -19,18 +19,19 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.7.0b4
-Requires-Dist: orjson>=3.10.3
+Requires-Dist: httpx[brotli,http2,socks]>=0.27.0
 Provides-Extra: lxml
 Requires-Dist: lxml>=5.2.1; extra == "lxml"
+Provides-Extra: orjson
+Requires-Dist: orjson>=3.10.3; extra == "orjson"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: ruff>=0.4.3; extra == "dev"
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search)](https://pepy.tech/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search/week)](https://pepy.tech/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
@@ -57,18 +58,14 @@
 * [7. translate() - translation](#7-translate---translation-by-duckduckgocom)
 * [8. suggestions() - suggestions](#8-suggestions---suggestions-by-duckduckgocom)
 
 ## Install
 ```python
 pip install -U duckduckgo_search
 ```
-There is also a beta release that uses the `httpx` library:
-```python
-pip install -U duckduckgo_search==5.3.0b4
-```
 > [!NOTE]
 > you can install lxml to use the `text` function with `backend='html'` or `backend='lite'` (size ≈ 12Mb)</br>
 > `pip install -U duckduckgo_search[lxml]`
 
 ## CLI version
 
 ```python3
```

### Comparing `duckduckgo_search-5.3.1/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.1/pyproject.toml` & `duckduckgo_search-5.3.1b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,16 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "click>=8.1.7",    
-    "curl_cffi>=0.7.0b4",
-    "orjson>=3.10.3",
+    "click>=8.1.7",  
+    "httpx[brotli, http2, socks]>=0.27.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
@@ -43,14 +42,17 @@
 [tool.setuptools.dynamic]
 version = {attr = "duckduckgo_search.version.__version__"}
 
 [project.optional-dependencies]
 lxml = [
     "lxml>=5.2.1",
 ]
+orjson = [
+    "orjson>=3.10.3",
+]
 dev = [
     "mypy>=1.10.0",
     "pytest>=8.2.0",
     "ruff>=0.4.3",
 ]
 
 [tool.ruff]
@@ -64,15 +66,15 @@
     "UP",  # pyupgrade
     "B",  # flake8-bugbear
     "SIM",  # flake8-simplify
     "I",  # isort
 ]
 ignore = ["D100"]
 
+[tool.ruff.per-file-ignores]
+"utils.py" = ["E501"]
+
 [tool.mypy]
 python_version = "3.8"
 strict = true
 exclude = ['cli\.py$', '__main__\.py$', "tests/", "build/"]
 
-[[tool.mypy.overrides]]
-module = "curl_cffi"
-ignore_missing_imports = true
```

### Comparing `duckduckgo_search-5.3.1/tests/test_cli.py` & `duckduckgo_search-5.3.1b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.1/tests/test_duckduckgo_search.py` & `duckduckgo_search-5.3.1b1/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

