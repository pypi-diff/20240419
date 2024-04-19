# Comparing `tmp/openbb_yfinance-1.1.4.tar.gz` & `tmp/openbb_yfinance-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_yfinance-1.1.4.tar", max compression
+gzip compressed data, was "openbb_yfinance-1.1.5.tar", max compression
```

## Comparing `openbb_yfinance-1.1.4.tar` & `openbb_yfinance-1.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      450 2024-02-29 11:03:36.978859 openbb_yfinance-1.1.4/README.md
--rw-r--r--   0        0        0     4232 2024-03-21 17:38:35.661543 openbb_yfinance-1.1.4/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-02-29 11:03:36.979066 openbb_yfinance-1.1.4/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-01 13:46:32.186015 openbb_yfinance-1.1.4/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-03-21 17:38:35.661819 openbb_yfinance-1.1.4/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     1935 2024-03-21 17:38:35.661928 openbb_yfinance-1.1.4/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-03-13 16:36:51.900644 openbb_yfinance-1.1.4/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-03-13 16:36:51.900730 openbb_yfinance-1.1.4/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-03-13 16:36:51.900846 openbb_yfinance-1.1.4/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-03-21 17:38:35.662100 openbb_yfinance-1.1.4/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-03-21 17:38:35.662226 openbb_yfinance-1.1.4/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-03-21 17:38:35.662401 openbb_yfinance-1.1.4/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5722 2024-03-13 16:36:51.901334 openbb_yfinance-1.1.4/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-03-13 16:36:51.901450 openbb_yfinance-1.1.4/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-02-29 11:03:36.979842 openbb_yfinance-1.1.4/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10040 2024-04-01 11:58:23.835972 openbb_yfinance-1.1.4/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-03-21 17:38:35.662520 openbb_yfinance-1.1.4/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-03-21 17:38:35.662638 openbb_yfinance-1.1.4/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-03-21 17:38:35.662730 openbb_yfinance-1.1.4/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-03-21 17:38:35.662848 openbb_yfinance-1.1.4/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-03-13 16:36:51.901953 openbb_yfinance-1.1.4/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-03-13 16:36:51.902047 openbb_yfinance-1.1.4/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-03-21 17:38:35.662968 openbb_yfinance-1.1.4/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-03-13 16:36:51.902309 openbb_yfinance-1.1.4/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-03-13 16:36:51.902559 openbb_yfinance-1.1.4/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-03-21 17:38:35.663075 openbb_yfinance-1.1.4/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-03-21 17:38:35.663197 openbb_yfinance-1.1.4/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     3922 2024-03-13 16:36:51.902853 openbb_yfinance-1.1.4/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-03-13 16:36:51.902907 openbb_yfinance-1.1.4/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-03-21 17:38:35.663370 openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-03-21 17:38:35.663509 openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.980652 openbb_yfinance-1.1.4/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-02-29 11:03:36.980745 openbb_yfinance-1.1.4/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-03-13 16:36:51.903317 openbb_yfinance-1.1.4/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6639 2024-03-21 17:38:35.663686 openbb_yfinance-1.1.4/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-03-13 16:36:51.903594 openbb_yfinance-1.1.4/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0      484 2024-04-01 14:19:31.712085 openbb_yfinance-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 openbb_yfinance-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      450 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/README.md
+-rw-r--r--   0        0        0     4232 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     2036 2024-04-19 16:31:25.550563 openbb_yfinance-1.1.5/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5858 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10102 2024-04-19 16:31:25.550563 openbb_yfinance-1.1.5/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4230 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-04-19 13:09:31.739184 openbb_yfinance-1.1.5/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0      484 2024-04-19 16:42:17.983382 openbb_yfinance-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 openbb_yfinance-1.1.5/PKG-INFO
```

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/__init__.py` & `openbb_yfinance-1.1.5/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/active.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/available_indices.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/available_indices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Yahoo Finance Available Indices Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.available_indices import (
     AvailableIndicesData,
     AvailableIndicesQueryParams,
@@ -39,18 +41,19 @@
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> YFinanceAvailableIndicesQueryParams:
         """Transform the query params."""
         return YFinanceAvailableIndicesQueryParams(**params)
 
     @staticmethod
     def extract_data(
-        query: YFinanceAvailableIndicesQueryParams,
+        query: YFinanceAvailableIndicesQueryParams,  # pylint disable=unused-argument
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
+        """Extract the data."""
         indices = pd.DataFrame(INDICES).transpose().reset_index()
         indices.columns = ["code", "name", "ticker"]
 
         return indices.to_dict("records")
 
     @staticmethod
     def transform_data(
```

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/balance_sheet.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/cash_flow.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/company_news.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/crypto_historical.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/currency_historical.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/equity_historical.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/equity_profile.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/equity_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """YFinance Equity Profile Model."""
 
 # pylint: disable=unused-argument
 import asyncio
 import warnings
