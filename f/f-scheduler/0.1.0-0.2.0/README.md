# Comparing `tmp/f-scheduler-0.1.0.tar.gz` & `tmp/f_scheduler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f-scheduler-0.1.0.tar", last modified: Tue Mar 12 02:26:40 2024, max compression
+gzip compressed data, was "f_scheduler-0.2.0.tar", last modified: Fri Apr 19 11:30:53 2024, max compression
```

## Comparing `f-scheduler-0.1.0.tar` & `f_scheduler-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:40.058479 f-scheduler-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-12 02:26:40.058479 f-scheduler-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:40.054479 f-scheduler-0.1.0/f_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:40.058479 f-scheduler-0.1.0/f_scheduler/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/modules/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:40.058479 f-scheduler-0.1.0/f_scheduler/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/operators/base_op.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/operators/condition_op.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/operators/function_op.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/operators/iter_function_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:40.058479 f-scheduler-0.1.0/f_scheduler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/f_scheduler/utils/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 02:26:40.058479 f-scheduler-0.1.0/f_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-12 02:26:40.000000 f-scheduler-0.1.0/f_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-12 02:26:40.000000 f-scheduler-0.1.0/f_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 02:26:40.000000 f-scheduler-0.1.0/f_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-12 02:26:40.000000 f-scheduler-0.1.0/f_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-12 02:26:40.000000 f-scheduler-0.1.0/f_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-12 02:26:33.000000 f-scheduler-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 02:26:40.058479 f-scheduler-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:53.636348 f_scheduler-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-19 11:30:53.636348 f_scheduler-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:53.632348 f_scheduler-0.2.0/f_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:53.632348 f_scheduler-0.2.0/f_scheduler/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/modules/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:53.636348 f_scheduler-0.2.0/f_scheduler/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/operators/base_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/operators/condition_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/operators/function_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/operators/iter_function_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:53.636348 f_scheduler-0.2.0/f_scheduler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/f_scheduler/utils/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:30:53.636348 f_scheduler-0.2.0/f_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-19 11:30:53.000000 f_scheduler-0.2.0/f_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 11:30:53.000000 f_scheduler-0.2.0/f_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:30:53.000000 f_scheduler-0.2.0/f_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 11:30:53.000000 f_scheduler-0.2.0/f_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 11:30:53.000000 f_scheduler-0.2.0/f_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-19 11:30:49.000000 f_scheduler-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:30:53.636348 f_scheduler-0.2.0/setup.cfg
```

### Comparing `f-scheduler-0.1.0/LICENSE` & `f_scheduler-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f-scheduler-0.1.0/PKG-INFO` & `f_scheduler-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f-scheduler
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simplify Function Scheduler with Python 3
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/f-scheduler
 Project-URL: Bug Tracker, https://github.com/minwook-shin/f-scheduler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `f-scheduler-0.1.0/README.md` & `f_scheduler-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `f-scheduler-0.1.0/f_scheduler/modules/dag.py` & `f_scheduler-0.2.0/f_scheduler/modules/dag.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,7 +18,14 @@
         self.tasks.clear()
 
     def get_return_value(self, task_id):
         return self.tasks[task_id].return_value
 
     def get_all_tasks(self):
         return self.tasks
+
+    def update_task(self, task_id, new_param):
+        task = self.tasks[task_id]
+        if task:
+            task.param = new_param
+        else:
+            print(f"No task found with id: {task_id}")
```

### Comparing `f-scheduler-0.1.0/f_scheduler/operators/function_op.py` & `f_scheduler-0.2.0/f_scheduler/operators/function_op.py`

 * *Files identical despite different names*

### Comparing `f-scheduler-0.1.0/f_scheduler/operators/iter_function_op.py` & `f_scheduler-0.2.0/f_scheduler/operators/iter_function_op.py`

 * *Files identical despite different names*

### Comparing `f-scheduler-0.1.0/f_scheduler.egg-info/PKG-INFO` & `f_scheduler-0.2.0/f_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f-scheduler
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simplify Function Scheduler with Python 3
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/f-scheduler
 Project-URL: Bug Tracker, https://github.com/minwook-shin/f-scheduler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `f-scheduler-0.1.0/f_scheduler.egg-info/SOURCES.txt` & `f_scheduler-0.2.0/f_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `f-scheduler-0.1.0/pyproject.toml` & `f_scheduler-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools.packages.find]
 include = ['f_scheduler*']
 exclude = ['f_scheduler*tests']
 
 [project]
 name = "f-scheduler"
-version = "0.1.0"
+version = "0.2.0"
 description = "Simplify Function Scheduler with Python 3"
 authors = [
     {name = "minwook-shin", email = "minwook0106@gmail.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

