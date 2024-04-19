# Comparing `tmp/openbb_intrinio-1.1.4.tar.gz` & `tmp/openbb_intrinio-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_intrinio-1.1.4.tar", max compression
+gzip compressed data, was "openbb_intrinio-1.1.5.tar", max compression
```

## Comparing `openbb_intrinio-1.1.4.tar` & `openbb_intrinio-1.1.5.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0      435 2024-02-29 11:03:36.874696 openbb_intrinio-1.1.4/README.md
--rw-r--r--   0        0        0     4877 2024-03-21 17:38:35.647407 openbb_intrinio-1.1.4/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-02-29 11:03:36.874926 openbb_intrinio-1.1.4/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-03-21 17:38:35.647677 openbb_intrinio-1.1.4/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-03-21 17:38:35.647832 openbb_intrinio-1.1.4/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-03-21 17:38:35.648040 openbb_intrinio-1.1.4/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-03-21 17:38:35.648194 openbb_intrinio-1.1.4/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3273 2024-03-22 23:30:27.583493 openbb_intrinio-1.1.4/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-03-21 17:38:35.648311 openbb_intrinio-1.1.4/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-03-13 16:36:51.743339 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2377 2024-03-21 17:38:35.648469 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-03-21 17:38:35.648601 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-03-21 17:38:35.648729 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7025 2024-03-18 09:35:41.453005 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-03-14 20:24:16.781915 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-03-21 17:38:35.648867 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-03-21 17:38:35.648989 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-03-21 17:38:35.649110 openbb_intrinio-1.1.4/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-03-21 17:38:35.649277 openbb_intrinio-1.1.4/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     3716 2024-03-13 16:36:51.743945 openbb_intrinio-1.1.4/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     4829 2024-03-13 16:36:51.744032 openbb_intrinio-1.1.4/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-03-21 17:38:35.649392 openbb_intrinio-1.1.4/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-03-21 17:38:35.649563 openbb_intrinio-1.1.4/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-03-13 16:36:51.744490 openbb_intrinio-1.1.4/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-03-21 17:38:35.649669 openbb_intrinio-1.1.4/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-03-21 17:38:35.649782 openbb_intrinio-1.1.4/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-03-13 16:36:51.745028 openbb_intrinio-1.1.4/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3328 2024-03-13 16:36:51.745129 openbb_intrinio-1.1.4/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-03-21 17:38:35.649897 openbb_intrinio-1.1.4/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8829 2024-03-19 14:52:38.490220 openbb_intrinio-1.1.4/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-03-21 17:38:35.650024 openbb_intrinio-1.1.4/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-03-13 16:36:51.745487 openbb_intrinio-1.1.4/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     5359 2024-03-21 17:38:35.650166 openbb_intrinio-1.1.4/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-03-21 17:38:35.650280 openbb_intrinio-1.1.4/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-03-13 16:36:51.745863 openbb_intrinio-1.1.4/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2550 2024-03-21 17:38:35.650413 openbb_intrinio-1.1.4/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.876946 openbb_intrinio-1.1.4/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-02-29 11:03:36.877031 openbb_intrinio-1.1.4/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4002 2024-03-13 16:36:51.746151 openbb_intrinio-1.1.4/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-03-18 09:35:41.453455 openbb_intrinio-1.1.4/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0      489 2024-04-01 14:21:12.248104 openbb_intrinio-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 openbb_intrinio-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      435 2024-04-17 12:33:20.669645 openbb_intrinio-1.1.5/README.md
+-rw-r--r--   0        0        0     5393 2024-04-17 12:33:20.669645 openbb_intrinio-1.1.5/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-17 12:33:20.669645 openbb_intrinio-1.1.5/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22983 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     3273 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     8675 2024-04-19 13:10:31.748034 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2376 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7321 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8417 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9694 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5090 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-04-19 13:10:31.748034 openbb_intrinio-1.1.5/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-04-19 13:10:31.748034 openbb_intrinio-1.1.5/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3357 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-04-19 16:31:25.550563 openbb_intrinio-1.1.5/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6513 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     2560 2024-04-19 16:31:25.550563 openbb_intrinio-1.1.5/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0      489 2024-04-19 16:43:17.507536 openbb_intrinio-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 openbb_intrinio-1.1.5/PKG-INFO
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/__init__.py` & `openbb_intrinio-1.1.5/openbb_intrinio/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 from openbb_intrinio.models.etf_holdings import IntrinioEtfHoldingsFetcher
 from openbb_intrinio.models.etf_info import IntrinioEtfInfoFetcher
 from openbb_intrinio.models.etf_price_performance import (
     IntrinioEtfPricePerformanceFetcher,
 )
 from openbb_intrinio.models.etf_search import IntrinioEtfSearchFetcher
 from openbb_intrinio.models.financial_ratios import IntrinioFinancialRatiosFetcher
