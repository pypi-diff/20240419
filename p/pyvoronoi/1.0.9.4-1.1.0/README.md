# Comparing `tmp/pyvoronoi-1.0.9.4.tar.gz` & `tmp/pyvoronoi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoronoi-1.0.9.4.tar", last modified: Fri Jan  5 00:32:25 2024, max compression
+gzip compressed data, was "pyvoronoi-1.1.0.tar", last modified: Thu Apr 18 23:39:50 2024, max compression
```

## Comparing `pyvoronoi-1.0.9.4.tar` & `pyvoronoi-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 00:32:25.950749 pyvoronoi-1.0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-01-05 00:32:25.950749 pyvoronoi-1.0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 00:32:25.946749 pyvoronoi-1.0.9.4/pyvoronoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 00:32:25.942749 pyvoronoi-1.0.9.4/pyvoronoi/boost/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 00:32:25.950749 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 00:32:25.950749 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/config.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/cstdint.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/limits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    35615 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/suffix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17237 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_ctypes.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    62729 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_predicates.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_robust_fpt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_structures.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/interval_concept.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/interval_data.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/interval_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18389 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/isotropy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/point_concept.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/point_data.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/point_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    50898 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/rectangle_concept.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/rectangle_data.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/rectangle_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20086 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/segment_concept.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/segment_data.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/segment_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19489 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi_diagram.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi_geometry_type.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   943756 2024-01-05 00:32:14.000000 pyvoronoi-1.0.9.4/pyvoronoi/pyvoronoi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/pyvoronoi.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/voronoi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/pyvoronoi/voronoi.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 00:32:25.946749 pyvoronoi-1.0.9.4/pyvoronoi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-01-05 00:32:25.000000 pyvoronoi-1.0.9.4/pyvoronoi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-01-05 00:32:25.000000 pyvoronoi-1.0.9.4/pyvoronoi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 00:32:25.000000 pyvoronoi-1.0.9.4/pyvoronoi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-05 00:32:25.000000 pyvoronoi-1.0.9.4/pyvoronoi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 00:32:25.950749 pyvoronoi-1.0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-01-05 00:32:07.000000 pyvoronoi-1.0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:39:50.951664 pyvoronoi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-18 23:39:50.947664 pyvoronoi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:39:50.943664 pyvoronoi-1.1.0/pyvoronoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:39:50.943664 pyvoronoi-1.1.0/pyvoronoi/boost/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:39:50.947664 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:39:50.947664 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/config.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/cstdint.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/limits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    35615 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/suffix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17237 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_ctypes.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    62729 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_predicates.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_robust_fpt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_structures.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/interval_concept.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/interval_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/interval_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18389 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/isotropy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/point_concept.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/point_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/point_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    50898 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/rectangle_concept.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/rectangle_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/rectangle_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20086 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/segment_concept.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/segment_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/segment_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19489 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi_diagram.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi_geometry_type.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)  1051479 2024-04-18 23:39:29.000000 pyvoronoi-1.1.0/pyvoronoi/pyvoronoi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18801 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/pyvoronoi.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/voronoi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/pyvoronoi/voronoi.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:39:50.943664 pyvoronoi-1.1.0/pyvoronoi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-18 23:39:50.000000 pyvoronoi-1.1.0/pyvoronoi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-18 23:39:50.000000 pyvoronoi-1.1.0/pyvoronoi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 23:39:50.000000 pyvoronoi-1.1.0/pyvoronoi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 23:39:50.000000 pyvoronoi-1.1.0/pyvoronoi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 23:39:50.951664 pyvoronoi-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-18 23:39:22.000000 pyvoronoi-1.1.0/setup.py
```

### Comparing `pyvoronoi-1.0.9.4/MANIFEST.in` & `pyvoronoi-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/PKG-INFO` & `pyvoronoi-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pyvoronoi
-Version: 1.0.9.4
+Version: 1.1.0
 Summary: Cython wrapper for the Boost Voronoi library (version 1.59.0)
 Home-page: https://github.com/fabanc/pyvoronoi
 Author: Fabien Ancelin / Andrii Sydorchuk, Voxel8
 Author-email: 
+License: UNKNOWN
 Keywords: voronoi,Boost,polygon
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: Environment :: Other Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,15 +27,17 @@
 
 # pyvoronoi
 
 A wrapper for Boost's Voronoi diagram library. The full documentation of the Boost Voronoi API is available [here](https://www.boost.org/doc/libs/1_75_0/libs/polygon/doc/voronoi_main.htm).
 
 ## Install
 
-The install have been tested on Windows and Linux Ubuntu. If you notice any issue on Mac, reach out to me, I am interested in making sure it works for you.
+The installation have been tested on Windows and Linux Ubuntu. If you notice any issue on Mac, reach out to us, we are interested in making sure it works for you.
+
+Windows users will need Microsoft Visual C++ installed on their machine. You can find information about the version needed on [this](https://wiki.python.org/moin/WindowsCompilers) link. Python version from 3.5 to 3.12 rely on Visual C++ 14.x.
 
 ### Dependencies
 
 Cython dependency is optional. Cpp sources generated with Cython are available in releases.
 
 Note on using the setup.py:
 
@@ -59,14 +63,19 @@
 
 Cython required.
 
 Clone the repository:
 
 ``git clone https://github.com/fabanc/pyvoronoi.git``
 
+
+Install the development dependencies:
+
+`pip install -requirements_dev.txt`
+
 Install:
 
 ``python setup.py install``
 
 After every modification of .pyx files compile with Cython:
 
 ``python setup.py build_ext --inplace``
@@ -179,14 +188,54 @@
 for c in cells:
     print("Cell contains point: {0}. Contains segment: {1}. Is open: {2}, Site Index: {3}".format(c.contains_point, c.contains_segment, c.is_open, c.site))
     print(",".join(map(str,c.vertices)))
     for sIndex in c.edges:
         print("Start Index: {0}, End Index = {1}".format(edges[sIndex].start, edges[sIndex].end))
 ```
 
+Note that since version 1.0.4 each of the Get function has an equivalent function that returns an iterator. This is more memory friendly.
+
+|Goal|Return a list|Return an iterator|
+| - | - | - |
+| Return vertices | GetVertices | IterateVertices |
+| Return edges | GetEdges | IterateEdges |
+| Return cells | GetCells | IterateCells |
+
+They are functionaly equivalent as defined in this automated test:
+
+```python
+    def test_iterators(self):
+        pv = pyvoronoi.Pyvoronoi(1)
+        pv.AddPoint([5,5])
+        pv.AddSegment([[0,0],[0,10]])
+        pv.AddSegment([[0,0],[10,0]])
+        pv.AddSegment([[0,10],[10,10]])
+        pv.AddSegment([[10,0],[10,10]])
+        pv.Construct()
+
+        vertices = pv.GetVertices()
+        vertex_generator = pv.IterateVertices()
+        for v in vertices:
+            v_generator = next(vertex_generator)
+            self.assertEqual(v, v_generator)
+
+        edges = pv.GetEdges()
+        edge_generator = pv.IterateEdges()
+        for e in edges:
+            e_generator = next(edge_generator)
+            self.assertEqual(e, e_generator)
+
+        cells = pv.GetCells()
+        cell_generator = pv.IterateCells()
+        for c in cells:
+            c_generator = next(cell_generator)
+            self.assertEqual(c, c_generator)
+```
+
+
 Some output edges returned by the boost voronoi API are suposed to be curved. In the C++ API, it is up to you to code it. Luckily, you can do it in python using the following the function DiscretizeCurvedEdge.
 The sample below shows you how to do that:
 
 ```python
 for cIndex in range(len(cells)):
     cell = cells[cIndex]
     if cell.is_open == False:
@@ -214,7 +263,9 @@
 # License
 
 -  Pyvoronoi is available under `MIT
    license <http://opensource.org/licenses/MIT>`__.
 -  The core Voronoi library is available under `Boost Software
    License <http://www.boost.org/LICENSE_1_0.txt>`__. Freeware for both
    open source and commercial applications.
+
+
```

### Comparing `pyvoronoi-1.0.9.4/README.md` & `pyvoronoi-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 # pyvoronoi
 
 A wrapper for Boost's Voronoi diagram library. The full documentation of the Boost Voronoi API is available [here](https://www.boost.org/doc/libs/1_75_0/libs/polygon/doc/voronoi_main.htm).
 
 ## Install
 
-The install have been tested on Windows and Linux Ubuntu. If you notice any issue on Mac, reach out to me, I am interested in making sure it works for you.
+The installation have been tested on Windows and Linux Ubuntu. If you notice any issue on Mac, reach out to us, we are interested in making sure it works for you.
+
+Windows users will need Microsoft Visual C++ installed on their machine. You can find information about the version needed on [this](https://wiki.python.org/moin/WindowsCompilers) link. Python version from 3.5 to 3.12 rely on Visual C++ 14.x.
 
 ### Dependencies
 
 Cython dependency is optional. Cpp sources generated with Cython are available in releases.
 
 Note on using the setup.py:
 
@@ -35,14 +37,19 @@
 
 Cython required.
 
 Clone the repository:
 
 ``git clone https://github.com/fabanc/pyvoronoi.git``
 
+
+Install the development dependencies:
+
+`pip install -requirements_dev.txt`
+
 Install:
 
 ``python setup.py install``
 
 After every modification of .pyx files compile with Cython:
 
 ``python setup.py build_ext --inplace``
@@ -155,14 +162,54 @@
 for c in cells:
     print("Cell contains point: {0}. Contains segment: {1}. Is open: {2}, Site Index: {3}".format(c.contains_point, c.contains_segment, c.is_open, c.site))
     print(",".join(map(str,c.vertices)))
     for sIndex in c.edges:
         print("Start Index: {0}, End Index = {1}".format(edges[sIndex].start, edges[sIndex].end))
 ```
 
+Note that since version 1.0.4 each of the Get function has an equivalent function that returns an iterator. This is more memory friendly.
+
+|Goal|Return a list|Return an iterator|
+| - | - | - |
+| Return vertices | GetVertices | IterateVertices |
+| Return edges | GetEdges | IterateEdges |
+| Return cells | GetCells | IterateCells |
+
+They are functionaly equivalent as defined in this automated test:
+
+```python
+    def test_iterators(self):
+        pv = pyvoronoi.Pyvoronoi(1)
+        pv.AddPoint([5,5])
+        pv.AddSegment([[0,0],[0,10]])
+        pv.AddSegment([[0,0],[10,0]])
+        pv.AddSegment([[0,10],[10,10]])
+        pv.AddSegment([[10,0],[10,10]])
+        pv.Construct()
+
+        vertices = pv.GetVertices()
+        vertex_generator = pv.IterateVertices()
+        for v in vertices:
+            v_generator = next(vertex_generator)
+            self.assertEqual(v, v_generator)
+
+        edges = pv.GetEdges()
+        edge_generator = pv.IterateEdges()
+        for e in edges:
+            e_generator = next(edge_generator)
+            self.assertEqual(e, e_generator)
+
+        cells = pv.GetCells()
+        cell_generator = pv.IterateCells()
+        for c in cells:
+            c_generator = next(cell_generator)
+            self.assertEqual(c, c_generator)
+```
+
+
 Some output edges returned by the boost voronoi API are suposed to be curved. In the C++ API, it is up to you to code it. Luckily, you can do it in python using the following the function DiscretizeCurvedEdge.
 The sample below shows you how to do that:
 
 ```python
 for cIndex in range(len(cells)):
     cell = cells[cIndex]
     if cell.is_open == False:
```

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/config.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/config.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/cstdint.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/cstdint.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/limits.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/limits.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/suffix.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/suffix.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_ctypes.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_ctypes.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_predicates.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_predicates.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_robust_fpt.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_robust_fpt.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/detail/voronoi_structures.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/detail/voronoi_structures.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/interval_concept.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/interval_concept.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/interval_data.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/interval_data.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/interval_traits.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/interval_traits.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/isotropy.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/isotropy.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/point_concept.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/point_concept.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/point_data.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/point_data.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/point_traits.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/point_traits.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/rectangle_concept.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/rectangle_concept.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/rectangle_data.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/rectangle_data.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/rectangle_traits.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/rectangle_traits.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/segment_concept.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/segment_concept.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/segment_data.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/segment_data.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/segment_traits.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/segment_traits.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi_builder.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi_builder.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi_diagram.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi_diagram.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/boost/polygon/voronoi_geometry_type.hpp` & `pyvoronoi-1.1.0/pyvoronoi/boost/polygon/voronoi_geometry_type.hpp`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/pyvoronoi.cpp` & `pyvoronoi-1.1.0/pyvoronoi/pyvoronoi.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.7 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "pyvoronoi/voronoi.hpp"
         ],
@@ -40,18 +40,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_7" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030007F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -135,14 +135,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -196,14 +198,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -257,60 +261,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -393,14 +420,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -601,22 +631,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -666,15 +696,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -752,16 +782,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1105,15 +1140,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1192,15 +1227,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1295,32 +1330,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1362,15 +1380,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1496,17 +1514,20 @@
 
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9pyvoronoi_Pyvoronoi;
-struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize;
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices;
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges;
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells;
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize;
 
-/* "pyvoronoi.pyx":210
+/* "pyvoronoi.pyx":196
  * ####################################
  * 
  * cdef class Pyvoronoi:             # <<<<<<<<<<<<<<
  *     cdef VoronoiDiagram *thisptr
  *     cdef int constructed
  */
 struct __pyx_obj_9pyvoronoi_Pyvoronoi {
@@ -1514,31 +1535,85 @@
   struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *__pyx_vtab;
   VoronoiDiagram *thisptr;
   int constructed;
   int SCALING_FACTOR;
 };
 
 
-/* "pyvoronoi.pyx":433
+/* "pyvoronoi.pyx":310
+ *         return output
+ * 
+ *     def IterateVertices(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountVertices()
+ *         for index in  range(count):
+ */
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices {
+  PyObject_HEAD
+  PyObject *__pyx_v_count;
+  PyObject *__pyx_v_index;
+  struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self;
+  PyObject *__pyx_t_0;
+  Py_ssize_t __pyx_t_1;
+  PyObject *(*__pyx_t_2)(PyObject *);
+};
+
+
+/* "pyvoronoi.pyx":322
+ *         return output
+ * 
+ *     def IterateEdges(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountEdges()
+ *         for index in range(count):
+ */
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges {
+  PyObject_HEAD
+  PyObject *__pyx_v_count;
+  PyObject *__pyx_v_index;
+  struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self;
+  PyObject *__pyx_t_0;
+  Py_ssize_t __pyx_t_1;
+  PyObject *(*__pyx_t_2)(PyObject *);
+};
+
+
+/* "pyvoronoi.pyx":334
+ *         return output
+ * 
+ *     def IterateCells(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountCells()
+ *         for index in range(count):
+ */
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells {
+  PyObject_HEAD
+  PyObject *__pyx_v_count;
+  PyObject *__pyx_v_index;
+  struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self;
+  PyObject *__pyx_t_0;
+  Py_ssize_t __pyx_t_1;
+  PyObject *(*__pyx_t_2)(PyObject *);
+};
+
+
+/* "pyvoronoi.pyx":436
  *         return [boost_x, computed_point_y]
  * 
  *     def Discretize(self, point, segment, parabola_start, parabola_end, max_dist, parabola_equation_tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.
  */
-struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize {
+struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize {
   PyObject_HEAD
   PyObject *__pyx_v_angle;
   PyObject *__pyx_v_shift_x;
   PyObject *__pyx_v_shift_y;
 };
 
 
 
-/* "pyvoronoi.pyx":210
+/* "pyvoronoi.pyx":196
  * ####################################
  * 
  * cdef class Pyvoronoi:             # <<<<<<<<<<<<<<
  *     cdef VoronoiDiagram *thisptr
  *     cdef int constructed
  */
 
@@ -1719,16 +1794,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -1736,16 +1811,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -1869,56 +1945,22 @@
 /* PyObjectFastCall.proto */
 #define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* PyObjectSetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
-#else
-#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
-#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
-#endif
-
-/* ListAppend.proto */
-#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
-static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
-    PyListObject* L = (PyListObject*) list;
-    Py_ssize_t len = Py_SIZE(list);
-    if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
-        Py_INCREF(x);
-        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-        L->ob_item[len] = x;
-        #else
-        PyList_SET_ITEM(list, len, x);
-        #endif
-        __Pyx_SET_SIZE(list, len + 1);
-        return 0;
-    }
-    return PyList_Append(list, x);
-}
+/* PyIntBinop.proto */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_MultiplyCObj(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
-#define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
+#define __Pyx_PyInt_MultiplyCObj(op1, op2, intval, inplace, zerodivision_check)\
+    (inplace ? PyNumber_InPlaceMultiply(op1, op2) : PyNumber_Multiply(op1, op2))
 #endif
 
-/* PyObjectCall2Args.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
-/* PyObjectCallMethod1.proto */
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
-
-/* append.proto */
-static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x);
-
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1933,68 +1975,101 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_MultiplyCObj(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_MultiplyCObj(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceMultiply(op1, op2) : PyNumber_Multiply(op1, op2))
-#endif
-
 /* pow2.proto */
 #define __Pyx_PyNumber_Power2(a, b) PyNumber_Power(a, b, Py_None)
 
-/* SliceObject.proto */
-#define __Pyx_PyObject_DelSlice(obj, cstart, cstop, py_start, py_stop, py_slice, has_cstart, has_cstop, wraparound)\
-    __Pyx_PyObject_SetSlice(obj, (PyObject*)NULL, cstart, cstop, py_start, py_stop, py_slice, has_cstart, has_cstop, wraparound)
-static CYTHON_INLINE int __Pyx_PyObject_SetSlice(
-        PyObject* obj, PyObject* value, Py_ssize_t cstart, Py_ssize_t cstop,
-        PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
-        int has_cstart, int has_cstop, int wraparound);
-
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
-/* PyIntCompare.proto */
-static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+/* ListCompAppend.proto */
+#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
+static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
+    PyListObject* L = (PyListObject*) list;
+    Py_ssize_t len = Py_SIZE(list);
+    if (likely(L->allocated > len)) {
+        Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
+        PyList_SET_ITEM(list, len, x);
+        #endif
+        __Pyx_SET_SIZE(list, len + 1);
+        return 0;
+    }
+    return PyList_Append(list, x);
+}
+#else
+#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
+#endif
 
-/* ObjectGetItem.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
+/* ListAppend.proto */
+#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
+static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
+    PyListObject* L = (PyListObject*) list;
+    Py_ssize_t len = Py_SIZE(list);
+    if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
+        Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
+        PyList_SET_ITEM(list, len, x);
+        #endif
+        __Pyx_SET_SIZE(list, len + 1);
+        return 0;
+    }
+    return PyList_Append(list, x);
+}
+#else
+#define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
-#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* pep479.proto */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen);
+
+/* PyIntCompare.proto */
+static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
 /* RaiseClosureNameError.proto */
 static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname);
 
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_TrueDivideObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_TrueDivideObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceTrueDivide(op1, op2) : PyNumber_TrueDivide(op1, op2))
 #endif
 
 /* PyObjectCallNoArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
 /* PyObjectCallMethod0.proto */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
 /* pop.proto */
 static CYTHON_INLINE PyObject* __Pyx__PyObject_Pop(PyObject* L);
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE PyObject* __Pyx_PyList_Pop(PyObject* L);
@@ -2138,15 +2213,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -2235,27 +2310,36 @@
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
 #if PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+
+/* Py3UpdateBases.proto */
+static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
+
+/* CalculateMetaclass.proto */
+static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
+
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? _PyDict_SetItem_KnownHash(ns, name, value, ((PyASCIIObject *) name)->hash) : PyObject_SetItem(ns, name, value))
 #elif CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? PyDict_SetItem(ns, name, value) : PyObject_SetItem(ns, name, value))
 #else
 #define __Pyx_SetNameInClass(ns, name, value)  PyObject_SetItem(ns, name, value)
 #endif
 
-/* CalculateMetaclass.proto */
-static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
+/* PyObjectCall2Args.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyObjectLookupSpecial.proto */
 #if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
 #define __Pyx_PyObject_LookupSpecialNoError(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 0)
 #define __Pyx_PyObject_LookupSpecial(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 1)
 static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error);
 #else
@@ -2265,17 +2349,14 @@
 
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
                                       PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
 
-/* Py3UpdateBases.proto */
-static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
-
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -2308,23 +2389,26 @@
 static PyObject* __pyx_convert__to_py_struct__Point(struct Point s);
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *);
+
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
 #else
@@ -2350,14 +2434,117 @@
 #define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* SwapException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCallMethod1.proto */
+static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
+
+/* CoroutineBase.proto */
+struct __pyx_CoroutineObject;
+typedef PyObject *(*__pyx_coroutine_body_t)(struct __pyx_CoroutineObject *, PyThreadState *, PyObject *);
+#if CYTHON_USE_EXC_INFO_STACK
+#define __Pyx_ExcInfoStruct  _PyErr_StackItem
+#else
+typedef struct {
+    PyObject *exc_type;
+    PyObject *exc_value;
+    PyObject *exc_traceback;
+} __Pyx_ExcInfoStruct;
+#endif
+typedef struct __pyx_CoroutineObject {
+    PyObject_HEAD
+    __pyx_coroutine_body_t body;
+    PyObject *closure;
+    __Pyx_ExcInfoStruct gi_exc_state;
+    PyObject *gi_weakreflist;
+    PyObject *classobj;
+    PyObject *yieldfrom;
+    PyObject *gi_name;
+    PyObject *gi_qualname;
+    PyObject *gi_modulename;
+    PyObject *gi_code;
+    PyObject *gi_frame;
+    int resume_label;
+    char is_running;
+} __pyx_CoroutineObject;
+static __pyx_CoroutineObject *__Pyx__Coroutine_New(
+    PyTypeObject *type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
+    PyObject *name, PyObject *qualname, PyObject *module_name);
+static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
+            __pyx_CoroutineObject *gen, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
+            PyObject *name, PyObject *qualname, PyObject *module_name);
+static CYTHON_INLINE void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *self);
+static int __Pyx_Coroutine_clear(PyObject *self);
+static PyObject *__Pyx_Coroutine_Send(PyObject *self, PyObject *value);
+static PyObject *__Pyx_Coroutine_Close(PyObject *self);
+static PyObject *__Pyx_Coroutine_Throw(PyObject *gen, PyObject *args);
+#if CYTHON_USE_EXC_INFO_STACK
+#define __Pyx_Coroutine_SwapException(self)
+#define __Pyx_Coroutine_ResetAndClearException(self)  __Pyx_Coroutine_ExceptionClear(&(self)->gi_exc_state)
+#else
+#define __Pyx_Coroutine_SwapException(self) {\
+    __Pyx_ExceptionSwap(&(self)->gi_exc_state.exc_type, &(self)->gi_exc_state.exc_value, &(self)->gi_exc_state.exc_traceback);\
+    __Pyx_Coroutine_ResetFrameBackpointer(&(self)->gi_exc_state);\
+    }
+#define __Pyx_Coroutine_ResetAndClearException(self) {\
+    __Pyx_ExceptionReset((self)->gi_exc_state.exc_type, (self)->gi_exc_state.exc_value, (self)->gi_exc_state.exc_traceback);\
+    (self)->gi_exc_state.exc_type = (self)->gi_exc_state.exc_value = (self)->gi_exc_state.exc_traceback = NULL;\
+    }
+#endif
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyGen_FetchStopIterationValue(pvalue)\
+    __Pyx_PyGen__FetchStopIterationValue(__pyx_tstate, pvalue)
+#else
+#define __Pyx_PyGen_FetchStopIterationValue(pvalue)\
+    __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, pvalue)
+#endif
+static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *tstate, PyObject **pvalue);
+static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state);
+
+/* PatchModuleWithCoroutine.proto */
+static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
+
+/* PatchGeneratorABC.proto */
+static int __Pyx_patch_abc(void);
+
+/* Generator.proto */
+#define __Pyx_Generator_USED
+#define __Pyx_Generator_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_GeneratorType)
+#define __Pyx_Generator_New(body, code, closure, name, qualname, module_name)\
+    __Pyx__Coroutine_New(__pyx_GeneratorType, body, code, closure, name, qualname, module_name)
+static PyObject *__Pyx_Generator_Next(PyObject *self);
+static int __pyx_Generator_init(PyObject *module);
+
 /* CheckBinaryVersion.proto */
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
@@ -2383,77 +2570,85 @@
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_map;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_MemoryError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_X[] = "X";
 static const char __pyx_k_Y[] = "Y";
+static const char __pyx_k_p[] = "p";
+static const char __pyx_k_s[] = "s";
 static const char __pyx_k_t[] = "t";
 static const char __pyx_k_x[] = "x";
-static const char __pyx_k_y[] = "y";
-static const char __pyx_k__2[] = "*";
+static const char __pyx_k__4[] = "*";
+static const char __pyx_k__5[] = ".";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_p0[] = "p0";
 static const char __pyx_k_p1[] = "p1";
 static const char __pyx_k__65[] = "?";
 static const char __pyx_k_cos[] = "cos";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_end[] = "end";
+static const char __pyx_k_int[] = "int";
 static const char __pyx_k_map[] = "map";
 static const char __pyx_k_pop[] = "pop";
 static const char __pyx_k_sin[] = "sin";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_Cell[] = "Cell";
 static const char __pyx_k_Edge[] = "Edge";
+static const char __pyx_k_args[] = "args";
+static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_cell[] = "cell";
 static const char __pyx_k_copy[] = "copy";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_edge[] = "edge";
-static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_math[] = "math";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_next[] = "next";
 static const char __pyx_k_self[] = "self";
+static const char __pyx_k_send[] = "send";
 static const char __pyx_k_site[] = "site";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_sqrt[] = "sqrt";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_twin[] = "twin";
 static const char __pyx_k_angle[] = "angle";
 static const char __pyx_k_atan2[] = "atan2";
+static const char __pyx_k_close[] = "close";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_delta[] = "delta";
 static const char __pyx_k_edges[] = "edges";
+static const char __pyx_k_float[] = "float";
 static const char __pyx_k_focus[] = "focus";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_point[] = "point";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_sites[] = "sites";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_sys_2[] = "_sys";
 static const char __pyx_k_theta[] = "theta";
+static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_Rotate[] = "Rotate";
 static const char __pyx_k_SILENT[] = "SILENT";
 static const char __pyx_k_Vertex[] = "Vertex";
-static const char __pyx_k_append[] = "append";
 static const char __pyx_k_c_cell[] = "c_cell";
 static const char __pyx_k_c_edge[] = "c_edge";
 static const char __pyx_k_copy_2[] = "_copy";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_output[] = "output";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_time_2[] = "_time";
+static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_GetCell[] = "GetCell";
 static const char __pyx_k_GetEdge[] = "GetEdge";
 static const char __pyx_k_boost_x[] = "boost_x";
 static const char __pyx_k_boost_y[] = "boost_y";
 static const char __pyx_k_c_point[] = "c_point";
 static const char __pyx_k_current[] = "current";
 static const char __pyx_k_disable[] = "disable";
@@ -2496,78 +2691,76 @@
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_tolerance[] = "tolerance";
 static const char __pyx_k_AddSegment[] = "AddSegment";
 static const char __pyx_k_CountCells[] = "CountCells";
 static const char __pyx_k_CountEdges[] = "CountEdges";
 static const char __pyx_k_Discretize[] = "Discretize";
+static const char __pyx_k_NamedTuple[] = "NamedTuple";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_is_primary[] = "is_primary";
 static const char __pyx_k_log_action[] = "log_action";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
-static const char __pyx_k_Cell___init[] = "Cell.__init__";
-static const char __pyx_k_Edge___init[] = "Edge.__init__";
 static const char __pyx_k_GetSegments[] = "GetSegments";
 static const char __pyx_k_GetVertices[] = "GetVertices";
 static const char __pyx_k_MemoryError[] = "MemoryError";
+static const char __pyx_k_annotations[] = "__annotations__";
 static const char __pyx_k_description[] = "description";
 static const char __pyx_k_directrix_y[] = "directrix_y";
 static const char __pyx_k_end_point_x[] = "end_point_x";
 static const char __pyx_k_end_point_y[] = "end_point_y";
-static const char __pyx_k_inputPoints[] = "inputPoints";
 static const char __pyx_k_mid_point_x[] = "mid_point_x";
 static const char __pyx_k_mro_entries[] = "__mro_entries__";
-static const char __pyx_k_outputCells[] = "outputCells";
-static const char __pyx_k_outputEdges[] = "outputEdges";
 static const char __pyx_k_point_start[] = "point_start";
 static const char __pyx_k_segmentSite[] = "segmentSite";
 static const char __pyx_k_unicodedata[] = "unicodedata";
 static const char __pyx_k_GetParabolaY[] = "GetParabolaY";
+static const char __pyx_k_IterateCells[] = "IterateCells";
+static const char __pyx_k_IterateEdges[] = "IterateEdges";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_parabola_end[] = "parabola_end";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_CountVertices[] = "CountVertices";
 static const char __pyx_k_RetrievePoint[] = "RetrievePoint";
-static const char __pyx_k_Vertex___init[] = "Vertex.__init__";
-static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_edgeEndVertex[] = "edgeEndVertex";
 static const char __pyx_k_focus_rotated[] = "focus_rotated";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
-static const char __pyx_k_inputSegments[] = "inputSegments";
 static const char __pyx_k_input_segment[] = "input_segment";
 static const char __pyx_k_is_degenerate[] = "is_degenerate";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_start_point_x[] = "start_point_x";
 static const char __pyx_k_start_point_y[] = "start_point_y";
 static const char __pyx_k_unicodedata_2[] = "_unicodedata";
 static const char __pyx_k_contains_point[] = "contains_point";
-static const char __pyx_k_outputVertices[] = "outputVertices";
 static const char __pyx_k_parabola_start[] = "parabola_start";
 static const char __pyx_k_scaling_factor[] = "scaling_factor";
 static const char __pyx_k_DistanceSquared[] = "DistanceSquared";
+static const char __pyx_k_IterateVertices[] = "IterateVertices";
 static const char __pyx_k_RetrieveSegment[] = "RetrieveSegment";
 static const char __pyx_k_RotateWithShift[] = "RotateWithShift";
 static const char __pyx_k_cell_identifier[] = "cell_identifier";
 static const char __pyx_k_edgeStartVertex[] = "edgeStartVertex";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_source_category[] = "source_category";
 static const char __pyx_k_VoronoiException[] = "VoronoiException";
 static const char __pyx_k_computed_point_y[] = "computed_point_y";
 static const char __pyx_k_contains_segment[] = "contains_segment";
 static const char __pyx_k_non_scaled_point[] = "non_scaled_point";
+static const char __pyx_k_typing_Type_Edge[] = "[typing.Type[Edge]]";
 static const char __pyx_k_Pyvoronoi_GetCell[] = "Pyvoronoi.GetCell";
 static const char __pyx_k_Pyvoronoi_GetEdge[] = "Pyvoronoi.GetEdge";
 static const char __pyx_k_densified_rotated[] = "densified_rotated";
 static const char __pyx_k_Pyvoronoi_AddPoint[] = "Pyvoronoi.AddPoint";
 static const char __pyx_k_Pyvoronoi_GetCells[] = "Pyvoronoi.GetCells";
 static const char __pyx_k_Pyvoronoi_GetEdges[] = "Pyvoronoi.GetEdges";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_non_scaled_segment[] = "non_scaled_segment";
+static const char __pyx_k_typing_Type_Vertex[] = "[typing.Type[Vertex]]";
 static const char __pyx_k_Pyvoronoi_Construct[] = "Pyvoronoi.Construct";
 static const char __pyx_k_Pyvoronoi_GetPoints[] = "Pyvoronoi.GetPoints";
 static const char __pyx_k_Pyvoronoi_GetVertex[] = "Pyvoronoi.GetVertex";
 static const char __pyx_k_RetrieveScaledPoint[] = "RetrieveScaledPoint";
 static const char __pyx_k_DiscretizeCurvedEdge[] = "DiscretizeCurvedEdge";
 static const char __pyx_k_Pyvoronoi_AddSegment[] = "Pyvoronoi.AddSegment";
 static const char __pyx_k_Pyvoronoi_CountCells[] = "Pyvoronoi.CountCells";
@@ -2576,21 +2769,24 @@
 static const char __pyx_k_RetriveScaledSegment[] = "RetriveScaledSegment";
 static const char __pyx_k_directix_end_rotated[] = "directix_end_rotated";
 static const char __pyx_k_parabola_end_rotated[] = "parabola_end_rotated";
 static const char __pyx_k_GetLineAngleInRadians[] = "GetLineAngleInRadians";
 static const char __pyx_k_Pyvoronoi_GetSegments[] = "Pyvoronoi.GetSegments";
 static const char __pyx_k_Pyvoronoi_GetVertices[] = "Pyvoronoi.GetVertices";
 static const char __pyx_k_Pyvoronoi_GetParabolaY[] = "Pyvoronoi.GetParabolaY";
+static const char __pyx_k_Pyvoronoi_IterateCells[] = "Pyvoronoi.IterateCells";
+static const char __pyx_k_Pyvoronoi_IterateEdges[] = "Pyvoronoi.IterateEdges";
 static const char __pyx_k_directix_start_rotated[] = "directix_start_rotated";
 static const char __pyx_k_parabola_start_rotated[] = "parabola_start_rotated";
 static const char __pyx_k_Pyvoronoi_CountVertices[] = "Pyvoronoi.CountVertices";
 static const char __pyx_k_Pyvoronoi_RetrievePoint[] = "Pyvoronoi.RetrievePoint";
 static const char __pyx_k_pyvoronoi_pyvoronoi_pyx[] = "pyvoronoi/pyvoronoi.pyx";
 static const char __pyx_k_Discretize_locals_lambda[] = "Discretize.<locals>.<lambda>";
 static const char __pyx_k_FocusOnDirectixException[] = "FocusOnDirectixException";
+static const char __pyx_k_Pyvoronoi_IterateVertices[] = "Pyvoronoi.IterateVertices";
 static const char __pyx_k_Pyvoronoi_RetrieveSegment[] = "Pyvoronoi.RetrieveSegment";
 static const char __pyx_k_Pyvoronoi___reduce_cython[] = "Pyvoronoi.__reduce_cython__";
 static const char __pyx_k_UnsolvableParabolaEquation[] = "UnsolvableParabolaEquation";
 static const char __pyx_k_parabola_end_rotated_check[] = "parabola_end_rotated_check";
 static const char __pyx_k_Pyvoronoi___setstate_cython[] = "Pyvoronoi.__setstate_cython__";
 static const char __pyx_k_ReturnCurvedSiteInformation[] = "ReturnCurvedSiteInformation";
 static const char __pyx_k_parabola_equation_tolerance[] = "parabola_equation_tolerance";
@@ -2608,17 +2804,14 @@
 static const char __pyx_k_Parabola_equation_tolerance_must[] = "Parabola equation tolerance must be greater than 0 or equal to 0. Value passed: {0}";
 static const char __pyx_k_Pyvoronoi_CheckUnsolvableParabol[] = "Pyvoronoi.CheckUnsolvableParabolaEquation";
 static const char __pyx_k_Pyvoronoi_ReturnCurvedSiteInform[] = "Pyvoronoi.ReturnCurvedSiteInformation";
 static const char __pyx_k_The_computed_Y_on_the_parabola_f[] = "The computed Y on the parabola for the starting / ending point is different from the rotated point returned by Boost. Difference: {0}. Maximum tolerance: {1}";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_9pyvoronoi_log_action(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_description); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_6Vertex___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_y); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_4Edge___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_start, PyObject *__pyx_v_end, PyObject *__pyx_v_cell, PyObject *__pyx_v_twin); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_4Cell___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_cell_identifier, PyObject *__pyx_v_site, PyObject *__pyx_v_vertices, PyObject *__pyx_v_edges, PyObject *__pyx_v_source_category); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_2Rotate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_point, PyObject *__pyx_v_theta); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_4RotateWithShift(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_point, PyObject *__pyx_v_theta, PyObject *__pyx_v_shift_x, PyObject *__pyx_v_shift_y); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_6Unrotate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_point, PyObject *__pyx_v_theta, PyObject *__pyx_v_shift_x, PyObject *__pyx_v_shift_y); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_8GetLineAngleInRadians(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_start_point_x, PyObject *__pyx_v_start_point_y, PyObject *__pyx_v_end_point_x, PyObject *__pyx_v_end_point_y); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_10DistanceSquared(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_point_start, PyObject *__pyx_v_point_end); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_12Distance(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_point_start, PyObject *__pyx_v_point_end); /* proto */
 static int __pyx_pf_9pyvoronoi_9Pyvoronoi___cinit__(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_scaling_factor); /* proto */
@@ -2631,32 +2824,38 @@
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_14GetCell(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_16CountVertices(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_18CountEdges(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_20CountCells(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_22GetPoints(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_24GetSegments(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_26GetVertices(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_28GetEdges(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_30GetCells(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_32ReturnCurvedSiteInformation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_edge); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_34DiscretizeCurvedEdge(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_36RetrievePoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_38RetrieveSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_40RetrieveScaledPoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_42RetriveScaledSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_44GetParabolaY(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_focus, PyObject *__pyx_v_directrix_y); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_46CheckUnsolvableParabolaEquation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_boost_x, PyObject *__pyx_v_boost_y, PyObject *__pyx_v_focus, PyObject *__pyx_v_directix, PyObject *__pyx_v_tolerance); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_28IterateVertices(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_31GetEdges(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_33IterateEdges(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_36GetCells(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_38IterateCells(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_41ReturnCurvedSiteInformation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_edge); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_43DiscretizeCurvedEdge(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_45RetrievePoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_47RetrieveSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_49RetrieveScaledPoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_51RetriveScaledSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_53GetParabolaY(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_focus, PyObject *__pyx_v_directrix_y); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_55CheckUnsolvableParabolaEquation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_boost_x, PyObject *__pyx_v_boost_y, PyObject *__pyx_v_focus, PyObject *__pyx_v_directix, PyObject *__pyx_v_tolerance); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_48Discretize(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_point, PyObject *__pyx_v_segment, PyObject *__pyx_v_parabola_start, PyObject *__pyx_v_parabola_end, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_57Discretize(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_point, PyObject *__pyx_v_segment, PyObject *__pyx_v_parabola_start, PyObject *__pyx_v_parabola_end, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance); /* proto */
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_14SCALING_FACTOR___get__(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
 static int __pyx_pf_9pyvoronoi_9Pyvoronoi_14SCALING_FACTOR_2__set__(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_50__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_52__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_59__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_61__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_9pyvoronoi_Pyvoronoi(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct__Discretize(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct__IterateVertices(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct_1_IterateEdges(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct_2_IterateCells(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct_3_Discretize(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyList_Type_pop = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -2679,22 +2878,27 @@
   PyTypeObject *__pyx_CoroutineAwaitType;
   #endif
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_9pyvoronoi_Pyvoronoi;
-  PyObject *__pyx_type_9pyvoronoi___pyx_scope_struct__Discretize;
+  PyObject *__pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices;
+  PyObject *__pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges;
+  PyObject *__pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells;
+  PyObject *__pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize;
   #endif
   PyTypeObject *__pyx_ptype_9pyvoronoi_Pyvoronoi;
-  PyTypeObject *__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize;
+  PyTypeObject *__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices;
+  PyTypeObject *__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges;
+  PyTypeObject *__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells;
+  PyTypeObject *__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize;
   PyObject *__pyx_n_s_AddPoint;
   PyObject *__pyx_n_s_AddSegment;
   PyObject *__pyx_n_s_Cell;
-  PyObject *__pyx_n_s_Cell___init;
   PyObject *__pyx_n_s_CheckUnsolvableParabolaEquation;
   PyObject *__pyx_n_s_Construct;
   PyObject *__pyx_kp_s_Construct_has_already_been_calle;
   PyObject *__pyx_kp_s_Construct_has_been_called_can_t;
   PyObject *__pyx_n_s_CountCells;
   PyObject *__pyx_n_s_CountEdges;
   PyObject *__pyx_n_s_CountVertices;
@@ -2702,28 +2906,31 @@
   PyObject *__pyx_kp_s_Deleting_the_VoronoiDiagram_inst;
   PyObject *__pyx_n_s_Discretize;
   PyObject *__pyx_n_s_DiscretizeCurvedEdge;
   PyObject *__pyx_n_s_Discretize_locals_lambda;
   PyObject *__pyx_n_s_Distance;
   PyObject *__pyx_n_s_DistanceSquared;
   PyObject *__pyx_n_s_Edge;
-  PyObject *__pyx_n_s_Edge___init;
   PyObject *__pyx_n_s_FocusOnDirectixException;
   PyObject *__pyx_n_s_GetCell;
   PyObject *__pyx_n_s_GetCells;
   PyObject *__pyx_n_s_GetEdge;
   PyObject *__pyx_n_s_GetEdges;
   PyObject *__pyx_n_s_GetLineAngleInRadians;
   PyObject *__pyx_n_s_GetParabolaY;
   PyObject *__pyx_n_s_GetPoints;
   PyObject *__pyx_n_s_GetSegments;
   PyObject *__pyx_n_s_GetVertex;
   PyObject *__pyx_n_s_GetVertices;
+  PyObject *__pyx_n_s_IterateCells;
+  PyObject *__pyx_n_s_IterateEdges;
+  PyObject *__pyx_n_s_IterateVertices;
   PyObject *__pyx_kp_s_Max_distance_must_be_greater_tha;
   PyObject *__pyx_n_s_MemoryError;
+  PyObject *__pyx_n_s_NamedTuple;
   PyObject *__pyx_kp_s_Parabola_equation_tolerance_must;
   PyObject *__pyx_n_s_Pyvoronoi;
   PyObject *__pyx_n_s_Pyvoronoi_AddPoint;
   PyObject *__pyx_n_s_Pyvoronoi_AddSegment;
   PyObject *__pyx_n_s_Pyvoronoi_CheckUnsolvableParabol;
   PyObject *__pyx_n_s_Pyvoronoi_Construct;
   PyObject *__pyx_n_s_Pyvoronoi_CountCells;
@@ -2736,14 +2943,17 @@
   PyObject *__pyx_n_s_Pyvoronoi_GetEdge;
   PyObject *__pyx_n_s_Pyvoronoi_GetEdges;
   PyObject *__pyx_n_s_Pyvoronoi_GetParabolaY;
   PyObject *__pyx_n_s_Pyvoronoi_GetPoints;
   PyObject *__pyx_n_s_Pyvoronoi_GetSegments;
   PyObject *__pyx_n_s_Pyvoronoi_GetVertex;
   PyObject *__pyx_n_s_Pyvoronoi_GetVertices;
+  PyObject *__pyx_n_s_Pyvoronoi_IterateCells;
+  PyObject *__pyx_n_s_Pyvoronoi_IterateEdges;
+  PyObject *__pyx_n_s_Pyvoronoi_IterateVertices;
   PyObject *__pyx_n_s_Pyvoronoi_RetrievePoint;
   PyObject *__pyx_n_s_Pyvoronoi_RetrieveScaledPoint;
   PyObject *__pyx_n_s_Pyvoronoi_RetrieveSegment;
   PyObject *__pyx_n_s_Pyvoronoi_RetriveScaledSegment;
   PyObject *__pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform;
   PyObject *__pyx_n_s_Pyvoronoi___reduce_cython;
   PyObject *__pyx_n_s_Pyvoronoi___setstate_cython;
@@ -2757,35 +2967,37 @@
   PyObject *__pyx_n_s_SILENT;
   PyObject *__pyx_kp_s_The_computed_Y_on_the_parabola_f;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_Unrotate;
   PyObject *__pyx_n_s_UnsolvableParabolaEquation;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_Vertex;
-  PyObject *__pyx_n_s_Vertex___init;
   PyObject *__pyx_n_s_VoronoiException;
   PyObject *__pyx_n_s_X;
   PyObject *__pyx_n_s_Y;
-  PyObject *__pyx_n_s__2;
+  PyObject *__pyx_n_s__4;
+  PyObject *__pyx_kp_u__5;
   PyObject *__pyx_n_s__65;
   PyObject *__pyx_n_s_angle;
-  PyObject *__pyx_n_s_append;
+  PyObject *__pyx_n_s_annotations;
+  PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_atan2;
+  PyObject *__pyx_n_s_bool;
   PyObject *__pyx_n_s_boost_x;
   PyObject *__pyx_n_s_boost_y;
   PyObject *__pyx_n_s_c_cell;
   PyObject *__pyx_n_s_c_edge;
   PyObject *__pyx_n_s_c_point;
   PyObject *__pyx_n_s_c_segment;
   PyObject *__pyx_n_s_c_vertex;
   PyObject *__pyx_n_s_cell;
   PyObject *__pyx_n_s_cell_identifier;
-  PyObject *__pyx_n_s_class_getitem;
   PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_close;
   PyObject *__pyx_n_s_computed_point_y;
   PyObject *__pyx_n_s_contains_point;
   PyObject *__pyx_n_s_contains_segment;
   PyObject *__pyx_n_s_copy;
   PyObject *__pyx_n_s_copy_2;
   PyObject *__pyx_n_s_cos;
   PyObject *__pyx_n_s_count;
@@ -2806,27 +3018,26 @@
   PyObject *__pyx_n_s_edgeEndVertex;
   PyObject *__pyx_n_s_edgeStartVertex;
   PyObject *__pyx_n_s_edges;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_end;
   PyObject *__pyx_n_s_end_point_x;
   PyObject *__pyx_n_s_end_point_y;
+  PyObject *__pyx_n_s_float;
   PyObject *__pyx_n_s_focus;
   PyObject *__pyx_n_s_focus_rotated;
   PyObject *__pyx_n_s_format;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_index;
-  PyObject *__pyx_n_s_init;
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_initializing;
-  PyObject *__pyx_n_s_inputPoints;
-  PyObject *__pyx_n_s_inputSegments;
   PyObject *__pyx_n_s_input_segment;
+  PyObject *__pyx_n_s_int;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_is_degenerate;
   PyObject *__pyx_n_s_is_linear;
   PyObject *__pyx_n_s_is_open;
   PyObject *__pyx_n_s_is_primary;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_log_action;
@@ -2841,17 +3052,15 @@
   PyObject *__pyx_n_s_mro_entries;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_next;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_non_scaled_point;
   PyObject *__pyx_n_s_non_scaled_segment;
   PyObject *__pyx_n_s_output;
-  PyObject *__pyx_n_s_outputCells;
-  PyObject *__pyx_n_s_outputEdges;
-  PyObject *__pyx_n_s_outputVertices;
+  PyObject *__pyx_n_s_p;
   PyObject *__pyx_n_s_p0;
   PyObject *__pyx_n_s_p1;
   PyObject *__pyx_n_s_parabola_end;
   PyObject *__pyx_n_s_parabola_end_rotated;
   PyObject *__pyx_n_s_parabola_end_rotated_check;
   PyObject *__pyx_n_s_parabola_equation_tolerance;
   PyObject *__pyx_n_s_parabola_start;
@@ -2870,18 +3079,20 @@
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_vtable;
   PyObject *__pyx_n_s_qualname;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
+  PyObject *__pyx_n_s_s;
   PyObject *__pyx_n_s_scaling_factor;
   PyObject *__pyx_n_s_segment;
   PyObject *__pyx_n_s_segmentSite;
   PyObject *__pyx_n_s_self;
+  PyObject *__pyx_n_s_send;
   PyObject *__pyx_n_s_set_name;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shift_x;
   PyObject *__pyx_n_s_shift_y;
   PyObject *__pyx_n_s_sin;
   PyObject *__pyx_n_s_site;
@@ -2896,81 +3107,83 @@
   PyObject *__pyx_n_s_struct;
   PyObject *__pyx_n_s_super;
   PyObject *__pyx_n_s_sys;
   PyObject *__pyx_n_s_sys_2;
   PyObject *__pyx_n_s_t;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_theta;
+  PyObject *__pyx_n_s_throw;
   PyObject *__pyx_n_s_time;
   PyObject *__pyx_n_s_time_2;
   PyObject *__pyx_n_s_tolerance;
   PyObject *__pyx_n_s_twin;
   PyObject *__pyx_n_s_twinCell;
   PyObject *__pyx_n_s_twinEdge;
+  PyObject *__pyx_n_s_typing;
+  PyObject *__pyx_kp_s_typing_Type_Edge;
+  PyObject *__pyx_kp_s_typing_Type_Vertex;
   PyObject *__pyx_n_s_unicodedata;
   PyObject *__pyx_n_s_unicodedata_2;
   PyObject *__pyx_n_s_vertices;
   PyObject *__pyx_n_s_x;
-  PyObject *__pyx_n_s_y;
   PyObject *__pyx_float_0_0;
   PyObject *__pyx_float_0_0001;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_2;
   PyObject *__pyx_int_neg_1;
-  PyObject *__pyx_slice_;
-  PyObject *__pyx_tuple__3;
-  PyObject *__pyx_tuple__5;
-  PyObject *__pyx_tuple__7;
-  PyObject *__pyx_tuple__9;
-  PyObject *__pyx_tuple__11;
-  PyObject *__pyx_tuple__13;
-  PyObject *__pyx_tuple__15;
-  PyObject *__pyx_tuple__17;
+  PyObject *__pyx_codeobj_;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_tuple__12;
+  PyObject *__pyx_tuple__14;
+  PyObject *__pyx_tuple__16;
   PyObject *__pyx_tuple__19;
-  PyObject *__pyx_tuple__22;
-  PyObject *__pyx_tuple__24;
-  PyObject *__pyx_tuple__26;
-  PyObject *__pyx_tuple__28;
-  PyObject *__pyx_tuple__30;
-  PyObject *__pyx_tuple__32;
-  PyObject *__pyx_tuple__39;
+  PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__23;
+  PyObject *__pyx_tuple__25;
+  PyObject *__pyx_tuple__27;
+  PyObject *__pyx_tuple__29;
+  PyObject *__pyx_tuple__34;
+  PyObject *__pyx_tuple__36;
+  PyObject *__pyx_tuple__38;
+  PyObject *__pyx_tuple__40;
   PyObject *__pyx_tuple__43;
   PyObject *__pyx_tuple__45;
   PyObject *__pyx_tuple__47;
   PyObject *__pyx_tuple__48;
   PyObject *__pyx_tuple__50;
   PyObject *__pyx_tuple__52;
   PyObject *__pyx_tuple__54;
   PyObject *__pyx_tuple__56;
   PyObject *__pyx_tuple__58;
   PyObject *__pyx_tuple__60;
   PyObject *__pyx_tuple__63;
-  PyObject *__pyx_codeobj__4;
-  PyObject *__pyx_codeobj__6;
-  PyObject *__pyx_codeobj__8;
-  PyObject *__pyx_codeobj__10;
-  PyObject *__pyx_codeobj__12;
-  PyObject *__pyx_codeobj__14;
-  PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__2;
+  PyObject *__pyx_codeobj__3;
+  PyObject *__pyx_codeobj__7;
+  PyObject *__pyx_codeobj__9;
+  PyObject *__pyx_codeobj__11;
+  PyObject *__pyx_codeobj__13;
+  PyObject *__pyx_codeobj__15;
+  PyObject *__pyx_codeobj__17;
   PyObject *__pyx_codeobj__18;
   PyObject *__pyx_codeobj__20;
-  PyObject *__pyx_codeobj__21;
-  PyObject *__pyx_codeobj__23;
-  PyObject *__pyx_codeobj__25;
-  PyObject *__pyx_codeobj__27;
-  PyObject *__pyx_codeobj__29;
+  PyObject *__pyx_codeobj__22;
+  PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__26;
+  PyObject *__pyx_codeobj__28;
+  PyObject *__pyx_codeobj__30;
   PyObject *__pyx_codeobj__31;
+  PyObject *__pyx_codeobj__32;
   PyObject *__pyx_codeobj__33;
-  PyObject *__pyx_codeobj__34;
   PyObject *__pyx_codeobj__35;
-  PyObject *__pyx_codeobj__36;
   PyObject *__pyx_codeobj__37;
-  PyObject *__pyx_codeobj__38;
-  PyObject *__pyx_codeobj__40;
+  PyObject *__pyx_codeobj__39;
   PyObject *__pyx_codeobj__41;
   PyObject *__pyx_codeobj__42;
   PyObject *__pyx_codeobj__44;
   PyObject *__pyx_codeobj__46;
   PyObject *__pyx_codeobj__49;
   PyObject *__pyx_codeobj__51;
   PyObject *__pyx_codeobj__53;
@@ -3020,20 +3233,25 @@
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_9pyvoronoi_Pyvoronoi);
   Py_CLEAR(clear_module_state->__pyx_type_9pyvoronoi_Pyvoronoi);
-  Py_CLEAR(clear_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize);
-  Py_CLEAR(clear_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct__Discretize);
+  Py_CLEAR(clear_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices);
+  Py_CLEAR(clear_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices);
+  Py_CLEAR(clear_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges);
+  Py_CLEAR(clear_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges);
+  Py_CLEAR(clear_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells);
+  Py_CLEAR(clear_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells);
+  Py_CLEAR(clear_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize);
+  Py_CLEAR(clear_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize);
   Py_CLEAR(clear_module_state->__pyx_n_s_AddPoint);
   Py_CLEAR(clear_module_state->__pyx_n_s_AddSegment);
   Py_CLEAR(clear_module_state->__pyx_n_s_Cell);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Cell___init);
   Py_CLEAR(clear_module_state->__pyx_n_s_CheckUnsolvableParabolaEquation);
   Py_CLEAR(clear_module_state->__pyx_n_s_Construct);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Construct_has_already_been_calle);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Construct_has_been_called_can_t);
   Py_CLEAR(clear_module_state->__pyx_n_s_CountCells);
   Py_CLEAR(clear_module_state->__pyx_n_s_CountEdges);
   Py_CLEAR(clear_module_state->__pyx_n_s_CountVertices);
@@ -3041,28 +3259,31 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_Deleting_the_VoronoiDiagram_inst);
   Py_CLEAR(clear_module_state->__pyx_n_s_Discretize);
   Py_CLEAR(clear_module_state->__pyx_n_s_DiscretizeCurvedEdge);
   Py_CLEAR(clear_module_state->__pyx_n_s_Discretize_locals_lambda);
   Py_CLEAR(clear_module_state->__pyx_n_s_Distance);
   Py_CLEAR(clear_module_state->__pyx_n_s_DistanceSquared);
   Py_CLEAR(clear_module_state->__pyx_n_s_Edge);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Edge___init);
   Py_CLEAR(clear_module_state->__pyx_n_s_FocusOnDirectixException);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetCell);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetCells);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetEdge);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetEdges);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetLineAngleInRadians);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetParabolaY);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetPoints);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetSegments);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetVertex);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetVertices);
+  Py_CLEAR(clear_module_state->__pyx_n_s_IterateCells);
+  Py_CLEAR(clear_module_state->__pyx_n_s_IterateEdges);
+  Py_CLEAR(clear_module_state->__pyx_n_s_IterateVertices);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Max_distance_must_be_greater_tha);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_NamedTuple);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Parabola_equation_tolerance_must);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_AddPoint);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_AddSegment);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_CheckUnsolvableParabol);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_Construct);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_CountCells);
@@ -3075,14 +3296,17 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_GetEdge);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_GetEdges);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_GetParabolaY);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_GetPoints);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_GetSegments);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_GetVertex);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_GetVertices);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_IterateCells);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_IterateEdges);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_IterateVertices);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_RetrievePoint);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_RetrieveScaledPoint);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_RetrieveSegment);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_RetriveScaledSegment);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyvoronoi___setstate_cython);
@@ -3096,35 +3320,37 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_SILENT);
   Py_CLEAR(clear_module_state->__pyx_kp_s_The_computed_Y_on_the_parabola_f);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Unrotate);
   Py_CLEAR(clear_module_state->__pyx_n_s_UnsolvableParabolaEquation);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Vertex);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Vertex___init);
   Py_CLEAR(clear_module_state->__pyx_n_s_VoronoiException);
   Py_CLEAR(clear_module_state->__pyx_n_s_X);
   Py_CLEAR(clear_module_state->__pyx_n_s_Y);
-  Py_CLEAR(clear_module_state->__pyx_n_s__2);
+  Py_CLEAR(clear_module_state->__pyx_n_s__4);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__5);
   Py_CLEAR(clear_module_state->__pyx_n_s__65);
   Py_CLEAR(clear_module_state->__pyx_n_s_angle);
-  Py_CLEAR(clear_module_state->__pyx_n_s_append);
+  Py_CLEAR(clear_module_state->__pyx_n_s_annotations);
+  Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_atan2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bool);
   Py_CLEAR(clear_module_state->__pyx_n_s_boost_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_boost_y);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_cell);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_edge);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_point);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_segment);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_vertex);
   Py_CLEAR(clear_module_state->__pyx_n_s_cell);
   Py_CLEAR(clear_module_state->__pyx_n_s_cell_identifier);
-  Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_computed_point_y);
   Py_CLEAR(clear_module_state->__pyx_n_s_contains_point);
   Py_CLEAR(clear_module_state->__pyx_n_s_contains_segment);
   Py_CLEAR(clear_module_state->__pyx_n_s_copy);
   Py_CLEAR(clear_module_state->__pyx_n_s_copy_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_cos);
   Py_CLEAR(clear_module_state->__pyx_n_s_count);
@@ -3145,27 +3371,26 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_edgeEndVertex);
   Py_CLEAR(clear_module_state->__pyx_n_s_edgeStartVertex);
   Py_CLEAR(clear_module_state->__pyx_n_s_edges);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_end);
   Py_CLEAR(clear_module_state->__pyx_n_s_end_point_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_end_point_y);
+  Py_CLEAR(clear_module_state->__pyx_n_s_float);
   Py_CLEAR(clear_module_state->__pyx_n_s_focus);
   Py_CLEAR(clear_module_state->__pyx_n_s_focus_rotated);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
-  Py_CLEAR(clear_module_state->__pyx_n_s_init);
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
-  Py_CLEAR(clear_module_state->__pyx_n_s_inputPoints);
-  Py_CLEAR(clear_module_state->__pyx_n_s_inputSegments);
   Py_CLEAR(clear_module_state->__pyx_n_s_input_segment);
+  Py_CLEAR(clear_module_state->__pyx_n_s_int);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_degenerate);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_linear);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_open);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_primary);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_log_action);
@@ -3180,17 +3405,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_mro_entries);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_next);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_non_scaled_point);
   Py_CLEAR(clear_module_state->__pyx_n_s_non_scaled_segment);
   Py_CLEAR(clear_module_state->__pyx_n_s_output);
-  Py_CLEAR(clear_module_state->__pyx_n_s_outputCells);
-  Py_CLEAR(clear_module_state->__pyx_n_s_outputEdges);
-  Py_CLEAR(clear_module_state->__pyx_n_s_outputVertices);
+  Py_CLEAR(clear_module_state->__pyx_n_s_p);
   Py_CLEAR(clear_module_state->__pyx_n_s_p0);
   Py_CLEAR(clear_module_state->__pyx_n_s_p1);
   Py_CLEAR(clear_module_state->__pyx_n_s_parabola_end);
   Py_CLEAR(clear_module_state->__pyx_n_s_parabola_end_rotated);
   Py_CLEAR(clear_module_state->__pyx_n_s_parabola_end_rotated_check);
   Py_CLEAR(clear_module_state->__pyx_n_s_parabola_equation_tolerance);
   Py_CLEAR(clear_module_state->__pyx_n_s_parabola_start);
@@ -3209,18 +3432,20 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
   Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
+  Py_CLEAR(clear_module_state->__pyx_n_s_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_scaling_factor);
   Py_CLEAR(clear_module_state->__pyx_n_s_segment);
   Py_CLEAR(clear_module_state->__pyx_n_s_segmentSite);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
+  Py_CLEAR(clear_module_state->__pyx_n_s_send);
   Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shift_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_shift_y);
   Py_CLEAR(clear_module_state->__pyx_n_s_sin);
   Py_CLEAR(clear_module_state->__pyx_n_s_site);
@@ -3235,81 +3460,83 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_struct);
   Py_CLEAR(clear_module_state->__pyx_n_s_super);
   Py_CLEAR(clear_module_state->__pyx_n_s_sys);
   Py_CLEAR(clear_module_state->__pyx_n_s_sys_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_t);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_theta);
+  Py_CLEAR(clear_module_state->__pyx_n_s_throw);
   Py_CLEAR(clear_module_state->__pyx_n_s_time);
   Py_CLEAR(clear_module_state->__pyx_n_s_time_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_tolerance);
   Py_CLEAR(clear_module_state->__pyx_n_s_twin);
   Py_CLEAR(clear_module_state->__pyx_n_s_twinCell);
   Py_CLEAR(clear_module_state->__pyx_n_s_twinEdge);
+  Py_CLEAR(clear_module_state->__pyx_n_s_typing);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_typing_Type_Edge);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_typing_Type_Vertex);
   Py_CLEAR(clear_module_state->__pyx_n_s_unicodedata);
   Py_CLEAR(clear_module_state->__pyx_n_s_unicodedata_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_vertices);
   Py_CLEAR(clear_module_state->__pyx_n_s_x);
-  Py_CLEAR(clear_module_state->__pyx_n_s_y);
   Py_CLEAR(clear_module_state->__pyx_float_0_0);
   Py_CLEAR(clear_module_state->__pyx_float_0_0001);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_2);
   Py_CLEAR(clear_module_state->__pyx_int_neg_1);
-  Py_CLEAR(clear_module_state->__pyx_slice_);
-  Py_CLEAR(clear_module_state->__pyx_tuple__3);
-  Py_CLEAR(clear_module_state->__pyx_tuple__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__7);
-  Py_CLEAR(clear_module_state->__pyx_tuple__9);
-  Py_CLEAR(clear_module_state->__pyx_tuple__11);
-  Py_CLEAR(clear_module_state->__pyx_tuple__13);
-  Py_CLEAR(clear_module_state->__pyx_tuple__15);
-  Py_CLEAR(clear_module_state->__pyx_tuple__17);
+  Py_CLEAR(clear_module_state->__pyx_codeobj_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_tuple__12);
+  Py_CLEAR(clear_module_state->__pyx_tuple__14);
+  Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_tuple__19);
-  Py_CLEAR(clear_module_state->__pyx_tuple__22);
-  Py_CLEAR(clear_module_state->__pyx_tuple__24);
-  Py_CLEAR(clear_module_state->__pyx_tuple__26);
-  Py_CLEAR(clear_module_state->__pyx_tuple__28);
-  Py_CLEAR(clear_module_state->__pyx_tuple__30);
-  Py_CLEAR(clear_module_state->__pyx_tuple__32);
-  Py_CLEAR(clear_module_state->__pyx_tuple__39);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__23);
+  Py_CLEAR(clear_module_state->__pyx_tuple__25);
+  Py_CLEAR(clear_module_state->__pyx_tuple__27);
+  Py_CLEAR(clear_module_state->__pyx_tuple__29);
+  Py_CLEAR(clear_module_state->__pyx_tuple__34);
+  Py_CLEAR(clear_module_state->__pyx_tuple__36);
+  Py_CLEAR(clear_module_state->__pyx_tuple__38);
+  Py_CLEAR(clear_module_state->__pyx_tuple__40);
   Py_CLEAR(clear_module_state->__pyx_tuple__43);
   Py_CLEAR(clear_module_state->__pyx_tuple__45);
   Py_CLEAR(clear_module_state->__pyx_tuple__47);
   Py_CLEAR(clear_module_state->__pyx_tuple__48);
   Py_CLEAR(clear_module_state->__pyx_tuple__50);
   Py_CLEAR(clear_module_state->__pyx_tuple__52);
   Py_CLEAR(clear_module_state->__pyx_tuple__54);
   Py_CLEAR(clear_module_state->__pyx_tuple__56);
   Py_CLEAR(clear_module_state->__pyx_tuple__58);
   Py_CLEAR(clear_module_state->__pyx_tuple__60);
   Py_CLEAR(clear_module_state->__pyx_tuple__63);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__12);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__2);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__3);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
   Py_CLEAR(clear_module_state->__pyx_codeobj__18);
   Py_CLEAR(clear_module_state->__pyx_codeobj__20);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__28);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__30);
   Py_CLEAR(clear_module_state->__pyx_codeobj__31);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__32);
   Py_CLEAR(clear_module_state->__pyx_codeobj__33);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__34);
   Py_CLEAR(clear_module_state->__pyx_codeobj__35);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__36);
   Py_CLEAR(clear_module_state->__pyx_codeobj__37);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__38);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__40);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__39);
   Py_CLEAR(clear_module_state->__pyx_codeobj__41);
   Py_CLEAR(clear_module_state->__pyx_codeobj__42);
   Py_CLEAR(clear_module_state->__pyx_codeobj__44);
   Py_CLEAR(clear_module_state->__pyx_codeobj__46);
   Py_CLEAR(clear_module_state->__pyx_codeobj__49);
   Py_CLEAR(clear_module_state->__pyx_codeobj__51);
   Py_CLEAR(clear_module_state->__pyx_codeobj__53);
@@ -3337,20 +3564,25 @@
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_9pyvoronoi_Pyvoronoi);
   Py_VISIT(traverse_module_state->__pyx_type_9pyvoronoi_Pyvoronoi);
-  Py_VISIT(traverse_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize);
-  Py_VISIT(traverse_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct__Discretize);
+  Py_VISIT(traverse_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices);
+  Py_VISIT(traverse_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices);
+  Py_VISIT(traverse_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges);
+  Py_VISIT(traverse_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges);
+  Py_VISIT(traverse_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells);
+  Py_VISIT(traverse_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells);
+  Py_VISIT(traverse_module_state->__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize);
+  Py_VISIT(traverse_module_state->__pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize);
   Py_VISIT(traverse_module_state->__pyx_n_s_AddPoint);
   Py_VISIT(traverse_module_state->__pyx_n_s_AddSegment);
   Py_VISIT(traverse_module_state->__pyx_n_s_Cell);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Cell___init);
   Py_VISIT(traverse_module_state->__pyx_n_s_CheckUnsolvableParabolaEquation);
   Py_VISIT(traverse_module_state->__pyx_n_s_Construct);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Construct_has_already_been_calle);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Construct_has_been_called_can_t);
   Py_VISIT(traverse_module_state->__pyx_n_s_CountCells);
   Py_VISIT(traverse_module_state->__pyx_n_s_CountEdges);
   Py_VISIT(traverse_module_state->__pyx_n_s_CountVertices);
@@ -3358,28 +3590,31 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_Deleting_the_VoronoiDiagram_inst);
   Py_VISIT(traverse_module_state->__pyx_n_s_Discretize);
   Py_VISIT(traverse_module_state->__pyx_n_s_DiscretizeCurvedEdge);
   Py_VISIT(traverse_module_state->__pyx_n_s_Discretize_locals_lambda);
   Py_VISIT(traverse_module_state->__pyx_n_s_Distance);
   Py_VISIT(traverse_module_state->__pyx_n_s_DistanceSquared);
   Py_VISIT(traverse_module_state->__pyx_n_s_Edge);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Edge___init);
   Py_VISIT(traverse_module_state->__pyx_n_s_FocusOnDirectixException);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetCell);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetCells);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetEdge);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetEdges);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetLineAngleInRadians);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetParabolaY);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetPoints);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetSegments);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetVertex);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetVertices);
+  Py_VISIT(traverse_module_state->__pyx_n_s_IterateCells);
+  Py_VISIT(traverse_module_state->__pyx_n_s_IterateEdges);
+  Py_VISIT(traverse_module_state->__pyx_n_s_IterateVertices);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Max_distance_must_be_greater_tha);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_NamedTuple);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Parabola_equation_tolerance_must);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_AddPoint);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_AddSegment);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_CheckUnsolvableParabol);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_Construct);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_CountCells);
@@ -3392,14 +3627,17 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_GetEdge);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_GetEdges);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_GetParabolaY);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_GetPoints);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_GetSegments);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_GetVertex);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_GetVertices);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_IterateCells);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_IterateEdges);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_IterateVertices);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_RetrievePoint);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_RetrieveScaledPoint);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_RetrieveSegment);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_RetriveScaledSegment);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyvoronoi___setstate_cython);
@@ -3413,35 +3651,37 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_SILENT);
   Py_VISIT(traverse_module_state->__pyx_kp_s_The_computed_Y_on_the_parabola_f);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Unrotate);
   Py_VISIT(traverse_module_state->__pyx_n_s_UnsolvableParabolaEquation);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Vertex);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Vertex___init);
   Py_VISIT(traverse_module_state->__pyx_n_s_VoronoiException);
   Py_VISIT(traverse_module_state->__pyx_n_s_X);
   Py_VISIT(traverse_module_state->__pyx_n_s_Y);
-  Py_VISIT(traverse_module_state->__pyx_n_s__2);
+  Py_VISIT(traverse_module_state->__pyx_n_s__4);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__5);
   Py_VISIT(traverse_module_state->__pyx_n_s__65);
   Py_VISIT(traverse_module_state->__pyx_n_s_angle);
-  Py_VISIT(traverse_module_state->__pyx_n_s_append);
+  Py_VISIT(traverse_module_state->__pyx_n_s_annotations);
+  Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_atan2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bool);
   Py_VISIT(traverse_module_state->__pyx_n_s_boost_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_boost_y);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_cell);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_edge);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_point);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_segment);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_vertex);
   Py_VISIT(traverse_module_state->__pyx_n_s_cell);
   Py_VISIT(traverse_module_state->__pyx_n_s_cell_identifier);
-  Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_computed_point_y);
   Py_VISIT(traverse_module_state->__pyx_n_s_contains_point);
   Py_VISIT(traverse_module_state->__pyx_n_s_contains_segment);
   Py_VISIT(traverse_module_state->__pyx_n_s_copy);
   Py_VISIT(traverse_module_state->__pyx_n_s_copy_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_cos);
   Py_VISIT(traverse_module_state->__pyx_n_s_count);
@@ -3462,27 +3702,26 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_edgeEndVertex);
   Py_VISIT(traverse_module_state->__pyx_n_s_edgeStartVertex);
   Py_VISIT(traverse_module_state->__pyx_n_s_edges);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_end);
   Py_VISIT(traverse_module_state->__pyx_n_s_end_point_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_end_point_y);
+  Py_VISIT(traverse_module_state->__pyx_n_s_float);
   Py_VISIT(traverse_module_state->__pyx_n_s_focus);
   Py_VISIT(traverse_module_state->__pyx_n_s_focus_rotated);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
-  Py_VISIT(traverse_module_state->__pyx_n_s_init);
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
-  Py_VISIT(traverse_module_state->__pyx_n_s_inputPoints);
-  Py_VISIT(traverse_module_state->__pyx_n_s_inputSegments);
   Py_VISIT(traverse_module_state->__pyx_n_s_input_segment);
+  Py_VISIT(traverse_module_state->__pyx_n_s_int);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_degenerate);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_linear);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_open);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_primary);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_log_action);
@@ -3497,17 +3736,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_mro_entries);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_next);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_non_scaled_point);
   Py_VISIT(traverse_module_state->__pyx_n_s_non_scaled_segment);
   Py_VISIT(traverse_module_state->__pyx_n_s_output);
-  Py_VISIT(traverse_module_state->__pyx_n_s_outputCells);
-  Py_VISIT(traverse_module_state->__pyx_n_s_outputEdges);
-  Py_VISIT(traverse_module_state->__pyx_n_s_outputVertices);
+  Py_VISIT(traverse_module_state->__pyx_n_s_p);
   Py_VISIT(traverse_module_state->__pyx_n_s_p0);
   Py_VISIT(traverse_module_state->__pyx_n_s_p1);
   Py_VISIT(traverse_module_state->__pyx_n_s_parabola_end);
   Py_VISIT(traverse_module_state->__pyx_n_s_parabola_end_rotated);
   Py_VISIT(traverse_module_state->__pyx_n_s_parabola_end_rotated_check);
   Py_VISIT(traverse_module_state->__pyx_n_s_parabola_equation_tolerance);
   Py_VISIT(traverse_module_state->__pyx_n_s_parabola_start);
@@ -3526,18 +3763,20 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
   Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
+  Py_VISIT(traverse_module_state->__pyx_n_s_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_scaling_factor);
   Py_VISIT(traverse_module_state->__pyx_n_s_segment);
   Py_VISIT(traverse_module_state->__pyx_n_s_segmentSite);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
+  Py_VISIT(traverse_module_state->__pyx_n_s_send);
   Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shift_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_shift_y);
   Py_VISIT(traverse_module_state->__pyx_n_s_sin);
   Py_VISIT(traverse_module_state->__pyx_n_s_site);
@@ -3552,81 +3791,83 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_struct);
   Py_VISIT(traverse_module_state->__pyx_n_s_super);
   Py_VISIT(traverse_module_state->__pyx_n_s_sys);
   Py_VISIT(traverse_module_state->__pyx_n_s_sys_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_t);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_theta);
+  Py_VISIT(traverse_module_state->__pyx_n_s_throw);
   Py_VISIT(traverse_module_state->__pyx_n_s_time);
   Py_VISIT(traverse_module_state->__pyx_n_s_time_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_tolerance);
   Py_VISIT(traverse_module_state->__pyx_n_s_twin);
   Py_VISIT(traverse_module_state->__pyx_n_s_twinCell);
   Py_VISIT(traverse_module_state->__pyx_n_s_twinEdge);
+  Py_VISIT(traverse_module_state->__pyx_n_s_typing);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_typing_Type_Edge);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_typing_Type_Vertex);
   Py_VISIT(traverse_module_state->__pyx_n_s_unicodedata);
   Py_VISIT(traverse_module_state->__pyx_n_s_unicodedata_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_vertices);
   Py_VISIT(traverse_module_state->__pyx_n_s_x);
-  Py_VISIT(traverse_module_state->__pyx_n_s_y);
   Py_VISIT(traverse_module_state->__pyx_float_0_0);
   Py_VISIT(traverse_module_state->__pyx_float_0_0001);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_2);
   Py_VISIT(traverse_module_state->__pyx_int_neg_1);
-  Py_VISIT(traverse_module_state->__pyx_slice_);
-  Py_VISIT(traverse_module_state->__pyx_tuple__3);
-  Py_VISIT(traverse_module_state->__pyx_tuple__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__7);
-  Py_VISIT(traverse_module_state->__pyx_tuple__9);
-  Py_VISIT(traverse_module_state->__pyx_tuple__11);
-  Py_VISIT(traverse_module_state->__pyx_tuple__13);
-  Py_VISIT(traverse_module_state->__pyx_tuple__15);
-  Py_VISIT(traverse_module_state->__pyx_tuple__17);
+  Py_VISIT(traverse_module_state->__pyx_codeobj_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_tuple__12);
+  Py_VISIT(traverse_module_state->__pyx_tuple__14);
+  Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_tuple__19);
-  Py_VISIT(traverse_module_state->__pyx_tuple__22);
-  Py_VISIT(traverse_module_state->__pyx_tuple__24);
-  Py_VISIT(traverse_module_state->__pyx_tuple__26);
-  Py_VISIT(traverse_module_state->__pyx_tuple__28);
-  Py_VISIT(traverse_module_state->__pyx_tuple__30);
-  Py_VISIT(traverse_module_state->__pyx_tuple__32);
-  Py_VISIT(traverse_module_state->__pyx_tuple__39);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__23);
+  Py_VISIT(traverse_module_state->__pyx_tuple__25);
+  Py_VISIT(traverse_module_state->__pyx_tuple__27);
+  Py_VISIT(traverse_module_state->__pyx_tuple__29);
+  Py_VISIT(traverse_module_state->__pyx_tuple__34);
+  Py_VISIT(traverse_module_state->__pyx_tuple__36);
+  Py_VISIT(traverse_module_state->__pyx_tuple__38);
+  Py_VISIT(traverse_module_state->__pyx_tuple__40);
   Py_VISIT(traverse_module_state->__pyx_tuple__43);
   Py_VISIT(traverse_module_state->__pyx_tuple__45);
   Py_VISIT(traverse_module_state->__pyx_tuple__47);
   Py_VISIT(traverse_module_state->__pyx_tuple__48);
   Py_VISIT(traverse_module_state->__pyx_tuple__50);
   Py_VISIT(traverse_module_state->__pyx_tuple__52);
   Py_VISIT(traverse_module_state->__pyx_tuple__54);
   Py_VISIT(traverse_module_state->__pyx_tuple__56);
   Py_VISIT(traverse_module_state->__pyx_tuple__58);
   Py_VISIT(traverse_module_state->__pyx_tuple__60);
   Py_VISIT(traverse_module_state->__pyx_tuple__63);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__12);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__2);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__3);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
   Py_VISIT(traverse_module_state->__pyx_codeobj__18);
   Py_VISIT(traverse_module_state->__pyx_codeobj__20);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__28);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__30);
   Py_VISIT(traverse_module_state->__pyx_codeobj__31);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__32);
   Py_VISIT(traverse_module_state->__pyx_codeobj__33);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__34);
   Py_VISIT(traverse_module_state->__pyx_codeobj__35);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__36);
   Py_VISIT(traverse_module_state->__pyx_codeobj__37);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__38);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__40);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__39);
   Py_VISIT(traverse_module_state->__pyx_codeobj__41);
   Py_VISIT(traverse_module_state->__pyx_codeobj__42);
   Py_VISIT(traverse_module_state->__pyx_codeobj__44);
   Py_VISIT(traverse_module_state->__pyx_codeobj__46);
   Py_VISIT(traverse_module_state->__pyx_codeobj__49);
   Py_VISIT(traverse_module_state->__pyx_codeobj__51);
   Py_VISIT(traverse_module_state->__pyx_codeobj__53);
@@ -3662,22 +3903,27 @@
 #define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
 #endif
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_9pyvoronoi_Pyvoronoi __pyx_mstate_global->__pyx_type_9pyvoronoi_Pyvoronoi
-#define __pyx_type_9pyvoronoi___pyx_scope_struct__Discretize __pyx_mstate_global->__pyx_type_9pyvoronoi___pyx_scope_struct__Discretize
+#define __pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices __pyx_mstate_global->__pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices
+#define __pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges __pyx_mstate_global->__pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges
+#define __pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells __pyx_mstate_global->__pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells
+#define __pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize __pyx_mstate_global->__pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize
 #endif
 #define __pyx_ptype_9pyvoronoi_Pyvoronoi __pyx_mstate_global->__pyx_ptype_9pyvoronoi_Pyvoronoi
-#define __pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize __pyx_mstate_global->__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize
+#define __pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices __pyx_mstate_global->__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices
+#define __pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges __pyx_mstate_global->__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges
+#define __pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells __pyx_mstate_global->__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells
+#define __pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize __pyx_mstate_global->__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize
 #define __pyx_n_s_AddPoint __pyx_mstate_global->__pyx_n_s_AddPoint
 #define __pyx_n_s_AddSegment __pyx_mstate_global->__pyx_n_s_AddSegment
 #define __pyx_n_s_Cell __pyx_mstate_global->__pyx_n_s_Cell
-#define __pyx_n_s_Cell___init __pyx_mstate_global->__pyx_n_s_Cell___init
 #define __pyx_n_s_CheckUnsolvableParabolaEquation __pyx_mstate_global->__pyx_n_s_CheckUnsolvableParabolaEquation
 #define __pyx_n_s_Construct __pyx_mstate_global->__pyx_n_s_Construct
 #define __pyx_kp_s_Construct_has_already_been_calle __pyx_mstate_global->__pyx_kp_s_Construct_has_already_been_calle
 #define __pyx_kp_s_Construct_has_been_called_can_t __pyx_mstate_global->__pyx_kp_s_Construct_has_been_called_can_t
 #define __pyx_n_s_CountCells __pyx_mstate_global->__pyx_n_s_CountCells
 #define __pyx_n_s_CountEdges __pyx_mstate_global->__pyx_n_s_CountEdges
 #define __pyx_n_s_CountVertices __pyx_mstate_global->__pyx_n_s_CountVertices
@@ -3685,28 +3931,31 @@
 #define __pyx_kp_s_Deleting_the_VoronoiDiagram_inst __pyx_mstate_global->__pyx_kp_s_Deleting_the_VoronoiDiagram_inst
 #define __pyx_n_s_Discretize __pyx_mstate_global->__pyx_n_s_Discretize
 #define __pyx_n_s_DiscretizeCurvedEdge __pyx_mstate_global->__pyx_n_s_DiscretizeCurvedEdge
 #define __pyx_n_s_Discretize_locals_lambda __pyx_mstate_global->__pyx_n_s_Discretize_locals_lambda
 #define __pyx_n_s_Distance __pyx_mstate_global->__pyx_n_s_Distance
 #define __pyx_n_s_DistanceSquared __pyx_mstate_global->__pyx_n_s_DistanceSquared
 #define __pyx_n_s_Edge __pyx_mstate_global->__pyx_n_s_Edge
-#define __pyx_n_s_Edge___init __pyx_mstate_global->__pyx_n_s_Edge___init
 #define __pyx_n_s_FocusOnDirectixException __pyx_mstate_global->__pyx_n_s_FocusOnDirectixException
 #define __pyx_n_s_GetCell __pyx_mstate_global->__pyx_n_s_GetCell
 #define __pyx_n_s_GetCells __pyx_mstate_global->__pyx_n_s_GetCells
 #define __pyx_n_s_GetEdge __pyx_mstate_global->__pyx_n_s_GetEdge
 #define __pyx_n_s_GetEdges __pyx_mstate_global->__pyx_n_s_GetEdges
 #define __pyx_n_s_GetLineAngleInRadians __pyx_mstate_global->__pyx_n_s_GetLineAngleInRadians
 #define __pyx_n_s_GetParabolaY __pyx_mstate_global->__pyx_n_s_GetParabolaY
 #define __pyx_n_s_GetPoints __pyx_mstate_global->__pyx_n_s_GetPoints
 #define __pyx_n_s_GetSegments __pyx_mstate_global->__pyx_n_s_GetSegments
 #define __pyx_n_s_GetVertex __pyx_mstate_global->__pyx_n_s_GetVertex
 #define __pyx_n_s_GetVertices __pyx_mstate_global->__pyx_n_s_GetVertices
+#define __pyx_n_s_IterateCells __pyx_mstate_global->__pyx_n_s_IterateCells
+#define __pyx_n_s_IterateEdges __pyx_mstate_global->__pyx_n_s_IterateEdges
+#define __pyx_n_s_IterateVertices __pyx_mstate_global->__pyx_n_s_IterateVertices
 #define __pyx_kp_s_Max_distance_must_be_greater_tha __pyx_mstate_global->__pyx_kp_s_Max_distance_must_be_greater_tha
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
+#define __pyx_n_s_NamedTuple __pyx_mstate_global->__pyx_n_s_NamedTuple
 #define __pyx_kp_s_Parabola_equation_tolerance_must __pyx_mstate_global->__pyx_kp_s_Parabola_equation_tolerance_must
 #define __pyx_n_s_Pyvoronoi __pyx_mstate_global->__pyx_n_s_Pyvoronoi
 #define __pyx_n_s_Pyvoronoi_AddPoint __pyx_mstate_global->__pyx_n_s_Pyvoronoi_AddPoint
 #define __pyx_n_s_Pyvoronoi_AddSegment __pyx_mstate_global->__pyx_n_s_Pyvoronoi_AddSegment
 #define __pyx_n_s_Pyvoronoi_CheckUnsolvableParabol __pyx_mstate_global->__pyx_n_s_Pyvoronoi_CheckUnsolvableParabol
 #define __pyx_n_s_Pyvoronoi_Construct __pyx_mstate_global->__pyx_n_s_Pyvoronoi_Construct
 #define __pyx_n_s_Pyvoronoi_CountCells __pyx_mstate_global->__pyx_n_s_Pyvoronoi_CountCells
@@ -3719,14 +3968,17 @@
 #define __pyx_n_s_Pyvoronoi_GetEdge __pyx_mstate_global->__pyx_n_s_Pyvoronoi_GetEdge
 #define __pyx_n_s_Pyvoronoi_GetEdges __pyx_mstate_global->__pyx_n_s_Pyvoronoi_GetEdges
 #define __pyx_n_s_Pyvoronoi_GetParabolaY __pyx_mstate_global->__pyx_n_s_Pyvoronoi_GetParabolaY
 #define __pyx_n_s_Pyvoronoi_GetPoints __pyx_mstate_global->__pyx_n_s_Pyvoronoi_GetPoints
 #define __pyx_n_s_Pyvoronoi_GetSegments __pyx_mstate_global->__pyx_n_s_Pyvoronoi_GetSegments
 #define __pyx_n_s_Pyvoronoi_GetVertex __pyx_mstate_global->__pyx_n_s_Pyvoronoi_GetVertex
 #define __pyx_n_s_Pyvoronoi_GetVertices __pyx_mstate_global->__pyx_n_s_Pyvoronoi_GetVertices
+#define __pyx_n_s_Pyvoronoi_IterateCells __pyx_mstate_global->__pyx_n_s_Pyvoronoi_IterateCells
+#define __pyx_n_s_Pyvoronoi_IterateEdges __pyx_mstate_global->__pyx_n_s_Pyvoronoi_IterateEdges
+#define __pyx_n_s_Pyvoronoi_IterateVertices __pyx_mstate_global->__pyx_n_s_Pyvoronoi_IterateVertices
 #define __pyx_n_s_Pyvoronoi_RetrievePoint __pyx_mstate_global->__pyx_n_s_Pyvoronoi_RetrievePoint
 #define __pyx_n_s_Pyvoronoi_RetrieveScaledPoint __pyx_mstate_global->__pyx_n_s_Pyvoronoi_RetrieveScaledPoint
 #define __pyx_n_s_Pyvoronoi_RetrieveSegment __pyx_mstate_global->__pyx_n_s_Pyvoronoi_RetrieveSegment
 #define __pyx_n_s_Pyvoronoi_RetriveScaledSegment __pyx_mstate_global->__pyx_n_s_Pyvoronoi_RetriveScaledSegment
 #define __pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform __pyx_mstate_global->__pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform
 #define __pyx_n_s_Pyvoronoi___reduce_cython __pyx_mstate_global->__pyx_n_s_Pyvoronoi___reduce_cython
 #define __pyx_n_s_Pyvoronoi___setstate_cython __pyx_mstate_global->__pyx_n_s_Pyvoronoi___setstate_cython
@@ -3740,35 +3992,37 @@
 #define __pyx_n_s_SILENT __pyx_mstate_global->__pyx_n_s_SILENT
 #define __pyx_kp_s_The_computed_Y_on_the_parabola_f __pyx_mstate_global->__pyx_kp_s_The_computed_Y_on_the_parabola_f
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_Unrotate __pyx_mstate_global->__pyx_n_s_Unrotate
 #define __pyx_n_s_UnsolvableParabolaEquation __pyx_mstate_global->__pyx_n_s_UnsolvableParabolaEquation
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_Vertex __pyx_mstate_global->__pyx_n_s_Vertex
-#define __pyx_n_s_Vertex___init __pyx_mstate_global->__pyx_n_s_Vertex___init
 #define __pyx_n_s_VoronoiException __pyx_mstate_global->__pyx_n_s_VoronoiException
 #define __pyx_n_s_X __pyx_mstate_global->__pyx_n_s_X
 #define __pyx_n_s_Y __pyx_mstate_global->__pyx_n_s_Y
-#define __pyx_n_s__2 __pyx_mstate_global->__pyx_n_s__2
+#define __pyx_n_s__4 __pyx_mstate_global->__pyx_n_s__4
+#define __pyx_kp_u__5 __pyx_mstate_global->__pyx_kp_u__5
 #define __pyx_n_s__65 __pyx_mstate_global->__pyx_n_s__65
 #define __pyx_n_s_angle __pyx_mstate_global->__pyx_n_s_angle
-#define __pyx_n_s_append __pyx_mstate_global->__pyx_n_s_append
+#define __pyx_n_s_annotations __pyx_mstate_global->__pyx_n_s_annotations
+#define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_atan2 __pyx_mstate_global->__pyx_n_s_atan2
+#define __pyx_n_s_bool __pyx_mstate_global->__pyx_n_s_bool
 #define __pyx_n_s_boost_x __pyx_mstate_global->__pyx_n_s_boost_x
 #define __pyx_n_s_boost_y __pyx_mstate_global->__pyx_n_s_boost_y
 #define __pyx_n_s_c_cell __pyx_mstate_global->__pyx_n_s_c_cell
 #define __pyx_n_s_c_edge __pyx_mstate_global->__pyx_n_s_c_edge
 #define __pyx_n_s_c_point __pyx_mstate_global->__pyx_n_s_c_point
 #define __pyx_n_s_c_segment __pyx_mstate_global->__pyx_n_s_c_segment
 #define __pyx_n_s_c_vertex __pyx_mstate_global->__pyx_n_s_c_vertex
 #define __pyx_n_s_cell __pyx_mstate_global->__pyx_n_s_cell
 #define __pyx_n_s_cell_identifier __pyx_mstate_global->__pyx_n_s_cell_identifier
-#define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
 #define __pyx_n_s_computed_point_y __pyx_mstate_global->__pyx_n_s_computed_point_y
 #define __pyx_n_s_contains_point __pyx_mstate_global->__pyx_n_s_contains_point
 #define __pyx_n_s_contains_segment __pyx_mstate_global->__pyx_n_s_contains_segment
 #define __pyx_n_s_copy __pyx_mstate_global->__pyx_n_s_copy
 #define __pyx_n_s_copy_2 __pyx_mstate_global->__pyx_n_s_copy_2
 #define __pyx_n_s_cos __pyx_mstate_global->__pyx_n_s_cos
 #define __pyx_n_s_count __pyx_mstate_global->__pyx_n_s_count
@@ -3789,27 +4043,26 @@
 #define __pyx_n_s_edgeEndVertex __pyx_mstate_global->__pyx_n_s_edgeEndVertex
 #define __pyx_n_s_edgeStartVertex __pyx_mstate_global->__pyx_n_s_edgeStartVertex
 #define __pyx_n_s_edges __pyx_mstate_global->__pyx_n_s_edges
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_end __pyx_mstate_global->__pyx_n_s_end
 #define __pyx_n_s_end_point_x __pyx_mstate_global->__pyx_n_s_end_point_x
 #define __pyx_n_s_end_point_y __pyx_mstate_global->__pyx_n_s_end_point_y
+#define __pyx_n_s_float __pyx_mstate_global->__pyx_n_s_float
 #define __pyx_n_s_focus __pyx_mstate_global->__pyx_n_s_focus
 #define __pyx_n_s_focus_rotated __pyx_mstate_global->__pyx_n_s_focus_rotated
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
-#define __pyx_n_s_init __pyx_mstate_global->__pyx_n_s_init
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
-#define __pyx_n_s_inputPoints __pyx_mstate_global->__pyx_n_s_inputPoints
-#define __pyx_n_s_inputSegments __pyx_mstate_global->__pyx_n_s_inputSegments
 #define __pyx_n_s_input_segment __pyx_mstate_global->__pyx_n_s_input_segment
+#define __pyx_n_s_int __pyx_mstate_global->__pyx_n_s_int
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_is_degenerate __pyx_mstate_global->__pyx_n_s_is_degenerate
 #define __pyx_n_s_is_linear __pyx_mstate_global->__pyx_n_s_is_linear
 #define __pyx_n_s_is_open __pyx_mstate_global->__pyx_n_s_is_open
 #define __pyx_n_s_is_primary __pyx_mstate_global->__pyx_n_s_is_primary
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_log_action __pyx_mstate_global->__pyx_n_s_log_action
@@ -3824,17 +4077,15 @@
 #define __pyx_n_s_mro_entries __pyx_mstate_global->__pyx_n_s_mro_entries
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_next __pyx_mstate_global->__pyx_n_s_next
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_non_scaled_point __pyx_mstate_global->__pyx_n_s_non_scaled_point
 #define __pyx_n_s_non_scaled_segment __pyx_mstate_global->__pyx_n_s_non_scaled_segment
 #define __pyx_n_s_output __pyx_mstate_global->__pyx_n_s_output
-#define __pyx_n_s_outputCells __pyx_mstate_global->__pyx_n_s_outputCells
-#define __pyx_n_s_outputEdges __pyx_mstate_global->__pyx_n_s_outputEdges
-#define __pyx_n_s_outputVertices __pyx_mstate_global->__pyx_n_s_outputVertices
+#define __pyx_n_s_p __pyx_mstate_global->__pyx_n_s_p
 #define __pyx_n_s_p0 __pyx_mstate_global->__pyx_n_s_p0
 #define __pyx_n_s_p1 __pyx_mstate_global->__pyx_n_s_p1
 #define __pyx_n_s_parabola_end __pyx_mstate_global->__pyx_n_s_parabola_end
 #define __pyx_n_s_parabola_end_rotated __pyx_mstate_global->__pyx_n_s_parabola_end_rotated
 #define __pyx_n_s_parabola_end_rotated_check __pyx_mstate_global->__pyx_n_s_parabola_end_rotated_check
 #define __pyx_n_s_parabola_equation_tolerance __pyx_mstate_global->__pyx_n_s_parabola_equation_tolerance
 #define __pyx_n_s_parabola_start __pyx_mstate_global->__pyx_n_s_parabola_start
@@ -3853,18 +4104,20 @@
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
 #define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
+#define __pyx_n_s_s __pyx_mstate_global->__pyx_n_s_s
 #define __pyx_n_s_scaling_factor __pyx_mstate_global->__pyx_n_s_scaling_factor
 #define __pyx_n_s_segment __pyx_mstate_global->__pyx_n_s_segment
 #define __pyx_n_s_segmentSite __pyx_mstate_global->__pyx_n_s_segmentSite
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
+#define __pyx_n_s_send __pyx_mstate_global->__pyx_n_s_send
 #define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shift_x __pyx_mstate_global->__pyx_n_s_shift_x
 #define __pyx_n_s_shift_y __pyx_mstate_global->__pyx_n_s_shift_y
 #define __pyx_n_s_sin __pyx_mstate_global->__pyx_n_s_sin
 #define __pyx_n_s_site __pyx_mstate_global->__pyx_n_s_site
@@ -3879,81 +4132,83 @@
 #define __pyx_n_s_struct __pyx_mstate_global->__pyx_n_s_struct
 #define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
 #define __pyx_n_s_sys __pyx_mstate_global->__pyx_n_s_sys
 #define __pyx_n_s_sys_2 __pyx_mstate_global->__pyx_n_s_sys_2
 #define __pyx_n_s_t __pyx_mstate_global->__pyx_n_s_t
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_theta __pyx_mstate_global->__pyx_n_s_theta
+#define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
 #define __pyx_n_s_time __pyx_mstate_global->__pyx_n_s_time
 #define __pyx_n_s_time_2 __pyx_mstate_global->__pyx_n_s_time_2
 #define __pyx_n_s_tolerance __pyx_mstate_global->__pyx_n_s_tolerance
 #define __pyx_n_s_twin __pyx_mstate_global->__pyx_n_s_twin
 #define __pyx_n_s_twinCell __pyx_mstate_global->__pyx_n_s_twinCell
 #define __pyx_n_s_twinEdge __pyx_mstate_global->__pyx_n_s_twinEdge
+#define __pyx_n_s_typing __pyx_mstate_global->__pyx_n_s_typing
+#define __pyx_kp_s_typing_Type_Edge __pyx_mstate_global->__pyx_kp_s_typing_Type_Edge
+#define __pyx_kp_s_typing_Type_Vertex __pyx_mstate_global->__pyx_kp_s_typing_Type_Vertex
 #define __pyx_n_s_unicodedata __pyx_mstate_global->__pyx_n_s_unicodedata
 #define __pyx_n_s_unicodedata_2 __pyx_mstate_global->__pyx_n_s_unicodedata_2
 #define __pyx_n_s_vertices __pyx_mstate_global->__pyx_n_s_vertices
 #define __pyx_n_s_x __pyx_mstate_global->__pyx_n_s_x
-#define __pyx_n_s_y __pyx_mstate_global->__pyx_n_s_y
 #define __pyx_float_0_0 __pyx_mstate_global->__pyx_float_0_0
 #define __pyx_float_0_0001 __pyx_mstate_global->__pyx_float_0_0001
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_2 __pyx_mstate_global->__pyx_int_2
 #define __pyx_int_neg_1 __pyx_mstate_global->__pyx_int_neg_1
-#define __pyx_slice_ __pyx_mstate_global->__pyx_slice_
-#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
-#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
-#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
-#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
-#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
-#define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
-#define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
-#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
+#define __pyx_codeobj_ __pyx_mstate_global->__pyx_codeobj_
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
+#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
+#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
-#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
-#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
-#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
-#define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
-#define __pyx_tuple__30 __pyx_mstate_global->__pyx_tuple__30
-#define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
-#define __pyx_tuple__39 __pyx_mstate_global->__pyx_tuple__39
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
+#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
+#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
+#define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
+#define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
+#define __pyx_tuple__36 __pyx_mstate_global->__pyx_tuple__36
+#define __pyx_tuple__38 __pyx_mstate_global->__pyx_tuple__38
+#define __pyx_tuple__40 __pyx_mstate_global->__pyx_tuple__40
 #define __pyx_tuple__43 __pyx_mstate_global->__pyx_tuple__43
 #define __pyx_tuple__45 __pyx_mstate_global->__pyx_tuple__45
 #define __pyx_tuple__47 __pyx_mstate_global->__pyx_tuple__47
 #define __pyx_tuple__48 __pyx_mstate_global->__pyx_tuple__48
 #define __pyx_tuple__50 __pyx_mstate_global->__pyx_tuple__50
 #define __pyx_tuple__52 __pyx_mstate_global->__pyx_tuple__52
 #define __pyx_tuple__54 __pyx_mstate_global->__pyx_tuple__54
 #define __pyx_tuple__56 __pyx_mstate_global->__pyx_tuple__56
 #define __pyx_tuple__58 __pyx_mstate_global->__pyx_tuple__58
 #define __pyx_tuple__60 __pyx_mstate_global->__pyx_tuple__60
 #define __pyx_tuple__63 __pyx_mstate_global->__pyx_tuple__63
-#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
-#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
-#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
-#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
-#define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
-#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
-#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__2 __pyx_mstate_global->__pyx_codeobj__2
+#define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
+#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
+#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
+#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
+#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
+#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
+#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
 #define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
-#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
-#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
-#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
-#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
-#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
+#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
+#define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
+#define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
+#define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
 #define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
-#define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 #define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
-#define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
 #define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
-#define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
-#define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
+#define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
 #define __pyx_codeobj__41 __pyx_mstate_global->__pyx_codeobj__41
 #define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
 #define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
 #define __pyx_codeobj__46 __pyx_mstate_global->__pyx_codeobj__46
 #define __pyx_codeobj__49 __pyx_mstate_global->__pyx_codeobj__49
 #define __pyx_codeobj__51 __pyx_mstate_global->__pyx_codeobj__51
 #define __pyx_codeobj__53 __pyx_mstate_global->__pyx_codeobj__53
@@ -4110,15 +4365,15 @@
   __Pyx_XDECREF(__pyx_v_o);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":17
+/* "pyvoronoi.pyx":18
  * 
  * SILENT = True
  * def log_action(description):             # <<<<<<<<<<<<<<
  *     if not SILENT:
  *         print(description)
  */
 
@@ -4171,31 +4426,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_description)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "log_action") < 0)) __PYX_ERR(0, 17, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "log_action") < 0)) __PYX_ERR(0, 18, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_description = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("log_action", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 17, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("log_action", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 18, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -4225,49 +4480,49 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("log_action", 1);
 
-  /* "pyvoronoi.pyx":18
+  /* "pyvoronoi.pyx":19
  * SILENT = True
  * def log_action(description):
  *     if not SILENT:             # <<<<<<<<<<<<<<
  *         print(description)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SILENT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SILENT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (!__pyx_t_2);
   if (__pyx_t_3) {
 
-    /* "pyvoronoi.pyx":19
+    /* "pyvoronoi.pyx":20
  * def log_action(description):
  *     if not SILENT:
  *         print(description)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_v_description); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_v_description); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyvoronoi.pyx":18
+    /* "pyvoronoi.pyx":19
  * SILENT = True
  * def log_action(description):
  *     if not SILENT:             # <<<<<<<<<<<<<<
  *         print(description)
  * 
  */
   }
 
-  /* "pyvoronoi.pyx":17
+  /* "pyvoronoi.pyx":18
  * 
  * SILENT = True
  * def log_action(description):             # <<<<<<<<<<<<<<
  *     if not SILENT:
  *         print(description)
  */
 
@@ -4280,725 +4535,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":121
- *     X = 0.0
- *     Y = 0.0
- *     def __init__(self,x,y):             # <<<<<<<<<<<<<<
- *         self.X = x
- *         self.Y = y
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_6Vertex_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_6Vertex_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_6Vertex_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_6Vertex_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_x = 0;
-  PyObject *__pyx_v_y = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[3] = {0,0,0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_x,&__pyx_n_s_y,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 121, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_y)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 121, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 121, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 3)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-    }
-    __pyx_v_self = values[0];
-    __pyx_v_x = values[1];
-    __pyx_v_y = values[2];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 121, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("pyvoronoi.Vertex.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_6Vertex___init__(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_y);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9pyvoronoi_6Vertex___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_y) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__init__", 1);
-
-  /* "pyvoronoi.pyx":122
- *     Y = 0.0
- *     def __init__(self,x,y):
- *         self.X = x             # <<<<<<<<<<<<<<
- *         self.Y = y
- * 
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_X, __pyx_v_x) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":123
- *     def __init__(self,x,y):
- *         self.X = x
- *         self.Y = y             # <<<<<<<<<<<<<<
- * 
- * class Edge:
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_Y, __pyx_v_y) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":121
- *     X = 0.0
- *     Y = 0.0
- *     def __init__(self,x,y):             # <<<<<<<<<<<<<<
- *         self.X = x
- *         self.Y = y
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("pyvoronoi.Vertex.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "pyvoronoi.pyx":133
- *     twin = -1
- * 
- *     def __init__(self, start, end, cell, twin):             # <<<<<<<<<<<<<<
- *         self.start = start
- *         self.end = end
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_4Edge_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_4Edge_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_4Edge_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_4Edge_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_start = 0;
-  PyObject *__pyx_v_end = 0;
-  PyObject *__pyx_v_cell = 0;
-  PyObject *__pyx_v_twin = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[5] = {0,0,0,0,0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_start,&__pyx_n_s_end,&__pyx_n_s_cell,&__pyx_n_s_twin,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 1); __PYX_ERR(0, 133, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 2); __PYX_ERR(0, 133, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cell)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 3); __PYX_ERR(0, 133, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_twin)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 4); __PYX_ERR(0, 133, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 133, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 5)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
-      values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
-    }
-    __pyx_v_self = values[0];
-    __pyx_v_start = values[1];
-    __pyx_v_end = values[2];
-    __pyx_v_cell = values[3];
-    __pyx_v_twin = values[4];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 133, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("pyvoronoi.Edge.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_4Edge___init__(__pyx_self, __pyx_v_self, __pyx_v_start, __pyx_v_end, __pyx_v_cell, __pyx_v_twin);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9pyvoronoi_4Edge___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_start, PyObject *__pyx_v_end, PyObject *__pyx_v_cell, PyObject *__pyx_v_twin) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__init__", 1);
-
-  /* "pyvoronoi.pyx":134
- * 
- *     def __init__(self, start, end, cell, twin):
- *         self.start = start             # <<<<<<<<<<<<<<
- *         self.end = end
- *         self.cell = cell
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_start, __pyx_v_start) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":135
- *     def __init__(self, start, end, cell, twin):
- *         self.start = start
- *         self.end = end             # <<<<<<<<<<<<<<
- *         self.cell = cell
- *         self.twin = twin
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_end, __pyx_v_end) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":136
- *         self.start = start
- *         self.end = end
- *         self.cell = cell             # <<<<<<<<<<<<<<
- *         self.twin = twin
- * 
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cell, __pyx_v_cell) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":137
- *         self.end = end
- *         self.cell = cell
- *         self.twin = twin             # <<<<<<<<<<<<<<
- * 
- * class Cell:
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_twin, __pyx_v_twin) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":133
- *     twin = -1
- * 
- *     def __init__(self, start, end, cell, twin):             # <<<<<<<<<<<<<<
- *         self.start = start
- *         self.end = end
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("pyvoronoi.Edge.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "pyvoronoi.pyx":151
- *     source_category = None
- * 
- *     def __init__(self, cell_identifier, site, vertices, edges, source_category):             # <<<<<<<<<<<<<<
- *         self.cell_identifier = cell_identifier
- *         self.site = site
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_4Cell_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_4Cell_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_4Cell_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_4Cell_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_cell_identifier = 0;
-  PyObject *__pyx_v_site = 0;
-  PyObject *__pyx_v_vertices = 0;
-  PyObject *__pyx_v_edges = 0;
-  PyObject *__pyx_v_source_category = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[6] = {0,0,0,0,0,0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_cell_identifier,&__pyx_n_s_site,&__pyx_n_s_vertices,&__pyx_n_s_edges,&__pyx_n_s_source_category,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
-        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cell_identifier)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 1); __PYX_ERR(0, 151, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_site)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 2); __PYX_ERR(0, 151, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vertices)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 3); __PYX_ERR(0, 151, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_edges)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 4); __PYX_ERR(0, 151, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  5:
-        if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_source_category)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 5); __PYX_ERR(0, 151, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 151, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 6)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
-      values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
-      values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
-    }
-    __pyx_v_self = values[0];
-    __pyx_v_cell_identifier = values[1];
-    __pyx_v_site = values[2];
-    __pyx_v_vertices = values[3];
-    __pyx_v_edges = values[4];
-    __pyx_v_source_category = values[5];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, __pyx_nargs); __PYX_ERR(0, 151, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("pyvoronoi.Cell.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_4Cell___init__(__pyx_self, __pyx_v_self, __pyx_v_cell_identifier, __pyx_v_site, __pyx_v_vertices, __pyx_v_edges, __pyx_v_source_category);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9pyvoronoi_4Cell___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_cell_identifier, PyObject *__pyx_v_site, PyObject *__pyx_v_vertices, PyObject *__pyx_v_edges, PyObject *__pyx_v_source_category) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  int __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__init__", 1);
-
-  /* "pyvoronoi.pyx":152
- * 
- *     def __init__(self, cell_identifier, site, vertices, edges, source_category):
- *         self.cell_identifier = cell_identifier             # <<<<<<<<<<<<<<
- *         self.site = site
- *         self.source_category = source_category
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cell_identifier, __pyx_v_cell_identifier) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":153
- *     def __init__(self, cell_identifier, site, vertices, edges, source_category):
- *         self.cell_identifier = cell_identifier
- *         self.site = site             # <<<<<<<<<<<<<<
- *         self.source_category = source_category
- *         self.vertices = vertices
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_site, __pyx_v_site) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":154
- *         self.cell_identifier = cell_identifier
- *         self.site = site
- *         self.source_category = source_category             # <<<<<<<<<<<<<<
- *         self.vertices = vertices
- *         self.edges = edges
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_source_category, __pyx_v_source_category) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":155
- *         self.site = site
- *         self.source_category = source_category
- *         self.vertices = vertices             # <<<<<<<<<<<<<<
- *         self.edges = edges
- *         if len(self.vertices) > 0:
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vertices, __pyx_v_vertices) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":156
- *         self.source_category = source_category
- *         self.vertices = vertices
- *         self.edges = edges             # <<<<<<<<<<<<<<
- *         if len(self.vertices) > 0:
- *             self.vertices.append(self.vertices[0])
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_edges, __pyx_v_edges) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":157
- *         self.vertices = vertices
- *         self.edges = edges
- *         if len(self.vertices) > 0:             # <<<<<<<<<<<<<<
- *             self.vertices.append(self.vertices[0])
- * 
- */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_vertices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 157, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__pyx_t_2 > 0);
-  if (__pyx_t_3) {
-
-    /* "pyvoronoi.pyx":158
- *         self.edges = edges
- *         if len(self.vertices) > 0:
- *             self.vertices.append(self.vertices[0])             # <<<<<<<<<<<<<<
- * 
- * 
- */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_vertices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_vertices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 158, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Append(__pyx_t_1, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 158, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-    /* "pyvoronoi.pyx":157
- *         self.vertices = vertices
- *         self.edges = edges
- *         if len(self.vertices) > 0:             # <<<<<<<<<<<<<<
- *             self.vertices.append(self.vertices[0])
- * 
- */
-  }
-
-  /* "pyvoronoi.pyx":151
- *     source_category = None
- * 
- *     def __init__(self, cell_identifier, site, vertices, edges, source_category):             # <<<<<<<<<<<<<<
- *         self.cell_identifier = cell_identifier
- *         self.site = site
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("pyvoronoi.Cell.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "pyvoronoi.pyx":173
+/* "pyvoronoi.pyx":159
  * ##ROTATION
  * ####################################
  * def Rotate(point, theta):             # <<<<<<<<<<<<<<
  *     t = -1 * theta
  *     cos = math.cos(t)
  */
 
@@ -5054,43 +4599,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_theta)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Rotate", 1, 2, 2, 1); __PYX_ERR(0, 173, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Rotate", 1, 2, 2, 1); __PYX_ERR(0, 159, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Rotate") < 0)) __PYX_ERR(0, 173, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Rotate") < 0)) __PYX_ERR(0, 159, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_point = values[0];
     __pyx_v_theta = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Rotate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 173, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Rotate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 159, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5125,36 +4670,36 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Rotate", 1);
 
-  /* "pyvoronoi.pyx":174
+  /* "pyvoronoi.pyx":160
  * ####################################
  * def Rotate(point, theta):
  *     t = -1 * theta             # <<<<<<<<<<<<<<
  *     cos = math.cos(t)
  *     sin = math.sin(t)
  */
-  __pyx_t_1 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_1, __pyx_v_theta, -1L, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_1, __pyx_v_theta, -1L, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_t = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":175
+  /* "pyvoronoi.pyx":161
  * def Rotate(point, theta):
  *     t = -1 * theta
  *     cos = math.cos(t)             # <<<<<<<<<<<<<<
  *     sin = math.sin(t)
  *     return [(point[0] * cos) - (point[1] * sin),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_cos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_cos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5167,31 +4712,31 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_t};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_cos = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":176
+  /* "pyvoronoi.pyx":162
  *     t = -1 * theta
  *     cos = math.cos(t)
  *     sin = math.sin(t)             # <<<<<<<<<<<<<<
  *     return [(point[0] * cos) - (point[1] * sin),
  * 	(point[0] * sin) + (point[1] * cos)]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -5204,86 +4749,86 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_t};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_sin = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":177
+  /* "pyvoronoi.pyx":163
  *     cos = math.cos(t)
  *     sin = math.sin(t)
  *     return [(point[0] * cos) - (point[1] * sin),             # <<<<<<<<<<<<<<
  * 	(point[0] * sin) + (point[1] * cos)]
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_v_cos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_v_cos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_v_sin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_v_sin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":178
+  /* "pyvoronoi.pyx":164
  *     sin = math.sin(t)
  *     return [(point[0] * cos) - (point[1] * sin),
  * 	(point[0] * sin) + (point[1] * cos)]             # <<<<<<<<<<<<<<
  * 
  * def RotateWithShift(point, theta, shift_x, shift_y):
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_v_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_v_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyNumber_Multiply(__pyx_t_3, __pyx_v_cos); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Multiply(__pyx_t_3, __pyx_v_cos); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":177
+  /* "pyvoronoi.pyx":163
  *     cos = math.cos(t)
  *     sin = math.sin(t)
  *     return [(point[0] * cos) - (point[1] * sin),             # <<<<<<<<<<<<<<
  * 	(point[0] * sin) + (point[1] * cos)]
  * 
  */
-  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":173
+  /* "pyvoronoi.pyx":159
  * ##ROTATION
  * ####################################
  * def Rotate(point, theta):             # <<<<<<<<<<<<<<
  *     t = -1 * theta
  *     cos = math.cos(t)
  */
 
@@ -5300,15 +4845,15 @@
   __Pyx_XDECREF(__pyx_v_cos);
   __Pyx_XDECREF(__pyx_v_sin);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":180
+/* "pyvoronoi.pyx":166
  * 	(point[0] * sin) + (point[1] * cos)]
  * 
  * def RotateWithShift(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  */
 
@@ -5370,50 +4915,50 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_theta)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, 1); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, 1); __PYX_ERR(0, 166, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shift_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, 2); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, 2); __PYX_ERR(0, 166, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shift_y)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, 3); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, 3); __PYX_ERR(0, 166, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RotateWithShift") < 0)) __PYX_ERR(0, 180, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RotateWithShift") < 0)) __PYX_ERR(0, 166, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -5422,15 +4967,15 @@
     __pyx_v_point = values[0];
     __pyx_v_theta = values[1];
     __pyx_v_shift_x = values[2];
     __pyx_v_shift_y = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 180, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("RotateWithShift", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 166, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5463,40 +5008,40 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("RotateWithShift", 1);
 
-  /* "pyvoronoi.pyx":181
+  /* "pyvoronoi.pyx":167
  * 
  * def RotateWithShift(point, theta, shift_x, shift_y):
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)             # <<<<<<<<<<<<<<
  * 
  * def Unrotate(point, theta, shift_x, shift_y):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Rotate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Rotate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_v_shift_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_v_shift_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyNumber_Subtract(__pyx_t_3, __pyx_v_shift_y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Subtract(__pyx_t_3, __pyx_v_shift_y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
@@ -5510,23 +5055,23 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_t_3, __pyx_v_theta};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":180
+  /* "pyvoronoi.pyx":166
  * 	(point[0] * sin) + (point[1] * cos)]
  * 
  * def RotateWithShift(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  */
 
@@ -5541,15 +5086,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":183
+/* "pyvoronoi.pyx":169
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  * def Unrotate(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     cos = math.cos(theta)
  *     sin = math.sin(theta)
  */
 
@@ -5611,50 +5156,50 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_theta)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, 1); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, 1); __PYX_ERR(0, 169, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shift_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, 2); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, 2); __PYX_ERR(0, 169, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shift_y)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, 3); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, 3); __PYX_ERR(0, 169, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Unrotate") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Unrotate") < 0)) __PYX_ERR(0, 169, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -5663,15 +5208,15 @@
     __pyx_v_point = values[0];
     __pyx_v_theta = values[1];
     __pyx_v_shift_x = values[2];
     __pyx_v_shift_y = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 183, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Unrotate", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 169, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5705,24 +5250,24 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Unrotate", 1);
 
-  /* "pyvoronoi.pyx":184
+  /* "pyvoronoi.pyx":170
  * 
  * def Unrotate(point, theta, shift_x, shift_y):
  *     cos = math.cos(theta)             # <<<<<<<<<<<<<<
  *     sin = math.sin(theta)
  *     return [(point[0] * cos) - (point[1] * sin) + shift_x, (point[0] * sin) + (point[1] * cos) + shift_y]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_cos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_cos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5735,31 +5280,31 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_theta};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_cos = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":185
+  /* "pyvoronoi.pyx":171
  * def Unrotate(point, theta, shift_x, shift_y):
  *     cos = math.cos(theta)
  *     sin = math.sin(theta)             # <<<<<<<<<<<<<<
  *     return [(point[0] * cos) - (point[1] * sin) + shift_x, (point[0] * sin) + (point[1] * cos) + shift_y]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -5772,76 +5317,76 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_theta};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_sin = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":186
+  /* "pyvoronoi.pyx":172
  *     cos = math.cos(theta)
  *     sin = math.sin(theta)
  *     return [(point[0] * cos) - (point[1] * sin) + shift_x, (point[0] * sin) + (point[1] * cos) + shift_y]             # <<<<<<<<<<<<<<
  * 
  * def GetLineAngleInRadians(start_point_x, start_point_y,end_point_x, end_point_y):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_v_cos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_v_cos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_v_sin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_v_sin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_v_shift_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_v_shift_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_v_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_v_sin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = PyNumber_Multiply(__pyx_t_1, __pyx_v_cos); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Multiply(__pyx_t_1, __pyx_v_cos); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_Add(__pyx_t_1, __pyx_v_shift_y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Add(__pyx_t_1, __pyx_v_shift_y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_5)) __PYX_ERR(0, 172, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_5 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":183
+  /* "pyvoronoi.pyx":169
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  * def Unrotate(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     cos = math.cos(theta)
  *     sin = math.sin(theta)
  */
 
@@ -5857,15 +5402,15 @@
   __Pyx_XDECREF(__pyx_v_cos);
   __Pyx_XDECREF(__pyx_v_sin);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":188
+/* "pyvoronoi.pyx":174
  *     return [(point[0] * cos) - (point[1] * sin) + shift_x, (point[0] * sin) + (point[1] * cos) + shift_y]
  * 
  * def GetLineAngleInRadians(start_point_x, start_point_y,end_point_x, end_point_y):             # <<<<<<<<<<<<<<
  *     return math.atan2(end_point_y - start_point_y, end_point_x - start_point_x)
  * 
  */
 
@@ -5927,50 +5472,50 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start_point_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start_point_y)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, 1); __PYX_ERR(0, 188, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, 1); __PYX_ERR(0, 174, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end_point_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, 2); __PYX_ERR(0, 188, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, 2); __PYX_ERR(0, 174, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end_point_y)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, 3); __PYX_ERR(0, 188, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, 3); __PYX_ERR(0, 174, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetLineAngleInRadians") < 0)) __PYX_ERR(0, 188, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetLineAngleInRadians") < 0)) __PYX_ERR(0, 174, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -5979,15 +5524,15 @@
     __pyx_v_start_point_x = values[0];
     __pyx_v_start_point_y = values[1];
     __pyx_v_end_point_x = values[2];
     __pyx_v_end_point_y = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 188, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("GetLineAngleInRadians", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 174, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6020,30 +5565,30 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetLineAngleInRadians", 1);
 
-  /* "pyvoronoi.pyx":189
+  /* "pyvoronoi.pyx":175
  * 
  * def GetLineAngleInRadians(start_point_x, start_point_y,end_point_x, end_point_y):
  *     return math.atan2(end_point_y - start_point_y, end_point_x - start_point_x)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_atan2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_atan2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Subtract(__pyx_v_end_point_y, __pyx_v_start_point_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_v_end_point_y, __pyx_v_start_point_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyNumber_Subtract(__pyx_v_end_point_x, __pyx_v_start_point_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_v_end_point_x, __pyx_v_start_point_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -6057,23 +5602,23 @@
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_t_2, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":188
+  /* "pyvoronoi.pyx":174
  *     return [(point[0] * cos) - (point[1] * sin) + shift_x, (point[0] * sin) + (point[1] * cos) + shift_y]
  * 
  * def GetLineAngleInRadians(start_point_x, start_point_y,end_point_x, end_point_y):             # <<<<<<<<<<<<<<
  *     return math.atan2(end_point_y - start_point_y, end_point_x - start_point_x)
  * 
  */
 
@@ -6088,15 +5633,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":195
+/* "pyvoronoi.pyx":181
  * ##DISTANCE
  * ####################################
  * def DistanceSquared(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the squared length of the line.
  *     :return: a float representing the squared length of the line.
  */
 
@@ -6153,43 +5698,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point_start)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point_end)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("DistanceSquared", 1, 2, 2, 1); __PYX_ERR(0, 195, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("DistanceSquared", 1, 2, 2, 1); __PYX_ERR(0, 181, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "DistanceSquared") < 0)) __PYX_ERR(0, 195, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "DistanceSquared") < 0)) __PYX_ERR(0, 181, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_point_start = values[0];
     __pyx_v_point_end = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("DistanceSquared", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 195, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("DistanceSquared", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 181, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6220,53 +5765,53 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("DistanceSquared", 1);
 
-  /* "pyvoronoi.pyx":199
+  /* "pyvoronoi.pyx":185
  *     :return: a float representing the squared length of the line.
  *     """
  *     return pow(point_end[0] - point_start[0], 2) + pow(point_end[1] - point_start[1], 2)             # <<<<<<<<<<<<<<
  * 
  * def Distance(point_start, point_end):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point_end, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point_end, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_point_start, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_point_start, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyNumber_Power2(__pyx_t_3, __pyx_int_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Power2(__pyx_t_3, __pyx_int_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point_end, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point_end, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point_start, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_point_start, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Power2(__pyx_t_4, __pyx_int_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Power2(__pyx_t_4, __pyx_int_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":195
+  /* "pyvoronoi.pyx":181
  * ##DISTANCE
  * ####################################
  * def DistanceSquared(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the squared length of the line.
  *     :return: a float representing the squared length of the line.
  */
 
@@ -6280,15 +5825,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":201
+/* "pyvoronoi.pyx":187
  *     return pow(point_end[0] - point_start[0], 2) + pow(point_end[1] - point_start[1], 2)
  * 
  * def Distance(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the length of the line"""
  *     return math.sqrt(DistanceSquared(point_start, point_end))
  */
 
@@ -6345,43 +5890,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point_start)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point_end)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Distance", 1, 2, 2, 1); __PYX_ERR(0, 201, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Distance", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Distance") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Distance") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_point_start = values[0];
     __pyx_v_point_end = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Distance", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 201, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Distance", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6414,28 +5959,28 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Distance", 1);
 
-  /* "pyvoronoi.pyx":203
+  /* "pyvoronoi.pyx":189
  * def Distance(point_start, point_end):
  *     """Returns the length of the line"""
  *     return math.sqrt(DistanceSquared(point_start, point_end))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_math); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DistanceSquared); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DistanceSquared); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
@@ -6447,15 +5992,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_v_point_start, __pyx_v_point_end};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
@@ -6470,23 +6015,23 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":201
+  /* "pyvoronoi.pyx":187
  *     return pow(point_end[0] - point_start[0], 2) + pow(point_end[1] - point_start[1], 2)
  * 
  * def Distance(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the length of the line"""
  *     return math.sqrt(DistanceSquared(point_start, point_end))
  */
 
@@ -6501,18 +6046,18 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":222
+/* "pyvoronoi.pyx":201
  *     cdef public int SCALING_FACTOR
  * 
- *     def __cinit__(self, scaling_factor = None):             # <<<<<<<<<<<<<<
+ *     def __cinit__(self, scaling_factor = 1):             # <<<<<<<<<<<<<<
  *         """ Creates an instance of the Pyvoronoi class.
  *         """
  */
 
 /* Python wrapper */
 static int __pyx_pw_9pyvoronoi_9Pyvoronoi_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_9pyvoronoi_9Pyvoronoi_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -6530,49 +6075,49 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_scaling_factor,0};
-    values[0] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)Py_None));
+    values[0] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)__pyx_int_1));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_scaling_factor);
           if (value) { values[0] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 222, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_scaling_factor = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 222, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
@@ -6599,27 +6144,28 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 1);
 
-  /* "pyvoronoi.pyx":225
+  /* "pyvoronoi.pyx":204
  *         """ Creates an instance of the Pyvoronoi class.
  *         """
  *         log_action("Creating an VoronoiDiagram instance")             # <<<<<<<<<<<<<<
+ * 
  *         self.thisptr = new VoronoiDiagram()
- *         self.constructed = 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -6631,110 +6177,58 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_s_Creating_an_VoronoiDiagram_insta};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":226
- *         """
+  /* "pyvoronoi.pyx":206
  *         log_action("Creating an VoronoiDiagram instance")
+ * 
  *         self.thisptr = new VoronoiDiagram()             # <<<<<<<<<<<<<<
  *         self.constructed = 0
- * 
+ *         self.SCALING_FACTOR = scaling_factor if scaling_factor is not None else 1
  */
   __pyx_v_self->thisptr = new VoronoiDiagram();
 
-  /* "pyvoronoi.pyx":227
- *         log_action("Creating an VoronoiDiagram instance")
+  /* "pyvoronoi.pyx":207
+ * 
  *         self.thisptr = new VoronoiDiagram()
  *         self.constructed = 0             # <<<<<<<<<<<<<<
+ *         self.SCALING_FACTOR = scaling_factor if scaling_factor is not None else 1
  * 
- *         if scaling_factor != None:
  */
   __pyx_v_self->constructed = 0;
 
-  /* "pyvoronoi.pyx":229
+  /* "pyvoronoi.pyx":208
+ *         self.thisptr = new VoronoiDiagram()
  *         self.constructed = 0
+ *         self.SCALING_FACTOR = scaling_factor if scaling_factor is not None else 1             # <<<<<<<<<<<<<<
  * 
- *         if scaling_factor != None:             # <<<<<<<<<<<<<<
- *             self.SCALING_FACTOR = scaling_factor
- *         else:
+ *     def __dealloc__(self):
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_scaling_factor, Py_None, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 229, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_5 = (__pyx_v_scaling_factor != Py_None);
   if (__pyx_t_5) {
-
-    /* "pyvoronoi.pyx":230
- * 
- *         if scaling_factor != None:
- *             self.SCALING_FACTOR = scaling_factor             # <<<<<<<<<<<<<<
- *         else:
- *             self.SCALING_FACTOR = 1
- */
-    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_v_scaling_factor); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L1_error)
-    __pyx_v_self->SCALING_FACTOR = __pyx_t_4;
-
-    /* "pyvoronoi.pyx":229
- *         self.constructed = 0
- * 
- *         if scaling_factor != None:             # <<<<<<<<<<<<<<
- *             self.SCALING_FACTOR = scaling_factor
- *         else:
- */
-    goto __pyx_L3;
-  }
-
-  /* "pyvoronoi.pyx":232
- *             self.SCALING_FACTOR = scaling_factor
- *         else:
- *             self.SCALING_FACTOR = 1             # <<<<<<<<<<<<<<
- * 
- *         del self.inputPoints[:]
- */
-  /*else*/ {
-    __pyx_v_self->SCALING_FACTOR = 1;
+    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_scaling_factor); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_4 = __pyx_t_6;
+  } else {
+    __pyx_t_4 = 1;
   }
-  __pyx_L3:;
+  __pyx_v_self->SCALING_FACTOR = __pyx_t_4;
 
-  /* "pyvoronoi.pyx":234
- *             self.SCALING_FACTOR = 1
- * 
- *         del self.inputPoints[:]             # <<<<<<<<<<<<<<
- *         del self.inputSegments[:]
- * 
- */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputPoints); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_DelSlice(__pyx_t_1, 0, 0, NULL, NULL, &__pyx_slice_, 0, 0, 1) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "pyvoronoi.pyx":235
- * 
- *         del self.inputPoints[:]
- *         del self.inputSegments[:]             # <<<<<<<<<<<<<<
- * 
- *     def __dealloc__(self):
- */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputSegments); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_DelSlice(__pyx_t_1, 0, 0, NULL, NULL, &__pyx_slice_, 0, 0, 1) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "pyvoronoi.pyx":222
+  /* "pyvoronoi.pyx":201
  *     cdef public int SCALING_FACTOR
  * 
- *     def __cinit__(self, scaling_factor = None):             # <<<<<<<<<<<<<<
+ *     def __cinit__(self, scaling_factor = 1):             # <<<<<<<<<<<<<<
  *         """ Creates an instance of the Pyvoronoi class.
  *         """
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -6745,16 +6239,16 @@
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":237
- *         del self.inputSegments[:]
+/* "pyvoronoi.pyx":210
+ *         self.SCALING_FACTOR = scaling_factor if scaling_factor is not None else 1
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         log_action("Deleting the VoronoiDiagram instance")
  *         del self.thisptr
  */
 
 /* Python wrapper */
@@ -6777,22 +6271,22 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 1);
 
-  /* "pyvoronoi.pyx":238
+  /* "pyvoronoi.pyx":211
  * 
  *     def __dealloc__(self):
  *         log_action("Deleting the VoronoiDiagram instance")             # <<<<<<<<<<<<<<
  *         del self.thisptr
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -6804,31 +6298,31 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_s_Deleting_the_VoronoiDiagram_inst};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":239
+  /* "pyvoronoi.pyx":212
  *     def __dealloc__(self):
  *         log_action("Deleting the VoronoiDiagram instance")
  *         del self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def AddPoint(self, point):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "pyvoronoi.pyx":237
- *         del self.inputSegments[:]
+  /* "pyvoronoi.pyx":210
+ *         self.SCALING_FACTOR = scaling_factor if scaling_factor is not None else 1
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         log_action("Deleting the VoronoiDiagram instance")
  *         del self.thisptr
  */
 
   /* function exit code */
@@ -6838,15 +6332,15 @@
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_WriteUnraisable("pyvoronoi.Pyvoronoi.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "pyvoronoi.pyx":241
+/* "pyvoronoi.pyx":214
  *         del self.thisptr
  * 
  *     def AddPoint(self, point):             # <<<<<<<<<<<<<<
  *         """ Add a point
  *         """
  */
 
@@ -6900,31 +6394,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "AddPoint") < 0)) __PYX_ERR(0, 241, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "AddPoint") < 0)) __PYX_ERR(0, 214, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_point = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("AddPoint", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 241, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("AddPoint", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 214, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6953,39 +6447,37 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   struct Point __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("AddPoint", 1);
 
-  /* "pyvoronoi.pyx":245
+  /* "pyvoronoi.pyx":218
  *         """
  * 
  *         if self.constructed == 1:             # <<<<<<<<<<<<<<
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')
  * 
  */
   __pyx_t_1 = (__pyx_v_self->constructed == 1);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyvoronoi.pyx":246
+    /* "pyvoronoi.pyx":219
  * 
  *         if self.constructed == 1:
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')             # <<<<<<<<<<<<<<
  * 
  *         cdef Point c_point = self._to_voronoi_point(point)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VoronoiException); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VoronoiException); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -6997,101 +6489,75 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_s_Construct_has_been_called_can_t};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 246, __pyx_L1_error)
+    __PYX_ERR(0, 219, __pyx_L1_error)
 
-    /* "pyvoronoi.pyx":245
+    /* "pyvoronoi.pyx":218
  *         """
  * 
  *         if self.constructed == 1:             # <<<<<<<<<<<<<<
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')
  * 
  */
   }
 
-  /* "pyvoronoi.pyx":248
+  /* "pyvoronoi.pyx":221
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')
  * 
  *         cdef Point c_point = self._to_voronoi_point(point)             # <<<<<<<<<<<<<<
  *         self.thisptr.AddPoint(c_point)
- *         self.inputPoints.append([c_point.X, c_point.Y])
+ * 
  */
-  __pyx_t_6 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_point(__pyx_v_self, __pyx_v_point); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_point(__pyx_v_self, __pyx_v_point); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L1_error)
   __pyx_v_c_point = __pyx_t_6;
 
-  /* "pyvoronoi.pyx":249
+  /* "pyvoronoi.pyx":222
  * 
  *         cdef Point c_point = self._to_voronoi_point(point)
  *         self.thisptr.AddPoint(c_point)             # <<<<<<<<<<<<<<
- *         self.inputPoints.append([c_point.X, c_point.Y])
- * 
- */
-  __pyx_v_self->thisptr->AddPoint(__pyx_v_c_point);
-
-  /* "pyvoronoi.pyx":250
- *         cdef Point c_point = self._to_voronoi_point(point)
- *         self.thisptr.AddPoint(c_point)
- *         self.inputPoints.append([c_point.X, c_point.Y])             # <<<<<<<<<<<<<<
  * 
  *     def AddSegment(self, segment):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputPoints); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_c_point.X); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_c_point.Y); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error);
-  __pyx_t_3 = 0;
-  __pyx_t_4 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_2, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_v_self->thisptr->AddPoint(__pyx_v_c_point);
 
-  /* "pyvoronoi.pyx":241
+  /* "pyvoronoi.pyx":214
  *         del self.thisptr
  * 
  *     def AddPoint(self, point):             # <<<<<<<<<<<<<<
  *         """ Add a point
  *         """
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.AddPoint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":252
- *         self.inputPoints.append([c_point.X, c_point.Y])
+/* "pyvoronoi.pyx":224
+ *         self.thisptr.AddPoint(c_point)
  * 
  *     def AddSegment(self, segment):             # <<<<<<<<<<<<<<
  *         """ Add a segment
  *         """
  */
 
 /* Python wrapper */
@@ -7144,31 +6610,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_segment)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "AddSegment") < 0)) __PYX_ERR(0, 252, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "AddSegment") < 0)) __PYX_ERR(0, 224, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_segment = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("AddSegment", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 252, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("AddSegment", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 224, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -7197,40 +6663,37 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   struct Segment __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("AddSegment", 1);
 
-  /* "pyvoronoi.pyx":256
+  /* "pyvoronoi.pyx":228
  *         """
  * 
  *         if self.constructed == 1:             # <<<<<<<<<<<<<<
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')
  * 
  */
   __pyx_t_1 = (__pyx_v_self->constructed == 1);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyvoronoi.pyx":257
+    /* "pyvoronoi.pyx":229
  * 
  *         if self.constructed == 1:
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')             # <<<<<<<<<<<<<<
  * 
  *         cdef Segment c_segment = self._to_voronoi_segment(segment)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VoronoiException); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VoronoiException); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -7242,122 +6705,75 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_s_Construct_has_been_called_can_t};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 257, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 257, __pyx_L1_error)
+    __PYX_ERR(0, 229, __pyx_L1_error)
 
-    /* "pyvoronoi.pyx":256
+    /* "pyvoronoi.pyx":228
  *         """
  * 
  *         if self.constructed == 1:             # <<<<<<<<<<<<<<
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')
  * 
  */
   }
 
-  /* "pyvoronoi.pyx":259
+  /* "pyvoronoi.pyx":231
  *             raise VoronoiException('Construct() has been called, can\'t add more elements')
  * 
  *         cdef Segment c_segment = self._to_voronoi_segment(segment)             # <<<<<<<<<<<<<<
  *         self.thisptr.AddSegment(c_segment)
- *         self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])
+ * 
  */
-  __pyx_t_6 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_segment(__pyx_v_self, __pyx_v_segment); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_segment(__pyx_v_self, __pyx_v_segment); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L1_error)
   __pyx_v_c_segment = __pyx_t_6;
 
-  /* "pyvoronoi.pyx":260
+  /* "pyvoronoi.pyx":232
  * 
  *         cdef Segment c_segment = self._to_voronoi_segment(segment)
  *         self.thisptr.AddSegment(c_segment)             # <<<<<<<<<<<<<<
- *         self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])
- * 
- */
-  __pyx_v_self->thisptr->AddSegment(__pyx_v_c_segment);
-
-  /* "pyvoronoi.pyx":261
- *         cdef Segment c_segment = self._to_voronoi_segment(segment)
- *         self.thisptr.AddSegment(c_segment)
- *         self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])             # <<<<<<<<<<<<<<
  * 
  *     def Construct(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputSegments); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_c_segment.p0.X); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_c_segment.p0.Y); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error);
-  __pyx_t_3 = 0;
-  __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_c_segment.p1.X); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_c_segment.p1.Y); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error);
-  __pyx_t_4 = 0;
-  __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_7)) __PYX_ERR(0, 261, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_8);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_8)) __PYX_ERR(0, 261, __pyx_L1_error);
-  __pyx_t_7 = 0;
-  __pyx_t_8 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Append(__pyx_t_2, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 261, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_self->thisptr->AddSegment(__pyx_v_c_segment);
 
-  /* "pyvoronoi.pyx":252
- *         self.inputPoints.append([c_point.X, c_point.Y])
+  /* "pyvoronoi.pyx":224
+ *         self.thisptr.AddPoint(c_point)
  * 
  *     def AddSegment(self, segment):             # <<<<<<<<<<<<<<
  *         """ Add a segment
  *         """
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.AddSegment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":263
- *         self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])
+/* "pyvoronoi.pyx":234
+ *         self.thisptr.AddSegment(c_segment)
  * 
  *     def Construct(self):             # <<<<<<<<<<<<<<
  *         """ Generates the voronoi diagram for the added points and segments. Voronoi cell structure will be generated.
  *         """
  */
 
 /* Python wrapper */
@@ -7411,32 +6827,32 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Construct", 1);
 
-  /* "pyvoronoi.pyx":267
+  /* "pyvoronoi.pyx":238
  *         """
  * 
  *         if self.constructed == 1:             # <<<<<<<<<<<<<<
  *             raise VoronoiException('Construct() has already been called')
  * 
  */
   __pyx_t_1 = (__pyx_v_self->constructed == 1);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyvoronoi.pyx":268
+    /* "pyvoronoi.pyx":239
  * 
  *         if self.constructed == 1:
  *             raise VoronoiException('Construct() has already been called')             # <<<<<<<<<<<<<<
  * 
  *         self.constructed = 1
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VoronoiException); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VoronoiException); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -7448,78 +6864,78 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_s_Construct_has_already_been_calle};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 268, __pyx_L1_error)
+    __PYX_ERR(0, 239, __pyx_L1_error)
 
-    /* "pyvoronoi.pyx":267
+    /* "pyvoronoi.pyx":238
  *         """
  * 
  *         if self.constructed == 1:             # <<<<<<<<<<<<<<
  *             raise VoronoiException('Construct() has already been called')
  * 
  */
   }
 
-  /* "pyvoronoi.pyx":270
+  /* "pyvoronoi.pyx":241
  *             raise VoronoiException('Construct() has already been called')
  * 
  *         self.constructed = 1             # <<<<<<<<<<<<<<
- * 
  *         self.thisptr.Construct()
+ *         self.thisptr.MapVertexIndexes()
  */
   __pyx_v_self->constructed = 1;
 
-  /* "pyvoronoi.pyx":272
- *         self.constructed = 1
+  /* "pyvoronoi.pyx":242
  * 
+ *         self.constructed = 1
  *         self.thisptr.Construct()             # <<<<<<<<<<<<<<
- * 
  *         self.thisptr.MapVertexIndexes()
+ *         self.thisptr.MapEdgeIndexes()
  */
   __pyx_v_self->thisptr->Construct();
 
-  /* "pyvoronoi.pyx":274
+  /* "pyvoronoi.pyx":243
+ *         self.constructed = 1
  *         self.thisptr.Construct()
- * 
  *         self.thisptr.MapVertexIndexes()             # <<<<<<<<<<<<<<
  *         self.thisptr.MapEdgeIndexes()
  *         self.thisptr.MapCellIndexes()
  */
   __pyx_v_self->thisptr->MapVertexIndexes();
 
-  /* "pyvoronoi.pyx":275
- * 
+  /* "pyvoronoi.pyx":244
+ *         self.thisptr.Construct()
  *         self.thisptr.MapVertexIndexes()
  *         self.thisptr.MapEdgeIndexes()             # <<<<<<<<<<<<<<
  *         self.thisptr.MapCellIndexes()
  * 
  */
   __pyx_v_self->thisptr->MapEdgeIndexes();
 
-  /* "pyvoronoi.pyx":276
+  /* "pyvoronoi.pyx":245
  *         self.thisptr.MapVertexIndexes()
  *         self.thisptr.MapEdgeIndexes()
  *         self.thisptr.MapCellIndexes()             # <<<<<<<<<<<<<<
  * 
  *     def GetVertex(self, index):
  */
   __pyx_v_self->thisptr->MapCellIndexes();
 
-  /* "pyvoronoi.pyx":263
- *         self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])
+  /* "pyvoronoi.pyx":234
+ *         self.thisptr.AddSegment(c_segment)
  * 
  *     def Construct(self):             # <<<<<<<<<<<<<<
  *         """ Generates the voronoi diagram for the added points and segments. Voronoi cell structure will be generated.
  *         """
  */
 
   /* function exit code */
@@ -7533,15 +6949,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":278
+/* "pyvoronoi.pyx":247
  *         self.thisptr.MapCellIndexes()
  * 
  *     def GetVertex(self, index):             # <<<<<<<<<<<<<<
  *         """
  *         """
  */
 
@@ -7595,31 +7011,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 278, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetVertex") < 0)) __PYX_ERR(0, 278, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetVertex") < 0)) __PYX_ERR(0, 247, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_index = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("GetVertex", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 278, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("GetVertex", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 247, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -7646,111 +7062,116 @@
   struct c_Vertex __pyx_v_c_vertex;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PY_LONG_LONG __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetVertex", 1);
 
-  /* "pyvoronoi.pyx":281
+  /* "pyvoronoi.pyx":250
  *         """
  *         """
  *         c_vertex = self.thisptr.GetVertex(index)             # <<<<<<<<<<<<<<
- *         return Vertex(c_vertex.X / self.SCALING_FACTOR, c_vertex.Y / self.SCALING_FACTOR)
- * 
+ *         return Vertex(
+ *             X=c_vertex.X / self.SCALING_FACTOR,
  */
-  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_index); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_index); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
   __pyx_v_c_vertex = __pyx_v_self->thisptr->GetVertex(__pyx_t_1);
 
-  /* "pyvoronoi.pyx":282
+  /* "pyvoronoi.pyx":251
  *         """
  *         c_vertex = self.thisptr.GetVertex(index)
- *         return Vertex(c_vertex.X / self.SCALING_FACTOR, c_vertex.Y / self.SCALING_FACTOR)             # <<<<<<<<<<<<<<
- * 
- *     def GetEdge(self, index):
+ *         return Vertex(             # <<<<<<<<<<<<<<
+ *             X=c_vertex.X / self.SCALING_FACTOR,
+ *             Y=c_vertex.Y / self.SCALING_FACTOR
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Vertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Vertex); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "pyvoronoi.pyx":252
+ *         c_vertex = self.thisptr.GetVertex(index)
+ *         return Vertex(
+ *             X=c_vertex.X / self.SCALING_FACTOR,             # <<<<<<<<<<<<<<
+ *             Y=c_vertex.Y / self.SCALING_FACTOR
+ *         )
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (unlikely(__pyx_v_self->SCALING_FACTOR == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 282, __pyx_L1_error)
+    __PYX_ERR(0, 252, __pyx_L1_error)
   }
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_c_vertex.X / ((double)__pyx_v_self->SCALING_FACTOR))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_c_vertex.X / ((double)__pyx_v_self->SCALING_FACTOR))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_X, __pyx_t_4) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":253
+ *         return Vertex(
+ *             X=c_vertex.X / self.SCALING_FACTOR,
+ *             Y=c_vertex.Y / self.SCALING_FACTOR             # <<<<<<<<<<<<<<
+ *         )
+ * 
+ */
   if (unlikely(__pyx_v_self->SCALING_FACTOR == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 282, __pyx_L1_error)
+    __PYX_ERR(0, 253, __pyx_L1_error)
   }
-  __pyx_t_5 = PyFloat_FromDouble((__pyx_v_c_vertex.Y / ((double)__pyx_v_self->SCALING_FACTOR))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 282, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = NULL;
-  __pyx_t_7 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_6);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_7 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_c_vertex.Y / ((double)__pyx_v_self->SCALING_FACTOR))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_Y, __pyx_t_4) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":251
+ *         """
+ *         c_vertex = self.thisptr.GetVertex(index)
+ *         return Vertex(             # <<<<<<<<<<<<<<
+ *             X=c_vertex.X / self.SCALING_FACTOR,
+ *             Y=c_vertex.Y / self.SCALING_FACTOR
+ */
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_4;
+  __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":278
+  /* "pyvoronoi.pyx":247
  *         self.thisptr.MapCellIndexes()
  * 
  *     def GetVertex(self, index):             # <<<<<<<<<<<<<<
  *         """
  *         """
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.GetVertex", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":284
- *         return Vertex(c_vertex.X / self.SCALING_FACTOR, c_vertex.Y / self.SCALING_FACTOR)
+/* "pyvoronoi.pyx":256
+ *         )
  * 
  *     def GetEdge(self, index):             # <<<<<<<<<<<<<<
  *         c_edge =  self.thisptr.GetEdge(index)
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
+ *         edge = Edge(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_13GetEdge(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -7798,31 +7219,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 256, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetEdge") < 0)) __PYX_ERR(0, 284, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetEdge") < 0)) __PYX_ERR(0, 256, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_index = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("GetEdge", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 284, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("GetEdge", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 256, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -7850,148 +7271,167 @@
   PyObject *__pyx_v_edge = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PY_LONG_LONG __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetEdge", 1);
 
-  /* "pyvoronoi.pyx":285
+  /* "pyvoronoi.pyx":257
  * 
  *     def GetEdge(self, index):
  *         c_edge =  self.thisptr.GetEdge(index)             # <<<<<<<<<<<<<<
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
- *         edge.is_primary = c_edge.isPrimary != False
+ *         edge = Edge(
+ *             start=c_edge.start,
  */
-  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_index); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_index); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 257, __pyx_L1_error)
   __pyx_v_c_edge = __pyx_v_self->thisptr->GetEdge(__pyx_t_1);
 
-  /* "pyvoronoi.pyx":286
+  /* "pyvoronoi.pyx":258
  *     def GetEdge(self, index):
  *         c_edge =  self.thisptr.GetEdge(index)
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)             # <<<<<<<<<<<<<<
- *         edge.is_primary = c_edge.isPrimary != False
- *         edge.is_linear = c_edge.isLinear != False
+ *         edge = Edge(             # <<<<<<<<<<<<<<
+ *             start=c_edge.start,
+ *             end=c_edge.end,
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Edge); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "pyvoronoi.pyx":259
+ *         c_edge =  self.thisptr.GetEdge(index)
+ *         edge = Edge(
+ *             start=c_edge.start,             # <<<<<<<<<<<<<<
+ *             end=c_edge.end,
+ *             cell=c_edge.cell,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Edge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.end); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.cell); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.twin); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = NULL;
-  __pyx_t_9 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_9 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[5] = {__pyx_t_8, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7};
-    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_9, 4+__pyx_t_9);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
-  __pyx_v_edge = __pyx_t_2;
-  __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_start, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":287
- *         c_edge =  self.thisptr.GetEdge(index)
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
- *         edge.is_primary = c_edge.isPrimary != False             # <<<<<<<<<<<<<<
- *         edge.is_linear = c_edge.isLinear != False
- *         return edge
+  /* "pyvoronoi.pyx":260
+ *         edge = Edge(
+ *             start=c_edge.start,
+ *             end=c_edge.end,             # <<<<<<<<<<<<<<
+ *             cell=c_edge.cell,
+ *             twin=c_edge.twin,
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong((__pyx_v_c_edge.isPrimary != 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_edge, __pyx_n_s_is_primary, __pyx_t_2) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_end, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":288
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
- *         edge.is_primary = c_edge.isPrimary != False
- *         edge.is_linear = c_edge.isLinear != False             # <<<<<<<<<<<<<<
+  /* "pyvoronoi.pyx":261
+ *             start=c_edge.start,
+ *             end=c_edge.end,
+ *             cell=c_edge.cell,             # <<<<<<<<<<<<<<
+ *             twin=c_edge.twin,
+ *             is_primary= c_edge.isPrimary != False,
+ */
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.cell); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_cell, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":262
+ *             end=c_edge.end,
+ *             cell=c_edge.cell,
+ *             twin=c_edge.twin,             # <<<<<<<<<<<<<<
+ *             is_primary= c_edge.isPrimary != False,
+ *             is_linear = c_edge.isLinear != False
+ */
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_edge.twin); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_twin, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":263
+ *             cell=c_edge.cell,
+ *             twin=c_edge.twin,
+ *             is_primary= c_edge.isPrimary != False,             # <<<<<<<<<<<<<<
+ *             is_linear = c_edge.isLinear != False
+ *         )
+ */
+  __pyx_t_4 = __Pyx_PyBool_FromLong((__pyx_v_c_edge.isPrimary != 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_is_primary, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":264
+ *             twin=c_edge.twin,
+ *             is_primary= c_edge.isPrimary != False,
+ *             is_linear = c_edge.isLinear != False             # <<<<<<<<<<<<<<
+ *         )
  *         return edge
- * 
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong((__pyx_v_c_edge.isLinear != 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_edge, __pyx_n_s_is_linear, __pyx_t_2) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBool_FromLong((__pyx_v_c_edge.isLinear != 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_is_linear, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":258
+ *     def GetEdge(self, index):
+ *         c_edge =  self.thisptr.GetEdge(index)
+ *         edge = Edge(             # <<<<<<<<<<<<<<
+ *             start=c_edge.start,
+ *             end=c_edge.end,
+ */
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_edge = __pyx_t_4;
+  __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":289
- *         edge.is_primary = c_edge.isPrimary != False
- *         edge.is_linear = c_edge.isLinear != False
+  /* "pyvoronoi.pyx":266
+ *             is_linear = c_edge.isLinear != False
+ *         )
  *         return edge             # <<<<<<<<<<<<<<
  * 
  *     def GetCell(self, index):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_edge);
   __pyx_r = __pyx_v_edge;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":284
- *         return Vertex(c_vertex.X / self.SCALING_FACTOR, c_vertex.Y / self.SCALING_FACTOR)
+  /* "pyvoronoi.pyx":256
+ *         )
  * 
  *     def GetEdge(self, index):             # <<<<<<<<<<<<<<
  *         c_edge =  self.thisptr.GetEdge(index)
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
+ *         edge = Edge(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.GetEdge", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_edge);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":291
+/* "pyvoronoi.pyx":268
  *         return edge
  * 
  *     def GetCell(self, index):             # <<<<<<<<<<<<<<
  *         c_cell = self.thisptr.GetCell(index)
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
+ *         cell = Cell(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_15GetCell(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -8039,31 +7479,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 291, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetCell") < 0)) __PYX_ERR(0, 291, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetCell") < 0)) __PYX_ERR(0, 268, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_index = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("GetCell", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 291, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("GetCell", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 268, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -8091,172 +7531,198 @@
   PyObject *__pyx_v_cell = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PY_LONG_LONG __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetCell", 1);
 
-  /* "pyvoronoi.pyx":292
+  /* "pyvoronoi.pyx":269
  * 
  *     def GetCell(self, index):
  *         c_cell = self.thisptr.GetCell(index)             # <<<<<<<<<<<<<<
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
- *         cell.contains_point = c_cell.contains_point != False
+ *         cell = Cell(
+ *             cell_identifier=c_cell.cell_identifier,
  */
-  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_index); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_index); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L1_error)
   __pyx_v_c_cell = __pyx_v_self->thisptr->GetCell(__pyx_t_1);
 
-  /* "pyvoronoi.pyx":293
+  /* "pyvoronoi.pyx":270
  *     def GetCell(self, index):
  *         c_cell = self.thisptr.GetCell(index)
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)             # <<<<<<<<<<<<<<
- *         cell.contains_point = c_cell.contains_point != False
- *         cell.contains_segment = c_cell.contains_segment != False
+ *         cell = Cell(             # <<<<<<<<<<<<<<
+ *             cell_identifier=c_cell.cell_identifier,
+ *             site=c_cell.site,
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Cell); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "pyvoronoi.pyx":271
+ *         c_cell = self.thisptr.GetCell(index)
+ *         cell = Cell(
+ *             cell_identifier=c_cell.cell_identifier,             # <<<<<<<<<<<<<<
+ *             site=c_cell.site,
+ *             vertices=c_cell.vertices,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Cell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_cell.cell_identifier); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_cell.cell_identifier); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_cell.site); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __pyx_convert_vector_to_py_PY_LONG_LONG(__pyx_v_c_cell.vertices); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __pyx_convert_vector_to_py_PY_LONG_LONG(__pyx_v_c_cell.edges); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_c_cell.source_category); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = NULL;
-  __pyx_t_10 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_9)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_9);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_10 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[6] = {__pyx_t_9, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8};
-    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_10, 5+__pyx_t_10);
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
-  __pyx_v_cell = __pyx_t_2;
-  __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_cell_identifier, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":294
- *         c_cell = self.thisptr.GetCell(index)
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
- *         cell.contains_point = c_cell.contains_point != False             # <<<<<<<<<<<<<<
- *         cell.contains_segment = c_cell.contains_segment != False
- *         cell.is_degenerate = c_cell.is_degenerate != False
+  /* "pyvoronoi.pyx":272
+ *         cell = Cell(
+ *             cell_identifier=c_cell.cell_identifier,
+ *             site=c_cell.site,             # <<<<<<<<<<<<<<
+ *             vertices=c_cell.vertices,
+ *             edges=c_cell.edges,
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.contains_point != 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_cell, __pyx_n_s_contains_point, __pyx_t_2) < 0) __PYX_ERR(0, 294, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_c_cell.site); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_site, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":295
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
- *         cell.contains_point = c_cell.contains_point != False
- *         cell.contains_segment = c_cell.contains_segment != False             # <<<<<<<<<<<<<<
- *         cell.is_degenerate = c_cell.is_degenerate != False
- *         cell.is_open = c_cell.is_open != False
+  /* "pyvoronoi.pyx":273
+ *             cell_identifier=c_cell.cell_identifier,
+ *             site=c_cell.site,
+ *             vertices=c_cell.vertices,             # <<<<<<<<<<<<<<
+ *             edges=c_cell.edges,
+ *             source_category=c_cell.source_category,
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.contains_segment != 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_cell, __pyx_n_s_contains_segment, __pyx_t_2) < 0) __PYX_ERR(0, 295, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __pyx_convert_vector_to_py_PY_LONG_LONG(__pyx_v_c_cell.vertices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vertices, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":296
- *         cell.contains_point = c_cell.contains_point != False
- *         cell.contains_segment = c_cell.contains_segment != False
- *         cell.is_degenerate = c_cell.is_degenerate != False             # <<<<<<<<<<<<<<
- *         cell.is_open = c_cell.is_open != False
- *         return cell
+  /* "pyvoronoi.pyx":274
+ *             site=c_cell.site,
+ *             vertices=c_cell.vertices,
+ *             edges=c_cell.edges,             # <<<<<<<<<<<<<<
+ *             source_category=c_cell.source_category,
+ *             contains_point=c_cell.contains_point != False,
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.is_degenerate != 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_cell, __pyx_n_s_is_degenerate, __pyx_t_2) < 0) __PYX_ERR(0, 296, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __pyx_convert_vector_to_py_PY_LONG_LONG(__pyx_v_c_cell.edges); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_edges, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":297
- *         cell.contains_segment = c_cell.contains_segment != False
- *         cell.is_degenerate = c_cell.is_degenerate != False
- *         cell.is_open = c_cell.is_open != False             # <<<<<<<<<<<<<<
+  /* "pyvoronoi.pyx":275
+ *             vertices=c_cell.vertices,
+ *             edges=c_cell.edges,
+ *             source_category=c_cell.source_category,             # <<<<<<<<<<<<<<
+ *             contains_point=c_cell.contains_point != False,
+ *             contains_segment=c_cell.contains_segment != False,
+ */
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_c_cell.source_category); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_category, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":276
+ *             edges=c_cell.edges,
+ *             source_category=c_cell.source_category,
+ *             contains_point=c_cell.contains_point != False,             # <<<<<<<<<<<<<<
+ *             contains_segment=c_cell.contains_segment != False,
+ *             is_degenerate=c_cell.is_degenerate != False,
+ */
+  __pyx_t_4 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.contains_point != 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_contains_point, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":277
+ *             source_category=c_cell.source_category,
+ *             contains_point=c_cell.contains_point != False,
+ *             contains_segment=c_cell.contains_segment != False,             # <<<<<<<<<<<<<<
+ *             is_degenerate=c_cell.is_degenerate != False,
+ *             is_open = c_cell.is_open != False
+ */
+  __pyx_t_4 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.contains_segment != 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_contains_segment, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":278
+ *             contains_point=c_cell.contains_point != False,
+ *             contains_segment=c_cell.contains_segment != False,
+ *             is_degenerate=c_cell.is_degenerate != False,             # <<<<<<<<<<<<<<
+ *             is_open = c_cell.is_open != False
+ *         )
+ */
+  __pyx_t_4 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.is_degenerate != 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_is_degenerate, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":279
+ *             contains_segment=c_cell.contains_segment != False,
+ *             is_degenerate=c_cell.is_degenerate != False,
+ *             is_open = c_cell.is_open != False             # <<<<<<<<<<<<<<
+ *         )
  *         return cell
- * 
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.is_open != 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_cell, __pyx_n_s_is_open, __pyx_t_2) < 0) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBool_FromLong((__pyx_v_c_cell.is_open != 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_is_open, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "pyvoronoi.pyx":270
+ *     def GetCell(self, index):
+ *         c_cell = self.thisptr.GetCell(index)
+ *         cell = Cell(             # <<<<<<<<<<<<<<
+ *             cell_identifier=c_cell.cell_identifier,
+ *             site=c_cell.site,
+ */
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_cell = __pyx_t_4;
+  __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":298
- *         cell.is_degenerate = c_cell.is_degenerate != False
- *         cell.is_open = c_cell.is_open != False
+  /* "pyvoronoi.pyx":281
+ *             is_open = c_cell.is_open != False
+ *         )
  *         return cell             # <<<<<<<<<<<<<<
  * 
  *     def CountVertices(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_cell);
   __pyx_r = __pyx_v_cell;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":291
+  /* "pyvoronoi.pyx":268
  *         return edge
  * 
  *     def GetCell(self, index):             # <<<<<<<<<<<<<<
  *         c_cell = self.thisptr.GetCell(index)
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
+ *         cell = Cell(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.GetCell", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_cell);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":300
+/* "pyvoronoi.pyx":283
  *         return cell
  * 
  *     def CountVertices(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountVertices()
  * 
  */
 
@@ -8306,29 +7772,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("CountVertices", 1);
 
-  /* "pyvoronoi.pyx":301
+  /* "pyvoronoi.pyx":284
  * 
  *     def CountVertices(self):
  *         return self.thisptr.CountVertices()             # <<<<<<<<<<<<<<
  * 
  *     def CountEdges(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->thisptr->CountVertices()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->thisptr->CountVertices()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":300
+  /* "pyvoronoi.pyx":283
  *         return cell
  * 
  *     def CountVertices(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountVertices()
  * 
  */
 
@@ -8339,15 +7805,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":303
+/* "pyvoronoi.pyx":286
  *         return self.thisptr.CountVertices()
  * 
  *     def CountEdges(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountEdges()
  * 
  */
 
@@ -8397,29 +7863,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("CountEdges", 1);
 
-  /* "pyvoronoi.pyx":304
+  /* "pyvoronoi.pyx":287
  * 
  *     def CountEdges(self):
  *         return self.thisptr.CountEdges()             # <<<<<<<<<<<<<<
  * 
  *     def CountCells(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->thisptr->CountEdges()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->thisptr->CountEdges()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":303
+  /* "pyvoronoi.pyx":286
  *         return self.thisptr.CountVertices()
  * 
  *     def CountEdges(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountEdges()
  * 
  */
 
@@ -8430,15 +7896,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":306
+/* "pyvoronoi.pyx":289
  *         return self.thisptr.CountEdges()
  * 
  *     def CountCells(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountCells()
  * 
  */
 
@@ -8488,29 +7954,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("CountCells", 1);
 
-  /* "pyvoronoi.pyx":307
+  /* "pyvoronoi.pyx":290
  * 
  *     def CountCells(self):
  *         return self.thisptr.CountCells()             # <<<<<<<<<<<<<<
  * 
  *     def GetPoints(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->thisptr->CountCells()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->thisptr->CountCells()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":306
+  /* "pyvoronoi.pyx":289
  *         return self.thisptr.CountEdges()
  * 
  *     def CountCells(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountCells()
  * 
  */
 
@@ -8521,15 +7987,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":309
+/* "pyvoronoi.pyx":292
  *         return self.thisptr.CountCells()
  * 
  *     def GetPoints(self):             # <<<<<<<<<<<<<<
  *         """ Returns the points added to the voronoi diagram
  *         """
  */
 
@@ -8572,57 +8038,91 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_22GetPoints(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+  struct Point __pyx_7genexpr__pyx_v_p;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  std::vector<struct Point> ::iterator __pyx_t_2;
+  std::vector<struct Point>  __pyx_t_3;
+  struct Point __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetPoints", 1);
 
-  /* "pyvoronoi.pyx":312
+  /* "pyvoronoi.pyx":295
  *         """ Returns the points added to the voronoi diagram
  *         """
- *         return self.inputPoints             # <<<<<<<<<<<<<<
+ *         return [[p.X , p.Y ] for p in self.thisptr.GetPoints()]             # <<<<<<<<<<<<<<
+ * 
  * 
- *     def GetSegments(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputPoints); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  { /* enter inner scope */
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __pyx_v_self->thisptr->GetPoints();
+    __pyx_t_2 = __pyx_t_3.begin();
+    for (;;) {
+      if (!(__pyx_t_2 != __pyx_t_3.end())) break;
+      __pyx_t_4 = *__pyx_t_2;
+      ++__pyx_t_2;
+      __pyx_7genexpr__pyx_v_p = __pyx_t_4;
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_7genexpr__pyx_v_p.X); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_7genexpr__pyx_v_p.Y); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GIVEREF(__pyx_t_5);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_5)) __PYX_ERR(0, 295, __pyx_L1_error);
+      __Pyx_GIVEREF(__pyx_t_6);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_6)) __PYX_ERR(0, 295, __pyx_L1_error);
+      __pyx_t_5 = 0;
+      __pyx_t_6 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 295, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    }
+  } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":309
+  /* "pyvoronoi.pyx":292
  *         return self.thisptr.CountCells()
  * 
  *     def GetPoints(self):             # <<<<<<<<<<<<<<
  *         """ Returns the points added to the voronoi diagram
  *         """
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.GetPoints", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":314
- *         return self.inputPoints
+/* "pyvoronoi.pyx":298
+ * 
  * 
  *     def GetSegments(self):             # <<<<<<<<<<<<<<
  *         """ Returns the segments added to the voronoi diagram
  *         """
  */
 
 /* Python wrapper */
@@ -8664,57 +8164,113 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_24GetSegments(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+  struct Segment __pyx_8genexpr1__pyx_v_s;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  std::vector<struct Segment> ::iterator __pyx_t_2;
+  std::vector<struct Segment>  __pyx_t_3;
+  struct Segment __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetSegments", 1);
 
-  /* "pyvoronoi.pyx":317
+  /* "pyvoronoi.pyx":301
  *         """ Returns the segments added to the voronoi diagram
  *         """
- *         return self.inputSegments             # <<<<<<<<<<<<<<
+ *         return [[[s.p0.X, s.p0.Y], [s.p1.X, s.p1.Y]] for s in self.thisptr.GetSegments()]             # <<<<<<<<<<<<<<
  * 
  *     def GetVertices(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputSegments); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  { /* enter inner scope */
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __pyx_v_self->thisptr->GetSegments();
+    __pyx_t_2 = __pyx_t_3.begin();
+    for (;;) {
+      if (!(__pyx_t_2 != __pyx_t_3.end())) break;
+      __pyx_t_4 = *__pyx_t_2;
+      ++__pyx_t_2;
+      __pyx_8genexpr1__pyx_v_s = __pyx_t_4;
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_s.p0.X); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_s.p0.Y); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GIVEREF(__pyx_t_5);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error);
+      __Pyx_GIVEREF(__pyx_t_6);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_6)) __PYX_ERR(0, 301, __pyx_L1_error);
+      __pyx_t_5 = 0;
+      __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_s.p1.X); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_s.p1.Y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_GIVEREF(__pyx_t_6);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_6)) __PYX_ERR(0, 301, __pyx_L1_error);
+      __Pyx_GIVEREF(__pyx_t_5);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error);
+      __pyx_t_6 = 0;
+      __pyx_t_5 = 0;
+      __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_GIVEREF(__pyx_t_7);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error);
+      __Pyx_GIVEREF(__pyx_t_8);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_8)) __PYX_ERR(0, 301, __pyx_L1_error);
+      __pyx_t_7 = 0;
+      __pyx_t_8 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 301, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+  } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":314
- *         return self.inputPoints
+  /* "pyvoronoi.pyx":298
+ * 
  * 
  *     def GetSegments(self):             # <<<<<<<<<<<<<<
  *         """ Returns the segments added to the voronoi diagram
  *         """
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.GetSegments", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":319
- *         return self.inputSegments
+/* "pyvoronoi.pyx":303
+ *         return [[[s.p0.X, s.p0.Y], [s.p1.X, s.p1.Y]] for s in self.thisptr.GetSegments()]
  * 
  *     def GetVertices(self):             # <<<<<<<<<<<<<<
  *         count = self.CountVertices()
  *         output = []
  */
 
 /* Python wrapper */
@@ -8773,22 +8329,22 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetVertices", 1);
 
-  /* "pyvoronoi.pyx":320
+  /* "pyvoronoi.pyx":304
  * 
  *     def GetVertices(self):
  *         count = self.CountVertices()             # <<<<<<<<<<<<<<
  *         output = []
  *         for index in  range(count):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CountVertices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CountVertices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -8800,106 +8356,106 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_count = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":321
+  /* "pyvoronoi.pyx":305
  *     def GetVertices(self):
  *         count = self.CountVertices()
  *         output = []             # <<<<<<<<<<<<<<
  *         for index in  range(count):
  *             output.append(self.GetVertex(index))
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_output = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":322
+  /* "pyvoronoi.pyx":306
  *         count = self.CountVertices()
  *         output = []
  *         for index in  range(count):             # <<<<<<<<<<<<<<
  *             output.append(self.GetVertex(index))
  *         return output
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 306, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 322, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 306, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 322, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 306, __pyx_L1_error)
           #endif
           if (__pyx_t_5 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 322, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 306, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 322, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 306, __pyx_L1_error)
           #endif
           if (__pyx_t_5 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 322, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 306, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_6(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 322, __pyx_L1_error)
+          else __PYX_ERR(0, 306, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pyvoronoi.pyx":323
+    /* "pyvoronoi.pyx":307
  *         output = []
  *         for index in  range(count):
  *             output.append(self.GetVertex(index))             # <<<<<<<<<<<<<<
  *         return output
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetVertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetVertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_7 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
@@ -8911,45 +8467,45 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_v_index};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_output, __pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_output, __pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyvoronoi.pyx":322
+    /* "pyvoronoi.pyx":306
  *         count = self.CountVertices()
  *         output = []
  *         for index in  range(count):             # <<<<<<<<<<<<<<
  *             output.append(self.GetVertex(index))
  *         return output
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":324
+  /* "pyvoronoi.pyx":308
  *         for index in  range(count):
  *             output.append(self.GetVertex(index))
  *         return output             # <<<<<<<<<<<<<<
  * 
- *     def GetEdges(self):
+ *     def IterateVertices(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_output);
   __pyx_r = __pyx_v_output;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":319
- *         return self.inputSegments
+  /* "pyvoronoi.pyx":303
+ *         return [[[s.p0.X, s.p0.Y], [s.p1.X, s.p1.Y]] for s in self.thisptr.GetSegments()]
  * 
  *     def GetVertices(self):             # <<<<<<<<<<<<<<
  *         count = self.CountVertices()
  *         output = []
  */
 
   /* function exit code */
@@ -8964,33 +8520,338 @@
   __Pyx_XDECREF(__pyx_v_count);
   __Pyx_XDECREF(__pyx_v_output);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+static PyObject *__pyx_gb_9pyvoronoi_9Pyvoronoi_30generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pyvoronoi.pyx":326
+/* "pyvoronoi.pyx":310
  *         return output
  * 
+ *     def IterateVertices(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountVertices()
+ *         for index in  range(count):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_29IterateVertices(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_29IterateVertices = {"IterateVertices", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_29IterateVertices, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_29IterateVertices(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("IterateVertices (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("IterateVertices", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "IterateVertices", 0))) return NULL;
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_28IterateVertices(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_28IterateVertices(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *__pyx_cur_scope;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("IterateVertices", 0);
+  __pyx_cur_scope = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct__IterateVertices(__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices, __pyx_empty_tuple, NULL);
+  if (unlikely(!__pyx_cur_scope)) {
+    __pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *)Py_None);
+    __Pyx_INCREF(Py_None);
+    __PYX_ERR(0, 310, __pyx_L1_error)
+  } else {
+    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
+  }
+  __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
+  __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
+  __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
+  {
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9pyvoronoi_9Pyvoronoi_30generator, __pyx_codeobj_, (PyObject *) __pyx_cur_scope, __pyx_n_s_IterateVertices, __pyx_n_s_Pyvoronoi_IterateVertices, __pyx_n_s_pyvoronoi); if (unlikely(!gen)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_cur_scope);
+    __Pyx_RefNannyFinishContext();
+    return (PyObject *) gen;
+  }
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.IterateVertices", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_gb_9pyvoronoi_9Pyvoronoi_30generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+{
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *__pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *)__pyx_generator->closure);
+  PyObject *__pyx_r = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  PyObject *(*__pyx_t_6)(PyObject *);
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("IterateVertices", 0);
+  switch (__pyx_generator->resume_label) {
+    case 0: goto __pyx_L3_first_run;
+    case 1: goto __pyx_L6_resume_from_yield;
+    default: /* CPython raises the right error here */
+    __Pyx_RefNannyFinishContext();
+    return NULL;
+  }
+  __pyx_L3_first_run:;
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 310, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":311
+ * 
+ *     def IterateVertices(self):
+ *         count = self.CountVertices()             # <<<<<<<<<<<<<<
+ *         for index in  range(count):
+ *             yield self.GetVertex(index)
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_CountVertices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_cur_scope->__pyx_v_count = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "pyvoronoi.pyx":312
+ *     def IterateVertices(self):
+ *         count = self.CountVertices()
+ *         for index in  range(count):             # <<<<<<<<<<<<<<
+ *             yield self.GetVertex(index)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_cur_scope->__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
+    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = NULL;
+  } else {
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 312, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_6)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 312, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 312, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 312, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 312, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      }
+    } else {
+      __pyx_t_1 = __pyx_t_6(__pyx_t_2);
+      if (unlikely(!__pyx_t_1)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 312, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_1);
+    }
+    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_index);
+    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_index, __pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_1);
+    __pyx_t_1 = 0;
+
+    /* "pyvoronoi.pyx":313
+ *         count = self.CountVertices()
+ *         for index in  range(count):
+ *             yield self.GetVertex(index)             # <<<<<<<<<<<<<<
+ * 
+ *     def GetEdges(self):
+ */
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_GetVertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 = NULL;
+    __pyx_t_4 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_4 = 1;
+      }
+    }
+    #endif
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_index};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
+    __pyx_cur_scope->__pyx_t_1 = __pyx_t_5;
+    __pyx_cur_scope->__pyx_t_2 = __pyx_t_6;
+    __Pyx_XGIVEREF(__pyx_r);
+    __Pyx_RefNannyFinishContext();
+    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+    /* return from generator, yielding value */
+    __pyx_generator->resume_label = 1;
+    return __pyx_r;
+    __pyx_L6_resume_from_yield:;
+    __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
+    __pyx_cur_scope->__pyx_t_0 = 0;
+    __Pyx_XGOTREF(__pyx_t_2);
+    __pyx_t_5 = __pyx_cur_scope->__pyx_t_1;
+    __pyx_t_6 = __pyx_cur_scope->__pyx_t_2;
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 313, __pyx_L1_error)
+
+    /* "pyvoronoi.pyx":312
+ *     def IterateVertices(self):
+ *         count = self.CountVertices()
+ *         for index in  range(count):             # <<<<<<<<<<<<<<
+ *             yield self.GetVertex(index)
+ * 
+ */
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
+
+  /* "pyvoronoi.pyx":310
+ *         return output
+ * 
+ *     def IterateVertices(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountVertices()
+ *         for index in  range(count):
+ */
+
+  /* function exit code */
+  PyErr_SetNone(PyExc_StopIteration);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_Generator_Replace_StopIteration(0);
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("IterateVertices", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
+  #if !CYTHON_USE_EXC_INFO_STACK
+  __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+  #endif
+  __pyx_generator->resume_label = -1;
+  __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pyvoronoi.pyx":315
+ *             yield self.GetVertex(index)
+ * 
  *     def GetEdges(self):             # <<<<<<<<<<<<<<
  *         count = self.CountEdges()
  *         output = []
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_29GetEdges(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_32GetEdges(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_29GetEdges = {"GetEdges", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_29GetEdges, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_29GetEdges(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_32GetEdges = {"GetEdges", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_32GetEdges, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_32GetEdges(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -9007,22 +8868,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("GetEdges", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "GetEdges", 0))) return NULL;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_28GetEdges(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_31GetEdges(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_28GetEdges(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_31GetEdges(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
   PyObject *__pyx_v_count = NULL;
   PyObject *__pyx_v_output = NULL;
   PyObject *__pyx_v_index = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -9033,22 +8894,22 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetEdges", 1);
 
-  /* "pyvoronoi.pyx":327
+  /* "pyvoronoi.pyx":316
  * 
  *     def GetEdges(self):
  *         count = self.CountEdges()             # <<<<<<<<<<<<<<
  *         output = []
  *         for index in range(count):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CountEdges); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CountEdges); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -9060,106 +8921,106 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_count = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":328
+  /* "pyvoronoi.pyx":317
  *     def GetEdges(self):
  *         count = self.CountEdges()
  *         output = []             # <<<<<<<<<<<<<<
  *         for index in range(count):
  *             output.append(self.GetEdge(index))
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_output = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":329
+  /* "pyvoronoi.pyx":318
  *         count = self.CountEdges()
  *         output = []
  *         for index in range(count):             # <<<<<<<<<<<<<<
  *             output.append(self.GetEdge(index))
  *         return output
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 318, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 329, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 318, __pyx_L1_error)
           #endif
           if (__pyx_t_5 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 329, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 318, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 329, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 318, __pyx_L1_error)
           #endif
           if (__pyx_t_5 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 329, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 318, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_6(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 329, __pyx_L1_error)
+          else __PYX_ERR(0, 318, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pyvoronoi.pyx":330
+    /* "pyvoronoi.pyx":319
  *         output = []
  *         for index in range(count):
  *             output.append(self.GetEdge(index))             # <<<<<<<<<<<<<<
  *         return output
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetEdge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetEdge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_7 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
@@ -9171,45 +9032,45 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_v_index};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_output, __pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 330, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_output, __pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyvoronoi.pyx":329
+    /* "pyvoronoi.pyx":318
  *         count = self.CountEdges()
  *         output = []
  *         for index in range(count):             # <<<<<<<<<<<<<<
  *             output.append(self.GetEdge(index))
  *         return output
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":331
+  /* "pyvoronoi.pyx":320
  *         for index in range(count):
  *             output.append(self.GetEdge(index))
  *         return output             # <<<<<<<<<<<<<<
  * 
- *     def GetCells(self):
+ *     def IterateEdges(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_output);
   __pyx_r = __pyx_v_output;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":326
- *         return output
+  /* "pyvoronoi.pyx":315
+ *             yield self.GetVertex(index)
  * 
  *     def GetEdges(self):             # <<<<<<<<<<<<<<
  *         count = self.CountEdges()
  *         output = []
  */
 
   /* function exit code */
@@ -9224,33 +9085,338 @@
   __Pyx_XDECREF(__pyx_v_count);
   __Pyx_XDECREF(__pyx_v_output);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+static PyObject *__pyx_gb_9pyvoronoi_9Pyvoronoi_35generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pyvoronoi.pyx":333
+/* "pyvoronoi.pyx":322
  *         return output
  * 
+ *     def IterateEdges(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountEdges()
+ *         for index in range(count):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_34IterateEdges(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_34IterateEdges = {"IterateEdges", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_34IterateEdges, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_34IterateEdges(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("IterateEdges (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("IterateEdges", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "IterateEdges", 0))) return NULL;
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_33IterateEdges(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_33IterateEdges(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *__pyx_cur_scope;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("IterateEdges", 0);
+  __pyx_cur_scope = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct_1_IterateEdges(__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges, __pyx_empty_tuple, NULL);
+  if (unlikely(!__pyx_cur_scope)) {
+    __pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *)Py_None);
+    __Pyx_INCREF(Py_None);
+    __PYX_ERR(0, 322, __pyx_L1_error)
+  } else {
+    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
+  }
+  __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
+  __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
+  __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
+  {
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9pyvoronoi_9Pyvoronoi_35generator1, __pyx_codeobj__2, (PyObject *) __pyx_cur_scope, __pyx_n_s_IterateEdges, __pyx_n_s_Pyvoronoi_IterateEdges, __pyx_n_s_pyvoronoi); if (unlikely(!gen)) __PYX_ERR(0, 322, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_cur_scope);
+    __Pyx_RefNannyFinishContext();
+    return (PyObject *) gen;
+  }
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.IterateEdges", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_gb_9pyvoronoi_9Pyvoronoi_35generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+{
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *__pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *)__pyx_generator->closure);
+  PyObject *__pyx_r = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  PyObject *(*__pyx_t_6)(PyObject *);
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("IterateEdges", 0);
+  switch (__pyx_generator->resume_label) {
+    case 0: goto __pyx_L3_first_run;
+    case 1: goto __pyx_L6_resume_from_yield;
+    default: /* CPython raises the right error here */
+    __Pyx_RefNannyFinishContext();
+    return NULL;
+  }
+  __pyx_L3_first_run:;
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 322, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":323
+ * 
+ *     def IterateEdges(self):
+ *         count = self.CountEdges()             # <<<<<<<<<<<<<<
+ *         for index in range(count):
+ *             yield self.GetEdge(index)
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_CountEdges); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_cur_scope->__pyx_v_count = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "pyvoronoi.pyx":324
+ *     def IterateEdges(self):
+ *         count = self.CountEdges()
+ *         for index in range(count):             # <<<<<<<<<<<<<<
+ *             yield self.GetEdge(index)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_cur_scope->__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
+    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = NULL;
+  } else {
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 324, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_6)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 324, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 324, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 324, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 324, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      }
+    } else {
+      __pyx_t_1 = __pyx_t_6(__pyx_t_2);
+      if (unlikely(!__pyx_t_1)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 324, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_1);
+    }
+    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_index);
+    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_index, __pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_1);
+    __pyx_t_1 = 0;
+
+    /* "pyvoronoi.pyx":325
+ *         count = self.CountEdges()
+ *         for index in range(count):
+ *             yield self.GetEdge(index)             # <<<<<<<<<<<<<<
+ * 
+ *     def GetCells(self):
+ */
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_GetEdge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 = NULL;
+    __pyx_t_4 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_4 = 1;
+      }
+    }
+    #endif
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_index};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
+    __pyx_cur_scope->__pyx_t_1 = __pyx_t_5;
+    __pyx_cur_scope->__pyx_t_2 = __pyx_t_6;
+    __Pyx_XGIVEREF(__pyx_r);
+    __Pyx_RefNannyFinishContext();
+    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+    /* return from generator, yielding value */
+    __pyx_generator->resume_label = 1;
+    return __pyx_r;
+    __pyx_L6_resume_from_yield:;
+    __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
+    __pyx_cur_scope->__pyx_t_0 = 0;
+    __Pyx_XGOTREF(__pyx_t_2);
+    __pyx_t_5 = __pyx_cur_scope->__pyx_t_1;
+    __pyx_t_6 = __pyx_cur_scope->__pyx_t_2;
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 325, __pyx_L1_error)
+
+    /* "pyvoronoi.pyx":324
+ *     def IterateEdges(self):
+ *         count = self.CountEdges()
+ *         for index in range(count):             # <<<<<<<<<<<<<<
+ *             yield self.GetEdge(index)
+ * 
+ */
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
+
+  /* "pyvoronoi.pyx":322
+ *         return output
+ * 
+ *     def IterateEdges(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountEdges()
+ *         for index in range(count):
+ */
+
+  /* function exit code */
+  PyErr_SetNone(PyExc_StopIteration);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_Generator_Replace_StopIteration(0);
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("IterateEdges", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
+  #if !CYTHON_USE_EXC_INFO_STACK
+  __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+  #endif
+  __pyx_generator->resume_label = -1;
+  __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pyvoronoi.pyx":327
+ *             yield self.GetEdge(index)
+ * 
  *     def GetCells(self):             # <<<<<<<<<<<<<<
  *         count = self.CountCells()
  *         output = []
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_31GetCells(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_37GetCells(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_31GetCells = {"GetCells", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_31GetCells, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_31GetCells(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_37GetCells = {"GetCells", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_37GetCells, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_37GetCells(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -9267,22 +9433,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("GetCells", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "GetCells", 0))) return NULL;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_30GetCells(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_36GetCells(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_30GetCells(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_36GetCells(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
   PyObject *__pyx_v_count = NULL;
   PyObject *__pyx_v_output = NULL;
   PyObject *__pyx_v_index = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -9293,22 +9459,22 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetCells", 1);
 
-  /* "pyvoronoi.pyx":334
+  /* "pyvoronoi.pyx":328
  * 
  *     def GetCells(self):
  *         count = self.CountCells()             # <<<<<<<<<<<<<<
  *         output = []
  *         for index in range(count):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CountCells); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CountCells); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -9320,106 +9486,106 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_count = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":335
+  /* "pyvoronoi.pyx":329
  *     def GetCells(self):
  *         count = self.CountCells()
  *         output = []             # <<<<<<<<<<<<<<
  *         for index in range(count):
  *             output.append(self.GetCell(index))
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_output = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":336
+  /* "pyvoronoi.pyx":330
  *         count = self.CountCells()
  *         output = []
  *         for index in range(count):             # <<<<<<<<<<<<<<
  *             output.append(self.GetCell(index))
  *         return output
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 330, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 330, __pyx_L1_error)
           #endif
           if (__pyx_t_5 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 330, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 330, __pyx_L1_error)
           #endif
           if (__pyx_t_5 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 330, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_6(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 336, __pyx_L1_error)
+          else __PYX_ERR(0, 330, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pyvoronoi.pyx":337
+    /* "pyvoronoi.pyx":331
  *         output = []
  *         for index in range(count):
  *             output.append(self.GetCell(index))             # <<<<<<<<<<<<<<
  *         return output
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetCell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetCell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_7 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
@@ -9431,45 +9597,45 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_v_index};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 331, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_output, __pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 337, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_output, __pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyvoronoi.pyx":336
+    /* "pyvoronoi.pyx":330
  *         count = self.CountCells()
  *         output = []
  *         for index in range(count):             # <<<<<<<<<<<<<<
  *             output.append(self.GetCell(index))
  *         return output
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":338
+  /* "pyvoronoi.pyx":332
  *         for index in range(count):
  *             output.append(self.GetCell(index))
  *         return output             # <<<<<<<<<<<<<<
  * 
- *     def ReturnCurvedSiteInformation(self, edge):
+ *     def IterateCells(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_output);
   __pyx_r = __pyx_v_output;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":333
- *         return output
+  /* "pyvoronoi.pyx":327
+ *             yield self.GetEdge(index)
  * 
  *     def GetCells(self):             # <<<<<<<<<<<<<<
  *         count = self.CountCells()
  *         output = []
  */
 
   /* function exit code */
@@ -9484,34 +9650,339 @@
   __Pyx_XDECREF(__pyx_v_count);
   __Pyx_XDECREF(__pyx_v_output);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+static PyObject *__pyx_gb_9pyvoronoi_9Pyvoronoi_40generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pyvoronoi.pyx":340
+/* "pyvoronoi.pyx":334
  *         return output
  * 
+ *     def IterateCells(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountCells()
+ *         for index in range(count):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_39IterateCells(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_39IterateCells = {"IterateCells", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_39IterateCells, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_39IterateCells(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("IterateCells (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("IterateCells", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "IterateCells", 0))) return NULL;
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_38IterateCells(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_38IterateCells(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *__pyx_cur_scope;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("IterateCells", 0);
+  __pyx_cur_scope = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct_2_IterateCells(__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells, __pyx_empty_tuple, NULL);
+  if (unlikely(!__pyx_cur_scope)) {
+    __pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *)Py_None);
+    __Pyx_INCREF(Py_None);
+    __PYX_ERR(0, 334, __pyx_L1_error)
+  } else {
+    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
+  }
+  __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
+  __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
+  __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
+  {
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9pyvoronoi_9Pyvoronoi_40generator2, __pyx_codeobj__3, (PyObject *) __pyx_cur_scope, __pyx_n_s_IterateCells, __pyx_n_s_Pyvoronoi_IterateCells, __pyx_n_s_pyvoronoi); if (unlikely(!gen)) __PYX_ERR(0, 334, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_cur_scope);
+    __Pyx_RefNannyFinishContext();
+    return (PyObject *) gen;
+  }
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.IterateCells", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_gb_9pyvoronoi_9Pyvoronoi_40generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+{
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *__pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *)__pyx_generator->closure);
+  PyObject *__pyx_r = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  PyObject *(*__pyx_t_6)(PyObject *);
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("IterateCells", 0);
+  switch (__pyx_generator->resume_label) {
+    case 0: goto __pyx_L3_first_run;
+    case 1: goto __pyx_L6_resume_from_yield;
+    default: /* CPython raises the right error here */
+    __Pyx_RefNannyFinishContext();
+    return NULL;
+  }
+  __pyx_L3_first_run:;
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 334, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":335
+ * 
+ *     def IterateCells(self):
+ *         count = self.CountCells()             # <<<<<<<<<<<<<<
+ *         for index in range(count):
+ *             yield self.GetCell(index)
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_CountCells); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_cur_scope->__pyx_v_count = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "pyvoronoi.pyx":336
+ *     def IterateCells(self):
+ *         count = self.CountCells()
+ *         for index in range(count):             # <<<<<<<<<<<<<<
+ *             yield self.GetCell(index)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_cur_scope->__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
+    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = NULL;
+  } else {
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_6)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      }
+    } else {
+      __pyx_t_1 = __pyx_t_6(__pyx_t_2);
+      if (unlikely(!__pyx_t_1)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 336, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_1);
+    }
+    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_index);
+    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_index, __pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_1);
+    __pyx_t_1 = 0;
+
+    /* "pyvoronoi.pyx":337
+ *         count = self.CountCells()
+ *         for index in range(count):
+ *             yield self.GetCell(index)             # <<<<<<<<<<<<<<
+ * 
+ *     def ReturnCurvedSiteInformation(self, edge):
+ */
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_GetCell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 = NULL;
+    __pyx_t_4 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_4 = 1;
+      }
+    }
+    #endif
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_index};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
+    __pyx_cur_scope->__pyx_t_1 = __pyx_t_5;
+    __pyx_cur_scope->__pyx_t_2 = __pyx_t_6;
+    __Pyx_XGIVEREF(__pyx_r);
+    __Pyx_RefNannyFinishContext();
+    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+    /* return from generator, yielding value */
+    __pyx_generator->resume_label = 1;
+    return __pyx_r;
+    __pyx_L6_resume_from_yield:;
+    __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
+    __pyx_cur_scope->__pyx_t_0 = 0;
+    __Pyx_XGOTREF(__pyx_t_2);
+    __pyx_t_5 = __pyx_cur_scope->__pyx_t_1;
+    __pyx_t_6 = __pyx_cur_scope->__pyx_t_2;
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 337, __pyx_L1_error)
+
+    /* "pyvoronoi.pyx":336
+ *     def IterateCells(self):
+ *         count = self.CountCells()
+ *         for index in range(count):             # <<<<<<<<<<<<<<
+ *             yield self.GetCell(index)
+ * 
+ */
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
+
+  /* "pyvoronoi.pyx":334
+ *         return output
+ * 
+ *     def IterateCells(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountCells()
+ *         for index in range(count):
+ */
+
+  /* function exit code */
+  PyErr_SetNone(PyExc_StopIteration);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_Generator_Replace_StopIteration(0);
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("IterateCells", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
+  #if !CYTHON_USE_EXC_INFO_STACK
+  __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
+  #endif
+  __pyx_generator->resume_label = -1;
+  __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pyvoronoi.pyx":339
+ *             yield self.GetCell(index)
+ * 
  *     def ReturnCurvedSiteInformation(self, edge):             # <<<<<<<<<<<<<<
  *         """Return the index of the point side and the segment site associated  with a segment index
  *         """
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_33ReturnCurvedSiteInformation(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_42ReturnCurvedSiteInformation(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_32ReturnCurvedSiteInformation, "Return the index of the point side and the segment site associated  with a segment index\n        ");
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_33ReturnCurvedSiteInformation = {"ReturnCurvedSiteInformation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_33ReturnCurvedSiteInformation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_32ReturnCurvedSiteInformation};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_33ReturnCurvedSiteInformation(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_41ReturnCurvedSiteInformation, "Return the index of the point side and the segment site associated  with a segment index\n        ");
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_42ReturnCurvedSiteInformation = {"ReturnCurvedSiteInformation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_42ReturnCurvedSiteInformation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_41ReturnCurvedSiteInformation};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_42ReturnCurvedSiteInformation(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_edge = 0;
@@ -9547,58 +10018,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_edge)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 340, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 339, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "ReturnCurvedSiteInformation") < 0)) __PYX_ERR(0, 340, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "ReturnCurvedSiteInformation") < 0)) __PYX_ERR(0, 339, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_edge = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("ReturnCurvedSiteInformation", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 340, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("ReturnCurvedSiteInformation", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 339, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.ReturnCurvedSiteInformation", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_32ReturnCurvedSiteInformation(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_edge);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_41ReturnCurvedSiteInformation(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_edge);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_32ReturnCurvedSiteInformation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_edge) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_41ReturnCurvedSiteInformation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_edge) {
   PyObject *__pyx_v_twinEdge = NULL;
   PyObject *__pyx_v_cell = NULL;
   PyObject *__pyx_v_twinCell = NULL;
   PyObject *__pyx_v_pointSite = NULL;
   PyObject *__pyx_v_segmentSite = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -9609,24 +10080,24 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("ReturnCurvedSiteInformation", 1);
 
-  /* "pyvoronoi.pyx":343
+  /* "pyvoronoi.pyx":342
  *         """Return the index of the point side and the segment site associated  with a segment index
  *         """
  *         twinEdge = self.GetEdge(edge.twin)             # <<<<<<<<<<<<<<
  * 
  *         cell = self.GetCell(edge.cell)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetEdge); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetEdge); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_twin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_twin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -9639,31 +10110,31 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_twinEdge = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":345
+  /* "pyvoronoi.pyx":344
  *         twinEdge = self.GetEdge(edge.twin)
  * 
  *         cell = self.GetCell(edge.cell)             # <<<<<<<<<<<<<<
  *         twinCell = self.GetCell(twinEdge.cell)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetCell); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetCell); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_cell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_cell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -9676,31 +10147,31 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_cell = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":346
+  /* "pyvoronoi.pyx":345
  * 
  *         cell = self.GetCell(edge.cell)
  *         twinCell = self.GetCell(twinEdge.cell)             # <<<<<<<<<<<<<<
  * 
  *         pointSite = self.RetrieveScaledPoint(cell) if cell.contains_point == True else self.RetrieveScaledPoint(twinCell)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetCell); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetCell); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_twinEdge, __pyx_n_s_cell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_twinEdge, __pyx_n_s_cell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -9713,36 +10184,36 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_twinCell = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":348
+  /* "pyvoronoi.pyx":347
  *         twinCell = self.GetCell(twinEdge.cell)
  * 
  *         pointSite = self.RetrieveScaledPoint(cell) if cell.contains_point == True else self.RetrieveScaledPoint(twinCell)             # <<<<<<<<<<<<<<
  *         segmentSite = self.RetriveScaledSegment(twinCell) if cell.contains_point == True else self.RetriveScaledSegment(cell)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_contains_point); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_contains_point); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, Py_True, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, Py_True, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_6) {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveScaledPoint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveScaledPoint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
@@ -9754,22 +10225,22 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_cell};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveScaledPoint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveScaledPoint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
@@ -9781,39 +10252,39 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_twinCell};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __pyx_v_pointSite = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":349
+  /* "pyvoronoi.pyx":348
  * 
  *         pointSite = self.RetrieveScaledPoint(cell) if cell.contains_point == True else self.RetrieveScaledPoint(twinCell)
  *         segmentSite = self.RetriveScaledSegment(twinCell) if cell.contains_point == True else self.RetriveScaledSegment(cell)             # <<<<<<<<<<<<<<
  * 
  *         return [pointSite, segmentSite]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_contains_point); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_contains_point); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, Py_True, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, Py_True, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_6) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetriveScaledSegment); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetriveScaledSegment); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -9825,22 +10296,22 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_twinCell};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetriveScaledSegment); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetriveScaledSegment); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -9852,46 +10323,46 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_cell};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   }
   __pyx_v_segmentSite = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":351
+  /* "pyvoronoi.pyx":350
  *         segmentSite = self.RetriveScaledSegment(twinCell) if cell.contains_point == True else self.RetriveScaledSegment(cell)
  * 
  *         return [pointSite, segmentSite]             # <<<<<<<<<<<<<<
  * 
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_pointSite);
   __Pyx_GIVEREF(__pyx_v_pointSite);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_pointSite)) __PYX_ERR(0, 351, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_pointSite)) __PYX_ERR(0, 350, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_segmentSite);
   __Pyx_GIVEREF(__pyx_v_segmentSite);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_v_segmentSite)) __PYX_ERR(0, 351, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_v_segmentSite)) __PYX_ERR(0, 350, __pyx_L1_error);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":340
- *         return output
+  /* "pyvoronoi.pyx":339
+ *             yield self.GetCell(index)
  * 
  *     def ReturnCurvedSiteInformation(self, edge):             # <<<<<<<<<<<<<<
  *         """Return the index of the point side and the segment site associated  with a segment index
  *         """
  */
 
   /* function exit code */
@@ -9909,32 +10380,32 @@
   __Pyx_XDECREF(__pyx_v_pointSite);
   __Pyx_XDECREF(__pyx_v_segmentSite);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":353
+/* "pyvoronoi.pyx":352
  *         return [pointSite, segmentSite]
  * 
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):             # <<<<<<<<<<<<<<
  *         if(max_dist <= 0):
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_35DiscretizeCurvedEdge(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_44DiscretizeCurvedEdge(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_35DiscretizeCurvedEdge = {"DiscretizeCurvedEdge", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_35DiscretizeCurvedEdge, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_35DiscretizeCurvedEdge(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_44DiscretizeCurvedEdge = {"DiscretizeCurvedEdge", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_44DiscretizeCurvedEdge, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_44DiscretizeCurvedEdge(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_index = 0;
@@ -9977,37 +10448,37 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_dist)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("DiscretizeCurvedEdge", 0, 2, 3, 1); __PYX_ERR(0, 353, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("DiscretizeCurvedEdge", 0, 2, 3, 1); __PYX_ERR(0, 352, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parabola_equation_tolerance);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "DiscretizeCurvedEdge") < 0)) __PYX_ERR(0, 353, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "DiscretizeCurvedEdge") < 0)) __PYX_ERR(0, 352, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -10017,42 +10488,42 @@
     }
     __pyx_v_index = values[0];
     __pyx_v_max_dist = values[1];
     __pyx_v_parabola_equation_tolerance = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("DiscretizeCurvedEdge", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 353, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("DiscretizeCurvedEdge", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 352, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.DiscretizeCurvedEdge", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_34DiscretizeCurvedEdge(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_index, __pyx_v_max_dist, __pyx_v_parabola_equation_tolerance);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_43DiscretizeCurvedEdge(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_index, __pyx_v_max_dist, __pyx_v_parabola_equation_tolerance);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_34DiscretizeCurvedEdge(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_43DiscretizeCurvedEdge(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance) {
   PyObject *__pyx_v_edge = NULL;
   PyObject *__pyx_v_sites = NULL;
   PyObject *__pyx_v_pointSite = NULL;
   PyObject *__pyx_v_segmentSite = NULL;
   PyObject *__pyx_v_edgeStartVertex = NULL;
   PyObject *__pyx_v_edgeEndVertex = NULL;
   PyObject *__pyx_r = NULL;
@@ -10066,34 +10537,34 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("DiscretizeCurvedEdge", 1);
 
-  /* "pyvoronoi.pyx":354
+  /* "pyvoronoi.pyx":353
  * 
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):
  *         if(max_dist <= 0):             # <<<<<<<<<<<<<<
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  * 
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_max_dist, __pyx_int_0, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_max_dist, __pyx_int_0, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "pyvoronoi.pyx":355
+    /* "pyvoronoi.pyx":354
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):
  *         if(max_dist <= 0):
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))             # <<<<<<<<<<<<<<
  * 
  *         if(parabola_equation_tolerance < 0):
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Max_distance_must_be_greater_tha, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Max_distance_must_be_greater_tha, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -10105,54 +10576,54 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_max_dist};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 355, __pyx_L1_error)
+    __PYX_ERR(0, 354, __pyx_L1_error)
 
-    /* "pyvoronoi.pyx":354
+    /* "pyvoronoi.pyx":353
  * 
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):
  *         if(max_dist <= 0):             # <<<<<<<<<<<<<<
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  * 
  */
   }
 
-  /* "pyvoronoi.pyx":357
+  /* "pyvoronoi.pyx":356
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  * 
  *         if(parabola_equation_tolerance < 0):             # <<<<<<<<<<<<<<
  *             raise ValueError("Parabola equation tolerance must be greater than 0 or equal to 0. Value passed: {0}".format(parabola_equation_tolerance))
  * 
  */
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_parabola_equation_tolerance, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_v_parabola_equation_tolerance, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "pyvoronoi.pyx":358
+    /* "pyvoronoi.pyx":357
  * 
  *         if(parabola_equation_tolerance < 0):
  *             raise ValueError("Parabola equation tolerance must be greater than 0 or equal to 0. Value passed: {0}".format(parabola_equation_tolerance))             # <<<<<<<<<<<<<<
  * 
  *         edge = self.GetEdge(index)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Parabola_equation_tolerance_must, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Parabola_equation_tolerance_must, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
@@ -10164,42 +10635,42 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_parabola_equation_tolerance};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 358, __pyx_L1_error)
+    __PYX_ERR(0, 357, __pyx_L1_error)
 
-    /* "pyvoronoi.pyx":357
+    /* "pyvoronoi.pyx":356
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  * 
  *         if(parabola_equation_tolerance < 0):             # <<<<<<<<<<<<<<
  *             raise ValueError("Parabola equation tolerance must be greater than 0 or equal to 0. Value passed: {0}".format(parabola_equation_tolerance))
  * 
  */
   }
 
-  /* "pyvoronoi.pyx":360
+  /* "pyvoronoi.pyx":359
  *             raise ValueError("Parabola equation tolerance must be greater than 0 or equal to 0. Value passed: {0}".format(parabola_equation_tolerance))
  * 
  *         edge = self.GetEdge(index)             # <<<<<<<<<<<<<<
  *         sites = self.ReturnCurvedSiteInformation(edge)
  *         pointSite = sites[0]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetEdge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetEdge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -10211,29 +10682,29 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_index};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_edge = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":361
+  /* "pyvoronoi.pyx":360
  * 
  *         edge = self.GetEdge(index)
  *         sites = self.ReturnCurvedSiteInformation(edge)             # <<<<<<<<<<<<<<
  *         pointSite = sites[0]
  *         segmentSite = sites[1]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_ReturnCurvedSiteInformation); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_ReturnCurvedSiteInformation); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -10245,55 +10716,55 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_edge};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 361, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_sites = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":362
+  /* "pyvoronoi.pyx":361
  *         edge = self.GetEdge(index)
  *         sites = self.ReturnCurvedSiteInformation(edge)
  *         pointSite = sites[0]             # <<<<<<<<<<<<<<
  *         segmentSite = sites[1]
  * 
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_sites, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_sites, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pointSite = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":363
+  /* "pyvoronoi.pyx":362
  *         sites = self.ReturnCurvedSiteInformation(edge)
  *         pointSite = sites[0]
  *         segmentSite = sites[1]             # <<<<<<<<<<<<<<
  * 
  *         edgeStartVertex = self.GetVertex(edge.start)
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_sites, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_sites, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_segmentSite = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":365
+  /* "pyvoronoi.pyx":364
  *         segmentSite = sites[1]
  * 
  *         edgeStartVertex = self.GetVertex(edge.start)             # <<<<<<<<<<<<<<
  *         edgeEndVertex = self.GetVertex(edge.end)
  *         return self.Discretize(pointSite,segmentSite, [edgeStartVertex.X,edgeStartVertex.Y], [edgeEndVertex.X, edgeEndVertex.Y], max_dist, parabola_equation_tolerance)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetVertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetVertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
@@ -10306,31 +10777,31 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 365, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 364, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_edgeStartVertex = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":366
+  /* "pyvoronoi.pyx":365
  * 
  *         edgeStartVertex = self.GetVertex(edge.start)
  *         edgeEndVertex = self.GetVertex(edge.end)             # <<<<<<<<<<<<<<
  *         return self.Discretize(pointSite,segmentSite, [edgeStartVertex.X,edgeStartVertex.Y], [edgeEndVertex.X, edgeEndVertex.Y], max_dist, parabola_equation_tolerance)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetVertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetVertex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edge, __pyx_n_s_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
@@ -10343,53 +10814,53 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 366, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 365, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_edgeEndVertex = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":367
+  /* "pyvoronoi.pyx":366
  *         edgeStartVertex = self.GetVertex(edge.start)
  *         edgeEndVertex = self.GetVertex(edge.end)
  *         return self.Discretize(pointSite,segmentSite, [edgeStartVertex.X,edgeStartVertex.Y], [edgeEndVertex.X, edgeEndVertex.Y], max_dist, parabola_equation_tolerance)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Discretize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Discretize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeStartVertex, __pyx_n_s_X); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeStartVertex, __pyx_n_s_X); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeStartVertex, __pyx_n_s_Y); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeStartVertex, __pyx_n_s_Y); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_4)) __PYX_ERR(0, 366, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_6)) __PYX_ERR(0, 367, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_6)) __PYX_ERR(0, 366, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeEndVertex, __pyx_n_s_X); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeEndVertex, __pyx_n_s_X); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeEndVertex, __pyx_n_s_Y); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_edgeEndVertex, __pyx_n_s_Y); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_6)) __PYX_ERR(0, 367, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_6)) __PYX_ERR(0, 366, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_4)) __PYX_ERR(0, 366, __pyx_L1_error);
   __pyx_t_6 = 0;
   __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -10404,23 +10875,23 @@
   #endif
   {
     PyObject *__pyx_callargs[7] = {__pyx_t_4, __pyx_v_pointSite, __pyx_v_segmentSite, __pyx_t_7, __pyx_t_8, __pyx_v_max_dist, __pyx_v_parabola_equation_tolerance};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 6+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 366, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":353
+  /* "pyvoronoi.pyx":352
  *         return [pointSite, segmentSite]
  * 
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):             # <<<<<<<<<<<<<<
  *         if(max_dist <= 0):
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  */
 
@@ -10442,33 +10913,33 @@
   __Pyx_XDECREF(__pyx_v_edgeStartVertex);
   __Pyx_XDECREF(__pyx_v_edgeEndVertex);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":370
+/* "pyvoronoi.pyx":369
  * 
  * 
  *     def RetrievePoint(self, cell):             # <<<<<<<<<<<<<<
  *         """Retrive the input point associated with a cell.
  * 		:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_37RetrievePoint(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_46RetrievePoint(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_36RetrievePoint, "Retrive the input point associated with a cell.\n\t\t:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.\n        ");
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_37RetrievePoint = {"RetrievePoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_37RetrievePoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_36RetrievePoint};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_37RetrievePoint(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_45RetrievePoint, "Retrive the input point associated with a cell.\n\t\t:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.\n        ");
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_46RetrievePoint = {"RetrievePoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_46RetrievePoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_45RetrievePoint};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_46RetrievePoint(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_cell = 0;
@@ -10504,172 +10975,191 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cell)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 370, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RetrievePoint") < 0)) __PYX_ERR(0, 370, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RetrievePoint") < 0)) __PYX_ERR(0, 369, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_cell = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("RetrievePoint", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 370, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("RetrievePoint", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 369, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.RetrievePoint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_36RetrievePoint(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_45RetrievePoint(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_36RetrievePoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_45RetrievePoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
+  struct Point __pyx_v_point;
   PyObject *__pyx_v_input_segment = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
+  unsigned int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("RetrievePoint", 1);
 
-  /* "pyvoronoi.pyx":374
+  /* "pyvoronoi.pyx":373
  * 		:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.
  *         """
  *         if(cell.source_category == 0):             # <<<<<<<<<<<<<<
- *             return self.inputPoints[cell.site]
- * 
+ *             point = self.thisptr.GetPoint(cell.site)
+ *             return [point.X, point.Y]
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_source_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_source_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "pyvoronoi.pyx":375
+    /* "pyvoronoi.pyx":374
  *         """
  *         if(cell.source_category == 0):
- *             return self.inputPoints[cell.site]             # <<<<<<<<<<<<<<
+ *             point = self.thisptr.GetPoint(cell.site)             # <<<<<<<<<<<<<<
+ *             return [point.X, point.Y]
+ * 
+ */
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_site); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 374, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_v_point = __pyx_v_self->thisptr->GetPoint(__pyx_t_3);
+
+    /* "pyvoronoi.pyx":375
+ *         if(cell.source_category == 0):
+ *             point = self.thisptr.GetPoint(cell.site)
+ *             return [point.X, point.Y]             # <<<<<<<<<<<<<<
  * 
  *         input_segment = self.RetrieveSegment(cell)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputPoints); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_point.X); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_site); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 375, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_point.Y); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_r = __pyx_t_4;
+    __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_1);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error);
+    __pyx_t_1 = 0;
     __pyx_t_4 = 0;
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "pyvoronoi.pyx":374
+    /* "pyvoronoi.pyx":373
  * 		:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.
  *         """
  *         if(cell.source_category == 0):             # <<<<<<<<<<<<<<
- *             return self.inputPoints[cell.site]
- * 
+ *             point = self.thisptr.GetPoint(cell.site)
+ *             return [point.X, point.Y]
  */
   }
 
   /* "pyvoronoi.pyx":377
- *             return self.inputPoints[cell.site]
+ *             return [point.X, point.Y]
  * 
  *         input_segment = self.RetrieveSegment(cell)             # <<<<<<<<<<<<<<
  *         if(cell.source_category == 1):
  *             return input_segment[0]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveSegment); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveSegment); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_1 = NULL;
-  __pyx_t_5 = 0;
+  __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+  if (likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_1)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_5 = 1;
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_6 = 1;
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_cell};
-    __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_v_input_segment = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_v_input_segment = __pyx_t_5;
+  __pyx_t_5 = 0;
 
   /* "pyvoronoi.pyx":378
  * 
  *         input_segment = self.RetrieveSegment(cell)
  *         if(cell.source_category == 1):             # <<<<<<<<<<<<<<
  *             return input_segment[0]
  *         else:
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_source_category); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_4, __pyx_int_1, 1, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 378, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_source_category); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_2 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_5, __pyx_int_1, 1, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 378, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_2) {
 
     /* "pyvoronoi.pyx":379
  *         input_segment = self.RetrieveSegment(cell)
  *         if(cell.source_category == 1):
  *             return input_segment[0]             # <<<<<<<<<<<<<<
  *         else:
  *             return input_segment[1]
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_input_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_r = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_input_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
     goto __pyx_L0;
 
     /* "pyvoronoi.pyx":378
  * 
  *         input_segment = self.RetrieveSegment(cell)
  *         if(cell.source_category == 1):             # <<<<<<<<<<<<<<
  *             return input_segment[0]
@@ -10682,34 +11172,34 @@
  *         else:
  *             return input_segment[1]             # <<<<<<<<<<<<<<
  * 
  *     def RetrieveSegment(self, cell):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_input_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_r = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_input_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
     goto __pyx_L0;
   }
 
-  /* "pyvoronoi.pyx":370
+  /* "pyvoronoi.pyx":369
  * 
  * 
  *     def RetrievePoint(self, cell):             # <<<<<<<<<<<<<<
  *         """Retrive the input point associated with a cell.
  * 		:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.RetrievePoint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_input_segment);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -10720,24 +11210,24 @@
  * 
  *     def RetrieveSegment(self, cell):             # <<<<<<<<<<<<<<
  *         """Retrive the input segment associated with a cell.
  *         """
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_39RetrieveSegment(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_48RetrieveSegment(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_38RetrieveSegment, "Retrive the input segment associated with a cell.\n        ");
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_39RetrieveSegment = {"RetrieveSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_39RetrieveSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_38RetrieveSegment};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_39RetrieveSegment(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_47RetrieveSegment, "Retrive the input segment associated with a cell.\n        ");
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_48RetrieveSegment = {"RetrieveSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_48RetrieveSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_47RetrieveSegment};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_48RetrieveSegment(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_cell = 0;
@@ -10803,66 +11293,124 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.RetrieveSegment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_38RetrieveSegment(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_47RetrieveSegment(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_38RetrieveSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_47RetrieveSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
+  struct Segment __pyx_v_segment;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  Py_ssize_t __pyx_t_4;
+  unsigned int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("RetrieveSegment", 1);
 
   /* "pyvoronoi.pyx":386
  *         """Retrive the input segment associated with a cell.
  *         """
- *         return self.inputSegments[cell.site - len(self.inputPoints)]             # <<<<<<<<<<<<<<
- * 
- * 
+ *         segment = self.thisptr.GetSegment(cell.site - self.thisptr.CountPoints())             # <<<<<<<<<<<<<<
+ *         return [
+ *             [segment.p0.X,segment.p0.Y],
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputSegments); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_site); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell, __pyx_n_s_site); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->thisptr->CountPoints()); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_inputPoints); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyInt_As_unsigned_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_v_segment = __pyx_v_self->thisptr->GetSegment(__pyx_t_4);
+
+  /* "pyvoronoi.pyx":387
+ *         """
+ *         segment = self.thisptr.GetSegment(cell.site - self.thisptr.CountPoints())
+ *         return [             # <<<<<<<<<<<<<<
+ *             [segment.p0.X,segment.p0.Y],
+ *             [segment.p1.X, segment.p1.Y]
+ */
+  __Pyx_XDECREF(__pyx_r);
+
+  /* "pyvoronoi.pyx":388
+ *         segment = self.thisptr.GetSegment(cell.site - self.thisptr.CountPoints())
+ *         return [
+ *             [segment.p0.X,segment.p0.Y],             # <<<<<<<<<<<<<<
+ *             [segment.p1.X, segment.p1.Y]
+ *         ]
+ */
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_segment.p0.X); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_segment.p0.Y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 388, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_2 = 0;
+
+  /* "pyvoronoi.pyx":389
+ *         return [
+ *             [segment.p0.X,segment.p0.Y],
+ *             [segment.p1.X, segment.p1.Y]             # <<<<<<<<<<<<<<
+ *         ]
+ * 
+ */
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_segment.p1.X); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_segment.p1.Y); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error);
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+
+  /* "pyvoronoi.pyx":387
+ *         """
+ *         segment = self.thisptr.GetSegment(cell.site - self.thisptr.CountPoints())
+ *         return [             # <<<<<<<<<<<<<<
+ *             [segment.p0.X,segment.p0.Y],
+ *             [segment.p1.X, segment.p1.Y]
+ */
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_t_5 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "pyvoronoi.pyx":383
  *             return input_segment[1]
  * 
@@ -10881,32 +11429,32 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":389
- * 
+/* "pyvoronoi.pyx":392
+ *         ]
  * 
  *     def RetrieveScaledPoint(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_point = self.RetrievePoint(cell)
  *         return [
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_41RetrieveScaledPoint(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_50RetrieveScaledPoint(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_41RetrieveScaledPoint = {"RetrieveScaledPoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_41RetrieveScaledPoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_41RetrieveScaledPoint(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_50RetrieveScaledPoint = {"RetrieveScaledPoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_50RetrieveScaledPoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_50RetrieveScaledPoint(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_cell = 0;
@@ -10942,79 +11490,79 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cell)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 392, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RetrieveScaledPoint") < 0)) __PYX_ERR(0, 389, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RetrieveScaledPoint") < 0)) __PYX_ERR(0, 392, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_cell = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("RetrieveScaledPoint", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 389, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("RetrieveScaledPoint", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 392, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.RetrieveScaledPoint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_40RetrieveScaledPoint(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_49RetrieveScaledPoint(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_40RetrieveScaledPoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_49RetrieveScaledPoint(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
   PyObject *__pyx_v_non_scaled_point = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("RetrieveScaledPoint", 1);
 
-  /* "pyvoronoi.pyx":390
+  /* "pyvoronoi.pyx":393
  * 
  *     def RetrieveScaledPoint(self, cell):
  *         non_scaled_point = self.RetrievePoint(cell)             # <<<<<<<<<<<<<<
  *         return [
  * 			non_scaled_point[0] / self.SCALING_FACTOR,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrievePoint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrievePoint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -11026,83 +11574,83 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_cell};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_non_scaled_point = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":391
+  /* "pyvoronoi.pyx":394
  *     def RetrieveScaledPoint(self, cell):
  *         non_scaled_point = self.RetrievePoint(cell)
  *         return [             # <<<<<<<<<<<<<<
  * 			non_scaled_point[0] / self.SCALING_FACTOR,
  * 			non_scaled_point[1] / self.SCALING_FACTOR
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "pyvoronoi.pyx":392
+  /* "pyvoronoi.pyx":395
  *         non_scaled_point = self.RetrievePoint(cell)
  *         return [
  * 			non_scaled_point[0] / self.SCALING_FACTOR,             # <<<<<<<<<<<<<<
  * 			non_scaled_point[1] / self.SCALING_FACTOR
  * 		]
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_non_scaled_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_non_scaled_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":393
+  /* "pyvoronoi.pyx":396
  *         return [
  * 			non_scaled_point[0] / self.SCALING_FACTOR,
  * 			non_scaled_point[1] / self.SCALING_FACTOR             # <<<<<<<<<<<<<<
  * 		]
  * 
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_non_scaled_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_non_scaled_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":391
+  /* "pyvoronoi.pyx":394
  *     def RetrieveScaledPoint(self, cell):
  *         non_scaled_point = self.RetrievePoint(cell)
  *         return [             # <<<<<<<<<<<<<<
  * 			non_scaled_point[0] / self.SCALING_FACTOR,
  * 			non_scaled_point[1] / self.SCALING_FACTOR
  */
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 394, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_5)) __PYX_ERR(0, 391, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_5)) __PYX_ERR(0, 394, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_5 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":389
- * 
+  /* "pyvoronoi.pyx":392
+ *         ]
  * 
  *     def RetrieveScaledPoint(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_point = self.RetrievePoint(cell)
  *         return [
  */
 
   /* function exit code */
@@ -11116,32 +11664,32 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_non_scaled_point);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":396
+/* "pyvoronoi.pyx":399
  * 		]
  * 
  *     def RetriveScaledSegment(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_segment = self.RetrieveSegment(cell)
  *         return [
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_43RetriveScaledSegment(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_52RetriveScaledSegment(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_43RetriveScaledSegment = {"RetriveScaledSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_43RetriveScaledSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_43RetriveScaledSegment(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_52RetriveScaledSegment = {"RetriveScaledSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_52RetriveScaledSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_52RetriveScaledSegment(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_cell = 0;
@@ -11177,80 +11725,80 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cell)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 399, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RetriveScaledSegment") < 0)) __PYX_ERR(0, 396, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RetriveScaledSegment") < 0)) __PYX_ERR(0, 399, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_cell = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("RetriveScaledSegment", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 396, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("RetriveScaledSegment", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 399, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.RetriveScaledSegment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_42RetriveScaledSegment(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_51RetriveScaledSegment(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_cell);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_42RetriveScaledSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_51RetriveScaledSegment(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_cell) {
   PyObject *__pyx_v_non_scaled_segment = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("RetriveScaledSegment", 1);
 
-  /* "pyvoronoi.pyx":397
+  /* "pyvoronoi.pyx":400
  * 
  *     def RetriveScaledSegment(self, cell):
  *         non_scaled_segment = self.RetrieveSegment(cell)             # <<<<<<<<<<<<<<
  *         return [
  * 			[non_scaled_segment[0][0] / self.SCALING_FACTOR, non_scaled_segment[0][1] / self.SCALING_FACTOR],
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveSegment); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RetrieveSegment); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -11262,126 +11810,126 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_cell};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_non_scaled_segment = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":398
+  /* "pyvoronoi.pyx":401
  *     def RetriveScaledSegment(self, cell):
  *         non_scaled_segment = self.RetrieveSegment(cell)
  *         return [             # <<<<<<<<<<<<<<
  * 			[non_scaled_segment[0][0] / self.SCALING_FACTOR, non_scaled_segment[0][1] / self.SCALING_FACTOR],
  * 			[non_scaled_segment[1][0] / self.SCALING_FACTOR,non_scaled_segment[1][1] / self.SCALING_FACTOR]
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "pyvoronoi.pyx":399
+  /* "pyvoronoi.pyx":402
  *         non_scaled_segment = self.RetrieveSegment(cell)
  *         return [
  * 			[non_scaled_segment[0][0] / self.SCALING_FACTOR, non_scaled_segment[0][1] / self.SCALING_FACTOR],             # <<<<<<<<<<<<<<
  * 			[non_scaled_segment[1][0] / self.SCALING_FACTOR,non_scaled_segment[1][1] / self.SCALING_FACTOR]
  * 		]
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 399, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_5)) __PYX_ERR(0, 399, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_5)) __PYX_ERR(0, 402, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":400
+  /* "pyvoronoi.pyx":403
  *         return [
  * 			[non_scaled_segment[0][0] / self.SCALING_FACTOR, non_scaled_segment[0][1] / self.SCALING_FACTOR],
  * 			[non_scaled_segment[1][0] / self.SCALING_FACTOR,non_scaled_segment[1][1] / self.SCALING_FACTOR]             # <<<<<<<<<<<<<<
  * 		]
  * 
  */
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_non_scaled_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_6)) __PYX_ERR(0, 403, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_6 = 0;
 
-  /* "pyvoronoi.pyx":398
+  /* "pyvoronoi.pyx":401
  *     def RetriveScaledSegment(self, cell):
  *         non_scaled_segment = self.RetrieveSegment(cell)
  *         return [             # <<<<<<<<<<<<<<
  * 			[non_scaled_segment[0][0] / self.SCALING_FACTOR, non_scaled_segment[0][1] / self.SCALING_FACTOR],
  * 			[non_scaled_segment[1][0] / self.SCALING_FACTOR,non_scaled_segment[1][1] / self.SCALING_FACTOR]
  */
-  __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 398, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 401, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_5 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":396
+  /* "pyvoronoi.pyx":399
  * 		]
  * 
  *     def RetriveScaledSegment(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_segment = self.RetrieveSegment(cell)
  *         return [
  */
 
@@ -11397,33 +11945,33 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_non_scaled_segment);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":403
+/* "pyvoronoi.pyx":406
  * 		]
  * 
  *     def GetParabolaY(self, x, focus, directrix_y):             # <<<<<<<<<<<<<<
  *         """
  * 		Solve the parabola equation for a given value on the x-axis and return the associated value on the y-axis.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_45GetParabolaY(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_54GetParabolaY(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_44GetParabolaY, "\n\t\tSolve the parabola equation for a given value on the x-axis and return the associated value on the y-axis.\n\t\tThis equation assumes that the directix is parallel to the x-axis.\n        Parabola equation are different if the directix is parallel to the y-axis.\n\t\t:param x: the x-value used to solve the equation.\n        :param focus: the focus point used for solving the equation of the parabola.\n        :param directix: the directix value used for solving the equation of the parabola.\n        :return: the associated value on the y-axis.\n        ");
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_45GetParabolaY = {"GetParabolaY", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_45GetParabolaY, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_44GetParabolaY};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_45GetParabolaY(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_53GetParabolaY, "\n\t\tSolve the parabola equation for a given value on the x-axis and return the associated value on the y-axis.\n\t\tThis equation assumes that the directix is parallel to the x-axis.\n        Parabola equation are different if the directix is parallel to the y-axis.\n\t\t:param x: the x-value used to solve the equation.\n        :param focus: the focus point used for solving the equation of the parabola.\n        :param directix: the directix value used for solving the equation of the parabola.\n        :return: the associated value on the y-axis.\n        ");
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_54GetParabolaY = {"GetParabolaY", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_54GetParabolaY, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_53GetParabolaY};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_54GetParabolaY(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_x = 0;
@@ -11465,140 +12013,140 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 403, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 406, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_focus)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 403, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 406, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("GetParabolaY", 1, 3, 3, 1); __PYX_ERR(0, 403, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("GetParabolaY", 1, 3, 3, 1); __PYX_ERR(0, 406, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_directrix_y)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 403, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 406, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("GetParabolaY", 1, 3, 3, 2); __PYX_ERR(0, 403, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("GetParabolaY", 1, 3, 3, 2); __PYX_ERR(0, 406, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetParabolaY") < 0)) __PYX_ERR(0, 403, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetParabolaY") < 0)) __PYX_ERR(0, 406, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_x = values[0];
     __pyx_v_focus = values[1];
     __pyx_v_directrix_y = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("GetParabolaY", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 403, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("GetParabolaY", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 406, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.GetParabolaY", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_44GetParabolaY(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_x, __pyx_v_focus, __pyx_v_directrix_y);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_53GetParabolaY(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_x, __pyx_v_focus, __pyx_v_directrix_y);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_44GetParabolaY(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_focus, PyObject *__pyx_v_directrix_y) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_53GetParabolaY(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_focus, PyObject *__pyx_v_directrix_y) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetParabolaY", 1);
 
-  /* "pyvoronoi.pyx":413
+  /* "pyvoronoi.pyx":416
  *         :return: the associated value on the y-axis.
  *         """
  *         return (pow(x - focus[0], 2) + pow(focus[1], 2) - pow(directrix_y, 2)) / (2 * (focus[1] - directrix_y));             # <<<<<<<<<<<<<<
  * 
  *     def CheckUnsolvableParabolaEquation(self, boost_x, boost_y, focus, directix, tolerance):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_focus, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_focus, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_v_x, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_v_x, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Power2(__pyx_t_2, __pyx_int_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Power2(__pyx_t_2, __pyx_int_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_focus, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_focus, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyNumber_Power2(__pyx_t_2, __pyx_int_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Power2(__pyx_t_2, __pyx_int_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyNumber_Power2(__pyx_v_directrix_y, __pyx_int_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Power2(__pyx_v_directrix_y, __pyx_int_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_focus, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_focus, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_t_3, __pyx_v_directrix_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_t_3, __pyx_v_directrix_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_MultiplyCObj(__pyx_int_2, __pyx_t_2, 2, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_MultiplyCObj(__pyx_int_2, __pyx_t_2, 2, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":403
+  /* "pyvoronoi.pyx":406
  * 		]
  * 
  *     def GetParabolaY(self, x, focus, directrix_y):             # <<<<<<<<<<<<<<
  *         """
  * 		Solve the parabola equation for a given value on the x-axis and return the associated value on the y-axis.
  */
 
@@ -11611,33 +12159,33 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":415
+/* "pyvoronoi.pyx":418
  *         return (pow(x - focus[0], 2) + pow(focus[1], 2) - pow(directrix_y, 2)) / (2 * (focus[1] - directrix_y));
  * 
  *     def CheckUnsolvableParabolaEquation(self, boost_x, boost_y, focus, directix, tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Compare the y-coordinate of a point on the parabola returned by Boost with the computed value.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_47CheckUnsolvableParabolaEquation(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_56CheckUnsolvableParabolaEquation(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_46CheckUnsolvableParabolaEquation, "\n        Compare the y-coordinate of a point on the parabola returned by Boost with the computed value.\n\t\tThe function will return an exception if the difference between the computed y-value and the y-value returned by Boost.\n\t\tThe computed point will be returned otherwise.\n        :param boost_x: the x-value of the point parabola returned by boost.\n        :param boost_y: the y-value of the point parabola returned by boost.\n        :param focus: the focus point used for solving the equation of the parabola.\n        :param directix: the directix value used for solving the equation of the parabola.\n\t\t:param tolerance: the distance allowed between the point computed by boost and the point computed by the equation.\n\t\t:return: the point on the parabola computed using the value of boost_x.\n\t\t");
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_47CheckUnsolvableParabolaEquation = {"CheckUnsolvableParabolaEquation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_47CheckUnsolvableParabolaEquation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_46CheckUnsolvableParabolaEquation};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_47CheckUnsolvableParabolaEquation(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_55CheckUnsolvableParabolaEquation, "\n        Compare the y-coordinate of a point on the parabola returned by Boost with the computed value.\n\t\tThe function will return an exception if the difference between the computed y-value and the y-value returned by Boost.\n\t\tThe computed point will be returned otherwise.\n        :param boost_x: the x-value of the point parabola returned by boost.\n        :param boost_y: the y-value of the point parabola returned by boost.\n        :param focus: the focus point used for solving the equation of the parabola.\n        :param directix: the directix value used for solving the equation of the parabola.\n\t\t:param tolerance: the distance allowed between the point computed by boost and the point computed by the equation.\n\t\t:return: the point on the parabola computed using the value of boost_x.\n\t\t");
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_56CheckUnsolvableParabolaEquation = {"CheckUnsolvableParabolaEquation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_56CheckUnsolvableParabolaEquation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_55CheckUnsolvableParabolaEquation};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_56CheckUnsolvableParabolaEquation(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_boost_x = 0;
@@ -11685,60 +12233,60 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boost_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boost_y)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 1); __PYX_ERR(0, 415, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 1); __PYX_ERR(0, 418, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_focus)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 2); __PYX_ERR(0, 415, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 2); __PYX_ERR(0, 418, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_directix)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 3); __PYX_ERR(0, 415, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 3); __PYX_ERR(0, 418, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_tolerance)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 4); __PYX_ERR(0, 415, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, 4); __PYX_ERR(0, 418, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "CheckUnsolvableParabolaEquation") < 0)) __PYX_ERR(0, 415, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "CheckUnsolvableParabolaEquation") < 0)) __PYX_ERR(0, 418, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -11749,42 +12297,42 @@
     __pyx_v_boost_y = values[1];
     __pyx_v_focus = values[2];
     __pyx_v_directix = values[3];
     __pyx_v_tolerance = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 415, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("CheckUnsolvableParabolaEquation", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 418, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.CheckUnsolvableParabolaEquation", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_46CheckUnsolvableParabolaEquation(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_boost_x, __pyx_v_boost_y, __pyx_v_focus, __pyx_v_directix, __pyx_v_tolerance);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_55CheckUnsolvableParabolaEquation(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_boost_x, __pyx_v_boost_y, __pyx_v_focus, __pyx_v_directix, __pyx_v_tolerance);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_46CheckUnsolvableParabolaEquation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_boost_x, PyObject *__pyx_v_boost_y, PyObject *__pyx_v_focus, PyObject *__pyx_v_directix, PyObject *__pyx_v_tolerance) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_55CheckUnsolvableParabolaEquation(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_boost_x, PyObject *__pyx_v_boost_y, PyObject *__pyx_v_focus, PyObject *__pyx_v_directix, PyObject *__pyx_v_tolerance) {
   PyObject *__pyx_v_computed_point_y = NULL;
   PyObject *__pyx_v_delta = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -11793,22 +12341,22 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("CheckUnsolvableParabolaEquation", 1);
 
-  /* "pyvoronoi.pyx":427
+  /* "pyvoronoi.pyx":430
  * 		:return: the point on the parabola computed using the value of boost_x.
  * 		"""
  *         computed_point_y = self.GetParabolaY(boost_x, focus, directix)             # <<<<<<<<<<<<<<
  *         delta = computed_point_y - boost_y if computed_point_y > boost_y else boost_y - computed_point_y
  *         if delta > tolerance:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetParabolaY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetParabolaY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -11820,67 +12368,67 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_v_boost_x, __pyx_v_focus, __pyx_v_directix};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_computed_point_y = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":428
+  /* "pyvoronoi.pyx":431
  * 		"""
  *         computed_point_y = self.GetParabolaY(boost_x, focus, directix)
  *         delta = computed_point_y - boost_y if computed_point_y > boost_y else boost_y - computed_point_y             # <<<<<<<<<<<<<<
  *         if delta > tolerance:
  *             raise UnsolvableParabolaEquation("The computed Y on the parabola for the starting / ending point is different from the rotated point returned by Boost. Difference: {0}. Maximum tolerance: {1}".format(delta, tolerance))
  */
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_computed_point_y, __pyx_v_boost_y, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_computed_point_y, __pyx_v_boost_y, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
-    __pyx_t_2 = PyNumber_Subtract(__pyx_v_computed_point_y, __pyx_v_boost_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(__pyx_v_computed_point_y, __pyx_v_boost_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
-    __pyx_t_2 = PyNumber_Subtract(__pyx_v_boost_y, __pyx_v_computed_point_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(__pyx_v_boost_y, __pyx_v_computed_point_y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   }
   __pyx_v_delta = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyvoronoi.pyx":429
+  /* "pyvoronoi.pyx":432
  *         computed_point_y = self.GetParabolaY(boost_x, focus, directix)
  *         delta = computed_point_y - boost_y if computed_point_y > boost_y else boost_y - computed_point_y
  *         if delta > tolerance:             # <<<<<<<<<<<<<<
  *             raise UnsolvableParabolaEquation("The computed Y on the parabola for the starting / ending point is different from the rotated point returned by Boost. Difference: {0}. Maximum tolerance: {1}".format(delta, tolerance))
  *         return [boost_x, computed_point_y]
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_delta, __pyx_v_tolerance, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_delta, __pyx_v_tolerance, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_5)) {
 
-    /* "pyvoronoi.pyx":430
+    /* "pyvoronoi.pyx":433
  *         delta = computed_point_y - boost_y if computed_point_y > boost_y else boost_y - computed_point_y
  *         if delta > tolerance:
  *             raise UnsolvableParabolaEquation("The computed Y on the parabola for the starting / ending point is different from the rotated point returned by Boost. Difference: {0}. Maximum tolerance: {1}".format(delta, tolerance))             # <<<<<<<<<<<<<<
  *         return [boost_x, computed_point_y]
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnsolvableParabolaEquation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnsolvableParabolaEquation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_The_computed_Y_on_the_parabola_f, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 430, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_The_computed_Y_on_the_parabola_f, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
@@ -11892,15 +12440,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_7, __pyx_v_delta, __pyx_v_tolerance};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_t_6 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -11915,52 +12463,52 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_3};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 430, __pyx_L1_error)
+    __PYX_ERR(0, 433, __pyx_L1_error)
 
-    /* "pyvoronoi.pyx":429
+    /* "pyvoronoi.pyx":432
  *         computed_point_y = self.GetParabolaY(boost_x, focus, directix)
  *         delta = computed_point_y - boost_y if computed_point_y > boost_y else boost_y - computed_point_y
  *         if delta > tolerance:             # <<<<<<<<<<<<<<
  *             raise UnsolvableParabolaEquation("The computed Y on the parabola for the starting / ending point is different from the rotated point returned by Boost. Difference: {0}. Maximum tolerance: {1}".format(delta, tolerance))
  *         return [boost_x, computed_point_y]
  */
   }
 
-  /* "pyvoronoi.pyx":431
+  /* "pyvoronoi.pyx":434
  *         if delta > tolerance:
  *             raise UnsolvableParabolaEquation("The computed Y on the parabola for the starting / ending point is different from the rotated point returned by Boost. Difference: {0}. Maximum tolerance: {1}".format(delta, tolerance))
  *         return [boost_x, computed_point_y]             # <<<<<<<<<<<<<<
  * 
  *     def Discretize(self, point, segment, parabola_start, parabola_end, max_dist, parabola_equation_tolerance):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_boost_x);
   __Pyx_GIVEREF(__pyx_v_boost_x);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_boost_x)) __PYX_ERR(0, 431, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_boost_x)) __PYX_ERR(0, 434, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_computed_point_y);
   __Pyx_GIVEREF(__pyx_v_computed_point_y);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_v_computed_point_y)) __PYX_ERR(0, 431, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 1, __pyx_v_computed_point_y)) __PYX_ERR(0, 434, __pyx_L1_error);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":415
+  /* "pyvoronoi.pyx":418
  *         return (pow(x - focus[0], 2) + pow(focus[1], 2) - pow(directrix_y, 2)) / (2 * (focus[1] - directrix_y));
  * 
  *     def CheckUnsolvableParabolaEquation(self, boost_x, boost_y, focus, directix, tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Compare the y-coordinate of a point on the parabola returned by Boost with the computed value.
  */
 
@@ -11977,33 +12525,33 @@
   __Pyx_XDECREF(__pyx_v_computed_point_y);
   __Pyx_XDECREF(__pyx_v_delta);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":433
+/* "pyvoronoi.pyx":436
  *         return [boost_x, computed_point_y]
  * 
  *     def Discretize(self, point, segment, parabola_start, parabola_end, max_dist, parabola_equation_tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_49Discretize(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_58Discretize(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_48Discretize, "\n        Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.\n        :param point: The input point associated with the cell or the neighbour cell. The point is used as the focus in the equation of the parabola.\n        :param segment: The input segment associated with the cell or the neighbour cell. The point is used as the directix in the equation of the parabola.\n        :param max dist: The maximum distance between 2 vertices on the discretized geometry.\n        :param parabola_equation_tolerance: The maximum difference allowed between the y coordinate returned by Boost, and the equation of the parabola.\n\t\t:return: the list of points on the parabola.\n\t\t");
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_49Discretize = {"Discretize", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_49Discretize, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_48Discretize};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_49Discretize(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_9pyvoronoi_9Pyvoronoi_57Discretize, "\n        Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.\n        :param point: The input point associated with the cell or the neighbour cell. The point is used as the focus in the equation of the parabola.\n        :param segment: The input segment associated with the cell or the neighbour cell. The point is used as the directix in the equation of the parabola.\n        :param max dist: The maximum distance between 2 vertices on the discretized geometry.\n        :param parabola_equation_tolerance: The maximum difference allowed between the y coordinate returned by Boost, and the equation of the parabola.\n\t\t:return: the list of points on the parabola.\n\t\t");
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_58Discretize = {"Discretize", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_58Discretize, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_57Discretize};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_58Discretize(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_point = 0;
@@ -12054,70 +12602,70 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_segment)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 1); __PYX_ERR(0, 433, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 1); __PYX_ERR(0, 436, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parabola_start)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 2); __PYX_ERR(0, 433, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 2); __PYX_ERR(0, 436, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parabola_end)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 3); __PYX_ERR(0, 433, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 3); __PYX_ERR(0, 436, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_dist)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 4); __PYX_ERR(0, 433, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 4); __PYX_ERR(0, 436, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parabola_equation_tolerance)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 5); __PYX_ERR(0, 433, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, 5); __PYX_ERR(0, 436, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Discretize") < 0)) __PYX_ERR(0, 433, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Discretize") < 0)) __PYX_ERR(0, 436, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 6)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -12130,42 +12678,42 @@
     __pyx_v_parabola_start = values[2];
     __pyx_v_parabola_end = values[3];
     __pyx_v_max_dist = values[4];
     __pyx_v_parabola_equation_tolerance = values[5];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, __pyx_nargs); __PYX_ERR(0, 433, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Discretize", 1, 6, 6, __pyx_nargs); __PYX_ERR(0, 436, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.Discretize", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_48Discretize(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_point, __pyx_v_segment, __pyx_v_parabola_start, __pyx_v_parabola_end, __pyx_v_max_dist, __pyx_v_parabola_equation_tolerance);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_57Discretize(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v_point, __pyx_v_segment, __pyx_v_parabola_start, __pyx_v_parabola_end, __pyx_v_max_dist, __pyx_v_parabola_equation_tolerance);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":505
+/* "pyvoronoi.pyx":508
  *         #Unrotate the computed intermediate points
  * 		###############################
  *         densified = map(lambda x: Unrotate(x, angle, shift_x, shift_y), densified_rotated)             # <<<<<<<<<<<<<<
  *         return densified
  * 
  */
 
@@ -12218,31 +12766,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 505, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 508, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 505, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 508, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_x = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 505, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 508, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -12262,34 +12810,34 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_lambda_funcdef_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x) {
-  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *__pyx_cur_scope;
-  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *__pyx_outer_scope;
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *__pyx_cur_scope;
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 1);
-  __pyx_outer_scope = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *) __Pyx_CyFunction_GetClosure(__pyx_self);
+  __pyx_outer_scope = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Unrotate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Unrotate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (unlikely(!__pyx_cur_scope->__pyx_v_angle)) { __Pyx_RaiseClosureNameError("angle"); __PYX_ERR(0, 505, __pyx_L1_error) }
-  if (unlikely(!__pyx_cur_scope->__pyx_v_shift_x)) { __Pyx_RaiseClosureNameError("shift_x"); __PYX_ERR(0, 505, __pyx_L1_error) }
-  if (unlikely(!__pyx_cur_scope->__pyx_v_shift_y)) { __Pyx_RaiseClosureNameError("shift_y"); __PYX_ERR(0, 505, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_angle)) { __Pyx_RaiseClosureNameError("angle"); __PYX_ERR(0, 508, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_shift_x)) { __Pyx_RaiseClosureNameError("shift_x"); __PYX_ERR(0, 508, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_shift_y)) { __Pyx_RaiseClosureNameError("shift_y"); __PYX_ERR(0, 508, __pyx_L1_error) }
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12300,15 +12848,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_3, __pyx_v_x, __pyx_cur_scope->__pyx_v_angle, __pyx_cur_scope->__pyx_v_shift_x, __pyx_cur_scope->__pyx_v_shift_y};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 4+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 505, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -12321,24 +12869,24 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":433
+/* "pyvoronoi.pyx":436
  *         return [boost_x, computed_point_y]
  * 
  *     def Discretize(self, point, segment, parabola_start, parabola_end, max_dist, parabola_equation_tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.
  */
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_48Discretize(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_point, PyObject *__pyx_v_segment, PyObject *__pyx_v_parabola_start, PyObject *__pyx_v_parabola_end, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance) {
-  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *__pyx_cur_scope;
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_57Discretize(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_point, PyObject *__pyx_v_segment, PyObject *__pyx_v_parabola_start, PyObject *__pyx_v_parabola_end, PyObject *__pyx_v_max_dist, PyObject *__pyx_v_parabola_equation_tolerance) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *__pyx_cur_scope;
   PyObject *__pyx_v_focus_rotated = NULL;
   PyObject *__pyx_v_directix_start_rotated = NULL;
   CYTHON_UNUSED PyObject *__pyx_v_directix_end_rotated = NULL;
   PyObject *__pyx_v_parabola_start_rotated = NULL;
   PyObject *__pyx_v_parabola_end_rotated = NULL;
   PyObject *__pyx_v_directix = NULL;
   PyObject *__pyx_v_parabola_start_rotated_check = NULL;
@@ -12365,105 +12913,105 @@
   PyObject *__pyx_t_10 = NULL;
   Py_ssize_t __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Discretize", 0);
-  __pyx_cur_scope = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct__Discretize(__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct_3_Discretize(__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 433, __pyx_L1_error)
+    __PYX_ERR(0, 436, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
 
-  /* "pyvoronoi.pyx":444
+  /* "pyvoronoi.pyx":447
  * 
  * 		#Test if the input point is on the input line. If yes, it is impossible to compute a parabola.
  *         if(point[0] == segment[0][0] and point[1] == segment[0][1]) or (point[0] == segment[1][0] and point[1] == segment[1][1]):             # <<<<<<<<<<<<<<
  *             raise FocusOnDirectixException()
  * 
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (!__pyx_t_5) {
     goto __pyx_L5_next_or;
   } else {
   }
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_1 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_L5_next_or:;
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
   } else {
     __pyx_t_1 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_1 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyvoronoi.pyx":445
+    /* "pyvoronoi.pyx":448
  * 		#Test if the input point is on the input line. If yes, it is impossible to compute a parabola.
  *         if(point[0] == segment[0][0] and point[1] == segment[0][1]) or (point[0] == segment[1][0] and point[1] == segment[1][1]):
  *             raise FocusOnDirectixException()             # <<<<<<<<<<<<<<
  * 
  * 		###############################
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FocusOnDirectixException); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FocusOnDirectixException); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_2)) {
@@ -12475,50 +13023,50 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 445, __pyx_L1_error)
+    __PYX_ERR(0, 448, __pyx_L1_error)
 
-    /* "pyvoronoi.pyx":444
+    /* "pyvoronoi.pyx":447
  * 
  * 		#Test if the input point is on the input line. If yes, it is impossible to compute a parabola.
  *         if(point[0] == segment[0][0] and point[1] == segment[0][1]) or (point[0] == segment[1][0] and point[1] == segment[1][1]):             # <<<<<<<<<<<<<<
  *             raise FocusOnDirectixException()
  * 
  */
   }
 
-  /* "pyvoronoi.pyx":454
+  /* "pyvoronoi.pyx":457
  * 		#Input segment becomes the directix of the parabola equation.
  * 		###############################
  *         shift_x = min(segment[0][0], segment[1][0])             # <<<<<<<<<<<<<<
  *         shift_y = min(segment[0][1], segment[1][1])
  *         angle = GetLineAngleInRadians(
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 454, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
   } else {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_3 = __pyx_t_2;
@@ -12528,33 +13076,33 @@
   __pyx_t_4 = __pyx_t_3;
   __Pyx_INCREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_cur_scope->__pyx_v_shift_x = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":455
+  /* "pyvoronoi.pyx":458
  * 		###############################
  *         shift_x = min(segment[0][0], segment[1][0])
  *         shift_y = min(segment[0][1], segment[1][1])             # <<<<<<<<<<<<<<
  *         angle = GetLineAngleInRadians(
  *             segment[0][0],
  */
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 455, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_t_3);
     __pyx_t_4 = __pyx_t_3;
   } else {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_4 = __pyx_t_2;
@@ -12564,73 +13112,73 @@
   __pyx_t_3 = __pyx_t_4;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_cur_scope->__pyx_v_shift_y = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":456
+  /* "pyvoronoi.pyx":459
  *         shift_x = min(segment[0][0], segment[1][0])
  *         shift_y = min(segment[0][1], segment[1][1])
  *         angle = GetLineAngleInRadians(             # <<<<<<<<<<<<<<
  *             segment[0][0],
  *             segment[0][1],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_GetLineAngleInRadians); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 456, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_GetLineAngleInRadians); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "pyvoronoi.pyx":457
+  /* "pyvoronoi.pyx":460
  *         shift_y = min(segment[0][1], segment[1][1])
  *         angle = GetLineAngleInRadians(
  *             segment[0][0],             # <<<<<<<<<<<<<<
  *             segment[0][1],
  *             segment[1][0],
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":458
+  /* "pyvoronoi.pyx":461
  *         angle = GetLineAngleInRadians(
  *             segment[0][0],
  *             segment[0][1],             # <<<<<<<<<<<<<<
  *             segment[1][0],
  *             segment[1][1],
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":459
+  /* "pyvoronoi.pyx":462
  *             segment[0][0],
  *             segment[0][1],
  *             segment[1][0],             # <<<<<<<<<<<<<<
  *             segment[1][1],
  *         )
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":460
+  /* "pyvoronoi.pyx":463
  *             segment[0][1],
  *             segment[1][0],
  *             segment[1][1],             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
@@ -12647,30 +13195,30 @@
     PyObject *__pyx_callargs[5] = {__pyx_t_2, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 456, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_cur_scope->__pyx_v_angle = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":463
+  /* "pyvoronoi.pyx":466
  *         )
  * 
  *         focus_rotated = RotateWithShift(point, angle, shift_x, shift_y)             # <<<<<<<<<<<<<<
  *         directix_start_rotated = RotateWithShift(segment[0], angle, shift_x, shift_y)
  *         directix_end_rotated = RotateWithShift(segment[1], angle, shift_x, shift_y)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_10 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_10)) {
@@ -12682,31 +13230,31 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_10, __pyx_v_point, __pyx_cur_scope->__pyx_v_angle, __pyx_cur_scope->__pyx_v_shift_x, __pyx_cur_scope->__pyx_v_shift_y};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 463, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_focus_rotated = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":464
+  /* "pyvoronoi.pyx":467
  * 
  *         focus_rotated = RotateWithShift(point, angle, shift_x, shift_y)
  *         directix_start_rotated = RotateWithShift(segment[0], angle, shift_x, shift_y)             # <<<<<<<<<<<<<<
  *         directix_end_rotated = RotateWithShift(segment[1], angle, shift_x, shift_y)
  *         parabola_start_rotated = RotateWithShift(parabola_start, angle, shift_x, shift_y)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_9 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_9)) {
@@ -12719,31 +13267,31 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_9, __pyx_t_10, __pyx_cur_scope->__pyx_v_angle, __pyx_cur_scope->__pyx_v_shift_x, __pyx_cur_scope->__pyx_v_shift_y};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_directix_start_rotated = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":465
+  /* "pyvoronoi.pyx":468
  *         focus_rotated = RotateWithShift(point, angle, shift_x, shift_y)
  *         directix_start_rotated = RotateWithShift(segment[0], angle, shift_x, shift_y)
  *         directix_end_rotated = RotateWithShift(segment[1], angle, shift_x, shift_y)             # <<<<<<<<<<<<<<
  *         parabola_start_rotated = RotateWithShift(parabola_start, angle, shift_x, shift_y)
  *         parabola_end_rotated = RotateWithShift(parabola_end, angle, shift_x, shift_y)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_9 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_9)) {
@@ -12756,29 +13304,29 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_9, __pyx_t_10, __pyx_cur_scope->__pyx_v_angle, __pyx_cur_scope->__pyx_v_shift_x, __pyx_cur_scope->__pyx_v_shift_y};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_directix_end_rotated = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":466
+  /* "pyvoronoi.pyx":469
  *         directix_start_rotated = RotateWithShift(segment[0], angle, shift_x, shift_y)
  *         directix_end_rotated = RotateWithShift(segment[1], angle, shift_x, shift_y)
  *         parabola_start_rotated = RotateWithShift(parabola_start, angle, shift_x, shift_y)             # <<<<<<<<<<<<<<
  *         parabola_end_rotated = RotateWithShift(parabola_end, angle, shift_x, shift_y)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_10 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_10)) {
@@ -12790,29 +13338,29 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_10, __pyx_v_parabola_start, __pyx_cur_scope->__pyx_v_angle, __pyx_cur_scope->__pyx_v_shift_x, __pyx_cur_scope->__pyx_v_shift_y};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_parabola_start_rotated = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":467
+  /* "pyvoronoi.pyx":470
  *         directix_end_rotated = RotateWithShift(segment[1], angle, shift_x, shift_y)
  *         parabola_start_rotated = RotateWithShift(parabola_start, angle, shift_x, shift_y)
  *         parabola_end_rotated = RotateWithShift(parabola_end, angle, shift_x, shift_y)             # <<<<<<<<<<<<<<
  * 
  * 		###############################
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RotateWithShift); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_10 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_10)) {
@@ -12824,45 +13372,45 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_10, __pyx_v_parabola_end, __pyx_cur_scope->__pyx_v_angle, __pyx_cur_scope->__pyx_v_shift_x, __pyx_cur_scope->__pyx_v_shift_y};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 467, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_parabola_end_rotated = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":474
+  /* "pyvoronoi.pyx":477
  * 		#Boost
  * 		###############################
  *         directix = directix_start_rotated[1]             # <<<<<<<<<<<<<<
  *         parabola_start_rotated_check = self.CheckUnsolvableParabolaEquation(parabola_start_rotated[0], parabola_start_rotated[1], focus_rotated, directix, parabola_equation_tolerance)
  *         parabola_end_rotated_check = self.CheckUnsolvableParabolaEquation(parabola_end_rotated[0], parabola_end_rotated[1], focus_rotated, directix, parabola_equation_tolerance)
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_directix_start_rotated, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_directix_start_rotated, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_directix = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":475
+  /* "pyvoronoi.pyx":478
  * 		###############################
  *         directix = directix_start_rotated[1]
  *         parabola_start_rotated_check = self.CheckUnsolvableParabolaEquation(parabola_start_rotated[0], parabola_start_rotated[1], focus_rotated, directix, parabola_equation_tolerance)             # <<<<<<<<<<<<<<
  *         parabola_end_rotated_check = self.CheckUnsolvableParabolaEquation(parabola_end_rotated[0], parabola_end_rotated[1], focus_rotated, directix, parabola_equation_tolerance)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CheckUnsolvableParabolaEquation); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CheckUnsolvableParabolaEquation); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_parabola_start_rotated, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_parabola_start_rotated, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_parabola_start_rotated, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_parabola_start_rotated, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_8 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_8)) {
@@ -12876,33 +13424,33 @@
   #endif
   {
     PyObject *__pyx_callargs[6] = {__pyx_t_8, __pyx_t_10, __pyx_t_9, __pyx_v_focus_rotated, __pyx_v_directix, __pyx_v_parabola_equation_tolerance};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 5+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 475, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_parabola_start_rotated_check = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":476
+  /* "pyvoronoi.pyx":479
  *         directix = directix_start_rotated[1]
  *         parabola_start_rotated_check = self.CheckUnsolvableParabolaEquation(parabola_start_rotated[0], parabola_start_rotated[1], focus_rotated, directix, parabola_equation_tolerance)
  *         parabola_end_rotated_check = self.CheckUnsolvableParabolaEquation(parabola_end_rotated[0], parabola_end_rotated[1], focus_rotated, directix, parabola_equation_tolerance)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CheckUnsolvableParabolaEquation); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CheckUnsolvableParabolaEquation); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_parabola_end_rotated, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_parabola_end_rotated, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_parabola_end_rotated, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_parabola_end_rotated, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_8 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_8)) {
@@ -12916,95 +13464,95 @@
   #endif
   {
     PyObject *__pyx_callargs[6] = {__pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_v_focus_rotated, __pyx_v_directix, __pyx_v_parabola_equation_tolerance};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 5+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 479, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_parabola_end_rotated_check = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":482
+  /* "pyvoronoi.pyx":485
  *         #Compute the intermediate points
  * 		###############################
  *         densified_rotated  = [parabola_start_rotated_check]             # <<<<<<<<<<<<<<
  *         previous = densified_rotated[0]
  *         next  = [parabola_end_rotated_check]
  */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_parabola_start_rotated_check);
   __Pyx_GIVEREF(__pyx_v_parabola_start_rotated_check);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_parabola_start_rotated_check)) __PYX_ERR(0, 482, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_parabola_start_rotated_check)) __PYX_ERR(0, 485, __pyx_L1_error);
   __pyx_v_densified_rotated = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":483
+  /* "pyvoronoi.pyx":486
  * 		###############################
  *         densified_rotated  = [parabola_start_rotated_check]
  *         previous = densified_rotated[0]             # <<<<<<<<<<<<<<
  *         next  = [parabola_end_rotated_check]
  * 
  */
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_densified_rotated, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_densified_rotated, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_previous = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":484
+  /* "pyvoronoi.pyx":487
  *         densified_rotated  = [parabola_start_rotated_check]
  *         previous = densified_rotated[0]
  *         next  = [parabola_end_rotated_check]             # <<<<<<<<<<<<<<
  * 
  *         while (len(next) > 0):
  */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_parabola_end_rotated_check);
   __Pyx_GIVEREF(__pyx_v_parabola_end_rotated_check);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_parabola_end_rotated_check)) __PYX_ERR(0, 484, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_parabola_end_rotated_check)) __PYX_ERR(0, 487, __pyx_L1_error);
   __pyx_v_next = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":486
+  /* "pyvoronoi.pyx":489
  *         next  = [parabola_end_rotated_check]
  * 
  *         while (len(next) > 0):             # <<<<<<<<<<<<<<
  *             current = next[-1]
  *             distance = Distance(current, previous)
  */
   while (1) {
-    __pyx_t_11 = __Pyx_PyList_GET_SIZE(__pyx_v_next); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 486, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyList_GET_SIZE(__pyx_v_next); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 489, __pyx_L1_error)
     __pyx_t_1 = (__pyx_t_11 > 0);
     if (!__pyx_t_1) break;
 
-    /* "pyvoronoi.pyx":487
+    /* "pyvoronoi.pyx":490
  * 
  *         while (len(next) > 0):
  *             current = next[-1]             # <<<<<<<<<<<<<<
  *             distance = Distance(current, previous)
  * 
  */
-    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_next, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_next, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_current, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "pyvoronoi.pyx":488
+    /* "pyvoronoi.pyx":491
  *         while (len(next) > 0):
  *             current = next[-1]
  *             distance = Distance(current, previous)             # <<<<<<<<<<<<<<
  * 
  *             if distance > max_dist:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Distance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Distance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_10)) {
@@ -13016,62 +13564,62 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_10, __pyx_v_current, __pyx_v_previous};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 488, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_distance, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "pyvoronoi.pyx":490
+    /* "pyvoronoi.pyx":493
  *             distance = Distance(current, previous)
  * 
  *             if distance > max_dist:             # <<<<<<<<<<<<<<
  *                 mid_point_x = (previous[0] + current[0]) / 2
  *                 mid_point = [mid_point_x, self.GetParabolaY(mid_point_x, focus_rotated, directix)]
  */
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_distance, __pyx_v_max_dist, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_distance, __pyx_v_max_dist, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_1) {
 
-      /* "pyvoronoi.pyx":491
+      /* "pyvoronoi.pyx":494
  * 
  *             if distance > max_dist:
  *                 mid_point_x = (previous[0] + current[0]) / 2             # <<<<<<<<<<<<<<
  *                 mid_point = [mid_point_x, self.GetParabolaY(mid_point_x, focus_rotated, directix)]
  *                 next.append(mid_point)
  */
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_previous, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_previous, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_current, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_current, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_10 = PyNumber_Add(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 491, __pyx_L1_error)
+      __pyx_t_10 = PyNumber_Add(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 494, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_10, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_10, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF_SET(__pyx_v_mid_point_x, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "pyvoronoi.pyx":492
+      /* "pyvoronoi.pyx":495
  *             if distance > max_dist:
  *                 mid_point_x = (previous[0] + current[0]) / 2
  *                 mid_point = [mid_point_x, self.GetParabolaY(mid_point_x, focus_rotated, directix)]             # <<<<<<<<<<<<<<
  *                 next.append(mid_point)
  *             else:
  */
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetParabolaY); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 492, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetParabolaY); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 495, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_3 = NULL;
       __pyx_t_6 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_3)) {
@@ -13083,136 +13631,136 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_v_mid_point_x, __pyx_v_focus_rotated, __pyx_v_directix};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_6, 3+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
-      __pyx_t_10 = PyList_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 492, __pyx_L1_error)
+      __pyx_t_10 = PyList_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 495, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_INCREF(__pyx_v_mid_point_x);
       __Pyx_GIVEREF(__pyx_v_mid_point_x);
-      if (__Pyx_PyList_SET_ITEM(__pyx_t_10, 0, __pyx_v_mid_point_x)) __PYX_ERR(0, 492, __pyx_L1_error);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_10, 0, __pyx_v_mid_point_x)) __PYX_ERR(0, 495, __pyx_L1_error);
       __Pyx_GIVEREF(__pyx_t_4);
-      if (__Pyx_PyList_SET_ITEM(__pyx_t_10, 1, __pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_10, 1, __pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error);
       __pyx_t_4 = 0;
       __Pyx_XDECREF_SET(__pyx_v_mid_point, ((PyObject*)__pyx_t_10));
       __pyx_t_10 = 0;
 
-      /* "pyvoronoi.pyx":493
+      /* "pyvoronoi.pyx":496
  *                 mid_point_x = (previous[0] + current[0]) / 2
  *                 mid_point = [mid_point_x, self.GetParabolaY(mid_point_x, focus_rotated, directix)]
  *                 next.append(mid_point)             # <<<<<<<<<<<<<<
  *             else:
  *                 densified_rotated.append(current)
  */
-      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_next, __pyx_v_mid_point); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 493, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_next, __pyx_v_mid_point); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 496, __pyx_L1_error)
 
-      /* "pyvoronoi.pyx":490
+      /* "pyvoronoi.pyx":493
  *             distance = Distance(current, previous)
  * 
  *             if distance > max_dist:             # <<<<<<<<<<<<<<
  *                 mid_point_x = (previous[0] + current[0]) / 2
  *                 mid_point = [mid_point_x, self.GetParabolaY(mid_point_x, focus_rotated, directix)]
  */
       goto __pyx_L10;
     }
 
-    /* "pyvoronoi.pyx":495
+    /* "pyvoronoi.pyx":498
  *                 next.append(mid_point)
  *             else:
  *                 densified_rotated.append(current)             # <<<<<<<<<<<<<<
  *                 next.pop()
  *                 previous = current
  */
     /*else*/ {
-      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_densified_rotated, __pyx_v_current); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 495, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_densified_rotated, __pyx_v_current); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 498, __pyx_L1_error)
 
-      /* "pyvoronoi.pyx":496
+      /* "pyvoronoi.pyx":499
  *             else:
  *                 densified_rotated.append(current)
  *                 next.pop()             # <<<<<<<<<<<<<<
  *                 previous = current
  * 
  */
-      __pyx_t_10 = __Pyx_PyList_Pop(__pyx_v_next); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 496, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyList_Pop(__pyx_v_next); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 499, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-      /* "pyvoronoi.pyx":497
+      /* "pyvoronoi.pyx":500
  *                 densified_rotated.append(current)
  *                 next.pop()
  *                 previous = current             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __Pyx_INCREF(__pyx_v_current);
       __Pyx_DECREF_SET(__pyx_v_previous, __pyx_v_current);
     }
     __pyx_L10:;
   }
 
-  /* "pyvoronoi.pyx":500
+  /* "pyvoronoi.pyx":503
  * 
  * 
  *         densified_rotated[0] = parabola_start_rotated             # <<<<<<<<<<<<<<
  *         densified_rotated[-1] = parabola_end_rotated
  * 		###############################
  */
-  if (unlikely((__Pyx_SetItemInt(__pyx_v_densified_rotated, 0, __pyx_v_parabola_start_rotated, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0))) __PYX_ERR(0, 500, __pyx_L1_error)
+  if (unlikely((__Pyx_SetItemInt(__pyx_v_densified_rotated, 0, __pyx_v_parabola_start_rotated, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0))) __PYX_ERR(0, 503, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":501
+  /* "pyvoronoi.pyx":504
  * 
  *         densified_rotated[0] = parabola_start_rotated
  *         densified_rotated[-1] = parabola_end_rotated             # <<<<<<<<<<<<<<
  * 		###############################
  *         #Unrotate the computed intermediate points
  */
-  if (unlikely((__Pyx_SetItemInt(__pyx_v_densified_rotated, -1L, __pyx_v_parabola_end_rotated, long, 1, __Pyx_PyInt_From_long, 1, 1, 1) < 0))) __PYX_ERR(0, 501, __pyx_L1_error)
+  if (unlikely((__Pyx_SetItemInt(__pyx_v_densified_rotated, -1L, __pyx_v_parabola_end_rotated, long, 1, __Pyx_PyInt_From_long, 1, 1, 1) < 0))) __PYX_ERR(0, 504, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":505
+  /* "pyvoronoi.pyx":508
  *         #Unrotate the computed intermediate points
  * 		###############################
  *         densified = map(lambda x: Unrotate(x, angle, shift_x, shift_y), densified_rotated)             # <<<<<<<<<<<<<<
  *         return densified
  * 
  */
-  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_10Discretize_lambda, 0, __pyx_n_s_Discretize_locals_lambda, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pyvoronoi, __pyx_d, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_10Discretize_lambda, 0, __pyx_n_s_Discretize_locals_lambda, ((PyObject*)__pyx_cur_scope), __pyx_n_s_pyvoronoi, __pyx_d, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_10);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_10)) __PYX_ERR(0, 505, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_10)) __PYX_ERR(0, 508, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_densified_rotated);
   __Pyx_GIVEREF(__pyx_v_densified_rotated);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_densified_rotated)) __PYX_ERR(0, 505, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_densified_rotated)) __PYX_ERR(0, 508, __pyx_L1_error);
   __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_4, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_4, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_densified = __pyx_t_10;
   __pyx_t_10 = 0;
 
-  /* "pyvoronoi.pyx":506
+  /* "pyvoronoi.pyx":509
  * 		###############################
  *         densified = map(lambda x: Unrotate(x, angle, shift_x, shift_y), densified_rotated)
  *         return densified             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_densified);
   __pyx_r = __pyx_v_densified;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":433
+  /* "pyvoronoi.pyx":436
  *         return [boost_x, computed_point_y]
  * 
  *     def Discretize(self, point, segment, parabola_start, parabola_end, max_dist, parabola_equation_tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.
  */
 
@@ -13246,15 +13794,15 @@
   __Pyx_XDECREF(__pyx_v_densified);
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":509
+/* "pyvoronoi.pyx":512
  * 
  * 
  *     cdef Segment _to_voronoi_segment(self, object py_segment):             # <<<<<<<<<<<<<<
  *         return Segment(self._to_voronoi_point(py_segment[0]), self._to_voronoi_point(py_segment[1]))
  * 
  */
 
@@ -13265,35 +13813,35 @@
   PyObject *__pyx_t_2 = NULL;
   struct Point __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_to_voronoi_segment", 1);
 
-  /* "pyvoronoi.pyx":510
+  /* "pyvoronoi.pyx":513
  * 
  *     cdef Segment _to_voronoi_segment(self, object py_segment):
  *         return Segment(self._to_voronoi_point(py_segment[0]), self._to_voronoi_point(py_segment[1]))             # <<<<<<<<<<<<<<
  * 
  *     cdef Point _to_voronoi_point(self, object py_point):
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_segment, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_point(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_point(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1.p0 = __pyx_t_3;
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_segment, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_point(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_point(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1.p1 = __pyx_t_3;
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":509
+  /* "pyvoronoi.pyx":512
  * 
  * 
  *     cdef Segment _to_voronoi_segment(self, object py_segment):             # <<<<<<<<<<<<<<
  *         return Segment(self._to_voronoi_point(py_segment[0]), self._to_voronoi_point(py_segment[1]))
  * 
  */
 
@@ -13303,15 +13851,15 @@
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi._to_voronoi_segment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":512
+/* "pyvoronoi.pyx":515
  *         return Segment(self._to_voronoi_point(py_segment[0]), self._to_voronoi_point(py_segment[1]))
  * 
  *     cdef Point _to_voronoi_point(self, object py_point):             # <<<<<<<<<<<<<<
  *         return Point(self._to_voronoi_int(py_point[0]), self._to_voronoi_int(py_point[1]))
  * 
  */
 
@@ -13322,35 +13870,35 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_to_voronoi_point", 1);
 
-  /* "pyvoronoi.pyx":513
+  /* "pyvoronoi.pyx":516
  * 
  *     cdef Point _to_voronoi_point(self, object py_point):
  *         return Point(self._to_voronoi_int(py_point[0]), self._to_voronoi_int(py_point[1]))             # <<<<<<<<<<<<<<
  * 
  *     cdef int _to_voronoi_int(self, val):
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_point, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_int(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_int(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1.X = __pyx_t_3;
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_py_point, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_int(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_9pyvoronoi_Pyvoronoi *)__pyx_v_self->__pyx_vtab)->_to_voronoi_int(__pyx_v_self, __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1.Y = __pyx_t_3;
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":512
+  /* "pyvoronoi.pyx":515
  *         return Segment(self._to_voronoi_point(py_segment[0]), self._to_voronoi_point(py_segment[1]))
  * 
  *     cdef Point _to_voronoi_point(self, object py_point):             # <<<<<<<<<<<<<<
  *         return Point(self._to_voronoi_int(py_point[0]), self._to_voronoi_int(py_point[1]))
  * 
  */
 
@@ -13360,15 +13908,15 @@
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi._to_voronoi_point", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":515
+/* "pyvoronoi.pyx":518
  *         return Point(self._to_voronoi_int(py_point[0]), self._to_voronoi_int(py_point[1]))
  * 
  *     cdef int _to_voronoi_int(self, val):             # <<<<<<<<<<<<<<
  *         return val * self.SCALING_FACTOR
  * 
  */
 
@@ -13379,32 +13927,32 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_to_voronoi_int", 1);
 
-  /* "pyvoronoi.pyx":516
+  /* "pyvoronoi.pyx":519
  * 
  *     cdef int _to_voronoi_int(self, val):
  *         return val * self.SCALING_FACTOR             # <<<<<<<<<<<<<<
  * 
  *     cdef double _to_voronoi_double(self, val):
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_v_val, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_v_val, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":515
+  /* "pyvoronoi.pyx":518
  *         return Point(self._to_voronoi_int(py_point[0]), self._to_voronoi_int(py_point[1]))
  * 
  *     cdef int _to_voronoi_int(self, val):             # <<<<<<<<<<<<<<
  *         return val * self.SCALING_FACTOR
  * 
  */
 
@@ -13415,15 +13963,15 @@
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi._to_voronoi_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":518
+/* "pyvoronoi.pyx":521
  *         return val * self.SCALING_FACTOR
  * 
  *     cdef double _to_voronoi_double(self, val):             # <<<<<<<<<<<<<<
  *         return val * <double>self.SCALING_FACTOR
  * 
  */
 
@@ -13434,32 +13982,32 @@
   PyObject *__pyx_t_2 = NULL;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_to_voronoi_double", 1);
 
-  /* "pyvoronoi.pyx":519
+  /* "pyvoronoi.pyx":522
  * 
  *     cdef double _to_voronoi_double(self, val):
  *         return val * <double>self.SCALING_FACTOR             # <<<<<<<<<<<<<<
  * 
  *     cdef double _from_voronoi_value(self, val):
  */
-  __pyx_t_1 = PyFloat_FromDouble(((double)__pyx_v_self->SCALING_FACTOR)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(((double)__pyx_v_self->SCALING_FACTOR)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_v_val, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_v_val, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":518
+  /* "pyvoronoi.pyx":521
  *         return val * self.SCALING_FACTOR
  * 
  *     cdef double _to_voronoi_double(self, val):             # <<<<<<<<<<<<<<
  *         return val * <double>self.SCALING_FACTOR
  * 
  */
 
@@ -13470,15 +14018,15 @@
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi._to_voronoi_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":521
+/* "pyvoronoi.pyx":524
  *         return val * <double>self.SCALING_FACTOR
  * 
  *     cdef double _from_voronoi_value(self, val):             # <<<<<<<<<<<<<<
  *         return val / <double>self.SCALING_FACTOR
  */
 
 static double __pyx_f_9pyvoronoi_9Pyvoronoi__from_voronoi_value(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_val) {
@@ -13488,30 +14036,30 @@
   PyObject *__pyx_t_2 = NULL;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_from_voronoi_value", 1);
 
-  /* "pyvoronoi.pyx":522
+  /* "pyvoronoi.pyx":525
  * 
  *     cdef double _from_voronoi_value(self, val):
  *         return val / <double>self.SCALING_FACTOR             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = PyFloat_FromDouble(((double)__pyx_v_self->SCALING_FACTOR)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(((double)__pyx_v_self->SCALING_FACTOR)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_v_val, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_v_val, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L1_error)
+  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
-  /* "pyvoronoi.pyx":521
+  /* "pyvoronoi.pyx":524
  *         return val * <double>self.SCALING_FACTOR
  * 
  *     cdef double _from_voronoi_value(self, val):             # <<<<<<<<<<<<<<
  *         return val / <double>self.SCALING_FACTOR
  */
 
   /* function exit code */
@@ -13521,20 +14069,20 @@
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi._from_voronoi_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyvoronoi.pyx":220
- *     outputCells = []
- * 
+/* "pyvoronoi.pyx":199
+ *     cdef VoronoiDiagram *thisptr
+ *     cdef int constructed
  *     cdef public int SCALING_FACTOR             # <<<<<<<<<<<<<<
  * 
- *     def __cinit__(self, scaling_factor = None):
+ *     def __cinit__(self, scaling_factor = 1):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_14SCALING_FACTOR_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_14SCALING_FACTOR_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
@@ -13553,15 +14101,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->SCALING_FACTOR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13591,15 +14139,15 @@
 
 static int __pyx_pf_9pyvoronoi_9Pyvoronoi_14SCALING_FACTOR_2__set__(struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
   __pyx_v_self->SCALING_FACTOR = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.SCALING_FACTOR.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -13611,23 +14159,23 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_51__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_60__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_51__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_51__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_51__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_60__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_60__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_60__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -13644,22 +14192,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_50__reduce_cython__(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_59__reduce_cython__(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_50__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_59__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
@@ -13691,23 +14239,23 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_53__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_62__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_53__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_53__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_53__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_9pyvoronoi_9Pyvoronoi_62__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_62__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9pyvoronoi_9Pyvoronoi_62__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
@@ -13773,28 +14321,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pyvoronoi.Pyvoronoi.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_52__setstate_cython__(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_9pyvoronoi_9Pyvoronoi_61__setstate_cython__(((struct __pyx_obj_9pyvoronoi_Pyvoronoi *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_52__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9pyvoronoi_9Pyvoronoi_61__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9pyvoronoi_Pyvoronoi *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
@@ -13895,27 +14443,30 @@
   {"GetCell", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_15GetCell, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"CountVertices", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_17CountVertices, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"CountEdges", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_19CountEdges, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"CountCells", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_21CountCells, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"GetPoints", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_23GetPoints, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_22GetPoints},
   {"GetSegments", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_25GetSegments, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_24GetSegments},
   {"GetVertices", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_27GetVertices, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"GetEdges", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_29GetEdges, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"GetCells", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_31GetCells, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"ReturnCurvedSiteInformation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_33ReturnCurvedSiteInformation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_32ReturnCurvedSiteInformation},
-  {"DiscretizeCurvedEdge", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_35DiscretizeCurvedEdge, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"RetrievePoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_37RetrievePoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_36RetrievePoint},
-  {"RetrieveSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_39RetrieveSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_38RetrieveSegment},
-  {"RetrieveScaledPoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_41RetrieveScaledPoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"RetriveScaledSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_43RetriveScaledSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"GetParabolaY", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_45GetParabolaY, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_44GetParabolaY},
-  {"CheckUnsolvableParabolaEquation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_47CheckUnsolvableParabolaEquation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_46CheckUnsolvableParabolaEquation},
-  {"Discretize", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_49Discretize, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_48Discretize},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_51__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_53__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"IterateVertices", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_29IterateVertices, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"GetEdges", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_32GetEdges, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"IterateEdges", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_34IterateEdges, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"GetCells", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_37GetCells, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"IterateCells", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_39IterateCells, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"ReturnCurvedSiteInformation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_42ReturnCurvedSiteInformation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_41ReturnCurvedSiteInformation},
+  {"DiscretizeCurvedEdge", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_44DiscretizeCurvedEdge, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"RetrievePoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_46RetrievePoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_45RetrievePoint},
+  {"RetrieveSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_48RetrieveSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_47RetrieveSegment},
+  {"RetrieveScaledPoint", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_50RetrieveScaledPoint, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"RetriveScaledSegment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_52RetriveScaledSegment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"GetParabolaY", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_54GetParabolaY, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_53GetParabolaY},
+  {"CheckUnsolvableParabolaEquation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_56CheckUnsolvableParabolaEquation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_55CheckUnsolvableParabolaEquation},
+  {"Discretize", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_58Discretize, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9pyvoronoi_9Pyvoronoi_57Discretize},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_60__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9pyvoronoi_9Pyvoronoi_62__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_9pyvoronoi_Pyvoronoi[] = {
   {(char *)"SCALING_FACTOR", __pyx_getprop_9pyvoronoi_9Pyvoronoi_SCALING_FACTOR, __pyx_setprop_9pyvoronoi_9Pyvoronoi_SCALING_FACTOR, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -14014,121 +14565,642 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
-static struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *__pyx_freelist_9pyvoronoi___pyx_scope_struct__Discretize[8];
-static int __pyx_freecount_9pyvoronoi___pyx_scope_struct__Discretize = 0;
+#if CYTHON_USE_FREELISTS
+static struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *__pyx_freelist_9pyvoronoi___pyx_scope_struct__IterateVertices[8];
+static int __pyx_freecount_9pyvoronoi___pyx_scope_struct__IterateVertices = 0;
+#endif
 
-static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct__Discretize(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct__IterateVertices(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
-  if (likely((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct__Discretize > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize)))) {
-    o = (PyObject*)__pyx_freelist_9pyvoronoi___pyx_scope_struct__Discretize[--__pyx_freecount_9pyvoronoi___pyx_scope_struct__Discretize];
-    memset(o, 0, sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize));
+  #if CYTHON_USE_FREELISTS
+  if (likely((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct__IterateVertices > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices)))) {
+    o = (PyObject*)__pyx_freelist_9pyvoronoi___pyx_scope_struct__IterateVertices[--__pyx_freecount_9pyvoronoi___pyx_scope_struct__IterateVertices];
+    memset(o, 0, sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
   {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   #endif
   return o;
 }
 
-static void __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__Discretize(PyObject *o) {
-  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *)o;
+static void __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__IterateVertices(PyObject *o) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__Discretize) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__IterateVertices) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->__pyx_v_count);
+  Py_CLEAR(p->__pyx_v_index);
+  Py_CLEAR(p->__pyx_v_self);
+  Py_CLEAR(p->__pyx_t_0);
+  #if CYTHON_USE_FREELISTS
+  if (((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct__IterateVertices < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices)))) {
+    __pyx_freelist_9pyvoronoi___pyx_scope_struct__IterateVertices[__pyx_freecount_9pyvoronoi___pyx_scope_struct__IterateVertices++] = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *)o);
+  } else
+  #endif
+  {
+    #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+    (*Py_TYPE(o)->tp_free)(o);
+    #else
+    {
+      freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+      if (tp_free) tp_free(o);
+    }
+    #endif
+  }
+}
+
+static int __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct__IterateVertices(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices *)o;
+  if (p->__pyx_v_count) {
+    e = (*v)(p->__pyx_v_count, a); if (e) return e;
+  }
+  if (p->__pyx_v_index) {
+    e = (*v)(p->__pyx_v_index, a); if (e) return e;
+  }
+  if (p->__pyx_v_self) {
+    e = (*v)(((PyObject *)p->__pyx_v_self), a); if (e) return e;
+  }
+  if (p->__pyx_t_0) {
+    e = (*v)(p->__pyx_t_0, a); if (e) return e;
+  }
+  return 0;
+}
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__IterateVertices},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_9pyvoronoi___pyx_scope_struct__IterateVertices},
+  {Py_tp_new, (void *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct__IterateVertices},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices_spec = {
+  "pyvoronoi.__pyx_scope_struct__IterateVertices",
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
+  __pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices_slots,
+};
+#else
+
+static PyTypeObject __pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "pyvoronoi.""__pyx_scope_struct__IterateVertices", /*tp_name*/
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__IterateVertices), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__IterateVertices, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
+  0, /*tp_doc*/
+  __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct__IterateVertices, /*tp_traverse*/
+  0, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  0, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
+  0, /*tp_dictoffset*/
+  #endif
+  0, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_9pyvoronoi___pyx_scope_struct__IterateVertices, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
+  0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+#endif
+
+#if CYTHON_USE_FREELISTS
+static struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *__pyx_freelist_9pyvoronoi___pyx_scope_struct_1_IterateEdges[8];
+static int __pyx_freecount_9pyvoronoi___pyx_scope_struct_1_IterateEdges = 0;
+#endif
+
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct_1_IterateEdges(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  PyObject *o;
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  #if CYTHON_USE_FREELISTS
+  if (likely((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct_1_IterateEdges > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges)))) {
+    o = (PyObject*)__pyx_freelist_9pyvoronoi___pyx_scope_struct_1_IterateEdges[--__pyx_freecount_9pyvoronoi___pyx_scope_struct_1_IterateEdges];
+    memset(o, 0, sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges));
+    (void) PyObject_INIT(o, t);
+    PyObject_GC_Track(o);
+  } else
+  #endif
+  {
+    o = (*t->tp_alloc)(t, 0);
+    if (unlikely(!o)) return 0;
+  }
+  #endif
+  return o;
+}
+
+static void __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_1_IterateEdges(PyObject *o) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_1_IterateEdges) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->__pyx_v_count);
+  Py_CLEAR(p->__pyx_v_index);
+  Py_CLEAR(p->__pyx_v_self);
+  Py_CLEAR(p->__pyx_t_0);
+  #if CYTHON_USE_FREELISTS
+  if (((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct_1_IterateEdges < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges)))) {
+    __pyx_freelist_9pyvoronoi___pyx_scope_struct_1_IterateEdges[__pyx_freecount_9pyvoronoi___pyx_scope_struct_1_IterateEdges++] = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *)o);
+  } else
+  #endif
+  {
+    #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+    (*Py_TYPE(o)->tp_free)(o);
+    #else
+    {
+      freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+      if (tp_free) tp_free(o);
+    }
+    #endif
+  }
+}
+
+static int __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_1_IterateEdges(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges *)o;
+  if (p->__pyx_v_count) {
+    e = (*v)(p->__pyx_v_count, a); if (e) return e;
+  }
+  if (p->__pyx_v_index) {
+    e = (*v)(p->__pyx_v_index, a); if (e) return e;
+  }
+  if (p->__pyx_v_self) {
+    e = (*v)(((PyObject *)p->__pyx_v_self), a); if (e) return e;
+  }
+  if (p->__pyx_t_0) {
+    e = (*v)(p->__pyx_t_0, a); if (e) return e;
+  }
+  return 0;
+}
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_1_IterateEdges},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_1_IterateEdges},
+  {Py_tp_new, (void *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct_1_IterateEdges},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges_spec = {
+  "pyvoronoi.__pyx_scope_struct_1_IterateEdges",
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
+  __pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges_slots,
+};
+#else
+
+static PyTypeObject __pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "pyvoronoi.""__pyx_scope_struct_1_IterateEdges", /*tp_name*/
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_1_IterateEdges), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_1_IterateEdges, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
+  0, /*tp_doc*/
+  __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_1_IterateEdges, /*tp_traverse*/
+  0, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  0, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
+  0, /*tp_dictoffset*/
+  #endif
+  0, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_9pyvoronoi___pyx_scope_struct_1_IterateEdges, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
+  0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+#endif
+
+#if CYTHON_USE_FREELISTS
+static struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *__pyx_freelist_9pyvoronoi___pyx_scope_struct_2_IterateCells[8];
+static int __pyx_freecount_9pyvoronoi___pyx_scope_struct_2_IterateCells = 0;
+#endif
+
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct_2_IterateCells(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  PyObject *o;
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  #if CYTHON_USE_FREELISTS
+  if (likely((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct_2_IterateCells > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells)))) {
+    o = (PyObject*)__pyx_freelist_9pyvoronoi___pyx_scope_struct_2_IterateCells[--__pyx_freecount_9pyvoronoi___pyx_scope_struct_2_IterateCells];
+    memset(o, 0, sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells));
+    (void) PyObject_INIT(o, t);
+    PyObject_GC_Track(o);
+  } else
+  #endif
+  {
+    o = (*t->tp_alloc)(t, 0);
+    if (unlikely(!o)) return 0;
+  }
+  #endif
+  return o;
+}
+
+static void __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_2_IterateCells(PyObject *o) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_2_IterateCells) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->__pyx_v_count);
+  Py_CLEAR(p->__pyx_v_index);
+  Py_CLEAR(p->__pyx_v_self);
+  Py_CLEAR(p->__pyx_t_0);
+  #if CYTHON_USE_FREELISTS
+  if (((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct_2_IterateCells < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells)))) {
+    __pyx_freelist_9pyvoronoi___pyx_scope_struct_2_IterateCells[__pyx_freecount_9pyvoronoi___pyx_scope_struct_2_IterateCells++] = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *)o);
+  } else
+  #endif
+  {
+    #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+    (*Py_TYPE(o)->tp_free)(o);
+    #else
+    {
+      freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+      if (tp_free) tp_free(o);
+    }
+    #endif
+  }
+}
+
+static int __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_2_IterateCells(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells *)o;
+  if (p->__pyx_v_count) {
+    e = (*v)(p->__pyx_v_count, a); if (e) return e;
+  }
+  if (p->__pyx_v_index) {
+    e = (*v)(p->__pyx_v_index, a); if (e) return e;
+  }
+  if (p->__pyx_v_self) {
+    e = (*v)(((PyObject *)p->__pyx_v_self), a); if (e) return e;
+  }
+  if (p->__pyx_t_0) {
+    e = (*v)(p->__pyx_t_0, a); if (e) return e;
+  }
+  return 0;
+}
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_2_IterateCells},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_2_IterateCells},
+  {Py_tp_new, (void *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct_2_IterateCells},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells_spec = {
+  "pyvoronoi.__pyx_scope_struct_2_IterateCells",
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
+  __pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells_slots,
+};
+#else
+
+static PyTypeObject __pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "pyvoronoi.""__pyx_scope_struct_2_IterateCells", /*tp_name*/
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_2_IterateCells), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_2_IterateCells, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
+  0, /*tp_doc*/
+  __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_2_IterateCells, /*tp_traverse*/
+  0, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  0, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
+  0, /*tp_dictoffset*/
+  #endif
+  0, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_9pyvoronoi___pyx_scope_struct_2_IterateCells, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
+  0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+#endif
+
+#if CYTHON_USE_FREELISTS
+static struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *__pyx_freelist_9pyvoronoi___pyx_scope_struct_3_Discretize[8];
+static int __pyx_freecount_9pyvoronoi___pyx_scope_struct_3_Discretize = 0;
+#endif
+
+static PyObject *__pyx_tp_new_9pyvoronoi___pyx_scope_struct_3_Discretize(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  PyObject *o;
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  #if CYTHON_USE_FREELISTS
+  if (likely((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct_3_Discretize > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize)))) {
+    o = (PyObject*)__pyx_freelist_9pyvoronoi___pyx_scope_struct_3_Discretize[--__pyx_freecount_9pyvoronoi___pyx_scope_struct_3_Discretize];
+    memset(o, 0, sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize));
+    (void) PyObject_INIT(o, t);
+    PyObject_GC_Track(o);
+  } else
+  #endif
+  {
+    o = (*t->tp_alloc)(t, 0);
+    if (unlikely(!o)) return 0;
+  }
+  #endif
+  return o;
+}
+
+static void __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_3_Discretize(PyObject *o) {
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_3_Discretize) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_angle);
   Py_CLEAR(p->__pyx_v_shift_x);
   Py_CLEAR(p->__pyx_v_shift_y);
-  #if CYTHON_COMPILING_IN_CPYTHON
-  if (((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct__Discretize < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize)))) {
-    __pyx_freelist_9pyvoronoi___pyx_scope_struct__Discretize[__pyx_freecount_9pyvoronoi___pyx_scope_struct__Discretize++] = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *)o);
+  #if CYTHON_USE_FREELISTS
+  if (((int)(__pyx_freecount_9pyvoronoi___pyx_scope_struct_3_Discretize < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize)))) {
+    __pyx_freelist_9pyvoronoi___pyx_scope_struct_3_Discretize[__pyx_freecount_9pyvoronoi___pyx_scope_struct_3_Discretize++] = ((struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
     #else
     {
       freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
       if (tp_free) tp_free(o);
     }
     #endif
   }
 }
 
-static int __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct__Discretize(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_3_Discretize(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *)o;
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *)o;
   if (p->__pyx_v_angle) {
     e = (*v)(p->__pyx_v_angle, a); if (e) return e;
   }
   if (p->__pyx_v_shift_x) {
     e = (*v)(p->__pyx_v_shift_x, a); if (e) return e;
   }
   if (p->__pyx_v_shift_y) {
     e = (*v)(p->__pyx_v_shift_y, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_9pyvoronoi___pyx_scope_struct__Discretize(PyObject *o) {
+static int __pyx_tp_clear_9pyvoronoi___pyx_scope_struct_3_Discretize(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize *)o;
+  struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *p = (struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize *)o;
   tmp = ((PyObject*)p->__pyx_v_angle);
   p->__pyx_v_angle = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_shift_x);
   p->__pyx_v_shift_x = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_shift_y);
   p->__pyx_v_shift_y = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_9pyvoronoi___pyx_scope_struct__Discretize_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__Discretize},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_9pyvoronoi___pyx_scope_struct__Discretize},
-  {Py_tp_clear, (void *)__pyx_tp_clear_9pyvoronoi___pyx_scope_struct__Discretize},
-  {Py_tp_new, (void *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct__Discretize},
+static PyType_Slot __pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_3_Discretize},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_3_Discretize},
+  {Py_tp_clear, (void *)__pyx_tp_clear_9pyvoronoi___pyx_scope_struct_3_Discretize},
+  {Py_tp_new, (void *)__pyx_tp_new_9pyvoronoi___pyx_scope_struct_3_Discretize},
   {0, 0},
 };
-static PyType_Spec __pyx_type_9pyvoronoi___pyx_scope_struct__Discretize_spec = {
-  "pyvoronoi.__pyx_scope_struct__Discretize",
-  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize),
+static PyType_Spec __pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize_spec = {
+  "pyvoronoi.__pyx_scope_struct_3_Discretize",
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_9pyvoronoi___pyx_scope_struct__Discretize_slots,
+  __pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize_slots,
 };
 #else
 
-static PyTypeObject __pyx_type_9pyvoronoi___pyx_scope_struct__Discretize = {
+static PyTypeObject __pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pyvoronoi.""__pyx_scope_struct__Discretize", /*tp_name*/
-  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct__Discretize), /*tp_basicsize*/
+  "pyvoronoi.""__pyx_scope_struct_3_Discretize", /*tp_name*/
+  sizeof(struct __pyx_obj_9pyvoronoi___pyx_scope_struct_3_Discretize), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct__Discretize, /*tp_dealloc*/
+  __pyx_tp_dealloc_9pyvoronoi___pyx_scope_struct_3_Discretize, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -14147,16 +15219,16 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct__Discretize, /*tp_traverse*/
-  __pyx_tp_clear_9pyvoronoi___pyx_scope_struct__Discretize, /*tp_clear*/
+  __pyx_tp_traverse_9pyvoronoi___pyx_scope_struct_3_Discretize, /*tp_traverse*/
+  __pyx_tp_clear_9pyvoronoi___pyx_scope_struct_3_Discretize, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
@@ -14165,15 +15237,15 @@
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_9pyvoronoi___pyx_scope_struct__Discretize, /*tp_new*/
+  __pyx_tp_new_9pyvoronoi___pyx_scope_struct_3_Discretize, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -14216,15 +15288,14 @@
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_n_s_AddPoint, __pyx_k_AddPoint, sizeof(__pyx_k_AddPoint), 0, 0, 1, 1},
     {&__pyx_n_s_AddSegment, __pyx_k_AddSegment, sizeof(__pyx_k_AddSegment), 0, 0, 1, 1},
     {&__pyx_n_s_Cell, __pyx_k_Cell, sizeof(__pyx_k_Cell), 0, 0, 1, 1},
-    {&__pyx_n_s_Cell___init, __pyx_k_Cell___init, sizeof(__pyx_k_Cell___init), 0, 0, 1, 1},
     {&__pyx_n_s_CheckUnsolvableParabolaEquation, __pyx_k_CheckUnsolvableParabolaEquation, sizeof(__pyx_k_CheckUnsolvableParabolaEquation), 0, 0, 1, 1},
     {&__pyx_n_s_Construct, __pyx_k_Construct, sizeof(__pyx_k_Construct), 0, 0, 1, 1},
     {&__pyx_kp_s_Construct_has_already_been_calle, __pyx_k_Construct_has_already_been_calle, sizeof(__pyx_k_Construct_has_already_been_calle), 0, 0, 1, 0},
     {&__pyx_kp_s_Construct_has_been_called_can_t, __pyx_k_Construct_has_been_called_can_t, sizeof(__pyx_k_Construct_has_been_called_can_t), 0, 0, 1, 0},
     {&__pyx_n_s_CountCells, __pyx_k_CountCells, sizeof(__pyx_k_CountCells), 0, 0, 1, 1},
     {&__pyx_n_s_CountEdges, __pyx_k_CountEdges, sizeof(__pyx_k_CountEdges), 0, 0, 1, 1},
     {&__pyx_n_s_CountVertices, __pyx_k_CountVertices, sizeof(__pyx_k_CountVertices), 0, 0, 1, 1},
@@ -14232,28 +15303,31 @@
     {&__pyx_kp_s_Deleting_the_VoronoiDiagram_inst, __pyx_k_Deleting_the_VoronoiDiagram_inst, sizeof(__pyx_k_Deleting_the_VoronoiDiagram_inst), 0, 0, 1, 0},
     {&__pyx_n_s_Discretize, __pyx_k_Discretize, sizeof(__pyx_k_Discretize), 0, 0, 1, 1},
     {&__pyx_n_s_DiscretizeCurvedEdge, __pyx_k_DiscretizeCurvedEdge, sizeof(__pyx_k_DiscretizeCurvedEdge), 0, 0, 1, 1},
     {&__pyx_n_s_Discretize_locals_lambda, __pyx_k_Discretize_locals_lambda, sizeof(__pyx_k_Discretize_locals_lambda), 0, 0, 1, 1},
     {&__pyx_n_s_Distance, __pyx_k_Distance, sizeof(__pyx_k_Distance), 0, 0, 1, 1},
     {&__pyx_n_s_DistanceSquared, __pyx_k_DistanceSquared, sizeof(__pyx_k_DistanceSquared), 0, 0, 1, 1},
     {&__pyx_n_s_Edge, __pyx_k_Edge, sizeof(__pyx_k_Edge), 0, 0, 1, 1},
-    {&__pyx_n_s_Edge___init, __pyx_k_Edge___init, sizeof(__pyx_k_Edge___init), 0, 0, 1, 1},
     {&__pyx_n_s_FocusOnDirectixException, __pyx_k_FocusOnDirectixException, sizeof(__pyx_k_FocusOnDirectixException), 0, 0, 1, 1},
     {&__pyx_n_s_GetCell, __pyx_k_GetCell, sizeof(__pyx_k_GetCell), 0, 0, 1, 1},
     {&__pyx_n_s_GetCells, __pyx_k_GetCells, sizeof(__pyx_k_GetCells), 0, 0, 1, 1},
     {&__pyx_n_s_GetEdge, __pyx_k_GetEdge, sizeof(__pyx_k_GetEdge), 0, 0, 1, 1},
     {&__pyx_n_s_GetEdges, __pyx_k_GetEdges, sizeof(__pyx_k_GetEdges), 0, 0, 1, 1},
     {&__pyx_n_s_GetLineAngleInRadians, __pyx_k_GetLineAngleInRadians, sizeof(__pyx_k_GetLineAngleInRadians), 0, 0, 1, 1},
     {&__pyx_n_s_GetParabolaY, __pyx_k_GetParabolaY, sizeof(__pyx_k_GetParabolaY), 0, 0, 1, 1},
     {&__pyx_n_s_GetPoints, __pyx_k_GetPoints, sizeof(__pyx_k_GetPoints), 0, 0, 1, 1},
     {&__pyx_n_s_GetSegments, __pyx_k_GetSegments, sizeof(__pyx_k_GetSegments), 0, 0, 1, 1},
     {&__pyx_n_s_GetVertex, __pyx_k_GetVertex, sizeof(__pyx_k_GetVertex), 0, 0, 1, 1},
     {&__pyx_n_s_GetVertices, __pyx_k_GetVertices, sizeof(__pyx_k_GetVertices), 0, 0, 1, 1},
+    {&__pyx_n_s_IterateCells, __pyx_k_IterateCells, sizeof(__pyx_k_IterateCells), 0, 0, 1, 1},
+    {&__pyx_n_s_IterateEdges, __pyx_k_IterateEdges, sizeof(__pyx_k_IterateEdges), 0, 0, 1, 1},
+    {&__pyx_n_s_IterateVertices, __pyx_k_IterateVertices, sizeof(__pyx_k_IterateVertices), 0, 0, 1, 1},
     {&__pyx_kp_s_Max_distance_must_be_greater_tha, __pyx_k_Max_distance_must_be_greater_tha, sizeof(__pyx_k_Max_distance_must_be_greater_tha), 0, 0, 1, 0},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
+    {&__pyx_n_s_NamedTuple, __pyx_k_NamedTuple, sizeof(__pyx_k_NamedTuple), 0, 0, 1, 1},
     {&__pyx_kp_s_Parabola_equation_tolerance_must, __pyx_k_Parabola_equation_tolerance_must, sizeof(__pyx_k_Parabola_equation_tolerance_must), 0, 0, 1, 0},
     {&__pyx_n_s_Pyvoronoi, __pyx_k_Pyvoronoi, sizeof(__pyx_k_Pyvoronoi), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_AddPoint, __pyx_k_Pyvoronoi_AddPoint, sizeof(__pyx_k_Pyvoronoi_AddPoint), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_AddSegment, __pyx_k_Pyvoronoi_AddSegment, sizeof(__pyx_k_Pyvoronoi_AddSegment), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_CheckUnsolvableParabol, __pyx_k_Pyvoronoi_CheckUnsolvableParabol, sizeof(__pyx_k_Pyvoronoi_CheckUnsolvableParabol), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_Construct, __pyx_k_Pyvoronoi_Construct, sizeof(__pyx_k_Pyvoronoi_Construct), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_CountCells, __pyx_k_Pyvoronoi_CountCells, sizeof(__pyx_k_Pyvoronoi_CountCells), 0, 0, 1, 1},
@@ -14266,14 +15340,17 @@
     {&__pyx_n_s_Pyvoronoi_GetEdge, __pyx_k_Pyvoronoi_GetEdge, sizeof(__pyx_k_Pyvoronoi_GetEdge), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_GetEdges, __pyx_k_Pyvoronoi_GetEdges, sizeof(__pyx_k_Pyvoronoi_GetEdges), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_GetParabolaY, __pyx_k_Pyvoronoi_GetParabolaY, sizeof(__pyx_k_Pyvoronoi_GetParabolaY), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_GetPoints, __pyx_k_Pyvoronoi_GetPoints, sizeof(__pyx_k_Pyvoronoi_GetPoints), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_GetSegments, __pyx_k_Pyvoronoi_GetSegments, sizeof(__pyx_k_Pyvoronoi_GetSegments), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_GetVertex, __pyx_k_Pyvoronoi_GetVertex, sizeof(__pyx_k_Pyvoronoi_GetVertex), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_GetVertices, __pyx_k_Pyvoronoi_GetVertices, sizeof(__pyx_k_Pyvoronoi_GetVertices), 0, 0, 1, 1},
+    {&__pyx_n_s_Pyvoronoi_IterateCells, __pyx_k_Pyvoronoi_IterateCells, sizeof(__pyx_k_Pyvoronoi_IterateCells), 0, 0, 1, 1},
+    {&__pyx_n_s_Pyvoronoi_IterateEdges, __pyx_k_Pyvoronoi_IterateEdges, sizeof(__pyx_k_Pyvoronoi_IterateEdges), 0, 0, 1, 1},
+    {&__pyx_n_s_Pyvoronoi_IterateVertices, __pyx_k_Pyvoronoi_IterateVertices, sizeof(__pyx_k_Pyvoronoi_IterateVertices), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_RetrievePoint, __pyx_k_Pyvoronoi_RetrievePoint, sizeof(__pyx_k_Pyvoronoi_RetrievePoint), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_RetrieveScaledPoint, __pyx_k_Pyvoronoi_RetrieveScaledPoint, sizeof(__pyx_k_Pyvoronoi_RetrieveScaledPoint), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_RetrieveSegment, __pyx_k_Pyvoronoi_RetrieveSegment, sizeof(__pyx_k_Pyvoronoi_RetrieveSegment), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_RetriveScaledSegment, __pyx_k_Pyvoronoi_RetriveScaledSegment, sizeof(__pyx_k_Pyvoronoi_RetriveScaledSegment), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform, __pyx_k_Pyvoronoi_ReturnCurvedSiteInform, sizeof(__pyx_k_Pyvoronoi_ReturnCurvedSiteInform), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi___reduce_cython, __pyx_k_Pyvoronoi___reduce_cython, sizeof(__pyx_k_Pyvoronoi___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Pyvoronoi___setstate_cython, __pyx_k_Pyvoronoi___setstate_cython, sizeof(__pyx_k_Pyvoronoi___setstate_cython), 0, 0, 1, 1},
@@ -14287,35 +15364,37 @@
     {&__pyx_n_s_SILENT, __pyx_k_SILENT, sizeof(__pyx_k_SILENT), 0, 0, 1, 1},
     {&__pyx_kp_s_The_computed_Y_on_the_parabola_f, __pyx_k_The_computed_Y_on_the_parabola_f, sizeof(__pyx_k_The_computed_Y_on_the_parabola_f), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_Unrotate, __pyx_k_Unrotate, sizeof(__pyx_k_Unrotate), 0, 0, 1, 1},
     {&__pyx_n_s_UnsolvableParabolaEquation, __pyx_k_UnsolvableParabolaEquation, sizeof(__pyx_k_UnsolvableParabolaEquation), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_Vertex, __pyx_k_Vertex, sizeof(__pyx_k_Vertex), 0, 0, 1, 1},
-    {&__pyx_n_s_Vertex___init, __pyx_k_Vertex___init, sizeof(__pyx_k_Vertex___init), 0, 0, 1, 1},
     {&__pyx_n_s_VoronoiException, __pyx_k_VoronoiException, sizeof(__pyx_k_VoronoiException), 0, 0, 1, 1},
     {&__pyx_n_s_X, __pyx_k_X, sizeof(__pyx_k_X), 0, 0, 1, 1},
     {&__pyx_n_s_Y, __pyx_k_Y, sizeof(__pyx_k_Y), 0, 0, 1, 1},
-    {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
+    {&__pyx_n_s__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 1, 1},
+    {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
     {&__pyx_n_s__65, __pyx_k__65, sizeof(__pyx_k__65), 0, 0, 1, 1},
     {&__pyx_n_s_angle, __pyx_k_angle, sizeof(__pyx_k_angle), 0, 0, 1, 1},
-    {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
+    {&__pyx_n_s_annotations, __pyx_k_annotations, sizeof(__pyx_k_annotations), 0, 0, 1, 1},
+    {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_atan2, __pyx_k_atan2, sizeof(__pyx_k_atan2), 0, 0, 1, 1},
+    {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
     {&__pyx_n_s_boost_x, __pyx_k_boost_x, sizeof(__pyx_k_boost_x), 0, 0, 1, 1},
     {&__pyx_n_s_boost_y, __pyx_k_boost_y, sizeof(__pyx_k_boost_y), 0, 0, 1, 1},
     {&__pyx_n_s_c_cell, __pyx_k_c_cell, sizeof(__pyx_k_c_cell), 0, 0, 1, 1},
     {&__pyx_n_s_c_edge, __pyx_k_c_edge, sizeof(__pyx_k_c_edge), 0, 0, 1, 1},
     {&__pyx_n_s_c_point, __pyx_k_c_point, sizeof(__pyx_k_c_point), 0, 0, 1, 1},
     {&__pyx_n_s_c_segment, __pyx_k_c_segment, sizeof(__pyx_k_c_segment), 0, 0, 1, 1},
     {&__pyx_n_s_c_vertex, __pyx_k_c_vertex, sizeof(__pyx_k_c_vertex), 0, 0, 1, 1},
     {&__pyx_n_s_cell, __pyx_k_cell, sizeof(__pyx_k_cell), 0, 0, 1, 1},
     {&__pyx_n_s_cell_identifier, __pyx_k_cell_identifier, sizeof(__pyx_k_cell_identifier), 0, 0, 1, 1},
-    {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
     {&__pyx_n_s_computed_point_y, __pyx_k_computed_point_y, sizeof(__pyx_k_computed_point_y), 0, 0, 1, 1},
     {&__pyx_n_s_contains_point, __pyx_k_contains_point, sizeof(__pyx_k_contains_point), 0, 0, 1, 1},
     {&__pyx_n_s_contains_segment, __pyx_k_contains_segment, sizeof(__pyx_k_contains_segment), 0, 0, 1, 1},
     {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
     {&__pyx_n_s_copy_2, __pyx_k_copy_2, sizeof(__pyx_k_copy_2), 0, 0, 1, 1},
     {&__pyx_n_s_cos, __pyx_k_cos, sizeof(__pyx_k_cos), 0, 0, 1, 1},
     {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
@@ -14336,27 +15415,26 @@
     {&__pyx_n_s_edgeEndVertex, __pyx_k_edgeEndVertex, sizeof(__pyx_k_edgeEndVertex), 0, 0, 1, 1},
     {&__pyx_n_s_edgeStartVertex, __pyx_k_edgeStartVertex, sizeof(__pyx_k_edgeStartVertex), 0, 0, 1, 1},
     {&__pyx_n_s_edges, __pyx_k_edges, sizeof(__pyx_k_edges), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
     {&__pyx_n_s_end_point_x, __pyx_k_end_point_x, sizeof(__pyx_k_end_point_x), 0, 0, 1, 1},
     {&__pyx_n_s_end_point_y, __pyx_k_end_point_y, sizeof(__pyx_k_end_point_y), 0, 0, 1, 1},
+    {&__pyx_n_s_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 0, 1, 1},
     {&__pyx_n_s_focus, __pyx_k_focus, sizeof(__pyx_k_focus), 0, 0, 1, 1},
     {&__pyx_n_s_focus_rotated, __pyx_k_focus_rotated, sizeof(__pyx_k_focus_rotated), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
-    {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
     {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
-    {&__pyx_n_s_inputPoints, __pyx_k_inputPoints, sizeof(__pyx_k_inputPoints), 0, 0, 1, 1},
-    {&__pyx_n_s_inputSegments, __pyx_k_inputSegments, sizeof(__pyx_k_inputSegments), 0, 0, 1, 1},
     {&__pyx_n_s_input_segment, __pyx_k_input_segment, sizeof(__pyx_k_input_segment), 0, 0, 1, 1},
+    {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_is_degenerate, __pyx_k_is_degenerate, sizeof(__pyx_k_is_degenerate), 0, 0, 1, 1},
     {&__pyx_n_s_is_linear, __pyx_k_is_linear, sizeof(__pyx_k_is_linear), 0, 0, 1, 1},
     {&__pyx_n_s_is_open, __pyx_k_is_open, sizeof(__pyx_k_is_open), 0, 0, 1, 1},
     {&__pyx_n_s_is_primary, __pyx_k_is_primary, sizeof(__pyx_k_is_primary), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_log_action, __pyx_k_log_action, sizeof(__pyx_k_log_action), 0, 0, 1, 1},
@@ -14371,17 +15449,15 @@
     {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_next, __pyx_k_next, sizeof(__pyx_k_next), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_non_scaled_point, __pyx_k_non_scaled_point, sizeof(__pyx_k_non_scaled_point), 0, 0, 1, 1},
     {&__pyx_n_s_non_scaled_segment, __pyx_k_non_scaled_segment, sizeof(__pyx_k_non_scaled_segment), 0, 0, 1, 1},
     {&__pyx_n_s_output, __pyx_k_output, sizeof(__pyx_k_output), 0, 0, 1, 1},
-    {&__pyx_n_s_outputCells, __pyx_k_outputCells, sizeof(__pyx_k_outputCells), 0, 0, 1, 1},
-    {&__pyx_n_s_outputEdges, __pyx_k_outputEdges, sizeof(__pyx_k_outputEdges), 0, 0, 1, 1},
-    {&__pyx_n_s_outputVertices, __pyx_k_outputVertices, sizeof(__pyx_k_outputVertices), 0, 0, 1, 1},
+    {&__pyx_n_s_p, __pyx_k_p, sizeof(__pyx_k_p), 0, 0, 1, 1},
     {&__pyx_n_s_p0, __pyx_k_p0, sizeof(__pyx_k_p0), 0, 0, 1, 1},
     {&__pyx_n_s_p1, __pyx_k_p1, sizeof(__pyx_k_p1), 0, 0, 1, 1},
     {&__pyx_n_s_parabola_end, __pyx_k_parabola_end, sizeof(__pyx_k_parabola_end), 0, 0, 1, 1},
     {&__pyx_n_s_parabola_end_rotated, __pyx_k_parabola_end_rotated, sizeof(__pyx_k_parabola_end_rotated), 0, 0, 1, 1},
     {&__pyx_n_s_parabola_end_rotated_check, __pyx_k_parabola_end_rotated_check, sizeof(__pyx_k_parabola_end_rotated_check), 0, 0, 1, 1},
     {&__pyx_n_s_parabola_equation_tolerance, __pyx_k_parabola_equation_tolerance, sizeof(__pyx_k_parabola_equation_tolerance), 0, 0, 1, 1},
     {&__pyx_n_s_parabola_start, __pyx_k_parabola_start, sizeof(__pyx_k_parabola_start), 0, 0, 1, 1},
@@ -14400,18 +15476,20 @@
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
     {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+    {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
     {&__pyx_n_s_scaling_factor, __pyx_k_scaling_factor, sizeof(__pyx_k_scaling_factor), 0, 0, 1, 1},
     {&__pyx_n_s_segment, __pyx_k_segment, sizeof(__pyx_k_segment), 0, 0, 1, 1},
     {&__pyx_n_s_segmentSite, __pyx_k_segmentSite, sizeof(__pyx_k_segmentSite), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
     {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shift_x, __pyx_k_shift_x, sizeof(__pyx_k_shift_x), 0, 0, 1, 1},
     {&__pyx_n_s_shift_y, __pyx_k_shift_y, sizeof(__pyx_k_shift_y), 0, 0, 1, 1},
     {&__pyx_n_s_sin, __pyx_k_sin, sizeof(__pyx_k_sin), 0, 0, 1, 1},
     {&__pyx_n_s_site, __pyx_k_site, sizeof(__pyx_k_site), 0, 0, 1, 1},
@@ -14426,439 +15504,431 @@
     {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
     {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
     {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
     {&__pyx_n_s_sys_2, __pyx_k_sys_2, sizeof(__pyx_k_sys_2), 0, 0, 1, 1},
     {&__pyx_n_s_t, __pyx_k_t, sizeof(__pyx_k_t), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_theta, __pyx_k_theta, sizeof(__pyx_k_theta), 0, 0, 1, 1},
+    {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
     {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
     {&__pyx_n_s_time_2, __pyx_k_time_2, sizeof(__pyx_k_time_2), 0, 0, 1, 1},
     {&__pyx_n_s_tolerance, __pyx_k_tolerance, sizeof(__pyx_k_tolerance), 0, 0, 1, 1},
     {&__pyx_n_s_twin, __pyx_k_twin, sizeof(__pyx_k_twin), 0, 0, 1, 1},
     {&__pyx_n_s_twinCell, __pyx_k_twinCell, sizeof(__pyx_k_twinCell), 0, 0, 1, 1},
     {&__pyx_n_s_twinEdge, __pyx_k_twinEdge, sizeof(__pyx_k_twinEdge), 0, 0, 1, 1},
+    {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
+    {&__pyx_kp_s_typing_Type_Edge, __pyx_k_typing_Type_Edge, sizeof(__pyx_k_typing_Type_Edge), 0, 0, 1, 0},
+    {&__pyx_kp_s_typing_Type_Vertex, __pyx_k_typing_Type_Vertex, sizeof(__pyx_k_typing_Type_Vertex), 0, 0, 1, 0},
     {&__pyx_n_s_unicodedata, __pyx_k_unicodedata, sizeof(__pyx_k_unicodedata), 0, 0, 1, 1},
     {&__pyx_n_s_unicodedata_2, __pyx_k_unicodedata_2, sizeof(__pyx_k_unicodedata_2), 0, 0, 1, 1},
     {&__pyx_n_s_vertices, __pyx_k_vertices, sizeof(__pyx_k_vertices), 0, 0, 1, 1},
     {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
-    {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 322, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 355, __pyx_L1_error)
-  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 508, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 68, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pyvoronoi.pyx":234
- *             self.SCALING_FACTOR = 1
- * 
- *         del self.inputPoints[:]             # <<<<<<<<<<<<<<
- *         del self.inputSegments[:]
- * 
- */
-  __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice_);
-  __Pyx_GIVEREF(__pyx_slice_);
-
-  /* "pyvoronoi.pyx":17
+  /* "pyvoronoi.pyx":18
  * 
  * SILENT = True
  * def log_action(description):             # <<<<<<<<<<<<<<
  *     if not SILENT:
  *         print(description)
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_description); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_log_action, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 17, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":121
- *     X = 0.0
- *     Y = 0.0
- *     def __init__(self,x,y):             # <<<<<<<<<<<<<<
- *         self.X = x
- *         self.Y = y
- */
-  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_y); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_init, 121, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 121, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":133
- *     twin = -1
- * 
- *     def __init__(self, start, end, cell, twin):             # <<<<<<<<<<<<<<
- *         self.start = start
- *         self.end = end
- */
-  __pyx_tuple__7 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_cell, __pyx_n_s_twin); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_init, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 133, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":151
- *     source_category = None
- * 
- *     def __init__(self, cell_identifier, site, vertices, edges, source_category):             # <<<<<<<<<<<<<<
- *         self.cell_identifier = cell_identifier
- *         self.site = site
- */
-  __pyx_tuple__9 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_cell_identifier, __pyx_n_s_site, __pyx_n_s_vertices, __pyx_n_s_edges, __pyx_n_s_source_category); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_init, 151, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_s_description); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_log_action, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":173
+  /* "pyvoronoi.pyx":159
  * ##ROTATION
  * ####################################
  * def Rotate(point, theta):             # <<<<<<<<<<<<<<
  *     t = -1 * theta
  *     cos = math.cos(t)
  */
-  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_point, __pyx_n_s_theta, __pyx_n_s_t, __pyx_n_s_cos, __pyx_n_s_sin); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 173, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Rotate, 173, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_point, __pyx_n_s_theta, __pyx_n_s_t, __pyx_n_s_cos, __pyx_n_s_sin); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Rotate, 159, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 159, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":180
+  /* "pyvoronoi.pyx":166
  * 	(point[0] * sin) + (point[1] * cos)]
  * 
  * def RotateWithShift(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(4, __pyx_n_s_point, __pyx_n_s_theta, __pyx_n_s_shift_x, __pyx_n_s_shift_y); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 180, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RotateWithShift, 180, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(4, __pyx_n_s_point, __pyx_n_s_theta, __pyx_n_s_shift_x, __pyx_n_s_shift_y); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RotateWithShift, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 166, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":183
+  /* "pyvoronoi.pyx":169
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  * def Unrotate(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     cos = math.cos(theta)
  *     sin = math.sin(theta)
  */
-  __pyx_tuple__15 = PyTuple_Pack(6, __pyx_n_s_point, __pyx_n_s_theta, __pyx_n_s_shift_x, __pyx_n_s_shift_y, __pyx_n_s_cos, __pyx_n_s_sin); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Unrotate, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(6, __pyx_n_s_point, __pyx_n_s_theta, __pyx_n_s_shift_x, __pyx_n_s_shift_y, __pyx_n_s_cos, __pyx_n_s_sin); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Unrotate, 169, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 169, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":188
+  /* "pyvoronoi.pyx":174
  *     return [(point[0] * cos) - (point[1] * sin) + shift_x, (point[0] * sin) + (point[1] * cos) + shift_y]
  * 
  * def GetLineAngleInRadians(start_point_x, start_point_y,end_point_x, end_point_y):             # <<<<<<<<<<<<<<
  *     return math.atan2(end_point_y - start_point_y, end_point_x - start_point_x)
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(4, __pyx_n_s_start_point_x, __pyx_n_s_start_point_y, __pyx_n_s_end_point_x, __pyx_n_s_end_point_y); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 188, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetLineAngleInRadians, 188, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(4, __pyx_n_s_start_point_x, __pyx_n_s_start_point_y, __pyx_n_s_end_point_x, __pyx_n_s_end_point_y); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetLineAngleInRadians, 174, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 174, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":195
+  /* "pyvoronoi.pyx":181
  * ##DISTANCE
  * ####################################
  * def DistanceSquared(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the squared length of the line.
  *     :return: a float representing the squared length of the line.
  */
-  __pyx_tuple__19 = PyTuple_Pack(2, __pyx_n_s_point_start, __pyx_n_s_point_end); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 195, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_DistanceSquared, 195, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(2, __pyx_n_s_point_start, __pyx_n_s_point_end); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_DistanceSquared, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 181, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":201
+  /* "pyvoronoi.pyx":187
  *     return pow(point_end[0] - point_start[0], 2) + pow(point_end[1] - point_start[1], 2)
  * 
  * def Distance(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the length of the line"""
  *     return math.sqrt(DistanceSquared(point_start, point_end))
  */
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Distance, 201, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Distance, 187, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 187, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":241
+  /* "pyvoronoi.pyx":214
  *         del self.thisptr
  * 
  *     def AddPoint(self, point):             # <<<<<<<<<<<<<<
  *         """ Add a point
  *         """
  */
-  __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_point, __pyx_n_s_c_point); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 241, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_AddPoint, 241, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_point, __pyx_n_s_c_point); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_AddPoint, 214, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 214, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":252
- *         self.inputPoints.append([c_point.X, c_point.Y])
+  /* "pyvoronoi.pyx":224
+ *         self.thisptr.AddPoint(c_point)
  * 
  *     def AddSegment(self, segment):             # <<<<<<<<<<<<<<
  *         """ Add a segment
  *         """
  */
-  __pyx_tuple__24 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_segment, __pyx_n_s_c_segment); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 252, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_AddSegment, 252, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_segment, __pyx_n_s_c_segment); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_AddSegment, 224, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 224, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":263
- *         self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])
+  /* "pyvoronoi.pyx":234
+ *         self.thisptr.AddSegment(c_segment)
  * 
  *     def Construct(self):             # <<<<<<<<<<<<<<
  *         """ Generates the voronoi diagram for the added points and segments. Voronoi cell structure will be generated.
  *         """
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 263, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Construct, 263, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Construct, 234, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 234, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":278
+  /* "pyvoronoi.pyx":247
  *         self.thisptr.MapCellIndexes()
  * 
  *     def GetVertex(self, index):             # <<<<<<<<<<<<<<
  *         """
  *         """
  */
-  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_c_vertex); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 278, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetVertex, 278, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_c_vertex); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetVertex, 247, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 247, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":284
- *         return Vertex(c_vertex.X / self.SCALING_FACTOR, c_vertex.Y / self.SCALING_FACTOR)
+  /* "pyvoronoi.pyx":256
+ *         )
  * 
  *     def GetEdge(self, index):             # <<<<<<<<<<<<<<
  *         c_edge =  self.thisptr.GetEdge(index)
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
+ *         edge = Edge(
  */
-  __pyx_tuple__30 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_c_edge, __pyx_n_s_edge); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetEdge, 284, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_c_edge, __pyx_n_s_edge); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetEdge, 256, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 256, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":291
+  /* "pyvoronoi.pyx":268
  *         return edge
  * 
  *     def GetCell(self, index):             # <<<<<<<<<<<<<<
  *         c_cell = self.thisptr.GetCell(index)
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
+ *         cell = Cell(
  */
-  __pyx_tuple__32 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_c_cell, __pyx_n_s_cell); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetCell, 291, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_c_cell, __pyx_n_s_cell); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetCell, 268, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 268, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":300
+  /* "pyvoronoi.pyx":283
  *         return cell
  * 
  *     def CountVertices(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountVertices()
  * 
  */
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CountVertices, 300, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CountVertices, 283, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 283, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":303
+  /* "pyvoronoi.pyx":286
  *         return self.thisptr.CountVertices()
  * 
  *     def CountEdges(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountEdges()
  * 
  */
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CountEdges, 303, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CountEdges, 286, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 286, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":306
+  /* "pyvoronoi.pyx":289
  *         return self.thisptr.CountEdges()
  * 
  *     def CountCells(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountCells()
  * 
  */
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CountCells, 306, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CountCells, 289, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 289, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":309
+  /* "pyvoronoi.pyx":292
  *         return self.thisptr.CountCells()
  * 
  *     def GetPoints(self):             # <<<<<<<<<<<<<<
  *         """ Returns the points added to the voronoi diagram
  *         """
  */
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetPoints, 309, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_p); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetPoints, 292, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 292, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":314
- *         return self.inputPoints
+  /* "pyvoronoi.pyx":298
+ * 
  * 
  *     def GetSegments(self):             # <<<<<<<<<<<<<<
  *         """ Returns the segments added to the voronoi diagram
  *         """
  */
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetSegments, 314, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_s); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetSegments, 298, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 298, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":319
- *         return self.inputSegments
+  /* "pyvoronoi.pyx":303
+ *         return [[[s.p0.X, s.p0.Y], [s.p1.X, s.p1.Y]] for s in self.thisptr.GetSegments()]
  * 
  *     def GetVertices(self):             # <<<<<<<<<<<<<<
  *         count = self.CountVertices()
  *         output = []
  */
-  __pyx_tuple__39 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_count, __pyx_n_s_output, __pyx_n_s_index); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 319, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetVertices, 319, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_count, __pyx_n_s_output, __pyx_n_s_index); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetVertices, 303, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 303, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":326
+  /* "pyvoronoi.pyx":310
  *         return output
  * 
+ *     def IterateVertices(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountVertices()
+ *         for index in  range(count):
+ */
+  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_count, __pyx_n_s_index); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_IterateVertices, 310, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 310, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":315
+ *             yield self.GetVertex(index)
+ * 
  *     def GetEdges(self):             # <<<<<<<<<<<<<<
  *         count = self.CountEdges()
  *         output = []
  */
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetEdges, 326, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetEdges, 315, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 315, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":333
+  /* "pyvoronoi.pyx":322
  *         return output
  * 
+ *     def IterateEdges(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountEdges()
+ *         for index in range(count):
+ */
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_IterateEdges, 322, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 322, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":327
+ *             yield self.GetEdge(index)
+ * 
  *     def GetCells(self):             # <<<<<<<<<<<<<<
  *         count = self.CountCells()
  *         output = []
  */
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetCells, 333, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetCells, 327, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 327, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":340
+  /* "pyvoronoi.pyx":334
  *         return output
  * 
+ *     def IterateCells(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountCells()
+ *         for index in range(count):
+ */
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_IterateCells, 334, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 334, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":339
+ *             yield self.GetCell(index)
+ * 
  *     def ReturnCurvedSiteInformation(self, edge):             # <<<<<<<<<<<<<<
  *         """Return the index of the point side and the segment site associated  with a segment index
  *         """
  */
-  __pyx_tuple__43 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_edge, __pyx_n_s_twinEdge, __pyx_n_s_cell, __pyx_n_s_twinCell, __pyx_n_s_pointSite, __pyx_n_s_segmentSite); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_edge, __pyx_n_s_twinEdge, __pyx_n_s_cell, __pyx_n_s_twinCell, __pyx_n_s_pointSite, __pyx_n_s_segmentSite); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_ReturnCurvedSiteInformation, 340, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_ReturnCurvedSiteInformation, 339, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 339, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":353
+  /* "pyvoronoi.pyx":352
  *         return [pointSite, segmentSite]
  * 
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):             # <<<<<<<<<<<<<<
  *         if(max_dist <= 0):
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  */
-  __pyx_tuple__45 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_max_dist, __pyx_n_s_parabola_equation_tolerance, __pyx_n_s_edge, __pyx_n_s_sites, __pyx_n_s_pointSite, __pyx_n_s_segmentSite, __pyx_n_s_edgeStartVertex, __pyx_n_s_edgeEndVertex); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_index, __pyx_n_s_max_dist, __pyx_n_s_parabola_equation_tolerance, __pyx_n_s_edge, __pyx_n_s_sites, __pyx_n_s_pointSite, __pyx_n_s_segmentSite, __pyx_n_s_edgeStartVertex, __pyx_n_s_edgeEndVertex); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_DiscretizeCurvedEdge, 353, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 353, __pyx_L1_error)
-  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_float_0_0001); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_DiscretizeCurvedEdge, 352, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_float_0_0001); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
 
-  /* "pyvoronoi.pyx":370
+  /* "pyvoronoi.pyx":369
  * 
  * 
  *     def RetrievePoint(self, cell):             # <<<<<<<<<<<<<<
  *         """Retrive the input point associated with a cell.
  * 		:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.
  */
-  __pyx_tuple__48 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_cell, __pyx_n_s_input_segment); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_cell, __pyx_n_s_point, __pyx_n_s_input_segment); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__48);
   __Pyx_GIVEREF(__pyx_tuple__48);
-  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetrievePoint, 370, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetrievePoint, 369, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 369, __pyx_L1_error)
 
   /* "pyvoronoi.pyx":383
  *             return input_segment[1]
  * 
  *     def RetrieveSegment(self, cell):             # <<<<<<<<<<<<<<
  *         """Retrive the input segment associated with a cell.
  *         """
  */
-  __pyx_tuple__50 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_cell); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_cell, __pyx_n_s_segment); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
-  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetrieveSegment, 383, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetrieveSegment, 383, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 383, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":389
- * 
+  /* "pyvoronoi.pyx":392
+ *         ]
  * 
  *     def RetrieveScaledPoint(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_point = self.RetrievePoint(cell)
  *         return [
  */
-  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_cell, __pyx_n_s_non_scaled_point); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_cell, __pyx_n_s_non_scaled_point); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetrieveScaledPoint, 389, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetrieveScaledPoint, 392, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 392, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":396
+  /* "pyvoronoi.pyx":399
  * 		]
  * 
  *     def RetriveScaledSegment(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_segment = self.RetrieveSegment(cell)
  *         return [
  */
-  __pyx_tuple__54 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_cell, __pyx_n_s_non_scaled_segment); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_cell, __pyx_n_s_non_scaled_segment); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__54);
   __Pyx_GIVEREF(__pyx_tuple__54);
-  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetriveScaledSegment, 396, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_RetriveScaledSegment, 399, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 399, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":403
+  /* "pyvoronoi.pyx":406
  * 		]
  * 
  *     def GetParabolaY(self, x, focus, directrix_y):             # <<<<<<<<<<<<<<
  *         """
  * 		Solve the parabola equation for a given value on the x-axis and return the associated value on the y-axis.
  */
-  __pyx_tuple__56 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_focus, __pyx_n_s_directrix_y); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_focus, __pyx_n_s_directrix_y); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__56);
   __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetParabolaY, 403, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_GetParabolaY, 406, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 406, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":415
+  /* "pyvoronoi.pyx":418
  *         return (pow(x - focus[0], 2) + pow(focus[1], 2) - pow(directrix_y, 2)) / (2 * (focus[1] - directrix_y));
  * 
  *     def CheckUnsolvableParabolaEquation(self, boost_x, boost_y, focus, directix, tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Compare the y-coordinate of a point on the parabola returned by Boost with the computed value.
  */
-  __pyx_tuple__58 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_boost_x, __pyx_n_s_boost_y, __pyx_n_s_focus, __pyx_n_s_directix, __pyx_n_s_tolerance, __pyx_n_s_computed_point_y, __pyx_n_s_delta); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_boost_x, __pyx_n_s_boost_y, __pyx_n_s_focus, __pyx_n_s_directix, __pyx_n_s_tolerance, __pyx_n_s_computed_point_y, __pyx_n_s_delta); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CheckUnsolvableParabolaEquation, 415, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_CheckUnsolvableParabolaEquation, 418, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 418, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":433
+  /* "pyvoronoi.pyx":436
  *         return [boost_x, computed_point_y]
  * 
  *     def Discretize(self, point, segment, parabola_start, parabola_end, max_dist, parabola_equation_tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.
  */
-  __pyx_tuple__60 = PyTuple_Pack(26, __pyx_n_s_self, __pyx_n_s_point, __pyx_n_s_segment, __pyx_n_s_parabola_start, __pyx_n_s_parabola_end, __pyx_n_s_max_dist, __pyx_n_s_parabola_equation_tolerance, __pyx_n_s_shift_x, __pyx_n_s_shift_y, __pyx_n_s_angle, __pyx_n_s_focus_rotated, __pyx_n_s_directix_start_rotated, __pyx_n_s_directix_end_rotated, __pyx_n_s_parabola_start_rotated, __pyx_n_s_parabola_end_rotated, __pyx_n_s_directix, __pyx_n_s_parabola_start_rotated_check, __pyx_n_s_parabola_end_rotated_check, __pyx_n_s_densified_rotated, __pyx_n_s_previous, __pyx_n_s_next, __pyx_n_s_current, __pyx_n_s_distance, __pyx_n_s_mid_point_x, __pyx_n_s_mid_point, __pyx_n_s_densified); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(26, __pyx_n_s_self, __pyx_n_s_point, __pyx_n_s_segment, __pyx_n_s_parabola_start, __pyx_n_s_parabola_end, __pyx_n_s_max_dist, __pyx_n_s_parabola_equation_tolerance, __pyx_n_s_shift_x, __pyx_n_s_shift_y, __pyx_n_s_angle, __pyx_n_s_focus_rotated, __pyx_n_s_directix_start_rotated, __pyx_n_s_directix_end_rotated, __pyx_n_s_parabola_start_rotated, __pyx_n_s_parabola_end_rotated, __pyx_n_s_directix, __pyx_n_s_parabola_start_rotated_check, __pyx_n_s_parabola_end_rotated_check, __pyx_n_s_densified_rotated, __pyx_n_s_previous, __pyx_n_s_next, __pyx_n_s_current, __pyx_n_s_distance, __pyx_n_s_mid_point_x, __pyx_n_s_mid_point, __pyx_n_s_densified); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Discretize, 433, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyvoronoi_pyvoronoi_pyx, __pyx_n_s_Discretize, 436, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 436, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -14937,57 +16007,114 @@
   __pyx_vtabptr_9pyvoronoi_Pyvoronoi = &__pyx_vtable_9pyvoronoi_Pyvoronoi;
   __pyx_vtable_9pyvoronoi_Pyvoronoi._to_voronoi_segment = (struct Segment (*)(struct __pyx_obj_9pyvoronoi_Pyvoronoi *, PyObject *))__pyx_f_9pyvoronoi_9Pyvoronoi__to_voronoi_segment;
   __pyx_vtable_9pyvoronoi_Pyvoronoi._to_voronoi_point = (struct Point (*)(struct __pyx_obj_9pyvoronoi_Pyvoronoi *, PyObject *))__pyx_f_9pyvoronoi_9Pyvoronoi__to_voronoi_point;
   __pyx_vtable_9pyvoronoi_Pyvoronoi._to_voronoi_int = (int (*)(struct __pyx_obj_9pyvoronoi_Pyvoronoi *, PyObject *))__pyx_f_9pyvoronoi_9Pyvoronoi__to_voronoi_int;
   __pyx_vtable_9pyvoronoi_Pyvoronoi._to_voronoi_double = (double (*)(struct __pyx_obj_9pyvoronoi_Pyvoronoi *, PyObject *))__pyx_f_9pyvoronoi_9Pyvoronoi__to_voronoi_double;
   __pyx_vtable_9pyvoronoi_Pyvoronoi._from_voronoi_value = (double (*)(struct __pyx_obj_9pyvoronoi_Pyvoronoi *, PyObject *))__pyx_f_9pyvoronoi_9Pyvoronoi__from_voronoi_value;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_9pyvoronoi_Pyvoronoi = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9pyvoronoi_Pyvoronoi_spec, NULL); if (unlikely(!__pyx_ptype_9pyvoronoi_Pyvoronoi)) __PYX_ERR(0, 210, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9pyvoronoi_Pyvoronoi_spec, __pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_ptype_9pyvoronoi_Pyvoronoi = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9pyvoronoi_Pyvoronoi_spec, NULL); if (unlikely(!__pyx_ptype_9pyvoronoi_Pyvoronoi)) __PYX_ERR(0, 196, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9pyvoronoi_Pyvoronoi_spec, __pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   #else
   __pyx_ptype_9pyvoronoi_Pyvoronoi = &__pyx_type_9pyvoronoi_Pyvoronoi;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_9pyvoronoi_Pyvoronoi->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9pyvoronoi_Pyvoronoi->tp_dictoffset && __pyx_ptype_9pyvoronoi_Pyvoronoi->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_9pyvoronoi_Pyvoronoi->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_vtabptr_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_vtabptr_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_MergeVtables(__pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Pyvoronoi, (PyObject *) __pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  #endif
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices_spec, NULL); if (unlikely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices)) __PYX_ERR(0, 310, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices_spec, __pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
+  #else
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices = &__pyx_type_9pyvoronoi___pyx_scope_struct__IterateVertices;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices->tp_dictoffset && __pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_9pyvoronoi___pyx_scope_struct__IterateVertices->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  }
+  #endif
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges_spec, NULL); if (unlikely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges)) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges_spec, __pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  #else
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges = &__pyx_type_9pyvoronoi___pyx_scope_struct_1_IterateEdges;
+  #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Pyvoronoi, (PyObject *) __pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges->tp_print = 0;
+  #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_9pyvoronoi_Pyvoronoi) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges->tp_dictoffset && __pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_9pyvoronoi___pyx_scope_struct_1_IterateEdges->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9pyvoronoi___pyx_scope_struct__Discretize_spec, NULL); if (unlikely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize)) __PYX_ERR(0, 433, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9pyvoronoi___pyx_scope_struct__Discretize_spec, __pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells_spec, NULL); if (unlikely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells)) __PYX_ERR(0, 334, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells_spec, __pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
   #else
-  __pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize = &__pyx_type_9pyvoronoi___pyx_scope_struct__Discretize;
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells = &__pyx_type_9pyvoronoi___pyx_scope_struct_2_IterateCells;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize->tp_print = 0;
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize->tp_dictoffset && __pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_9pyvoronoi___pyx_scope_struct__Discretize->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells->tp_dictoffset && __pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_9pyvoronoi___pyx_scope_struct_2_IterateCells->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  }
+  #endif
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize_spec, NULL); if (unlikely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize)) __PYX_ERR(0, 436, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize_spec, __pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
+  #else
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize = &__pyx_type_9pyvoronoi___pyx_scope_struct_3_Discretize;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize->tp_dictoffset && __pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_9pyvoronoi___pyx_scope_struct_3_Discretize->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -15347,853 +16474,913 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyvoronoi.pyx":11
  * import copy as _copy
  * import unicodedata as _unicodedata
  * import time as _time             # <<<<<<<<<<<<<<
  * import math
- * 
+ * import typing
  */
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_time, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_time_2, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyvoronoi.pyx":12
  * import unicodedata as _unicodedata
  * import time as _time
  * import math             # <<<<<<<<<<<<<<
- * 
- * from cython.operator cimport dereference as deref
+ * import typing
+ * from typing import NamedTuple
  */
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_math, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_math, __pyx_t_2) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":16
+  /* "pyvoronoi.pyx":13
+ * import time as _time
+ * import math
+ * import typing             # <<<<<<<<<<<<<<
+ * from typing import NamedTuple
+ * from cython.operator cimport dereference as deref
+ */
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_typing, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_typing, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pyvoronoi.pyx":14
+ * import math
+ * import typing
+ * from typing import NamedTuple             # <<<<<<<<<<<<<<
+ * from cython.operator cimport dereference as deref
+ * 
+ */
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_n_s_NamedTuple);
+  __Pyx_GIVEREF(__pyx_n_s_NamedTuple);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_NamedTuple)) __PYX_ERR(0, 14, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_NamedTuple); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NamedTuple, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "pyvoronoi.pyx":17
  * from cython.operator cimport dereference as deref
  * 
  * SILENT = True             # <<<<<<<<<<<<<<
  * def log_action(description):
  *     if not SILENT:
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SILENT, Py_True) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SILENT, Py_True) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":17
+  /* "pyvoronoi.pyx":18
  * 
  * SILENT = True
  * def log_action(description):             # <<<<<<<<<<<<<<
  *     if not SILENT:
  *         print(description)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_1log_action, 0, __pyx_n_s_log_action, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_action, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_1log_action, 0, __pyx_n_s_log_action, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_action, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":118
+  /* "pyvoronoi.pyx":123
  * ##VORONOY UTILS
  * ####################################
- * class Vertex:             # <<<<<<<<<<<<<<
- *     X = 0.0
- *     Y = 0.0
+ * class Vertex(NamedTuple):             # <<<<<<<<<<<<<<
+ *     X : float = 0.0
+ *     Y : float = 0.0
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Vertex, __pyx_n_s_Vertex, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_NamedTuple); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-
-  /* "pyvoronoi.pyx":119
- * ####################################
- * class Vertex:
- *     X = 0.0             # <<<<<<<<<<<<<<
- *     Y = 0.0
- *     def __init__(self,x,y):
- */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_X, __pyx_float_0_0) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":120
- * class Vertex:
- *     X = 0.0
- *     Y = 0.0             # <<<<<<<<<<<<<<
- *     def __init__(self,x,y):
- *         self.X = x
- */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_Y, __pyx_float_0_0) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
-
-  /* "pyvoronoi.pyx":121
- *     X = 0.0
- *     Y = 0.0
- *     def __init__(self,x,y):             # <<<<<<<<<<<<<<
- *         self.X = x
- *         self.Y = y
- */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_6Vertex_1__init__, 0, __pyx_n_s_Vertex___init, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_Vertex, __pyx_n_s_Vertex, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__pyx_t_3 != __pyx_t_2) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 123, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_X, __pyx_n_s_float) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_Y, __pyx_n_s_float) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_annotations, __pyx_t_2) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":118
- * ##VORONOY UTILS
+  /* "pyvoronoi.pyx":124
  * ####################################
- * class Vertex:             # <<<<<<<<<<<<<<
- *     X = 0.0
- *     Y = 0.0
+ * class Vertex(NamedTuple):
+ *     X : float = 0.0             # <<<<<<<<<<<<<<
+ *     Y : float = 0.0
+ * 
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_Vertex, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Vertex, __pyx_t_3) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_X, __pyx_float_0_0) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
 
   /* "pyvoronoi.pyx":125
- *         self.Y = y
+ * class Vertex(NamedTuple):
+ *     X : float = 0.0
+ *     Y : float = 0.0             # <<<<<<<<<<<<<<
  * 
- * class Edge:             # <<<<<<<<<<<<<<
- *     start = -1
- *     end = -1
+ * class Edge(NamedTuple):
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Edge, __pyx_n_s_Edge, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_Y, __pyx_float_0_0) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":126
- * 
- * class Edge:
- *     start = -1             # <<<<<<<<<<<<<<
- *     end = -1
- *     is_primary = False
+  /* "pyvoronoi.pyx":123
+ * ##VORONOY UTILS
+ * ####################################
+ * class Vertex(NamedTuple):             # <<<<<<<<<<<<<<
+ *     X : float = 0.0
+ *     Y : float = 0.0
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_start, __pyx_int_neg_1) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_Vertex, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Vertex, __pyx_t_2) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyvoronoi.pyx":127
- * class Edge:
- *     start = -1
- *     end = -1             # <<<<<<<<<<<<<<
- *     is_primary = False
- *     is_linear = False
+ *     Y : float = 0.0
+ * 
+ * class Edge(NamedTuple):             # <<<<<<<<<<<<<<
+ *     start : int =  -1
+ *     end : int = -1
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_end, __pyx_int_neg_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_NamedTuple); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_3, __pyx_n_s_Edge, __pyx_n_s_Edge, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__pyx_t_3 != __pyx_t_4) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(0, 127, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_start, __pyx_n_s_int) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_end, __pyx_n_s_int) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_is_primary, __pyx_n_s_bool) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_is_linear, __pyx_n_s_bool) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_cell, __pyx_n_s_int) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_twin, __pyx_n_s_int) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_annotations, __pyx_t_4) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pyvoronoi.pyx":128
- *     start = -1
- *     end = -1
- *     is_primary = False             # <<<<<<<<<<<<<<
- *     is_linear = False
- *     cell = -1
+ * 
+ * class Edge(NamedTuple):
+ *     start : int =  -1             # <<<<<<<<<<<<<<
+ *     end : int = -1
+ *     is_primary : bool = False
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_is_primary, Py_False) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_start, __pyx_int_neg_1) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
 
   /* "pyvoronoi.pyx":129
- *     end = -1
- *     is_primary = False
- *     is_linear = False             # <<<<<<<<<<<<<<
- *     cell = -1
- *     twin = -1
+ * class Edge(NamedTuple):
+ *     start : int =  -1
+ *     end : int = -1             # <<<<<<<<<<<<<<
+ *     is_primary : bool = False
+ *     is_linear : bool =  False
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_is_linear, Py_False) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_end, __pyx_int_neg_1) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
 
   /* "pyvoronoi.pyx":130
- *     is_primary = False
- *     is_linear = False
- *     cell = -1             # <<<<<<<<<<<<<<
- *     twin = -1
- * 
+ *     start : int =  -1
+ *     end : int = -1
+ *     is_primary : bool = False             # <<<<<<<<<<<<<<
+ *     is_linear : bool =  False
+ *     cell : int = -1
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_cell, __pyx_int_neg_1) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_is_primary, Py_False) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
 
   /* "pyvoronoi.pyx":131
- *     is_linear = False
- *     cell = -1
- *     twin = -1             # <<<<<<<<<<<<<<
+ *     end : int = -1
+ *     is_primary : bool = False
+ *     is_linear : bool =  False             # <<<<<<<<<<<<<<
+ *     cell : int = -1
+ *     twin : int = -1
+ */
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_is_linear, Py_False) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":132
+ *     is_primary : bool = False
+ *     is_linear : bool =  False
+ *     cell : int = -1             # <<<<<<<<<<<<<<
+ *     twin : int = -1
  * 
- *     def __init__(self, start, end, cell, twin):
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_twin, __pyx_int_neg_1) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_cell, __pyx_int_neg_1) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
 
   /* "pyvoronoi.pyx":133
- *     twin = -1
+ *     is_linear : bool =  False
+ *     cell : int = -1
+ *     twin : int = -1             # <<<<<<<<<<<<<<
+ * 
  * 
- *     def __init__(self, start, end, cell, twin):             # <<<<<<<<<<<<<<
- *         self.start = start
- *         self.end = end
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_4Edge_1__init__, 0, __pyx_n_s_Edge___init, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_twin, __pyx_int_neg_1) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":125
- *         self.Y = y
+  /* "pyvoronoi.pyx":127
+ *     Y : float = 0.0
  * 
- * class Edge:             # <<<<<<<<<<<<<<
- *     start = -1
- *     end = -1
+ * class Edge(NamedTuple):             # <<<<<<<<<<<<<<
+ *     start : int =  -1
+ *     end : int = -1
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_Edge, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Edge, __pyx_t_3) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_Edge, __pyx_t_3, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Edge, __pyx_t_4) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":139
- *         self.twin = twin
+  /* "pyvoronoi.pyx":136
  * 
- * class Cell:             # <<<<<<<<<<<<<<
- *     cell_identifier = -1
- *     site = -1
+ * 
+ * class Cell(NamedTuple):             # <<<<<<<<<<<<<<
+ *     cell_identifier : int = -1
+ *     site : int = -1
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Cell, __pyx_n_s_Cell, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_NamedTuple); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_Cell, __pyx_n_s_Cell, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__pyx_t_3 != __pyx_t_5) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_4, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(0, 136, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_cell_identifier, __pyx_n_s_int) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_site, __pyx_n_s_int) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_contains_point, __pyx_n_s_bool) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_contains_segment, __pyx_n_s_bool) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_is_open, __pyx_n_s_bool) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_is_degenerate, __pyx_n_s_bool) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_vertices, __pyx_kp_s_typing_Type_Vertex) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_edges, __pyx_kp_s_typing_Type_Edge) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_source_category, __pyx_n_s_int) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_annotations, __pyx_t_5) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":140
+  /* "pyvoronoi.pyx":137
  * 
- * class Cell:
- *     cell_identifier = -1             # <<<<<<<<<<<<<<
- *     site = -1
- *     contains_point = False
+ * class Cell(NamedTuple):
+ *     cell_identifier : int = -1             # <<<<<<<<<<<<<<
+ *     site : int = -1
+ *     contains_point : bool = False
+ */
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_cell_identifier, __pyx_int_neg_1) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+
+  /* "pyvoronoi.pyx":138
+ * class Cell(NamedTuple):
+ *     cell_identifier : int = -1
+ *     site : int = -1             # <<<<<<<<<<<<<<
+ *     contains_point : bool = False
+ *     contains_segment : bool = False
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_cell_identifier, __pyx_int_neg_1) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_site, __pyx_int_neg_1) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":141
- * class Cell:
- *     cell_identifier = -1
- *     site = -1             # <<<<<<<<<<<<<<
- *     contains_point = False
- *     contains_segment = False
+  /* "pyvoronoi.pyx":139
+ *     cell_identifier : int = -1
+ *     site : int = -1
+ *     contains_point : bool = False             # <<<<<<<<<<<<<<
+ *     contains_segment : bool = False
+ *     is_open : bool = False
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_site, __pyx_int_neg_1) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_contains_point, Py_False) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":142
- *     cell_identifier = -1
- *     site = -1
- *     contains_point = False             # <<<<<<<<<<<<<<
- *     contains_segment = False
- *     is_open = False
+  /* "pyvoronoi.pyx":140
+ *     site : int = -1
+ *     contains_point : bool = False
+ *     contains_segment : bool = False             # <<<<<<<<<<<<<<
+ *     is_open : bool = False
+ *     is_degenerate: bool = False
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_contains_point, Py_False) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_contains_segment, Py_False) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":143
- *     site = -1
- *     contains_point = False
- *     contains_segment = False             # <<<<<<<<<<<<<<
- *     is_open = False
- * 
+  /* "pyvoronoi.pyx":141
+ *     contains_point : bool = False
+ *     contains_segment : bool = False
+ *     is_open : bool = False             # <<<<<<<<<<<<<<
+ *     is_degenerate: bool = False
+ *     vertices : [typing.Type[Vertex]] = []
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_contains_segment, Py_False) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_is_open, Py_False) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":144
- *     contains_point = False
- *     contains_segment = False
- *     is_open = False             # <<<<<<<<<<<<<<
- * 
- *     vertices = []
+  /* "pyvoronoi.pyx":142
+ *     contains_segment : bool = False
+ *     is_open : bool = False
+ *     is_degenerate: bool = False             # <<<<<<<<<<<<<<
+ *     vertices : [typing.Type[Vertex]] = []
+ *     edges : [typing.Type[Edge]] = []
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_is_open, Py_False) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_is_degenerate, Py_False) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":146
- *     is_open = False
- * 
- *     vertices = []             # <<<<<<<<<<<<<<
- *     edges = []
- * 
+  /* "pyvoronoi.pyx":143
+ *     is_open : bool = False
+ *     is_degenerate: bool = False
+ *     vertices : [typing.Type[Vertex]] = []             # <<<<<<<<<<<<<<
+ *     edges : [typing.Type[Edge]] = []
+ *     source_category : int  = None
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_vertices, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_vertices, __pyx_t_5) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":147
- * 
- *     vertices = []
- *     edges = []             # <<<<<<<<<<<<<<
+  /* "pyvoronoi.pyx":144
+ *     is_degenerate: bool = False
+ *     vertices : [typing.Type[Vertex]] = []
+ *     edges : [typing.Type[Edge]] = []             # <<<<<<<<<<<<<<
+ *     source_category : int  = None
  * 
- *     source_category = None
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_edges, __pyx_t_3) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_edges, __pyx_t_5) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":149
- *     edges = []
+  /* "pyvoronoi.pyx":145
+ *     vertices : [typing.Type[Vertex]] = []
+ *     edges : [typing.Type[Edge]] = []
+ *     source_category : int  = None             # <<<<<<<<<<<<<<
  * 
- *     source_category = None             # <<<<<<<<<<<<<<
- * 
- *     def __init__(self, cell_identifier, site, vertices, edges, source_category):
+ * class VoronoiException(Exception):
  */
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_source_category, Py_None) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_source_category, Py_None) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
 
-  /* "pyvoronoi.pyx":151
- *     source_category = None
+  /* "pyvoronoi.pyx":136
  * 
- *     def __init__(self, cell_identifier, site, vertices, edges, source_category):             # <<<<<<<<<<<<<<
- *         self.cell_identifier = cell_identifier
- *         self.site = site
- */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_4Cell_1__init__, 0, __pyx_n_s_Cell___init, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-  /* "pyvoronoi.pyx":139
- *         self.twin = twin
  * 
- * class Cell:             # <<<<<<<<<<<<<<
- *     cell_identifier = -1
- *     site = -1
+ * class Cell(NamedTuple):             # <<<<<<<<<<<<<<
+ *     cell_identifier : int = -1
+ *     site : int = -1
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_Cell, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Cell, __pyx_t_3) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_Cell, __pyx_t_3, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Cell, __pyx_t_5) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyvoronoi.pyx":161
- * 
+  /* "pyvoronoi.pyx":147
+ *     source_category : int  = None
  * 
  * class VoronoiException(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 161, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 147, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_VoronoiException, __pyx_n_s_VoronoiException, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_2, __pyx_n_s_VoronoiException, __pyx_n_s_VoronoiException, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__pyx_t_3 != __pyx_t_2) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (__pyx_t_2 != __pyx_t_3) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(0, 147, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_VoronoiException, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_VoronoiException, __pyx_t_2) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_VoronoiException, __pyx_t_2, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_VoronoiException, __pyx_t_3) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyvoronoi.pyx":164
+  /* "pyvoronoi.pyx":150
  *     pass
  * 
  * class FocusOnDirectixException(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 164, __pyx_L1_error);
-  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 150, __pyx_L1_error);
+  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_FocusOnDirectixException, __pyx_n_s_FocusOnDirectixException, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__pyx_t_4 != __pyx_t_3) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(0, 164, __pyx_L1_error)
-  }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_FocusOnDirectixException, __pyx_t_4, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_FocusOnDirectixException, __pyx_n_s_FocusOnDirectixException, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FocusOnDirectixException, __pyx_t_3) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__pyx_t_4 != __pyx_t_2) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_3, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 150, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_FocusOnDirectixException, __pyx_t_4, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FocusOnDirectixException, __pyx_t_2) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyvoronoi.pyx":167
+  /* "pyvoronoi.pyx":153
  *     pass
  * 
  * class UnsolvableParabolaEquation(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 167, __pyx_L1_error);
-  __pyx_t_5 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 153, __pyx_L1_error);
+  __pyx_t_5 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_5, __pyx_n_s_UnsolvableParabolaEquation, __pyx_n_s_UnsolvableParabolaEquation, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_5, __pyx_n_s_UnsolvableParabolaEquation, __pyx_n_s_UnsolvableParabolaEquation, (PyObject *) NULL, __pyx_n_s_pyvoronoi, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   if (__pyx_t_5 != __pyx_t_4) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_3, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(0, 167, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(0, 153, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_UnsolvableParabolaEquation, __pyx_t_5, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_UnsolvableParabolaEquation, __pyx_t_5, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnsolvableParabolaEquation, __pyx_t_4) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnsolvableParabolaEquation, __pyx_t_4) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":173
+  /* "pyvoronoi.pyx":159
  * ##ROTATION
  * ####################################
  * def Rotate(point, theta):             # <<<<<<<<<<<<<<
  *     t = -1 * theta
  *     cos = math.cos(t)
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_3Rotate, 0, __pyx_n_s_Rotate, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_3Rotate, 0, __pyx_n_s_Rotate, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Rotate, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Rotate, __pyx_t_5) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":180
+  /* "pyvoronoi.pyx":166
  * 	(point[0] * sin) + (point[1] * cos)]
  * 
  * def RotateWithShift(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_5RotateWithShift, 0, __pyx_n_s_RotateWithShift, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_5RotateWithShift, 0, __pyx_n_s_RotateWithShift, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RotateWithShift, __pyx_t_5) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RotateWithShift, __pyx_t_5) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":183
+  /* "pyvoronoi.pyx":169
  *     return Rotate([point[0] - shift_x, point[1] - shift_y], theta)
  * 
  * def Unrotate(point, theta, shift_x, shift_y):             # <<<<<<<<<<<<<<
  *     cos = math.cos(theta)
  *     sin = math.sin(theta)
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_7Unrotate, 0, __pyx_n_s_Unrotate, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_7Unrotate, 0, __pyx_n_s_Unrotate, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Unrotate, __pyx_t_5) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Unrotate, __pyx_t_5) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":188
+  /* "pyvoronoi.pyx":174
  *     return [(point[0] * cos) - (point[1] * sin) + shift_x, (point[0] * sin) + (point[1] * cos) + shift_y]
  * 
  * def GetLineAngleInRadians(start_point_x, start_point_y,end_point_x, end_point_y):             # <<<<<<<<<<<<<<
  *     return math.atan2(end_point_y - start_point_y, end_point_x - start_point_x)
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9GetLineAngleInRadians, 0, __pyx_n_s_GetLineAngleInRadians, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9GetLineAngleInRadians, 0, __pyx_n_s_GetLineAngleInRadians, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GetLineAngleInRadians, __pyx_t_5) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GetLineAngleInRadians, __pyx_t_5) < 0) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":195
+  /* "pyvoronoi.pyx":181
  * ##DISTANCE
  * ####################################
  * def DistanceSquared(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the squared length of the line.
  *     :return: a float representing the squared length of the line.
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_11DistanceSquared, 0, __pyx_n_s_DistanceSquared, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_11DistanceSquared, 0, __pyx_n_s_DistanceSquared, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DistanceSquared, __pyx_t_5) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DistanceSquared, __pyx_t_5) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyvoronoi.pyx":201
+  /* "pyvoronoi.pyx":187
  *     return pow(point_end[0] - point_start[0], 2) + pow(point_end[1] - point_start[1], 2)
  * 
  * def Distance(point_start, point_end):             # <<<<<<<<<<<<<<
  *     """Returns the length of the line"""
  *     return math.sqrt(DistanceSquared(point_start, point_end))
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_13Distance, 0, __pyx_n_s_Distance, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_13Distance, 0, __pyx_n_s_Distance, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Distance, __pyx_t_5) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Distance, __pyx_t_5) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pyvoronoi.pyx":214
- *     cdef int constructed
- * 
- *     inputPoints = []             # <<<<<<<<<<<<<<
- *     inputSegments = []
- *     outputEdges = []
- */
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_inputPoints, __pyx_t_5) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
-
-  /* "pyvoronoi.pyx":215
- * 
- *     inputPoints = []
- *     inputSegments = []             # <<<<<<<<<<<<<<
- *     outputEdges = []
- *     outputVertices = []
- */
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_inputSegments, __pyx_t_5) < 0) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
-
-  /* "pyvoronoi.pyx":216
- *     inputPoints = []
- *     inputSegments = []
- *     outputEdges = []             # <<<<<<<<<<<<<<
- *     outputVertices = []
- *     outputCells = []
- */
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_outputEdges, __pyx_t_5) < 0) __PYX_ERR(0, 216, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
-
-  /* "pyvoronoi.pyx":217
- *     inputSegments = []
- *     outputEdges = []
- *     outputVertices = []             # <<<<<<<<<<<<<<
- *     outputCells = []
- * 
- */
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 217, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_outputVertices, __pyx_t_5) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
-
-  /* "pyvoronoi.pyx":218
- *     outputEdges = []
- *     outputVertices = []
- *     outputCells = []             # <<<<<<<<<<<<<<
- * 
- *     cdef public int SCALING_FACTOR
- */
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_outputCells, __pyx_t_5) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
-
-  /* "pyvoronoi.pyx":241
  *         del self.thisptr
  * 
  *     def AddPoint(self, point):             # <<<<<<<<<<<<<<
  *         """ Add a point
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_5AddPoint, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_AddPoint, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_5AddPoint, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_AddPoint, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_AddPoint, __pyx_t_5) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_AddPoint, __pyx_t_5) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":252
- *         self.inputPoints.append([c_point.X, c_point.Y])
+  /* "pyvoronoi.pyx":224
+ *         self.thisptr.AddPoint(c_point)
  * 
  *     def AddSegment(self, segment):             # <<<<<<<<<<<<<<
  *         """ Add a segment
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_7AddSegment, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_AddSegment, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_7AddSegment, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_AddSegment, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_AddSegment, __pyx_t_5) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_AddSegment, __pyx_t_5) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":263
- *         self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])
+  /* "pyvoronoi.pyx":234
+ *         self.thisptr.AddSegment(c_segment)
  * 
  *     def Construct(self):             # <<<<<<<<<<<<<<
  *         """ Generates the voronoi diagram for the added points and segments. Voronoi cell structure will be generated.
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_9Construct, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_Construct, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_9Construct, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_Construct, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_Construct, __pyx_t_5) < 0) __PYX_ERR(0, 263, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_Construct, __pyx_t_5) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":278
+  /* "pyvoronoi.pyx":247
  *         self.thisptr.MapCellIndexes()
  * 
  *     def GetVertex(self, index):             # <<<<<<<<<<<<<<
  *         """
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_11GetVertex, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetVertex, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_11GetVertex, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetVertex, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetVertex, __pyx_t_5) < 0) __PYX_ERR(0, 278, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetVertex, __pyx_t_5) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":284
- *         return Vertex(c_vertex.X / self.SCALING_FACTOR, c_vertex.Y / self.SCALING_FACTOR)
+  /* "pyvoronoi.pyx":256
+ *         )
  * 
  *     def GetEdge(self, index):             # <<<<<<<<<<<<<<
  *         c_edge =  self.thisptr.GetEdge(index)
- *         edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
+ *         edge = Edge(
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_13GetEdge, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetEdge, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_13GetEdge, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetEdge, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetEdge, __pyx_t_5) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetEdge, __pyx_t_5) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":291
+  /* "pyvoronoi.pyx":268
  *         return edge
  * 
  *     def GetCell(self, index):             # <<<<<<<<<<<<<<
  *         c_cell = self.thisptr.GetCell(index)
- *         cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
+ *         cell = Cell(
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_15GetCell, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetCell, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_15GetCell, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetCell, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetCell, __pyx_t_5) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetCell, __pyx_t_5) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":300
+  /* "pyvoronoi.pyx":283
  *         return cell
  * 
  *     def CountVertices(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountVertices()
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_17CountVertices, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CountVertices, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_17CountVertices, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CountVertices, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CountVertices, __pyx_t_5) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CountVertices, __pyx_t_5) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":303
+  /* "pyvoronoi.pyx":286
  *         return self.thisptr.CountVertices()
  * 
  *     def CountEdges(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountEdges()
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_19CountEdges, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CountEdges, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_19CountEdges, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CountEdges, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CountEdges, __pyx_t_5) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CountEdges, __pyx_t_5) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":306
+  /* "pyvoronoi.pyx":289
  *         return self.thisptr.CountEdges()
  * 
  *     def CountCells(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr.CountCells()
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_21CountCells, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CountCells, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_21CountCells, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CountCells, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CountCells, __pyx_t_5) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CountCells, __pyx_t_5) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":309
+  /* "pyvoronoi.pyx":292
  *         return self.thisptr.CountCells()
  * 
  *     def GetPoints(self):             # <<<<<<<<<<<<<<
  *         """ Returns the points added to the voronoi diagram
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_23GetPoints, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetPoints, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_23GetPoints, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetPoints, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetPoints, __pyx_t_5) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetPoints, __pyx_t_5) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":314
- *         return self.inputPoints
+  /* "pyvoronoi.pyx":298
+ * 
  * 
  *     def GetSegments(self):             # <<<<<<<<<<<<<<
  *         """ Returns the segments added to the voronoi diagram
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_25GetSegments, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetSegments, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_25GetSegments, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetSegments, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetSegments, __pyx_t_5) < 0) __PYX_ERR(0, 314, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetSegments, __pyx_t_5) < 0) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":319
- *         return self.inputSegments
+  /* "pyvoronoi.pyx":303
+ *         return [[[s.p0.X, s.p0.Y], [s.p1.X, s.p1.Y]] for s in self.thisptr.GetSegments()]
  * 
  *     def GetVertices(self):             # <<<<<<<<<<<<<<
  *         count = self.CountVertices()
  *         output = []
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_27GetVertices, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetVertices, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_27GetVertices, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetVertices, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetVertices, __pyx_t_5) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetVertices, __pyx_t_5) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":326
+  /* "pyvoronoi.pyx":310
  *         return output
  * 
+ *     def IterateVertices(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountVertices()
+ *         for index in  range(count):
+ */
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_29IterateVertices, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_IterateVertices, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_IterateVertices, __pyx_t_5) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
+
+  /* "pyvoronoi.pyx":315
+ *             yield self.GetVertex(index)
+ * 
  *     def GetEdges(self):             # <<<<<<<<<<<<<<
  *         count = self.CountEdges()
  *         output = []
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_29GetEdges, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetEdges, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_32GetEdges, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetEdges, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetEdges, __pyx_t_5) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetEdges, __pyx_t_5) < 0) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":333
+  /* "pyvoronoi.pyx":322
  *         return output
  * 
+ *     def IterateEdges(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountEdges()
+ *         for index in range(count):
+ */
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_34IterateEdges, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_IterateEdges, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_IterateEdges, __pyx_t_5) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
+
+  /* "pyvoronoi.pyx":327
+ *             yield self.GetEdge(index)
+ * 
  *     def GetCells(self):             # <<<<<<<<<<<<<<
  *         count = self.CountCells()
  *         output = []
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_31GetCells, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetCells, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_37GetCells, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetCells, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetCells, __pyx_t_5) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetCells, __pyx_t_5) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":340
+  /* "pyvoronoi.pyx":334
  *         return output
  * 
+ *     def IterateCells(self):             # <<<<<<<<<<<<<<
+ *         count = self.CountCells()
+ *         for index in range(count):
+ */
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_39IterateCells, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_IterateCells, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_IterateCells, __pyx_t_5) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
+
+  /* "pyvoronoi.pyx":339
+ *             yield self.GetCell(index)
+ * 
  *     def ReturnCurvedSiteInformation(self, edge):             # <<<<<<<<<<<<<<
  *         """Return the index of the point side and the segment site associated  with a segment index
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_33ReturnCurvedSiteInformation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_42ReturnCurvedSiteInformation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_ReturnCurvedSiteInform, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_ReturnCurvedSiteInformation, __pyx_t_5) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_ReturnCurvedSiteInformation, __pyx_t_5) < 0) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":353
+  /* "pyvoronoi.pyx":352
  *         return [pointSite, segmentSite]
  * 
  *     def DiscretizeCurvedEdge(self, index, max_dist, parabola_equation_tolerance = 0.0001):             # <<<<<<<<<<<<<<
  *         if(max_dist <= 0):
  *             raise ValueError("Max distance must be greater than 0. Value passed: {0}".format(max_dist))
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_35DiscretizeCurvedEdge, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_DiscretizeCurvedEdge, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_44DiscretizeCurvedEdge, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_DiscretizeCurvedEdge, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__47);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_DiscretizeCurvedEdge, __pyx_t_5) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_DiscretizeCurvedEdge, __pyx_t_5) < 0) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":370
+  /* "pyvoronoi.pyx":369
  * 
  * 
  *     def RetrievePoint(self, cell):             # <<<<<<<<<<<<<<
  *         """Retrive the input point associated with a cell.
  * 		:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_37RetrievePoint, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetrievePoint, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_46RetrievePoint, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetrievePoint, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_RetrievePoint, __pyx_t_5) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_RetrievePoint, __pyx_t_5) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
   /* "pyvoronoi.pyx":383
  *             return input_segment[1]
  * 
  *     def RetrieveSegment(self, cell):             # <<<<<<<<<<<<<<
  *         """Retrive the input segment associated with a cell.
  *         """
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_39RetrieveSegment, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetrieveSegment, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_48RetrieveSegment, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetrieveSegment, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_RetrieveSegment, __pyx_t_5) < 0) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":389
- * 
+  /* "pyvoronoi.pyx":392
+ *         ]
  * 
  *     def RetrieveScaledPoint(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_point = self.RetrievePoint(cell)
  *         return [
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_41RetrieveScaledPoint, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetrieveScaledPoint, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_50RetrieveScaledPoint, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetrieveScaledPoint, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_RetrieveScaledPoint, __pyx_t_5) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_RetrieveScaledPoint, __pyx_t_5) < 0) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":396
+  /* "pyvoronoi.pyx":399
  * 		]
  * 
  *     def RetriveScaledSegment(self, cell):             # <<<<<<<<<<<<<<
  *         non_scaled_segment = self.RetrieveSegment(cell)
  *         return [
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_43RetriveScaledSegment, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetriveScaledSegment, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_52RetriveScaledSegment, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_RetriveScaledSegment, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_RetriveScaledSegment, __pyx_t_5) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_RetriveScaledSegment, __pyx_t_5) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":403
+  /* "pyvoronoi.pyx":406
  * 		]
  * 
  *     def GetParabolaY(self, x, focus, directrix_y):             # <<<<<<<<<<<<<<
  *         """
  * 		Solve the parabola equation for a given value on the x-axis and return the associated value on the y-axis.
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_45GetParabolaY, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetParabolaY, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_54GetParabolaY, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_GetParabolaY, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetParabolaY, __pyx_t_5) < 0) __PYX_ERR(0, 403, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_GetParabolaY, __pyx_t_5) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":415
+  /* "pyvoronoi.pyx":418
  *         return (pow(x - focus[0], 2) + pow(focus[1], 2) - pow(directrix_y, 2)) / (2 * (focus[1] - directrix_y));
  * 
  *     def CheckUnsolvableParabolaEquation(self, boost_x, boost_y, focus, directix, tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Compare the y-coordinate of a point on the parabola returned by Boost with the computed value.
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_47CheckUnsolvableParabolaEquation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CheckUnsolvableParabol, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_56CheckUnsolvableParabolaEquation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_CheckUnsolvableParabol, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CheckUnsolvableParabolaEquation, __pyx_t_5) < 0) __PYX_ERR(0, 415, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_CheckUnsolvableParabolaEquation, __pyx_t_5) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
-  /* "pyvoronoi.pyx":433
+  /* "pyvoronoi.pyx":436
  *         return [boost_x, computed_point_y]
  * 
  *     def Discretize(self, point, segment, parabola_start, parabola_end, max_dist, parabola_equation_tolerance):             # <<<<<<<<<<<<<<
  *         """
  *         Interpolate points on a parabola. The points are garanteed to be closer than the value of the parameter max_dist.
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_49Discretize, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_Discretize, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_58Discretize, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi_Discretize, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_Discretize, __pyx_t_5) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9pyvoronoi_Pyvoronoi, __pyx_n_s_Discretize, __pyx_t_5) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9pyvoronoi_Pyvoronoi);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_51__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi___reduce_cython, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_60__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi___reduce_cython, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_5) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_53__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi___setstate_cython, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9pyvoronoi_9Pyvoronoi_62__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Pyvoronoi___setstate_cython, NULL, __pyx_n_s_pyvoronoi, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_5) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pyvoronoi.pyx":1
  * """             # <<<<<<<<<<<<<<
  * Cython wrapper for the C++ translation of the Voronoi diagram part of Boost's
@@ -16629,19 +17816,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -16720,15 +17907,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -16739,15 +17926,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -16771,15 +17958,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -17177,271 +18364,14 @@
 
 /* PyObjectCallOneArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *args[2] = {NULL, arg};
     return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
-/* PyObjectSetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_setattro))
-        return tp->tp_setattro(obj, attr_name, value);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_setattr))
-        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
-#endif
-    return PyObject_SetAttr(obj, attr_name, value);
-}
-#endif
-
-/* PyObjectCall2Args */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args[3] = {NULL, arg1, arg2};
-    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    __Pyx_TypeName type_name;
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
-        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
-#elif PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (likely(descr != NULL)) {
-        *method = descr;
-        return 0;
-    }
-    type_name = __Pyx_PyType_GetName(tp);
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
-                 type_name, name);
-#else
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
-                 type_name, PyString_AS_STRING(name));
-#endif
-    __Pyx_DECREF_TypeName(type_name);
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
-}
-
-/* PyObjectCallMethod1 */
-#if !(CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2)
-static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
-    PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
-    Py_DECREF(method);
-    return result;
-}
-#endif
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
-#if CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2
-    PyObject *args[2] = {obj, arg};
-    (void) __Pyx_PyObject_GetMethod;
-    (void) __Pyx_PyObject_CallOneArg;
-    (void) __Pyx_PyObject_Call2Args;
-    return PyObject_VectorcallMethod(method_name, args, 2 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
-#else
-    PyObject *method = NULL, *result;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_Call2Args(method, obj, arg);
-        Py_DECREF(method);
-        return result;
-    }
-    if (unlikely(!method)) return NULL;
-    return __Pyx__PyObject_CallMethod1(method, arg);
-#endif
-}
-
-/* append */
-static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x) {
-    if (likely(PyList_CheckExact(L))) {
-        if (unlikely(__Pyx_PyList_Append(L, x) < 0)) return -1;
-    } else {
-        PyObject* retval = __Pyx_PyObject_CallMethod1(L, __pyx_n_s_append, x);
-        if (unlikely(!retval))
-            return -1;
-        Py_DECREF(retval);
-    }
-    return 0;
-}
-
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (unlikely(!j)) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
-        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
-        if (mm && mm->mp_subscript) {
-            PyObject *r, *key = PyInt_FromSsize_t(i);
-            if (unlikely(!key)) return NULL;
-            r = mm->mp_subscript(o, key);
-            Py_DECREF(key);
-            return r;
-        }
-        if (likely(sm && sm->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
-                Py_ssize_t l = sm->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return sm->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || !PyMapping_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_MultiplyCObj(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
     CYTHON_MAYBE_UNUSED_VAR(intval);
     CYTHON_MAYBE_UNUSED_VAR(inplace);
     CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
@@ -17581,117 +18511,107 @@
             PyFPE_END_PROTECT(result)
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceMultiply : PyNumber_Multiply)(op1, op2);
 }
 #endif
 
-/* SliceObject */
-static CYTHON_INLINE int __Pyx_PyObject_SetSlice(PyObject* obj, PyObject* value,
-        Py_ssize_t cstart, Py_ssize_t cstop,
-        PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
-        int has_cstart, int has_cstop, int wraparound) {
-    __Pyx_TypeName obj_type_name;
-#if CYTHON_USE_TYPE_SLOTS
-    PyMappingMethods* mp;
-#if PY_MAJOR_VERSION < 3
-    PySequenceMethods* ms = Py_TYPE(obj)->tp_as_sequence;
-    if (likely(ms && ms->sq_ass_slice)) {
-        if (!has_cstart) {
-            if (_py_start && (*_py_start != Py_None)) {
-                cstart = __Pyx_PyIndex_AsSsize_t(*_py_start);
-                if ((cstart == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-            } else
-                cstart = 0;
-        }
-        if (!has_cstop) {
-            if (_py_stop && (*_py_stop != Py_None)) {
-                cstop = __Pyx_PyIndex_AsSsize_t(*_py_stop);
-                if ((cstop == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-            } else
-                cstop = PY_SSIZE_T_MAX;
-        }
-        if (wraparound && unlikely((cstart < 0) | (cstop < 0)) && likely(ms->sq_length)) {
-            Py_ssize_t l = ms->sq_length(obj);
-            if (likely(l >= 0)) {
-                if (cstop < 0) {
-                    cstop += l;
-                    if (cstop < 0) cstop = 0;
-                }
-                if (cstart < 0) {
-                    cstart += l;
-                    if (cstart < 0) cstart = 0;
-                }
-            } else {
-                if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                    goto bad;
-                PyErr_Clear();
-            }
-        }
-        return ms->sq_ass_slice(obj, cstart, cstop, value);
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (unlikely(!j)) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
     }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 #else
-    CYTHON_UNUSED_VAR(wraparound);
+    return PySequence_GetItem(o, i);
 #endif
-    mp = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(mp && mp->mp_ass_subscript))
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 #else
-    CYTHON_UNUSED_VAR(wraparound);
+    return PySequence_GetItem(o, i);
 #endif
-    {
-        int result;
-        PyObject *py_slice, *py_start, *py_stop;
-        if (_py_slice) {
-            py_slice = *_py_slice;
-        } else {
-            PyObject* owned_start = NULL;
-            PyObject* owned_stop = NULL;
-            if (_py_start) {
-                py_start = *_py_start;
-            } else {
-                if (has_cstart) {
-                    owned_start = py_start = PyInt_FromSsize_t(cstart);
-                    if (unlikely(!py_start)) goto bad;
-                } else
-                    py_start = Py_None;
-            }
-            if (_py_stop) {
-                py_stop = *_py_stop;
-            } else {
-                if (has_cstop) {
-                    owned_stop = py_stop = PyInt_FromSsize_t(cstop);
-                    if (unlikely(!py_stop)) {
-                        Py_XDECREF(owned_start);
-                        goto bad;
-                    }
-                } else
-                    py_stop = Py_None;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
             }
-            py_slice = PySlice_New(py_start, py_stop, Py_None);
-            Py_XDECREF(owned_start);
-            Py_XDECREF(owned_stop);
-            if (unlikely(!py_slice)) goto bad;
+            return sm->sq_item(o, i);
         }
-#if CYTHON_USE_TYPE_SLOTS
-        result = mp->mp_ass_subscript(obj, py_slice, value);
+    }
 #else
-        result = value ? PyObject_SetItem(obj, py_slice, value) : PyObject_DelItem(obj, py_slice);
-#endif
-        if (!_py_slice) {
-            Py_DECREF(py_slice);
-        }
-        return result;
+    if (is_list || !PyMapping_Check(o)) {
+        return PySequence_GetItem(o, i);
     }
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError,
-        "'" __Pyx_FMT_TYPENAME "' object does not support slice %.10s",
-        obj_type_name, value ? "assignment" : "deletion");
-    __Pyx_DECREF_TypeName(obj_type_name);
-bad:
-    return -1;
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* WriteUnraisableException */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil) {
     PyObject *old_exc, *old_val, *old_tb;
@@ -17965,14 +18885,139 @@
     PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
     return 0;
 }
 
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* pep479 */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen) {
+    PyObject *exc, *val, *tb, *cur_exc;
+    __Pyx_PyThreadState_declare
+    #ifdef __Pyx_StopAsyncIteration_USED
+    int is_async_stopiteration = 0;
+    #endif
+    CYTHON_MAYBE_UNUSED_VAR(in_async_gen);
+    cur_exc = PyErr_Occurred();
+    if (likely(!__Pyx_PyErr_GivenExceptionMatches(cur_exc, PyExc_StopIteration))) {
+        #ifdef __Pyx_StopAsyncIteration_USED
+        if (in_async_gen && unlikely(__Pyx_PyErr_GivenExceptionMatches(cur_exc, __Pyx_PyExc_StopAsyncIteration))) {
+            is_async_stopiteration = 1;
+        } else
+        #endif
+            return;
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_GetException(&exc, &val, &tb);
+    Py_XDECREF(exc);
+    Py_XDECREF(val);
+    Py_XDECREF(tb);
+    PyErr_SetString(PyExc_RuntimeError,
+        #ifdef __Pyx_StopAsyncIteration_USED
+        is_async_stopiteration ? "async generator raised StopAsyncIteration" :
+        in_async_gen ? "async generator raised StopIteration" :
+        #endif
+        "generator raised StopIteration");
+}
+
 /* PyIntCompare */
 static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace) {
     CYTHON_MAYBE_UNUSED_VAR(intval);
     CYTHON_UNUSED_VAR(inplace);
     if (op1 == op2) {
         return 1;
     }
@@ -18037,64 +19082,14 @@
 #endif
         return ((double)a == (double)b);
     }
     return __Pyx_PyObject_IsTrueAndDecref(
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
-/* ObjectGetItem */
-#if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
-    PyObject *runerr = NULL;
-    Py_ssize_t key_value;
-    key_value = __Pyx_PyIndex_AsSsize_t(index);
-    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
-        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
-    }
-    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
-        __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
-        PyErr_Clear();
-        PyErr_Format(PyExc_IndexError,
-            "cannot fit '" __Pyx_FMT_TYPENAME "' into an index-sized integer", index_type_name);
-        __Pyx_DECREF_TypeName(index_type_name);
-    }
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
-    __Pyx_TypeName obj_type_name;
-    if (likely(PyType_Check(obj))) {
-        PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (!meth) {
-            PyErr_Clear();
-        } else {
-            PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
-            Py_DECREF(meth);
-            return result;
-        }
-    }
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError,
-        "'" __Pyx_FMT_TYPENAME "' object is not subscriptable", obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key) {
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyMappingMethods *mm = tp->tp_as_mapping;
-    PySequenceMethods *sm = tp->tp_as_sequence;
-    if (likely(mm && mm->mp_subscript)) {
-        return mm->mp_subscript(obj, key);
-    }
-    if (likely(sm && sm->sq_item)) {
-        return __Pyx_PyObject_GetIndex(obj, key);
-    }
-    return __Pyx_PyObject_GetItem_Slow(obj, key);
-}
-#endif
-
 /* RaiseClosureNameError */
 static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname) {
     PyErr_Format(PyExc_NameError, "free variable '%s' referenced before assignment in enclosing scope", varname);
 }
 
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
@@ -18193,14 +19188,115 @@
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
     PyObject *arg[2] = {NULL, NULL};
     return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
+#endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
 /* PyObjectCallMethod0 */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
     PyObject *method = NULL, *result = NULL;
     int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
     if (likely(is_method)) {
         result = __Pyx_PyObject_CallOneArg(method, obj);
         Py_DECREF(method);
@@ -18211,17 +19307,18 @@
     Py_DECREF(method);
 bad:
     return result;
 }
 
 /* UnpackUnboundCMethod */
 static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *result;
     PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
     if (unlikely(!selfless_args)) return NULL;
-    PyObject *result = PyObject_Call(method, selfless_args, kwargs);
+    result = PyObject_Call(method, selfless_args, kwargs);
     Py_DECREF(selfless_args);
     return result;
 }
 static PyMethodDef __Pyx_UnboundCMethod_Def = {
      "CythonUnboundCMethod",
      __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
      METH_VARARGS | METH_KEYWORDS,
@@ -19419,15 +20516,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -20167,15 +21264,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__2;
+    PyObject *module, *from_list, *star = __pyx_n_s__4;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -20217,14 +21314,125 @@
     } else if (PyErr_Occurred()) {
         PyErr_Clear();
     }
 #endif
     return __Pyx__ImportDottedModule(name, parts_tuple);
 }
 
+/* ImportFrom */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
+    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        const char* module_name_str = 0;
+        PyObject* module_name = 0;
+        PyObject* module_dot = 0;
+        PyObject* full_name = 0;
+        PyErr_Clear();
+        module_name_str = PyModule_GetName(module);
+        if (unlikely(!module_name_str)) { goto modbad; }
+        module_name = PyUnicode_FromString(module_name_str);
+        if (unlikely(!module_name)) { goto modbad; }
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__5);
+        if (unlikely(!module_dot)) { goto modbad; }
+        full_name = PyUnicode_Concat(module_dot, name);
+        if (unlikely(!full_name)) { goto modbad; }
+        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+        {
+            PyObject *modules = PyImport_GetModuleDict();
+            if (unlikely(!modules))
+                goto modbad;
+            value = PyObject_GetItem(modules, full_name);
+        }
+        #else
+        value = PyImport_GetModule(full_name);
+        #endif
+      modbad:
+        Py_XDECREF(full_name);
+        Py_XDECREF(module_dot);
+        Py_XDECREF(module_name);
+    }
+    if (unlikely(!value)) {
+        PyErr_Format(PyExc_ImportError,
+        #if PY_MAJOR_VERSION < 3
+            "cannot import name %.230s", PyString_AS_STRING(name));
+        #else
+            "cannot import name %S", name);
+        #endif
+    }
+    return value;
+}
+
+/* Py3UpdateBases */
+static PyObject*
+__Pyx_PEP560_update_bases(PyObject *bases)
+{
+    Py_ssize_t i, j, size_bases;
+    PyObject *base, *meth, *new_base, *result, *new_bases = NULL;
+    size_bases = PyTuple_GET_SIZE(bases);
+    for (i = 0; i < size_bases; i++) {
+        base  = PyTuple_GET_ITEM(bases, i);
+        if (PyType_Check(base)) {
+            if (new_bases) {
+                if (PyList_Append(new_bases, base) < 0) {
+                    goto error;
+                }
+            }
+            continue;
+        }
+        meth = __Pyx_PyObject_GetAttrStrNoError(base, __pyx_n_s_mro_entries);
+        if (!meth && PyErr_Occurred()) {
+            goto error;
+        }
+        if (!meth) {
+            if (new_bases) {
+                if (PyList_Append(new_bases, base) < 0) {
+                    goto error;
+                }
+            }
+            continue;
+        }
+        new_base = __Pyx_PyObject_CallOneArg(meth, bases);
+        Py_DECREF(meth);
+        if (!new_base) {
+            goto error;
+        }
+        if (!PyTuple_Check(new_base)) {
+            PyErr_SetString(PyExc_TypeError,
+                            "__mro_entries__ must return a tuple");
+            Py_DECREF(new_base);
+            goto error;
+        }
+        if (!new_bases) {
+            if (!(new_bases = PyList_New(i))) {
+                goto error;
+            }
+            for (j = 0; j < i; j++) {
+                base = PyTuple_GET_ITEM(bases, j);
+                PyList_SET_ITEM(new_bases, j, base);
+                Py_INCREF(base);
+            }
+        }
+        j = PyList_GET_SIZE(new_bases);
+        if (PyList_SetSlice(new_bases, j, j, new_base) < 0) {
+            goto error;
+        }
+        Py_DECREF(new_base);
+    }
+    if (!new_bases) {
+        Py_INCREF(bases);
+        return bases;
+    }
+    result = PyList_AsTuple(new_bases);
+    Py_DECREF(new_bases);
+    return result;
+error:
+    Py_XDECREF(new_bases);
+    return NULL;
+}
+
 /* CalculateMetaclass */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
     Py_ssize_t i, nbases;
 #if CYTHON_ASSUME_SAFE_MACROS
     nbases = PyTuple_GET_SIZE(bases);
 #else
     nbases = PyTuple_Size(bases);
@@ -20267,14 +21475,20 @@
         metaclass = &PyType_Type;
 #endif
     }
     Py_INCREF((PyObject*) metaclass);
     return (PyObject*) metaclass;
 }
 
+/* PyObjectCall2Args */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args[3] = {NULL, arg1, arg2};
+    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
 /* PyObjectLookupSpecial */
 #if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error) {
     PyObject *res;
     PyTypeObject *tp = Py_TYPE(obj);
 #if PY_MAJOR_VERSION < 3
     if (unlikely(PyInstance_Check(obj)))
@@ -20498,82 +21712,14 @@
     }
 #else
     (void) &__Pyx_GetBuiltinName;
 #endif
     return result;
 }
 
-/* Py3UpdateBases */
-static PyObject*
-__Pyx_PEP560_update_bases(PyObject *bases)
-{
-    Py_ssize_t i, j, size_bases;
-    PyObject *base, *meth, *new_base, *result, *new_bases = NULL;
-    size_bases = PyTuple_GET_SIZE(bases);
-    for (i = 0; i < size_bases; i++) {
-        base  = PyTuple_GET_ITEM(bases, i);
-        if (PyType_Check(base)) {
-            if (new_bases) {
-                if (PyList_Append(new_bases, base) < 0) {
-                    goto error;
-                }
-            }
-            continue;
-        }
-        meth = __Pyx_PyObject_GetAttrStrNoError(base, __pyx_n_s_mro_entries);
-        if (!meth && PyErr_Occurred()) {
-            goto error;
-        }
-        if (!meth) {
-            if (new_bases) {
-                if (PyList_Append(new_bases, base) < 0) {
-                    goto error;
-                }
-            }
-            continue;
-        }
-        new_base = __Pyx_PyObject_CallOneArg(meth, bases);
-        Py_DECREF(meth);
-        if (!new_base) {
-            goto error;
-        }
-        if (!PyTuple_Check(new_base)) {
-            PyErr_SetString(PyExc_TypeError,
-                            "__mro_entries__ must return a tuple");
-            Py_DECREF(new_base);
-            goto error;
-        }
-        if (!new_bases) {
-            if (!(new_bases = PyList_New(i))) {
-                goto error;
-            }
-            for (j = 0; j < i; j++) {
-                base = PyTuple_GET_ITEM(bases, j);
-                PyList_SET_ITEM(new_bases, j, base);
-                Py_INCREF(base);
-            }
-        }
-        j = PyList_GET_SIZE(new_bases);
-        if (PyList_SetSlice(new_bases, j, j, new_base) < 0) {
-            goto error;
-        }
-        Py_DECREF(new_base);
-    }
-    if (!new_bases) {
-        Py_INCREF(bases);
-        return bases;
-    }
-    result = PyList_AsTuple(new_bases);
-    Py_DECREF(new_bases);
-    return result;
-error:
-    Py_XDECREF(new_bases);
-    return NULL;
-}
-
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -20834,15 +21980,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -21258,78 +22404,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const PY_LONG_LONG neg_one = (PY_LONG_LONG) -1, const_zero = (PY_LONG_LONG) 0;
@@ -21659,14 +22741,351 @@
         Py_XDECREF(py_bytes);
         Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntFromPy */
+static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if ((sizeof(unsigned int) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(unsigned int, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (unsigned int) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(unsigned int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(unsigned int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) >= 2 * PyLong_SHIFT)) {
+                                return (unsigned int) (((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(unsigned int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) >= 3 * PyLong_SHIFT)) {
+                                return (unsigned int) (((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(unsigned int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT)) {
+                                return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (unsigned int) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if ((sizeof(unsigned int) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned int, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(unsigned int) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(unsigned int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(unsigned int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (unsigned int) (((unsigned int)-1)*(((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
+                        }
+                        break;
+                    case 2:
+                        if ((8 * sizeof(unsigned int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (unsigned int) ((((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
+                        }
+                        break;
+                    case -3:
+                        if ((8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (unsigned int) (((unsigned int)-1)*(((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(unsigned int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (unsigned int) ((((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
+                        }
+                        break;
+                    case -4:
+                        if ((8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (unsigned int) (((unsigned int)-1)*(((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(unsigned int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (unsigned int) ((((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+            if ((sizeof(unsigned int) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned int, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(unsigned int) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned int, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+            unsigned int val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+#if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+#endif
+            if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (unsigned int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (unsigned int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (unsigned int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (unsigned int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (unsigned int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(unsigned int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((unsigned int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(unsigned int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((unsigned int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((unsigned int) 1) << (sizeof(unsigned int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+            return (unsigned int) -1;
+        }
+    } else {
+        unsigned int val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (unsigned int) -1;
+        val = __Pyx_PyInt_As_unsigned_int(tmp);
+        Py_DECREF(tmp);
+        return val;
+    }
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to unsigned int");
+    return (unsigned int) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to unsigned int");
+    return (unsigned int) -1;
+}
+
 /* FormatTypeName */
 #if CYTHON_COMPILING_IN_LIMITED_API
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
@@ -22064,14 +23483,1258 @@
     if (likely(PyExceptionClass_Check(err))) {
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* SwapException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_value = exc_info->exc_value;
+    exc_info->exc_value = *value;
+    if (tmp_value == NULL || tmp_value == Py_None) {
+        Py_XDECREF(tmp_value);
+        tmp_value = NULL;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+    } else {
+        tmp_type = (PyObject*) Py_TYPE(tmp_value);
+        Py_INCREF(tmp_type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        tmp_tb = ((PyBaseExceptionObject*) tmp_value)->traceback;
+        Py_XINCREF(tmp_tb);
+        #else
+        tmp_tb = PyException_GetTraceback(tmp_value);
+        #endif
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = *type;
+    exc_info->exc_value = *value;
+    exc_info->exc_traceback = *tb;
+  #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = *type;
+    tstate->exc_value = *value;
+    tstate->exc_traceback = *tb;
+  #endif
+    *type = tmp_type;
+    *value = tmp_value;
+    *tb = tmp_tb;
+}
+#else
+static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    PyErr_GetExcInfo(&tmp_type, &tmp_value, &tmp_tb);
+    PyErr_SetExcInfo(*type, *value, *tb);
+    *type = tmp_type;
+    *value = tmp_value;
+    *tb = tmp_tb;
+}
+#endif
+
+/* PyObjectCallMethod1 */
+#if !(CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2)
+static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
+    PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
+    Py_DECREF(method);
+    return result;
+}
+#endif
+static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
+#if CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2
+    PyObject *args[2] = {obj, arg};
+    (void) __Pyx_PyObject_GetMethod;
+    (void) __Pyx_PyObject_CallOneArg;
+    (void) __Pyx_PyObject_Call2Args;
+    return PyObject_VectorcallMethod(method_name, args, 2 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
+#else
+    PyObject *method = NULL, *result;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_Call2Args(method, obj, arg);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) return NULL;
+    return __Pyx__PyObject_CallMethod1(method, arg);
+#endif
+}
+
+/* CoroutineBase */
+#include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+#define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
+static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *__pyx_tstate, PyObject **pvalue) {
+    PyObject *et, *ev, *tb;
+    PyObject *value = NULL;
+    CYTHON_UNUSED_VAR(__pyx_tstate);
+    __Pyx_ErrFetch(&et, &ev, &tb);
+    if (!et) {
+        Py_XDECREF(tb);
+        Py_XDECREF(ev);
+        Py_INCREF(Py_None);
+        *pvalue = Py_None;
+        return 0;
+    }
+    if (likely(et == PyExc_StopIteration)) {
+        if (!ev) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#if PY_VERSION_HEX >= 0x030300A0
+        else if (likely(__Pyx_IS_TYPE(ev, (PyTypeObject*)PyExc_StopIteration))) {
+            value = ((PyStopIterationObject *)ev)->value;
+            Py_INCREF(value);
+            Py_DECREF(ev);
+        }
+#endif
+        else if (unlikely(PyTuple_Check(ev))) {
+            if (PyTuple_GET_SIZE(ev) >= 1) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                value = PyTuple_GET_ITEM(ev, 0);
+                Py_INCREF(value);
+#else
+                value = PySequence_ITEM(ev, 0);
+#endif
+            } else {
+                Py_INCREF(Py_None);
+                value = Py_None;
+            }
+            Py_DECREF(ev);
+        }
+        else if (!__Pyx_TypeCheck(ev, (PyTypeObject*)PyExc_StopIteration)) {
+            value = ev;
+        }
+        if (likely(value)) {
+            Py_XDECREF(tb);
+            Py_DECREF(et);
+            *pvalue = value;
+            return 0;
+        }
+    } else if (!__Pyx_PyErr_GivenExceptionMatches(et, PyExc_StopIteration)) {
+        __Pyx_ErrRestore(et, ev, tb);
+        return -1;
+    }
+    PyErr_NormalizeException(&et, &ev, &tb);
+    if (unlikely(!PyObject_TypeCheck(ev, (PyTypeObject*)PyExc_StopIteration))) {
+        __Pyx_ErrRestore(et, ev, tb);
+        return -1;
+    }
+    Py_XDECREF(tb);
+    Py_DECREF(et);
+#if PY_VERSION_HEX >= 0x030300A0
+    value = ((PyStopIterationObject *)ev)->value;
+    Py_INCREF(value);
+    Py_DECREF(ev);
+#else
+    {
+        PyObject* args = __Pyx_PyObject_GetAttrStr(ev, __pyx_n_s_args);
+        Py_DECREF(ev);
+        if (likely(args)) {
+            value = PySequence_GetItem(args, 0);
+            Py_DECREF(args);
+        }
+        if (unlikely(!value)) {
+            __Pyx_ErrRestore(NULL, NULL, NULL);
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+    }
+#endif
+    *pvalue = value;
+    return 0;
+}
+static CYTHON_INLINE
+void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *exc_state) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_CLEAR(exc_state->exc_value);
+#else
+    PyObject *t, *v, *tb;
+    t = exc_state->exc_type;
+    v = exc_state->exc_value;
+    tb = exc_state->exc_traceback;
+    exc_state->exc_type = NULL;
+    exc_state->exc_value = NULL;
+    exc_state->exc_traceback = NULL;
+    Py_XDECREF(t);
+    Py_XDECREF(v);
+    Py_XDECREF(tb);
+#endif
+}
+#define __Pyx_Coroutine_AlreadyRunningError(gen)  (__Pyx__Coroutine_AlreadyRunningError(gen), (PyObject*)NULL)
+static void __Pyx__Coroutine_AlreadyRunningError(__pyx_CoroutineObject *gen) {
+    const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
+    if ((0)) {
+    #ifdef __Pyx_Coroutine_USED
+    } else if (__Pyx_Coroutine_Check((PyObject*)gen)) {
+        msg = "coroutine already executing";
+    #endif
+    #ifdef __Pyx_AsyncGen_USED
+    } else if (__Pyx_AsyncGen_CheckExact((PyObject*)gen)) {
+        msg = "async generator already executing";
+    #endif
+    } else {
+        msg = "generator already executing";
+    }
+    PyErr_SetString(PyExc_ValueError, msg);
+}
+#define __Pyx_Coroutine_NotStartedError(gen)  (__Pyx__Coroutine_NotStartedError(gen), (PyObject*)NULL)
+static void __Pyx__Coroutine_NotStartedError(PyObject *gen) {
+    const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
+    if ((0)) {
+    #ifdef __Pyx_Coroutine_USED
+    } else if (__Pyx_Coroutine_Check(gen)) {
+        msg = "can't send non-None value to a just-started coroutine";
+    #endif
+    #ifdef __Pyx_AsyncGen_USED
+    } else if (__Pyx_AsyncGen_CheckExact(gen)) {
+        msg = "can't send non-None value to a just-started async generator";
+    #endif
+    } else {
+        msg = "can't send non-None value to a just-started generator";
+    }
+    PyErr_SetString(PyExc_TypeError, msg);
+}
+#define __Pyx_Coroutine_AlreadyTerminatedError(gen, value, closing)  (__Pyx__Coroutine_AlreadyTerminatedError(gen, value, closing), (PyObject*)NULL)
+static void __Pyx__Coroutine_AlreadyTerminatedError(PyObject *gen, PyObject *value, int closing) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
+    CYTHON_MAYBE_UNUSED_VAR(closing);
+    #ifdef __Pyx_Coroutine_USED
+    if (!closing && __Pyx_Coroutine_Check(gen)) {
+        PyErr_SetString(PyExc_RuntimeError, "cannot reuse already awaited coroutine");
+    } else
+    #endif
+    if (value) {
+        #ifdef __Pyx_AsyncGen_USED
+        if (__Pyx_AsyncGen_CheckExact(gen))
+            PyErr_SetNone(__Pyx_PyExc_StopAsyncIteration);
+        else
+        #endif
+        PyErr_SetNone(PyExc_StopIteration);
+    }
+}
+static
+PyObject *__Pyx_Coroutine_SendEx(__pyx_CoroutineObject *self, PyObject *value, int closing) {
+    __Pyx_PyThreadState_declare
+    PyThreadState *tstate;
+    __Pyx_ExcInfoStruct *exc_state;
+    PyObject *retval;
+    assert(!self->is_running);
+    if (unlikely(self->resume_label == 0)) {
+        if (unlikely(value && value != Py_None)) {
+            return __Pyx_Coroutine_NotStartedError((PyObject*)self);
+        }
+    }
+    if (unlikely(self->resume_label == -1)) {
+        return __Pyx_Coroutine_AlreadyTerminatedError((PyObject*)self, value, closing);
+    }
+#if CYTHON_FAST_THREAD_STATE
+    __Pyx_PyThreadState_assign
+    tstate = __pyx_tstate;
+#else
+    tstate = __Pyx_PyThreadState_Current;
+#endif
+    exc_state = &self->gi_exc_state;
+    if (exc_state->exc_value) {
+        #if CYTHON_COMPILING_IN_PYPY
+        #else
+        PyObject *exc_tb;
+        #if PY_VERSION_HEX >= 0x030B00a4 && !CYTHON_COMPILING_IN_CPYTHON
+        exc_tb = PyException_GetTraceback(exc_state->exc_value);
+        #elif PY_VERSION_HEX >= 0x030B00a4
+        exc_tb = ((PyBaseExceptionObject*) exc_state->exc_value)->traceback;
+        #else
+        exc_tb = exc_state->exc_traceback;
+        #endif
+        if (exc_tb) {
+            PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
+            PyFrameObject *f = tb->tb_frame;
+            assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
+            f->f_back = tstate->frame;
+            #endif
+            #if PY_VERSION_HEX >= 0x030B00a4 && !CYTHON_COMPILING_IN_CPYTHON
+            Py_DECREF(exc_tb);
+            #endif
+        }
+        #endif
+    }
+#if CYTHON_USE_EXC_INFO_STACK
+    exc_state->previous_item = tstate->exc_info;
+    tstate->exc_info = exc_state;
+#else
+    if (exc_state->exc_type) {
+        __Pyx_ExceptionSwap(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
+    } else {
+        __Pyx_Coroutine_ExceptionClear(exc_state);
+        __Pyx_ExceptionSave(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
+    }
+#endif
+    self->is_running = 1;
+    retval = self->body(self, tstate, value);
+    self->is_running = 0;
+#if CYTHON_USE_EXC_INFO_STACK
+    exc_state = &self->gi_exc_state;
+    tstate->exc_info = exc_state->previous_item;
+    exc_state->previous_item = NULL;
+    __Pyx_Coroutine_ResetFrameBackpointer(exc_state);
+#endif
+    return retval;
+}
+static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state) {
+#if CYTHON_COMPILING_IN_PYPY
+    CYTHON_UNUSED_VAR(exc_state);
+#else
+    PyObject *exc_tb;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    if (!exc_state->exc_value) return;
+    exc_tb = PyException_GetTraceback(exc_state->exc_value);
+    #else
+    exc_tb = exc_state->exc_traceback;
+    #endif
+    if (likely(exc_tb)) {
+        PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
+        PyFrameObject *f = tb->tb_frame;
+        Py_CLEAR(f->f_back);
+        #if PY_VERSION_HEX >= 0x030B00a4
+        Py_DECREF(exc_tb);
+        #endif
+    }
+#endif
+}
+static CYTHON_INLINE
+PyObject *__Pyx_Coroutine_MethodReturn(PyObject* gen, PyObject *retval) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
+    if (unlikely(!retval)) {
+        __Pyx_PyThreadState_declare
+        __Pyx_PyThreadState_assign
+        if (!__Pyx_PyErr_Occurred()) {
+            PyObject *exc = PyExc_StopIteration;
+            #ifdef __Pyx_AsyncGen_USED
+            if (__Pyx_AsyncGen_CheckExact(gen))
+                exc = __Pyx_PyExc_StopAsyncIteration;
+            #endif
+            __Pyx_PyErr_SetNone(exc);
+        }
+    }
+    return retval;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
+static CYTHON_INLINE
+PyObject *__Pyx_PyGen_Send(PyGenObject *gen, PyObject *arg) {
+#if PY_VERSION_HEX <= 0x030A00A1
+    return _PyGen_Send(gen, arg);
+#else
+    PyObject *result;
+    if (PyIter_Send((PyObject*)gen, arg ? arg : Py_None, &result) == PYGEN_RETURN) {
+        if (PyAsyncGen_CheckExact(gen)) {
+            assert(result == Py_None);
+            PyErr_SetNone(PyExc_StopAsyncIteration);
+        }
+        else if (result == Py_None) {
+            PyErr_SetNone(PyExc_StopIteration);
+        }
+        else {
+#if PY_VERSION_HEX < 0x030d00A1
+            _PyGen_SetStopIterationValue(result);
+#else
+            if (!PyTuple_Check(result) && !PyExceptionInstance_Check(result)) {
+                PyErr_SetObject(PyExc_StopIteration, result);
+            } else {
+                PyObject *exc = __Pyx_PyObject_CallOneArg(PyExc_StopIteration, result);
+                if (likely(exc != NULL)) {
+                    PyErr_SetObject(PyExc_StopIteration, exc);
+                    Py_DECREF(exc);
+                }
+            }
+#endif
+        }
+        Py_DECREF(result);
+        result = NULL;
+    }
+    return result;
+#endif
+}
+#endif
+static CYTHON_INLINE
+PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
+    PyObject *ret;
+    PyObject *val = NULL;
+    __Pyx_Coroutine_Undelegate(gen);
+    __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, &val);
+    ret = __Pyx_Coroutine_SendEx(gen, val, 0);
+    Py_XDECREF(val);
+    return ret;
+}
+static PyObject *__Pyx_Coroutine_Send(PyObject *self, PyObject *value) {
+    PyObject *retval;
+    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject*) self;
+    PyObject *yf = gen->yieldfrom;
+    if (unlikely(gen->is_running))
+        return __Pyx_Coroutine_AlreadyRunningError(gen);
+    if (yf) {
+        PyObject *ret;
+        gen->is_running = 1;
+        #ifdef __Pyx_Generator_USED
+        if (__Pyx_Generator_CheckExact(yf)) {
+            ret = __Pyx_Coroutine_Send(yf, value);
+        } else
+        #endif
+        #ifdef __Pyx_Coroutine_USED
+        if (__Pyx_Coroutine_Check(yf)) {
+            ret = __Pyx_Coroutine_Send(yf, value);
+        } else
+        #endif
+        #ifdef __Pyx_AsyncGen_USED
+        if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
+            ret = __Pyx_async_gen_asend_send(yf, value);
+        } else
+        #endif
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
+        if (PyGen_CheckExact(yf)) {
+            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+        } else
+        #endif
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
+        if (PyCoro_CheckExact(yf)) {
+            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+        } else
+        #endif
+        {
+            if (value == Py_None)
+                ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
+            else
+                ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
+        }
+        gen->is_running = 0;
+        if (likely(ret)) {
+            return ret;
+        }
+        retval = __Pyx_Coroutine_FinishDelegation(gen);
+    } else {
+        retval = __Pyx_Coroutine_SendEx(gen, value, 0);
+    }
+    return __Pyx_Coroutine_MethodReturn(self, retval);
+}
+static int __Pyx_Coroutine_CloseIter(__pyx_CoroutineObject *gen, PyObject *yf) {
+    PyObject *retval = NULL;
+    int err = 0;
+    #ifdef __Pyx_Generator_USED
+    if (__Pyx_Generator_CheckExact(yf)) {
+        retval = __Pyx_Coroutine_Close(yf);
+        if (!retval)
+            return -1;
+    } else
+    #endif
+    #ifdef __Pyx_Coroutine_USED
+    if (__Pyx_Coroutine_Check(yf)) {
+        retval = __Pyx_Coroutine_Close(yf);
+        if (!retval)
+            return -1;
+    } else
+    if (__Pyx_CoroutineAwait_CheckExact(yf)) {
+        retval = __Pyx_CoroutineAwait_Close((__pyx_CoroutineAwaitObject*)yf, NULL);
+        if (!retval)
+            return -1;
+    } else
+    #endif
+    #ifdef __Pyx_AsyncGen_USED
+    if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
+        retval = __Pyx_async_gen_asend_close(yf, NULL);
+    } else
+    if (__pyx_PyAsyncGenAThrow_CheckExact(yf)) {
+        retval = __Pyx_async_gen_athrow_close(yf, NULL);
+    } else
+    #endif
+    {
+        PyObject *meth;
+        gen->is_running = 1;
+        meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_close);
+        if (unlikely(!meth)) {
+            if (unlikely(PyErr_Occurred())) {
+                PyErr_WriteUnraisable(yf);
+            }
+        } else {
+            retval = __Pyx_PyObject_CallNoArg(meth);
+            Py_DECREF(meth);
+            if (unlikely(!retval))
+                err = -1;
+        }
+        gen->is_running = 0;
+    }
+    Py_XDECREF(retval);
+    return err;
+}
+static PyObject *__Pyx_Generator_Next(PyObject *self) {
+    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject*) self;
+    PyObject *yf = gen->yieldfrom;
+    if (unlikely(gen->is_running))
+        return __Pyx_Coroutine_AlreadyRunningError(gen);
+    if (yf) {
+        PyObject *ret;
+        gen->is_running = 1;
+        #ifdef __Pyx_Generator_USED
+        if (__Pyx_Generator_CheckExact(yf)) {
+            ret = __Pyx_Generator_Next(yf);
+        } else
+        #endif
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
+        if (PyGen_CheckExact(yf)) {
+            ret = __Pyx_PyGen_Send((PyGenObject*)yf, NULL);
+        } else
+        #endif
+        #ifdef __Pyx_Coroutine_USED
+        if (__Pyx_Coroutine_Check(yf)) {
+            ret = __Pyx_Coroutine_Send(yf, Py_None);
+        } else
+        #endif
+            ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
+        gen->is_running = 0;
+        if (likely(ret)) {
+            return ret;
+        }
+        return __Pyx_Coroutine_FinishDelegation(gen);
+    }
+    return __Pyx_Coroutine_SendEx(gen, Py_None, 0);
+}
+static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
+    return __Pyx_Coroutine_Close(self);
+}
+static PyObject *__Pyx_Coroutine_Close(PyObject *self) {
+    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
+    PyObject *retval, *raised_exception;
+    PyObject *yf = gen->yieldfrom;
+    int err = 0;
+    if (unlikely(gen->is_running))
+        return __Pyx_Coroutine_AlreadyRunningError(gen);
+    if (yf) {
+        Py_INCREF(yf);
+        err = __Pyx_Coroutine_CloseIter(gen, yf);
+        __Pyx_Coroutine_Undelegate(gen);
+        Py_DECREF(yf);
+    }
+    if (err == 0)
+        PyErr_SetNone(PyExc_GeneratorExit);
+    retval = __Pyx_Coroutine_SendEx(gen, NULL, 1);
+    if (unlikely(retval)) {
+        const char *msg;
+        Py_DECREF(retval);
+        if ((0)) {
+        #ifdef __Pyx_Coroutine_USED
+        } else if (__Pyx_Coroutine_Check(self)) {
+            msg = "coroutine ignored GeneratorExit";
+        #endif
+        #ifdef __Pyx_AsyncGen_USED
+        } else if (__Pyx_AsyncGen_CheckExact(self)) {
+#if PY_VERSION_HEX < 0x03060000
+            msg = "async generator ignored GeneratorExit - might require Python 3.6+ finalisation (PEP 525)";
+#else
+            msg = "async generator ignored GeneratorExit";
+#endif
+        #endif
+        } else {
+            msg = "generator ignored GeneratorExit";
+        }
+        PyErr_SetString(PyExc_RuntimeError, msg);
+        return NULL;
+    }
+    raised_exception = PyErr_Occurred();
+    if (likely(!raised_exception || __Pyx_PyErr_GivenExceptionMatches2(raised_exception, PyExc_GeneratorExit, PyExc_StopIteration))) {
+        if (raised_exception) PyErr_Clear();
+        Py_INCREF(Py_None);
+        return Py_None;
+    }
+    return NULL;
+}
+static PyObject *__Pyx__Coroutine_Throw(PyObject *self, PyObject *typ, PyObject *val, PyObject *tb,
+                                        PyObject *args, int close_on_genexit) {
+    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
+    PyObject *yf = gen->yieldfrom;
+    if (unlikely(gen->is_running))
+        return __Pyx_Coroutine_AlreadyRunningError(gen);
+    if (yf) {
+        PyObject *ret;
+        Py_INCREF(yf);
+        if (__Pyx_PyErr_GivenExceptionMatches(typ, PyExc_GeneratorExit) && close_on_genexit) {
+            int err = __Pyx_Coroutine_CloseIter(gen, yf);
+            Py_DECREF(yf);
+            __Pyx_Coroutine_Undelegate(gen);
+            if (err < 0)
+                return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
+            goto throw_here;
+        }
+        gen->is_running = 1;
+        if (0
+        #ifdef __Pyx_Generator_USED
+            || __Pyx_Generator_CheckExact(yf)
+        #endif
+        #ifdef __Pyx_Coroutine_USED
+            || __Pyx_Coroutine_Check(yf)
+        #endif
+            ) {
+            ret = __Pyx__Coroutine_Throw(yf, typ, val, tb, args, close_on_genexit);
+        #ifdef __Pyx_Coroutine_USED
+        } else if (__Pyx_CoroutineAwait_CheckExact(yf)) {
+            ret = __Pyx__Coroutine_Throw(((__pyx_CoroutineAwaitObject*)yf)->coroutine, typ, val, tb, args, close_on_genexit);
+        #endif
+        } else {
+            PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_throw);
+            if (unlikely(!meth)) {
+                Py_DECREF(yf);
+                if (unlikely(PyErr_Occurred())) {
+                    gen->is_running = 0;
+                    return NULL;
+                }
+                __Pyx_Coroutine_Undelegate(gen);
+                gen->is_running = 0;
+                goto throw_here;
+            }
+            if (likely(args)) {
+                ret = __Pyx_PyObject_Call(meth, args, NULL);
+            } else {
+                PyObject *cargs[4] = {NULL, typ, val, tb};
+                ret = __Pyx_PyObject_FastCall(meth, cargs+1, 3 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+            }
+            Py_DECREF(meth);
+        }
+        gen->is_running = 0;
+        Py_DECREF(yf);
+        if (!ret) {
+            ret = __Pyx_Coroutine_FinishDelegation(gen);
+        }
+        return __Pyx_Coroutine_MethodReturn(self, ret);
+    }
+throw_here:
+    __Pyx_Raise(typ, val, tb, NULL);
+    return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
+}
+static PyObject *__Pyx_Coroutine_Throw(PyObject *self, PyObject *args) {
+    PyObject *typ;
+    PyObject *val = NULL;
+    PyObject *tb = NULL;
+    if (unlikely(!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb)))
+        return NULL;
+    return __Pyx__Coroutine_Throw(self, typ, val, tb, args, 1);
+}
+static CYTHON_INLINE int __Pyx_Coroutine_traverse_excstate(__Pyx_ExcInfoStruct *exc_state, visitproc visit, void *arg) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_VISIT(exc_state->exc_value);
+#else
+    Py_VISIT(exc_state->exc_type);
+    Py_VISIT(exc_state->exc_value);
+    Py_VISIT(exc_state->exc_traceback);
+#endif
+    return 0;
+}
+static int __Pyx_Coroutine_traverse(__pyx_CoroutineObject *gen, visitproc visit, void *arg) {
+    Py_VISIT(gen->closure);
+    Py_VISIT(gen->classobj);
+    Py_VISIT(gen->yieldfrom);
+    return __Pyx_Coroutine_traverse_excstate(&gen->gi_exc_state, visit, arg);
+}
+static int __Pyx_Coroutine_clear(PyObject *self) {
+    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
+    Py_CLEAR(gen->closure);
+    Py_CLEAR(gen->classobj);
+    Py_CLEAR(gen->yieldfrom);
+    __Pyx_Coroutine_ExceptionClear(&gen->gi_exc_state);
+#ifdef __Pyx_AsyncGen_USED
+    if (__Pyx_AsyncGen_CheckExact(self)) {
+        Py_CLEAR(((__pyx_PyAsyncGenObject*)gen)->ag_finalizer);
+    }
+#endif
+    Py_CLEAR(gen->gi_code);
+    Py_CLEAR(gen->gi_frame);
+    Py_CLEAR(gen->gi_name);
+    Py_CLEAR(gen->gi_qualname);
+    Py_CLEAR(gen->gi_modulename);
+    return 0;
+}
+static void __Pyx_Coroutine_dealloc(PyObject *self) {
+    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
+    PyObject_GC_UnTrack(gen);
+    if (gen->gi_weakreflist != NULL)
+        PyObject_ClearWeakRefs(self);
+    if (gen->resume_label >= 0) {
+        PyObject_GC_Track(self);
+#if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
+        if (unlikely(PyObject_CallFinalizerFromDealloc(self)))
+#else
+        Py_TYPE(gen)->tp_del(self);
+        if (unlikely(Py_REFCNT(self) > 0))
+#endif
+        {
+            return;
+        }
+        PyObject_GC_UnTrack(self);
+    }
+#ifdef __Pyx_AsyncGen_USED
+    if (__Pyx_AsyncGen_CheckExact(self)) {
+        /* We have to handle this case for asynchronous generators
+           right here, because this code has to be between UNTRACK
+           and GC_Del. */
+        Py_CLEAR(((__pyx_PyAsyncGenObject*)self)->ag_finalizer);
+    }
+#endif
+    __Pyx_Coroutine_clear(self);
+    __Pyx_PyHeapTypeObject_GC_Del(gen);
+}
+static void __Pyx_Coroutine_del(PyObject *self) {
+    PyObject *error_type, *error_value, *error_traceback;
+    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
+    __Pyx_PyThreadState_declare
+    if (gen->resume_label < 0) {
+        return;
+    }
+#if !CYTHON_USE_TP_FINALIZE
+    assert(self->ob_refcnt == 0);
+    __Pyx_SET_REFCNT(self, 1);
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&error_type, &error_value, &error_traceback);
+#ifdef __Pyx_AsyncGen_USED
+    if (__Pyx_AsyncGen_CheckExact(self)) {
+        __pyx_PyAsyncGenObject *agen = (__pyx_PyAsyncGenObject*)self;
+        PyObject *finalizer = agen->ag_finalizer;
+        if (finalizer && !agen->ag_closed) {
+            PyObject *res = __Pyx_PyObject_CallOneArg(finalizer, self);
+            if (unlikely(!res)) {
+                PyErr_WriteUnraisable(self);
+            } else {
+                Py_DECREF(res);
+            }
+            __Pyx_ErrRestore(error_type, error_value, error_traceback);
+            return;
+        }
+    }
+#endif
+    if (unlikely(gen->resume_label == 0 && !error_value)) {
+#ifdef __Pyx_Coroutine_USED
+#ifdef __Pyx_Generator_USED
+    if (!__Pyx_Generator_CheckExact(self))
+#endif
+        {
+        PyObject_GC_UnTrack(self);
+#if PY_MAJOR_VERSION >= 3  || defined(PyErr_WarnFormat)
+        if (unlikely(PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "coroutine '%.50S' was never awaited", gen->gi_qualname) < 0))
+            PyErr_WriteUnraisable(self);
+#else
+        {PyObject *msg;
+        char *cmsg;
+        #if CYTHON_COMPILING_IN_PYPY
+        msg = NULL;
+        cmsg = (char*) "coroutine was never awaited";
+        #else
+        char *cname;
+        PyObject *qualname;
+        qualname = gen->gi_qualname;
+        cname = PyString_AS_STRING(qualname);
+        msg = PyString_FromFormat("coroutine '%.50s' was never awaited", cname);
+        if (unlikely(!msg)) {
+            PyErr_Clear();
+            cmsg = (char*) "coroutine was never awaited";
+        } else {
+            cmsg = PyString_AS_STRING(msg);
+        }
+        #endif
+        if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, cmsg, 1) < 0))
+            PyErr_WriteUnraisable(self);
+        Py_XDECREF(msg);}
+#endif
+        PyObject_GC_Track(self);
+        }
+#endif
+    } else {
+        PyObject *res = __Pyx_Coroutine_Close(self);
+        if (unlikely(!res)) {
+            if (PyErr_Occurred())
+                PyErr_WriteUnraisable(self);
+        } else {
+            Py_DECREF(res);
+        }
+    }
+    __Pyx_ErrRestore(error_type, error_value, error_traceback);
+#if !CYTHON_USE_TP_FINALIZE
+    assert(Py_REFCNT(self) > 0);
+    if (likely(--self->ob_refcnt == 0)) {
+        return;
+    }
+    {
+        Py_ssize_t refcnt = Py_REFCNT(self);
+        _Py_NewReference(self);
+        __Pyx_SET_REFCNT(self, refcnt);
+    }
+#if CYTHON_COMPILING_IN_CPYTHON
+    assert(PyType_IS_GC(Py_TYPE(self)) &&
+           _Py_AS_GC(self)->gc.gc_refs != _PyGC_REFS_UNTRACKED);
+    _Py_DEC_REFTOTAL;
+#endif
+#ifdef COUNT_ALLOCS
+    --Py_TYPE(self)->tp_frees;
+    --Py_TYPE(self)->tp_allocs;
+#endif
+#endif
+}
+static PyObject *
+__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, void *context)
+{
+    PyObject *name = self->gi_name;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!name)) name = Py_None;
+    Py_INCREF(name);
+    return name;
+}
+static int
+__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(self->gi_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, void *context)
+{
+    PyObject *name = self->gi_qualname;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!name)) name = Py_None;
+    Py_INCREF(name);
+    return name;
+}
+static int
+__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(self->gi_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, void *context)
+{
+    PyObject *frame = self->gi_frame;
+    CYTHON_UNUSED_VAR(context);
+    if (!frame) {
+        if (unlikely(!self->gi_code)) {
+            Py_RETURN_NONE;
+        }
+        frame = (PyObject *) PyFrame_New(
+            PyThreadState_Get(),            /*PyThreadState *tstate,*/
+            (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
+            __pyx_d,                 /*PyObject *globals,*/
+            0                               /*PyObject *locals*/
+        );
+        if (unlikely(!frame))
+            return NULL;
+        self->gi_frame = frame;
+    }
+    Py_INCREF(frame);
+    return frame;
+}
+static __pyx_CoroutineObject *__Pyx__Coroutine_New(
+            PyTypeObject* type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
+            PyObject *name, PyObject *qualname, PyObject *module_name) {
+    __pyx_CoroutineObject *gen = PyObject_GC_New(__pyx_CoroutineObject, type);
+    if (unlikely(!gen))
+        return NULL;
+    return __Pyx__Coroutine_NewInit(gen, body, code, closure, name, qualname, module_name);
+}
+static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
+            __pyx_CoroutineObject *gen, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
+            PyObject *name, PyObject *qualname, PyObject *module_name) {
+    gen->body = body;
+    gen->closure = closure;
+    Py_XINCREF(closure);
+    gen->is_running = 0;
+    gen->resume_label = 0;
+    gen->classobj = NULL;
+    gen->yieldfrom = NULL;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    gen->gi_exc_state.exc_value = NULL;
+    #else
+    gen->gi_exc_state.exc_type = NULL;
+    gen->gi_exc_state.exc_value = NULL;
+    gen->gi_exc_state.exc_traceback = NULL;
+    #endif
+#if CYTHON_USE_EXC_INFO_STACK
+    gen->gi_exc_state.previous_item = NULL;
+#endif
+    gen->gi_weakreflist = NULL;
+    Py_XINCREF(qualname);
+    gen->gi_qualname = qualname;
+    Py_XINCREF(name);
+    gen->gi_name = name;
+    Py_XINCREF(module_name);
+    gen->gi_modulename = module_name;
+    Py_XINCREF(code);
+    gen->gi_code = code;
+    gen->gi_frame = NULL;
+    PyObject_GC_Track(gen);
+    return gen;
+}
+
+/* PatchModuleWithCoroutine */
+static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
+#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
+    int result;
+    PyObject *globals, *result_obj;
+    globals = PyDict_New();  if (unlikely(!globals)) goto ignore;
+    result = PyDict_SetItemString(globals, "_cython_coroutine_type",
+    #ifdef __Pyx_Coroutine_USED
+        (PyObject*)__pyx_CoroutineType);
+    #else
+        Py_None);
+    #endif
+    if (unlikely(result < 0)) goto ignore;
+    result = PyDict_SetItemString(globals, "_cython_generator_type",
+    #ifdef __Pyx_Generator_USED
+        (PyObject*)__pyx_GeneratorType);
+    #else
+        Py_None);
+    #endif
+    if (unlikely(result < 0)) goto ignore;
+    if (unlikely(PyDict_SetItemString(globals, "_module", module) < 0)) goto ignore;
+    if (unlikely(PyDict_SetItemString(globals, "__builtins__", __pyx_b) < 0)) goto ignore;
+    result_obj = PyRun_String(py_code, Py_file_input, globals, globals);
+    if (unlikely(!result_obj)) goto ignore;
+    Py_DECREF(result_obj);
+    Py_DECREF(globals);
+    return module;
+ignore:
+    Py_XDECREF(globals);
+    PyErr_WriteUnraisable(module);
+    if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, "Cython module failed to patch module with custom type", 1) < 0)) {
+        Py_DECREF(module);
+        module = NULL;
+    }
+#else
+    py_code++;
+#endif
+    return module;
+}
+
+/* PatchGeneratorABC */
+#ifndef CYTHON_REGISTER_ABCS
+#define CYTHON_REGISTER_ABCS 1
+#endif
+#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
+static PyObject* __Pyx_patch_abc_module(PyObject *module);
+static PyObject* __Pyx_patch_abc_module(PyObject *module) {
+    module = __Pyx_Coroutine_patch_module(
+        module, ""
+"if _cython_generator_type is not None:\n"
+"    try: Generator = _module.Generator\n"
+"    except AttributeError: pass\n"
+"    else: Generator.register(_cython_generator_type)\n"
+"if _cython_coroutine_type is not None:\n"
+"    try: Coroutine = _module.Coroutine\n"
+"    except AttributeError: pass\n"
+"    else: Coroutine.register(_cython_coroutine_type)\n"
+    );
+    return module;
+}
+#endif
+static int __Pyx_patch_abc(void) {
+#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
+    static int abc_patched = 0;
+    if (CYTHON_REGISTER_ABCS && !abc_patched) {
+        PyObject *module;
+        module = PyImport_ImportModule((PY_MAJOR_VERSION >= 3) ? "collections.abc" : "collections");
+        if (unlikely(!module)) {
+            PyErr_WriteUnraisable(NULL);
+            if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning,
+                    ((PY_MAJOR_VERSION >= 3) ?
+                        "Cython module failed to register with collections.abc module" :
+                        "Cython module failed to register with collections module"), 1) < 0)) {
+                return -1;
+            }
+        } else {
+            module = __Pyx_patch_abc_module(module);
+            abc_patched = 1;
+            if (unlikely(!module))
+                return -1;
+            Py_DECREF(module);
+        }
+        module = PyImport_ImportModule("backports_abc");
+        if (module) {
+            module = __Pyx_patch_abc_module(module);
+            Py_XDECREF(module);
+        }
+        if (!module) {
+            PyErr_Clear();
+        }
+    }
+#else
+    if ((0)) __Pyx_Coroutine_patch_module(NULL, NULL);
+#endif
+    return 0;
+}
+
+/* Generator */
+static PyMethodDef __pyx_Generator_methods[] = {
+    {"send", (PyCFunction) __Pyx_Coroutine_Send, METH_O,
+     (char*) PyDoc_STR("send(arg) -> send 'arg' into generator,\nreturn next yielded value or raise StopIteration.")},
+    {"throw", (PyCFunction) __Pyx_Coroutine_Throw, METH_VARARGS,
+     (char*) PyDoc_STR("throw(typ[,val[,tb]]) -> raise exception in generator,\nreturn next yielded value or raise StopIteration.")},
+    {"close", (PyCFunction) __Pyx_Coroutine_Close_Method, METH_NOARGS,
+     (char*) PyDoc_STR("close() -> raise GeneratorExit inside generator.")},
+    {0, 0, 0, 0}
+};
+static PyMemberDef __pyx_Generator_memberlist[] = {
+    {(char *) "gi_running", T_BOOL, offsetof(__pyx_CoroutineObject, is_running), READONLY, NULL},
+    {(char*) "gi_yieldfrom", T_OBJECT, offsetof(__pyx_CoroutineObject, yieldfrom), READONLY,
+     (char*) PyDoc_STR("object being iterated by 'yield from', or None")},
+    {(char*) "gi_code", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_code), READONLY, NULL},
+    {(char *) "__module__", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_modulename), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CoroutineObject, gi_weakreflist), READONLY, 0},
+#endif
+    {0, 0, 0, 0, 0}
+};
+static PyGetSetDef __pyx_Generator_getsets[] = {
+    {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
+     (char*) PyDoc_STR("name of the generator"), 0},
+    {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
+     (char*) PyDoc_STR("qualified name of the generator"), 0},
+    {(char *) "gi_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
+     (char*) PyDoc_STR("Frame of the generator"), 0},
+    {0, 0, 0, 0, 0}
+};
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_GeneratorType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_Coroutine_dealloc},
+    {Py_tp_traverse, (void *)__Pyx_Coroutine_traverse},
+    {Py_tp_iter, (void *)PyObject_SelfIter},
+    {Py_tp_iternext, (void *)__Pyx_Generator_Next},
+    {Py_tp_methods, (void *)__pyx_Generator_methods},
+    {Py_tp_members, (void *)__pyx_Generator_memberlist},
+    {Py_tp_getset, (void *)__pyx_Generator_getsets},
+    {Py_tp_getattro, (void *) __Pyx_PyObject_GenericGetAttrNoDict},
+#if CYTHON_USE_TP_FINALIZE
+    {Py_tp_finalize, (void *)__Pyx_Coroutine_del},
+#endif
+    {0, 0},
+};
+static PyType_Spec __pyx_GeneratorType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "generator",
+    sizeof(__pyx_CoroutineObject),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
+    __pyx_GeneratorType_slots
+};
+#else
+static PyTypeObject __pyx_GeneratorType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "generator",
+    sizeof(__pyx_CoroutineObject),
+    0,
+    (destructor) __Pyx_Coroutine_dealloc,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
+    0,
+    (traverseproc) __Pyx_Coroutine_traverse,
+    0,
+    0,
+    offsetof(__pyx_CoroutineObject, gi_weakreflist),
+    0,
+    (iternextfunc) __Pyx_Generator_Next,
+    __pyx_Generator_methods,
+    __pyx_Generator_memberlist,
+    __pyx_Generator_getsets,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if CYTHON_USE_TP_FINALIZE
+    0,
+#else
+    __Pyx_Coroutine_del,
+#endif
+    0,
+#if CYTHON_USE_TP_FINALIZE
+    __Pyx_Coroutine_del,
+#elif PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_Generator_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_GeneratorType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_GeneratorType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+    __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
+    __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
+#endif
+    if (unlikely(!__pyx_GeneratorType)) {
+        return -1;
+    }
+    return 0;
+}
+
 /* CheckBinaryVersion */
 static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
```

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/pyvoronoi.pyx` & `pyvoronoi-1.1.0/pyvoronoi/pyvoronoi.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 import sys as _sys
 import struct
 import copy as _copy
 import unicodedata as _unicodedata
 import time as _time
 import math
-
+import typing
+from typing import NamedTuple
 from cython.operator cimport dereference as deref
 
 SILENT = True
 def log_action(description):
     if not SILENT:
         print(description)
 
@@ -93,74 +94,59 @@
     cdef cppclass VoronoiDiagram:
         VoronoiDiagram()
         void AddPoint(Point p)
         void AddSegment(Segment s)
         void Construct()
         vector[Point] GetPoints()
         vector[Segment] GetSegments()
+        Point GetPoint(unsigned index)
+        Segment GetSegment(unsigned index)
 
         void MapVertexIndexes()
         void MapEdgeIndexes()
         void MapCellIndexes()
 
+        long long CountPoints();
+        long long CountSegments();
         long long CountVertices()
         long long CountEdges()
         long long CountCells()
 
         c_Vertex GetVertex(long long index)
         c_Edge GetEdge(long long index)
         c_Cell GetCell(long long index)
 
 
 
 ####################################
 ##VORONOY UTILS
 ####################################
-class Vertex:
-    X = 0.0
-    Y = 0.0
-    def __init__(self,x,y):
-        self.X = x
-        self.Y = y
-
-class Edge:
-    start = -1
-    end = -1
-    is_primary = False
-    is_linear = False
-    cell = -1
-    twin = -1
-
-    def __init__(self, start, end, cell, twin):
-        self.start = start
-        self.end = end
-        self.cell = cell
-        self.twin = twin
-
-class Cell:
-    cell_identifier = -1
-    site = -1
-    contains_point = False
-    contains_segment = False
-    is_open = False
-
-    vertices = []
-    edges = []
-
-    source_category = None
-
-    def __init__(self, cell_identifier, site, vertices, edges, source_category):
-        self.cell_identifier = cell_identifier
-        self.site = site
-        self.source_category = source_category
-        self.vertices = vertices
-        self.edges = edges
-        if len(self.vertices) > 0:
-            self.vertices.append(self.vertices[0])
-
+class Vertex(NamedTuple):
+    X : float = 0.0
+    Y : float = 0.0
+
+class Edge(NamedTuple):
+    start : int =  -1
+    end : int = -1
+    is_primary : bool = False
+    is_linear : bool =  False
+    cell : int = -1
+    twin : int = -1
+
+
+class Cell(NamedTuple):
+    cell_identifier : int = -1
+    site : int = -1
+    contains_point : bool = False
+    contains_segment : bool = False
+    is_open : bool = False
+    is_degenerate: bool = False
+    vertices : [typing.Type[Vertex]] = []
+    edges : [typing.Type[Edge]] = []
+    source_category : int  = None
 
 class VoronoiException(Exception):
     pass
 
 class FocusOnDirectixException(Exception):
     pass
 
@@ -206,141 +192,154 @@
 ####################################
 ##PYVORONOI OPERATIONS
 ####################################
 
 cdef class Pyvoronoi:
     cdef VoronoiDiagram *thisptr
     cdef int constructed
-
-    inputPoints = []
-    inputSegments = []
-    outputEdges = []
-    outputVertices = []
-    outputCells = []
-
     cdef public int SCALING_FACTOR
 
-    def __cinit__(self, scaling_factor = None):
+    def __cinit__(self, scaling_factor = 1):
         """ Creates an instance of the Pyvoronoi class.
         """
         log_action("Creating an VoronoiDiagram instance")
+
         self.thisptr = new VoronoiDiagram()
         self.constructed = 0
-
-        if scaling_factor != None:
-            self.SCALING_FACTOR = scaling_factor
-        else:
-            self.SCALING_FACTOR = 1
-
-        del self.inputPoints[:]
-        del self.inputSegments[:]
+        self.SCALING_FACTOR = scaling_factor if scaling_factor is not None else 1
 
     def __dealloc__(self):
         log_action("Deleting the VoronoiDiagram instance")
         del self.thisptr
 
     def AddPoint(self, point):
         """ Add a point
         """
 
         if self.constructed == 1:
             raise VoronoiException('Construct() has been called, can\'t add more elements')
 
         cdef Point c_point = self._to_voronoi_point(point)
         self.thisptr.AddPoint(c_point)
-        self.inputPoints.append([c_point.X, c_point.Y])
 
     def AddSegment(self, segment):
         """ Add a segment
         """
 
         if self.constructed == 1:
             raise VoronoiException('Construct() has been called, can\'t add more elements')
 
         cdef Segment c_segment = self._to_voronoi_segment(segment)
         self.thisptr.AddSegment(c_segment)
-        self.inputSegments.append([[c_segment.p0.X, c_segment.p0.Y], [c_segment.p1.X, c_segment.p1.Y]])
 
     def Construct(self):
         """ Generates the voronoi diagram for the added points and segments. Voronoi cell structure will be generated.
         """
 
         if self.constructed == 1:
             raise VoronoiException('Construct() has already been called')
 
         self.constructed = 1
-
         self.thisptr.Construct()
-
         self.thisptr.MapVertexIndexes()
         self.thisptr.MapEdgeIndexes()
         self.thisptr.MapCellIndexes()
 
     def GetVertex(self, index):
         """
         """
         c_vertex = self.thisptr.GetVertex(index)
-        return Vertex(c_vertex.X / self.SCALING_FACTOR, c_vertex.Y / self.SCALING_FACTOR)
+        return Vertex(
+            X=c_vertex.X / self.SCALING_FACTOR, 
+            Y=c_vertex.Y / self.SCALING_FACTOR
+        )
 
     def GetEdge(self, index):
         c_edge =  self.thisptr.GetEdge(index)
-        edge = Edge(c_edge.start, c_edge.end, c_edge.cell, c_edge.twin)
-        edge.is_primary = c_edge.isPrimary != False
-        edge.is_linear = c_edge.isLinear != False
+        edge = Edge(
+            start=c_edge.start,
+            end=c_edge.end,
+            cell=c_edge.cell,
+            twin=c_edge.twin,
+            is_primary= c_edge.isPrimary != False,
+            is_linear = c_edge.isLinear != False
+        )
         return edge
 
     def GetCell(self, index):
         c_cell = self.thisptr.GetCell(index)
-        cell = Cell(c_cell.cell_identifier, c_cell.site, c_cell.vertices, c_cell.edges, c_cell.source_category)
-        cell.contains_point = c_cell.contains_point != False
-        cell.contains_segment = c_cell.contains_segment != False
-        cell.is_degenerate = c_cell.is_degenerate != False
-        cell.is_open = c_cell.is_open != False
+        cell = Cell(
+            cell_identifier=c_cell.cell_identifier,
+            site=c_cell.site,
+            vertices=c_cell.vertices,
+            edges=c_cell.edges,
+            source_category=c_cell.source_category,
+            contains_point=c_cell.contains_point != False,
+            contains_segment=c_cell.contains_segment != False,
+            is_degenerate=c_cell.is_degenerate != False,
+            is_open = c_cell.is_open != False
+        )
         return cell
 
     def CountVertices(self):
         return self.thisptr.CountVertices()
 
     def CountEdges(self):
         return self.thisptr.CountEdges()
 
     def CountCells(self):
         return self.thisptr.CountCells()
 
     def GetPoints(self):
         """ Returns the points added to the voronoi diagram
         """
-        return self.inputPoints
+        return [[p.X , p.Y ] for p in self.thisptr.GetPoints()]
+
 
     def GetSegments(self):
         """ Returns the segments added to the voronoi diagram
         """
-        return self.inputSegments
+        return [[[s.p0.X, s.p0.Y], [s.p1.X, s.p1.Y]] for s in self.thisptr.GetSegments()]
 
     def GetVertices(self):
         count = self.CountVertices()
         output = []
         for index in  range(count):
             output.append(self.GetVertex(index))
         return output
 
+    def IterateVertices(self):
+        count = self.CountVertices()
+        for index in  range(count):
+            yield self.GetVertex(index)
+
     def GetEdges(self):
         count = self.CountEdges()
         output = []
         for index in range(count):
             output.append(self.GetEdge(index))
         return output
 
+    def IterateEdges(self):
+        count = self.CountEdges()
+        for index in range(count):
+            yield self.GetEdge(index)
+
     def GetCells(self):
         count = self.CountCells()
         output = []
         for index in range(count):
             output.append(self.GetCell(index))
         return output
 
+    def IterateCells(self):
+        count = self.CountCells()
+        for index in range(count):
+            yield self.GetCell(index)
+
     def ReturnCurvedSiteInformation(self, edge):
         """Return the index of the point side and the segment site associated  with a segment index
         """
         twinEdge = self.GetEdge(edge.twin)
 
         cell = self.GetCell(edge.cell)
         twinCell = self.GetCell(twinEdge.cell)
@@ -368,27 +367,31 @@
 
 
     def RetrievePoint(self, cell):
         """Retrive the input point associated with a cell.
 		:param cell: the cell that contains a point. The point can be either a input point or the end point of an input segment.
         """
         if(cell.source_category == 0):
-            return self.inputPoints[cell.site]
+            point = self.thisptr.GetPoint(cell.site)
+            return [point.X, point.Y]
 
         input_segment = self.RetrieveSegment(cell)
         if(cell.source_category == 1):
             return input_segment[0]
         else:
             return input_segment[1]
 
     def RetrieveSegment(self, cell):
         """Retrive the input segment associated with a cell.
         """
-        return self.inputSegments[cell.site - len(self.inputPoints)]
-
+        segment = self.thisptr.GetSegment(cell.site - self.thisptr.CountPoints())
+        return [
+            [segment.p0.X,segment.p0.Y],
+            [segment.p1.X, segment.p1.Y]
+        ]
 
     def RetrieveScaledPoint(self, cell):
         non_scaled_point = self.RetrievePoint(cell)
         return [
 			non_scaled_point[0] / self.SCALING_FACTOR,
 			non_scaled_point[1] / self.SCALING_FACTOR
 		]
```

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/voronoi.cpp` & `pyvoronoi-1.1.0/pyvoronoi/voronoi.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -18,18 +18,34 @@
 	construct_voronoi(points.begin(), points.end(), segments.begin(), segments.end(), &vd);
 }
 
 std::vector<Point> VoronoiDiagram::GetPoints() {
 	return points;
 }
 
+Point VoronoiDiagram::GetPoint(unsigned index) {
+	return points.at(index);
+}
+
 std::vector<Segment> VoronoiDiagram::GetSegments() {
 	return segments;
 }
 
+Segment VoronoiDiagram::GetSegment(unsigned index) {
+	return segments.at(index);
+}
+
+long long VoronoiDiagram::CountPoints(){
+	return points.size();
+}
+
+long long VoronoiDiagram::CountSegments(){
+	return segments.size();
+}
+
 long long VoronoiDiagram::CountVertices(){
 	return vd.num_vertices();
 }
 
 long long VoronoiDiagram::CountEdges(){
 	return vd.num_edges();
 }
@@ -166,25 +182,20 @@
 				edge_start = map_vertices_to_indexes[edge->vertex0()];
 			}
 
 			if (edge->vertex1() != NULL){
 				edge_end = map_vertices_to_indexes[edge->vertex1()];
 			}
 
-			long vertices_count = vertex_identifiers.size();
-			if (vertices_count == 0){
-				vertex_identifiers.push_back(edge_start);
-			}
-			else{
-				if (vertex_identifiers[vertices_count - 1] != edge_start){
-					vertex_identifiers.push_back(edge_start);
-				}
-			}
+			//long vertices_count = vertex_identifiers.size();
+			vertex_identifiers.push_back(edge_start);
+            if ( vertex_identifiers.back() == edge_start){
+                vertex_identifiers.push_back(edge_end);
+            }
 
-			vertex_identifiers.push_back(edge_end);
 			//Move to the next edge
 			edge = edge->next();
 
 		} while (edge != cell->incident_edge());
 	}
 
 	c_Cell c_cell = c_Cell(
@@ -197,8 +208,8 @@
 	);
 
 	c_cell.is_degenerate = cell->is_degenerate();
 	c_cell.vertices = vertex_identifiers;
 	c_cell.edges = edge_identifiers;
 
 	return c_cell;
-}
+}
```

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi/voronoi.hpp` & `pyvoronoi-1.1.0/pyvoronoi/voronoi.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -111,16 +111,21 @@
 public:
 	VoronoiDiagram();
 	void AddPoint(Point p);
 	void AddSegment(Segment s);
 	void Construct();
 
 	std::vector<Point> GetPoints();
+	Point GetPoint(unsigned index);
 	std::vector<Segment> GetSegments();
+	Segment GetSegment(unsigned index);
 
+
+	long long CountPoints();
+	long long CountSegments();
 	long long CountVertices();
 	long long CountEdges();
 	long long CountCells();
 
 	//Map index to vertex
 	typedef std::pair<long long, const voronoi_diagram<double>::vertex_type*> index_to_vertex;
 	std::map<long long, const voronoi_diagram<double>::vertex_type*> map_indexes_to_vertices;
```

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi.egg-info/PKG-INFO` & `pyvoronoi-1.1.0/pyvoronoi.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pyvoronoi
-Version: 1.0.9.4
+Version: 1.1.0
 Summary: Cython wrapper for the Boost Voronoi library (version 1.59.0)
 Home-page: https://github.com/fabanc/pyvoronoi
 Author: Fabien Ancelin / Andrii Sydorchuk, Voxel8
 Author-email: 
+License: UNKNOWN
 Keywords: voronoi,Boost,polygon
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: Environment :: Other Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,15 +27,17 @@
 
 # pyvoronoi
 
 A wrapper for Boost's Voronoi diagram library. The full documentation of the Boost Voronoi API is available [here](https://www.boost.org/doc/libs/1_75_0/libs/polygon/doc/voronoi_main.htm).
 
 ## Install
 
-The install have been tested on Windows and Linux Ubuntu. If you notice any issue on Mac, reach out to me, I am interested in making sure it works for you.
+The installation have been tested on Windows and Linux Ubuntu. If you notice any issue on Mac, reach out to us, we are interested in making sure it works for you.
+
+Windows users will need Microsoft Visual C++ installed on their machine. You can find information about the version needed on [this](https://wiki.python.org/moin/WindowsCompilers) link. Python version from 3.5 to 3.12 rely on Visual C++ 14.x.
 
 ### Dependencies
 
 Cython dependency is optional. Cpp sources generated with Cython are available in releases.
 
 Note on using the setup.py:
 
@@ -59,14 +63,19 @@
 
 Cython required.
 
 Clone the repository:
 
 ``git clone https://github.com/fabanc/pyvoronoi.git``
 
+
+Install the development dependencies:
+
+`pip install -requirements_dev.txt`
+
 Install:
 
 ``python setup.py install``
 
 After every modification of .pyx files compile with Cython:
 
 ``python setup.py build_ext --inplace``
@@ -179,14 +188,54 @@
 for c in cells:
     print("Cell contains point: {0}. Contains segment: {1}. Is open: {2}, Site Index: {3}".format(c.contains_point, c.contains_segment, c.is_open, c.site))
     print(",".join(map(str,c.vertices)))
     for sIndex in c.edges:
         print("Start Index: {0}, End Index = {1}".format(edges[sIndex].start, edges[sIndex].end))
 ```
 
+Note that since version 1.0.4 each of the Get function has an equivalent function that returns an iterator. This is more memory friendly.
+
+|Goal|Return a list|Return an iterator|
+| - | - | - |
+| Return vertices | GetVertices | IterateVertices |
+| Return edges | GetEdges | IterateEdges |
+| Return cells | GetCells | IterateCells |
+
+They are functionaly equivalent as defined in this automated test:
+
+```python
+    def test_iterators(self):
+        pv = pyvoronoi.Pyvoronoi(1)
+        pv.AddPoint([5,5])
+        pv.AddSegment([[0,0],[0,10]])
+        pv.AddSegment([[0,0],[10,0]])
+        pv.AddSegment([[0,10],[10,10]])
+        pv.AddSegment([[10,0],[10,10]])
+        pv.Construct()
+
+        vertices = pv.GetVertices()
+        vertex_generator = pv.IterateVertices()
+        for v in vertices:
+            v_generator = next(vertex_generator)
+            self.assertEqual(v, v_generator)
+
+        edges = pv.GetEdges()
+        edge_generator = pv.IterateEdges()
+        for e in edges:
+            e_generator = next(edge_generator)
+            self.assertEqual(e, e_generator)
+
+        cells = pv.GetCells()
+        cell_generator = pv.IterateCells()
+        for c in cells:
+            c_generator = next(cell_generator)
+            self.assertEqual(c, c_generator)
+```
+
+
 Some output edges returned by the boost voronoi API are suposed to be curved. In the C++ API, it is up to you to code it. Luckily, you can do it in python using the following the function DiscretizeCurvedEdge.
 The sample below shows you how to do that:
 
 ```python
 for cIndex in range(len(cells)):
     cell = cells[cIndex]
     if cell.is_open == False:
@@ -214,7 +263,9 @@
 # License
 
 -  Pyvoronoi is available under `MIT
    license <http://opensource.org/licenses/MIT>`__.
 -  The core Voronoi library is available under `Boost Software
    License <http://www.boost.org/LICENSE_1_0.txt>`__. Freeware for both
    open source and commercial applications.
+
+
```

### Comparing `pyvoronoi-1.0.9.4/pyvoronoi.egg-info/SOURCES.txt` & `pyvoronoi-1.1.0/pyvoronoi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvoronoi-1.0.9.4/setup.py` & `pyvoronoi-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-﻿from __future__ import print_function
-import sys
+﻿import sys
 import os
 from setuptools import setup
 from setuptools.extension import Extension
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
-version = '1.0.9.4'
+version = '1.1.0'
 
 """
 Note on using the setup.py:
 setup.py operates in 2 modes that are based on the presence of the 'dev' file in the root of the project.
  - When 'dev' is present, Cython will be used to compile the .pyx sources. This is the development mode
    (as you get it in the git repository).
  - When 'dev' is absent, C/C++ compiler will be used to compile the .cpp sources (that were prepared in
@@ -25,15 +24,15 @@
 if dev_mode:
     from Cython.Distutils import build_ext
 
     print('Development mode: Compiling Cython modules from .pyx sources.')
     sources = ["pyvoronoi/pyvoronoi.pyx", "pyvoronoi/voronoi.cpp"]
 
 else:
-    from distutils.command.build_ext import build_ext
+    from setuptools.command.build_ext import build_ext
 
     print('Distribution mode: Compiling from Cython generated .cpp sources.')
     sources = ["pyvoronoi/pyvoronoi.cpp", "pyvoronoi/voronoi.cpp"]
 
 
 ext = Extension("pyvoronoi",
                 sources=sources,
@@ -62,37 +61,27 @@
 
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
 
 # This command has been borrowed from
 # http://www.pydanny.com/python-dot-py-tricks.html
-if sys.argv[-1] == 'publish':
-    os.system("python setup.py sdist upload")
-    os.system("python setup.py bdist_wheel upload")
-    sys.exit()
 
 if sys.argv[-1] == 'tag':
-    os.system("git tag -a %s -m 'version %s'" % (version, version))
+    tag_command = "git tag -a v%s -m 'v%s'" % (version, version)
+    print(tag_command)
+    os.system(tag_command)
     os.system("git push --tags")
     sys.exit()
 
 class build_ext_subclass( build_ext ):
     def build_extensions(self):
         print(f'Compiler type: {self.compiler.compiler_type} - Version: {sys.version_info.major}.{sys.version_info.minor}')
-        if sys.version_info.major < 3:
-            c = self.compiler.compiler_type
-            if c == 'msvc':
-                for e in self.extensions:
-                    e.extra_compile_args = ["/EHsc"]
-                userdir = os.environ["USERPROFILE"]
-                os.environ["INCLUDE"] = userdir + "\\AppData\\Local\\Programs\\Common\\Microsoft\\Visual C++ for Python\\9.0\\VC\\include\\"
-
         # Starting from 3.11, the file longintrepr.h has moved. It is no longer under Python@3.XX\include but Python@3.XX\include\cpython        
-        elif sys.version_info.major == 3 and sys.version_info.minor >= 11:
+        if sys.version_info.major == 3 and sys.version_info.minor >= 11:
             c = self.compiler.compiler_type
             if c == 'msvc':
                 for e in self.extensions:
                     install_dir = os.path.dirname(sys.executable)
                     cpython_directory = os.path.join(install_dir, 'include', 'cpython')         
                     e.extra_compile_args = [cpython_directory]
         build_ext.build_extensions(self)
```

