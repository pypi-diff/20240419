# Comparing `tmp/rug-0.9.2.tar.gz` & `tmp/rug-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rug-0.9.2.tar", max compression
+gzip compressed data, was "rug-0.9.3.tar", max compression
```

## Comparing `rug-0.9.2.tar` & `rug-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      759 2023-09-07 13:49:46.329152 rug-0.9.2/README.md
--rw-r--r--   0        0        0      851 2023-09-17 07:28:11.428905 rug-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      288 2023-08-06 16:18:57.666687 rug-0.9.2/rug/__init__.py
--rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.9.2/rug/alphaquery.py
--rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.9.2/rug/barchart.py
--rw-r--r--   0        0        0     5183 2023-09-17 07:26:30.451733 rug-0.9.2/rug/base.py
--rw-r--r--   0        0        0     4988 2023-09-17 07:26:52.027983 rug-0.9.2/rug/etfdb.py
--rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.9.2/rug/exceptions.py
--rw-r--r--   0        0        0     3038 2023-06-16 06:33:17.358960 rug-0.9.2/rug/finviz.py
--rw-r--r--   0        0        0     5724 2023-09-17 06:58:03.640040 rug-0.9.2/rug/stockanalysis.py
--rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.9.2/rug/stocktwits.py
--rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.9.2/rug/tipranks.py
--rw-r--r--   0        0        0     5057 2023-08-31 12:46:14.412383 rug-0.9.2/rug/yahoo.py
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 rug-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      759 2023-09-07 13:49:46.329152 rug-0.9.3/README.md
+-rw-r--r--   0        0        0      830 2023-12-04 09:28:58.109528 rug-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-08-06 16:18:57.666687 rug-0.9.3/rug/__init__.py
+-rw-r--r--   0        0        0     4266 2023-12-03 18:50:25.632204 rug-0.9.3/rug/alphaquery.py
+-rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.9.3/rug/barchart.py
+-rw-r--r--   0        0        0     5607 2023-12-01 08:43:59.318011 rug-0.9.3/rug/base.py
+-rw-r--r--   0        0        0     4988 2023-09-17 07:26:52.027983 rug-0.9.3/rug/etfdb.py
+-rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.9.3/rug/exceptions.py
+-rw-r--r--   0        0        0     3032 2023-12-01 11:20:29.637400 rug-0.9.3/rug/finviz.py
+-rw-r--r--   0        0        0     5724 2023-09-17 06:58:03.640040 rug-0.9.3/rug/stockanalysis.py
+-rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.9.3/rug/stocktwits.py
+-rw-r--r--   0        0        0     6915 2023-11-27 11:49:57.587894 rug-0.9.3/rug/tipranks.py
+-rw-r--r--   0        0        0     5057 2023-08-31 12:46:14.412383 rug-0.9.3/rug/yahoo.py
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 rug-0.9.3/PKG-INFO
```

### Comparing `rug-0.9.2/README.md` & `rug-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/pyproject.toml` & `rug-0.9.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rug"
-version = "0.9.2"
+version = "0.9.3"
 description = "Library for fetching various stock data from the internet (official and unofficial APIs)."
 authors = ["Pavel Hrdina"]
 classifiers = [
     "Programming Language :: Python :: 3.6",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: Developers",
@@ -13,19 +13,18 @@
 readme = "README.md"
 documentation = "https://rug.readthedocs.io/en/latest/"
 homepage = "https://gitlab.com/imn1/rug"
 repository = "https://gitlab.com/imn1/rug"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-httpx = "^0.23"
+python = "^3.11"
+httpx = "^0.25"
 
 [tool.poetry.dev-dependencies]
 sphinx = "^5"
-jupyterlab = "^3.4.0"
 pytest = "^6.2.5"
 furo = "^2022.6.21"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `rug-0.9.2/rug/alphaquery.py` & `rug-0.9.3/rug/alphaquery.py`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/rug/barchart.py` & `rug-0.9.3/rug/barchart.py`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/rug/base.py` & `rug-0.9.3/rug/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
 import re
 from datetime import date, datetime
 from html.parser import HTMLParser
 from itertools import zip_longest
 
 import httpx
 
 from .exceptions import HttpException
 
+# logging.basicConfig(level=logging.DEBUG)
+
 
 class BaseAPI:
     timeout = 10
     user_agent = (
         "Mozilla/5.0 (X11; Linux x86_64; rv:103.0) Gecko/20100101 Firefox/103.0"
     )
 
@@ -28,37 +31,47 @@
         """
         Wraps https.get() method and raises custom exception
         in case of httpx expcetion.
         Also rises an exception for any non 2xx or 3xx status.
         """
 
         try:
-            response = httpx.get(*args, timeout=self.timeout, **kwargs)
+            response = httpx.get(
+                *args, timeout=self.timeout, follow_redirects=True, **kwargs
+            )
         except Exception as exc:
             raise HttpException(
                 f"Couldn't perform GET request with args {args}"
             ) from exc
 
         response.raise_for_status()
+        self.check_redirects(response)
 
         return response
 
     async def _aget(self, *args):
         async with httpx.AsyncClient() as client:
             try:
-                response = await client.get(*args, timeout=self.timeout)
+                response = await client.get(
+                    *args, timeout=self.timeout, follow_redirects=True
+                )
             except Exception as exc:
                 raise HttpException(
                     f"Couldn't perform GET request with args {args}"
                 ) from exc
 
             response.raise_for_status()
+            self.check_redirects(response)
 
             return response
 
+    def check_redirects(self, response):
+        if response.url.path.startswith("/lookup"):
+            raise HttpException(f"Couldn't find the symbol {self.symbol}")
+
 
 class Data(dict):
     """
     Dict substitution which recursivelly handles
     non-existing keys.
     """
```

### Comparing `rug-0.9.2/rug/etfdb.py` & `rug-0.9.3/rug/etfdb.py`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/rug/exceptions.py` & `rug-0.9.3/rug/exceptions.py`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/rug/finviz.py` & `rug-0.9.3/rug/finviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 f"https://finviz.com/quote.ashx?t={self.symbol.upper()}&ty=c&ta=1&p=d",
                 headers={"User-Agent": self.user_agent},
             )
         except Exception as e:
             raise SymbolNotFound from e
 
         finds = re.findall(
-            r"<table[^>]*fullview-ratings-outer[^>]*>(.+?)</table>",
+            r"<table[^>]*js-table-ratings[^>]*>(.+?)</table>",
             html.text,
             re.DOTALL,
         )
         rows = []
 
         if finds:
             html = HtmlTableParser.fix_empty_cells(finds[0])
