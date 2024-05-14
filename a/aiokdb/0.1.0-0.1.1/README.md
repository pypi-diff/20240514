# Comparing `tmp/aiokdb-0.1.0.tar.gz` & `tmp/aiokdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokdb-0.1.0.tar", last modified: Wed Jan 24 14:36:27 2024, max compression
+gzip compressed data, was "aiokdb-0.1.1.tar", last modified: Tue May 14 08:12:34 2024, max compression
```

## Comparing `aiokdb-0.1.0.tar` & `aiokdb-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:27.001328 aiokdb-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:26.993327 aiokdb-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:26.997328 aiokdb-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-01-24 14:36:15.000000 aiokdb-0.1.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-01-24 14:36:15.000000 aiokdb-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-24 14:36:15.000000 aiokdb-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-24 14:36:15.000000 aiokdb-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-01-24 14:36:27.001328 aiokdb-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-01-24 14:36:15.000000 aiokdb-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:26.997328 aiokdb-0.1.0/aiokdb/
--rw-r--r--   0 runner    (1001) docker     (127)    29210 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/format.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-24 14:36:15.000000 aiokdb-0.1.0/aiokdb/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:27.001328 aiokdb-0.1.0/aiokdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-01-24 14:36:26.000000 aiokdb-0.1.0/aiokdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-24 14:36:26.000000 aiokdb-0.1.0/aiokdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 14:36:26.000000 aiokdb-0.1.0/aiokdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-24 14:36:26.000000 aiokdb-0.1.0/aiokdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-24 14:36:15.000000 aiokdb-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-24 14:36:15.000000 aiokdb-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 14:36:27.001328 aiokdb-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:26.997328 aiokdb-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 14:36:15.000000 aiokdb-0.1.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-01-24 14:36:15.000000 aiokdb-0.1.0/test/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-01-24 14:36:15.000000 aiokdb-0.1.0/test/test_client_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-24 14:36:15.000000 aiokdb-0.1.0/test/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-01-24 14:36:15.000000 aiokdb-0.1.0/test/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-01-24 14:36:15.000000 aiokdb-0.1.0/test/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-01-24 14:36:15.000000 aiokdb-0.1.0/test/test_serialization_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.108641 aiokdb-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.104641 aiokdb-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.104641 aiokdb-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-14 08:12:24.000000 aiokdb-0.1.1/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 08:12:24.000000 aiokdb-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-14 08:12:24.000000 aiokdb-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 08:12:24.000000 aiokdb-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-14 08:12:34.108641 aiokdb-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-14 08:12:24.000000 aiokdb-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.104641 aiokdb-0.1.1/aiokdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    29541 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.108641 aiokdb-0.1.1/aiokdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-14 08:12:24.000000 aiokdb-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 08:12:24.000000 aiokdb-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:12:34.108641 aiokdb-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.108641 aiokdb-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_client_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_serialization_examples.py
```

### Comparing `aiokdb-0.1.0/.github/workflows/check.yml` & `aiokdb-0.1.1/.github/workflows/check.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,13 @@
 
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - run: python -m pip install --upgrade pip
-    - run: python -m pip install "ruff<1" "mypy<2" "black<23" "isort<6" pytest
+    - run: python -m pip install "ruff<1" "mypy<2" pytest
     - run: pip install -r requirements.txt
     - run: ruff check .
+    - run: ruff format --check .
     - run: mypy --strict .
-    - run: black --check .
-    - run: isort --check --profile black .
     - run: pytest .
```

### Comparing `aiokdb-0.1.0/.github/workflows/publish.yml` & `aiokdb-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/.gitignore` & `aiokdb-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/LICENSE` & `aiokdb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/PKG-INFO` & `aiokdb-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pure Python asyncio connector to KDB
 Author-email: Chris Shucksmith <chris@shucksmith.co.uk>
 Project-URL: Homepage, https://github.com/TeaEngineering/aiokdb
 Project-URL: Issues, https://github.com/TeaEngineering/aiokdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,13 +67,13 @@
 ```
 
 ## Tests
 
 The unit tests in `test/test_rpc.py` will use a real KDB binary to test against (over RPC) if you set `KDB_PYTEST_SERVICE` to a URL of the form `kdb://user:password@hostname:port`, otherwise that test is skipped and they are self contained.
 
 * Formatting with `ruff check .`
-* Formatting with `black .`
+* Formatting with `ruff format .`
 * imports `isort --check --profile black .`
 * Check type annotations with `mypy --strict .`
 * Run `pytest .` in the root directory
```

### Comparing `aiokdb-0.1.0/README.md` & `aiokdb-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,13 +53,13 @@
 ```
 
 ## Tests
 
 The unit tests in `test/test_rpc.py` will use a real KDB binary to test against (over RPC) if you set `KDB_PYTEST_SERVICE` to a URL of the form `kdb://user:password@hostname:port`, otherwise that test is skipped and they are self contained.
 
 * Formatting with `ruff check .`
