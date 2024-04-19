# Comparing `tmp/RabbitSpider-1.3.0.tar.gz` & `tmp/rabbitspider-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RabbitSpider-1.3.0.tar", last modified: Thu Apr 11 01:55:09 2024, max compression
+gzip compressed data, was "rabbitspider-1.5.tar", last modified: Fri Apr 19 08:41:35 2024, max compression
```

## Comparing `RabbitSpider-1.3.0.tar` & `rabbitspider-1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 01:55:09.368448 RabbitSpider-1.3.0/
--rw-rw-rw-   0        0        0      560 2024-04-11 01:55:09.367449 RabbitSpider-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 01:55:09.348501 RabbitSpider-1.3.0/RabbitSpider/
--rw-rw-rw-   0        0        0        0 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 01:55:09.360468 RabbitSpider-1.3.0/RabbitSpider/core/
--rw-rw-rw-   0        0        0        0 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/core/__init__.py
--rw-rw-rw-   0        0        0     4090 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/core/download.py
--rw-rw-rw-   0        0        0     6819 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/core/engine.py
--rw-rw-rw-   0        0        0     2456 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/core/scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-11 01:55:09.362463 RabbitSpider-1.3.0/RabbitSpider/http/
--rw-rw-rw-   0        0        0        1 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/http/__init__.py
--rw-rw-rw-   0        0        0      833 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/http/request.py
--rw-rw-rw-   0        0        0     2698 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/http/response.py
--rw-rw-rw-   0        0        0      379 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-11 01:55:09.366452 RabbitSpider-1.3.0/RabbitSpider/utils/
--rw-rw-rw-   0        0        0        1 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/utils/__init__.py
--rw-rw-rw-   0        0        0     1213 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/utils/control.py
--rw-rw-rw-   0        0        0      483 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/utils/dupefilter.py
--rw-rw-rw-   0        0        0      131 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/utils/expections.py
--rw-rw-rw-   0        0        0     3477 2024-04-11 01:46:55.000000 RabbitSpider-1.3.0/RabbitSpider/utils/fast_monitor.py
--rw-rw-rw-   0        0        0     1879 2024-04-11 01:51:48.000000 RabbitSpider-1.3.0/RabbitSpider/utils/rabbit_go.py
-drwxrwxrwx   0        0        0        0 2024-04-11 01:55:09.366452 RabbitSpider-1.3.0/RabbitSpider.egg-info/
--rw-rw-rw-   0        0        0      560 2024-04-11 01:55:09.000000 RabbitSpider-1.3.0/RabbitSpider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2024-04-11 01:55:09.000000 RabbitSpider-1.3.0/RabbitSpider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 01:55:09.000000 RabbitSpider-1.3.0/RabbitSpider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2024-04-11 01:55:09.000000 RabbitSpider-1.3.0/RabbitSpider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 01:55:09.000000 RabbitSpider-1.3.0/RabbitSpider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 01:55:09.368448 RabbitSpider-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-04-11 01:55:07.000000 RabbitSpider-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.495566 rabbitspider-1.5/
+-rw-rw-rw-   0        0        0      470 2024-04-19 08:41:35.494569 rabbitspider-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2567 2024-04-11 02:19:57.000000 rabbitspider-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.433733 rabbitspider-1.5/RabbitSpider/
+-rw-rw-rw-   0        0        0        0 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.455674 rabbitspider-1.5/RabbitSpider/core/
+-rw-rw-rw-   0        0        0        0 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/core/__init__.py
+-rw-rw-rw-   0        0        0     4090 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/core/download.py
+-rw-rw-rw-   0        0        0     7244 2024-04-19 06:09:05.000000 rabbitspider-1.5/RabbitSpider/core/engine.py
+-rw-rw-rw-   0        0        0     2456 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/core/scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.466677 rabbitspider-1.5/RabbitSpider/http/
+-rw-rw-rw-   0        0        0        1 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/http/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/http/request.py
+-rw-rw-rw-   0        0        0     2698 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/http/response.py
+-rw-rw-rw-   0        0        0      415 2024-04-19 04:58:50.000000 rabbitspider-1.5/RabbitSpider/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.492574 rabbitspider-1.5/RabbitSpider/utils/
+-rw-rw-rw-   0        0        0        1 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/__init__.py
+-rw-rw-rw-   0        0        0     1211 2024-04-19 04:42:59.000000 rabbitspider-1.5/RabbitSpider/utils/control.py
+-rw-rw-rw-   0        0        0      483 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/dupefilter.py
+-rw-rw-rw-   0        0        0      131 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/expections.py
+-rw-rw-rw-   0        0        0     3477 2024-04-11 02:19:57.000000 rabbitspider-1.5/RabbitSpider/utils/fast_monitor.py
+-rw-rw-rw-   0        0        0     1879 2024-04-19 04:01:31.000000 rabbitspider-1.5/RabbitSpider/utils/rabbit_go.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:41:35.493572 rabbitspider-1.5/RabbitSpider.egg-info/
+-rw-rw-rw-   0        0        0      470 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      649 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 08:41:35.000000 rabbitspider-1.5/RabbitSpider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:41:35.495566 rabbitspider-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      612 2024-04-19 08:37:59.000000 rabbitspider-1.5/setup.py
```

### Comparing `RabbitSpider-1.3.0/RabbitSpider/core/download.py` & `rabbitspider-1.5/RabbitSpider/core/download.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.3.0/RabbitSpider/core/engine.py` & `rabbitspider-1.5/RabbitSpider/core/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import asyncio
 import os
 import pickle
 import sys
