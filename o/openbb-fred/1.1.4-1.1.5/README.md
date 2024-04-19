# Comparing `tmp/openbb_fred-1.1.4.tar.gz` & `tmp/openbb_fred-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fred-1.1.4.tar", max compression
+gzip compressed data, was "openbb_fred-1.1.5.tar", max compression
```

## Comparing `openbb_fred-1.1.4.tar` & `openbb_fred-1.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      444 2024-02-29 11:03:36.865850 openbb_fred-1.1.4/README.md
--rw-r--r--   0        0        0     3126 2024-03-21 17:38:35.646889 openbb_fred-1.1.4/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-02-29 11:03:36.866196 openbb_fred-1.1.4/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-02-29 11:03:36.866284 openbb_fred-1.1.4/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-03-13 16:36:51.737518 openbb_fred-1.1.4/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-03-13 16:36:51.737624 openbb_fred-1.1.4/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-02-29 11:03:36.866494 openbb_fred-1.1.4/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-02-29 11:03:36.866551 openbb_fred-1.1.4/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-02-29 11:03:36.866626 openbb_fred-1.1.4/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-02-29 11:03:36.866706 openbb_fred-1.1.4/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-02-29 11:03:36.866781 openbb_fred-1.1.4/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-03-13 16:36:51.737725 openbb_fred-1.1.4/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-02-29 11:03:36.866951 openbb_fred-1.1.4/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-02-29 11:03:36.867021 openbb_fred-1.1.4/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-02-29 11:03:36.867092 openbb_fred-1.1.4/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-03-13 16:36:51.737806 openbb_fred-1.1.4/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-03-13 16:36:51.737921 openbb_fred-1.1.4/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6312 2024-03-19 14:52:38.489944 openbb_fred-1.1.4/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-02-29 11:03:36.867365 openbb_fred-1.1.4/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-02-29 11:03:36.867442 openbb_fred-1.1.4/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-03-13 16:36:51.738119 openbb_fred-1.1.4/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-02-29 11:03:36.867578 openbb_fred-1.1.4/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-02-29 11:03:36.867653 openbb_fred-1.1.4/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-02-29 11:03:36.867734 openbb_fred-1.1.4/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-02-29 11:03:36.867879 openbb_fred-1.1.4/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-02-29 11:03:36.868080 openbb_fred-1.1.4/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-02-29 11:03:36.868229 openbb_fred-1.1.4/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-03-13 16:36:51.738236 openbb_fred-1.1.4/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-03-13 16:36:51.738365 openbb_fred-1.1.4/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-02-29 11:03:36.868524 openbb_fred-1.1.4/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-02-29 11:03:36.868834 openbb_fred-1.1.4/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      439 2024-04-01 14:20:11.129481 openbb_fred-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_fred-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      444 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/README.md
+-rw-r--r--   0        0        0     3126 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-04-19 13:10:31.748034 openbb_fred-1.1.5/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6338 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6656 2024-04-19 13:10:31.748034 openbb_fred-1.1.5/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      439 2024-04-19 16:41:03.859203 openbb_fred-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_fred-1.1.5/PKG-INFO
```

### Comparing `openbb_fred-1.1.4/openbb_fred/__init__.py` & `openbb_fred-1.1.5/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/ameribor_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/cp.py` & `openbb_fred-1.1.5/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/cpi.py` & `openbb_fred-1.1.5/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/dwpcr_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/ecb_interest_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/estr_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/fed_projections.py` & `openbb_fred-1.1.5/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/fed_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/ffrmc.py` & `openbb_fred-1.1.5/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/hqm.py` & `openbb_fred-1.1.5/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/ice_bofa.py` & `openbb_fred-1.1.5/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/iorb_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/moody.py` & `openbb_fred-1.1.5/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/regional.py` & `openbb_fred-1.1.5/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/search.py` & `openbb_fred-1.1.5/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/series.py` & `openbb_fred-1.1.5/openbb_fred/models/series.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """FRED Series Model."""
 
