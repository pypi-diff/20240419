# Comparing `tmp/replit_river-0.1.6.tar.gz` & `tmp/replit_river-0.1.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.6.tar", max compression
+gzip compressed data, was "replit_river-0.1.7b1.tar", max compression
```

## Comparing `replit_river-0.1.6.tar` & `replit_river-0.1.7b1.tar`

### file list

```diff
@@ -1,19 +1,26 @@
--rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.6/LICENSE
--rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.6/README.md
--rw-r--r--   0        0        0     1742 2024-04-17 19:11:30.870951 replit_river-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-17 00:20:58.071349 replit_river-0.1.6/replit_river/__init__.py
--rw-r--r--   0        0        0    19574 2024-04-17 18:56:54.976159 replit_river-0.1.6/replit_river/client.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.6/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.6/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-17 00:20:58.072227 replit_river-0.1.6/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.6/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.6/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12620 2024-04-17 19:05:12.058141 replit_river-0.1.6/replit_river/codegen/server.py
--rw-r--r--   0        0        0      478 2024-04-17 00:20:58.073048 replit_river-0.1.6/replit_river/error_schema.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.6/replit_river/py.typed
--rw-r--r--   0        0        0    11973 2024-04-17 19:05:34.905421 replit_river-0.1.6/replit_river/rpc.py
--rw-r--r--   0        0        0     2152 2024-04-17 00:20:58.073573 replit_river-0.1.6/replit_river/seq_manager.py
--rw-r--r--   0        0        0     1340 2024-04-17 00:20:58.073881 replit_river-0.1.6/replit_river/server.py
--rw-r--r--   0        0        0     2336 2024-04-17 19:05:00.731417 replit_river-0.1.6/replit_river/task_manager.py
--rw-r--r--   0        0        0    14852 2024-04-17 19:05:12.100062 replit_river-0.1.6/replit_river/transport.py
--rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 replit_river-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.7b1/LICENSE
+-rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.7b1/README.md
+-rw-r--r--   0        0        0     1749 2024-04-18 22:55:32.006505 replit_river-0.1.7b1/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-17 00:20:58.071349 replit_river-0.1.7b1/replit_river/__init__.py
+-rw-r--r--   0        0        0     5174 2024-04-18 22:52:24.688442 replit_river-0.1.7b1/replit_river/client.py
+-rw-r--r--   0        0        0    11759 2024-04-18 22:24:01.621432 replit_river-0.1.7b1/replit_river/client_session.py
+-rw-r--r--   0        0        0     4314 2024-04-18 08:52:55.632770 replit_river-0.1.7b1/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.7b1/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.7b1/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13363 2024-04-17 00:20:58.072227 replit_river-0.1.7b1/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.7b1/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.7b1/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12620 2024-04-17 19:05:12.058141 replit_river-0.1.7b1/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      515 2024-04-18 05:17:58.181429 replit_river-0.1.7b1/replit_river/error_schema.py
+-rw-r--r--   0        0        0     1207 2024-04-18 21:12:58.850511 replit_river-0.1.7b1/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     2517 2024-04-18 09:00:07.281730 replit_river-0.1.7b1/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.7b1/replit_river/py.typed
+-rw-r--r--   0        0        0    11973 2024-04-17 19:05:34.905421 replit_river-0.1.7b1/replit_river/rpc.py
+-rw-r--r--   0        0        0     2138 2024-04-18 05:49:40.092134 replit_river-0.1.7b1/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     1763 2024-04-18 22:44:37.391550 replit_river-0.1.7b1/replit_river/server.py
+-rw-r--r--   0        0        0     6248 2024-04-18 22:49:44.450317 replit_river-0.1.7b1/replit_river/server_transport.py
+-rw-r--r--   0        0        0    13435 2024-04-18 21:13:20.653051 replit_river-0.1.7b1/replit_river/session.py
+-rw-r--r--   0        0        0     2336 2024-04-18 08:09:29.872971 replit_river-0.1.7b1/replit_river/task_manager.py
+-rw-r--r--   0        0        0     1208 2024-04-18 22:47:19.826728 replit_river-0.1.7b1/replit_river/transport.py
+-rw-r--r--   0        0        0     1329 2024-04-18 08:30:42.434967 replit_river-0.1.7b1/replit_river/transport_options.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b1/PKG-INFO
```

### Comparing `replit_river-0.1.6/LICENSE` & `replit_river-0.1.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/README.md` & `replit_river-0.1.7b1/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/pyproject.toml` & `replit_river-0.1.7b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.6"
+version="0.1.7-beta.1"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.6/replit_river/codegen/client.py` & `replit_river-0.1.7b1/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/replit_river/codegen/run.py` & `replit_river-0.1.7b1/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/replit_river/codegen/schema.py` & `replit_river-0.1.7b1/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/replit_river/codegen/server.py` & `replit_river-0.1.7b1/replit_river/codegen/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/replit_river/rpc.py` & `replit_river-0.1.7b1/replit_river/rpc.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/replit_river/seq_manager.py` & `replit_river-0.1.7b1/replit_river/seq_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import logging
 
 from replit_river.rpc import TransportMessage
 
 
 class IgnoreTransportMessageException(Exception):
     """Exception to ignore a transport message, but good to continue."""
 
