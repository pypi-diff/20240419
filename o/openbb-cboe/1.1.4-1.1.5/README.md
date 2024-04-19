# Comparing `tmp/openbb_cboe-1.1.4.tar.gz` & `tmp/openbb_cboe-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_cboe-1.1.4.tar", max compression
+gzip compressed data, was "openbb_cboe-1.1.5.tar", max compression
```

## Comparing `openbb_cboe-1.1.4.tar` & `openbb_cboe-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      423 2024-02-29 11:03:36.757989 openbb_cboe-1.1.4/README.md
--rw-r--r--   0        0        0     1779 2024-03-21 17:38:35.637071 openbb_cboe-1.1.4/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-02-29 11:03:36.758231 openbb_cboe-1.1.4/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-03-21 17:38:35.637199 openbb_cboe-1.1.4/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-03-21 17:38:35.637321 openbb_cboe-1.1.4/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-03-21 17:38:35.637473 openbb_cboe-1.1.4/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-03-21 17:38:35.637646 openbb_cboe-1.1.4/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2154 2024-03-21 17:38:35.637760 openbb_cboe-1.1.4/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-03-21 17:38:35.637910 openbb_cboe-1.1.4/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-03-21 17:38:35.638057 openbb_cboe-1.1.4/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-03-21 17:38:35.638181 openbb_cboe-1.1.4/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-03-13 16:36:51.640860 openbb_cboe-1.1.4/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-03-21 17:38:35.638327 openbb_cboe-1.1.4/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.759328 openbb_cboe-1.1.4/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-02-29 11:03:36.759398 openbb_cboe-1.1.4/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6469 2024-03-13 16:36:51.641162 openbb_cboe-1.1.4/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      494 2024-04-01 14:21:00.514790 openbb_cboe-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 openbb_cboe-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      423 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/README.md
+-rw-r--r--   0        0        0     1779 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-04-19 13:10:31.744034 openbb_cboe-1.1.5/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4725 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     5698 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      494 2024-04-19 16:41:47.231306 openbb_cboe-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 openbb_cboe-1.1.5/PKG-INFO
```

### Comparing `openbb_cboe-1.1.4/openbb_cboe/__init__.py` & `openbb_cboe-1.1.5/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/available_indices.py` & `openbb_cboe-1.1.5/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/equity_historical.py` & `openbb_cboe-1.1.5/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/equity_quote.py` & `openbb_cboe-1.1.5/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/equity_search.py` & `openbb_cboe-1.1.5/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/futures_curve.py` & `openbb_cboe-1.1.5/openbb_cboe/models/futures_curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         List[CboeFuturesCurveData],
     ]
 ):
     """Transform the query, extract and transform the data from the CBOE endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> CboeFuturesCurveQueryParams:
+        """Transform the query."""
         return CboeFuturesCurveQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: CboeFuturesCurveQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the CBOE endpoint."""
