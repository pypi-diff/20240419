# Comparing `tmp/scratchcommunication-2.4.1.tar.gz` & `tmp/scratchcommunication-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.4.1.tar", last modified: Fri Apr 19 12:59:09 2024, max compression
+gzip compressed data, was "scratchcommunication-2.4.2.tar", last modified: Fri Apr 19 13:26:01 2024, max compression
```

## Comparing `scratchcommunication-2.4.1.tar` & `scratchcommunication-2.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15014 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17966 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 12:59:09.000000 scratchcommunication-2.4.1/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:59:09.830842 scratchcommunication-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-19 12:59:06.000000 scratchcommunication-2.4.1/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:26:01.715242 scratchcommunication-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-19 13:26:01.715242 scratchcommunication-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:26:01.711242 scratchcommunication-2.4.2/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18148 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:26:01.711242 scratchcommunication-2.4.2/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:26:01.715242 scratchcommunication-2.4.2/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-19 13:26:01.000000 scratchcommunication-2.4.2/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 13:26:01.000000 scratchcommunication-2.4.2/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:26:01.000000 scratchcommunication-2.4.2/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:26:01.000000 scratchcommunication-2.4.2/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 13:26:01.000000 scratchcommunication-2.4.2/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:26:01.715242 scratchcommunication-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:26:01.711242 scratchcommunication-2.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-19 13:25:55.000000 scratchcommunication-2.4.2/tests/test1.py
```

### Comparing `scratchcommunication-2.4.1/LICENSE` & `scratchcommunication-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.1/PKG-INFO` & `scratchcommunication-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.4.1
+Version: 2.4.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -109,44 +109,46 @@
 
 ## Connecting to Turbowarp Cloud Variables
 
 To connect to Turbowarps Cloud Variables you can use the `scratchcommunication.cloud.TwCloudConnection` class
 
 ```python
 tw_cloud = scratchcommunication.TwCloudConnection(
+    contact_info = "Your contact info", # Specify some contact info. Turbowarp will block your connection otherwise.
     project_id = "Your project id here", 
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
     accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
-    keep_all_events = False, # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
-    contact_info = None # (Optional) Allows you to give turbowarp your contact info. If you don't add any it defaults to your session username or nothing.
+    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
+    contact_info = "Your contact info",
     project_id = "Your project id here",
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
     accept_strs = False,
-    keep_all_events = False,
-    contact_info = None
+    keep_all_events = False
 )
 ```
 
+**Warning: You need to add sufficient contact_info for your turbowarp connection or it might not work!**
+
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
 To set or get cloud variables you can use `scratchcommunication.cloud.CloudConnection.set_variable` and `scratchcommunication.cloud.CloudConnection.get_variable`.
 
 ```python
@@ -310,14 +312,15 @@
 )
 ```
 
 You can also use Turbowarp for cloud sockets.
 
 ```python
 cloud_socket = session.create_turbowarp_cloud_socket( # session.create_tw_cloud_socket also works here
+    contact_info = "Your contact info",
     project_id = "Your project id here",
     packet_size = 220, # (Optional) I recommend leaving this value be if you only use Scratch and Turbowarp.
     cloudconnection_kwargs = None, # (Optional) Allows for adding keyword arguments for the Cloud Connection used in the cloud socket. Look at the documentation for Cloud Connection if you do not know which keyword arguments there are
     security = None # (Optional) Allows for a secure connection. Recommended. Look at Cloud Socket Security for more info.
 )
 ```
```

### Comparing `scratchcommunication-2.4.1/README.md` & `scratchcommunication-2.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,44 +85,46 @@
 
 ## Connecting to Turbowarp Cloud Variables
 
 To connect to Turbowarps Cloud Variables you can use the `scratchcommunication.cloud.TwCloudConnection` class
 
 ```python
 tw_cloud = scratchcommunication.TwCloudConnection(
+    contact_info = "Your contact info", # Specify some contact info. Turbowarp will block your connection otherwise.
     project_id = "Your project id here", 
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
     accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
-    keep_all_events = False, # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
-    contact_info = None # (Optional) Allows you to give turbowarp your contact info. If you don't add any it defaults to your session username or nothing.
+    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
+    contact_info = "Your contact info",
     project_id = "Your project id here",
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
     accept_strs = False,
-    keep_all_events = False,
-    contact_info = None
+    keep_all_events = False
 )
 ```
 
