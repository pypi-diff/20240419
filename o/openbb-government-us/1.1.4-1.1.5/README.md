# Comparing `tmp/openbb_government_us-1.1.4.tar.gz` & `tmp/openbb_government_us-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_government_us-1.1.4.tar", max compression
+gzip compressed data, was "openbb_government_us-1.1.5.tar", max compression
```

## Comparing `openbb_government_us-1.1.4.tar` & `openbb_government_us-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      445 2024-02-29 11:03:36.873075 openbb_government_us-1.1.4/README.md
--rw-r--r--   0        0        0      988 2024-03-21 17:38:35.647065 openbb_government_us-1.1.4/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-02-29 11:03:36.873377 openbb_government_us-1.1.4/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-03-13 16:36:51.740330 openbb_government_us-1.1.4/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5221 2024-03-21 17:38:35.647219 openbb_government_us-1.1.4/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.873541 openbb_government_us-1.1.4/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-03-13 16:36:51.740949 openbb_government_us-1.1.4/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0      522 2024-04-01 14:20:27.742856 openbb_government_us-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 openbb_government_us-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      445 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/README.md
+-rw-r--r--   0        0        0      988 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5269 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0      522 2024-04-19 16:42:24.367398 openbb_government_us-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 openbb_government_us-1.1.5/PKG-INFO
```

### Comparing `openbb_government_us-1.1.4/openbb_government_us/__init__.py` & `openbb_government_us-1.1.5/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.1.4/openbb_government_us/models/treasury_auctions.py` & `openbb_government_us-1.1.5/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.1.4/openbb_government_us/models/treasury_prices.py` & `openbb_government_us-1.1.5/openbb_government_us/models/treasury_prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""US Government Treasury Prices"""
+"""US Government Treasury Prices."""
 
 # pylint: disable=unused-argument
 import asyncio
 from datetime import datetime, timedelta
 from io import StringIO
 from typing import Any, Dict, List, Literal, Optional
 
@@ -34,20 +34,21 @@
 
 class GovernmentUSTreasuryPricesFetcher(
     Fetcher[
         GovernmentUSTreasuryPricesQueryParams,
         List[GovernmentUSTreasuryPricesData],
     ]
 ):
+    """US Government Treasury Prices Fetcher."""
+
     @staticmethod
     def transform_query(
         params: Dict[str, Any]
     ) -> GovernmentUSTreasuryPricesQueryParams:
         """Transform query params."""
-
         if params.get("date") is None:
             _date = datetime.now().date()
         else:
             _date = (
                 datetime.strptime(params["date"], "%Y-%m-%d").date()
                 if isinstance(params["date"], str)
                 else params["date"]
@@ -62,15 +63,14 @@
     @staticmethod
     async def aextract_data(
         query: GovernmentUSTreasuryPricesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> str:
         """Extract the raw data from US Treasury website."""
-
         url = "https://treasurydirect.gov/GA-FI/FedInvest/securityPriceDetail"
 
         HEADERS = {
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
             "Accept-Language": "en-CA,en-US;q=0.7,en;q=0.3",
             "Accept-Encoding": "gzip, deflate, br",
             "Referer": "https://treasurydirect.gov/",
@@ -106,15 +106,14 @@
     @staticmethod
     def transform_data(
         query: GovernmentUSTreasuryPricesQueryParams,
         data: str,
         **kwargs: Any,
     ) -> List[GovernmentUSTreasuryPricesData]:
         """Transform the data."""
-
         try:
             if not data:
                 raise EmptyDataError("Data not found")
             results = read_csv(StringIO(data), header=0)
             results.columns = Index(
                 [
                     "cusip",
```

### Comparing `openbb_government_us-1.1.4/pyproject.toml` & `openbb_government_us-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "openbb-government-us"
-version = "1.1.4"
+version = "1.1.5"
 description = "US Government Data Extension for OpenBB"
 authors = ["OpenBB <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_government_us" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.1.5"
+openbb-core = "^1.1.6"
 random-user-agent = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
```

### Comparing `openbb_government_us-1.1.4/PKG-INFO` & `openbb_government_us-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-government-us
-Version: 1.1.4
+Version: 1.1.5
 Summary: US Government Data Extension for OpenBB
 Author: OpenBB
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
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Government US Provider
 
 This extension integrates the [US Government](https://data.gov) data provider into the OpenBB Platform.
```

