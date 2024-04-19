# Comparing `tmp/empulse-0.3.0.tar.gz` & `tmp/empulse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empulse-0.3.0.tar", last modified: Thu Apr 18 11:00:48 2024, max compression
+gzip compressed data, was "empulse-0.3.1.tar", last modified: Fri Apr 19 16:53:56 2024, max compression
```

## Comparing `empulse-0.3.0.tar` & `empulse-0.3.1.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.096900 empulse-0.3.0/
--rw-rw-rw-   0        0        0     2807 2024-04-18 08:30:25.000000 empulse-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     6974 2024-04-18 11:00:48.095199 empulse-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2024-04-18 08:30:25.000000 empulse-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.015143 empulse-0.3.0/empulse/
--rw-rw-rw-   0        0        0       23 2024-04-18 09:16:39.000000 empulse-0.3.0/empulse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.062199 empulse-0.3.0/empulse/metrics/
--rw-rw-rw-   0        0        0      417 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/__init__.py
--rw-rw-rw-   0        0        0     2355 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/_convex_hull.py
--rw-rw-rw-   0        0        0     2516 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.066612 empulse-0.3.0/empulse/metrics/acquisition/
--rw-rw-rw-   0        0        0      333 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/acquisition/__init__.py
--rw-rw-rw-   0        0        0     1950 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/acquisition/_validation.py
--rw-rw-rw-   0        0        0     6659 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/acquisition/cost.py
--rw-rw-rw-   0        0        0     7776 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/acquisition/deterministic.py
--rw-rw-rw-   0        0        0    10466 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/acquisition/stochastic.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.071611 empulse-0.3.0/empulse/metrics/churn/
--rw-rw-rw-   0        0        0      355 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/churn/__init__.py
--rw-rw-rw-   0        0        0     3606 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/churn/_validation.py
--rw-rw-rw-   0        0        0     7393 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/churn/cost.py
--rw-rw-rw-   0        0        0     9176 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/churn/deterministic.py
--rw-rw-rw-   0        0        0    18722 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/churn/stochastic.py
--rw-rw-rw-   0        0        0     4371 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/common.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.077612 empulse-0.3.0/empulse/metrics/credit_scoring/
--rw-rw-rw-   0        0        0      232 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/credit_scoring/__init__.py
--rw-rw-rw-   0        0        0     1039 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/credit_scoring/_validation.py
--rw-rw-rw-   0        0        0     6437 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/credit_scoring/deterministic.py
--rw-rw-rw-   0        0        0     9399 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/credit_scoring/stochastic.py
--rw-rw-rw-   0        0        0    13798 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/emp.py
--rw-rw-rw-   0        0        0     1717 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/lift.py
--rw-rw-rw-   0        0        0     5270 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/metrics/mp.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.085640 empulse-0.3.0/empulse/models/
--rw-rw-rw-   0        0        0      249 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/models/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/models/_wrapper.py
--rw-rw-rw-   0        0        0     9645 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/models/b2boost.py
--rw-rw-rw-   0        0        0     2928 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/models/bias_relabeling.py
--rw-rw-rw-   0        0        0     2856 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/models/bias_resampling.py
--rw-rw-rw-   0        0        0     4333 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/models/bias_reweighing.py
--rw-rw-rw-   0        0        0    10872 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/models/proflogit.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.089250 empulse-0.3.0/empulse/optimizers/
--rw-rw-rw-   0        0        0       70 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/optimizers/__init__.py
--rw-rw-rw-   0        0        0    12791 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/optimizers/generation.py
--rw-rw-rw-   0        0        0      225 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/optimizers/optimizer.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.093197 empulse-0.3.0/empulse/samplers/
--rw-rw-rw-   0        0        0       84 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/samplers/__init__.py
--rw-rw-rw-   0        0        0     1234 2024-04-18 08:30:25.000000 empulse-0.3.0/empulse/samplers/_strategies.py
--rw-rw-rw-   0        0        0     5492 2024-04-18 09:53:46.000000 empulse-0.3.0/empulse/samplers/bias_relabler.py
--rw-rw-rw-   0        0        0     4261 2024-04-18 10:57:32.000000 empulse-0.3.0/empulse/samplers/bias_resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:48.055197 empulse-0.3.0/empulse.egg-info/
--rw-rw-rw-   0        0        0     6974 2024-04-18 11:00:47.000000 empulse-0.3.0/empulse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2024-04-18 11:00:47.000000 empulse-0.3.0/empulse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:00:47.000000 empulse-0.3.0/empulse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2024-04-18 11:00:47.000000 empulse-0.3.0/empulse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 11:00:47.000000 empulse-0.3.0/empulse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1969 2024-04-18 09:16:39.000000 empulse-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 11:00:48.097226 empulse-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-04-18 08:30:25.000000 empulse-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.725226 empulse-0.3.1/
+-rw-rw-rw-   0        0        0     2807 2024-04-18 08:30:25.000000 empulse-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6974 2024-04-19 16:53:56.723241 empulse-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2024-04-18 08:30:25.000000 empulse-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.302262 empulse-0.3.1/empulse/
+-rw-rw-rw-   0        0        0       23 2024-04-19 16:51:54.000000 empulse-0.3.1/empulse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.416829 empulse-0.3.1/empulse/metrics/
+-rw-rw-rw-   0        0        0      417 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2355 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/_convex_hull.py
+-rw-rw-rw-   0        0        0     2516 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.472688 empulse-0.3.1/empulse/metrics/acquisition/
+-rw-rw-rw-   0        0        0      333 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/acquisition/__init__.py
+-rw-rw-rw-   0        0        0     1950 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/acquisition/_validation.py
+-rw-rw-rw-   0        0        0     6659 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/acquisition/cost.py
+-rw-rw-rw-   0        0        0     7776 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/acquisition/deterministic.py
+-rw-rw-rw-   0        0        0    10466 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/acquisition/stochastic.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.527214 empulse-0.3.1/empulse/metrics/churn/
+-rw-rw-rw-   0        0        0      355 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/churn/__init__.py
+-rw-rw-rw-   0        0        0     3606 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/churn/_validation.py
+-rw-rw-rw-   0        0        0     7393 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/churn/cost.py
+-rw-rw-rw-   0        0        0     9176 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/churn/deterministic.py
+-rw-rw-rw-   0        0        0    18722 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/churn/stochastic.py
+-rw-rw-rw-   0        0        0     4371 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/common.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.566878 empulse-0.3.1/empulse/metrics/credit_scoring/
+-rw-rw-rw-   0        0        0      232 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/credit_scoring/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/credit_scoring/_validation.py
+-rw-rw-rw-   0        0        0     6437 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/credit_scoring/deterministic.py
+-rw-rw-rw-   0        0        0     9399 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/credit_scoring/stochastic.py
+-rw-rw-rw-   0        0        0    13798 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/emp.py
+-rw-rw-rw-   0        0        0     1717 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/lift.py
+-rw-rw-rw-   0        0        0     5270 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/metrics/mp.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.651375 empulse-0.3.1/empulse/models/
+-rw-rw-rw-   0        0        0      249 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/models/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/models/_wrapper.py
+-rw-rw-rw-   0        0        0     9645 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/models/b2boost.py
+-rw-rw-rw-   0        0        0     7490 2024-04-19 16:45:09.000000 empulse-0.3.1/empulse/models/bias_relabeling.py
+-rw-rw-rw-   0        0        0     7646 2024-04-19 16:45:09.000000 empulse-0.3.1/empulse/models/bias_resampling.py
+-rw-rw-rw-   0        0        0     8732 2024-04-19 16:45:09.000000 empulse-0.3.1/empulse/models/bias_reweighing.py
+-rw-rw-rw-   0        0        0    10872 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/models/proflogit.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.680271 empulse-0.3.1/empulse/optimizers/
+-rw-rw-rw-   0        0        0       36 2024-04-19 16:05:16.000000 empulse-0.3.1/empulse/optimizers/__init__.py
+-rw-rw-rw-   0        0        0    12745 2024-04-19 16:06:16.000000 empulse-0.3.1/empulse/optimizers/generation.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.720134 empulse-0.3.1/empulse/samplers/
+-rw-rw-rw-   0        0        0       84 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/samplers/__init__.py
+-rw-rw-rw-   0        0        0     1234 2024-04-18 08:30:25.000000 empulse-0.3.1/empulse/samplers/_strategies.py
+-rw-rw-rw-   0        0        0     5965 2024-04-19 16:45:09.000000 empulse-0.3.1/empulse/samplers/bias_relabler.py
+-rw-rw-rw-   0        0        0     4968 2024-04-19 16:45:09.000000 empulse-0.3.1/empulse/samplers/bias_resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:53:56.344667 empulse-0.3.1/empulse.egg-info/
+-rw-rw-rw-   0        0        0     6974 2024-04-19 16:53:56.000000 empulse-0.3.1/empulse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1369 2024-04-19 16:53:56.000000 empulse-0.3.1/empulse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 16:53:56.000000 empulse-0.3.1/empulse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      291 2024-04-19 16:53:56.000000 empulse-0.3.1/empulse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-19 16:53:56.000000 empulse-0.3.1/empulse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1969 2024-04-19 16:51:54.000000 empulse-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 16:53:56.725853 empulse-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2024-04-18 08:30:25.000000 empulse-0.3.1/setup.py
```

### Comparing `empulse-0.3.0/LICENSE` & `empulse-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/PKG-INFO` & `empulse-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empulse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Value-driven metrics and models for scikit-learn
 Author-email: Shimanto Rahman <shimanto.rahman@ugent.be>
 License: MIT License
         
         Copyright (c) 2023 Shimanto Rahman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `empulse-0.3.0/README.md` & `empulse-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/_convex_hull.py` & `empulse-0.3.1/empulse/metrics/_convex_hull.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/_validation.py` & `empulse-0.3.1/empulse/metrics/_validation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/acquisition/_validation.py` & `empulse-0.3.1/empulse/metrics/acquisition/_validation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/acquisition/cost.py` & `empulse-0.3.1/empulse/metrics/acquisition/cost.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/acquisition/deterministic.py` & `empulse-0.3.1/empulse/metrics/acquisition/deterministic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/acquisition/stochastic.py` & `empulse-0.3.1/empulse/metrics/acquisition/stochastic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/churn/_validation.py` & `empulse-0.3.1/empulse/metrics/churn/_validation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/churn/cost.py` & `empulse-0.3.1/empulse/metrics/churn/cost.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/churn/deterministic.py` & `empulse-0.3.1/empulse/metrics/churn/deterministic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/churn/stochastic.py` & `empulse-0.3.1/empulse/metrics/churn/stochastic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/common.py` & `empulse-0.3.1/empulse/metrics/common.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/credit_scoring/_validation.py` & `empulse-0.3.1/empulse/metrics/credit_scoring/_validation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/credit_scoring/deterministic.py` & `empulse-0.3.1/empulse/metrics/credit_scoring/deterministic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/credit_scoring/stochastic.py` & `empulse-0.3.1/empulse/metrics/credit_scoring/stochastic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/emp.py` & `empulse-0.3.1/empulse/metrics/emp.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/lift.py` & `empulse-0.3.1/empulse/metrics/lift.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/metrics/mp.py` & `empulse-0.3.1/empulse/metrics/mp.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/models/_wrapper.py` & `empulse-0.3.1/empulse/models/_wrapper.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/models/b2boost.py` & `empulse-0.3.1/empulse/models/b2boost.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/models/bias_reweighing.py` & `empulse-0.3.1/empulse/samplers/bias_resampler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,118 @@
-from typing import Callable, Union, Optional
 from itertools import product
+from typing import Union, Callable, Optional, TypeVar
 
 import numpy as np
 from numpy.typing import ArrayLike
-from sklearn.base import ClassifierMixin, BaseEstimator, clone
+from sklearn.base import OneToOneFeatureMixin, BaseEstimator
+from sklearn.utils import check_random_state, _safe_indexing
 
-from ..samplers._strategies import _independent_weights, Strategy, StrategyFn
-from ._wrapper import WrapperMixin
+from ._strategies import _independent_weights, Strategy, StrategyFn
 
+_XT = TypeVar('_XT', bound=ArrayLike)
+_YT = TypeVar('_YT', bound=ArrayLike)
 
-def _to_sample_weights(group_weights: np.ndarray, y_true: np.ndarray, protected_attr: np.ndarray):
-    """Convert group weights to sample weights."""
-    sample_weight = np.empty(len(y_true))
-    for target_class, protected_val in product(np.unique(y_true), np.unique(protected_attr)):
-        protected_val = int(protected_val)
-        idx_class = np.flatnonzero(y_true == target_class)
-        idx_prot_attr = np.flatnonzero(protected_attr == protected_val)
-        idx_class_prot = np.intersect1d(idx_class, idx_prot_attr)
-        sample_weight[idx_class_prot] = group_weights[target_class, protected_val]
-    return sample_weight / np.max(sample_weight)
 
-
-def _independent_sample_weights(y_true: np.ndarray, protected_attr: np.ndarray) -> np.ndarray:
-    group_weights = _independent_weights(y_true, protected_attr)
-    return _to_sample_weights(group_weights, y_true, protected_attr)
-
-
-class BiasReweighingClassifier(BaseEstimator, ClassifierMixin, WrapperMixin):
+class BiasResampler(OneToOneFeatureMixin, BaseEstimator):
     """
-    Classifier which reweighs instances during training to remove bias against a subgroup.
+    Sampler which resamples instances to remove bias against a subgroup
 
     Parameters
     ----------
-    estimator : Estimator instance
-        Base estimator which is used for fitting and predicting.
-        Base estimator must accept `sample_weight` as an argument in its `fit` method.
-    strategy : Literal or Callable, default = 'statistical parity'
-        Function which computes the sample weights based on the target and protected attribute.
-        .. note::
-            Sample weights should be normalized to fall between 0 and 1.
-        if ``Literal`` sample weights are computed so:
-            - `'statistical_parity'` or `'demographic parity'`: probability of positive predictions
-            are equal between subgroups of protected attribute.
-            - other strategies coming in future versions.
-    transform_attr : Optional[Callable], default = None
-        Function which transforms protected attribute before computing sample weights.
+   strategy : {'statistical parity', 'demographic parity'} or Callable, default='statistical parity'
+        Determines how the group weights are computed.
+        Group weights determine how much to over or undersample each combination of target and protected attribute.
+        For example, a weight of 2 for the pair (y_true == 1, protected_attr == 0) means that the resampled dataset
+        should have twice as many instances with y_true == 1 and protected_attr == 0 compared to the original dataset.
+
+        - ``'statistical_parity'`` or ``'demographic parity'``: \
+        probability of positive predictions are equal between subgroups of protected attribute.
+
+        - ``Callable``: function which computes the group weights based on the target and protected attribute. \
+        Callable accepts two arguments: y_true and protected_attr and returns the group weights. \
+        Group weights are a 2x2 matrix where the rows represent the target variable and the columns represent the \
+        protected attribute. \
+        The element at position (i, j) is the weight for the pair (y_true == i, protected_attr == j).
+    transform_attr : Optional[Callable], default=None
+        Function which transforms protected attribute before resampling the training data.
     """
+    _estimator_type = "sampler"
 
     strategy_mapping: dict[str, StrategyFn] = {
-        'statistical parity': _independent_sample_weights,
-        'demographic parity': _independent_sample_weights,
+        'statistical parity': _independent_weights,
+        'demographic parity': _independent_weights,
     }
 
     def __init__(
             self,
-            estimator,
             *,
-            strategy: Union[StrategyFn, Strategy] = 'statistical parity',
-            transform_attr: Optional[Callable[[np.ndarray], np.ndarray]] = None
+            strategy: Union[Callable, Strategy] = 'statistical parity',
+            transform_attr: Optional[Callable] = None,
+            random_state=None
     ):
-        self.estimator = estimator
+        if isinstance(strategy, str):
+            strategy = self.strategy_mapping[strategy]
         self.strategy = strategy
         self.transform_attr = transform_attr
+        self.random_state = check_random_state(random_state)
+        self.sample_indices_ = None
 
-    def fit(
+    def fit_resample(
             self,
-            X: ArrayLike,
-            y: ArrayLike,
+            X: _XT,
+            y: _YT,
             *,
             protected_attr: Optional[ArrayLike] = None,
-            **fit_params
-    ) -> 'BiasReweighingClassifier':
+    ) -> tuple[_XT, _YT]:
         """
-        Fit the estimator and reweigh the instances according to the strategy.
+        Resample the data according to the strategy.
+
         Parameters
         ----------
         X : ArrayLike
             Training data.
         y : ArrayLike
             Target values.
         protected_attr : Optional[ArrayLike]
-            Protected attribute used to determine the sample weights.
-        fit_params : dict
-            Additional parameters passed to the estimator's `fit` method.
+            Protected attribute used to determine the number of promotion and demotion pairs.
 
         Returns
         -------
-        self : BiasReweighingClassifier
+        X : ArrayLike
+            Resampled training data.
+        y : np.ndarray
+            Resampled target values.
         """
-        X, y = np.asarray(X), np.asarray(y)
         if protected_attr is None:
-            self.estimator.fit(X, y, **fit_params)
-            return self
-        protected_attr = np.asarray(protected_attr)
-
-        if isinstance(self.strategy, str):
-            strategy_fn = self.strategy_mapping[self.strategy]
-        else:
-            strategy_fn = self.strategy
+            return X, y
 
         if self.transform_attr is not None:
             protected_attr = self.transform_attr(protected_attr)
 
-        sample_weights = strategy_fn(y, protected_attr)
-        self.estimator = clone(self.estimator)
-        self.estimator.fit(X, y, sample_weight=sample_weights, **fit_params)
+        class_weights = self.strategy(y, protected_attr)
+        # if class_weights are all 1, no resampling is needed
+        if np.allclose(class_weights, np.ones(class_weights.shape)):
+            return X, y
+        indices = np.empty((0,), dtype=int)
+
+        # determine the number of samples to be drawn for each class and protected attribute value
+        for target_class, protected_val in product(np.unique(y), np.unique(protected_attr)):
+            protected_val = int(protected_val)
+            idx_class = np.flatnonzero(y == target_class)
+            idx_protected_attr = np.flatnonzero(protected_attr == protected_val)
+            idx_class_prot = np.intersect1d(idx_class, idx_protected_attr)
+            n_samples = int(class_weights[target_class, protected_val] * len(idx_class_prot))
+            if n_samples > len(idx_class_prot):  # oversampling
+                indices = np.concatenate((indices, idx_class_prot))
+                indices = np.concatenate((
+                    indices,
+                    self.random_state.choice(idx_class_prot, n_samples - len(idx_class_prot), replace=True)
+                ))
+            else:  # undersampling
+                indices = np.concatenate((
+                    indices,
+                    self.random_state.choice(idx_class_prot, n_samples, replace=False)
+                ))
 
-        return self
+        self.sample_indices_ = indices
 
+        return _safe_indexing(X, indices), _safe_indexing(y, indices)
```

