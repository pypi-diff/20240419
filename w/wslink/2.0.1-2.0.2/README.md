# Comparing `tmp/wslink-2.0.1.tar.gz` & `tmp/wslink-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wslink-2.0.1.tar", last modified: Tue Apr 16 15:42:42 2024, max compression
+gzip compressed data, was "wslink-2.0.2.tar", last modified: Thu Apr 18 23:22:34 2024, max compression
```

## Comparing `wslink-2.0.1.tar` & `wslink-2.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 15:42:08.000000 wslink-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-16 15:42:42.576406 wslink-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-16 15:42:08.000000 wslink-2.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 15:42:42.576406 wslink-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-16 15:42:08.000000 wslink-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.572406 wslink-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/aiohttp/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/aiohttp/relay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/generic/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/jupyter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/tornado/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/tornado/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/chunking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21170 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/ssl_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 23:22:03.000000 wslink-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-18 23:22:34.727270 wslink-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-18 23:22:03.000000 wslink-2.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 23:22:34.727270 wslink-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-18 23:22:03.000000 wslink-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.719271 wslink-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/backends/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/aiohttp/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/aiohttp/relay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/backends/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/generic/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/src/wslink/backends/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/jupyter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/src/wslink/backends/tornado/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/tornado/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/chunking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21170 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/ssl_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/src/wslink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/top_level.txt
```

### Comparing `wslink-2.0.1/PKG-INFO` & `wslink-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-2.0.1/README.rst` & `wslink-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/setup.py` & `wslink-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/LICENSE` & `wslink-2.0.2/src/wslink/LICENSE`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/__init__.py` & `wslink-2.0.2/src/wslink/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/backends/__init__.py` & `wslink-2.0.2/src/wslink/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/backends/aiohttp/__init__.py` & `wslink-2.0.2/src/wslink/backends/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/backends/aiohttp/launcher.py` & `wslink-2.0.2/src/wslink/backends/aiohttp/launcher.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/backends/aiohttp/relay.py` & `wslink-2.0.2/src/wslink/backends/aiohttp/relay.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/backends/generic/core.py` & `wslink-2.0.2/src/wslink/backends/generic/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,58 +20,62 @@
 
     def on_message(self, callback):
         self._on_message_fn = callback
 
     async def send(self, is_binary, msg):
         await self._ws.onMessage(is_binary, msg, self.client_id)
 
-    def close(self):
-        self._ws.disconnect(self)
+    async def close(self):
+        await self.on_close(self._ws)
 
     # -------------------------------------------------------------------------
     # Method used by FakeWS
     # -------------------------------------------------------------------------
 
     @property
     def client_id(self):
         return self._id
 
-    def on_connect(self, ws):
+    async def on_connect(self, ws):
         self.closed = False
         self._ws = ws
+        await self._ws.onConnect(
+            {"type": "generic", "connection": self}, self.client_id
+        )
 
-    def on_close(self, ws):
+    async def on_close(self, ws):
         self.closed = True
         if self._ws == ws:
+            ws.disconnect(self.client_id)
             self._ws = None
 
     async def send_str(self, value):
         await self._on_message_fn(False, value)
 
     async def send_bytes(self, value):
         await self._on_message_fn(True, value)
 
 
 class WsEndpoint(WslinkHandler):
     def __init__(self, protocol=None, web_app=None):
         super().__init__(protocol, web_app)
 
-    def connect(self):
+    async def connect(self):
         conn = WsConnection()
         self.connections[conn.client_id] = conn
-        conn.on_connect(self)
+        await conn.on_connect(self)
         return conn
 
-    def disconnect(self, client_or_id):
+    async def disconnect(self, client_or_id):
         client_or_id = (
             client_or_id if isinstance(client_or_id, str) else client_or_id.client_id
         )
         if client_or_id in self.connections:
             client = self.connections.pop(client_or_id)
-            client.on_close(self)
+            await client.onClose(client_or_id)
 
 
 class GenericServer(AbstractWebApp):
     def __init__(self, server_config):
         AbstractWebApp.__init__(self, server_config)
         self._websockets = {}
         self._stop_event = asyncio.Event()
```

