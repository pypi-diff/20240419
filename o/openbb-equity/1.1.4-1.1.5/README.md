# Comparing `tmp/openbb_equity-1.1.4.tar.gz` & `tmp/openbb_equity-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_equity-1.1.4.tar", max compression
+gzip compressed data, was "openbb_equity-1.1.5.tar", max compression
```

## Comparing `openbb_equity-1.1.4.tar` & `openbb_equity-1.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      938 2024-02-29 11:03:36.734962 openbb_equity-1.1.4/README.md
--rw-r--r--   0        0        0       19 2024-02-29 11:03:36.735289 openbb_equity-1.1.4/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-02-29 11:03:36.735486 openbb_equity-1.1.4/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-03-13 16:36:51.567454 openbb_equity-1.1.4/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-02-29 11:03:36.735656 openbb_equity-1.1.4/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2326 2024-03-13 16:36:51.567755 openbb_equity-1.1.4/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-02-29 11:03:36.735800 openbb_equity-1.1.4/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1109 2024-03-13 16:36:51.568234 openbb_equity-1.1.4/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-02-29 11:03:36.735942 openbb_equity-1.1.4/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5811 2024-03-13 16:36:51.568426 openbb_equity-1.1.4/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3452 2024-03-13 16:36:51.568603 openbb_equity-1.1.4/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-02-29 11:03:36.736112 openbb_equity-1.1.4/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     2652 2024-03-13 16:36:51.568953 openbb_equity-1.1.4/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-02-29 11:03:36.736244 openbb_equity-1.1.4/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-03-13 16:36:51.569355 openbb_equity-1.1.4/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-02-29 11:03:36.736420 openbb_equity-1.1.4/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3769 2024-03-13 16:36:51.569810 openbb_equity-1.1.4/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-02-29 11:03:36.736541 openbb_equity-1.1.4/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-03-22 18:22:13.174274 openbb_equity-1.1.4/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.736634 openbb_equity-1.1.4/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-02-29 11:03:36.736696 openbb_equity-1.1.4/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-03-13 16:36:51.570690 openbb_equity-1.1.4/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0      452 2024-04-01 14:18:55.114548 openbb_equity-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 openbb_equity-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      938 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/README.md
+-rw-r--r--   0        0        0       19 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-17 12:33:20.501645 openbb_equity-1.1.5/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0      452 2024-04-19 16:39:48.883042 openbb_equity-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 openbb_equity-1.1.5/PKG-INFO
```

### Comparing `openbb_equity-1.1.4/README.md` & `openbb_equity-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.4/openbb_equity/calendar/calendar_router.py` & `openbb_equity-1.1.5/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.4/openbb_equity/compare/compare_router.py` & `openbb_equity-1.1.5/openbb_equity/compare/compare_router.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
     """Get the closest peers for a given company.
 
     Peers consist of companies trading on the same exchange, operating within the same sector
-    and with comparable market capitalizations."""
+    and with comparable market capitalizations.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="CompareGroups",
     examples=[
         APIEx(parameters={"provider": "finviz"}),
@@ -63,9 +64,10 @@
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
     """Get company data grouped by sector, industry or country and display either performance or valuation metrics.
 
     Valuation metrics include price to earnings, price to book, price to sales ratios and price to cash flow.
-    Performance metrics include the stock price change for different time periods."""
+    Performance metrics include the stock price change for different time periods.
+    """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_equity-1.1.4/openbb_equity/darkpool/darkpool_router.py` & `openbb_equity-1.1.5/openbb_equity/darkpool/darkpool_router.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,9 +31,10 @@
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
     """Get the weekly aggregate trade data for Over The Counter deals.
 
     ATS and non-ATS trading data for each ATS/firm
-    with trade reporting obligations under FINRA rules."""
+    with trade reporting obligations under FINRA rules.
+    """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_equity-1.1.4/openbb_equity/discovery/discovery_router.py` & `openbb_equity-1.1.5/openbb_equity/discovery/discovery_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,18 +140,19 @@
 )
 async def top_retail(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Tracks over $30B USD/day of individual investors trades.
+    """Track over $30B USD/day of individual investors trades.
 
     It gives a daily view into retail activity and sentiment for over 9,500 US traded stocks,
-    ADRs, and ETPs."""
+    ADRs, and ETPs.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="UpcomingReleaseDays",
     examples=[APIEx(parameters={"provider": "seeking_alpha"})],
 )
