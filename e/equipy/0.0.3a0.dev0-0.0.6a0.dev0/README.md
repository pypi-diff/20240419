# Comparing `tmp/equipy-0.0.3a0.dev0.tar.gz` & `tmp/equipy-0.0.6a0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equipy-0.0.3a0.dev0.tar", last modified: Wed Dec  6 20:22:15 2023, max compression
+gzip compressed data, was "equipy-0.0.6a0.dev0.tar", last modified: Fri Apr 19 12:17:22 2024, max compression
```

## Comparing `equipy-0.0.3a0.dev0.tar` & `equipy-0.0.6a0.dev0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.211196 equipy-0.0.3a0.dev0/equipy/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/equipy/fairness/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/fairness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/fairness/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12004 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/fairness/_wasserstein.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/equipy/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/graphs/_arrow_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/graphs/_density_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/graphs/_waterfall_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/equipy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/metrics/_fairness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/metrics/_performance_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/equipy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/utils/checkers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/equipy/utils/permutations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/utils/permutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/utils/permutations/_compute_permutations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/equipy/utils/permutations/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/utils/permutations/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/utils/permutations/metrics/_fairness_permutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/equipy/utils/permutations/metrics/_performance_permutations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/equipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-06 20:22:15.000000 equipy-0.0.3a0.dev0/equipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-12-06 20:22:15.000000 equipy-0.0.3a0.dev0/equipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 20:22:15.000000 equipy-0.0.3a0.dev0/equipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-06 20:22:15.000000 equipy-0.0.3a0.dev0/equipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-06 20:22:15.000000 equipy-0.0.3a0.dev0/equipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 20:22:15.215196 equipy-0.0.3a0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-12-06 20:21:43.000000 equipy-0.0.3a0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy/fairness/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/fairness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/fairness/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19415 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/fairness/_wasserstein.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/graphs/_arrow_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/graphs/_density_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/graphs/_waterfall_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/metrics/_fairness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/metrics/_performance_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/utils/checkers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy/utils/permutations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/utils/permutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/utils/permutations/_compute_permutations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy/utils/permutations/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/utils/permutations/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/utils/permutations/metrics/_fairness_permutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/equipy/utils/permutations/metrics/_performance_permutations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/equipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-19 12:17:22.000000 equipy-0.0.6a0.dev0/equipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 12:17:22.000000 equipy-0.0.6a0.dev0/equipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:17:22.000000 equipy-0.0.6a0.dev0/equipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 12:17:22.000000 equipy-0.0.6a0.dev0/equipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 12:17:22.000000 equipy-0.0.6a0.dev0/equipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:17:22.976440 equipy-0.0.6a0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-19 12:16:55.000000 equipy-0.0.6a0.dev0/setup.py
```

### Comparing `equipy-0.0.3a0.dev0/LICENSE` & `equipy-0.0.6a0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `equipy-0.0.3a0.dev0/equipy/fairness/_base.py` & `equipy-0.0.6a0.dev0/equipy/fairness/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,138 +1,132 @@
+"""
+Base class containing all necessary calculations to make predictions fair.
+"""
+
+# Authors: Agathe F, Suzie G, Francois H, Philipp R, Arthur C
+# License: BSD 3 clause
 from statsmodels.distributions.empirical_distribution import ECDF
 import numpy as np
+import pandas as pd
 from ..metrics._fairness_metrics import EQF
 
+
 class BaseHelper():
     """
     Base class providing helper methods for Wasserstein distance-based fairness adjustment.
 
     Attributes
     ----------
     ecdf : dict
         Dictionary storing ECDF (Empirical Cumulative Distribution Function) objects for each sensitive modality.
     eqf : dict
         Dictionary storing EQF (Empirical Quantile Function) objects for each sensitive modality.
 
-    Methods
-    -------
-    _get_modalities(sensitive_feature)
-        Get unique modalities from the input sensitive attribute array.
-    _get_location_modalities(sensitive_feature)
-        Get the indices of occurrences for each modality in the input sensitive attribute array.
-    _get_weights(sensitive_feature)
-        Calculate weights (probabilities) for each modality based on their occurrences.
-    _estimate_ecdf_eqf(y, sensitive_feature, sigma)
-        Estimate ECDF and EQF for each modality, incorporating random noise within [-sigma, sigma].
-    _get_correction(self, weights, mod, y_with_noise, location_modalities, modalities_test)
-        Calculate correction of y.
-    _fair_y_values(self, y, modalities_test, location_modalities, weights)
-        Apply fairness correction to input values.
-
     Notes
     -----
     This base class provides essential methods for Wasserstein distance-based fairness adjustment. It includes
     methods for modality extraction, localization of modalities in the input data, weight calculation, and ECDF/EQF 
     estimation with random noise.
     """
 
     def __init__(self):
         self.ecdf = {}
         self.eqf = {}
 
         self.weights = {}
 
-    def _get_modalities(self, sensitive_feature):
+    def _get_modalities(self, sensitive_feature: pd.DataFrame) -> set:
         """
-        Get unique modalities from the input sensitive attribute array.
+        Get unique modalities from the input sensitive attribute DataFrame.
 
         Parameters
         ----------
-        sensitive_feature : array-like, shape (n_samples,)
+        sensitive_feature : pandas DataFrame, shape (n_samples, 1)
             Input samples representing the sensitive attributes.
 
         Returns
         -------
-        list
-            List of unique modalities present in the input sensitive attribute array.
+        set
+            Set of modalities present in the input sensitive attribute array.
         """
-        return set(sensitive_feature)
+        return set(sensitive_feature.iloc[:, 0])
 
-    def _get_location_modalities(self, sensitive_feature):
+    def _get_location_modalities(self, sensitive_feature: pd.DataFrame) -> dict[str, np.ndarray]:
         """
         Get the indices of occurrences for each modality in the input sensitive attribute array.
 
         Parameters
         ----------
-        sensitive_feature : array-like, shape (n_samples,)
+        sensitive_feature : pd.DataFrame, shape (n_samples, 1)
             Input sample representing the sensitive attribute.
 
         Returns
         -------
         dict
             Dictionary where keys are modalities and values are arrays containing their indices.
         """
         location_modalities = {}
         for modality in self._get_modalities(sensitive_feature):
             location_modalities[modality] = np.where(
                 sensitive_feature == modality)[0]
         return location_modalities
 
-    def _compute_weights(self, sensitive_feature):
+    def _compute_weights(self, sensitive_feature: pd.DataFrame) -> dict[str, float]:
         """
         Calculate weights (probabilities) for each modality based on their occurrences.
 
         Parameters
         ----------
-        sensitive_feature : array-like, shape (n_samples,)
+        sensitive_feature : pd.DataFrame, shape (n_samples, 1)
             Input samples representing the sensitive attribute.
 
         Returns
         -------
         dict
             Dictionary where keys are modalities and values are their corresponding weights.
         """
         location_modalities = self._get_location_modalities(sensitive_feature)
         for modality in self._get_modalities(sensitive_feature):
             self.weights[modality] = len(
                 location_modalities[modality])/len(sensitive_feature)
+        return self.weights
 
-    def _estimate_ecdf_eqf(self, y, sensitive_feature, sigma):
+    def _estimate_ecdf_eqf(self, y: np.ndarray, sensitive_feature: pd.DataFrame, sigma: float) -> tuple[dict[str, float]]:
         """
         Estimate ECDF and EQF for each modality, incorporating random noise within [-sigma, sigma].
 
         Parameters
         ----------
         y : array-like, shape (n_samples,)
             Target values corresponding to the sensitive attribute array.
-        sensitive_feature : array-like, shape (n_samples,)
+        sensitive_feature : pd.DataFrame, shape (n_samples, 1)
             Input samples representing the sensitive attribute.
         sigma : float
             Standard deviation of the random noise added to the data.
 
         Returns
         -------
-        None
+        dict, dict
+            Dictionaries where keys are sensitive features and values are their ecdf and eqf.
         """
         location_modalities = self._get_location_modalities(sensitive_feature)
         eps = np.random.uniform(-sigma, sigma, len(y))
         for modality in self._get_modalities(sensitive_feature):
             self.ecdf[modality] = ECDF(y[location_modalities[modality]] +
                                        eps[location_modalities[modality]])
             self.eqf[modality] = EQF(
                 y[location_modalities[modality]]+eps[location_modalities[modality]])
+        return self.ecdf, self.eqf
 
-    def _get_correction(self, mod, y_with_noise, location_modalities, modalities_test):
+    def _get_correction(self, mod: str, y_with_noise: np.ndarray, location_modalities: dict[str, np.ndarray], modalities_test: set) -> float:
         """
         Calculate correction of y.
 
         Parameters
         ----------
-        weights : dict
-            A dictionary of weights for each modality.
         mod : str
             The current modality for which the correction is calculated.
         y_with_noise : np.ndarray
             y plus a random noise.
         location_modalities : dict
             A dictionary mapping modalities to their locations.
         modalities_test : set
@@ -145,28 +139,26 @@
         """
         correction = 0
         for _mod in modalities_test:
             correction += self.weights[_mod] * self.eqf[_mod](
                 self.ecdf[mod](y_with_noise[location_modalities[mod]]))
         return correction
 
-    def _fair_y_values(self, y, sensitive_feature, modalities_test):
+    def _fair_y_values(self, y: np.ndarray, sensitive_feature: pd.DataFrame, modalities_test: list) -> np.ndarray:
         """
         Apply fairness correction to input values.
 
         Parameters
         ----------
         y : np.ndarray
             Input values.
-        sensitive_features : np.ndarray, shape (n_samples, n_sensitive_features)
-            The test samples representing multiple sensitive attributes.
+        sensitive_features : pd.DataFrame, shape (n_samples, 1)
+            The test samples representing a single sensitive attribute.
         modalities_test : list
             List of modalities for correction.
-        weights : dict
-            A dictionary of weights for each modality.
 
         Returns
         -------
         np.ndarray
             Fair values after applying correction.
         """
         location_modalities = self._get_location_modalities(sensitive_feature)
```

