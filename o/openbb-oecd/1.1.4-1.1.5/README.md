# Comparing `tmp/openbb_oecd-1.1.4.tar.gz` & `tmp/openbb_oecd-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_oecd-1.1.4.tar", max compression
+gzip compressed data, was "openbb_oecd-1.1.5.tar", max compression
```

## Comparing `openbb_oecd-1.1.4.tar` & `openbb_oecd-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.884104 openbb_oecd-1.1.4/README.md
--rw-r--r--   0        0        0      981 2024-03-21 17:38:35.652197 openbb_oecd-1.1.4/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-03-13 16:36:51.763328 openbb_oecd-1.1.4/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-03-13 16:36:51.763472 openbb_oecd-1.1.4/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-03-13 16:36:51.763745 openbb_oecd-1.1.4/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-03-13 16:36:51.763872 openbb_oecd-1.1.4/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-03-13 16:36:51.764186 openbb_oecd-1.1.4/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-03-13 16:36:51.764245 openbb_oecd-1.1.4/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-03-13 16:36:51.764318 openbb_oecd-1.1.4/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-03-13 16:36:51.764590 openbb_oecd-1.1.4/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8668 2024-03-13 16:36:51.764757 openbb_oecd-1.1.4/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0      485 2024-04-01 14:20:33.323389 openbb_oecd-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 openbb_oecd-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/README.md
+-rw-r--r--   0        0        0      981 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0      485 2024-04-19 16:42:30.271413 openbb_oecd-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 openbb_oecd-1.1.5/PKG-INFO
```

### Comparing `openbb_oecd-1.1.4/openbb_oecd/__init__.py` & `openbb_oecd-1.1.5/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/models/composite_leading_indicator.py` & `openbb_oecd-1.1.5/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/models/gdp_forecast.py` & `openbb_oecd-1.1.5/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/models/gdp_nominal.py` & `openbb_oecd-1.1.5/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/models/gdp_real.py` & `openbb_oecd-1.1.5/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/models/long_term_interest_rate.py` & `openbb_oecd-1.1.5/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/models/short_term_interest_rate.py` & `openbb_oecd-1.1.5/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/models/unemployment.py` & `openbb_oecd-1.1.5/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/utils/constants.py` & `openbb_oecd-1.1.5/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.4/openbb_oecd/utils/helpers.py` & `openbb_oecd-1.1.5/openbb_oecd/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""OECD helper functions."""
+
 import ssl
 from datetime import date
 from io import StringIO
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import requests
@@ -16,35 +18,37 @@
 Path(cache).mkdir(parents=True, exist_ok=True)
 
 # OECD does not play well with newer python.  This code block from stackoverflow helps
 # to create a custom session:
 
 
 class CustomHttpAdapter(requests.adapters.HTTPAdapter):
-    # "Transport adapter" that allows us to use custom ssl_context.
+    """Transport adapter" that allows us to use custom ssl_context."""
 
     def __init__(self, ssl_context=None, **kwargs):
+        """Initialize the adapter with a custom ssl_context."""
         self.ssl_context = ssl_context
         super().__init__(**kwargs)
 
     # pylint: disable=arguments-differ
     def init_poolmanager(self, connections, maxsize, block=False):
+        """Initialize the poolmanager with a custom ssl_context."""
         self.poolmanager = urllib3.poolmanager.PoolManager(  # pylint: disable=attribute-defined-outside-init
             num_pools=connections,
             maxsize=maxsize,
             block=block,
             ssl_context=self.ssl_context,
         )
 
 
 # pylint: enable=arguments-differ
 
 
 def get_legacy_session():
-    """Stackoverflow code to create a custom session."""
+    """Create a custom session."""
     ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
     ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
     session = requests.Session()
     session.mount("https://", CustomHttpAdapter(ctx))
     return session
 
 
@@ -60,17 +64,17 @@
     return data
 
 
 ### The functions below are for using the new oecd data-explorer instead of the stats.oecd
 
 
 def oecd_xml_to_df(xml_string: str) -> DataFrame:
-    """Helper function to parse the OECD XML and return a dataframe.
+    """Parse the OECD XML and return a dataframe.
 
-     Parameters
+    Parameters
     ----------
     xml_string : str
         A string containing the OECD XML data.
 
     Returns
     -------
     DataFrame
@@ -104,15 +108,15 @@
             data.append(obs_data)
 
     # Create a DataFrame
     return DataFrame(data)
 
 
 def parse_url(url: str) -> DataFrame:
-    """Helper function to parse the SDMX url and return a dataframe.
+    """Parse the SDMX url and return a dataframe.
 
     Parameters
     ----------
     url:str
         URL to parse
 
     Returns
@@ -189,29 +193,28 @@
         with open(f"{cache_str}.timestamp", "w") as f:
             f.write(str(date.today()))
     else:
         raise NotImplementedError
 
 
 def query_dict_to_path(query_dict: dict) -> str:
-    """Convert the query dict into something usable for writing file"""
+    """Convert the query dict into something usable for writing file."""
     items = sorted(query_dict.items())
     key_parts = [f"{key}_{value}" for key, value in items]
     return "-".join(key_parts).replace("/", "_").replace(" ", "_")
 
 
 def get_possibly_cached_data(
     url: str,
     function: Optional[str] = None,
     query_dict: Optional[dict] = None,
     cache_method: str = "csv",
     skip_cache: bool = False,
 ) -> DataFrame:
-    """
-    Retrieve data from a given URL or from the cache if available and valid.
+    """Retrieve data from a given URL or from the cache if available and valid.
 
     Parameters
     ----------
     url : str
         The URL from which to fetch the data if it's not available in the cache.
     function : Optional[str], optional
         The name of the function for which data is being fetched or cached.
@@ -221,16 +224,17 @@
         The method used for caching the data (default is 'csv').
 
     Returns
     -------
     DataFrame
         A Pandas DataFrame containing the fetched or cached data.
     """
-
-    base_cache = f"{cache}/{function}_{query_dict_to_path(query_dict)}"
+    base_cache = (
+        f"{cache}/{function}_{query_dict_to_path(query_dict if query_dict else {})}"
+    )
     if cache_method == "parquet":
         cache_path = base_cache + ".parquet"
     elif cache_method == "csv":
         cache_path = base_cache + ".csv"
 
     use_cache = check_cache_exists_and_valid(
         cache_str=base_cache, cache_method=cache_method
@@ -244,15 +248,15 @@
         data = parse_url(url)
         if not skip_cache:
             write_to_cache(cache_str=base_cache, data=data, cache_method=cache_method)
     return data
 
 
 def oecd_date_to_python_date(input_date: Union[str, int]) -> date:
-    """Darrens good idea to make the dates filterable"""
+    """Use Darrens good idea to make the dates filterable."""
     input_date = str(input_date)
     if "Q" in input_date:
         return to_datetime(input_date).to_period("Q").to_timestamp("Q").date()
     if len(input_date) == 4:
         return date(int(input_date), 12, 31)
     if len(input_date) == 7:
         return to_datetime(input_date).to_period("M").to_timestamp("M").date()
```

### Comparing `openbb_oecd-1.1.4/PKG-INFO` & `openbb_oecd-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: openbb-oecd
-Version: 1.1.4
+Version: 1.1.5
 Summary: OECD extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: defusedxml (>=0.8.0rc2,<0.9.0)
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Requires-Dist: urllib3 (>1.26.16)
 Description-Content-Type: text/markdown
```

