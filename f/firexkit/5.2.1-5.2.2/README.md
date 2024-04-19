# Comparing `tmp/firexkit-5.2.1.tar.gz` & `tmp/firexkit-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexkit-5.2.1.tar", last modified: Tue Mar  5 21:55:50 2024, max compression
+gzip compressed data, was "firexkit-5.2.2.tar", last modified: Fri Apr 19 21:52:42 2024, max compression
```

## Comparing `firexkit-5.2.1.tar` & `firexkit-5.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-03-05 21:55:50.046508 firexkit-5.2.1/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2024-03-05 21:55:39.000000 firexkit-5.2.1/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       73 2024-03-05 21:55:39.000000 firexkit-5.2.1/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-03-05 21:55:50.046508 firexkit-5.2.1/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       38 2024-03-05 21:55:39.000000 firexkit-5.2.1/README.md
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-03-05 21:55:50.047508 firexkit-5.2.1/firexkit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/__init__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2024-03-05 21:55:50.047508 firexkit-5.2.1/firexkit/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11286 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/argument_conversion.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6941 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/bag_of_goodies.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2957 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/broker.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8370 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/chain.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1327 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/firex_exceptions.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1004 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/firexkit_common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3178 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/inspect.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-03-05 21:55:50.045508 firexkit-5.2.1/firexkit/install_resources/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      482 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/install_resources/cloud-ci-install-configs.json
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1938 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/memory_utils.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       82 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/permissions.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3315 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/proc_utils.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-03-05 21:55:50.046508 firexkit-5.2.1/firexkit/resources/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3448 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/resources/firex.css
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7676 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/resources/firex_logo.png
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      836 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/resources.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    34337 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/result.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3358 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/revoke.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    69110 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/task.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-03-05 21:55:50.046508 firexkit-5.2.1/firexkit/templates/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      300 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/templates/link.html
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2874 2024-03-05 21:55:39.000000 firexkit-5.2.1/firexkit/templates/log_template.html
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-03-05 21:55:50.045508 firexkit-5.2.1/firexkit.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-03-05 21:55:50.000000 firexkit-5.2.1/firexkit.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      833 2024-03-05 21:55:50.000000 firexkit-5.2.1/firexkit.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-03-05 21:55:50.000000 firexkit-5.2.1/firexkit.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       34 2024-03-05 21:55:50.000000 firexkit-5.2.1/firexkit.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       21 2024-03-05 21:55:50.000000 firexkit-5.2.1/firexkit.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2024-03-05 21:55:50.000000 firexkit-5.2.1/firexkit.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-03-05 21:55:50.000000 firexkit-5.2.1/firexkit.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2024-03-05 21:55:50.047508 firexkit-5.2.1/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      681 2024-03-05 21:55:39.000000 firexkit-5.2.1/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-03-05 21:55:39.000000 firexkit-5.2.1/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.083270 firexkit-5.2.2/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2024-04-19 21:52:17.000000 firexkit-5.2.2/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       73 2024-04-19 21:52:17.000000 firexkit-5.2.2/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-04-19 21:52:42.083270 firexkit-5.2.2/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       38 2024-04-19 21:52:17.000000 firexkit-5.2.2/README.md
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.084270 firexkit-5.2.2/firexkit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/__init__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2024-04-19 21:52:42.084270 firexkit-5.2.2/firexkit/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11286 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/argument_conversion.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6941 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/bag_of_goodies.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2957 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/broker.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8370 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/chain.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1327 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/firex_exceptions.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1004 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/firexkit_common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3178 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/inspect.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.082270 firexkit-5.2.2/firexkit/install_resources/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      482 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/install_resources/cloud-ci-install-configs.json
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1938 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/memory_utils.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       82 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/permissions.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3315 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/proc_utils.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.083270 firexkit-5.2.2/firexkit/resources/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3448 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/resources/firex.css
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7676 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/resources/firex_logo.png
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      836 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/resources.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    34337 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/result.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3358 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/revoke.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70465 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/task.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.083270 firexkit-5.2.2/firexkit/templates/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      300 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/templates/link.html
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2874 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/templates/log_template.html
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.082270 firexkit-5.2.2/firexkit.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      833 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       34 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       21 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2024-04-19 21:52:42.084270 firexkit-5.2.2/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      681 2024-04-19 21:52:18.000000 firexkit-5.2.2/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-04-19 21:52:18.000000 firexkit-5.2.2/versioneer.py
```

### Comparing `firexkit-5.2.1/LICENSE` & `firexkit-5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/argument_conversion.py` & `firexkit-5.2.2/firexkit/argument_conversion.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/bag_of_goodies.py` & `firexkit-5.2.2/firexkit/bag_of_goodies.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/broker.py` & `firexkit-5.2.2/firexkit/broker.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/chain.py` & `firexkit-5.2.2/firexkit/chain.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/firex_exceptions.py` & `firexkit-5.2.2/firexkit/firex_exceptions.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/firexkit_common.py` & `firexkit-5.2.2/firexkit/firexkit_common.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/inspect.py` & `firexkit-5.2.2/firexkit/inspect.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/memory_utils.py` & `firexkit-5.2.2/firexkit/memory_utils.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/proc_utils.py` & `firexkit-5.2.2/firexkit/proc_utils.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/resources/firex.css` & `firexkit-5.2.2/firexkit/resources/firex.css`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/resources/firex_logo.png` & `firexkit-5.2.2/firexkit/resources/firex_logo.png`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/resources.py` & `firexkit-5.2.2/firexkit/resources.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/result.py` & `firexkit-5.2.2/firexkit/result.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/revoke.py` & `firexkit-5.2.2/firexkit/revoke.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit/task.py` & `firexkit-5.2.2/firexkit/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 REPLACEMENT_TASK_NAME_POSTFIX = '_orig'
 FIREX_REVOKE_COMPLETE_EVENT_TYPE = 'task-firex-revoked'
 
 REDIS_DB_KEY_FOR_RESULTS_WITH_REPORTS = 'FIREX_RESULTS_WITH_REPORTS'
 REDIS_DB_KEY_PREFIX_FOR_ENQUEUE_ONCE_UID = 'ENQUEUE_CHILD_ONCE_UID_'
 REDIS_DB_KEY_PREFIX_FOR_ENQUEUE_ONCE_COUNT = 'ENQUEUE_CHILD_ONCE_COUNT_'