+**Warning: You need to add sufficient contact_info for your turbowarp connection or it might not work!**
+
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
 To set or get cloud variables you can use `scratchcommunication.cloud.CloudConnection.set_variable` and `scratchcommunication.cloud.CloudConnection.get_variable`.
 
 ```python
@@ -286,14 +288,15 @@
 )
 ```
 
 You can also use Turbowarp for cloud sockets.
 
 ```python
 cloud_socket = session.create_turbowarp_cloud_socket( # session.create_tw_cloud_socket also works here
+    contact_info = "Your contact info",
     project_id = "Your project id here",
     packet_size = 220, # (Optional) I recommend leaving this value be if you only use Scratch and Turbowarp.
     cloudconnection_kwargs = None, # (Optional) Allows for adding keyword arguments for the Cloud Connection used in the cloud socket. Look at the documentation for Cloud Connection if you do not know which keyword arguments there are
     security = None # (Optional) Allows for a secure connection. Recommended. Look at Cloud Socket Security for more info.
 )
 ```
```

### Comparing `scratchcommunication-2.4.1/scratchcommunication/cloud.py` & `scratchcommunication-2.4.2/scratchcommunication/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,30 +456,31 @@
         reconnect : bool = True, 
         receive_from_websocket : bool = True, 
         warning_type : type[Warning] = ErrorInEventHandler,
         daemon_thread : bool = False, 
         cloud_host : str = "wss://clouddata.turbowarp.org/", 
         accept_strs : bool = False,
         keep_all_events : bool = False,
-        contact_info : str = None
+        contact_info : str
     ):
         super().__init__(
             project_id=project_id, 
             username=username,
             session=session,
             quickaccess=quickaccess,
             reconnect=reconnect,
             receive_from_websocket=receive_from_websocket,
             warning_type=warning_type,
             daemon_thread=daemon_thread,
             connect=False,
             keep_all_events=keep_all_events
         )
         self.supports_cloud_logs = False
-        self.contact_info = contact_info or ("@"+session.username if session else "Anonymous")
+        self.contact_info = contact_info or ((f"@{session.username} on scratch" if session else "Anonymous") if username == "player1000" else f"@{username} on scratch")
+        assert self.contact_info != "Anonymous", "You need to specify your contact_info for the turbowarp cloud."
         self.user_agent = f"scratchcommunication - {self.contact_info}"
         self.cloud_host = cloud_host
         self.accept_strs = accept_strs
         self._connect()
         if not self.receive_from_websocket:
             while True:
                 try:
@@ -491,15 +492,15 @@
         self.data_reception.start()
 
     def _connect(self, *, cloud_host = None, retry : int = 10):
         try:
             if cloud_host is not None:
                 self.cloud_host = cloud_host
             self.websocket = WebSocket()
-            self.websocket.connect(self.cloud_host, enable_multithread=True, timeout=5, header={"user-agent": self.user_agent})
+            self.websocket.connect(self.cloud_host, enable_multithread=True, timeout=5, header={"User-Agent": self.user_agent})
             self.handshake()
             self.emit_event("connect")
         except Exception as e:
             if retry == 1:
                 raise ConnectionError(
                     f"There was an error while connecting to the cloud server."
                 ) from e
```

### Comparing `scratchcommunication-2.4.1/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.4.2/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.1/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.4.2/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.1/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.4.2/scratchcommunication/cloudrequests/requests.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.1/scratchcommunication/security.py` & `scratchcommunication-2.4.2/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.1/scratchcommunication/session.py` & `scratchcommunication-2.4.2/scratchcommunication/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,18 +103,18 @@
 
     def create_cloud_socket(self, project_id : int, *, packet_size : int = 220, cloudconnection_kwargs : dict = None, security : tuple = None, **kwargs):
         '''
         Create a cloud socket to a project.
         '''
         return cloud_socket.CloudSocket(cloud=self.create_cloudconnection(project_id, warning_type=ErrorInCloudSocket, **(cloudconnection_kwargs if cloudconnection_kwargs else {})), packet_size=packet_size, security=security, **kwargs)
 
