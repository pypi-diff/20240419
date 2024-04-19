# Comparing `tmp/qaml-0.0.7.8.tar.gz` & `tmp/qaml-0.0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.8.tar", last modified: Thu Apr 18 20:16:20 2024, max compression
+gzip compressed data, was "qaml-0.0.7.9.tar", last modified: Fri Apr 19 14:19:14 2024, max compression
```

## Comparing `qaml-0.0.7.8.tar` & `qaml-0.0.7.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:16:20.430022 qaml-0.0.7.8/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.8/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:16:20.429882 qaml-0.0.7.8/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.8/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-18 20:16:16.000000 qaml-0.0.7.8/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:16:20.428993 qaml-0.0.7.8/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.8/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.7.8/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    13192 2024-04-18 20:15:06.000000 qaml-0.0.7.8/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:16:20.429705 qaml-0.0.7.8/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-18 20:16:20.430053 qaml-0.0.7.8/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-19 14:19:14.713387 qaml-0.0.7.9/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.9/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-19 14:19:14.713245 qaml-0.0.7.9/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.9/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-19 14:18:58.000000 qaml-0.0.7.9/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-19 14:19:14.712391 qaml-0.0.7.9/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.9/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.7.9/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    12871 2024-04-19 14:15:29.000000 qaml-0.0.7.9/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-19 14:19:14.713089 qaml-0.0.7.9/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-19 14:19:14.000000 qaml-0.0.7.9/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-19 14:19:14.713420 qaml-0.0.7.9/setup.cfg
```

### Comparing `qaml-0.0.7.8/LICENSE` & `qaml-0.0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.8/PKG-INFO` & `qaml-0.0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.8
+Version: 0.0.7.9
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.8/README.md` & `qaml-0.0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.8/pyproject.toml` & `qaml-0.0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.8"
+version = "0.0.7.9"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.8/qaml/__main__.py` & `qaml-0.0.7.9/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.8/qaml/client.py` & `qaml-0.0.7.9/qaml/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,23 @@
         self.api_key = api_key or os.environ.get("QAML_API_KEY")
         self.driver = None
         self.platform = None
         self.screen_size = None
         self.req_session = requests.Session()
         self.req_session.headers.update({"Authorization": f"Bearer {api_key}"})
         self.context = ''
+        self.available_functions = {
+            "tap": self.tap_coordinates,
+            "drag": self.drag,
+            "swipe": self.swipe,
+            "scroll": self.scroll,
+            "type_text": self.type_text,
+            "sleep": self.sleep,
+            "report_error": self.report_error
+        }
 
     def setup_driver(self):
         raise NotImplementedError
 
     def tap_coordinates(self, x, y):
         raise NotImplementedError
 
@@ -61,44 +70,24 @@
         PIL_image = PIL_image.resize(new_size)
         buffered = BytesIO()
         PIL_image.save(buffered, format="PNG")
         screenshot = base64.b64encode(buffered.getvalue()).decode("utf-8")
         return screenshot
 
     def _execute_function(self, function_name, **kwargs):
-        available_functions = {
-            "tap": self.tap_coordinates,
-            "drag": self.drag,
-            "swipe": self.swipe,
-            "scroll": self.scroll,
-            "type_text": self.type_text,
-            "sleep": self.sleep,
-            "report_error": self.report_error,
-            "switch_to_app": self.switch_to_app,
-        }
-        function = available_functions.get(function_name)
+        function = self.available_functions.get(function_name)
         if function:
             function(**kwargs)
 
     def execute(self, script):
         screenshot = self.get_screenshot()
         payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.context}
         response = self.req_session.post("https://api.camelqa.com/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(f"Action: {script} - Response: {response.text}")
         actions = response.json()
-        available_functions = {
-            "tap": self.tap_coordinates,
-            "drag": self.drag,
-            "swipe": self.swipe,
-            "scroll": self.scroll,
-            "type_text": self.type_text,
-            "sleep": self.sleep,
-            "report_error": self.report_error,
-            "switch_to_app": self.switch_to_app,
-        }
         for action in actions:
             self._execute_function(action["name"], **json.loads(action["arguments"]))
 
     def agent(self, task):
         progress = []
         while True:
             screenshot = self.get_screenshot()
@@ -172,14 +161,15 @@
 
     def type_text(self, text):
         subprocess.run(["adb", "shell", "input", "text", f"'{text}'"])
 
 class IOSClient(BaseClient):
     def __init__(self, api_key, driver=None, use_mjpeg=True, use_hid_typing=False):
         super().__init__(api_key)
+        self.available_functions["switch_to_app"] = self.switch_to_app
         self.platform = "iOS"
         self.use_mjpeg = use_mjpeg
         self.use_hid_typing = use_hid_typing
         if driver:
             self.driver = driver
         else:
             def get_ios_udid():
```

### Comparing `qaml-0.0.7.8/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.9/qaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.8
+Version: 0.0.7.9
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

