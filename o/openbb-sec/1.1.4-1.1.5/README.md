# Comparing `tmp/openbb_sec-1.1.4.tar.gz` & `tmp/openbb_sec-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_sec-1.1.4.tar", max compression
+gzip compressed data, was "openbb_sec-1.1.5.tar", max compression
```

## Comparing `openbb_sec-1.1.4.tar` & `openbb_sec-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      424 2024-02-29 11:03:36.896002 openbb_sec-1.1.4/README.md
--rw-r--r--   0        0        0     1562 2024-03-21 17:38:35.653641 openbb_sec-1.1.4/openbb_sec/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896154 openbb_sec-1.1.4/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-03-21 17:38:35.653808 openbb_sec-1.1.4/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8277 2024-03-21 17:38:35.653936 openbb_sec-1.1.4/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2617 2024-03-21 17:38:35.654048 openbb_sec-1.1.4/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-03-21 17:38:35.654140 openbb_sec-1.1.4/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-03-21 17:38:35.654328 openbb_sec-1.1.4/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-03-21 17:38:35.654598 openbb_sec-1.1.4/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-03-21 17:38:35.654754 openbb_sec-1.1.4/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.779245 openbb_sec-1.1.4/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-03-21 17:38:35.654871 openbb_sec-1.1.4/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-03-21 17:38:35.655006 openbb_sec-1.1.4/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-03-21 17:38:35.655140 openbb_sec-1.1.4/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-03-21 17:38:35.655251 openbb_sec-1.1.4/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896831 openbb_sec-1.1.4/openbb_sec/py.typed
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896870 openbb_sec-1.1.4/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-02-29 11:03:36.896953 openbb_sec-1.1.4/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13834 2024-03-21 17:38:35.655553 openbb_sec-1.1.4/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7410 2024-03-21 17:38:35.655723 openbb_sec-1.1.4/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.780521 openbb_sec-1.1.4/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      516 2024-04-01 14:20:00.173560 openbb_sec-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 openbb_sec-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      424 2024-04-17 12:33:20.697645 openbb_sec-1.1.5/README.md
+-rw-r--r--   0        0        0     1562 2024-04-17 12:33:20.697645 openbb_sec-1.1.5/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0     8328 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     2615 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2720 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    32406 2024-04-19 13:10:31.748034 openbb_sec-1.1.5/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2754 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2079 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2790 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3009 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1714 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    13896 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7434 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      516 2024-04-19 16:42:10.779363 openbb_sec-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 openbb_sec-1.1.5/PKG-INFO
```

### Comparing `openbb_sec-1.1.4/openbb_sec/__init__.py` & `openbb_sec-1.1.5/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/cik_map.py` & `openbb_sec-1.1.5/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/company_filings.py` & `openbb_sec-1.1.5/openbb_sec/models/company_filings.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,31 +141,31 @@
 
     @staticmethod
     def extract_data(
         query: SecCompanyFilingsQueryParams,  # pylint: disable=unused-argument
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Extracts the data from the SEC endpoint."""
+        """Extract the data from the SEC endpoint."""
         filings = pd.DataFrame()
 
         if query.symbol and not query.cik:
             query.cik = symbol_map(query.symbol.lower(), use_cache=query.use_cache)
             if not query.cik:
                 return []
         if query.cik is None:
             return []
 
         # The leading 0s need to be inserted but are typically removed from the data to store as an integer.
-        if len(query.cik) != 10:
+        if len(query.cik) != 10:  # type: ignore
             cik_: str = ""
-            temp = 10 - len(query.cik)
+            temp = 10 - len(query.cik)  # type: ignore
             for i in range(temp):
                 cik_ = cik_ + "0"
-            query.cik = cik_ + query.cik
+            query.cik = cik_ + str(query.cik)  # type: ignore
 
         url = f"https://data.sec.gov/submissions/CIK{query.cik}.json"
         r = (
             requests.get(url, headers=HEADERS, timeout=5)
             if query.use_cache is False
             else sec_session_company_filings.get(url, headers=HEADERS, timeout=5)
         )
@@ -232,9 +232,9 @@
 
         return filings.to_dict("records")
 
     @staticmethod
     def transform_data(
         query: SecCompanyFilingsQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecCompanyFilingsData]:
-        """Transforms the data."""
+        """Transform the data."""
         return [SecCompanyFilingsData.model_validate(d) for d in data]
```

### Comparing `openbb_sec-1.1.4/openbb_sec/models/equity_ftd.py` & `openbb_sec-1.1.5/openbb_sec/models/equity_ftd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     @staticmethod
     def extract_data(
         query: SecEquityFtdQueryParams,  # pylint: disable=unused-argument
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Extracts the data from the SEC website."""
+        """Extract the data from the SEC website."""
         results = []
         limit = query.limit if query.limit is not None and query.limit > 0 else 0
         symbol = query.symbol.upper()
 
         urls_data = get_ftd_urls()
         urls = list(urls_data.values())
         if limit > 0:
@@ -79,9 +79,9 @@
 
         return results
 
     @staticmethod
     def transform_data(
         query: SecEquityFtdQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecEquityFtdData]:
-        """Transforms the data to the standard format."""
+        """Transform the data to the standard format."""
         return [SecEquityFtdData.model_validate(d) for d in data]
```

### Comparing `openbb_sec-1.1.4/openbb_sec/models/equity_search.py` & `openbb_sec-1.1.5/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/etf_holdings.py` & `openbb_sec-1.1.5/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/form_13FHR.py` & `openbb_sec-1.1.5/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/institutions_search.py` & `openbb_sec-1.1.5/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/rss_litigation.py` & `openbb_sec-1.1.5/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/schema_files.py` & `openbb_sec-1.1.5/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/sic_search.py` & `openbb_sec-1.1.5/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/models/symbol_map.py` & `openbb_sec-1.1.5/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/utils/definitions.py` & `openbb_sec-1.1.5/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.4/openbb_sec/utils/helpers.py` & `openbb_sec-1.1.5/openbb_sec/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""SEC Helpers module"""
+"""SEC Helpers module."""
 
 # pylint: skip-file
 from datetime import timedelta
 from io import BytesIO
 from typing import Dict, List, Optional
 from zipfile import ZipFile
 
@@ -26,42 +26,41 @@
 
 sec_session_company_filings = requests_cache.CachedSession(
     f"{cache_dir}/http/sec_company_filings", expire_after=timedelta(days=1)
 )
 
 
 def get_all_companies(use_cache: bool = True) -> pd.DataFrame:
-    """Gets all company names, tickers, and CIK numbers registered with the SEC.
+    """Get all company names, tickers, and CIK numbers registered with the SEC.
+
     Companies are sorted by market cap.
 
     Returns
     -------
     pd.DataFrame: Pandas DataFrame with columns for Symbol, Company Name, and CIK Number.
 
     Example
     -------
     >>> tickers = get_all_companies()
     """
-
     url = "https://www.sec.gov/files/company_tickers.json"
 
     r = (
         sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
         if use_cache is True
         else requests.get(url, headers=SEC_HEADERS, timeout=5)
     )
     df = pd.DataFrame(r.json()).transpose()
     cols = ["cik", "symbol", "name"]
     df.columns = cols
     return df.astype(str)
 
 
 def get_all_ciks(use_cache: bool = True) -> pd.DataFrame:
-    """Gets a list of entity names and their CIK number."""
-
+    """Get a list of entity names and their CIK number."""
     HEADERS = {
         "User-Agent": "my real company name definitelynot@fakecompany.com",
         "Accept-Encoding": "gzip, deflate",
         "Host": "www.sec.gov",
     }
     url = "https://www.sec.gov/Archives/edgar/cik-lookup-data.txt"
     r = (
@@ -82,16 +81,15 @@
     df.columns = cols
     df = df.dropna()
 
     return df
 
 
 def get_mf_and_etf_map(use_cache: bool = True) -> pd.DataFrame:
-    """Returns the CIK number of a ticker symbol for querying the SEC API."""
-
+    """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbols = pd.DataFrame()
 
     url = "https://www.sec.gov/files/company_tickers_mf.json"
     r = (
         sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
         if use_cache is True
         else requests.get(url, headers=SEC_HEADERS, timeout=5)
@@ -106,16 +104,15 @@
     """Search for an institution by name.  It is case-insensitive."""
     institutions = get_all_ciks(use_cache=use_cache)
     hp = institutions["Institution"].str.contains(keyword, case=False)
     return institutions[hp].astype(str)
 
 
 def symbol_map(symbol: str, use_cache: bool = True) -> str:
-    """Returns the CIK number of a ticker symbol for querying the SEC API."""
-
+    """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbol = symbol.upper().replace(".", "-")
     symbols = get_all_companies(use_cache=use_cache)
 
     if symbol not in symbols["symbol"].to_list():
         symbols = get_mf_and_etf_map(use_cache=use_cache).astype(str)
         if symbol not in symbols["symbol"].to_list():
             return ""
@@ -126,16 +123,15 @@
     for i in range(temp):
         cik_ = cik_ + "0"
 
     return str(cik_ + cik)
 
 
 def cik_map(cik: int, use_cache: bool = True) -> str:
-    """
-    Converts a CIK number to a ticker symbol.  Enter CIK as an integer with no leading zeros.
+    """Convert a CIK number to a ticker symbol.  Enter CIK as an integer with no leading zeros.
 
     Function is not meant for funds.
 
     Parameters
     ----------
     cik : int
         The CIK number to convert to a ticker symbol.
@@ -160,15 +156,16 @@
     quarter: Optional[QUARTERS] = None,
     taxonomy: TAXONOMIES = "us-gaap",
     units: str = "USD",
     fact: str = "Revenues",
     instantaneous: bool = False,
     use_cache: bool = True,
 ) -> Dict:
-    """
+    """Get a frame of data for a given fact.
+
     The xbrl/frames API aggregates one fact for each reporting entity
     that is last filed that most closely fits the calendrical period requested.
 
     This API supports for annual, quarterly and instantaneous data:
 
     https://data.sec.gov/api/xbrl/frames/us-gaap/AccountsPayableCurrent/USD/CY2019Q1I.json
 
@@ -193,15 +190,14 @@
     InterestAndDebtExpense
     IncomeTaxExpenseBenefit
     NetIncomeLoss
 
     Facts where units are, "shares":
     WeightedAverageNumberOfDilutedSharesOutstanding
     """
-
     if fact in ["WeightedAverageNumberOfDilutedSharesOutstanding"]:
         units = "shares"
 
     url = f"https://data.sec.gov/api/xbrl/frames/{taxonomy}/{fact}/{units}/CY{year}"
 
     if quarter:
         url = url + f"Q{quarter}"
@@ -233,14 +229,15 @@
 
     results = {"metadata": metadata, "data": data}
 
     return results
 
 
 def get_schema_filelist(query: str = "", url: str = "") -> List:
+    """Get a list of schema files from the SEC website."""
     results: List = []
     url = url if url else f"https://xbrl.fasb.org/us-gaap/{query}"
     _url = url
     _url = url + "/" if query else _url
     r = sec_session_companies.get(_url, headers=HEADERS, timeout=5)
 
     if r.status_code != 200:
@@ -296,15 +293,14 @@
             results["price"] = results["price"].astype(float)
 
     return results.reset_index(drop=True).to_dict("records")
 
 
 def get_ftd_urls() -> Dict:
     """Get Fails-to-Deliver Data URLs."""
-
     results = {}
     position = None
     key = "title"
     value = "Fails-to-Deliver Data"
 
     r = requests.get("https://www.sec.gov/data.json", timeout=5, headers=SEC_HEADERS)
     if r.status_code != 200:
@@ -326,16 +322,16 @@
 
     return results
 
 
 def get_series_id(
     symbol: Optional[str] = None, cik: Optional[str] = None, use_cache: bool = True
 ):
-    """
-    This function maps the fund to the series and class IDs for validating the correct filing.
+    """Map the fund to the series and class IDs for validating the correct filing.
+
     For an exact match, use a symbol.
     """
     symbol = symbol if symbol else ""
     cik = cik if cik else ""
 
     results = pd.DataFrame()
     if not symbol and not cik:
@@ -355,16 +351,15 @@
     if len(results) > 0:
         results = results[results[choice if not symbol else choice] == target]
 
         return results
 
 
 def get_nport_candidates(symbol: str, use_cache: bool = True) -> List[Dict]:
-    """Gets a list of all NPORT-P filings for a given fund's symbol."""
-
+    """Get a list of all NPORT-P filings for a given fund's symbol."""
     results = []
     _series_id = get_series_id(symbol, use_cache=use_cache)
     try:
         series_id = (
             symbol_map(symbol, use_cache)
             if _series_id is None or len(_series_id) == 0
             else _series_id["seriesId"].iloc[0]
```

### Comparing `openbb_sec-1.1.4/openbb_sec/utils/parse_13f.py` & `openbb_sec-1.1.5/openbb_sec/utils/parse_13f.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Utility functions for parsing SEC Form 13F-HR."""
 
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
 
 import xmltodict
 from bs4 import BeautifulSoup
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_sec.models.company_filings import SecCompanyFilingsFetcher
 from openbb_sec.utils.definitions import HEADERS
 from pandas import DataFrame, offsets, to_datetime
@@ -18,15 +18,15 @@
         .strftime("%Y-%m-%d")
     )
 
 
 def get_13f_candidates(symbol: Optional[str] = None, cik: Optional[str] = None):
     """Get the 13F-HR filings for a given symbol or CIK."""
     fetcher = SecCompanyFilingsFetcher()
-    params = {}
+    params: Dict[str, Any] = {}
     if cik is not None:
         params["cik"] = str(cik)
     if symbol is not None:
         params["symbol"] = symbol
     if cik is None and symbol is None:
         raise ValueError("Either symbol or cik must be provided.")
 
@@ -42,15 +42,15 @@
         DataFrame(data=filings)
         .query("`reportDate` >= '2013-06-30'")
         .set_index("reportDate")["completeSubmissionUrl"]
     )
 
 
 async def complete_submission_callback(response, _):
-    """Callback function for processing the response object."""
+    """Use callback function for processing the response object."""
     if response.status == 200:
         return await response.text()
     raise RuntimeError(f"Request failed with status code {response.status}")
 
 
 async def get_complete_submission(url: str):
     """Get the Complete Submission TXT file string from the SEC API."""
@@ -102,15 +102,15 @@
     raise ValueError(
         "Failed to get the period of report from the form header."
         + " Check the response from `parse_header`."
     )
 
 
 async def parse_13f_hr(filing: str):
-    """Parses a 13F-HR filing from the Complete Submission TXT file string."""
+    """Parse a 13F-HR filing from the Complete Submission TXT file string."""
     data = DataFrame()
 
     # Check if the input string is a URL
     if filing.startswith("https://"):
         filing = await get_complete_submission(filing)  # type: ignore
 
     # Validate the submission so we know that we can parse it.
```

### Comparing `openbb_sec-1.1.4/pyproject.toml` & `openbb_sec-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "openbb-sec"
-version = "1.1.4"
+version = "1.1.5"
 description = "SEC extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_sec" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-openbb-core = "^1.1.5"
+openbb-core = "^1.1.6"
 requests-cache = "^1.1.0"
 xmltodict = "^0.13.0"
 pytest-freezegun = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openbb_sec-1.1.4/PKG-INFO` & `openbb_sec-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-sec
-Version: 1.1.4
+Version: 1.1.5
 Summary: SEC extension for OpenBB
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
 Requires-Dist: pytest-freezegun (>=0.4.2,<0.5.0)
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # OpenBB SEC Provider
```

