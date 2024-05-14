# Comparing `tmp/nonebot_adapter_tailchat-0.1.0b7.tar.gz` & `tmp/nonebot_adapter_tailchat-0.1.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b7.tar", max compression
+gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b8.tar", max compression
```

## Comparing `nonebot_adapter_tailchat-0.1.0b7.tar` & `nonebot_adapter_tailchat-0.1.0b8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11335 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/LICENSE
--rw-r--r--   0        0        0     1488 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/README.md
--rw-r--r--   0        0        0      260 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/__init__.py
--rw-r--r--   0        0        0     7316 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/adapter.py
--rw-r--r--   0        0        0    24554 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/api.py
--rw-r--r--   0        0        0     8081 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bbcode.py
--rw-r--r--   0        0        0     5415 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bot.py
--rw-r--r--   0        0        0      675 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/config.py
--rw-r--r--   0        0        0      158 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/const.py
--rw-r--r--   0        0        0    11139 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/event.py
--rw-r--r--   0        0        0     1517 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/exception.py
--rw-r--r--   0        0        0    11160 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/message.py
--rw-r--r--   0        0        0     5976 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/model.py
--rw-r--r--   0        0        0      374 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/permission.py
--rw-r--r--   0        0        0      456 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/rule.py
--rw-r--r--   0        0        0     2103 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/util.py
--rw-r--r--   0        0        0     1407 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/pyproject.toml
--rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b7/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/LICENSE
+-rw-r--r--   0        0        0     1786 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/README.md
+-rw-r--r--   0        0        0      260 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/__init__.py
+-rw-r--r--   0        0        0     7279 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/adapter.py
+-rw-r--r--   0        0        0    24793 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/api.py
+-rw-r--r--   0        0        0     8185 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bbcode.py
+-rw-r--r--   0        0        0     4249 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bot.py
+-rw-r--r--   0        0        0      675 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/config.py
+-rw-r--r--   0        0        0      158 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/const.py
+-rw-r--r--   0        0        0    14519 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/event.py
+-rw-r--r--   0        0        0     1517 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/exception.py
+-rw-r--r--   0        0        0    16040 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/message.py
+-rw-r--r--   0        0        0     5976 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/model.py
+-rw-r--r--   0        0        0      374 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/permission.py
+-rw-r--r--   0        0        0      470 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/rule.py
+-rw-r--r--   0        0        0     2103 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/util.py
+-rw-r--r--   0        0        0     1423 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b8/PKG-INFO
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/LICENSE` & `nonebot_adapter_tailchat-0.1.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b7/README.md` & `nonebot_adapter_tailchat-0.1.0b8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 <div align="center">
 
 # Nonebot Adapter Tailchat
 
 ## Tailchat 适配器
 
