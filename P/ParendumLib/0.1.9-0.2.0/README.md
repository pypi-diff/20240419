# Comparing `tmp/ParendumLib-0.1.9.tar.gz` & `tmp/ParendumLib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParendumLib-0.1.9.tar", last modified: Mon Apr 15 12:35:18 2024, max compression
+gzip compressed data, was "ParendumLib-0.2.0.tar", last modified: Fri Apr 19 11:09:25 2024, max compression
```

## Comparing `ParendumLib-0.1.9.tar` & `ParendumLib-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/
--rw-rw-rw-   0        0        0      233 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.141933 ParendumLib-0.1.9/ParendumLib.egg-info/
--rw-rw-rw-   0        0        0      233 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1253 2023-12-17 23:21:59.000000 ParendumLib-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.146577 ParendumLib-0.1.9/parendumlib/
--rw-rw-rw-   0        0        0      222 2023-12-27 22:30:57.000000 ParendumLib-0.1.9/parendumlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/parendumlib/database/
--rw-rw-rw-   0        0        0        0 2023-12-27 20:05:10.000000 ParendumLib-0.1.9/parendumlib/database/__init__.py
--rw-rw-rw-   0        0        0     3458 2023-12-27 20:21:09.000000 ParendumLib-0.1.9/parendumlib/database/mongodb.py
--rw-rw-rw-   0        0        0       55 2023-10-10 13:03:24.000000 ParendumLib-0.1.9/parendumlib/exceptions.py
--rw-rw-rw-   0        0        0     5318 2023-12-21 01:19:55.000000 ParendumLib-0.1.9/parendumlib/logger.py
--rw-rw-rw-   0        0        0     4996 2024-04-15 12:30:24.000000 ParendumLib-0.1.9/parendumlib/mailer.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/parendumlib/permissions/
--rw-rw-rw-   0        0        0        0 2023-12-27 22:27:26.000000 ParendumLib-0.1.9/parendumlib/permissions/__init__.py
--rw-rw-rw-   0        0        0     3273 2023-12-27 22:35:03.000000 ParendumLib-0.1.9/parendumlib/permissions/mongodb.py
--rw-rw-rw-   0        0        0     1483 2023-12-27 22:31:06.000000 ParendumLib-0.1.9/parendumlib/responses.py
--rw-rw-rw-   0        0        0     2089 2023-12-28 22:19:08.000000 ParendumLib-0.1.9/parendumlib/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      386 2024-04-15 12:30:32.000000 ParendumLib-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:09:25.065127 ParendumLib-0.2.0/
+-rw-rw-rw-   0        0        0      233 2024-04-19 11:09:25.065127 ParendumLib-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 11:09:25.056743 ParendumLib-0.2.0/ParendumLib.egg-info/
+-rw-rw-rw-   0        0        0      233 2024-04-19 11:09:25.000000 ParendumLib-0.2.0/ParendumLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-19 11:09:25.000000 ParendumLib-0.2.0/ParendumLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:09:25.000000 ParendumLib-0.2.0/ParendumLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2024-04-19 11:09:25.000000 ParendumLib-0.2.0/ParendumLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 11:09:25.000000 ParendumLib-0.2.0/ParendumLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1253 2023-12-17 23:21:59.000000 ParendumLib-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 11:09:25.061770 ParendumLib-0.2.0/parendumlib/
+-rw-rw-rw-   0        0        0      222 2023-12-27 22:30:57.000000 ParendumLib-0.2.0/parendumlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:09:25.063121 ParendumLib-0.2.0/parendumlib/database/
+-rw-rw-rw-   0        0        0        0 2023-12-27 20:05:10.000000 ParendumLib-0.2.0/parendumlib/database/__init__.py
+-rw-rw-rw-   0        0        0     3458 2023-12-27 20:21:09.000000 ParendumLib-0.2.0/parendumlib/database/mongodb.py
+-rw-rw-rw-   0        0        0       55 2023-10-10 13:03:24.000000 ParendumLib-0.2.0/parendumlib/exceptions.py
+-rw-rw-rw-   0        0        0     6215 2024-04-19 11:08:15.000000 ParendumLib-0.2.0/parendumlib/logger.py
+-rw-rw-rw-   0        0        0     4897 2024-04-19 11:02:59.000000 ParendumLib-0.2.0/parendumlib/mailer.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:09:25.064128 ParendumLib-0.2.0/parendumlib/permissions/
+-rw-rw-rw-   0        0        0        0 2023-12-27 22:27:26.000000 ParendumLib-0.2.0/parendumlib/permissions/__init__.py
+-rw-rw-rw-   0        0        0     3273 2023-12-27 22:35:03.000000 ParendumLib-0.2.0/parendumlib/permissions/mongodb.py
+-rw-rw-rw-   0        0        0     1483 2023-12-27 22:31:06.000000 ParendumLib-0.2.0/parendumlib/responses.py
+-rw-rw-rw-   0        0        0     2089 2023-12-28 22:19:08.000000 ParendumLib-0.2.0/parendumlib/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:09:25.065127 ParendumLib-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-04-19 11:09:10.000000 ParendumLib-0.2.0/setup.py
```

### Comparing `ParendumLib-0.1.9/README.md` & `ParendumLib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.9/parendumlib/database/mongodb.py` & `ParendumLib-0.2.0/parendumlib/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.9/parendumlib/logger.py` & `ParendumLib-0.2.0/parendumlib/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             if response.status_code == 200:
                 return response.json()
             return dict(code=response.status_code, error=response.json())
         except Exception as e:
             return dict(code=500, error=str(e))
 
     def _log(self, level: str, function: str, message: str, status_code: int, elapsed_time: int = 1,
-             arguments: list = None, content: dict = None):
+             arguments: list = None, content: dict = None, save: bool = False):
         _new_log = dict(
             function=function,
             message=message,
             level=level.lower(),
             status_code=status_code or 0,
             elapsed_time=elapsed_time
         )
