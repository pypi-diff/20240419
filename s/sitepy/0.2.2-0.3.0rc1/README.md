# Comparing `tmp/sitepy-0.2.2.tar.gz` & `tmp/sitepy-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.2.2.tar", last modified: Thu Apr 18 22:21:07 2024, max compression
+gzip compressed data, was "sitepy-0.3.0rc1.tar", last modified: Thu Apr 18 23:00:17 2024, max compression
```

## Comparing `sitepy-0.2.2.tar` & `sitepy-0.3.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 22:21:07.040802 sitepy-0.2.2/
--rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     1810 2024-04-18 22:21:07.039802 sitepy-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 22:21:07.041802 sitepy-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-04-18 22:20:58.000000 sitepy-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 22:21:07.026798 sitepy-0.2.2/sitepy/
--rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.2.2/sitepy/__init__.py
--rw-rw-rw-   0        0        0    11681 2024-04-18 22:20:30.000000 sitepy-0.2.2/sitepy/core.py
--rw-rw-rw-   0        0        0      250 2024-04-18 20:08:02.000000 sitepy-0.2.2/sitepy/gpt.py
--rw-rw-rw-   0        0        0    28927 2024-04-18 21:14:00.000000 sitepy-0.2.2/sitepy/profanity.py
--rw-rw-rw-   0        0        0      343 2024-04-18 20:45:59.000000 sitepy-0.2.2/sitepy/recaptcha.py
-drwxrwxrwx   0        0        0        0 2024-04-18 22:21:07.037801 sitepy-0.2.2/sitepy.egg-info/
--rw-rw-rw-   0        0        0     1810 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 23:00:17.402061 sitepy-0.3.0rc1/
+-rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.3.0rc1/LICENSE
+-rw-rw-rw-   0        0        0     1813 2024-04-18 23:00:17.401061 sitepy-0.3.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.3.0rc1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 23:00:17.402061 sitepy-0.3.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-04-18 22:58:11.000000 sitepy-0.3.0rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:00:17.387058 sitepy-0.3.0rc1/sitepy/
+-rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.3.0rc1/sitepy/__init__.py
+-rw-rw-rw-   0        0        0    11932 2024-04-18 22:57:43.000000 sitepy-0.3.0rc1/sitepy/core.py
+-rw-rw-rw-   0        0        0      236 2024-04-18 22:58:21.000000 sitepy-0.3.0rc1/sitepy/gpt.py
+-rw-rw-rw-   0        0        0    28925 2024-04-18 22:58:26.000000 sitepy-0.3.0rc1/sitepy/profanity.py
+-rw-rw-rw-   0        0        0      318 2024-04-18 22:59:08.000000 sitepy-0.3.0rc1/sitepy/recaptcha.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:00:17.398061 sitepy-0.3.0rc1/sitepy.egg-info/
+-rw-rw-rw-   0        0        0     1813 2024-04-18 23:00:16.000000 sitepy-0.3.0rc1/sitepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-18 23:00:17.000000 sitepy-0.3.0rc1/sitepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 23:00:16.000000 sitepy-0.3.0rc1/sitepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 23:00:16.000000 sitepy-0.3.0rc1/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.2.2/LICENSE` & `sitepy-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sitepy-0.2.2/PKG-INFO` & `sitepy-0.3.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.2.2
+Version: 0.3.0rc1
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sitepy-0.2.2/README.md` & `sitepy-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `sitepy-0.2.2/setup.py` & `sitepy-0.3.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.2.2',
+    version='0.3.0-pre1',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     license='Apache 2.0',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
```

