# Comparing `tmp/bucketed_scene_flow_eval-2.0.4.tar.gz` & `tmp/bucketed_scene_flow_eval-2.0.5.tar.gz`

## Comparing `bucketed_scene_flow_eval-2.0.4.tar` & `bucketed_scene_flow_eval-2.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/build_pypi.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py
--rw-r--r--   0        0        0    22729 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py
--rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/waymoopen/__init__.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py
--rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/__init__.py
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/camera_projection.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/dataclasses.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/pointcloud.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/rgb_image.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/se2.py
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/se3.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/__init__.py
--rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py
--rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/bucketed_epe.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/eval.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/threeway_epe.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/abstract_dataset.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/utils/__init__.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/utils/loaders.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/integration_tests.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/integration_tests.sh
--rwxr-xr-x   0        0        0     4217 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/setup.sh
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/datasets/argoverse2/av2_small_tests.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/datasets/argoverse2/av2_tiny_tests.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/datasets/nuscenes/nuscenes_tests.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/datastructures/rgb.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/eval/bucketed_epe.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/tests/eval/threeway_epe.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/LICENSE
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/README.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/build_pypi.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py
+-rw-r--r--   0        0        0    22729 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py
+-rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/waymoopen/__init__.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/__init__.py
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/camera_projection.py
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/dataclasses.py
+-rw-r--r--   0        0        0     7504 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/pointcloud.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/rgb_image.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/se2.py
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/se3.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/__init__.py
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py
+-rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/bucketed_epe.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/eval.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/threeway_epe.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/abstract_dataset.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/utils/__init__.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/utils/loaders.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/integration_tests.py
+-rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/integration_tests.sh
+-rwxr-xr-x   0        0        0     4217 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/setup.sh
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/datasets/argoverse2/av2_small_tests.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/datasets/argoverse2/av2_tiny_tests.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/datasets/nuscenes/nuscenes_tests.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/datastructures/rgb.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/eval/bucketed_epe.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/tests/eval/threeway_epe.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.5/PKG-INFO
```

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/__init__.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/__init__.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/camera_projection.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/camera_projection.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/dataclasses.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/dataclasses.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,16 +179,19 @@
             np.array([[i, i + 1] for i in range(len(trajectory) - 1)])
         )
         line_set.colors = o3d.utility.Vector3dVector(
             np.tile(np.array(color), (len(trajectory) - 1, 1))
         )
         self.add_geometry(line_set)
 
+    def render(self, vis, reset_view: bool = True):
+        for geometry in self.geometry_list:
+            vis.add_geometry(geometry, reset_bounding_box=reset_view)
+
     def run(self, vis=o3d.visualization.Visualizer()):
         print("Running visualizer on geometry list of length", len(self.geometry_list))
         vis.create_window(window_name="Benchmark Visualizer")
         vis.get_render_option().point_size = self.point_size
 
-        for geometry in self.geometry_list:
-            vis.add_geometry(geometry)
+        self.render()
 
         vis.run()
```

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/pointcloud.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/pointcloud.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/rgb_image.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/rgb_image.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/se2.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/se2.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/datastructures/se3.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/datastructures/se3.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/bucketed_epe.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/bucketed_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/eval/threeway_epe.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/eval/threeway_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/__init__.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/abstract_dataset.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/abstract_dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/utils/__init__.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/bucketed_scene_flow_eval/utils/loaders.py` & `bucketed_scene_flow_eval-2.0.5/bucketed_scene_flow_eval/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/integration_tests.py` & `bucketed_scene_flow_eval-2.0.5/tests/integration_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/setup.sh` & `bucketed_scene_flow_eval-2.0.5/tests/setup.sh`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/datasets/argoverse2/av2_small_tests.py` & `bucketed_scene_flow_eval-2.0.5/tests/datasets/argoverse2/av2_small_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/datasets/argoverse2/av2_tiny_tests.py` & `bucketed_scene_flow_eval-2.0.5/tests/datasets/argoverse2/av2_tiny_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/datasets/nuscenes/nuscenes_tests.py` & `bucketed_scene_flow_eval-2.0.5/tests/datasets/nuscenes/nuscenes_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/datastructures/rgb.py` & `bucketed_scene_flow_eval-2.0.5/tests/datastructures/rgb.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/eval/bucketed_epe.py` & `bucketed_scene_flow_eval-2.0.5/tests/eval/bucketed_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/tests/eval/threeway_epe.py` & `bucketed_scene_flow_eval-2.0.5/tests/eval/threeway_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/LICENSE` & `bucketed_scene_flow_eval-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/README.md` & `bucketed_scene_flow_eval-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.4/pyproject.toml` & `bucketed_scene_flow_eval-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "/data_prep_scripts",
   "/launch.sh",
   "/README.md",
 ]
 
 [project]
 name = "bucketed_scene_flow_eval"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
   { name="Kyle Vedder", email="kvedder@seas.upenn.edu" },
 ]
 description = "Bucketed Scene Flow Evaluation"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `bucketed_scene_flow_eval-2.0.4/PKG-INFO` & `bucketed_scene_flow_eval-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bucketed_scene_flow_eval
-Version: 2.0.4
+Version: 2.0.5
 Summary: Bucketed Scene Flow Evaluation
 Author-email: Kyle Vedder <kvedder@seas.upenn.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

