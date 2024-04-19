# Comparing `tmp/echoloader-0.1.95.tar.gz` & `tmp/echoloader-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoloader-0.1.95.tar", max compression
+gzip compressed data, was "echoloader-0.1.96.tar", max compression
```

## Comparing `echoloader-0.1.95.tar` & `echoloader-0.1.96.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       24 2024-04-03 13:28:22.687204 echoloader-0.1.95/echoloader/__init__.py
--rw-r--r--   0        0        0      143 2023-11-20 16:09:52.768334 echoloader-0.1.95/echoloader/__main__.py
--rw-r--r--   0        0        0      931 2024-01-16 15:07:01.945522 echoloader-0.1.95/echoloader/config.py
--rw-r--r--   0        0        0     1856 2024-02-13 06:10:05.802876 echoloader-0.1.95/echoloader/dimse/__init__.py
--rw-r--r--   0        0        0     3125 2024-02-13 06:10:05.804882 echoloader-0.1.95/echoloader/dimse/dimse.py
--rw-r--r--   0        0        0      882 2024-02-13 06:10:05.805881 echoloader-0.1.95/echoloader/dimse/fs.py
--rw-r--r--   0        0        0      367 2024-02-13 06:10:05.807885 echoloader-0.1.95/echoloader/dimse/store.py
--rw-r--r--   0        0        0     2141 2024-02-13 06:10:05.808881 echoloader-0.1.95/echoloader/dimse/tls.py
--rw-r--r--   0        0        0    11166 2024-02-13 06:10:05.810887 echoloader-0.1.95/echoloader/lib/hl7.py
--rw-r--r--   0        0        0     2954 2024-02-13 06:10:05.811881 echoloader-0.1.95/echoloader/login.py
--rw-r--r--   0        0        0      979 2024-02-13 06:10:05.813882 echoloader-0.1.95/echoloader/qt.py
--rw-r--r--   0        0        0    17175 2024-03-23 07:31:12.576868 echoloader-0.1.95/echoloader/results_sync/__init__.py
--rw-r--r--   0        0        0     2937 2024-02-13 06:10:05.818041 echoloader-0.1.95/echoloader/results_sync/hl7_sync.py
--rw-r--r--   0        0        0     4724 2024-03-23 07:31:12.577918 echoloader-0.1.95/echoloader/sync.py
--rw-r--r--   0        0        0    41572 2024-04-03 13:28:22.690204 echoloader-0.1.95/echoloader/watcher.py
--rw-r--r--   0        0        0      849 2024-04-03 13:28:22.695729 echoloader-0.1.95/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 echoloader-0.1.95/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-19 14:36:43.618282 echoloader-0.1.96/echoloader/__init__.py
+-rw-r--r--   0        0        0      143 2023-11-20 16:09:52.768334 echoloader-0.1.96/echoloader/__main__.py
+-rw-r--r--   0        0        0      931 2024-01-16 15:07:01.945522 echoloader-0.1.96/echoloader/config.py
+-rw-r--r--   0        0        0     1856 2024-02-13 06:10:05.802876 echoloader-0.1.96/echoloader/dimse/__init__.py
+-rw-r--r--   0        0        0     3125 2024-02-13 06:10:05.804882 echoloader-0.1.96/echoloader/dimse/dimse.py
+-rw-r--r--   0        0        0      882 2024-02-13 06:10:05.805881 echoloader-0.1.96/echoloader/dimse/fs.py
+-rw-r--r--   0        0        0      367 2024-02-13 06:10:05.807885 echoloader-0.1.96/echoloader/dimse/store.py
+-rw-r--r--   0        0        0     2141 2024-02-13 06:10:05.808881 echoloader-0.1.96/echoloader/dimse/tls.py
+-rw-r--r--   0        0        0    11166 2024-02-13 06:10:05.810887 echoloader-0.1.96/echoloader/lib/hl7.py
+-rw-r--r--   0        0        0     2954 2024-02-13 06:10:05.811881 echoloader-0.1.96/echoloader/login.py
+-rw-r--r--   0        0        0      979 2024-02-13 06:10:05.813882 echoloader-0.1.96/echoloader/qt.py
+-rw-r--r--   0        0        0    17177 2024-04-19 06:41:21.735964 echoloader-0.1.96/echoloader/results_sync/__init__.py
+-rw-r--r--   0        0        0     2937 2024-02-13 06:10:05.818041 echoloader-0.1.96/echoloader/results_sync/hl7_sync.py
+-rw-r--r--   0        0        0     4724 2024-03-23 07:31:12.577918 echoloader-0.1.96/echoloader/sync.py
+-rw-r--r--   0        0        0    41608 2024-04-19 14:36:43.619293 echoloader-0.1.96/echoloader/watcher.py
+-rw-r--r--   0        0        0      849 2024-04-19 14:36:43.624300 echoloader-0.1.96/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 echoloader-0.1.96/PKG-INFO
```

### Comparing `echoloader-0.1.95/echoloader/config.py` & `echoloader-0.1.96/echoloader/config.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/dimse/__init__.py` & `echoloader-0.1.96/echoloader/dimse/__init__.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/dimse/dimse.py` & `echoloader-0.1.96/echoloader/dimse/dimse.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/dimse/fs.py` & `echoloader-0.1.96/echoloader/dimse/fs.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/dimse/tls.py` & `echoloader-0.1.96/echoloader/dimse/tls.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/lib/hl7.py` & `echoloader-0.1.96/echoloader/lib/hl7.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/login.py` & `echoloader-0.1.96/echoloader/login.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/qt.py` & `echoloader-0.1.96/echoloader/qt.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/results_sync/__init__.py` & `echoloader-0.1.96/echoloader/results_sync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
                 sync_status = 'SUCCESS'
             elif self.sync_status_success.get(destination_id) and self.sync_status_failed.get(destination_id):
                 sync_status = 'PARTIAL'
             elif self.sync_status_failed.get(destination_id):
                 sync_status = 'FAILED'
 
             if self.sync_status_failed.get(destination_id):
