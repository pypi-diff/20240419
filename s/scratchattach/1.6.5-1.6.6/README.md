# Comparing `tmp/scratchattach-1.6.5.tar.gz` & `tmp/scratchattach-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.5.tar", last modified: Tue Apr 16 19:59:37 2024, max compression
+gzip compressed data, was "scratchattach-1.6.6.tar", last modified: Fri Apr 19 13:11:25 2024, max compression
```

## Comparing `scratchattach-1.6.5.tar` & `scratchattach-1.6.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 19:59:37.735682 scratchattach-1.6.5/
--rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.5/LICENSE
--rw-rw-rw-   0        0        0     4042 2024-04-16 19:59:37.735682 scratchattach-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 19:59:37.724176 scratchattach-1.6.5/scratchattach/
--rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.5/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    20920 2024-04-16 19:58:40.000000 scratchattach-1.6.5/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    24874 2024-04-16 18:08:07.000000 scratchattach-1.6.5/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.5/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.5/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.5/scratchattach/forum.py
--rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.5/scratchattach/project.py
--rw-rw-rw-   0        0        0    22000 2023-09-30 18:44:30.000000 scratchattach-1.6.5/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.5/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.5/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-04-16 19:59:37.735682 scratchattach-1.6.5/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4042 2024-04-16 19:59:37.000000 scratchattach-1.6.5/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-04-16 19:59:37.000000 scratchattach-1.6.5/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 19:59:37.000000 scratchattach-1.6.5/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-16 19:59:37.000000 scratchattach-1.6.5/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 19:59:37.000000 scratchattach-1.6.5/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 19:59:37.737184 scratchattach-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-04-16 19:59:22.000000 scratchattach-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:25.965941 scratchattach-1.6.6/
+-rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0     4042 2024-04-19 13:11:25.965941 scratchattach-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:25.948937 scratchattach-1.6.6/scratchattach/
+-rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.6/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    22391 2024-04-19 13:08:19.000000 scratchattach-1.6.6/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    25085 2024-04-19 13:04:10.000000 scratchattach-1.6.6/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.6/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.6/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.6/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.6/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.6/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.6/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.6/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:25.964941 scratchattach-1.6.6/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4042 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 13:11:25.965941 scratchattach-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2024-04-19 12:33:08.000000 scratchattach-1.6.6/setup.py
```

### Comparing `scratchattach-1.6.5/LICENSE` & `scratchattach-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/PKG-INFO` & `scratchattach-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.5
+Version: 1.6.6
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.5/README.md` & `scratchattach-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach/__init__.py` & `scratchattach-1.6.6/scratchattach/__init__.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach/cloud.py` & `scratchattach-1.6.6/scratchattach/cloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,29 +9,34 @@
 import warnings
 
 class _CloudMixin:
     """
     Base class for a connection to a cloud variable server.
     """
 
-    def __init__(self, *, project_id, username="scratchattach", session_id=None, cloud_host=None, _allow_non_numeric=False, _ws_timeout=None):
+    def __init__(self, *, project_id, username="scratchattach", session_id=None, cloud_host=None, purpose="", contact="", _allow_non_numeric=False, _ws_timeout=None):
         self._session_id = session_id
         self._username = username
         try:
             self.project_id = int(project_id)
         except ValueError: #non-numeric project id (possible on turbowarp's cloud server)
             self.project_id = str(project_id)
         self._ratelimited_until = 0 #deals with the 0.1 second rate limit for cloud variable sets
         self._connect_timestamp = 0 #timestamp of when the cloud connection was opened
         self._ws_timeout = _ws_timeout
+
+        # user agent information (for connecting to TurboWarp's cloud servers)
+        self.user_agent_purpose = purpose
+        self.user_agent_contact = contact
+
         self.websocket = websocket.WebSocket()
         self._connect(cloud_host=cloud_host)
         self._handshake()
         self.cloud_host = cloud_host
-        self.allow_non_numeric = _allow_non_numeric #TurboWarp only. If this is true, turbowarp cloud variables can be set to non-numeric values (if) the cloud_host wss allows it)
+        self.allow_non_numeric = _allow_non_numeric #TurboWarp only. If this is true, turbowarp cloud variables can be set to non-numeric values (if the cloud_host wss allows it)
 
     def _send_packet(self, packet):
         self.websocket.send(json.dumps(packet) + "\n")
 
     def disconnect(self):
         self.websocket.close()
 