### Comparing `wslink-2.0.1/src/wslink/backends/jupyter/core.py` & `wslink-2.0.2/src/wslink/backends/jupyter/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         if server_name != self._name:
             return
 
         connection = self._connections.get(client_id, None)
 
         if connection is None:
-            connection = self._endpoint.connect()
+            connection = await self._endpoint.connect()
             connection.on_message(partial(self.on_msg_from_server, client_id))
             self._connections[client_id] = connection
 
         is_binary = len(buffers) > 0
 
         message = None
```

### Comparing `wslink-2.0.1/src/wslink/backends/tornado/core.py` & `wslink-2.0.2/src/wslink/backends/tornado/core.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/chunking.py` & `wslink-2.0.2/src/wslink/chunking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import secrets
 import msgpack
 from typing import Dict, Tuple, Union
+
 if sys.version_info >= (3, 8):
     from typing import TypedDict  # pylint: disable=no-name-in-module
 else:
     from typing_extensions import TypedDict
 
 UINT32_LENGTH = 4
 ID_LOCATION = 0
@@ -14,24 +15,28 @@
 MESSAGE_OFFSET_LENGTH = UINT32_LENGTH
 MESSAGE_SIZE_LOCATION = MESSAGE_OFFSET_LOCATION + MESSAGE_OFFSET_LENGTH
 MESSAGE_SIZE_LENGTH = UINT32_LENGTH
 
 HEADER_LENGTH = ID_LENGTH + MESSAGE_OFFSET_LENGTH + MESSAGE_SIZE_LENGTH
 
 
-def _encode_header(id: bytes, offset: int, size: int) -> bytes:
+def _encode_header(id: int, offset: int, size: int) -> bytes:
     return (
-        id
+        id.to_bytes(ID_LENGTH, "little", signed=False)
         + offset.to_bytes(MESSAGE_OFFSET_LENGTH, "little", signed=False)
         + size.to_bytes(MESSAGE_SIZE_LENGTH, "little", signed=False)
     )
 
 
-def _decode_header(header: bytes) -> Tuple[bytes, int, int]:
-    id = header[ID_LOCATION:ID_LENGTH]
+def _decode_header(header: bytes) -> Tuple[int, int, int]:
+    id = int.from_bytes(
+        header[ID_LOCATION:ID_LENGTH],
+        "little",
+        signed=False,
+    )
     offset = int.from_bytes(
         header[
             MESSAGE_OFFSET_LOCATION : MESSAGE_OFFSET_LOCATION + MESSAGE_OFFSET_LENGTH
         ],
         "little",
         signed=False,
     )
@@ -47,15 +52,15 @@
     total_size = len(message)
 
     if max_size == 0:
         max_content_size = total_size
     else:
         max_content_size = max(max_size - HEADER_LENGTH, 1)
 
-    id = secrets.token_bytes(ID_LENGTH)
+    id = int.from_bytes(secrets.token_bytes(ID_LENGTH), "little", signed=False)
 
     offset = 0
 
     while offset < total_size:
         header = _encode_header(id, offset, total_size)
         chunk_content = message[offset : offset + max_content_size]
```

### Comparing `wslink-2.0.1/src/wslink/launcher.py` & `wslink-2.0.2/src/wslink/launcher.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/protocol.py` & `wslink-2.0.2/src/wslink/protocol.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/publish.py` & `wslink-2.0.2/src/wslink/publish.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/server.py` & `wslink-2.0.2/src/wslink/server.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/ssl_context.py` & `wslink-2.0.2/src/wslink/ssl_context.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink/websocket.py` & `wslink-2.0.2/src/wslink/websocket.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.1/src/wslink.egg-info/PKG-INFO` & `wslink-2.0.2/src/wslink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-2.0.1/src/wslink.egg-info/SOURCES.txt` & `wslink-2.0.2/src/wslink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

