# Comparing `tmp/dm_aiomodbus-0.1.7.tar.gz` & `tmp/dm_aiomodbus-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_aiomodbus-0.1.7.tar", last modified: Mon Apr 15 08:15:37 2024, max compression
+gzip compressed data, was "dm_aiomodbus-0.1.8.tar", last modified: Fri Apr 19 11:40:41 2024, max compression
```

## Comparing `dm_aiomodbus-0.1.7.tar` & `dm_aiomodbus-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:37.679501 dm_aiomodbus-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-15 08:15:37.679501 dm_aiomodbus-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-15 08:15:23.000000 dm_aiomodbus-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:37.679501 dm_aiomodbus-0.1.7/dm_aiomodbus/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-15 08:15:23.000000 dm_aiomodbus-0.1.7/dm_aiomodbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-15 08:15:23.000000 dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-15 08:15:23.000000 dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-15 08:15:23.000000 dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_simulator_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-15 08:15:23.000000 dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_temp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:37.679501 dm_aiomodbus-0.1.7/dm_aiomodbus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-15 08:15:37.000000 dm_aiomodbus-0.1.7/dm_aiomodbus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-15 08:15:37.000000 dm_aiomodbus-0.1.7/dm_aiomodbus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:15:37.000000 dm_aiomodbus-0.1.7/dm_aiomodbus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 08:15:37.000000 dm_aiomodbus-0.1.7/dm_aiomodbus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 08:15:37.000000 dm_aiomodbus-0.1.7/dm_aiomodbus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:15:37.679501 dm_aiomodbus-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-15 08:15:37.000000 dm_aiomodbus-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:41.703598 dm_aiomodbus-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-19 11:40:41.703598 dm_aiomodbus-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-19 11:40:30.000000 dm_aiomodbus-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:41.703598 dm_aiomodbus-0.1.8/dm_aiomodbus/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-19 11:40:30.000000 dm_aiomodbus-0.1.8/dm_aiomodbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-19 11:40:30.000000 dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-19 11:40:30.000000 dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-19 11:40:30.000000 dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_simulator_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-19 11:40:30.000000 dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_temp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:41.703598 dm_aiomodbus-0.1.8/dm_aiomodbus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-19 11:40:41.000000 dm_aiomodbus-0.1.8/dm_aiomodbus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 11:40:41.000000 dm_aiomodbus-0.1.8/dm_aiomodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:40:41.000000 dm_aiomodbus-0.1.8/dm_aiomodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 11:40:41.000000 dm_aiomodbus-0.1.8/dm_aiomodbus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 11:40:41.000000 dm_aiomodbus-0.1.8/dm_aiomodbus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:40:41.707598 dm_aiomodbus-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-19 11:40:41.000000 dm_aiomodbus-0.1.8/setup.py
```

### Comparing `dm_aiomodbus-0.1.7/PKG-INFO` & `dm_aiomodbus-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomodbus
-Version: 0.1.7
+Version: 0.1.8
 Summary: This is my custom aiomodbus client
 Home-page: https://pypi.org/project/dm-aiomodbus
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomodbus
 Keywords: dm aiomodbus
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomodbus-0.1.7/README.md` & `dm_aiomodbus-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_base_client.py` & `dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_base_client.py`

 * *Files identical despite different names*

### Comparing `dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_clients.py` & `dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_clients.py`

 * *Files identical despite different names*

### Comparing `dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_simulator_client.py` & `dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_simulator_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self,
         disconnect_timeout_s: int = None,
         after_execute_timeout_ms: int = None,
         name_tag: str = None,
     ):
         super().__init__(
             aio_modbus_lib_class=AsyncModbusTcpClient,
-            modbus_config={"host": "192.168.0.0"},
+            modbus_config={"host": "simulator"},
             disconnect_timeout_s=disconnect_timeout_s,
             after_execute_timeout_ms=after_execute_timeout_ms,
             name_tag=name_tag
         )
         self.__connected = False
 
     @property
@@ -27,12 +27,13 @@
         self.__connected = True
         self._logger.info("Connected!")
 
     def _disconnect(self) -> None:
         self.__connected = False
         self._logger.info("Disconnected!")
 
-    async def _read(self, method, kwargs: dict) -> list | None:
-        return [i for i in range(kwargs["count"])]
+    async def _read(self, method, kwargs: dict) -> (list, str):
+        registers = [i for i in range(kwargs["count"])]
+        return (registers, "")
 
-    async def _write(self, method, kwargs: dict) -> bool:
-        return True
+    async def _write(self, method, kwargs: dict) -> (bool, str):
+        return (True, "")
```

### Comparing `dm_aiomodbus-0.1.7/dm_aiomodbus/aiomodbus_temp_client.py` & `dm_aiomodbus-0.1.8/dm_aiomodbus/aiomodbus_temp_client.py`

 * *Files identical despite different names*

### Comparing `dm_aiomodbus-0.1.7/dm_aiomodbus.egg-info/PKG-INFO` & `dm_aiomodbus-0.1.8/dm_aiomodbus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomodbus
-Version: 0.1.7
+Version: 0.1.8
 Summary: This is my custom aiomodbus client
 Home-page: https://pypi.org/project/dm-aiomodbus
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomodbus
 Keywords: dm aiomodbus
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomodbus-0.1.7/setup.py` & `dm_aiomodbus-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomodbus',
-    version='v0.1.7',
+    version='v0.1.8',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomodbus client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomodbus',
     packages=find_packages(),
```

