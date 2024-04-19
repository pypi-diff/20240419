# Comparing `tmp/openbb_tradier-1.0.1.tar.gz` & `tmp/openbb_tradier-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradier-1.0.1.tar", max compression
+gzip compressed data, was "openbb_tradier-1.0.2.tar", max compression
```

## Comparing `openbb_tradier-1.0.1.tar` & `openbb_tradier-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      438 2024-03-13 16:36:51.891842 openbb_tradier-1.0.1/README.md
--rw-r--r--   0        0        0     1241 2024-03-21 17:38:35.660567 openbb_tradier-1.0.1/openbb_tradier/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.893874 openbb_tradier-1.0.1/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-21 17:38:35.660734 openbb_tradier-1.0.1/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9162 2024-03-21 17:38:35.660909 openbb_tradier-1.0.1/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-03-21 17:38:35.661032 openbb_tradier-1.0.1/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10222 2024-03-21 17:38:35.661130 openbb_tradier-1.0.1/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.894734 openbb_tradier-1.0.1/openbb_tradier/py.typed
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.894779 openbb_tradier-1.0.1/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-03-13 16:36:51.894856 openbb_tradier-1.0.1/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      474 2024-04-01 14:19:44.027846 openbb_tradier-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 openbb_tradier-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      438 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/README.md
+-rw-r--r--   0        0        0     1241 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6582 2024-04-19 16:31:25.550563 openbb_tradier-1.0.2/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9222 2024-04-19 16:31:25.550563 openbb_tradier-1.0.2/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-04-19 16:31:25.550563 openbb_tradier-1.0.2/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      474 2024-04-19 16:43:00.275490 openbb_tradier-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 openbb_tradier-1.0.2/PKG-INFO
```

### Comparing `openbb_tradier-1.0.1/openbb_tradier/__init__.py` & `openbb_tradier-1.0.2/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.1/openbb_tradier/models/equity_historical.py` & `openbb_tradier-1.0.2/openbb_tradier/models/equity_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tradier Equity Historical Model"""
+"""Tradier Equity Historical Model."""
 
 # pylint: disable = unused-argument
 
 import asyncio
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Literal, Optional
 from warnings import warn
@@ -12,15 +12,15 @@
     EquityHistoricalData,
     EquityHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import (
     QUERY_DESCRIPTIONS,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_tradier.utils.constants import INTERVALS_DICT
 from pandas import to_datetime
 from pydantic import Field
 from pytz import timezone
 
 
 class TradierEquityHistoricalQueryParams(EquityHistoricalQueryParams):
@@ -52,15 +52,14 @@
     Fetcher[TradierEquityHistoricalQueryParams, List[TradierEquityHistoricalData]]
 ):
     """Tradier Equity Historical Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TradierEquityHistoricalQueryParams:
         """Transform the query."""
-
         if params.get("interval") in ["1d", "1W", "1M"]:
             if params.get("start_date") is None:
                 params["start_date"] = (datetime.now() - timedelta(days=365)).date()
             if params.get("end_date") is None:
                 params["end_date"] = datetime.now().date()
 
         if params.get("interval") in ["1m", "5m", "15m"]:
