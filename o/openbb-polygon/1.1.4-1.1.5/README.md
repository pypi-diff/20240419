# Comparing `tmp/openbb_polygon-1.1.4.tar.gz` & `tmp/openbb_polygon-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_polygon-1.1.4.tar", max compression
+gzip compressed data, was "openbb_polygon-1.1.5.tar", max compression
```

## Comparing `openbb_polygon-1.1.4.tar` & `openbb_polygon-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      430 2024-02-29 11:03:36.885809 openbb_polygon-1.1.4/README.md
--rw-r--r--   0        0        0     2100 2024-03-21 17:38:35.652390 openbb_polygon-1.1.4/openbb_polygon/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.885969 openbb_polygon-1.1.4/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-03-21 17:38:35.652575 openbb_polygon-1.1.4/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-03-21 17:38:35.652696 openbb_polygon-1.1.4/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-03-13 16:36:51.767779 openbb_polygon-1.1.4/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6130 2024-03-13 16:36:51.767909 openbb_polygon-1.1.4/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6054 2024-03-13 16:36:51.768003 openbb_polygon-1.1.4/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-03-21 17:38:35.652826 openbb_polygon-1.1.4/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7020 2024-03-13 16:36:51.768639 openbb_polygon-1.1.4/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-03-21 17:38:35.652992 openbb_polygon-1.1.4/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-03-21 17:38:35.653155 openbb_polygon-1.1.4/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     5973 2024-03-13 16:36:51.768957 openbb_polygon-1.1.4/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3618 2024-03-21 17:38:35.653278 openbb_polygon-1.1.4/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-03-21 17:38:35.653455 openbb_polygon-1.1.4/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.887235 openbb_polygon-1.1.4/openbb_polygon/py.typed
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.887288 openbb_polygon-1.1.4/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3690 2024-03-13 16:36:51.769344 openbb_polygon-1.1.4/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0      457 2024-04-01 14:20:16.520095 openbb_polygon-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 openbb_polygon-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      430 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/README.md
+-rw-r--r--   0        0        0     2100 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     6961 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6283 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6255 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6125 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     7150 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-04-19 13:10:31.748034 openbb_polygon-1.1.5/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6142 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0      457 2024-04-19 16:43:11.675521 openbb_polygon-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 openbb_polygon-1.1.5/PKG-INFO
```

### Comparing `openbb_polygon-1.1.4/openbb_polygon/__init__.py` & `openbb_polygon-1.1.5/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/balance_sheet.py` & `openbb_polygon-1.1.5/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/cash_flow.py` & `openbb_polygon-1.1.5/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/company_news.py` & `openbb_polygon-1.1.5/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/crypto_historical.py` & `openbb_polygon-1.1.5/openbb_polygon/models/crypto_historical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Polygon Crypto Historical Price Model."""
 
 # pylint: disable=unused-argument,protected-access,line-too-long
 
 import warnings
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.crypto_historical import (
     CryptoHistoricalData,
     CryptoHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
 )
-from pytz import timezone
 
 _warn = warnings.warn
 
 
 class PolygonCryptoHistoricalQueryParams(CryptoHistoricalQueryParams):
     """Polygon Crypto Historical Price Query.
 
@@ -142,25 +145,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore
+            results: list = data.get("results", [])  # type: ignore
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore
+                next_url = data.get("next_url", None)  # type: ignore
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(r["t"] / 1000, tz=timezone("UTC"))
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone.utc)  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol.replace("X:", "")
```

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/currency_historical.py` & `openbb_polygon-1.1.5/openbb_polygon/models/currency_historical.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Polygon Currency Historical Price Model."""
 
 # pylint: disable=unused-argument,protected-access,line-too-long
 
 import warnings
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_historical import (
     CurrencyHistoricalData,
     CurrencyHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
 )
-from pytz import timezone
 
 _warn = warnings.warn
 
 
 class PolygonCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """Polygon Currency Historical Price Query.
 
@@ -139,25 +142,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore[union-attr]
+            results: list = data.get("results", [])  # type: ignore[union-attr]
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore[union-attr]
+                next_url = data.get("next_url", None)  # type: ignore[union-attr]
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(r["t"] / 1000, tz=timezone("UTC"))
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone.utc)  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol
```

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/currency_pairs.py` & `openbb_polygon-1.1.5/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/equity_historical.py` & `openbb_polygon-1.1.5/openbb_polygon/models/equity_historical.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Polygon Equity Historical Price Model."""
 
 # pylint: disable=unused-argument,protected-access
 
 import warnings
-from datetime import datetime
+from datetime import (
+    datetime,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_historical import (
     EquityHistoricalData,
     EquityHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pandas import to_datetime
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
@@ -148,27 +151,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore
+            results: list = data.get("results", [])  # type: ignore
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore
+                next_url = data.get("next_url", None)  # type: ignore
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(
-                    r["t"] / 1000, tz=timezone("America/New_York")
-                )
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone("America/New_York"))  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol
```

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/equity_nbbo.py` & `openbb_polygon-1.1.5/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/income_statement.py` & `openbb_polygon-1.1.5/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/index_historical.py` & `openbb_polygon-1.1.5/openbb_polygon/models/index_historical.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
 )
@@ -139,27 +140,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore[union-attr]
+            results: list = data.get("results", [])  # type: ignore[union-attr]
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore[union-attr]
+                next_url = data.get("next_url", None)  # type: ignore[union-attr]
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(
-                    r["t"] / 1000, tz=timezone("America/New_York")
-                )
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone("America/New_York"))  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol
```

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/market_indices.py` & `openbb_polygon-1.1.5/openbb_polygon/models/market_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Polygon Market Indices Model."""
 
