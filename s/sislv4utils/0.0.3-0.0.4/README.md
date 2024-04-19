# Comparing `tmp/sislv4utils-0.0.3.tar.gz` & `tmp/sislv4utils-0.0.4.tar.gz`

## Comparing `sislv4utils-0.0.3.tar` & `sislv4utils-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/pyproject.toml.backup
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/src/sislv4utils/__init__.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/src/sislv4utils/config.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/src/sislv4utils/elastic.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/src/sislv4utils/message.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/src/sislv4utils/mqtt.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/src/sislv4utils/objectstore.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/src/sislv4utils/service.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/LICENSE
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/README.md
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sislv4utils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/src/sislv4utils/__init__.py
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/src/sislv4utils/config.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/src/sislv4utils/elastic.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/src/sislv4utils/message.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/src/sislv4utils/mqtt.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/src/sislv4utils/objectstore.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/src/sislv4utils/service.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/LICENSE
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 sislv4utils-0.0.4/PKG-INFO
```

### Comparing `sislv4utils-0.0.3/pyproject.toml.backup` & `sislv4utils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "sislv4utils1"
-version = "0.0.3"
+name = "sislv4utils"
+version = "0.0.4"
 
 authors = [
   { name="Bibhas Das", email="bibhas.das@somnetics.in" },
 ]
 
 description = "Seamless v4 utilities"
```

### Comparing `sislv4utils-0.0.3/src/sislv4utils/config.py` & `sislv4utils-0.0.4/src/sislv4utils/service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,174 +1,181 @@
 import os
 import sys
-import errno
+import getopt
+import resource
 import logging
-import configparser
-from os.path import join as make_path
-import etcd3
-from enum import Enum
-
-class Provider(Enum):
-        ETCD = 0,
-        FILE = 1
+import falcon
+import random
+import string
+from abc import abstractmethod, ABCMeta
+from wsgiref.simple_server import make_server
+
+from sislv4utils.config import Config
+from sislv4utils.message import MessageQueue
+from sislv4utils.mqtt import MqttClient
 
-class Config(object):
+class Service(object, metaclass=ABCMeta):
     # region members
 
-    _logformat = '%(asctime)s : %(levelname)s - %(filename)s (line: %(lineno)d) %(funcName)s() -> %(message)s'
-    _rundir_ = 'run'
-    _tmpdir_ = 'tmp'
-    _etcd_host = os.getenv('ETCD_HOST', '')
-    _etcd_port = int(os.getenv('ETCD_PORT', 2379))
-    _etcd_root = os.getenv('ETCD_ROOT', '/')
-    _provider = Provider.ETCD
+    _interactive = False
+    _config: Config = None
 
-    WAR_OPTIONVAL = 'Unable to parse value for option [{0}::{1}].'
-    ERR_PARSEFAIL = 'Error parsing config file.'
+    ERR_UNKNOWN_ERRORMSG = 'Exception caught {0} => ( {1} )'
 
     # endregion
-    # region methods
+    # region method
 
-    def __init__(self, provider: Provider = Provider.ETCD):
-        Config._provider = provider
-
-        # base path; all other folders will be relative to this path
-        self._moddir = os.path.dirname(
-            sys.modules[self.__class__.__module__].__file__)
-
-        # the run folder; if not available make one
-        self._rundir = make_path(self._moddir, Config._rundir_)
-        if not os.path.isdir(self._rundir):
-            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), self._rundir)
-
-        # temp path; if not available make one
-        self._tmpdir = make_path(self._rundir, Config._tmpdir_)
-        if not os.path.isdir(self._tmpdir):
-            os.makedirs(self._tmpdir)
-
-        # create a logfile in the run folder if one does not exists
-        self._logfile = make_path(self._rundir, 'service.log')
-
-        if Config._etcd_root[-1] != '/':
-            Config._etcd_root = Config._etcd_root + '/'
-
-        if Config._provider == Provider.ETCD:
-            self._parse()
-            return
-
-        # default config file; should be located in run folder
-        # if not provided by an user try to use this
-        self._cnffile = make_path(self._rundir, 'config.cnf')
-
-        # if the config file, whether default or user provided does not exists
-        # we have to stop the execution
-        if not os.path.isfile(self._cnffile):
-            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), self._cnffile)
-
-        # try to read the config file; if for some reason we cannot read it
-        # then there is no point in proceding further
-        self.cf = configparser.ConfigParser()
-        if len(self.cf.read(self._cnffile)) <= 0:
-            raise Exception(Config.ERR_PARSEFAIL)
-
-        self._parse()
-
-
-    def _parse(self):
-        # set the log level; by default it is 20 which is information
-        self._loglevel = self._parse_value('log', 'loglevel', 20, 'int', False)
-
-        # some basic settings taht are expcted to be found in the config file
-        self._host = self._parse_value('app', 'host', 'localhost', '', False)
-        self._port = self._parse_value('app', 'port', 8080, 'int', False)
-        self._user = self._parse_value('app', 'username', '', '', False)
-        self._pass = self._parse_value('app', 'password', '', '', False)
-
-
-    def _parse_value(self, section: str, option: str, default: any, data_type='', throw_error=False) -> any:
+    def start(self) -> None:
         try:
