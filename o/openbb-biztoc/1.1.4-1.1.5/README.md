# Comparing `tmp/openbb_biztoc-1.1.4.tar.gz` & `tmp/openbb_biztoc-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_biztoc-1.1.4.tar", max compression
+gzip compressed data, was "openbb_biztoc-1.1.5.tar", max compression
```

## Comparing `openbb_biztoc-1.1.4.tar` & `openbb_biztoc-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      216 2024-02-29 11:03:36.756333 openbb_biztoc-1.1.4/README.md
--rw-r--r--   0        0        0      779 2024-03-21 17:38:35.636799 openbb_biztoc-1.1.4/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.756521 openbb_biztoc-1.1.4/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-03-21 17:38:35.636957 openbb_biztoc-1.1.4/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.756679 openbb_biztoc-1.1.4/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3829 2024-02-29 11:03:36.756771 openbb_biztoc-1.1.4/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0      450 2024-04-01 14:20:43.771457 openbb_biztoc-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 openbb_biztoc-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      216 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/README.md
+-rw-r--r--   0        0        0      779 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-19 13:10:31.744034 openbb_biztoc-1.1.5/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0      450 2024-04-19 16:40:51.999177 openbb_biztoc-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 openbb_biztoc-1.1.5/PKG-INFO
```

### Comparing `openbb_biztoc-1.1.4/openbb_biztoc/__init__.py` & `openbb_biztoc-1.1.5/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_biztoc-1.1.4/openbb_biztoc/models/world_news.py` & `openbb_biztoc-1.1.5/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_biztoc-1.1.4/openbb_biztoc/utils/helpers.py` & `openbb_biztoc-1.1.5/openbb_biztoc/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,96 +1,95 @@
-"""Biztoc Helpers"""
+"""Biztoc Helpers."""
 
 from datetime import timedelta
 from typing import Dict, List, Literal
 
 import requests
 import requests_cache
 from openbb_core.app.utils import get_user_cache_directory
 
+# pylint: disable=C0325
+
 cache_dir = get_user_cache_directory()
 
 biztoc_session_tags = requests_cache.CachedSession(
     f"{cache_dir}/http/biztoc_tags", expire_after=timedelta(days=1)
 )
 biztoc_session_sources = requests_cache.CachedSession(
     f"{cache_dir}/http/biztoc_sources", expire_after=timedelta(days=3)
 )
 
 
 def get_sources(api_key: str) -> List[Dict]:
-    """Valid sources for Biztoc queries."""
-
+    """Get valid sources for Biztoc queries."""
     headers = {
         "X-RapidAPI-Key": f"{api_key}",
         "X-RapidAPI-Host": "biztoc.p.rapidapi.com",
         "Accept": "application/json",
         "Accept-Encoding": "gzip",
     }
     sources = biztoc_session_sources.get(
         "https://biztoc.p.rapidapi.com/sources", headers=headers, timeout=10
     )
 
     return sources.json()
 
 
 def get_pages(api_key: str) -> List[str]:
-    """Valid pages for Biztoc queries."""
-
+    """Get valid pages for Biztoc queries."""
     headers = {
         "X-RapidAPI-Key": f"{api_key}",
         "X-RapidAPI-Host": "biztoc.p.rapidapi.com",
         "Accept": "application/json",
         "Accept-Encoding": "gzip",
     }
     pages = biztoc_session_sources.get(
         "https://biztoc.p.rapidapi.com/pages", headers=headers, timeout=10
     )
 
     return pages.json()
 
 
 def get_tags_by_page(page_id: str, api_key: str) -> List[str]:
-    """Valid tags required for Biztoc queries."""
-
+    """Get valid tags required for Biztoc queries."""
     headers = {
         "X-RapidAPI-Key": f"{api_key}",
         "X-RapidAPI-Host": "biztoc.p.rapidapi.com",
         "Accept": "application/json",
         "Accept-Encoding": "gzip",
     }
     tags = biztoc_session_tags.get(
         f"https://biztoc.p.rapidapi.com/tags/{page_id}", headers=headers, timeout=10
     )
 
     return tags.json()
 
 
 def get_all_tags(api_key) -> Dict[str, List[str]]:
+    """Get all tags for all pages."""
     tags: Dict[str, List[str]] = {}
 
     pages = get_pages(api_key)
     for page in pages:
         page_tags = get_tags_by_page(page, api_key)
-        tags.update({page: [x["tag"] for x in page_tags]})
+        tags.update({page: [x["tag"] for x in page_tags]})  # type: ignore
 
     return tags
 
 
 def get_news(
     api_key: str,
     filter_: Literal[
         "crypto", "hot", "latest", "main", "media", "source", "tag"
     ] = "latest",
     source: str = "bloomberg",
     tag: str = "",
     term: str = "",
 ) -> List[Dict]:
-    """Calls the BizToc API and returns the data."""
-
+    """Call the BizToc API and returns the data."""
     results = []
     term = term.replace(" ", "%20") if term else ""
     _tags = get_all_tags(api_key)
     pages = get_pages(api_key)
     tags = []
     tag = tag.lower() if tag else ""
     for page in pages:
```

### Comparing `openbb_biztoc-1.1.4/PKG-INFO` & `openbb_biztoc-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-biztoc
-Version: 1.1.4
+Version: 1.1.5
 Summary: 
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
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Biztoc Provider
 
 This extension integrates the Biztoc data provider
 into the OpenBB Platform.
```

