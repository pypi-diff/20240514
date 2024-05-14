# Comparing `tmp/omuplugin_onecomme-0.3.1.tar.gz` & `tmp/omuplugin_onecomme-0.3.2.tar.gz`

## Comparing `omuplugin_onecomme-0.3.1.tar` & `omuplugin_onecomme-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/src/omuplugin_onecomme/__init__.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/src/omuplugin_onecomme/onecomme.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/src/omuplugin_onecomme/plugin.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/src/omuplugin_onecomme/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/README.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/__init__.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/onecomme.py
+-rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/plugin.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/types.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/README.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/PKG-INFO
```

### Comparing `omuplugin_onecomme-0.3.1/src/omuplugin_onecomme/onecomme.py` & `omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/types.py`

 * *Files identical despite different names*

### Comparing `omuplugin_onecomme-0.3.1/src/omuplugin_onecomme/plugin.py` & `omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import asyncio
+import socket
 from html import escape
 from typing import TypedDict
 
 from aiohttp import web
 from loguru import logger
 from omuchat import App, Client, events, model
 from omuchat.model import content
 
-from .onecomme import Badge, Comment, CommentData, CommentServiceData
+from .types import Badge, Comment, CommentData, CommentServiceData
 
 APP = App(
     "cc.omuchat:onecomme/plugin",
     version="0.1.0",
 )
 client = Client(APP)
 app = web.Application()
@@ -115,19 +116,20 @@
 async def handle(request: web.Request) -> web.WebSocketResponse:
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     messages = [
         await to_comment(message)
         for message in (await client.chat.messages.fetch_items(before=35)).values()
     ]
-
     await ws.send_json(
         {
             "type": "connected",
-            "data": CommentsData(comments=[message for message in messages if message]),
+            "data": CommentsData(
+                comments=list(reversed(tuple(filter(None, messages))))
+            ),
         }
     )
     sessions.add(ws)
     try:
         async for msg in ws:
             if msg.type == web.WSMsgType.TEXT:
                 pass
@@ -172,18 +174,36 @@
 
 @client.on(events.message.remove)
 async def on_message_delete(message: model.Message) -> None:
     for ws in sessions:
         await ws.send_json({"type": "deleted", "data": [message.key()]})
 
 
+def is_port_free() -> bool:
+    try:
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+            s.bind(
+                (
+                    "localhost",
+                    11180,
+                )
+            )
+            return True
+    except OSError:
+        return False
+
+
 @client.on(events.ready)
 async def on_ready():
+    port_free = is_port_free()
+    if not port_free:
+        raise OSError("Port 11180 already in use")
     app.add_routes([web.get("/sub", handle)])
     runner = web.AppRunner(app)
     await runner.setup()
     site = web.TCPSite(runner, "localhost", 11180)
     asyncio.create_task(site.start())
+    logger.info("OneComme server started")
 
 
 if __name__ == "__main__":
     client.run()
```

### Comparing `omuplugin_onecomme-0.3.1/pyproject.toml` & `omuplugin_onecomme-0.3.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_onecomme"
-version = "0.3.1"
+version = "0.3.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