-            if Config._provider== Provider.FILE:
-                return getattr(self.cf, ('get' + data_type))(section, option)
-
-            etcdctl = etcd3.client(host=self._etcd_host, port=self._etcd_port)
-            ret, _ = etcdctl.get(Config._etcd_root + section + '/' + option)
-            if ret== None:
-                raise Exception()
-
-            ret = ret.decode().strip()
-
-            if data_type == "int":
-                ret = int(ret)
-            elif data_type == 'float':
-                ret= float(ret)
-            elif data_type == 'boolean':
-                ret= ret.lower() in ['true', '1', 't', 'y', 'yes']
-            else:
+            self.init_server()
+            self.start_server()
+            sys.exit(0)
+    
+        except getopt.GetoptError as err:
+            print(str(err))
+            sys.exit(1)
+
+        except Exception as err:
+            logging.error(str(err))
+            sys.exit(1)
+
+    def init_server(self) -> None:
+        # let us parse the configuration parameters
+        # and check if weed to run in interactive mode
+        opts, _ = getopt.getopt(sys.argv[1:], "i")
+        for opt, _ in opts:
+            if opt in ("-i"):
+                Service._interactive = True
+
+        # set appropriate mode i.e. interactive vs daemon
+        self._set_mode()
+
+    # a pure virtual method that will be implemented 
+    # in subsequent derived classes
+    @abstractmethod
+    def start_server(self) -> None:
+        pass
+
+    def _set_mode(self) -> None:
+        cf: Config = Service._config
+
+        # if we are running on interactive mode
+        # start logging and return from here
+        if Service._interactive:
+            return cf.start_logging(console=True)
+
+        # fork accordingly
+        if os.fork() != 0:
+            sys.exit(0)
+        os.setsid()
+        if os.fork() != 0:
+            sys.exit(0)
+
+        # close all open files and streams
+        maxfd = resource.getrlimit(resource.RLIMIT_NOFILE)[1]
+        if maxfd == resource.RLIM_INFINITY:
+            maxfd = 1024
+        for fd in range(0, maxfd):
+            try:
+                os.close(fd)
+            except OSError:
                 pass
 
-            return ret
-
-        except (configparser.Error, Exception) as e:
-            # wll, we encountered an error
-            message = Config.WAR_OPTIONVAL.format(section, option)
-
-            # if this setting is absolutely mandatory
-            # raise an exception and stop execution
-            if throw_error:
-                raise Exception(message)
-
-            # otherwise just log a warning and move on
-            logging.warning(message)
-            logging.debug('assuming [ {0} ] to continue.'.format(default))
-
-            return default
-
-
-    def set_etcd_key(key: str, value: str)-> None:
-        if Config._provider == Provider.ETCD:
-            etcd= etcd3.client(host= Config._etcd_host, port= Config._etcd_port)
-            etcd.put(Config._etcd_root + key, value)
-
-
-    def start_logging(self, console: bool = False) -> None:
-        # a service can be started either in interective mode or
-        # in daemon mode. it is decided by the command line argument
-        # the program was started with. the command line args are parsed
-        # and in case we are running in interactive mode, we log everything to console
-
-        if console:
-            logging.basicConfig(format=self._logformat, level=self._loglevel, handlers=[
-                logging.StreamHandler(sys.stdout)
-            ])
-
-        # othrwise log everything to the specified logfile
-           # while running in daemon mode, console is not available
-        else:
-            logging.basicConfig(format=self._logformat, level=self._loglevel, handlers=[
-                logging.FileHandler(self._logfile)
-            ])
+        # duplicate stdout & stdin
+        os.open(os.devnull, os.O_RDWR)
+        os.dup2(0, 1)
+        os.dup2(0, 2)
+
+        # start logging in the logfile
+        return cf.start_logging(console=False)
+    
+    def get_random_string(self, prefix: str = '', width: int = 6):
+        random_string = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(width))
+        return (prefix + random_string)
 
     # endregion
-    # region properties
 
