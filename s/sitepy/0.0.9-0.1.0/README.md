# Comparing `tmp/sitepy-0.0.9.tar.gz` & `tmp/sitepy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.0.9.tar", last modified: Thu Apr 18 18:57:05 2024, max compression
+gzip compressed data, was "sitepy-0.1.0.tar", last modified: Thu Apr 18 21:21:52 2024, max compression
```

## Comparing `sitepy-0.0.9.tar` & `sitepy-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:05.166716 sitepy-0.0.9/
--rw-rw-rw-   0        0        0     1787 2024-04-18 18:57:05.157631 sitepy-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      913 2024-04-17 20:28:24.000000 sitepy-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 18:57:05.167813 sitepy-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-04-18 18:56:36.000000 sitepy-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:05.032173 sitepy-0.0.9/sitepy/
--rw-rw-rw-   0        0        0      130 2024-04-18 18:55:57.000000 sitepy-0.0.9/sitepy/__init__.py
--rw-rw-rw-   0        0        0     3274 2024-04-18 01:58:35.000000 sitepy-0.0.9/sitepy/sitepy.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:05.155028 sitepy-0.0.9/sitepy.egg-info/
--rw-rw-rw-   0        0        0     1787 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 18:57:04.000000 sitepy-0.0.9/sitepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 21:21:52.889144 sitepy-0.1.0/
+-rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1810 2024-04-18 21:21:52.888144 sitepy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 21:21:52.890145 sitepy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-04-18 21:21:44.000000 sitepy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 21:21:52.872139 sitepy-0.1.0/sitepy/
+-rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.1.0/sitepy/__init__.py
+-rw-rw-rw-   0        0        0     3540 2024-04-18 21:20:39.000000 sitepy-0.1.0/sitepy/core.py
+-rw-rw-rw-   0        0        0      250 2024-04-18 20:08:02.000000 sitepy-0.1.0/sitepy/gpt.py
+-rw-rw-rw-   0        0        0    28927 2024-04-18 21:14:00.000000 sitepy-0.1.0/sitepy/profanity.py
+-rw-rw-rw-   0        0        0      343 2024-04-18 20:45:59.000000 sitepy-0.1.0/sitepy/recaptcha.py
+drwxrwxrwx   0        0        0        0 2024-04-18 21:21:52.884143 sitepy-0.1.0/sitepy.egg-info/
+-rw-rw-rw-   0        0        0     1810 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.0.9/PKG-INFO` & `sitepy-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # sitepy
 
 A simple web framework for Python.
 
 ## Installation
```

### Comparing `sitepy-0.0.9/README.md` & `sitepy-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 - Static file serving: Files in the static directory are served at /static.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
-[Apache](LICENSE)
+[Apache](sitepy/LICENSE)
```

### Comparing `sitepy-0.0.9/setup.py` & `sitepy-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.0.9',
+    version='0.1.0',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     license='Apache 2.0',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
```

### Comparing `sitepy-0.0.9/sitepy/sitepy.py` & `sitepy-0.1.0/sitepy/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,54 +27,57 @@
     def use(self, middleware):
         self.middleware.append(middleware)
 
     def logger_middleware(self, environ):
         print(f"Request received for {environ['PATH_INFO']}")
 
     def __call__(self, environ, start_response):
-        path = environ['PATH_INFO']
-        method = environ['REQUEST_METHOD']
-        for middleware in self.middleware:
-            middleware(environ)
-        handler = None
-        for route, methods in self.routes.keys():
-            if path == route and method in methods:
-                handler = self.routes[(route, methods)]
-                break
-        if handler:
-            try:
-                request_body_size = int(environ.get('CONTENT_LENGTH', 0))
-            except ValueError:
-                request_body_size = 0
-            request_body = environ['wsgi.input'].read(request_body_size)
-            params = parse_qs(request_body) if request_body else {}
-            handler_args = inspect.signature(handler).parameters
-            response_body = handler(params) if handler_args else handler()
-            status = '200 OK'
-            headers = [('Content-type', 'text/html')]
-            start_response(status, headers)
-            return [response_body.encode()]
-        elif path.startswith('/' + self.static_dir):
-            try:
-                with open(path[1:], 'rb') as f:
-                    response_body = f.read()
+        try:
+            path = environ['PATH_INFO']
+            method = environ['REQUEST_METHOD']
+            for middleware in self.middleware:
+                middleware(environ)
+            handler = None
+            for route, methods in self.routes.keys():
+                if path == route and method in methods:
+                    handler = self.routes[(route, methods)]
+                    break
+            if handler:
+                try:
+                    request_body_size = int(environ.get('CONTENT_LENGTH', 0))
+                except ValueError:
+                    request_body_size = 0
+                request_body = environ['wsgi.input'].read(request_body_size)
+                params = parse_qs(request_body.decode()) if request_body else {}
+                handler_args = inspect.signature(handler).parameters
+                response_body = handler(params) if handler_args else handler()
                 status = '200 OK'
-                headers = [('Content-type', 'application/octet-stream')]
+                headers = [('Content-type', 'text/html')]
                 start_response(status, headers)
-                return [response_body]
-            except FileNotFoundError:
+                return [response_body.encode()]
+            elif path.startswith('/' + self.static_dir):
+                try:
+                    with open(path[1:], 'rb') as f:
+                        response_body = f.read()
+                    status = '200 OK'
+                    headers = [('Content-type', 'application/octet-stream')]
+                    start_response(status, headers)
+                    return [response_body]
+                except FileNotFoundError:
+                    status = '404 NOT FOUND'
+                    headers = [('Content-type', 'text/html')]
+                    start_response(status, headers)
+                    return ['File not found'.encode()]
+            else:
                 status = '404 NOT FOUND'
                 headers = [('Content-type', 'text/html')]
                 start_response(status, headers)
-                return ['File not found'.encode()]
-        else:
-            status = '404 NOT FOUND'
-            headers = [('Content-type', 'text/html')]
-            start_response(status, headers)
-            return ['Route not found'.encode()]
+                return ['Route not found'.encode()]
+        except KeyboardInterrupt:
+            print('\nServer shutting down...')
 
     def run(self, host='localhost', port=8080):
         try:
             server = make_server(host, port, self)
             print(f'Serving on {host}:{port}')
             server.serve_forever()
         except KeyboardInterrupt:
```

### Comparing `sitepy-0.0.9/sitepy.egg-info/PKG-INFO` & `sitepy-0.1.0/sitepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # sitepy
 
 A simple web framework for Python.
 
 ## Installation
```

