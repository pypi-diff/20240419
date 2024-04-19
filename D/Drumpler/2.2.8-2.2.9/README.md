# Comparing `tmp/drumpler-2.2.8.tar.gz` & `tmp/drumpler-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.8.tar", last modified: Thu Apr 18 17:19:36 2024, max compression
+gzip compressed data, was "drumpler-2.2.9.tar", last modified: Thu Apr 18 17:29:10 2024, max compression
```

## Comparing `drumpler-2.2.8.tar` & `drumpler-2.2.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.950159 drumpler-2.2.8/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.948097 drumpler-2.2.8/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      336 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.8/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 17:19:36.949164 drumpler-2.2.8/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.8/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.945681 drumpler-2.2.8/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.8/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)    10636 2024-04-18 15:58:42.000000 drumpler-2.2.8/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.8/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.8/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.8/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.8/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-18 17:19:36.950343 drumpler-2.2.8/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-18 17:19:26.000000 drumpler-2.2.8/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.946890 drumpler-2.2.8/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.8/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:29:10.474001 drumpler-2.2.9/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:29:10.472170 drumpler-2.2.9/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 17:29:10.000000 drumpler-2.2.9/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      360 2024-04-18 17:29:10.000000 drumpler-2.2.9/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-18 17:29:10.000000 drumpler-2.2.9/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-18 17:29:10.000000 drumpler-2.2.9/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-18 17:29:10.000000 drumpler-2.2.9/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.9/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 17:29:10.473078 drumpler-2.2.9/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.9/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:29:10.470759 drumpler-2.2.9/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.9/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)       22 2024-04-18 17:27:18.000000 drumpler-2.2.9/drumpler/__version__.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10688 2024-04-18 17:26:52.000000 drumpler-2.2.9/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.9/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.9/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.9/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.9/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-18 17:29:10.474173 drumpler-2.2.9/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)     1210 2024-04-18 17:29:04.000000 drumpler-2.2.9/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:29:10.471409 drumpler-2.2.9/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.9/test/test_drumpler.py
```

### Comparing `drumpler-2.2.8/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.9/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.8
+Version: 2.2.9
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.8/LICENSE` & `drumpler-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.8/PKG-INFO` & `drumpler-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.8
+Version: 2.2.9
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.8/README.md` & `drumpler-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.8/drumpler/drumpler.py` & `drumpler-2.2.9/drumpler/drumpler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import psutil
 from datetime import datetime, timezone
 from flask import Flask, request, jsonify
 from .sql_base import db, init_app  # Import db and the initialization function
 from .sql_request import SqlRequest
 from .sql_job import SqlJob
 from .sql_event import SqlEvent
+from .__version__ import __version__
 
 app = Flask(__name__)
 
 class Drumpler:
     def __init__(self, authorization_key, host="http://127.0.0.1", port=5000, debug=True, database_uri='sqlite:///default.db'):
         self.app = app  # Use the global app instance
         self.authorization_key = authorization_key
@@ -59,15 +60,15 @@
         self.app.add_url_rule('/events', view_func=self.__create_event, methods=['POST'])
 
     def __authorize_request(self):
         authorization = request.headers.get('Authorization')
         return authorization and authorization == f"Bearer {self.authorization_key}"
     
     def hello_world(self):
-        return "Hello Drumpler!"
+        return f"Hello Drumpler {__version__}!"
 
     def __process_request(self):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
         data = request.get_json() or {}  # Fallback to an empty dict if no JSON is provided
         custom_value = request.args.get('custom_value', None)
```

### Comparing `drumpler-2.2.8/drumpler/sql_job.py` & `drumpler-2.2.9/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.8/test/test_drumpler.py` & `drumpler-2.2.9/test/test_drumpler.py`

 * *Files identical despite different names*