### Comparing `equipy-0.0.3a0.dev0/equipy/metrics/_fairness_metrics.py` & `equipy-0.0.6a0.dev0/equipy/metrics/_fairness_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-from matplotlib.collections import EventCollection
+"""
+Computation of the fairness (i.e. measurement of the similarity in prediction distribution between
+different population groups according to their sensitive attributes).
+"""
+
+# Authors: Agathe F, Suzie G, Francois H, Philipp R, Arthur C
+# License: BSD 3 clause
 import numpy as np
-from sklearn.metrics import accuracy_score, mean_squared_error
 import warnings
 from scipy.interpolate import interp1d
 import numpy as np
-import ot
+from typing import Union
+import pandas as pd
 
-# WARNING:You cannot calculate the EQF function of a single value : this means that if only one individual
-# has a specific sensitive value, you cannot use the transform function.
+# WARNING:You cannot calculate the EQF function of a single value : this means that if
+# only one individual has a specific sensitive value, you cannot use the transform function.
 
 
 class EQF:
     """
     Empirical Quantile Function (EQF) Class.
 
-    This class computes the linear interpolation of the empirical quantile function for a given set of sample data.
+    This class computes the linear interpolation of the empirical quantile function for a given set
+    of sample data.
 
     Parameters
     ----------
     sample_data : array-like
         A 1-D array or list-like object containing the sample data.
 
     Attributes
@@ -35,48 +42,38 @@
     __init__(sample_data)
         Initializes the EQF object by calculating the interpolater, min_val, and max_val.
     _calculate_eqf(sample_data)
         Private method to calculate interpolater, min_val, and max_val.
     __call__(value_)
         Callable method to compute the interpolated value for a given quantile.
 
-    Example usage
-    -------------
-    >>> sample_data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
-    >>> eqf = EQF(sample_data)
-    >>> print(eqf(0.5))  # Interpolated value at quantile 0.5
-    5.5
+    Raises
+    ------
+    ValueError
+        If the input value_ is outside the range [0, 1].
 
-    Example usage
-    -------------
+    Example 
+    -------
     >>> sample_data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
     >>> eqf = EQF(sample_data)
     >>> print(eqf([0.2, 0.5, 0.8]))  # Interpolated value at quantiles 0.2, 0.5, and 0.8
     [2.8 5.5 8.2]
 
-
-    Raises
-    ------
-    ValueError
-        If the input value_ is outside the range [0, 1].
-
     Note
     ----
     - The EQF interpolates values within the range [0, 1] representing quantiles.
     - The input sample_data should be a list or array-like containing numerical values.
     """
 
