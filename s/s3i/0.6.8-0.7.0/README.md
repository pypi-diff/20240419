# Comparing `tmp/s3i-0.6.8-py3-none-any.whl.zip` & `tmp/s3i-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 27710 bytes, number of entries: 19
--rw-r--r--  2.0 unx     1150 b- defN 24-Apr-10 15:48 s3i/__init__.py
--rw-r--r--  2.0 unx    11141 b- defN 24-Apr-10 21:26 s3i/broker.py
+Zip file size: 25253 bytes, number of entries: 19
+-rw-r--r--  2.0 unx     1106 b- defN 24-Apr-19 12:32 s3i/__init__.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-Apr-19 12:32 s3i/broker.py
 -rw-r--r--  2.0 unx    23600 b- defN 24-Apr-10 15:48 s3i/broker_message.py
 -rw-r--r--  2.0 unx     6627 b- defN 24-Apr-10 15:48 s3i/callback_manager.py
 -rw-r--r--  2.0 unx     7206 b- defN 24-Apr-10 15:48 s3i/config.py
 -rw-r--r--  2.0 unx     3028 b- defN 24-Apr-10 17:26 s3i/directory.py
 -rw-r--r--  2.0 unx     5324 b- defN 24-Apr-10 17:26 s3i/ditto_manager.py
--rw-r--r--  2.0 unx    14678 b- defN 24-Apr-10 15:48 s3i/event_system.py
+-rw-r--r--  2.0 unx    14682 b- defN 24-Apr-19 12:32 s3i/event_system.py
 -rw-r--r--  2.0 unx    15645 b- defN 24-Apr-10 15:48 s3i/exception.py
--rw-r--r--  2.0 unx    12097 b- defN 24-Apr-10 15:48 s3i/identity_provider.py
+-rw-r--r--  2.0 unx     2361 b- defN 24-Apr-19 12:32 s3i/identity_provider.py
 -rw-r--r--  2.0 unx     4567 b- defN 21-Nov-09 20:20 s3i/key_pgp.py
 -rw-r--r--  2.0 unx     1008 b- defN 21-Nov-09 20:20 s3i/logger.py
 -rw-r--r--  2.0 unx      455 b- defN 21-Nov-09 20:20 s3i/repository.py
 -rw-r--r--  2.0 unx     1110 b- defN 24-Apr-10 17:26 s3i/tools.py
--rw-rw-rw-  2.0 unx     7651 b- defN 24-Apr-10 21:31 s3i-0.6.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1360 b- defN 24-Apr-10 21:31 s3i-0.6.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 21:31 s3i-0.6.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 21:31 s3i-0.6.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1407 b- defN 24-Apr-10 21:31 s3i-0.6.8.dist-info/RECORD
-19 files, 118150 bytes uncompressed, 25486 bytes compressed:  78.4%
+-rw-rw-rw-  2.0 unx     7651 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1469 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1406 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/RECORD
+19 files, 108127 bytes uncompressed, 23029 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: s3i/repository.py
 Comment: 
 
 Filename: s3i/tools.py
 Comment: 
 
-Filename: s3i-0.6.8.dist-info/LICENSE.txt
+Filename: s3i-0.7.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: s3i-0.6.8.dist-info/METADATA
+Filename: s3i-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: s3i-0.6.8.dist-info/WHEEL
+Filename: s3i-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: s3i-0.6.8.dist-info/top_level.txt
+Filename: s3i-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: s3i-0.6.8.dist-info/RECORD
+Filename: s3i-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## s3i/__init__.py

```diff
@@ -1,9 +1,8 @@
 from s3i.identity_provider import IdentityProvider
-from s3i.identity_provider import TokenType
 from s3i.ditto_manager import DittoManager
 from s3i.directory import Directory
 from s3i.repository import Repository
 from s3i.broker import BrokerREST, BrokerAMQP
 from s3i.config import Config
 from s3i.broker_message import UserMessage, ServiceReply, ServiceRequest, GetValueReply, GetValueRequest, \
     SetValueRequest, SetValueReply, \
```

## s3i/broker.py

