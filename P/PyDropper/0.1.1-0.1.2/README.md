# Comparing `tmp/pydropper-0.1.1.tar.gz` & `tmp/pydropper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydropper-0.1.1.tar", max compression
+gzip compressed data, was "pydropper-0.1.2.tar", max compression
```

## Comparing `pydropper-0.1.1.tar` & `pydropper-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-04-17 04:46:17.465496 pydropper-0.1.1/LICENSE
--rw-r--r--   0        0        0     1356 2024-04-17 07:11:50.487159 pydropper-0.1.1/README.md
--rw-r--r--   0        0        0       22 2024-04-19 09:00:00.051634 pydropper-0.1.1/pydropper/__init__.py
--rw-r--r--   0        0        0       27 2024-04-17 06:57:32.511939 pydropper-0.1.1/pydropper/env.py
--rw-r--r--   0        0        0      454 2024-04-19 09:00:51.846725 pydropper-0.1.1/pydropper/main.py
--rw-r--r--   0        0        0       40 2024-04-17 05:19:54.009724 pydropper-0.1.1/pydropper/server/__init__.py
--rw-r--r--   0        0        0      227 2024-04-17 05:21:42.763548 pydropper-0.1.1/pydropper/server/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2291 2024-04-18 02:21:24.323352 pydropper-0.1.1/pydropper/server/__pycache__/funcs.cpython-312.pyc
--rw-r--r--   0        0        0     1579 2024-04-18 07:25:21.933269 pydropper-0.1.1/pydropper/server/__pycache__/server_main.cpython-312.pyc
--rw-r--r--   0        0        0     1011 2024-04-17 07:03:39.145192 pydropper-0.1.1/pydropper/server/funcs.py
--rw-r--r--   0        0        0      555 2024-04-18 02:47:52.726173 pydropper-0.1.1/pydropper/server/server_main.py
--rw-r--r--   0        0        0      386 2024-04-19 09:01:44.217351 pydropper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 pydropper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-17 04:46:17.465496 pydropper-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1356 2024-04-17 07:11:50.487159 pydropper-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-19 09:00:00.051634 pydropper-0.1.2/pydropper/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-17 06:57:32.511939 pydropper-0.1.2/pydropper/env.py
+-rw-r--r--   0        0        0      549 2024-04-19 09:11:57.351897 pydropper-0.1.2/pydropper/main.py
+-rw-r--r--   0        0        0       40 2024-04-17 05:19:54.009724 pydropper-0.1.2/pydropper/server/__init__.py
+-rw-r--r--   0        0        0      227 2024-04-17 05:21:42.763548 pydropper-0.1.2/pydropper/server/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2291 2024-04-18 02:21:24.323352 pydropper-0.1.2/pydropper/server/__pycache__/funcs.cpython-312.pyc
+-rw-r--r--   0        0        0     1579 2024-04-18 07:25:21.933269 pydropper-0.1.2/pydropper/server/__pycache__/server_main.cpython-312.pyc
+-rw-r--r--   0        0        0     1014 2024-04-19 09:13:06.040822 pydropper-0.1.2/pydropper/server/funcs.py
+-rw-r--r--   0        0        0      621 2024-04-19 09:12:39.299288 pydropper-0.1.2/pydropper/server/server_main.py
+-rw-r--r--   0        0        0      386 2024-04-19 09:14:34.412612 pydropper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 pydropper-0.1.2/PKG-INFO
```

### Comparing `pydropper-0.1.1/LICENSE` & `pydropper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydropper-0.1.1/README.md` & `pydropper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pydropper-0.1.1/pydropper/server/__pycache__/funcs.cpython-312.pyc` & `pydropper-0.1.2/pydropper/server/__pycache__/funcs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pydropper-0.1.1/pydropper/server/__pycache__/server_main.cpython-312.pyc` & `pydropper-0.1.2/pydropper/server/__pycache__/server_main.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pydropper-0.1.1/pydropper/server/funcs.py` & `pydropper-0.1.2/pydropper/server/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 
 
 class Server(Thread):
     def __init__(self):
         super().__init__()
         self.config = uvicorn.Config(
-            app="PyDrop.server.server_main:app",
+            app="PyDropper.server.server_main:app",
             host="0.0.0.0",
             port=8001,
             log_level="info",
         )
         self.server = uvicorn.Server(config=self.config)
         self._stop_event = Event()
```

### Comparing `pydropper-0.1.1/PKG-INFO` & `pydropper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDropper
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: jiho7407
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: fastapi (>=0.110.1,<0.111.0)
```

