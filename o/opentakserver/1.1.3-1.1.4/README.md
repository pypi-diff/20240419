# Comparing `tmp/opentakserver-1.1.3.tar.gz` & `tmp/opentakserver-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentakserver-1.1.3.tar", max compression
+gzip compressed data, was "opentakserver-1.1.4.tar", max compression
```

## Comparing `opentakserver-1.1.3.tar` & `opentakserver-1.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.3/LICENSE
--rw-r--r--   0        0        0      128 2024-04-17 21:45:50.332409 opentakserver-1.1.3/opentakserver/__init__.py
--rw-r--r--   0        0        0    11181 2024-04-17 20:16:08.695625 opentakserver-1.1.3/opentakserver/app.py
--rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.3/opentakserver/blueprints/__init__.py
--rw-r--r--   0        0        0    46717 2024-04-11 18:07:13.514520 opentakserver-1.1.3/opentakserver/blueprints/api.py
--rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.3/opentakserver/blueprints/config.py
--rw-r--r--   0        0        0    26677 2024-04-17 04:54:25.448133 opentakserver-1.1.3/opentakserver/blueprints/marti.py
--rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.3/opentakserver/blueprints/ots_socketio.py
--rw-r--r--   0        0        0     4588 2024-04-11 02:49:02.199161 opentakserver-1.1.3/opentakserver/blueprints/scheduled_jobs.py
--rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.3/opentakserver/blueprints/scheduler_api.py
--rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.3/opentakserver/ca_config.py
--rw-r--r--   0        0        0    22983 2024-04-17 21:16:52.373937 opentakserver-1.1.3/opentakserver/certificate_authority.py
--rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.3/opentakserver/controllers/__init__.py
--rw-r--r--   0        0        0    10712 2024-04-11 02:48:20.040469 opentakserver-1.1.3/opentakserver/controllers/client_controller.py
--rw-r--r--   0        0        0    34898 2024-04-11 02:48:54.783881 opentakserver-1.1.3/opentakserver/controllers/cot_controller.py
--rw-r--r--   0        0        0     4057 2024-04-17 19:59:02.623288 opentakserver-1.1.3/opentakserver/defaultconfig.py
--rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.3/opentakserver/EmailValidator.py
--rw-r--r--   0        0        0      393 2024-04-17 03:09:51.512546 opentakserver-1.1.3/opentakserver/extensions.py
--rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.3/opentakserver/forms/__init__.py
--rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.3/opentakserver/forms/MediaMTXGlobalConfig.py
--rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.3/opentakserver/forms/MediaMTXPathConfig.py
--rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.3/opentakserver/functions.py
--rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.3/opentakserver/models/__init__.py
--rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.3/opentakserver/models/Alert.py
--rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.3/opentakserver/models/Base.py
--rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.3/opentakserver/models/CasEvac.py
--rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.3/opentakserver/models/Certificate.py
--rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.3/opentakserver/models/Chatrooms.py
--rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.3/opentakserver/models/ChatroomsUids.py
--rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.3/opentakserver/models/Config.py
--rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.3/opentakserver/models/CoT.py
--rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.3/opentakserver/models/DataPackage.py
--rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.3/opentakserver/models/EUD.py
--rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.3/opentakserver/models/GeoChat.py
--rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.3/opentakserver/models/Icon.py
--rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.3/opentakserver/models/Marker.py
--rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.3/opentakserver/models/Point.py
--rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.3/opentakserver/models/RBLine.py
--rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.3/opentakserver/models/role.py
--rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.3/opentakserver/models/Team.py
--rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.3/opentakserver/models/user.py
--rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.3/opentakserver/models/VideoRecording.py
--rw-r--r--   0        0        0     5476 2024-04-16 19:41:24.153676 opentakserver-1.1.3/opentakserver/models/VideoStream.py
--rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.3/opentakserver/models/WebAuthn.py
--rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.3/opentakserver/models/ZMIST.py
--rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.3/opentakserver/mumble/__init__.py
--rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.3/opentakserver/mumble/mumble_authenticator.py
--rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.3/opentakserver/mumble/mumble_ice_app.py
--rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.3/opentakserver/mumble/Murmur.ice
--rw-r--r--   0        0        0     3527 2024-04-10 20:27:14.987143 opentakserver-1.1.3/opentakserver/SocketServer.py
--rw-r--r--   0        0        0     1739 2024-04-17 21:45:50.320439 opentakserver-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2073 2024-04-11 21:18:43.687758 opentakserver-1.1.3/README.md
--rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 opentakserver-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.4/LICENSE
+-rw-r--r--   0        0        0      128 2024-04-19 13:33:00.560562 opentakserver-1.1.4/opentakserver/__init__.py
+-rw-r--r--   0        0        0    11215 2024-04-19 02:47:08.352294 opentakserver-1.1.4/opentakserver/app.py
+-rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.4/opentakserver/blueprints/__init__.py
+-rw-r--r--   0        0        0    46981 2024-04-19 03:39:10.045751 opentakserver-1.1.4/opentakserver/blueprints/api.py
+-rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.4/opentakserver/blueprints/config.py
+-rw-r--r--   0        0        0    26677 2024-04-19 02:42:08.495269 opentakserver-1.1.4/opentakserver/blueprints/marti.py
+-rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.4/opentakserver/blueprints/ots_socketio.py
+-rw-r--r--   0        0        0     4687 2024-04-19 02:52:24.809653 opentakserver-1.1.4/opentakserver/blueprints/scheduled_jobs.py
+-rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.4/opentakserver/blueprints/scheduler_api.py
+-rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.4/opentakserver/ca_config.py
+-rw-r--r--   0        0        0    22983 2024-04-17 21:16:52.373937 opentakserver-1.1.4/opentakserver/certificate_authority.py
+-rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.4/opentakserver/controllers/__init__.py
+-rw-r--r--   0        0        0    10751 2024-04-19 02:47:08.322372 opentakserver-1.1.4/opentakserver/controllers/client_controller.py
+-rw-r--r--   0        0        0    34945 2024-04-19 02:47:08.369247 opentakserver-1.1.4/opentakserver/controllers/cot_controller.py
+-rw-r--r--   0        0        0     4158 2024-04-19 03:39:10.047745 opentakserver-1.1.4/opentakserver/defaultconfig.py
+-rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.4/opentakserver/EmailValidator.py
+-rw-r--r--   0        0        0      393 2024-04-17 03:09:51.512546 opentakserver-1.1.4/opentakserver/extensions.py
+-rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.4/opentakserver/forms/__init__.py
+-rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.4/opentakserver/forms/MediaMTXGlobalConfig.py
+-rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.4/opentakserver/forms/MediaMTXPathConfig.py
+-rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.4/opentakserver/functions.py
+-rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.4/opentakserver/models/__init__.py
+-rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.4/opentakserver/models/Alert.py
+-rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.4/opentakserver/models/Base.py
+-rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.4/opentakserver/models/CasEvac.py
+-rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.4/opentakserver/models/Certificate.py
+-rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.4/opentakserver/models/Chatrooms.py
+-rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.4/opentakserver/models/ChatroomsUids.py
+-rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.4/opentakserver/models/Config.py
+-rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.4/opentakserver/models/CoT.py
+-rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.4/opentakserver/models/DataPackage.py
+-rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.4/opentakserver/models/EUD.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.4/opentakserver/models/GeoChat.py
+-rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.4/opentakserver/models/Icon.py
+-rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.4/opentakserver/models/Marker.py
+-rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.4/opentakserver/models/Point.py
+-rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.4/opentakserver/models/RBLine.py
+-rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.4/opentakserver/models/role.py
+-rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.4/opentakserver/models/Team.py
+-rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.4/opentakserver/models/user.py
+-rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.4/opentakserver/models/VideoRecording.py
+-rw-r--r--   0        0        0     5476 2024-04-16 19:41:24.153676 opentakserver-1.1.4/opentakserver/models/VideoStream.py
+-rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.4/opentakserver/models/WebAuthn.py
+-rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.4/opentakserver/models/ZMIST.py
+-rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.4/opentakserver/mumble/__init__.py
+-rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.4/opentakserver/mumble/mumble_authenticator.py
+-rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.4/opentakserver/mumble/mumble_ice_app.py
+-rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.4/opentakserver/mumble/Murmur.ice
+-rw-r--r--   0        0        0     3527 2024-04-10 20:27:14.987143 opentakserver-1.1.4/opentakserver/SocketServer.py
+-rw-r--r--   0        0        0     1739 2024-04-19 13:33:00.549622 opentakserver-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2073 2024-04-11 21:18:43.687758 opentakserver-1.1.4/README.md
+-rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 opentakserver-1.1.4/PKG-INFO
```

### Comparing `opentakserver-1.1.3/LICENSE` & `opentakserver-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/app.py` & `opentakserver-1.1.4/opentakserver/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     flask_wtf.CSRFProtect(app)
 
     socketio_logger = False
     if app.config.get("DEBUG"):
         socketio_logger = logger
     socketio.init_app(app, logger=socketio_logger)
 
