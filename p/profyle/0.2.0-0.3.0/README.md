# Comparing `tmp/profyle-0.2.0.tar.gz` & `tmp/profyle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profyle-0.2.0.tar", max compression
+gzip compressed data, was "profyle-0.3.0.tar", max compression
```

## Comparing `profyle-0.2.0.tar` & `profyle-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1078 2023-02-21 14:39:22.202379 profyle-0.2.0/LICENSE
--rw-r--r--   0        0        0     4998 2023-10-17 14:37:25.563714 profyle-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-10-17 08:17:23.855383 profyle-0.2.0/profyle/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 05:27:30.127575 profyle-0.2.0/profyle/application/__init__.py
--rw-r--r--   0        0        0     1827 2023-10-17 12:42:44.769423 profyle-0.2.0/profyle/application/profyle.py
--rw-r--r--   0        0        0        0 2023-04-16 06:22:35.839150 profyle-0.2.0/profyle/application/trace/__init__.py
--rw-r--r--   0        0        0      266 2023-04-16 06:14:40.270016 profyle-0.2.0/profyle/application/trace/create.py
--rw-r--r--   0        0        0      260 2023-10-17 09:29:02.031990 profyle-0.2.0/profyle/application/trace/delete.py
--rw-r--r--   0        0        0      446 2023-10-17 09:03:09.861756 profyle-0.2.0/profyle/application/trace/get.py
--rw-r--r--   0        0        0      334 2023-10-14 08:48:24.083149 profyle-0.2.0/profyle/application/trace/store.py
--rw-r--r--   0        0        0      123 2023-04-16 06:53:09.964904 profyle-0.2.0/profyle/application/trace/vacuum.py
--rw-r--r--   0        0        0        0 2023-04-16 05:27:42.973808 profyle-0.2.0/profyle/domain/__init__.py
--rw-r--r--   0        0        0      848 2023-10-17 13:15:16.058527 profyle-0.2.0/profyle/domain/trace.py
--rw-r--r--   0        0        0      962 2023-10-17 09:28:55.618776 profyle-0.2.0/profyle/domain/trace_repository.py
--rw-r--r--   0        0        0       71 2023-10-17 13:41:50.214379 profyle-0.2.0/profyle/fastapi.py
--rw-r--r--   0        0        0       69 2023-10-17 13:41:46.886809 profyle-0.2.0/profyle/flask.py
--rw-r--r--   0        0        0        0 2023-10-17 08:14:46.621316 profyle-0.2.0/profyle/infrastructure/__init__.py
--rw-r--r--   0        0        0     3646 2023-10-17 13:36:12.410292 profyle-0.2.0/profyle/infrastructure/http_server.py
--rw-r--r--   0        0        0        0 2023-02-21 14:39:22.129946 profyle-0.2.0/profyle/infrastructure/middleware/__init__.py
--rw-r--r--   0        0        0     1339 2023-10-17 10:17:20.993978 profyle-0.2.0/profyle/infrastructure/middleware/fastapi.py
--rw-r--r--   0        0        0     1293 2023-10-17 10:21:13.951605 profyle-0.2.0/profyle/infrastructure/middleware/flask.py
--rw-r--r--   0        0        0      242 2023-10-17 06:39:49.089790 profyle-0.2.0/profyle/infrastructure/sqlite3/get_connection.py
--rw-r--r--   0        0        0     4124 2023-10-17 09:20:26.650679 profyle-0.2.0/profyle/infrastructure/sqlite3/repository.py
--rw-r--r--   0        0        0   362807 2023-10-14 19:20:41.557351 profyle-0.2.0/profyle/infrastructure/web/static/libs/tailwind.js
--rw-r--r--   0        0        0     6581 2023-10-17 07:46:15.077854 profyle-0.2.0/profyle/infrastructure/web/templates/traces.html
--rw-r--r--   0        0        0     1226 2023-10-17 13:36:23.674978 profyle-0.2.0/profyle/main.py
--rw-r--r--   0        0        0      602 2023-10-17 06:38:49.468243 profyle-0.2.0/profyle/settings.py
--rw-r--r--   0        0        0     1874 2023-10-17 18:00:06.694464 profyle-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6687 1970-01-01 00:00:00.000000 profyle-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-02-21 14:39:22.202379 profyle-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5234 2024-04-19 13:47:36.830006 profyle-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-10-17 08:17:23.855383 profyle-0.3.0/profyle/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 05:27:30.127575 profyle-0.3.0/profyle/application/__init__.py
+-rw-r--r--   0        0        0     1854 2023-11-15 11:41:52.299434 profyle-0.3.0/profyle/application/profyle.py
+-rw-r--r--   0        0        0        0 2023-04-16 06:22:35.839150 profyle-0.3.0/profyle/application/trace/__init__.py
+-rw-r--r--   0        0        0      266 2023-04-16 06:14:40.270016 profyle-0.3.0/profyle/application/trace/create.py
+-rw-r--r--   0        0        0      372 2023-11-14 13:38:42.861811 profyle-0.3.0/profyle/application/trace/delete.py
+-rw-r--r--   0        0        0      446 2023-11-15 11:41:52.299439 profyle-0.3.0/profyle/application/trace/get.py
+-rw-r--r--   0        0        0      334 2023-10-14 08:48:24.083149 profyle-0.3.0/profyle/application/trace/store.py
+-rw-r--r--   0        0        0      123 2023-04-16 06:53:09.964904 profyle-0.3.0/profyle/application/trace/vacuum.py
+-rw-r--r--   0        0        0       77 2023-11-12 10:46:20.117764 profyle-0.3.0/profyle/django.py
+-rw-r--r--   0        0        0        0 2023-04-16 05:27:42.973808 profyle-0.3.0/profyle/domain/__init__.py
+-rw-r--r--   0        0        0      766 2023-11-15 11:39:40.473916 profyle-0.3.0/profyle/domain/trace.py
+-rw-r--r--   0        0        0     1044 2023-11-15 11:13:17.970630 profyle-0.3.0/profyle/domain/trace_repository.py
+-rw-r--r--   0        0        0       78 2023-11-15 10:54:30.137957 profyle-0.3.0/profyle/fastapi.py
+-rw-r--r--   0        0        0       76 2023-11-12 10:46:38.405057 profyle-0.3.0/profyle/flask.py
+-rw-r--r--   0        0        0        0 2023-10-17 08:14:46.621316 profyle-0.3.0/profyle/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3645 2023-11-15 11:41:52.297953 profyle-0.3.0/profyle/infrastructure/http_server.py
+-rw-r--r--   0        0        0        0 2023-11-15 12:54:11.883723 profyle-0.3.0/profyle/infrastructure/middleware/__init__.py
+-rw-r--r--   0        0        0     1452 2024-04-19 10:55:35.119636 profyle-0.3.0/profyle/infrastructure/middleware/django.py
+-rw-r--r--   0        0        0     1721 2023-11-15 13:25:00.812583 profyle-0.3.0/profyle/infrastructure/middleware/fastapi.py
+-rw-r--r--   0        0        0     1673 2024-04-19 10:46:29.639887 profyle-0.3.0/profyle/infrastructure/middleware/flask.py
+-rw-r--r--   0        0        0      242 2023-10-17 06:39:49.089790 profyle-0.3.0/profyle/infrastructure/sqlite3/get_connection.py
+-rw-r--r--   0        0        0     4433 2023-11-15 11:41:52.298001 profyle-0.3.0/profyle/infrastructure/sqlite3/repository.py
+-rw-r--r--   0        0        0   362807 2023-10-14 19:20:41.557351 profyle-0.3.0/profyle/infrastructure/web/static/libs/tailwind.js
+-rw-r--r--   0        0        0     6581 2023-10-17 07:46:15.077854 profyle-0.3.0/profyle/infrastructure/web/templates/traces.html
+-rw-r--r--   0        0        0     1436 2023-11-15 11:39:33.332266 profyle-0.3.0/profyle/main.py
+-rw-r--r--   0        0        0      602 2023-11-15 11:41:52.297880 profyle-0.3.0/profyle/settings.py
+-rw-r--r--   0        0        0     2291 2024-04-19 14:41:41.174836 profyle-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 profyle-0.3.0/PKG-INFO
```

### Comparing `profyle-0.2.0/LICENSE` & `profyle-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `profyle-0.2.0/README.md` & `profyle-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     src="https://github.com/vpcarlos/profyle/blob/main/docs/img/profyle.png?raw=true" 
     width="300"
     alt="Profyle"
  >
 </p>
 
 ### Development tool for analysing and managing python traces
-
+[![Tests](https://github.com/vpcarlos/profyle/actions/workflows/test.yml/badge.svg)](https://github.com/vpcarlos/profyle/actions/workflows/test.yml)
 <a href="https://pypi.org/project/profyle" target="_blank">
     <img src="https://img.shields.io/pypi/v/profyle" alt="Package version">
 </a>
 <a href="https://pypi.org/project/profyle" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/profyle.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 
@@ -36,55 +36,55 @@
 </div>
 
 ## Example
 
 ### 1. Implement
 In order to track all your API requests you must implement the <code>ProfyleMiddleware</code>
 #### ProfyleMiddleware
-| Attribute | Required | Default | Description |
-| --- | --- | --- | --- |
-| `enabled` | No | `True` | Enable or disable Profyle |
-| `pattern` | No | `None` | 0nly trace those paths that match with pattern (<a href="https://en.wikipedia.org/wiki/Glob_(programming)" class="external-link" target="_blank">glob pattern</a>)  |
-| `max_stack_depth` | No | `-1` | Limit maximum stack trace depth |
-| `min_duration` | No | `0` (milisecons) | Only record traces with a greather duration than the limit. |
+| Attribute | Required | Default | Description | ENV Variable |
+| --- | --- | --- | --- | --- |
+| `enabled` | No | `True` | Enable or disable Profyle | `PROFYLE_ENABLED` |
+| `pattern` | No | `None` | 0nly trace those paths that match with [pattern](https://en.wikipedia.org/wiki/Glob_(programming))  | `PROFYLE_PATTERN` |
+| `max_stack_depth` | No | `-1` | Limit maximum stack trace depth | `PROFYLE_MAX_STACK_DEPTH` |
+| `min_duration` | No | `0` (milisecons) | Only record traces with a greather duration than the limit. | `PROFYLE_MIN_DURATION` |
 
 
 <details markdown="1" open>
 <summary>FastAPI</summary>
 
 ```Python
 from fastapi import FastAPI
 from profyle.fastapi import ProfyleMiddleware
 
 app = FastAPI()
 # Trace all requests
 app.add_middleware(ProfyleMiddleware)
 