-![License](https://img.shields.io/github/license/eya46/nonebot-adapter-tailchat)
-![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
-![NoneBot](https://img.shields.io/badge/nonebot-2.3.0+-red.svg)
+[![License](https://img.shields.io/github/license/eya46/nonebot-adapter-tailchat)](https://github.com/eya46/nonebot-adapter-tailchat/blob/master/LICENSE)
+[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)](https://docs.python.org/zh-cn/3.9/library/index.html)
+[![NoneBot](https://img.shields.io/badge/nonebot-2.3.0+-red.svg)](https://nonebot.dev)
+[![Tailchat](https://img.shields.io/badge/Tailchat-1.11.3+-blue.svg)](https://tailchat.msgbyte.com)
 </div>
 
 ## 环境要求
 
+- Tailchat >= 1.11.3
+    - api: `getMessage`
 - Python 3.9+
 - NoneBot 2.3.0+
 - pydantic >= 2.0.0
 - HTTPClient驱动器
     - > 默认需要,除非 `useHttp=False`, 且配置了 `jwt`
     - ~httpx
     - ~aiohttp
@@ -52,13 +55,14 @@
 ```
 
 ## 详细配置项
 
 [config.py](./nonebot_adapter_tailchat/config.py)
 
 ## 相关项目
+
 - [dcwatson/bbcode](https://github.com/dcwatson/bbcode)
 - [Tailchat](https://github.com/msgbyte/tailchat)
 - [python-socketio](https://github.com/miguelgrinberg/python-socketio)
 - [nonebot2](https://github.com/nonebot/nonebot2)
 - [pydantic2](https://docs.pydantic.dev/latest/)
 - ...
```

#### html2text {}

```diff
@@ -1,19 +1,23 @@
                                    _[_n_o_n_e_b_o_t_]
-     # Nonebot Adapter Tailchat ## Tailchat ééå¨ ![License](https://
-img.shields.io/github/license/eya46/nonebot-adapter-tailchat) ![Python](https:/
-/img.shields.io/badge/python-3.9+-blue.svg) ![NoneBot](https://img.shields.io/
-                         badge/nonebot-2.3.0+-red.svg)
-## ç¯å¢è¦æ± - Python 3.9+ - NoneBot 2.3.0+ - pydantic >= 2.0.0 -
-HTTPClienté©±å¨å¨ - > é»è®¤éè¦,é¤é `useHttp=False`, ä¸éç½®äº `jwt`
-- ~httpx - ~aiohttp ## Tailchatæºå¨äººå¼å¯æ¹å¼ 1. å®è£
-`å¼æ¾å¹³å°æä»¶` 2. è¿å¥ `è®¾ç½®` -> `å¼æ¾å¹³å°` -> `åå»ºåºç¨` -
-> `å¡«ååºæ¬ä¿¡æ¯` 3. è¿å¥ `åºç¨` -> `æºå¨äºº` -
-> `å¼å¯æºå¨äººè½å` 4. å¨ `åºæ¬ä¿¡æ¯` åè·å `appId` å
-`appSecret` > ææªæ¯æ `æ¶æ¯åè°å°å` ## éç½®æ¹å¼ `.env` æä»¶
-```dotenv TAILCHAT_BOTS=' [ { "url": "https://xxxxxxx/", "appId": "ts_******",
-"appSecret": "****" } ] ' TAILCHAT_RECONNECT_INTERVAL=5 TAILCHAT_TIME_OUT=5 ```
-## è¯¦ç»éç½®é¡¹ [config.py](./nonebot_adapter_tailchat/config.py) ##
-ç¸å³é¡¹ç® - [dcwatson/bbcode](https://github.com/dcwatson/bbcode) -
-[Tailchat](https://github.com/msgbyte/tailchat) - [python-socketio](https://
-github.com/miguelgrinberg/python-socketio) - [nonebot2](https://github.com/
-nonebot/nonebot2) - [pydantic2](https://docs.pydantic.dev/latest/) - ...
+     # Nonebot Adapter Tailchat ## Tailchat ééå¨ [![License](https://
+    img.shields.io/github/license/eya46/nonebot-adapter-tailchat)](https://
+   github.com/eya46/nonebot-adapter-tailchat/blob/master/LICENSE) [![Python]
+ (https://img.shields.io/badge/python-3.9+-blue.svg)](https://docs.python.org/
+zh-cn/3.9/library/index.html) [![NoneBot](https://img.shields.io/badge/nonebot-
+  2.3.0+-red.svg)](https://nonebot.dev) [![Tailchat](https://img.shields.io/
+        badge/Tailchat-1.11.3+-blue.svg)](https://tailchat.msgbyte.com)
+## ç¯å¢è¦æ± - Tailchat >= 1.11.3 - api: `getMessage` - Python 3.9+ -
+NoneBot 2.3.0+ - pydantic >= 2.0.0 - HTTPClienté©±å¨å¨ - >
+é»è®¤éè¦,é¤é `useHttp=False`, ä¸éç½®äº `jwt` - ~httpx - ~aiohttp ##
+Tailchatæºå¨äººå¼å¯æ¹å¼ 1. å®è£ `å¼æ¾å¹³å°æä»¶` 2. è¿å¥ `è®¾ç½®`
+-> `å¼æ¾å¹³å°` -> `åå»ºåºç¨` -> `å¡«ååºæ¬ä¿¡æ¯` 3. è¿å¥ `åºç¨`
+-> `æºå¨äºº` -> `å¼å¯æºå¨äººè½å` 4. å¨ `åºæ¬ä¿¡æ¯` åè·å
+`appId` å `appSecret` > ææªæ¯æ `æ¶æ¯åè°å°å` ## éç½®æ¹å¼
+`.env` æä»¶ ```dotenv TAILCHAT_BOTS=' [ { "url": "https://xxxxxxx/", "appId":
+"ts_******", "appSecret": "****" } ] ' TAILCHAT_RECONNECT_INTERVAL=5
+TAILCHAT_TIME_OUT=5 ``` ## è¯¦ç»éç½®é¡¹ [config.py](./
+nonebot_adapter_tailchat/config.py) ## ç¸å³é¡¹ç® - [dcwatson/bbcode](https:/
+/github.com/dcwatson/bbcode) - [Tailchat](https://github.com/msgbyte/tailchat)
+- [python-socketio](https://github.com/miguelgrinberg/python-socketio) -
+[nonebot2](https://github.com/nonebot/nonebot2) - [pydantic2](https://
+docs.pydantic.dev/latest/) - ...
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/adapter.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,43 +5,40 @@
 from traceback import print_exc
 from typing import Any, Optional
 
 from nonebot import escape_tag, get_plugin_config
 from nonebot.adapters import Adapter as BaseAdapter
 from nonebot.drivers import Driver
 from nonebot.internal.driver import ContentTypes, HTTPClientMixin, Request, Response
-from typing_extensions import override
+from nonebot.message import handle_event
 from yarl import URL
 
 from .bot import Bot
 from .config import BotInfo, Config
 from .const import ADAPTER_NAME, Undefined
 from .event import get_event
 from .exception import ConnectionException, DisconnectException, get_error
 from .message import Message
 from .util import log, retry
 
 
 class Adapter(BaseAdapter):
-    @override
     def __init__(self, driver: Driver, **kwargs: Any):
         super().__init__(driver, **kwargs)
         self.adapter_config: Config = get_plugin_config(Config)
         self.tasks = []
         self.on_ready(self._setup)
         self.on_ready(Message.update_parser)
         self.driver.on_shutdown(self._shutdown)
         self.is_http_client_driver = isinstance(self.driver, HTTPClientMixin)
 
     @classmethod
-    @override
     def get_name(cls) -> str:
         return ADAPTER_NAME
 
-    @override
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         use_http = data.get("use_http_", bot.base_info.useHttp)  # 使用http
         use_sio = data.get("use_sio_", not use_http)  # 使用socketio
         use_api = data.get("use_api_", True)  # url / 'api' / api
         if not bot.base_info.useHttp and (not use_sio or use_http):
             log("WARNING", f"use_http is False, but api <y>{api}</y> use / strictly.")
         if use_http or not use_sio:
@@ -148,15 +145,15 @@
 
     @staticmethod
     async def _handle_event(bot: Bot, event: str, data: dict, _: Optional[any] = None):
         model = get_event(event)
         log.trace(f"Event: {event}, MatchModel: {model}, Data: {data}")
         data["event_name"] = data.get("event_name", event)
         data["self_id"] = data.get("self_id", bot.self_id)
-        await bot.handle_event(model.model_validate(data))
+        await handle_event(bot, await model.build(bot, data))
 
     @staticmethod
     def _loads(data: ContentTypes) -> Any:
         try:
             return json.loads(data)
         except json.JSONDecodeError:
             log.error("Error when loads data", escape_tag(data.decode() if isinstance(data, bytes) else str(data)))
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/api.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,20 @@
     async def clearInbox(self):
         """清空所有的收件箱内容"""
         return await self.call_api("chat.inbox.clear")
 
     async def setAppInfo(self, *, appId: str, fieldName: str, fieldValue: str):
         return await self.call_api("openapi.app.setAppInfo", appId=appId, fieldName=fieldName, fieldValue=fieldValue)
 
+    async def getMessage(self, *, messageId: str) -> MessageRet:
+        """获取消息"""
+        return TypeAdapter(MessageRet).validate_python(
+            await self.call_api("chat.message.getMessage", messageId=messageId)
+        )
+
     async def addConverse(self, *, converseId: str):
         return await self.call_api("user.dmlist.addConverse", converseId=converseId)
 
     async def addReaction(self, *, emoji: str, messageId: str):
         """添加消息表情"""
         return await self.call_api("chat.message.addReaction", emoji=emoji, messageId=messageId)
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bbcode.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bbcode.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
 from collections import OrderedDict, defaultdict, deque
 from shlex import split
 from sys import getrecursionlimit
 from typing import TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
-    from .message import B, MessageSegment
+    from .message import BBCODE, MessageSegment
 
 
 class Parser:
     def __init__(
         self,
         seg: type["MessageSegment"],
-        tags: dict[str, type["B"]],
+        tags: dict[str, type["BBCODE"]],
         drop_unrecognized=False,
         max_tag_depth=None,
     ):
         self.seg = seg
         self.tag_opener = "["
         self.tag_closer = "]"
         self.tags = tags
@@ -136,25 +136,27 @@
                     if valid and tag_name in self.tags:
                         if closer:
                             if len(tags[tag_name]) == 0:  # 未找到对应的开始标签
                                 tokens.append(self.seg.text(tag))
                                 continue
                             # 从右到左, 找到第一个匹配的未闭合的标签, 找到后将其闭合
                             # 期间的表判断 1. tags为空 则加入其中
-                            # 2. 有tag, 判断relation, 如果不相同的relation则把其中tag变成text, 并加入tag.
+                            # 2. 有tag, 判断relation, 如果不相同的relation/重复的BBCode 则把其中tag变成text, 并加入tag.
                             #   相同则直接加入tag
                             tag_start = tags[tag_name].pop()
-                            bbcode_start = tag_start.data["tags"][0]
+                            bbcode_start = tag_start.tags[0]
                             for i in tokens[::-1]:
                                 if isinstance(i, self.seg):  # 是纯文本
-                                    if len(i.data["tags"]) == 0:
+                                    if len(i.tags) == 0:
                                         i.extend(tag_start)
                                     else:
-                                        if any(_.relation != bbcode_start.relation for _ in i.data["tags"][:]):
-                                            for _ in i.data["tags"][::-1]:
+                                        if bbcode_start in i.tags or any(
+                                            _.relation != bbcode_start.relation for _ in i.tags
+                                        ):
+                                            for _ in i.tags[::-1]:
                                                 i.down(_)
                                         i.extend(tag_start)
                                 else:  # 是标签
                                     _tag_name = i[1]
                                     if _tag_name == tag_name:
                                         tokens.remove(i)
                                         break
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bot.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from base64 import urlsafe_b64decode
 from functools import wraps
 from hashlib import md5
 from json import loads
 from time import time
 from typing import TYPE_CHECKING, Optional, Union
 
-from nonebot.message import handle_event
 from pydantic import TypeAdapter
 from socketio import AsyncClient as AsyncSocketClient
-from typing_extensions import override
 
 from .api import API
 from .config import BotInfo
 from .event import Event, MessageEvent
-from .message import At, Message, MessageSegment
+from .message import Message, MessageSegment
 from .model import (
     BaseBotInfo,
     JwtPayload,
     MessageRet,
     TokenInfo,
 )
-from .util import log
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
 def _with_update_info(func):
     @wraps(func)
@@ -43,41 +40,14 @@
     async def connect(self):
         return await self.sio.connect(
             url=self.url,
             auth={"token": self.base_info.jwt},
             transports=["websocket"],
         )
 
-    async def _check_is_to_me(self, event: Event):
-        try:
-            message: Message = event.get_message()
-            # at
-            seg: MessageSegment = message[0]
-            if seg.type == At.__name__.lower():
-                if seg.get_tag(At).main == event.self_id:
-                    event._isToMe = True
-                    message.pop(0)
-                return
-            # nickname
-            if seg.type == "text":
-                text = seg.get_text().strip()
-                for i in self.config.nickname:
-                    if text.startswith(i):
-                        event._isToMe = True
-                        if len(text) == len(i):
-                            message.pop(0)
-                        else:
-                            seg.data["text"] = text[len(i) :]
-        except Exception as e:
-            log.debug(f"Bot._check_is_to_me error: {e}")
-
-    async def handle_event(self, event: Event) -> None:
-        await self._check_is_to_me(event)
-        await handle_event(self, event)
-
     @staticmethod
     def md5(text: str) -> str:
         return md5(text.encode()).hexdigest()
 
     @staticmethod
     def decode_jwt(jwt: str) -> tuple[dict, JwtPayload, str]:
         segments = jwt.split(".")
@@ -98,23 +68,21 @@
 
     async def update_info(self, jwt: Optional[str]):
         jwt = jwt or self.base_info.jwt
         self.info = await self.resolveToken(token=jwt)
         self.base_info.jwt = jwt
         self.self_id = self.info.userId
 
-    @override
     def __init__(self, adapter: "Adapter", self_id: str, base_info: BotInfo):
         super().__init__(adapter, self_id)
         self.url = str(base_info.url)
         self.base_info = base_info
         self.sio = AsyncSocketClient(serializer="msgpack")
         self.info: Optional[TokenInfo] = None
 
-    @override
     async def send(
         self,
         event: Event,
         message: Union[str, Message, MessageSegment],
         encode: bool = False,
         **kwargs,
     ) -> MessageRet:
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/config.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/event.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,116 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Literal, Optional, TypeVar, Union, get_args
+from typing import TYPE_CHECKING, Literal, Optional, TypeVar, Union, cast, get_args
 
 from nonebot.adapters import Event as BaseEvent
 from nonebot.compat import model_dump
 from pydantic import Field
 from pydantic_core import PydanticUndefined
-from typing_extensions import override
+from typing_extensions import Self
 
-from .message import Message
+from .message import At, Message, MessageSegment
 from .model import (
     Announcement,
     ConverseType,
     GroupInfo,
     MessageMeta,
+    MessageRet,
     ObjectId,
     Payload,
     Reaction,
     Replay,
     StaticAnnouncement,
     datetime,
 )
+from .util import log
 
 if TYPE_CHECKING:
     from .bot import Bot
 
 
 class Event(BaseEvent, ABC):
     event_name: str
     event_type: str
 
     self_id: ObjectId
 
     _isToMe: bool = False
 
-    @override
     def get_type(self) -> str:
         return self.event_type
 
-    @override
     def get_event_name(self) -> str:
         return self.event_name
 
-    @override
     def get_event_description(self) -> str:
         return str(model_dump(self))
 
-    @override
     def is_tome(self) -> bool:
         return not self.is_self() and (self._isToMe or self._is_tome)
 
     @property
     @abstractmethod
     def _is_tome(self) -> bool:
         return True
 
     def is_self(self) -> bool:
         return self.self_id == self.get_user_id()
 
+    async def _get_message(self, bot: "Bot" = None) -> Message:
+        return self.get_message()
+
+    @classmethod
+    async def build(cls, bot: "Bot", obj: dict) -> Self:
+        event = cls.model_validate(obj)
+        try:
+            message: Message = await event._get_message(bot)
+            # at
+            seg: MessageSegment = message[0]
+            if seg.type == At.__name__.lower():
+                if seg.get_tag(At).main == event.self_id:
+                    event._isToMe = True
+                    message.pop(0)
+            # nickname
+            elif seg.type == "text":
+                text = seg.get_text().strip()
+                for i in bot.config.nickname:
+                    if text.startswith(i):
+                        event._isToMe = True
+                        if len(text) == len(i):
+                            message.pop(0)
+                        else:
+                            seg.data["text"] = text[len(i) :]
+        except Exception as e:
+            log.debug(f"Event.build error: {e}")
+        return event
+
 
 class NoticeEvent(Event, ABC):
     event_type: Literal["notice"] = "notice"
 
     def get_message(self) -> Message:
         raise ValueError("Event has no message!")
 
     def get_session_id(self) -> str:
         raise ValueError("Event has no context!")
 
 
 class RequestEvent(Event, ABC):
     event_type: Literal["request"] = "request"
 
-    @override
     def get_session_id(self) -> str:
         raise ValueError("Event has no context!")
 
-    @override
     def get_message(self) -> Message:
         raise ValueError("Event has no context!")
 
 
 class MessageEvent(Event, ABC):
     event_type: Literal["message"] = "message"
 
-    @override
     def get_plaintext(self) -> str:
         return self.get_message().extract_plain_text()
 
     @abstractmethod
     def get_message_id(self) -> str:
         raise NotImplementedError
 
@@ -178,16 +201,15 @@
     createdAt: datetime
     updatedAt: datetime
 
     v: int = Field(alias="__v")
 
     @property
     def _is_tome(self) -> bool:
-        # TODO: 判断是否是自己
-        return False
+        return True
 
     def get_user_id(self) -> str:
         raise ValueError("Event has no context!")
 
 
 @register_event_class
 class MessageDeleteEvent(NoticeEvent):
@@ -250,40 +272,124 @@
     event_name: Literal["notify:group.updateInfo"]
 
     def get_user_id(self) -> str:
         # TODO: ...
         raise ValueError("Event has no context!")
 
 
-class ReactionEvent(NoticeEvent):
+class DefaultReactionEvent(NoticeEvent):
     converseId: ObjectId
     messageId: ObjectId
     reaction: Reaction
 
+    message: Optional[MessageRet] = None
+    content: Optional[Message] = None
+
     def get_user_id(self) -> str:
         return self.reaction.author
 
     @property
     def _is_tome(self) -> bool:
-        # TODO: ...
+        if self.message:
+            return self.message.author == self.self_id
         return False
 
     def get_session_id(self) -> str:
         return f"{self.converseId}:{self.messageId}:{self.reaction.author}"
 
+    def is_group(self) -> bool:
+        if self.message is None:
+            raise ValueError("Event has no context!")
+        return not not self.message.groupId
+
+    def get_message(self) -> Message:
+        if self.content:
+            return self.content
+        return super().get_message()
+
+    async def _get_message(self, bot: Optional["Bot"] = None) -> Message:
+        if self.content:
+            return self.content
+        if self.message:
+            self.content = Message(self.message.content)
+            return self.content
+        if bot:
+            self.message = await bot.getMessage(messageId=self.messageId)
+            self.content = Message(self.message.content)
+            return self.content
+        raise ValueError("Event has no context!")
+
 
 @register_event_class
-class ReactionAddEvent(ReactionEvent):
+class DefaultReactionAddEvent(DefaultReactionEvent):
     event_name: Literal["notify:chat.message.addReaction"]
 
+    @classmethod
+    async def build(cls, bot: "Bot", obj: dict) -> Self:
+        event = cast(cls, await super().build(bot, obj))
+        if event.message is None:
+            return event
+        if event.is_group():
+            return GroupReactionAddEvent.model_validate(dict(event))
+        return PrivateReactionAddEvent.model_validate(dict(event))
+
+
+class PrivateReactionAddEvent(DefaultReactionAddEvent):
+    message: MessageRet
+    content: Message
+
+    def is_group(self) -> bool:
+        return False
+
+
+class GroupReactionAddEvent(DefaultReactionAddEvent):
+    message: MessageRet
+    content: Message
+
+    def is_group(self) -> bool:
+        return True
+
+    @property
+    def groupId(self) -> ObjectId:
+        return self.message.groupId
+
 
 @register_event_class
-class ReactionRemoveEvent(ReactionEvent):
+class DefaultReactionRemoveEvent(DefaultReactionEvent):
     event_name: Literal["notify:chat.message.removeReaction"]
 
+    @classmethod
+    async def build(cls, bot: "Bot", obj: dict) -> Self:
+        event = cast(cls, await super().build(bot, obj))
+        if event.message is None:
+            return event
+        if event.is_group():
+            return GroupReactionRemoveEvent.model_validate(dict(event))
+        return PrivateReactionRemoveEvent.model_validate(dict(event))
+
+
+class PrivateReactionRemoveEvent(DefaultReactionRemoveEvent):
+    message: MessageRet
+    content: Message
+
+    def is_group(self) -> bool:
+        return False
+
+
+class GroupReactionRemoveEvent(DefaultReactionRemoveEvent):
+    message: MessageRet
+    content: Message
+
+    def is_group(self) -> bool:
+        return True
+
+    @property
+    def groupId(self) -> ObjectId:
+        return self.message.groupId
+
 
 class DefaultMessageEvent(MessageEvent):
     id: ObjectId = Field(alias="_id")
     author: ObjectId
     hasRecall: bool
     converseId: ObjectId
     meta: Optional[MessageMeta] = Field(default=None)
@@ -305,31 +411,28 @@
     def get_group_id(self) -> Optional[str]:
         return self.groupId
 
     @property
     def replay(self) -> Optional[Replay]:
         return self.meta.replay if self.meta else None
 
-    @override
     def get_message(self) -> Message:
         return self.content
 
-    @override
     def get_user_id(self) -> str:
         return self.author
 
     def _is_tome(self) -> bool:
         # 私聊/提及/回复
         return (
             not self.is_group()
             or (self.meta and self.self_id in self.meta.mentions)
             or (self.meta and self.meta.replay and self.self_id == self.meta.replay.author)
         )
 
-    @override
     def get_event_description(self) -> str:
         return (
             f"Message {self.id} from {self.author}"
             + (f"@[群:{self.groupId}]" if self.groupId else "")
             + f" {self.content.show()}"
         )
 
@@ -382,19 +485,17 @@
 
     def is_group(self):
         return not not self.payload.groupId
 
     def _is_tome(self) -> bool:
         return True
 
-    @override
     def get_user_id(self) -> str:
         return self.payload.messageAuthor
 
-    @override
     def get_event_description(self) -> str:
         return (
             f"AtMessage {self.payload.messageId} from {self.payload.messageAuthor}"
             + (f"@[群:{self.get_group_id()}]" if self.payload.groupId else "")
             + f" {self.payload.messageSnippet.show()}"
         )
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/exception.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/message.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from abc import ABC
 from collections import UserDict, defaultdict, deque
 from collections.abc import Iterable
 from dataclasses import dataclass
 from functools import wraps
-from typing import Optional, TypedDict, TypeVar, Union
+from inspect import isclass
+from typing import Optional, SupportsIndex, TypedDict, TypeVar, Union
 
 from nonebot.adapters import (
     Message as BaseMessage,
 )
 from nonebot.adapters import (
     MessageSegment as BaseMessageSegment,
 )
-from typing_extensions import Self, override
+from typing_extensions import Self, overload
 
 from .bbcode import Parser
 
-B = TypeVar("B", bound="BBCode")
-BBCODES: dict[str, type[B]] = {}
-RELATION: dict[int, list[B]] = defaultdict(list)
+BBCODE = TypeVar("BBCODE", bound="BBCode")
+BBCODES: dict[str, type[BBCODE]] = {}
+RELATION: dict[int, list[BBCODE]] = defaultdict(list)
 
 
-def _register_bbcode(code: Union[int, type[B]]):
+def _register_bbcode(code: Union[int, type[BBCODE]]):
     if isinstance(code, int):
 
-        def _(bbcode: type[B]) -> type[B]:
+        def _(bbcode: type[BBCODE]) -> type[BBCODE]:
             bbcode.relation = code
             for tag in bbcode.tags:
                 BBCODES[tag] = bbcode
             RELATION[code].append(bbcode)
             return bbcode
 
         return _
@@ -38,15 +39,15 @@
     RELATION[_code].append(code)
     return code
 
 
 class Box(TypedDict):
     text: str
     extra: dict[str, str]
-    tags: list[B]
+    tags: list[type[BBCODE]]
 
 
 class BBCode(UserDict, ABC):
     relation: int
     keys_: set[str] = set()
     tags: set[str]
 
@@ -81,25 +82,40 @@
 
     @property
     def tail(self) -> str:
         return f"[/{self.tag}]"
 
     @classmethod
     def tag_in(cls, msg: Union["MessageSegment", "Message"]) -> bool:
-        if isinstance(msg, MessageSegment):
-            return any(isinstance(_, cls) for _ in msg.data["tags"])
+        if isinstance(msg, Message):
+            for seg in msg:  # 递归
+                if cls.tag_in(seg):
+                    return True
+            return False
+        if cls == BBCode:  # 是BBCode
+            return len(msg.tags) > 0
+        elif isclass(cls):  # 子类
+            return cls in msg.tags
+        else:  # 实例化子类
+            # 参数相同 + 在tags中
+            return msg.extra | cls.data == msg.extra and type(cls) in msg.tags
 
-        return any(BBCode.tag_in(_) for _ in msg)
+    @classmethod
+    def decode(cls, box: Box) -> str:
+        return str(cls(box=box))
 
     def __str__(self):
         return self.head + self.text + self.tail
 
     def __repr__(self):
         return f"{self.tag}({self.data})" if len(self.data) else f"{self.tag}"
 
+    def __missing__(self, key) -> None:
+        return None
+
 
 @_register_bbcode
 class Markdown(BBCode):
     tags = {"md", "markdown"}
 
 
 @_register_bbcode
@@ -128,30 +144,30 @@
 
 @_register_bbcode
 class Emoji(BBCode):
     tags = {"emoji"}
 
 
 @_register_bbcode(0)
-class Bold(BBCode):
+class B(BBCode):
     tags = {"b"}
 
 
 @_register_bbcode(0)
-class Italic(BBCode):
+class I(BBCode):
     tags = {"i"}
 
 
 @_register_bbcode(0)
-class Underline(BBCode):
+class U(BBCode):
     tags = {"u"}
 
 
 @_register_bbcode(0)
-class Strikeout(BBCode):
+class S(BBCode):
     tags = {"s"}
 
 
 @_register_bbcode
 class At(BBCode):
     tags = {"at"}
     keys_ = {"at"}
@@ -187,29 +203,26 @@
 
 
 @dataclass
 class MessageSegment(BaseMessageSegment["Message"]):
     data: Box
 
     @classmethod
-    @override
     def get_message_class(cls) -> type["Message"]:
         return Message
 
-    @override
     def __str__(self) -> str:
         return self.data["text"]
 
     def get_text(self) -> str:
         return self.data["text"]
 
     def set_text(self, text: str):
         self.data["text"] = text
 
-    @override
     def is_text(self) -> bool:
         return self.type == "text"
 
     @classmethod
     def card(cls, *, text: str, type_: str, data: str) -> Self:
         return cls.build(text, [Card], {"type": type_, "data": data})
 
@@ -232,23 +245,23 @@
 
     @classmethod
     def code(cls, text: str) -> Self:
         return cls.build(text, [Code])
 
     @classmethod
     def text(cls, text: str, *, b: bool = False, i: bool = False, u: bool = False, s: bool = False) -> Self:
-        _: list[type[B]] = []
+        _: list[type[BBCODE]] = []
         if b:
-            _.append(Bold)
+            _.append(B)
         if i:
-            _.append(Italic)
+            _.append(I)
         if u:
-            _.append(Underline)
+            _.append(U)
         if s:
-            _.append(Strikeout)
+            _.append(S)
         return cls.build(text, _)
 
     @classmethod
     def emoji(cls, text: str) -> Self:
         return cls.build(text, [Emoji])
 
     @classmethod
@@ -258,170 +271,291 @@
         return cls.build(url, [Img], {"width": width, "height": height})
 
     @classmethod
     def md(cls, text: str) -> Self:
         return cls.build(text, [Markdown])
 
     @classmethod
-    def build(cls, text: str, tags: list[type[B]], extra: Optional[dict[str, str]] = None) -> Self:
+    def build(cls, text: str, tags: list[type[BBCODE]], extra: Optional[dict[str, str]] = None) -> Self:
         if extra is None:
             extra = {}
         if (length := len(tags)) == 0:
             type_ = "text"
         elif length == 1:
             type_ = tags[0].__name__.lower()
         else:
             type_ = "rich"
 
         _ = cls(
             type_,
             {"text": text, "extra": extra, "tags": []},
         )
-        for tag in tags:
-            _.data["tags"].append(tag(box=_.data))
+        _.data["tags"] = tags
         return _
 
     def tag_relation(self) -> set[int]:
-        return {_.relation for _ in self.data["tags"]}
+        return {_.relation for _ in self.tags}
 
     def merge_text(self, seg: Union[str, Self]) -> Self:
         self.data["text"] += seg if isinstance(self, str) else seg.get_text()
         return self
 
     def extend(self, seg: Self, strict: bool = True) -> Self:
         """
         新消息段的 text = self.text or seg.text
         :param seg: 要合并的消息段
         :param strict: 严格模式
         :return: 新消息段
         """
-        if strict and (relations := self.tag_relation()) and any(_.relation not in relations for _ in seg.data["tags"]):
+        if strict and (relations := self.tag_relation()) and any(_.relation not in relations for _ in seg.tags):
             raise ValueError("Tag relation not match")
 
         if self.type == "text":
             self.type = seg.type
         elif self.type != "rich":
             self.type = "rich"
 
-        self.data["extra"].update(seg.data["extra"])
-        for idx, tag in enumerate(seg.data["tags"]):
-            seg.data["tags"][idx] = tag.__class__(box=self.data)
-        self.data["tags"].extend(seg.data["tags"])
+        self.extra.update(seg.extra)
+        self.tags.extend(seg.tags)
         self.set_text(self.get_text() or seg.get_text())
         return self
 
-    def remove(self, bbcode: Union[B, type[B]]) -> Self:
-        if bbcode is type[B]:
-            bbcode: B = self.get_tag(bbcode)
-        self.data["tags"].remove(bbcode)
+    def remove(self, bbcode: Union[BBCODE, type[BBCODE]]) -> Self:
         for _ in bbcode.keys_ | bbcode.tags:
-            self.data["extra"].pop(_, _)
-
+            self.extra.pop(_, _)
+        self.tags.remove(bbcode if isclass(bbcode) else type(bbcode))
         return self
 
-    def down(self, bbcode: Union[B, type[B]]) -> Self:
+    def down(self, bbcode: Union[BBCODE, type[BBCODE]]) -> Self:
         """把bbcode变为文本"""
-        if bbcode is type[B]:
-            bbcode: B = self.get_tag(bbcode)
+        if bbcode is not isclass(bbcode):
+            bbcode: BBCODE = self.get_tag(bbcode)
+        if bbcode is None:
+            return self
+        bbcode: BBCODE
         self.data["text"] = str(bbcode)
         return self.remove(bbcode)
 
-    def get_tag(self, bbcode: type[B]) -> Optional[B]:
-        for _ in self.data["tags"]:
-            if isinstance(_, bbcode):
-                return _
+    @property
+    def tags(self) -> list[type[BBCODE]]:
+        return self.data["tags"]
+
+    @property
+    def extra(self) -> dict[str, str]:
+        return self.data["extra"]
+
+    def get_tag(self, bbcode: type[BBCode], index: int = 0) -> Optional[BBCODE]:
+        """
+        获取消息段中的BBCode
+        :param bbcode: BBCode 或 子类
+        :param index: 第几个，只有 bbcode=BBCode 时才有效
+        :return:
+        """
+        if bbcode == BBCode:
+            tags = self.tags
+            if len(tags) > index:
+                return tags[index](box=self.data)
+            return None
+        if bbcode in self.tags:
+            return bbcode(box=self.data)
         return None
 
-    def get_tags(self) -> list[B]:
-        return self.data["tags"]
+    def get_tags(self) -> list[BBCODE]:
+        return [tag(box=self.data) for tag in self.tags]
 
     def decode(self) -> str:
         _ = deque([self.data["text"]])
-        for tag in self.data["tags"][::-1]:
-            _.appendleft(tag.head)
-            _.append(tag.tail)
+        for tag in self.tags[::-1]:
+            bbcode: BBCODE = tag(box=self.data)
+            _.appendleft(bbcode.head)
+            _.append(bbcode.tail)
         return "".join(_)
 
+    def index(self, value: Union[str, type[BBCODE], BBCODE], raise_: bool = True) -> int:
+        index = 0
+        if isinstance(value, str):
+            for tag in self.tags:
+                if value in tag.keys_:
+                    return index
+                index += 1
+        else:
+            if not isclass(value):
+                value = type(value)
+            for tag in self.tags:
+                if tag == value:
+                    return index
+                index += 1
+        if raise_:
+            raise ValueError(f"{value} not in list")
+        return -1
+
 
 def _update_parser(func):
     @wraps(func)
     def _(*args, **kwargs):
         res = func(*args, **kwargs)
         Message.parser = Parser(MessageSegment, BBCODES)
         return res
 
     return _
 
 
 class Message(BaseMessage[MessageSegment]):
     parser: Parser = Parser(MessageSegment, BBCODES)
 
+    @classmethod
+    def get_segment_class(cls) -> type[MessageSegment]:
+        return MessageSegment
+
     def __init__(
         self,
         message: Union[str, None, Iterable[MessageSegment], MessageSegment] = None,
     ):
         super().__init__(message)
         self.reduce()  # 合并连续的纯文本
 
+    @classmethod
+    def _construct(cls, msg: str) -> Iterable[MessageSegment]:
+        yield from cls.parser.tokenize(msg)
+
+    @classmethod
+    def update_parser(cls):
+        cls.parser = Parser(MessageSegment, BBCODES)
+
+    @classmethod
+    def register_bbcode(cls, code: Union[int, type[BBCODE]]):
+        _register_bbcode(code)
+        cls.update_parser()
+
+    @overload
+    def __getitem__(self, args: str) -> Self: ...
+
+    @overload
+    def __getitem__(self, args: tuple[str, int]) -> MessageSegment: ...
+
+    @overload
+    def __getitem__(self, args: tuple[str, slice]) -> Self: ...
+
+    @overload
+    def __getitem__(self, args: int) -> MessageSegment: ...
+
+    @overload
+    def __getitem__(self, args: slice) -> Self: ...
+
+    @overload
+    def __getitem__(self, args: type[BBCODE]) -> list[BBCODE]: ...
+
+    @overload
+    def __getitem__(self, args: tuple[type[BBCODE], int]) -> BBCODE: ...
+
+    @overload
+    def __getitem__(self, args: tuple[type[BBCODE], slice]) -> list[BBCODE]: ...
+
+    def __getitem__(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self,
+        args: Union[str, tuple[Union[str, type[BBCODE]], Union[int, slice]], int, slice, type[BBCODE]],
+    ) -> Union[MessageSegment, Self, BBCODE, list[BBCODE]]:
+        # 判断是否为 type[B]
+        arg1 = args
+        arg2 = slice(None)
+        if isinstance(args, tuple):
+            arg1, arg2 = args
+
+        if isclass(arg1) and issubclass(arg1, BBCode):  # 是类 + 是BBCode
+            return self.get_tag(arg1, arg2, strict=True) if isinstance(arg2, int) else self.get_tags(arg1)[arg2]
+        return super().__getitem__(args)
+
+    def has(self, value: Union[MessageSegment, str, type[BBCODE], BBCODE]) -> bool:
+        return value in self
+
+    def __contains__(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, value: Union[MessageSegment, str, type[BBCODE], BBCODE]
+    ) -> bool:
+        if isinstance(value, (MessageSegment, str)):
+            return super().__contains__(value)
+        return value.tag_in(self)
+
+    def index(self, value: Union[MessageSegment, str, type[BBCODE], BBCODE], *args: SupportsIndex) -> int:
+        if isinstance(value, (MessageSegment, str)):
+            return super().index(value, *args)
+        index = 0
+        for seg in self:
+            _index = seg.index(value, raise_=False)
+            if _index != -1:
+                return _index + index
+            index += len(seg.tags)
+        raise ValueError(f"{value} not in list")
+
+    def count(self, value: Union[MessageSegment, str, type[BBCode]]) -> int:
+        if isinstance(value, (MessageSegment, str)):
+            return super().count(value)
+        return sum(1 for seg in self if value in seg.tags)
+
+    def only(self, value: Union[MessageSegment, str, type[BBCODE]]) -> bool:
+        if isinstance(value, (MessageSegment, str)):
+            return super().__contains__(value)
+        for seg in self:
+            for tag in seg.tags:
+                if tag != value:
+                    return False
+        return True
+
     def reduce(self):
         # MIT https://github.com/nonebot/adapter-onebot/blob/v2.4.3/nonebot/adapters/onebot/v11/message.py#L334-L342
         """合并消息内连续的纯文本段。"""
         index = 1
         while index < len(self):
-            if len(self[index - 1].get_tags()) == 0 and len(self[index].get_tags()) == 0:
+            if len(self[index - 1].tags) == 0 and len(self[index].tags) == 0:  # 连续的纯文本
                 self[index - 1].merge_text(self[index])
                 del self[index]
             else:
                 index += 1
 
     def merge_text(self) -> Self:
-        if len(self) < 2:
+        if len(self) < 2:  # 只有一个消息段
             return self
         _ = [self[0]]
         for seg in self[1:]:
             seg: MessageSegment
-            if len(seg.get_tags()) == 0 and len(_[-1].get_tags()) == 0:
+            if len(seg.tags) == 0 and len(_[-1].tags) == 0:  # 连续的纯文本
                 _[-1].merge_text(seg)
                 continue
             _.append(seg)
         return Message(_)
 
-    @classmethod
-    def update_parser(cls):
-        cls.parser = Parser(MessageSegment, BBCODES)
-
-    @classmethod
-    def register_bbcode(cls, code: Union[int, type[B]]):
-        _register_bbcode(code)
-        cls.update_parser()
-
-    @override
-    def __contains__(  # pyright: ignore[reportIncompatibleMethodOverride]
-        self, value: Union[MessageSegment, str, type[B]]
-    ) -> bool:
-        if issubclass(value, BBCode):
-            return value.tag_in(self)
-        return super().__contains__(value)
-
-    @override
-    def has(self, value: Union[MessageSegment, str, type[B]]) -> bool:
-        return value in self
-
-    @classmethod
-    @override
-    def get_segment_class(cls) -> type[MessageSegment]:
-        return MessageSegment
-
-    @classmethod
-    @override
-    def _construct(cls, msg: str) -> Iterable[MessageSegment]:
-        yield from cls.parser.tokenize(msg)
-
-    @override
     def extract_plain_text(self) -> str:
         return "".join(seg.data["text"] for seg in self if seg.is_text())
 
     def decode(self) -> str:
         return "".join(seg.decode() for seg in self)
 
     def show(self) -> str:
         return " ".join(seg.decode() for seg in self)
+
+    def get_tag(self, bbcode: type[BBCode], index: int = 0, strict: bool = False) -> Optional[BBCODE]:
+        if bbcode == BBCode:
+            for seg in self:
+                for tag in seg.tags:
+                    if index == 0:
+                        return tag(box=seg.data)
+                    index -= 1
+            if strict:
+                raise IndexError(f"{bbcode} not in list")
+            return None
+        for seg in self:
+            for tag in seg.tags:
+                if tag == bbcode:
+                    if index == 0:
+                        return bbcode(box=seg.data)
+                    index -= 1
+        if strict:
+            raise IndexError(f"{bbcode} not in list")
+        return None
+
+    def get_tags(self, bbcode: type[BBCode]) -> list[BBCODE]:
+        if bbcode == BBCode:
+            return [tag(box=seg.data) for seg in self for tag in seg.tags]
+        return [tag(box=seg.data) for seg in self for tag in seg.tags if tag == bbcode]
+
+    @property
+    def tags(self) -> list[type[BBCODE]]:
+        return [tag for seg in self for tag in seg.tags]
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/model.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/util.py` & `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b7/pyproject.toml` & `nonebot_adapter_tailchat-0.1.0b8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-tailchat"
-version = "0.1.0b7"
+version = "0.1.0b8"
 description = "NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2"
 authors = ["eya46 <61458340+eya46@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "nonebot_adapter_tailchat" }]
 keywords = ["bot", "tailchat", "nonebot2"]
 repository = "https://github.com/eya46/nonebot-adapter-tailchat"
@@ -45,12 +45,13 @@
 ignore = [
     "E402", # 导包位置
     "E722", # 空except
     "C901", # 复杂函数名
     "PYI048", # Function body must contain exactly one statement
     "PYI021", # Docstrings should not be included in stubs
     #    "T201", # no print
+    "E742", # I
 ]
 
 [tool.ruff.format]
 quote-style = "double"
 docstring-code-format = true
```

### Comparing `nonebot_adapter_tailchat-0.1.0b7/PKG-INFO` & `nonebot_adapter_tailchat-0.1.0b8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-tailchat
-Version: 0.1.0b7
+Version: 0.1.0b8
 Summary: NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2
 Home-page: https://github.com/eya46/nonebot-adapter-tailchat
 License: Apache-2.0
 Keywords: bot,tailchat,nonebot2
 Author: eya46
 Author-email: 61458340+eya46@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -28,21 +28,24 @@
 
 <div align="center">
 
 # Nonebot Adapter Tailchat
 
 ## Tailchat 适配器
 
-![License](https://img.shields.io/github/license/eya46/nonebot-adapter-tailchat)
-![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
-![NoneBot](https://img.shields.io/badge/nonebot-2.3.0+-red.svg)
+[![License](https://img.shields.io/github/license/eya46/nonebot-adapter-tailchat)](https://github.com/eya46/nonebot-adapter-tailchat/blob/master/LICENSE)
+[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)](https://docs.python.org/zh-cn/3.9/library/index.html)
+[![NoneBot](https://img.shields.io/badge/nonebot-2.3.0+-red.svg)](https://nonebot.dev)
+[![Tailchat](https://img.shields.io/badge/Tailchat-1.11.3+-blue.svg)](https://tailchat.msgbyte.com)
 </div>
 
 ## 环境要求
 
+- Tailchat >= 1.11.3
+    - api: `getMessage`
 - Python 3.9+
 - NoneBot 2.3.0+
 - pydantic >= 2.0.0
 - HTTPClient驱动器
     - > 默认需要,除非 `useHttp=False`, 且配置了 `jwt`
     - ~httpx
     - ~aiohttp
@@ -76,13 +79,14 @@
 ```
 
 ## 详细配置项
 
 [config.py](./nonebot_adapter_tailchat/config.py)
 
 ## 相关项目
+
 - [dcwatson/bbcode](https://github.com/dcwatson/bbcode)
 - [Tailchat](https://github.com/msgbyte/tailchat)
 - [python-socketio](https://github.com/miguelgrinberg/python-socketio)
 - [nonebot2](https://github.com/nonebot/nonebot2)
 - [pydantic2](https://docs.pydantic.dev/latest/)
 - ...
```

#### html2text {}

```diff
@@ -1,33 +1,37 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b7 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b8 Summary:
 NoneBot2 Tailchat ééå¨ / Tailchat adapter for nonebot2 Home-page: https://
 github.com/eya46/nonebot-adapter-tailchat License: Apache-2.0 Keywords:
 bot,tailchat,nonebot2 Author: eya46 Author-email:
 61458340+eya46@users.noreply.github.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: msgpack (>=1.0.8,<2.0.0) Requires-Dist: nonebot2 (>=2.3.0)
 Requires-Dist: pydantic (>=2.0.0) Requires-Dist: python-socketio[asyncio-
 client] (>=5.11.2,<6.0.0) Project-URL: Repository, https://github.com/eya46/
 nonebot-adapter-tailchat Project-URL: Tailchat, https://tailchat.msgbyte.com/
 Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
-     # Nonebot Adapter Tailchat ## Tailchat ééå¨ ![License](https://
-img.shields.io/github/license/eya46/nonebot-adapter-tailchat) ![Python](https:/
-/img.shields.io/badge/python-3.9+-blue.svg) ![NoneBot](https://img.shields.io/
-                         badge/nonebot-2.3.0+-red.svg)
-## ç¯å¢è¦æ± - Python 3.9+ - NoneBot 2.3.0+ - pydantic >= 2.0.0 -
-HTTPClienté©±å¨å¨ - > é»è®¤éè¦,é¤é `useHttp=False`, ä¸éç½®äº `jwt`
-- ~httpx - ~aiohttp ## Tailchatæºå¨äººå¼å¯æ¹å¼ 1. å®è£
-`å¼æ¾å¹³å°æä»¶` 2. è¿å¥ `è®¾ç½®` -> `å¼æ¾å¹³å°` -> `åå»ºåºç¨` -
-> `å¡«ååºæ¬ä¿¡æ¯` 3. è¿å¥ `åºç¨` -> `æºå¨äºº` -
-> `å¼å¯æºå¨äººè½å` 4. å¨ `åºæ¬ä¿¡æ¯` åè·å `appId` å
-`appSecret` > ææªæ¯æ `æ¶æ¯åè°å°å` ## éç½®æ¹å¼ `.env` æä»¶
-```dotenv TAILCHAT_BOTS=' [ { "url": "https://xxxxxxx/", "appId": "ts_******",
-"appSecret": "****" } ] ' TAILCHAT_RECONNECT_INTERVAL=5 TAILCHAT_TIME_OUT=5 ```
-## è¯¦ç»éç½®é¡¹ [config.py](./nonebot_adapter_tailchat/config.py) ##
-ç¸å³é¡¹ç® - [dcwatson/bbcode](https://github.com/dcwatson/bbcode) -
-[Tailchat](https://github.com/msgbyte/tailchat) - [python-socketio](https://
-github.com/miguelgrinberg/python-socketio) - [nonebot2](https://github.com/
-nonebot/nonebot2) - [pydantic2](https://docs.pydantic.dev/latest/) - ...
+     # Nonebot Adapter Tailchat ## Tailchat ééå¨ [![License](https://
+    img.shields.io/github/license/eya46/nonebot-adapter-tailchat)](https://
+   github.com/eya46/nonebot-adapter-tailchat/blob/master/LICENSE) [![Python]
+ (https://img.shields.io/badge/python-3.9+-blue.svg)](https://docs.python.org/
+zh-cn/3.9/library/index.html) [![NoneBot](https://img.shields.io/badge/nonebot-
+  2.3.0+-red.svg)](https://nonebot.dev) [![Tailchat](https://img.shields.io/
+        badge/Tailchat-1.11.3+-blue.svg)](https://tailchat.msgbyte.com)
+## ç¯å¢è¦æ± - Tailchat >= 1.11.3 - api: `getMessage` - Python 3.9+ -
+NoneBot 2.3.0+ - pydantic >= 2.0.0 - HTTPClienté©±å¨å¨ - >
+é»è®¤éè¦,é¤é `useHttp=False`, ä¸éç½®äº `jwt` - ~httpx - ~aiohttp ##
+Tailchatæºå¨äººå¼å¯æ¹å¼ 1. å®è£ `å¼æ¾å¹³å°æä»¶` 2. è¿å¥ `è®¾ç½®`
+-> `å¼æ¾å¹³å°` -> `åå»ºåºç¨` -> `å¡«ååºæ¬ä¿¡æ¯` 3. è¿å¥ `åºç¨`
+-> `æºå¨äºº` -> `å¼å¯æºå¨äººè½å` 4. å¨ `åºæ¬ä¿¡æ¯` åè·å
+`appId` å `appSecret` > ææªæ¯æ `æ¶æ¯åè°å°å` ## éç½®æ¹å¼
+`.env` æä»¶ ```dotenv TAILCHAT_BOTS=' [ { "url": "https://xxxxxxx/", "appId":
+"ts_******", "appSecret": "****" } ] ' TAILCHAT_RECONNECT_INTERVAL=5
+TAILCHAT_TIME_OUT=5 ``` ## è¯¦ç»éç½®é¡¹ [config.py](./
+nonebot_adapter_tailchat/config.py) ## ç¸å³é¡¹ç® - [dcwatson/bbcode](https:/
+/github.com/dcwatson/bbcode) - [Tailchat](https://github.com/msgbyte/tailchat)
+- [python-socketio](https://github.com/miguelgrinberg/python-socketio) -
+[nonebot2](https://github.com/nonebot/nonebot2) - [pydantic2](https://
+docs.pydantic.dev/latest/) - ...
```

