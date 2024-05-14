# Comparing `tmp/conetwork_test-0.1.1.tar.gz` & `tmp/conetwork_test-0.1.2.tar.gz`

## Comparing `conetwork_test-0.1.1.tar` & `conetwork_test-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-------   0     1000     1000     1045 2024-05-10 13:42:36.000000 conetwork_test-0.1.1/fleece-network/Cargo.toml
--rw-r--r--   0     1000     1000   117062 2024-05-10 13:42:36.000000 conetwork_test-0.1.1/fleece-network/Cargo.lock
--rw-r--r--   0     1000     1000      668 2024-05-08 04:34:11.000000 conetwork_test-0.1.1/fleece-network/src/bin/center.rs
--rw-r--r--   0     1000     1000     2320 2024-05-14 06:44:49.000000 conetwork_test-0.1.1/fleece-network/src/bin/peer.rs
--rw-r--r--   0     1000     1000     3440 2024-05-14 04:23:22.000000 conetwork_test-0.1.1/fleece-network/src/center/mod.rs
--rw-r--r--   0     1000     1000    11063 2024-05-13 14:23:05.000000 conetwork_test-0.1.1/fleece-network/src/channel/behaviour.rs
--rw-r--r--   0     1000     1000     4075 2024-05-13 14:08:57.000000 conetwork_test-0.1.1/fleece-network/src/channel/codec.rs
--rw-r--r--   0     1000     1000    17288 2024-05-13 14:01:46.000000 conetwork_test-0.1.1/fleece-network/src/channel/handler.rs
--rw-r--r--   0     1000     1000     7249 2024-05-08 05:51:30.000000 conetwork_test-0.1.1/fleece-network/src/channel/legacy_stream.rs
--rw-r--r--   0     1000     1000     3477 2024-05-12 12:24:02.000000 conetwork_test-0.1.1/fleece-network/src/channel/message.rs
--rw-r--r--   0     1000     1000      388 2024-05-11 04:18:09.000000 conetwork_test-0.1.1/fleece-network/src/channel/mod.rs
--rw-r--r--   0     1000     1000      438 2024-05-08 04:34:11.000000 conetwork_test-0.1.1/fleece-network/src/error.rs
--rw-r--r--   0     1000     1000      128 2024-05-12 07:53:54.000000 conetwork_test-0.1.1/fleece-network/src/lib.rs
--rw-r--r--   0     1000     1000     1410 2024-05-12 15:29:27.000000 conetwork_test-0.1.1/fleece-network/src/peer/behaviour.rs
--rw-r--r--   0     1000     1000     5214 2024-05-13 14:02:22.000000 conetwork_test-0.1.1/fleece-network/src/peer/codec.rs
--rw-r--r--   0     1000     1000     3147 2024-05-14 02:45:36.000000 conetwork_test-0.1.1/fleece-network/src/peer/codec_legacy.rs
--rw-r--r--   0     1000     1000    11513 2024-05-14 04:23:03.000000 conetwork_test-0.1.1/fleece-network/src/peer/eventloop.rs
--rw-r--r--   0     1000     1000     1099 2024-05-08 04:34:11.000000 conetwork_test-0.1.1/fleece-network/src/peer/handler.rs
--rw-r--r--   0     1000     1000      121 2024-05-10 06:59:55.000000 conetwork_test-0.1.1/fleece-network/src/peer/mod.rs
--rw-r--r--   0     1000     1000     4160 2024-05-14 04:23:30.000000 conetwork_test-0.1.1/fleece-network/src/peer/peer.rs
--rw-r--r--   0     1000     1000     3753 2024-05-12 14:52:11.000000 conetwork_test-0.1.1/fleece-network/src/peer/proxy.rs
--rw-r--r--   0     1000     1000     1751 2024-05-12 15:31:08.000000 conetwork_test-0.1.1/fleece-network/src/router.rs
--rw-r--r--   0     1000     1000     7249 2024-05-12 15:30:38.000000 conetwork_test-0.1.1/fleece-network/src/stream.rs
--rw-r--r--   0     1000     1000     3915 2024-05-12 15:30:41.000000 conetwork_test-0.1.1/fleece-network/src/transport.rs
--rw-r--r--   0     1000     1000     4293 2024-05-12 15:30:31.000000 conetwork_test-0.1.1/fleece-network/src/utils/buflist.rs
--rw-r--r--   0     1000     1000     2159 2024-05-13 14:00:02.000000 conetwork_test-0.1.1/fleece-network/src/utils/chunk.rs
--rw-r--r--   0     1000     1000       32 2024-05-12 15:30:32.000000 conetwork_test-0.1.1/fleece-network/src/utils/mod.rs
--rw-r--r--   0     1000     1000     2650 2024-05-08 04:34:11.000000 conetwork_test-0.1.1/fleece-network/src/utils-legacy.rs
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 conetwork_test-0.1.1/python/Cargo.toml
--rw-r--r--   0     1000     1000       25 2024-05-14 05:31:54.000000 conetwork_test-0.1.1/python/.gitignore
--rw-r--r--   0     1000     1000      528 2024-05-14 07:01:45.000000 conetwork_test-0.1.1/python/example.py
--rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 conetwork_test-0.1.1/python/pysrc/fleece_network/__init__.py
--rw-r--r--   0     1000     1000     1763 2024-05-14 07:28:41.000000 conetwork_test-0.1.1/python/pysrc/fleece_network/peer.py
--rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 conetwork_test-0.1.1/python/pysrc/fleece_network/py.typed
--rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 conetwork_test-0.1.1/python/pysrc/fleece_network/serde.py
--rw-r--r--   0     1000     1000       15 2024-05-08 04:34:11.000000 conetwork_test-0.1.1/python/src/lib.rs
--rw-r--r--   0     1000     1000     5518 2024-05-14 05:21:02.000000 conetwork_test-0.1.1/python/src/proxy.rs
--rw-r--r--   0     1000     1000   120600 2024-05-14 07:37:12.000000 conetwork_test-0.1.1/python/Cargo.lock
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 conetwork_test-0.1.1/pyproject.toml
--rw-r--r--   0     1000     1000     1763 2024-05-14 07:28:41.000000 conetwork_test-0.1.1/pysrc/fleece_network/peer.py
--rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 conetwork_test-0.1.1/pysrc/fleece_network/__init__.py
--rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 conetwork_test-0.1.1/pysrc/fleece_network/py.typed
--rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 conetwork_test-0.1.1/pysrc/fleece_network/serde.py
--rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 conetwork_test-0.1.1/PKG-INFO
+-rw-------   0     1000     1000     1045 2024-05-10 13:42:36.000000 conetwork_test-0.1.2/fleece-network/Cargo.toml
+-rw-r--r--   0     1000     1000   117062 2024-05-10 13:42:36.000000 conetwork_test-0.1.2/fleece-network/Cargo.lock
+-rw-r--r--   0     1000     1000      668 2024-05-08 04:34:11.000000 conetwork_test-0.1.2/fleece-network/src/bin/center.rs
+-rw-r--r--   0     1000     1000     2320 2024-05-14 06:44:49.000000 conetwork_test-0.1.2/fleece-network/src/bin/peer.rs
+-rw-r--r--   0     1000     1000     3440 2024-05-14 04:23:22.000000 conetwork_test-0.1.2/fleece-network/src/center/mod.rs
+-rw-r--r--   0     1000     1000    11063 2024-05-13 14:23:05.000000 conetwork_test-0.1.2/fleece-network/src/channel/behaviour.rs
+-rw-r--r--   0     1000     1000     4075 2024-05-13 14:08:57.000000 conetwork_test-0.1.2/fleece-network/src/channel/codec.rs
+-rw-r--r--   0     1000     1000    17288 2024-05-13 14:01:46.000000 conetwork_test-0.1.2/fleece-network/src/channel/handler.rs
+-rw-r--r--   0     1000     1000     7249 2024-05-08 05:51:30.000000 conetwork_test-0.1.2/fleece-network/src/channel/legacy_stream.rs
+-rw-r--r--   0     1000     1000     3477 2024-05-12 12:24:02.000000 conetwork_test-0.1.2/fleece-network/src/channel/message.rs
+-rw-r--r--   0     1000     1000      388 2024-05-11 04:18:09.000000 conetwork_test-0.1.2/fleece-network/src/channel/mod.rs
+-rw-r--r--   0     1000     1000      438 2024-05-08 04:34:11.000000 conetwork_test-0.1.2/fleece-network/src/error.rs
+-rw-r--r--   0     1000     1000      128 2024-05-12 07:53:54.000000 conetwork_test-0.1.2/fleece-network/src/lib.rs
+-rw-r--r--   0     1000     1000     1410 2024-05-12 15:29:27.000000 conetwork_test-0.1.2/fleece-network/src/peer/behaviour.rs
+-rw-r--r--   0     1000     1000     5214 2024-05-13 14:02:22.000000 conetwork_test-0.1.2/fleece-network/src/peer/codec.rs
+-rw-r--r--   0     1000     1000     3147 2024-05-14 02:45:36.000000 conetwork_test-0.1.2/fleece-network/src/peer/codec_legacy.rs
+-rw-r--r--   0     1000     1000    11513 2024-05-14 04:23:03.000000 conetwork_test-0.1.2/fleece-network/src/peer/eventloop.rs
+-rw-r--r--   0     1000     1000     1099 2024-05-08 04:34:11.000000 conetwork_test-0.1.2/fleece-network/src/peer/handler.rs
+-rw-r--r--   0     1000     1000      121 2024-05-10 06:59:55.000000 conetwork_test-0.1.2/fleece-network/src/peer/mod.rs
+-rw-r--r--   0     1000     1000     4160 2024-05-14 04:23:30.000000 conetwork_test-0.1.2/fleece-network/src/peer/peer.rs
+-rw-r--r--   0     1000     1000     3753 2024-05-12 14:52:11.000000 conetwork_test-0.1.2/fleece-network/src/peer/proxy.rs
+-rw-r--r--   0     1000     1000     1751 2024-05-12 15:31:08.000000 conetwork_test-0.1.2/fleece-network/src/router.rs
+-rw-r--r--   0     1000     1000     7249 2024-05-12 15:30:38.000000 conetwork_test-0.1.2/fleece-network/src/stream.rs
+-rw-r--r--   0     1000     1000     3915 2024-05-12 15:30:41.000000 conetwork_test-0.1.2/fleece-network/src/transport.rs
+-rw-r--r--   0     1000     1000     4293 2024-05-12 15:30:31.000000 conetwork_test-0.1.2/fleece-network/src/utils/buflist.rs
+-rw-r--r--   0     1000     1000     2159 2024-05-13 14:00:02.000000 conetwork_test-0.1.2/fleece-network/src/utils/chunk.rs
+-rw-r--r--   0     1000     1000       32 2024-05-12 15:30:32.000000 conetwork_test-0.1.2/fleece-network/src/utils/mod.rs
+-rw-r--r--   0     1000     1000     2650 2024-05-08 04:34:11.000000 conetwork_test-0.1.2/fleece-network/src/utils-legacy.rs
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 conetwork_test-0.1.2/python/Cargo.toml
+-rw-r--r--   0     1000     1000       25 2024-05-14 05:31:54.000000 conetwork_test-0.1.2/python/.gitignore
+-rw-r--r--   0     1000     1000      528 2024-05-14 07:01:45.000000 conetwork_test-0.1.2/python/example.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 conetwork_test-0.1.2/python/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000     1762 2024-05-14 07:42:00.000000 conetwork_test-0.1.2/python/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 conetwork_test-0.1.2/python/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 conetwork_test-0.1.2/python/pysrc/fleece_network/serde.py
+-rw-r--r--   0     1000     1000       15 2024-05-08 04:34:11.000000 conetwork_test-0.1.2/python/src/lib.rs
+-rw-r--r--   0     1000     1000     5518 2024-05-14 05:21:02.000000 conetwork_test-0.1.2/python/src/proxy.rs
+-rw-r--r--   0     1000     1000   120600 2024-05-14 07:42:08.000000 conetwork_test-0.1.2/python/Cargo.lock
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 conetwork_test-0.1.2/pyproject.toml
+-rw-r--r--   0     1000     1000     1762 2024-05-14 07:42:00.000000 conetwork_test-0.1.2/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 conetwork_test-0.1.2/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 conetwork_test-0.1.2/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 conetwork_test-0.1.2/pysrc/fleece_network/serde.py
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 conetwork_test-0.1.2/PKG-INFO
```

### Comparing `conetwork_test-0.1.1/fleece-network/Cargo.toml` & `conetwork_test-0.1.2/fleece-network/Cargo.toml`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/Cargo.lock` & `conetwork_test-0.1.2/fleece-network/Cargo.lock`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/bin/center.rs` & `conetwork_test-0.1.2/fleece-network/src/bin/center.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/bin/peer.rs` & `conetwork_test-0.1.2/fleece-network/src/bin/peer.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/center/mod.rs` & `conetwork_test-0.1.2/fleece-network/src/center/mod.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/channel/behaviour.rs` & `conetwork_test-0.1.2/fleece-network/src/channel/behaviour.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/channel/codec.rs` & `conetwork_test-0.1.2/fleece-network/src/channel/codec.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/channel/handler.rs` & `conetwork_test-0.1.2/fleece-network/src/channel/handler.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/channel/legacy_stream.rs` & `conetwork_test-0.1.2/fleece-network/src/channel/legacy_stream.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/channel/message.rs` & `conetwork_test-0.1.2/fleece-network/src/channel/message.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/peer/behaviour.rs` & `conetwork_test-0.1.2/fleece-network/src/peer/behaviour.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/peer/codec.rs` & `conetwork_test-0.1.2/fleece-network/src/peer/codec.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/peer/codec_legacy.rs` & `conetwork_test-0.1.2/fleece-network/src/peer/codec_legacy.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/peer/eventloop.rs` & `conetwork_test-0.1.2/fleece-network/src/peer/eventloop.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/peer/handler.rs` & `conetwork_test-0.1.2/fleece-network/src/peer/handler.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/peer/peer.rs` & `conetwork_test-0.1.2/fleece-network/src/peer/peer.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/peer/proxy.rs` & `conetwork_test-0.1.2/fleece-network/src/peer/proxy.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/router.rs` & `conetwork_test-0.1.2/fleece-network/src/router.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/stream.rs` & `conetwork_test-0.1.2/fleece-network/src/stream.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/transport.rs` & `conetwork_test-0.1.2/fleece-network/src/transport.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/utils/buflist.rs` & `conetwork_test-0.1.2/fleece-network/src/utils/buflist.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/utils/chunk.rs` & `conetwork_test-0.1.2/fleece-network/src/utils/chunk.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/fleece-network/src/utils-legacy.rs` & `conetwork_test-0.1.2/fleece-network/src/utils-legacy.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/python/Cargo.toml` & `conetwork_test-0.1.2/python/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "fleece-network-python"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 
 [lib]
 name = "fleece_network_rust"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `conetwork_test-0.1.1/python/example.py` & `conetwork_test-0.1.2/python/example.py`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/python/pysrc/fleece_network/peer.py` & `conetwork_test-0.1.2/python/pysrc/fleece_network/peer.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         )
         return response.status, response.payload
 
     def run(self):
         thread = Thread(target=self._listen)
         thread.start()
 
