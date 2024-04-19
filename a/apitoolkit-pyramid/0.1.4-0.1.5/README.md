# Comparing `tmp/apitoolkit-pyramid-0.1.4.tar.gz` & `tmp/apitoolkit-pyramid-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apitoolkit-pyramid-0.1.4.tar", last modified: Mon Apr 15 10:53:27 2024, max compression
+gzip compressed data, was "apitoolkit-pyramid-0.1.5.tar", last modified: Fri Apr 19 14:55:23 2024, max compression
```

## Comparing `apitoolkit-pyramid-0.1.4.tar` & `apitoolkit-pyramid-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     1067 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.1.4/LICENSE
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     5739 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/PKG-INFO
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     5504 2024-04-03 08:44:57.000000 apitoolkit-pyramid-0.1.4/README.md
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-15 10:53:27.704083 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6419 2024-04-15 10:52:15.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid/__init__.py
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     5739 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      266 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)        1 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       84 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/requires.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       19 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       38 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/setup.cfg
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      634 2024-04-15 10:52:35.000000 apitoolkit-pyramid-0.1.4/setup.py
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-19 14:55:23.763910 apitoolkit-pyramid-0.1.5/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     1067 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.1.5/LICENSE
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6294 2024-04-19 14:55:23.763910 apitoolkit-pyramid-0.1.5/PKG-INFO
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6059 2024-04-19 14:13:52.000000 apitoolkit-pyramid-0.1.5/README.md
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-19 14:55:23.743909 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     7591 2024-04-19 14:53:50.000000 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid/__init__.py
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-19 14:55:23.759910 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid.egg-info/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6294 2024-04-19 14:55:23.000000 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      266 2024-04-19 14:55:23.000000 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)        1 2024-04-19 14:55:23.000000 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       84 2024-04-19 14:55:23.000000 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       19 2024-04-19 14:55:23.000000 apitoolkit-pyramid-0.1.5/apitoolkit_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       38 2024-04-19 14:55:23.763910 apitoolkit-pyramid-0.1.5/setup.cfg
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      634 2024-04-19 14:55:19.000000 apitoolkit-pyramid-0.1.5/setup.py
```

### Comparing `apitoolkit-pyramid-0.1.4/LICENSE` & `apitoolkit-pyramid-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apitoolkit-pyramid-0.1.4/PKG-INFO` & `apitoolkit-pyramid-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apitoolkit-pyramid
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python Pyramid SDK for Apitoolkit integration
 Author: APIToolkit
 Author-email: hello@apitoolkit.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # API Toolkit Python Pyramid SDK
@@ -19,14 +19,20 @@
 
 Add your APIToolkit API key `APITOOLKIT_KEY` to your `development.ini` or `production.ini` files or in your settings:
 
 ```python
 APITOOLKIT_KEY = "<YOUR_API_KEY>"
 ```
 
