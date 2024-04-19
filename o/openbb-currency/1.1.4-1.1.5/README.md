# Comparing `tmp/openbb_currency-1.1.4.tar.gz` & `tmp/openbb_currency-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_currency-1.1.4.tar", max compression
+gzip compressed data, was "openbb_currency-1.1.5.tar", max compression
```

## Comparing `openbb_currency-1.1.4.tar` & `openbb_currency-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      454 2024-02-29 11:03:36.730583 openbb_currency-1.1.4/README.md
--rw-r--r--   0        0        0       32 2024-02-29 11:03:36.730878 openbb_currency-1.1.4/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3794 2024-03-13 16:36:51.559019 openbb_currency-1.1.4/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-02-29 11:03:36.730995 openbb_currency-1.1.4/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-03-13 16:36:51.559499 openbb_currency-1.1.4/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.731082 openbb_currency-1.1.4/openbb_currency/py.typed
--rw-r--r--   0        0        0      464 2024-04-01 14:19:13.124194 openbb_currency-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_currency-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      454 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/README.md
+-rw-r--r--   0        0        0       32 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3848 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/py.typed
+-rw-r--r--   0        0        0      464 2024-04-19 16:40:14.511095 openbb_currency-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_currency-1.1.5/PKG-INFO
```

### Comparing `openbb_currency-1.1.4/openbb_currency/currency_router.py` & `openbb_currency-1.1.5/openbb_currency/currency_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     StandardParams,
 )
 from openbb_core.app.query import Query
 from openbb_core.app.router import Router
 
 from openbb_currency.price.price_router import router as price_router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Foreign exchange (FX) market data.")
 router.include_router(price_router)
 
 
 # pylint: disable=unused-argument
 @router.command(
     model="CurrencyPairs",
     examples=[
@@ -61,15 +61,15 @@
 )
 async def reference_rates(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Current, official, currency reference rates.
+    """Get current, official, currency reference rates.
 
     Foreign exchange reference rates are the exchange rates set by a major financial institution or regulatory body,
     serving as a benchmark for the value of currencies around the world.
     These rates are used as a standard to facilitate international trade and financial transactions,
     ensuring consistency and reliability in currency conversion.
     They are typically updated on a daily basis and reflect the market conditions at a specific time.
     Central banks and financial institutions often use these rates to guide their own exchange rates,
```

### Comparing `openbb_currency-1.1.4/openbb_currency/price/price_router.py` & `openbb_currency-1.1.5/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_currency-1.1.4/PKG-INFO` & `openbb_currency-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-currency
-Version: 1.1.4
+Version: 1.1.5
 Summary: Currency extension for OpenBB
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
 
 # OpenBB Currency Extension
 
 This extension provides currency exchange related data for the OpenBB Platform.
 
 ## Installation
```