```diff
@@ -1,19 +1,19 @@
 import asyncio
 import functools
+import logging
 import ssl
 import requests
 import json
 
 import pika
 import pika.exceptions
 from pika.adapters.asyncio_connection import AsyncioConnection
 from s3i.exception import raise_error_from_s3ib_amqp, raise_error_from_broker_api_response, S3IBrokerRESTError, \
     S3IBrokerAMQPError
-from s3i.logger import APP_LOGGER
 from s3i.callback_manager import CallbackManager
 from s3i.config import Config
 
 CONTENT_TYPE = "application/json"
 HOST = "broker.s3i.vswf.dev"
 VIRTUAL_HOST = "s3i"
 DIRECT_EXCHANGE = "demo.direct"
@@ -102,210 +102,205 @@
 
 class BrokerAMQP:
     _ON_CONNECTION_OPEN = "_on_connection_open"
     _ON_CONNECTION_CLOSED = "_on_connection_closed"
     _ON_CHANNEL_OPEN = "_on_channel_open"
     _ON_CHANNEL_CLOSED = "_on_channel_closed"
 
-    def __init__(self, token, endpoint, callback, loop=asyncio.get_event_loop(), listenToEvents=False):
+    def __init__(self, token, loop=asyncio.get_event_loop(), logger=logging.getLogger()):
         self.__token = token
-        self.__endpoint = endpoint
-        self.__event_endpoint = None
-        self.__loop = loop
-        self.__callback = callback
-        self.__credentials = None
-        self.__connection_parameters = None
+
         self.__connection = None
         self.__channel = None
-        self.__consumer_tag = None
-        self.__event_consumer_tag = None
-        self.__listen_to_events = listenToEvents
 
+        self.__loop = loop
+        self.__logger = logger
+
+        self.__delivery_tag = 0
+        self.__consumer_tag = None
         self.__is_consuming = False
-        self.__schedule_messages = []
-        self.__callbacks = CallbackManager()
+
+        self.__callback_manager = CallbackManager()
 
     @property
     def token(self):
         return self.__token
 
-    @token.setter
-    def token(self, value):
-        self.__token = value
-
     @property
     def connection(self):
         return self.__connection
 
     @property
     def channel(self):
         return self.__channel
 
+    @property
+    def delivery_tag(self):
+        return self.__delivery_tag
+
     def connect(self):
-        self.__credentials = pika.PlainCredentials(
+        credentials = pika.PlainCredentials(
             username=" ",
             password=self.__token,
             erase_on_connect=True
         )
-        self.__connection_parameters = pika.ConnectionParameters(
+        connection_parameters = pika.ConnectionParameters(
             host=HOST,
             virtual_host=VIRTUAL_HOST,
-            credentials=self.__credentials,
-            heartbeat=3600,
+            credentials=credentials,
+            heartbeat=10,
             port=5671,
             ssl_options=pika.SSLOptions(ssl.SSLContext())
         )
-        self.__connection = AsyncioConnection(
-            parameters=self.__connection_parameters,
+        AsyncioConnection(
+            parameters=connection_parameters,
             on_open_callback=self.on_connection_open,
             on_open_error_callback=self.on_connection_open_error,
             on_close_callback=self.on_connection_closed,
             custom_ioloop=self.__loop
         )
-        if self.__listen_to_events:
-            self.create_event_queue()
+
+    def reconnect_token_expired(self, token):
+        self.__token = token
+        self.__connection.update_secret(token, reason="Token expired")
 
     def on_connection_open(self, _unused_connection):
-        APP_LOGGER.info("[S3I]: Connection to Broker built")
+        self.__logger.info("[S3I]: Opening broker connection succeed")
+        self.__connection = _unused_connection
 
-        self.__channel = _unused_connection.channel(
+        _unused_connection.channel(
             on_open_callback=self.on_channel_open
         )
-        self.__callbacks.process(
+
+        self.__callback_manager.process(
             self._ON_CONNECTION_OPEN,
             self.__loop
         )
 
-    @staticmethod
-    def on_connection_open_error(_unused_connection, err):
-        APP_LOGGER.error("[S3I]: Connection to broker failed: {}".format(err))
-
-    def on_connection_closed(self, _unused_connection, reason):
-        APP_LOGGER.info("[S3I]: Connection to Broker closed: {}".format(reason))
-        if self.__is_consuming:
-            self.__until_all_closed_and_reconnect()
+    def on_connection_open_error(self, _unused_connection, err):
+        self.__logger.error("[S3I]: Opening broker connection failed: {}".format(err))
+
+    def on_connection_closed(self, _unused_connection, err):
+        self.__logger.info("[S3I]: Current Broker connection closed: {}".format(err))
 
     def on_channel_open(self, _unused_channel):
-        APP_LOGGER.info("[S3I]: Channel open and start consuming messages")
+        self.__logger.info("[S3I]: Opening broker channel succeed")
+        self.__channel = _unused_channel
+
+        # Add callback function for channel closing
         _unused_channel.add_on_close_callback(self.on_channel_closed)
         _unused_channel.basic_qos(
             prefetch_count=1
         )
-        if self.__callback is not None:
-            self.start_consuming()
-        self.__callbacks.process(
-            self._ON_CHANNEL_OPEN,
-            self.__loop
-        )
+
+        self.__callback_manager.process(self._ON_CHANNEL_OPEN, self.__loop)
+
+    def on_channel_closed(self, channel, reason):
+        self.__logger.info("[S3I]: Current broker channel closed: {}".format(reason))
+        self.__callback_manager.process(self._ON_CHANNEL_CLOSED, self.__loop)
+        if not self.__connection.is_closed:
+            self.__connection.close()
 
     def add_on_channel_open_callback(self, callback, one_shot, *args, **kwargs):
-        self.__callbacks.add(
+        self.__callback_manager.add(
             self._ON_CHANNEL_OPEN,
             callback,
             one_shot,
             False,
             *args,
             **kwargs
         )
 
+    def add_on_channel_close_callback(self, callback, one_shot, *arg, **kwargs):
+        self.__callback_manager.add(
+            self._ON_CHANNEL_CLOSED,
+            callback,
+            one_shot,
+            False,
+            *arg,
+            **kwargs
+        )
+
     def add_on_connection_open_callback(self, callback, one_shot, *args, **kwargs):
-        self.__callbacks.add(
+        self.__callback_manager.add(
             self._ON_CONNECTION_OPEN,
             callback,
             one_shot,
             False,
             *args,
             **kwargs
         )
 
-    def start_consuming(self):
+    def add_on_connection_close_callback(self, callback, one_shot, *args, **kwargs):
+        self.__callback_manager.add(
+            self._ON_CONNECTION_CLOSED,
+            callback,
+            one_shot,
+            False,
+            *args,
+            **kwargs
+        )
+
+    def start_consuming(self, endpoint, on_message):
         self.__consumer_tag = self.__channel.basic_consume(
             auto_ack=True,
             exclusive=True,
-            queue=self.__endpoint,
-            on_message_callback=self.__callback
+            queue=endpoint,
+            on_message_callback=on_message
         )
-        if self.__event_endpoint is not None:
-            self.__event_consumer_tag = self.__channel.basic_consume(
-                auto_ack=True,
-                exclusive=True,
-                queue=self.__event_endpoint,
-                on_message_callback=self.__callback)
-
+        self.__logger.info(f"Consuming to endpoint {endpoint}")
         self.__is_consuming = True
 
     def stop_consuming(self):
-        if self.__event_consumer_tag is not None:
-            self.__channel.basic_cancel(self.__event_consumer_tag)
-
         cb = functools.partial(
             self.on_consumer_cancel_ok, userdata=self.__consumer_tag
         )
         self.__channel.basic_cancel(self.__consumer_tag, cb)
         self.__is_consuming = False
 
-    def on_channel_closed(self, channel, reason):
-        APP_LOGGER.info("[S3I]: Channel is closed: {}".format(reason))
-        if not self.__connection.is_closed:
-            self.__connection.close()
-
     def on_consumer_cancel_ok(self, _unused_frame, userdata):
         if not self.__is_consuming:
             self.__channel.close()
 
-    def reconnect_token_expired(self, token):
-        self.__token = token
-        """
-        Stop comsuming and invoke the stop function for channel and connection 
-        """
-        if self.__is_consuming:
-            self.stop_consuming()
-        """
-        Check if the channel and connection are closed 
-        """
-        self.__until_all_closed_and_reconnect()
+    def publish_message(self, endpoint: str, message: dict):
+        msg_id = message.get("identifier")
+        if isinstance(message, dict):
+            message = json.dumps(message)
+        self.__delivery_tag += 1
+        raise_error_from_s3ib_amqp(
+            self.__channel.basic_publish,
+            S3IBrokerAMQPError,
+            DIRECT_EXCHANGE,
+            endpoint,
+            message,
+            pika.BasicProperties(
+                content_type="application/json",
+                delivery_mode=pika.DeliveryMode.Transient
+            )
+        )
+        self.__logger.info(f"Sending normal message (message id: {msg_id}, delivery tag: {self.__delivery_tag}) to {endpoint}")
 
-    def __until_all_closed_and_reconnect(self):
-        if not self.__channel.is_closed or not self.__connection.is_closed:
-            self.__loop.call_later(
-                0.1,
-                self.__until_all_closed_and_reconnect
+    def publish_event(self, topic, message):
+        msg_id = message.get("identifier")
+        if isinstance(message, dict):
+            message = json.dumps(message)
+        self.__delivery_tag += 1
+        raise_error_from_s3ib_amqp(
+            self.__channel.basic_publish,
+            S3IBrokerAMQPError,
+            EVENT_EXCHANGE,
+            topic,
+            message,
+            pika.BasicProperties(
+                content_type="application/json",
+                delivery_mode=pika.DeliveryMode.Transient
             )
-        else:
-            APP_LOGGER.info("[S3I]: Reconnect to Broker")
-            self.connect()
+        )
+        self.__logger.info(f"Sending event message (message id: {msg_id}, delivery tag: {self.__delivery_tag}) to {topic}")
 
-    def send(self, endpoints, msg):
-        if isinstance(msg, dict):
-            msg = json.dumps(msg)
-        if self.__channel.is_open:
-            for endpoint in endpoints:
-                raise_error_from_s3ib_amqp(
-                    self.__channel.basic_publish,
-                    S3IBrokerAMQPError,
-                    DIRECT_EXCHANGE,
-                    endpoint,
-                    msg,
-                    pika.BasicProperties(
-                        content_type="application/json",
-                        delivery_mode=2
-                    ))
-                APP_LOGGER.info("[S3I]: Sending message successes")
-        
-    def publish_event(self, msg, topic):
-        if self.__channel.is_open:
-            raise_error_from_s3ib_amqp(
-                self.__channel.basic_publish,
-                S3IBrokerAMQPError,
-                EVENT_EXCHANGE,
-                topic,
-                msg,
-                pika.BasicProperties(
-                    content_type="application/json",
-                ))
 
     def create_event_queue(self):
         conf = Config(self.__token)
         identifier = self.__endpoint.replace("s3ibs://", '')
         identifier = identifier.replace("s3ib://", '')
         response = conf.create_broker_event_queue(thing_id=identifier, topic=[])
         self.__event_endpoint = response.json()['queue_name']
@@ -318,23 +313,22 @@
                 S3IBrokerAMQPError,
                 exchange=EVENT_EXCHANGE,
                 queue=self.__event_endpoint,
                 routing_key=topic
             )
 
         else:
-            APP_LOGGER.error("[S3I]: No event endpoint configured yet")
+            self.__logger.error("[S3I]: No event endpoint configured yet")
             return False
 
     def unsubscribe_topic(self, topic):
         if self.__channel.is_open and self.__event_endpoint is not None:
             raise_error_from_s3ib_amqp(
                 self.__channel.queue_unbind,
                 S3IBrokerAMQPError,
                 exchange=EVENT_EXCHANGE,
                 queue=self.__event_endpoint,
                 routing_key=topic
             )
-
         else:
-            APP_LOGGER.error("[S3I]: No event endpoint configured yet")
+            self.__logger.error("[S3I]: No event endpoint configured yet")
             return False
```