+When using ini files separate mulitple values with comma.
+
+```ini
+APITOOLKIT_REDACT_HEADERS = X-Secret1,X-Secret2
+```
+
 Then add apitoolkit pyramid tween in your server's config:
 
 ```python
 from wsgiref.simple_server import make_server
 from pyramid.config import Configurator
 from pyramid.response import Response
 from pyramid.view import view_config
@@ -59,14 +65,15 @@
 ### Configuration Parameters
 
 APITOOLKIT_KEY: `required` API key for accessing the APIToolkit service.
 APITOOLKIT_REDACT_HEADERS: `optional` List of headers to redact in captured requests.
 APITOOLKIT_DEBUG: `optional` Flag to enable debug mode.
 APITOOLKIT_REDACT_REQ_BODY: `optional` List of fields to redact in request bodies.
 APITOOLKIT_REDACT_RES_BODY: `optional` List of fields to redact in response bodies.
+APITOOLKIT_ROUTES_WHITELIST: `optional` List of routes prefixes that should be captured.
 APITOOLKIT_SERVICE_VERSION: `optional` Version of the service (helps in monitoring different versions of your deployments).
 APITOOLKIT_TAGS: `optional` Tags associated with the service.
 
 ## Client Redacting fields
 
 The SDK provides a way for customers to redact senstive fields from data it sends to APIToolkit servers, redacting means that those fields would never leave your servers at all. So you feel safer that your sensitive data only stays on your servers.
 
@@ -87,14 +94,26 @@
 the `APITOOLKIT_REDACT_REQ_BODY` and `APITOOLKIT_REDACT_RES_BODY` expects a list of JSONPath strings as arguments.
 
 The choice of JSONPath was selected to allow you have great flexibility in descibing which fields within your responses are sensitive.
 Also note that these list of items to be redacted will be aplied to all endpoint requests and responses on your server.
 To learn more about jsonpath to help form your queries, please take a look at this cheatsheet:
 [https://lzone.de/cheat-sheet/JSONPath](https://lzone.de/cheat-sheet/JSONPath)
 
+## Routes Whitelist
+
+If you only want to capture specific app routes you can configure prefixes that need be matched.
+
+```python
+settings = {
+"APITOOLKIT_ROUTES_WHITELIST": ["/api/first", "/api/second"],
+}
+```
+
+This will only capture requests that are incoming to your app with these prefixes, e.a. `/api/first/customer/1` but not `/api/health`.
+
 ## Debugging
 
 You can add `APITOOLKIT_DEBUG` to your app's settings and set it to `True` to enable debug logging from the SDK. This will print out logs for each request/response captured by the tween. APITOOLKIT_DEBUG defaults to `False`.
 
 # Outgoing Requests
 
 To monitor outgoing HTTP requests from your Pyramid application, you can use the `observe_request` function from the `apitoolkit_pyramid` module. This allows you to capture and send copies of all outgoing requests to an apitoolkit server for monitoring and analysis. All outgoing request are associated with the incoming request that trigger them.
```

### Comparing `apitoolkit-pyramid-0.1.4/README.md` & `apitoolkit-pyramid-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 Add your APIToolkit API key `APITOOLKIT_KEY` to your `development.ini` or `production.ini` files or in your settings:
 
 ```python
 APITOOLKIT_KEY = "<YOUR_API_KEY>"
 ```
 
+When using ini files separate mulitple values with comma.
+
+```ini
+APITOOLKIT_REDACT_HEADERS = X-Secret1,X-Secret2
+```
+
 Then add apitoolkit pyramid tween in your server's config:
 
 ```python
 from wsgiref.simple_server import make_server
 from pyramid.config import Configurator
 from pyramid.response import Response
 from pyramid.view import view_config
@@ -50,14 +56,15 @@
 ### Configuration Parameters
 
 APITOOLKIT_KEY: `required` API key for accessing the APIToolkit service.
 APITOOLKIT_REDACT_HEADERS: `optional` List of headers to redact in captured requests.
 APITOOLKIT_DEBUG: `optional` Flag to enable debug mode.
 APITOOLKIT_REDACT_REQ_BODY: `optional` List of fields to redact in request bodies.
 APITOOLKIT_REDACT_RES_BODY: `optional` List of fields to redact in response bodies.
+APITOOLKIT_ROUTES_WHITELIST: `optional` List of routes prefixes that should be captured.
 APITOOLKIT_SERVICE_VERSION: `optional` Version of the service (helps in monitoring different versions of your deployments).
 APITOOLKIT_TAGS: `optional` Tags associated with the service.
 
 ## Client Redacting fields
 
 The SDK provides a way for customers to redact senstive fields from data it sends to APIToolkit servers, redacting means that those fields would never leave your servers at all. So you feel safer that your sensitive data only stays on your servers.
 
@@ -78,14 +85,26 @@
 the `APITOOLKIT_REDACT_REQ_BODY` and `APITOOLKIT_REDACT_RES_BODY` expects a list of JSONPath strings as arguments.
 
 The choice of JSONPath was selected to allow you have great flexibility in descibing which fields within your responses are sensitive.
 Also note that these list of items to be redacted will be aplied to all endpoint requests and responses on your server.
 To learn more about jsonpath to help form your queries, please take a look at this cheatsheet:
 [https://lzone.de/cheat-sheet/JSONPath](https://lzone.de/cheat-sheet/JSONPath)
 
+## Routes Whitelist
+
+If you only want to capture specific app routes you can configure prefixes that need be matched.
+
+```python
+settings = {
+"APITOOLKIT_ROUTES_WHITELIST": ["/api/first", "/api/second"],
+}
+```
+
+This will only capture requests that are incoming to your app with these prefixes, e.a. `/api/first/customer/1` but not `/api/health`.
+
 ## Debugging
 
 You can add `APITOOLKIT_DEBUG` to your app's settings and set it to `True` to enable debug logging from the SDK. This will print out logs for each request/response captured by the tween. APITOOLKIT_DEBUG defaults to `False`.
 
 # Outgoing Requests
 
 To monitor outgoing HTTP requests from your Pyramid application, you can use the `observe_request` function from the `apitoolkit_pyramid` module. This allows you to capture and send copies of all outgoing requests to an apitoolkit server for monitoring and analysis. All outgoing request are associated with the incoming request that trigger them.
```