-@app.get("/items/{item_id}")
-async def read_item(item_id: int):
-    return {"item_id": item_id}
+@app.get("/")
+async def root():
+    return {"hello": "world"}
 ```
 
 ```Python
 from fastapi import FastAPI
 from profyle.fastapi import ProfyleMiddleware
 
 app = FastAPI()
-# Trace all requests that match that start with /api/products 
+# Trace all requests that match that start with /users 
 # with a minimum duration of 100ms and a maximum stack depth of 20
 app.add_middleware(
     ProfyleMiddleware,
-    pattern="/api/products*",
+    pattern="/users*",
     max_stack_depth=20,
     min_duration=100
 )
 
-@app.get("/items/{item_id}")
-async def read_item(item_id: int):
-    return {"item_id": item_id}
+@app.get("/users/{user_id}")
+async def get_user(user_id: int):
+    return {"hello": "user"}
 ```
 </details>
 
 <details markdown="1">
 <summary>Flask</summary>
 
 ```Python
@@ -92,22 +92,31 @@
 from profyle.flask import ProfyleMiddleware
 
 app = Flask(__name__)
 
 app.wsgi_app = ProfyleMiddleware(app.wsgi_app, pattern="*/api/products*")
 
 @app.route("/")
-def hello_world():
+def root():
     return "<p>Hello, World!</p>"
 ```
 </details>
 
 <details markdown="1">
 <summary>Django</summary>
-Soon..
+
+```Python
+# settings.py
+
+MIDDLEWARE = [
+    ...
+    "profyle.django.ProfyleMiddleware",
+    ...
+]
+```
 </details>
 
 ### 2. Run
 * Run the web server:
 
 <div class="termy">
 
@@ -184,8 +193,8 @@
 
 ```console
 $ profyle check
 
 DB size: 30MB
 ```
 
-</div>
+</div>
```

