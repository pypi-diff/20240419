# Comparing `tmp/open_fleet-0.0.2.tar.gz` & `tmp/open_fleet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_fleet-0.0.2.tar", last modified: Wed Apr 17 12:56:32 2024, max compression
+gzip compressed data, was "open_fleet-0.0.3.tar", last modified: Fri Apr 19 10:22:17 2024, max compression
```

## Comparing `open_fleet-0.0.2.tar` & `open_fleet-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.484314 open_fleet-0.0.2/
--rw-r--r--   0 huangshiyu   (501) staff       (20)    11357 2024-04-17 07:28:40.000000 open_fleet-0.0.2/LICENSE
--rw-r--r--   0 huangshiyu   (501) staff       (20)     1828 2024-04-17 12:56:32.484110 open_fleet-0.0.2/PKG-INFO
--rw-r--r--   0 huangshiyu   (501) staff       (20)      506 2024-04-17 12:56:16.000000 open_fleet-0.0.2/README.md
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.480780 open_fleet-0.0.2/fleet/
--rw-r--r--   0 huangshiyu   (501) staff       (20)      457 2024-04-17 12:56:27.000000 open_fleet-0.0.2/fleet/__init__.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.481358 open_fleet-0.0.2/fleet/config/
--rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:11.000000 open_fleet-0.0.2/fleet/config/__init__.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      653 2024-04-16 11:50:22.000000 open_fleet-0.0.2/fleet/config/config.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     9602 2024-04-17 10:49:17.000000 open_fleet-0.0.2/fleet/manager.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.482459 open_fleet-0.0.2/fleet/utils/
--rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:03.000000 open_fleet-0.0.2/fleet/utils/__init__.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      496 2024-04-17 07:18:40.000000 open_fleet-0.0.2/fleet/utils/file_utils.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      573 2024-04-16 07:33:32.000000 open_fleet-0.0.2/fleet/utils/host_utils.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2143 2024-04-17 10:43:53.000000 open_fleet-0.0.2/fleet/utils/time_tracker.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     5543 2024-04-17 09:52:18.000000 open_fleet-0.0.2/fleet/worker.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.483519 open_fleet-0.0.2/open_fleet.egg-info/
--rw-r--r--   0 huangshiyu   (501) staff       (20)     1828 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/PKG-INFO
--rw-r--r--   0 huangshiyu   (501) staff       (20)      398 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/SOURCES.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)        1 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/dependency_links.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)       94 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/requires.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)        6 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/top_level.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)       38 2024-04-17 12:56:32.484357 open_fleet-0.0.2/setup.cfg
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2456 2024-04-17 12:55:11.000000 open_fleet-0.0.2/setup.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.395015 open_fleet-0.0.3/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)    11357 2024-04-17 07:28:40.000000 open_fleet-0.0.3/LICENSE
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2824 2024-04-19 10:22:17.394745 open_fleet-0.0.3/PKG-INFO
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     1502 2024-04-19 10:21:25.000000 open_fleet-0.0.3/README.md
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.390547 open_fleet-0.0.3/fleet/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      457 2024-04-19 03:11:12.000000 open_fleet-0.0.3/fleet/__init__.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.390886 open_fleet-0.0.3/fleet/config/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:11.000000 open_fleet-0.0.3/fleet/config/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      741 2024-04-19 03:23:03.000000 open_fleet-0.0.3/fleet/config/config.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     9966 2024-04-19 08:08:58.000000 open_fleet-0.0.3/fleet/manager.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.391350 open_fleet-0.0.3/fleet/manager_utils/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-19 05:23:58.000000 open_fleet-0.0.3/fleet/manager_utils/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     3506 2024-04-19 09:51:32.000000 open_fleet-0.0.3/fleet/manager_utils/assign_jobs.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.392783 open_fleet-0.0.3/fleet/utils/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:03.000000 open_fleet-0.0.3/fleet/utils/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      517 2024-04-19 06:51:31.000000 open_fleet-0.0.3/fleet/utils/file_utils.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      573 2024-04-16 07:33:32.000000 open_fleet-0.0.3/fleet/utils/host_utils.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2186 2024-04-19 03:24:42.000000 open_fleet-0.0.3/fleet/utils/time_tracker.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     6733 2024-04-19 06:50:33.000000 open_fleet-0.0.3/fleet/worker.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.394041 open_fleet-0.0.3/open_fleet.egg-info/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2824 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/PKG-INFO
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      465 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/SOURCES.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        1 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/dependency_links.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)       94 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/requires.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        6 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/top_level.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)       38 2024-04-19 10:22:17.395069 open_fleet-0.0.3/setup.cfg
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2455 2024-04-19 10:21:57.000000 open_fleet-0.0.3/setup.py
```

### Comparing `open_fleet-0.0.2/LICENSE` & `open_fleet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.2/fleet/config/config.py` & `open_fleet-0.0.3/fleet/config/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional, List, Union
 import argparse
 
 
 def get_args(input: Optional[Union[str, List[str]]] = None):
     parser = argparse.ArgumentParser(description="Runner")
     parser.add_argument("--base_dir", default=None, type=str,
-                        help="directory to store the status of the nodes and tasks")
+                        help="directory to store the status of the nodes and jobs")
     parser.add_argument("--node_id", default=None, type=str, help="node id for the worker")