-    def __init__(self,
-                 sample_data,
-                 ):
+    def __init__(self, sample_data: Union[np.ndarray, list[float]]):
         self._calculate_eqf(sample_data)
         if len(sample_data) == 1:
             warnings.warn('One of your sample data contains a single value')
 
-    def _calculate_eqf(self, sample_data):
+    def _calculate_eqf(self, sample_data: Union[np.ndarray, list[float]]) -> None:
         """
         Calculate the Empirical Quantile Function for the given sample data.
 
         Parameters
         ----------
         sample_data : array-like
             A 1-D array or list-like object containing the sample data.
@@ -101,15 +98,15 @@
 
         else:
             self.interpolater = interp1d(linspace, sorted_data)
 
         self.min_val = sorted_data[0]
         self.max_val = sorted_data[-1]
 
-    def __call__(self, value_):
+    def __call__(self, value_: float) -> float:
         """
         Compute the interpolated value for a given quantile.
 
         Parameters
         ----------
         value_ : float
             Array of quantile values between 0 and 1.
@@ -136,139 +133,150 @@
             elif np.any(value_ < 0) or np.any(value_ > 1):
                 raise ValueError(
                     'value_ should contain only numbers between 0 and 1')
             else:
                 raise ValueError('Error with input value')
 
 
