# Comparing `tmp/es_wait-0.1.2.tar.gz` & `tmp/es_wait-0.1.3.tar.gz`

## Comparing `es_wait-0.1.2.tar` & `es_wait-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.1.2/pytest.ini
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/args.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/base.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/exists.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/health.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/restore.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.1.2/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.1.2/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.1.2/README.md
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.1.3/pytest.ini
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/args.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/base.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/health.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.1.3/src/es_wait/task.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.1.3/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.1.3/README.md
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.1.3/PKG-INFO
```

### Comparing `es_wait-0.1.2/src/es_wait/args.py` & `es_wait-0.1.3/src/es_wait/args.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/src/es_wait/base.py` & `es_wait-0.1.3/src/es_wait/base.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/src/es_wait/exists.py` & `es_wait-0.1.3/src/es_wait/exists.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 class Exists(Waiter):
     """Class Definition"""
     ACTIONS: t.Optional[str] = None
-    IDX_OR_DS = t.Literal['index', 'datastream', 'idx', 'ds']
-    TEMPLATE = t.Literal['index_template', 'template', 'tmpl']
-    COMPONENT = t.Literal['component_template', 'component', 'comp']
+    IDX_OR_DS = ['index', 'datastream', 'idx', 'ds']
+    TEMPLATE = ['index_template', 'template', 'tmpl']
+    COMPONENT = ['component_template', 'component', 'comp']
     def __init__(
             self,
             client: Elasticsearch,
             action: t.Optional[str] = None,
             pause: float = 1.5,
             timeout: float = 15,
             name: str = None,
```

### Comparing `es_wait-0.1.2/src/es_wait/health.py` & `es_wait-0.1.3/src/es_wait/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 class Health(Waiter):
     ACTIONS = ['allocation', 'cluster_routing', 'mount', 'replicas', 'shrink']
-    RELO_ACTIONS = t.Literal['allocation', 'cluster_routing']
-    STATUS_ACTIONS = t.Literal['mount', 'replicas', 'shrink']
+    RELO_ACTIONS = ['allocation', 'cluster_routing']
+    STATUS_ACTIONS = ['mount', 'replicas', 'shrink']
     RELO_ARGS = {'relocating_shards': 0}
     STATUS_ARGS = {'status': 'green'}
     def __init__(
             self,
             client: Elasticsearch,
             action: t.Literal[
                 'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'] = None,
```

### Comparing `es_wait-0.1.2/src/es_wait/relocate.py` & `es_wait-0.1.3/src/es_wait/relocate.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/src/es_wait/restore.py` & `es_wait-0.1.3/src/es_wait/restore.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/src/es_wait/snapshot.py` & `es_wait-0.1.3/src/es_wait/snapshot.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/src/es_wait/task.py` & `es_wait-0.1.3/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/.gitignore` & `es_wait-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/LICENSE` & `es_wait-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/pyproject.toml` & `es_wait-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.2/PKG-INFO` & `es_wait-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.1.2
+Version: 0.1.3
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