```

### Comparing `rug-0.9.2/rug/stockanalysis.py` & `rug-0.9.3/rug/stockanalysis.py`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/rug/stocktwits.py` & `rug-0.9.3/rug/stocktwits.py`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/rug/tipranks.py` & `rug-0.9.3/rug/tipranks.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         dividends = []
 
         if data["dividend"]["history"]:
             for item in data["dividend"]["history"]:
                 dividends.append(
                     {
-                        "yield": float(item["yield"]) * 100,
+                        "yield": float(item["yield"] or 0) * 100,
                         "amount": float(item["amount"]),
                         "ex_date": datetime.strptime(
                             item["executionDate"], "%Y-%m-%dT%H:%M:%S.000Z"
                         ).date()
                         if item["executionDate"]
                         else None,
                         "payment_date": datetime.strptime(
```

### Comparing `rug-0.9.2/rug/yahoo.py` & `rug-0.9.3/rug/yahoo.py`

 * *Files identical despite different names*

### Comparing `rug-0.9.2/PKG-INFO` & `rug-0.9.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: rug
-Version: 0.9.2
+Version: 0.9.3
 Summary: Library for fetching various stock data from the internet (official and unofficial APIs).
 Home-page: https://gitlab.com/imn1/rug
 License: MIT
 Author: Pavel Hrdina
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: httpx (>=0.23,<0.24)
+Requires-Dist: httpx (>=0.25,<0.26)
 Project-URL: Documentation, https://rug.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.com/imn1/rug
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://gitlab.com/imn1/rug/-/raw/master/assets/logo.png">
 </div>
```

