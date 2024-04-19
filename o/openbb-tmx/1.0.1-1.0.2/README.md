# Comparing `tmp/openbb_tmx-1.0.1.tar.gz` & `tmp/openbb_tmx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tmx-1.0.1.tar", max compression
+gzip compressed data, was "openbb_tmx-1.0.2.tar", max compression
```

## Comparing `openbb_tmx-1.0.1.tar` & `openbb_tmx-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2369 2024-03-13 16:36:51.803442 openbb_tmx-1.0.1/README.md
--rw-r--r--   0        0        0     3319 2024-03-21 17:38:35.656878 openbb_tmx-1.0.1/openbb_tmx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.804121 openbb_tmx-1.0.1/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-03-21 17:38:35.657064 openbb_tmx-1.0.1/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-03-21 17:38:35.657217 openbb_tmx-1.0.1/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5170 2024-03-21 17:38:35.657345 openbb_tmx-1.0.1/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-03-21 17:38:35.657496 openbb_tmx-1.0.1/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4373 2024-03-21 17:38:35.657642 openbb_tmx-1.0.1/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8830 2024-03-21 17:38:35.657823 openbb_tmx-1.0.1/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5446 2024-03-21 17:38:35.658001 openbb_tmx-1.0.1/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12441 2024-03-21 17:38:35.658160 openbb_tmx-1.0.1/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-03-21 17:38:35.658331 openbb_tmx-1.0.1/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-03-21 17:38:35.658468 openbb_tmx-1.0.1/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-03-21 17:38:35.658625 openbb_tmx-1.0.1/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-03-21 17:38:35.658764 openbb_tmx-1.0.1/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-03-21 17:38:35.658932 openbb_tmx-1.0.1/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-03-21 17:38:35.659035 openbb_tmx-1.0.1/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4439 2024-03-21 17:38:35.659165 openbb_tmx-1.0.1/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-03-21 17:38:35.659289 openbb_tmx-1.0.1/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3055 2024-03-21 17:38:35.659409 openbb_tmx-1.0.1/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-03-21 17:38:35.659521 openbb_tmx-1.0.1/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10268 2024-03-21 17:38:35.659626 openbb_tmx-1.0.1/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6055 2024-03-21 17:38:35.659773 openbb_tmx-1.0.1/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-03-21 17:38:35.659904 openbb_tmx-1.0.1/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5688 2024-03-21 17:38:35.660009 openbb_tmx-1.0.1/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-03-21 17:38:35.660112 openbb_tmx-1.0.1/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.806449 openbb_tmx-1.0.1/openbb_tmx/py.typed
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.806502 openbb_tmx-1.0.1/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-03-13 16:36:51.806596 openbb_tmx-1.0.1/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38297 2024-03-21 17:38:35.660407 openbb_tmx-1.0.1/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0      636 2024-04-01 14:21:26.089284 openbb_tmx-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 openbb_tmx-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2369 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/README.md
+-rw-r--r--   0        0        0     3319 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5162 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4647 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8843 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5455 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12451 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10325 2024-04-19 13:10:31.748034 openbb_tmx-1.0.2/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5986 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5133 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0      636 2024-04-19 16:41:11.435221 openbb_tmx-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 openbb_tmx-1.0.2/PKG-INFO
```

### Comparing `openbb_tmx-1.0.1/README.md` & `openbb_tmx-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/__init__.py` & `openbb_tmx-1.0.2/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/available_indices.py` & `openbb_tmx-1.0.2/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/bond_prices.py` & `openbb_tmx-1.0.2/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/calendar_earnings.py` & `openbb_tmx-1.0.2/openbb_tmx/models/calendar_earnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Earnings Calendar Model"""
+"""TMX Earnings Calendar Model."""
 
 # pylint: disable=unused-argument
 import asyncio
 import json
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Optional
 
@@ -81,22 +81,20 @@
     @staticmethod
     async def aextract_data(
         query: TmxCalendarEarningsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
-        results = []
-        dates = []
+        results: List[Dict] = []
         user_agent = get_random_agent()
         dates = date_range(query.start_date, end=query.end_date)
 
         async def create_task(date, results):
-            """Creates a task for a single date in the range."""
+            """Create a task for a single date in the range."""
             data = []
             date = date.strftime("%Y-%m-%d")
             payload = gql.get_earnings_date_payload.copy()
             payload["variables"]["date"] = date
             url = "https://app-money.tmx.com/graphql"
             r = await get_data_from_gql(
                 method="POST",
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/company_filings.py` & `openbb_tmx-1.0.2/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/company_news.py` & `openbb_tmx-1.0.2/openbb_tmx/models/company_news.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,25 @@
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
     page: Optional[int] = Field(
         default=1, description="The page number to start from. Use with limit."
     )
 
+    @field_validator("symbol", mode="before")
+    @classmethod
+    def symbols_validate(cls, v):
+        """Validate the symbols."""
+        if v is None:
+            raise ValueError("Symbol is a required field for TMX.")
+        return v
+
 
 class TmxCompanyNewsData(CompanyNewsData):
-    """TMX Stock News Data"""
+    """TMX Stock News Data."""
 
     __alias_dict__ = {
         "date": "datetime",
         "title": "headline",
     }
 
     source: Optional[str] = Field(description="Source of the news.", default=None)
@@ -59,30 +67,29 @@
     async def aextract_data(
         query: TmxCompanyNewsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
         user_agent = get_random_agent()
-        symbols = query.symbol.split(",")
-        results = []
+        symbols = query.symbol.split(",")  # type: ignore
+        results: List[Dict] = []
 
         async def create_task(symbol, results):
-            """Makes a POST request to the TMX GraphQL endpoint for a single symbol."""
-
+            """Make a POST request to the TMX GraphQL endpoint for a single symbol."""
             symbol = (
                 symbol.upper().replace(".TO", "").replace(".TSX", "").replace("-", ".")
             )
             payload = gql.get_company_news_events_payload
             payload["variables"]["symbol"] = symbol
             payload["variables"]["page"] = query.page
             payload["variables"]["limit"] = query.limit
             payload["variables"]["locale"] = "en"
             url = "https://app-money.tmx.com/graphql"
-            data = {}
+            data: Dict = {}
             response = await get_data_from_gql(
                 method="POST",
                 url=url,
                 data=json.dumps(payload),
                 headers={
                     "authority": "app-money.tmx.com",
                     "referer": f"https://money.tmx.com/en/quote/{symbol}",
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/equity_historical.py` & `openbb_tmx-1.0.2/openbb_tmx/models/equity_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     source: https://money.tmx.com
     """
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
     interval: Union[
         Literal["1m", "2m", "5m", "15m", "30m", "60m", "1h", "1d", "1W", "1M"], str, int
-    ] = Field(
+    ] = Field(  # type: ignore
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " Or, any integer (entered as a string) representing the number of minutes."
         + " Default is daily data."
         + " There is no extended hours data, and intraday data is limited to after April 12 2022.",
         default="day",
     )
     adjustment: Literal["splits_only", "splits_and_dividends", "unadjusted"] = Field(
@@ -142,20 +142,19 @@
     @staticmethod
     async def aextract_data(
         query: TmxEquityHistoricalQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         results: List[Dict] = []
         symbols = query.symbol.split(",")
 
         async def create_task(symbol, results):
-            """Makes a POST request to the TMX GraphQL endpoint for a single ticker."""
+            """Make a POST request to the TMX GraphQL endpoint for a single ticker."""
             data: List[Dict] = []
             # A different request is used for each type of interval.
             if query.interval == "day":
                 data = await get_daily_price_history(
                     symbol,
                     start_date=query.start_date,
                     end_date=query.end_date,
@@ -195,15 +194,14 @@
     @staticmethod
     def transform_data(
         query: TmxEquityHistoricalQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TmxEquityHistoricalData]:
         """Return the transformed data."""
-
         results = DataFrame(data)
         if results.empty or len(results) == 0:
             raise EmptyDataError()
 
         # Handle the date formatting differences.
         results = results.rename(columns={"dateTime": "datetime"})
         if query.interval != "day":
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/equity_profile.py` & `openbb_tmx-1.0.2/openbb_tmx/models/equity_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Equity Profile fetcher"""
+"""TMX Equity Profile fetcher."""
 
 # pylint: disable=unused-argument
 import asyncio
 import json
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
@@ -80,26 +80,24 @@
     @staticmethod
     async def aextract_data(
         query: TmxEquityProfileQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         symbols = query.symbol.split(",")
 
         # The list where the results will be stored and appended to.
-        results = []
+        results: List[Dict] = []
         user_agent = get_random_agent()
 
         url = "https://app-money.tmx.com/graphql"
 
         async def create_task(symbol: str, results) -> None:
-            """Makes a POST request to the TMX GraphQL endpoint for a single symbol."""
-
+            """Make a POST request to the TMX GraphQL endpoint for a single symbol."""
             symbol = (
                 symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
             )
 
             payload = gql.stock_info_payload.copy()
             payload["variables"]["symbol"] = symbol
 
@@ -129,15 +127,14 @@
     @staticmethod
     def transform_data(
         query: TmxEquityProfileQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TmxEquityProfileData]:
         """Return the transformed data."""
-
         # Get only the items associated with `equity.profile()`.
         items_list = [
             "shortDescription",
             "longDescription",
             "website",
             "phoneNumber",
             "fullAddress",
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/equity_quote.py` & `openbb_tmx-1.0.2/openbb_tmx/models/equity_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Equity Profile fetcher"""
+"""TMX Equity Profile fetcher."""
 
 # pylint: disable=unused-argument
 
 import asyncio
 import json
 import warnings
 from datetime import (
@@ -233,15 +233,15 @@
         "div_ex_date",
         "div_pay_date",
         mode="before",
         check_fields=False,
     )
     @classmethod
     def date_validate(cls, v):  # pylint: disable=E0213
-        """Return the datetime object from the date string"""
+        """Return the datetime object from the date string."""
         if v:
             try:
                 return datetime.strptime(v, "%Y-%m-%d").date()
             except ValueError:
                 return datetime.strptime(v, "%Y-%m-%d %H:%M:%S.%f").date()
         return None
 
@@ -277,26 +277,24 @@
     @staticmethod
     async def aextract_data(
         query: TmxEquityQuoteQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         symbols = query.symbol.split(",")
 
         # The list where the results will be stored and appended to.
-        results = []
+        results: List[Dict] = []
         user_agent = get_random_agent()
 
         url = "https://app-money.tmx.com/graphql"
 
         async def create_task(symbol: str, results) -> None:
-            """Makes a POST request to the TMX GraphQL endpoint for a single symbol."""
-
+            """Make a POST request to the TMX GraphQL endpoint for a single symbol."""
             symbol = (
                 symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
             )
 
             payload = gql.stock_info_payload.copy()
             payload["variables"]["symbol"] = symbol
 
@@ -328,15 +326,14 @@
     @staticmethod
     def transform_data(
         query: TmxEquityQuoteQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TmxEquityQuoteData]:
         """Return the transformed data."""
-
         # Remove the items associated with `equity.profile()`.
         items_list = [
             "shortDescription",
             "longDescription",
             "website",
             "phoneNumber",
             "fullAddress",
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/equity_search.py` & `openbb_tmx-1.0.2/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/etf_countries.py` & `openbb_tmx-1.0.2/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/etf_holdings.py` & `openbb_tmx-1.0.2/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/etf_info.py` & `openbb_tmx-1.0.2/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/etf_search.py` & `openbb_tmx-1.0.2/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/etf_sectors.py` & `openbb_tmx-1.0.2/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/gainers.py` & `openbb_tmx-1.0.2/openbb_tmx/models/gainers.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     def normalize_percent(cls, v):
         """Return percents as normalized percentage points."""
         return float(v) / 100 if v else 0
 
     @model_validator(mode="before")
     @classmethod
     def check_metric(cls, values):
+        """Check for missing metrics."""
         for k, v in values.items():
             if v is None or v == "-":
                 values[k] = 0
             if k in ["Dividend Yield"]:
                 values[k] = float(v) / 100 if v else None
         return values
 
@@ -100,15 +101,14 @@
     @staticmethod
     async def aextract_data(
         query: TmxGainersQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[TmxGainersData]:
         """Return the raw data from the TMX endpoint."""
-
         user_agent = get_random_agent()
         payload = gql.get_stock_list_payload.copy()
         payload["variables"]["stockListId"] = STOCK_LISTS_DICT[query.category]
 
         url = "https://app-money.tmx.com/graphql"
         response = await get_data_from_gql(
             method="POST",
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/historical_dividends.py` & `openbb_tmx-1.0.2/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/index_constituents.py` & `openbb_tmx-1.0.2/openbb_tmx/models/index_constituents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Index Constituents Model"""
+"""TMX Index Constituents Model."""
 
 # pylint: disable=unused-argument
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.index_constituents import (
     IndexConstituentsData,
@@ -45,27 +45,28 @@
 
 class TmxIndexConstituentsFetcher(
     Fetcher[
         TmxIndexConstituentsQueryParams,
         List[TmxIndexConstituentsData],
     ]
 ):
+    """TMX Index Constituents Fetcher."""
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TmxIndexConstituentsQueryParams:
         """Transform the query."""
         return TmxIndexConstituentsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: TmxIndexConstituentsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the TMX endpoint."""
-
         url = "https://tmxinfoservices.com/files/indices/sptsx-indices.json"
 
         data = await get_data_from_url(
             url,
             use_cache=query.use_cache,
             backend=tmx_indices_backend,
         )
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/index_sectors.py` & `openbb_tmx-1.0.2/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/index_snapshots.py` & `openbb_tmx-1.0.2/openbb_tmx/models/index_snapshots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Index Snapshots Model"""
+"""TMX Index Snapshots Model."""
 
 # pylint: disable=unused-argument
 import json
 from typing import Any, Dict, List, Literal, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.index_snapshots import (
@@ -20,15 +20,15 @@
 )
 from pydantic import Field, field_validator
 
 
 class TmxIndexSnapshotsQueryParams(IndexSnapshotsQueryParams):
     """TMX Index Snapshots Query Params."""
 
-    region: Literal[None, "ca", "us"] = Field(default="ca")
+    region: Literal[None, "ca", "us"] = Field(default="ca")  # type: ignore
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request."
         + " Index data is from a single JSON file, updated each day after close."
         + " It is cached for one day. To bypass, set to False.",
     )
 
@@ -147,14 +147,16 @@
 
 class TmxIndexSnapshotsFetcher(
     Fetcher[
         TmxIndexSnapshotsQueryParams,
         List[TmxIndexSnapshotsData],
     ]
 ):
+    """TMX Index Snapshots Fetcher."""
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TmxIndexSnapshotsQueryParams:
         """Transform the query."""
         return TmxIndexSnapshotsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/insider_trading.py` & `openbb_tmx-1.0.2/openbb_tmx/models/insider_trading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TMX Insider Trading Model"""
+"""TMX Insider Trading Model."""
 
 # pylint: disable=unused-argument
 import json
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.insider_trading import (
@@ -13,24 +13,24 @@
 from openbb_core.provider.utils.helpers import to_snake_case
 from openbb_tmx.utils import gql
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, field_validator
 
 
 class TmxInsiderTradingQueryParams(InsiderTradingQueryParams):
-    """TMX Insider Trading Query Params"""
+    """TMX Insider Trading Query Params."""
 
     summary: bool = Field(
         default=False,
         description="Return a summary of the insider activity instead of the individuals.",
     )
 
 
 class TmxInsiderTradingData(InsiderTradingData):
-    """TMX Insider Trading Data"""
+    """TMX Insider Trading Data."""
 
     period: str = Field(
         description="The period of the activity. Bucketed by three, six, and twelve months."
     )
     owner_name: Optional[str] = Field(
         default=None, description="The name of the insider."
     )
@@ -62,14 +62,15 @@
         default=None,
         description="The total net activity by all insiders over the period.",
     )
 
     @field_validator("period", mode="before", check_fields=False)
     @classmethod
     def period_to_snake_case(cls, v):
+        """Convert the period to snake case."""
         return to_snake_case(v) if v else None
 
 
 class TmxInsiderTradingFetcher(
     Fetcher[
         TmxInsiderTradingQueryParams,
         List[TmxInsiderTradingData],
@@ -85,15 +86,14 @@
     @staticmethod
     async def aextract_data(
         query: TmxInsiderTradingQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-
         results = []
         user_agent = get_random_agent()
         symbol = (
             query.symbol.upper()
             .replace("-", ".")
             .replace(".TO", "")
             .replace(".TSX", "")
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/options_chains.py` & `openbb_tmx-1.0.2/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/price_target_consensus.py` & `openbb_tmx-1.0.2/openbb_tmx/models/price_target_consensus.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 
 
 class TmxPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """TMX Price Target Consensus Query."""
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def check_symbol(cls, value):
+        """Check the symbol."""
+        if not value:
+            raise RuntimeError("Error: Symbol is a required field for TMX.")
+        return value
+
 
 class TmxPriceTargetConsensusData(PriceTargetConsensusData):
     """TMX Price Target Consensus Data."""
 
     __alias_dict__ = {
         "target_consensus": "price_target",
         "target_high": "price_target_high",
@@ -84,16 +92,16 @@
     @staticmethod
     async def aextract_data(
         query: TmxPriceTargetConsensusQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the TMX endpoint."""
-        symbols = query.symbol.split(",")
-        results = []
+        symbols = query.symbol.split(",")  # type: ignore
+        results: List[Dict] = []
 
         async def create_task(symbol, results):
             """Create a task for each symbol provided."""
             symbol = (
                 symbol.upper()
                 .replace("-", ".")
                 .replace(".TO", "")
```

### Comparing `openbb_tmx-1.0.1/openbb_tmx/models/treasury_prices.py` & `openbb_tmx-1.0.2/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/utils/gql.py` & `openbb_tmx-1.0.2/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.1/openbb_tmx/utils/helpers.py` & `openbb_tmx-1.0.2/openbb_tmx/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import (
     date as dateType,
     datetime,
     time,
     timedelta,
 )
 from io import StringIO
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional, Union
 
 import exchange_calendars as xcals
 import pandas as pd
 import pytz
 from aiohttp_client_cache import SQLiteBackend
 from aiohttp_client_cache.session import CachedSession
 from dateutil import rrule
@@ -261,15 +261,15 @@
     "^XCM": "PHLX Chemicals Sector",
     "^XEX": "PHLX Europe Sector",
     "^XND": "Nasdaq-100 Micro Index",
 }
 
 
 async def response_callback(response, _: Any):
-    """Callback for HTTP Client Response."""
+    """Use callback for HTTP Client Response."""
     content_type = response.headers.get("Content-Type", "")
     if "application/json" in content_type:
         return await response.json()
     if "text" in content_type:
         return await response.text()
     return await response.read()
 
@@ -292,29 +292,28 @@
         data = await amake_request(url, response_callback=response_callback, timeout=20)
 
     return data
 
 
 async def get_data_from_gql(url: str, headers, data, **kwargs: Any) -> Any:
     """Make an asynchronous GraphQL request."""
-
     response = await amake_request(
         url=url,
         method="POST",
         response_callback=response_callback,
         headers=headers,
         data=data,
         timeout=30,
     )
 
     return response
 
 
 def replace_values_in_list_of_dicts(data):
-    """Helper function to replace "NA" and "-" with None in a list of dictionaries."""
+    """Replace "NA" and "-" with None in a list of dictionaries."""
     for d in data:
         for k, v in d.items():
             if isinstance(v, dict):
                 replace_values_in_list_of_dicts([v])  # Recurse into nested dictionary
             elif isinstance(v, list):
                 for i in range(len(v)):  # pylint: disable=C0200
                     if isinstance(v[i], dict):
@@ -325,52 +324,47 @@
                         v[i] = None  # Replace "NA" and "-" with None
             elif v in ("NA", "-"):
                 d[k] = None  # Replace "NA" and "-" with None
     return data
 
 
 def check_weekday(date) -> str:
-    """Helper function to check if the input date is a weekday, and if not, returns the next weekday.
+    """Check if the input date is a weekday, and if not, returns the next weekday.
 
     Parameters
     ----------
     date: str
         The date to check in YYYY-MM-DD format.
 
     Returns
     -------
     str
         Date in YYYY-MM-DD format.  If the date is a weekend, returns the date of the next weekday.
     """
-
     if pd.to_datetime(date).weekday() > 4:
         return next_workday(pd.to_datetime(date)).strftime("%Y-%m-%d")
     return date
 
 
 async def get_all_etfs(use_cache: bool = True) -> List[Dict]:
-    """
-    Gets a summary of the TMX ETF universe.
+    """Get a summary of the TMX ETF universe.
 
     Returns
     -------
     Dict
         Dictionary with all TMX-listed ETFs.
     """
-
     url = "https://dgr53wu9i7rmp.cloudfront.net/etfs/etfs.json"
 
     response = await get_data_from_url(
         url, use_cache=use_cache, backend=tmx_etfs_backend
     )
 
-    if response is None:
-        raise RuntimeError(
-            f"There was a problem with the request. Could not get ETFs.  -> {response.status_code}"
-        )
+    if not response or response is None:
+        raise RuntimeError("There was a problem with the request. Could not get ETFs.")
 
     response = replace_values_in_list_of_dicts(response)
 
     etfs = pd.DataFrame(response).rename(columns=COLUMNS_DICT)
 
     etfs = etfs.drop(
         columns=[
@@ -399,16 +393,15 @@
 
     return etfs.to_dict(orient="records")
 
 
 async def get_tmx_tickers(
     exchange: Literal["tsx", "tsxv"] = "tsx", use_cache: bool = True
 ) -> Dict:
-    """Gets a dictionary of either TSX or TSX-V symbols and names."""
-
+    """Get a dictionary of either TSX or TSX-V symbols and names."""
     tsx_json_url = "https://www.tsx.com/json/company-directory/search"
     url = f"{tsx_json_url}/{exchange}/*"
     response = await get_data_from_url(
         url, use_cache=use_cache, backend=tmx_companies_backend
     )
     data = (
         pd.DataFrame.from_records(response["results"])[["symbol", "name"]]
@@ -416,32 +409,31 @@
         .sort_index()
     )
     results = data.to_dict()["name"]
     return results
 
 
 async def get_all_tmx_companies(use_cache: bool = True) -> Dict:
-    """Merges TSX and TSX-V listings into a single dictionary."""
+    """Merge TSX and TSX-V listings into a single dictionary."""
     all_tmx = {}
     tsx_tickers = await get_tmx_tickers(use_cache=use_cache)
     tsxv_tickers = await get_tmx_tickers("tsxv", use_cache=use_cache)
     all_tmx.update(tsxv_tickers)
     all_tmx.update(tsx_tickers)
     return all_tmx
 
 
 async def get_all_options_tickers(use_cache: bool = True) -> pd.DataFrame:
-    """Returns a DataFrame with all valid ticker symbols."""
-
+    """Return a DataFrame with all valid ticker symbols."""
     url = "https://www.m-x.ca/en/trading/data/options-list"
 
     r = await get_data_from_url(url, use_cache=use_cache, backend=tmx_companies_backend)
 
-    if r is None:
-        raise RuntimeError(f"Error with the request:  {r.status_code}")
+    if r is None or r == []:
+        raise RuntimeError("Error with the request")  # mypy: ignore
 
     options_listings = pd.read_html(StringIO(r))
     listings = pd.concat(options_listings)
     listings = listings.set_index("Option Symbol").drop_duplicates().sort_index()
     symbols = listings[:-1]
     symbols = symbols.fillna(value="")
     symbols["Underlying Symbol"] = (
@@ -452,16 +444,15 @@
         to_snake_case(col).replace("name_of_", "") for col in symbols.columns
     ]
 
     return symbols.set_index("option_symbol")
 
 
 async def get_current_options(symbol: str, use_cache: bool = True) -> pd.DataFrame:
-    """Gets the current quotes for the complete options chain."""
-
+    """Get the current quotes for the complete options chain."""
     SYMBOLS = await get_all_options_tickers(use_cache=use_cache)
     data = pd.DataFrame()
     symbol = symbol.upper()
 
     # Remove exchange  identifiers from the symbol.
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
     # Underlying symbol may have a different ticker symbol than the ticker used to lookup options.
@@ -554,16 +545,15 @@
 
     return chains
 
 
 async def download_eod_chains(
     symbol: str, date: Optional[dateType] = None, use_cache: bool = False
 ) -> pd.DataFrame:
-    """Downloads EOD chains data for a given symbol and date."""
-
+    """Download EOD chains data for a given symbol and date."""
     symbol = symbol.upper()
     SYMBOLS = await get_all_options_tickers(use_cache=False)
     # Remove echange  identifiers from the symbol.
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
 
     # Underlying symbol may have a different ticker symbol than the ticker used to lookup options.
     if len(SYMBOLS[SYMBOLS["underlying_symbol"].str.contains(symbol)]) == 1:
@@ -578,18 +568,18 @@
 
     cal = xcals.get_calendar("XTSE")
 
     if date is None:
         EOD_URL = BASE_URL + f"{symbol}" "&dnld=1#quotes"
     if date is not None:
         date = check_weekday(date)  # type: ignore
-        if cal.is_session(date) is False:
+        if cal.is_session(date) is False:  # type: ignore
             date = (pd.to_datetime(date) + timedelta(days=1)).strftime("%Y-%m-%d")  # type: ignore
         date = check_weekday(date)  # type: ignore
-        if cal.is_session(date=date) is False:
+        if cal.is_session(date=date) is False:  # type: ignore
             date = (pd.to_datetime(date) + timedelta(days=1)).strftime("%Y-%m-%d")  # type: ignore
 
         EOD_URL = (
             BASE_URL + f"{symbol}" "&from=" f"{date}" "&to=" f"{date}" "&dnld=1#quotes"
         )
 
     r = await get_data_from_url(EOD_URL, use_cache=use_cache)  # type: ignore
@@ -713,16 +703,16 @@
     results = r.get("data").get("filings")
 
     return results
 
 
 async def get_daily_price_history(
     symbol: str,
-    start_date: Optional[dateType] = None,
-    end_date: Optional[dateType] = None,
+    start_date: Optional[Union[str, dateType]] = None,
+    end_date: Optional[Union[str, dateType]] = None,
     adjustment: Literal[
         "splits_only", "unadjusted", "splits_and_dividends"
     ] = "splits_only",
 ):
     """Get historical price data."""
     start_date = (
         datetime.strptime(start_date, "%Y-%m-%d")
@@ -830,29 +820,31 @@
     results = [d for d in results if d["openPrice"] is not None]
 
     return sorted(results, key=lambda x: x["datetime"], reverse=False)
 
 
 async def get_weekly_or_monthly_price_history(
     symbol: str,
-    start_date: Optional[dateType] = None,
-    end_date: Optional[dateType] = None,
+    start_date: Optional[Union[str, dateType]] = None,
+    end_date: Optional[Union[str, dateType]] = None,
     interval: Literal["month", "week"] = "month",
 ):
     """Get historical price data."""
-    start_date = (
-        datetime.strptime(start_date, "%Y-%m-%d")
-        if isinstance(start_date, str)
-        else start_date
-    )
-    end_date = (
-        datetime.strptime(end_date, "%Y-%m-%d")
-        if isinstance(end_date, str)
-        else end_date
-    )
+    if start_date:
+        start_date = (
+            datetime.strptime(start_date, "%Y-%m-%d")
+            if isinstance(start_date, str)
+            else start_date
+        )
+    if end_date:
+        end_date = (
+            datetime.strptime(end_date, "%Y-%m-%d")
+            if isinstance(end_date, str)
+            else end_date
+        )
     user_agent = get_random_agent()
     results: List[Dict] = []
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
     start_date = (
         (datetime.now() - timedelta(weeks=52 * 100)).date()
         if start_date is None
         else start_date
@@ -864,16 +856,22 @@
         payload["variables"].pop("interval")
     if "startDateTime" in payload["variables"]:
         payload["variables"].pop("startDateTime")
     if "endDateTime" in payload["variables"]:
         payload["variables"].pop("endDateTime")
     payload["variables"]["symbol"] = symbol
     payload["variables"]["freq"] = interval
-    payload["variables"]["end"] = end_date.strftime("%Y-%m-%d")
-    payload["variables"]["start"] = start_date.strftime("%Y-%m-%d")
+    payload["variables"]["end"] = (
+        end_date.strftime("%Y-%m-%d") if isinstance(end_date, dateType) else end_date
+    )
+    payload["variables"]["start"] = (
+        start_date.strftime("%Y-%m-%d")
+        if isinstance(start_date, dateType)
+        else start_date
+    )
     url = "https://app-money.tmx.com/graphql"
     data = await get_data_from_gql(
         method="POST",
         url=url,
         data=json.dumps(payload),
         headers={
             "authority": "app-money.tmx.com",
@@ -910,46 +908,48 @@
         results = data["data"].get("getTimeSeriesData")
         results = sorted(results, key=lambda x: x["dateTime"], reverse=False)
     return results
 
 
 async def get_intraday_price_history(
     symbol: str,
-    start_date: Optional[dateType] = None,
-    end_date: Optional[dateType] = None,
+    start_date: Optional[Union[str, dateType]] = None,
+    end_date: Optional[Union[str, dateType]] = None,
     interval: Optional[int] = 1,
 ):
     """Get historical price data."""
-    start_date = (
-        datetime.strptime(start_date, "%Y-%m-%d")
-        if isinstance(start_date, str)
-        else start_date
-    )
-    end_date = (
-        datetime.strptime(end_date, "%Y-%m-%d")
-        if isinstance(end_date, str)
-        else end_date
-    )
+    if start_date:
+        start_date = (
+            datetime.strptime(start_date, "%Y-%m-%d")
+            if isinstance(start_date, str)
+            else start_date
+        )
+    if end_date:
+        end_date = (
+            datetime.strptime(end_date, "%Y-%m-%d")
+            if isinstance(end_date, str)
+            else end_date
+        )
     user_agent = get_random_agent()
     results: List[Dict] = []
     symbol = symbol.upper().replace("-", ".").replace(".TO", "").replace(".TSX", "")
     start_date = (
         (datetime.now() - timedelta(weeks=4)).date()
         if start_date is None
         else start_date
     )
     end_date = datetime.now().date() if end_date is None else end_date
     # This is the first date of available intraday data.
     date_check = datetime(2022, 4, 12).date()
     start_date = max(start_date, date_check)
-    if end_date < date_check:
+    if end_date < date_check:  # type: ignore
         end_date = datetime.now().date()
     # Generate a list of dates from start_date to end_date with a frequency of 3 weeks
     dates = list(
-        rrule.rrule(rrule.WEEKLY, interval=4, dtstart=start_date, until=end_date)
+        rrule.rrule(rrule.WEEKLY, interval=4, dtstart=start_date, until=end_date)  # type: ignore
     )
 
     if dates[-1] != end_date:
         dates.append(end_date)  # type: ignore
 
     # Create a list of 4-week chunks
     chunks = [
@@ -1035,16 +1035,18 @@
     if len(results) > 0 and "dateTime" in results[0]:
         results = sorted(results, key=lambda x: x["dateTime"], reverse=False)
 
     return results
 
 
 async def get_all_bonds(use_cache: bool = True) -> pd.DataFrame:
-    """Gets all bonds reference data published by CIRO. The complete list is approximately 70-100K securities."""
+    """Get all bonds reference data published by CIRO.
 
+    The complete list is approximately 70-100K securities.
+    """
     url = "https://bondtradedata.iiroc.ca/debtip/designatedbonds/list"
     response = await get_data_from_url(
         url, use_cache=use_cache, timeout=30, backend=tmx_bonds_backend
     )
 
     # Convert the response to a DataFrame and set the types for proper filtering in-fetcher.
     # This is done here because multiple functions might share this response object.
```

### Comparing `openbb_tmx-1.0.1/pyproject.toml` & `openbb_tmx-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "openbb-tmx"
-version = "1.0.1"
+version = "1.0.2"
 description = "Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API."
 authors = ["OpenBB <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_tmx" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp-client-cache = "^0.10.0"
 aiosqlite = "^0.19.0"
 random-user-agent = "^1.0.1"
 exchange-calendars = "^4.2.8"
-openbb-core = "^1.1.5"
+openbb-core = "^1.1.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tmx = "openbb_tmx:tmx_provider"
```

### Comparing `openbb_tmx-1.0.1/PKG-INFO` & `openbb_tmx-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-tmx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API.
 Author: OpenBB
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
 Requires-Dist: exchange-calendars (>=4.2.8,<5.0.0)
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # openbb-tmx: A Community Data Provider Extension
 
 `openbb-tmx` is an unofficial, community, data provider extension for the OpenBB Platform.
```

