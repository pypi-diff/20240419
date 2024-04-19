# Comparing `tmp/scgraph-1.5.2.tar.gz` & `tmp/scgraph-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-1.5.2.tar", last modified: Wed Apr 17 18:08:15 2024, max compression
+gzip compressed data, was "scgraph-2.0.0.tar", last modified: Fri Apr 19 19:10:45 2024, max compression
```

## Comparing `scgraph-1.5.2.tar` & `scgraph-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.314331 scgraph-1.5.2/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.5.2/LICENSE
--rw-r--r--   0 conmak    (1000) conmak    (1000)    10269 2024-04-17 18:08:15.314331 scgraph-1.5.2/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     9647 2024-02-27 15:29:33.000000 scgraph-1.5.2/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-04-17 16:57:16.000000 scgraph-1.5.2/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.306331 scgraph-1.5.2/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-09-15 15:24:50.000000 scgraph-1.5.2/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    33414 2024-04-17 17:55:15.000000 scgraph-1.5.2/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.310331 scgraph-1.5.2/scgraph/geographs/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-09-15 15:24:50.000000 scgraph-1.5.2/scgraph/geographs/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143112 2024-03-04 21:44:33.000000 scgraph-1.5.2/scgraph/geographs/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   923120 2024-03-04 21:46:50.000000 scgraph-1.5.2/scgraph/geographs/north_america_rail.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   976574 2024-03-04 21:47:47.000000 scgraph-1.5.2/scgraph/geographs/oak_ridge_maritime.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1414756 2024-03-04 21:48:18.000000 scgraph-1.5.2/scgraph/geographs/us_freeway.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     3946 2024-02-27 15:33:35.000000 scgraph-1.5.2/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.314331 scgraph-1.5.2/scgraph.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)    10269 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-04-17 18:08:15.314331 scgraph-1.5.2/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.098317 scgraph-2.0.0/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-2.0.0/LICENSE
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9178 2024-04-19 19:10:45.098317 scgraph-2.0.0/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8556 2024-04-19 19:07:52.000000 scgraph-2.0.0/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-04-19 18:27:15.000000 scgraph-2.0.0/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.090317 scgraph-2.0.0/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-19 19:03:42.000000 scgraph-2.0.0/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    38367 2024-04-19 19:09:29.000000 scgraph-2.0.0/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.094317 scgraph-2.0.0/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-09-15 15:24:50.000000 scgraph-2.0.0/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   733914 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   557967 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/north_america_rail.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   583015 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/oak_ridge_maritime.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   867927 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/us_freeway.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4256 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.098317 scgraph-2.0.0/scgraph.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9178 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-04-19 19:10:45.098317 scgraph-2.0.0/setup.cfg
```

### Comparing `scgraph-1.5.2/LICENSE` & `scgraph-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.2/PKG-INFO` & `scgraph-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.5.2
+Version: 2.0.0
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 
 ![scgraph](https://raw.githubusercontent.com/connor-makowski/scgraph/main/static/scgraph.png)
 
 ## Documentation
 
 Getting Started: https://github.com/connor-makowski/scgraph
 
-Low Level: https://connor-makowski.github.io/scgraph/core.html
+Low Level: https://connor-makowski.github.io/scgraph/scgraph/core.html
 
 
 ## Key Features
 
 - Calculate the shortest path between two points on earth using a latitude / longitude pair
     - Inputs:
         - A latitude / longitude pair for the origin
@@ -85,41 +85,25 @@
     origin_node={"latitude": 31.23,"longitude": 121.47}, 
     destination_node={"latitude": 32.08,"longitude": -81.09},
     output_units='km'
 )
 print('Length: ',output['length']) #=> Length:  19596.4653
 ```
 
-In the above example, the `output` variable is a dictionary with three keys: `length`, `coordinate_path` and `path`.
+In the above example, the `output` variable is a dictionary with three keys: `length` and `coordinate_path`.
 
 - `length`: The distance between the passed origin and destination when traversing the graph along the shortest path
     - Notes: 
         - This will be in the units specified by the `output_units` parameter. 
         - `output_units` options:
             - `km` (kilometers - default)
             - `m` (meters)
             - `mi` (miles)
             - `ft` (feet)
-- `coordinate_path`: A list of dictionaries (`latitude` and `longitude`) that make up the shortest path
-- `path`: A list of node ids (from the network data set) that make up the shortest path
-    - In general, these are only relevant if you are providing your own custom network data set
-
-To get the latitude / longitude pairs that make up the shortest path, as a list of lists, you could do something like the following:
-
-```py
-# Use a maritime network geograph
-from scgraph.geographs.marnet import marnet_geograph
-
-# Get the shortest path between 
-output = marnet_geograph.get_shortest_path(
-    origin_node={"latitude": 31.23,"longitude": 121.47}, 
-    destination_node={"latitude": 32.08,"longitude": -81.09}
-)
-print(str([[i['latitude'],i['longitude']] for i in output['coordinate_path']]))
-```
+- `coordinate_path`: A list of lists [`latitude`,`longitude`] that make up the shortest path
 
 ## Included GeoGraphs
 
 - marnet_geograph:
     - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
     - Attribution: [searoute](https://github.com/genthalili/searoute-py)
@@ -183,59 +167,59 @@
 You can specify your own custom graphs for direct access to the solving algorithms. This requires the use of the low level `Graph` class
 
 ```py
 from scgraph import Graph
 
 # Define a graph
 # See the graph definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-graph = {
-    0:{1: 5, 2: 1},
-    1:{0: 5, 2: 2, 3: 1},
-    2:{0: 1, 1: 2, 3: 4, 4: 8},
-    3:{1: 1, 2: 4, 4: 3, 5: 6},
-    4:{2: 8, 3: 3},
-    5:{3: 6}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+graph = [
+    {1: 5, 2: 1},
+    {0: 5, 2: 2, 3: 1},
+    {0: 1, 1: 2, 3: 4, 4: 8},
+    {1: 1, 2: 4, 4: 3, 5: 6},
+    {2: 8, 3: 3},
+    {3: 6}
+]
 
 # Optional: Validate your graph
 Graph.validate_graph(graph=graph)
 
-# Get the shortest path between 0 and 5
+# Get the shortest path between idx 0 and idx 5
 output = Graph.dijkstra_makowski(graph=graph, origin_id=0, destination_id=5)
 #=> {'path': [0, 2, 1, 3, 5], 'length': 10}
 ```
 
 You can also use a slightly higher level `GeoGraph` class to work with latitude / longitude pairs
 
 ```py
 from scgraph import GeoGraph
 
 # Define nodes
 # See the nodes definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-nodes = {
