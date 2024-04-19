# Comparing `tmp/PKNSETools-0.1.20240418.90.tar.gz` & `tmp/PKNSETools-0.1.20240419.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240418.90.tar", last modified: Thu Apr 18 14:16:43 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240419.91.tar", last modified: Fri Apr 19 10:24:02 2024, max compression
```

## Comparing `PKNSETools-0.1.20240418.90.tar` & `PKNSETools-0.1.20240419.91.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:16:43.685306 PKNSETools-0.1.20240418.90/
--rw-rw-rw-   0        0        0     2661 2024-04-18 14:16:43.685306 PKNSETools-0.1.20240418.90/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 14:16:43.669693 PKNSETools-0.1.20240418.90/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-04-18 14:16:43.669693 PKNSETools-0.1.20240418.90/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:16:43.669693 PKNSETools-0.1.20240418.90/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3392 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0     6446 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    12681 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-04-18 14:16:39.000000 PKNSETools-0.1.20240418.90/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:16:43.685306 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61965 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29930 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:16:43.669693 PKNSETools-0.1.20240418.90/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-04-18 14:16:43.000000 PKNSETools-0.1.20240418.90/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2024-04-18 14:16:43.000000 PKNSETools-0.1.20240418.90/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:16:43.000000 PKNSETools-0.1.20240418.90/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 14:16:37.000000 PKNSETools-0.1.20240418.90/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-04-18 14:16:43.000000 PKNSETools-0.1.20240418.90/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-18 14:16:43.000000 PKNSETools-0.1.20240418.90/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/README.md
--rw-rw-rw-   0        0        0       86 2024-04-18 14:16:43.685306 PKNSETools-0.1.20240418.90/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-04-18 14:14:38.000000 PKNSETools-0.1.20240418.90/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/
+-rw-rw-rw-   0        0        0     2661 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3392 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10032 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2223 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     5168 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0     6446 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    12673 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       30 2024-04-19 10:23:58.000000 PKNSETools-0.1.20240419.91/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61965 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29930 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2661 2024-04-19 10:24:02.000000 PKNSETools-0.1.20240419.91/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2024-04-19 10:24:02.000000 PKNSETools-0.1.20240419.91/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:24:02.000000 PKNSETools-0.1.20240419.91/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 10:23:56.000000 PKNSETools-0.1.20240419.91/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-04-19 10:24:02.000000 PKNSETools-0.1.20240419.91/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 10:24:02.000000 PKNSETools-0.1.20240419.91/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-19 10:24:02.901794 PKNSETools-0.1.20240419.91/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-04-19 10:22:35.000000 PKNSETools-0.1.20240419.91/setup.py
```

### Comparing `PKNSETools-0.1.20240418.90/PKG-INFO` & `PKNSETools-0.1.20240419.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240418.90
+Version: 0.1.20240419.91
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240418.90.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240419.91.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240419.91/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240419.91/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240419.91/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240419.91/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240419.91/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240419.91/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240419.91/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240419.91/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240419.91/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/PKMultiProcessorClient.py` & `PKNSETools-0.1.20240419.91/PKNSETools/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240419.91/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                         + colorText.FAIL
                         + "[+] Enter Stock Code(s) for screening (Multiple codes should be seperated by ,): "
                     )
                 ).upper()
             stockCode = stockCode.replace(" ", "")
             listStockCodes = stockCode.split(",")
         else:
-            OutputControls().printOutput(colorText.BOLD + "[+] Getting Stock Codes From NSE... ", end="")
+            OutputControls().printOutput(colorText.BOLD + "[+] Getting Stock Codes From NSE... ")
             listStockCodes = self.fetchNiftyCodes(tickerOption)
             if len(listStockCodes) > 10:
                 OutputControls().printOutput(
                     colorText.GREEN
                     + ("=> Done! Fetched %d stock codes." % len(listStockCodes))
                     + colorText.END
                 )
```

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240419.91/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240419.91/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240418.90
+Version: 0.1.20240419.91
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240418.90.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240419.91.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240418.90/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240419.91/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/README.md` & `PKNSETools-0.1.20240419.91/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240418.90/setup.py` & `PKNSETools-0.1.20240419.91/setup.py`

 * *Files identical despite different names*