### Comparing `empulse-0.3.0/empulse/models/proflogit.py` & `empulse-0.3.1/empulse/models/proflogit.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/optimizers/generation.py` & `empulse-0.3.1/empulse/optimizers/generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 from typing import Optional, Callable, Generator
 
 import numpy as np
 from joblib import Parallel, delayed
 from scipy.optimize import OptimizeResult
 from sklearn.utils import check_random_state
 
-from empulse.optimizers import Optimizer
 
-
-class Generation(Optimizer):
+class Generation:
     """
-    Generation of a Real-coded Genetic Algorithm (RGA)
+    A single generation of a Real-coded Genetic Algorithm (RGA)
 
     Parameters
     ----------
     population_size : int or None, default=None
         Number of individuals in the population.
         If ``None``, population size is set to ``10 * n_dim``.
```

### Comparing `empulse-0.3.0/empulse/samplers/_strategies.py` & `empulse-0.3.1/empulse/samplers/_strategies.py`

 * *Files identical despite different names*

### Comparing `empulse-0.3.0/empulse/samplers/bias_relabler.py` & `empulse-0.3.1/empulse/samplers/bias_relabler.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,28 +28,34 @@
 
     # number of pairs to swap label
     return abs(round((discrimination * n_protected * n_unprotected) / n))
 
 
 class BiasRelabler(OneToOneFeatureMixin, BaseEstimator):
     """