-    rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters('127.0.0.1'))
+    rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters(app.config.get("OTS_RABBITMQ_SERVER_ADDRESS")))
     channel = rabbit_connection.channel()
     channel.exchange_declare('cot', durable=True, exchange_type='fanout')
     channel.exchange_declare('dms', durable=True, exchange_type='direct')
     channel.exchange_declare('chatrooms', durable=True, exchange_type='direct')
     channel.queue_declare(queue='cot_controller')
     channel.exchange_declare(exchange='cot_controller', exchange_type='fanout')
```

### Comparing `opentakserver-1.1.3/opentakserver/blueprints/api.py` & `opentakserver-1.1.4/opentakserver/blueprints/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,28 +615,28 @@
             v.generate_xml(request.json.get("ip"))
 
             with app.app_context():
                 try:
 
                     db.session.add(v)
                     db.session.commit()
-                    r = requests.post("http://localhost:9997/v3/config/paths/add/{}".format(v.path),
+                    r = requests.post("{}/v3/config/paths/add/{}".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), v.path),
                                       json=path_config)
                     if r.status_code == 200:
                         logger.debug("Added path {} to mediamtx".format(v.path))
                     else:
                         logger.error(
                             "Failed to add path {} to mediamtx. Status code {} {}".format(v.path, r.status_code,
                                                                                           r.text))
                     logger.debug("Inserted video stream {}".format(v.uid))
                 except sqlalchemy.exc.IntegrityError as e:
                     try:
                         db.session.rollback()
                         video = db.session.query(VideoStream).filter(VideoStream.path == v.path).first()
