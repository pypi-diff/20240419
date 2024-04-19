# Comparing `tmp/dynabench-0.2.4.tar.gz` & `tmp/dynabench-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynabench-0.2.4.tar", last modified: Wed Nov  8 13:02:15 2023, max compression
+gzip compressed data, was "dynabench-0.3.0.tar", max compression
```

## Comparing `dynabench-0.2.4.tar` & `dynabench-0.3.0.tar`

### file list

```diff
@@ -1,82 +1,22 @@
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.468835 dynabench-0.2.4/
--rw-r--r--   0 andi      (1000) andi      (1000)     1074 2023-06-27 16:04:10.000000 dynabench-0.2.4/LICENCE
--rw-r--r--   0 andi      (1000) andi      (1000)    18657 2023-06-27 16:04:10.000000 dynabench-0.2.4/LICENCE_data
--rw-r--r--   0 andi      (1000) andi      (1000)    12115 2023-11-08 13:02:15.465502 dynabench-0.2.4/PKG-INFO
--rw-r--r--   0 andi      (1000) andi      (1000)    11292 2023-06-27 16:04:20.000000 dynabench-0.2.4/README.md
--rw-r--r--   0 andi      (1000) andi      (1000)      968 2023-11-08 13:01:16.000000 dynabench-0.2.4/pyproject.toml
--rw-r--r--   0 andi      (1000) andi      (1000)       38 2023-11-08 13:02:15.468835 dynabench-0.2.4/setup.cfg
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.462169 dynabench-0.2.4/src/
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.462169 dynabench-0.2.4/src/dynabench/
--rw-r--r--   0 andi      (1000) andi      (1000)       38 2023-10-24 15:03:31.000000 dynabench-0.2.4/src/dynabench/_init_.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/dataset/
--rw-r--r--   0 andi      (1000) andi      (1000)       39 2023-10-18 15:13:14.000000 dynabench-0.2.4/src/dynabench/dataset/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)     4804 2023-10-31 08:57:53.000000 dynabench-0.2.4/src/dynabench/dataset/download.py
--rw-r--r--   0 andi      (1000) andi      (1000)     3130 2023-11-02 12:58:47.000000 dynabench-0.2.4/src/dynabench/dataset/iterator.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2474 2023-11-08 13:00:17.000000 dynabench-0.2.4/src/dynabench/dataset/simulation_iterator.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/generator/
--rw-r--r--   0 andi      (1000) andi      (1000)      502 2023-07-06 10:03:25.000000 dynabench-0.2.4/src/dynabench/generator/__init__.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/generator/fourier/
--rw-r--r--   0 andi      (1000) andi      (1000)     1712 2023-07-06 10:03:50.000000 dynabench-0.2.4/src/dynabench/generator/fourier/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)     7053 2023-07-06 09:54:44.000000 dynabench-0.2.4/src/dynabench/generator/fourier/equations.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2622 2023-07-06 14:06:58.000000 dynabench-0.2.4/src/dynabench/generator/fourier/solver.py
--rw-r--r--   0 andi      (1000) andi      (1000)     1789 2023-07-05 13:11:54.000000 dynabench-0.2.4/src/dynabench/generator/initial.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/generator/postprocessing/
--rw-r--r--   0 andi      (1000) andi      (1000)     2493 2023-07-06 10:17:21.000000 dynabench-0.2.4/src/dynabench/generator/postprocessing/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2203 2023-07-06 10:16:08.000000 dynabench-0.2.4/src/dynabench/generator/postprocessing/interpolate.py
--rw-r--r--   0 andi      (1000) andi      (1000)        0 2023-07-06 09:13:17.000000 dynabench-0.2.4/src/dynabench/generator/postprocessing/saving.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/generator/pypde/
--rw-r--r--   0 andi      (1000) andi      (1000)     8443 2023-07-05 13:20:41.000000 dynabench-0.2.4/src/dynabench/generator/pypde/equations.py
--rw-r--r--   0 andi      (1000) andi      (1000)     7232 2023-07-05 15:25:10.000000 dynabench-0.2.4/src/dynabench/generator/pypde/solver.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/
--rw-r--r--   0 andi      (1000) andi      (1000)       71 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/__init__.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/baseline/
--rw-r--r--   0 andi      (1000) andi      (1000)      338 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/baseline/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)      495 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/baseline/baseline_difference.py
--rw-r--r--   0 andi      (1000) andi      (1000)      452 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/baseline/baseline_persistence.py
--rw-r--r--   0 andi      (1000) andi      (1000)      476 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/baseline/baseline_zero.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/cloud/
--rw-r--r--   0 andi      (1000) andi      (1000)      139 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/cloud/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)     1559 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/cloud/feast.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2294 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/cloud/point_gnn.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2386 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/cloud/point_net.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2529 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/cloud/point_transformer.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/components/
--rw-r--r--   0 andi      (1000) andi      (1000)       61 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/components/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)     6951 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/components/convLSTM.py
--rw-r--r--   0 andi      (1000) andi      (1000)      836 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/components/mlp.py
--rw-r--r--   0 andi      (1000) andi      (1000)     3260 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/components/point_gnn_conv.py
--rw-r--r--   0 andi      (1000) andi      (1000)      570 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/components/resnet.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/gnn/
--rw-r--r--   0 andi      (1000) andi      (1000)       44 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/gnn/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)     1211 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/gnn/gat.py
--rw-r--r--   0 andi      (1000) andi      (1000)     1200 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/gnn/gcn.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2665 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/graphmodule.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/graphpde/
--rw-r--r--   0 andi      (1000) andi      (1000)       30 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/graphpde/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)      695 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/graphpde/dynamics_layer.py
--rw-r--r--   0 andi      (1000) andi      (1000)     1560 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/graphpde/graphpde.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/grid/
--rw-r--r--   0 andi      (1000) andi      (1000)       92 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/grid/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)      943 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/grid/cnn.py
--rw-r--r--   0 andi      (1000) andi      (1000)      643 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/grid/neuralpde.py
--rwxr-xr-x   0 andi      (1000) andi      (1000)     1225 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/grid/resnet.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2526 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/gridmodule.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/model/neural_operator/
--rw-r--r--   0 andi      (1000) andi      (1000)       31 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/neural_operator/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)      884 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/neural_operator/kernel_nn.py
--rw-r--r--   0 andi      (1000) andi      (1000)    11418 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/neural_operator/nn_conv.py
--rw-r--r--   0 andi      (1000) andi      (1000)    39817 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/model/neural_operator/utilities.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench/utils/
--rw-r--r--   0 andi      (1000) andi      (1000)       77 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/utils/__init__.py
--rw-r--r--   0 andi      (1000) andi      (1000)     2317 2023-09-11 10:24:12.000000 dynabench-0.2.4/src/dynabench/utils/animation.py
--rw-r--r--   0 andi      (1000) andi      (1000)      551 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/utils/archive.py
--rw-r--r--   0 andi      (1000) andi      (1000)     1746 2023-07-05 12:21:59.000000 dynabench-0.2.4/src/dynabench/utils/colors.py
--rw-r--r--   0 andi      (1000) andi      (1000)      488 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/utils/logging.py
--rw-r--r--   0 andi      (1000) andi      (1000)        0 2023-06-27 16:04:10.000000 dynabench-0.2.4/src/dynabench/utils/metrics.py
-drwxr-xr-x   0 andi      (1000) andi      (1000)        0 2023-11-08 13:02:15.465502 dynabench-0.2.4/src/dynabench.egg-info/
--rw-r--r--   0 andi      (1000) andi      (1000)    12115 2023-11-08 13:02:15.000000 dynabench-0.2.4/src/dynabench.egg-info/PKG-INFO
--rw-r--r--   0 andi      (1000) andi      (1000)     2307 2023-11-08 13:02:15.000000 dynabench-0.2.4/src/dynabench.egg-info/SOURCES.txt
--rw-r--r--   0 andi      (1000) andi      (1000)        1 2023-11-08 13:02:15.000000 dynabench-0.2.4/src/dynabench.egg-info/dependency_links.txt
--rw-r--r--   0 andi      (1000) andi      (1000)       64 2023-11-08 13:02:15.000000 dynabench-0.2.4/src/dynabench.egg-info/requires.txt
--rw-r--r--   0 andi      (1000) andi      (1000)       16 2023-11-08 13:02:15.000000 dynabench-0.2.4/src/dynabench.egg-info/top_level.txt
--rw-r--r--   0 andi      (1000) andi      (1000)      536 2023-10-18 12:43:56.000000 dynabench-0.2.4/src/setup.py
+-rw-r--r--   0        0        0     1074 2024-04-19 07:42:53.501591 dynabench-0.3.0/LICENCE
+-rw-r--r--   0        0        0    18657 2024-04-19 07:42:53.501591 dynabench-0.3.0/LICENCE_data
+-rw-r--r--   0        0        0    11415 2024-04-19 15:34:38.150726 dynabench-0.3.0/README.md
+-rw-r--r--   0        0        0      822 2024-04-19 15:31:13.754053 dynabench-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/_init_.py
+-rw-r--r--   0        0        0      266 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/__init__.py
+-rw-r--r--   0        0        0      504 2024-04-19 07:45:03.504922 dynabench-0.3.0/src/dynabench/dataset/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8924 2024-04-19 07:45:03.504922 dynabench-0.3.0/src/dynabench/dataset/__pycache__/_download.cpython-311.pyc
+-rw-r--r--   0        0        0     5826 2024-04-19 07:45:03.518256 dynabench-0.3.0/src/dynabench/dataset/__pycache__/_iterator.cpython-311.pyc
+-rw-r--r--   0        0        0     4744 2024-04-19 07:45:03.541589 dynabench-0.3.0/src/dynabench/dataset/__pycache__/_simulation_iterator.cpython-311.pyc
+-rw-r--r--   0        0        0     6087 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/_download.py
+-rw-r--r--   0        0        0     3119 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/_iterator.py
+-rw-r--r--   0        0        0     2466 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/_simulation_iterator.py
+-rw-r--r--   0        0        0      201 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/equation/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-19 14:58:43.960657 dynabench-0.3.0/src/dynabench/equation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2061 2024-04-19 07:45:03.501589 dynabench-0.3.0/src/dynabench/equation/__pycache__/_advection.cpython-311.pyc
+-rw-r--r--   0        0        0     2662 2024-04-19 07:45:03.344923 dynabench-0.3.0/src/dynabench/equation/__pycache__/_base.cpython-311.pyc
+-rw-r--r--   0        0        0     1224 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/equation/_advection.py
+-rw-r--r--   0        0        0     1456 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/equation/_base.py
+-rw-r--r--   0        0        0       69 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/model/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-19 14:58:43.960657 dynabench-0.3.0/src/dynabench/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12038 1970-01-01 00:00:00.000000 dynabench-0.3.0/PKG-INFO
```

### Comparing `dynabench-0.2.4/LICENCE` & `dynabench-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `dynabench-0.2.4/LICENCE_data` & `dynabench-0.3.0/LICENCE_data`

 * *Files identical despite different names*

