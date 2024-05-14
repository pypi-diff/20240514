# Comparing `tmp/kelvin_sdk_pubsub-3.0.4-py3-none-any.whl.zip` & `tmp/kelvin_sdk_pubsub-3.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16569 bytes, number of entries: 14
--rw-r--r--  2.0 unx      473 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/__init__.py
--rw-r--r--  2.0 unx     1946 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/client.py
--rw-r--r--  2.0 unx    19399 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/config.py
--rw-r--r--  2.0 unx    21039 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/connection.py
--rw-r--r--  2.0 unx      149 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/error.py
--rw-r--r--  2.0 unx     1988 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/prometheus.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/py.typed
--rw-r--r--  2.0 unx     5438 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/types.py
--rw-r--r--  2.0 unx      740 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/utils.py
--rw-r--r--  2.0 unx      411 b- defN 24-Apr-18 20:47 kelvin/sdk/pubsub/version.py
--rw-r--r--  2.0 unx     3009 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1179 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/RECORD
-14 files, 55870 bytes uncompressed, 14593 bytes compressed:  73.9%
+Zip file size: 16678 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      473 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/__init__.py
+-rw-r--r--  2.0 unx     1946 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/client.py
+-rw-r--r--  2.0 unx    19399 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/config.py
+-rw-r--r--  2.0 unx    21673 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/connection.py
+-rw-r--r--  2.0 unx      149 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/error.py
+-rw-r--r--  2.0 unx     1988 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/prometheus.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/py.typed
+-rw-r--r--  2.0 unx     5438 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/types.py
+-rw-r--r--  2.0 unx      740 b- defN 24-May-14 14:14 kelvin/sdk/pubsub/utils.py
+-rw-r--r--  2.0 unx      411 b- defN 24-May-14 14:20 kelvin/sdk/pubsub/version.py
+-rw-r--r--  2.0 unx     3009 b- defN 24-May-14 14:20 kelvin_sdk_pubsub-3.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 14:20 kelvin_sdk_pubsub-3.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-14 14:20 kelvin_sdk_pubsub-3.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1179 b- defN 24-May-14 14:20 kelvin_sdk_pubsub-3.0.5.dist-info/RECORD
+14 files, 56504 bytes uncompressed, 14702 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: kelvin/sdk/pubsub/utils.py
 Comment: 
 
 Filename: kelvin/sdk/pubsub/version.py
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.4.dist-info/METADATA
+Filename: kelvin_sdk_pubsub-3.0.5.dist-info/METADATA
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.4.dist-info/WHEEL
+Filename: kelvin_sdk_pubsub-3.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.4.dist-info/top_level.txt
+Filename: kelvin_sdk_pubsub-3.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.4.dist-info/RECORD
+Filename: kelvin_sdk_pubsub-3.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kelvin/sdk/pubsub/connection.py

```diff
@@ -317,29 +317,28 @@
             max_attempts=max_attempts,
             min_interval=self.min_interval,
             max_interval=self.max_interval,
             keepalive=config.keepalive,
         )
         client.on_connect = self._on_connect
         client.on_message = self._on_message
-
-        client.loop_start()
+        client.on_disconnect = self._on_disconnect
 
         if not self._connect_count:
             self._send_storage_config()
         self._connect_count += 1
 
     def conn_check(self) -> None:
         if self._client is None:
             return
 
         rc = self._client._send_simple_command(PINGREQ)  # noqa
         if rc != MQTT_ERR_SUCCESS:
             logger.info("Mqtt connection lost. Reconnecting")
-            self._client.reconnect()  # noqa
+            self._reconnect()  # noqa
 
     def _send_storage_config(self) -> None:
         """Send storage configuration."""
 
         client = self._client
         if client is None:
             return
@@ -422,14 +421,32 @@
                 with queue.mutex:
                     if queue.full():
                         logger.warning("Queue full. Discarding oldest message", topic=topic)
                         queue.get_nowait()
                         queue.task_done()
                     queue.put_nowait(result)
 
+    def _on_disconnect(self, client: Client, userdata: Any, rc: int) -> None:
+        """Disconnect handler."""
+        logger.info("Disconnected", rc=rc)
+        if rc != MQTT_ERR_SUCCESS:
+            self._reconnect()
+
+    def _reconnect(self) -> None:
+        """Reconnect."""
+        logger.info("Reconnecting")
+        client = self._client
+        if client is None:
+            return
+
+        try:
+            client.reconnect()
+        except ConnectionRefusedError:
+            logger.error("Connection refused")
+
     def send(self, message: Union[Message, Sequence[Message]]) -> None:
         """Send message."""
 
         client = self._client
         if client is None:
             return
 
@@ -438,25 +455,30 @@
         messages = message if isinstance(message, Sequence) else [message]
 
         for message in messages:
             for topic, payload, retain, asset, metric in self._make_payloads(message):
                 ret = client.publish(topic, payload, qos=qos, retain=retain)
                 if ret.rc != MQTT_ERR_SUCCESS:
                     logger.info("Publish failed. Reconnecting Mqtt")
-                    client.reconnect()
+                    self._reconnect()
                     client.publish(topic, payload, qos=qos, retain=retain)
                 self.prometheus_client.set_asset_metric_timestamp(asset, metric)
                 self._output_count += 1
 
+        client.loop_write()
+
     def receive(self, timeout: Optional[float] = None) -> Optional[Message]:
         """Receive message."""
 
         if self._client is None:
             return None
 
+        self._client.loop_misc()
+        self._client.loop_read()
+
         try:
             message = self._queue.get(timeout=timeout)
         except Empty:
             return None
         else:
             self._queue.task_done()
             return message
```

