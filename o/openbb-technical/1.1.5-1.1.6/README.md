# Comparing `tmp/openbb_technical-1.1.5.tar.gz` & `tmp/openbb_technical-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_technical-1.1.5.tar", max compression
+gzip compressed data, was "openbb_technical-1.1.6.tar", max compression
```

## Comparing `openbb_technical-1.1.5.tar` & `openbb_technical-1.1.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      605 2024-02-29 11:03:36.743618 openbb_technical-1.1.5/README.md
--rw-r--r--   0        0        0       43 2024-02-29 11:03:36.744125 openbb_technical-1.1.5/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16751 2024-03-18 09:35:41.446222 openbb_technical-1.1.5/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.744320 openbb_technical-1.1.5/openbb_technical/py.typed
--rw-r--r--   0        0        0    57417 2024-03-25 15:07:22.155086 openbb_technical-1.1.5/openbb_technical/technical_router.py
--rw-r--r--   0        0        0      614 2024-04-01 14:19:25.552681 openbb_technical-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 openbb_technical-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      605 2024-04-17 12:33:20.505645 openbb_technical-1.1.6/README.md
+-rw-r--r--   0        0        0       43 2024-04-17 12:33:20.505645 openbb_technical-1.1.6/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-04-19 16:31:25.534563 openbb_technical-1.1.6/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.505645 openbb_technical-1.1.6/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-04-19 16:31:25.534563 openbb_technical-1.1.6/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    64220 2024-04-19 16:31:25.534563 openbb_technical-1.1.6/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0      614 2024-04-19 16:40:37.463144 openbb_technical-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 openbb_technical-1.1.6/PKG-INFO
```

### Comparing `openbb_technical-1.1.5/README.md` & `openbb_technical-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openbb_technical-1.1.5/openbb_technical/helpers.py` & `openbb_technical-1.1.6/openbb_technical/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Technical Analysis Helpers."""
 
-import warnings
 from typing import Any, List, Literal, Optional, Tuple, Union
+from warnings import warn
 
 import numpy as np
 import pandas as pd
 
-_warn = warnings.warn
-
 
 def validate_data(data: list, length: Union[int, List[int]]) -> None:
     """Validate data."""
     if isinstance(length, int):
         length = [length]
     for item in length:
         if item > len(data):
@@ -47,19 +45,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 1:
-        _warn("Error: Window must be at least 1, defaulting to 30.")
+        warn("Error: Window must be at least 1, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     rs = (1.0 / (4.0 * np.log(2.0))) * (
         (data["high"] / data["low"]).apply(np.log)
     ) ** 2.0
@@ -78,15 +76,15 @@
 def standard_deviation(
     data: pd.DataFrame,
     window: int = 30,
     trading_periods: Optional[int] = None,
     is_crypto: bool = False,
     clean: bool = True,
 ) -> pd.DataFrame:
-    """Standard deviation.
+    """Calculate the Standard deviation.
 
     Measures how widely returns are dispersed from the average return.
     It is the most common (and biased) estimator of volatility.
 
     Parameters
     ----------
     data : pd.DataFrame
@@ -102,19 +100,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 2:
-        _warn("Error: Window must be at least 2, defaulting to 30.")
+        warn("Error: Window must be at least 2, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_return = (data["close"] / data["close"].shift(1)).apply(np.log)
 
     result = log_return.rolling(window=window, center=False).std() * np.sqrt(
@@ -155,19 +153,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 1:
-        _warn("Error: Window must be at least 1, defaulting to 30.")
+        warn("Error: Window must be at least 1, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_hl = (data["high"] / data["low"]).apply(np.log)
     log_co = (data["close"] / data["open"]).apply(np.log)
 
@@ -216,19 +214,19 @@
 
     Example
     -------
     >>> data = obb.equity.price.historical('BTC-USD')
     >>> df = obb.technical.hodges_tompkins(data, is_crypto = True)
     """
     if window < 2:
