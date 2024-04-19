# Comparing `tmp/openbb_nasdaq-1.1.5.tar.gz` & `tmp/openbb_nasdaq-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nasdaq-1.1.5.tar", max compression
+gzip compressed data, was "openbb_nasdaq-1.1.6.tar", max compression
```

## Comparing `openbb_nasdaq-1.1.5.tar` & `openbb_nasdaq-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      430 2024-02-29 11:03:36.880528 openbb_nasdaq-1.1.5/README.md
--rw-r--r--   0        0        0     1840 2024-03-21 17:38:35.650621 openbb_nasdaq-1.1.5/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.880694 openbb_nasdaq-1.1.5/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3954 2024-03-21 17:38:35.650736 openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6262 2024-03-21 17:38:35.650845 openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-03-21 17:38:35.651100 openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     5969 2024-03-21 17:38:35.651308 openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2173 2024-03-21 17:38:35.651441 openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-03-21 17:38:35.651670 openbb_nasdaq-1.1.5/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-03-13 16:36:51.754918 openbb_nasdaq-1.1.5/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5090 2024-03-21 17:38:35.651807 openbb_nasdaq-1.1.5/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-03-21 17:38:35.651935 openbb_nasdaq-1.1.5/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-03-21 17:38:35.652047 openbb_nasdaq-1.1.5/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-03-13 16:36:51.755257 openbb_nasdaq-1.1.5/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.755288 openbb_nasdaq-1.1.5/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.881374 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-02-29 11:03:36.881453 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-03-13 16:36:51.755367 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-03-13 16:36:51.755567 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      508 2024-04-01 14:19:55.357414 openbb_nasdaq-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 openbb_nasdaq-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      430 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/README.md
+-rw-r--r--   0        0        0     1840 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-04-19 15:17:18.352283 openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5109 2024-04-19 15:17:18.352283 openbb_nasdaq-1.1.6/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-04-19 13:10:31.748034 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      508 2024-04-19 16:40:57.859190 openbb_nasdaq-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 openbb_nasdaq-1.1.6/PKG-INFO
```

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/__init__.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_dividend.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         "payment_date",
         "declaration_date",
         mode="before",
         check_fields=False,
     )
     @classmethod
     def validate_date(cls, v: str):
+        """Validate the date."""
         v = v.replace("N/A", "")
         return datetime.strptime(v, "%m/%d/%Y").date() if v else None
 
 
 class NasdaqCalendarDividendFetcher(
     Fetcher[
         NasdaqCalendarDividendQueryParams,
```

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_earnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Nasdaq Earnings Calendar Model."""
 
+# pylint: disable=unused-argument
+
 from concurrent.futures import ThreadPoolExecutor
 from datetime import (
     date as dateType,
     datetime,
     timedelta,
 )
 from typing import Any, Dict, List, Optional
@@ -134,14 +136,16 @@
     Fetcher[
         NasdaqCalendarEarningsQueryParams,
         List[NasdaqCalendarEarningsData],
     ]
 ):
     """Transform the query, extract and transform the data from the Nasdaq endpoints."""
 
+    require_credentials = False
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqCalendarEarningsQueryParams:
         """Transform the query params."""
         now = datetime.today().date()
         transformed_params = params
 
         if params.get("start_date") is None:
```

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,32 +81,33 @@
 
 
 class NasdaqCotData(COTData):
     """Nasdaq CFTC Commitment of Traders Reports Data."""
 
     @field_validator("date", mode="before", check_fields=False)
     def date_validate(cls, v):  # pylint: disable=E0213
-        """Return the datetime object from the date string"""
-
+        """Return the datetime object from the date string."""
         return datetime.strptime(v, "%Y-%m-%d").date()
 
 
 class NasdaqCotFetcher(Fetcher[NasdaqCotQueryParams, List[NasdaqCotData]]):
     """Transform the query, extract and transform the data from the Nasdaq endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqCotQueryParams:
