# Comparing `tmp/openbb_etf-1.1.4.tar.gz` & `tmp/openbb_etf-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_etf-1.1.4.tar", max compression
+gzip compressed data, was "openbb_etf-1.1.5.tar", max compression
```

## Comparing `openbb_etf-1.1.4.tar` & `openbb_etf-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      216 2024-02-29 11:03:36.737177 openbb_etf-1.1.4/README.md
--rw-r--r--   0        0        0       28 2024-02-29 11:03:36.737607 openbb_etf-1.1.4/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-02-29 11:03:36.737701 openbb_etf-1.1.4/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-03-13 16:36:51.571874 openbb_etf-1.1.4/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6010 2024-03-18 09:35:41.445390 openbb_etf-1.1.4/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.737920 openbb_etf-1.1.4/openbb_etf/py.typed
--rw-r--r--   0        0        0      441 2024-04-01 14:19:07.467348 openbb_etf-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 openbb_etf-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      216 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/README.md
+-rw-r--r--   0        0        0       28 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6392 2024-04-19 13:09:31.715183 openbb_etf-1.1.5/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/py.typed
+-rw-r--r--   0        0        0      441 2024-04-19 16:39:36.851018 openbb_etf-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 openbb_etf-1.1.5/PKG-INFO
```

### Comparing `openbb_etf-1.1.4/openbb_etf/discovery/discovery_router.py` & `openbb_etf-1.1.5/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_etf-1.1.4/openbb_etf/etf_router.py` & `openbb_etf-1.1.5/openbb_etf/etf_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """ETF Router."""
 
+from openbb_core.app.deprecation import OpenBBDeprecationWarning
 from openbb_core.app.model.command_context import CommandContext
 from openbb_core.app.model.example import APIEx
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.provider_interface import (
     ExtraParams,
     ProviderChoices,
     StandardParams,
 )
 from openbb_core.app.query import Query
 from openbb_core.app.router import Router
 
 from openbb_etf.discovery.discovery_router import router as discovery_router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Exchange Traded Funds market data.")
 router.include_router(discovery_router)
 
 # pylint: disable=unused-argument
 
 
 @router.command(
     model="EtfSearch",
@@ -168,14 +169,21 @@
 ) -> OBBject:
     """Use this function to get the holdings dates, if available."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="EtfHoldingsPerformance",
+    deprecated=True,
+    deprecation=OpenBBDeprecationWarning(
+        message="This endpoint is deprecated; pass a list of holdings symbols directly to"
+        + " `/equity/price/performance` instead.",
+        since=(4, 1),
+        expected_removal=(4, 2),
+    ),
     examples=[APIEx(parameters={"symbol": "XLK", "provider": "fmp"})],
 )
 async def holdings_performance(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
```

### Comparing `openbb_etf-1.1.4/PKG-INFO` & `openbb_etf-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-etf
-Version: 1.1.4
+Version: 1.1.5
 Summary: ETF extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ETF data extension for OpenBB SDK
 
 This extension provides a set of commands for ETF data retrieval.
 
 ## Installation
```