## s3i/event_system.py

```diff
@@ -183,15 +183,15 @@
 
     def emit_named_event(self, publisher, topic, content):
         event_obj = self.__named_event_dict.get(topic)
         if isinstance(event_obj, NamedEvent):
             event_obj.generate_event_msg(content=content)
             publisher.publish_event(
                 topic=topic,
-                msg=json.dumps(event_obj.msg)
+                message=json.dumps(event_obj.msg)
             )
         else:
             raise ValueError
 
 
     def emit_custom_event(self, publisher, topic):
         event_obj = self.__custom_event_dict.get(topic)
```

## s3i/identity_provider.py

```diff
@@ -1,306 +1,68 @@
-import requests
-import json
-from enum import Enum
-import time
-import threading
-from jwt.algorithms import RSAPSSAlgorithm
-from jwt import DecodeError, ExpiredSignature, InvalidTokenError
-import jwt
-from s3i.exception import S3IIdentityProviderError, raise_error_from_keycloak_response
-from s3i.logger import APP_LOGGER
-import webbrowser
-
-
-oauth2_flows = ["password", "client_credentials", "authorization_code_flow"]
-oauth_proxy_url = "https://auth.s3i.vswf.dev"
-
-
-class TokenType(Enum):
-    """Enum TokenType covers all available tokens specified in openID connect"""
-
-    # COMPLETE_BUNDLE = 1
-    ID_TOKEN = 2
-    ACCESS_TOKEN = 3
-    REFRESH_TOKEN = 4
-
+from keycloak import KeycloakOpenID
 
 class IdentityProvider:
-    """ Class IdentityProvider contains functions to communicate with S3I IdentityProvider """
-
-    def __init__(self, grant_type, client_id, client_secret, realm="KWH",
-                 identity_provider_url="https://idp.s3i.vswf.dev/", username=None,
-                 password=None):
-        """
-        Constructor
-
-        :param grant_type: grant type to obtain JWT. Here only the types "password" and "client_credentials" are implemented. In subsequent version authorization_code will be implemented 
-        :type grant_type: str
-        :param client_id: id of registered client in S3I IdentityProvider
-        :type client_id: str 
-        :param client_secret: credential of registered client in S3I IdentityProvider which must corredspond to client id 
-        :type client_secret: str 
-        :param realm: registered realm in S3I IdentityProvider 
-        :type realm: str
-        :param identity_provider_url: url of S3I IdentityProvider 
-        :type identity_provider_url: str 
-        :param username: username of registered user in S3I IdentityProvider. If grant type is set up as password, this field must be filled 
-        :type username: str 
-        :param password: password of registered user in S3I IdentityProvider. If grant type is set up as password, this field must be filled 
-        :type password: str
-
-        """
-        self._grant_type = grant_type
-        self._client_id = client_id
-        self._client_secret = client_secret
-        self._realm = realm
-        self._username = username
-        self._password = password
-        self._identity_provider_url = identity_provider_url
-        self._identity_provider_get_token = self.identity_provider_url + \
-                                            "auth/realms/" + self.realm + "/protocol/openid-connect/token"
-        self._identity_provider_header = {
-            "Content-Type": "application/x-www-form-urlencoded"}
-        self._token_bundle = None
-        self._token_inspector_run = False
-        self._last_login = 0
-        self._identity_provider_get_pub_key = self.identity_provider_url + \
-                                              "auth/realms/" + self.realm + "/protocol/openid-connect/certs"
-
-    @property
-    def identity_provider_url(self):
-        """Url of S3I IdentityProvider
-        """
-        return self._identity_provider_url
-
-    @property
-    def identity_provider_get_token(self):
-        """Url to obtain a token from the S3I IdentityProvider
-        """
-        return self._identity_provider_get_token
-
-    @property
-    def identity_provider_header(self):
-        """Header which is sent to the S3I IdentityProvider via HTTP
-        """
-        return self._identity_provider_header
-
-    @property
-    def grand_type(self):
-        """OAuth grant type which is used
-        """
-        return self._grant_type
+    def __init__(self, client_id, client_secret, realm, idp_url, logger, username=None, password=None):
+        self.__client_id = client_id
+        self.__client_secret = client_secret
+        self.__realm = realm
+        self.__idp_url = idp_url
+
+        self.__connection = None
+        self.__token_set = None
+        self.__access_token = None
+        self.__refresh_token = None
+        self.__logger = logger
+        self.__username = username
+        self.__password = password
 
     @property
     def client_id(self):
-        """
-        """
-        return self._client_id
+        return self.__client_id
 
     @property
-    def client_secret(self):
-        """
-        """
-        return self._client_secret
+    def token_set(self):
+        return self.__token_set
 
     @property
-    def realm(self):
-        """
-        """
-        return self._realm
+    def access_token(self):
+        return self.__access_token
 
     @property
-    def username(self):
-        """
-        """
-        return self._username
+    def refresh_token(self):
+        return self.__refresh_token
 
-    @property
-    def password(self):
-        """
-        """
-        return self._password
+    def connect(self):
+        self.__logger.info("Connect to the Identity Provider")
+        self.__connection = KeycloakOpenID(
+            server_url=self.__idp_url,
+            realm_name=self.__realm,
+            client_id=self.__client_id,
+            client_secret_key=self.__client_secret
+        )
 
-    def stop_run_forever(self):
-        """ Stops the run forever loop when the next iteration happens """
-        self._token_inspector_run = False
-
-    def get_token(self, token_type, request_new=False, scope="openid"):
-        """ 
-        Returns a token from the S3I IdentityProvider, request a new one if there is no valid token available
-        Works only if the IdentityProvider is NOT in the run_forever loop
-
-        :param token_type: type of token, see enum TokenType
-        :type token_type: TokenType
-        :param request_new: request a new token in any case
-        :type request_new: bool
-        :param scope: client scope
-        :type scope: str
-        :return: token
-        :rtype: str
-        """
-        if self._token_inspector_run:
-            return None
-        if request_new:
-            self._authenticate(scope=scope)
+    def get_token_set(self):
+        if self.__username and self.__password:
+            self.__token_set = self.__connection.token(
+                username=self.__username,
+                password=self.__password
+            )
         else:
-            if self._token_bundle is None:
-                self._authenticate(scope=scope)
-            if self._time_until_token_valid() <= 0:
-                self._authenticate(scope=scope)
-        # all tokens are valid
-        if token_type == TokenType.ACCESS_TOKEN:
-            return self._token_bundle["access_token"]
-        elif token_type == TokenType.ID_TOKEN:
-            return self._token_bundle["id_token"]
-        elif token_type == TokenType.REFRESH_TOKEN:
-            return self._token_bundle["refresh_token"]
-        return None
-
-    def get_certs(self):
-        """
-        Return a certificate of S³I Identity Provider
-
-        """
-        certs = requests.get(url=self._identity_provider_get_pub_key,
-                             headers={"Authorization": "Bearer {}".format(
-                                 self.get_token(token_type=TokenType.ACCESS_TOKEN))})
-        return certs.json()
-
-    def verify_token(self, token, aud="rabbitmq"):
-        """
-        This function verifies if the given jwt token is issued by the S³I Identity Provider
- 
-        :param token: jwt token
-        :type token: str
-        :param aud: audience, by default rabbitmq.
-        :type aud: str
-        :return: True if token is issued by S³I, else False
-        :rtype: bool
-        """
-        keys = self.get_certs().get("keys")
-        """search public key"""
-        for key in keys:
-            if key["alg"] == "RS256" and key["kty"] == "RSA" and key["use"] == "sig":
-                public_key = RSAPSSAlgorithm.from_jwk(json.dumps(key))
-                break
-        try:
-            """decode the access token with public key that was searched above"""
-            jwt.decode(jwt=token, verify=True, key=public_key, algorithms=['RS256'], audience=aud)
-        except (DecodeError, ExpiredSignature, InvalidTokenError):
-            return False
-        else:
-            return True
-
-    def run_forever(self, token_type, on_new_token, sleep_interval=5, scope=""):
-        """ 
-        Requests tokens from the S³I IdentityProvider and refreshs them if they reach their timeout
-
-        :param token_type: type of token, see enum TokenType (REFRESH_TOKEN is no valid param)
-        :type token_type: TokenType
-        :param on_new_token: callback if a new token is available
-        :type on_new_token: callback
-        :param scope: client scope
-        :type scope: str
-        """
-        if token_type == TokenType.REFRESH_TOKEN:
-            return None
-        on_new_token(self.get_token(token_type, request_new=True, scope=scope))
-        self._token_inspector_run = True
-        threading._start_new_thread(
-            self._run_forever_loop, (token_type, on_new_token, sleep_interval, scope))
-
-    def _run_forever_loop(self, token_type, on_new_token, slep_interval, scope=""):
-        while True and self._token_inspector_run:
-            while True:
-                if not self._token_inspector_run:
-                    return None  # exit
-                if self._time_until_token_valid() > slep_interval * 2:
-                    time.sleep(slep_interval)
-                else:
-                    break
-            # its time to refresh the tokens
-            APP_LOGGER.info("request for new token")
-            APP_LOGGER.info("last login: {}, now: {}, expires in: {}".format(self._last_login,
-                                                                             time.time(),
-                                                                             self._token_bundle["expires_in"]))
-            if self._token_bundle["expires_in"] < 60:
-                ### keycloak returns an unexpected token expire time
-                self._authenticate(scope=scope)
-            else:
-                self._refresh_token(self._token_bundle["refresh_token"], scope)
-            if token_type == TokenType.ACCESS_TOKEN:
-                on_new_token(self._token_bundle["access_token"])
-            elif token_type == TokenType.ID_TOKEN:
-                on_new_token(self._token_bundle["id_token"])
-
-    def _authenticate(self, scope):
-        """ Request the token-bundle from the S³I IdentityProvider 
-        
-            :param scope: client scope
-            :type scope: str 
-        """
-
-        self._last_login = time.time()
-        if self.grand_type not in oauth2_flows:
-            return {}
-        elif self.grand_type == "authorization_code_flow":
-            init_url = "{0}/initialize/{1}/{2}".format(oauth_proxy_url, self.client_id, self.client_secret)
-            init_resp = requests.get(init_url)
-            init_resp_json = init_resp.json()
-            webbrowser.open_new_tab("{}/{}".format(oauth_proxy_url, init_resp_json["redirect_url"]))
-            proxy_user_id = init_resp_json["proxy_user_identifier"]
-            proxy_user_secret = init_resp_json["proxy_secret"]
-            pickup_url = "{}/pickup/{}/{}".format(oauth_proxy_url, proxy_user_id, proxy_user_secret)
-
-            max_retries = 100
-            pickup_resp = requests.get(pickup_url)
-            for i in range(max_retries):
-                if not pickup_resp.text:
-                    pickup_resp = requests.get(pickup_url)
-                    time.sleep(0.5)
-                else:
-                    break
-            pickup_resp_json = pickup_resp.json()
-            decoded_jwt = jwt.decode(pickup_resp_json["access_token"], verify=False)
-            pickup_resp_json["expires_in"] = decoded_jwt["exp"] - decoded_jwt["iat"]
-            self._token_bundle = pickup_resp_json
-
-        else:
-            body = dict()
-            body["grant_type"] = self._grant_type
-            body["client_id"] = self._client_id
-            body["client_secret"] = self._client_secret
-            if self.grand_type == "password":
-                body["username"] = self._username
-                body["password"] = self._password
-            if scope:
-                body["scope"] = scope
-            response = requests.post(url=self._identity_provider_get_token,
-                                     data=body, headers=self._identity_provider_header)
-            raise_error_from_keycloak_response(response, S3IIdentityProviderError, 200)
-            self._token_bundle = response.json()
-
-    def _refresh_token(self, token, scope=""):
-        """ Refreshes the given token
-
-        :param token: type of token, see enum TokenType
-        :type token: str
-        """
-        self._last_login = time.time()
-        body = dict()
-        body["grant_type"] = "refresh_token"
-        body["client_id"] = self._client_id
-        body["client_secret"] = self._client_secret
-        body["refresh_token"] = token
-        if scope:
-            body["scope"] = scope
-        response = requests.post(url=self._identity_provider_get_token,
-                                 data=body, headers=self._identity_provider_header)
-        raise_error_from_keycloak_response(response, S3IIdentityProviderError, 200)
-        self._token_bundle = response.json()
-
-    def _time_until_token_valid(self):
-        """ Returns the time until the token expires """
-        time_token_valid = self._token_bundle["expires_in"]
-        time_since_login = time.time() - self._last_login
-        return time_token_valid - time_since_login
+            self.__token_set = self.__connection.token(
+                grant_type=["client_credentials"]
+            )
+        if self.__token_set:
+            self.__logger.info("Token set obtained")
+            self.__access_token = self.__token_set["access_token"]
+            self.__refresh_token = self.__token_set["refresh_token"]
+
+    def refresh_token_set(self):
+        if self.__refresh_token:
+            __token_set = self.__connection.refresh_token(
+                self.__refresh_token
+            )
+            if __token_set["refresh_token"] != self.__token_set["refresh_token"] and __token_set["access_token"] != self.__token_set["access_token"]:
+                self.__logger.info("Token set refreshed")
+                self.__token_set = __token_set
+                if self.__token_set:
+                    self.__access_token = self.__token_set["access_token"]
+                    self.__refresh_token = self.__token_set["refresh_token"]
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `s3i-0.6.8.dist-info/LICENSE.txt` & `s3i-0.7.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `s3i-0.6.8.dist-info/METADATA` & `s3i-0.7.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: s3i
-Version: 0.6.8
+Version: 0.7.0
 Home-page: https://www.kwh40.de/
 Author: Kompetenzzentrum Wald und Holz 4.0
 Author-email: s3i@kwh40.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.txt
 Requires-Dist: alabaster ==0.7.12
 Requires-Dist: astroid ==2.3.3
 Requires-Dist: certifi ==2019.11.28
 Requires-Dist: cffi ==1.13.2
 Requires-Dist: chardet ==3.0.4
 Requires-Dist: colorama ==0.4.3
-Requires-Dist: cryptography ==2.8
+Requires-Dist: cryptography ==42.0.5
 Requires-Dist: idna ==2.8
 Requires-Dist: isort ==4.3.21
 Requires-Dist: Jinja2 ==2.10.3
+Requires-Dist: jsonschema ==4.21.1
 Requires-Dist: lazy-object-proxy ==1.4.3
 Requires-Dist: MarkupSafe ==1.1.1
 Requires-Dist: mccabe ==0.6.1
-Requires-Dist: pika ==1.1.0
+Requires-Dist: pika ==1.3.2
 Requires-Dist: pockets ==0.9.1
 Requires-Dist: pycparser ==2.19
 Requires-Dist: Pygments ==2.5.2
 Requires-Dist: PyJWT ==1.7.1
 Requires-Dist: python-benedict ==0.21.0
 Requires-Dist: pyparsing ==2.4.5
 Requires-Dist: pytz ==2019.3
 Requires-Dist: pyrql ==0.6.0
-Requires-Dist: requests ==2.22.0
+Requires-Dist: python-keycloak ==3.9.0
+Requires-Dist: requests ==2.25.1
 Requires-Dist: six ==1.13.0
 Requires-Dist: snowballstemmer ==2.0.0
 Requires-Dist: typed-ast ==1.4.0
 Requires-Dist: wrapt ==1.11.2
 Requires-Dist: pgpy
 Requires-Dist: python-gnupg
 Requires-Dist: websocket-client
 Requires-Dist: schema ==0.7.1
 Requires-Dist: pynput
+Requires-Dist: urllib3 ==1.26.5
```

