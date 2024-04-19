# Comparing `tmp/rfb-cycler-cu-manager-0.0.2.tar.gz` & `tmp/rfb_cycler_cu_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfb-cycler-cu-manager-0.0.2.tar", last modified: Tue Mar 19 11:42:46 2024, max compression
+gzip compressed data, was "rfb_cycler_cu_manager-0.0.3.tar", last modified: Fri Apr 19 12:25:23 2024, max compression
```

## Comparing `rfb-cycler-cu-manager-0.0.2.tar` & `rfb_cycler_cu_manager-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:42:46.509147 rfb-cycler-cu-manager-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-19 11:42:43.000000 rfb-cycler-cu-manager-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43352 2024-03-19 11:42:46.509147 rfb-cycler-cu-manager-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:42:46.509147 rfb-cycler-cu-manager-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:42:46.505147 rfb-cycler-cu-manager-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:42:46.505147 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-19 11:42:46.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/cu_broker_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/cu_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-19 11:42:15.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/register.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:42:46.505147 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43352 2024-03-19 11:42:46.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-19 11:42:46.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:42:46.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 11:42:46.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 11:42:46.000000 rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:23.086016 rfb_cycler_cu_manager-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-19 12:25:20.000000 rfb_cycler_cu_manager-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43352 2024-04-19 12:25:23.086016 rfb_cycler_cu_manager-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:25:23.086016 rfb_cycler_cu_manager-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:23.078016 rfb_cycler_cu_manager-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:23.082016 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 12:25:22.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/cu_broker_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/cu_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32605 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-19 12:25:00.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:23.082016 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43352 2024-04-19 12:25:23.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-19 12:25:23.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:25:23.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-19 12:25:23.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 12:25:23.000000 rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/top_level.txt
```

### Comparing `rfb-cycler-cu-manager-0.0.2/LICENSE.txt` & `rfb_cycler_cu_manager-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rfb-cycler-cu-manager-0.0.2/PKG-INFO` & `rfb_cycler_cu_manager-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-cycler-cu-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Module used to manage the computational unit.
 Author-email: Javier Sanz <javiersanzmoline+pypi@gmail.com>, Raldea <r.aldea.csic+pypi@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rfb-cycler-cu-manager-0.0.2/pyproject.toml` & `rfb_cycler_cu_manager-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/context.py` & `rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 
 ######################             CONSTANTS              ######################
 # For further information check out README.md
 DEFAULT_TX_CAN_NAME     : str = 'TX_CAN'            # Default tx_can system queue name
 DEFAULT_TX_SCPI_NAME    : str = 'TX_SCPI'           # Default tx_scpi system queue name
 DEFAULT_RX_CAN_NAME     : str = 'RX_CAN_QUEUE'      # Default rx_can system queue name
 DEFAULT_CAN_ENABLED     : bool = False              # Default value, hardware is compatible with can
-DEFAULT_DETECT_TIMEOUT  : int = 2                   # Default time to read asked devices answers
+DEFAULT_DETECT_TIMEOUT  : int = 15                   # Default time to read asked devices answers
 DEFAULT_DEV_PATH        : str = '/dev/wattrex/'     # Default path to the devices
 DEFAULT_SCPI_QUEUE_PREFIX : str = 'DET_'             # Default prefix for the scpi queues
 DEFAULT_CU_ID_PATH      : str = './config/cu_manager/.cu_id'
 # Default path to credential file for rabbitmq
 DEFAULT_CRED_PATH       : str = './config/.cred.yaml'
 
 CONSTANTS_NAMES = ('DEFAULT_TX_CAN_NAME', 'DEFAULT_TX_SCPI_NAME',
                    'DEFAULT_RX_CAN_NAME', 'DEFAULT_DETECT_TIMEOUT',
                    'DEFAULT_DEV_PATH', 'DEFAULT_SCPI_QUEUE_PREFIX',
                    'DEFAULT_CU_ID_PATH', 'DEFAULT_CRED_PATH', 'DEFAULT_CAN_ENABLED')
 
 sys_conf_update_config_params(context=globals(),
                               constants_names=CONSTANTS_NAMES,
-                              section='wattrex_cycler_cu_manager')
+                              section='rfb_cycler_cu_manager')
```

### Comparing `rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/cu_broker_client.py` & `rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/cu_broker_client.py`

 * *Files identical despite different names*

### Comparing `rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/cu_manager.py` & `rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/cu_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         hb = self.__gather_heartbeat(self.cu_id)
         self.client_mqtt.publish_heartbeat(hb)
 
     def process_cycler_deploy_processes(self) -> None:
         '''
         Process the cycler deploy processes
         '''
