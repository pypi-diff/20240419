# Comparing `tmp/flops_utils-0.1.3.tar.gz` & `tmp/flops_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.1.3.tar", max compression
+gzip compressed data, was "flops_utils-0.1.4.tar", max compression
```

## Comparing `flops_utils-0.1.3.tar` & `flops_utils-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.1.3/README.md
--rw-r--r--   0        0        0     1443 2024-04-19 13:13:46.351869 flops_utils-0.1.3/flops_utils/logging.py
--rw-r--r--   0        0        0       42 2024-04-19 13:26:41.911868 flops_utils-0.1.3/flops_utils/testing.py
--rw-r--r--   0        0        0      514 2024-04-19 13:27:02.835868 flops_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 flops_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.1.4/README.md
+-rw-r--r--   0        0        0     1445 2024-04-19 13:33:07.691867 flops_utils-0.1.4/flops_utils/logging.py
+-rw-r--r--   0        0        0       42 2024-04-19 13:26:41.911868 flops_utils-0.1.4/flops_utils/testing.py
+-rw-r--r--   0        0        0      514 2024-04-19 13:33:15.331867 flops_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 flops_utils-0.1.4/PKG-INFO
```

### Comparing `flops_utils-0.1.3/flops_utils/logging.py` & `flops_utils-0.1.4/flops_utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(self, fmt):
         super().__init__()
         self.fmt = fmt
         self.FORMATS = {
             # logging.DEBUG: self.grey + self.fmt + self.reset,
             logging.INFO: self.light_blue + str(self.fmt).upper() + self.reset,
             logging.DEBUG: self.fmt,
-            logging.INFO: self.fmt,
+            # logging.INFO: self.fmt,
             logging.WARNING: self.yellow + self.fmt + self.reset,
             logging.ERROR: self.red + self.fmt + self.reset,
             logging.CRITICAL: self.bold_red + self.fmt + self.reset,
         }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
```

### Comparing `flops_utils-0.1.3/pyproject.toml` & `flops_utils-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flops_utils"
-version = "0.1.3"
+version = "0.1.4"
 description = "A library containing commong utilities for FLOps"
 authors = ["Alexander Malyuk <malyuk.alexander1999@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

