# Comparing `tmp/openbb_index-1.1.4.tar.gz` & `tmp/openbb_index-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_index-1.1.4.tar", max compression
+gzip compressed data, was "openbb_index-1.1.5.tar", max compression
```

## Comparing `openbb_index-1.1.4.tar` & `openbb_index-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      460 2024-02-29 11:03:36.739916 openbb_index-1.1.4/README.md
--rw-r--r--   0        0        0       23 2024-02-29 11:03:36.740144 openbb_index-1.1.4/openbb_index/__init__.py
--rw-r--r--   0        0        0     4053 2024-03-13 16:36:51.577125 openbb_index-1.1.4/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-03-13 16:36:51.577211 openbb_index-1.1.4/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-03-13 16:36:51.577338 openbb_index-1.1.4/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.740242 openbb_index-1.1.4/openbb_index/py.typed
--rw-r--r--   0        0        0      446 2024-04-01 14:19:00.666251 openbb_index-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_index-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      460 2024-04-17 12:33:20.501645 openbb_index-1.1.5/README.md
+-rw-r--r--   0        0        0       23 2024-04-17 12:33:20.501645 openbb_index-1.1.5/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-04-17 12:33:20.501645 openbb_index-1.1.5/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-04-17 12:33:20.501645 openbb_index-1.1.5/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-17 12:33:20.501645 openbb_index-1.1.5/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_index-1.1.5/openbb_index/py.typed
+-rw-r--r--   0        0        0      446 2024-04-19 16:39:54.543053 openbb_index-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_index-1.1.5/PKG-INFO
```

### Comparing `openbb_index-1.1.4/openbb_index/index_router.py` & `openbb_index-1.1.5/openbb_index/index_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     StandardParams,
 )
 from openbb_core.app.query import Query
 from openbb_core.app.router import Router
 
 from openbb_index.price.price_router import router as price_router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Indices data.")
 router.include_router(price_router)
 
 # pylint: disable=unused-argument
 
 
 @router.command(
     model="MarketIndices",
@@ -32,15 +32,15 @@
 )
 async def market(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Historical Market Indices."""
+    """Get Historical Market Indices."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="IndexConstituents",
     examples=[
         APIEx(parameters={"symbol": "dowjones", "provider": "fmp"}),
@@ -52,15 +52,15 @@
 )
 async def constituents(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Index Constituents."""
+    """Get Index Constituents."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="IndexSnapshots",
     examples=[
         APIEx(parameters={"provider": "tmx"}),
@@ -103,15 +103,15 @@
 )
 async def search(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Filters indices for rows containing the query."""
+    """Filter indices for rows containing the query."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="SP500Multiples",
     examples=[
         APIEx(parameters={"provider": "nasdaq"}),
@@ -120,23 +120,23 @@
 )
 async def sp500_multiples(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Historical S&P 500 multiples and Shiller PE ratios."""
+    """Get historical S&P 500 multiples and Shiller PE ratios."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="IndexSectors",
     examples=[APIEx(parameters={"symbol": "^TX60", "provider": "tmx"})],
 )
 async def sectors(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Index Sectors. Sector weighting of an index."""
+    """Get Index Sectors. Sector weighting of an index."""
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_index-1.1.4/openbb_index/price/price_router.py` & `openbb_index-1.1.5/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_index-1.1.4/PKG-INFO` & `openbb_index-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-index
-Version: 1.1.4
+Version: 1.1.5
 Summary: Index extension for OpenBB
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
 
 # OpenBB Index Extension
 
 The Index extension provides global and european index data access for the OpenBB Platform.
 
 ## Installation
```