@@ -149,24 +154,27 @@
     :.websocket: The websocket connection (WebSocket object from the websocket-client library)
 
     :.cloud_host: The websocket URL of the cloud variable server
     
     :.allow_non_numeric: Whether the cloud variables can be set to non-numeric values
     """
 
-    def _connect(self, *, cloud_host=None, timeout=None):
+    def _connect(self, *, cloud_host=None):
         try:
             if cloud_host is None:
                 cloud_host = "wss://clouddata.turbowarp.org/"
                 self.cloud_host = cloud_host
+            purpose_string = ""
+            if self.user_agent_purpose != "" or self.user_agent_contact != "":
+                purpose_string = f" (Purpose:{self.user_agent_purpose}; Contact:{self.user_agent_contact})"
             self.websocket.connect(
                 cloud_host,
                 enable_multithread=True,
                 timeout = self._ws_timeout,
-                header = {"User-Agent":"scratchattach/1.6.4" if timeout is None else "scratchattach/1.6.4 short-term connection (for get_cloud method)"}
+                header = {"User-Agent":f"scratchattach/1.6.6{purpose_string}" if self._ws_timeout is None else f"scratchattach/1.6.6 (short-term connection){purpose_string}"}
             )
         except Exception:
             raise(exceptions.ConnectionError)
         self._connect_timestamp = time.time()
 
 
     def set_var(self, variable, value):
@@ -319,21 +327,25 @@
         self._events[function.__name__] = function
 
 class TwCloudEvents(CloudEvents):
     """
     Class that calls events on TurboWarp cloud variable updates. Data fetched from Turbowarp cloud websocket.
     """
     def __init__(self, project_id, **entries):
-        cloud_connection = TwCloudConnection(project_id=project_id)
+        self.__dict__.update(entries)
+        if not "purpose" in entries:
+            self.purpose = ""
+        if not "contact" in entries:
+            self.contact = ""
+        cloud_connection = TwCloudConnection(project_id=project_id, purpose=self.purpose, contact=self.contact)
         self.data = []
         self._thread = None
         self.running = False
         self._events = {}
         self.connection = cloud_connection
-        self.__dict__.update(entries)
 
     def _update(self):
         while True:
             try:
                 data = self.connection.websocket.recv().split('\n')
                 result = []
                 for i in data:
@@ -433,63 +445,71 @@
         if response == []:
             return None
         else:
             return response[0]["value"]
     except Exception:
         return None
 
-def get_tw_cloud(project_id):
+def get_tw_cloud(project_id, *, purpose="", contact=""):
     """
     Gets the clouddata of a TurboWarp cloud project.
 
     Warning:
         Do not spam this method, it creates a new connection to the TurboWarp cloud server every time it is called.
 
     Args:
         project_id (str):
-    
+
+    Keyword Arguments:
+        purpose (str): (optional) Provide information about what you're using TurboWarp's cloud server for
+        contact (str): (optional) Provide an email address or another way you can be contacted
+
     Returns:
         dict: The values of the project's cloud variables
     """
 
     try:
-        conn = TwCloudConnection(project_id=project_id, _ws_timeout=1)
+        conn = TwCloudConnection(project_id=project_id, _ws_timeout=1, purpose=purpose, contact=contact)
         data = conn.websocket.recv().split("\n")
         conn.disconnect()
 
         result = []
         for i in data:
             try:
                 result.append(json.loads(i))
             except Exception: pass
         return result
     except websocket._exceptions.WebSocketTimeoutException:
         return []
     except Exception:
         raise exceptions.FetchError
 
-def get_tw_var(project_id, variable):
+def get_tw_var(project_id, variable, *, purpose="", contact=""):
     """
     Gets the value of of a TurboWarp cloud variable.
 
     Warning:
         Do not spam this method, it creates a new connection to the TurboWarp cloud server every time it is called.
 
     Args:
         project_id (str):
         variable (str): The name of the cloud variable (specified without the cloud emoji)
-    
+
+    Keyword Arguments:
+        purpose (str): (optional) Provide information about what you're using TurboWarp's cloud server for
+        contact (str): (optional) Provide an email address or another way you can be contacted
+
     Returns:
         str: The cloud variable's value
     
     If the value can't be fetched, the method returns None.
     """
     try:
         variable = "☁ " + str(variable)
-        result = get_tw_cloud(project_id)
+        result = get_tw_cloud(project_id, purpose=purpose, contact=contact)
         if result == []:
             return None
         else:
             for i in result:
                 if i['name'] == variable:
                     return i['value']
             else:
@@ -514,23 +534,27 @@
         response = json.loads(requests.get(f"https://clouddata.scratch.mit.edu/logs?projectid={project_id}&limit={limit}&offset={offset}").text)
         if filter_by_var_named is None: return response
         else:
             return list(filter(lambda k: k["name"] == "☁ "+filter_by_var_named, response))
     except Exception:
         return []
 
-def connect_tw_cloud(project_id_arg=None, *, project_id=None):
+def connect_tw_cloud(project_id_arg=None, *, project_id=None, purpose="", contact=""):
     """
     Connects to TurboWarp's cloud websocket.
 
     Args:
         project_id (str)