-from loguru import logger
 from abc import ABC, abstractmethod
 from collections.abc import AsyncGenerator, Coroutine
 from traceback import print_exc
 from typing import Optional
 from aio_pika.abc import AbstractIncomingMessage
-from RabbitSpider.core.scheduler import Scheduler
-from aio_pika.exceptions import QueueEmpty, ChannelClosed
-from RabbitSpider.utils.control import SettingManager
-from RabbitSpider.utils.dupefilter import RFPDupeFilter
+from loguru import logger
 from RabbitSpider.http.request import Request
 from RabbitSpider.utils.control import TaskManager
+from RabbitSpider.utils.control import SettingManager
+from RabbitSpider.utils.dupefilter import RFPDupeFilter
 from RabbitSpider.utils.expections import RabbitExpect
+from RabbitSpider.core.scheduler import Scheduler
 from RabbitSpider.core.download import CurlDownload, AiohttpDownload
+from aio_pika.exceptions import QueueEmpty, ChannelClosed
 
 
 class Engine(ABC):
     queue = os.path.basename(sys.argv[0])
     allow_status_code: list = [200]
     max_retry: int = 5
     http2 = False
@@ -27,17 +27,19 @@
 
     def __init__(self, sync):
         self._filter = None
         self._scheduler = None
         self._connection = None
         self._channel = None
         self._download = None
+        self._task_manager = None
         self._sync = sync
+        self.logger = None
         self.settings = SettingManager()
-        self.task_manager = TaskManager(self._sync)
+        self._task_manager = TaskManager(self._sync)
 
     async def start_spider(self):
         await self._scheduler.create_queue(self._channel, self.queue)
         start_request = self.start_requests()
         await self.routing(start_request)
 
     @abstractmethod
@@ -62,18 +64,18 @@
     async def routing(self, result):
         if isinstance(result, AsyncGenerator):
             async for req in result:
                 if isinstance(req, Request):
                     ret = pickle.dumps(req.model_dump())
                     if req.dupe_filter:
                         if self._filter.request_seen(ret):
-                            logger.info(f'生产数据：{req.model_dump()}')
+                            self.logger.info(f'生产数据：{req.model_dump()}')
                             await self._scheduler.producer(self._channel, queue=self.queue, body=ret)
                     else:
-                        logger.info(f'生产数据：{req.model_dump()}')
+                        self.logger.info(f'生产数据：{req.model_dump()}')
                         await self._scheduler.producer(self._channel, queue=self.queue, body=ret)
 
                 elif isinstance(req, dict):
                     await self.save_item(req)
         elif isinstance(result, Coroutine):
             await result
         else:
@@ -82,48 +84,48 @@
     async def crawl(self):
         session = await self._download.new_session()
         while True:
             try:
                 incoming_message: Optional[AbstractIncomingMessage] = await self._scheduler.consumer(self._channel,
                                                                                                      queue=self.queue)
             except QueueEmpty:
-                if self.task_manager.all_done():
+                if self._task_manager.all_done():
                     await self._download.exit(session)
                     await self._scheduler.delete_queue(self._channel, self.queue)
                     await self._channel.close()
                     await self._connection.close()
                     break
                 else:
                     continue
             except ChannelClosed:
                 self._connection, self._channel = self._scheduler.connect()
-                logger.warning('mq重新连接!')
+                self.logger.warning('mq重新连接!')
                 continue
             if incoming_message:
-                await self.task_manager.semaphore.acquire()
-                self.task_manager.create_task(self.deal_resp(incoming_message, session))
+                await self._task_manager.semaphore.acquire()
+                self._task_manager.create_task(self.deal_resp(incoming_message, session))
             else:
                 print(incoming_message)
 
     async def consume(self):
         session = await self._download.new_session()
         while True:
             try:
                 await self._scheduler.consumer(self._channel, queue=self.queue, callback=self.deal_resp,
                                                prefetch=self._sync,
                                                args=session)
                 break
             except ChannelClosed:
                 self._connection, self._channel = self._scheduler.connect()
-                logger.warning('mq重新连接!')
+                self.logger.warning('mq重新连接!')
 
     async def deal_resp(self, incoming_message: AbstractIncomingMessage, session):
         ret = self.before_request(pickle.loads(incoming_message.body))
         try:
