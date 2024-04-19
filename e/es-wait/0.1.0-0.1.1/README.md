# Comparing `tmp/es_wait-0.1.0.tar.gz` & `tmp/es_wait-0.1.1.tar.gz`

## Comparing `es_wait-0.1.0.tar` & `es_wait-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.1.0/pytest.ini
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/args.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/base.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/exists.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/health.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/restore.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.1.0/src/es_wait/task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.1.0/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.1.0/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.1.0/README.md
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 es_wait-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.1.1/pytest.ini
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/args.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/base.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/health.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/task.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.1.1/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.1.1/README.md
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.1.1/PKG-INFO
```

### Comparing `es_wait-0.1.0/src/es_wait/args.py` & `es_wait-0.1.1/src/es_wait/args.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.0/src/es_wait/base.py` & `es_wait-0.1.1/src/es_wait/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from time import sleep
 from datetime import datetime, timezone
 from elasticsearch8 import Elasticsearch
 
 class Waiter:
     """Class Definition"""
-    ACTIONS = t.Literal['any', 'listed', 'actions']
+    ACTIONS = ['any', 'listed', 'actions']
     def __init__(
             self,
             client: Elasticsearch,
             action: t.Union[str, t.Sequence[str]] = None,
             pause: float = 9,    # The delay between checks
             timeout: float = -1, # How long is too long
         ) -> None:
```

### Comparing `es_wait-0.1.0/src/es_wait/exists.py` & `es_wait-0.1.1/src/es_wait/exists.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 class Exists(Waiter):
     """Class Definition"""
-    ACTIONS = t.Optional[str] = None
+    ACTIONS: t.Optional[str] = None
     IDX_OR_DS = t.Literal['index', 'datastream', 'idx', 'ds']
     TEMPLATE = t.Literal['index_template', 'template', 'tmpl']
     COMPONENT = t.Literal['component_template', 'component', 'comp']
     def __init__(
             self,
             client: Elasticsearch,
             action: t.Optional[str] = None,
```

### Comparing `es_wait-0.1.0/src/es_wait/health.py` & `es_wait-0.1.1/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.0/src/es_wait/relocate.py` & `es_wait-0.1.1/src/es_wait/relocate.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 class Relocate(Waiter):
-    ACTIONS = ['relocate']
+    ACTIONS: t.Optional[str] = None
     def __init__(
             self,
             client: Elasticsearch,
-            action: t.Literal['relocate'] = None,
+            action: t.Optional[str] = None,
             pause: float = 9,
             timeout: float = -1,
             name: str = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
         self.empty_check(name)
```

### Comparing `es_wait-0.1.0/src/es_wait/restore.py` & `es_wait-0.1.1/src/es_wait/restore.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 class Restore(Waiter):
-    ACTIONS = t.Literal['restore']
+    ACTIONS: t.Optional[str] = None
     def __init__(
             self,
             client: Elasticsearch,
-            action: t.Literal['restore'] = None,
+            action: t.Optional[str] = None,
             pause: float = 9,
             timeout: float = -1,
             index_list: t.Sequence[str] = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
         self.empty_check(index_list)
```

### Comparing `es_wait-0.1.0/src/es_wait/snapshot.py` & `es_wait-0.1.1/src/es_wait/snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 class Snapshot(Waiter):
-    ACTIONS = t.Literal['snapshot']
+    ACTIONS: t.Optional[str] = None
     def __init__(
             self,
             client: Elasticsearch,
-            action: t.Literal['snapshot'] = None,
+            action: t.Optional[str] = None,
             pause: float = 9,
             timeout: float = -1,
             snapshot: str = None,
             repository: str = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
```

### Comparing `es_wait-0.1.0/src/es_wait/task.py` & `es_wait-0.1.1/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.0/.gitignore` & `es_wait-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.0/LICENSE` & `es_wait-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.0/pyproject.toml` & `es_wait-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -191,7 +191,11 @@
 dependencies = [
     "coverage[toml]",
     "mock",
     "requests",
     "pytest >=7.2.1",
     "pytest-cov",
 ]
+
+[publish.index.repos.main]
+url = "https://upload.pypi.org/legacy/"
+username = "__token__"
```

### Comparing `es_wait-0.1.0/PKG-INFO` & `es_wait-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.1.0
+Version: 0.1.1
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