-                        r = requests.post("http://localhost:9997/v3/config/paths/add/{}".format(v.path),
+                        r = requests.post("{}/v3/config/paths/add/{}".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), v.path),
                                           json=json.loads(video.mediamtx_settings))
                         if r.status_code == 200:
                             logger.debug("Added path {} to mediamtx".format(v.path))
                         else:
                             logger.error(
                                 "Failed to add path {} to mediamtx. Status code {} {}".format(v.path, r.status_code,
                                                                                               r.text))
@@ -815,33 +815,33 @@
     if event == 'init':
         rtsp_port = bleach.clean(request.args.get("rtsp_port"))
         path = bleach.clean(request.args.get("path"))
 
         if path == 'startup':
             paths = VideoStream.query.all()
             for path in paths:
-                r = requests.post("http://localhost:9997/v3/config/paths/add/{}".format(path.path),
+                r = requests.post("{}/v3/config/paths/add/{}".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), path.path),
                                   json=json.loads(path.mediamtx_settings))
                 logger.debug("Init added {} {}".format(path, r.status_code))
 
             # Get all paths from MediaMTX and make sure they're in OTS's database
-            r = requests.get("http://localhost:9997/v3/paths/list")
+            r = requests.get("{}/v3/paths/list".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS")))
             paths = r.json()
             for path in paths['items']:
                 video_stream = db.session.query(VideoStream).where(VideoStream.path == path['name']).first()
                 if not video_stream:
                     if not path['source']:
                         continue
                     video_stream = VideoStream()
                     video_stream.protocol = get_stream_protocol(path['source']['type'])
 
-                    r = requests.get("http://localhost:9997/v3/config/global/get")
+                    r = requests.get("{}/v3/config/global/get".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS")))
                     video_stream.port = r.json()['rtspAddress'].replace(":", "")
 
-                    r = requests.get("http://localhost:9997/v3/config/paths/get/{}".format(path['name']))
+                    r = requests.get("{}/v3/config/paths/get/{}".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), path['name']))
                     video_stream.mediamtx_settings = json.dumps(r.json())
 
                     video_stream.path = path['name']
                     video_stream.alias = path['name']
                     video_stream.rtsp_reliable = 1
                     video_stream.ready = event == 'ready'
                     video_stream.rover_port = -1
