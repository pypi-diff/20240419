# Comparing `tmp/anedya_dev_sdk-0.1.5.tar.gz` & `tmp/anedya_dev_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anedya_dev_sdk-0.1.5.tar", last modified: Thu Apr 18 10:31:22 2024, max compression
+gzip compressed data, was "anedya_dev_sdk-0.1.6.tar", last modified: Fri Apr 19 11:59:23 2024, max compression
```

## Comparing `anedya_dev_sdk-0.1.5.tar` & `anedya_dev_sdk-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 10:31:22.628436 anedya_dev_sdk-0.1.5/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya_dev_sdk-0.1.5/LICENSE
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya_dev_sdk-0.1.5/MANIFEST.in
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-18 10:31:22.628436 anedya_dev_sdk-0.1.5/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1261 2024-04-09 11:23:38.000000 anedya_dev_sdk-0.1.5/README.md
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-18 10:31:22.628436 anedya_dev_sdk-0.1.5/setup.cfg
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya_dev_sdk-0.1.5/setup.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 10:31:22.624436 anedya_dev_sdk-0.1.5/src/
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 10:31:22.628436 anedya_dev_sdk-0.1.5/src/anedya/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-04-18 07:34:23.000000 anedya_dev_sdk-0.1.5/src/anedya/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4237 2024-04-18 10:16:51.000000 anedya_dev_sdk-0.1.5/src/anedya/anedya.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 10:31:22.628436 anedya_dev_sdk-0.1.5/src/anedya/client/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya_dev_sdk-0.1.5/src/anedya/client/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3435 2024-04-18 07:09:53.000000 anedya_dev_sdk-0.1.5/src/anedya/client/bindDevice.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1161 2024-04-18 10:15:46.000000 anedya_dev_sdk-0.1.5/src/anedya/client/callbacks.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya_dev_sdk-0.1.5/src/anedya/client/certs.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2244 2024-04-18 10:28:59.000000 anedya_dev_sdk-0.1.5/src/anedya/client/mqttHandlers.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3417 2024-04-18 07:17:54.000000 anedya_dev_sdk-0.1.5/src/anedya/client/submitData.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2975 2024-04-18 07:12:59.000000 anedya_dev_sdk-0.1.5/src/anedya/client/submitLogs.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3167 2024-04-18 07:17:21.000000 anedya_dev_sdk-0.1.5/src/anedya/client/timeSync.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4524 2024-04-18 10:21:18.000000 anedya_dev_sdk-0.1.5/src/anedya/config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya_dev_sdk-0.1.5/src/anedya/errors.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3383 2024-04-18 07:24:16.000000 anedya_dev_sdk-0.1.5/src/anedya/models.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya_dev_sdk-0.1.5/src/anedya/transaction.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 10:31:22.628436 anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-18 10:31:22.000000 anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      678 2024-04-18 10:31:22.000000 anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-18 10:31:22.000000 anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-18 10:31:22.000000 anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/requires.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-18 10:31:22.000000 anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 10:31:22.628436 anedya_dev_sdk-0.1.5/tests/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.5/tests/test_config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.5/tests/test_core.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya_dev_sdk-0.1.6/LICENSE
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya_dev_sdk-0.1.6/MANIFEST.in
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1261 2024-04-09 11:23:38.000000 anedya_dev_sdk-0.1.6/README.md
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/setup.cfg
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya_dev_sdk-0.1.6/setup.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.410248 anedya_dev_sdk-0.1.6/src/
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.410248 anedya_dev_sdk-0.1.6/src/anedya/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-04-18 07:34:23.000000 anedya_dev_sdk-0.1.6/src/anedya/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4298 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/anedya.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/src/anedya/client/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya_dev_sdk-0.1.6/src/anedya/client/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3435 2024-04-18 07:09:53.000000 anedya_dev_sdk-0.1.6/src/anedya/client/bindDevice.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1165 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/client/callbacks.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya_dev_sdk-0.1.6/src/anedya/client/certs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     5390 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/client/commandsUpdate.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2244 2024-04-18 10:28:59.000000 anedya_dev_sdk-0.1.6/src/anedya/client/mqttHandlers.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3417 2024-04-18 07:17:54.000000 anedya_dev_sdk-0.1.6/src/anedya/client/submitData.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2973 2024-04-19 11:55:17.000000 anedya_dev_sdk-0.1.6/src/anedya/client/submitLogs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3167 2024-04-18 07:17:21.000000 anedya_dev_sdk-0.1.6/src/anedya/client/timeSync.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4524 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1710 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/errors.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3449 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/models.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya_dev_sdk-0.1.6/src/anedya/transaction.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      714 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/requires.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/tests/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.6/tests/test_config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.6/tests/test_core.py
```

### Comparing `anedya_dev_sdk-0.1.5/LICENSE` & `anedya_dev_sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/PKG-INFO` & `anedya_dev_sdk-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
-Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
+Home-page: https://github.com/anedyaio/anedya-dev-sdk-python
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
-Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
-Project-URL: Source, https://github.com/anedyaio/anedya-dev-sdk-pyhton
+Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-python
+Project-URL: Source, https://github.com/anedyaio/anedya-dev-sdk-python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anedya_dev_sdk-0.1.5/README.md` & `anedya_dev_sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/setup.cfg` & `anedya_dev_sdk-0.1.6/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = anedya-dev-sdk
-version = 0.1.5
-url = https://github.com/anedyaio/anedya-dev-sdk-pyhton
+version = 0.1.6
+url = https://github.com/anedyaio/anedya-dev-sdk-python
 author = Anedya Systems
 author_email = support@anedya.io
 description = Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 long_description = file: README.md
 requires_python = ">=3.7"
 dependencies = ["requests","paho-mqtt>=2.0.0"]
 license = Apache License 2.0