## Comparing `s3i-0.6.8.dist-info/RECORD` & `s3i-0.7.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-s3i/__init__.py,sha256=XcktGr-t5oji7QhpS698sssz5ViT_G7Luz-b29CWmsQ,1150
-s3i/broker.py,sha256=9BuxHuJmlChB52v0K7PJromyYm8cB2ge7sEmmmFXGn8,11141
+s3i/__init__.py,sha256=Sfd_rF3kYzXkXrGKupuyJBvMPibiWZA-xNZ3gPlVbZo,1106
+s3i/broker.py,sha256=Zr7TTpQqdnH24zywDFTfoU1ImtcaSe_PEzpiW_FcSE8,10786
 s3i/broker_message.py,sha256=xIVE6Ku6T6yBih8NcVoweVU3vpCkTrRZsI7oZEEUhCI,23600
 s3i/callback_manager.py,sha256=5lTs4h-pNfExBtFUEfHsKVXVrQOl5EwRg-vw_wQUFZI,6627
 s3i/config.py,sha256=aoLSe6W-B4o5eW6onabsLJTutkXvlrpGNWXVoxG_CNI,7206
 s3i/directory.py,sha256=taOw4SrxIwzoDEBUMP_nsr57COi_LMtGG0Tkb6ozDb0,3028
 s3i/ditto_manager.py,sha256=tskSKozUZ6UMdtofj5zqWVTZQxATvShnv9g79XjrDos,5324