@@ -22,14 +21,15 @@
     def __init__(
         self,
     ) -> None:
         self._seq_lock = asyncio.Lock()
         self.seq = 0
         self._ack_lock = asyncio.Lock()
         self.ack = 0
+        self.receiver_ack = 0
 
     async def get_seq_and_increment(self) -> int:
         """Get the current sequence number and increment it.
         This removes one lock acquire than get_seq and increment_seq separately.
         """
         async with self._seq_lock:
             current_value = self.seq
@@ -49,24 +49,23 @@
         async with self._ack_lock:
             return self.ack
 
     async def check_seq_and_update(self, msg: TransportMessage) -> None:
         async with self._ack_lock:
             if msg.seq != self.ack:
                 if msg.seq < self.ack:
-                    logging.debug(
+                    raise IgnoreTransportMessageException(
                         f"{msg.from_} received duplicate msg, got {msg.seq}"
                         f" expected {self.ack}"
                     )
-                    raise IgnoreTransportMessageException
                 else:
-                    logging.error(
-                        f"{msg.from_} received duplicate msg, got {msg.seq}"
+                    raise InvalidTransportMessageException(
+                        f"{msg.from_} received out of order, got {msg.seq}"
                         f" expected {self.ack}"
                     )
-                    raise InvalidTransportMessageException
+            self.receiver_ack = msg.ack
         await self._set_ack(msg.seq + 1)
 
     async def _set_ack(self, new_ack: int) -> int:
         async with self._ack_lock:
             self.ack = new_ack
             return self.ack
```

### Comparing `replit_river-0.1.6/replit_river/server.py` & `replit_river-0.1.7b1/replit_river/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 import logging
-from typing import Dict, Mapping, Tuple
+from typing import Mapping, Tuple
 
-import nanoid  # type: ignore
 from websockets.exceptions import ConnectionClosedError
 from websockets.server import WebSocketServerProtocol
 
-from replit_river.transport import Transport, TransportManager
+from replit_river.server_transport import ServerTransport
+from replit_river.transport import TransportOptions
 
 from .rpc import (
     GenericRpcHandler,
 )
 
 
 class Server(object):
-    def __init__(self, server_id: str) -> None:
-        self._handlers: Dict[Tuple[str, str], Tuple[str, GenericRpcHandler]] = {}
-        self._server_id = server_id or nanoid.generate()
-        self._transport_manager = TransportManager()
+    def __init__(self, server_id: str, transport_options: TransportOptions) -> None:
+        self._server_id = server_id or "SERVER"
+        self._transport_options = transport_options
+        self._transport = ServerTransport(
+            transport_id=self._server_id,
+            transport_options=transport_options,
+            is_server=True,
+        )
+
+    async def close(self) -> None:
+        await self._transport.close_all_sessions()
 
     def add_rpc_handlers(
         self,
         rpc_handlers: Mapping[Tuple[str, str], Tuple[str, GenericRpcHandler]],
     ) -> None:
-        self._handlers.update(rpc_handlers)
+        self._transport._handlers.update(rpc_handlers)
 
     async def serve(self, websocket: WebSocketServerProtocol) -> None:
-        logging.debug("got a client")
-        transport = Transport(
-            self._server_id, self._handlers, websocket, self._transport_manager
-        )
+        logging.debug("River server started establishing session")
+        try:
+            session = await self._transport.establish_session(websocket)
+        except Exception as e:
+            logging.error(f"Error establishing handshake, closing websocket: {e}")
+            await websocket.close()
+            return
+        logging.debug("River server session established, start serving messages")
         try:
-            await transport.serve()
+            await session._serve()
         except ConnectionClosedError as e:
             logging.debug(f"ConnectionClosedError while serving {e}")
         except Exception as e:
             logging.error(f"River transport error in server {self._server_id}: {e}")
-        finally:
-            if transport:
-                await transport.close()
+            await websocket.close()
```

### Comparing `replit_river-0.1.6/replit_river/task_manager.py` & `replit_river-0.1.7b1/replit_river/task_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.6/PKG-INFO` & `replit_river-0.1.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.6
+Version: 0.1.7b1
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