@@ -866,15 +866,15 @@
         source_id = bleach.clean(request.args.get("source_id"))
 
         video_stream = db.session.query(VideoStream).where(VideoStream.path == path).first()
         if video_stream:
             video_stream.ready = event == 'ready'
             db.session.add(video_stream)
             db.session.commit()
-            r = requests.patch("http://localhost:9997/v3/config/paths/patch/{}".format(path),
+            r = requests.patch("{}/v3/config/paths/patch/{}".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), path),
                                json=json.loads(video_stream.mediamtx_settings))
             logger.debug("Ready Patched path {}: {} - {}".format(path, r.status_code, r.text))
         else:
             video_stream = VideoStream()
             if source_type.startswith('rtsps'):
                 video_stream.protocol = 'rtsps'
             if source_type.startswith('rtsp'):
@@ -1036,17 +1036,17 @@
             if isinstance(value, str):
                 value = bleach.clean(value)
             if value is not None:
                 settings[key] = value
                 logger.debug("set {} to {}".format(key, value))
 
         if request.path.endswith('update'):
-            r = requests.patch("http://localhost:9997/v3/config/paths/patch/{}".format(path), json=settings)
+            r = requests.patch("{}/v3/config/paths/patch/{}".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), path), json=settings)
         else:
-            r = requests.post("http://localhost:9997/v3/config/paths/add/{}".format(path), json=settings)
+            r = requests.post("{}/v3/config/paths/add/{}".format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), path), json=settings)
 
         if r.status_code == 200:
             logger.debug("Patched path {}: {}".format(path, r.status_code))
             video.mediamtx_settings = json.dumps(settings)
             db.session.add(video)
             db.session.commit()
             return jsonify({'success': True})
@@ -1066,15 +1066,15 @@
 def delete_stream():
     try:
         path = bleach.clean(request.args.get("path", ""))
 
         if not path:
             return jsonify({'success': False, 'error': 'Please specify a path name'}), 400
 
-        r = requests.delete('http://localhost:9997/v3/config/paths/delete/{}'.format(path))
+        r = requests.delete('{}/v3/config/paths/delete/{}'.format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"), path))
         logger.debug("Delete status code: {}".format(r.status_code))
         video = db.session.query(VideoStream).filter(VideoStream.path == path)
         if not video:
             return jsonify({'success': False, 'error': 'Path {} not found'.format(path)}), 400
 
         video.delete()
         db.session.commit()
```

### Comparing `opentakserver-1.1.3/opentakserver/blueprints/config.py` & `opentakserver-1.1.4/opentakserver/blueprints/config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/blueprints/marti.py` & `opentakserver-1.1.4/opentakserver/blueprints/marti.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/blueprints/ots_socketio.py` & `opentakserver-1.1.4/opentakserver/blueprints/ots_socketio.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/blueprints/scheduled_jobs.py` & `opentakserver-1.1.4/opentakserver/blueprints/scheduled_jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     with apscheduler.app.app_context():
         try:
             r = requests.get('https://api.airplanes.live/v2/point/{}/{}/{}'
                              .format(app.config["OTS_AIRPLANES_LIVE_LAT"],
                                      app.config["OTS_AIRPLANES_LIVE_LON"],
                                      app.config["OTS_AIRPLANES_LIVE_RADIUS"]))
             if r.status_code == 200:
-                rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters('127.0.0.1'))
+                rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters(app.config.get("OTS_RABBITMQ_SERVER_ADDRESS")))
                 channel = rabbit_connection.channel()
 
                 for craft in r.json()['ac']:
                     try:
                         event = adsbxcot.adsbx_to_cot(craft, known_craft=None)
                     except ValueError:
                         continue