-            logger.info(f'消费数据：{ret}')
+            self.logger.info(f'消费数据：{ret}')
             response = await self._download.fetch(session, ret)
         except Exception:
             print_exc()
             response = None
         if response and response.status in self.allow_status_code:
             try:
                 callback = getattr(self, ret['callback'])
@@ -136,18 +138,23 @@
                     task.cancel()
         else:
             if ret['retry'] < self.max_retry:
                 ret['retry'] += 1
                 await self._scheduler.producer(self._channel, queue=self.queue, body=pickle.dumps(ret),
                                                priority=ret['retry'])
             else:
-                logger.error(f'请求失败：{ret}')
+                self.logger.error(f'请求失败：{ret}')
         await incoming_message.ack()
 
     async def run(self, mode):
+        logger.add("../rabbit_log/rabbit_{time:YYYY-MM-DD}.log", level=self.settings.get('LOG_LEVEL'), rotation="1 day",
+                   retention="1 week",
+                   format="{time:YYYY-MM-DD HH:mm:ss.sss} | {level}  | {extra[scope]} | {name}:{line} - {message}")
+        self.logger = logger.bind(scope=self.queue)
+
         self._filter = RFPDupeFilter(self.settings.get('REDIS_FILTER_NAME'),
                                      self.settings.get('REDIS_QUEUE_HOST'),
                                      self.settings.get('REDIS_QUEUE_PORT'),
                                      self.settings.get('REDIS_QUEUE_DB'))
 
         self._scheduler = Scheduler(self.settings.get('RABBIT_USERNAME'),
                                     self.settings.get('RABBIT_PASSWORD'),
@@ -164,8 +171,8 @@
             await self.start_spider()
             await self.crawl()
         elif mode == 'm':
             await self.start_spider()
         elif mode == 'w':
             await self.consume()
         else:
-            raise RabbitExpect('执行模式错误！')
+            raise RabbitExpect('执行模式错误！')
```

### Comparing `RabbitSpider-1.3.0/RabbitSpider/core/scheduler.py` & `rabbitspider-1.5/RabbitSpider/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.3.0/RabbitSpider/http/request.py` & `rabbitspider-1.5/RabbitSpider/http/request.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.3.0/RabbitSpider/http/response.py` & `rabbitspider-1.5/RabbitSpider/http/response.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.3.0/RabbitSpider/utils/control.py` & `rabbitspider-1.5/RabbitSpider/utils/control.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,23 +25,26 @@
 
     def set(self, key, value):
         self[key] = value
 
 
 class TaskManager(object):
     def __init__(self, sync: int):
-        self.current_task: Final[list] = list()
+        self.current_task: Final[set] = set()
         self.semaphore = Semaphore(sync)
 
     def create_task(self, coroutine) -> Task:
         task = asyncio.create_task(coroutine)
-        self.current_task.append(task)
+        self.current_task.add(task)
 
         def done_callback(_fut: Future):
             self.current_task.remove(task)
             self.semaphore.release()
 
         task.add_done_callback(done_callback)
         return task
 
     def all_done(self):
         return len(self.current_task) == 0
+
+
+
```

### Comparing `RabbitSpider-1.3.0/RabbitSpider/utils/fast_monitor.py` & `rabbitspider-1.5/RabbitSpider/utils/fast_monitor.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.3.0/RabbitSpider/utils/rabbit_go.py` & `rabbitspider-1.5/RabbitSpider/utils/rabbit_go.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.3.0/RabbitSpider.egg-info/SOURCES.txt` & `rabbitspider-1.5/RabbitSpider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.3.0/setup.py` & `rabbitspider-1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from setuptools import setup, find_packages
+import setuptools
 
-setup(
+setuptools.setup(
     name='RabbitSpider',
-    version='1.3.0',
+    version='1.5',
+    author='一纸',
     author_email='2395396520@qq.com',
+    url='https://github.com/YunTom/RabbitSpider/tree/master',
     packages=['RabbitSpider', 'RabbitSpider.core', 'RabbitSpider.http', 'RabbitSpider.utils'],
     python_requires='>=3.8',
     install_requires=[
-        'aio-pika~=9.4.1',
-        'aiohttp~=3.9.3',
-        'pydantic~=2.6.4',
-        'chardet~=5.2.0',
-        'parsel~=1.9.0',
-        'w3lib~=2.1.2',
-        'requests~=2.31.0',
-        'redis~=5.0.3',
-        'uvicorn~=0.29.0',
-        'starlette~=0.37.2',
-        'fastapi~=0.110.1',
-        'SQLAlchemy~=2.0.29',
-        'loguru~=0.7.2',
-        'curl_cffi~=0.6.2'
-    ]
+        'aio-pika>=9.4.1',
+        'aiohttp>=3.9.5',
+        'curl_cffi>=0.6.2',
+        'loguru>=0.7.2',
+        'parsel>=1.9.1',
+        'pydantic>=2.7.0',
+        'redis>=5.0.3',
+        'w3lib>=2.1.2',
+        'chardet>=5.2.0',
+    ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