-    Sampler which relabels instances to remove bias against a subgroup.
+    Sampler which relabels instances to remove bias against a subgroup
 
     Parameters
     ----------
     estimator : Estimator instance
         Base estimator which is used to determine the number of promotion and demotion pairs.
-    strategy : Literal or Callable, default = 'statistical parity'
-        Function which computes the group weights based on the target and protected attribute.
-        if ``Literal`` group weights are computed so:
-            - `'statistical_parity'` or `'demographic parity'`: probability of positive predictions
-            are equal between subgroups of protected attribute.
-            - other strategies coming in future versions.
-    transform_attr : Optional[Callable], default = None
-        Function which transforms protected attribute before computing sample weights.
+    strategy : {'statistical parity', 'demographic parity'} or Callable, default='statistical parity'
+        Determines how the group weights are computed.
+        Group weights determine how many instances to relabel for each combination of target and protected attribute.
+
+        - ``'statistical_parity'`` or ``'demographic parity'``: \
+        probability of positive predictions are equal between subgroups of protected attribute.
+
+        - ``Callable``: function which computes the group weights based on the target and protected attribute. \
+        Callable accepts two arguments: y_true and protected_attr and returns the group weights. \
+        Group weights are a 2x2 matrix where the rows represent the target variable and the columns represent the \
+        protected attribute. \
+        The element at position (i, j) is the weight for the pair (y_true == i, protected_attr == j).
+    transform_attr : Optional[Callable], default=None
+        Function which transforms protected attribute before resampling the training data.
     """
     _estimator_type = "sampler"
 
     strategy_mapping: dict[str, StrategyFn] = {
         'statistical parity': _independent_pairs,
         'demographic parity': _independent_pairs,
     }
@@ -72,22 +78,24 @@
             X: _XT,
             y: ArrayLike,
             *,
             protected_attr: Optional[ArrayLike] = None
     ) -> tuple[_XT, np.ndarray]:
         """
         Fit the estimator and relabel the data according to the strategy.