@@ -67,20 +67,20 @@
 @apscheduler.task("interval", name="Delete Video Recordings", id="delete_video_recordings", next_run_time=None)
 def delete_video_recordings():
     with apscheduler.app.app_context():
         VideoRecording.query.delete()
         db.session.commit()
 
         try:
-            r = requests.get('http://localhost:9997/v3/recordings/list')
+            r = requests.get('{}/v3/recordings/list'.format(app.config.get("OTS_MEDIAMTX_API_ADDRESS")))
             if r.status_code == 200:
                 recordings = r.json()
                 for path in recordings['items']:
                     for recording in path['segments']:
-                        r = requests.delete('http://localhost:9997/v3/recordings/deletesegment',
+                        r = requests.delete('{}/v3/recordings/deletesegment'.format(app.config.get("OTS_MEDIAMTX_API_ADDRESS"),),
                                             params={'start': recording['start'], 'path': path['name']})
                         if r.status_code != 200:
                             logger.error(
                                 "Failed to delete {} from {}: {}".format(recording['start'], path['name'], r.text))
         except BaseException as e:
             logger.error("Failed to delete recordings: {}".format(e))
```

### Comparing `opentakserver-1.1.3/opentakserver/blueprints/scheduler_api.py` & `opentakserver-1.1.4/opentakserver/blueprints/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/ca_config.py` & `opentakserver-1.1.4/opentakserver/ca_config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/certificate_authority.py` & `opentakserver-1.1.4/opentakserver/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/controllers/client_controller.py` & `opentakserver-1.1.4/opentakserver/controllers/client_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                         self.common_name = c[0][1]
                         self.logger.debug("Got common name {}".format(self.common_name))
             except BaseException as e:
                 logger.warning("Failed to do handshake: {}".format(e))
 
         # RabbitMQ
         try:
-            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters('127.0.0.1'),
+            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters(self.app.config.get("OTS_RABBITMQ_SERVER_ADDRESS")),
                                                            self.on_connection_open)
             self.rabbit_channel = None
             self.iothread = Thread(target=self.rabbit_connection.ioloop.start)
             self.iothread.daemon = True
             self.iothread.start()
             self.is_consuming = False
         except BaseException as e:
```

### Comparing `opentakserver-1.1.3/opentakserver/controllers/cot_controller.py` & `opentakserver-1.1.4/opentakserver/controllers/cot_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         self.online_euds = {}
         self.online_callsigns = {}
         self.exchanges = []
 
         # RabbitMQ
         try:
-            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters('127.0.0.1'),
+            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters(self.context.app.config.get("OTS_RABBITMQ_SERVER_ADDRESS")),
                                                            self.on_connection_open)
             self.rabbit_channel = None
             self.iothread = Thread(target=self.rabbit_connection.ioloop.start)
             self.iothread.daemon = True
             self.iothread.start()
             self.is_consuming = False
         except BaseException as e:
```

### Comparing `opentakserver-1.1.3/opentakserver/defaultconfig.py` & `opentakserver-1.1.4/opentakserver/defaultconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
                               # 8080, 8443, and 8446 and proxy requests to OTS_LISTENER_PORT
     OTS_MARTI_HTTP_PORT = 8080
     OTS_MARTI_HTTPS_PORT = 8443
     OTS_ENABLE_TCP_STREAMING_PORT = True
     OTS_TCP_STREAMING_PORT = 8088
     OTS_SSL_STREAMING_PORT = 8089
     OTS_BACKUP_COUNT = 7
