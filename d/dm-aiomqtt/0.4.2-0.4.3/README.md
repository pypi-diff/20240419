# Comparing `tmp/dm_aiomqtt-0.4.2.tar.gz` & `tmp/dm_aiomqtt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_aiomqtt-0.4.2.tar", last modified: Thu Apr 18 16:44:20 2024, max compression
+gzip compressed data, was "dm_aiomqtt-0.4.3.tar", last modified: Fri Apr 19 08:01:03 2024, max compression
```

## Comparing `dm_aiomqtt-0.4.2.tar` & `dm_aiomqtt-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-18 16:44:12.000000 dm_aiomqtt-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/dm_aiomqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 16:44:12.000000 dm_aiomqtt-0.4.2/dm_aiomqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-04-18 16:44:12.000000 dm_aiomqtt-0.4.2/dm_aiomqtt/dm_aiomqtt_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-19 08:00:52.000000 dm_aiomqtt-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:03.837780 dm_aiomqtt-0.4.3/dm_aiomqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 08:00:52.000000 dm_aiomqtt-0.4.3/dm_aiomqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-19 08:00:52.000000 dm_aiomqtt-0.4.3/dm_aiomqtt/dm_aiomqtt_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/setup.py
```

### Comparing `dm_aiomqtt-0.4.2/PKG-INFO` & `dm_aiomqtt-0.4.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: dm-aiomqtt
-Version: 0.4.2
-Summary: This is my custom aiomqtt client
-Home-page: https://pypi.org/project/dm-aiomqtt
-Author: dimka4621
-Author-email: mismartconfig@gmail.com
-Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
-Keywords: dm aiomqtt
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: dm-logger==0.5.2
-Requires-Dist: aiomqtt==2.0.0
-
 # DM-aiomqtt
 
 ## Urls
 
 * [PyPI](https://pypi.org/project/dm-aiomqtt)
 * [GitHub](https://github.com/DIMKA4621/dm-aiomqtt)
 
@@ -78,14 +61,34 @@
        port=8883,
        ca_crt="ssl/ca.crt",
        client_crt="ssl/client.crt",
        client_key="ssl/client.key"
    )
    ```
 
+### RESEND_NOT_SUCCESS_MESSAGES
+
+Set this parameter `resend_not_success_messages=True` when create mqtt client
+
+   ```python
+   mqtt_client = DMAioMqttClient(
+       host="localhost",
+       port=1883,
+       resend_not_success_messages=True
+   )
+   ```
+
+Now, in case of loss of connection, all messages that were sent during this period will be re-sent as soon as the connection appears again.
+**BUT** the `payload` will be in a changed format `[your_payload]_dt_[iso_local_datetime]`
+
+**Example**:
+Your payload: `"{"temp": 12}"`
+Edited payload: `"{"temp": 12}_dt_2024-04-19T09:57:40"`
+
+
 ### Set custom logger
 
 _If you want set up custom logger_
 
 ```python
 from dm_aiomqtt import DMAioMqttClient
```

### Comparing `dm_aiomqtt-0.4.2/dm_aiomqtt/dm_aiomqtt_client.py` & `dm_aiomqtt-0.4.3/dm_aiomqtt/dm_aiomqtt_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dm_logger import DMLogger
 from typing import Union, Callable, Coroutine, Literal, List, Optional
 import asyncio
 import aiomqtt
 import json
-import uuid
 import ssl
 import re
 import os
+from .message_db import MessageDB
 
 
 class DMAioMqttClient:
     """
     See usage examples here:
         https://pypi.org/project/dm-aiomqtt
         https://github.com/DIMKA4621/dm-aiomqtt
@@ -29,15 +29,16 @@
         username: str = "",
         password: str = "",
         ca_crt: str = "",
         client_crt: str = "",
         client_key: str = "",
         keepalive: int = 5,
         identifier: str = None,
-        clean_session: bool = True
+        clean_session: bool = True,
+        resend_not_success_messages: bool = False
     ) -> None:
         if self.__logger is None:
             self.__logger = DMLogger(f"DMAioMqttClient-{host}:{port}")
 
         self.__mqtt_config = {
             "hostname": host,
             "port": port,
@@ -49,27 +50,33 @@
         if username or password:
             self.__mqtt_config["username"] = username
             self.__mqtt_config["password"] = password
         self.__mqtt_config["tls_context"] = self.__get_tls_context(ca_crt, client_crt, client_key)
 
         self.__subscribes = {}
         self.__pattern_subscribes = {}
+        self.__resend_ns_msg = resend_not_success_messages
+        self.__message_db = MessageDB()
+
         self.__client: aiomqtt.Client = aiomqtt.Client(**self.__mqtt_config)
         self.__connected_event = asyncio.Event()
 
     async def start(self) -> None:
         _ = asyncio.create_task(self.__connect_loop())
         await self.__connected_event.wait()
 
     async def __connect_loop(self) -> None:
         while True:
             try:
                 async with aiomqtt.Client(**self.__mqtt_config) as self.__client:
                     self.__logger.info("Connected!")
                     self.__connected_event.set()
+
+                    if self.__resend_ns_msg:
+                        await self.__resend_not_success_messages()
                     await self.__subscribe()
                     await self.__listen()
             except Exception as e:
                 if self.__connected_event.is_set():
                     self.__logger.error(f"Error: {e}")
                 self.__connected_event.clear()
                 self.__connecting = False
@@ -123,25 +130,32 @@
                 will not be converted
         """
 
         async def cb(payload):
             if payload_to_json is True or (payload_to_json == "auto" and type(payload) not in (str, int, float)):
                 payload = json.dumps(payload, ensure_ascii=False)
             try:
-                await self.__connected_event.wait()
                 await self.__client.publish(topic, payload, qos)
             except Exception as e:
+                if self.__resend_ns_msg:
+                    await self.__message_db.insert([topic, payload, qos])
                 if error_logging:
                     self.__logger.warning(f"Publish not sent: {e}")
             else:
                 if sent_logging:
                     self.__logger.debug(f"Published message to '{topic}' topic ({qos=}): {payload}")
 
         _ = asyncio.create_task(cb(payload))
 
+    async def __resend_not_success_messages(self) -> None:
+        messages = await self.__message_db.get_all()
+        for topic, payload, qos, iso_dt in messages:
+            payload = f"{payload}_dt_{iso_dt}"
+            self.publish(topic, payload, qos)
+
     def __get_callbacks_from_pattern_subscribes(self, current_topic: str) -> List[Callable]:
         callbacks = []
         for topic, params in self.__pattern_subscribes.items():
             pattern = topic.replace("+", "[^/]+?")
             pattern = pattern.replace("/#", "(/.+)*")
             if re.search(pattern, current_topic):
                 callbacks.append(params["cb"])
```

### Comparing `dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/PKG-INFO` & `dm_aiomqtt-0.4.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.2
+Version: 0.4.3
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
@@ -78,14 +78,34 @@
        port=8883,
        ca_crt="ssl/ca.crt",
        client_crt="ssl/client.crt",
        client_key="ssl/client.key"
    )
    ```
 
+### RESEND_NOT_SUCCESS_MESSAGES
+
+Set this parameter `resend_not_success_messages=True` when create mqtt client
+
+   ```python
+   mqtt_client = DMAioMqttClient(
+       host="localhost",
+       port=1883,
+       resend_not_success_messages=True
+   )
+   ```
+
+Now, in case of loss of connection, all messages that were sent during this period will be re-sent as soon as the connection appears again.
+**BUT** the `payload` will be in a changed format `[your_payload]_dt_[iso_local_datetime]`
+
+**Example**:
+Your payload: `"{"temp": 12}"`
+Edited payload: `"{"temp": 12}_dt_2024-04-19T09:57:40"`
+
+
 ### Set custom logger
 
 _If you want set up custom logger_
 
 ```python
 from dm_aiomqtt import DMAioMqttClient
```

### Comparing `dm_aiomqtt-0.4.2/setup.py` & `dm_aiomqtt-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomqtt',
-    version='v0.4.2',
+    version='v0.4.3',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomqtt client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomqtt',
     packages=find_packages(),
```