-    0: {"latitude": 0, "longitude": 0},
-    1: {"latitude": 0, "longitude": 1},
-    2: {"latitude": 1, "longitude": 0},
-    3: {"latitude": 1, "longitude": 1},
-    4: {"latitude": 1, "longitude": 2},
-    5: {"latitude": 2, "longitude": 1}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+nodes = [
+    [0,0],
+    [0,1],
+    [1,0],
+    [1,1],
+    [1,2],
+    [2,1]
+]
 # Define a graph
 # See the graph definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-graph = {
-    0:{1: 5, 2: 1},
-    1:{0: 5, 2: 2, 3: 1},
-    2:{0: 1, 1: 2, 3: 4, 4: 8},
-    3:{1: 1, 2: 4, 4: 3, 5: 6},
-    4:{2: 8, 3: 3},
-    5:{3: 6}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+graph = [
+    {1: 5, 2: 1},
+    {0: 5, 2: 2, 3: 1},
+    {0: 1, 1: 2, 3: 4, 4: 8},
+    {1: 1, 2: 4, 4: 3, 5: 6},
+    {2: 8, 3: 3},
+    {3: 6}
+]
 
 # Create a GeoGraph object
 my_geograph = GeoGraph(nodes=nodes, graph=graph)
 
 # Optional: Validate your graph
 my_geograph.validate_graph()
 
@@ -245,23 +229,22 @@
 # Get the shortest path between two points
 output = my_geograph.get_shortest_path(
     origin_node = {'latitude': 0, 'longitude': 0},
     destination_node = {'latitude': 2, 'longitude': 1}
 )
 #=>
 # {
-#     "path": [6, 0, 2, 1, 3, 5, 7],
 #     "coordinate_path": [
-#         {'latitude': 0, 'longitude': 0},
-#         {'latitude': 0, 'longitude': 0},
-#         {'latitude': 1, 'longitude': 0},
-#         {'latitude': 0, 'longitude': 1},
-#         {'latitude': 1, 'longitude': 1},
-#         {'latitude': 2, 'longitude': 1},
-#         {'latitude': 2, 'longitude': 1}
+#         [0,0],
+#         [0,0],
+#         [1,0],
+#         [0,1],
+#         [1,1],
+#         [2,1],
+#         [2,1]
 #     ],
 #     "length": 10
 # }
 ```
 
 ## Attributions and Thanks
 Originally inspired by [searoute](https://github.com/genthalili/searoute-py) including the use of one of their [datasets](https://github.com/genthalili/searoute-py/blob/main/searoute/data/marnet_densified_v2_old.geojson) that has been modified to work properly with this package.
```

### Comparing `scgraph-1.5.2/README.md` & `scgraph-2.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 ![scgraph](https://raw.githubusercontent.com/connor-makowski/scgraph/main/static/scgraph.png)
 
 ## Documentation
 
 Getting Started: https://github.com/connor-makowski/scgraph
 
-Low Level: https://connor-makowski.github.io/scgraph/core.html
+Low Level: https://connor-makowski.github.io/scgraph/scgraph/core.html
 
 
 ## Key Features
 
 - Calculate the shortest path between two points on earth using a latitude / longitude pair
     - Inputs:
         - A latitude / longitude pair for the origin
@@ -70,41 +70,25 @@
     origin_node={"latitude": 31.23,"longitude": 121.47}, 
     destination_node={"latitude": 32.08,"longitude": -81.09},
     output_units='km'
 )
 print('Length: ',output['length']) #=> Length:  19596.4653
 ```
 
-In the above example, the `output` variable is a dictionary with three keys: `length`, `coordinate_path` and `path`.
+In the above example, the `output` variable is a dictionary with three keys: `length` and `coordinate_path`.
 
 - `length`: The distance between the passed origin and destination when traversing the graph along the shortest path
     - Notes: 
         - This will be in the units specified by the `output_units` parameter. 
         - `output_units` options:
             - `km` (kilometers - default)
             - `m` (meters)
             - `mi` (miles)
             - `ft` (feet)
-- `coordinate_path`: A list of dictionaries (`latitude` and `longitude`) that make up the shortest path
-- `path`: A list of node ids (from the network data set) that make up the shortest path
-    - In general, these are only relevant if you are providing your own custom network data set
-
-To get the latitude / longitude pairs that make up the shortest path, as a list of lists, you could do something like the following:
-
-```py
-# Use a maritime network geograph
-from scgraph.geographs.marnet import marnet_geograph
-
-# Get the shortest path between 
-output = marnet_geograph.get_shortest_path(
-    origin_node={"latitude": 31.23,"longitude": 121.47}, 
-    destination_node={"latitude": 32.08,"longitude": -81.09}
-)
-print(str([[i['latitude'],i['longitude']] for i in output['coordinate_path']]))
-```
+- `coordinate_path`: A list of lists [`latitude`,`longitude`] that make up the shortest path
 
 ## Included GeoGraphs
 
 - marnet_geograph:
     - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
     - Attribution: [searoute](https://github.com/genthalili/searoute-py)
@@ -168,59 +152,59 @@
 You can specify your own custom graphs for direct access to the solving algorithms. This requires the use of the low level `Graph` class
 
 ```py
 from scgraph import Graph
 
 # Define a graph
 # See the graph definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-graph = {
-    0:{1: 5, 2: 1},
-    1:{0: 5, 2: 2, 3: 1},
-    2:{0: 1, 1: 2, 3: 4, 4: 8},
-    3:{1: 1, 2: 4, 4: 3, 5: 6},
-    4:{2: 8, 3: 3},
-    5:{3: 6}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+graph = [
+    {1: 5, 2: 1},
+    {0: 5, 2: 2, 3: 1},
+    {0: 1, 1: 2, 3: 4, 4: 8},
+    {1: 1, 2: 4, 4: 3, 5: 6},
+    {2: 8, 3: 3},
+    {3: 6}
+]
 
 # Optional: Validate your graph
 Graph.validate_graph(graph=graph)
 
-# Get the shortest path between 0 and 5
+# Get the shortest path between idx 0 and idx 5
 output = Graph.dijkstra_makowski(graph=graph, origin_id=0, destination_id=5)
 #=> {'path': [0, 2, 1, 3, 5], 'length': 10}
 ```
 
 You can also use a slightly higher level `GeoGraph` class to work with latitude / longitude pairs
 
 ```py
 from scgraph import GeoGraph
 
 # Define nodes
 # See the nodes definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-nodes = {
