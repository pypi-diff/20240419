# Comparing `tmp/openbb_news-1.1.4.tar.gz` & `tmp/openbb_news-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_news-1.1.4.tar", max compression
+gzip compressed data, was "openbb_news-1.1.5.tar", max compression
```

## Comparing `openbb_news-1.1.4.tar` & `openbb_news-1.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      420 2024-02-29 11:03:36.740608 openbb_news-1.1.4/README.md
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.740830 openbb_news-1.1.4/openbb_news/__init__.py
--rw-r--r--   0        0        0     3170 2024-03-13 16:36:51.578769 openbb_news-1.1.4/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.740930 openbb_news-1.1.4/openbb_news/py.typed
--rw-r--r--   0        0        0      440 2024-04-01 14:18:40.096044 openbb_news-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 openbb_news-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      420 2024-04-17 12:33:20.501645 openbb_news-1.1.5/README.md
+-rw-r--r--   0        0        0       29 2024-04-17 12:33:20.501645 openbb_news-1.1.5/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-17 12:33:20.501645 openbb_news-1.1.5/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_news-1.1.5/openbb_news/py.typed
+-rw-r--r--   0        0        0      440 2024-04-19 16:40:26.343120 openbb_news-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 openbb_news-1.1.5/PKG-INFO
```

### Comparing `openbb_news-1.1.4/openbb_news/news_router.py` & `openbb_news-1.1.5/openbb_news/news_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ExtraParams,
     ProviderChoices,
     StandardParams,
 )
 from openbb_core.app.query import Query
 from openbb_core.app.router import Router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Financial market news data.")
 
 
 @router.command(
     model="WorldNews",
     examples=[
         APIEx(parameters={"provider": "fmp"}),
         APIEx(parameters={"limit": 100, "provider": "intrinio"}),
```

### Comparing `openbb_news-1.1.4/PKG-INFO` & `openbb_news-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-news
-Version: 1.1.4
+Version: 1.1.5
 Summary: News extension for OpenBB
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
 
 # OpenBB News Extension
 
 This extension provides news for the OpenBB Platform.
 
 ## Installation
```

