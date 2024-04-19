# Comparing `tmp/pyepo-0.3.6.tar.gz` & `tmp/pyepo-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepo-0.3.6.tar", last modified: Wed Feb 14 04:00:03 2024, max compression
+gzip compressed data, was "pyepo-0.3.7.tar", last modified: Fri Apr 19 05:03:49 2024, max compression
```

## Comparing `pyepo-0.3.6.tar` & `pyepo-0.3.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.753250 pyepo-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-14 04:00:03.753250 pyepo-0.3.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.745250 pyepo-0.3.6/pyepo/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/EPO.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.749250 pyepo-0.3.6/pyepo/data/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/data/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/data/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/data/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.749250 pyepo-0.3.6/pyepo/func/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/abcmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)    18525 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/perturbed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/spoplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/func/utlis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.749250 pyepo-0.3.6/pyepo/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/metric/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/metric/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/metric/regret.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/metric/unambregret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.749250 pyepo-0.3.6/pyepo/model/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.753250 pyepo-0.3.6/pyepo/model/copt/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/copt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/copt/coptmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/copt/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/copt/shortestpath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.753250 pyepo-0.3.6/pyepo/model/grb/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/grb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/grb/grbmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/grb/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/grb/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/grb/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.753250 pyepo-0.3.6/pyepo/model/omo/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/omo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/omo/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/omo/omomodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/omo/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/model/opt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.753250 pyepo-0.3.6/pyepo/twostage/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/twostage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/twostage/autosklearnpred.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/twostage/sklearnpred.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-14 03:59:53.000000 pyepo-0.3.6/pyepo/utlis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 04:00:03.753250 pyepo-0.3.6/pyepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-14 04:00:03.000000 pyepo-0.3.6/pyepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-14 04:00:03.000000 pyepo-0.3.6/pyepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 04:00:03.000000 pyepo-0.3.6/pyepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-14 04:00:03.000000 pyepo-0.3.6/pyepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 04:00:03.000000 pyepo-0.3.6/pyepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 04:00:03.753250 pyepo-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-14 03:59:53.000000 pyepo-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.517354 pyepo-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-19 05:03:49.517354 pyepo-0.3.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.509354 pyepo-0.3.7/pyepo/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/EPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.509354 pyepo-0.3.7/pyepo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.509354 pyepo-0.3.7/pyepo/func/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/abcmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/perturbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/spoplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/utlis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/regret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/unambregret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/copt/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/coptmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/shortestpath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/grb/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/grbmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/omo/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/omomodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/opt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.517354 pyepo-0.3.7/pyepo/twostage/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/twostage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/twostage/autosklearnpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/twostage/sklearnpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/utlis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.517354 pyepo-0.3.7/pyepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:03:49.517354 pyepo-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-19 05:03:40.000000 pyepo-0.3.7/setup.py
```

### Comparing `pyepo-0.3.6/PKG-INFO` & `pyepo-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepo
-Version: 0.3.6
+Version: 0.3.7
 Summary: PyTorch-based End-to-End Predict-then-Optimize Tool
 Home-page: https://github.com/khalil-research/PyEPO
 Author: Bo Tang
 Author-email: bolucas.tang@mail.utoronto.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyepo-0.3.6/pyepo/data/dataset.py` & `pyepo-0.3.7/pyepo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/data/knapsack.py` & `pyepo-0.3.7/pyepo/data/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/data/shortestpath.py` & `pyepo-0.3.7/pyepo/data/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/data/tsp.py` & `pyepo-0.3.7/pyepo/data/tsp.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/func/abcmodule.py` & `pyepo-0.3.7/pyepo/func/abcmodule.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
 
 class optModule(nn.Module):
     """
         An abstract module for the learning to rank losses, which measure the difference in how the predicted cost
         vector and the true cost vector rank a pool of feasible solutions.
     """