-    0: {"latitude": 0, "longitude": 0},
-    1: {"latitude": 0, "longitude": 1},
-    2: {"latitude": 1, "longitude": 0},
-    3: {"latitude": 1, "longitude": 1},
-    4: {"latitude": 1, "longitude": 2},
-    5: {"latitude": 2, "longitude": 1}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+nodes = [
+    [0,0],
+    [0,1],
+    [1,0],
+    [1,1],
+    [1,2],
+    [2,1]
+]
 # Define a graph
 # See the graph definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-graph = {
-    0:{1: 5, 2: 1},
-    1:{0: 5, 2: 2, 3: 1},
-    2:{0: 1, 1: 2, 3: 4, 4: 8},
-    3:{1: 1, 2: 4, 4: 3, 5: 6},
-    4:{2: 8, 3: 3},
-    5:{3: 6}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+graph = [
+    {1: 5, 2: 1},
+    {0: 5, 2: 2, 3: 1},
+    {0: 1, 1: 2, 3: 4, 4: 8},
+    {1: 1, 2: 4, 4: 3, 5: 6},
+    {2: 8, 3: 3},
+    {3: 6}
+]
 
 # Create a GeoGraph object
 my_geograph = GeoGraph(nodes=nodes, graph=graph)
 
 # Optional: Validate your graph
 my_geograph.validate_graph()
 
@@ -230,23 +214,22 @@
 # Get the shortest path between two points
 output = my_geograph.get_shortest_path(
     origin_node = {'latitude': 0, 'longitude': 0},
     destination_node = {'latitude': 2, 'longitude': 1}
 )
 #=>
 # {
-#     "path": [6, 0, 2, 1, 3, 5, 7],
 #     "coordinate_path": [
-#         {'latitude': 0, 'longitude': 0},
-#         {'latitude': 0, 'longitude': 0},
-#         {'latitude': 1, 'longitude': 0},
-#         {'latitude': 0, 'longitude': 1},
-#         {'latitude': 1, 'longitude': 1},
-#         {'latitude': 2, 'longitude': 1},
-#         {'latitude': 2, 'longitude': 1}
+#         [0,0],
+#         [0,0],
+#         [1,0],
+#         [0,1],
+#         [1,1],
+#         [2,1],
+#         [2,1]
 #     ],
 #     "length": 10
 # }
 ```
 
 ## Attributions and Thanks
 Originally inspired by [searoute](https://github.com/genthalili/searoute-py) including the use of one of their [datasets](https://github.com/genthalili/searoute-py/blob/main/searoute/data/marnet_densified_v2_old.geojson) that has been modified to work properly with this package.
```

