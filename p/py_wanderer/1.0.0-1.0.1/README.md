# Comparing `tmp/py_wanderer-1.0.0.tar.gz` & `tmp/py_wanderer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_wanderer-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_wanderer-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_wanderer-1.0.0.tar` & `py_wanderer-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2024-04-18 01:43:22.051405 py_wanderer-1.0.0/LICENSE
--rw-r--r--   0        0        0      571 2024-04-18 02:00:10.983987 py_wanderer-1.0.0/py_wanderer/__init__.py
--rw-r--r--   0        0        0    12796 2024-04-18 01:02:13.808210 py_wanderer-1.0.0/py_wanderer/algorithms.py
--rw-r--r--   0        0        0     2360 2024-04-17 23:41:47.137929 py_wanderer-1.0.0/py_wanderer/heuristics.py
--rw-r--r--   0        0        0     3030 2024-04-18 01:53:51.748090 py_wanderer-1.0.0/py_wanderer/maze.py
--rw-r--r--   0        0        0      527 2024-04-18 01:58:25.863533 py_wanderer-1.0.0/py_wanderer/plotter.py
--rw-r--r--   0        0        0      421 2024-04-18 18:32:04.901324 py_wanderer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 py_wanderer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-18 01:43:22.051405 py_wanderer-1.0.1/LICENSE
+-rw-r--r--   0        0        0      571 2024-04-18 18:48:43.366728 py_wanderer-1.0.1/py_wanderer/__init__.py
+-rw-r--r--   0        0        0    10722 2024-04-18 18:49:04.214876 py_wanderer-1.0.1/py_wanderer/algorithms.py
+-rw-r--r--   0        0        0     2360 2024-04-17 23:41:47.137929 py_wanderer-1.0.1/py_wanderer/heuristics.py
+-rw-r--r--   0        0        0     3030 2024-04-18 01:53:51.748090 py_wanderer-1.0.1/py_wanderer/maze.py
+-rw-r--r--   0        0        0      527 2024-04-18 01:58:25.863533 py_wanderer-1.0.1/py_wanderer/plotter.py
+-rw-r--r--   0        0        0      421 2024-04-18 18:32:04.901324 py_wanderer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 py_wanderer-1.0.1/PKG-INFO
```

### Comparing `py_wanderer-1.0.0/LICENSE` & `py_wanderer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.0/py_wanderer/__init__.py` & `py_wanderer-1.0.1/py_wanderer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Maze builder and pathfinding algorithms."""
 
 from .algorithms import ALGORITHMS, PathfindingAlgorithm, Heuristic
 from .heuristics import HEURISTICS
 from .maze import Maze
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 ALGORITHMS = ALGORITHMS
 HEURISTICS = HEURISTICS
 
 def __getattr__(name):
     if name in globals():
         return globals()[name]
```

### Comparing `py_wanderer-1.0.0/py_wanderer/algorithms.py` & `py_wanderer-1.0.1/py_wanderer/algorithms.py`

 * *Files 16% similar despite different names*

```diff
@@ -150,63 +150,14 @@
                     self.g_score[neighbor] = tentative_g_score
                     estimated_f_score = tentative_g_score + self.heuristic_function(neighbor, self.goal)
                     self.f_score[neighbor] = estimated_f_score
                     heappush(self.open_set, (estimated_f_score, neighbor))
 
         return []
 
-class BidirectionalSearch(PathfindingAlgorithm):
-    def run(self) -> list[tuple[int, int]]:
-        open_set_start = []
-        open_set_goal = []
-        heappush(open_set_start, (0, self.start))
-        heappush(open_set_goal, (0, self.goal))
-
-        came_from_start = {self.start: None}
-        came_from_goal = {self.goal: None}
-
-        g_score_start = defaultdict(lambda: float('inf'))
-        g_score_goal = defaultdict(lambda: float('inf'))
-
-        g_score_start[self.start] = 0
-        g_score_goal[self.goal] = 0
-
-        while open_set_start and open_set_goal:
-            current_start = heappop(open_set_start)[1]
-            current_goal = heappop(open_set_goal)[1]
-
-            if current_start in came_from_goal or current_goal in came_from_start:
-                return self.reconstruct_bidirectional_path(came_from_start, came_from_goal, current_start, current_goal)
-
-            self.process_neighbors(current_start, g_score_start, came_from_start, open_set_start)
-            self.process_neighbors(current_goal, g_score_goal, came_from_goal, open_set_goal)
-
-        return []
-
-    def process_neighbors(self, current, g_score, came_from, open_set):
-        for neighbor in self.get_neighbors(current):
-            tentative_g_score = g_score[current] + 1
-            if tentative_g_score < g_score[neighbor]:
-                came_from[neighbor] = current
-                g_score[neighbor] = tentative_g_score
-                heappush(open_set, (tentative_g_score, neighbor))
-
-    def reconstruct_bidirectional_path(self, came_from_start, came_from_goal, meet_start, meet_goal):
-        # reconstruct path from both sides meeting at a common node
-        path_start = []
-        while meet_start:
-            path_start.append(meet_start)
-            meet_start = came_from_start[meet_start]
-        path_goal = []
-        while meet_goal:
-            path_goal.append(meet_goal)
-            meet_goal = came_from_goal[meet_goal]
-        path_start.reverse()
-        return path_start + path_goal[1:]
-
 class IterativeDeepeningDFS(PathfindingAlgorithm):
     def run(self):
         import itertools
 
         def dls(node, depth):
             if node == self.goal:
                 return self.reconstruct_path(node)
```

### Comparing `py_wanderer-1.0.0/py_wanderer/heuristics.py` & `py_wanderer-1.0.1/py_wanderer/heuristics.py`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.0/py_wanderer/maze.py` & `py_wanderer-1.0.1/py_wanderer/maze.py`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.0/py_wanderer/plotter.py` & `py_wanderer-1.0.1/py_wanderer/plotter.py`

 * *Files identical despite different names*

