# Comparing `tmp/sitepy-0.2.1.tar.gz` & `tmp/sitepy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.2.1.tar", last modified: Thu Apr 18 22:10:54 2024, max compression
+gzip compressed data, was "sitepy-0.2.2.tar", last modified: Thu Apr 18 22:21:07 2024, max compression
```

## Comparing `sitepy-0.2.1.tar` & `sitepy-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 22:10:54.257706 sitepy-0.2.1/
--rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1810 2024-04-18 22:10:54.256706 sitepy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 22:10:54.258710 sitepy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-04-18 22:10:49.000000 sitepy-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 22:10:54.241702 sitepy-0.2.1/sitepy/
--rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.2.1/sitepy/__init__.py
--rw-rw-rw-   0        0        0    11691 2024-04-18 22:10:25.000000 sitepy-0.2.1/sitepy/core.py
--rw-rw-rw-   0        0        0      250 2024-04-18 20:08:02.000000 sitepy-0.2.1/sitepy/gpt.py
--rw-rw-rw-   0        0        0    28927 2024-04-18 21:14:00.000000 sitepy-0.2.1/sitepy/profanity.py
--rw-rw-rw-   0        0        0      343 2024-04-18 20:45:59.000000 sitepy-0.2.1/sitepy/recaptcha.py
-drwxrwxrwx   0        0        0        0 2024-04-18 22:10:54.254705 sitepy-0.2.1/sitepy.egg-info/
--rw-rw-rw-   0        0        0     1810 2024-04-18 22:10:53.000000 sitepy-0.2.1/sitepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-18 22:10:53.000000 sitepy-0.2.1/sitepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 22:10:53.000000 sitepy-0.2.1/sitepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 22:10:53.000000 sitepy-0.2.1/sitepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 22:21:07.040802 sitepy-0.2.2/
+-rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1810 2024-04-18 22:21:07.039802 sitepy-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 22:21:07.041802 sitepy-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-04-18 22:20:58.000000 sitepy-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:21:07.026798 sitepy-0.2.2/sitepy/
+-rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.2.2/sitepy/__init__.py
+-rw-rw-rw-   0        0        0    11681 2024-04-18 22:20:30.000000 sitepy-0.2.2/sitepy/core.py
+-rw-rw-rw-   0        0        0      250 2024-04-18 20:08:02.000000 sitepy-0.2.2/sitepy/gpt.py
+-rw-rw-rw-   0        0        0    28927 2024-04-18 21:14:00.000000 sitepy-0.2.2/sitepy/profanity.py
+-rw-rw-rw-   0        0        0      343 2024-04-18 20:45:59.000000 sitepy-0.2.2/sitepy/recaptcha.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:21:07.037801 sitepy-0.2.2/sitepy.egg-info/
+-rw-rw-rw-   0        0        0     1810 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 22:21:06.000000 sitepy-0.2.2/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.2.1/LICENSE` & `sitepy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sitepy-0.2.1/PKG-INFO` & `sitepy-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sitepy-0.2.1/README.md` & `sitepy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sitepy-0.2.1/setup.py` & `sitepy-0.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.2.1',
+    version='0.2.2',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     license='Apache 2.0',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
```

### Comparing `sitepy-0.2.1/sitepy/core.py` & `sitepy-0.2.2/sitepy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,18 +333,15 @@
 			<span></span><span></span>
 			<span></span><span></span>
 			<span></span>
 		</div>
     <p> We're unable to find out what's happening! We suggest you to
 			<br/>
 			<a href="/">Go Home</a>
-			or visit here later.</p>
-    <br>
-    <br>
-    <p>Credits to <a href='https://codepen.io/adsingh14' target="_blank">AMAN (@adsingh14)!</a></p>
+			or visit here later. Credits to <a href='https://codepen.io/adsingh14' target="_blank">AMAN (@adsingh14)!</a></p>
 </body>
 </html>
 """
 
 
 class SitePy:
     def __init__(
@@ -434,14 +431,15 @@
                 ]
         except KeyboardInterrupt:
             print("\nServer shutting down...")
         except Exception as e:
             status = "500 INTERNAL SERVER ERROR"
             headers = [("Content-type", "text/html")]
             start_response(status, headers)
+            print(e)
             return [
                 (
                     self.custom_500_page.encode()
                     if self.custom_500_page
                     else f00.encode()
                 )
             ]
```

#### html2text {}

```diff
@@ -7,18 +7,15 @@
 Good luck.
 Credits to _R_i_t_h_i_k_ _S_a_m_a_n_t_h_u_l_a_ _(_@_c_o_d_e_2_r_i_t_h_i_k_)_!
 """ f00 = """
 **** IInntteerrnnaall SSeerrvveerr eerrrroorr !! ****
 ************ 55 ************
 ************ 0000 ************
 We're unable to find out what's happening! We suggest you to
-_G_o_ _H_o_m_e or visit here later.
-
-
-Credits to _A_M_A_N_ _(_@_a_d_s_i_n_g_h_1_4_)_!
+_G_o_ _H_o_m_e or visit here later. Credits to _A_M_A_N_ _(_@_a_d_s_i_n_g_h_1_4_)_!
 """ class SitePy: def __init__( self, static_dir="static",
 templates_dir="templates", custom_404_page=None, custom_500_page=None ):
 self.routes = {} self.middleware = [self.logger_middleware] self.static_dir =
 static_dir self.templates_dir = templates_dir self.custom_404_page =
 custom_404_page self.custom_500_page = custom_500_page def render_template
 (self, template_name, context={}): template_path = os.path.join
 (self.templates_dir, template_name) with open(template_path, "r") as f:
@@ -45,12 +42,12 @@
 headers = [("Content-type", "text/html")] start_response(status, headers)
 return [ ( self.custom_404_page.encode() if self.custom_404_page else
 fof.encode() ) ] else: status = "404 NOT FOUND" headers = [("Content-type",
 "text/html")] start_response(status, headers) return [
 ( self.custom_404_page.encode() if self.custom_404_page else fof.encode() ) ]
 except KeyboardInterrupt: print("\nServer shutting down...") except Exception
 as e: status = "500 INTERNAL SERVER ERROR" headers = [("Content-type", "text/
-html")] start_response(status, headers) return [ ( self.custom_500_page.encode
-() if self.custom_500_page else f00.encode() ) ] def run(self,
-host="localhost", port=8080): try: server = make_server(host, port, self) print
-(f"Serving on {host}:{port}") server.serve_forever() except KeyboardInterrupt:
-print("\nServer shutting down...") server.server_close()
+html")] start_response(status, headers) print(e) return [
+( self.custom_500_page.encode() if self.custom_500_page else f00.encode() ) ]
+def run(self, host="localhost", port=8080): try: server = make_server(host,
+port, self) print(f"Serving on {host}:{port}") server.serve_forever() except
+KeyboardInterrupt: print("\nServer shutting down...") server.server_close()
```

### Comparing `sitepy-0.2.1/sitepy/profanity.py` & `sitepy-0.2.2/sitepy/profanity.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.2.1/sitepy.egg-info/PKG-INFO` & `sitepy-0.2.2/sitepy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

