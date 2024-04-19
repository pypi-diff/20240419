# Comparing `tmp/openbb_benzinga-1.1.4.tar.gz` & `tmp/openbb_benzinga-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_benzinga-1.1.4.tar", max compression
+gzip compressed data, was "openbb_benzinga-1.1.5.tar", max compression
```

## Comparing `openbb_benzinga-1.1.4.tar` & `openbb_benzinga-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      439 2024-02-29 11:03:36.753944 openbb_benzinga-1.1.4/README.md
--rw-r--r--   0        0        0      877 2024-03-21 17:38:35.636625 openbb_benzinga-1.1.4/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754175 openbb_benzinga-1.1.4/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    14906 2024-03-28 17:15:52.365272 openbb_benzinga-1.1.4/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-03-13 16:36:51.636904 openbb_benzinga-1.1.4/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9745 2024-03-14 20:30:27.171935 openbb_benzinga-1.1.4/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-03-13 16:36:51.637143 openbb_benzinga-1.1.4/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754477 openbb_benzinga-1.1.4/openbb_benzinga/py.typed
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754550 openbb_benzinga-1.1.4/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      463 2024-04-01 14:21:35.794640 openbb_benzinga-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_benzinga-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      439 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/README.md
+-rw-r--r--   0        0        0      877 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    17979 2024-04-19 16:31:25.550563 openbb_benzinga-1.1.5/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9801 2024-04-19 16:31:25.550563 openbb_benzinga-1.1.5/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      463 2024-04-19 16:41:36.303279 openbb_benzinga-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_benzinga-1.1.5/PKG-INFO
```

### Comparing `openbb_benzinga-1.1.4/openbb_benzinga/__init__.py` & `openbb_benzinga-1.1.5/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.1.4/openbb_benzinga/models/analyst_search.py` & `openbb_benzinga-1.1.5/openbb_benzinga/models/analyst_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Benzinga Analyst Search Model."""
 
 # pylint: disable=unused-argument
 
-from datetime import datetime
+from datetime import (
+    date as dateType,
+    timezone,
+)
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.analyst_search import (
     AnalystSearchData,
     AnalystSearchQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request, get_querystring
+from openbb_core.provider.utils.helpers import (
+    amake_request,
+    get_querystring,
+    safe_fromtimestamp,
+)
 from pydantic import Field, field_validator, model_validator
-from pytz import UTC
 
 
 class BenzingaAnalystSearchQueryParams(AnalystSearchQueryParams):
     """Benzinga Analyst Search Query.
 
     Source: https://docs.benzinga.io/benzinga-apis/calendar/get-analysts
     """
@@ -141,14 +147,25 @@
     std_dev_1m: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last month",
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="1m_stdev",
     )
+    smart_score_1m: Optional[float] = Field(
+        default=None,
+        description="A weighted average smart score over the last month.",
+        alias="1m_smart_score",
+    )
+    success_rate_1m: Optional[float] = Field(
+        default=None,
+        description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last month",
+        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        alias="1m_success_rate",
+    )
     gain_count_3m: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 3 months",
         alias="3m_gain_count",
     )
     loss_count_3m: Optional[int] = Field(
         default=None,
@@ -165,14 +182,25 @@
     std_dev_3m: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 3 months",
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="3m_stdev",
     )
+    smart_score_3m: Optional[float] = Field(
+        default=None,
+        description="A weighted average smart score over the last 3 months.",
+        alias="3m_smart_score",
+    )
+    success_rate_3m: Optional[float] = Field(
+        default=None,
+        description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 3 months",
+        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        alias="3m_success_rate",
+    )
     gain_count_6m: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 6 months",
         alias="6m_gain_count",
     )
     loss_count_6m: Optional[int] = Field(
         default=None,
@@ -213,14 +241,25 @@
     std_dev_9m: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 9 months",
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="9m_stdev",
     )
+    smart_score_9m: Optional[float] = Field(
+        default=None,
+        description="A weighted average smart score over the last 9 months.",
+        alias="9m_smart_score",
+    )
+    success_rate_9m: Optional[float] = Field(
+        default=None,
+        description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 9 months",
+        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        alias="9m_success_rate",
+    )
     gain_count_1y: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 1 year",
         alias="1y_gain_count",
     )
     loss_count_1y: Optional[int] = Field(
         default=None,
@@ -237,14 +276,25 @@
     std_dev_1y: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 1 year",
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="1y_stdev",
     )
+    smart_score_1y: Optional[float] = Field(
+        default=None,
+        description="A weighted average smart score over the last 1 year.",
+        alias="1y_smart_score",
+    )
+    success_rate_1y: Optional[float] = Field(
+        default=None,
+        description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 1 year",
+        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        alias="1y_success_rate",
+    )
     gain_count_2y: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 2 years",
         alias="2y_gain_count",
     )
     loss_count_2y: Optional[int] = Field(
         default=None,
@@ -261,14 +311,25 @@
     std_dev_2y: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 2 years",
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="2y_stdev",
     )
+    smart_score_2y: Optional[float] = Field(
+        default=None,
+        description="A weighted average smart score over the last 3 years.",
+        alias="2y_smart_score",
+    )
+    success_rate_2y: Optional[float] = Field(
+        default=None,
+        description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 2 years",
+        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        alias="2y_success_rate",
+    )
     gain_count_3y: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 3 years",
         alias="3y_gain_count",
     )
     loss_count_3y: Optional[int] = Field(
         default=None,
@@ -285,22 +346,34 @@
     std_dev_3y: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 3 years",
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="3y_stdev",
     )
+    smart_score_3y: Optional[float] = Field(
+        default=None,
+        description="A weighted average smart score over the last 3 years.",
+        alias="3y_smart_score",
+    )
+    success_rate_3y: Optional[float] = Field(
+        default=None,
+        description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 3 years",
+        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        alias="3y_success_rate",
+    )
 
     @field_validator("last_updated", mode="before", check_fields=False)
     @classmethod
-    def validate_date(cls, v):
+    def validate_date(cls, v: float) -> Optional[dateType]:
+        """Validate last_updated."""
         if v:
-            dt = datetime.fromtimestamp(v, UTC)
+            dt = safe_fromtimestamp(v, tz=timezone.utc)
             return dt.date() if dt.time() == dt.min.time() else dt
-        return v
+        return None
 
     @model_validator(mode="before")
     @classmethod
     def replace_empty_strings(cls, values):
         """Check for empty strings and replace with None."""
         return (
             {k: None if v == "" else v for k, v in values.items()}
@@ -336,15 +409,14 @@
     @staticmethod
     async def aextract_data(
         query: BenzingaAnalystSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the raw data."""
