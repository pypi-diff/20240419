# Comparing `tmp/tickthon-0.2.8.tar.gz` & `tmp/tickthon-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickthon-0.2.8.tar", last modified: Wed Mar 13 02:25:55 2024, max compression
+gzip compressed data, was "tickthon-0.2.9.tar", last modified: Thu Mar 14 01:40:04 2024, max compression
```

## Comparing `tickthon-0.2.8.tar` & `tickthon-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:55.901619 tickthon-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-13 02:25:47.000000 tickthon-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-13 02:25:55.901619 tickthon-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-13 02:25:47.000000 tickthon-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-13 02:25:53.000000 tickthon-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 02:25:55.901619 tickthon-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:55.897619 tickthon-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:55.897619 tickthon-0.2.8/src/tickthon/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/_task_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/_ticktick_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:55.901619 tickthon-0.2.8/src/tickthon/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/data/day_log_words.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/data/ticktick_id_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/data/ticktick_list_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/data/ticktick_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/data/ticktick_task_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/expense_log_model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/task_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-03-13 02:25:47.000000 tickthon-0.2.8/src/tickthon/ticktick_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:55.901619 tickthon-0.2.8/src/tickthon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-13 02:25:55.000000 tickthon-0.2.8/src/tickthon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-13 02:25:55.000000 tickthon-0.2.8/src/tickthon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 02:25:55.000000 tickthon-0.2.8/src/tickthon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-13 02:25:55.000000 tickthon-0.2.8/src/tickthon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 02:25:55.000000 tickthon-0.2.8/src/tickthon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 02:25:55.901619 tickthon-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-13 02:25:47.000000 tickthon-0.2.8/tests/test_expense_log_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-13 02:25:47.000000 tickthon-0.2.8/tests/test_task_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-13 02:25:47.000000 tickthon-0.2.8/tests/test_ticktick_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-13 02:25:47.000000 tickthon-0.2.8/tests/test_ticktick_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 01:40:04.348022 tickthon-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-14 01:39:56.000000 tickthon-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-14 01:40:04.348022 tickthon-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-14 01:39:56.000000 tickthon-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-14 01:40:02.000000 tickthon-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 01:40:04.348022 tickthon-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 01:40:04.340022 tickthon-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 01:40:04.344022 tickthon-0.2.9/src/tickthon/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/_task_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/_ticktick_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 01:40:04.344022 tickthon-0.2.9/src/tickthon/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/data/day_log_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/data/ticktick_id_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/data/ticktick_list_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/data/ticktick_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/data/ticktick_task_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/expense_log_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/task_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-03-14 01:39:56.000000 tickthon-0.2.9/src/tickthon/ticktick_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 01:40:04.344022 tickthon-0.2.9/src/tickthon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-14 01:40:04.000000 tickthon-0.2.9/src/tickthon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-14 01:40:04.000000 tickthon-0.2.9/src/tickthon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 01:40:04.000000 tickthon-0.2.9/src/tickthon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-14 01:40:04.000000 tickthon-0.2.9/src/tickthon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 01:40:04.000000 tickthon-0.2.9/src/tickthon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 01:40:04.344022 tickthon-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-14 01:39:56.000000 tickthon-0.2.9/tests/test_expense_log_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-14 01:39:56.000000 tickthon-0.2.9/tests/test_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-14 01:39:56.000000 tickthon-0.2.9/tests/test_ticktick_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-14 01:39:56.000000 tickthon-0.2.9/tests/test_ticktick_client.py
```

### Comparing `tickthon-0.2.8/LICENSE` & `tickthon-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/PKG-INFO` & `tickthon-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickthon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Yet another unofficial Ticktick API client, it is based on ticktick-py
 Author-email: anggelomos <anggelomos@outlook.com>
 Project-URL: repository, https://github.com/anggelomos/tickthon
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tickthon-0.2.8/README.md` & `tickthon-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/pyproject.toml` & `tickthon-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tickthon"
-version = "0.2.8"
+version = "0.2.9"
 description = "Yet another unofficial Ticktick API client, it is based on ticktick-py"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3.10",]
 dependencies = [ "requests", "attrs", "python-dateutil",]
 [[project.authors]]
 name = "anggelomos"
