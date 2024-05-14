# Comparing `tmp/rabbitspider-1.5.tar.gz` & `tmp/rabbitspider-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitspider-1.5.tar", last modified: Fri Apr 19 08:41:35 2024, max compression
+gzip compressed data, was "rabbitspider-1.6.tar", last modified: Tue May 14 01:29:11 2024, max compression
```

## Comparing `rabbitspider-1.5.tar` & `rabbitspider-1.6.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.495566 rabbitspider-1.5/
--rw-rw-rw-   0        0        0      470 2024-04-19 08:41:35.494569 rabbitspider-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2567 2024-04-11 02:19:57.000000 rabbitspider-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.433733 rabbitspider-1.5/RabbitSpider/
--rw-rw-rw-   0        0        0        0 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.455674 rabbitspider-1.5/RabbitSpider/core/
--rw-rw-rw-   0        0        0        0 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/core/__init__.py
--rw-rw-rw-   0        0        0     4090 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/core/download.py
--rw-rw-rw-   0        0        0     7244 2024-04-19 06:09:05.000000 rabbitspider-1.5/RabbitSpider/core/engine.py
--rw-rw-rw-   0        0        0     2456 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/core/scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.466677 rabbitspider-1.5/RabbitSpider/http/
--rw-rw-rw-   0        0        0        1 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/http/__init__.py
--rw-rw-rw-   0        0        0      833 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/http/request.py
--rw-rw-rw-   0        0        0     2698 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/http/response.py
--rw-rw-rw-   0        0        0      415 2024-04-19 04:58:50.000000 rabbitspider-1.5/RabbitSpider/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.492574 rabbitspider-1.5/RabbitSpider/utils/
--rw-rw-rw-   0        0        0        1 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/__init__.py
--rw-rw-rw-   0        0        0     1211 2024-04-19 04:42:59.000000 rabbitspider-1.5/RabbitSpider/utils/control.py
--rw-rw-rw-   0        0        0      483 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/dupefilter.py
--rw-rw-rw-   0        0        0      131 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/expections.py
--rw-rw-rw-   0        0        0     3477 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/fast_monitor.py
--rw-rw-rw-   0        0        0     1879 2024-04-19 04:01:31.000000 rabbitspider-1.5/RabbitSpider/utils/rabbit_go.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.493572 rabbitspider-1.5/RabbitSpider.egg-info/
--rw-rw-rw-   0        0        0      470 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 08:41:35.495566 rabbitspider-1.5/setup.cfg
--rw-rw-rw-   0        0        0      612 2024-04-19 08:37:59.000000 rabbitspider-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:29:11.653812 rabbitspider-1.6/
+-rw-rw-rw-   0        0        0      500 2024-05-14 01:29:11.651817 rabbitspider-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2613 2024-05-12 03:17:43.000000 rabbitspider-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 01:29:11.616910 rabbitspider-1.6/RabbitSpider/
+-rw-rw-rw-   0        0        0        0 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:29:11.645833 rabbitspider-1.6/RabbitSpider/core/
+-rw-rw-rw-   0        0        0        0 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/core/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/core/download.py
+-rw-rw-rw-   0        0        0     7442 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/core/engine.py
+-rw-rw-rw-   0        0        0     1959 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/core/scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:29:11.647827 rabbitspider-1.6/RabbitSpider/http/
+-rw-rw-rw-   0        0        0        1 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/http/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/http/request.py
+-rw-rw-rw-   0        0        0     2692 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/http/response.py
+-rw-rw-rw-   0        0        0      260 2024-05-14 01:15:38.000000 rabbitspider-1.6/RabbitSpider/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:29:11.650819 rabbitspider-1.6/RabbitSpider/utils/
+-rw-rw-rw-   0        0        0        1 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/utils/__init__.py
+-rw-rw-rw-   0        0        0     1208 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/utils/control.py
+-rw-rw-rw-   0        0        0      483 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/utils/dupefilter.py
+-rw-rw-rw-   0        0        0      131 2024-05-12 03:17:43.000000 rabbitspider-1.6/RabbitSpider/utils/expections.py
+-rw-rw-rw-   0        0        0     2020 2024-05-14 01:12:06.000000 rabbitspider-1.6/RabbitSpider/utils/rabbit_go.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:29:11.651817 rabbitspider-1.6/RabbitSpider.egg-info/
+-rw-rw-rw-   0        0        0      500 2024-05-14 01:29:11.000000 rabbitspider-1.6/RabbitSpider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-05-14 01:29:11.000000 rabbitspider-1.6/RabbitSpider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 01:29:11.000000 rabbitspider-1.6/RabbitSpider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2024-05-14 01:29:11.000000 rabbitspider-1.6/RabbitSpider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 01:29:11.000000 rabbitspider-1.6/RabbitSpider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 01:29:11.653812 rabbitspider-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-05-14 01:21:20.000000 rabbitspider-1.6/setup.py
```

### Comparing `rabbitspider-1.5/README.md` & `rabbitspider-1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 基于rabbitmq 做消息队列开发的分布式异步爬虫框架，支持web监控，定时任务，运行模式 auto 先生产后消费，m 只生产，w 只消费
 
