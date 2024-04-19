# Comparing `tmp/cellworld_game-0.0.18.tar.gz` & `tmp/cellworld_game-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_game-0.0.18.tar", last modified: Thu Apr 18 17:03:16 2024, max compression
+gzip compressed data, was "cellworld_game-0.0.20.tar", last modified: Fri Apr 19 21:00:22 2024, max compression
```

## Comparing `cellworld_game-0.0.18.tar` & `cellworld_game-0.0.20.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 17:03:16.073573 cellworld_game-0.0.18/
--rw-rw-rw-   0        0        0       36 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/MANIFEST.in
--rw-rw-rw-   0        0        0      429 2024-04-18 17:03:16.072573 cellworld_game-0.0.18/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 17:03:16.042494 cellworld_game-0.0.18/cellworld_game/
--rw-rw-rw-   0        0        0       40 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game/README.md
--rw-rw-rw-   0        0        0      353 2024-04-18 16:30:52.000000 cellworld_game-0.0.18/cellworld_game/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 17:03:16.066494 cellworld_game-0.0.18/cellworld_game/__pycache__/
--rw-rw-rw-   0        0        0      700 2024-04-17 16:19:33.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     9842 2024-04-17 17:55:17.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     4974 2024-04-10 15:31:18.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
--rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/geometry.cpython-312.pyc
--rw-rw-rw-   0        0        0     8588 2024-04-16 17:26:10.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/model.cpython-312.pyc
--rw-rw-rw-   0        0        0     7484 2024-04-17 18:10:32.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/mouse.cpython-312.pyc
--rw-rw-rw-   0        0        0     2666 2024-04-10 15:31:18.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/navigation.cpython-312.pyc
--rw-rw-rw-   0        0        0     4654 2024-04-17 18:08:23.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     6071 2024-03-31 20:09:24.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
--rw-rw-rw-   0        0        0      934 2024-04-17 14:24:14.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/resources.cpython-312.pyc
--rw-rw-rw-   0        0        0     3344 2024-04-16 17:23:22.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/robot.cpython-312.pyc
--rw-rw-rw-   0        0        0     9945 2024-04-10 15:31:18.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/util.cpython-312.pyc
--rw-rw-rw-   0        0        0     9429 2024-04-17 18:13:18.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/view.cpython-312.pyc
--rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.18/cellworld_game/__pycache__/visibility.cpython-312.pyc
--rw-rw-rw-   0        0        0     5912 2024-04-17 17:55:01.000000 cellworld_game-0.0.18/cellworld_game/agent.py
--rw-rw-rw-   0        0        0     3620 2024-04-10 15:24:24.000000 cellworld_game-0.0.18/cellworld_game/cellworld_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-18 17:03:16.070503 cellworld_game-0.0.18/cellworld_game/files/
--rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.18/cellworld_game/files/agent.png
--rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.18/cellworld_game/files/predator.png
--rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.18/cellworld_game/files/prey.png
--rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.18/cellworld_game/geometry.py
--rw-rw-rw-   0        0        0     1636 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game/license.txt
--rw-rw-rw-   0        0        0     6818 2024-04-16 17:26:07.000000 cellworld_game-0.0.18/cellworld_game/model.py
--rw-rw-rw-   0        0        0     4237 2024-04-18 16:24:24.000000 cellworld_game-0.0.18/cellworld_game/mouse.py
--rw-rw-rw-   0        0        0     1775 2024-04-10 15:24:24.000000 cellworld_game-0.0.18/cellworld_game/navigation.py
--rw-rw-rw-   0        0        0     3242 2024-04-17 18:01:31.000000 cellworld_game-0.0.18/cellworld_game/navigation_agent.py
--rw-rw-rw-   0        0        0     4973 2024-03-31 20:08:15.000000 cellworld_game-0.0.18/cellworld_game/ray_tracing.py
--rw-rw-rw-   0        0        0      269 2024-04-17 14:24:07.000000 cellworld_game-0.0.18/cellworld_game/resources.py
--rw-rw-rw-   0        0        0     1905 2024-04-16 17:23:15.000000 cellworld_game-0.0.18/cellworld_game/robot.py
--rw-rw-rw-   0        0        0      183 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game/setup.cfg
--rw-rw-rw-   0        0        0     7908 2024-04-10 15:24:24.000000 cellworld_game-0.0.18/cellworld_game/util.py
--rw-rw-rw-   0        0        0     6402 2024-04-17 18:29:02.000000 cellworld_game-0.0.18/cellworld_game/view.py
--rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.18/cellworld_game/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-18 17:03:16.071558 cellworld_game-0.0.18/cellworld_game.egg-info/
--rw-rw-rw-   0        0        0      429 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1542 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/cellworld_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 17:03:16.073573 cellworld_game-0.0.18/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-04-18 17:03:15.000000 cellworld_game-0.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:00:22.251527 cellworld_game-0.0.20/
+-rw-rw-rw-   0        0        0       36 2024-04-19 21:00:21.000000 cellworld_game-0.0.20/MANIFEST.in
+-rw-rw-rw-   0        0        0      479 2024-04-19 21:00:22.250518 cellworld_game-0.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-04-19 21:00:21.000000 cellworld_game-0.0.20/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 21:00:22.221519 cellworld_game-0.0.20/cellworld_game/
+-rw-rw-rw-   0        0        0       40 2024-04-19 21:00:21.000000 cellworld_game-0.0.20/cellworld_game/README.md
+-rw-rw-rw-   0        0        0      353 2024-04-18 16:30:52.000000 cellworld_game-0.0.20/cellworld_game/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:00:22.244518 cellworld_game-0.0.20/cellworld_game/__pycache__/
+-rw-rw-rw-   0        0        0      700 2024-04-17 16:19:33.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9842 2024-04-17 17:55:17.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4974 2024-04-10 15:31:18.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/geometry.cpython-312.pyc
+-rw-rw-rw-   0        0        0     8588 2024-04-16 17:26:10.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/model.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7484 2024-04-17 18:10:32.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/mouse.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2666 2024-04-10 15:31:18.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/navigation.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4654 2024-04-17 18:08:23.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6071 2024-03-31 20:09:24.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
+-rw-rw-rw-   0        0        0      934 2024-04-17 14:24:14.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/resources.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3344 2024-04-16 17:23:22.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/robot.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9945 2024-04-10 15:31:18.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/util.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9429 2024-04-17 18:13:18.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/view.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.20/cellworld_game/__pycache__/visibility.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5912 2024-04-17 17:55:01.000000 cellworld_game-0.0.20/cellworld_game/agent.py
+-rw-rw-rw-   0        0        0     3620 2024-04-10 15:24:24.000000 cellworld_game-0.0.20/cellworld_game/cellworld_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:00:22.248517 cellworld_game-0.0.20/cellworld_game/files/
+-rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.20/cellworld_game/files/agent.png
+-rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.20/cellworld_game/files/predator.png
+-rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.20/cellworld_game/files/prey.png
+-rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.20/cellworld_game/geometry.py
+-rw-rw-rw-   0        0        0     1636 2024-04-19 21:00:21.000000 cellworld_game-0.0.20/cellworld_game/license.txt
+-rw-rw-rw-   0        0        0     6818 2024-04-16 17:26:07.000000 cellworld_game-0.0.20/cellworld_game/model.py
+-rw-rw-rw-   0        0        0     4237 2024-04-18 16:24:24.000000 cellworld_game-0.0.20/cellworld_game/mouse.py
+-rw-rw-rw-   0        0        0     1775 2024-04-10 15:24:24.000000 cellworld_game-0.0.20/cellworld_game/navigation.py
+-rw-rw-rw-   0        0        0     3242 2024-04-17 18:01:31.000000 cellworld_game-0.0.20/cellworld_game/navigation_agent.py
+-rw-rw-rw-   0        0        0     4973 2024-03-31 20:08:15.000000 cellworld_game-0.0.20/cellworld_game/ray_tracing.py
+-rw-rw-rw-   0        0        0      220 2024-04-19 14:17:58.000000 cellworld_game-0.0.20/cellworld_game/resources.py
+-rw-rw-rw-   0        0        0     1905 2024-04-16 17:23:15.000000 cellworld_game-0.0.20/cellworld_game/robot.py
+-rw-rw-rw-   0        0        0      183 2024-04-19 21:00:21.000000 cellworld_game-0.0.20/cellworld_game/setup.cfg
+-rw-rw-rw-   0        0        0     7908 2024-04-10 15:24:24.000000 cellworld_game-0.0.20/cellworld_game/util.py
+-rw-rw-rw-   0        0        0     6402 2024-04-17 18:29:02.000000 cellworld_game-0.0.20/cellworld_game/view.py
+-rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.20/cellworld_game/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:00:22.249528 cellworld_game-0.0.20/cellworld_game.egg-info/
+-rw-rw-rw-   0        0        0      479 2024-04-19 21:00:22.000000 cellworld_game-0.0.20/cellworld_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1542 2024-04-19 21:00:22.000000 cellworld_game-0.0.20/cellworld_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 21:00:22.000000 cellworld_game-0.0.20/cellworld_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 21:00:22.000000 cellworld_game-0.0.20/cellworld_game.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-19 21:00:22.000000 cellworld_game-0.0.20/cellworld_game.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-19 21:00:22.000000 cellworld_game-0.0.20/cellworld_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 21:00:22.252518 cellworld_game-0.0.20/setup.cfg
+-rw-rw-rw-   0        0        0      665 2024-04-19 21:00:21.000000 cellworld_game-0.0.20/setup.py
```

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/__init__.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/agent.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/geometry.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/geometry.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/model.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/model.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/mouse.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/mouse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/navigation.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/navigation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/resources.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/resources.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/robot.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/robot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/util.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/util.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/view.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/view.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/__pycache__/visibility.cpython-312.pyc` & `cellworld_game-0.0.20/cellworld_game/__pycache__/visibility.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/agent.py` & `cellworld_game-0.0.20/cellworld_game/agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/cellworld_loader.py` & `cellworld_game-0.0.20/cellworld_game/cellworld_loader.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/files/agent.png` & `cellworld_game-0.0.20/cellworld_game/files/agent.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/files/predator.png` & `cellworld_game-0.0.20/cellworld_game/files/predator.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/files/prey.png` & `cellworld_game-0.0.20/cellworld_game/files/prey.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/license.txt` & `cellworld_game-0.0.20/cellworld_game/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/model.py` & `cellworld_game-0.0.20/cellworld_game/model.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/mouse.py` & `cellworld_game-0.0.20/cellworld_game/mouse.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/navigation.py` & `cellworld_game-0.0.20/cellworld_game/navigation.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/navigation_agent.py` & `cellworld_game-0.0.20/cellworld_game/navigation_agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/ray_tracing.py` & `cellworld_game-0.0.20/cellworld_game/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/robot.py` & `cellworld_game-0.0.20/cellworld_game/robot.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/util.py` & `cellworld_game-0.0.20/cellworld_game/util.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/view.py` & `cellworld_game-0.0.20/cellworld_game/view.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game/visibility.py` & `cellworld_game-0.0.20/cellworld_game/visibility.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.18/cellworld_game.egg-info/SOURCES.txt` & `cellworld_game-0.0.20/cellworld_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