-                error_summary = ', '.join(self.sync_status_failed[destination_id])
+                error_summary = '<br>'.join(self.sync_status_failed[destination_id])
 
             if self.is_echoloader and sync_destination.get('sync_log_id'):
                 self.update_sync_status(sync_destination, sync_status, error_summary)
                 continue
 
             sync_log = {
                 'sync_source': self.sync_source,
```

### Comparing `echoloader-0.1.95/echoloader/results_sync/hl7_sync.py` & `echoloader-0.1.96/echoloader/results_sync/hl7_sync.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/sync.py` & `echoloader-0.1.96/echoloader/sync.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.95/echoloader/watcher.py` & `echoloader-0.1.96/echoloader/watcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1050,24 +1050,26 @@
                 httpd = ThreadingHTTPServer(server_address=('0.0.0.0', args.proxy),
                                             RequestHandlerClass=create_proxy(args))
                 thread = threading.Thread(target=httpd.serve_forever)
                 thread.start()
             while observer or handler.processing() or sync or pacs or pacs_tls or httpd:
                 gc.collect()
                 if args.app_config and args.auth:
+                    app_config = None
                     try:
                         args.auth.get_user()
                         app_config = args.auth.user.get('dicom_router_config', {}).get('general', {})
-                        if app_config != args.app_config:
-                            logger.warning('Configuration updated')
-                            logger.warning(f'Old configuration: {json.dumps(args.app_config)}')
-                            logger.warning(f'New configuration: {json.dumps(app_config)}')
-                            raise ConfigUpdatedException()
                     except Exception as exc:
                         logger.error(f'Failed to get user due to {exc}')
+
+                    if app_config and app_config != args.app_config:
+                        logger.warning('Configuration updated')
+                        logger.warning(f'Old configuration: {json.dumps(args.app_config)}')
+                        logger.warning(f'New configuration: {json.dumps(app_config)}')
+                        raise ConfigUpdatedException()
                 time.sleep(5)
             break
         except KeyboardInterrupt:
             break
         except ConfigUpdatedException:
             pass
         finally:
```

### Comparing `echoloader-0.1.95/pyproject.toml` & `echoloader-0.1.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "echoloader"
-version = "0.1.95"
+version = "0.1.96"
 description = ""
 authors = ["mathias <mathias@us2.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 requests = "^2.27.1"
 watchdog = "^2.1.7"
```

### Comparing `echoloader-0.1.95/PKG-INFO` & `echoloader-0.1.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoloader
-Version: 0.1.95
+Version: 0.1.96
 Summary: 
 Author: mathias
 Author-email: mathias@us2.ai
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: av (==10.0.0)
```