-安装pip install RabbitSpider==1.3.0
+安装pip install RabbitSpider==1.5
 
     from jsonpath import jsonpath
     from RabbitSpider.core.engine import Engine
     from RabbitSpider.http.request import Request
     from RabbitSpider.http.response import Response
     from RabbitSpider.utils.rabbit_go import go
+    from RabbitSpider.core.download import AiohttpDownload, CurlDownload
 
 
     class Test(Engine):
-    
+
         def __init__(self, sync):
             super().__init__(sync)
             # pip 安装需要添加rabbitmq redis 配置
             self.settings.set('RABBIT_HOST', '121.36.225.245')
             self.settings.set('RABBIT_PORT', 5672)
             self.settings.set('RABBIT_USERNAME', 'yuntom')
             self.settings.set('RABBIT_PASSWORD', '123456')
             self.settings.set('RABBIT_VIRTUAL_HOST', '/')
-            self.settings.set('REDIS_FILTER_NAME', 'filter_queue')
             self.settings.set('REDIS_QUEUE_HOST', '127.0.0.1')
             self.settings.set('REDIS_QUEUE_PORT', 6379)
             self.settings.set('REDIS_QUEUE_DB', 1)
+            self.settings.set('LOG_LEVEL', 'ERROR')
     
         async def start_requests(self):
             for i in range(50):
                 data = '{"token":"","pn":0,"rn":10,"sdt":"","edt":"","wd":"","inc_wd":"","exc_wd":"","fields":"","cnum":"","sort":"{\\"webdate\\":\\"0\\",\\"id\\":\\"0\\"}","ssort":"","cl":10000,"terminal":"","condition":[{"fieldName":"categorynum","equal":"002006","notEqual":null,"equalList":null,"notEqualList":null,"isLike":true,"likeType":2}],"time":[{"fieldName":"webdate","startTime":"2024-01-25 00:00:00","endTime":"2024-02-24 23:59:59"}],"highlights":"","statistics":null,"unionCondition":[],"accuracy":"","noParticiple":"1","searchRange":null,"noWd":true}'
                 yield Request(url='https://www.jxsggzy.cn/XZinterface/rest/esinteligentsearch/getFullTextDataNew',
                               data=data, method='post', dupe_filter=False)
     
@@ -34,15 +35,14 @@
             url = 'https://www.jxsggzy.cn/' + jsonpath(response.json(), expr='$..linkurl')[0]
             yield Request(url=url, dupe_filter=False, callback=self.parse_item)
     
         async def parse_item(self, request: Request, response: Response):
             item = {'title': response.xpath('//p[@class="title"]/text()').get()}
             yield item
     
-        async def save_item(self, item: dict):
+        async def process_item(self, item: dict):
             """入库逻辑"""
             print(item)
-    
-    
+
     if __name__ == '__main__':
         go(Test, 'auto', 10)
```

### Comparing `rabbitspider-1.5/RabbitSpider/core/engine.py` & `rabbitspider-1.6/RabbitSpider/core/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,178 +1,185 @@
 import asyncio
 import os
 import pickle
 import sys
-from abc import ABC, abstractmethod
 from collections.abc import AsyncGenerator, Coroutine
 from traceback import print_exc
 from typing import Optional
 from aio_pika.abc import AbstractIncomingMessage
 from loguru import logger
 from RabbitSpider.http.request import Request
