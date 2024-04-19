# Comparing `tmp/scratchcommunication-2.3.2.tar.gz` & `tmp/scratchcommunication-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.3.2.tar", last modified: Fri Apr 12 19:15:58 2024, max compression
+gzip compressed data, was "scratchcommunication-2.4.1.tar", last modified: Fri Apr 19 12:59:09 2024, max compression
```

## Comparing `scratchcommunication-2.3.2.tar` & `scratchcommunication-2.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:15:58.089802 scratchcommunication-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-12 19:15:58.085802 scratchcommunication-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12692 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:15:58.085802 scratchcommunication-2.3.2/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:15:58.085802 scratchcommunication-2.3.2/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:15:58.085802 scratchcommunication-2.3.2/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-12 19:15:58.000000 scratchcommunication-2.3.2/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 19:15:58.000000 scratchcommunication-2.3.2/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:15:58.000000 scratchcommunication-2.3.2/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 19:15:58.000000 scratchcommunication-2.3.2/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 19:15:58.000000 scratchcommunication-2.3.2/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:15:58.089802 scratchcommunication-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:15:58.085802 scratchcommunication-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 19:15:54.000000 scratchcommunication-2.3.2/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15014 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17966 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/tests/test1.py
```

### Comparing `scratchcommunication-2.3.2/LICENSE` & `scratchcommunication-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.3.2/PKG-INFO` & `scratchcommunication-2.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.3.2
+Version: 2.4.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -117,15 +117,16 @@
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
     accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
-    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
+    keep_all_events = False, # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
+    contact_info = None # (Optional) Allows you to give turbowarp your contact info. If you don't add any it defaults to your session username or nothing.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
@@ -133,15 +134,16 @@
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
     accept_strs = False,
-    keep_all_events = False
+    keep_all_events = False,
+    contact_info = None
 )
 ```
 
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
@@ -213,15 +215,15 @@
 )
 ```
 
 If you set `daemon_thread` to `True` when creating the object, the background thread will terminate when your process ends.
 
 # Cloud requests
 
-Cloud requests are based on cloud sockets and allow you to have your project send requests to your server which it automatically responds to.
+Cloud requests are based on cloud sockets and allow you to have your project send requests to your server which it automatically responds to. You'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
 
 ## Creating a cloud requests handler
 
 To use cloud requests, you first need to create a [cloud socket](#cloud-sockets) to your project and then a cloud requests handler which uses it to communicate to your Scratch project.
 
 ```python
 cloud_requests = scratchcommunication.RequestHandler(
@@ -271,14 +273,28 @@
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
 
 ```python
 cloud_requests.stop()
 ```
 
+## Encrypted data transmition
+
+See [Cloud Socket Security](#cloud-socket-security) for this.
+
+## Client side
+
+If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
+
+You'll always first need to connect on your client side for your messages to work. This is done using the "[cloud socket] connect securely" or "[cloud socket] connect insecurely" blocks. 
+
+When you are connected, you can use the block "[cloud requests] initiate new request (%s)" to initiate a new request with its name. The name must not contain spaces. When you have initiated a new request, you can add arguments to the request by using the "[cloud requests] add argument (%s)" block. When you are done creating the request, you can use the block "[cloud requests] send iniated request" to send it and wait for the response.
+
+The received data will be in the variable "[cloud] reception". You can change the timeout using the "# TIMEOUT" variable (If you don't need a timeout, just let it stay). You can also change the packet size using the "# PACKET SIZE" variable, but I would advise against this if you are not using turbowarp.
+
 # Cloud sockets
 
 Cloud sockets (inspired by sockets) are connections from a scratch project to a python program where both sides can send data to one another and there is even the possibility to add security to the connection using RSA.
 
 Warning: Cloud sockets are low level. They allow you to do more but are more difficult to use. You shouldn't use them directly. You might want to use them in [cloud requests](#cloud-requests) instead.
 
 ## Creating a cloud socket
@@ -328,20 +344,30 @@
 ```python
 msg = client.recv()
 client.send("Hello!")
 ```
 
 **Your messages will be public and easy to fake in both direction unless you activate [security](#cloud-socket-security).**
 
-In order to stop the cloud socket from running anymore you can you `scratchcommunication.cloud_socket.CloudSocket.stop`
+In order to stop the cloud socket from running anymore you can use `scratchcommunication.cloud_socket.CloudSocket.stop`
 
 ```python
 cloud_socket.stop()
 ```
 
+## Client side
+
+If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud socket to work.
+
+You'll always first need to connect on your client side for your messages to work. This is done using the "[cloud socket] connect securely" or "[cloud socket] connect insecurely" blocks. 
+
+Afterwards, you can use the "[cloud socket] send (%s)" block and the "[cloud socket] recv" block. 
+
+The received data will be in the variable "[cloud] reception". You can change the timeout using the "# TIMEOUT" variable (If you don't need a timeout, just let it stay). You can also change the packet size using the "# PACKET SIZE" variable, but I would advise against this if you are not using turbowarp.
+
 ## Cloud Socket Security
 
 You might want to be able to send private data that only the designated recipient can read, but that is impossible unless you use asymmetric encryption or something similar. Fortunately for you, the hard work has already been done.
 
 You will need to generate RSA keys for this. In order to do that, you can just use `scratchcommunication.security.RSAKeys.create_new_keys`.
 
 ```python
```

### Comparing `scratchcommunication-2.3.2/README.md` & `scratchcommunication-2.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -93,15 +93,16 @@
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
     accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
-    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
+    keep_all_events = False, # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
+    contact_info = None # (Optional) Allows you to give turbowarp your contact info. If you don't add any it defaults to your session username or nothing.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
@@ -109,15 +110,16 @@
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
     accept_strs = False,
-    keep_all_events = False
+    keep_all_events = False,
+    contact_info = None
 )
 ```
 
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
@@ -189,15 +191,15 @@
 )
 ```
 
 If you set `daemon_thread` to `True` when creating the object, the background thread will terminate when your process ends.
 
 # Cloud requests
 