-def diff_quantile(data1, data2, n_min=1000):
+def diff_quantile(data1: np.ndarray,
+                  data2: np.ndarray,
+                  approximate=True) -> float:
     """
-    Compute the unfairness between two populations based on their quantile functions. 
-    If the number of points in data1 is less than n_min, compute the Wasserstein distance using the POT package. 
-    Otherwise, determine unfairness as the maximum difference in quantiles between the two populations.
+    Compute the unfairness between two populations based on their quantile functions. If the option
+    approximate is set to False, compute the compute the Wasserstein distance using the POT package 
+    which requires an install. Else, determine unfairness as the maximum difference in quantiles
+    between the two populations.
 
     Parameters
     ----------
-    data1 : array-like
+    data1 : np.ndarray
         The first set of data points.
-    data2 : array-like
+    data2 : np.ndarray
         The second set of data points.
-    n_min : float
-        Below this threshold, compute the Wasserstein distance.
+    approximate : bool
+        if False, compute distance using optimal transport map, else use quantile approximation
 
     Returns
     -------
     float
         The unfairness value between the two populations.
 
     Example
     -------
     >>> data1 = np.array([5, 2, 4, 6, 1])
     >>> data2 = np.array([9, 6, 4, 7, 6])
     >>> diff = compute_unfairness(data1, data2, n_min=5)
     >>> print(diff)
     3.9797979797979797
     """
+    if approximate:
+        probs = np.linspace(0.01, 0.99, num=100)
+        eqf1 = np.quantile(data1, probs)
+        eqf2 = np.quantile(data2, probs)
+        unfair_value = np.max(np.abs(eqf1-eqf2))
+    else:
+        try:
+            import ot
+        except ModuleNotFoundError:
+            print('POT not installed, install before using'\
+                  'approximate=False option')
+        except Exception as e:
+            print(f"Unexpected {e=}, {type(e)=}")
+            raise
 
-    n1 = len(data1)  # data1 corresponds to y
-    n2 = len(data2)
-
-    if n1 < n_min:
+        n1 = len(data1)  # data1 corresponds to y
+        n2 = len(data2)
         # weights of each point of the two distributions
         a, b = np.ones((n1,)) / n1, np.ones((n2,)) / n2
         M = ot.dist(data1.reshape((n1, 1)), data2.reshape((n2, 1)),
                     metric='euclidean')  # euclidian distance matrix
         M = M/M.max()
         unfair_value = ot.emd2(a, b, M)
 
-    else:
-        probs = np.linspace(0.01, 0.99, num=100)
-        eqf1 = np.quantile(data1, probs)
-        eqf2 = np.quantile(data2, probs)
-        unfair_value = np.max(np.abs(eqf1-eqf2))
-
     return unfair_value
 
 