+    parser.add_argument("--timeout",default=None, type=int, help="timeout for each job")
     if input is not None:
         if isinstance(input, str):
             input = [element for element in input.split(" ") if element]
         args = parser.parse_args(input)
     else:
         args = parser.parse_args()
     return args
```

### Comparing `open_fleet-0.0.2/fleet/manager.py` & `open_fleet-0.0.3/fleet/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 from typing import List, Any, Dict
 import time
 import json
+from multiprocessing import Process
 
 from pathlib import Path
 from rich.console import Console
-from rich.progress import Progress, BarColumn, TextColumn, TimeRemainingColumn
+from rich.progress import Progress, BarColumn, TextColumn
 
 from fleet.utils.file_utils import safe_load_json
 from fleet.utils.time_tracker import TimeTracker
+from fleet.manager_utils.assign_jobs import loop_assignment
 
 
 class Manager:
     def __init__(self, args, job_list: List[Any], info: Dict = {}):
         base_dir = args.base_dir
         self.base_dir = Path(base_dir)
         self.console = Console()
         self.base_dir.mkdir(parents=True, exist_ok=True)
         self.nodes_dir = self.base_dir / 'nodes'
 
         self.status_dir = self.base_dir / 'status'
+        self.working_dir = self.base_dir / 'working'
+
         self.heart_dir = self.base_dir / 'heart'
 
+        # to store the available nodes
+        self.available_dir = self.base_dir / 'available'
+
+        self.finished_file = self.base_dir / 'finished'
+
         self.nodes_dir.mkdir(parents=True, exist_ok=True)
         print(f"nodes_dir: {self.nodes_dir}")
         self.heart_dir.mkdir(parents=True, exist_ok=True)
         print(f"heart_dir: {self.heart_dir}")
         self.status_dir.mkdir(parents=True, exist_ok=True)
         print(f"status_dir: {self.status_dir}")
+        self.available_dir.mkdir(parents=True, exist_ok=True)
+        print(f"available_dir: {self.available_dir}")
+        self.working_dir.mkdir(parents=True, exist_ok=True)
 
         self.job_list = job_list
         self.total_jobs = len(job_list)
         self.info = info
-        self.working_task_status = {}
+        # self.working_task_status = {}
+        self.working_num = 0
         self.unassigned_task_status = {}
 
         self.no_available_nodes_num = 0
 
         self.success_num = 0
         self.crashed_num = 0
         self.failed_num = 0
 
         self.dead_nodes = {}
         self.available_nodes = {}
 
         self.time_tracker = TimeTracker(total_tasks=self.total_jobs)
 
+        self.first_assigned = True
+
+        self.job_assign_process = None
+
+        self.previous_log_time = None
+        # self.new_finished_num = 0
+
     def initialize_tasks(self):
         self.finished_num = 0
         for idx, job_input in enumerate(self.job_list):
             task_name = f'task{idx + 1}'
             task_status_path = self.status_dir / f'{task_name}.status'
             if not task_status_path.exists():
                 status_info = {'status': 'unassigned', 'input': job_input, "task_status_path": str(task_status_path)}
