# Comparing `tmp/lddya-4.1.1.tar.gz` & `tmp/lddya-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lddya-4.1.1.tar", last modified: Tue Apr 16 13:28:22 2024, max compression
+gzip compressed data, was "lddya-4.1.2.tar", last modified: Fri Apr 19 12:29:49 2024, max compression
```

## Comparing `lddya-4.1.1.tar` & `lddya-4.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 13:28:22.419533 lddya-4.1.1/
--rw-rw-rw-   0        0        0      348 2024-04-16 13:28:22.419533 lddya-4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       74 2021-12-03 06:05:24.000000 lddya-4.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 13:28:22.415522 lddya-4.1.1/lddya/
--rw-rw-rw-   0        0        0    28753 2024-04-16 12:26:50.000000 lddya-4.1.1/lddya/Algorithm.py
--rw-rw-rw-   0        0        0     7851 2022-11-01 06:31:16.000000 lddya-4.1.1/lddya/Data.py
--rw-rw-rw-   0        0        0     1444 2022-01-21 14:37:00.000000 lddya-4.1.1/lddya/DataFrame.py
--rw-rw-rw-   0        0        0     2372 2024-04-11 02:41:50.000000 lddya-4.1.1/lddya/Draw.py
--rw-rw-rw-   0        0        0     5181 2024-04-16 13:26:39.000000 lddya-4.1.1/lddya/Map.py
--rw-rw-rw-   0        0        0    16714 2021-12-03 06:05:24.000000 lddya-4.1.1/lddya/Optimizer.py
--rw-rw-rw-   0        0        0       54 2023-09-07 03:17:02.000000 lddya-4.1.1/lddya/__init__.py
--rw-rw-rw-   0        0        0      393 2021-12-03 06:05:24.000000 lddya-4.1.1/lddya/tool.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:28:22.418030 lddya-4.1.1/lddya.egg-info/
--rw-rw-rw-   0        0        0      348 2024-04-16 13:28:22.000000 lddya-4.1.1/lddya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2024-04-16 13:28:22.000000 lddya-4.1.1/lddya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 13:28:22.000000 lddya-4.1.1/lddya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-16 13:28:22.000000 lddya-4.1.1/lddya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-16 13:28:22.000000 lddya-4.1.1/lddya.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 13:28:22.419533 lddya-4.1.1/setup.cfg
--rw-rw-rw-   0        0        0      848 2024-04-16 13:26:03.000000 lddya-4.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:29:49.348319 lddya-4.1.2/
+-rw-rw-rw-   0        0        0      380 2024-04-19 12:29:49.348319 lddya-4.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2021-12-03 06:05:24.000000 lddya-4.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 12:29:49.344318 lddya-4.1.2/lddya/
+-rw-rw-rw-   0        0        0    28773 2024-04-19 12:28:51.000000 lddya-4.1.2/lddya/Algorithm.py
+-rw-rw-rw-   0        0        0     7851 2022-11-01 06:31:16.000000 lddya-4.1.2/lddya/Data.py
+-rw-rw-rw-   0        0        0     1444 2022-01-21 14:37:00.000000 lddya-4.1.2/lddya/DataFrame.py
+-rw-rw-rw-   0        0        0     2372 2024-04-11 02:41:50.000000 lddya-4.1.2/lddya/Draw.py
+-rw-rw-rw-   0        0        0     5181 2024-04-16 13:26:39.000000 lddya-4.1.2/lddya/Map.py
+-rw-rw-rw-   0        0        0    16714 2021-12-03 06:05:24.000000 lddya-4.1.2/lddya/Optimizer.py
+-rw-rw-rw-   0        0        0       54 2023-09-07 03:17:02.000000 lddya-4.1.2/lddya/__init__.py
+-rw-rw-rw-   0        0        0      415 2024-04-19 12:27:55.000000 lddya-4.1.2/lddya/tool.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:29:49.348319 lddya-4.1.2/lddya.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-19 12:29:49.000000 lddya-4.1.2/lddya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2024-04-19 12:29:49.000000 lddya-4.1.2/lddya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 12:29:49.000000 lddya-4.1.2/lddya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-19 12:29:49.000000 lddya-4.1.2/lddya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-19 12:29:49.000000 lddya-4.1.2/lddya.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 12:29:49.349318 lddya-4.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      880 2024-04-19 12:29:27.000000 lddya-4.1.2/setup.py
```

### Comparing `lddya-4.1.1/lddya/Algorithm.py` & `lddya-4.1.2/lddya/Algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,16 +172,16 @@
 
 ################################################## 2 A*算法路径规划 ###########################################
 class A_Star_path():
     def __init__(self,map_data,start = np.array([0,0]),end = np.array([0,0])) -> None:
         print('A* Task:',start,end)
         self.map_data = np.array(map_data)
         self.size_map = self.map_data.shape[0]
-        self.start = start
-        self.end   =  end
+        self.start = np.array(start)
+        self.end   =  np.array(end)
         self.open_list  = pd.DataFrame([[start[0],start[1],0,abs(self.start[0]-self.end[0])+abs(self.start[1]-self.end[1]),abs(self.start[0]-self.end[0])+abs(self.start[1]-self.end[1]),-1,-1]],columns=['pos_y','pos_x','g','h','f','parent_y','parent_x'])
         self.close_list = pd.DataFrame([[999,999,0,0,0,0,0]],columns=['pos_y','pos_x','g','h','f','parent_y','parent_x'])
         self.best_way_len = 0
         
 
     def run(self):
         running = True
```

### Comparing `lddya-4.1.1/lddya/Data.py` & `lddya-4.1.2/lddya/Data.py`

 * *Files identical despite different names*

### Comparing `lddya-4.1.1/lddya/DataFrame.py` & `lddya-4.1.2/lddya/DataFrame.py`

 * *Files identical despite different names*

### Comparing `lddya-4.1.1/lddya/Draw.py` & `lddya-4.1.2/lddya/Draw.py`

 * *Files identical despite different names*

### Comparing `lddya-4.1.1/lddya/Map.py` & `lddya-4.1.2/lddya/Map.py`

 * *Files identical despite different names*

### Comparing `lddya-4.1.1/lddya/Optimizer.py` & `lddya-4.1.2/lddya/Optimizer.py`

 * *Files identical despite different names*