+from RabbitSpider.http.response import Response
 from RabbitSpider.utils.control import TaskManager
 from RabbitSpider.utils.control import SettingManager
 from RabbitSpider.utils.dupefilter import RFPDupeFilter
 from RabbitSpider.utils.expections import RabbitExpect
 from RabbitSpider.core.scheduler import Scheduler
-from RabbitSpider.core.download import CurlDownload, AiohttpDownload
+from RabbitSpider.core.download import CurlDownload
 from aio_pika.exceptions import QueueEmpty, ChannelClosed
 
 
-class Engine(ABC):
-    queue = os.path.basename(sys.argv[0])
+class Engine(object):
+    name = os.path.basename(sys.argv[0])
     allow_status_code: list = [200]
     max_retry: int = 5
-    http2 = False
-    tls = 'chrome120'
+    http_version = 1
+    tls = "chrome120"
 
     def __init__(self, sync):
         self._filter = None
         self._scheduler = None
         self._connection = None
         self._channel = None
         self._download = None
         self._task_manager = None
         self._sync = sync
         self.logger = None
+        self.session = None
+        self._future = None
         self.settings = SettingManager()
         self._task_manager = TaskManager(self._sync)
+        self._download = CurlDownload(http_version=self.http_version, impersonate=self.tls)
 
     async def start_spider(self):
-        await self._scheduler.create_queue(self._channel, self.queue)
+        await self._scheduler.create_queue(self._channel, self.name)
         start_request = self.start_requests()
         await self.routing(start_request)
 
-    @abstractmethod
+    async def open_spider(self):
+        """初始化数据库"""
+        self.logger.info(f'{self.name}任务开始！')
+
     async def start_requests(self):
         """初始请求"""
         pass
 
-    @abstractmethod
-    async def parse(self, request, response):
+    async def parse(self, request: Request, response: Response):
         """默认回调"""
         pass
 
-    @abstractmethod
-    async def save_item(self, item: dict):
+    async def process_item(self, item: dict):
         """入库逻辑"""
         pass
 
+    async def close_spider(self):
+        self.logger.info(f'{self.name}任务结束！')
+
     def before_request(self, ret):
         """请求前"""
         return ret
 
     async def routing(self, result):
         if isinstance(result, AsyncGenerator):
             async for req in result:
                 if isinstance(req, Request):
                     ret = pickle.dumps(req.model_dump())
                     if req.dupe_filter:
                         if self._filter.request_seen(ret):
                             self.logger.info(f'生产数据：{req.model_dump()}')
-                            await self._scheduler.producer(self._channel, queue=self.queue, body=ret)
+                            await self._scheduler.producer(self._channel, queue=self.name, body=ret)
                     else:
                         self.logger.info(f'生产数据：{req.model_dump()}')
-                        await self._scheduler.producer(self._channel, queue=self.queue, body=ret)
+                        await self._scheduler.producer(self._channel, queue=self.name, body=ret)
 
                 elif isinstance(req, dict):
-                    await self.save_item(req)
+                    await self.process_item(req)
         elif isinstance(result, Coroutine):
             await result
         else:
             raise RabbitExpect('回调函数返回类型错误！')
 
     async def crawl(self):
-        session = await self._download.new_session()
+        self.session = await self._download.new_session()
         while True:
             try:
                 incoming_message: Optional[AbstractIncomingMessage] = await self._scheduler.consumer(self._channel,
-                                                                                                     queue=self.queue)
+                                                                                                     queue=self.name)
             except QueueEmpty:
                 if self._task_manager.all_done():
-                    await self._download.exit(session)
-                    await self._scheduler.delete_queue(self._channel, self.queue)
+                    await self._download.exit(self.session)
+                    await self._scheduler.delete_queue(self._channel, self.name)
                     await self._channel.close()
                     await self._connection.close()
                     break
                 else:
                     continue
-            except ChannelClosed:
-                self._connection, self._channel = self._scheduler.connect()
-                self.logger.warning('mq重新连接!')
-                continue
+            except Exception:
+                break
             if incoming_message:
                 await self._task_manager.semaphore.acquire()
-                self._task_manager.create_task(self.deal_resp(incoming_message, session))
+                self._task_manager.create_task(self.deal_resp(incoming_message))
             else:
                 print(incoming_message)
 
     async def consume(self):