+    OTS_RABBITMQ_SERVER_ADDRESS = "127.0.0.1"
+    OTS_MEDIAMTX_API_ADDRESS = "http://localhost:9997"
     OTS_MEDIAMTX_TOKEN = str(secrets.SystemRandom().getrandbits(128))
     OTS_VERSION = opentakserver.__version__
     OTS_SSL_VERIFICATION_MODE = 2  # Equivalent to ssl.CERT_REQUIRED. https://docs.python.org/3/library/ssl.html#ssl.SSLContext.verify_mode
     OTS_NODE_ID = ''.join(random.choices(string.ascii_lowercase + string.digits, k=64))
     OTS_CA_NAME = 'OpenTAKServer-CA'
     OTS_CA_FOLDER = os.path.join(OTS_DATA_FOLDER, 'ca')
     OTS_CA_PASSWORD = 'atakatak'
```

### Comparing `opentakserver-1.1.3/opentakserver/EmailValidator.py` & `opentakserver-1.1.4/opentakserver/EmailValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/forms/MediaMTXGlobalConfig.py` & `opentakserver-1.1.4/opentakserver/forms/MediaMTXGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/forms/MediaMTXPathConfig.py` & `opentakserver-1.1.4/opentakserver/forms/MediaMTXPathConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/Alert.py` & `opentakserver-1.1.4/opentakserver/models/Alert.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/CasEvac.py` & `opentakserver-1.1.4/opentakserver/models/CasEvac.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/Certificate.py` & `opentakserver-1.1.4/opentakserver/models/Certificate.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/Chatrooms.py` & `opentakserver-1.1.4/opentakserver/models/Chatrooms.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/ChatroomsUids.py` & `opentakserver-1.1.4/opentakserver/models/ChatroomsUids.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/CoT.py` & `opentakserver-1.1.4/opentakserver/models/CoT.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/DataPackage.py` & `opentakserver-1.1.4/opentakserver/models/DataPackage.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/EUD.py` & `opentakserver-1.1.4/opentakserver/models/EUD.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/GeoChat.py` & `opentakserver-1.1.4/opentakserver/models/GeoChat.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/Icon.py` & `opentakserver-1.1.4/opentakserver/models/Icon.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/Marker.py` & `opentakserver-1.1.4/opentakserver/models/Marker.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/Point.py` & `opentakserver-1.1.4/opentakserver/models/Point.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/RBLine.py` & `opentakserver-1.1.4/opentakserver/models/RBLine.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/Team.py` & `opentakserver-1.1.4/opentakserver/models/Team.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/user.py` & `opentakserver-1.1.4/opentakserver/models/user.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/VideoRecording.py` & `opentakserver-1.1.4/opentakserver/models/VideoRecording.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/VideoStream.py` & `opentakserver-1.1.4/opentakserver/models/VideoStream.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/models/ZMIST.py` & `opentakserver-1.1.4/opentakserver/models/ZMIST.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/mumble/mumble_authenticator.py` & `opentakserver-1.1.4/opentakserver/mumble/mumble_authenticator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/mumble/mumble_ice_app.py` & `opentakserver-1.1.4/opentakserver/mumble/mumble_ice_app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/mumble/Murmur.ice` & `opentakserver-1.1.4/opentakserver/mumble/Murmur.ice`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/opentakserver/SocketServer.py` & `opentakserver-1.1.4/opentakserver/SocketServer.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/pyproject.toml` & `opentakserver-1.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentakserver"
-version = "1.1.3"
+version = "1.1.4"
 description = "A server for ATAK, WinTAK, and iTAK"
 authors = ["OpenTAKServer <opentakserver@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/brian7704/OpenTAKServer"
 documentation = "https://docs.opentakserver.io"
```

### Comparing `opentakserver-1.1.3/README.md` & `opentakserver-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.3/PKG-INFO` & `opentakserver-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentakserver
-Version: 1.1.3
+Version: 1.1.4
 Summary: A server for ATAK, WinTAK, and iTAK
 Home-page: https://github.com/brian7704/OpenTAKServer
 License: GPL-3.0-or-later
 Author: OpenTAKServer
 Author-email: opentakserver@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