-import json
-import warnings
 from typing import Any, Dict, List, Literal, Optional
 
 import pandas as pd
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.fred_series import (
     SeriesData,
     SeriesQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
     get_querystring,
 )
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FredSeriesQueryParams(SeriesQueryParams):
     """FRED Series Query Params."""
 
     __alias_dict__ = {
         "symbol": "series_id",
         "start_date": "observation_start",
@@ -141,17 +138,26 @@
             observations_response = await response.json()
             series_id = response.url.query.get("series_id")
 
             metadata_response = await session.get_json(
                 f"{metadata_url}?series_id={series_id}&file_type=json&api_key={api_key}",
                 timeout=5,
             )
-            _metadata = metadata_response.get("seriess", [{}])[0]
 
-            observations = observations_response.get("observations")
+            # seriess is not a typo, it's the actual key in the response
+            _metadata = (
+                metadata_response.get("seriess", [{}])[0]
+                if isinstance(metadata_response, dict)
+                else {}
+            ) or {}
+            observations = (
+                observations_response.get("observations")
+                if isinstance(observations_response, dict)
+                else []
+            ) or []
             try:
                 for d in observations:
                     d.pop("realtime_start")
                     d.pop("realtime_end")
 
                 data = (
                     pd.DataFrame(observations)
@@ -173,33 +179,28 @@
                     "notes": _metadata.get("notes"),
                     "data": data,
                 }
             }
 
         results = await amake_requests(urls, callback, timeout=5, **kwargs)
 
-        metadata, data = {}, {}
-        for item in results:
-            for series_id, result in item.items():
-                data[series_id] = result.pop("data")
-                metadata[series_id] = result
-
-        _warn(json.dumps(metadata))
-
-        return data
+        return results
 
     # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
-        query: FredSeriesQueryParams, data: Dict, **kwargs: Any
-    ) -> List[FredSeriesData]:
+        query: FredSeriesQueryParams, data: List[Dict[str, Any]], **kwargs: Any
+    ) -> AnnotatedResult[List[FredSeriesData]]:
         """Transform data."""
-        results = (
-            pd.DataFrame(data)
+        series = {_id: s.pop("data", {}) for d in data for _id, s in d.items()}
+        metadata = {_id: m for d in data for _id, m in d.items()}
+        records = (
+            pd.DataFrame(series)
             .filter(items=query.symbol.split(","), axis=1)
             .reset_index()
             .rename(columns={"index": "date"})
             .fillna("N/A")
             .replace("N/A", None)
             .to_dict("records")
         )
-        return [FredSeriesData.model_validate(d) for d in results]
+        validated = [FredSeriesData.model_validate(r) for r in records]
+        return AnnotatedResult(result=validated, metadata=metadata)
```

### Comparing `openbb_fred-1.1.4/openbb_fred/models/sofr_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/sonia_rates.py` & `openbb_fred-1.1.5/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/spot.py` & `openbb_fred-1.1.5/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/tbffr.py` & `openbb_fred-1.1.5/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/tmc.py` & `openbb_fred-1.1.5/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/models/us_yield_curve.py` & `openbb_fred-1.1.5/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/utils/commercial_paper.csv` & `openbb_fred-1.1.5/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_fred-1.1.5/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/utils/cpi.csv` & `openbb_fred-1.1.5/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/utils/fred_base.py` & `openbb_fred-1.1.5/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/utils/fred_helpers.py` & `openbb_fred-1.1.5/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/utils/harmonized_cpi.csv` & `openbb_fred-1.1.5/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_fred-1.1.5/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.4/PKG-INFO` & `openbb_fred-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-fred
-Version: 1.1.4
+Version: 1.1.5
 Summary: FRED extension for OpenBB
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
 
 # OpenBB FRED Provider
 
 This extension integrates the [FRED](https://fred.stlouisfed.org/docs/api/fred/) data provider into the OpenBB Platform.
 
 ## Installation
```