-        session = await self._download.new_session()
-        while True:
-            try:
-                await self._scheduler.consumer(self._channel, queue=self.queue, callback=self.deal_resp,
-                                               prefetch=self._sync,
-                                               args=session)
-                break
-            except ChannelClosed:
-                self._connection, self._channel = self._scheduler.connect()
-                self.logger.warning('mq重新连接!')
+        self.session = await self._download.new_session()
+        await self._scheduler.consumer(self._channel, queue=self.name, callback=self.deal_resp,
+                                       prefetch=self._sync)
+        self._future = asyncio.Future()
+        await self._future
 
-    async def deal_resp(self, incoming_message: AbstractIncomingMessage, session):
+    async def deal_resp(self, incoming_message):
         ret = self.before_request(pickle.loads(incoming_message.body))
+        self.logger.info(f'消费数据：{ret}')
         try:
-            self.logger.info(f'消费数据：{ret}')
-            response = await self._download.fetch(session, ret)
-        except Exception:
+            response = await self._download.fetch(self.session, ret)
+        except Exception as e:
+            self.logger.error(f'请求失败：{e}')
             print_exc()
             response = None
         if response and response.status in self.allow_status_code:
             try:
                 callback = getattr(self, ret['callback'])
                 result = callback(Request(**ret), response)
                 if result:
                     await self.routing(result)
-            except Exception:
+            except Exception as e:
+                self.logger.error(f'请求失败：{e}')
                 print_exc()
                 for task in asyncio.all_tasks():
                     task.cancel()
         else:
             if ret['retry'] < self.max_retry:
                 ret['retry'] += 1
-                await self._scheduler.producer(self._channel, queue=self.queue, body=pickle.dumps(ret),
+                await self._scheduler.producer(self._channel, queue=self.name, body=pickle.dumps(ret),
                                                priority=ret['retry'])
             else:
                 self.logger.error(f'请求失败：{ret}')
-        await incoming_message.ack()
+        try:
+            await self._channel.declare_queue(name=self.name, passive=True)
+            await incoming_message.ack()
+        except Exception:
+            self._future.set_result('done') if self._future else None
+            self.logger.info(f'队列{self.name}已删除！')
 
-    async def run(self, mode):
+    async def load_setting(self):
         logger.add("../rabbit_log/rabbit_{time:YYYY-MM-DD}.log", level=self.settings.get('LOG_LEVEL'), rotation="1 day",
                    retention="1 week",
-                   format="{time:YYYY-MM-DD HH:mm:ss.sss} | {level}  | {extra[scope]} | {name}:{line} - {message}")
-        self.logger = logger.bind(scope=self.queue)
+                   format="{time:YYYY-MM-DD HH:mm:ss} | {level} | {extra[scope]} | {name}:{line} - {message}")
+        self.logger = logger.bind(scope=self.name)
 
