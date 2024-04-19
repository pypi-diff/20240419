# Comparing `tmp/knot_tube-0.1.tar.gz` & `tmp/knot_tube-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knot_tube-0.1.tar", last modified: Tue Apr 16 11:49:08 2024, max compression
+gzip compressed data, was "knot_tube-0.2.tar", last modified: Fri Apr 19 12:55:39 2024, max compression
```

## Comparing `knot_tube-0.1.tar` & `knot_tube-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-16 11:49:08.485358 knot_tube-0.1/
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      141 2024-04-16 11:49:08.485358 knot_tube-0.1/PKG-INFO
-drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-16 11:49:08.485358 knot_tube-0.1/knot_tube/
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2023-04-14 13:52:36.000000 knot_tube-0.1/knot_tube/__init__.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     7521 2023-09-18 06:57:25.000000 knot_tube-0.1/knot_tube/knot.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     1593 2024-01-16 14:30:38.000000 knot_tube-0.1/knot_tube/lammps.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2024-01-28 13:31:15.000000 knot_tube-0.1/knot_tube/pdb.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     1191 2024-04-16 11:49:03.000000 knot_tube-0.1/knot_tube/polymer.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     5809 2024-03-11 05:22:15.000000 knot_tube-0.1/knot_tube/xyz.py
-drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-16 11:49:08.485358 knot_tube-0.1/knot_tube.egg-info/
--rw-r--r--   0 yongjian  (1002) yongjian  (1002)      141 2024-04-16 11:49:08.000000 knot_tube-0.1/knot_tube.egg-info/PKG-INFO
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      287 2024-04-16 11:49:08.000000 knot_tube-0.1/knot_tube.egg-info/SOURCES.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        1 2024-04-16 11:49:08.000000 knot_tube-0.1/knot_tube.egg-info/dependency_links.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       12 2024-04-16 11:49:08.000000 knot_tube-0.1/knot_tube.egg-info/requires.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       10 2024-04-16 11:49:08.000000 knot_tube-0.1/knot_tube.egg-info/top_level.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       38 2024-04-16 11:49:08.485358 knot_tube-0.1/setup.cfg
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      336 2024-04-16 11:46:54.000000 knot_tube-0.1/setup.py
+drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-19 12:55:39.464678 knot_tube-0.2/
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      141 2024-04-19 12:55:39.464678 knot_tube-0.2/PKG-INFO
+drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-19 12:55:39.464678 knot_tube-0.2/knot_tube/
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2023-04-14 13:52:36.000000 knot_tube-0.2/knot_tube/__init__.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     7521 2023-09-18 06:57:25.000000 knot_tube-0.2/knot_tube/knot.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     1593 2024-01-16 14:30:38.000000 knot_tube-0.2/knot_tube/lammps.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2024-01-28 13:31:15.000000 knot_tube-0.2/knot_tube/pdb.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     1751 2024-04-16 12:03:58.000000 knot_tube-0.2/knot_tube/polymer.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     5809 2024-03-11 05:22:15.000000 knot_tube-0.2/knot_tube/xyz.py
+drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-19 12:55:39.464678 knot_tube-0.2/knot_tube.egg-info/
+-rw-r--r--   0 yongjian  (1002) yongjian  (1002)      141 2024-04-19 12:55:39.000000 knot_tube-0.2/knot_tube.egg-info/PKG-INFO
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      287 2024-04-19 12:55:39.000000 knot_tube-0.2/knot_tube.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        1 2024-04-19 12:55:39.000000 knot_tube-0.2/knot_tube.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       22 2024-04-19 12:55:39.000000 knot_tube-0.2/knot_tube.egg-info/requires.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       10 2024-04-19 12:55:39.000000 knot_tube-0.2/knot_tube.egg-info/top_level.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       38 2024-04-19 12:55:39.464678 knot_tube-0.2/setup.cfg
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      335 2024-04-19 12:55:33.000000 knot_tube-0.2/setup.py
```

### Comparing `knot_tube-0.1/knot_tube/knot.py` & `knot_tube-0.2/knot_tube/knot.py`

 * *Files identical despite different names*

### Comparing `knot_tube-0.1/knot_tube/lammps.py` & `knot_tube-0.2/knot_tube/lammps.py`

 * *Files identical despite different names*

### Comparing `knot_tube-0.1/knot_tube/polymer.py` & `knot_tube-0.2/knot_tube/polymer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import numpy as np
 
-def bond_length(xyz:np.ndarray):
-    """计算轨迹的键长分布,输入应该为N_frames, N_atoms, 3的numpy array."""
-    print("original shape:", xyz.shape)
+def bond_length(xyz:np.ndarray,type = "open"):
+    """计算轨迹的键长分布,输入应该为N_frames, N_atoms, 3的numpy array. type="open"表示开链，type="ring"表示闭链."""
+    #print("original shape:", xyz.shape)
     temp = xyz.transpose(1,2,0)
-    print("temp shape:", temp.shape)
-
-    bond_length = np.linalg.norm(temp[1:] - temp[:-1], axis=2)
+    #print("temp shape:", temp.shape)
+    if(type == "ring"):
+        bond_length = np.linalg.norm(temp[1:] - temp[:-1], axis=1)
+        # 闭链需要计算首尾原子的键长
+        end_to_start_bond = np.linalg.norm(temp[-1] - temp[0], axis=0)
+        #print("end_to_start_bond shape:", end_to_start_bond.shape)
+        # 从(N_frames) 变为 (1, N_frames)
+        end_to_start_bond = end_to_start_bond.reshape(1,-1)
+        bond_length = np.concatenate((bond_length, end_to_start_bond), axis=0)
+    elif(type == "open"):
+        bond_length = np.linalg.norm(temp[1:] - temp[:-1], axis=1)
     print("bond_length shape:", bond_length.shape)
     bond_length = bond_length.flatten()
     return bond_length
 
 def radius_of_gyration(trajectory:np.ndarray):
     """计算轨迹的质心半径分布,输入应该为N_frames, N_atoms, 3的numpy array."""
     # 计算每帧的质心
```

### Comparing `knot_tube-0.1/knot_tube/xyz.py` & `knot_tube-0.2/knot_tube/xyz.py`

 * *Files identical despite different names*