@@ -73,164 +93,160 @@
 
             else:
                 if status_info['status'] == 'unassigned':
                     self.unassigned_task_status[task_name] = status_info
                     self.unassigned_task_status[task_name]["task_status_path"] = str(task_status_path)
                 else:
                     assert status_info['status'] == 'assigned'
-                    self.working_task_status[task_name] = status_info
-                    self.working_task_status[task_name]["task_status_path"] = str(task_status_path)
+                    # self.working_task_status[task_name] = status_info
+                    # self.working_task_status[task_name]["task_status_path"] = str(task_status_path)
+                    working_file = self.working_dir / task_name
+                    if not working_file.exists():
+                        status_info["task_status_path"] = str(task_status_path)
+                        working_file.write_text(json.dumps(status_info))
 
         if self.finished_num == 0:
             success_rate = 0
         else:
             success_rate = self.success_num / self.finished_num * 100
-        time_summary = self.time_tracker.summary
-        self.progress.update(self.task_id,
-                             description=f"Success Rate: {success_rate:.2f}% Finished: {self.finished_num}/{self.total_jobs} {time_summary}")
 
-    def check_task_status_and_assign(self):
-        self.monitor_heartbeats()
+        self.progress.update(self.task_id,
+                             description=f"Success Rate: {success_rate:.2f}% Finished: {self.finished_num}/{self.total_jobs}")
 
-        available_nodes = []
-        for node in self.available_nodes:
-            node_file = self.nodes_dir / f"{node}.status"
-            node_info = safe_load_json(node_file)
-            if node_info and node_info["status"] == 'idle':
-                available_nodes.append((node, node_file))
+        if self.finished_num > 0:
+            self.first_assigned = False
 
-        for node in self.dead_nodes:
+    def process_dead_nodes(self, dead_nodes):
+        # check if the task is assigned to a dead node
+        for node in dead_nodes:
             node_file = self.nodes_dir / f"{node}.status"
             node_info = safe_load_json(node_file)
             if node_info and node_info["status"] == 'busy':
                 task_status_path = node_info["task_status_path"]
 
                 status_info = safe_load_json(Path(task_status_path))
 
                 if status_info and status_info['status'] == 'assigned':
                     status_info['status'] = 'crashed'
                     Path(task_status_path).write_text(json.dumps(status_info))
-                    node_info['status'] = 'idle'
+                    node_info['status'] = 'dead'
                     node_file.write_text(json.dumps(node_info))
 
-        if not available_nodes:
-            if self.no_available_nodes_num % 100 == 10:
-                self.console.log("No available nodes, sleep 1 seconds...")
-
-            if self.no_available_nodes_num % 100 < 10:
-                time.sleep(1)
-            else:
-                time.sleep(10)
-
-            self.no_available_nodes_num += 1
 
+    def log_status(self):
+        current_time = time.time()
+        if self.previous_log_time is None or current_time - self.previous_log_time > 1 or self.finished_num == self.total_jobs:
+            self.previous_log_time = current_time
         else:
-            self.no_available_nodes_num = 0
-            self.assign_task_to_node(available_nodes)
-
-        self.check_working_tasks()
+            return
 
-        # log status
         if self.finished_num == 0:
             success_rate = 0
         else:
             success_rate = self.success_num / self.finished_num * 100
-
         time_summary = self.time_tracker.summary
-        self.progress.update(self.task_id,
-                             description=f"Success Rate: {success_rate:.2f}% Finished: {self.finished_num}/{self.total_jobs} Nodes(Good/Dead): {len(self.available_nodes)}/{len(self.dead_nodes)} {time_summary}")
 
-    def assign_task_to_node(self, available_nodes):
-        assign_new_node_num = 0
-        for job_key in list(self.unassigned_task_status.keys()):
-            status_info = self.unassigned_task_status[job_key]
-            assert status_info['status'] == 'unassigned'
-            if available_nodes:
-                # self.console.log("available_nodes", available_nodes)
-                chosen_node, node_file = available_nodes.pop()
-                status_info['assigned_to'] = chosen_node
-                status_info['status'] = 'assigned'
-                task_status_file = Path(status_info["task_status_path"])
-                task_status_file.write_text(json.dumps(status_info))
-
-                node_info = {
-                    "status": "busy",
-                    "task": job_key,
-                    "task_status_path": status_info["task_status_path"]
-                }
-                node_file.write_text(json.dumps(node_info))
 