@@ -81,15 +80,14 @@
     @staticmethod
     async def aextract_data(
         query: TradierEquityHistoricalQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Tradier endpoint."""
-
         api_key = credentials.get("tradier_api_key") if credentials else ""
         sandbox = True
 
         if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
             raise ValueError(
                 "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
             )
@@ -116,15 +114,14 @@
         end_point = "timesales" if query.interval in ["1m", "5m", "15m"] else "history"
         results = []
         start_time = "09:30" if query.extended_hours is False else "00:00"
         end_time = "16:00" if query.extended_hours is False else "20:00"
 
         async def get_one(symbol):
             """Get data for one symbol."""
-
             result = []
 
             url = (
                 f"{BASE_URL}v1/markets/{end_point}?symbol={symbol}&interval={interval}"
             )
 
             if query.interval in ["1m", "5m", "15m"]:
@@ -146,15 +143,15 @@
             if interval in ["1min", "5min", "15min"] and data.get("series"):  # type: ignore
                 result = data["series"].get("data")  # type: ignore
                 for r in result:
                     if len(query.symbol.split(",")) > 1:
                         r["symbol"] = symbol
                     _ = r.pop("time")
                     r["timestamp"] = (
-                        datetime.fromtimestamp(r.get("timestamp"))
+                        safe_fromtimestamp(r.get("timestamp"))
                         .replace(microsecond=0)
                         .astimezone(timezone("America/New_York"))
                     )
 
             if result != []:
                 results.extend(result)
             if result == []:
```

### Comparing `openbb_tradier-1.0.1/openbb_tradier/models/equity_quote.py` & `openbb_tradier-1.0.2/openbb_tradier/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tradier Equity Quote Model"""
+"""Tradier Equity Quote Model."""
 
 # pylint: disable = unused-argument
 
 from datetime import (
     date as dateType,
     datetime,
 )
@@ -11,15 +11,15 @@
 from dateutil.parser import parse
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_quote import (
     EquityQuoteData,
     EquityQuoteQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
 class TradierEquityQuoteQueryParams(EquityQuoteQueryParams):
     """Tradier Equity Quote Query."""
@@ -153,15 +153,16 @@
         mode="before",
         check_fields=False,
     )
     @classmethod
     def validate_dates(cls, v):
         """Validate the dates."""
         if v != 0 and v is not None and isinstance(v, int):
-            v = datetime.fromtimestamp(int(v) / 1000)
+            v = int(v) / 1000  # milliseconds to seconds
+            v = safe_fromtimestamp(v)
             v = v.replace(microsecond=0)
             v = v.astimezone(timezone("America/New_York"))
             return v
         if v is not None and isinstance(v, str):
             v = parse(v)
             v = v.replace(microsecond=0, tzinfo=timezone("UTC"))
             v = v.astimezone(timezone("America/New_York"))
@@ -198,15 +199,14 @@
     @staticmethod
     async def aextract_data(
         query: TradierEquityQuoteQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Tradier endpoint."""
-
         api_key = credentials.get("tradier_api_key") if credentials else ""
         sandbox = True
 
         if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
             raise ValueError(
                 "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
             )
@@ -241,15 +241,14 @@
     @staticmethod
     def transform_data(
         query: TradierEquityQuoteQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TradierEquityQuoteData]:
         """Transform and validate the data."""
-
         results: List[TradierEquityQuoteData] = []
 
         for d in data:
 
             d["exch"] = (
                 OPTIONS_EXCHANGES.get(d["exch"])
                 if d.get("type") in ["option", "index"]
```

### Comparing `openbb_tradier-1.0.1/openbb_tradier/models/equity_search.py` & `openbb_tradier-1.0.2/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.1/openbb_tradier/models/options_chains.py` & `openbb_tradier-1.0.2/openbb_tradier/models/options_chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-"""Tradier Options Chains Model"""
+"""Tradier Options Chains Model."""
 
 # pylint: disable = unused-argument
 
 import asyncio
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 from dateutil.parser import parse
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.options_chains import (
     OptionsChainsData,
     OptionsChainsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
 class TradierOptionsChainsQueryParams(OptionsChainsQueryParams):
-    """
-    Tradier Options Chains Query.
+    """Tradier Options Chains Query.
 
     Source: https://documentation.tradier.com/brokerage-api/markets/get-options-chains
 
     Greeks/IV data is updated once per hour.
     This data is calculated using the ORATS APIs and is supplied directly from them.
     """
 
 
 class TradierOptionsChainsData(OptionsChainsData):
-    """Tradier Options Chains Data"""
+    """Tradier Options Chains Data."""
 
     __alias_dict__ = {
         "expiration": "expiration_date",
         "contract_symbol": "symbol",
         "last_trade_price": "last",
         "bid_size": "bidsize",
         "ask_size": "asksize",
@@ -123,15 +122,16 @@
         mode="before",
         check_fields=False,
     )
     @classmethod
     def validate_dates(cls, v):
         """Validate the dates."""
         if v != 0 and v is not None and isinstance(v, int):
-            v = datetime.fromtimestamp(int(v) / 1000)
+            v = int(v) / 1000  # milliseconds to seconds
+            v = safe_fromtimestamp(v)
             v = v.replace(microsecond=0)
             v = v.astimezone(timezone("America/New_York"))
             return v
         if v is not None and isinstance(v, str):
             v = parse(v)
             v = v.replace(microsecond=0, tzinfo=timezone("UTC"))
             v = v.astimezone(timezone("America/New_York"))
@@ -173,24 +173,24 @@
 class TradierOptionsChainsFetcher(
     Fetcher[TradierOptionsChainsQueryParams, List[TradierOptionsChainsData]]
 ):
     """Tradier Options Chains Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TradierOptionsChainsQueryParams:
+        """Transform the query parameters."""
         return TradierOptionsChainsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: TradierOptionsChainsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Return the raw data from the Tradier endpoint"""
-
+        """Return the raw data from the Tradier endpoint."""
         api_key = credentials.get("tradier_api_key") if credentials else ""
         sandbox = True
 
         if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
             raise ValueError(
                 "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
             )
@@ -212,15 +212,14 @@
             "Authorization": f"Bearer {api_key}",
             "Accept": "application/json",
         }
 
         # Get the expiration dates for the symbol so we can gather the chains data.
         async def get_expirations(symbol):
             """Get the expiration dates for the given symbol."""
-
             url = (
                 f"{BASE_URL}expirations?symbol={symbol}&includeAllRoots=true"
                 "&strikes=false&contractSize=false&expirationType=false"
             )
             response = await amake_request(url, headers=HEADERS)
             if response.get("expirations") and isinstance(response["expirations"].get("date"), list):  # type: ignore
                 expirations = response["expirations"].get("date")  # type: ignore
```

### Comparing `openbb_tradier-1.0.1/openbb_tradier/utils/constants.py` & `openbb_tradier-1.0.2/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.1/PKG-INFO` & `openbb_tradier-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-tradier
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tradier Provider Extension for the OpenBB Platform
 Author: OpenBB
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
 
 # OpenBB Tradier Provider
 
 `openbb-tradier` is a data provider extension for the OpenBB Platform.
 
 ## Installation
```