+    
+    Keyword Arguments:
+        purpose (str): (optional) Provide information about what you're using TurboWarp's cloud server for
+        contact (str): (optional) Provide an email address or another way you can be contacted
 
     Returns:
         scratchattach.cloud.TwCloudConnection: An object that represents a connection to TurboWarp's cloud server
     """
     if project_id is None:
         project_id = project_id_arg
     if project_id is None:
         return None
 
-    return TwCloudConnection(project_id = project_id)
+    return TwCloudConnection(project_id = project_id, purpose=purpose, contact=contact)
```

### Comparing `scratchattach-1.6.5/scratchattach/cloud_requests.py` & `scratchattach-1.6.6/scratchattach/cloud_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,14 +552,16 @@
     Framework (inspired by discord.py) that allows TurboWarp cloud variables and Python to communicate. More information: https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests
     """
     def __init__(self,
                  cloud_connection,
                  *,
                  used_cloud_vars=["1", "2", "3", "4", "5", "6", "7", "8", "9"],
                  ignore_exceptions=True,
+                 purpose="",
+                 contact="",
                  _force_reconnect = False, # this argument is no longer used and only exists for backwards compatibility
                  _packet_length=98800):
         print(
             "\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m"
         )
         if _packet_length > 98800:
             warnings.warn(
@@ -568,33 +570,38 @@
         self.used_cloud_vars = used_cloud_vars
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.packet_length = _packet_length
 
+        # user agent data
+        self.purpose = purpose
+        self.contact = contact
+
         self.init_attributes()
 
     def get_requester(self):
         return None
 
     def run(self,
             thread=False,
             data_from_websocket=True,
             no_packet_loss=False,
-            daemon=False):
+            daemon=False
+            ):
         '''
         Starts the request handler.
         
         Args:
             thread: Whether the request handler should be run in a thread.
             data_from_websocket: Whether the websocket should be used to detect requests.
             no_packet_loss: Whether the request handler should reconnect to the cloud websocket before responding to a request, this can help to avoid packet loss.
         '''
         self.force_reconnect = no_packet_loss
-        events = [cloud.TwCloudEvents(self.project_id, update_interval=0)]
+        events = [cloud.TwCloudEvents(self.project_id, update_interval=0, purpose=self.purpose, contact=self.contact)]
         self.cloud_events = events
         if thread:
             thread = Thread(target=self._run, args=[events], daemon=daemon)
             thread.start()
         else:
             self._run(events)
```

### Comparing `scratchattach-1.6.5/scratchattach/encoder.py` & `scratchattach-1.6.6/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach/exceptions.py` & `scratchattach-1.6.6/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach/forum.py` & `scratchattach-1.6.6/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach/project.py` & `scratchattach-1.6.6/scratchattach/project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach/session.py` & `scratchattach-1.6.6/scratchattach/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,16 +358,16 @@
         if project_id is None:
             project_id = project_id_arg
         if project_id is None:
             return None
 
         return cloud.CloudConnection(username = self._username, session_id = self.session_id, project_id = int(project_id))
 
-    def connect_tw_cloud(self, project_id_arg=None, *, project_id=None):
-        return cloud.connect_tw_cloud(project_id_arg, project_id=project_id)
+    def connect_tw_cloud(self, project_id_arg=None, *, project_id=None, purpose="", contact=""):
+        return cloud.connect_tw_cloud(project_id_arg, project_id=project_id, purpose=purpose, contact=contact)
 
     def connect_user(self, username):
         """
         Gets a user.
 
         Args:
             username (str): Username of the requested user
```

### Comparing `scratchattach-1.6.5/scratchattach/studio.py` & `scratchattach-1.6.6/scratchattach/studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach/user.py` & `scratchattach-1.6.6/scratchattach/user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.5/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.6.6/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.5
+Version: 1.6.6
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.5/setup.py` & `scratchattach-1.6.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.6.5'
+VERSION = '1.6.6'
 DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