-    @property
-    def apphost(self) -> str:
-        return self._host
-
-    @property
-    def appport(self) -> int:
-        return self._port
-
-    @property
-    def appuser(self) -> str:
-        return self._user
-
-    @property
-    def apppass(self) -> str:
-        return self._pass
-
-    @property
-    def etcdctl(self) -> any:
-        return etcd3.client(host= Config._etcd_host,
-            port= Config._etcd_port)
+class MQService(Service, metaclass=ABCMeta):
+    def __init__(self, name: str = ''):
+        self._name = self.get_random_string(
+            "mqservice-", 8) if not name else name
+
+    def start_server(self) -> None:
+        cf: Config = Service._config
+
+        # listen to a particuler queue with a given binding key
+        logging.info('listening on {0}:{1}...'.format(cf.mq_binding_exchange, cf.mq_binding_key))
+        with MessageQueue(host=cf.mq_host, port=cf.mq_port,
+            username=cf.appuser, password=cf.apppass) as ch:
+            ch.listen(exchange_name=cf.mq_binding_exchange, queue_name=self._name, binding_key=cf.mq_binding_key,
+                event_handler=self, event_callback_func='_callback_func_')
+
+    def _callback_func_(self, ch, method, properties, body, binding_key):
+        del ch, method, properties, binding_key
+
+        try:self.process(body)
+        except Exception as e:
+            logging.error(Service.ERR_UNKNOWN_ERRORMSG.format("_callback_func", str(e)))
+
+    @abstractmethod
+    def process(self, message: str) -> None:
+        pass
+
+class WebService(Service, metaclass=ABCMeta):
+
+    def __init__(self, name: str = ''):
+        self._name = self.get_random_string(
+            "webservice-", 8) if not name else name
+        
+    def start_server(self) -> None:
+        cf: Config = Service._config
+
+        # check if we are asked tor run on all interfaces
+        # they will be marked as * or all in config file
+        iface = cf.apphost
+        if iface == '*' or iface == 'all':
+            iface = ''
+
+        # add your routes here
+        self._app= falcon.App()
+        self._app.add_sink(self.on_post_request, '/')
+
+        # run falcon webserver
+        logging.info('serving on {0}:{1}...'.format(cf.apphost, cf.appport))
+        with make_server(iface, cf.appport, self._app) as httpd:
+            try: httpd.serve_forever()
+            except KeyboardInterrupt: return
+            
+    def on_post_request(self, req: falcon.Request, resp: falcon.Response) -> None:
+        try:
+            resp.content_type = falcon.MEDIA_TEXT
+            self.process(req, resp)
 
-    # endregion
+        # catch all exceptions
+        except Exception as e:
+            resp.status, resp.text = (falcon.HTTP_500,
+                Service.ERR_UNKNOWN_ERRORMSG.format('on_post_request', str(e)))
+    
+    @abstractmethod
+    def process(self, req: falcon.Request, resp: falcon.Response) -> None:
+        pass
+
+class MQTTService(Service, metaclass=ABCMeta):
+    def __init__(self, name: str = ''):
+        self._name = self.get_random_string(
+            "mqttservice-", 8) if not name else name
+
+    def start_server(self) -> None:
+        cf: Config = Service._config
+
+        # listen for a particuler topic
+        logging.info('subscribing {0}@{1}:{2} for topic...'.format(cf.mqtt_topic, cf.mqtt_host, cf.mqtt_port))
+        with MqttClient(host = cf.mqtt_host, port = cf.mqtt_port, 
+            username=cf.appuser, password=cf.apppass, randname=self._queue_name) as channel:
+            channel.listen(cf.mqtt_topic, self, '_on_message_callback_')
+
+    def _on_message_callback_(self, client, userdata, message) -> None:
+        self.process(message.payload)
+
+    @abstractmethod
+    def process(self, payload: str) -> None:
+        pass
```

### Comparing `sislv4utils-0.0.3/src/sislv4utils/elastic.py` & `sislv4utils-0.0.4/src/sislv4utils/elastic.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.3/src/sislv4utils/message.py` & `sislv4utils-0.0.4/src/sislv4utils/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,22 @@
 
     def __init__(self, host: str, port: int, username: str, password: str):
         self.conn = None
 
         # prepare all connection related parameters
         self.credential = pika.PlainCredentials(username, password)
         self.parameters = pika.ConnectionParameters(host=host, port=port, credentials= self.credential)
-        self.channels = []
 
     def __enter__(self):
         # create a blocking connection
         self.connect()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         del exc_type, exc_value, exc_traceback
-
-        # close all open channels
-        for ch in self.channels:
-            ch.close()
-
-        # cleanup and close this object
-        self.channels.clear()
         self.close()
 
     #endregion
     #region methods
 
     def connect(self):
         if not self.conn:
@@ -61,15 +53,14 @@
 
         # check if we have a valid connection
         if not self.conn:
             raise Exception(MessageQueue.ERR_NOT_CONNECTED)
 
         # create a new channel and add it to our list
         channel = self.conn.channel()