+from openbb_intrinio.models.forward_eps_estimates import (
+    IntrinioForwardEpsEstimatesFetcher,
+)
+from openbb_intrinio.models.forward_sales_estimates import (
+    IntrinioForwardSalesEstimatesFetcher,
+)
 from openbb_intrinio.models.fred_series import IntrinioFredSeriesFetcher
 from openbb_intrinio.models.historical_attributes import (
     IntrinioHistoricalAttributesFetcher,
 )
 from openbb_intrinio.models.historical_dividends import (
     IntrinioHistoricalDividendsFetcher,
 )
@@ -33,14 +39,17 @@
 #     IntrinioInstitutionalOwnershipFetcher,
 # )
 from openbb_intrinio.models.key_metrics import IntrinioKeyMetricsFetcher
 from openbb_intrinio.models.latest_attributes import IntrinioLatestAttributesFetcher
 from openbb_intrinio.models.market_snapshots import IntrinioMarketSnapshotsFetcher
 from openbb_intrinio.models.options_chains import IntrinioOptionsChainsFetcher
 from openbb_intrinio.models.options_unusual import IntrinioOptionsUnusualFetcher
+from openbb_intrinio.models.price_target_consensus import (
+    IntrinioPriceTargetConsensusFetcher,
+)
 from openbb_intrinio.models.reported_financials import IntrinioReportedFinancialsFetcher
 from openbb_intrinio.models.search_attributes import (
     IntrinioSearchAttributesFetcher,
 )
 from openbb_intrinio.models.share_statistics import IntrinioShareStatisticsFetcher
 from openbb_intrinio.models.world_news import IntrinioWorldNewsFetcher
 
@@ -63,26 +72,29 @@
         "EquitySearch": IntrinioEquitySearchFetcher,
         "EtfHistorical": IntrinioEquityHistoricalFetcher,
         "EtfHoldings": IntrinioEtfHoldingsFetcher,
         "EtfInfo": IntrinioEtfInfoFetcher,
         "EtfPricePerformance": IntrinioEtfPricePerformanceFetcher,
         "EtfSearch": IntrinioEtfSearchFetcher,
         "FinancialRatios": IntrinioFinancialRatiosFetcher,
+        "ForwardEpsEstimates": IntrinioForwardEpsEstimatesFetcher,
+        "ForwardSalesEstimates": IntrinioForwardSalesEstimatesFetcher,
         "FredSeries": IntrinioFredSeriesFetcher,
         "HistoricalAttributes": IntrinioHistoricalAttributesFetcher,
         "HistoricalDividends": IntrinioHistoricalDividendsFetcher,
         "IncomeStatement": IntrinioIncomeStatementFetcher,
         "IndexHistorical": IntrinioIndexHistoricalFetcher,
         "InsiderTrading": IntrinioInsiderTradingFetcher,
         # "InstitutionalOwnership": IntrinioInstitutionalOwnershipFetcher, # Disabled due to unreliable Intrinio endpoint
         "KeyMetrics": IntrinioKeyMetricsFetcher,
         "LatestAttributes": IntrinioLatestAttributesFetcher,
         "MarketIndices": IntrinioIndexHistoricalFetcher,
         "MarketSnapshots": IntrinioMarketSnapshotsFetcher,
         "OptionsChains": IntrinioOptionsChainsFetcher,
         "OptionsUnusual": IntrinioOptionsUnusualFetcher,
+        "PriceTargetConsensus": IntrinioPriceTargetConsensusFetcher,
         "ReportedFinancials": IntrinioReportedFinancialsFetcher,
         "SearchAttributes": IntrinioSearchAttributesFetcher,
         "ShareStatistics": IntrinioShareStatisticsFetcher,
         "WorldNews": IntrinioWorldNewsFetcher,
     },
 )
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/balance_sheet.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/calendar_ipo.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/cash_flow.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/company_filings.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/company_news.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/currency_pairs.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_historical.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_info.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     # pylint: disable=W0613:unused-argument
     @staticmethod
     def transform_data(
         query: IntrinioEquityInfoQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioEquityInfoData]:
-        """Transforms the data."""
+        """Transform the data."""
         return [IntrinioEquityInfoData.model_validate(d) for d in data]
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_quote.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_search.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/etf_holdings.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_holdings.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_holdings import (
     EtfHoldingsData,
     EtfHoldingsQueryParams,
 )
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_request,
 )
 from pydantic import Field, model_validator
 
@@ -21,14 +22,20 @@
 class IntrinioEtfHoldingsQueryParams(EtfHoldingsQueryParams):
     """
     Intrinio ETF Holdings Query Params.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_holdings_v2
     """
 