### Comparing `profyle-0.2.0/profyle/application/profyle.py` & `profyle-0.3.0/profyle/application/profyle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import fnmatch
 import json
 import re
-from typing import Optional
 from dataclasses import dataclass
 from tempfile import NamedTemporaryFile
+from typing import Optional
 
 from viztracer import VizTracer
 
 from profyle.application.trace.store import store_trace
-from profyle.domain.trace_repository import TraceRepository
 from profyle.domain.trace import TraceCreate
+from profyle.domain.trace_repository import TraceRepository
 
 
 @dataclass
 class profyle:
     name: str
     repo: TraceRepository
     max_stack_depth: int = -1
@@ -27,15 +27,16 @@
             self.tracer = VizTracer(
                 log_func_args=True,
                 log_print=True,
                 log_func_retval=True,
                 log_async=True,
                 file_info=True,
                 min_duration=self.min_duration,
-                max_stack_depth=self.max_stack_depth
+                max_stack_depth=self.max_stack_depth,
+                verbose=0
             )
             self.tracer.start()
 
     def __exit__(
         self,
         *args,
     ) -> None:
```

### Comparing `profyle-0.2.0/profyle/domain/trace_repository.py` & `profyle-0.3.0/profyle/domain/trace_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from profyle.domain.trace import Trace, TraceCreate
 
 
 class TraceRepository(ABC):