@@ -17,16 +17,16 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Libraries :: Python Modules
 project_urls = 
 	Documentation = https://docs.anedya.io
-	Release notes = https://github.com/anedyaio/anedya-dev-sdk-pyhton
-	Source = https://github.com/anedyaio/anedya-dev-sdk-pyhton
+	Release notes = https://github.com/anedyaio/anedya-dev-sdk-python
+	Source = https://github.com/anedyaio/anedya-dev-sdk-python
 
 [bdist_wheel]
 universal = 1
 
 [options]
 install_requires = 
 	requests
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/anedya.py` & `anedya_dev_sdk-0.1.6/src/anedya/anedya.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,10 +100,11 @@
     def disconnect(self):
         self._mqttclient.disconnect()
         return
 
     from .client.bindDevice import bind_device
     from .client.submitData import submit_data
     from .client.submitLogs import submit_logs
+    from .client.commandsUpdate import update_command_status
     from .client.timeSync import get_time
     from .client.mqttHandlers import _onconnect_handler, _ondisconnect_handler
     from .client.callbacks import _error_callback, _response_callback, _command_callback
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/client/bindDevice.py` & `anedya_dev_sdk-0.1.6/src/anedya/client/bindDevice.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/client/callbacks.py` & `anedya_dev_sdk-0.1.6/src/anedya/client/callbacks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from ..models import CommandMessage
+from ..models import CommandDetails
 
 
 def _response_callback(self, client, userdata, message):
     # This callback is called when a message is received on response topic.
     payload_data = json.loads(message.payload)
     # Find the transaction and mark that transaction as complete.
     # Fetch the ID
@@ -21,14 +21,14 @@
     return
 
 
 def _command_callback(self, client, userdata, message):
     payload_data = json.loads(message.payload)
     # This callback is called when a command is received.
     # Convert the received command to python object and call client callback
-    cmd = CommandMessage(payload_data)
     # Call the client callback
     try:
+        cmd = CommandDetails(payload_data)
         self.on_command(cmd)
     except Exception:
         pass
     return
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/client/certs.py` & `anedya_dev_sdk-0.1.6/src/anedya/client/certs.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/client/mqttHandlers.py` & `anedya_dev_sdk-0.1.6/src/anedya/client/mqttHandlers.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/client/submitData.py` & `anedya_dev_sdk-0.1.6/src/anedya/client/submitData.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/client/submitLogs.py` & `anedya_dev_sdk-0.1.6/src/anedya/client/submitLogs.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         AnedyaTxFailure: Method can raise this method if the transaction fails.
     """
     if self._config is None:
         raise AnedyaInvalidConfig('Configuration not provided')
     if self._config.connection_mode == ConnectionMode.HTTP:
         return _submit_log_http(self, logs=logs, timeout=timeout)
     elif self._config.connection_mode == ConnectionMode.MQTT:
-        return _submit_data_mqtt(self, logs=logs, timeout=timeout)
+        return _submit_log_mqtt(self, logs=logs, timeout=timeout)
     else:
         raise AnedyaInvalidConfig('Invalid connection mode')
 
 
 def _submit_log_http(self, logs: LogsCache, timeout: float | None = None):
     if self._config._testmode:
         url = "https://device.stageapi.anedya.io/v1/logs/submitLogs"
@@ -38,15 +38,15 @@
         payload = json.loads(jsonResponse)
         if payload['success'] is not True:
             raise AnedyaTxFailure(payload['error'], payload['errCode'])
     except ValueError:
         raise AnedyaTxFailure(message="Invalid JSON response")
 
 
-def _submit_data_mqtt(self, data: LogsCache, timeout: float | None = None):
+def _submit_log_mqtt(self, data: LogsCache, timeout: float | None = None):
     # Create and register a transaction
     tr = self._transactions.create_transaction()
     # Encode the payload
     d = SubmitLogsMQTTReq(tr.get_id(), data)
     payload = d.encodeJSON()
     # Publish the message
     self._mqttclient.publish(topic="$anedya/device/" + str(self._config._deviceID) + "/submitLogs/json",
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/client/timeSync.py` & `anedya_dev_sdk-0.1.6/src/anedya/client/timeSync.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/config.py` & `anedya_dev_sdk-0.1.6/src/anedya/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 import uuid
 from .errors import AnedyaInvalidConfig
-from .models import CommandMessage
+from .models import CommandDetails
 from typing import Callable
 
 
 class ConnectionMode(Enum):
     HTTP = "HTTP"
     MQTT = "MQTT"
 
@@ -118,15 +118,15 @@
             AnedyaInvalidConfig: Raised when the callback is not a valid function
         """
         if not callable(callback):
             raise AnedyaInvalidConfig(
                 "Callback function needs to be a valid function")
         self.on_disconnect = callback
 
