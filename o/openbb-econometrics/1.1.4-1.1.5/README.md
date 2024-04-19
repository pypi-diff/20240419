# Comparing `tmp/openbb_econometrics-1.1.4.tar.gz` & `tmp/openbb_econometrics-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_econometrics-1.1.4.tar", max compression
+gzip compressed data, was "openbb_econometrics-1.1.5.tar", max compression
```

## Comparing `openbb_econometrics-1.1.4.tar` & `openbb_econometrics-1.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      448 2024-02-29 11:03:36.733012 openbb_econometrics-1.1.4/README.md
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.733220 openbb_econometrics-1.1.4/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28108 2024-03-14 20:24:16.775321 openbb_econometrics-1.1.4/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.733411 openbb_econometrics-1.1.4/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4036 2024-02-29 11:03:36.733509 openbb_econometrics-1.1.4/openbb_econometrics/utils.py
--rw-r--r--   0        0        0      689 2024-04-01 14:18:35.488207 openbb_econometrics-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 openbb_econometrics-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      448 2024-04-17 12:33:20.497645 openbb_econometrics-1.1.5/README.md
+-rw-r--r--   0        0        0       37 2024-04-17 12:33:20.497645 openbb_econometrics-1.1.5/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-04-17 12:33:20.497645 openbb_econometrics-1.1.5/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.497645 openbb_econometrics-1.1.5/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-04-17 12:33:20.501645 openbb_econometrics-1.1.5/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0      689 2024-04-19 16:39:23.874992 openbb_econometrics-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 openbb_econometrics-1.1.5/PKG-INFO
```

### Comparing `openbb_econometrics-1.1.4/openbb_econometrics/econometrics_router.py` & `openbb_econometrics-1.1.5/openbb_econometrics/econometrics_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pydantic import PositiveInt
 from statsmodels.stats.diagnostic import acorr_breusch_godfrey  # type: ignore
 from statsmodels.stats.stattools import durbin_watson  # type: ignore
 from statsmodels.tsa.stattools import adfuller, grangercausalitytests  # type: ignore
 
 from openbb_econometrics.utils import get_engle_granger_two_step_cointegration_test
 
-router = Router(prefix="")
+router = Router(prefix="", description="Econometrics analysis tools.")
 
 
 @router.command(
     methods=["POST"],
     examples=[
         PythonEx(
             description="Get the correlation matrix of a dataset.",
```

### Comparing `openbb_econometrics-1.1.4/openbb_econometrics/utils.py` & `openbb_econometrics-1.1.5/openbb_econometrics/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Utility functions for the econometrics extension of the OpenBB platform."""
+
 import warnings
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
 from statsmodels.tsa.stattools import adfuller
 
 
 def get_engle_granger_two_step_cointegration_test(
     dependent_series: pd.Series, independent_series: pd.Series
 ) -> Tuple[float, float, float, pd.Series, float, float]:
-    """Estimates long-run and short-run cointegration relationship for series y and x and apply
-    the two-step Engle & Granger test for cointegration.
+    """Estimate long-run and short-run cointegration relationship for series y and x.
+
+    Then apply the two-step Engle & Granger test for cointegration.
 
     Uses a 2-step process to first estimate coefficients for the long-run relationship
         y_t = c + gamma * x_t + z_t
 
     and then the short-term relationship,
         y_t - y_(t-1) = alpha * z_(t-1) + epsilon_t,
 
@@ -83,15 +86,15 @@
 
     adfstat, pvalue, _, _, _ = adfuller(z, maxlag=1, autolag=None)
 
     return c, gamma, alpha, z, adfstat, pvalue
 
 
 def mock_multi_index_data():
-    """Creates a mock multi-index dataframe for testing purposes."""
+    """Create a mock multi-index dataframe for testing purposes."""
     arrays = [
         ["individual_" + str(i) for i in range(1, 11) for _ in range(5)],
         list(range(1, 6)) * 10,
     ]
     index = pd.MultiIndex.from_arrays(arrays, names=("individual", "time"))
 
     df = pd.DataFrame(
```

### Comparing `openbb_econometrics-1.1.4/pyproject.toml` & `openbb_econometrics-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "openbb-econometrics"
-version = "1.1.4"
+version = "1.1.5"
 description = "Econometrics Toolkit for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_econometrics" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"                 # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 arch = "^5.5.0"
 linearmodels = "<=4.25"                # ^4.26 has setuptools-scm in setup_requires
-openbb-core = "^1.1.5"
+openbb-core = "^1.1.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 econometrics = "openbb_econometrics.econometrics_router:router"
```

### Comparing `openbb_econometrics-1.1.4/PKG-INFO` & `openbb_econometrics-1.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-econometrics
-Version: 1.1.4
+Version: 1.1.5
 Summary: Econometrics Toolkit for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arch (>=5.5.0,<6.0.0)
 Requires-Dist: linearmodels (<=4.25)
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # Econometrics extension for OpenBB Platform
 
 This extension provides a set of econometrics tools.
```