-    def create_turbowarp_cloud_socket(self, project_id : int, *, packet_size : int = 90000, cloudconnection_kwargs : dict = None, security : tuple = None, **kwargs):
+    def create_turbowarp_cloud_socket(self, contact_info : str, project_id : int, *, packet_size : int = 90000, cloudconnection_kwargs : dict = None, security : tuple = None, **kwargs):
         '''
         Create a cloud socket to a turbowarp project.
         '''
-        return cloud_socket.CloudSocket(cloud=self.create_tw_cloudconnection(project_id, warning_type=ErrorInCloudSocket, **(cloudconnection_kwargs if cloudconnection_kwargs else {})), packet_size=packet_size, security=security, **kwargs)
+        return cloud_socket.CloudSocket(cloud=self.create_tw_cloudconnection(project_id, contact_info=contact_info, warning_type=ErrorInCloudSocket, **(cloudconnection_kwargs if cloudconnection_kwargs else {})), packet_size=packet_size, security=security, **kwargs)
     
     def create_tw_cloud_socket(self, *args, **kwargs):
         '''
         Same as create_turbowarp_cloud_socket
         '''
         return self.create_turbowarp_cloud_socket(*args, **kwargs)
```

### Comparing `scratchcommunication-2.4.1/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.4.2/scratchcommunication.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.4.1
+Version: 2.4.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -109,44 +109,46 @@
 
 ## Connecting to Turbowarp Cloud Variables
 
 To connect to Turbowarps Cloud Variables you can use the `scratchcommunication.cloud.TwCloudConnection` class
 
 ```python
 tw_cloud = scratchcommunication.TwCloudConnection(
+    contact_info = "Your contact info", # Specify some contact info. Turbowarp will block your connection otherwise.
     project_id = "Your project id here", 
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
     accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
-    keep_all_events = False, # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
-    contact_info = None # (Optional) Allows you to give turbowarp your contact info. If you don't add any it defaults to your session username or nothing.
+    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
+    contact_info = "Your contact info",
     project_id = "Your project id here",
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
     accept_strs = False,
-    keep_all_events = False,
-    contact_info = None
+    keep_all_events = False
 )
 ```
 
+**Warning: You need to add sufficient contact_info for your turbowarp connection or it might not work!**
+
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
 To set or get cloud variables you can use `scratchcommunication.cloud.CloudConnection.set_variable` and `scratchcommunication.cloud.CloudConnection.get_variable`.
 
 ```python
@@ -310,14 +312,15 @@
 )
 ```
 
 You can also use Turbowarp for cloud sockets.
 
 ```python
 cloud_socket = session.create_turbowarp_cloud_socket( # session.create_tw_cloud_socket also works here
+    contact_info = "Your contact info",
     project_id = "Your project id here",
     packet_size = 220, # (Optional) I recommend leaving this value be if you only use Scratch and Turbowarp.
     cloudconnection_kwargs = None, # (Optional) Allows for adding keyword arguments for the Cloud Connection used in the cloud socket. Look at the documentation for Cloud Connection if you do not know which keyword arguments there are
     security = None # (Optional) Allows for a secure connection. Recommended. Look at Cloud Socket Security for more info.
 )
 ```
```

### Comparing `scratchcommunication-2.4.1/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.4.2/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.1/setup.py` & `scratchcommunication-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scratchcommunication',
-    version='2.4.1',
+    version='2.4.2',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/scratchcommunication',
     packages=find_packages(exclude=[]),
```

### Comparing `scratchcommunication-2.4.1/tests/test1.py` & `scratchcommunication-2.4.2/tests/test1.py`

 * *Files identical despite different names*

