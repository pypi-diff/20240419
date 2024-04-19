# Comparing `tmp/openbb_commodity-1.0.2.tar.gz` & `tmp/openbb_commodity-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_commodity-1.0.2.tar", max compression
+gzip compressed data, was "openbb_commodity-1.0.3.tar", max compression
```

## Comparing `openbb_commodity-1.0.2.tar` & `openbb_commodity-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      459 2024-03-13 16:36:51.554064 openbb_commodity-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.554538 openbb_commodity-1.0.2/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1260 2024-03-13 16:36:51.554980 openbb_commodity-1.0.2/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0      470 2024-04-01 14:18:29.422654 openbb_commodity-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_commodity-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      459 2024-04-17 12:33:20.497645 openbb_commodity-1.0.3/README.md
+-rw-r--r--   0        0        0       34 2024-04-17 12:33:20.497645 openbb_commodity-1.0.3/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-17 12:33:20.497645 openbb_commodity-1.0.3/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0      470 2024-04-19 16:40:00.579066 openbb_commodity-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_commodity-1.0.3/PKG-INFO
```

### Comparing `openbb_commodity-1.0.2/openbb_commodity/commodity_router.py` & `openbb_commodity-1.0.3/openbb_commodity/commodity_router.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ProviderChoices,
     StandardParams,
 )
 from openbb_core.app.query import Query
 from openbb_core.app.router import Router
 from pydantic import BaseModel
 
-router = Router(prefix="")
+router = Router(prefix="", description="Commodity market data.")
 
 
 # pylint: disable=unused-argument
 @router.command(
     model="LbmaFixing",
     examples=[
         APIEx(parameters={"provider": "nasdaq"}),
```

### Comparing `openbb_commodity-1.0.2/PKG-INFO` & `openbb_commodity-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-commodity
-Version: 1.0.2
+Version: 1.0.3
 Summary: Commodity extension for OpenBB
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
 
 # Commodity Extension for OpenBB Platform
 
 This extension provides a set of commands for commodity-related data.
 
 ## Installation
```