-        self.channels.append(channel)
 
         # setup a queue and make it ready for basic consumption
         channel.queue_declare(queue=queue_name, durable=True, auto_delete=True)
         channel.queue_bind(exchange=exchange_name, queue=queue_name, routing_key=binding_key)
         channel.basic_consume(
             queue=queue_name,
             auto_ack=True,
@@ -83,10 +74,9 @@
         try:
             channel.start_consuming()
         except KeyboardInterrupt:
             pass
 
         # close everything, remove from list of channels and return
         channel.close()
-        self.channels.remove(channel)
 
     #endregion
```

### Comparing `sislv4utils-0.0.3/src/sislv4utils/mqtt.py` & `sislv4utils-0.0.4/src/sislv4utils/mqtt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-import string
-import random
 import time
 import paho.mqtt.client as mqttc
 
 class MqttClient(object):
     #region members
 
-    ERR_NOT_CONNECTED = 'not connected to any message queue'
+    ERR_NOT_CONNECTED = 'not connected to any broker'
 
     #endregion
     #region constructor / destructor
 
-    def __init__(self, host: str, port: int, username: str, password: str, 
-        randname: str = "", randsize: int = 6):
+    def __init__(self, host: str, port: int, username: str, password: str, queue_name: str):
 
         self._host: str = host
         self._port: int = port
-
-        self._conn = mqttc.Client(mqttc.CallbackAPIVersion.VERSION2,
-            client_id= self.get_random_string(randname, randsize))
+        self._conn: mqttc.Client = mqttc.Client(mqttc.CallbackAPIVersion.VERSION2, client_id= queue_name)
         self._conn.username_pw_set(username, password)
         self._connected = False
 
     def __enter__(self):
         # create a blocking connection
         self.connect()
         return self
@@ -31,39 +26,38 @@
         del exc_type, exc_value, exc_traceback
         self.close()
 
     #endregion
     #region methods
 
     def connect(self):
-        if self._connected: return
-        if self._conn.connect(self._host, self._port) == 0:
+        if not self._connected and self._conn.connect(host= self._host, port= self._port) == 0:
             self._connected = True
 
     def close(self):
-        if not self._connected: return
-        if self._conn.disconnect() == 0:
+        if self._connected and self._conn.disconnect()== 0:            
             self._connected = False
 
     def publish(self, topic: str, message: str) -> None:
-        # check if we have a valid connection
         if not self._connected:
             raise Exception(MqttClient.ERR_NOT_CONNECTED)
-        
+                
         self._conn.loop_start()
         self._conn.publish(topic, message)
         time.sleep(1)
         self._conn.loop_stop()
 
-    def listen(self, topic: str):
-       # check if we have a valid connection
-       if not self._connected:
+    def listen(self, topic: str, event_handler: callable, event_callback_func: str):
+        if not self._connected:
             raise Exception(MqttClient.ERR_NOT_CONNECTED)
 
-       self._conn.subscribe(topic)
-       self._conn.loop_forever()
+        self._conn.on_message = lambda client, userdata, message: getattr(
+            event_handler, event_callback_func)(client, userdata, message)
 
-    def get_random_string(self, prefix: str = '', width: int = 6):
-        random_string = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(width))
-        return (prefix + random_string)
+        try:
+            self._conn.subscribe(topic)
+            self._conn.loop_forever()
+            
+        except KeyboardInterrupt:
+            pass
  
     #endregion
```

### Comparing `sislv4utils-0.0.3/src/sislv4utils/objectstore.py` & `sislv4utils-0.0.4/src/sislv4utils/objectstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
     def upload(self, bucket_name: str, objectid: str, localfile: str) -> bool:
         self.s3.fput_object(bucket_name=bucket_name, object_name=objectid, file_path=localfile)
         return self.object_exists(bucket_name=bucket_name, object_name=objectid)
 
     def put_object(self, bucket_name: str, object_name: str, data: any):
         self.s3.put_object(bucket_name=bucket_name, object_name=object_name,
-                           data=io.BytesIO(data), length=-1,
-                           part_size=ObjectStore._default_chunk_size)
+            data=io.BytesIO(data), length=-1, part_size=ObjectStore._default_chunk_size)
 
     def bucket_exists(self, bucket_name: str) -> bool:
         return self.s3.bucket_exists(bucket_name)
 
     def object_exists(self, bucket_name: str, object_name: str) -> bool:
         try:
             self.s3.stat_object(bucket_name=bucket_name, object_name=object_name)
         except:
             return False
         else:
             return True
 
     # endregion
+
```

### Comparing `sislv4utils-0.0.3/.gitignore` & `sislv4utils-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.3/LICENSE` & `sislv4utils-0.0.4/LICENSE`

 * *Files identical despite different names*