-    def set_on_command(self, callback: Callable[[CommandMessage], None]):
+    def set_on_command(self, callback: Callable[[CommandDetails], None]):
         """
         Set a callback function that will be called when a command is received.
 
         Args:
             callback (function): A callback function that will be called when a command is received. The callback function should not block.
 
         Raises:
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/errors.py` & `anedya_dev_sdk-0.1.6/src/anedya/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,7 +58,16 @@
     """
     Raised when a transaction fails
     """
     def __init__(self, message, code):
         self.message = message
         self.code = code
         super().__init__(self.message)
+
+
+class AnedyaInvalidType(Exception):
+    """
+    Raised when an invalid type is passed
+    """
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/models.py` & `anedya_dev_sdk-0.1.6/src/anedya/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,28 +98,30 @@
         self.logs = []
 
     def encodeJSON(self):
         data = json.dumps(self, cls=AnedyaEncoder)
         return data
 
 
-class CommandMessage:
+class CommandDetails:
     def __init__(self, commandMsg: dict):
         self.command = commandMsg["command"]
-        self.id = uuid.UUID(commandMsg["id"])
+        self.id = uuid.UUID(commandMsg["commandId"])
         if type == "string":
             self.data = commandMsg["data"]
         elif type == "binary":
             base64_bytes = commandMsg["data"].encode("ascii")
             data_bytes = base64.b64decode(base64_bytes)
             self.data = data_bytes
         else:
             raise Exception("Invalid datatype")
-        self.type = commandMsg["type"]
+        self.type = commandMsg["datatype"]
         self.exp = datetime.datetime.fromtimestamp(commandMsg["exp"] / 1000)
+        self.status = None
+        self.updated = None
 
 
 class AnedyaEncoder(json.JSONEncoder):
     def default(self, obj):
         if hasattr(obj, 'toJSON'):
             return obj.toJSON()
         else:
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya/transaction.py` & `anedya_dev_sdk-0.1.6/src/anedya/transaction.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/PKG-INFO` & `anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
-Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
+Home-page: https://github.com/anedyaio/anedya-dev-sdk-python
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
-Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
-Project-URL: Source, https://github.com/anedyaio/anedya-dev-sdk-pyhton
+Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-python
+Project-URL: Source, https://github.com/anedyaio/anedya-dev-sdk-python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anedya_dev_sdk-0.1.5/src/anedya_dev_sdk.egg-info/SOURCES.txt` & `anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/anedya/errors.py
 src/anedya/models.py
 src/anedya/transaction.py
 src/anedya/client/__init__.py
 src/anedya/client/bindDevice.py
 src/anedya/client/callbacks.py
 src/anedya/client/certs.py
+src/anedya/client/commandsUpdate.py
 src/anedya/client/mqttHandlers.py
 src/anedya/client/submitData.py
 src/anedya/client/submitLogs.py
 src/anedya/client/timeSync.py
 src/anedya_dev_sdk.egg-info/PKG-INFO
 src/anedya_dev_sdk.egg-info/SOURCES.txt
 src/anedya_dev_sdk.egg-info/dependency_links.txt
```

### Comparing `anedya_dev_sdk-0.1.5/tests/test_config.py` & `anedya_dev_sdk-0.1.6/tests/test_config.py`

 * *Files identical despite different names*