+REDIS_DB_KEY_PREFIX_FOR_CACHE_ENABLED_UID = 'CACHE_ENABLED'
 
 logger = get_task_logger(__name__)
 
 ################################################################
 # Monkey patching
 _orig_chain_apply_async__ = _chain.apply_async
 
@@ -248,35 +249,52 @@
         return super().setdefault(*args, **kwargs)
 
     def update(self, *args, **kwargs):
         self.warn()
         super().update(*args, **kwargs)
 
 
+def get_cache_enabled_uid_dbkey(cache_key_info: str) -> str:
+    return f'{REDIS_DB_KEY_PREFIX_FOR_CACHE_ENABLED_UID}{cache_key_info}'
+
+
 def get_enqueue_child_once_uid_dbkey(enqueue_once_key: str) -> str:
     return f'{REDIS_DB_KEY_PREFIX_FOR_ENQUEUE_ONCE_UID}{enqueue_once_key}'
 
 
 def get_enqueue_child_once_count_dbkey(enqueue_once_key: str) -> str:
     return f'{REDIS_DB_KEY_PREFIX_FOR_ENQUEUE_ONCE_COUNT}{enqueue_once_key}'
 
 
 def get_current_enqueue_child_once_uid_dbkeys(db) -> list[str]:
     return db.client.keys(get_enqueue_child_once_uid_dbkey('*'))
 
 
+def get_current_cache_enabled_uid_dbkeys(db) -> list[str]:
+    return db.client.keys(get_cache_enabled_uid_dbkey('*'))
+
+
 def get_current_enqueue_child_once_uids(db) -> set[str]:
     """Returns a set of all task/result ids that were executed with enqueue_once"""
 
     # First, we need to find all the enqueue_once keys
     keys = get_current_enqueue_child_once_uid_dbkeys(db)
     # Then we get the task/result ids stored in those keys
     return {v.decode() for v in db.mget(keys)}
 
 