-
         symbol = query.symbol.upper().split(",")[0]
         FUTURES = await get_settlement_prices(**kwargs)
         if len(FUTURES) == 0:
             raise EmptyDataError()
 
         if symbol not in FUTURES["product"].unique().tolist():
             raise RuntimeError(
@@ -64,8 +64,9 @@
 
     @staticmethod
     def transform_data(
         query: CboeFuturesCurveQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[CboeFuturesCurveData]:
+        """Transform data."""
         return [CboeFuturesCurveData.model_validate(d) for d in data]
```

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/index_constituents.py` & `openbb_cboe-1.1.5/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/index_historical.py` & `openbb_cboe-1.1.5/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/index_search.py` & `openbb_cboe-1.1.5/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/index_snapshots.py` & `openbb_cboe-1.1.5/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/models/options_chains.py` & `openbb_cboe-1.1.5/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.4/openbb_cboe/utils/helpers.py` & `openbb_cboe-1.1.5/openbb_cboe/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Cboe Helpers"""
+"""Cboe Helpers."""
 
 # pylint: disable=expression-not-assigned, unused-argument
 
 from datetime import date as dateType
 from io import BytesIO, StringIO
 from typing import Any, List, Literal, Optional
 
@@ -77,48 +77,47 @@
 ]
 
 cache_dir = get_user_cache_directory()
 backend = SQLiteBackend(f"{cache_dir}/http/cboe_directories", expire_after=3600 * 24)
 
 
 async def response_callback(response: ClientResponse, _: Any):
-    """Callback for HTTP Client Response."""
+    """Use callback for HTTP Client Response."""
     content_type = response.headers.get("Content-Type", "")
     if "application/json" in content_type:
         return await response.json()
     if "text" in content_type:
         return await response.text()
     return await response.read()
 
 
 async def get_cboe_data(url, use_cache: bool = True, **kwargs) -> Any:
-    """Generic Cboe HTTP request."""
+    """Use the generic Cboe HTTP request."""
     if use_cache is True:
         async with CachedSession(cache=backend) as cached_session:
             try:
                 response = await cached_session.get(url, timeout=10, **kwargs)
                 data = await response_callback(response, None)
             finally:
                 await cached_session.close()
     else:
         data = await amake_request(url, response_callback=response_callback)
 
     return data
 
 
 async def get_company_directory(use_cache: bool = True, **kwargs) -> DataFrame:
-    """
-    Get the US Company Directory for Cboe options. If use_cache is True,
-    the data will be cached for 24 hours.
+    """Get the US Company Directory for Cboe options.
+
+    If use_cache is True, the data will be cached for 24 hours.
 
     Returns
     -------
     DataFrame: Pandas DataFrame of the Cboe listings directory
     """
-
     url = "https://www.cboe.com/us/options/symboldir/equity_index_options/?download=csv"
 
     results = await get_cboe_data(url, use_cache)
 
     response = BytesIO(results)
 
     directory = read_csv(response)
@@ -132,23 +131,22 @@
         }
     ).set_index("symbol")
 
     return directory.astype(str)
 
 
 async def get_index_directory(use_cache: bool = True, **kwargs) -> DataFrame:
-    """
-    Get the Cboe Index Directory. If use_cache is True,
-    the data will be cached for 24 hours.
+    """Get the Cboe Index Directory.
+
+    If use_cache is True, the data will be cached for 24 hours.
 
     Returns
-    --------
+    -------
     List[Dict]: A list of dictionaries containing the index information.
     """
-
     url = "https://cdn.cboe.com/api/global/us_indices/definitions/all_indices.json"
 
     results = await get_cboe_data(url, use_cache=use_cache)
 
     [result.pop("featured") for result in results]
     [result.pop("featured_order") for result in results]
     [result.pop("display") for result in results]
@@ -158,19 +156,18 @@
     return results
 
 
 async def list_futures(**kwargs) -> List[dict]:
     """List of CBOE futures and their underlying symbols.
 
     Returns
-    --------
+    -------
     pd.DataFrame
         Pandas DataFrame with results.
     """
-
     r = await get_cboe_data(
         "https://cdn.cboe.com/api/global/delayed_quotes/symbol_book/futures-roots.json"
     )
     data = r.get("data")
     [d.pop("sort_order") for d in data]
 
     return data
@@ -179,18 +176,18 @@
 async def get_settlement_prices(
     settlement_date: Optional[dateType] = None,
     options: bool = False,
     archives: bool = False,
     final_settlement: bool = False,
     **kwargs,
 ) -> DataFrame:
-    """Gets the settlement prices of CBOE futures.
+    """Get the settlement prices of CBOE futures.
 
     Parameters
-    -----------
+    ----------
     settlement_date: Optional[date]
         The settlement date. Only valid for active contracts. [YYYY-MM-DD]
     options: bool
         If true, returns options on futures.
     archives: bool
         Settlement price archives for select years and products.  Overridden by other parameters.
     final_settlement: bool
```

### Comparing `openbb_cboe-1.1.4/PKG-INFO` & `openbb_cboe-1.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-cboe
-Version: 1.1.4
+Version: 1.1.5
 Summary: CBOE extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp-client-cache (>=0.10.0,<0.11.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB CBOE Provider
 
 This extension integrates the [CBOE](https://www.cboe.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