-        _warn("Error: Window must be at least 2, defaulting to 30.")
+        warn("Error: Window must be at least 2, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_return = (data["close"] / data["close"].shift(1)).apply(np.log)
 
     vol = log_return.rolling(window=window, center=False).std() * np.sqrt(
@@ -276,19 +274,19 @@
 
     Returns
     -------
     pd.Series : results
         Pandas Series with results.
     """
     if window < 1:
-        _warn("Error: Window must be at least 1, defaulting to 30.")
+        warn("Error: Window must be at least 1, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_ho = (data["high"] / data["open"]).apply(np.log)
     log_lo = (data["low"] / data["open"]).apply(np.log)
     log_co = (data["close"] / data["open"]).apply(np.log)
@@ -333,19 +331,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 2:
-        _warn("Error: Window must be at least 2, defaulting to 30.")
+        warn("Error: Window must be at least 2, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_ho = (data["high"] / data["open"]).apply(np.log)
     log_lo = (data["low"] / data["open"]).apply(np.log)
     log_co = (data["close"] / data["open"]).apply(np.log)
@@ -543,20 +541,20 @@
     """
     if close_col not in data.columns:
         raise ValueError(f"Column {close_col} not in data")
 
     if start_date and end_date:
         if start_date not in data.index:
             date0 = data.index[data.index.get_indexer([end_date], method="nearest")[0]]
-            _warn(f"Start date not in data.  Using nearest: {date0}")
+            warn(f"Start date not in data.  Using nearest: {date0}")
         else:
             date0 = start_date
         if end_date not in data.index:
             date1 = data.index[data.index.get_indexer([end_date], method="nearest")[0]]
-            _warn(f"End date not in data.  Using nearest: {date1}")
+            warn(f"End date not in data.  Using nearest: {date1}")
         else:
             date1 = end_date
 
         data0 = data.loc[date0, close_col]
         data1 = data.loc[date1, close_col]
 
         min_pr = min(data0, data1)
```

### Comparing `openbb_technical-1.1.5/openbb_technical/technical_router.py` & `openbb_technical-1.1.6/openbb_technical/technical_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Technical Analysis Router."""
 
 # pylint: disable=too-many-lines
-from typing import List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional
 
 import pandas as pd
 import pandas_ta as ta
 from openbb_core.app.model.example import APIEx, PythonEx
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.router import Router
 from openbb_core.app.utils import (
@@ -13,23 +13,165 @@
     df_to_basemodel,
     get_target_column,
     get_target_columns,
 )
 from openbb_core.provider.abstract.data import Data
 from pydantic import NonNegativeFloat, NonNegativeInt, PositiveFloat, PositiveInt
 
-from .helpers import (
+from openbb_technical.helpers import (
     calculate_cones,
     calculate_fib_levels,
     clenow_momentum,
     validate_data,
 )
+from openbb_technical.relative_rotation import (
+    RelativeRotationData,
+    RelativeRotationFetcher,
+    RelativeRotationQueryParams,
+)
 
 # TODO: Split this into multiple files
-router = Router(prefix="")
+router = Router(prefix="", description="Technical Analysis tools.")
+
+
+@router.command(
+    methods=["POST"],
+    examples=[
+        PythonEx(
+            description="Calculate the Relative Strength Ratio and Relative Strength Momentum"
+            + " for a group of symbols against a benchmark.",
+            code=[
+                "stock_data = obb.equity.price.historical("
+                + "symbol='AAPL,MSFT,GOOGL,META,AMZN,TSLA,SPY', start_date='2022-01-01', provider='yfinance')",
+                "rr_data = obb.technical.relative_rotation(data=stock_data.results, benchmark='SPY')",
+                "rs_ratios = rr_data.results.rs_ratios",
+                "rs_momentum = rr_data.results.rs_momentum",
+            ],
+        ),
+        PythonEx(
+            description="When the assets are not traded 252 days per year,"
+            + "adjust the momentum and volatility periods accordingly.",
+            code=[
+                "crypto_data = obb.crypto.price.historical("
+                + " symbol='BTCUSD,ETHUSD,SOLUSD', start_date='2021-01-01', provider='yfinance')",
+                "rr_data = obb.technical.relative_rotation(data=crypto_data.results, benchmark='BTCUSD',"
+                + " long_period=365, short_period=30, window=30, trading_periods=365)",
+            ],
+        ),
+        APIEx(
+            description="Note that the mock data displayed here is insufficient."
+            + " It must contain multiple symbols, with the benchmark, and be daily data at least 1 year in length.",
+            parameters={"benchmark": "SPY", "data": APIEx.mock_data("timeseries")},
+        ),
+    ],
+)
+async def relative_rotation(
+    data: List[Data],
+    benchmark: str,
+    study: Literal["price", "volume", "volatility"] = "price",
+    long_period: Optional[int] = 252,
+    short_period: Optional[int] = 21,
+    window: Optional[int] = 21,
+    trading_periods: Optional[int] = 252,
+    chart_params: Optional[Dict[str, Any]] = None,
+) -> OBBject[RelativeRotationData]:
+    """Calculate the Relative Strength Ratio and Relative Strength Momentum for a group of symbols against a benchmark.
+
+    Parameters
+    ----------
+    data : list[Data]
+        The data to be used for the relative rotation calculations.
+        This should be the multi-symbol output from the 'equity.price.historical' endpoint, or similar.
+        Or a pivot table with the 'date' column as the index, the symbols as the columns, and the 'study' as the values.
+        It is recommended to use the 'equity.price.historical' endpoint to get the data, and feed the results as-is.
+    benchmark : str
+        The symbol to be used as the benchmark.
+    study : Literal[price, volume, volatility]
+        The data point for the calculations. If 'price', the closing price will be used.
+        If 'volatility', the standard deviation of the closing price will be used.
+        If 'data' is supplied as a pivot table,
+        the 'study' will assume the values are the closing price and 'volume' will be ignored.
+    long_period : int, optional
+        The length of the long period for momentum calculation, by default 252.
+        Adjust this value when supplying a time series with an interval that is not daily.
+        For example, if the data is monthly, the long period should be 12.
+    short_period : int, optional
+        The length of the short period for momentum calculation, by default 21.
+        Adjust this value when supplying a time series with an interval that is not daily.
+    window : int, optional
+        The length of window for the standard deviation calculation, by default 21.
+        Adjust this value when supplying a time series with an interval that is not daily.
+    trading_periods : int, optional
+        The number of trading periods per year, for the standard deviation calculation, by default 252.
+        Adjust this value when supplying a time series with an interval that is not daily.
+    chart_params : dict[str, Any], optional
+        Additional parameters to pass when `chart=True` and the `openbb-charting` extension is installed.
+        Parameters can be passed again to redraw the chart using the charting.to_chart() method of the response.
+
+        ChartParams
+        -----------
+        date : str, optional
+            A target end date within the data to use for the chart, by default is the last date in the data.
+        show_tails : bool
+            Show the tails on the chart, by default True.
+        tail_periods : int
+            Number of periods to show in the tails, by default 16.
+        tail_interval : Literal[day, week, month]
+            Interval to show the tails, by default 'week'.
+        title : str, optional
+            Title of the chart.
+
+    Returns
+    -------
+    OBBject[RelativeRotationData]
+        results : RelativeRotationData
+            symbols : list[str]:
+                The symbols that are being compared against the benchmark.
+            benchmark : str
+                The benchmark symbol.
+            study : Literal[price, volume, volatility]
+                The data point for the selected.
+            long_period : int
+                The length of the long period for momentum calculation, as entered by the user.
+            short_period : int
+                The length of the short period for momentum calculation, as entered by the user.
+            window : int
+                The length of window for the standard deviation calculation.
+            trading_periods : int
+                The number of trading periods per year, for the standard deviation calculation.
+            start_date : str
+                The start date of the data after adjusting the length of the data for the calculations.
+            end_date : str
+                The end date of the data.
+            symbols_data : list[Data]
+                The data representing the selected 'study' for each symbol.
+            benchmark_data : list[Data]
+                The data representing the selected 'study' for the benchmark.
+            rs_ratios : list[Data]
+                The normalized relative strength ratios data.
+            rs_momentum : list[Data]
+                The normalized relative strength momentum data.
+    """
+
+    params = RelativeRotationQueryParams(
+        data=data,
+        benchmark=benchmark,
+        study=study,
+        long_period=long_period,
+        short_period=short_period,
+        window=window,
+        trading_periods=trading_periods,
+        chart_params=chart_params,
+    )
+
+    return OBBject(
+        results=RelativeRotationFetcher.transform_data(
+            params, RelativeRotationFetcher.extract_data(params, {})
+        )
+    )
 
 
 @router.command(
     methods=["POST"],
     examples=[
         PythonEx(
             description="Get the Average True Range.",
@@ -485,15 +627,15 @@
         APIEx(parameters={"length": 2, "data": APIEx.mock_data("timeseries")}),
     ],
 )
 def aroon(
     data: List[Data],
     index: str = "date",
     length: int = 25,
-    scalar: int = 100,
+    scalar: float = 100,
 ) -> OBBject[List[Data]]:
     """Calculate the Aroon Indicator.
 
     The word aroon is Sanskrit for "dawn's early light." The Aroon
     indicator attempts to show when a new trend is dawning. The indicator consists
     of two lines (Up and Down) that measure how long it has been since the highest
     high/lowest low has occurred within an n period range.
@@ -509,15 +651,15 @@
     ----------
     data : List[Data]
         List of data to be used for the calculation.
     index: str, optional
         Index column name to use with `data`, by default "date".
     length : int, optional
         Number of periods to be used for the calculation, by default 25.
-    scalar : int, optional
+    scalar : float, optional
         Scalar to be used for the calculation, by default 100.
 
     Returns
     -------
     OBBject[List[Data]]
         The calculated data.
     """
```

### Comparing `openbb_technical-1.1.5/pyproject.toml` & `openbb_technical-1.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "openbb-technical"
-version = "1.1.5"
+version = "1.1.6"
 description = "Technical Analysis extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_technical" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"  # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 scikit-learn = "^1.3.1"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.1.5"
+openbb-core = "^1.1.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 technical = "openbb_technical.technical_router:router"
```

### Comparing `openbb_technical-1.1.5/PKG-INFO` & `openbb_technical-1.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-technical
-Version: 1.1.5
+Version: 1.1.6
 Summary: Technical Analysis extension for OpenBB
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
 Requires-Dist: scikit-learn (>=1.3.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Technical Analysis Extension
```