### Comparing `apitoolkit-pyramid-0.1.4/apitoolkit_pyramid/__init__.py` & `apitoolkit-pyramid-0.1.5/apitoolkit_pyramid/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,72 @@
+import base64
+import json
+import time
 import uuid
+from datetime import datetime
+from urllib.parse import urlsplit
+
+import pytz
 import requests
+from apitoolkit_python import report_error, observe_request
 from google.cloud import pubsub_v1
 from google.oauth2 import service_account
 from jsonpath_ng import parse
-import json
-import base64
-import time
-from datetime import datetime
-import pytz
-from apitoolkit_python import observe_request, report_error
-from urllib.parse import urlsplit
 from pyramid.request import Request
 
+OPTIONAL_SETTINGS = (
+    # var in class, environment name, type, default value
+    ('debug', 'APITOOLKIT_DEBUG', bool, False),
+    ('redact_headers', 'APITOOLKIT_REDACT_HEADERS', list, []),
+    ('redact_request_body', 'APITOOLKIT_REDACT_REQ_BODY', list, []),
+    ('redact_response_body', 'APITOOLKIT_REDACT_RES_BODY', list, []),
+    ('routes_whitelist', 'APITOOLKIT_ROUTES_WHITELIST', list, []),
+    ('service_version', 'APITOOLKIT_SERVICE_VERSION', str, None),
+    ('tags', 'APITOOLKIT_TAGS', list, []),
+)
+
 
 class APIToolkit(object):
     def __init__(self, handler, registry):
         self.publisher = None
         self.topic_name = None
         self.meta = None
-        self.redact_headers = registry.settings.get('APITOOLKIT_REDACT_HEADERS', [])
-        self.debug = registry.settings.get('APITOOLKIT_DEBUG', False)
-        self.redact_request_body = registry.settings.get('APITOOLKIT_REDACT_REQ_BODY', [])
-        self.redact_response_body = registry.settings.get('APITOOLKIT_REDACT_RES_BODY', [])
         self.get_response = handler
 
-        self.service_version = registry.settings.get("APITOOLKIT_SERVICE_VERSION", None)
-        self.tags =registry.settings.get("APITOOLKIT_TAGS", [])
-
         api_key = registry.settings.get('APITOOLKIT_KEY')
         root_url = registry.settings.get('APITOOLKIT_ROOT_URL',
                            "https://app.apitoolkit.io")
 
+        for var_name, env_id, _type, default in OPTIONAL_SETTINGS:
+            self.prepare_optional_settings(var_name, registry.settings.get(env_id), _type, default)
+
         response = requests.get(url=root_url + "/api/client_metadata",
                                 headers={"Authorization": f"Bearer {api_key}"})
         response.raise_for_status()
         data = response.json()
         credentials = service_account.Credentials.from_service_account_info(
             data["pubsub_push_service_account"])
 
         self.publisher = pubsub_v1.PublisherClient(credentials=credentials)
         self.topic_name = 'projects/{project_id}/topics/{topic}'.format(
             project_id=data['pubsub_project_id'],
             topic=data['topic_id'],
         )
         self.meta = data
 