-                self.console.log(f"Assign task {job_key} to node {chosen_node}")
-                assign_new_node_num += 1
-                # 移除未完成任务
-                del self.unassigned_task_status[job_key]
-                # 添加到工作任务
-                self.working_task_status[job_key] = status_info
-            else:
-                break
-        if assign_new_node_num > 0:
-            self.console.log(f"Assigned jobs to {assign_new_node_num} nodes.")
-            # time.sleep(10)
+        self.progress.update(self.task_id, description=f"Success Rate: {success_rate:.2f}% Finished/Working: {self.finished_num}/{self.working_num}/{self.total_jobs} Nodes(Good/Dead): {len(self.available_nodes)}/{len(self.dead_nodes)} {time_summary}")
+
+    def check_task_status_and_assign(self):
+        self.monitor_heartbeats()
+        self.check_working_tasks()
+        self.log_status()
 
     def check_working_tasks(self):
-        for job_key in list(self.working_task_status.keys()):
-            status_info = self.working_task_status[job_key]
+        self.working_num = 0
+        # self.new_finished_num = 0
+        # Remove finished tasks in working_task_status
+        working_files = list(self.working_dir.glob("*"))
+
+        # for job_key in list(self.working_task_status.keys()):
+        for working_file in working_files:
+            # status_info = self.working_task_status[job_key]
+            status_info = safe_load_json(working_file)
             task_status_file = Path(status_info["task_status_path"])
 
             assert task_status_file.exists(), f"task_status_file {task_status_file} not exists"
 
             status_info_in_file = safe_load_json(task_status_file)
             if status_info_in_file is None:
                 continue
 
             assert status_info_in_file['status'] in ["assigned", "success", "crashed", "failed"]
 
             if status_info_in_file['status'] == "assigned":
-                continue
+                self.working_num += 1
             else:
                 if status_info_in_file['status'] == 'success':
                     self.success_num += 1
                 elif status_info_in_file['status'] == 'crashed':
                     self.crashed_num += 1
                 elif status_info_in_file['status'] == 'failed':
                     self.failed_num += 1
 
-                del self.working_task_status[job_key]
+                # del self.working_task_status[job_key]
+                working_file.unlink()
+
                 self.finished_num += 1
+                # self.new_finished_num += 1
+                # self.console.log(f"{self.finished_num}/{self.new_finished_num}")
+
                 self.time_tracker.update()
                 self.progress.update(self.task_id, advance=1)
 
-    def run(self):
 
+    def loop_assignment(self):
+        loop_assignment(self.available_dir, self.nodes_dir, self.working_dir, self.unassigned_task_status, self.console)
+
+    def start_job_assignment(self):
+        self.job_assign_process = Process(target=self.loop_assignment)
+        self.job_assign_process.start()
+
+    def stop_job_assignment(self):
+        if self.job_assign_process:
+            self.job_assign_process.terminate()
+            self.job_assign_process.join()
+
+    def run(self):
         with Progress(
                 TextColumn("[progress.description]{task.description}"),
                 BarColumn(),
                 TextColumn("{task.percentage:>3.0f}%"),
                 console=self.console
         ) as progress:
             self.task_id = progress.add_task("Processing Jobs", total=self.total_jobs)
             self.progress = progress
             # self.pbar = tqdm(total=len(self.job_list), desc="Processing Jobs")
             self.initialize_tasks()
 
-            while True:
-                self.check_task_status_and_assign()
-                # time.sleep(10)  # 每10秒检查一次
-                if self.finished_num == self.total_jobs:
-                    break
+            self.start_job_assignment()
 
-            # self.pbar.close()
+            try:
+                while True:
+                    if self.finished_num == self.total_jobs:
+                        if not self.finished_file.exists():
+                            self.finished_file.touch()
+                        break
+
+                    self.check_task_status_and_assign()
+            finally:
+                self.stop_job_assignment()
 
     def monitor_heartbeats(self, heartbeat_timeout: int = 120):
         self.available_nodes = {}
-        self.dead_nodes = {}
+        new_dead_nodes = {}
 
         current_time = int(time.time())
         for node_file in self.heart_dir.iterdir():