-def unfairness(y, sensitive_features, n_min=1000):
+def unfairness(y: np.ndarray, sensitive_features: pd.DataFrame, n_min: float = 1000) -> float:
     """
-    Compute the unfairness value for a given fair output (y) and multiple sensitive attributes data (sensitive_features) containing several modalities.
-    If there is a single sensitive feature, it calculates the maximum quantile difference between different modalities of that single sensitive feature.
-    If there are multiple sensitive features, it calculates the maximum quantile difference for each sensitive feature
-    and then takes the maximum of these maximums.
+    Compute the unfairness value for a given fair output (y) and multiple sensitive attributes data
+    (sensitive_features) containing several modalities. If there is a single sensitive feature,
+    it calculates the maximum quantile difference between different modalities of that single
+    sensitive feature. If there are multiple sensitive features, it calculates the maximum quantile
+    difference for each sensitive feature and then takes the sum of these maximums.
 
     Parameters
     ----------
-    y : array-like
+    y : np.ndarray
         Predicted (fair or not) output data.
-    sensitive_features : array-like
+    sensitive_features : pd.DataFrame
         Sensitive attribute data.
     n_min : float
         Below this threshold, compute the unfairness based on the Wasserstein distance.
 
     Returns
     -------
     float
         Unfairness value in the dataset.
 
     Example
     -------
     >>> y = np.array([5, 0, 6, 7, 9])
-    >>> sensitive_features = np.array([[1, 2, 1, 1, 2], [0, 1, 2, 1, 0]]).T
-    >>> unf = compute_unfairness(y, sensitive_features, n_min=5)
+    >>> sensitive_features = pd.DataFrame({'color': ['red', 'blue', 'green', 'blue'],
+                                           'nb_child': [1, 2, 0, 2]})
+    >>> unf = unfairness(y, sensitive_features, n_min=5)
     >>> print(unf)
     6.0
     """
     new_list = []
-    if sensitive_features.ndim == 1:
-        modalities = list(set(sensitive_features))
+    for col in sensitive_features.columns:
+        sensitive_feature = sensitive_features[col]
+        modalities = list(sensitive_feature.unique())
         lst_unfairness = []
         for modality in modalities:
-            y_modality = y[sensitive_features == modality]
+            y_modality = y[sensitive_feature == modality]
             lst_unfairness.append(diff_quantile(y, y_modality, n_min))
         new_list.append(max(lst_unfairness))
-    else:
-        for sensitive_feature in sensitive_features.T:
-            modalities = list(set(sensitive_feature))
-            lst_unfairness = []
-            for modality in modalities:
-                y_modality = y[sensitive_feature == modality]
-                lst_unfairness.append(diff_quantile(y, y_modality, n_min))
-            new_list.append(max(lst_unfairness))
-    return max(new_list)
+    unfs = np.sum(new_list)
+    return unfs
 
 
-def unfairness_dict(y_fair_dict, sensitive_features, n_min=1000):
+def unfairness_dict(y_fair_dict: dict[str, np.ndarray],
+                    sensitive_features: pd.DataFrame,
+                    n_min: float = 1000) -> dict[str, float]:
     """
-    Compute unfairness values for sequentially fair output datasets and multiple sensitive attributes datasets.
+    Compute unfairness values for sequentially fair output datasets and multiple sensitive
+    attributes datasets.
 
     Parameters
     ----------
     y_fair_dict : dict
         A dictionary where keys represent sensitive features and values are arrays
         containing the fair predictions corresponding to each sensitive feature.
         Each sensitive feature's fairness adjustment is performed sequentially,
         ensuring that each feature is treated fairly relative to the previous ones.
-    sensitive_features : array-like
+    sensitive_features : pd.DataFrame
         Sensitive attribute data.
     n_min : float
         Below this threshold, compute the unfairness based on the Wasserstein distance.
 
     Returns
     -------
     dict
         A dictionary containing unfairness values for each level of fairness.
-        The level of fairness corresponds to the number of sensitive attributes to which fairness has been applied.
+        The level of fairness corresponds to the number of sensitive attributes to which 
+        fairness has been applied.
 
     Example
     -------
-    >>> y_fair_dict = {'Base model':np.array([19,39,65]), 'sensitive_feature_1':np.array([22,40,50]), 'sensitive_feature_2':np.array([28,39,42])}
-    >>> sensitive_features = np.array([['blue', 2], ['red', 9], ['green', 5]])
-    >>> unfs_dict = compute_unfairness_multi(y_fair_dict, sensitive_features, n_min=5)
+    >>> y_fair_dict = {'Base model':np.array([19,39,65]), 'color':np.array([22,40,50]),
+                       'nb_child':np.array([28,39,42])}
+    >>> sensitive_features = pd.DataFrame({'color': ['red', 'blue', 'green', 'blue'],
+                                           'nb_child': [1, 2, 0, 2]})
+    >>> unfs_dict = unfairness_dict(y_fair_dict, sensitive_features, n_min=5)
     >>> print(unfs_dict)
-    {'sensitive_feature_0': 46.0, 'sensitive_feature_1': 28.0, 'sensitive_feature_2': 14.0}
+    {'Base model': 46.0, 'color': 28.0, 'nb_child': 14.0}
     """
     unfairness_dict = {}
