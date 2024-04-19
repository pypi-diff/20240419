# Comparing `tmp/openbb_tradingeconomics-1.1.4.tar.gz` & `tmp/openbb_tradingeconomics-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradingeconomics-1.1.4.tar", max compression
+gzip compressed data, was "openbb_tradingeconomics-1.1.5.tar", max compression
```

## Comparing `openbb_tradingeconomics-1.1.4.tar` & `openbb_tradingeconomics-1.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      469 2024-02-29 11:03:36.974304 openbb_tradingeconomics-1.1.4/README.md
--rw-r--r--   0        0        0      440 2024-03-21 17:38:35.661271 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4529 2024-03-13 16:36:51.898559 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4567 2024-03-13 16:36:51.898679 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3636 2024-03-13 16:36:51.898787 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0      512 2024-04-01 14:21:45.210039 openbb_tradingeconomics-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      469 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/README.md
+-rw-r--r--   0        0        0      440 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     4606 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0      512 2024-04-19 16:43:06.055506 openbb_tradingeconomics-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.1.5/PKG-INFO
```

### Comparing `openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
             check_item(v.lower(), COUNTRIES)
             result.append(v.lower())
         return ",".join(result)
 
     @field_validator("importance")
     @classmethod
     def importance_to_number(cls, v):
+        """Convert importance to number."""
         string_to_value = {"Low": 1, "Medium": 2, "High": 3}
         return string_to_value.get(v, None)
 
 
 class TEEconomicCalendarData(EconomicCalendarData):
     """Trading Economics Economic Calendar Data."""
 
@@ -89,14 +90,15 @@
         "previous": "Previous",
         "revised": "Revised",
     }
 
     @field_validator("date", mode="before")
     @classmethod
     def validate_date(cls, v: str) -> datetime:
+        """Validate the date."""
         return to_datetime(v, utc=True)
 
 
 class TEEconomicCalendarFetcher(
     Fetcher[
         TEEconomicCalendarQueryParams,
         List[TEEconomicCalendarData],
```

### Comparing `openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/countries.py` & `openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/countries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Countries list for Trading Economics API."""
+
 country_dict = {
     "G20": [
         "United States",
         "Euro Area",
         "China",
         "Japan",
         "Germany",
```

### Comparing `openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/url_generator.py` & `openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/url_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from datetime import date
 from typing import Dict, List
 from urllib.parse import quote, urlencode
 
 
 def check_args(query_args: Dict, to_include: List[str]):
+    """Check if all fields in to_include are present in query_args."""
     available_args = ["country", "start_date", "end_date", "importance", "group"]
 
     # Check if all fields in to_include are present in query_args
     # and elements in available_args that are not in to_include are not present in query_args
     return all(field in query_args for field in to_include) and all(
         field not in query_args for field in available_args if field not in to_include
     )
 
 
 def generate_url(in_query):
-    """
-    Generate the url for trading economimcs.  There is not a single api endpoint to hit so these are
-    generated based on the combinations.  There are also some combinations that return no data so that will return ""
+    """Generate the url for trading economimcs.
+
+    There is not a single api endpoint to hit so these are generated based on the combinations.
+    There are also some combinations that return no data so that will return an empty string.
     """
     # Converting the input query to a dict of params that are not None
     query = {k: v for k, v in in_query.dict().items() if v is not None}
 
     # Nothing -- just a snapshot
     if not query:
         return "https://api.tradingeconomics.com/calendar?c="
```

### Comparing `openbb_tradingeconomics-1.1.4/pyproject.toml` & `openbb_tradingeconomics-1.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "openbb-tradingeconomics"
-version = "1.1.4"
+version = "1.1.5"
 description = "Trading Economics extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_tradingeconomics" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.1.5"
+openbb-core = "^1.1.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tradingeconomics = "openbb_tradingeconomics:tradingeconomics_provider"
```

### Comparing `openbb_tradingeconomics-1.1.4/PKG-INFO` & `openbb_tradingeconomics-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-tradingeconomics
-Version: 1.1.4
+Version: 1.1.5
 Summary: Trading Economics extension for OpenBB
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
 
 # OpenBB Trading Economics Provider
 
 This extension integrates the [Trading Economics](https://docs.tradingeconomics.com/) data provider into the OpenBB SDK.
 
 ## Installation
```