## kelvin/sdk/pubsub/version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '3.0.4'
-__version_tuple__ = version_tuple = (3, 0, 4)
+__version__ = version = '3.0.5'
+__version_tuple__ = version_tuple = (3, 0, 5)
```

## Comparing `kelvin_sdk_pubsub-3.0.4.dist-info/METADATA` & `kelvin_sdk_pubsub-3.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kelvin-sdk-pubsub
-Version: 3.0.4
+Version: 3.0.5
 Summary: Kelvin Pub-Sub Client
 Home-page: https://kelvininc.com/
 Author: Kelvin Inc
 Author-email: engineering@kelvininc.com
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `kelvin_sdk_pubsub-3.0.4.dist-info/RECORD` & `kelvin_sdk_pubsub-3.0.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 kelvin/sdk/pubsub/__init__.py,sha256=bh0J3qAcQVxlaLBhlZX1SH1AQx0vAuu0klD0ehVSwOM,473
 kelvin/sdk/pubsub/client.py,sha256=NJX2ru0DdL8PSfFmY9pMbHhYRrbFg63ZZLDKnuBr9-Q,1946
 kelvin/sdk/pubsub/config.py,sha256=PvXQ_3hUDny4bg9PkAI45IMY0J5W_pDP4MIYVkV32IU,19399
-kelvin/sdk/pubsub/connection.py,sha256=vfBJo606tMiyo4H8mVZUxvnEHW9nrMUlnR0_quDEOq8,21039
+kelvin/sdk/pubsub/connection.py,sha256=ajBOBAnaCo6idFYmvzVNKH9qbqR-ns-a__CuYO5VS2c,21673
 kelvin/sdk/pubsub/error.py,sha256=muFeb6nK3hm8VBjv_ErFYvRJdmJ4uNeLSYmpgSSA-IU,149
 kelvin/sdk/pubsub/prometheus.py,sha256=LbJfB6YVOrry2YwXlo9IjO8pbzGcsK873xGrBp5Id00,1988
 kelvin/sdk/pubsub/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kelvin/sdk/pubsub/types.py,sha256=-vGsE8NX4FpFmkI7FDa4Oy3nbTH0qIfhAsOOQbMRWYk,5438
 kelvin/sdk/pubsub/utils.py,sha256=JqsTPzuAEqHZd7Y1FqUYSqMq6cvqKd67fOjlQWjTfKY,740
-kelvin/sdk/pubsub/version.py,sha256=yyqcyuVbO5Bq7rMS_oAT4a92vlOM2Jk4fCNagNkWYJk,411
-kelvin_sdk_pubsub-3.0.4.dist-info/METADATA,sha256=KuwubBNfldCnYNHrwJOVIIcwpEPzYltJRjiPOF8pFsU,3009
-kelvin_sdk_pubsub-3.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-kelvin_sdk_pubsub-3.0.4.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
-kelvin_sdk_pubsub-3.0.4.dist-info/RECORD,,
+kelvin/sdk/pubsub/version.py,sha256=NqRbOVcxQkddLTmShuqlFBHUHHK5PYebiY46i5lZ5Uc,411
+kelvin_sdk_pubsub-3.0.5.dist-info/METADATA,sha256=rSB742aqLVrs61EhwB_bGt43VYPoR78fDC1pez8_NnU,3009
+kelvin_sdk_pubsub-3.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kelvin_sdk_pubsub-3.0.5.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
+kelvin_sdk_pubsub-3.0.5.dist-info/RECORD,,
```

