# Comparing `tmp/fleece_network-0.2.2.tar.gz` & `tmp/fleece_network-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleece_network-0.2.2.tar", max compression
+gzip compressed data
```

## Comparing `fleece_network-0.2.2.tar` & `fleece_network-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,44 @@
--rw-r--r--   0        0        0      327 2024-04-20 11:21:04.274155 fleece_network-0.2.2/README.md
--rw-r--r--   0        0        0       66 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/__init__.py
--rw-r--r--   0        0        0      349 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aioice/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aioice/candidate.py
--rw-r--r--   0        0        0    41823 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aioice/ice.py
--rw-r--r--   0        0        0     6655 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aioice/mdns.py
--rw-r--r--   0        0        0    12369 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aioice/stun.py
--rw-r--r--   0        0        0    15054 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aioice/turn.py
--rw-r--r--   0        0        0      264 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aioice/utils.py
--rw-r--r--   0        0        0     1375 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aiortc/__init__.py
--rw-r--r--   0        0        0      824 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aiortc/clock.py
--rw-r--r--   0        0        0      180 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aiortc/exceptions.py
--rw-r--r--   0        0        0    21027 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aiortc/rate.py
--rw-r--r--   0        0        0     1040 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aiortc/rtcconfiguration.py
--rw-r--r--   0        0        0     6531 2024-04-20 11:21:04.274155 fleece_network-0.2.2/fleece_network/aiortc/rtcdatachannel.py
--rw-r--r--   0        0        0    13289 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/rtcdtlstransport.py
--rw-r--r--   0        0        0    11425 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/rtcicetransport.py
--rw-r--r--   0        0        0    31914 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/rtcpeerconnection.py
--rw-r--r--   0        0        0     4612 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/rtcrtpparameters.py
--rw-r--r--   0        0        0    61945 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/rtcsctptransport.py
--rw-r--r--   0        0        0      500 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/rtcsessiondescription.py
--rw-r--r--   0        0        0    24050 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/rtp.py
--rw-r--r--   0        0        0    21790 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/sdp.py
--rw-r--r--   0        0        0     2879 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/stats.py
--rw-r--r--   0        0        0      978 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/aiortc/utils.py
--rw-r--r--   0        0        0      718 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/messages.py
--rw-r--r--   0        0        0    21922 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/peer.py
--rw-r--r--   0        0        0        0 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/py.typed
--rw-r--r--   0        0        0      641 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/sede.py
--rw-r--r--   0        0        0     2150 2024-04-20 11:21:04.278155 fleece_network-0.2.2/fleece_network/signaling.py
--rw-r--r--   0        0        0      619 2024-04-20 11:21:04.278155 fleece_network-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fleece_network-0.2.2/PKG-INFO
+-rw-------   0     1000     1000     1045 2024-05-10 13:42:36.000000 fleece_network-0.4.0/fleece-network/Cargo.toml
+-rw-r--r--   0     1000     1000   117062 2024-05-10 13:42:36.000000 fleece_network-0.4.0/fleece-network/Cargo.lock
+-rw-r--r--   0     1000     1000      668 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/bin/center.rs
+-rw-r--r--   0     1000     1000     2320 2024-05-13 14:19:20.000000 fleece_network-0.4.0/fleece-network/src/bin/peer.rs
+-rw-r--r--   0     1000     1000     3440 2024-05-14 04:23:22.000000 fleece_network-0.4.0/fleece-network/src/center/mod.rs
+-rw-r--r--   0     1000     1000    11063 2024-05-13 14:23:05.000000 fleece_network-0.4.0/fleece-network/src/channel/behaviour.rs
+-rw-r--r--   0     1000     1000     4075 2024-05-13 14:08:57.000000 fleece_network-0.4.0/fleece-network/src/channel/codec.rs
+-rw-r--r--   0     1000     1000    17288 2024-05-13 14:01:46.000000 fleece_network-0.4.0/fleece-network/src/channel/handler.rs
+-rw-r--r--   0     1000     1000     7249 2024-05-08 05:51:30.000000 fleece_network-0.4.0/fleece-network/src/channel/legacy_stream.rs
+-rw-r--r--   0     1000     1000     3477 2024-05-12 12:24:02.000000 fleece_network-0.4.0/fleece-network/src/channel/message.rs
+-rw-r--r--   0     1000     1000      388 2024-05-11 04:18:09.000000 fleece_network-0.4.0/fleece-network/src/channel/mod.rs
+-rw-r--r--   0     1000     1000      438 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/error.rs
+-rw-r--r--   0     1000     1000      128 2024-05-12 07:53:54.000000 fleece_network-0.4.0/fleece-network/src/lib.rs
+-rw-r--r--   0     1000     1000     1410 2024-05-12 15:29:27.000000 fleece_network-0.4.0/fleece-network/src/peer/behaviour.rs
+-rw-r--r--   0     1000     1000     5214 2024-05-13 14:02:22.000000 fleece_network-0.4.0/fleece-network/src/peer/codec.rs
+-rw-r--r--   0     1000     1000     3147 2024-05-14 02:45:36.000000 fleece_network-0.4.0/fleece-network/src/peer/codec_legacy.rs
+-rw-r--r--   0     1000     1000    11513 2024-05-14 04:23:03.000000 fleece_network-0.4.0/fleece-network/src/peer/eventloop.rs
+-rw-r--r--   0     1000     1000     1099 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/peer/handler.rs
+-rw-r--r--   0     1000     1000      121 2024-05-10 06:59:55.000000 fleece_network-0.4.0/fleece-network/src/peer/mod.rs
+-rw-r--r--   0     1000     1000     4160 2024-05-14 04:23:30.000000 fleece_network-0.4.0/fleece-network/src/peer/peer.rs
+-rw-r--r--   0     1000     1000     3753 2024-05-12 14:52:11.000000 fleece_network-0.4.0/fleece-network/src/peer/proxy.rs
+-rw-r--r--   0     1000     1000     1751 2024-05-12 15:31:08.000000 fleece_network-0.4.0/fleece-network/src/router.rs
+-rw-r--r--   0     1000     1000     7249 2024-05-12 15:30:38.000000 fleece_network-0.4.0/fleece-network/src/stream.rs
+-rw-r--r--   0     1000     1000     3915 2024-05-12 15:30:41.000000 fleece_network-0.4.0/fleece-network/src/transport.rs
+-rw-r--r--   0     1000     1000     4293 2024-05-12 15:30:31.000000 fleece_network-0.4.0/fleece-network/src/utils/buflist.rs
+-rw-r--r--   0     1000     1000     2159 2024-05-13 14:00:02.000000 fleece_network-0.4.0/fleece-network/src/utils/chunk.rs
+-rw-r--r--   0     1000     1000       32 2024-05-12 15:30:32.000000 fleece_network-0.4.0/fleece-network/src/utils/mod.rs
+-rw-r--r--   0     1000     1000     2650 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/utils-legacy.rs
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 fleece_network-0.4.0/python/Cargo.toml
+-rw-r--r--   0     1000     1000       25 2024-05-14 05:31:54.000000 fleece_network-0.4.0/python/.gitignore
+-rw-r--r--   0     1000     1000      528 2024-05-14 06:17:50.000000 fleece_network-0.4.0/python/example.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.0/python/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000     1615 2024-05-14 05:32:36.000000 fleece_network-0.4.0/python/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.0/python/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 fleece_network-0.4.0/python/pysrc/fleece_network/serde.py
+-rw-r--r--   0     1000     1000       15 2024-05-08 04:34:11.000000 fleece_network-0.4.0/python/src/lib.rs
+-rw-r--r--   0     1000     1000     5518 2024-05-14 05:21:02.000000 fleece_network-0.4.0/python/src/proxy.rs
+-rw-r--r--   0     1000     1000   120600 2024-05-14 06:33:50.000000 fleece_network-0.4.0/python/Cargo.lock
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 fleece_network-0.4.0/pyproject.toml
+-rw-r--r--   0     1000     1000     1615 2024-05-14 05:32:36.000000 fleece_network-0.4.0/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.0/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.0/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 fleece_network-0.4.0/pysrc/fleece_network/serde.py
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 fleece_network-0.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `fleece_network-0.2.2/fleece_network/sede.py` & `fleece_network-0.4.0/python/pysrc/fleece_network/serde.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pickle
 from typing import Any
 
 from safetensors.torch import load, save
-from torch import Tensor
 
 
-def dumps(tensors: dict[str, Tensor], metadata: dict[str, Any]) -> bytes:
+def dumps(tensors: dict[str, "Tensor"], metadata: dict[str, Any]) -> bytes:
     metadata_bytes = pickle.dumps(metadata)
     tensors_bytes = save(tensors)
     return (
         len(metadata_bytes).to_bytes(4, byteorder="big")
         + metadata_bytes
         + tensors_bytes
     )
 
 
-def loads(b: bytes) -> tuple[dict[str, Tensor], dict[str, Any]]:
+def loads(b: bytes) -> tuple[dict[str, "Tensor"], dict[str, Any]]:
     metadata_length = int.from_bytes(b[:4], byteorder="big")
     metadata = pickle.loads(b[4 : 4 + metadata_length])
     tensors = load(b[4 + metadata_length :])
     return tensors, metadata
```