+def get_current_cache_enabled_uids(db) -> set[str]:
+    """Returns a set of all task/result ids whose tasks were cache-enabled"""
+
+    # First, we need to find all the cache_enabled keys
+    keys = get_current_cache_enabled_uid_dbkeys(db)
+    # Then we get the task/result ids stored in those keys
+    return {v.decode() for v in db.mget(keys)}
+
+
 def add_task_result_with_report_to_db(db, result_id: str):
     """Append task id to the list of tasks with reports (e.g. tasks decorated with @email)"""
     db.client.rpush(REDIS_DB_KEY_FOR_RESULTS_WITH_REPORTS, result_id)
 
 
 def get_current_reports_uids(db) -> set[str]:
     """Return the list of task/results ids for all tasks with reports (e.g. @email) executed so far"""
@@ -681,15 +699,15 @@
         if not self._decorated_return_keys and self._task_return_keys:
             # This is only used if the @app.task(returns=) is used
             result = self.convert_returns_to_dict(self._task_return_keys, result)
         return result
 
     def _get_cache_key(self):
         # Need a sting hash of name + all_args
-        return str((self.name,) + tuple(sorted(self.all_args.items())))
+        return get_cache_enabled_uid_dbkey(str((self.name,) + tuple(sorted(self.all_args.items()))))
 
     def _cache_get(self, cache_key):
         cached_uuid = self.backend.get(cache_key)
         if cached_uuid is None:
             raise NotInCache()
         cached_uuid = cached_uuid.decode()
         logger.info(f'[Caching] found entry for key {cache_key!r} at {cached_uuid!r}')
@@ -905,40 +923,52 @@
         child_results = self.pending_enqueued_children if pending_only else self.enqueued_children
         self.wait_for_specific_children(child_results=child_results, **kwargs)
 
     def forget_child_result(self,
                             child_result: AsyncResult,
                             do_not_forget_report_nodes: bool = True,
                             do_not_forget_enqueue_once_nodes: bool = True,
+                            do_not_forget_cache_enabled_tasks_results: bool = True,
                             **kwargs):
 
         """Forget results of the tree rooted at the "chain-head" of child_result, while skipping subtrees in
         skip_subtree_nodes, as well as nodes in do_not_forget_nodes.
 
         If do_not_forget_report_nodes is True (default), do not forget report nodes (e.g. nodes decorated with @email)
 
         If do_not_forget_enqueue_once_nodes is True (default), do not forget subtrees rooted at nodes that were enqueued
         with enqueue_once
+
+        If do_not_forget_cache_enabled_tasks_results is True (default), do not forget subtrees rooted at nodes that belong to
+        services with cached=True
         """
         logger.debug('Forgetting results')
 
-        enqueue_once_subtree_nodes = None
+        skip_subtree_nodes: set[str] = set()
+
         if do_not_forget_enqueue_once_nodes:
             enqueue_once_subtree_nodes = get_current_enqueue_child_once_uids(self.backend)
             if enqueue_once_subtree_nodes:
+                skip_subtree_nodes.update(enqueue_once_subtree_nodes)
                 logger.debug(f'Enqueue once subtree nodes: {enqueue_once_subtree_nodes}')
 
+        if do_not_forget_cache_enabled_tasks_results:
+            cache_enabled_subtree_nodes = get_current_cache_enabled_uids(self.backend)
+            if cache_enabled_subtree_nodes:
+                skip_subtree_nodes.update(cache_enabled_subtree_nodes)
+                logger.debug(f'Cache-enabled  subtree nodes: {cache_enabled_subtree_nodes}')
+
         report_nodes = None
         if do_not_forget_report_nodes:
             report_nodes = get_current_reports_uids(self.backend)
             if report_nodes:
                 logger.debug(f'Report nodes: {report_nodes}')
 
         forget_chain_results(child_result,
-                             skip_subtree_nodes=enqueue_once_subtree_nodes,
+                             skip_subtree_nodes=skip_subtree_nodes,
                              do_not_forget_nodes=report_nodes,
                              **kwargs)
         # Since we forget the child, we need to also remove it from the list of enqueued_children
         self._remove_enqueued_child(child_result)
 
     def forget_specific_children_results(self, child_results: list[AsyncResult], **kwargs):
         """Forget results for the explicitly provided child_results"""
```

### Comparing `firexkit-5.2.1/firexkit/templates/log_template.html` & `firexkit-5.2.2/firexkit/templates/log_template.html`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/firexkit.egg-info/SOURCES.txt` & `firexkit-5.2.2/firexkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/setup.py` & `firexkit-5.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.1/versioneer.py` & `firexkit-5.2.2/versioneer.py`

 * *Files identical despite different names*