+    def prepare_optional_settings(self, var_name, value, _type, default):
+        if _type in (bool, str):
+            setattr(self, var_name, value or default)
+        elif _type is list:
+            # env value can directly be a list or when given via ini file a comma separated string
+            try:
+                setattr(self, var_name, value.split(','))
+            except AttributeError:
+                setattr(self, var_name, value or [])
+
     def getInfo(self):
         return {"project_id": self.meta["project_id"], "service_version": self.service_version, "tags": self.tags}
 
     def publish_message(self, payload):
         data = json.dumps(payload).encode('utf-8')
         if self.debug:
             print("APIToolkit: publish message")
@@ -80,54 +98,62 @@
     def process_exception(self, request, exception):
         report_error(request,exception)
         pass
 
     def __call__(self, request: Request):
         if self.debug:
             print("APIToolkit: making request")
+
         start_time = time.perf_counter_ns()
-        request_method = request.method
-        raw_url = request.url
-        parsed_url = urlsplit(raw_url)
-        url_path_with_query = parsed_url.path + parsed_url.query
-
-        request_body = None
-        query_params =  {key: value for key, value in request.params.items()}
-        request_headers = self.redact_headers_func(request.headers)
-        content_type = request.headers.get('Content-Type', '')
-
-        if content_type == 'application/json':
-            request_body = request.json_body
-        if content_type == 'text/plain':
-            request_body = request.body.decode('utf-8')
-        if content_type == 'application/x-www-form-urlencoded' or 'multipart/form-data' in content_type:
-            request_body = dict(request.POST.copy())
         request.apitoolkit_message_id = str(uuid.uuid4())
         request.apitoolkit_errors = []
         request.apitoolkit_client = self
 
         response = self.get_response(request)
+        
+        url_path = request.matched_route.pattern if request.matched_route is not None else request.path
+
+        if self.routes_whitelist:
+            # return early when route does not match any of the whitelist routes
+            if not any([url_path.startswith(route) for route in self.routes_whitelist]):
+                return response
 
         if self.debug:
             print("APIToolkit: after request")
-        end_time = time.perf_counter_ns()
-        url_path = request.matched_route.pattern if request.matched_route is not None else request.path
-        path_params = request.matchdict
-        duration = (end_time - start_time)
-        status_code = response.status_code
-        request_body = json.dumps(request_body)
-        response_headers = self.redact_headers_func(response.headers)
-        request_body = self.redact_fields(
-            request_body, self.redact_request_body)
-        response_body = self.redact_fields(
-            response.body, self.redact_response_body)
-        timestamp = datetime.now(pytz.timezone("UTC")).isoformat()
-        message_id = request.apitoolkit_message_id
-        errors = request.apitoolkit_errors
         try:
+            request_method = request.method
+            raw_url = request.url
+            parsed_url = urlsplit(raw_url)
+            url_path_with_query = parsed_url.path + parsed_url.query
+            request_body = None
+            query_params =  {key: value for key, value in request.params.items()}
+            request_headers = self.redact_headers_func(request.headers)
+            content_type = request.headers.get('Content-Type', '')
+
+            if content_type == 'application/json':
+                request_body = request.json_body
+            if content_type == 'text/plain':
+                request_body = request.body.decode('utf-8')
+            if content_type == 'application/x-www-form-urlencoded' or 'multipart/form-data' in content_type:
+                request_body = dict(request.POST.copy())
+            
+            end_time = time.perf_counter_ns()
+            url_path = request.matched_route.pattern if request.matched_route is not None else request.path
+            path_params = request.matchdict
+            duration = (end_time - start_time)
+            status_code = response.status_code
+            request_body = json.dumps(request_body)
+            response_headers = self.redact_headers_func(response.headers)
+            request_body = self.redact_fields(
+                request_body, self.redact_request_body)
+            response_body = self.redact_fields(
+                response.body, self.redact_response_body)
+            timestamp = datetime.now(pytz.timezone("UTC")).isoformat()
+            message_id = request.apitoolkit_message_id
+            errors = request.apitoolkit_errors
             payload = {
                 "query_params": query_params,
                 "path_params": path_params,
                 "request_headers": request_headers,
                 "response_headers": response_headers,
                 "proto_minor": 1,
                 "proto_major": 1,
@@ -145,11 +171,13 @@
                 "msg_id": message_id,
                 "parent_id": None,
                 "duration": duration,
                 "service_version": self.service_version,
                 "tags": self.tags,
                 "timestamp": timestamp
             }