-    def __init__(self, optmodel, processes=1, solve_ratio=1, dataset=None):
+    def __init__(self, optmodel, processes=1, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (None/optDataset): the training data
         """
         super().__init__()
         # optimization model
         if not isinstance(optmodel, optModel):
             raise TypeError("arg model is not an optModel")
         self.optmodel = optmodel
@@ -51,15 +52,17 @@
             raise ValueError("Invalid solving ratio {}. It should be between 0 and 1.".
                 format(self.solve_ratio))
         self.solpool = None
         if self.solve_ratio < 1: # init solution pool
             if not isinstance(dataset, optDataset): # type checking
                 raise TypeError("dataset is not an optDataset")
             self.solpool = np.unique(dataset.sols.copy(), axis=0) # remove duplicate
+        # reduction
+        self.reduction = reduction
 
     @abstractmethod
-    def forward(self, pred_cost, true_cost, reduction="mean"):
+    def forward(self, pred_cost, true_cost):
         """
         Forward pass
         """
         # convert tensor
         pass
```

### Comparing `pyepo-0.3.6/pyepo/func/blackbox.py` & `pyepo-0.3.7/pyepo/func/blackbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,109 +46,92 @@
         # build blackbox optimizer
         self.dbb = blackboxOptFunc()
 
     def forward(self, pred_cost):
         """
         Forward pass
         """
-        sols = self.dbb.apply(pred_cost, self.lambd, self.optmodel,
-                              self.processes, self.pool, self.solve_ratio, self)
+        sols = self.dbb.apply(pred_cost, self)
         return sols
 
 
 class blackboxOptFunc(Function):
     """
     A autograd function for differentiable black-box optimizer
     """
 
     @staticmethod
-    def forward(ctx, pred_cost, lambd, optmodel, processes, pool, solve_ratio, module):
+    def forward(ctx, pred_cost, module):
         """
         Forward pass for DBB
 
         Args:
             pred_cost (torch.tensor): a batch of predicted values of the cost
-            lambd (float): a hyperparameter for differentiable block-box to control interpolation degree
-            optmodel (optModel): an PyEPO optimization model
-            processes (int): number of processors, 1 for single-core, 0 for all of cores
-            pool (ProcessPool): process pool object
-            solve_ratio (float): the ratio of new solutions computed during training
             module (optModule): blackboxOpt module
 
         Returns:
             torch.tensor: predicted solutions
         """
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
         rand_sigma = np.random.uniform()
-        if rand_sigma <= solve_ratio:
-            sol, _ = _solve_in_pass(cp, optmodel, processes, pool)
-            if solve_ratio < 1:
+        if rand_sigma <= module.solve_ratio:
+            sol, _ = _solve_in_pass(cp, module.optmodel, module.processes, module.pool)
+            if module.solve_ratio < 1:
                 # add into solpool
                 module.solpool = np.concatenate((module.solpool, sol))
                 # remove duplicate
                 module.solpool = np.unique(module.solpool, axis=0)
         else:
-            sol, _ = _cache_in_pass(cp, optmodel, module.solpool)
+            sol, _ = _cache_in_pass(cp, module.optmodel, module.solpool)
         # convert to tensor
         sol = np.array(sol)
         pred_sol = torch.FloatTensor(sol).to(device)
         # save
         ctx.save_for_backward(pred_cost, pred_sol)
         # add other objects to ctx
-        ctx.lambd = lambd
-        ctx.optmodel = optmodel
-        ctx.processes = processes
-        ctx.pool = pool
-        ctx.solve_ratio = solve_ratio
-        if solve_ratio < 1:
-            ctx.module = module
-        ctx.rand_sigma = rand_sigma
+        ctx.lambd = module.lambd
+        ctx.module = module
         return pred_sol
 
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for DBB
         """
         pred_cost, pred_sol = ctx.saved_tensors
         lambd = ctx.lambd
-        optmodel = ctx.optmodel
-        processes = ctx.processes
-        pool = ctx.pool
-        solve_ratio = ctx.solve_ratio
-        rand_sigma = ctx.rand_sigma
-        if solve_ratio < 1:
-            module = ctx.module
+        module = ctx.module
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         wp = pred_sol.detach().to("cpu").numpy()
         dl = grad_output.detach().to("cpu").numpy()
         # perturbed costs
         cq = cp + lambd * dl
         # solve
-        if rand_sigma <= solve_ratio:
-            sol, _ = _solve_in_pass(cq, optmodel, processes, pool)
-            if solve_ratio < 1:
+        rand_sigma = np.random.uniform()
+        if rand_sigma <= module.solve_ratio:
+            sol, _ = _solve_in_pass(cq, module.optmodel, module.processes, module.pool)
+            if module.solve_ratio < 1:
                 # add into solpool
                 module.solpool = np.concatenate((module.solpool, sol))
                 # remove duplicate
                 module.solpool = np.unique(module.solpool, axis=0)
         else:
-            sol, _ = _cache_in_pass(cq, optmodel, module.solpool)
+            sol, _ = _cache_in_pass(cq, module.optmodel, module.solpool)
         # get gradient
-        grad = (np.array(sol) - wp) / lambd
+        grad = (sol - wp) / module.lambd
         # convert to tensor
         grad = torch.FloatTensor(grad).to(device)
-        return grad, None, None, None, None, None, None
+        return grad, None
 
 
 class negativeIdentity(optModule):
     """
     An autograd module for the differentiable optimizer, which yields optimal a
     solution and use negative identity as a gradient on the backward pass.
 
@@ -176,59 +159,54 @@
         # build blackbox optimizer
         self.nid = negativeIdentityFunc()
 
     def forward(self, pred_cost):
         """
         Forward pass
         """
-        sols = self.nid.apply(pred_cost, self.optmodel, self.processes,
-                              self.pool, self.solve_ratio, self)
+        sols = self.nid.apply(pred_cost, self)
         return sols
 
 
 class negativeIdentityFunc(Function):
     """
     A autograd function for differentiable black-box optimizer
     """
 
     @staticmethod
-    def forward(ctx, pred_cost, optmodel, processes, pool, solve_ratio, module):
+    def forward(ctx, pred_cost, module):
         """
         Forward pass for NID
 
         Args:
             pred_cost (torch.tensor): a batch of predicted values of the cost
-            optmodel (optModel): an PyEPO optimization model
-            processes (int): number of processors, 1 for single-core, 0 for all of cores
-            pool (ProcessPool): process pool object
-            solve_ratio (float): the ratio of new solutions computed during training
             module (optModule): blackboxOpt module
 
         Returns:
             torch.tensor: predicted solutions
         """
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
         rand_sigma = np.random.uniform()
-        if rand_sigma <= solve_ratio:
-            sol, _ = _solve_in_pass(cp, optmodel, processes, pool)
-            if solve_ratio < 1:
+        if rand_sigma <= module.solve_ratio:
+            sol, _ = _solve_in_pass(cp, module.optmodel, module.processes, module.pool)
+            if module.solve_ratio < 1:
                 # add into solpool
                 module.solpool = np.concatenate((module.solpool, sol))
                 # remove duplicate
                 module.solpool = np.unique(module.solpool, axis=0)
         else:
-            sol, _ = _cache_in_pass(cp, optmodel, module.solpool)
+            sol, _ = _cache_in_pass(cp, module.optmodel, module.solpool)
         # convert to tensor
         pred_sol = torch.FloatTensor(np.array(sol)).to(device)
         # add other objects to ctx
-        ctx.optmodel = optmodel
+        ctx.optmodel = module.optmodel
         return pred_sol
 
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for NID
         """
@@ -237,8 +215,8 @@
         device = grad_output.device
         # identity matrix
         I = torch.eye(grad_output.shape[1]).to(device)
         if optmodel.modelSense == EPO.MINIMIZE:
             grad = - I
         if optmodel.modelSense == EPO.MAXIMIZE:
             grad = I
-        return grad_output @ grad, None, None, None, None, None
+        return grad_output @ grad, None
```

### Comparing `pyepo-0.3.6/pyepo/func/contrastive.py` & `pyepo-0.3.7/pyepo/func/contrastive.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,30 @@
     maximizes the separation of the probability of the optimal solution.
 
     Thus allows us to design an algorithm based on stochastic gradient descent.
 
     Reference: <https://www.ijcai.org/proceedings/2021/390>
     """
 
-    def __init__(self, optmodel, processes=1, solve_ratio=1, dataset=None):
+    def __init__(self, optmodel, processes=1, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (None/optDataset): the training data, usually this is simply the training set
         """
-        super().__init__(optmodel, processes, solve_ratio, dataset)
+        super().__init__(optmodel, processes, solve_ratio, reduction, dataset)
         # solution pool
         if not isinstance(dataset, optDataset): # type checking
             raise TypeError("dataset is not an optDataset")
         self.solpool = np.unique(dataset.sols.copy(), axis=0) # remove duplicate
 
-    def forward(self, pred_cost, true_sol, reduction="mean"):
+    def forward(self, pred_cost, true_sol):
         """
         Forward pass
         """
         # get device
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
@@ -62,22 +63,22 @@
         objpool_cp = torch.einsum("bd,nd->bn", pred_cost, solpool)
         # get loss
         if self.optmodel.modelSense == EPO.MINIMIZE:
             loss = (obj_cp - objpool_cp).mean(axis=1)
         if self.optmodel.modelSense == EPO.MAXIMIZE:
             loss = (objpool_cp - obj_cp).mean(axis=1)
         # reduction
-        if reduction == "mean":
+        if self.reduction == "mean":
             loss = torch.mean(loss)
-        elif reduction == "sum":
+        elif self.reduction == "sum":
             loss = torch.sum(loss)
-        elif reduction == "none":
+        elif self.reduction == "none":
             loss = loss
         else:
-            raise ValueError("No reduction '{}'.".format(reduction))
+            raise ValueError("No reduction '{}'.".format(self.reduction))
         return loss
 
 
 class contrastiveMAP(optModule):
     """
     An autograd module for Maximum A Posterior contrastive estimation as
     surrogate loss functions, which is an efficient self-contrastive algorithm.
@@ -86,29 +87,30 @@
     maximizes the separation of the probability of the optimal solution.
 
     Thus, it allows us to design an algorithm based on stochastic gradient descent.
 
     Reference: <https://www.ijcai.org/proceedings/2021/390>
     """
 
-    def __init__(self, optmodel, processes=1, solve_ratio=1, dataset=None):
+    def __init__(self, optmodel, processes=1, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (None/optDataset): the training data, usually this is simply the training set
         """
-        super().__init__(optmodel, processes, solve_ratio, dataset)
+        super().__init__(optmodel, processes, solve_ratio, reduction, dataset)
         # solution pool
         if not isinstance(dataset, optDataset): # type checking
             raise TypeError("dataset is not an optDataset")
         self.solpool = np.unique(dataset.sols.copy(), axis=0) # remove duplicate
 
-    def forward(self, pred_cost, true_sol, reduction="mean"):
+    def forward(self, pred_cost, true_sol):
         """
         Forward pass
         """
         # get device
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
@@ -126,16 +128,16 @@
         objpool_cp = torch.einsum("bd,nd->bn", pred_cost, solpool)
         # get loss
         if self.optmodel.modelSense == EPO.MINIMIZE:
             loss, _ = (obj_cp - objpool_cp).max(axis=1)
         if self.optmodel.modelSense == EPO.MAXIMIZE:
             loss, _ = (objpool_cp - obj_cp).max(axis=1)
         # reduction
-        if reduction == "mean":
+        if self.reduction == "mean":
             loss = torch.mean(loss)
-        elif reduction == "sum":
+        elif self.reduction == "sum":
             loss = torch.sum(loss)
-        elif reduction == "none":
+        elif self.reduction == "none":
             loss = loss
         else:
-            raise ValueError("No reduction '{}'.".format(reduction))
+            raise ValueError("No reduction '{}'.".format(self.reduction))
         return loss
```

### Comparing `pyepo-0.3.6/pyepo/func/perturbed.py` & `pyepo-0.3.7/pyepo/func/perturbed.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,76 +51,56 @@
         # build optimizer
         self.ptb = perturbedOptFunc()
 
     def forward(self, pred_cost):
         """
         Forward pass
         """
-        sols = self.ptb.apply(pred_cost, self.optmodel, self.n_samples,
-                              self.sigma, self.processes, self.pool, self.rnd,
-                              self.solve_ratio, self)
+        sols = self.ptb.apply(pred_cost, self)
         return sols
 
 
 class perturbedOptFunc(Function):
     """
     A autograd function for perturbed optimizer
     """
 
     @staticmethod
-    def forward(ctx, pred_cost, optmodel, n_samples, sigma,
-                processes, pool, rnd, solve_ratio, module):
+    def forward(ctx, pred_cost, module):
         """
         Forward pass for perturbed
 
         Args:
             pred_cost (torch.tensor): a batch of predicted values of the cost
-            optmodel (optModel): an PyEPO optimization model
-            n_samples (int): number of Monte-Carlo samples
-            sigma (float): the amplitude of the perturbation
-            processes (int): number of processors, 1 for single-core, 0 for all of cores
-            pool (ProcessPool): process pool object
-            rnd (RondomState): numpy random state
-            solve_ratio (float): the ratio of new solutions computed during training
             module (optModule): perturbedOpt module
 
         Returns:
             torch.tensor: solution expectations with perturbation
         """
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         # sample perturbations
-        noises = rnd.normal(0, 1, size=(n_samples, *cp.shape))
-        ptb_c = cp + sigma * noises
+        noises = module.rnd.normal(0, 1, size=(module.n_samples, *cp.shape))
+        ptb_c = cp + module.sigma * noises
         # solve with perturbation
-        rand_sigma = np.random.uniform()
-        if rand_sigma <= solve_ratio:
-            ptb_sols = _solve_in_pass(ptb_c, optmodel, processes, pool)
-            if solve_ratio < 1:
-                sols = ptb_sols.reshape(-1, cp.shape[1])
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sols))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
-        else:
-            ptb_sols = _cache_in_pass(ptb_c, optmodel, module.solpool)
+        ptb_sols = _solve_or_cache(ptb_c, module)
         # solution expectation
         e_sol = ptb_sols.mean(axis=1)
         # convert to tensor
         noises = torch.FloatTensor(noises).to(device)
         ptb_sols = torch.FloatTensor(ptb_sols).to(device)
         e_sol = torch.FloatTensor(e_sol).to(device)
         # save solutions
         ctx.save_for_backward(ptb_sols, noises)
         # add other objects to ctx
-        ctx.optmodel = optmodel
-        ctx.n_samples = n_samples
-        ctx.sigma = sigma
+        ctx.optmodel = module.optmodel
+        ctx.n_samples = module.n_samples
+        ctx.sigma = module.sigma
         return e_sol
 
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for perturbed
         """
@@ -128,15 +108,15 @@
         optmodel = ctx.optmodel
         n_samples = ctx.n_samples
         sigma = ctx.sigma
         grad = torch.einsum("nbd,bn->bd",
                             noises,
                             torch.einsum("bnd,bd->bn", ptb_sols, grad_output))
         grad /= n_samples * sigma
-        return grad, None, None, None, None, None, None, None, None
+        return grad, None
 
 
 class perturbedFenchelYoung(optModule):
     """
     An autograd module for Fenchel-Young loss using perturbation techniques. The
     use of the loss improves the algorithmic by the specific expression of the
     gradients of the loss.
@@ -148,106 +128,87 @@
     and solutions with less computation. Thus, allows us to design an algorithm
     based on stochastic gradient descent.
 
     Reference: <https://papers.nips.cc/paper/2020/hash/6bb56208f672af0dd65451f869fedfd9-Abstract.html>
     """
 
     def __init__(self, optmodel, n_samples=10, sigma=1.0, processes=1,
-                 seed=135, solve_ratio=1, dataset=None):
+                 seed=135, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             n_samples (int): number of Monte-Carlo samples
             sigma (float): the amplitude of the perturbation
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             seed (int): random state seed
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (None/optDataset): the training data
         """
-        super().__init__(optmodel, processes, solve_ratio, dataset)
+        super().__init__(optmodel, processes, solve_ratio, reduction, dataset)
         # number of samples
         self.n_samples = n_samples
         # perturbation amplitude
         self.sigma = sigma
         # random state
         self.rnd = np.random.RandomState(seed)
         # build optimizer
         self.pfy = perturbedFenchelYoungFunc()
 
-    def forward(self, pred_cost, true_sol, reduction="mean"):
+    def forward(self, pred_cost, true_sol):
         """
         Forward pass
         """
-        loss = self.pfy.apply(pred_cost, true_sol, self.optmodel, self.n_samples,
-                              self.sigma, self.processes, self.pool, self.rnd,
-                              self.solve_ratio, self)
+        loss = self.pfy.apply(pred_cost, true_sol, self)
         # reduction
-        if reduction == "mean":
+        if self.reduction == "mean":
             loss = torch.mean(loss)
-        elif reduction == "sum":
+        elif self.reduction == "sum":
             loss = torch.sum(loss)
-        elif reduction == "none":
+        elif self.reduction == "none":
             loss = loss
         else:
-            raise ValueError("No reduction '{}'.".format(reduction))
+            raise ValueError("No reduction '{}'.".format(self.reduction))
         return loss
 
 
 class perturbedFenchelYoungFunc(Function):
     """
     A autograd function for Fenchel-Young loss using perturbation techniques.
     """
 
     @staticmethod
-    def forward(ctx, pred_cost, true_sol, optmodel, n_samples, sigma,
-                processes, pool, rnd, solve_ratio, module):
+    def forward(ctx, pred_cost, true_sol, module):
         """
         Forward pass for perturbed Fenchel-Young loss
 
         Args:
             pred_cost (torch.tensor): a batch of predicted values of the cost
             true_sol (torch.tensor): a batch of true optimal solutions
-            optmodel (optModel): an PyEPO optimization model
-            n_samples (int): number of Monte-Carlo samples
-            sigma (float): the amplitude of the perturbation
-            processes (int): number of processors, 1 for single-core, 0 for all of cores
-            pool (ProcessPool): process pool object
-            rnd (RondomState): numpy random state
-            solve_ratio (float): the ratio of new solutions computed during training
             module (optModule): perturbedFenchelYoung module
 
         Returns:
             torch.tensor: solution expectations with perturbation
         """
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         w = true_sol.detach().to("cpu").numpy()
         # sample perturbations
-        noises = rnd.normal(0, 1, size=(n_samples, *cp.shape))
-        ptb_c = cp + sigma * noises
+        noises = module.rnd.normal(0, 1, size=(module.n_samples, *cp.shape))
+        ptb_c = cp + module.sigma * noises
         # solve with perturbation
-        rand_sigma = np.random.uniform()
-        if rand_sigma <= solve_ratio:
-            ptb_sols = _solve_in_pass(ptb_c, optmodel, processes, pool)
-            if solve_ratio < 1:
-                sols = ptb_sols.reshape(-1, cp.shape[1])
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sols))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
-        else:
-            ptb_sols = _cache_in_pass(ptb_c, optmodel, module.solpool)
+        ptb_sols = _solve_or_cache(ptb_c, module)
         # solution expectation
         e_sol = ptb_sols.mean(axis=1)
         # difference
-        if optmodel.modelSense == EPO.MINIMIZE:
+        if module.optmodel.modelSense == EPO.MINIMIZE:
             diff = w - e_sol
-        if optmodel.modelSense == EPO.MAXIMIZE:
+        if module.optmodel.modelSense == EPO.MAXIMIZE:
             diff = e_sol - w
         # loss
         loss = np.sum(diff**2, axis=1)
         # convert to tensor
         diff = torch.FloatTensor(diff).to(device)
         loss = torch.FloatTensor(loss).to(device)
         # save solutions
@@ -257,176 +218,259 @@
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for perturbed Fenchel-Young loss
         """
         grad, = ctx.saved_tensors
         grad_output = torch.unsqueeze(grad_output, dim=-1)
-        return grad * grad_output, None, None, None, None, None, None, None, None, None
+        return grad * grad_output, None, None
 
 
 class implicitMLE(optModule):
     """
     An autograd module for Implicit Maximum Likelihood Estimator, which yield
     an optimal solution in a constrained exponential family distribution via
     Perturb-and-MAP.
 
-    For I-LME, it works as black-box combinatorial solvers, in which constraints
+    For I-MLE, it works as black-box combinatorial solvers, in which constraints
     are known and fixed, but the cost vector need to be predicted from
     contextual data.
 
-    The I-LME approximate gradient of optimizer smoothly. Thus, allows us to
+    The I-MLE approximate gradient of optimizer smoothly. Thus, allows us to
     design an algorithm based on stochastic gradient descent.
 
     Reference: <https://proceedings.neurips.cc/paper_files/paper/2021/hash/7a430339c10c642c4b2251756fd1b484-Abstract.html>
     """
 
-    def __init__(self, optmodel, n_samples=10, sigma=1.0, lambd=10, processes=1,
-                 distribution=sumGammaDistribution(kappa=5), solve_ratio=1,
-                 dataset=None):
+    def __init__(self, optmodel, n_samples=10, sigma=1.0, lambd=10,
+                 distribution=sumGammaDistribution(kappa=5), two_sides=False,
+                 processes=1, solve_ratio=1, dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             n_samples (int): number of Monte-Carlo samples
             sigma (float): noise temperature for the input distribution
             lambd (float): a hyperparameter for differentiable block-box to control interpolation degree
-            processes (int): number of processors, 1 for single-core, 0 for all of cores
             distribution (distribution): noise distribution
+            two_sides (bool): approximate gradient by two-sided perturbation or not
+            processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
             dataset (None/optDataset): the training data
         """
         super().__init__(optmodel, processes, solve_ratio, dataset)
         # number of samples
         self.n_samples = n_samples
         # noise temperature
         self.sigma = sigma
         # smoothing parameter
         if lambd <= 0:
             raise ValueError("lambda is not positive.")
         self.lambd = lambd
         # noise distribution
         self.distribution = distribution
+        # symmetric perturbation
+        self.two_sides = two_sides
         # build I-LME
-        self.ilme = implicitMLEFunc()
+        self.imle = implicitMLEFunc()
 
     def forward(self, pred_cost):
         """
         Forward pass
         """
-        sols = self.ilme.apply(pred_cost, self.optmodel, self.n_samples,
-                                self.sigma, self.lambd, self.processes,
-                                self.pool, self.distribution, self.solve_ratio,
-                                self)
+        sols = self.imle.apply(pred_cost, self)
         return sols
 
 
 class implicitMLEFunc(Function):
     """
     A autograd function for Implicit Maximum Likelihood Estimator
     """
 
     @staticmethod
-    def forward(ctx, pred_cost, optmodel, n_samples, sigma, lambd,
-                processes, pool, distribution, solve_ratio, module):
+    def forward(ctx, pred_cost, module):
         """
         Forward pass for IMLE
 
         Args:
             pred_cost (torch.tensor): a batch of predicted values of the cost
-            optmodel (optModel): an PyEPO optimization model
-            n_samples (int): number of Monte-Carlo samples
-            sigma (float): noise temperature for the input distribution
-            lambd (float): a hyperparameter for differentiable block-box to control interpolation degree
-            processes (int): number of processors, 1 for single-core, 0 for all of cores
-            pool (ProcessPool): process pool object
-            distribution (distribution): noise distribution
-            solve_ratio (float): the ratio of new solutions computed during training
             module (optModule): implicitMLE module
 
         Returns:
             torch.tensor: predicted solutions
         """
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         # sample perturbations
-        noises = distribution.sample(size=(n_samples, *cp.shape))
-        ptb_c = cp + sigma * noises
+        noises = module.distribution.sample(size=(module.n_samples, *cp.shape))
+        ptb_c = cp + module.sigma * noises
         # solve with perturbation
-        rand_sigma = np.random.uniform()
-        if rand_sigma <= solve_ratio:
-            ptb_sols = _solve_in_pass(ptb_c, optmodel, processes, pool)
-            if solve_ratio < 1:
-                sols = ptb_sols.reshape(-1, cp.shape[1])
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sols))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
-        else:
-            ptb_sols = _cache_in_pass(ptb_c, optmodel, module.solpool)
+        ptb_sols = _solve_or_cache(ptb_c, module)
         # solution average
         e_sol = ptb_sols.mean(axis=1)
         # convert to tensor
         e_sol = torch.FloatTensor(e_sol).to(device)
         # save
         ctx.save_for_backward(pred_cost)
         # add other objects to ctx
         ctx.noises = noises
         ctx.ptb_sols = ptb_sols
-        ctx.lambd = lambd
-        ctx.optmodel = optmodel
-        ctx.processes = processes
-        ctx.pool = pool
-        ctx.solve_ratio = solve_ratio
-        if solve_ratio < 1:
-            ctx.module = module
-        ctx.rand_sigma = rand_sigma
+        ctx.module = module
         return e_sol
 
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for IMLE
         """
         pred_cost, = ctx.saved_tensors
         noises = ctx.noises
         ptb_sols = ctx.ptb_sols
-        lambd = ctx.lambd
-        optmodel = ctx.optmodel
-        processes = ctx.processes
-        pool = ctx.pool
-        solve_ratio = ctx.solve_ratio
-        rand_sigma = ctx.rand_sigma
-        if solve_ratio < 1:
-            module = ctx.module
+        module = ctx.module
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         dl = grad_output.detach().to("cpu").numpy()
-        # perturbed costs
-        ptb_cq = cp + lambd * dl + noises
+        # positive perturbed costs
+        ptb_cp_pos = cp + module.lambd * dl + noises
         # solve with perturbation
-        rand_sigma = np.random.uniform()
-        if rand_sigma <= solve_ratio:
-            ptb_solsq = _solve_in_pass(ptb_cq, optmodel, processes, pool)
-            if solve_ratio < 1:
-                sols = ptb_solsq.reshape(-1, cp.shape[1])
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sols))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
+        ptb_sols_pos = _solve_or_cache(ptb_cp_pos, module)
+        if module.two_sides:
+            # negative perturbed costs
+            ptb_cp_neg = cp - module.lambd * dl + noises
+            # solve with perturbation
+            ptb_sols_neg = _solve_or_cache(ptb_cp_neg, module)
+            # get two-side gradient
+            grad = (ptb_sols_pos - ptb_sols_neg).mean(axis=1) / (2 * module.lambd)
         else:
-            ptb_solsq = _cache_in_pass(ptb_cq, optmodel, module.solpool)
-        # get gradient
-        grad =  (np.array(ptb_solsq) - ptb_sols).mean(axis=1) / lambd
+            # get single side gradient
+            grad = (ptb_sols_pos - ptb_sols).mean(axis=1) / module.lambd
         # convert to tensor
         grad = torch.FloatTensor(grad).to(device)
-        return grad, None, None, None, None, None, None, None, None, None
+        return grad, None, None
+
+
+class adaptiveImplicitMLE(optModule):
+    """
+    An autograd module for Adaptive Implicit Maximum Likelihood Estimator, which
+    adaptively choose hyperparameter λ and yield an optimal solution in a
+    constrained exponential family distribution via Perturb-and-MAP.
+
+    For AI-MLE, it works as black-box combinatorial solvers, in which constraints
+    are known and fixed, but the cost vector need to be predicted from
+    contextual data.
+
+    The AI-MLE approximate gradient of optimizer smoothly. Thus, allows us to
+    design an algorithm based on stochastic gradient descent.
+
+    Reference: <https://ojs.aaai.org/index.php/AAAI/article/view/26103>
+    """
+
+    def __init__(self, optmodel, n_samples=10, sigma=1.0,
+                 distribution=sumGammaDistribution(kappa=5), two_sides=False,
+                 processes=1, solve_ratio=1, dataset=None):
+        """
+        Args:
+            optmodel (optModel): an PyEPO optimization model
+            n_samples (int): number of Monte-Carlo samples
+            sigma (float): noise temperature for the input distribution
+            distribution (distribution): noise distribution
+            two_sides (bool): approximate gradient by two-sided perturbation or not
+            processes (int): number of processors, 1 for single-core, 0 for all of cores
+            solve_ratio (float): the ratio of new solutions computed during training
+            dataset (None/optDataset): the training data
+        """
+        super().__init__(optmodel, processes, solve_ratio, dataset)
+        # number of samples
+        self.n_samples = n_samples
+        # noise temperature
+        self.sigma = sigma
+        # noise distribution
+        self.distribution = distribution
+        # symmetric perturbation
+        self.two_sides = two_sides
+        # init adaptive params
+        self.alpha = 0 # adaptive magnitude α
+        self.grad_norm_avg = 1 # gradient norm estimate
+        self.step = 1e-3 # update step for α
+        # build I-LME
+        self.aimle = adaptiveImplicitMLEFunc()
+
+    def forward(self, pred_cost):
+        """
+        Forward pass
+        """
+        sols = self.aimle.apply(pred_cost, self)
+        return sols
+
+
+class adaptiveImplicitMLEFunc(implicitMLEFunc):
+    """
+    A autograd function for Adaptive Implicit Maximum Likelihood Estimator
+    """
+    @staticmethod
+    def backward(ctx, grad_output):
+        """
+        Backward pass for IMLE
+        """
+        pred_cost, = ctx.saved_tensors
+        noises = ctx.noises
+        ptb_sols = ctx.ptb_sols
+        module = ctx.module
+        # get device
+        device = pred_cost.device
+        # convert tenstor
+        cp = pred_cost.detach().to("cpu").numpy()
+        dl = grad_output.detach().to("cpu").numpy()
+        # calculate λ
+        lambd = module.alpha * np.linalg.norm(cp) / np.linalg.norm(dl)
+        # positive perturbed costs
+        ptb_cp_pos = cp + lambd * dl + noises
+        # solve with perturbation
+        ptb_sols_pos = _solve_or_cache(ptb_cp_pos, module)
+        if module.two_sides:
+            # negative perturbed costs
+            ptb_cp_neg = cp - lambd * dl + noises
+            # solve with perturbation
+            ptb_sols_neg = _solve_or_cache(ptb_cp_neg, module)
+            # get two-side gradient
+            grad = (ptb_sols_pos - ptb_sols_neg).mean(axis=1) / (2 * lambd + 1e-7)
+        else:
+            # get single side gradient
+            grad = (ptb_sols_pos - ptb_sols).mean(axis=1) / (lambd + 1e-7)
+        # convert to tensor
+        grad = torch.FloatTensor(grad).to(device)
+        # moving average of the gradient norm
+        grad_norm = (grad.abs() > 1e-7).float().mean()
+        module.grad_norm_avg = 0.9 * module.grad_norm_avg + 0.1 * grad_norm
+        # update α to make grad_norm closer to 1
+        if module.grad_norm_avg < 1:
+            module.alpha += module.step
+        else:
+            module.alpha -= module.step
+        return grad, None, None
+
+
+def _solve_or_cache(ptb_c, module):
+    rand_sigma = np.random.uniform()
+    # solve optimization
+    if rand_sigma <= module.solve_ratio:
+        ptb_sols = _solve_in_pass(ptb_c, module.optmodel, module.processes, module.pool)
+        if module.solve_ratio < 1:
+            sols = ptb_sols.reshape(-1, cp.shape[1])
+            # add into solpool
+            module.solpool = np.concatenate((module.solpool, sols))
+            # remove duplicate
+            module.solpool = np.unique(module.solpool, axis=0)
+    # best cached solution
+    else:
+        ptb_sols = _cache_in_pass(ptb_c, optmodel, module.solpool)
+    return ptb_sols
 
 
 def _solve_in_pass(ptb_c, optmodel, processes, pool):
     """
     A function to solve optimization in the forward pass
     """
     # number of instance
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyepo-0.3.6/pyepo/func/rank.py` & `pyepo-0.3.7/pyepo/func/rank.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,29 +25,30 @@
 
     Thus, it allows us to design an algorithm based on stochastic gradient
     descent.
 
     Reference: <https://proceedings.mlr.press/v162/mandi22a.html>
     """
 
-    def __init__(self, optmodel, processes=1, solve_ratio=1, dataset=None):
+    def __init__(self, optmodel, processes=1, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (optDataset): the training data, usually this is simply the training set
         """
-        super().__init__(optmodel, processes, solve_ratio, dataset)
+        super().__init__(optmodel, processes, solve_ratio, reduction, dataset)
         # solution pool
         if not isinstance(dataset, optDataset): # type checking
             raise TypeError("dataset is not an optDataset")
         self.solpool = np.unique(dataset.sols.copy(), axis=0) # remove duplicate
 
-    def forward(self, pred_cost, true_cost, reduction="mean"):
+    def forward(self, pred_cost, true_cost):
         """
         Forward pass
         """
         # get device
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
@@ -67,22 +68,22 @@
         if self.optmodel.modelSense == EPO.MINIMIZE:
             loss = - (F.log_softmax(objpool_cp, dim=1) *
                       F.softmax(objpool_c, dim=1))
         if self.optmodel.modelSense == EPO.MAXIMIZE:
             loss = - (F.log_softmax(- objpool_cp, dim=1) *
                       F.softmax(- objpool_c, dim=1))
         # reduction
-        if reduction == "mean":
+        if self.reduction == "mean":
             loss = torch.mean(loss)
-        elif reduction == "sum":
+        elif self.reduction == "sum":
             loss = torch.sum(loss)
-        elif reduction == "none":
+        elif self.reduction == "none":
             loss = loss
         else:
-            raise ValueError("No reduction '{}'.".format(reduction))
+            raise ValueError("No reduction '{}'.".format(self.reduction))
         return loss
 
 
 class pairwiseLTR(optModule):
     """
     An autograd module for pairwise learning to rank, where the goal is to learn
     an objective function that ranks a pool of feasible solutions correctly.
@@ -92,29 +93,30 @@
 
     Thus, it allows us to design an algorithm based on stochastic gradient
     descent.
 
     Reference: <https://proceedings.mlr.press/v162/mandi22a.html>
     """
 
-    def __init__(self, optmodel, processes=1, solve_ratio=1, dataset=None):
+    def __init__(self, optmodel, processes=1, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (optDataset): the training data
         """
-        super().__init__(optmodel, processes, solve_ratio, dataset)
+        super().__init__(optmodel, processes, solve_ratio, reduction, dataset)
         # solution pool
         if not isinstance(dataset, optDataset): # type checking
             raise TypeError("dataset is not an optDataset")
         self.solpool = np.unique(dataset.sols.copy(), axis=0) # remove duplicate
 
-    def forward(self, pred_cost, true_cost, reduction="mean"):
+    def forward(self, pred_cost, true_cost):
         """
         Forward pass
         """
         # get device
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
@@ -147,22 +149,22 @@
             # best vs rest loss
             if self.optmodel.modelSense == EPO.MINIMIZE:
                 loss.append(relu(objpool_cp_best - objpool_cp_rest).mean())
             if self.optmodel.modelSense == EPO.MAXIMIZE:
                 loss.append(relu(objpool_cp_rest - objpool_cp_best).mean())
         loss = torch.stack(loss)
         # reduction
-        if reduction == "mean":
+        if self.reduction == "mean":
             loss = torch.mean(loss)
-        elif reduction == "sum":
+        elif self.reduction == "sum":
             loss = torch.sum(loss)
-        elif reduction == "none":
+        elif self.reduction == "none":
             loss = loss
         else:
-            raise ValueError("No reduction '{}'.".format(reduction))
+            raise ValueError("No reduction '{}'.".format(self.reduction))
         return loss
 
 
 class pointwiseLTR(optModule):
     """
     An autograd module for pointwise learning to rank, where the goal is to
     learn an objective function that ranks a pool of feasible solutions
@@ -173,29 +175,30 @@
 
     Thus, it allows us to design an algorithm based on stochastic gradient
     descent.
 
     Reference: <https://proceedings.mlr.press/v162/mandi22a.html>
     """
 
-    def __init__(self, optmodel, processes=1, solve_ratio=1, dataset=None):
+    def __init__(self, optmodel, processes=1, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (optDataset): the training data
         """
-        super().__init__(optmodel, processes, solve_ratio, dataset)
+        super().__init__(optmodel, processes, solve_ratio, reduction, dataset)
         # solution pool
         if not isinstance(dataset, optDataset): # type checking
             raise TypeError("dataset is not an optDataset")
         self.solpool = np.unique(dataset.sols.copy(), axis=0) # remove duplicate
 
-    def forward(self, pred_cost, true_cost, reduction="mean"):
+    def forward(self, pred_cost, true_cost):
         """
         Forward pass
         """
         # get device
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
@@ -210,16 +213,16 @@
         solpool = torch.from_numpy(self.solpool.astype(np.float32)).to(device)
         # obj for solpool as score
         objpool_c = true_cost @ solpool.T # true cost
         objpool_cp = pred_cost @ solpool.T # pred cost
         # squared loss
         loss = (objpool_c - objpool_cp).square().mean(axis=1)
         # reduction
-        if reduction == "mean":
+        if self.reduction == "mean":
             loss = torch.mean(loss)
-        elif reduction == "sum":
+        elif self.reduction == "sum":
             loss = torch.sum(loss)
-        elif reduction == "none":
+        elif self.reduction == "none":
             loss = loss
         else:
-            raise ValueError("No reduction '{}'.".format(reduction))
+            raise ValueError("No reduction '{}'.".format(self.reduction))
         return loss
```

### Comparing `pyepo-0.3.6/pyepo/func/spoplus.py` & `pyepo-0.3.7/pyepo/func/spoplus.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,65 +23,59 @@
 
     The SPO+ Loss is convex with subgradient. Thus, it allows us to design an
     algorithm based on stochastic gradient descent.
 
     Reference: <https://doi.org/10.1287/mnsc.2020.3922>
     """
 
-    def __init__(self, optmodel, processes=1, solve_ratio=1, dataset=None):
+    def __init__(self, optmodel, processes=1, solve_ratio=1, reduction="mean", dataset=None):
         """
         Args:
             optmodel (optModel): an PyEPO optimization model
             processes (int): number of processors, 1 for single-core, 0 for all of cores
             solve_ratio (float): the ratio of new solutions computed during training
+            reduction (str): the reduction to apply to the output
             dataset (None/optDataset): the training data
         """
-        super().__init__(optmodel, processes, solve_ratio, dataset)
+        super().__init__(optmodel, processes, solve_ratio, reduction, dataset)
         # build carterion
         self.spop = SPOPlusFunc()
 
-    def forward(self, pred_cost, true_cost, true_sol, true_obj, reduction="mean"):
+    def forward(self, pred_cost, true_cost, true_sol, true_obj):
         """
         Forward pass
         """
-        loss = self.spop.apply(pred_cost, true_cost, true_sol, true_obj,
-                               self.optmodel, self.processes, self.pool,
-                               self.solve_ratio, self)
+        loss = self.spop.apply(pred_cost, true_cost, true_sol, true_obj, self)
         # reduction
-        if reduction == "mean":
+        if self.reduction == "mean":
             loss = torch.mean(loss)
-        elif reduction == "sum":
+        elif self.reduction == "sum":
             loss = torch.sum(loss)
-        elif reduction == "none":
+        elif self.reduction == "none":
             loss = loss
         else:
-            raise ValueError("No reduction '{}'.".format(reduction))
+            raise ValueError("No reduction '{}'.".format(self.reduction))
         return loss
 
 
 class SPOPlusFunc(Function):
     """
     A autograd function for SPO+ Loss
     """
 
     @staticmethod
-    def forward(ctx, pred_cost, true_cost, true_sol, true_obj,
-                optmodel, processes, pool, solve_ratio, module):
+    def forward(ctx, pred_cost, true_cost, true_sol, true_obj, module):
         """
         Forward pass for SPO+
 
         Args:
             pred_cost (torch.tensor): a batch of predicted values of the cost
             true_cost (torch.tensor): a batch of true values of the cost
             true_sol (torch.tensor): a batch of true optimal solutions
             true_obj (torch.tensor): a batch of true optimal objective values
-            optmodel (optModel): an PyEPO optimization model
-            processes (int): number of processors, 1 for single-core, 0 for all of cores
-            pool (ProcessPool): process pool object
-            solve_ratio (float): the ratio of new solutions computed during training
             module (optModule): SPOPlus modeul
 
         Returns:
             torch.tensor: SPO+ loss
         """
         # get device
         device = pred_cost.device
@@ -89,47 +83,47 @@
         cp = pred_cost.detach().to("cpu").numpy()
         c = true_cost.detach().to("cpu").numpy()
         w = true_sol.detach().to("cpu").numpy()
         z = true_obj.detach().to("cpu").numpy()
         # check sol
         #_check_sol(c, w, z)
         # solve
-        if np.random.uniform() <= solve_ratio:
-            sol, obj = _solve_in_pass(2*cp-c, optmodel, processes, pool)
-            if solve_ratio < 1:
+        if np.random.uniform() <= module.solve_ratio:
+            sol, obj = _solve_in_pass(2*cp-c, module.optmodel, module.processes, module.pool)
+            if module.solve_ratio < 1:
                 # add into solpool
                 module.solpool = np.concatenate((module.solpool, sol))
                 # remove duplicate
                 module.solpool = np.unique(module.solpool, axis=0)
         else:
-            sol, obj = _cache_in_pass(2*cp-c, optmodel, module.solpool)
+            sol, obj = _cache_in_pass(2*cp-c, module.optmodel, module.solpool)
         # calculate loss
         loss = []
         for i in range(len(cp)):
             loss.append(- obj[i] + 2 * np.dot(cp[i], w[i]) - z[i])
         # sense
-        if optmodel.modelSense == EPO.MINIMIZE:
+        if module.optmodel.modelSense == EPO.MINIMIZE:
             loss = np.array(loss)
-        if optmodel.modelSense == EPO.MAXIMIZE:
+        if module.optmodel.modelSense == EPO.MAXIMIZE:
             loss = - np.array(loss)
         # convert to tensor
         loss = torch.FloatTensor(loss).to(device)
         sol = np.array(sol)
         sol = torch.FloatTensor(sol).to(device)
         # save solutions
         ctx.save_for_backward(true_sol, sol)
         # add other objects to ctx
-        ctx.optmodel = optmodel
+        ctx.optmodel = module.optmodel
         return loss
 
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for SPO+
         """
         w, wq = ctx.saved_tensors
         optmodel = ctx.optmodel
         if optmodel.modelSense == EPO.MINIMIZE:
             grad = 2 * (w - wq)
         if optmodel.modelSense == EPO.MAXIMIZE:
             grad = 2 * (wq - w)
-        return grad_output * grad, None, None, None, None, None, None, None, None
+        return grad_output * grad, None, None, None, None
```

### Comparing `pyepo-0.3.6/pyepo/func/utlis.py` & `pyepo-0.3.7/pyepo/func/utlis.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/metric/metrics.py` & `pyepo-0.3.7/pyepo/metric/metrics.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/metric/mse.py` & `pyepo-0.3.7/pyepo/metric/mse.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/metric/regret.py` & `pyepo-0.3.7/pyepo/metric/regret.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/metric/unambregret.py` & `pyepo-0.3.7/pyepo/metric/unambregret.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/copt/coptmodel.py` & `pyepo-0.3.7/pyepo/model/copt/coptmodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/copt/knapsack.py` & `pyepo-0.3.7/pyepo/model/copt/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/copt/shortestpath.py` & `pyepo-0.3.7/pyepo/model/copt/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/grb/grbmodel.py` & `pyepo-0.3.7/pyepo/model/grb/grbmodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/grb/knapsack.py` & `pyepo-0.3.7/pyepo/model/grb/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/grb/shortestpath.py` & `pyepo-0.3.7/pyepo/model/grb/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/grb/tsp.py` & `pyepo-0.3.7/pyepo/model/grb/tsp.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/omo/knapsack.py` & `pyepo-0.3.7/pyepo/model/omo/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/omo/omomodel.py` & `pyepo-0.3.7/pyepo/model/omo/omomodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/omo/shortestpath.py` & `pyepo-0.3.7/pyepo/model/omo/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/model/opt.py` & `pyepo-0.3.7/pyepo/model/opt.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/twostage/autosklearnpred.py` & `pyepo-0.3.7/pyepo/twostage/autosklearnpred.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo/utlis.py` & `pyepo-0.3.7/pyepo/utlis.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/pyepo.egg-info/PKG-INFO` & `pyepo-0.3.7/pyepo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepo
-Version: 0.3.6
+Version: 0.3.7
 Summary: PyTorch-based End-to-End Predict-then-Optimize Tool
 Home-page: https://github.com/khalil-research/PyEPO
 Author: Bo Tang
 Author-email: bolucas.tang@mail.utoronto.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyepo-0.3.6/pyepo.egg-info/SOURCES.txt` & `pyepo-0.3.7/pyepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.6/setup.py` & `pyepo-0.3.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # project dir
     packages = setuptools.find_packages(),
     # description
     description = "PyTorch-based End-to-End Predict-then-Optimize Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # version
-    version = "0.3.6",
+    version = "0.3.7",
     # Github repo
     url = "https://github.com/khalil-research/PyEPO",
     # author name
     author = "Bo Tang",
     # mail address
     author_email = "bolucas.tang@mail.utoronto.ca",
     # dependencies
```

