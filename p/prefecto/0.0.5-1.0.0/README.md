# Comparing `tmp/prefecto-0.0.5.tar.gz` & `tmp/prefecto-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefecto-0.0.5.tar", last modified: Sun Aug 20 15:34:53 2023, max compression
+gzip compressed data, was "prefecto-1.0.0.tar", last modified: Fri Apr 19 17:02:34 2024, max compression
```

## Comparing `prefecto-0.0.5.tar` & `prefecto-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:53.923146 prefecto-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-20 15:34:02.000000 prefecto-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-20 15:34:53.923146 prefecto-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-20 15:34:02.000000 prefecto-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-20 15:34:02.000000 prefecto-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-20 15:34:53.923146 prefecto-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-20 15:34:02.000000 prefecto-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:53.919146 prefecto-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:53.923146 prefecto-0.0.5/src/prefecto/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-20 15:34:53.923146 prefecto-0.0.5/src/prefecto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/filesystems.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:53.923146 prefecto-0.0.5/src/prefecto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/serializers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/serializers/polars.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:53.923146 prefecto-0.0.5/src/prefecto/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-20 15:34:02.000000 prefecto-0.0.5/src/prefecto/testing/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:53.923146 prefecto-0.0.5/src/prefecto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-20 15:34:53.000000 prefecto-0.0.5/src/prefecto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-20 15:34:53.000000 prefecto-0.0.5/src/prefecto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-20 15:34:53.000000 prefecto-0.0.5/src/prefecto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-20 15:34:53.000000 prefecto-0.0.5/src/prefecto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-20 15:34:53.000000 prefecto-0.0.5/src/prefecto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-20 15:34:13.000000 prefecto-0.0.5/src/prefecto.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 15:34:53.923146 prefecto-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-20 15:34:02.000000 prefecto-0.0.5/tests/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-20 15:34:02.000000 prefecto-0.0.5/tests/test_filesystems.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-20 15:34:02.000000 prefecto-0.0.5/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-08-20 15:34:02.000000 prefecto-0.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:34.273749 prefecto-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 17:01:57.000000 prefecto-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-19 17:02:34.273749 prefecto-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-19 17:01:57.000000 prefecto-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-19 17:01:57.000000 prefecto-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:02:34.273749 prefecto-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 17:01:57.000000 prefecto-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:34.269749 prefecto-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:34.269749 prefecto-1.0.0/src/prefecto/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 17:01:57.000000 prefecto-1.0.0/src/prefecto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 17:02:34.273749 prefecto-1.0.0/src/prefecto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-19 17:01:57.000000 prefecto-1.0.0/src/prefecto/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:34.269749 prefecto-1.0.0/src/prefecto/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 17:01:57.000000 prefecto-1.0.0/src/prefecto/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-04-19 17:01:57.000000 prefecto-1.0.0/src/prefecto/concurrency/batch_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-19 17:01:57.000000 prefecto-1.0.0/src/prefecto/concurrency/kill_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-19 17:01:57.000000 prefecto-1.0.0/src/prefecto/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 17:01:57.000000 prefecto-1.0.0/src/prefecto/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:34.273749 prefecto-1.0.0/src/prefecto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-19 17:02:34.000000 prefecto-1.0.0/src/prefecto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-19 17:02:34.000000 prefecto-1.0.0/src/prefecto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:02:34.000000 prefecto-1.0.0/src/prefecto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 17:02:34.000000 prefecto-1.0.0/src/prefecto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 17:02:34.000000 prefecto-1.0.0/src/prefecto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:34.273749 prefecto-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-19 17:01:57.000000 prefecto-1.0.0/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-19 17:01:57.000000 prefecto-1.0.0/tests/test_logging.py
```

### Comparing `prefecto-0.0.5/LICENSE` & `prefecto-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.5/README.md` & `prefecto-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.5/src/prefecto/concurrency.py` & `prefecto-1.0.0/src/prefecto/concurrency/batch_task.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,97 @@
 """
-Tools to improve Prefect concurrency.
-
+Module to improve Prefect concurrency operations.
 """
+
 from __future__ import annotations
 
-from typing import Any, TypeVar
+from typing import TypeVar
 
 from prefect import unmapped
 from prefect.futures import PrefectFuture
 from prefect.tasks import Task
 from prefect.utilities.callables import get_call_parameters
 from typing_extensions import ParamSpec
 