-* Formatting with `black .`
+* Formatting with `ruff format .`
 * imports `isort --check --profile black .`
 * Check type annotations with `mypy --strict .`
 * Run `pytest .` in the root directory
```

### Comparing `aiokdb-0.1.0/aiokdb/__init__.py` & `aiokdb-0.1.1/aiokdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import array
 import enum
+import logging
 import struct
 import uuid
 from collections.abc import MutableSequence, Sequence
 from typing import Any, BinaryIO, Type, Union, cast
 
 __all__ = [
     "b9",
     "d9",
     "ktn",
 ]
 
 # mypy: disallow-untyped-defs
 
+logger = logging.getLogger(__name__)
+
 
 class WrongTypeForOperationError(TypeError):
     pass
 
 
 class AttrEnum(enum.IntEnum):
     NONE = 0
@@ -119,14 +122,16 @@
 DEFAULT_CONTEXT = KContext()
 
 
 def tn(t: int) -> str:
     te = t
     if te != TypeEnum.KRR:
         te = abs(t)
+    if te >= 20 and te < 40:
+        return "Enum ({t})"
     return f"{TypeEnum(te).name} ({t})"
 
 
 class KObj:
     def __init__(
         self,
         t: int = 0,
@@ -758,15 +763,15 @@
         raise Exception(f"Final position at {pos} expected {msglen}")
     return k
 
 
 def _d9_unpackfrom(data: bytes, offset: int) -> tuple[KObj, int]:
     (t,) = struct.unpack_from("<b", data, offset=offset)
     offset += 1
-    print(f" at offset {offset} unpacking type {tn(t)}")
+    logger.debug(f" at offset {offset}/{len(data)} unpacking type {tn(t)}")
     if t == -TypeEnum.KS or t == TypeEnum.KRR:
         return KSymAtom(t).frombytes(data, offset)
     elif t < 0:
         return KObjAtom(t).frombytes(data, offset)
     elif t >= 0 and t < 20:
         # ranged vector types, need to verify t
         return VECTOR_CONSTUCTORS[t](t).frombytes(data, offset)
@@ -780,15 +785,16 @@
     elif t == TypeEnum.XT:
         kkeys, offset = _d9_unpackfrom(data, offset + 1)
         return KFlip(kkeys), offset
     elif t == TypeEnum.SD:
         kkeys, offset = _d9_unpackfrom(data, offset)
         kvalues, offset = _d9_unpackfrom(data, offset)
         return KDict(kkeys, kvalues, t), offset
-
+    elif t >= 20 and t < 30:
+        return VECTOR_CONSTUCTORS[TypeEnum.KJ](t).frombytes(data, offset)
     raise ValueError(f"Unable to d9 unpack t={t}")
 
 
 # atom constructors
 def ka(t: Union[int, TypeEnum]) -> KObj:
     return KObjAtom(t)
 
@@ -991,7 +997,12 @@
 
 def fromfile(f: BinaryIO) -> KObj:
     # theres no length header since files have a size
     rb = f.read()
     assert rb[0:2] == b"\xff\x01"
     k, _ = _d9_unpackfrom(rb, 2)
     return k
+
+
+def writefile(k: KObj, f: BinaryIO) -> None:
+    f.write(b"\xff\x01")
+    f.write(k._databytes())
```

### Comparing `aiokdb-0.1.0/aiokdb/cli.py` & `aiokdb-0.1.1/aiokdb/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,19 +38,20 @@
             break
         except Exception:
             traceback.print_exc(limit=-2)
     return None
 
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.INFO)
-
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", default="localhost")
     parser.add_argument("--port", default=8890, type=int)
     parser.add_argument("--user", default="user")
     parser.add_argument("--password")
     parser.add_argument("--height", default=10, type=int)
-    args = parser.parse_args()
+    parser.add_argument("--debug", action="store_true")
 
+    args = parser.parse_args()
+    debug_level = {True: logging.DEBUG, False: logging.INFO}
+    logging.basicConfig(level=debug_level[args.debug])
     with patch_stdout():
         asyncio.run(main(args))
```

### Comparing `aiokdb-0.1.0/aiokdb/client.py` & `aiokdb-0.1.1/aiokdb/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import asyncio
 import logging
 import struct
 from typing import Any, Optional
 