+            if node_file.stem in self.dead_nodes:
+                continue
+
             node_info = safe_load_json(node_file)
             if node_info and node_info['status'] == "available" and current_time - node_info.get("last_heartbeat",
                                                                                                  0) <= heartbeat_timeout:
                 self.available_nodes[node_file.stem] = node_info
             else:
                 node_info['status'] = 'dead'
                 node_file.write_text(json.dumps(node_info))
                 self.dead_nodes[node_file.stem] = node_info
+                new_dead_nodes[node_file.stem] = node_info
+        self.process_dead_nodes(new_dead_nodes)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `open_fleet-0.0.2/fleet/utils/host_utils.py` & `open_fleet-0.0.3/fleet/utils/host_utils.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.2/fleet/utils/time_tracker.py` & `open_fleet-0.0.3/fleet/utils/time_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,17 @@
         return f"{time_second / 86400:.2f} day"
 
 
 class TimeTracker:
     def __init__(self, total_tasks: int):
         assert total_tasks > 0, "task number must larger than zero!"
         self.total_tasks = total_tasks
+        self.reset()
+
+    def reset(self):
         self.finished_tasks = 0
         self.start_time = time.time()
 
     def update(self, task_num: int = 1):
         self.finished_tasks += task_num
         self.current_time = time.time()
```

### Comparing `open_fleet-0.0.2/fleet/worker.py` & `open_fleet-0.0.3/fleet/worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,55 @@
 from typing import Callable, Dict
 import time
 import uuid
 import json
-from copy import deepcopy
-from multiprocessing import Process
+from multiprocessing import Process, Queue
+import traceback
 
 from pathlib import Path
 
 from fleet.utils.file_utils import safe_load_json
 
+def run_job(job_func, job_input, info, output_queue):
+    try:
+        result = job_func(job_input, info)
+        output_queue.put(result)
+    except Exception as e:
+        error_message = traceback.format_exc()
+        output_queue.put({"error": error_message, "status": "crashed"})
+
+
 class Worker:
     def __init__(self, args, job_func: Callable, info: Dict = {}):
         self.base_dir = Path(args.base_dir)
+        self.timeout = args.timeout
         unique_id = str(uuid.uuid4())
         self.node_id = f"{args.node_id}_{unique_id}" if args.node_id else unique_id
         self.nodes_dir = self.base_dir / 'nodes'
         self.status_dir = self.base_dir / 'status'
         self.heart_dir = self.base_dir / 'heart'
+        self.finished_file = self.base_dir / 'finished'
+        self.available_dir = self.base_dir / 'available'
+        self.available_file = self.available_dir / self.node_id
 
         self.node_status_path = self.nodes_dir / f'{self.node_id}.status'
         self.node_heart_status_path = self.heart_dir / f'{self.node_id}.heart'
 
         self.job_func = job_func
         self.info = info
 
-        self.unassigned_task_status = {}
+        # self.unassigned_task_status = {}
         self.not_find_job_num = 0
 
         self.heartbeat_process = None  # 添加一个属性来保存心跳进程的引用
 
+    def create_available_file(self):
+        if not self.available_file.exists():
+            self.available_file.touch()
+
     def heartbeat_daemon(self):
         """这个函数将作为独立的进程运行，负责发送心跳信号。"""
         try:
             while True:
                 self.send_heartbeat()
                 time.sleep(10)  # 设定心跳频率，例如每10秒发送一次心跳
         except KeyboardInterrupt:
@@ -71,80 +88,99 @@
             self.heartbeat_process.join()
             self.send_dead()  # 在进程终止时发送死亡信号
 
     def send_dead(self):
         self.send_heartbeat(status='dead')
 
     def register_node(self):
-        for task_status_file in self.status_dir.iterdir():
-            status_info = safe_load_json(task_status_file)
-            if status_info and status_info["status"] == "unassigned":
-                self.unassigned_task_status[task_status_file.stem] = status_info
-        print("Read task status done")
+        self.start_heartbeat()  # 在任务开始时启动心跳进程
+
+        # for task_status_file in self.status_dir.iterdir():
+        # status_info = safe_load_json(task_status_file)
+        # if status_info and status_info["status"] == "unassigned":
+        #     self.unassigned_task_status[task_status_file.stem] = status_info
+        # print("Read task status done")
         node_info = {
             "status": "idle"
         }
         # self.node_status_path.write_text('idle')
         self.node_status_path.write_text(json.dumps(node_info))
