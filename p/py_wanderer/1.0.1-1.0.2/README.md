# Comparing `tmp/py_wanderer-1.0.1.tar.gz` & `tmp/py_wanderer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_wanderer-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_wanderer-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_wanderer-1.0.1.tar` & `py_wanderer-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2024-04-18 01:43:22.051405 py_wanderer-1.0.1/LICENSE
--rw-r--r--   0        0        0      571 2024-04-18 18:48:43.366728 py_wanderer-1.0.1/py_wanderer/__init__.py
--rw-r--r--   0        0        0    10722 2024-04-18 18:49:04.214876 py_wanderer-1.0.1/py_wanderer/algorithms.py
--rw-r--r--   0        0        0     2360 2024-04-17 23:41:47.137929 py_wanderer-1.0.1/py_wanderer/heuristics.py
--rw-r--r--   0        0        0     3030 2024-04-18 01:53:51.748090 py_wanderer-1.0.1/py_wanderer/maze.py
--rw-r--r--   0        0        0      527 2024-04-18 01:58:25.863533 py_wanderer-1.0.1/py_wanderer/plotter.py
--rw-r--r--   0        0        0      421 2024-04-18 18:32:04.901324 py_wanderer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 py_wanderer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-18 01:43:22.051405 py_wanderer-1.0.2/LICENSE
+-rw-r--r--   0        0        0      563 2024-04-19 13:22:41.490609 py_wanderer-1.0.2/py_wanderer/__init__.py
+-rw-r--r--   0        0        0    10691 2024-04-19 13:22:41.475609 py_wanderer-1.0.2/py_wanderer/algorithms.py
+-rw-r--r--   0        0        0     2360 2024-04-17 23:41:47.137929 py_wanderer-1.0.2/py_wanderer/heuristics.py
+-rw-r--r--   0        0        0     3030 2024-04-18 01:53:51.748090 py_wanderer-1.0.2/py_wanderer/maze.py
+-rw-r--r--   0        0        0      527 2024-04-18 01:58:25.863533 py_wanderer-1.0.2/py_wanderer/plotter.py
+-rw-r--r--   0        0        0      421 2024-04-18 18:32:04.901324 py_wanderer-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 py_wanderer-1.0.2/PKG-INFO
```

### Comparing `py_wanderer-1.0.1/LICENSE` & `py_wanderer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.1/py_wanderer/__init__.py` & `py_wanderer-1.0.2/py_wanderer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Maze builder and pathfinding algorithms."""
 
 from .algorithms import ALGORITHMS, PathfindingAlgorithm, Heuristic
 from .heuristics import HEURISTICS
 from .maze import Maze
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 ALGORITHMS = ALGORITHMS
 HEURISTICS = HEURISTICS
 
+
 def __getattr__(name):
     if name in globals():
         return globals()[name]
-    
+
     if name[0].isupper():
         return next(algorithm for algorithm in ALGORITHMS if algorithm.__name__ == name)
     else:
         return next(heuristic for heuristic in HEURISTICS if heuristic.__name__ == name)
-
```

### Comparing `py_wanderer-1.0.1/py_wanderer/algorithms.py` & `py_wanderer-1.0.2/py_wanderer/algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import abc
 from collections import defaultdict
 from heapq import heappop, heappush
 from typing import Callable
 
 Heuristic = Callable[[tuple[int, int], tuple[int, int]], float]
 
+
 class PathfindingAlgorithm(abc.ABC):
     def __init__(
             self,
             grid: list[list[int]],
             start: tuple[int, int], goal: tuple[int, int],
             heuristic_function: Heuristic,
             directions: tuple[tuple[int, int], ...] = ((0, 1), (1, 0), (0, -1), (-1, 0))
@@ -40,19 +41,19 @@
         while current_node in self.came_from:
             next_node = self.came_from[current_node]
             path.append(current_node)
             current_node = next_node
         path.append(self.start)
         return path[::-1]
 
-
     @abc.abstractmethod
     def run(self):
         """Run the pathfinding algorithm."""
 
+
 class Dijkstra(PathfindingAlgorithm):
     def run(self):
         while self.open_set:
             current = heappop(self.open_set)[1]
             if current == self.goal:
                 return self.reconstruct_path(current)
             for neighbor in self.get_neighbors(current):
@@ -60,14 +61,15 @@
                 if tentative_g_score < self.g_score[neighbor]:
                     self.came_from[neighbor] = current
                     self.g_score[neighbor] = tentative_g_score
                     self.f_score[neighbor] = self.heuristic_function(neighbor, self.goal)
                     heappush(self.open_set, (self.f_score[neighbor], neighbor))
         return []
 
+
 class AStar(PathfindingAlgorithm):
     def run(self) -> list[tuple[int, int]]:
         while self.open_set:
             current = heappop(self.open_set)[1]
             if current == self.goal:
                 return self.reconstruct_path(current)
             for neighbor in self.get_neighbors(current):
@@ -75,14 +77,15 @@
                 if tentative_g_score < self.g_score[neighbor]:
                     self.came_from[neighbor] = current
                     self.g_score[neighbor] = tentative_g_score
                     self.f_score[neighbor] = self.g_score[neighbor] + self.heuristic_function(neighbor, self.goal)
                     heappush(self.open_set, (self.f_score[neighbor], neighbor))
         return []
 
+
 class ThetaStar(PathfindingAlgorithm):
     # like A* but with line of sight check
     def run(self) -> list[tuple[int, int]]:
         """ Execute the Theta* pathfinding algorithm. """
         while self.open_set:
             current = heappop(self.open_set)[1]
             if current == self.goal:
@@ -131,14 +134,15 @@
                     p -= 2 * dy
                 if self.grid[x][y] == 1:
                     return False
                 p += 2 * dx
 
         return True
 
+
 class JPS(PathfindingAlgorithm):
     def run(self) -> list[tuple[int, int]]:
         """ Execute the Jump Point Search pathfinding algorithm. """
         while self.open_set:
             current = heappop(self.open_set)[1]
             if current == self.goal:
                 return self.reconstruct_path(current)
@@ -150,14 +154,15 @@
                     self.g_score[neighbor] = tentative_g_score
                     estimated_f_score = tentative_g_score + self.heuristic_function(neighbor, self.goal)
                     self.f_score[neighbor] = estimated_f_score
                     heappush(self.open_set, (estimated_f_score, neighbor))
 
         return []
 
+
 class IterativeDeepeningDFS(PathfindingAlgorithm):
     def run(self):
         import itertools
 
         def dls(node, depth):
             if node == self.goal:
                 return self.reconstruct_path(node)
@@ -175,14 +180,15 @@
             self.came_from = {self.start: None}
             result = dls(self.start, depth)
             if result is not None:
                 return result
 
         return []
 
+
 class Swarm(PathfindingAlgorithm):
     def run(self) -> list[tuple[int, int]]:
         open_set_start = []
         open_set_goal = []
         heappush(open_set_start, (0, self.start))
         heappush(open_set_goal, (0, self.goal))
 
@@ -203,28 +209,29 @@
             current = heappop(open_set)[1]
             for neighbor in self.get_neighbors(current):
                 if neighbor not in came_from:
                     came_from[neighbor] = current
                     if neighbor in other_came_from:
                         return
                     heappush(open_set, (self.heuristic_function(neighbor, self.goal), neighbor))
-                    
+
     def reconstruct_bidirectional_path(self, came_from_start, came_from_goal, meet_start, meet_goal):
         # reconstruct path from both sides meeting at a common node
         path_start = []
         while meet_start:
             path_start.append(meet_start)
             meet_start = came_from_start[meet_start]
         path_goal = []
         while meet_goal:
             path_goal.append(meet_goal)
             meet_goal = came_from_goal[meet_goal]
         path_start.reverse()
         return path_start + path_goal[1:]
 
+
 class DepthFirstSearch(PathfindingAlgorithm):
     def run(self) -> list[tuple[int, int]]:
         stack = [self.start]
         self.came_from[self.start] = None
 
         while stack:
             current = stack.pop()
@@ -232,15 +239,16 @@
                 return self.reconstruct_path(current)
 
             for neighbor in self.get_neighbors(current):
                 if neighbor not in self.came_from:
                     self.came_from[neighbor] = current
                     stack.append(neighbor)
         return []
-    
+
+
 class BellmanFord(PathfindingAlgorithm):
     def run(self) -> list[tuple[int, int]]:
         self.g_score[self.start] = 0
 
         for _ in range(len(self.grid) * len(self.grid[0]) - 1):
             made_changes = False
             for u in range(len(self.grid)):
@@ -255,10 +263,10 @@
                                 made_changes = True
             if not made_changes:
                 break
 
         if self.g_score[self.goal] != float('inf'):
             return self.reconstruct_path(self.goal)
         return []
-    
 
-ALGORITHMS = [Dijkstra, AStar, ThetaStar, JPS, BidirectionalSearch, IterativeDeepeningDFS, Swarm, DepthFirstSearch, BellmanFord]
+
+ALGORITHMS = [Dijkstra, AStar, ThetaStar, JPS, IterativeDeepeningDFS, Swarm, DepthFirstSearch, BellmanFord]
```

### Comparing `py_wanderer-1.0.1/py_wanderer/heuristics.py` & `py_wanderer-1.0.2/py_wanderer/heuristics.py`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.1/py_wanderer/maze.py` & `py_wanderer-1.0.2/py_wanderer/maze.py`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.1/py_wanderer/plotter.py` & `py_wanderer-1.0.2/py_wanderer/plotter.py`

 * *Files identical despite different names*