-        self._filter = RFPDupeFilter(self.settings.get('REDIS_FILTER_NAME'),
+        self._filter = RFPDupeFilter(self.name,
                                      self.settings.get('REDIS_QUEUE_HOST'),
                                      self.settings.get('REDIS_QUEUE_PORT'),
                                      self.settings.get('REDIS_QUEUE_DB'))
 
         self._scheduler = Scheduler(self.settings.get('RABBIT_USERNAME'),
                                     self.settings.get('RABBIT_PASSWORD'),
                                     self.settings.get('RABBIT_HOST'),
                                     self.settings.get('RABBIT_PORT'),
                                     self.settings.get('RABBIT_VIRTUAL_HOST'))
-        self._connection, self._channel = self._scheduler.connect()
-        if self.settings.get('DOWNLOAD') == CurlDownload:
-            self._download = CurlDownload(http2=self.http2, impersonate=self.tls)
-        else:
-            self._download = AiohttpDownload()
+        self._connection, self._channel = await self._scheduler.connect()
 
+    async def run(self, mode):
+        await self.load_setting()
+        await self.open_spider()
         if mode == 'auto':
             await self.start_spider()
             await self.crawl()
         elif mode == 'm':
             await self.start_spider()
         elif mode == 'w':
             await self.consume()
         else:
             raise RabbitExpect('执行模式错误！')
+        await self.close_spider()
```

### Comparing `rabbitspider-1.5/RabbitSpider/core/scheduler.py` & `rabbitspider-1.6/RabbitSpider/core/scheduler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,48 @@
-import asyncio
 from typing import Callable, Optional
 from aio_pika import connect_robust, Message
-from aio_pika.pool import Pool
 
 
 class Scheduler(object):
     def __init__(self, username: str, password: str, host: str,
                  port: int, virtual_host: str):
         self.username = username
         self.password = password
         self.host = host
         self.port = port
         self.virtual_host = virtual_host
 
-    def connect(self):
-        connection_pool = Pool(self.get_connection, max_size=1)
-        channel_pool = Pool(self.get_channel, connection_pool, max_size=3)
-        return connection_pool, channel_pool
-
-    async def get_connection(self):
-        return await connect_robust(host=self.host, login=self.username, password=self.password,
-                                    virtualhost=self.virtual_host)
+    async def connect(self):
+        connection = await connect_robust(host=self.host, login=self.username, password=self.password,
+                                          virtualhost=self.virtual_host)
+        channel = await connection.channel()
+        return connection, channel
 
     @staticmethod
-    async def get_channel(connection_pool):
-        async with connection_pool.acquire() as connection:
-            return await connection.channel()
+    async def create_queue(channel, queue: str):
+        queue = await channel.declare_queue(name=queue, durable=True,
+                                            arguments={"x-max-priority": 10})
+        await queue.purge()
 
     @staticmethod
-    async def create_queue(channel_pool, queue: str):
-        async with channel_pool.acquire() as channel:
-            queue = await channel.declare_queue(name=queue, durable=True,
-                                                arguments={"x-max-priority": 10})
-            await queue.purge()
+    async def producer(channel, queue: str, body: bytes, priority: int = 1):
+        await channel.default_exchange.publish(Message(body=body, delivery_mode=2, priority=priority),
+                                               routing_key=queue)
 
     @staticmethod
-    async def producer(channel_pool, queue: str, body: bytes, priority: int = 1):
-        async with channel_pool.acquire() as channel:
-            await channel.default_exchange.publish(Message(body=body, delivery_mode=2, priority=priority),
-                                                   routing_key=queue)
+    async def consumer(channel, queue: str, callback: Optional[Callable] = None, prefetch: int = 1):
+        queue = await channel.declare_queue(name=queue, durable=True, passive=True,
+                                            arguments={"x-max-priority": 10})
+        if callback:
+            await channel.set_qos(prefetch_count=prefetch)
+            await queue.consume(callback=callback)
+        else:
+            return await queue.get()
 
     @staticmethod
-    async def consumer(channel_pool, queue: str, callback: Optional[Callable] = None, prefetch: int = 1, args=None):
-        async with channel_pool.acquire() as channel:
-
-            queue = await channel.declare_queue(name=queue, durable=True, passive=True,
-                                                arguments={"x-max-priority": 10})
-            if callback:
-                await channel.set_qos(prefetch_count=prefetch)
-                await queue.consume(callback=lambda message: callback(message, args))
-                await asyncio.Future()
-            else:
-                return await queue.get()
+    async def delete_queue(channel, queue: str):
+        await channel.queue_delete(queue)
 
     @staticmethod
-    async def delete_queue(channel_pool, queue: str):
-        async with channel_pool.acquire() as channel:
-            await channel.queue_delete(queue)
+    async def get_message_count(channel, queue: str):
+        queue = await channel.declare_queue(name=queue, durable=True, passive=True)
+        return queue.declaration_result.message_count
```

### Comparing `rabbitspider-1.5/RabbitSpider/http/request.py` & `rabbitspider-1.6/RabbitSpider/http/request.py`

 * *Files identical despite different names*

### Comparing `rabbitspider-1.5/RabbitSpider/http/response.py` & `rabbitspider-1.6/RabbitSpider/http/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Response:
     def __init__(self, content=None, status_code=None, charset=None, res=None):
         self.url = str(res.url)
         self.body = self.content = content
         self.status = self.status_code = status_code
         self.charset = charset
         self.res = res
-        self.cookies = {k: v.value for k, v in self.res.cookies.items()}
+        self.cookies = {k: v for k, v in self.res.cookies.items()}
         self.__r = parsel.Selector(self.text)
 
     def __str__(self):
         return self.text
 
     @property
     def text(self):
```

### Comparing `rabbitspider-1.5/RabbitSpider/utils/control.py` & `rabbitspider-1.6/RabbitSpider/utils/control.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,10 +41,7 @@
             self.semaphore.release()
 
         task.add_done_callback(done_callback)
         return task
 
     def all_done(self):
         return len(self.current_task) == 0
-
-
-
```

### Comparing `rabbitspider-1.5/RabbitSpider/utils/rabbit_go.py` & `rabbitspider-1.6/RabbitSpider/utils/rabbit_go.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import asyncio
 import time
 import requests
+import socket
 from datetime import datetime, timedelta
 from traceback import print_exc
 from signal import signal, SIGINT, SIGTERM
 from asyncio import WindowsSelectorEventLoopPolicy
 
 
 def main(spider, mode, sync, timer):
@@ -16,29 +17,31 @@
         rabbit = spider(sync)
     except Exception:
         print_exc()
         raise
 
     # def signal_handler(sig, frame):
     #     requests.post('http://127.0.0.1:8000/post/task',
-    #                   json={'name': rabbit.queue, 'status': 0,
+    #                   json={'name': rabbit.name, 'status': 0,
     #                         'stop_time': datetime.now().strftime('%Y-%m-%d %H:%M:%S')})
     #
     # signal(SIGINT, signal_handler)
     # signal(SIGTERM, signal_handler)
     try:
         # requests.post('http://127.0.0.1:8000/post/task',
-        #               json={'name': rabbit.queue, 'ip_address': '127.0.0.1', 'sync': sync, 'status': 1})
+        #               json={'name': rabbit.name, 'ip_address': f'{socket.gethostbyname(socket.gethostname())}',
+        #                     'sync': sync, 'status': 1})
         loop.run_until_complete(rabbit.run(mode))
         # if timer:
         #     requests.post('http://127.0.0.1:8000/post/task',
-        #                   json={'name': rabbit.queue,
+        #                   json={'name': rabbit.name,
+        #                         'sleep': timer,
         #                         'next_time': (datetime.now() + timedelta(minutes=timer)).strftime('%Y-%m-%d %H:%M:%S')})
-        # else:
-        #     requests.post('http://127.0.0.1:8000/delete/queue', json={'name': rabbit.queue})
+        # elif mode == 'auto':
+        #     requests.post('http://127.0.0.1:8000/delete/queue', json={'name': rabbit.name})
     except Exception:
         print_exc()
 
 
 def go(spider: object, mode: str = 'auto', sync: int = 1, timer: int = 0):
     for i in sys.argv[1:]:
         key, value = i.split('=')
```

### Comparing `rabbitspider-1.5/RabbitSpider.egg-info/SOURCES.txt` & `rabbitspider-1.6/RabbitSpider.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 RabbitSpider/http/__init__.py
 RabbitSpider/http/request.py
 RabbitSpider/http/response.py
 RabbitSpider/utils/__init__.py
 RabbitSpider/utils/control.py
 RabbitSpider/utils/dupefilter.py
 RabbitSpider/utils/expections.py
-RabbitSpider/utils/fast_monitor.py
 RabbitSpider/utils/rabbit_go.py
```

### Comparing `rabbitspider-1.5/setup.py` & `rabbitspider-1.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 setuptools.setup(
     name='RabbitSpider',
-    version='1.5',
+    version='1.6',
     author='一纸',
     author_email='2395396520@qq.com',
     url='https://github.com/YunTom/RabbitSpider/tree/master',
     packages=['RabbitSpider', 'RabbitSpider.core', 'RabbitSpider.http', 'RabbitSpider.utils'],
     python_requires='>=3.8',
     install_requires=[
         'aio-pika>=9.4.1',
-        'aiohttp>=3.9.5',
         'curl_cffi>=0.6.2',
         'loguru>=0.7.2',
         'parsel>=1.9.1',
         'pydantic>=2.7.0',
         'redis>=5.0.3',
         'w3lib>=2.1.2',
         'chardet>=5.2.0',
+        'loguru>=0.7.2',
+        'chardet>=5.2.0'
     ],
 )
```