+    __alias_dict__ = {"date": "as_of_date"}
+
+    date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("date", "")
+    )
+
 
 class IntrinioEtfHoldingsData(EtfHoldingsData):
     """Intrinio ETF Holdings Data."""
 
     __alias_dict__ = {
         "symbol": "ticker",
         "security_type": "type",
@@ -141,21 +148,19 @@
     @staticmethod
     async def aextract_data(
         query: IntrinioEtfHoldingsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
-
         api_key = credentials.get("intrinio_api_key") if credentials else ""
-
         symbol = query.symbol + ":US" if ":" not in query.symbol else query.symbol
-
         URL = f"https://api-v2.intrinio.com/etfs/{symbol}/holdings?page_size=10000&api_key={api_key}"
-
+        if query.date:
+            URL += f"&as_of_date={query.date}"
         data = []
 
         async def response_callback(response: ClientResponse, session: ClientSession):
             """Async response callback."""
             results = await response.json()
 
             if results.get("error"):  # type: ignore
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/etf_info.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/etf_price_performance.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/etf_search.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/financial_attributes.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/financial_ratios.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/fred_series.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/historical_attributes.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/historical_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Intrinio Historical Attributes Model."""
 
+# pylint: disable = unused-argument
+
 import warnings
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.app.model.abstract.warning import OpenBBWarning
 from openbb_core.provider.abstract.fetcher import Fetcher
@@ -58,79 +60,85 @@
         if params.get("end_date") is None:
             transformed_params["end_date"] = now
 
         return IntrinioHistoricalAttributesQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
-        query: IntrinioHistoricalAttributesQueryParams,  # pylint: disable=unused-argument
+        query: IntrinioHistoricalAttributesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
 
         base_url = "https://api-v2.intrinio.com"
         query_str = get_querystring(query.model_dump(by_alias=True), ["symbol", "tag"])
 
         def generate_url(symbol: str, tag: str) -> str:
-            """Returns the url for the given symbol and tag."""
+            """Return the url for the given symbol and tag."""
             url_params = f"{symbol}/{tag}?{query_str}&api_key={api_key}"
             url = f"{base_url}/historical_data/{url_params}"
             return url
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             """Return the response."""
             init_response = await response.json()
 
-            if message := init_response.get("error") or init_response.get("message"):
-                warnings.warn(message=message, category=OpenBBWarning)
+            if message := init_response.get(  # type: ignore
+                "error"
+            ) or init_response.get(  # type: ignore
+                "message"
+            ):
+                warnings.warn(message=str(message), category=OpenBBWarning)
                 return []
 
-            symbol = response.url.parts[-2]
-            tag = response.url.parts[-1]
+            symbol = response.url.parts[-2]  # type: ignore
+            tag = response.url.parts[-1]  # type: ignore
 
-            all_data: list = init_response.get("historical_data", [])
+            all_data: List = init_response.get("historical_data", [])  # type: ignore
             all_data = [{**item, "symbol": symbol, "tag": tag} for item in all_data]
 
-            next_page = init_response.get("next_page", None)
+            next_page = init_response.get("next_page", None)  # type: ignore
             while next_page:
-                url = response.url.update_query(next_page=next_page).human_repr()
+                url = response.url.update_query(  # type: ignore
+                    next_page=next_page
+                ).human_repr()
                 response_data = await session.get_json(url)
 
-                if message := response_data.get("error") or response_data.get(
+                if message := response_data.get("error") or response_data.get(  # type: ignore
                     "message"
                 ):
                     warnings.warn(message=message, category=OpenBBWarning)
                     return []
 
-                symbol = response.url.parts[-2]
-                tag = response_data.url.parts[-1]
+                symbol = response.url.parts[-2]  # type: ignore
+                tag = response_data.url.parts[-1]  # type: ignore
 
-                response_data = response_data.get("historical_data", [])
+                response_data = response_data.get("historical_data", [])  # type: ignore
                 response_data = [
                     {**item, "symbol": symbol, "tag": tag} for item in response_data
                 ]
 
                 all_data.extend(response_data)
-                next_page = response_data.get("next_page", None)
+                next_page = response_data.get("next_page", None)  # type: ignore
 
             return all_data
 
         urls = [
             generate_url(symbol, tag)
             for symbol in query.symbol.split(",")
             for tag in query.tag.split(",")
         ]
 
         return await amake_requests(urls, callback, **kwargs)
 
     @staticmethod
     def transform_data(
-        query: IntrinioHistoricalAttributesQueryParams,  # pylint: disable=unused-argument
+        query: IntrinioHistoricalAttributesQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioHistoricalAttributesData]:
         """Return the transformed data."""
         return [IntrinioHistoricalAttributesData.model_validate(d) for d in data]
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/historical_dividends.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/income_statement.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/index_historical.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/insider_trading.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/institutional_ownership.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/key_metrics.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/latest_attributes.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/latest_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,26 +53,27 @@
     ) -> Dict:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
 
         base_url = "https://api-v2.intrinio.com/companies"
 
         def generate_url(symbol: str, tag: str) -> str:
-            """Returns the url for the given symbol and tag."""
+            """Return the url for the given symbol and tag."""
             return f"{base_url}/{symbol}/data_point/{tag}?api_key={api_key}"
 
         async def callback(response: ClientResponse, _: Any) -> Dict:
             """Return the response."""
             response_data = await response.json()
 
             if isinstance(response_data, Dict) and (
                 "error" in response_data or "message" in response_data
             ):
                 warnings.warn(
-                    message=response_data.get("error") or response_data.get("message"),
+                    message=str(response_data.get("error"))
+                    or str(response_data.get("message")),
                     category=OpenBBWarning,
                 )
                 return {}
             if not response_data:
                 return {}
 
             tag = response.url.parts[-1]
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/market_indices.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/market_snapshots.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/market_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # pylint: disable=unused-argument
 
 import asyncio
 import gzip
 from datetime import (
     date as dateType,
     datetime,
+    timezone as datetime_timezone,
 )
 from io import BytesIO
 from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_snapshots import (
     MarketSnapshotsData,
     MarketSnapshotsQueryParams,
 )
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from pandas import DataFrame, notna, read_csv, to_datetime
 from pydantic import Field
 from pytz import timezone
 
 
 class IntrinioMarketSnapshotsQueryParams(MarketSnapshotsQueryParams):
     """Intrinio Market Snapshots Query.
@@ -101,15 +102,15 @@
         transformed_params = params
 
         if "date" in transformed_params:
             if isinstance(transformed_params["date"], datetime):
                 dt = transformed_params["date"]
                 dt = dt.astimezone(tz=timezone("America/New_York"))
             if isinstance(transformed_params["date"], dateType):
-                dt = transformed_params["date"]
+                dt = transformed_params["date"]  # type: ignore
                 if isinstance(dt, dateType):
                     dt = datetime(
                         dt.year,
                         dt.month,
                         dt.day,
                         20,
                         0,
@@ -139,15 +140,14 @@
     @staticmethod
     async def aextract_data(
         query: IntrinioMarketSnapshotsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
-
         api_key = credentials.get("intrinio_api_key") if credentials else ""
 
         # This gets the URL to the actual file.
         url = f"https://api-v2.intrinio.com/securities/snapshots?api_key={api_key}"
         if query.date:
             url += f"&at_datetime={query.date}"
 
@@ -212,15 +212,15 @@
                 "last_bid_timestamp",
                 "last_ask_timestamp",
             ]:
                 df[col] = (
                     to_datetime(
                         df[col].apply(
                             lambda x: (
-                                datetime.fromtimestamp(x, tz=timezone("UTC"))
+                                safe_fromtimestamp(x, tz=datetime_timezone.utc)
                                 if notna(x)
                                 else x
                             )
                         )
                     )
                     .dt.tz_convert("America/New_York")
                     .dt.floor("S")
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/options_chains.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/options_unusual.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/reported_financials.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/search_attributes.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/share_statistics.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/models/world_news.py` & `openbb_intrinio-1.1.5/openbb_intrinio/models/world_news.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class IntrinioWorldNewsData(WorldNewsData):
     """Intrinio World News Data."""
 
     __alias_dict__ = {"date": "publication_date", "text": "summary"}
 
     id: str = Field(description="Article ID.")
-    company: Dict[str, Any] = Field(
+    company: Optional[Dict[str, Any]] = Field(
         description="Company details related to the news article."
     )
 
     @field_validator("publication_date", mode="before", check_fields=False)
     def date_validate(cls, v):  # pylint: disable=E0213
         """Return the date as a datetime object."""
         return datetime.strptime(v, "%Y-%m-%dT%H:%M:%S.000Z")
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/utils/helpers.py` & `openbb_intrinio-1.1.5/openbb_intrinio/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     response = open_url(url)
     return BasicResponse(response)
 
 
 async def response_callback(
     response: ClientResponse, _: ClientSession
 ) -> Union[dict, List[dict]]:
-    """Callback for async_request."""
+    """Use callback for async_request."""
     data = await response.json()
 
     if isinstance(data, dict) and response.status != 200:
         if message := data.get("error", None) or data.get("message", None):
             raise RuntimeError(f"Error in Intrinio request -> {message}")
 
         if error := data.get("Error Message", None):
```

### Comparing `openbb_intrinio-1.1.4/openbb_intrinio/utils/references.py` & `openbb_intrinio-1.1.5/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.4/PKG-INFO` & `openbb_intrinio-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-intrinio
-Version: 1.1.4
+Version: 1.1.5
 Summary: Intrinio extension for OpenBB
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
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Intrinio Provider
 
 This extension integrates the [Intrinio](https://intrinio.com/) data provider into the OpenBB Platform.
```