-    def _listen(self):
+    def listen(self):
         while True:
             r = self.proxy.recv()
             if r is not None:
                 request_id, request = r
                 self.pool.submit(self._delegate, request_id, request)
             else:
                 break
```

### Comparing `conetwork_test-0.1.1/python/pysrc/fleece_network/serde.py` & `conetwork_test-0.1.2/python/pysrc/fleece_network/serde.py`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/python/src/proxy.rs` & `conetwork_test-0.1.2/python/src/proxy.rs`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/python/Cargo.lock` & `conetwork_test-0.1.2/python/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1226,15 +1226,15 @@
  "tracing-flame",
  "tracing-subscriber",
  "void",
 ]
 
 [[package]]
 name = "fleece-network-python"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "bytes",
  "chrono",
  "crossbeam-channel",
  "dyn-clone",
  "fleece-network",
  "futures",
```

### Comparing `conetwork_test-0.1.1/pyproject.toml` & `conetwork_test-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conetwork_test-0.1.1/pysrc/fleece_network/peer.py` & `conetwork_test-0.1.2/pysrc/fleece_network/peer.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         )
         return response.status, response.payload
 
     def run(self):
         thread = Thread(target=self._listen)
         thread.start()
 
-    def _listen(self):
+    def listen(self):
         while True:
             r = self.proxy.recv()
             if r is not None:
                 request_id, request = r
                 self.pool.submit(self._delegate, request_id, request)
             else:
                 break
```

### Comparing `conetwork_test-0.1.1/pysrc/fleece_network/serde.py` & `conetwork_test-0.1.2/pysrc/fleece_network/serde.py`

 * *Files identical despite different names*