-
         token = credentials.get("benzinga_api_key") if credentials else ""
         querystring = get_querystring(query.model_dump(), [])
         url = f"https://api.benzinga.com/api/v2.1/calendar/ratings/analysts?{querystring}&token={token}"
         response = await amake_request(url, **kwargs)
 
         if not response:
             raise EmptyDataError()
```

### Comparing `openbb_benzinga-1.1.4/openbb_benzinga/models/company_news.py` & `openbb_benzinga-1.1.5/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.1.4/openbb_benzinga/models/price_target.py` & `openbb_benzinga-1.1.5/openbb_benzinga/models/price_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.price_target import (
     PriceTargetData,
     PriceTargetQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_requests, get_querystring
+from openbb_core.provider.utils.helpers import (
+    amake_requests,
+    get_querystring,
+    safe_fromtimestamp,
+)
 from pydantic import Field, field_validator, model_validator
-from pytz import UTC
 
 COVERAGE_DICT = {
     "downgrades": "Downgrades",
     "maintains": "Maintains",
     "reinstates": "Reinstates",
     "reiterates": "Reiterates",
     "upgrades": "Upgrades",
@@ -217,20 +220,20 @@
     @classmethod
     def parse_date(cls, v: str):
         """Parse the publisihed_date."""
         return datetime.strptime(v, "%Y-%m-%d").date() if v else None
 
     @field_validator("last_updated", mode="before", check_fields=False)
     @classmethod
-    def validate_date(cls, v):
+    def validate_date(cls, v: float) -> Optional[dateType]:
         """Convert the Unix timestamp to a datetime object."""
         if v:
-            dt = datetime.fromtimestamp(v, UTC)
+            dt = safe_fromtimestamp(v, tz=timezone.utc)
             return dt.date() if dt.time() == dt.min.time() else dt
-        return v
+        return None
 
     @model_validator(mode="before")
     @classmethod
     def replace_empty_strings(cls, values):
         """Check for empty strings and replace with None."""
         return {k: None if v == "" else v for k, v in values.items()}
```

### Comparing `openbb_benzinga-1.1.4/openbb_benzinga/models/world_news.py` & `openbb_benzinga-1.1.5/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.1.4/PKG-INFO` & `openbb_benzinga-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-benzinga
-Version: 1.1.4
+Version: 1.1.5
 Summary: Benzinga extension for OpenBB
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
 
 # OpenBB Benzinga Provider
 
 This extension integrates the [Benzinga](https://www.benzinga.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