@@ -88,53 +88,65 @@
             _new_log["arguments"] = arguments
         if content:
             _new_log["content"] = content
         if hasattr(self.logger, level):
             getattr(self.logger, level)(f"[{function}] {message}")
         else:
             self.logger.info(f"[{level}:{function}] {message}")
-        self._do_post(f"{self.endpoint}/api/logs/new", _new_log)
+        if save:
+            self._do_post(f"{self.endpoint}/api/logs/new", _new_log)
 
     def _do_log(self, level: str, function: str, message: str, status_code: int, elapsed_time: int = 1,
-                arguments: list = None, content: dict = None):
-        thread = threading.Thread(target=self._log, args=(level, function, message, status_code, elapsed_time, arguments, content, ))
+                arguments: list = None, content: dict = None, save: bool = False):
+        thread = threading.Thread(target=self._log, args=(
+            level, function, message, status_code, elapsed_time, arguments, content, save,
+        ))
         thread.start()
 
-    def debug(self, message: str):
+    def log(self, level: str, message: str, status_code: int = 0, save: bool = False):
         stack = inspect.stack()
         caller_info = stack[1]
         caller_name = caller_info.function
         caller_line_no = caller_info.lineno
-        self._do_log('debug', f"{caller_name}():{caller_line_no}", message, 100)
+        self._do_log(level, f"{caller_name}():{caller_line_no}", message, status_code, save=save)
 
-    def info(self, message: str):
+    def success(self, message: str, status_code: int = 0, save: bool = False):
         stack = inspect.stack()
         caller_info = stack[1]
         caller_name = caller_info.function
         caller_line_no = caller_info.lineno
-        self._do_log('info', f"{caller_name}():{caller_line_no}", message, 200)
+        self._do_log('success', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
 
-    def warning(self, message: str):
+    def debug(self, message: str, status_code: int = 100, save: bool = False):
         stack = inspect.stack()
         caller_info = stack[1]
         caller_name = caller_info.function
         caller_line_no = caller_info.lineno
-        self._do_log('warning', f"{caller_name}():{caller_line_no}", message, 400)
+        self._do_log('debug', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
 
-    def error(self, message: str):
+    def info(self, message: str, status_code: int = 200, save: bool = False):
         stack = inspect.stack()
         caller_info = stack[1]
         caller_name = caller_info.function
         caller_line_no = caller_info.lineno
-        self._do_log('error', f"{caller_name}():{caller_line_no}", message, 500)
+        self._do_log('info', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
 
-    def exception(self, message: str):
+    def warning(self, message: str, status_code: int = 400, save: bool = False):
         stack = inspect.stack()
         caller_info = stack[1]
         caller_name = caller_info.function
         caller_line_no = caller_info.lineno
-        self._do_log('exception', f"{caller_name}():{caller_line_no}", message, 600)
+        self._do_log('warning', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
 
+    def error(self, message: str, status_code: int = 500, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('error', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
 
-if __name__ == '__main__':
-    c = Logger("localhost", api_key="183d96c0-0965-44fa-b7d7-d4fcf10610a5", api_secret="e4882d22-9d35-4f85-b32d-f497e8c08979", port=5626)
-    c.info("holi")
+    def exception(self, message: str, status_code: int = 600, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('exception', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
```

### Comparing `ParendumLib-0.1.9/parendumlib/mailer.py` & `ParendumLib-0.2.0/parendumlib/mailer.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 
             msg.attach(MIMEText(template, 'html'))
 
             try:
                 server = smtplib.SMTP(config.get('email', dict()).get('server'),
                                       config.get('email', dict()).get('port'))
             except Exception as e:
-                print(f"Error al conectar al servidor SMTP: {e}")
+                print(f"Error connecting to SMTP server: {e}")
                 return False
             try:
                 server.starttls()
             except Exception as e:
-                print(f"Error al iniciar TLS: {e}")
+                print(f"Error initializing TLS: {e}")
                 return False
             server.login(config.get('email', dict()).get('username'), config.get('email', dict()).get('password'))
             server.sendmail(config.get('email', dict()).get('username'), to, msg.as_string())
             server.quit()
             return True
         except Exception as e:
             print(f"[EXCEPTION] {str(e)} - Sending Email Template")
@@ -118,11 +118,7 @@
                 continue
 
             filename = part.get_filename()
             if filename:
                 payload = part.get_payload(decode=True)
                 attachments.append((filename, payload))
         return attachments
-
-
-if __name__ == '__main__':
-    mailer = GMailer("parendumou@gmail.com", "laeujjrdrxhwqnjo")
```

### Comparing `ParendumLib-0.1.9/parendumlib/permissions/mongodb.py` & `ParendumLib-0.2.0/parendumlib/permissions/mongodb.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.9/parendumlib/responses.py` & `ParendumLib-0.2.0/parendumlib/responses.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.9/parendumlib/utils.py` & `ParendumLib-0.2.0/parendumlib/utils.py`

 * *Files identical despite different names*