@@ -182,14 +183,15 @@
 )
 async def filings(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Get the URLs to SEC filings reported to EDGAR database, such as 10-K, 10-Q, 8-K, and more. SEC
-    filings include Form 10-K, Form 10-Q, Form 8-K, the proxy statement, Forms 3, 4, and 5, Schedule 13, Form 114,
+    """Get the URLs to SEC filings reported to EDGAR database, such as 10-K, 10-Q, 8-K, and more.
+
+    SEC filings include Form 10-K, Form 10-Q, Form 8-K, the proxy statement, Forms 3, 4, and 5, Schedule 13, Form 114,
     Foreign Investment Disclosures and others. The annual 10-K report is required to be
     filed annually and includes the company's financial statements, management discussion and analysis,
     and audited financial statements.
     """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_equity-1.1.4/openbb_equity/equity_router.py` & `openbb_equity-1.1.5/openbb_equity/equity_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from openbb_equity.discovery.discovery_router import router as discovery_router
 from openbb_equity.estimates.estimates_router import router as estimates_router
 from openbb_equity.fundamental.fundamental_router import router as fundamental_router
 from openbb_equity.ownership.ownership_router import router as ownership_router
 from openbb_equity.price.price_router import router as price_router
 from openbb_equity.shorts.shorts_router import router as shorts_router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Equity market data.")
 router.include_router(calendar_router)
 router.include_router(compare_router)
 router.include_router(estimates_router)
 router.include_router(darkpool_router)
 router.include_router(discovery_router)
 router.include_router(fundamental_router)
 router.include_router(ownership_router)
@@ -64,16 +64,18 @@
 )
 async def screener(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Screen for companies meeting various criteria. These criteria include
-    market cap, price, beta, volume, and dividend yield."""
+    """Screen for companies meeting various criteria.
+
+    These criteria include market cap, price, beta, volume, and dividend yield.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="EquityInfo",
     examples=[APIEx(parameters={"symbol": "AAPL", "provider": "fmp"})],
 )
```

### Comparing `openbb_equity-1.1.4/openbb_equity/estimates/estimates_router.py` & `openbb_equity-1.1.5/openbb_equity/estimates/estimates_router.py`

 * *Files 18% similar despite different names*

```diff
@@ -87,7 +87,53 @@
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
     """Search for specific analysts and get their forecast track record."""
     return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
+    model="ForwardSalesEstimates",
+    examples=[
+        APIEx(parameters={"symbol": "AAPL", "provider": "intrinio"}),
+        APIEx(
+            parameters={
+                "fiscal_year": 2025,
+                "fiscal_period": "fy",
+                "provider": "intrinio",
+            }
+        ),
+    ],
+)
+async def forward_sales(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:
+    """Get forward sales estimates."""
+    return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
+    model="ForwardEpsEstimates",
+    examples=[
+        APIEx(parameters={"symbol": "AAPL", "provider": "intrinio"}),
+        APIEx(
+            parameters={
+                "fiscal_year": 2025,
+                "fiscal_period": "fy",
+                "provider": "intrinio",
+            }
+        ),
+    ],
+)
+async def forward_eps(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:
+    """Get forward EPS estimates."""
+    return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_equity-1.1.4/openbb_equity/fundamental/fundamental_router.py` & `openbb_equity-1.1.5/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.4/openbb_equity/ownership/ownership_router.py` & `openbb_equity-1.1.5/openbb_equity/ownership/ownership_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
 )
 async def form_13f(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
+    """Get the form 13F.
+
     The Securities and Exchange Commission's (SEC) Form 13F is a quarterly report
     that is required to be filed by all institutional investment managers with at least
     $100 million in assets under management.
     Managers are required to file Form 13F within 45 days after the last day of the calendar quarter.
     Most funds wait until the end of this period in order to conceal
     their investment strategy from competitors and the public.
     """
```

### Comparing `openbb_equity-1.1.4/openbb_equity/price/price_router.py` & `openbb_equity-1.1.5/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.4/openbb_equity/shorts/shorts_router.py` & `openbb_equity-1.1.5/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.4/PKG-INFO` & `openbb_equity-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-equity
-Version: 1.1.4
+Version: 1.1.5
 Summary: Equity extension for OpenBB
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
 
 # OpenBB Equity Extension
 
 This extension provides equity market data tools for the OpenBB Platform.
 
 Features of the Equity extension include:
```