-    for i, y_fair in enumerate(y_fair_dict.values()):
+    for key, y_fair in y_fair_dict.items():
         result = unfairness(y_fair, sensitive_features, n_min)
-        unfairness_dict[f'sensitive_feature_{i}'] = result
+        unfairness_dict[key] = result
     return unfairness_dict
```

### Comparing `equipy-0.0.3a0.dev0/equipy/utils/checkers.py` & `equipy-0.0.6a0.dev0/equipy/utils/permutations/_compute_permutations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,100 @@
-import numpy as np
-import warnings
-
-def _check_metric(y):
-    """
-    Check that it is regression and not classification.
-
-    Parameters
-    ----------
-    y : array of shape (n_samples,)
-        Observed, true values.
-
-    Raises
-    ------
-    Warning 
-        If it is classification.
-    """
-    if np.all(np.isin(y, [0, 1])):
-        warnings.warn(
-            "You used mean squared error as metric but it looks like you are using classification scores")
-
-
-def _check_nb_observations(sensitive_features):
-    if sensitive_features.ndim == 1 & len(sensitive_features) == 1:
-        raise ValueError("Fairness can't be applied on a single observation")
-    if sensitive_features.ndim == 2 & np.shape(sensitive_features)[1] == 1:
-        raise ValueError("Fairness can't be applied on a single observation")
-
-
-def _check_shape(y, sensitive_feature):
-    """
-    Check the shape and data types of input arrays y and sensitive_feature.
-
-    Parameters
-    ----------
-    y : array-like
-        Target values of the data.
-    sensitive_feature : array-like
-        Input samples representing the sensitive attribute.
-
-    Raises
-    ------
-    ValueError
-        If the input arrays have incorrect shapes or data types.
-    """
-    if not isinstance(sensitive_feature, np.ndarray):
-        raise ValueError('sensitive_features must be an array')
-
-    if not isinstance(y, np.ndarray):
-        raise ValueError('y must be an array')
-
-    if len(sensitive_feature) != len(y):
-        raise ValueError(
-            'sensitive_features and y should have the same length')
-
-    if len(np.unique(sensitive_feature)) == 1:
-        raise ValueError(
-            "At least one of your sensitive attributes contains only one modality and so it is already fair. Remove it from your sensitive features.")
+"""Make predictions fair sequentially with respect to all orders of sensitive variables"""
 
-    if not (np.issubdtype(y.dtype, np.floating) or np.issubdtype(y.dtype, np.integer)):
-        raise ValueError('y should contain only float or integer numbers')
-
-
-def _check_mod(modalities_calib, modalities_test):
-    """
-    Check if modalities in test data are included in calibration data's modalities.
+import itertools
+import numpy as np
+import pandas as pd
 
-    Parameters
-    ----------
-    modalities_calib : list
-        Modalities from the calibration data.
-    modalities_test : list
-        Modalities from the test data.
-
-    Raises
-    ------
-    ValueError
-        If modalities in test data are not present in calibration data.
-    """
-    missing_modalities = set(modalities_test) - set(modalities_calib)
-    if len(missing_modalities) != 0:
-        raise ValueError(
-            f"The following modalities of the test sensitive features are not in modalities of the calibration sensitive features: {missing_modalities}")
+from ...fairness._wasserstein import MultiWasserstein
+from typing import Optional
 
 
-def _check_epsilon(epsilon):
+def permutations_columns(sensitive_features: pd.DataFrame) -> dict[tuple, list]:
     """
-    Check if epsilon (fairness parameter) is within the valid range [0, 1].
+    Generate permutations of columns in the input array sensitive_features.
 
     Parameters
     ----------
-    epsilon : float
-        Fairness parameter controlling the trade-off between fairness and accuracy.
+    sensitive_features : pd.DataFrame, shape (n_samples, n_sensitive_features)
+        Input array where each column represents a different sensitive feature.
 
-    Raises
-    ------
-    ValueError
-        If epsilon is outside the valid range [0, 1].
-    """
-    if epsilon < 0 or epsilon > 1:
-        raise ValueError(
-            'epsilon must be between 0 and 1')
+    Returns
+    -------
+    dict
+        A dictionary where keys are tuples representing permutations of column indices,
+        and values are corresponding permuted pandas dataframes of sensitive features.
+
+    Example
+    -------
+    >>> sensitive_features = [[1, 2], [3, 4], [5, 6]]
+    >>> generate_permutations_cols(sensitive_features)
+    {(1, 2): [[1, 2], [3, 4], [5, 6]], (2, 1): [[3, 4], [1, 2], [5, 6]]}
+
+    Note
+    ----
+    This function generates all possible permutations of columns and stores them in a dictionary.
+    """
+    n = sensitive_features.shape[1]
+    cols = list(sensitive_features.columns)
+    permut_cols = list(itertools.permutations(cols))
+
+    dict_all_combs = {}
+    for permutation in permut_cols:
+        permuted_sensitive_features = sensitive_features[list(permutation)]
+        dict_all_combs[permutation] = permuted_sensitive_features
+    return dict_all_combs
 
 
-def _check_epsilon_size(epsilon, sensitive_features):
+def calculate_perm_wasserstein(y_calib: np.ndarray, sensitive_features_calib: pd.DataFrame, y_test: np.ndarray, sensitive_features_test: pd.DataFrame, epsilon: Optional[list[float]] = None):
     """
