# Comparing `tmp/openbb_alpha_vantage-1.1.4.tar.gz` & `tmp/openbb_alpha_vantage-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_alpha_vantage-1.1.4.tar", max compression
+gzip compressed data, was "openbb_alpha_vantage-1.1.5.tar", max compression
```

## Comparing `openbb_alpha_vantage-1.1.4.tar` & `openbb_alpha_vantage-1.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      457 2024-02-29 11:03:36.752466 openbb_alpha_vantage-1.1.4/README.md
--rw-r--r--   0        0        0     1106 2024-03-28 12:01:02.099630 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752638 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12446 2024-03-21 17:38:35.636494 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-03-14 12:31:53.175465 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752779 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752842 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2516 2024-03-13 16:36:51.635177 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      493 2024-04-01 14:20:39.029115 openbb_alpha_vantage-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      457 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/README.md
+-rw-r--r--   0        0        0     1106 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12452 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      493 2024-04-19 16:41:41.591292 openbb_alpha_vantage-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.1.5/PKG-INFO
```

### Comparing `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/__init__.py` & `openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/equity_historical.py` & `openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/equity_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,26 +153,26 @@
         if "INTRADAY" in function:
             query_str += f"&interval={interval}&extended_hours={str(query.extended_hours).lower()}"
             intraday = True
 
         results = []
 
         async def callback(response, _):
-            """Callback function to process the response."""
+            """Use callback function to process the response."""
             try:
                 result = await response.json()
                 if "Information" in result:
                     warn(str(result.get("Information")))
             except Exception as _:
                 # TODO: This is hacky, find a better solution.
                 return await response.read()
             return await response.read()
 
         async def intraday_callback(response, _):
-            """Callback function to process the intraday response."""
+            """Use callback function to process the intraday response."""
             symbol = response.url.query.get("symbol", None)
             data = await response.read()
             if data:
                 df = read_csv(BytesIO(data))
                 if len(df) > 0:
                     df.rename(
                         columns={
@@ -185,15 +185,14 @@
                 results.extend(df.to_dict("records"))
             if not data:
                 warn(f"Symbol Error: No data found for {symbol}")
             return results
 
         async def get_one(symbol, intraday: bool = False):
             """Get data for one symbol."""
-
             if intraday is True:
                 adjusted = query.adjustment != "unadjusted"
                 if query.adjustment == "splits_only":
                     warn(
                         "Intraday does not support 'splits_only'. Using 'splits_and_dividends' instead."
                     )
                 url = (
@@ -294,15 +293,14 @@
         return results
 
     @staticmethod
     def transform_data(
         query: AVEquityHistoricalQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[AVEquityHistoricalData]:
         """Transform the data to the standard format."""
-
         if data == []:
             return []
         if "{" in data[0]:
             warn(str(data[0]["{"].strip()))
             return []
         return [
             AVEquityHistoricalData.model_validate(d)
```

### Comparing `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/historical_eps.py` & `openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/utils/helpers.py` & `openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,30 @@
             <= end_date,
             data,
         )
     )
 
 
 def calculate_adjusted_prices(df: pd.DataFrame, column: str, dividends: bool = False):
-    """Calculates the split-adjusted prices, or split and dividend adjusted prices.
+    """Calculate the split-adjusted prices, or split and dividend adjusted prices.
 
     Parameters
-    ------------
+    ----------
     df: pd.DataFrame
         DataFrame with unadjusted OHLCV values + split_factor + dividend
     column: str
         The column name to adjust.
     dividends: bool
         Whether to adjust for both splits and dividends. Default is split-adjusted only.
 
     Returns
-    --------
+    -------
     pd.DataFrame
         DataFrame with adjusted prices.
     """
-
     df = df.copy()
     adj_column = "adj_" + column
 
     # Reverse the DataFrame order, sorting by date in descending order
     df.sort_index(ascending=False, inplace=True)
 
     price_col = df[column].values
```

### Comparing `openbb_alpha_vantage-1.1.4/PKG-INFO` & `openbb_alpha_vantage-1.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-alpha-vantage
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alpha Vantage extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Alpha Vantage Provider
 
 This extension integrates the [Alpha Vantage](https://www.alphavantage.co/) data provider into the OpenBB Platform.
 
 ## Installation
```

