# Comparing `tmp/dm_aiomqtt-0.4.4.tar.gz` & `tmp/dm_aiomqtt-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_aiomqtt-0.4.4.tar", last modified: Fri Apr 19 09:08:29 2024, max compression
+gzip compressed data, was "dm_aiomqtt-0.4.5.tar", last modified: Fri Apr 19 16:04:20 2024, max compression
```

## Comparing `dm_aiomqtt-0.4.4.tar` & `dm_aiomqtt-0.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/dm_aiomqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/dm_aiomqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/dm_aiomqtt/dm_aiomqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/dm_aiomqtt/message_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:04:20.400370 dm_aiomqtt-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 16:04:20.400370 dm_aiomqtt-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-19 16:04:09.000000 dm_aiomqtt-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:04:20.396370 dm_aiomqtt-0.4.5/dm_aiomqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 16:04:09.000000 dm_aiomqtt-0.4.5/dm_aiomqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-19 16:04:09.000000 dm_aiomqtt-0.4.5/dm_aiomqtt/dm_aiomqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 16:04:09.000000 dm_aiomqtt-0.4.5/dm_aiomqtt/message_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:04:20.400370 dm_aiomqtt-0.4.5/dm_aiomqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 16:04:20.000000 dm_aiomqtt-0.4.5/dm_aiomqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 16:04:20.000000 dm_aiomqtt-0.4.5/dm_aiomqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:04:20.000000 dm_aiomqtt-0.4.5/dm_aiomqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 16:04:20.000000 dm_aiomqtt-0.4.5/dm_aiomqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 16:04:20.000000 dm_aiomqtt-0.4.5/dm_aiomqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:04:20.400370 dm_aiomqtt-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 16:04:19.000000 dm_aiomqtt-0.4.5/setup.py
```

### Comparing `dm_aiomqtt-0.4.4/PKG-INFO` & `dm_aiomqtt-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.4
+Version: 0.4.5
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomqtt-0.4.4/README.md` & `dm_aiomqtt-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.4/dm_aiomqtt/dm_aiomqtt_client.py` & `dm_aiomqtt-0.4.5/dm_aiomqtt/dm_aiomqtt_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                 will be converted all payload types
             - False:
                 will not be converted
         """
 
         async def cb(payload):
             if payload_to_json is True or (payload_to_json == "auto" and type(payload) not in (str, int, float)):
-                payload = json.dumps(payload, ensure_ascii=False)
+                payload = json.dumps(payload, ensure_ascii=False, separators=(',', ':'))
             try:
                 await self.__client.publish(topic, payload, qos)
             except Exception as e:
                 if self.__resend_ns_msg:
                     await self.__message_db.insert([topic, payload, qos])
                 if error_logging:
                     self.__logger.warning(f"Publish not sent: {e}")
```

### Comparing `dm_aiomqtt-0.4.4/dm_aiomqtt/message_db.py` & `dm_aiomqtt-0.4.5/dm_aiomqtt/message_db.py`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/PKG-INFO` & `dm_aiomqtt-0.4.5/dm_aiomqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.4
+Version: 0.4.5
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomqtt-0.4.4/setup.py` & `dm_aiomqtt-0.4.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomqtt',
-    version='v0.4.4',
+    version='v0.4.5',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomqtt client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomqtt',
     packages=find_packages(),
```