-    Check if the epsilon list matches the number of sensitive features.
+    Calculate Wasserstein distance for different permutations of sensitive features between calibration and test sets.
 
     Parameters
     ----------
-    epsilon : list, shape (n_sensitive_features,)
-        Fairness parameters controlling the trade-off between fairness and accuracy for each sensitive feature.
-
-    sensitive_features : array-like, shape (n_samples, n_sensitive_features)
-        Test samples representing multiple sensitive attributes.
-
-    Raises
-    ------
-    ValueError
-        If the length of epsilon does not match the number of sensitive features.
-    """
-
-    if sensitive_features.ndim == 1:
-        if len(epsilon) != 1:
-            raise ValueError(
-                'epsilon must have the same length than the number of sensitive features')
-    else:
-        if len(epsilon) != np.shape(sensitive_features)[1]:
-            raise ValueError(
-                'epsilon must have the same length than the number of sensitive features')
+    y_calib : np.ndarray, shape (n_samples,)
+        Calibration set predictions.
+    sensitive_features_calib : pd.DataFrame, shape (n_samples, n_sensitive_features)
+        Calibration set sensitive features.
+    y_test : np.ndarray, shape (n_samples,)
+        Test set predictions.
+    sensitive_features_test : pd.DataFrame, shape (n_samples, n_sensitive_features)
+        Test set sensitive features.
+    epsilon : np.ndarray, shape (n_sensitive_features,) or None, default= None
+        Fairness constraints.
+
+    Returns
+    -------
+    dict
+        A dictionary where keys are tuples representing permutations of column indices,
+        and values are corresponding sequential fairness values for each permutation.
+
+    Example
+    -------
+    >>> y_calib = [1, 2, 3]
+    >>> sensitive_features_calib = [[1, 2], [3, 4], [5, 6]]
+    >>> y_test = [4, 5, 6]
+    >>> sensitive_features_test = [[7, 8], [9, 10], [11, 12]]
+    >>> calculate_perm_wst(y_calib, sensitive_features_calib, y_test, sensitive_features_test)
+    {(1,2): {'Base model': 0.5, 'sens_var_1': 0.2, 'sens_var_2': 0}, (2, 1): {'Base model': 0.3, 'sens_var_2': 0.6, 'sens_var_1': 0.6}}
+
+    Note
+    ----
+    This function calculates Wasserstein distance for different permutations of sensitive features
+    between calibration and test sets and stores the sequential fairness values in a dictionary.
+    """
+    all_perm_calib = permutations_columns(sensitive_features_calib)
+    all_perm_test = permutations_columns(sensitive_features_test)
+    if epsilon is not None:
+        all_perm_epsilon = permutations_columns(
+            pd.DataFrame([epsilon], columns=sensitive_features_calib.columns))
+
+    store_dict = {}
+    for key in all_perm_calib:
+        wst = MultiWasserstein()
+        wst.fit(y_calib, all_perm_calib[key])
+        if epsilon is None:
+            wst.transform(y_test, all_perm_test[key])
+        else:
+            wst.transform(y_test, all_perm_test[key], 
+                          all_perm_epsilon[key].iloc[0].tolist())
+        store_dict[key] = wst.get_sequential_fairness()
+    return store_dict
```

### Comparing `equipy-0.0.3a0.dev0/equipy/utils/permutations/metrics/_fairness_permutations.py` & `equipy-0.0.6a0.dev0/equipy/utils/permutations/metrics/_fairness_permutations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Calculation of fairness sequentially with respect to all orders of sensitive variables"""
+
 import numpy as np
+import pandas as pd
 
 from ....metrics._fairness_metrics import unfairness_dict
 
 
-def unfairness_permutations(permut_y_fair_dict, all_combs_sensitive_features):
+def unfairness_permutations(permut_y_fair_dict: dict[tuple, dict[str, np.ndarray]], all_combs_sensitive_features: dict[tuple, pd.DataFrame]) -> list[dict[str, float]]:
     """
     Compute unfairness values for multiple fair output datasets and multiple sensitive attribute datasets.
 
     Parameters
     ----------
     permut_y_fair_dict : dict
         A dictionary containing permutations of fair output datasets.
