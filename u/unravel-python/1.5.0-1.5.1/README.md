# Comparing `tmp/unravel_python-1.5.0.tar.gz` & `tmp/unravel_python-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel_python-1.5.0.tar", last modified: Mon Apr 15 15:22:42 2024, max compression
+gzip compressed data, was "unravel_python-1.5.1.tar", last modified: Fri Apr 19 09:40:29 2024, max compression
```

## Comparing `unravel_python-1.5.0.tar` & `unravel_python-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.380000 unravel_python-1.5.0/
--rw-rw-rw-   0        0        0    35823 2024-02-01 10:17:26.000000 unravel_python-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     4515 2024-04-15 15:22:44.000000 unravel_python-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3801 2024-02-01 10:17:26.000000 unravel_python-1.5.0/README.md
--rw-rw-rw-   0        0        0      970 2024-02-01 10:17:26.000000 unravel_python-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 15:22:44.000000 unravel_python-1.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.380000 unravel_python-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.390000 unravel_python-1.5.0/src/unravel/
--rw-rw-rw-   0        0        0      358 2024-04-15 15:22:00.000000 unravel_python-1.5.0/src/unravel/__init__.py
--rw-rw-rw-   0        0        0     3038 2024-02-21 12:39:26.000000 unravel_python-1.5.0/src/unravel/analysis.py
--rw-rw-rw-   0        0        0    44450 2024-02-01 10:17:26.000000 unravel_python-1.5.0/src/unravel/core.py
--rw-rw-rw-   0        0        0     4547 2024-02-21 12:33:42.000000 unravel_python-1.5.0/src/unravel/example.py
--rw-rw-rw-   0        0        0    20774 2024-03-11 14:32:18.000000 unravel_python-1.5.0/src/unravel/stream.py
--rw-rw-rw-   0        0        0    15988 2024-04-15 14:45:40.000000 unravel_python-1.5.0/src/unravel/utils.py
--rw-rw-rw-   0        0        0    20577 2024-04-15 15:01:06.000000 unravel_python-1.5.0/src/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.390000 unravel_python-1.5.0/src/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     4515 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.740000 unravel_python-1.5.1/
+-rw-rw-rw-   0        0        0    35823 2024-02-01 10:17:26.000000 unravel_python-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     4515 2024-04-19 09:40:30.000000 unravel_python-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3801 2024-02-01 10:17:26.000000 unravel_python-1.5.1/README.md
+-rw-rw-rw-   0        0        0      970 2024-02-01 10:17:26.000000 unravel_python-1.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:40:30.000000 unravel_python-1.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.750000 unravel_python-1.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.750000 unravel_python-1.5.1/src/unravel/
+-rw-rw-rw-   0        0        0      358 2024-04-19 09:39:30.000000 unravel_python-1.5.1/src/unravel/__init__.py
+-rw-rw-rw-   0        0        0     3038 2024-02-21 12:39:26.000000 unravel_python-1.5.1/src/unravel/analysis.py
+-rw-rw-rw-   0        0        0    44450 2024-02-01 10:17:26.000000 unravel_python-1.5.1/src/unravel/core.py
+-rw-rw-rw-   0        0        0     4547 2024-02-21 12:33:42.000000 unravel_python-1.5.1/src/unravel/example.py
+-rw-rw-rw-   0        0        0    20810 2024-04-19 09:36:20.000000 unravel_python-1.5.1/src/unravel/stream.py
+-rw-rw-rw-   0        0        0    15988 2024-04-15 14:45:40.000000 unravel_python-1.5.1/src/unravel/utils.py
+-rw-rw-rw-   0        0        0    20577 2024-04-15 15:01:06.000000 unravel_python-1.5.1/src/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.760000 unravel_python-1.5.1/src/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     4515 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel_python-1.5.0/LICENSE` & `unravel_python-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/PKG-INFO` & `unravel_python-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: Implementation of UNRAVEL
 Author-email: Nicolas Delinte <nicolas.delinte@uclouvain.be>
 License: GNU General Public License v3.0
 Project-URL: GitHub, https://github.com/DelinteNicolas/UNRAVEL
 Project-URL: Documentation, https://unravel.readthedocs.io/en/latest/
 Keywords: tractography,multi-fixel
 Classifier: Intended Audience :: Science/Research
```

### Comparing `unravel_python-1.5.0/README.md` & `unravel_python-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/pyproject.toml` & `unravel_python-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/src/unravel/analysis.py` & `unravel_python-1.5.1/src/unravel/analysis.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/src/unravel/core.py` & `unravel_python-1.5.1/src/unravel/core.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/src/unravel/example.py` & `unravel_python-1.5.1/src/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/src/unravel/stream.py` & `unravel_python-1.5.1/src/unravel/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             n = get_streamline_number_from_index(streams, idx[j])
             dist[i, n] = i_dist
 
     return dist, median_array
 
 
 def remove_outlier_streamlines(trk_file, point_array, out_file: str = None,
-                               outlier_ratio: float = .5,
+                               outlier_ratio: float = 0,
                                remove_outlier_dir: bool = False,
                                verbose: bool = True, bandwidth: float = 0.2,
                                neighbors_required: int = 5,
                                bandwidth_dir: float = 1,
                                neighbors_required_dir: int = 10,
                                keep_ratio: float = 0.5):
     '''
@@ -295,15 +295,15 @@
         Path to tractogram file.
     point_array : 2D array of size (n, 3)
         Coordinates (x,y,z) of the n mean trajectory points.
     out_file : str, optional
         Path to output file. The default is None.
     outlier_ratio : int, optional
         Percentage of the streamline allowed to be an outlier [0:1]. Increasing
-        the value removes less streamlines. The default is 0.5 (50%).
+        the value removes less streamlines. The default is 0 (0%).
     remove_outlier_dir : bool, optional
         If True, removes streamlines whose direction are outliers.
         The default is False.
     verbose : bool, optional
         If True, prints number of streamlines removed. The default is False.
     bandwidth : float, optional.
         Bandwidth for the KDE, recommended values : [0.1-5]. The default is 0.2.
@@ -397,14 +397,15 @@
     n_idx = np.argwhere(n_sign > n_val*outlier_ratio)
 
     if len(n_idx) > keep_ratio*len(n_sign):
 
         sorted_indexes = np.argsort(-n_sign)
         keep_num_idx = int(len(n_sign)*keep_ratio)
         n_idx = sorted_indexes[:keep_num_idx]
+        n_idx = n_idx[..., np.newaxis]
 
     if remove_outlier_dir:
 
         streams_data = trk.streamlines.get_data()
 
         # Clustering end nodes based on streamline directions
         end_0 = streams_data[streams._offsets, :]
```

### Comparing `unravel_python-1.5.0/src/unravel/utils.py` & `unravel_python-1.5.1/src/unravel/utils.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/src/unravel/viz.py` & `unravel_python-1.5.1/src/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.0/src/unravel_python.egg-info/PKG-INFO` & `unravel_python-1.5.1/src/unravel_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: Implementation of UNRAVEL
 Author-email: Nicolas Delinte <nicolas.delinte@uclouvain.be>
 License: GNU General Public License v3.0
 Project-URL: GitHub, https://github.com/DelinteNicolas/UNRAVEL
 Project-URL: Documentation, https://unravel.readthedocs.io/en/latest/
 Keywords: tractography,multi-fixel
 Classifier: Intended Audience :: Science/Research
```

