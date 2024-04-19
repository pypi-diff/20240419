# Comparing `tmp/es_wait-0.1.1.tar.gz` & `tmp/es_wait-0.1.2.tar.gz`

## Comparing `es_wait-0.1.1.tar` & `es_wait-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.1.1/pytest.ini
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/args.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/base.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/exists.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/health.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/restore.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.1.1/src/es_wait/task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.1.1/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.1.1/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.1.1/README.md
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.1.2/pytest.ini
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/args.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/base.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/health.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.1.2/src/es_wait/task.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.1.2/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.1.2/README.md
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.1.2/PKG-INFO
```

### Comparing `es_wait-0.1.1/src/es_wait/args.py` & `es_wait-0.1.2/src/es_wait/args.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.1/src/es_wait/base.py` & `es_wait-0.1.2/src/es_wait/base.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.1/src/es_wait/exists.py` & `es_wait-0.1.2/src/es_wait/exists.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
             pause: float = 1.5,
             timeout: float = 15,
             name: str = None,
             kind: str = None
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Exists')
-        self.empty_check('name')
-        self.empty_check('kind')
         self.name = name
         self.kind = kind
+        self.empty_check('name')
+        self.empty_check('kind')
         self.checkid = f'check for {self.kindmap} {name} to exist'
 
     @property
     def check(self) -> bool:
         """
         Check if the named entity exists, based on kind
         """
```

### Comparing `es_wait-0.1.1/src/es_wait/health.py` & `es_wait-0.1.2/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.1/src/es_wait/relocate.py` & `es_wait-0.1.2/src/es_wait/relocate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
             action: t.Optional[str] = None,
             pause: float = 9,
             timeout: float = -1,
             name: str = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
-        self.empty_check(name)
         self.name = name
+        self.empty_check(name)
         self.checkid = f'check for the {self.name} index relocation process to complete'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.state`
         with a given index to check if all of the shards for that index are in the ``STARTED``
```

### Comparing `es_wait-0.1.1/src/es_wait/restore.py` & `es_wait-0.1.2/src/es_wait/restore.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
             action: t.Optional[str] = None,
             pause: float = 9,
             timeout: float = -1,
             index_list: t.Sequence[str] = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
-        self.empty_check(index_list)
         self.index_list = index_list
+        self.empty_check(index_list)
         self.checkid = 'check for completion of index_list restoration from snapshot'
 
     @property
     def check(self) -> bool:
         """
         Calls `client.indices.` :py:meth:`~.elasticsearch.client.IndicesClient.recovery`
         with a list of indices to check for complete recovery.  It will return ``True`` if recovery
```

### Comparing `es_wait-0.1.1/src/es_wait/snapshot.py` & `es_wait-0.1.2/src/es_wait/snapshot.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
             pause: float = 9,
             timeout: float = -1,
             snapshot: str = None,
             repository: str = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
-        self.empty_check(snapshot)
-        self.empty_check(repository)
         self.snapshot = snapshot
         self.repository = repository
+        self.empty_check(snapshot)
+        self.empty_check(repository)
         self.checkid = f'check for snapshot {self.snapshot} completion'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.snapshot.` :py:meth:`~.elasticsearch.client.SnapshotClient.get`
         and tests to see whether the snapshot is complete, and if so, with what status.  It will log
```

### Comparing `es_wait-0.1.1/src/es_wait/task.py` & `es_wait-0.1.2/src/es_wait/task.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
             action: t.Literal['forcemerge', 'reindex', 'update_by_query'] = None,
             pause: float = 9,
             timeout: float = -1,
             task_id: str = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
-        self.empty_check(task_id)
         self.task_id = task_id
+        self.empty_check(task_id)
         self.task_data = None
         self.task = None
         self.checkid = f'check for the {self.action} task to complete'
 
     @property
     def check(self) -> bool:
         """
```

### Comparing `es_wait-0.1.1/.gitignore` & `es_wait-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.1/LICENSE` & `es_wait-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.1/pyproject.toml` & `es_wait-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.1/PKG-INFO` & `es_wait-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.1.1
+Version: 0.1.2
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