-        for process in self.cycler_deploy_processes:
+        for process in list(self.cycler_deploy_processes):
             if process.poll() is not None:
                 self.cycler_deploy_processes.remove(process)
                 log.info(f"CS deployed: {process.args[2]}")
                 log.info(f"CS ({process.args[2]}) deploy process return code: {process.stdout}")
                 self.active_cs[int(process.args[2])] = datetime.now()
 
 
@@ -181,15 +181,16 @@
                 log.debug(f"Heartbeat received from cs: {msg_heart}")
                 if msg_heart in self.active_cs:
                     self.active_cs[msg_heart] = datetime.now()
                 else:
                     log.error(f"Received heartbeat from unknown cycler station: {msg_heart.cu_id}")
             else:
                 log.error("Received unknown message in heartbeat queue")
-        for cs_id, time_elapse in self.active_cs.items():
+        active_cs = self.active_cs
+        for cs_id, time_elapse in active_cs.items():
             if (datetime.now() - time_elapse).total_seconds() > 10:
                 log.info(f"CS {cs_id} disconnected")
                 del self.active_cs[cs_id]
         res.active_cs = list(self.active_cs.keys())
         return res
```

### Comparing `rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/detect.py` & `rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,18 @@
 ## The models corresponds to the bits of the serial number to know which sensor has.
 comp_dev = {
     'EPC': {'Model_0': 2},
             ## Future models of EPCs
             # , 'Model_1': 4, 'Model_2': 5, 'Model_3': 6, 'Model_4': 7, 'Model_5': 8,
             # 'Model_6': 9, 'Model_7': 10, 'Model_8': 11, 'Model_9': 12, 'Model_A': 13,
             # 'Model_B': 14, 'Model_C': 15, 'Model_D': 16, 'Model_E': 17},
-    'EA': {'VIRTUAL': 1, 'PS_2042-20_B': 4, 'PSB_10200-420': 6},
+    'EA': {'VIRTUAL': 1, 'PS_2042-20_B': 4, 'PSB_10200-420': 6, 'PSB_2384-05_B': 7,
+           'PSB_9080-120': 10, 'PSB_10500-180': 11, 'PS_2042-06B':9},
     'RS': {'RS-KEL103': 5},
-    'BK': {},
+    'BK': {'2831E': 8},
     'BMS': 3,
     'FLOW': {},
 }
 
 class DetectorC: #pylint: disable= too-many-instance-attributes
     '''
     Classmethod to handle DetectorCectorC .
@@ -357,15 +358,15 @@
         '''
         if not self.__reqs_bisources: #pylint: disable= too-many-nested-blocks
             ## Create a queue for each SCPI connected device
             for bisource_name in self.found_scpi_devs['bisource']:
                 try:
                     self.__rx_scpi[bisource_name] = SysShdIpcChanC(
                                                 name= DEFAULT_SCPI_QUEUE_PREFIX+bisource_name,
-                                                max_message_size=400)
+                                                max_message_size=600)
                 except Exception as exc:
                     log.error(f"Error creating queue for bisource: {exc}")
                     self.close()
                     raise exc
                 self.__tx_scpi.send_data(DrvScpiCmdDataC(
                                             data_type=DrvScpiCmdTypeE.ADD_DEV,
                                             port=DEFAULT_DEV_PATH+'bisource/'+bisource_name,
```

### Comparing `rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager/register.py` & `rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager/register.py`

 * *Files identical despite different names*

### Comparing `rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/PKG-INFO` & `rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-cycler-cu-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Module used to manage the computational unit.
 Author-email: Javier Sanz <javiersanzmoline+pypi@gmail.com>, Raldea <r.aldea.csic+pypi@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rfb-cycler-cu-manager-0.0.2/src/rfb_cycler_cu_manager.egg-info/SOURCES.txt` & `rfb_cycler_cu_manager-0.0.3/src/rfb_cycler_cu_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