-
     @abstractmethod
     def create_trace_selected_table(self) -> None:
         ...
 
     @abstractmethod
     def create_trace_table(self) -> None:
         ...
 
     @abstractmethod
     def delete_all_traces(self) -> int:
         ...
 
     @abstractmethod
+    def deleted_all_selected_traces(self) -> int:
+        ...
+
+    @abstractmethod
     def vacuum(self) -> None:
         ...
 
     @abstractmethod
     def store_trace_selected(self, trace_id: int) -> None:
         ...
```

### Comparing `profyle-0.2.0/profyle/infrastructure/http_server.py` & `profyle-0.3.0/profyle/infrastructure/http_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from sqlite3 import Connection
 
+import uvicorn
 from fastapi import Depends, FastAPI, Request
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from starlette.responses import RedirectResponse
-import uvicorn
 
 from profyle.application.trace.create import create_trace_selected_table, create_trace_table
-from profyle.application.trace.get import get_all_traces, get_trace_selected, get_trace_by_id
+from profyle.application.trace.get import get_all_traces, get_trace_by_id, get_trace_selected
 from profyle.application.trace.store import store_trace_selected
 from profyle.infrastructure.sqlite3.get_connection import get_connection
 from profyle.infrastructure.sqlite3.repository import SQLiteTraceRepository
 from profyle.settings import settings
 
