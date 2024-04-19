# Comparing `tmp/openbb_finra-1.1.4.tar.gz` & `tmp/openbb_finra-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_finra-1.1.4.tar", max compression
+gzip compressed data, was "openbb_finra-1.1.5.tar", max compression
```

## Comparing `openbb_finra-1.1.4.tar` & `openbb_finra-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      423 2024-02-29 11:03:36.800341 openbb_finra-1.1.4/README.md
--rw-r--r--   0        0        0      538 2024-03-21 17:38:35.639158 openbb_finra-1.1.4/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-03-13 16:36:51.707780 openbb_finra-1.1.4/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-03-13 16:36:51.707928 openbb_finra-1.1.4/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-03-13 16:36:51.708062 openbb_finra-1.1.4/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5360 2024-02-29 11:03:36.800831 openbb_finra-1.1.4/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0      445 2024-04-01 14:20:22.391752 openbb_finra-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 openbb_finra-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      423 2024-04-17 12:33:20.605645 openbb_finra-1.1.5/README.md
+-rw-r--r--   0        0        0      538 2024-04-17 12:33:20.605645 openbb_finra-1.1.5/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-04-17 12:33:20.605645 openbb_finra-1.1.5/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-04-17 12:33:20.605645 openbb_finra-1.1.5/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-04-17 12:33:20.605645 openbb_finra-1.1.5/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-04-17 12:33:20.605645 openbb_finra-1.1.5/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0      445 2024-04-19 16:42:01.087339 openbb_finra-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 openbb_finra-1.1.5/PKG-INFO
```

### Comparing `openbb_finra-1.1.4/openbb_finra/__init__.py` & `openbb_finra-1.1.5/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.4/openbb_finra/models/equity_short_interest.py` & `openbb_finra-1.1.5/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.4/openbb_finra/models/otc_aggregate.py` & `openbb_finra-1.1.5/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.4/openbb_finra/utils/data_storage.py` & `openbb_finra-1.1.5/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.4/openbb_finra/utils/helpers.py` & `openbb_finra-1.1.5/openbb_finra/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# Helper functions for FINRA API
+"""Helper functions for FINRA API."""
+
 import datetime
 from typing import List
 
 import requests
 
+# pylint: disable=W0621
+
 
 def get_finra_weeks(tier: str = "T1", is_ats: bool = True):
-    """Fetches the available weeks from FINRA that can be used."""
+    """Fetch the available weeks from FINRA that can be used."""
     request_header = {"Accept": "application/json", "Content-Type": "application/json"}
 
     request_data = {
         "compareFilters": [
             {
                 "compareType": "EQUAL",
                 "fieldName": "summaryTypeCode",
@@ -36,14 +39,15 @@
         timeout=3,
     )
 
     return response.json() if response.status_code == 200 else []
 
 
 def get_finra_data(symbol, week_start, tier: str = "T1", is_ats: bool = True):
+    """Get the data for a symbol from FINRA."""
     req_hdr = {
         "Accept": "application/json",
         "Content-Type": "application/json",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) ",
     }
 
     filters = [
@@ -89,48 +93,51 @@
         json=req_data,
         timeout=2,
     )
     return response
 
 
 def get_full_data(symbol, tier: str = "T1", is_ats: bool = True):
+    """Get the full data for a symbol from FINRA."""
     weeks = [week["weekStartDate"] for week in get_finra_weeks(tier, is_ats)]
 
     data = []
     for week in weeks:
         response = get_finra_data(symbol, week, tier, is_ats)
         r_json = response.json()
         if response.status_code == 200 and r_json:
             data.append(response.json()[0])
 
     return data
 
 
 def get_adjusted_date(year, month, day):
+    """Find the closest date if the date falls on a weekend."""
     # Get the date
     date = datetime.date(year, month, day)
 
     # If the date is a Saturday, subtract one day
     if date.weekday() == 5:
         date -= datetime.timedelta(days=1)
     # If the date is a Sunday, subtract two days
     elif date.weekday() == 6:
         date -= datetime.timedelta(days=2)
 
     return date
 
 
 def get_short_interest_dates() -> List[str]:
-    """
-    Get a list of dates for which the short interest data is available.  It is reported on the 15th and the
-    last day of each month,but if the date falls on a weekend, the date is adjusted to the closest friday.
+    """Get a list of dates for which the short interest data is available.
+
+    It is reported on the 15th and the last day of each month,but if the date falls on a weekend,
+    the date is adjusted to the closest friday.
     """
 
     def get_adjusted_date(year, month, day):
-        """If the date falls on a weekend, find the closest date"""
+        """Find the closest date if the date falls on a weekend."""
         # Get the date
         date = datetime.date(year, month, day)
 
         # If the date is a Saturday, subtract one day
         if date.weekday() == 5:
             date -= datetime.timedelta(days=1)
         # If the date is a Sunday, subtract two days
```

### Comparing `openbb_finra-1.1.4/PKG-INFO` & `openbb_finra-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-finra
-Version: 1.1.4
+Version: 1.1.5
 Summary: FINRA extension for OpenBB
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
 
 # OpenBB FINRA Provider
 
 This extension integrates the [FINRA](https://finra.org/) data provider into the OpenBB Platform.
 
 ## Installation
```