-from datetime import datetime
+from datetime import (
+    date as dateType,
+    timezone,
+)
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_info import (
     EquityInfoData,
     EquityInfoQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from pydantic import Field, field_validator
 from yfinance import Ticker
 
 _warn = warnings.warn
 
 
 class YFinanceEquityProfileQueryParams(EquityInfoQueryParams):
@@ -93,17 +97,17 @@
     beta: Optional[float] = Field(
         description="The beta of the asset relative to the broad market.",
         default=None,
     )
 
     @field_validator("first_stock_price_date", mode="before", check_fields=False)
     @classmethod
-    def validate_first_trade_date(cls, v):
+    def validate_first_trade_date(cls, v: float) -> Optional[dateType]:
         """Validate first stock price date."""
-        return datetime.utcfromtimestamp(v).date() if v else None
+        return safe_fromtimestamp(v, tz=timezone.utc).date() if v else None
 
 
 class YFinanceEquityProfileFetcher(
     Fetcher[YFinanceEquityProfileQueryParams, List[YFinanceEquityProfileData]]
 ):
     """YFinance Equity Profile fetcher."""
```

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/equity_quote.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/etf_historical.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/etf_info.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/etf_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_info import (
     EtfInfoData,
     EtfInfoQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from pydantic import Field, field_validator
 from yfinance import Ticker
 
 _warn = warnings.warn
 
 
 class YFinanceEtfInfoQueryParams(EtfInfoQueryParams):
@@ -271,15 +272,15 @@
                                 result[field] = ticker.get(field, None)
                         if "firstTradeDateEpochUtc" in result:
                             _first_trade = result.pop("firstTradeDateEpochUtc")
                             if (
                                 "fundInceptionDate" not in result
                                 and _first_trade is not None
                             ):
-                                result["fundInceptionDate"] = datetime.fromtimestamp(
+                                result["fundInceptionDate"] = safe_fromtimestamp(
                                     _first_trade
                                 )
                     except Exception as e:
                         _warn(f"Error processing data for {symbol}: {e}")
                         result = {}
                 if quote_type != "ETF":
                     _warn(f"{symbol} is not an ETF.")
```

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/futures_curve.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/futures_historical.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/gainers.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/growth_tech_equities.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/historical_dividends.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/income_statement.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/index_historical.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/key_executives.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/key_metrics.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/losers.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/market_indices.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/price_target_consensus.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/price_target_consensus.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.price_target_consensus import (
     PriceTargetConsensusData,
     PriceTargetConsensusQueryParams,
 )
-from pydantic import Field
+from pydantic import Field, field_validator
 from yfinance import Ticker
 
 _warn = warnings.warn
 
 
 class YFinancePriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """YFinance Price Target Consensus Query."""
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def check_symbol(cls, value):
+        """Check the symbol."""
+        if not value:
+            raise RuntimeError("Error: Symbol is a required field for yFinance.")
+        return value
+
 
 class YFinancePriceTargetConsensusData(PriceTargetConsensusData):
     """YFinance Price Target Consensus Data."""
 
     __alias_dict__ = {
         "target_high": "targetHighPrice",
         "target_low": "targetLowPrice",
@@ -74,15 +82,15 @@
     @staticmethod
     async def aextract_data(
         query: YFinancePriceTargetConsensusQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the raw data from YFinance."""
-        symbols = query.symbol.split(",")
+        symbols = query.symbol.split(",")  # type: ignore
         results = []
         fields = [
             "symbol",
             "currentPrice",
             "currency",
             "targetHighPrice",
             "targetLowPrice",
```

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/share_statistics.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/utils/futures.csv` & `openbb_yfinance-1.1.5/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/utils/helpers.py` & `openbb_yfinance-1.1.5/openbb_yfinance/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,27 +96,30 @@
     group_by: Literal["ticker", "column"] = "ticker",
     adjusted: bool = False,
     **kwargs: Any,
 ) -> pd.DataFrame:
     """Get yFinance OHLC data for any ticker and interval available."""
     symbol = symbol.upper()
     _start_date = start_date
-
+    intraday = False
     if interval in ["60m", "1h"]:
         period = "2y" if period in ["5y", "10y", "max"] else period
         _start_date = None
+        intraday = True
 
     if interval in ["2m", "5m", "15m", "30m", "90m"]:
         _start_date = (datetime.now().date() - relativedelta(days=58)).strftime(
             "%Y-%m-%d"
         )
+        intraday = True
 
     if interval == "1m":
         period = "5d"
         _start_date = None
+        intraday = True
 
     if adjusted is False:
         kwargs = dict(auto_adjust=False, back_adjust=False)
 
     try:
         data = yf.download(
             tickers=symbol,
@@ -154,48 +157,35 @@
             _data = _data.set_index(index_keys).sort_index()
             data = _data
     if not data.empty:
         data = data.reset_index()
         data = data.rename(columns={"Date": "date", "Datetime": "date"})
         data["date"] = data["date"].apply(pd.to_datetime)
         data = data[data["Open"] > 0]
-
         if start_date is not None:
             data = data[data["date"] >= pd.to_datetime(start_date)]
         if (
             end_date is not None
             and start_date is not None
             and pd.to_datetime(end_date) > pd.to_datetime(start_date)
         ):
             data = data[
-                data["date"] <= (pd.to_datetime(end_date) + relativedelta(days=1))
+                data["date"]
+                <= (
+                    pd.to_datetime(end_date)
+                    + relativedelta(minutes=719 if intraday is True else 0)
+                )
             ]
-
-        if period not in [
-            "max",
-            "1d",
-            "5d",
-            "1wk",
-            "1mo",
-            "3mo",
-            "6mo",
-            "1y",
-            "2y",
-            "5y",
-            "10y",
-        ]:
+        if intraday is True:
             data["date"] = data["date"].dt.strftime("%Y-%m-%d %H:%M:%S")
-        if interval not in ["1m", "2m", "5m", "15m", "30m", "90m", "60m", "1h"]:
+        else:
             data["date"] = data["date"].dt.strftime("%Y-%m-%d")
-
         if adjusted is False:
             data = data.drop(columns=["Adj Close"])
-
         data.columns = data.columns.str.lower().str.replace(" ", "_").to_list()
-
     return data
 
 
 def df_transform_numbers(data: pd.DataFrame, columns: list) -> pd.DataFrame:
     """Replace abbreviations of numbers with actual numbers."""
     multipliers = {"M": 1e6, "B": 1e9, "T": 1e12}
```

### Comparing `openbb_yfinance-1.1.4/openbb_yfinance/utils/references.py` & `openbb_yfinance-1.1.5/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.4/PKG-INFO` & `openbb_yfinance-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-yfinance
-Version: 1.1.4
+Version: 1.1.5
 Summary: yfinance extension for OpenBB
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
 Requires-Dist: yfinance (>=0.2.27,<0.3.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Yahoo!Finance Provider
 
 This extension integrates the [Yahoo!Finance](https://finance.yahoo.com/) data provider into the OpenBB Platform.
```

