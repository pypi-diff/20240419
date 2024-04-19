# Comparing `tmp/flops_utils-0.2.0.tar.gz` & `tmp/flops_utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.2.0.tar", max compression
+gzip compressed data, was "flops_utils-0.2.1.tar", max compression
```

## Comparing `flops_utils-0.2.0.tar` & `flops_utils-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.2.0/README.md
--rw-r--r--   0        0        0     1432 2024-04-19 13:37:07.439866 flops_utils-0.2.0/flops_utils/logging.py
--rw-r--r--   0        0        0     1384 2024-04-19 14:26:08.787861 flops_utils-0.2.0/flops_utils/notifications.py
--rw-r--r--   0        0        0      532 2024-04-19 14:26:53.475861 flops_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.2.1/README.md
+-rw-r--r--   0        0        0     1432 2024-04-19 13:37:07.439866 flops_utils-0.2.1/flops_utils/logging.py
+-rw-r--r--   0        0        0     1387 2024-04-19 14:34:28.295860 flops_utils-0.2.1/flops_utils/notifications.py
+-rw-r--r--   0        0        0      532 2024-04-19 14:34:47.963860 flops_utils-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.1/PKG-INFO
```

### Comparing `flops_utils-0.2.0/flops_utils/logging.py` & `flops_utils-0.2.1/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.2.0/flops_utils/notifications.py` & `flops_utils-0.2.1/flops_utils/notifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import socket
 import sys
 
 import paho.mqtt.client as paho_mqtt
-from flops_utils.logg import logger
+from flops_utils.logging import logger
 
 
 def notify_flops_ui(flops_ui_ip: str, msg: str) -> None:
     logger.debug(f"Sending message to FLOps UI: {msg}")
     client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     client_socket.connect((flops_ui_ip, 2727))
     client_socket.send(msg.encode())
```

### Comparing `flops_utils-0.2.0/pyproject.toml` & `flops_utils-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flops_utils"
-version = "0.2.0"
+version = "0.2.1"
 description = "A library containing commong utilities for FLOps"
 authors = ["Alexander Malyuk <malyuk.alexander1999@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 paho-mqtt = "2.0"
```