-        self.start_heartbeat()  # 在任务开始时启动心跳进程
-
+        self.create_available_file()
         print(f"Node {self.node_id} registered")
 
-    def check_and_process_tasks(self):
+    def process_job(self):
         find_job = False
-        for task_name in list(self.unassigned_task_status.keys()):
-            status_info = deepcopy(self.unassigned_task_status[task_name])
-            task_status_file = Path(status_info["task_status_path"])
-
-            status_info_in_file = safe_load_json(task_status_file)
-            if status_info_in_file is None:
-                continue
-
-            if status_info_in_file['status'] != 'unassigned':
-                del self.unassigned_task_status[task_name]
-            if status_info_in_file.get('assigned_to') == self.node_id:
-                # 标记节点为忙碌
-                # self.node_status_path.write_text('busy')
-
-                job_input = status_info.get('input')
-                print(f"Processing task: {job_input}")
-                find_job = True
+        node_info = safe_load_json(self.node_status_path)
+        if node_info and node_info['status'] == 'busy':
+            task_status_path = node_info['task_status_path']
+            status_info = safe_load_json(Path(task_status_path))
+            task_status_file = Path(node_info["task_status_path"])
+
+            job_input = status_info.get('input')
+            print(f"Processing task: {job_input}")
+            find_job = True
+
+            if self.timeout is None:
                 result = self.job_func(job_input, self.info)
-                print(f"Task {job_input} Done!")
-                if 'error' in result:
-                    status_info['error'] = result['error']
-
-                # 更新任务状态为完成
-                status_info['status'] = result['status']
-
-                task_status_file.write_text(json.dumps(status_info))
-
-                # 标记节点为空闲
-                node_info = {
-                    "status": "idle"
-                }
-                self.node_status_path.write_text(json.dumps(node_info))
-                break
+            else:
+                output_queue = Queue()
+                job_process = Process(target=run_job, args=(self.job_func, job_input, self.info, output_queue))
+                job_process.start()
+                job_process.join(timeout=self.timeout)
+                if job_process.is_alive():
+                    job_process.terminate()
+                    job_process.join()
+                    result = {"error": "job timeout", "status": "crashed"}
+                else:
+                    result = output_queue.get()
+
+            print(f"Task {job_input} Done!")
+            if 'error' in result:
+                status_info['error'] = result['error']
+
+            # 更新任务状态为完成
+            status_info['status'] = result['status']
+
+            task_status_file.write_text(json.dumps(status_info))
+
+            # 标记节点为空闲
+            node_info = {
+                "status": "idle"
+            }
+            self.node_status_path.write_text(json.dumps(node_info))
+            self.create_available_file()
+            return find_job
+        return find_job
+
+    def check_and_process_tasks(self):
+        find_job = self.process_job()
 
         if not find_job:
-            if self.not_find_job_num % 100 == 0:
+            if self.not_find_job_num % 100 == 20:
                 print("No task assigned...")
-            time.sleep(0.5)
+
+            if self.not_find_job_num < 20:
+                time.sleep(0.1)
+            else:
+                time.sleep(0.5)
+
             self.not_find_job_num += 1
         else:
             self.not_find_job_num = 0
 
     def run(self):
         self.register_node()
 
         try:
             while True:
                 self.check_and_process_tasks()
-                if len(self.unassigned_task_status) == 0:
+                if self.finished_file.exists():
                     break
                 if not self.check_heart():
                     break
 
         except Exception as e:
-            print(f"Error: {e}")
+            # traceback.print_exc()  # 打印异常信息和堆栈跟踪
+            error_message = traceback.format_exc()
+            print(error_message)
         finally:
             self.stop_heartbeat()  # 在任何结束时确保心跳进程被终止
```

### Comparing `open_fleet-0.0.2/setup.py` & `open_fleet-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
             "pytest-cov",
             "mypy",
             "isort",
             "black",
             "ruff",
         ],
         "dev": ["build", "twine"],
-
     }
 
     return req
 
 
 def get_version() -> str:
     # https://packaging.python.org/guides/single-sourcing-package-version/
```