### Comparing `sitepy-0.2.2/sitepy/core.py` & `sitepy-0.3.0rc1/sitepy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,15 +341,19 @@
 </body>
 </html>
 """
 
 
 class SitePy:
     def __init__(
-        self, static_dir="static", templates_dir="templates", custom_404_page=None, custom_500_page=None
+        self,
+        static_dir="static",
+        templates_dir="templates",
+        custom_404_page=None,
+        custom_500_page=None,
     ):
         self.routes = {}
         self.middleware = [self.logger_middleware]
         self.static_dir = static_dir
         self.templates_dir = templates_dir
         self.custom_404_page = custom_404_page
         self.custom_500_page = custom_500_page
@@ -379,24 +383,28 @@
         try:
             path = environ["PATH_INFO"]
             method = environ["REQUEST_METHOD"]
             for middleware in self.middleware:
                 middleware(environ)
             handler = None
             for route, methods in self.routes.keys():
-                if path == route and method in methods:
+                match = route.match(path)
+                if match and method in methods:
                     handler = self.routes[(route, methods)]
+                    params = match.groupdict()
                     break
             if handler:
                 try:
                     request_body_size = int(environ.get("CONTENT_LENGTH", 0))
                 except ValueError:
                     request_body_size = 0
                 request_body = environ["wsgi.input"].read(request_body_size)
+                body_params = parse_qs(request_body.decode()) if request_body else {}
                 params = parse_qs(request_body.decode()) if request_body else {}
+                params.update(body_params)
                 handler_args = inspect.signature(handler).parameters
                 response_body = handler(params) if handler_args else handler()
                 status = "200 OK"
                 headers = [("Content-type", "text/html")]
                 start_response(status, headers)
                 return [response_body.encode()]
             elif path.startswith("/" + self.static_dir):
```

#### html2text {}

```diff
@@ -9,36 +9,38 @@
 """ f00 = """
 **** IInntteerrnnaall SSeerrvveerr eerrrroorr !! ****
 ************ 55 ************
 ************ 0000 ************
 We're unable to find out what's happening! We suggest you to
 _G_o_ _H_o_m_e or visit here later. Credits to _A_M_A_N_ _(_@_a_d_s_i_n_g_h_1_4_)_!
 """ class SitePy: def __init__( self, static_dir="static",
-templates_dir="templates", custom_404_page=None, custom_500_page=None ):
+templates_dir="templates", custom_404_page=None, custom_500_page=None, ):
 self.routes = {} self.middleware = [self.logger_middleware] self.static_dir =
 static_dir self.templates_dir = templates_dir self.custom_404_page =
 custom_404_page self.custom_500_page = custom_500_page def render_template
 (self, template_name, context={}): template_path = os.path.join
 (self.templates_dir, template_name) with open(template_path, "r") as f:
 template = f.read() for key, value in context.items(): template =
 template.replace(f"{{{{ {key} }}}}", value) return template def route(self,
 path, methods=["GET"]): def wrapper(handler): self.routes[(path, tuple
 (methods))] = handler return handler return wrapper def use(self, middleware):
 self.middleware.append(middleware) def logger_middleware(self, environ): print
 (f"Request received for {environ['PATH_INFO']}") def __call__(self, environ,
 start_response): try: path = environ["PATH_INFO"] method = environ
 ["REQUEST_METHOD"] for middleware in self.middleware: middleware(environ)
-handler = None for route, methods in self.routes.keys(): if path == route and
-method in methods: handler = self.routes[(route, methods)] break if handler:
-try: request_body_size = int(environ.get("CONTENT_LENGTH", 0)) except
-ValueError: request_body_size = 0 request_body = environ["wsgi.input"].read
-(request_body_size) params = parse_qs(request_body.decode()) if request_body
-else {} handler_args = inspect.signature(handler).parameters response_body =
-handler(params) if handler_args else handler() status = "200 OK" headers = [
-("Content-type", "text/html")] start_response(status, headers) return
+handler = None for route, methods in self.routes.keys(): match = route.match
+(path) if match and method in methods: handler = self.routes[(route, methods)]
+params = match.groupdict() break if handler: try: request_body_size = int
+(environ.get("CONTENT_LENGTH", 0)) except ValueError: request_body_size = 0
+request_body = environ["wsgi.input"].read(request_body_size) body_params =
+parse_qs(request_body.decode()) if request_body else {} params = parse_qs
+(request_body.decode()) if request_body else {} params.update(body_params)
+handler_args = inspect.signature(handler).parameters response_body = handler
+(params) if handler_args else handler() status = "200 OK" headers = [("Content-
+type", "text/html")] start_response(status, headers) return
 [response_body.encode()] elif path.startswith("/" + self.static_dir): try: with
 open(path[1:], "rb") as f: response_body = f.read() status = "200 OK" headers =
 [("Content-type", "application/octet-stream")] start_response(status, headers)
 return [response_body] except FileNotFoundError: status = "404 NOT FOUND"
 headers = [("Content-type", "text/html")] start_response(status, headers)
 return [ ( self.custom_404_page.encode() if self.custom_404_page else
 fof.encode() ) ] else: status = "404 NOT FOUND" headers = [("Content-type",
```

### Comparing `sitepy-0.2.2/sitepy/profanity.py` & `sitepy-0.3.0rc1/sitepy/profanity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1729,15 +1729,14 @@
     "yellow showers",
     "yid",
     "yiffy",
     "yobbo",
     "zoophile",
     "zoophilia",
     "zubb",
-
 ]
 
 
 def check_profanity(text):
     # Check for profane phrases
     for phrase in custom_profanity_words:
         if phrase.lower() in text.lower().split():
```

### Comparing `sitepy-0.2.2/sitepy.egg-info/PKG-INFO` & `sitepy-0.3.0rc1/sitepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.2.2
+Version: 0.3.0rc1
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

