# Comparing `tmp/flops_utils-0.1.5.tar.gz` & `tmp/flops_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.1.5.tar", max compression
+gzip compressed data, was "flops_utils-0.2.0.tar", max compression
```

## Comparing `flops_utils-0.1.5.tar` & `flops_utils-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.1.5/README.md
--rw-r--r--   0        0        0     1432 2024-04-19 13:35:28.887867 flops_utils-0.1.5/flops_utils/logging.py
--rw-r--r--   0        0        0       42 2024-04-19 13:26:41.911868 flops_utils-0.1.5/flops_utils/testing.py
--rw-r--r--   0        0        0      514 2024-04-19 13:35:40.519867 flops_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 flops_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.2.0/README.md
+-rw-r--r--   0        0        0     1432 2024-04-19 13:37:07.439866 flops_utils-0.2.0/flops_utils/logging.py
+-rw-r--r--   0        0        0     1384 2024-04-19 14:26:08.787861 flops_utils-0.2.0/flops_utils/notifications.py
+-rw-r--r--   0        0        0      532 2024-04-19 14:26:53.475861 flops_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.0/PKG-INFO
```

### Comparing `flops_utils-0.1.5/flops_utils/logging.py` & `flops_utils-0.2.0/flops_utils/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     reset = "\x1b[0m"
 
     def __init__(self, fmt):
         super().__init__()
         self.fmt = fmt
         self.FORMATS = {
             # logging.DEBUG: self.grey + self.fmt + self.reset,
-            logging.INFO: self.light_blue + self.fmt + self.reset,
+            # logging.INFO: self.light_blue + self.fmt + self.reset,
             logging.DEBUG: self.fmt,
-            # logging.INFO: self.fmt,
+            logging.INFO: self.fmt,
             logging.WARNING: self.yellow + self.fmt + self.reset,
             logging.ERROR: self.red + self.fmt + self.reset,
             logging.CRITICAL: self.bold_red + self.fmt + self.reset,
         }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
```

### Comparing `flops_utils-0.1.5/pyproject.toml` & `flops_utils-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "flops_utils"
-version = "0.1.5"
+version = "0.2.0"
 description = "A library containing commong utilities for FLOps"
 authors = ["Alexander Malyuk <malyuk.alexander1999@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
+paho-mqtt = "2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 #[tool.poetry.scripts]
 #oak = "flops_utils.main:main"
```

