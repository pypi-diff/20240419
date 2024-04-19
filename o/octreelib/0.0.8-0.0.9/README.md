# Comparing `tmp/octreelib-0.0.8.tar.gz` & `tmp/octreelib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octreelib-0.0.8.tar", max compression
+gzip compressed data, was "octreelib-0.0.9.tar", max compression
```

## Comparing `octreelib-0.0.8.tar` & `octreelib-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-04-12 17:16:19.889083 octreelib-0.0.8/LICENSE
--rw-r--r--   0        0        0     1054 2024-04-12 17:16:19.889083 octreelib-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/__init__.py
--rw-r--r--   0        0        0      310 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/grid/__init__.py
--rw-r--r--   0        0        0    14432 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/grid/grid.py
--rw-r--r--   0        0        0     7307 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/grid/grid_base.py
--rw-r--r--   0        0        0      578 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/__init__.py
--rw-r--r--   0        0        0      740 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/interfaces.py
--rw-r--r--   0        0        0      462 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/point.py
--rw-r--r--   0        0        0       62 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/typing.py
--rw-r--r--   0        0        0     2411 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/voxel.py
--rw-r--r--   0        0        0      328 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree/__init__.py
--rw-r--r--   0        0        0    10556 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree/octree.py
--rw-r--r--   0        0        0     6827 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree/octree_base.py
--rw-r--r--   0        0        0      168 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree_manager/__init__.py
--rw-r--r--   0        0        0     6483 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree_manager/octree_manager.py
--rw-r--r--   0        0        0      207 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/ransac/__init__.py
--rw-r--r--   0        0        0     5658 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/ransac/cuda_ransac.py
--rw-r--r--   0        0        0     2376 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/ransac/util.py
--rw-r--r--   0        0        0      784 2024-04-12 17:16:50.297183 octreelib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 octreelib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 15:37:58.924652 octreelib-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1054 2024-04-19 15:37:58.924652 octreelib-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/grid/__init__.py
+-rw-r--r--   0        0        0    14432 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/grid/grid.py
+-rw-r--r--   0        0        0     7307 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/grid/grid_base.py
+-rw-r--r--   0        0        0      578 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/internal/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/internal/interfaces.py
+-rw-r--r--   0        0        0      462 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/internal/point.py
+-rw-r--r--   0        0        0       62 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/internal/typing.py
+-rw-r--r--   0        0        0     2411 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/internal/voxel.py
+-rw-r--r--   0        0        0      328 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/octree/__init__.py
+-rw-r--r--   0        0        0    10556 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/octree/octree.py
+-rw-r--r--   0        0        0     6827 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/octree/octree_base.py
+-rw-r--r--   0        0        0      168 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/octree_manager/__init__.py
+-rw-r--r--   0        0        0     6483 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/octree_manager/octree_manager.py
+-rw-r--r--   0        0        0      207 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/ransac/__init__.py
+-rw-r--r--   0        0        0     5661 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/ransac/cuda_ransac.py
+-rw-r--r--   0        0        0     2287 2024-04-19 15:37:58.924652 octreelib-0.0.9/octreelib/ransac/util.py
+-rw-r--r--   0        0        0      802 2024-04-19 15:38:23.640641 octreelib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 octreelib-0.0.9/PKG-INFO
```

### Comparing `octreelib-0.0.8/LICENSE` & `octreelib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/README.md` & `octreelib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/grid/grid.py` & `octreelib-0.0.9/octreelib/grid/grid.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/grid/grid_base.py` & `octreelib-0.0.9/octreelib/grid/grid_base.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/internal/__init__.py` & `octreelib-0.0.9/octreelib/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/internal/interfaces.py` & `octreelib-0.0.9/octreelib/internal/interfaces.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/internal/voxel.py` & `octreelib-0.0.9/octreelib/internal/voxel.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/octree/octree.py` & `octreelib-0.0.9/octreelib/octree/octree.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/octree/octree_base.py` & `octreelib-0.0.9/octreelib/octree/octree_base.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/octree_manager/octree_manager.py` & `octreelib-0.0.9/octreelib/octree_manager/octree_manager.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.8/octreelib/ransac/cuda_ransac.py` & `octreelib-0.0.9/octreelib/ransac/cuda_ransac.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,13 +145,13 @@
                     best_plane[i] = plane[i]
             cuda.syncthreads()
 
             # parallelize final mask computation among threads in the block
             for i in range(
                 block_start_indices[block_id] + thread_id,
                 block_start_indices[block_id] + block_sizes[block_id],
-                CUDA_THREADS,
+                cuda.blockDim.x,
             ):
                 if measure_distance(best_plane, point_cloud[i]) < threshold:
                     result_mask[i] = True
 
         return kernel
```

### Comparing `octreelib-0.0.8/octreelib/ransac/util.py` & `octreelib-0.0.9/octreelib/ransac/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,16 @@
 )
 def measure_distance(plane, point):
     """
     Measure the distance between a plane and a point.
     :param plane: Plane coefficients.
     :param point: Point coordinates.
     """
-    return (
-        math.fabs(
-            plane[0] * point[0] + plane[1] * point[1] + plane[2] * point[2] + plane[3]
-        )
-        / (plane[0] ** 2 + plane[1] ** 2 + plane[2] ** 2) ** 0.5
+    return math.fabs(
+        plane[0] * point[0] + plane[1] * point[1] + plane[2] * point[2] + plane[3]
     )
 
 
 @cuda.jit(device=True, inline=True)
 def get_plane_from_points(points, initial_point_indices):
     """
     Calculate the plane coefficients from the given points.
```

### Comparing `octreelib-0.0.8/pyproject.toml` & `octreelib-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octreelib"
-version = "0.0.8"
+version = "0.0.9"
 description = "Library for representing point clouds as OcTrees in SLAM"
 authors = [
   "Kiselyov Mikhail <kiselev.0353@gmail.com>",
   "Pavel Mokeev <pav3l.mokeev@gmail.com>"
 ]
 license = "APACHE"
 readme = "README.md"
@@ -17,14 +17,15 @@
 ]
 exclude = ["test"]
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 numpy = "^1.26.0"
 k3d = "^2.16.0"
+numba = "^0.59.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `octreelib-0.0.8/PKG-INFO` & `octreelib-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octreelib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for representing point clouds as OcTrees in SLAM
 Home-page: https://github.com/prime-slam/
 License: APACHE
 Author: Kiselyov Mikhail
 Author-email: kiselev.0353@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: k3d (>=2.16.0,<3.0.0)
+Requires-Dist: numba (>=0.59.0,<0.60.0)
 Requires-Dist: numpy (>=1.26.0,<2.0.0)
 Project-URL: Repository, https://github.com/prime-slam/octreelib
 Description-Content-Type: text/markdown
 
 # Octreelib
 
 [![tests](https://github.com/prime-slam/octreelib/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/prime-slam/octreelib/actions/workflows/python-package.yml)
```

