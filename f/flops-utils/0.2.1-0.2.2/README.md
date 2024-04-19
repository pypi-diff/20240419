# Comparing `tmp/flops_utils-0.2.1.tar.gz` & `tmp/flops_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.2.1.tar", max compression
+gzip compressed data, was "flops_utils-0.2.2.tar", max compression
```

## Comparing `flops_utils-0.2.1.tar` & `flops_utils-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.2.1/README.md
--rw-r--r--   0        0        0     1432 2024-04-19 13:37:07.439866 flops_utils-0.2.1/flops_utils/logging.py
--rw-r--r--   0        0        0     1387 2024-04-19 14:34:28.295860 flops_utils-0.2.1/flops_utils/notifications.py
--rw-r--r--   0        0        0      532 2024-04-19 14:34:47.963860 flops_utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.2.2/README.md
+-rw-r--r--   0        0        0     1355 2024-04-19 14:45:40.771859 flops_utils-0.2.2/flops_utils/logging.py
+-rw-r--r--   0        0        0     1387 2024-04-19 14:34:28.295860 flops_utils-0.2.2/flops_utils/notifications.py
+-rw-r--r--   0        0        0      532 2024-04-19 14:45:51.459859 flops_utils-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.2/PKG-INFO
```

### Comparing `flops_utils-0.2.1/flops_utils/logging.py` & `flops_utils-0.2.2/flops_utils/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,16 @@
     light_blue = "\x1b[38;5;45m"
     reset = "\x1b[0m"
 
     def __init__(self, fmt):
         super().__init__()
         self.fmt = fmt
         self.FORMATS = {
-            # logging.DEBUG: self.grey + self.fmt + self.reset,
-            # logging.INFO: self.light_blue + self.fmt + self.reset,
-            logging.DEBUG: self.fmt,
-            logging.INFO: self.fmt,
+            logging.DEBUG: self.grey + self.fmt + self.reset,
+            logging.INFO: self.light_blue + self.fmt + self.reset,
             logging.WARNING: self.yellow + self.fmt + self.reset,
             logging.ERROR: self.red + self.fmt + self.reset,
             logging.CRITICAL: self.bold_red + self.fmt + self.reset,
         }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
```

### Comparing `flops_utils-0.2.1/flops_utils/notifications.py` & `flops_utils-0.2.2/flops_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.2.1/pyproject.toml` & `flops_utils-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flops_utils"
-version = "0.2.1"
+version = "0.2.2"
 description = "A library containing commong utilities for FLOps"
 authors = ["Alexander Malyuk <malyuk.alexander1999@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 paho-mqtt = "2.0"
```

