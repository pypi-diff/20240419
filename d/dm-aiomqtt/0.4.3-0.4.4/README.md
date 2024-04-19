# Comparing `tmp/dm_aiomqtt-0.4.3.tar.gz` & `tmp/dm_aiomqtt-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_aiomqtt-0.4.3.tar", last modified: Fri Apr 19 08:01:03 2024, max compression
+gzip compressed data, was "dm_aiomqtt-0.4.4.tar", last modified: Fri Apr 19 09:08:29 2024, max compression
```

## Comparing `dm_aiomqtt-0.4.3.tar` & `dm_aiomqtt-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-19 08:00:52.000000 dm_aiomqtt-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:03.837780 dm_aiomqtt-0.4.3/dm_aiomqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 08:00:52.000000 dm_aiomqtt-0.4.3/dm_aiomqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-19 08:00:52.000000 dm_aiomqtt-0.4.3/dm_aiomqtt/dm_aiomqtt_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:01:03.841780 dm_aiomqtt-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 08:01:03.000000 dm_aiomqtt-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/dm_aiomqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/dm_aiomqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/dm_aiomqtt/dm_aiomqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 09:08:20.000000 dm_aiomqtt-0.4.4/dm_aiomqtt/message_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:08:29.381534 dm_aiomqtt-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 09:08:29.000000 dm_aiomqtt-0.4.4/setup.py
```

### Comparing `dm_aiomqtt-0.4.3/PKG-INFO` & `dm_aiomqtt-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.3
+Version: 0.4.4
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
@@ -91,21 +91,23 @@
        host="localhost",
        port=1883,
        resend_not_success_messages=True
    )
    ```
 
 Now, in case of loss of connection, all messages that were sent during this period will be re-sent as soon as the connection appears again.
+<br>
 **BUT** the `payload` will be in a changed format `[your_payload]_dt_[iso_local_datetime]`
 
 **Example**:
+<br>
 Your payload: `"{"temp": 12}"`
+<br>
 Edited payload: `"{"temp": 12}_dt_2024-04-19T09:57:40"`
 
-
 ### Set custom logger
 
 _If you want set up custom logger_
 
 ```python
 from dm_aiomqtt import DMAioMqttClient
```

### Comparing `dm_aiomqtt-0.4.3/README.md` & `dm_aiomqtt-0.4.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,21 +74,23 @@
        host="localhost",
        port=1883,
        resend_not_success_messages=True
    )
    ```
 
 Now, in case of loss of connection, all messages that were sent during this period will be re-sent as soon as the connection appears again.
+<br>
 **BUT** the `payload` will be in a changed format `[your_payload]_dt_[iso_local_datetime]`
 
 **Example**:
+<br>
 Your payload: `"{"temp": 12}"`
+<br>
 Edited payload: `"{"temp": 12}_dt_2024-04-19T09:57:40"`
 
-
 ### Set custom logger
 
 _If you want set up custom logger_
 
 ```python
 from dm_aiomqtt import DMAioMqttClient
```

### Comparing `dm_aiomqtt-0.4.3/dm_aiomqtt/dm_aiomqtt_client.py` & `dm_aiomqtt-0.4.4/dm_aiomqtt/dm_aiomqtt_client.py`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.3/dm_aiomqtt.egg-info/PKG-INFO` & `dm_aiomqtt-0.4.4/dm_aiomqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.3
+Version: 0.4.4
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
@@ -91,21 +91,23 @@
        host="localhost",
        port=1883,
        resend_not_success_messages=True
    )
    ```
 
 Now, in case of loss of connection, all messages that were sent during this period will be re-sent as soon as the connection appears again.
+<br>
 **BUT** the `payload` will be in a changed format `[your_payload]_dt_[iso_local_datetime]`
 
 **Example**:
+<br>
 Your payload: `"{"temp": 12}"`
+<br>
 Edited payload: `"{"temp": 12}_dt_2024-04-19T09:57:40"`
 
-
 ### Set custom logger
 
 _If you want set up custom logger_
 
 ```python
 from dm_aiomqtt import DMAioMqttClient
```

### Comparing `dm_aiomqtt-0.4.3/setup.py` & `dm_aiomqtt-0.4.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomqtt',
-    version='v0.4.3',
+    version='v0.4.4',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomqtt client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomqtt',
     packages=find_packages(),
```