-from datetime import datetime
+from datetime import (
+    datetime,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_indices import (
     MarketIndicesData,
     MarketIndicesQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from openbb_polygon.utils.helpers import get_data_many
 from pydantic import Field, PositiveInt
 
 
 class PolygonMarketIndicesQueryParams(MarketIndicesQueryParams):
     """Polygon Market Indices Query.
 
@@ -90,15 +93,16 @@
             f"I:{query.symbol}/range/{query.multiplier}/{query.timespan}/"
             f"{query.start_date}/{query.end_date}?adjusted={query.adjusted}"
             f"&sort={query.sort}&limit={query.limit}&apiKey={api_key}"
         )
         data = await get_data_many(request_url, "results", **kwargs)
 
         for d in data:
-            d["t"] = datetime.fromtimestamp(d["t"] / 1000)
+            v = d["t"] / 1000  # milliseconds to seconds
+            d["t"] = safe_fromtimestamp(v)
             if query.timespan not in ["minute", "hour"]:
                 d["t"] = d["t"].date()
 
         return data
 
     @staticmethod
     def transform_data(
```

### Comparing `openbb_polygon-1.1.4/openbb_polygon/models/market_snapshots.py` & `openbb_polygon-1.1.5/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.4/openbb_polygon/utils/helpers.py` & `openbb_polygon-1.1.5/openbb_polygon/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Polygon Helpers Module."""
 
 import json
 from io import StringIO
-from typing import Any, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union
 
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_request,
 )
@@ -27,39 +27,40 @@
 
     def json(self) -> dict:
         """Return the response as a dictionary."""
         return json.loads(self.text)
 
 
 def request(url: str) -> BasicResponse:
-    """
-    Request function for PyScript. Pass in Method and make sure to await.
+    """Request function for PyScript.
+
+    Pass in Method and make sure to await.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     url: str
         URL to make request to
 
-    Return:
-    -------
+    Return
+    ------
     response: BasicRequest
         BasicRequest object with status_code and text attributes
     """
     # pylint: disable=import-outside-toplevel
     from pyodide.http import open_url  # type: ignore
 
     response = open_url(url)
     return BasicResponse(response)
 
 
 async def response_callback(
     response: ClientResponse, _: ClientSession
 ) -> Union[dict, List[dict]]:
-    """Callback for make_request."""
-    data: dict = await response.json()
+    """Use callback for make_request."""
+    data: Dict = await response.json()  # type: ignore
 
     if response.status != 200:
         message = data.get("error", None) or data.get("message", None)
         raise RuntimeError(f"Error in Polygon request -> {message}")
 
     keys_in_data = "results" in data or "tickers" in data
 
@@ -75,23 +76,23 @@
 
 
 async def get_data_many(
     url: str, sub_dict: Optional[str] = None, **kwargs: Any
 ) -> List[dict]:
     """Get data from Polygon endpoint and convert to list of schemas.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     url: str
         The URL to get the data from.
     sub_dict: Optional[str]
         The sub-dictionary to use.
 
-    Returns:
-    --------
+    Returns
+    -------
     List[dict]
         Dictionary of data.
     """
     data = await get_data(url, **kwargs)
     if sub_dict and isinstance(data, dict):
         data = data.get(sub_dict, [])
     if isinstance(data, dict):
```

### Comparing `openbb_polygon-1.1.4/PKG-INFO` & `openbb_polygon-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-polygon
-Version: 1.1.4
+Version: 1.1.5
 Summary: Polygon extension for OpenBB
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
 
 # OpenBB Polygon Provider
 
 This extension integrates the [Polygon](https://polygon.io/) data provider into the OpenBB Platform.
 
 ## Installation
```