```

### Comparing `tickthon-0.2.8/src/tickthon/_task_utils.py` & `tickthon-0.2.9/src/tickthon/_task_utils.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/src/tickthon/_ticktick_api.py` & `tickthon-0.2.9/src/tickthon/_ticktick_api.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/src/tickthon/data/day_log_words.py` & `tickthon-0.2.9/src/tickthon/data/day_log_words.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/src/tickthon/data/ticktick_list_parameters.py` & `tickthon-0.2.9/src/tickthon/data/ticktick_list_parameters.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/src/tickthon/data/ticktick_payloads.py` & `tickthon-0.2.9/src/tickthon/data/ticktick_payloads.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/src/tickthon/data/ticktick_task_parameters.py` & `tickthon-0.2.9/src/tickthon/data/ticktick_task_parameters.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/src/tickthon/task_model.py` & `tickthon-0.2.9/src/tickthon/task_model.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/src/tickthon/ticktick_client.py` & `tickthon-0.2.9/src/tickthon/ticktick_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from ._ticktick_api import TicktickAPI
 from .data.ticktick_payloads import TicktickPayloads
 from .data.ticktick_id_keys import TicktickIdKeys as tik, TicktickFolderKeys as tfK
 from .data.ticktick_task_parameters import TicktickTaskParameters as ttp
 from .data.ticktick_list_parameters import TicktickListParameters as tlp
 from .task_model import Task
 from ._task_utils import (_is_task_an_expense_log, _is_task_active,
-                          dict_to_task, _parse_expense_log, _is_task_day_log, _is_day_log_a_highlight)
+                          dict_to_task, _parse_expense_log, _is_task_day_log, _is_day_log_a_highlight,
+                          _is_task_a_weight_measurement)
 
 current_date = datetime.utcnow()
 date_two_weeks_ago = (current_date - timedelta(days=14)).strftime("%Y-%m-%d")
 date_tomorrow = (current_date + timedelta(days=1)).strftime("%Y-%m-%d")
 
 
 class TicktickClient:
@@ -116,17 +117,16 @@
         self._cached_raw_active_tasks = raw_active_tasks
         self.all_active_tasks = self._parse_ticktick_tasks(raw_active_tasks, self.project_lists)
 
         self.all_day_logs = []
         self.expense_logs = []
         self.active_tasks = []
         for task in self.all_active_tasks:
-            # TODO: Add weight measurements once they are restored
-            # if _is_task_a_weight_measurement(task):
-            #     self.weight_measurements.append(task)
+            if _is_task_a_weight_measurement(task):
+                self.weight_measurements.append(task)
             if _is_task_day_log(task):
                 self.all_day_logs.append(task)
             elif _is_task_an_expense_log(task):
                 expense_log = _parse_expense_log(task)
                 if expense_log is not None:
                     self.expense_logs.append((task, expense_log))
             elif _is_task_active(task):
```

### Comparing `tickthon-0.2.8/src/tickthon.egg-info/PKG-INFO` & `tickthon-0.2.9/src/tickthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickthon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Yet another unofficial Ticktick API client, it is based on ticktick-py
 Author-email: anggelomos <anggelomos@outlook.com>
 Project-URL: repository, https://github.com/anggelomos/tickthon
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tickthon-0.2.8/src/tickthon.egg-info/SOURCES.txt` & `tickthon-0.2.9/src/tickthon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/tests/test_expense_log_model.py` & `tickthon-0.2.9/tests/test_expense_log_model.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/tests/test_task_model.py` & `tickthon-0.2.9/tests/test_task_model.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/tests/test_ticktick_api.py` & `tickthon-0.2.9/tests/test_ticktick_api.py`

 * *Files identical despite different names*

### Comparing `tickthon-0.2.8/tests/test_ticktick_client.py` & `tickthon-0.2.9/tests/test_ticktick_client.py`

 * *Files identical despite different names*