-
 app = FastAPI(
     title="Profyle",
     version="1.0.0"
 )
 
 app.add_middleware(
     CORSMiddleware,
```

### Comparing `profyle-0.2.0/profyle/infrastructure/middleware/fastapi.py` & `profyle-0.3.0/profyle/infrastructure/middleware/fastapi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,46 @@
+import os
 from typing import Optional
-from starlette.types import ASGIApp, Scope, Receive, Send
+
+from starlette.types import ASGIApp, Receive, Scope, Send
 
 from profyle.application.profyle import profyle
 from profyle.infrastructure.sqlite3.repository import SQLiteTraceRepository
 
 
 class ProfyleMiddleware:
     def __init__(
         self,
         app: ASGIApp,
         enabled: bool = True,
         pattern: Optional[str] = None,
         max_stack_depth: int = -1,
         min_duration: int = 0,
-        trace_repo: SQLiteTraceRepository = SQLiteTraceRepository()
+        trace_repo: SQLiteTraceRepository = SQLiteTraceRepository(),
     ):
         self.app = app
-        self.enabled = enabled
-        self.pattern = pattern
-        self.max_stack_depth = max_stack_depth
-        self.min_duration = min_duration
         self.trace_repo = trace_repo
 
+        PROFYLE_ENABLED = os.getenv("PROFYLE_ENABLED", "")
+        PROFYLE_PATTERN = os.getenv("PROFYLE_PATTERN")
+        PROFYLE_MAX_STACK_DEPTH = os.getenv("PROFYLE_MAX_STACK_DEPTH")
+        PROFYLE_MIN_DURATION = os.getenv("PROFYLE_MIN_DURATION")
+
+        self.enabled = PROFYLE_ENABLED.lower() == "true" or enabled
+        self.pattern = PROFYLE_PATTERN or pattern
+        self.max_stack_depth = int(PROFYLE_MAX_STACK_DEPTH or max_stack_depth)
+        self.min_duration = int(PROFYLE_MIN_DURATION or min_duration)
+
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         if self.enabled and scope["type"] == "http":
-            method = scope.get('method', '').upper()
-            path = scope.get('raw_path', b'').decode('utf-8')
+            method = scope.get("method", "").upper()
+            path = scope.get("raw_path", b"").decode("utf-8")
             with profyle(
                 name=f"{method} {path}",
                 pattern=self.pattern,
                 repo=self.trace_repo,
                 max_stack_depth=self.max_stack_depth,
-                min_duration=self.min_duration
+                min_duration=self.min_duration,
             ):
                 await self.app(scope, receive, send)
             return
         await self.app(scope, receive, send)
```

### Comparing `profyle-0.2.0/profyle/infrastructure/middleware/flask.py` & `profyle-0.3.0/profyle/infrastructure/middleware/flask.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Optional
 
 from profyle.application.profyle import profyle
 from profyle.domain.trace_repository import TraceRepository
 from profyle.infrastructure.sqlite3.repository import SQLiteTraceRepository
 
 
@@ -12,20 +13,27 @@
         enabled: bool = True,
         pattern: Optional[str] = None,
         max_stack_depth: int = -1,
         min_duration: int = 0,
         trace_repo: TraceRepository = SQLiteTraceRepository()
     ):
         self.app = app
-        self.enabled = enabled
-        self.pattern = pattern
-        self.max_stack_depth = max_stack_depth
-        self.min_duration = min_duration
         self.trace_repo = trace_repo
 
