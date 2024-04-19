# Comparing `tmp/openbb_economy-1.1.4.tar.gz` & `tmp/openbb_economy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_economy-1.1.4.tar", max compression
+gzip compressed data, was "openbb_economy-1.1.5.tar", max compression
```

## Comparing `openbb_economy-1.1.4.tar` & `openbb_economy-1.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      461 2024-02-29 11:03:36.733875 openbb_economy-1.1.4/README.md
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.734126 openbb_economy-1.1.4/openbb_economy/__init__.py
--rw-r--r--   0        0        0     9705 2024-03-13 16:36:51.565563 openbb_economy-1.1.4/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1742 2024-03-13 16:36:51.565999 openbb_economy-1.1.4/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.734317 openbb_economy-1.1.4/openbb_economy/py.typed
--rw-r--r--   0        0        0      458 2024-04-01 14:18:12.527372 openbb_economy-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openbb_economy-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      461 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/README.md
+-rw-r--r--   0        0        0       32 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/__init__.py
+-rw-r--r--   0        0        0     9797 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/py.typed
+-rw-r--r--   0        0        0      458 2024-04-19 16:39:30.623005 openbb_economy-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openbb_economy-1.1.5/PKG-INFO
```

### Comparing `openbb_economy-1.1.4/openbb_economy/economy_router.py` & `openbb_economy-1.1.5/openbb_economy/economy_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     StandardParams,
 )
 from openbb_core.app.query import Query
 from openbb_core.app.router import Router
 
 from openbb_economy.gdp.gdp_router import router as gdp_router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Economic data.")
 router.include_router(gdp_router)
 
 # pylint: disable=unused-argument
 
 
 @router.command(
     model="EconomicCalendar",
@@ -65,29 +65,32 @@
 )
 async def cpi(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Consumer Price Index (CPI).  Returns either the rescaled index value, or a rate of change (inflation)."""
+    """Get Consumer Price Index (CPI).
+
+    Returns either the rescaled index value, or a rate of change (inflation).
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="RiskPremium",
     examples=[APIEx(parameters={"provider": "fmp"})],
 )
 async def risk_premium(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Market Risk Premium by country."""
+    """Get Market Risk Premium by country."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="BalanceOfPayments",
     examples=[
         APIEx(parameters={"provider": "ecb"}),
@@ -111,16 +114,16 @@
 @router.command(model="FredSearch", examples=[APIEx(parameters={"provider": "fred"})])
 async def fred_search(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Search for FRED series or economic releases by ID or string.
+    """Search for FRED series or economic releases by ID or string.
+
     This does not return the observation values, only the metadata.
     Use this function to find series IDs for `fred_series()`.
     """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
@@ -156,15 +159,18 @@
 )
 async def money_measures(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Money Measures (M1/M2 and components). The Federal Reserve publishes as part of the H.6 Release."""
+    """Get Money Measures (M1/M2 and components).
+
+    The Federal Reserve publishes as part of the H.6 Release.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="Unemployment",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -184,15 +190,15 @@
 )
 async def unemployment(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Global unemployment data."""
+    """Get global unemployment data."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="CLI",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -201,16 +207,19 @@
 )
 async def composite_leading_indicator(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """The composite leading indicator (CLI) is designed to provide early signals of turning points
+    """Use the composite leading indicator (CLI).
+
+    It is designed to provide early signals of turning points
     in business cycles showing fluctuation of the economic activity around its long term potential level.
+
     CLIs show short-term economic movements in qualitative rather than quantitative terms.
     """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="STIR",
@@ -223,17 +232,19 @@
 )
 async def short_term_interest_rate(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Short-term interest rates are the rates at which short-term borrowings are effected between
+    """Get Short-term interest rates.
+
+    They are the rates at which short-term borrowings are effected between
     financial institutions or the rate at which short-term government paper is issued or traded in the market.
+
     Short-term interest rates are generally averages of daily rates, measured as a percentage.
     Short-term interest rates are based on three-month money market rates where available.
     Typical standardised names are "money market rate" and "treasury bill rate".
     """
     return await OBBject.from_query(Query(**locals()))
 
 
@@ -248,24 +259,25 @@
 )
 async def long_term_interest_rate(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Long-term interest rates refer to government bonds maturing in ten years.
+    """Get Long-term interest rates that refer to government bonds maturing in ten years.
+
     Rates are mainly determined by the price charged by the lender, the risk from the borrower and the
     fall in the capital value. Long-term interest rates are generally averages of daily rates,
     measured as a percentage. These interest rates are implied by the prices at which the government bonds are
     traded on financial markets, not the interest rates at which the loans were issued.
     In all cases, they refer to bonds whose capital repayment is guaranteed by governments.
     Long-term interest rates are one of the determinants of business investment.
     Low long-term interest rates encourage investment in new equipment and high interest rates discourage it.
-    Investment is, in turn, a major source of economic growth."""
+    Investment is, in turn, a major source of economic growth.
+    """
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="FredRegional",
     examples=[
         APIEx(
@@ -285,12 +297,12 @@
 )
 async def fred_regional(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """
-    Query the Geo Fred API for regional economic data by series group.
+    """Query the Geo Fred API for regional economic data by series group.
+
     The series group ID is found by using `fred_search` and the `series_id` parameter.
     """
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_economy-1.1.4/openbb_economy/gdp/gdp_router.py` & `openbb_economy-1.1.5/openbb_economy/gdp/gdp_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 )
 async def forecast(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Forecasted GDP Data."""
+    """Get Forecasted GDP Data."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="GdpNominal",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -42,15 +42,15 @@
 )
 async def nominal(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Nominal GDP Data."""
+    """Get Nominal GDP Data."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="GdpReal",
     examples=[
         APIEx(parameters={"provider": "oecd"}),
@@ -59,9 +59,9 @@
 )
 async def real(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Real GDP Data."""
+    """Get Real GDP Data."""
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_economy-1.1.4/PKG-INFO` & `openbb_economy-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-economy
-Version: 1.1.4
+Version: 1.1.5
 Summary: Economy extension for OpenBB
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
 
 # OpenBB Economy Extension
 
 The Economy extension provides global macroeconomic data access for the OpenBB Platform.
 
 ## Installation
```

