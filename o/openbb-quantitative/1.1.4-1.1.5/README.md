# Comparing `tmp/openbb_quantitative-1.1.4.tar.gz` & `tmp/openbb_quantitative-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_quantitative-1.1.4.tar", max compression
+gzip compressed data, was "openbb_quantitative-1.1.5.tar", max compression
```

## Comparing `openbb_quantitative-1.1.4.tar` & `openbb_quantitative-1.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      594 2024-02-29 11:03:36.741365 openbb_quantitative-1.1.4/README.md
--rw-r--r--   0        0        0       59 2024-02-29 11:03:36.741757 openbb_quantitative-1.1.4/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-03-13 16:36:51.579826 openbb_quantitative-1.1.4/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-03-13 16:36:51.579940 openbb_quantitative-1.1.4/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8610 2024-03-13 16:36:51.580310 openbb_quantitative-1.1.4/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.741954 openbb_quantitative-1.1.4/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10087 2024-03-13 16:36:51.580703 openbb_quantitative-1.1.4/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14280 2024-03-14 20:24:16.776370 openbb_quantitative-1.1.4/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1313 2024-03-13 16:36:51.581064 openbb_quantitative-1.1.4/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10975 2024-03-14 20:24:16.776513 openbb_quantitative-1.1.4/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0      609 2024-04-01 14:17:08.589820 openbb_quantitative-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 openbb_quantitative-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/README.md
+-rw-r--r--   0        0        0       59 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-04-17 12:33:20.501645 openbb_quantitative-1.1.5/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0      609 2024-04-19 16:40:07.535080 openbb_quantitative-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 openbb_quantitative-1.1.5/PKG-INFO
```

### Comparing `openbb_quantitative-1.1.4/README.md` & `openbb_quantitative-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 This extension works nicely with a companion `openbb-charting` extension
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
-pip install openbb-qa
+pip install openbb-quantitative
 ```
 
 For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
 
 Documentation available [here](https://docs.openbb.co/platform).
```

### Comparing `openbb_quantitative-1.1.4/openbb_quantitative/helpers.py` & `openbb_quantitative-1.1.5/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.1.4/openbb_quantitative/models.py` & `openbb_quantitative-1.1.5/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.1.4/openbb_quantitative/performance/performance_router.py` & `openbb_quantitative-1.1.5/openbb_quantitative/performance/performance_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""OpenBB Performance Extension router."""
+
 from typing import List
 
 import numpy as np
 import pandas as pd
 from openbb_core.app.model.example import APIEx, PythonEx
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.router import Router
```

### Comparing `openbb_quantitative-1.1.4/openbb_quantitative/quantitative_router.py` & `openbb_quantitative-1.1.5/openbb_quantitative/quantitative_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     KPSSTestModel,
     NormalityModel,
     SummaryModel,
     TestModel,
     UnitRootModel,
 )
 
-router = Router(prefix="")
+router = Router(prefix="", description="Quantitative analysis tools.")
 router.include_router(rolling_router)
 router.include_router(stats_router)
 router.include_router(performance_router)
 
 
 @router.command(
     methods=["POST"],
```

### Comparing `openbb_quantitative-1.1.4/openbb_quantitative/rolling/rolling_router.py` & `openbb_quantitative-1.1.5/openbb_quantitative/rolling/rolling_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,16 +372,15 @@
             }
         ),
     ],
 )
 def mean(
     data: List[Data], target: str, window: PositiveInt = 21, index: str = "date"
 ) -> OBBject[List[Data]]:
-    """
-    Calculate the rolling mean (average) of a target column within a given window size.
+    """Calculate the rolling average of a target column within a given window size.
 
     The rolling mean is a simple moving average that calculates the average of a target variable over a specified window.
     This function is widely used in financial analysis to smooth short-term fluctuations and highlight longer-term trends
     or cycles in time series data.
 
     Parameters
     ----------
```

### Comparing `openbb_quantitative-1.1.4/openbb_quantitative/statistics.py` & `openbb_quantitative-1.1.5/openbb_quantitative/statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Statistics Functions"""
+"""Statistics Functions."""
 
 from typing import Union
 
 from numpy import (
     mean as mean_np,
     ndarray,
     std,
@@ -12,30 +12,36 @@
 from scipy import stats
 
 # Because python is weird and these being the same name as the fastapi router functions
 # which overwrites the function signature, we add the _ after the function name
 
 
 def kurtosis_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Kurtosis is a measure of the "tailedness" of the probability distribution of a real-valued random variable."""
+    """Get Kurtosis.
+
+    It is a measure of the "tailedness" of the probability distribution of a real-valued random variable.
+    """
     return stats.kurtosis(data)
 
 
 def skew_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Skewness is a measure of the asymmetry of the probability distribution of a