+
         Parameters
         ----------
         X : ArrayLike
             Training data.
         y : ArrayLike
             Target values.
         protected_attr : Optional[ArrayLike]
             Protected attribute used to determine the number of promotion and demotion pairs.
+
         Returns
         -------
         X : ArrayLike
             Training data.
         y : np.ndarray
             Relabeled target values.
         """
```

### Comparing `empulse-0.3.0/empulse.egg-info/PKG-INFO` & `empulse-0.3.1/empulse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empulse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Value-driven metrics and models for scikit-learn
 Author-email: Shimanto Rahman <shimanto.rahman@ugent.be>
 License: MIT License
         
         Copyright (c) 2023 Shimanto Rahman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `empulse-0.3.0/empulse.egg-info/SOURCES.txt` & `empulse-0.3.1/empulse.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,12 +34,11 @@
 empulse/models/b2boost.py
 empulse/models/bias_relabeling.py
 empulse/models/bias_resampling.py
 empulse/models/bias_reweighing.py
 empulse/models/proflogit.py
 empulse/optimizers/__init__.py
 empulse/optimizers/generation.py
-empulse/optimizers/optimizer.py
 empulse/samplers/__init__.py
 empulse/samplers/_strategies.py
 empulse/samplers/bias_relabler.py
 empulse/samplers/bias_resampler.py
```

### Comparing `empulse-0.3.0/pyproject.toml` & `empulse-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "empulse"
-version = "0.3.0"
+version = "0.3.1"
 description = "Value-driven metrics and models for scikit-learn"
 readme = "README.md"
 authors = [
     { name = "Shimanto Rahman", email = "shimanto.rahman@ugent.be" },
 ]
 license = { file = "LICENSE" }
```