-s3i/event_system.py,sha256=hnIS5u2YfFol_wWoRM8IYEClkybQ18B-4nBF7tanJdo,14678
+s3i/event_system.py,sha256=I24OmyaKcHhYbgXEkflJLdxEW9KarYDfBk6IABKDKyI,14682
 s3i/exception.py,sha256=IgVQudVbCkSGe3Z_q2JMXMeF2blM0LpmVfXBYtdvBPk,15645
-s3i/identity_provider.py,sha256=O0QZXz1fVNNMJCH55lQ7Idz86BeRLiKTuwk_He4Ca24,12097
+s3i/identity_provider.py,sha256=q_DW5zhnmvydnuOGmT4nEqt6QM5iCEN67_-Q1Acfr18,2361
 s3i/key_pgp.py,sha256=1th7SmiLm7oQN5Qn-du8P3i24dvLvlFEFfPaHUH626c,4567
 s3i/logger.py,sha256=BjGtlc2_H_LfN9zH0q-I4lIilxglgUdXSkZHv3bk0r0,1008
 s3i/repository.py,sha256=SthJ_f55pl80USWr8aZnc6LB52igit4AfG6CbALVjpg,455
 s3i/tools.py,sha256=49mtYksygu_hqrwcKw_jJdcwwXHAfD662yrHAD4sq3w,1110
-s3i-0.6.8.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
-s3i-0.6.8.dist-info/METADATA,sha256=06csvwpbtcCvcDmcci3N_BumXD7aftrQBG0OMCuyRq0,1360
-s3i-0.6.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-s3i-0.6.8.dist-info/top_level.txt,sha256=_pR0bxLAE-quxyeIgilf0DVoaG-R7RpQlVArNNVes2I,4
-s3i-0.6.8.dist-info/RECORD,,
+s3i-0.7.0.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
+s3i-0.7.0.dist-info/METADATA,sha256=n6v4H444v9VdgzW4DKPjGDcpgQM9oeyT6NY5kKtiRP4,1469
+s3i-0.7.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+s3i-0.7.0.dist-info/top_level.txt,sha256=_pR0bxLAE-quxyeIgilf0DVoaG-R7RpQlVArNNVes2I,4
+s3i-0.7.0.dist-info/RECORD,,
```