+        PROFYLE_ENABLED = os.getenv("PROFYLE_ENABLED", "")
+        PROFYLE_PATTERN = os.getenv("PROFYLE_PATTERN")
+        PROFYLE_MAX_STACK_DEPTH = os.getenv("PROFYLE_MAX_STACK_DEPTH")
+        PROFYLE_MIN_DURATION = os.getenv("PROFYLE_MIN_DURATION")
+
+        self.enabled = PROFYLE_ENABLED.lower() == "true" or enabled
+        self.pattern = PROFYLE_PATTERN or pattern
+        self.max_stack_depth = int(PROFYLE_MAX_STACK_DEPTH or max_stack_depth)
+        self.min_duration = int(PROFYLE_MIN_DURATION or min_duration)
+
+
     def __call__(self, environ, start_response):
         if environ.get("wsgi.url_scheme") == "http" and self.enabled:
             method = environ.get("REQUEST_METHOD", "").upper()
             path = environ.get("REQUEST_URI")
             with profyle(
                 name=f"{method} {path}",
                 pattern=self.pattern,
```

### Comparing `profyle-0.2.0/profyle/infrastructure/sqlite3/repository.py` & `profyle-0.3.0/profyle/infrastructure/sqlite3/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import json
 from sqlite3 import Connection, Error, Row
 from typing import Optional
-import json
 
 from profyle.domain.trace import Trace, TraceCreate
 from profyle.domain.trace_repository import TraceRepository
 from profyle.infrastructure.sqlite3.get_connection import get_connection
 
 
 class SQLiteTraceRepository(TraceRepository):
@@ -14,27 +14,27 @@
         self.db = db
 
     def create_trace_selected_table(self) -> None:
         cursor = self.db.cursor()
         cursor.execute(
             """
             CREATE TABLE IF NOT EXISTS trace_selected (
-                id INTEGER PRIMARY KEY NOT NULL,   
+                id INTEGER PRIMARY KEY NOT NULL,
                 trace_id INTEGER
             );
             """
         )
 
     def create_trace_table(self) -> None:
         cursor = self.db.cursor()
         cursor.execute(
             """
-            CREATE TABLE IF NOT EXISTS traces (  
-                id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL, 
-                timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP NOT NULL, 
+            CREATE TABLE IF NOT EXISTS traces (
+                id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
+                timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP NOT NULL,
                 data JSON NOT NULL,
                 duration REAL NOT NULL,
                 name VARCHAR(64) NOT NULL
             );
             """
         )
 
@@ -45,29 +45,40 @@
             DELETE FROM traces
             """
         )
         self.db.commit()
         cursor.close()
         return cursor.rowcount
 
+    def deleted_all_selected_traces(self) -> int:
+        cursor = self.db.cursor()
+        cursor.execute(
+            """
+            DELETE FROM trace_selected
+            """
+        )
+        self.db.commit()
+        cursor.close()
+        return cursor.rowcount
+
     def vacuum(self) -> None:
         cursor = self.db.cursor()
         cursor.execute(
             """
             VACUUM
             """
         )
         self.db.commit()
         cursor.close()
 
     def store_trace_selected(self, trace_id: int) -> None:
         try:
             self.create_trace_selected_table()
             cursor = self.db.cursor()
-            replace_query = """ 
+            replace_query = """
                     REPLACE INTO trace_selected
                     ( id, trace_id) VALUES (?, ?)
                 """
             data_tuple = (
                 1,
                 trace_id
             )
@@ -78,15 +89,15 @@
             print("Failed to insert data into selected_trace table", error)
 
     def store_trace(self, trace: TraceCreate) -> None:
         try:
             self.create_trace_table()
             cursor = self.db.cursor()
 
-            insert_query = """ 
+            insert_query = """
                 INSERT INTO traces
                 ( data, duration, name) VALUES (?, ?, ?)
             """
 
             data_tuple = (
                 json.dumps(trace.data),
                 trace.duration,
@@ -98,16 +109,20 @@
 
         except Error as error:
             print("Failed to insert data into trace table", error)
 
     def get_all_traces(self) -> list[Trace]:
         self.db.row_factory = Row
         cursor = self.db.cursor()
-        cursor.execute(
-            "SELECT id, timestamp, duration, name FROM traces ORDER BY timestamp DESC")
+        cursor.execute("""
+            SELECT
+            id, timestamp, duration, name
+            FROM traces
+            ORDER BY timestamp DESC
+        """)
 
         traces = cursor.fetchall()
 
         return [
             Trace(**dict(trace))
             for trace in traces
         ]
```

### Comparing `profyle-0.2.0/profyle/infrastructure/web/static/libs/tailwind.js` & `profyle-0.3.0/profyle/infrastructure/web/static/libs/tailwind.js`

 * *Files identical despite different names*

### Comparing `profyle-0.2.0/profyle/infrastructure/web/templates/traces.html` & `profyle-0.3.0/profyle/infrastructure/web/templates/traces.html`

 * *Files identical despite different names*

### Comparing `profyle-0.2.0/profyle/main.py` & `profyle-0.3.0/profyle/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-import os
 import asyncio
+import os
 
 import typer
 from rich import print
 
-
-from profyle.infrastructure.sqlite3.repository import SQLiteTraceRepository
-from profyle.application.trace.delete import delete_all_traces
+from profyle.application.trace.delete import delete_all_selected_traces, delete_all_traces
 from profyle.application.trace.vacuum import vacuum
-from profyle.infrastructure.sqlite3.get_connection import get_connection
 from profyle.infrastructure.http_server import start_server
+from profyle.infrastructure.sqlite3.get_connection import get_connection
+from profyle.infrastructure.sqlite3.repository import SQLiteTraceRepository
 from profyle.settings import settings
 
-
 app = typer.Typer()
 
 
-@app.command()
+@app.command(help="Start the Profyle server")
 def start(port: int = 0, host: str = "127.0.0.1"):
     asyncio.run(start_server(port=port, host=host))
 
 
-@app.command()
+@app.command(help="Remove all traces")
 def clean():
     db = get_connection()
     sqlite_repo = SQLiteTraceRepository(db)
     removed_traces = delete_all_traces(sqlite_repo)
+    removed_selected_traces = delete_all_selected_traces(sqlite_repo)
     vacuum(sqlite_repo)
-    print(f"[green]{removed_traces} traces removed [/green]")
+    removed_traces = removed_traces + removed_selected_traces
+    print(f"[green]{removed_traces} records removed [/green]")
 
 
-@app.command()
-def check():
+@app.command(help="Proyfle info")
+def info():
     db_size_in_bytes = os.path.getsize(settings.get_path("profile.db"))
-    db_size_in_megabytes = round(db_size_in_bytes/10**6, 2)
-    db_size_in_gigabytes = round(db_size_in_megabytes/10**3, 2)
 
-    if db_size_in_megabytes > 1000:
-        print(f"[orange1]DB size: {db_size_in_gigabytes} GB [/orange1]")
-        return
-    print(f"[orange1]DB size: {db_size_in_megabytes} MB [/orange1]")
+    print(f"[bold]Project[/bold] → {settings.project_dir}")
+    print(db_size_in_bytes)
+    if db_size_in_bytes > 1e9:
+        db_size = f"{round(db_size_in_bytes/1e9, 2)} GB"
+    else:
+        db_size = f"{round(db_size_in_bytes/1e6, 2)} MB"
+
+    print(f"[bold]DB size[/bold] → {db_size}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `profyle-0.2.0/profyle/settings.py` & `profyle-0.3.0/profyle/settings.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
-from pydantic_settings import BaseSettings
 import viztracer
+from pydantic_settings import BaseSettings
 
 
 class Settings(BaseSettings):
     app_name: str = "Profyle"
     project_dir: str = os.path.normpath(
         os.path.join(
             os.path.abspath(__file__),
```

### Comparing `profyle-0.2.0/PKG-INFO` & `profyle-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profyle
-Version: 0.2.0
+Version: 0.3.0
 Summary: Profyle, a development tool for analysing and managing python traces
 Home-page: https://github.com/vpcarlos/profyle
 License: MIT
 Keywords: cprofile,devtool,perffeto,profyle,viztracer,fastapi,flask
 Author: Carlos Valdivia
 Author-email: vpcarlos97@gmail.com
 Maintainer: Carlos Valdivia
@@ -19,40 +19,41 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
 Requires-Dist: fastapi (>=0.70.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: uvicorn (>=0.20.0)
-Requires-Dist: viztracer (==0.16.0)
+Requires-Dist: viztracer (>=0.16.0,<0.17.0)
 Project-URL: Repository, https://github.com/vpcarlos/profyle
 Description-Content-Type: text/markdown
 
 <p align="center">
  <img 
     src="https://github.com/vpcarlos/profyle/blob/main/docs/img/profyle.png?raw=true" 
     width="300"
     alt="Profyle"
  >
 </p>
 
 ### Development tool for analysing and managing python traces
-
+[![Tests](https://github.com/vpcarlos/profyle/actions/workflows/test.yml/badge.svg)](https://github.com/vpcarlos/profyle/actions/workflows/test.yml)
 <a href="https://pypi.org/project/profyle" target="_blank">
     <img src="https://img.shields.io/pypi/v/profyle" alt="Package version">
 </a>
 <a href="https://pypi.org/project/profyle" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/profyle.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 
@@ -77,55 +78,55 @@
 </div>
 
 ## Example
 
 ### 1. Implement
 In order to track all your API requests you must implement the <code>ProfyleMiddleware</code>
 #### ProfyleMiddleware
-| Attribute | Required | Default | Description |
-| --- | --- | --- | --- |
-| `enabled` | No | `True` | Enable or disable Profyle |
-| `pattern` | No | `None` | 0nly trace those paths that match with pattern (<a href="https://en.wikipedia.org/wiki/Glob_(programming)" class="external-link" target="_blank">glob pattern</a>)  |
-| `max_stack_depth` | No | `-1` | Limit maximum stack trace depth |
-| `min_duration` | No | `0` (milisecons) | Only record traces with a greather duration than the limit. |
+| Attribute | Required | Default | Description | ENV Variable |
+| --- | --- | --- | --- | --- |
+| `enabled` | No | `True` | Enable or disable Profyle | `PROFYLE_ENABLED` |
+| `pattern` | No | `None` | 0nly trace those paths that match with [pattern](https://en.wikipedia.org/wiki/Glob_(programming))  | `PROFYLE_PATTERN` |
+| `max_stack_depth` | No | `-1` | Limit maximum stack trace depth | `PROFYLE_MAX_STACK_DEPTH` |
+| `min_duration` | No | `0` (milisecons) | Only record traces with a greather duration than the limit. | `PROFYLE_MIN_DURATION` |
 
 
 <details markdown="1" open>
 <summary>FastAPI</summary>
 
 ```Python
 from fastapi import FastAPI
 from profyle.fastapi import ProfyleMiddleware
 
 app = FastAPI()
 # Trace all requests
 app.add_middleware(ProfyleMiddleware)
 
-@app.get("/items/{item_id}")
-async def read_item(item_id: int):
-    return {"item_id": item_id}
+@app.get("/")
+async def root():
+    return {"hello": "world"}
 ```
 
 ```Python
 from fastapi import FastAPI
 from profyle.fastapi import ProfyleMiddleware
 
 app = FastAPI()
-# Trace all requests that match that start with /api/products 
+# Trace all requests that match that start with /users 
 # with a minimum duration of 100ms and a maximum stack depth of 20
 app.add_middleware(
     ProfyleMiddleware,
-    pattern="/api/products*",
+    pattern="/users*",
     max_stack_depth=20,
     min_duration=100
 )
 
-@app.get("/items/{item_id}")
-async def read_item(item_id: int):
-    return {"item_id": item_id}
+@app.get("/users/{user_id}")
+async def get_user(user_id: int):
+    return {"hello": "user"}
 ```
 </details>
 
 <details markdown="1">
 <summary>Flask</summary>
 
 ```Python
@@ -133,22 +134,31 @@
 from profyle.flask import ProfyleMiddleware
 
 app = Flask(__name__)
 
 app.wsgi_app = ProfyleMiddleware(app.wsgi_app, pattern="*/api/products*")
 
 @app.route("/")
-def hello_world():
+def root():
     return "<p>Hello, World!</p>"
 ```
 </details>
 
 <details markdown="1">
 <summary>Django</summary>
-Soon..
+
+```Python
+# settings.py
+
+MIDDLEWARE = [
+    ...
+    "profyle.django.ProfyleMiddleware",
+    ...
+]
+```
 </details>
 
 ### 2. Run
 * Run the web server:
 
 <div class="termy">
 
@@ -226,7 +236,8 @@
 ```console
 $ profyle check
 
 DB size: 30MB
 ```
 
 </div>
+
```