+            if self.debug: 
+                print(payload)
             self.publish_message(payload)
         except Exception as e:
             return response
         return response
```

### Comparing `apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/PKG-INFO` & `apitoolkit-pyramid-0.1.5/apitoolkit_pyramid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apitoolkit-pyramid
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python Pyramid SDK for Apitoolkit integration
 Author: APIToolkit
 Author-email: hello@apitoolkit.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # API Toolkit Python Pyramid SDK
@@ -19,14 +19,20 @@
 
 Add your APIToolkit API key `APITOOLKIT_KEY` to your `development.ini` or `production.ini` files or in your settings:
 
 ```python
 APITOOLKIT_KEY = "<YOUR_API_KEY>"
 ```
 
+When using ini files separate mulitple values with comma.
+
+```ini
+APITOOLKIT_REDACT_HEADERS = X-Secret1,X-Secret2
+```
+
 Then add apitoolkit pyramid tween in your server's config:
 
 ```python
 from wsgiref.simple_server import make_server
 from pyramid.config import Configurator
 from pyramid.response import Response
 from pyramid.view import view_config
@@ -59,14 +65,15 @@
 ### Configuration Parameters
 
 APITOOLKIT_KEY: `required` API key for accessing the APIToolkit service.
 APITOOLKIT_REDACT_HEADERS: `optional` List of headers to redact in captured requests.
 APITOOLKIT_DEBUG: `optional` Flag to enable debug mode.
 APITOOLKIT_REDACT_REQ_BODY: `optional` List of fields to redact in request bodies.
 APITOOLKIT_REDACT_RES_BODY: `optional` List of fields to redact in response bodies.
+APITOOLKIT_ROUTES_WHITELIST: `optional` List of routes prefixes that should be captured.
 APITOOLKIT_SERVICE_VERSION: `optional` Version of the service (helps in monitoring different versions of your deployments).
 APITOOLKIT_TAGS: `optional` Tags associated with the service.
 
 ## Client Redacting fields
 
 The SDK provides a way for customers to redact senstive fields from data it sends to APIToolkit servers, redacting means that those fields would never leave your servers at all. So you feel safer that your sensitive data only stays on your servers.
 
@@ -87,14 +94,26 @@
 the `APITOOLKIT_REDACT_REQ_BODY` and `APITOOLKIT_REDACT_RES_BODY` expects a list of JSONPath strings as arguments.
 
 The choice of JSONPath was selected to allow you have great flexibility in descibing which fields within your responses are sensitive.
 Also note that these list of items to be redacted will be aplied to all endpoint requests and responses on your server.
 To learn more about jsonpath to help form your queries, please take a look at this cheatsheet:
 [https://lzone.de/cheat-sheet/JSONPath](https://lzone.de/cheat-sheet/JSONPath)
 
+## Routes Whitelist
+
+If you only want to capture specific app routes you can configure prefixes that need be matched.
+
+```python
+settings = {
+"APITOOLKIT_ROUTES_WHITELIST": ["/api/first", "/api/second"],
+}
+```
+
+This will only capture requests that are incoming to your app with these prefixes, e.a. `/api/first/customer/1` but not `/api/health`.
+
 ## Debugging
 
 You can add `APITOOLKIT_DEBUG` to your app's settings and set it to `True` to enable debug logging from the SDK. This will print out logs for each request/response captured by the tween. APITOOLKIT_DEBUG defaults to `False`.
 
 # Outgoing Requests
 
 To monitor outgoing HTTP requests from your Pyramid application, you can use the `observe_request` function from the `apitoolkit_pyramid` module. This allows you to capture and send copies of all outgoing requests to an apitoolkit server for monitoring and analysis. All outgoing request are associated with the incoming request that trigger them.
```

### Comparing `apitoolkit-pyramid-0.1.4/setup.py` & `apitoolkit-pyramid-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="apitoolkit-pyramid",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     description='A Python Pyramid SDK for Apitoolkit integration',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='hello@apitoolkit.io',
     author='APIToolkit',
     install_requires=[
```