### Comparing `dynabench-0.2.4/PKG-INFO` & `dynabench-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: dynabench
-Version: 0.2.4
+Version: 0.3.0
 Summary: Benchmark dataset for learning dynamical systems from data
-Author-email: Andrzej Dulny <andrzej.dulny@protonmail.com>
-Project-URL: homepage, https://dynabench.github.io/
-Project-URL: documentation, https://dynabench.github.io/docs/
-Project-URL: source, https://github.com/badulion/dynabench
-Keywords: benchmark,torch,deep learning
+License: MIT
+Author: Andrzej Dulny
+Author-email: andzej.dulny@gmail.com
+Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: h5py (>=3.11.0,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENCE
-License-File: LICENCE_data
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: numpy>=1.23.5
-Requires-Dist: h5py>=3.9.0
-Provides-Extra: generator
-Requires-Dist: dedalus>=3; extra == "generator"
 
 # Dynabench: A benchmark dataset for learning dynamical systems from low-resolution data
 
 This is the repository containing the data generation algorithms as well as all baseline models for the __Dynabench: A benchmark dataset for learning dynamical systems from low-resolution data__ paper (accepted at ECML-PKDD 2023)
 
+**!!!You can find the documentation on how to use this package here: [dynabench.github.io](https://dynabench.github.io)**
+
 DynaBench is a benchmark dataset for learning dynamical systems from data. Dynamical systems are physical systems that are typically modelled by partial differential equations (e.g. numerical weather prediction, climate models, fluid simulation, electromagnetic field simulation etc.). The main challenge of learning to predict the evolution of these systems from data is the chaotic behaviour that these systems show (small deviation from the initial conditions leads to highly different predictions) as well as data availability. In real world settings only low-resolution data is available, with measurements sparsly scattered in the simulation domain (see following figure illustrating the distribution of weather monitoring stations in europe).
 
 
 ![Weather stations europe gif](demos/weather_stations.gif)
 
 In this benchmark we try to simulate this setting using synthetic data for easier evaluation and training of different machine learning models. To this end we generated simulation data by solving five different PDE systems which were then postprocessed to create low-resolution snapshots of the simulation.
```

### Comparing `dynabench-0.2.4/README.md` & `dynabench-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Dynabench: A benchmark dataset for learning dynamical systems from low-resolution data
 
 This is the repository containing the data generation algorithms as well as all baseline models for the __Dynabench: A benchmark dataset for learning dynamical systems from low-resolution data__ paper (accepted at ECML-PKDD 2023)
 
+**!!!You can find the documentation on how to use this package here: [dynabench.github.io](https://dynabench.github.io)**
+
 DynaBench is a benchmark dataset for learning dynamical systems from data. Dynamical systems are physical systems that are typically modelled by partial differential equations (e.g. numerical weather prediction, climate models, fluid simulation, electromagnetic field simulation etc.). The main challenge of learning to predict the evolution of these systems from data is the chaotic behaviour that these systems show (small deviation from the initial conditions leads to highly different predictions) as well as data availability. In real world settings only low-resolution data is available, with measurements sparsly scattered in the simulation domain (see following figure illustrating the distribution of weather monitoring stations in europe).
 
 
 ![Weather stations europe gif](demos/weather_stations.gif)
 
 In this benchmark we try to simulate this setting using synthetic data for easier evaluation and training of different machine learning models. To this end we generated simulation data by solving five different PDE systems which were then postprocessed to create low-resolution snapshots of the simulation.
```

### Comparing `dynabench-0.2.4/src/dynabench/dataset/download.py` & `dynabench-0.3.0/src/dynabench/dataset/_download.py`

 * *Files 25% similar despite different names*

```diff
@@ -52,37 +52,69 @@
 }
 
 BASE_URL = "https://wuedata.uni-wuerzburg.de/radar/api/datasets/%s/download"
 
 
 
 
-def download_raw(equation: str, structure: str, resolution: str, out_dir: str = "data/tmp/"):
+def download_raw(equation: str, structure: str, resolution: str, tmp_dir: str = "data/tmp/"):
+    """
+        Download the raw tar-file from the WUEData API.
+
+        Parameters
+        ----------
+        equation : str
+            Name of the equation to download.
+        structure : str
+            Description of how the observation points are structured. Can be "cloud" or "grid".
+        resolution : str
+            Resolution of the dataset. Can be "low", "medium", or "high".
+        tmp_dir : str
+            Directory where the temporary files should be saved. Defaults to "data/tmp/".
+        return : None
+    """
+
 
     # make an HTTP request within a context manager
     url = BASE_URL % DATASETS_WUEDATA[f"{equation}-{structure}-{resolution}"]
     with requests.get(url, stream=True) as r:
         
         # check header to get content length, in bytes
         total_length = int(r.headers.get("Content-Length"))
         
         # implement progress bar via tqdm
         with tqdm.wrapattr(r.raw, "read", total=total_length, desc="") as raw:
         
             # save the output to a file
-            out_path = os.path.join(out_dir, f"{equation}-{structure}-{resolution}.tar")
+            out_path = os.path.join(tmp_dir, f"{equation}-{structure}-{resolution}.tar")
             with open(out_path, 'wb') as output:
                 shutil.copyfileobj(raw, output)
             
 
             #shutil.rmtree("data/tmp")
 
-import hashlib
+def download_equation(equation: str, structure: str, resolution: str, out_dir: str = "data", tmp_dir: str = "data/tmp/"):
+    """
+        Download a dataset and unpack it to the right place.
+
+        Parameters
+        ----------
+        equation : str  
+            Name of the equation to download.
+        structure : str
+            Description of how the observation points are structured. Can be "cloud" or "grid".
+        resolution : str
+            Resolution of the dataset. Can be "low", "medium", or "high".
+        out_dir : str
+            Directory where the dataset should be saved. Defaults to "data/".
+        tmp_dir : str
+            Directory where the temporary files should be saved. Defaults to "data/tmp/". This directory will be deleted after the dataset is unpacked.
+        return : None
+    """
 
-def download_equation(equation: str, structure: str, resolution: str, out_dir: str = "data", tmp_dir: str = "tmp/"):
 
     # paths
     tmp_dir = os.path.join(out_dir, tmp_dir)
 
     os.makedirs(tmp_dir, exist_ok=True)
 
     # download the tar file
@@ -113,15 +145,15 @@
     print("Moving data...")
     target_path = os.path.join(out_dir, equation, structure, resolution)
     os.makedirs(target_path, exist_ok=True)
     for file in glob.glob(file_template):
         try:
             shutil.move(file, target_path)
         except shutil.Error:
-            continue
+            print(f"File {file} cannot be moved to {target_path}. Skipping.")
 
     # clean up
     print("Cleaning up...")
     shutil.rmtree(tmp_dir)
 
 if __name__ == "__main__":
     download_equation("wave", "cloud", "low")
```

### Comparing `dynabench-0.2.4/src/dynabench/dataset/iterator.py` & `dynabench-0.3.0/src/dynabench/dataset/_iterator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import glob
 from typing import Any
 import h5py
 import numpy as np
 
-from .download import download_equation
+from ._download import download_equation
 
 class DynabenchIterator:
 
     def __init__(
         self,
         split: str="train",
         equation: str="wave",
@@ -17,15 +17,15 @@
         base_path: str="data",
         lookback: int=1,
         rollout: int=1,
         download: bool=False,
         *args,
         **kwargs,
     ) -> None:
-        
+
         # download
         if download:
             download_equation(equation, structure, resolution, base_path)
         
         # parameters
         self.split = split
         self.equation = equation
@@ -51,15 +51,15 @@
         self.usable_simulation_lengths = [(shape[1] - self.lookback - self.rollout+1) for shape in self.shapes]
         self.number_of_simulations = [shape[0] for shape in self.shapes]
         self.datapoints_per_file = [length * number for length, number in zip(self.usable_simulation_lengths, self.number_of_simulations)]
         self.starting_indices = np.cumsum(self.datapoints_per_file) - self.datapoints_per_file[0]
 
     def _check_exists(self):
         return len(self.file_list) > 0
-    
+
     def __getitem__(self, index):
         if index < 0:
             index += len(self)
         if index > len(self) or index < 0:
             raise IndexError("Index out of bounds")
```

### Comparing `dynabench-0.2.4/src/dynabench/dataset/simulation_iterator.py` & `dynabench-0.3.0/src/dynabench/dataset/_simulation_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import glob
 from typing import Any
 import h5py
 import numpy as np
 
-from .download import download_equation
+from . import download_equation
 
 class DynabenchSimulationIterator:
 
     def __init__(
         self,
         split: str="train",
         equation: str="wave",
```