@@ -23,15 +26,15 @@
     -------
     >>> permut_y_fair_dict = {(1,2): {'Base model':np.array([19,39,65]), 'sens_var_1':np.array([22,40,50]), 'sens_var_2':np.array([28,39,42])},
     ...                        (2,1): {'Base model':np.array([19,39,65]), 'sens_var_2':np.array([34,39,60]), 'sens_var_1':np.array([28,39,42])}}
     >>> all_combs_sensitive_features = {(1,2): np.array([['blue', 2], ['red', 9], ['green', 5]]),
     ...                                (2,1): np.array([[2, 'blue'], [9, 'red'], [5, 'green']])}
     >>> unfs_list = compute_unfairness_permutations(permut_y_fair_dict, all_combs_sensitive_features)
     >>> print(unfs_list)
-    [{'sens_var_0': 46.0, 'sens_var_1': 28.0, 'sens_var_2': 14.0}, 
-     {'sens_var_0': 46.0, 'sens_var_1': 26.0, 'sens_var_2': 14.0}]
+    [{'Base model': 46.0, 'sens_var_1': 28.0, 'sens_var_2': 14.0}, 
+     {'Base modem': 46.0, 'sens_var_1': 26.0, 'sens_var_2': 14.0}]
     """
     unfs_list = []
     for key, value in permut_y_fair_dict.items():
         unfs_list.append(unfairness_dict(
-            value, np.array(all_combs_sensitive_features[key])))
+            value, all_combs_sensitive_features[key]))
     return unfs_list
```

### Comparing `equipy-0.0.3a0.dev0/equipy.egg-info/SOURCES.txt` & `equipy-0.0.6a0.dev0/equipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equipy-0.0.3a0.dev0/setup.py` & `equipy-0.0.6a0.dev0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 from setuptools import setup, find_packages
+import json 
+import os
 
-VERSION = "0.0.3-alpha-dev" 
-DESCRIPTION = "Equipy is a tool for fast, online fairness calibration"
+try:
+    with open("versioning/minor_build.json", "r") as f:
+        minor_version = json.load(f)
+except:
+    # for bugfixing
+    print(os.listdir())
+    print(os.getcwd())
+    os.system("cat equipy.egg-info/SOURCES.txt")
 
 with open("README.rst", "r") as f:
     long_description = f.read()
+
+VERSION = f"0.0.{minor_version['buildNumber']}-alpha-dev" 
+DESCRIPTION = "Equipy is a tool for fast, online fairness calibration"
 LONG_DESCRIPTION = long_description
 
 setup(
         name="equipy", 
         version=VERSION,
-        author="Agathe F, Suzie G, Francois H, Philipp R",
+        author="Agathe F, Suzie G, Francois H, Philipp R, Arthur C",
         author_email="nocontact@email.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(include=["equipy", "equipy.*"]),
         install_requires=["numpy", "scipy", "scikit-learn",
                           "matplotlib", "pandas", "statsmodels",
-                          "seaborn", "POT"], 
+                          "seaborn"], 
         setup_requires=["pytest-runner"],
         tests_require=["pytest"],
         keywords=["fairness", "wasserstein"],
         classifiers= [
             "Development Status :: 2 - Pre-Alpha",
             "License :: OSI Approved :: BSD License",
             "Programming Language :: Python :: 3",
```