### Comparing `scgraph-1.5.2/pyproject.toml` & `scgraph-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scgraph"
-version = "1.5.2"
+version = "2.0.0"
 description = "Determine an approximate route between two points on earth."
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `scgraph-1.5.2/scgraph/core.py` & `scgraph-2.0.0/scgraph/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from .utils import haversine, hard_round, distance_converter
 import json
 
 
 class Graph:
     @staticmethod
     def validate_graph(
-        graph: dict, check_symmetry: bool = True, check_connected: bool = True
+        graph: list[dict],
+        check_symmetry: bool = True,
+        check_connected: bool = True,
     ) -> None:
         """
         Function:
 
         - Validate that a graph is properly formatted
 
         Required Arguments:
 
         - `graph`
-            - Type: dict
-            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
-            - Note: Ids must be integers starting at 0 and increasing sequentially to the number of nodes in the graph
+            - Type: list of dictionaries
+            - What: A list of dictionaries where the indicies are origin node ids and the values are dictionaries of destination node indices and distances
             - Note: All nodes must be included as origins in the graph regardless of if they have any connected destinations
 
         Optional Arguments:
 
         - `check_symmetry`
             - Type: bool
             - What: Whether to check that the graph is symmetric
@@ -31,75 +32,64 @@
             - Type: bool
             - What: Whether to check that the graph is fully connected
             - Default: True
             - Note: For computational efficiency, only symmetric graphs are checked for connectivity
             - Note: If this is True, `check_symmetry` is forced to True and the graph will be checked for symmetry prior to checking for connectivity
         """
         check_symmetry = check_symmetry or check_connected
-        ids = []
-        assert isinstance(graph, dict), "Your graph must be a dictionary"
-        for origin_id, origin_dict in graph.items():
-            assert isinstance(
-                origin_id, int
-            ), f"Origin and destination ids must be integers but {origin_id} is not an integer"
+        assert isinstance(graph, list), "Your graph must be a list"
+        len_graph = len(graph)
+        for origin_id, origin_dict in enumerate(graph):
             assert isinstance(
                 origin_dict, dict
             ), f"Your graph must be a dictionary of dictionaries but the value for origin {origin_id} is not a dictionary"
-            ids.append(origin_id)
-            for destination_id, distance in origin_dict.items():
-                assert isinstance(
-                    destination_id, int
-                ), f"Origin and destination ids must be integers but {destination_id} at graph[{origin_id}] is not an integer"
-                assert isinstance(
-                    distance, (int, float)
-                ), f"Distances must be integers or floats but {distance} at graph[{origin_id}][{destination_id}] is not an integer or float"
-                ids.append(destination_id)
-                if check_symmetry:
+            destinations = list(origin_dict.keys())
+            lengths = list(origin_dict.values())
+            assert all(
+                [
+                    (isinstance(i, int) and i >= 0 and i < len_graph)
+                    for i in destinations
+                ]
+            ), f"Destination ids must be non-negative integers and equivalent to an existing index, but graph[{origin_id}] has an error in the destination ids"
+            assert all(
+                [(isinstance(i, (int, float)) and i >= 0) for i in lengths]
+            ), f"Distances must be integers or floats, but graph[{origin_id}] contains a non-integer or non-float distance"
+            if check_symmetry:
+                for destination_id, distance in origin_dict.items():
                     assert (
-                        graph.get(destination_id, {}).get(origin_id) == distance
+                        graph[destination_id].get(origin_id) == distance
                     ), f"Your graph is not symmetric, the distance from node {origin_id} to node {destination_id} is {distance} but the distance from node {destination_id} to node {origin_id} is {graph.get(destination_id, {}).get(origin_id)}"
-        ids = set(ids)
-        assert (
-            min(ids) == 0
-        ), f"Your graph must have ids starting at 0 but the minimum id is {min(ids)}"
-        assert (
-            max(ids) == len(ids) - 1
-        ), f"Your graph must have ids that are sequential starting at 0 but the maximum id is {max(ids)}"
-        assert len(graph) == len(
-            ids
-        ), f"Your graph must have origin ids for all nodes regardless of if they have any connected destinations"
         if check_connected:
             assert Graph.validate_connected(
                 graph
             ), "Your graph is not fully connected"
 
     @staticmethod
-    def validate_connected(graph: dict) -> bool:
+    def validate_connected(graph: list[dict]) -> bool:
         """
         Function:
 
         - Validate that a graph is fully connected
             - This means that every node in the graph has a path to every other node in the graph
             - Note: This assumes that the graph is symmetric
         - Return True if the graph is fully connected and False if it is not
 
         Required Arguments:
 
         - `graph`
-            - Type: dict
-            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
-            - Note: Ids must be integers starting at 0 and increasing sequentially to the number of nodes in the graph
+            - Type: list of dictionaries
+            - What: A list of dictionaries where the indicies are origin node ids and the values are dictionaries of destination node ids and distances
             - Note: All nodes must be included as origins in the graph regardless of if they have any connected destinations
 
         Optional Arguments:
 
         - None
         """
         origin_id = 0
-        destination_id = max(graph) + 1
+        destination_id = len(graph) + 1
 
         distance_matrix = [float("inf") for i in graph]
         open_leaves = {}
         predecessor = [None for i in graph]
 
         distance_matrix[origin_id] = 0
         open_leaves[origin_id] = 0
@@ -116,62 +106,74 @@
                 possible_distance = current_distance + connected_distance
                 if possible_distance < distance_matrix[connected_id]:
                     distance_matrix[connected_id] = possible_distance
                     predecessor[connected_id] = current_id
                     open_leaves[connected_id] = possible_distance
 
     @staticmethod
-    def input_check(graph: dict, origin_id: int, destination_id: int) -> None:
+    def input_check(
+        graph: list[dict], origin_id: int, destination_id: int
+    ) -> None:
         """
         Function:
 
         - Check that the inputs passed to the shortest path algorithm are valid
         - Raises an exception if the inputs passed are not valid
 
         Required Arguments:
 
         - `graph`
-            - Type: dict
-            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+            - Type: list[dict]
+            - What: A list of dictionaries where the indicies are origin node ids and the values are dictionaries of destination node ids and distances
         - `origin_id`
             - Type: int
             - What: The id of the origin node from the graph dictionary to start the shortest path from
         - `destination_id`
             - Type: int
             - What: The id of the destination node from the graph dictionary to end the shortest path at
 
         Optional Arguments:
 
         - None
         """
-        if origin_id not in graph:
+        if (
+            not isinstance(origin_id, int)
+            and origin_id < len(graph)
+            and origin_id >= 0
+        ):
             raise Exception(f"Origin node ({origin_id}) is not in the graph")
-        if destination_id not in graph:
+        if (
+            not isinstance(destination_id, int)
+            and origin_id < len(graph)
+            and origin_id >= 0
+        ):
             raise Exception(
                 f"Destination node ({destination_id}) is not in the graph"
             )
 
     @staticmethod
-    def dijkstra(graph: dict, origin_id: int, destination_id: int) -> dict:
+    def dijkstra(
+        graph: list[dict], origin_id: int, destination_id: int
+    ) -> dict:
         """
         Function:
 
         - Identify the shortest path between two nodes in a sparse network graph using a modified dijkstra algorithm
             - Modifications allow for a sparse distance matrix to be used instead of a dense distance matrix
             - This can dramatically reduce the memory and compute requirements of the algorithm
             - This algorithm runs in O(n^2) time where n is the number of nodes in the graph
         - Return a dictionary of various path information including:
             - `id_path`: A list of node ids in the order they are visited
             - `path`: A list of node dictionaries (lat + long) in the order they are visited
 
         Required Arguments:
 
         - `graph`
-            - Type: dict
-            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+            - Type: list[dict]
+            - What: A list of dictionaries where the indicies are origin node ids and the values are dictionaries of destination node ids and distances
         - `origin_id`
             - Type: int
             - What: The id of the origin node from the graph dictionary to start the shortest path from
         - `destination_id`
             - Type: int
             - What: The id of the destination node from the graph dictionary to end the shortest path at
 
@@ -216,15 +218,15 @@
         return {
             "path": output_path,
             "length": hard_round(4, distance_matrix[destination_id]),
         }
 
     @staticmethod
     def dijkstra_makowski(
-        graph: dict, origin_id: int, destination_id: int
+        graph: list[dict], origin_id: int, destination_id: int
     ) -> dict:
         """
         Function:
 
         - Identify the shortest path between two nodes in a sparse network graph using Makowski's modified Dijkstra algorithm
             - Modifications allow for a sparse distance matrix to be used instead of a dense distance matrix
             - Improvements include only computing future potential nodes based on the open leaves for each branch
@@ -237,16 +239,16 @@
         - Return a dictionary of various path information including:
             - `id_path`: A list of node ids in the order they are visited
             - `path`: A list of node dictionaries (lat + long) in the order they are visited
 
         Required Arguments:
 
         - `graph`
-            - Type: dict
-            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+            - Type: list[dict]
+            - What: A list of dictionaries where the indicies are origin node ids and the values are dictionaries of destination node ids and distances
         - `origin_id`
             - Type: int
             - What: The id of the origin node from the graph dictionary to start the shortest path from
         - `destination_id`
             - Type: int
             - What: The id of the destination node from the graph dictionary to end the shortest path at
 
@@ -291,32 +293,32 @@
         return {
             "path": output_path,
             "length": hard_round(4, distance_matrix[destination_id]),
         }
 
 
 class GeoGraph:
-    def __init__(self, graph: dict, nodes: dict) -> None:
+    def __init__(
+        self, graph: list[dict], nodes: list[list[int | float]]
+    ) -> None:
         """
         Function:
 
         - Create a GeoGraph object
 
         Required Arguments:
 
         - `graph`
-            - Type: dict
-            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
-            - Note: Ids must be integers starting at 0 and increasing sequentially to the number of nodes in the graph
+            - Type: list of dictionaries
+            - What: A list of dictionaries where the indicies are origin node ids and the values are dictionaries of destination node indices and distances
             - Note: All nodes must be included as origins in the graph regardless of if they have any connected destinations
         - `nodes`
-            - Type: dict
-            - What: A dictionary of dictionaries where the keys are node ids and the values are dictionaries of node coordinates (latitude and longitude)
-            - Note: Ids must be integers starting at 0 and increasing sequentially to the number of nodes in the graph
-            - Note: All nodes must be included in the nodes dictionary
+            - Type: list of lists
+            - What: A list of lists where the values are coordinates (latitude then longitude)
+            - Note: The length of the nodes list must be the same as that of the graph list
 
         Optional Arguments:
 
         """
         self.graph = graph
         self.nodes = nodes
 
@@ -366,50 +368,49 @@
 
         - None
 
         Optional Arguments:
 
         - None
         """
-        assert isinstance(self.nodes, dict), "Your nodes must be a dictionary"
-        for node, node_dict in self.nodes.items():
-            assert isinstance(
-                node_dict, dict
-            ), f"Your nodes must be a dictionary of dictionaries but the value for node {node} is not a dictionary"
-            for key, value in node_dict.items():
-                assert key in [
-                    "latitude",
-                    "longitude",
-                ], f"Your nodes must be a dictionary of dictionaries where the keys are 'latitude' and 'longitude' but the key ({key}) for node ({node}) is not 'latitude' or 'longitude'"
-                assert isinstance(
-                    value,
-                    (
-                        float,
-                        int,
-                    ),
-                ), f"Your nodes must be a dictionary of dictionaries where the values are floats or ints but the value for node ({node}) and key ({key}) is not a float"
-            assert (
-                node_dict.get("latitude") >= -90
-                and node_dict.get("latitude") <= 90
-            ), f"Your latitude values must be between -90 and 90 but the latitude value for node {node} is {node_dict.get('latitude')}"
-            assert (
-                node_dict.get("longitude") >= -180
-                and node_dict.get("longitude") <= 180
-            ), f"Your longitude values must be between -180 and 180 but the longitude value for node {node} is {node_dict.get('longitude')}"
+        assert isinstance(self.nodes, list), "Your nodes must be a dictionary"
+        assert all(
+            [isinstance(i, list) for i in self.nodes]
+        ), "Your nodes must be a list of lists"
+        assert all(
+            [len(i) == 2 for i in self.nodes]
+        ), "Your nodes must be a list of lists where each sub list has a length of 2"
+        assert all(
+            [
+                (
+                    isinstance(i[0], (int, float))
+                    and isinstance(i[1], (int, float))
+                )
+                for i in self.nodes
+            ]
+        ), "Your nodes must be a list of lists where each sub list has a numeric latitude and longitude value"
+        assert all(
+            [
+                (i[0] >= -90 and i[0] <= 90 and i[1] >= -180 and i[1] <= 180)
+                for i in self.nodes
+            ]
+        ), "Your nodes must be a list of lists where each sub list has a length of 2 with a latitude [-90,90] and longitude [-180,180] value"
 
     def get_shortest_path(
         self,
         origin_node,
         destination_node,
         output_units: str = "km",
         algorithm_fn=Graph.dijkstra_makowski,
         off_graph_circuity: [float, int] = 1,
         node_addition_type: str = "quadrant",
         node_addition_circuity: [float, int] = 4,
         geograph_units: str = "km",
+        output_coordinate_path: str = "list_of_lists",
+        output_path: bool = False,
         **kwargs,
     ) -> dict:
         """
         Function:
 
         - Identify the shortest path between two nodes in a sparse network graph
 
@@ -487,17 +488,29 @@
             - Default: 'km'
             - Options:
                 - 'km': Kilometers
                 - 'm': Meters
                 - 'mi': Miles
                 - 'ft': Feet
             - Note: In general, all scgraph provided geographs be in kilometers
+        - `output_coordinate_path`
+            - Type: str
+            - What: The format of the output coordinate path
+            - Default: 'list_of_lists'
+            - Options:
+                - 'list_of_dicts': A list of dictionaries with keys 'latitude' and 'longitude'
+                - 'list_of_lists': A list of lists with the first value being latitude and the second being longitude
+        - `output_path`
+            - Type: bool
+            - What: Whether to output the path as a list of geograph node ids (for debugging and other advanced uses)
+            - Default: False
         - `**kwargs`
             - Additional keyword arguments. These are included for forwards and backwards compatibility reasons, but are not currently used.
         """
+        original_graph_length = len(self.graph)
         # Add the origin and destination nodes to the graph
         origin_id = self.add_node(
             node=origin_node,
             node_addition_type=node_addition_type,
             circuity=node_addition_circuity,
         )
         destination_id = self.add_node(
@@ -519,20 +532,27 @@
                 off_graph_circuity=off_graph_circuity,
             )
             output["length"] = distance_converter(
                 output["length"],
                 input_units=geograph_units,
                 output_units=output_units,
             )
-            self.remove_added_node(node_id=origin_id)
-            self.remove_added_node(node_id=destination_id)
+            if output_coordinate_path == "list_of_dicts":
+                output["coordinate_path"] = [
+                    {"latitude": i[0], "longitude": i[1]}
+                    for i in output["coordinate_path"]
+                ]
+            if not output_path:
+                del output["path"]
+            while len(self.graph) > original_graph_length:
+                self.remove_appended_node()
             return output
         except Exception as e:
-            self.remove_added_node(node_id=origin_id)
-            self.remove_added_node(node_id=destination_id)
+            while len(self.graph) > original_graph_length:
+                self.remove_appended_node()
             raise e
 
     def adujust_circuity_length(
         self,
         output: dict,
         node_addition_circuity: [float, int],
         off_graph_circuity: [float, int],
@@ -585,48 +605,149 @@
 
         Optional Arguments:
 
         - None
         """
         return [self.nodes[node_id] for node_id in path]
 
-    def remove_added_node(self, node_id: int) -> None:
+    def remove_appended_node(self) -> None:
         """
         Function:
 
-        - Remove a node that has been added to the network from the network
+        - Remove the last node that was appended to the graph
         - Assumes that this node has symmetric flows
             - EG: If node A has a distance of 10 to node B, then node B has a distance of 10 to node A
         - Return None
 
         Required Arguments:
 
-        - `node_id`
-            - Type: str
-            - What: The name of the node to remove
+        - None
 
         Optional Arguments:
 
         - None
         """
-        # Assert that the node exists
-        assert (
-            node_id in self.nodes
-        ), f"Node {node_id} does not exist in the network"
-        reverse_connections = [i for i in self.graph[node_id].keys()]
+        node_id = len(self.graph) - 1
         for reverse_connection in [i for i in self.graph[node_id].keys()]:
             del self.graph[reverse_connection][node_id]
-        del self.graph[node_id]
-        del self.nodes[node_id]
+        self.graph = self.graph[:node_id]
+        self.nodes = self.nodes[:node_id]
+
+    def get_node_distances(
+        self,
+        node: list,
+        circuity: [int, float],
+        node_addition_type: str,
+        node_addition_math: str,
+        lat_lon_bound: [int, float],
+    ):
+        """
+        Function:
+
+        - Get the distances between a node and all other nodes in the graph
+        - This is used to determine the closest node to add to the graph when adding a new node
+
+        Required Arguments:
+
+        - `node`
+            - Type: list
+            - What: A list of the latitude and longitude of the node
+            - EG: [latitude, longitude] -> [31.23, 121.47]
+        - `circuity`
+            - Type: float | int
+            - What: The circuity to apply to any distance calculations
+            - Note: This defaults to 4 to prevent the algorithm from taking a direct route in direction of the destination over some impassible terrain (EG: a maritime network that goes through land)
+        - `node_addition_type`
+            - Type: str
+            - What: The type of node addition to use
+            - Options:
+                - 'quadrant': Add the closest node in each quadrant (ne, nw, se, sw) to the distance matrix for this node
+                - 'closest': Add only the closest node to the distance matrix for this node
+                - 'all': Add all nodes to the distance matrix for this node
+            - Notes:
+                - `dijkstra_makowski` will operate substantially faster if the `node_addition_type` is set to 'quadrant' or 'closest'
+                - `dijkstra` will operate at the similar speeds regardless of the `node_addition_type`
+                - When using `all`, you should consider using `dijkstra` instead of `dijkstra_makowski` as it will be faster
+        - `node_addition_math`
+            - Type: str
+            - What: The math to use when calculating the distance between nodes when determining the closest node (or closest quadrant node) to add to the graph
+            - Default: 'euclidean'
+            - Options:
+                - 'euclidean': Use the euclidean distance between nodes. This is much faster but is not accurate (especially near the poles)
+                - 'haversine': Use the haversine distance between nodes. This is slower but is an accurate representation of the surface distance between two points on the earth
+            - Notes:
+                - Once the closest node (or closest quadrant node) is determined, the haversine distance (with circuity) is used to calculate the distance between the nodes when adding it to the graph.
+        - `lat_lon_bound`
+            - Type: float | int
+            - What: Forms a bounding box around the node that is to be added to graph. Only selects graph nodes to consider joining that are within this bounding box.
+        """
+        assert node_addition_type in [
+            "quadrant",
+            "all",
+            "closest",
+        ], f"Invalid node addition type provided ({node_addition_type}), valid options are: ['quadrant', 'all', 'closest']"
+        assert node_addition_math in [
+            "euclidean",
+            "haversine",
+        ], f"Invalid node addition math provided ({node_addition_math}), valid options are: ['euclidean', 'haversine']"
+        # Get only bounded nodes
+        nodes = {
+            node_idx: node_i
+            for node_idx, node_i in enumerate(self.nodes)
+            if abs(node_i[0] - node[0]) < lat_lon_bound
+            and abs(node_i[1] - node[1]) < lat_lon_bound
+        }
+        if len(nodes) == 0:
+            # Default to all if the lat_lon_bound fails to find any nodes
+            return self.get_node_distances(
+                node=nodes,
+                circuity=circuity,
+                lat_lon_bound=180,
+                node_addition_type=node_addition_type,
+                node_addition_math=node_addition_math,
+            )
+        if node_addition_type == "all":
+            return {
+                node_idx: round(haversine(node, node_i, circuity=circuity), 4)
+                for node_idx, node_i in nodes.items()
+            }
+        if node_addition_math == "haversine":
+            dist_fn = lambda x: round(haversine(node, x, circuity=circuity), 4)
+        else:
+            dist_fn = lambda x: round(
+                ((node[0] - x[0]) ** 2 + (node[1] - x[1]) ** 2) ** 0.5, 4
+            )
+        if node_addition_type == "closest":
+            quadrant_fn = lambda x, y: "all"
+        else:
+            quadrant_fn = lambda x, y: ("n" if x[0] - y[0] > 0 else "s") + (
+                "e" if x[1] - y[1] > 0 else "w"
+            )
+        min_diffs = {}
+        min_diffs_idx = {}
+        for node_idx, node_i in nodes.items():
+            quadrant = quadrant_fn(node_i, node)
+            dist = dist_fn(node_i)
+            if dist < min_diffs.get(quadrant, 999999999):
+                min_diffs[quadrant] = dist
+                min_diffs_idx[quadrant] = node_idx
+        return {
+            node_idx: round(
+                haversine(node, self.nodes[node_idx], circuity=circuity), 4
+            )
+            for node_idx in min_diffs_idx.values()
+        }
 
     def add_node(
         self,
-        node: dict,
+        node: dict[int, float],
         circuity: [float, int],
         node_addition_type: str = "quadrant",
+        node_addition_math: str = "euclidean",
+        lat_lon_bound: [int, float] = 5,
     ) -> int:
         """
         Function:
 
         - Add a node to the network
         - Returns the id of the new node
 
@@ -651,14 +772,27 @@
                 - 'quadrant': Add the closest node in each quadrant (ne, nw, se, sw) to the distance matrix for this node
                 - 'closest': Add only the closest node to the distance matrix for this node
                 - 'all': Add all nodes to the distance matrix for this node
             - Notes:
                 - `dijkstra_makowski` will operate substantially faster if the `node_addition_type` is set to 'quadrant' or 'closest'
                 - `dijkstra` will operate at the similar speeds regardless of the `node_addition_type`
                 - When using `all`, you should consider using `dijkstra` instead of `dijkstra_makowski` as it will be faster
+        - `node_addition_math`
+            - Type: str
+            - What: The math to use when calculating the distance between nodes when determining the closest node (or closest quadrant node) to add to the graph
+            - Default: 'euclidean'
+            - Options:
+                - 'euclidean': Use the euclidean distance between nodes. This is much faster but is not accurate (especially near the poles)
+                - 'haversine': Use the haversine distance between nodes. This is slower but is an accurate representation of the surface distance between two points on the earth
+            - Notes:
+                - Once the closest node (or closest quadrant node) is determined, the haversine distance (with circuity) is used to calculate the distance between the nodes when adding it to the graph.
+        - `lat_lon_bound`
+            - Type: float | int
+            - What: Forms a bounding box around the node that is to be added to graph. Only selects graph nodes to consider joining that are within this bounding box.
+            - Default: 5
 
         """
         # Validate the inputs
         assert isinstance(node, dict), "Node must be a dictionary"
         assert "latitude" in node.keys(), "Node must have a latitude"
         assert "longitude" in node.keys(), "Node must have a longitude"
         assert (
@@ -669,64 +803,39 @@
         ), "Longitude must be between -180 and 180"
         assert circuity > 0, "Circuity must be greater than 0"
         assert node_addition_type in [
             "quadrant",
             "all",
             "closest",
         ], f"Invalid node addition type provided ({node_addition_type}), valid options are: ['quadrant', 'all', 'closest']"
+        assert node_addition_math in [
+            "euclidean",
+            "haversine",
+        ], f"Invalid node addition math provided ({node_addition_math}), valid options are: ['euclidean', 'haversine']"
+        assert isinstance(
+            lat_lon_bound, (int, float)
+        ), "Lat_lon_bound must be a number"
+        assert lat_lon_bound > 0, "Lat_lon_bound must be greater than 0"
 
+        node = [node["latitude"], node["longitude"]]
         # Get the distances to all other nodes
-        distances = {
-            node_i_id: {
-                "distance": round(
-                    haversine(node, node_i, circuity=circuity), 4
-                ),
-                "quadrant": (
-                    "n" if node["latitude"] > node_i["latitude"] else "s"
-                )
-                + ("e" if node["longitude"] > node_i["longitude"] else "w"),
-            }
-            for node_i_id, node_i in self.nodes.items()
-        }
+        distances = self.get_node_distances(
+            node=node,
+            circuity=circuity,
+            node_addition_type=node_addition_type,
+            node_addition_math=node_addition_math,
+            lat_lon_bound=lat_lon_bound,
+        )
 
         # Create the node
-        new_node_id = max(self.graph) + 1
-        self.nodes[new_node_id] = node
-        self.graph[new_node_id] = {}
-
-        if node_addition_type == "all":
-            for node_i_id, node_i_distnace_dict in distances.items():
-                self.graph[new_node_id][node_i_id] = node_i_distnace_dict[
-                    "distance"
-                ]
-                self.graph[node_i_id][new_node_id] = node_i_distnace_dict[
-                    "distance"
-                ]
-        elif node_addition_type == "closest":
-            min_node_id = min(distances, key=lambda x: distances[x]["distance"])
-            self.graph[new_node_id][min_node_id] = distances[min_node_id][
-                "distance"
-            ]
-            self.graph[min_node_id][new_node_id] = distances[min_node_id][
-                "distance"
-            ]
-        elif node_addition_type == "quadrant":
-            for quadrant in ["ne", "nw", "se", "sw"]:
-                min_node_id = min(
-                    distances,
-                    key=lambda x: distances[x]["distance"]
-                    if distances[x]["quadrant"] == quadrant
-                    else float("inf"),
-                )
-                self.graph[new_node_id][min_node_id] = distances[min_node_id][
-                    "distance"
-                ]
-                self.graph[min_node_id][new_node_id] = distances[min_node_id][
-                    "distance"
-                ]
+        new_node_id = len(self.graph)
+        self.nodes.append(node)
+        self.graph.append(distances)
+        for node_idx, node_distance in distances.items():
+            self.graph[node_idx][new_node_id] = node_distance
         return new_node_id
 
     def save_as_geojson(self, filename: str) -> None:
         """
         Function:
 
         - Save the current geograph object as a geojson file specifed by `filename`
```