-from aiokdb import cv
+from aiokdb import cv, logger
 from aiokdb.server import CredentialsException, KdbReader, KdbWriter
 
 
 # KDB client code
 async def open_qipc_connection(
     host: str = "127.0.0.1",
     port: int = 8890,
@@ -25,18 +25,18 @@
         auth = auth + ":" + password
 
     writer.write(auth.encode() + struct.pack("<B", ver) + b"\000")
     await writer.drain()
 
     try:
         data = await reader.readexactly(1)  # negotiated version, if auth correct
-        logging.info(f"Received: {data!r}")
         remote_ver = struct.unpack("<B", data)[0]
         if remote_ver != ver:
             raise Exception(f"expected version {ver}, server gave {remote_ver}")
+        logger.debug(f"Connected OK, remote_ver={remote_ver}")
     except asyncio.IncompleteReadError as e:
         raise CredentialsException(e)
 
     q_reader = KdbReader(reader)
     q_writer = KdbWriter(writer, q_reader, version=remote_ver)
     return q_reader, q_writer
```

### Comparing `aiokdb-0.1.0/aiokdb/extras.py` & `aiokdb-0.1.1/aiokdb/extras.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/aiokdb/format.py` & `aiokdb-0.1.1/aiokdb/format.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/aiokdb/server.py` & `aiokdb-0.1.1/aiokdb/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import itertools
 import logging
 import os
 import struct
 from functools import partial
 from typing import Any, Callable, Optional, Tuple
 
-from aiokdb import KException, KObj, MessageType, TypeEnum, b9, d9, krr
+from aiokdb import KException, KObj, MessageType, TypeEnum, b9, d9, krr, logger
 
 
 class CredentialsException(Exception):
     pass
 
 
 # TypeAlias for Optional KObj callback
@@ -22,15 +22,17 @@
     def __init__(self, reader: asyncio.StreamReader, raise_krr: bool = True):
         self.reader = reader
         self.raise_krr = raise_krr
 
     async def read(self) -> tuple[MessageType, KObj]:
         msgh = await self.reader.readexactly(8)
         ver, msgtype, flags, msglen = struct.unpack("<BBHI", msgh)
-        print(f"> recv ver={ver} msgtype={msgtype} flags={flags} msglen={msglen}")
+        logger.debug(
+            f"> recv ver={ver} msgtype={msgtype} flags={flags} msglen={msglen}"
+        )
         payload = await self.reader.readexactly(msglen - 8)
         # TODO: if compressed, decompress payload
         if flags != 0:
             print(payload)
             raise ValueError("compressed payload NYI {flags}")
         k = d9(msgh + payload)
         if self.raise_krr and k.t == TypeEnum.KRR:
@@ -49,15 +51,15 @@
         self.writer = writer
         self.qid = qid
         self.version = version
         self.reader = kreader
 
     def write(self, obj: KObj, mt: MessageType = MessageType.SYNC) -> None:
         bs = b9(obj, msgtype=mt)
-        print(f"< sending {bs!r}")
+        logger.debug(f"< sending {bs!r}")
         self.writer.write(bs)
 
     async def sync_req(self, obj: KObj, ooob: OptKcb = None) -> KObj:
         # responses arrive in the order that requests are sent
         # if tasks are calling this method along with read() directly
         # then responses will get muddled up or lost
         #
```

### Comparing `aiokdb-0.1.0/aiokdb/socket.py` & `aiokdb-0.1.1/aiokdb/socket.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/aiokdb.egg-info/PKG-INFO` & `aiokdb-0.1.1/aiokdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pure Python asyncio connector to KDB
 Author-email: Chris Shucksmith <chris@shucksmith.co.uk>
 Project-URL: Homepage, https://github.com/TeaEngineering/aiokdb
 Project-URL: Issues, https://github.com/TeaEngineering/aiokdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,13 +67,13 @@
 ```
 
 ## Tests
 
 The unit tests in `test/test_rpc.py` will use a real KDB binary to test against (over RPC) if you set `KDB_PYTEST_SERVICE` to a URL of the form `kdb://user:password@hostname:port`, otherwise that test is skipped and they are self contained.
 
 * Formatting with `ruff check .`
-* Formatting with `black .`
+* Formatting with `ruff format .`
 * imports `isort --check --profile black .`
 * Check type annotations with `mypy --strict .`
 * Run `pytest .` in the root directory
```

### Comparing `aiokdb-0.1.0/aiokdb.egg-info/SOURCES.txt` & `aiokdb-0.1.1/aiokdb.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 aiokdb.egg-info/SOURCES.txt
 aiokdb.egg-info/dependency_links.txt
 aiokdb.egg-info/top_level.txt
 test/__init__.py
 test/test_atoms.py
 test/test_client_server.py
 test/test_context.py
+test/test_file.py
 test/test_format.py
 test/test_rpc.py
 test/test_serialization_examples.py
```

### Comparing `aiokdb-0.1.0/pyproject.toml` & `aiokdb-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
+[tool.ruff.lint]
+extend-select = ["I"]
+
 [project]
 name = "aiokdb"
 authors = [
   { name="Chris Shucksmith", email="chris@shucksmith.co.uk" },
 ]
 description = "Pure Python asyncio connector to KDB"
 readme = "README.md"
```

### Comparing `aiokdb-0.1.0/test/test_atoms.py` & `aiokdb-0.1.1/test/test_atoms.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/test/test_client_server.py` & `aiokdb-0.1.1/test/test_client_server.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/test/test_format.py` & `aiokdb-0.1.1/test/test_format.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/test/test_rpc.py` & `aiokdb-0.1.1/test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.0/test/test_serialization_examples.py` & `aiokdb-0.1.1/test/test_serialization_examples.py`

 * *Files identical despite different names*