-    real-valued random variable about its mean."""
+    """Get Skewness.
+
+    It is a measure of the asymmetry of the probability distribution of a
+    real-valued random variable about its mean.
+    """
     return stats.skew(data)
 
 
 def mean_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Mean is the average of the numbers."""
+    """Get Mean which is the average of the numbers."""
     return mean_np(data)
 
 
 def std_dev_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Standard deviation is a measure of the amount of variation or dispersion of a set of values."""
+    """Get Standard deviation that is a measure of the amount of variation or dispersion of a set of values."""
     return std(data)
 
 
 def var_(data: Union[DataFrame, Series, ndarray]) -> float:
-    """Variance is a measure of the amount of variation or dispersion of a set of values."""
+    """Get Variance that is a measure of the amount of variation or dispersion of a set of values."""
     return var_np(data)
```

### Comparing `openbb_quantitative-1.1.4/openbb_quantitative/stats/stats_router.py` & `openbb_quantitative-1.1.5/openbb_quantitative/stats/stats_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,15 @@
                     sample={"date": "2023-01-01", "close": 0.05},
                 ),
             }
         ),
     ],
 )
 def variance(data: List[Data], target: str) -> OBBject[List[Data]]:
-    """
-    Calculate the  variance of a target column.
+    """Calculate the  variance of a target column.
 
     Variance measures the dispersion of a set of data points around their mean. It is a key metric for
     assessing the volatility and stability of financial returns or other time series data.
 
     Parameters
     ----------
     data: List[Data]
@@ -146,16 +145,15 @@
                     sample={"date": "2023-01-01", "close": 0.05},
                 ),
             }
         ),
     ],
 )
 def stdev(data: List[Data], target: str) -> OBBject[List[Data]]:
-    """
-    Calculate the rolling standard deviation of a target column.
+    """Calculate the rolling standard deviation of a target column.
 
     Standard deviation is a measure of the amount of variation or dispersion of a set of values.
     It is widely used to assess the risk and volatility of financial returns or other time series data
     It is the square root of the variance.
 
     Parameters
     ----------
@@ -196,16 +194,15 @@
                     sample={"date": "2023-01-01", "close": 0.05},
                 ),
             }
         ),
     ],
 )
 def kurtosis(data: List[Data], target: str) -> OBBject[List[Data]]:
-    """
-    Calculate the rolling kurtosis of a target column.
+    """Calculate the rolling kurtosis of a target column.
 
     Kurtosis measures the "tailedness" of the probability distribution of a real-valued random variable.
     High kurtosis indicates a distribution with heavy tails (outliers), suggesting a higher risk of extreme outcomes.
     Low kurtosis indicates a distribution with lighter tails (less outliers), suggesting less risk of extreme outcomes.
     This function helps in assessing the risk of outliers in financial returns or other time series data.
 
     Parameters
@@ -251,16 +248,15 @@
     ],
 )
 def quantile(
     data: List[Data],
     target: str,
     quantile_pct: NonNegativeFloat = 0.5,
 ) -> OBBject[List[Data]]:
-    """
-    Calculate the quantile of a target column at a specified quantile percentage.
+    """Calculate the quantile of a target column at a specified quantile percentage.
 
     Quantiles are points dividing the range of a probability distribution into  intervals with equal probabilities,
     or dividing the  sample in the same way.
 
     Parameters
     ----------
     data: List[Data]
@@ -308,16 +304,15 @@
         ),
     ],
 )
 def mean(
     data: List[Data],
     target: str,
 ) -> OBBject[List[Data]]:
-    """
-    Calculate the  mean (average) of a target column.
+    """Calculate the average of a target column.
 
     The rolling mean is a simple moving average that calculates the average of a target variable.
     This function is widely used in financial analysis to smooth short-term fluctuations and highlight longer-term trends
     or cycles in time series data.
 
     Parameters
     ----------
```

### Comparing `openbb_quantitative-1.1.4/pyproject.toml` & `openbb_quantitative-1.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "openbb-quantitative"
-version = "1.1.4"
+version = "1.1.5"
 description = "Quantitative Analysis extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_quantitative" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"   # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.1.5"
+openbb-core = "^1.1.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 quantitative = "openbb_quantitative.quantitative_router:router"
```

### Comparing `openbb_quantitative-1.1.4/PKG-INFO` & `openbb_quantitative-1.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-quantitative
-Version: 1.1.4
+Version: 1.1.5
 Summary: Quantitative Analysis extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # OpenBB QA Extension
 
@@ -25,14 +25,14 @@
 This extension works nicely with a companion `openbb-charting` extension
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
-pip install openbb-qa
+pip install openbb-quantitative
 ```
 
 For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
 
 Documentation available [here](https://docs.openbb.co/platform).
```