-from . import logging, states
+from prefecto import logging, states
+from prefecto.concurrency.kill_switch import KillSwitch
 
 T = TypeVar("T")  # Generic type var for capturing the inner return type of async funcs
 R = TypeVar("R")  # The return type of the user's function
 P = ParamSpec("P")  # The parameters of the task
 P_i = ParamSpec("P_i")  # The type of each parameter
 
 MapArgument = list[P_i] | unmapped[P_i]
 Batch = dict[str, MapArgument]
 
 
 class BatchTask:
-    """Wraps a `Task` to perform `Task.map` in batches.
+    """Wraps a `Task` to perform `Task.map` in batches, reducing the number of
+    concurrent tasks, mellowing Prefect API requests, and allowing for faster
+    failure detection.
+
+    ```python
+    from prefect import flow, task
+    from prefecto.concurrency import BatchTask
+
+    @task
+    def add(a, b):
+        return a + b
+
+    @flow
+    def my_flow():
+        batch_add = BatchTask(add, 2)
+        return batch_add.map([1,2,3,4], [2,3,4,5])
+
+    ```
+
+    The `kill_switch` argument can be used to stop the execution of the task
+    after a certain condition is met.
+
+    ```python
+    from prefect import flow, task
+    from prefecto.concurrency import BatchTask, AnyFailedSwitch
 
-    Args:
+    @task
+    def add(a, b):
+        return a + b
 
-        task (Task): The task to wrap.
-        size (int): The size of the batches to perform `Task.map` on.
+    @flow
+    def my_flow():
+        batch_add = BatchTask(add, 2, kill_switch=AnyFailedSwitch())
+        # This will error on the first batch and stop the execution.
+        return batch_add.map([1,2,3,4], [1,'2',3,4])
+
+    ```
+
+    See [kill switches][src.prefecto.concurrency.kill_switch] for more information.
 
     """
 
-    def __init__(self, task: Task[P, R], size: int):
+    def __init__(
+        self, task: Task[P, R], size: int, kill_switch: KillSwitch | None = None
+    ):
+        """Wrap the `task` to be executed in batches of `size`.
+
+        Args:
+
+                task (Task): The task to wrap.
+                size (int): The size of the batches to perform `Task.map` on.
+                kill_switch (KillSwitch, optional): A kill switch to stop the execution of the task
+                    after a certain condition is met.
+        """
         self.task: Task = task
         self.size: int = size
 
+        if kill_switch is not None and not isinstance(kill_switch, KillSwitch):
+            raise TypeError(
+                f"Expected 'kill_switch' to be a subclass of 'KillSwitch', got {type(kill_switch)}."
+            )
+        self._kill_switch = kill_switch
+
     def _make_batches(self, **params: MapArgument) -> list[Batch]:
         """Create batches of arguments to pass to the `Task.map` calls.
 
         Args:
             **params (MapArgument): Keyword arguments where each value is an
             iterable of equal length or an `unmapped` object. Should be at least
             one non-`unmapped` argument.
@@ -199,13 +250,17 @@
             is_processing: bool = True
             while is_processing:
                 # If any future is still processing, loop and poll again.
                 # If all futures are terminal, break while loop and continue
                 if all(states.is_terminal(f.get_state()) for f in futures):
                     is_processing = False
 
+            if self._kill_switch is not None:
+                for f in futures:
+                    self._kill_switch.raise_if_triggered(f.get_state())
+
         # Map the last batch
         logger.debug(
             f"Mapping {self.task.name} batch {len(batches)} of {len(batches)}."
         )
         results.extend(self.task.map(**batches[-1]))
         return results
```

### Comparing `prefecto-0.0.5/src/prefecto/logging.py` & `prefecto-1.0.0/src/prefecto/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Prefect logging utilities.
 """
+
 from __future__ import annotations
 
 import logging
 
 from prefect.logging import get_run_logger
```

### Comparing `prefecto-0.0.5/src/prefecto/states.py` & `prefecto-1.0.0/src/prefecto/states.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tools to improve Prefect states.
 
 """
+
 from __future__ import annotations
 
 from prefect import states
 
 
 def is_terminal(state: states.State) -> bool:
     """Return True if the state is terminal. Terminal states are:
```