### Comparing `scgraph-1.5.2/scgraph/utils.py` & `scgraph-2.0.0/scgraph/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import math, json
 
 
 def haversine(
-    origin: dict,
-    destination: dict,
+    origin: list[float, int],
+    destination: list[float, int],
     units: str = "km",
     circuity: [float, int] = 1,
 ):
     """
     Function:
 
     - Calculate the great circle distance in kilometers between two points on the earth (specified in decimal degrees)
 
     Required Arguments:
 
     - `origin`:
-        - Type: dict
-        - What: is the origin point? (dict with keys "longitude" and "latitude")
+        - Type: list of two floats | ints
+        - What: The origin point as a list of "longitude" and "latitude"
     - `destination`:
-        - Type: dict
-        - What: is the destination point? (dict with keys "longitude" and "latitude")
+        - Type: list of two floats | ints
+        - What: The destination point as a list of "longitude" and "latitude"
 
     Optional Arguments:
 
     - `units`:
         - Type: str
         - What: units to return the distance in? (one of "km", "m", "mi", or "ft")
         - Default: "km"
@@ -34,18 +34,18 @@
 
     """
     try:
         # convert decimal degrees to radians
         lon1, lat1, lon2, lat2 = map(
             math.radians,
             [
-                origin["longitude"],
-                origin["latitude"],
-                destination["longitude"],
-                destination["latitude"],
+                origin[1],
+                origin[0],
+                destination[1],
+                destination[0],
             ],
         )
         # haversine formula
         dlon = lon2 - lon1
         dlat = lat2 - lat1
         a = (
             math.sin(dlat / 2) ** 2
@@ -121,28 +121,35 @@
 
     - Convert a `get_shortest_path` output into a GeoJSON LineString dictionary object
     - Optionally save the output to a file
 
     Required Arguments:
 
     - `output`:
-        - Type: dict
+        - Type: list | dict
         - What: output of `get_shortest_path`
 
     Optional Arguments:
 
     - `filename`:
         - Type: str
         - What: path to save the output to
         - Default: None
         - Note: if `filename` is not None, the output will be saved to the specified path
     """
-    linestring = {
-        "type": "LineString",
-        "coordinates": [
-            [i["longitude"], i["latitude"]] for i in output["coordinate_path"]
-        ],
-    }
+    if isinstance(output["coordinate_path"], list):
+        linestring = {
+            "type": "LineString",
+            "coordinates": [[i[1], i[0]] for i in output["coordinate_path"]],
+        }
+    elif isinstance(output["coordinate_path"], dict):
+        linestring = {
+            "type": "LineString",
+            "coordinates": [
+                [i["longitude"], i["latitude"]]
+                for i in output["coordinate_path"]
+            ],
+        }
     if filename:
         with open(filename, "w") as f:
             f.write(json.dumps(linestring))
     return linestring
```

### Comparing `scgraph-1.5.2/scgraph.egg-info/PKG-INFO` & `scgraph-2.0.0/scgraph.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.5.2
+Version: 2.0.0
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 
 ![scgraph](https://raw.githubusercontent.com/connor-makowski/scgraph/main/static/scgraph.png)
 
 ## Documentation
 
 Getting Started: https://github.com/connor-makowski/scgraph
 
-Low Level: https://connor-makowski.github.io/scgraph/core.html
+Low Level: https://connor-makowski.github.io/scgraph/scgraph/core.html
 
 
 ## Key Features
 
 - Calculate the shortest path between two points on earth using a latitude / longitude pair
     - Inputs:
         - A latitude / longitude pair for the origin
@@ -85,41 +85,25 @@
     origin_node={"latitude": 31.23,"longitude": 121.47}, 
     destination_node={"latitude": 32.08,"longitude": -81.09},
     output_units='km'
 )
 print('Length: ',output['length']) #=> Length:  19596.4653
 ```
 
-In the above example, the `output` variable is a dictionary with three keys: `length`, `coordinate_path` and `path`.
+In the above example, the `output` variable is a dictionary with three keys: `length` and `coordinate_path`.
 
 - `length`: The distance between the passed origin and destination when traversing the graph along the shortest path
     - Notes: 
         - This will be in the units specified by the `output_units` parameter. 
         - `output_units` options:
             - `km` (kilometers - default)
             - `m` (meters)
             - `mi` (miles)
             - `ft` (feet)
-- `coordinate_path`: A list of dictionaries (`latitude` and `longitude`) that make up the shortest path
-- `path`: A list of node ids (from the network data set) that make up the shortest path
-    - In general, these are only relevant if you are providing your own custom network data set
-
-To get the latitude / longitude pairs that make up the shortest path, as a list of lists, you could do something like the following:
-
-```py
-# Use a maritime network geograph
-from scgraph.geographs.marnet import marnet_geograph
-
-# Get the shortest path between 
-output = marnet_geograph.get_shortest_path(
-    origin_node={"latitude": 31.23,"longitude": 121.47}, 
-    destination_node={"latitude": 32.08,"longitude": -81.09}
-)
-print(str([[i['latitude'],i['longitude']] for i in output['coordinate_path']]))
-```
+- `coordinate_path`: A list of lists [`latitude`,`longitude`] that make up the shortest path
 
 ## Included GeoGraphs
 
 - marnet_geograph:
     - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
     - Attribution: [searoute](https://github.com/genthalili/searoute-py)
@@ -183,59 +167,59 @@
 You can specify your own custom graphs for direct access to the solving algorithms. This requires the use of the low level `Graph` class
 
 ```py
 from scgraph import Graph
 
 # Define a graph
 # See the graph definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-graph = {
-    0:{1: 5, 2: 1},
-    1:{0: 5, 2: 2, 3: 1},
-    2:{0: 1, 1: 2, 3: 4, 4: 8},
-    3:{1: 1, 2: 4, 4: 3, 5: 6},
-    4:{2: 8, 3: 3},
-    5:{3: 6}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+graph = [
+    {1: 5, 2: 1},
+    {0: 5, 2: 2, 3: 1},
+    {0: 1, 1: 2, 3: 4, 4: 8},
+    {1: 1, 2: 4, 4: 3, 5: 6},
+    {2: 8, 3: 3},
+    {3: 6}
+]
 
 # Optional: Validate your graph
 Graph.validate_graph(graph=graph)
 
-# Get the shortest path between 0 and 5
+# Get the shortest path between idx 0 and idx 5
 output = Graph.dijkstra_makowski(graph=graph, origin_id=0, destination_id=5)
 #=> {'path': [0, 2, 1, 3, 5], 'length': 10}
 ```
 
 You can also use a slightly higher level `GeoGraph` class to work with latitude / longitude pairs
 
 ```py
 from scgraph import GeoGraph
 
 # Define nodes
 # See the nodes definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-nodes = {
-    0: {"latitude": 0, "longitude": 0},
-    1: {"latitude": 0, "longitude": 1},
-    2: {"latitude": 1, "longitude": 0},
-    3: {"latitude": 1, "longitude": 1},
-    4: {"latitude": 1, "longitude": 2},
-    5: {"latitude": 2, "longitude": 1}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+nodes = [
+    [0,0],
+    [0,1],
+    [1,0],
+    [1,1],
+    [1,2],
+    [2,1]
+]
 # Define a graph
 # See the graph definitions here: 
-# https://connor-makowski.github.io/scgraph/core.html
-graph = {
-    0:{1: 5, 2: 1},
-    1:{0: 5, 2: 2, 3: 1},
-    2:{0: 1, 1: 2, 3: 4, 4: 8},
-    3:{1: 1, 2: 4, 4: 3, 5: 6},
-    4:{2: 8, 3: 3},
-    5:{3: 6}
-}
+# https://connor-makowski.github.io/scgraph/scgraph/core.html
+graph = [
+    {1: 5, 2: 1},
+    {0: 5, 2: 2, 3: 1},
+    {0: 1, 1: 2, 3: 4, 4: 8},
+    {1: 1, 2: 4, 4: 3, 5: 6},
+    {2: 8, 3: 3},
+    {3: 6}
+]
 
 # Create a GeoGraph object
 my_geograph = GeoGraph(nodes=nodes, graph=graph)
 
 # Optional: Validate your graph
 my_geograph.validate_graph()
 
@@ -245,23 +229,22 @@
 # Get the shortest path between two points
 output = my_geograph.get_shortest_path(
     origin_node = {'latitude': 0, 'longitude': 0},
     destination_node = {'latitude': 2, 'longitude': 1}
 )
 #=>
 # {
-#     "path": [6, 0, 2, 1, 3, 5, 7],
 #     "coordinate_path": [
-#         {'latitude': 0, 'longitude': 0},
-#         {'latitude': 0, 'longitude': 0},
-#         {'latitude': 1, 'longitude': 0},
-#         {'latitude': 0, 'longitude': 1},
-#         {'latitude': 1, 'longitude': 1},
-#         {'latitude': 2, 'longitude': 1},
-#         {'latitude': 2, 'longitude': 1}
+#         [0,0],
+#         [0,0],
+#         [1,0],
+#         [0,1],
+#         [1,1],
+#         [2,1],
+#         [2,1]
 #     ],
 #     "length": 10
 # }
 ```
 
 ## Attributions and Thanks
 Originally inspired by [searoute](https://github.com/genthalili/searoute-py) including the use of one of their [datasets](https://github.com/genthalili/searoute-py/blob/main/searoute/data/marnet_densified_v2_old.geojson) that has been modified to work properly with this package.
```

