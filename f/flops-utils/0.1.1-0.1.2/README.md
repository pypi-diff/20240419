# Comparing `tmp/flops_utils-0.1.1.tar.gz` & `tmp/flops_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.1.1.tar", max compression
+gzip compressed data, was "flops_utils-0.1.2.tar", max compression
```

## Comparing `flops_utils-0.1.1.tar` & `flops_utils-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.1.1/README.md
--rw-r--r--   0        0        0     1430 2024-04-19 13:11:35.263869 flops_utils-0.1.1/flops_utils/logging.py
--rw-r--r--   0        0        0       42 2024-04-19 12:53:40.879871 flops_utils-0.1.1/flops_utils/main.py
--rw-r--r--   0        0        0      514 2024-04-19 13:12:03.003869 flops_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 flops_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.1.2/README.md
+-rw-r--r--   0        0        0     1443 2024-04-19 13:13:46.351869 flops_utils-0.1.2/flops_utils/logging.py
+-rw-r--r--   0        0        0       42 2024-04-19 12:53:40.879871 flops_utils-0.1.2/flops_utils/main.py
+-rw-r--r--   0        0        0      514 2024-04-19 13:14:05.055869 flops_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 flops_utils-0.1.2/PKG-INFO
```

### Comparing `flops_utils-0.1.1/flops_utils/logging.py` & `flops_utils-0.1.2/flops_utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     reset = "\x1b[0m"
 
     def __init__(self, fmt):
         super().__init__()
         self.fmt = fmt
         self.FORMATS = {
             # logging.DEBUG: self.grey + self.fmt + self.reset,
-            logging.INFO: self.light_blue + self.fmt + self.reset,
+            logging.INFO: self.light_blue + str(self.fmt).upper() + self.reset,
             logging.DEBUG: self.fmt,
             logging.INFO: self.fmt,
             logging.WARNING: self.yellow + self.fmt + self.reset,
             logging.ERROR: self.red + self.fmt + self.reset,
             logging.CRITICAL: self.bold_red + self.fmt + self.reset,
         }
```

### Comparing `flops_utils-0.1.1/pyproject.toml` & `flops_utils-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flops_utils"
-version = "0.1.1"
+version = "0.1.2"
 description = "A library containing commong utilities for FLOps"
 authors = ["Alexander Malyuk <malyuk.alexander1999@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```