+        """Transform the query parameters."""
         return NasdaqCotQueryParams(**params)
 
     @staticmethod
     def extract_data(
         query: NasdaqCotQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
+        """Extract the data from the Nasdaq Data Link API."""
         api_key = credentials.get("nasdaq_api_key") if credentials else ""
 
         # The "code" can be an exact name, a symbol, or a CFTC series code.
         series_id: str = ""
         series_ids = pd.DataFrame(CFTC).transpose().reset_index(drop=True)
         series_ids.columns = series_ids.columns.str.lower()
 
@@ -170,8 +171,9 @@
 
     @staticmethod
     def transform_data(
         query: NasdaqCotQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[NasdaqCotData]:
+        """Transform the data."""
         return [NasdaqCotData.model_validate(d) for d in data]
```

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot_search.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cot_search import (
     CotSearchData,
     CotSearchQueryParams,
 )
 from openbb_nasdaq.utils.series_ids import CFTC
 
+# pylint: disable=W0613
+
 
 class NasdaqCotSearchQueryParams(CotSearchQueryParams):
     """Nasdaq CFTC Commitment of Traders Reports Search Query.
 
     Source: https://data.nasdaq.com/data/CFTC-commodity-futures-trading-commission-reports/documentation
     """
 
@@ -27,14 +29,15 @@
 ):
     """Transform the query, extract and transform the data from the Nasdaq endpoints."""
 
     require_credentials = False
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqCotSearchQueryParams:
+        """Transform the query params."""
         return NasdaqCotSearchQueryParams(**params)
 
     @staticmethod
     def extract_data(
         query: NasdaqCotSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
@@ -56,8 +59,9 @@
 
     @staticmethod
     def transform_data(
         query: CotSearchQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[NasdaqCotSearchData]:
+        """Transform the data."""
         return [NasdaqCotSearchData.model_validate(d) for d in data]
```

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/economic_calendar.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/equity_search.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/historical_dividends.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/historical_dividends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """Nasdaq Historical Dividends Model."""
 
 # pylint: disable=unused-argument
 import asyncio
-import warnings
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from dateutil import parser
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.historical_dividends import (
     HistoricalDividendsData,
     HistoricalDividendsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_nasdaq.utils.helpers import IPO_HEADERS
 from pydantic import Field, field_validator
 
-_warn = warnings.warn
-
 
 class NasdaqHistoricalDividendsQueryParams(HistoricalDividendsQueryParams):
     """Nasdaq Historical Dividends Query Params."""
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
 
@@ -88,14 +86,16 @@
 
 
 class NasdaqHistoricalDividendsFetcher(
     Fetcher[NasdaqHistoricalDividendsQueryParams, List[NasdaqHistoricalDividendsData]]
 ):
     """Nasdaq Historical Dividends Fetcher."""
 
+    require_credentials = False
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqHistoricalDividendsQueryParams:
         """Transform the params to the provider-specific query."""
         return NasdaqHistoricalDividendsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
@@ -127,15 +127,15 @@
 
             if data:
                 if len(symbols) > 1:
                     for d in data:
                         d["symbol"] = symbol
                 results.extend(data)
             if not data:
-                _warn(f"No data found for {symbol}")
+                warn(f"No data found for {symbol}")
 
         tasks = [get_one(symbol) for symbol in symbols]
 
         await asyncio.gather(*tasks)
         if results:
             return results
         raise EmptyDataError()
```

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/models/top_retail.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/utils/helpers.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/utils/query_params.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/openbb_nasdaq/utils/series_ids.py` & `openbb_nasdaq-1.1.6/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.5/PKG-INFO` & `openbb_nasdaq-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-nasdaq
-Version: 1.1.5
+Version: 1.1.6
 Summary: Nasdaq extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nasdaq-data-link (>=1.0.4,<2.0.0)
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Nasdaq Provider
 
 This extension integrates the [Nasdaq](https://www.nasdaq.com) data provider into the OpenBB Platform.
```

