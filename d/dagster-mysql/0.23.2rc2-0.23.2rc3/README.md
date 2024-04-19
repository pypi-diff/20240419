# Comparing `tmp/dagster-mysql-0.23.2rc2.tar.gz` & `tmp/dagster-mysql-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mysql-0.23.2rc2.tar", last modified: Tue Apr 16 20:37:35 2024, max compression
+gzip compressed data, was "dagster-mysql-0.23.2rc3.tar", last modified: Thu Apr 18 21:16:51 2024, max compression
```

## Comparing `dagster-mysql-0.23.2rc2.tar` & `dagster-mysql-0.23.2rc3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:35.380220 dagster-mysql-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      591 2024-04-16 20:37:35.380220 dagster-mysql-0.23.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:35.376219 dagster-mysql-0.23.2rc2/dagster_mysql/
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:35.376219 dagster-mysql-0.23.2rc2/dagster_mysql/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/alembic/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:35.376219 dagster-mysql-0.23.2rc2/dagster_mysql/event_log/
--rw-r--r--   0 root         (0) root         (0)       68 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8525 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/event_log/event_log.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:35.380220 dagster-mysql-0.23.2rc2/dagster_mysql/run_storage/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/run_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7307 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/run_storage/run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:35.380220 dagster-mysql-0.23.2rc2/dagster_mysql/schedule_storage/
--rw-r--r--   0 root         (0) root         (0)       75 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/schedule_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7590 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/schedule_storage/schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     3742 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/storage.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/dagster_mysql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:35.376219 dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      591 2024-04-16 20:37:35.000000 dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2024-04-16 20:37:35.000000 dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:37:35.000000 dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:37:35.000000 dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2024-04-16 20:37:35.000000 dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 20:37:35.000000 dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-16 20:37:35.380220 dagster-mysql-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1289 2024-04-16 20:26:55.000000 dagster-mysql-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:51.733768 dagster-mysql-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      591 2024-04-18 21:16:51.737768 dagster-mysql-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:51.729768 dagster-mysql-0.23.2rc3/dagster_mysql/
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:51.729768 dagster-mysql-0.23.2rc3/dagster_mysql/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/alembic/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:51.729768 dagster-mysql-0.23.2rc3/dagster_mysql/event_log/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8490 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/event_log/event_log.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:51.733768 dagster-mysql-0.23.2rc3/dagster_mysql/run_storage/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/run_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7307 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/run_storage/run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:51.733768 dagster-mysql-0.23.2rc3/dagster_mysql/schedule_storage/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/schedule_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/schedule_storage/schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/storage.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/dagster_mysql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:51.729768 dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      591 2024-04-18 21:16:51.000000 dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2024-04-18 21:16:51.000000 dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:16:51.000000 dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:16:51.000000 dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-18 21:16:51.000000 dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 21:16:51.000000 dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-18 21:16:51.737768 dagster-mysql-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-04-18 21:10:09.000000 dagster-mysql-0.23.2rc3/setup.py
```

### Comparing `dagster-mysql-0.23.2rc2/LICENSE` & `dagster-mysql-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.2rc2/PKG-INFO` & `dagster-mysql-0.23.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql/alembic/alembic.ini` & `dagster-mysql-0.23.2rc3/dagster_mysql/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql/event_log/event_log.py` & `dagster-mysql-0.23.2rc3/dagster_mysql/event_log/event_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,17 +54,15 @@
     :py:class:`~dagster.IntSource` and can be configured from environment variables.
 
     """
 
     def __init__(self, mysql_url: str, inst_data: Optional[ConfigurableClassData] = None):
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
         self.mysql_url = check.str_param(mysql_url, "mysql_url")
-        self._disposed = False
-
-        self._event_watcher = SqlPollingEventWatcher(self)
+        self._event_watcher: Optional[SqlPollingEventWatcher] = None
 
         # Default to not holding any connections open to prevent accumulating connections per DagsterInstance
         self._engine = create_engine(
             self.mysql_url,
             isolation_level=mysql_isolation_level(),
             poolclass=db_pool.NullPool,
         )
@@ -196,28 +194,26 @@
         super(MySQLEventLogStorage, self).enable_secondary_index(name)
         if name in self._secondary_index_cache:
             del self._secondary_index_cache[name]
 
     def watch(self, run_id: str, cursor: Optional[str], callback: EventHandlerFn) -> None:
         if cursor and EventLogCursor.parse(cursor).is_offset_cursor():
             check.failed("Cannot call `watch` with an offset cursor")
-        self._event_watcher.watch_run(run_id, cursor, callback)
 
-    def end_watch(self, run_id: str, handler: EventHandlerFn) -> None:
-        self._event_watcher.unwatch_run(run_id, handler)
+        if self._event_watcher is None:
+            self._event_watcher = SqlPollingEventWatcher(self)
 
-    @property
-    def event_watcher(self) -> SqlPollingEventWatcher:
-        return self._event_watcher
+        self._event_watcher.watch_run(run_id, cursor, callback)
 
-    def __del__(self) -> None:
-        self.dispose()
+    def end_watch(self, run_id: str, handler: EventHandlerFn) -> None:
+        if self._event_watcher:
+            self._event_watcher.unwatch_run(run_id, handler)
 
     def dispose(self) -> None:
-        if not self._disposed:
-            self._disposed = True
+        if self._event_watcher:
             self._event_watcher.close()
+            self._event_watcher = None
 
     def alembic_version(self) -> AlembicVersion:
         alembic_config = mysql_alembic_config(__file__)
         with self._connect() as conn:
             return check_alembic_revision(alembic_config, conn)
```

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql/run_storage/run_storage.py` & `dagster-mysql-0.23.2rc3/dagster_mysql/run_storage/run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql/schedule_storage/schedule_storage.py` & `dagster-mysql-0.23.2rc3/dagster_mysql/schedule_storage/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql/storage.py` & `dagster-mysql-0.23.2rc3/dagster_mysql/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql/utils.py` & `dagster-mysql-0.23.2rc3/dagster_mysql/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/PKG-INFO` & `dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mysql-0.23.2rc2/dagster_mysql.egg-info/SOURCES.txt` & `dagster-mysql-0.23.2rc3/dagster_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.2rc2/setup.py` & `dagster-mysql-0.23.2rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     package_data={
         "dagster-mysql": [
             "dagster_mysql/alembic/*",
         ]
     },
     include_package_data=True,
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.2rc2", "mysql-connector-python"],
+    install_requires=["dagster==1.7.2rc3", "mysql-connector-python"],
     zip_safe=False,
 )
```