-Cloud requests are based on cloud sockets and allow you to have your project send requests to your server which it automatically responds to.
+Cloud requests are based on cloud sockets and allow you to have your project send requests to your server which it automatically responds to. You'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
 
 ## Creating a cloud requests handler
 
 To use cloud requests, you first need to create a [cloud socket](#cloud-sockets) to your project and then a cloud requests handler which uses it to communicate to your Scratch project.
 
 ```python
 cloud_requests = scratchcommunication.RequestHandler(
@@ -247,14 +249,28 @@
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
 
 ```python
 cloud_requests.stop()
 ```
 
+## Encrypted data transmition
+
+See [Cloud Socket Security](#cloud-socket-security) for this.
+
+## Client side
+
+If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
+
+You'll always first need to connect on your client side for your messages to work. This is done using the "[cloud socket] connect securely" or "[cloud socket] connect insecurely" blocks. 
+
+When you are connected, you can use the block "[cloud requests] initiate new request (%s)" to initiate a new request with its name. The name must not contain spaces. When you have initiated a new request, you can add arguments to the request by using the "[cloud requests] add argument (%s)" block. When you are done creating the request, you can use the block "[cloud requests] send iniated request" to send it and wait for the response.
+
+The received data will be in the variable "[cloud] reception". You can change the timeout using the "# TIMEOUT" variable (If you don't need a timeout, just let it stay). You can also change the packet size using the "# PACKET SIZE" variable, but I would advise against this if you are not using turbowarp.
+
 # Cloud sockets
 
 Cloud sockets (inspired by sockets) are connections from a scratch project to a python program where both sides can send data to one another and there is even the possibility to add security to the connection using RSA.
 
 Warning: Cloud sockets are low level. They allow you to do more but are more difficult to use. You shouldn't use them directly. You might want to use them in [cloud requests](#cloud-requests) instead.
 
 ## Creating a cloud socket
@@ -304,20 +320,30 @@
 ```python
 msg = client.recv()
 client.send("Hello!")
 ```
 
 **Your messages will be public and easy to fake in both direction unless you activate [security](#cloud-socket-security).**
 
-In order to stop the cloud socket from running anymore you can you `scratchcommunication.cloud_socket.CloudSocket.stop`
+In order to stop the cloud socket from running anymore you can use `scratchcommunication.cloud_socket.CloudSocket.stop`
 
 ```python
 cloud_socket.stop()
 ```
 
+## Client side
+
+If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud socket to work.
+
+You'll always first need to connect on your client side for your messages to work. This is done using the "[cloud socket] connect securely" or "[cloud socket] connect insecurely" blocks. 
+
+Afterwards, you can use the "[cloud socket] send (%s)" block and the "[cloud socket] recv" block. 
+
+The received data will be in the variable "[cloud] reception". You can change the timeout using the "# TIMEOUT" variable (If you don't need a timeout, just let it stay). You can also change the packet size using the "# PACKET SIZE" variable, but I would advise against this if you are not using turbowarp.
+
 ## Cloud Socket Security
 
 You might want to be able to send private data that only the designated recipient can read, but that is impossible unless you use asymmetric encryption or something similar. Fortunately for you, the hard work has already been done.
 
 You will need to generate RSA keys for this. In order to do that, you can just use `scratchcommunication.security.RSAKeys.create_new_keys`.
 
 ```python
```

### Comparing `scratchcommunication-2.3.2/scratchcommunication/cloud.py` & `scratchcommunication-2.4.1/scratchcommunication/cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,41 @@
-from typing import Literal, Union, Any
+from typing import Literal, Union, Any, Protocol
+from collections.abc import Callable
 from .exceptions import QuickAccessDisabledError, NotSupported, ErrorInEventHandler, StopException, EventExpiredError
 import json, time, requests, warnings, traceback, secrets, sys
 from websocket import WebSocket
 from func_timeout import StoppableThread
 
 NoneType = type(None)
 CloudConnection = None
 
+class EventDispatcher(Protocol):
+    def __call__(self, data : dict, **entries) -> None:
+        pass
+
 class Event:
     _id : int = None
     value : Union[float, int, bool] = None
     var : str = None
     name : str = None
     project : CloudConnection = None
+    type : str = None
     def __init__(self, _type: Literal["set", "delete", "connect", "create"], **entries):
         entries["type"] = _type
         self.__dict__.update(entries)
         self._data = None
         self.project = getattr(self, "project")
         self._id = secrets.randbits(16)
         
 
     @property
     def data(self):
-        if not hasattr(self, "var"):
+        if not self.project.supports_cloud_logs:
+            raise NotSupported("Cloud connection does not support cloud logs.")
+        if self.type != "set":
             raise NotSupported("No setting")
         if not self._data:
             try:
                 self._data = list(
                     filter(
                         lambda x: x["value"] == self.value,
                         self.project.get_cloud_logs(
@@ -70,28 +78,30 @@
     accept_strs : bool
     wait_until : Union[float, int]
     receive_from_websocket : bool
     data_reception : Any
     event_order : dict[Union[float, int, bool], dict[Event, int]]
     processed_events : list[Event]
     keep_all_events : bool
+    supports_cloud_logs : bool
     def __init__(
         self,
         *,
         project_id : int,
-        session = None,
+        session : Any = None,
         username : str = None,
         quickaccess : bool = False,
         reconnect : bool = True,
         receive_from_websocket : bool = True,
         warning_type : type[Warning] = ErrorInEventHandler,
         daemon_thread : bool = False,
         connect : bool = True,
         keep_all_events : bool = False
     ):
+        self.supports_cloud_logs = True
         self.keep_all_events = keep_all_events
         self.event_order = {}
         self.processed_events = []
         self.thread_running = True
         self.warning_type = warning_type
         self.project_id = project_id
         self.session = session
@@ -408,55 +418,69 @@
             except Exception:
                 warnings.warn(
                     f"There was an exception while trying to process an event: {traceback.format_exc()}",
                     self.warning_type
                 )
         return amount
 
-    def on(self, event : Literal["set", "delete", "connect", "create", "any"]):
+    def on(self, event : Literal["set", "delete", "connect", "create", "any"]) -> Callable[[Callable[[Event], None]], EventDispatcher]:
         """
         Register a new event.
         """
 
         def wrapper(func):
             if event in self.events:
                 eventlist = self.events[event]
             else:
                 eventlist = self.events[event] = []
             eventlist.append(func)
+            def dispatcher(data : dict = None, **entries):
+                return self.emit_event(event, **data, **entries)
+            return dispatcher
 
         return wrapper
 
 
 class TwCloudConnection(CloudConnection):
+    """
+    Connect to a non scratch cloud server and set cloud variables.
+    """
+    contact_info : str
+    user_agent : str
     def __init__(
         self, 
         *, 
         project_id : str, 
         username : str = "player1000", 
+        session : Any = None, 
         quickaccess : bool = False, 
         reconnect : bool = True, 
         receive_from_websocket : bool = True, 
         warning_type : type[Warning] = ErrorInEventHandler,
         daemon_thread : bool = False, 
         cloud_host : str = "wss://clouddata.turbowarp.org/", 
         accept_strs : bool = False,
-        keep_all_events : bool = False
+        keep_all_events : bool = False,
+        contact_info : str = None
     ):
         super().__init__(
             project_id=project_id, 
             username=username,
+            session=session,
             quickaccess=quickaccess,
             reconnect=reconnect,
             receive_from_websocket=receive_from_websocket,
             warning_type=warning_type,
             daemon_thread=daemon_thread,
             connect=False,
             keep_all_events=keep_all_events
         )
+        self.supports_cloud_logs = False
+        self.contact_info = contact_info or ("@"+session.username if session else "Anonymous")
+        self.user_agent = f"scratchcommunication - {self.contact_info}"
         self.cloud_host = cloud_host
         self.accept_strs = accept_strs
         self._connect()
         if not self.receive_from_websocket:
             while True:
                 try:
                     self.receive_new_data()
@@ -467,15 +491,15 @@
         self.data_reception.start()
 
     def _connect(self, *, cloud_host = None, retry : int = 10):
         try:
             if cloud_host is not None:
                 self.cloud_host = cloud_host
             self.websocket = WebSocket()
-            self.websocket.connect(self.cloud_host, enable_multithread=True, timeout=5)
+            self.websocket.connect(self.cloud_host, enable_multithread=True, timeout=5, header={"user-agent": self.user_agent})
             self.handshake()
             self.emit_event("connect")
         except Exception as e:
             if retry == 1:
                 raise ConnectionError(
                     f"There was an error while connecting to the cloud server."
                 ) from e
```

### Comparing `scratchcommunication-2.3.2/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.4.1/scratchcommunication/cloud_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
     def listen(self):
         """
         Start the cloud socket.
         """
         @self.cloud.on("set")
         def on_packet(event):
             try:
+                assert event.type == "set"
                 assert event.name == "FROM_CLIENT"
                 salt = 0
                 value = event.value.replace("-", "")
                 msg_data = value.split(".", 1)[0]
                 msg_type = int(value[0])
                 
                 # Key fragment
```

### Comparing `scratchcommunication-2.3.2/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.4.1/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.3.2/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.4.1/scratchcommunication/cloudrequests/requests.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.3.2/scratchcommunication/security.py` & `scratchcommunication-2.4.1/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.3.2/scratchcommunication/session.py` & `scratchcommunication-2.4.1/scratchcommunication/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         return cloud.CloudConnection(project_id=project_id, session=self, **kwargs)
     
     def create_turbowarp_cloudconnection(self, project_id : int, *, username = None, **kwargs) -> cloud.TwCloudConnection:
         '''
         Create a cloud connection to a turbowarp project.
         '''
         username = username or self.username
-        return cloud.TwCloudConnection(project_id=project_id, username=username, **kwargs)
+        return cloud.TwCloudConnection(project_id=project_id, username=username, session=self, **kwargs)
     
     def create_tw_cloudconnection(self, *args, **kwargs):
         '''
         Same as create_turbowarp_cloudconnection
         '''
         return self.create_turbowarp_cloudconnection(*args, **kwargs)
```

### Comparing `scratchcommunication-2.3.2/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.4.1/scratchcommunication.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.3.2
+Version: 2.4.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -117,15 +117,16 @@
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
     accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
-    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
+    keep_all_events = False, # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
+    contact_info = None # (Optional) Allows you to give turbowarp your contact info. If you don't add any it defaults to your session username or nothing.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
@@ -133,15 +134,16 @@
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
     accept_strs = False,
-    keep_all_events = False
+    keep_all_events = False,
+    contact_info = None
 )
 ```
 
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
@@ -213,15 +215,15 @@
 )
 ```
 
 If you set `daemon_thread` to `True` when creating the object, the background thread will terminate when your process ends.
 
 # Cloud requests
 
-Cloud requests are based on cloud sockets and allow you to have your project send requests to your server which it automatically responds to.
+Cloud requests are based on cloud sockets and allow you to have your project send requests to your server which it automatically responds to. You'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
 
 ## Creating a cloud requests handler
 
 To use cloud requests, you first need to create a [cloud socket](#cloud-sockets) to your project and then a cloud requests handler which uses it to communicate to your Scratch project.
 
 ```python
 cloud_requests = scratchcommunication.RequestHandler(
@@ -271,14 +273,28 @@
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
 
 ```python
 cloud_requests.stop()
 ```
 
+## Encrypted data transmition
+
+See [Cloud Socket Security](#cloud-socket-security) for this.
+
+## Client side
+
+If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
+
+You'll always first need to connect on your client side for your messages to work. This is done using the "[cloud socket] connect securely" or "[cloud socket] connect insecurely" blocks. 
+
+When you are connected, you can use the block "[cloud requests] initiate new request (%s)" to initiate a new request with its name. The name must not contain spaces. When you have initiated a new request, you can add arguments to the request by using the "[cloud requests] add argument (%s)" block. When you are done creating the request, you can use the block "[cloud requests] send iniated request" to send it and wait for the response.
+
+The received data will be in the variable "[cloud] reception". You can change the timeout using the "# TIMEOUT" variable (If you don't need a timeout, just let it stay). You can also change the packet size using the "# PACKET SIZE" variable, but I would advise against this if you are not using turbowarp.
+
 # Cloud sockets
 
 Cloud sockets (inspired by sockets) are connections from a scratch project to a python program where both sides can send data to one another and there is even the possibility to add security to the connection using RSA.
 
 Warning: Cloud sockets are low level. They allow you to do more but are more difficult to use. You shouldn't use them directly. You might want to use them in [cloud requests](#cloud-requests) instead.
 
 ## Creating a cloud socket
@@ -328,20 +344,30 @@
 ```python
 msg = client.recv()
 client.send("Hello!")
 ```
 
 **Your messages will be public and easy to fake in both direction unless you activate [security](#cloud-socket-security).**
 
-In order to stop the cloud socket from running anymore you can you `scratchcommunication.cloud_socket.CloudSocket.stop`
+In order to stop the cloud socket from running anymore you can use `scratchcommunication.cloud_socket.CloudSocket.stop`
 
 ```python
 cloud_socket.stop()
 ```
 
+## Client side
+
+If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud socket to work.
+
+You'll always first need to connect on your client side for your messages to work. This is done using the "[cloud socket] connect securely" or "[cloud socket] connect insecurely" blocks. 
+
+Afterwards, you can use the "[cloud socket] send (%s)" block and the "[cloud socket] recv" block. 
+
+The received data will be in the variable "[cloud] reception". You can change the timeout using the "# TIMEOUT" variable (If you don't need a timeout, just let it stay). You can also change the packet size using the "# PACKET SIZE" variable, but I would advise against this if you are not using turbowarp.
+
 ## Cloud Socket Security
 
 You might want to be able to send private data that only the designated recipient can read, but that is impossible unless you use asymmetric encryption or something similar. Fortunately for you, the hard work has already been done.
 
 You will need to generate RSA keys for this. In order to do that, you can just use `scratchcommunication.security.RSAKeys.create_new_keys`.
 
 ```python
```

### Comparing `scratchcommunication-2.3.2/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.4.1/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.3.2/setup.py` & `scratchcommunication-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scratchcommunication',
-    version='2.3.2',
+    version='2.4.1',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/scratchcommunication',
     packages=find_packages(exclude=[]),
```

### Comparing `scratchcommunication-2.3.2/tests/test1.py` & `scratchcommunication-2.4.1/tests/test1.py`

 * *Files identical despite different names*

