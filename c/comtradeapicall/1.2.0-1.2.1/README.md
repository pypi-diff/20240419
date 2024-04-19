# Comparing `tmp/comtradeapicall-1.2.0.tar.gz` & `tmp/comtradeapicall-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comtradeapicall-1.2.0.tar", last modified: Tue Mar 12 16:50:04 2024, max compression
+gzip compressed data, was "comtradeapicall-1.2.1.tar", last modified: Fri Apr 19 14:32:58 2024, max compression
```

## Comparing `comtradeapicall-1.2.0.tar` & `comtradeapicall-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 16:50:04.413079 comtradeapicall-1.2.0/
--rw-rw-rw-   0        0        0     1093 2023-01-09 21:17:11.000000 comtradeapicall-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    19828 2024-03-12 16:50:04.413079 comtradeapicall-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    19279 2024-03-12 16:47:37.000000 comtradeapicall-1.2.0/README.md
--rw-rw-rw-   0        0        0      539 2024-03-12 16:42:16.000000 comtradeapicall-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 16:50:04.413079 comtradeapicall-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-12 16:50:04.329372 comtradeapicall-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-12 16:50:04.345236 comtradeapicall-1.2.0/src/comtradeapicall/
--rw-rw-rw-   0        0        0     1098 2024-02-22 12:20:27.000000 comtradeapicall-1.2.0/src/comtradeapicall/AIS.py
--rw-rw-rw-   0        0        0     6397 2024-02-22 12:25:53.000000 comtradeapicall-1.2.0/src/comtradeapicall/Async.py
--rw-rw-rw-   0        0        0     6499 2024-03-11 16:42:30.000000 comtradeapicall-1.2.0/src/comtradeapicall/BulkDownload.py
--rw-rw-rw-   0        0        0     4625 2024-03-12 16:30:39.000000 comtradeapicall-1.2.0/src/comtradeapicall/DataAvailability.py
--rw-rw-rw-   0        0        0     3954 2024-03-12 16:37:30.000000 comtradeapicall-1.2.0/src/comtradeapicall/Metadata.py
--rw-rw-rw-   0        0        0    11150 2024-02-22 12:23:51.000000 comtradeapicall-1.2.0/src/comtradeapicall/PreviewGet.py
--rw-rw-rw-   0        0        0      957 2023-12-29 03:08:50.000000 comtradeapicall-1.2.0/src/comtradeapicall/SUV.py
--rw-rw-rw-   0        0        0     1815 2024-03-12 16:37:39.000000 comtradeapicall-1.2.0/src/comtradeapicall/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:50:04.411660 comtradeapicall-1.2.0/src/comtradeapicall.egg-info/
--rw-rw-rw-   0        0        0    19828 2024-03-12 16:50:04.000000 comtradeapicall-1.2.0/src/comtradeapicall.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17767 2023-02-16 11:24:18.000000 comtradeapicall-1.2.0/src/comtradeapicall.egg-info/PKG-INFO-W10LT-PF2ZCSNL
--rw-rw-rw-   0        0        0      514 2024-03-12 16:50:04.000000 comtradeapicall-1.2.0/src/comtradeapicall.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 16:50:04.000000 comtradeapicall-1.2.0/src/comtradeapicall.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-12 16:50:04.000000 comtradeapicall-1.2.0/src/comtradeapicall.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 14:32:58.626424 comtradeapicall-1.2.1/
+-rw-rw-rw-   0        0        0     1093 2023-01-09 21:17:11.000000 comtradeapicall-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    19840 2024-04-19 14:32:58.623913 comtradeapicall-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    19291 2024-04-19 14:12:06.000000 comtradeapicall-1.2.1/README.md
+-rw-rw-rw-   0        0        0      539 2024-04-19 14:02:41.000000 comtradeapicall-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:32:58.626424 comtradeapicall-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 14:32:58.414411 comtradeapicall-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 14:32:58.519194 comtradeapicall-1.2.1/src/comtradeapicall/
+-rw-rw-rw-   0        0        0     1216 2024-04-19 13:46:48.000000 comtradeapicall-1.2.1/src/comtradeapicall/AIS.py
+-rw-rw-rw-   0        0        0     7088 2024-04-19 13:47:00.000000 comtradeapicall-1.2.1/src/comtradeapicall/Async.py
+-rw-rw-rw-   0        0        0     6841 2024-04-19 13:47:09.000000 comtradeapicall-1.2.1/src/comtradeapicall/BulkDownload.py
+-rw-rw-rw-   0        0        0     4955 2024-04-19 13:47:26.000000 comtradeapicall-1.2.1/src/comtradeapicall/DataAvailability.py
+-rw-rw-rw-   0        0        0     4492 2024-04-19 13:47:24.000000 comtradeapicall-1.2.1/src/comtradeapicall/Metadata.py
+-rw-rw-rw-   0        0        0    11497 2024-04-19 13:47:35.000000 comtradeapicall-1.2.1/src/comtradeapicall/PreviewGet.py
+-rw-rw-rw-   0        0        0     1088 2024-04-19 13:47:42.000000 comtradeapicall-1.2.1/src/comtradeapicall/SUV.py
+-rw-rw-rw-   0        0        0     1815 2024-03-12 16:37:39.000000 comtradeapicall-1.2.1/src/comtradeapicall/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:32:58.621908 comtradeapicall-1.2.1/src/comtradeapicall.egg-info/
+-rw-rw-rw-   0        0        0    19840 2024-04-19 14:32:58.000000 comtradeapicall-1.2.1/src/comtradeapicall.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17767 2023-02-16 11:24:18.000000 comtradeapicall-1.2.1/src/comtradeapicall.egg-info/PKG-INFO-W10LT-PF2ZCSNL
+-rw-rw-rw-   0        0        0      514 2024-04-19 14:32:58.000000 comtradeapicall-1.2.1/src/comtradeapicall.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:32:58.000000 comtradeapicall-1.2.1/src/comtradeapicall.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 14:32:58.000000 comtradeapicall-1.2.1/src/comtradeapicall.egg-info/top_level.txt
```

### Comparing `comtradeapicall-1.2.0/LICENSE` & `comtradeapicall-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comtradeapicall-1.2.0/PKG-INFO` & `comtradeapicall-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comtradeapicall
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package to call UN Comtrade APIs
 Author-email: untradestats <untradestats@gmail.com>
 Project-URL: Homepage, https://github.com/uncomtrade/comtradeapicall
 Project-URL: Bug Tracker, https://github.com/uncomtrade/comtradeapicall/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 # UN Comtrade API Package
 This package simplifies calling [APIs of UN Comtrade](https://comtradedeveloper.un.org) to extract and download data
  (and much more). 
 
 ## Details
 [UN Comtrade](https://comtrade.un.org) provides free and premium APIs to extract and download data/metadata, however
  it is quite a learning curve to understand all of APIs end-points and parameters. This package simplifies it by
-  calling a single python function with the appropriate parameters. Learn more about UN Comtrade at the [UN Comtrade wiki](https://unstats.un.org/wiki/display/comtrade/UN+Comtrade).
+  calling a single python function with the appropriate parameters. Learn more about UN Comtrade at the [UN Comtrade Docs](https://uncomtrade.org/docs).
 
 This project is intended to be deployed at [The Python Package Index](https://pypi.org/project/comtradeapicall/), therefore the structure of
  folders follows the suggested layout from [Packaging Python Project](https://packaging.python.org/en/latest/tutorials/packaging-projects/). The main scripts are located at **/src/comtradeapicall/**. And the folder **tests** contains the example scripts how to install and use the package.
  
  ## Prerequisites
 This package assumes using Python 3.7 and the expected package dependencies are listed in the "requirements.txt" file
  for PIP, you need to run the following command to get dependencies:
@@ -94,15 +94,15 @@
 
 - **SUV:** Model class to extract data on Standard Unit Values (SUV) and their ranges
   - getSUV(**subscription_key**, **SelectionCriteria**, **[qtyUnitCode]**) : return data frame with SUV data
 
 - **AIS:** Model class to extract experimental trade data generated from AIS (ships tracking movement). See [Cerdeiro, Komaromi, Liu and Saeed (2020)](https://www.imf.org/en/Publications/WP/Issues/2020/05/14/World-Seaborne-Trade-in-Real-Time-A-Proof-of-Concept-for-Building-AIS-based-Nowcasts-from-49393). *When consuming the data, users should understand its limitation.*  
   - getAIS(**subscription_key**, **AISSelectionCriteria**, **[vesselTypeCode]**) : return data frame with AIS trade data
 
-See differences between final and tariff line data at the [Wiki](https://unstats.un.org/wiki/display/comtrade/New+Comtrade+FAQ+for+First+Time+Users#NewComtradeFAQforFirstTimeUsers-Whatisthetarifflinedata?)
+See differences between final and tariff line data at the [Docs](https://uncomtrade.org/docs/what-is-tariffline-data/)
  
 ## Selection Criteria
 - typeCode(str) : Product type. Goods (C) or Services (S)
 - freqCode(str) : The time interval at which observations occur. Annual (A) or Monthly (M)
 - clCode(str) : Indicates the product classification used and which version (HS, SITC)
 - period(str) :  Combination of year and month (for monthly), year for (annual)
 - reporterCode(str) : The country or geographic area to which the measured statistical phenomenon relates
@@ -124,14 +124,18 @@
 ## AIS Selection Criteria
 - typeCode(str) : Product type. Only Goods (C)
 - freqCode(str) : The time interval at which observations occur. Daily (D)
 - datefrom(str) and dateto(str) :  Date(s) of observation - ASCII format
 - countryareaCode(str) : The country or geographic area to which the measured statistical phenomenon relates. Use *getReference('ais:countriesareas')* for the complete list.
 - vesselTypeCode(str) : The high level categorization of vessels transporting the goods. Use *getReference('ais:vesseltypes')* for the complete list.
 - flowCode(str) : Trade flow (exports, imports)
+
+## Proxy Server
+- proxy_url(str) : All functions that call the API support the proxy server. Use the parameter proxy_url.
+
  
 ## Examples of python usage
 - Extract Australia imports of commodity code 91 in classic mode in May 2022
 ``` python
 mydf = comtradeapicall.previewFinalData(typeCode='C', freqCode='M', clCode='HS', period='202205',
                                         reporterCode='36', cmdCode='91', flowCode='M', partnerCode=None,
                                         partner2Code=None,
```

### Comparing `comtradeapicall-1.2.0/README.md` & `comtradeapicall-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # UN Comtrade API Package
 This package simplifies calling [APIs of UN Comtrade](https://comtradedeveloper.un.org) to extract and download data
  (and much more). 
 
 ## Details
 [UN Comtrade](https://comtrade.un.org) provides free and premium APIs to extract and download data/metadata, however
  it is quite a learning curve to understand all of APIs end-points and parameters. This package simplifies it by
-  calling a single python function with the appropriate parameters. Learn more about UN Comtrade at the [UN Comtrade wiki](https://unstats.un.org/wiki/display/comtrade/UN+Comtrade).
+  calling a single python function with the appropriate parameters. Learn more about UN Comtrade at the [UN Comtrade Docs](https://uncomtrade.org/docs).
 
 This project is intended to be deployed at [The Python Package Index](https://pypi.org/project/comtradeapicall/), therefore the structure of
  folders follows the suggested layout from [Packaging Python Project](https://packaging.python.org/en/latest/tutorials/packaging-projects/). The main scripts are located at **/src/comtradeapicall/**. And the folder **tests** contains the example scripts how to install and use the package.
  
  ## Prerequisites
 This package assumes using Python 3.7 and the expected package dependencies are listed in the "requirements.txt" file
  for PIP, you need to run the following command to get dependencies:
@@ -80,15 +80,15 @@
 
 - **SUV:** Model class to extract data on Standard Unit Values (SUV) and their ranges
   - getSUV(**subscription_key**, **SelectionCriteria**, **[qtyUnitCode]**) : return data frame with SUV data
 
 - **AIS:** Model class to extract experimental trade data generated from AIS (ships tracking movement). See [Cerdeiro, Komaromi, Liu and Saeed (2020)](https://www.imf.org/en/Publications/WP/Issues/2020/05/14/World-Seaborne-Trade-in-Real-Time-A-Proof-of-Concept-for-Building-AIS-based-Nowcasts-from-49393). *When consuming the data, users should understand its limitation.*  
   - getAIS(**subscription_key**, **AISSelectionCriteria**, **[vesselTypeCode]**) : return data frame with AIS trade data
 
-See differences between final and tariff line data at the [Wiki](https://unstats.un.org/wiki/display/comtrade/New+Comtrade+FAQ+for+First+Time+Users#NewComtradeFAQforFirstTimeUsers-Whatisthetarifflinedata?)
+See differences between final and tariff line data at the [Docs](https://uncomtrade.org/docs/what-is-tariffline-data/)
  
 ## Selection Criteria
 - typeCode(str) : Product type. Goods (C) or Services (S)
 - freqCode(str) : The time interval at which observations occur. Annual (A) or Monthly (M)
 - clCode(str) : Indicates the product classification used and which version (HS, SITC)
 - period(str) :  Combination of year and month (for monthly), year for (annual)
 - reporterCode(str) : The country or geographic area to which the measured statistical phenomenon relates
@@ -110,14 +110,18 @@
 ## AIS Selection Criteria
 - typeCode(str) : Product type. Only Goods (C)
 - freqCode(str) : The time interval at which observations occur. Daily (D)
 - datefrom(str) and dateto(str) :  Date(s) of observation - ASCII format
 - countryareaCode(str) : The country or geographic area to which the measured statistical phenomenon relates. Use *getReference('ais:countriesareas')* for the complete list.
 - vesselTypeCode(str) : The high level categorization of vessels transporting the goods. Use *getReference('ais:vesseltypes')* for the complete list.
 - flowCode(str) : Trade flow (exports, imports)
+
+## Proxy Server
+- proxy_url(str) : All functions that call the API support the proxy server. Use the parameter proxy_url.
+
  
 ## Examples of python usage
 - Extract Australia imports of commodity code 91 in classic mode in May 2022
 ``` python
 mydf = comtradeapicall.previewFinalData(typeCode='C', freqCode='M', clCode='HS', period='202205',
                                         reporterCode='36', cmdCode='91', flowCode='M', partnerCode=None,
                                         partner2Code=None,
```

### Comparing `comtradeapicall-1.2.0/pyproject.toml` & `comtradeapicall-1.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comtradeapicall"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="untradestats", email="untradestats@gmail.com" },
 ]
 description = "A package to call UN Comtrade APIs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/AIS.py` & `comtradeapicall-1.2.1/src/comtradeapicall/AIS.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import json
 from pandas import json_normalize
 import urllib3
 
-def getAIS(subscription_key, typeCode='C', freqCode='D', clCode='XX', countryareaCode='', vesselTypeCode='', flowCode='', dateFrom='', dateTo='', maxRecords=250000):
-    baseURL = 'https://comtradeapi.un.org/experimental/v1/getAIS/' + typeCode + '/' + freqCode + '/' + clCode
+
+def getAIS(subscription_key, typeCode='C', freqCode='D', clCode='XX', countryareaCode='', vesselTypeCode='', flowCode='', dateFrom='', dateTo='', maxRecords=250000, proxy_url=None):
+    baseURL = 'https://comtradeapi.un.org/experimental/v1/getAIS/' + \
+        typeCode + '/' + freqCode + '/' + clCode
     PARAMS = dict(countryareaCode=countryareaCode, vesselTypeCode=vesselTypeCode,
                   flowCode=flowCode, dateFrom=dateFrom, dateTo=dateTo,
                   maxRecords=maxRecords)
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET",baseURL, fields = fields, timeout=120)
+        resp = http.request("GET", baseURL, fields=fields, timeout=120)
         if resp.status != 200:
             print(resp.data.decode('utf-8'))
         else:
             jsonResult = json.loads(resp.data)
             df = json_normalize(jsonResult['data'])
             return df
     except urllib3.exceptions.RequestError as err:
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/Async.py` & `comtradeapicall-1.2.1/src/comtradeapicall/Async.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,76 +2,89 @@
 from pandas import json_normalize
 import os
 from urllib.parse import urlparse
 import json
 import urllib3
 import shutil
 
+
 def submitAsyncDataRequest(subscription_key, endPoint, typeCode, freqCode, clCode, period, reporterCode, cmdCode,
-                   flowCode, partnerCode, partner2Code, customsCode, motCode, aggregateBy, breakdownMode):
+                           flowCode, partnerCode, partner2Code, customsCode, motCode, aggregateBy, breakdownMode, proxy_url=None):
     if endPoint == 'TARIFFLINE':
-        baseURL = 'https://comtradeapi.un.org/async/v1/getTariffline/' + typeCode + '/' + freqCode + '/' + clCode
+        baseURL = 'https://comtradeapi.un.org/async/v1/getTariffline/' + \
+            typeCode + '/' + freqCode + '/' + clCode
     else:
-        baseURL = 'https://comtradeapi.un.org/async/v1/get/' + typeCode + '/' + freqCode + '/' + clCode
+        baseURL = 'https://comtradeapi.un.org/async/v1/get/' + \
+            typeCode + '/' + freqCode + '/' + clCode
 
     PARAMS = dict(reportercode=reporterCode, flowCode=flowCode,
                   period=period, cmdCode=cmdCode, partnerCode=partnerCode, partner2Code=partner2Code,
                   motCode=motCode, customsCode=customsCode, aggregateBy=aggregateBy, breakdownMode=breakdownMode)
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET",baseURL, fields = fields, timeout=120)
+        resp = http.request("GET", baseURL, fields=fields, timeout=120)
         if resp.status != 202:
             print(resp.data.decode('utf-8'))
         else:
             jsonResult = json.loads(resp.data)
             print('Return message:', jsonResult['message'])
             return jsonResult
     except urllib3.exceptions.RequestError as err:
         print(f'Request error: {err}')
 
+
 def submitAsyncFinalDataRequest(subscription_key, typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode,  aggregateBy=None,
-                              breakdownMode=None):
+                                partnerCode,
+                                partner2Code, customsCode, motCode,  aggregateBy=None,
+                                breakdownMode=None, proxy_url=None):
     return submitAsyncDataRequest(subscription_key, 'FINAL', typeCode, freqCode, clCode, period, reporterCode,
                                   cmdCode, flowCode,
                                   partnerCode,
-                                  partner2Code, customsCode, motCode, aggregateBy, breakdownMode)
+                                  partner2Code, customsCode, motCode, aggregateBy, breakdownMode, proxy_url=proxy_url)
+
 
 def submitAsyncTarifflineDataRequest(subscription_key, typeCode, freqCode, clCode, period, reporterCode, cmdCode,
-                                   flowCode,partnerCode, partner2Code, customsCode, motCode):
+                                     flowCode, partnerCode, partner2Code, customsCode, motCode, proxy_url=None):
     return submitAsyncDataRequest(subscription_key, 'TARIFFLINE', typeCode, freqCode, clCode, period, reporterCode,
                                   cmdCode, flowCode,
                                   partnerCode,
-                                  partner2Code, customsCode, motCode, None, None)
+                                  partner2Code, customsCode, motCode, aggregateBy=None, breakdownMode=None, proxy_url=proxy_url)
+
 
-def checkAsyncDataRequest(subscription_key, batchId=None):
+def checkAsyncDataRequest(subscription_key, batchId=None, proxy_url=None):
     baseURL = 'https://comtradeapi.un.org/async/v1/getDA/'
     PARAMS = dict(batchId=batchId)
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET",baseURL, fields = fields, timeout=120)
+        resp = http.request("GET", baseURL, fields=fields, timeout=120)
         if resp.status != 200:
             print(resp.data.decode('utf-8'))
         else:
             jsonResult = json.loads(resp.data)
             df = json_normalize(jsonResult['data'])
             return df
     except urllib3.exceptions.RequestError as err:
         print(f'Request error: {err}')
 
+
 def downloadAsyncFinalDataRequest(subscription_key, directory, typeCode, freqCode, clCode, period,
                                   reporterCode, cmdCode, flowCode, partnerCode, partner2Code, customsCode, motCode,
-                                  aggregateBy=None, breakdownMode=None):
+                                  aggregateBy=None, breakdownMode=None, proxy_url=None):
     myJson = submitAsyncFinalDataRequest(subscription_key, typeCode, freqCode, clCode, period, reporterCode,
-                                  cmdCode, flowCode,partnerCode,partner2Code, customsCode, motCode, aggregateBy, breakdownMode)
+                                         cmdCode, flowCode, partnerCode, partner2Code, customsCode, motCode, aggregateBy, breakdownMode, proxy_url=proxy_url)
     batchId = myJson['requestId']
     print("Processing and downloading the result. BatchId: ", batchId)
     status = ''
     while status != 'Completed' and status != 'Error':
         mydf = checkAsyncDataRequest(subscription_key, batchId=batchId)
         current_status = mydf.iloc[0]['status']
         if status != current_status:
@@ -79,28 +92,32 @@
             print("Batch Status: ", current_status)
         t.sleep(15)
     if status == 'Completed':
         url = mydf.iloc[0]['uri']
         a = urlparse(url)
         fileName = os.path.basename(a.path)
         download_path = os.path.join(directory, fileName)
-        #download file
-        httpFILE = urllib3.PoolManager()
+        # download file
+        if proxy_url:
+            httpFILE = urllib3.ProxyManager(proxy_url=proxy_url)
+        else:
+            httpFILE = urllib3.PoolManager()
         with open(download_path, 'wb') as out:
             r = httpFILE.request('GET', url, preload_content=False)
             shutil.copyfileobj(r, out)
         r.release_conn()
         print(fileName, ' downloaded successfully')
     else:
         print('Error occurred when processing batchId: ', batchId)
 
+
 def downloadAsyncTarifflineDataRequest(subscription_key, directory, typeCode, freqCode, clCode, period,
-                                  reporterCode, cmdCode, flowCode, partnerCode, partner2Code, customsCode, motCode):
+                                       reporterCode, cmdCode, flowCode, partnerCode, partner2Code, customsCode, motCode, proxy_url=None):
     myJson = submitAsyncTarifflineDataRequest(subscription_key, typeCode, freqCode, clCode, period, reporterCode,
-                                  cmdCode, flowCode,partnerCode,partner2Code, customsCode, motCode)
+                                              cmdCode, flowCode, partnerCode, partner2Code, customsCode, motCode, proxy_url=proxy_url)
     batchId = myJson['requestId']
     # check status -- looping
     print("Processing and downloading the result. BatchId: ", batchId)
     status = ''
     while status != 'Completed' and status != 'Error':
         mydf = checkAsyncDataRequest(subscription_key, batchId=batchId)
         current_status = mydf.iloc[0]['status']
@@ -109,16 +126,19 @@
             print("Batch Status: ", current_status)
         t.sleep(15)
     if status == 'Completed':
         url = mydf.iloc[0]['uri']
         a = urlparse(url)
         fileName = os.path.basename(a.path)
         download_path = os.path.join(directory, fileName)
-        #download file
-        httpFILE = urllib3.PoolManager()
+        # download file
+        if proxy_url:
+            httpFILE = urllib3.ProxyManager(proxy_url=proxy_url)
+        else:
+            httpFILE = urllib3.PoolManager()
         with open(download_path, 'wb') as out:
             r = httpFILE.request('GET', url, preload_content=False)
             shutil.copyfileobj(r, out)
         r.release_conn()
         print(fileName, ' downloaded successfully')
     else:
-        print('Error occurred when processing batchId: ', batchId)
+        print('Error occurred when processing batchId: ', batchId)
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/BulkDownload.py` & `comtradeapicall-1.2.1/src/comtradeapicall/BulkDownload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,100 +1,121 @@
 import os
 import shutil
 import gzip
 from pandas import json_normalize
 import urllib3
 import json
 
+
 def bulkDownloadFile(subscription_key, directory, tradeDataType, typeCode, freqCode, clCode, period, reporterCode,
-                     decompress, publishedDateFrom=None, publishedDateTo=None):
+                     decompress, publishedDateFrom=None, publishedDateTo=None, proxy_url=None):
 
     if tradeDataType == 'TARIFFLINE':
-        baseURLDataAvailability = 'https://comtradeapi.un.org/bulk/v1/getTariffline/' + typeCode + '/' + freqCode + '/' + clCode
+        baseURLDataAvailability = 'https://comtradeapi.un.org/bulk/v1/getTariffline/' + \
+            typeCode + '/' + freqCode + '/' + clCode
         prefixFile = 'TARIFFLINE'
     elif tradeDataType == "FINALCLASSIC":
-        baseURLDataAvailability = 'https://comtradeapi.un.org/bulk/v1/getClassic/' + typeCode + '/' + freqCode + '/' + clCode
+        baseURLDataAvailability = 'https://comtradeapi.un.org/bulk/v1/getClassic/' + \
+            typeCode + '/' + freqCode + '/' + clCode
         prefixFile = 'FINALCLASSIC'
     else:
-        baseURLDataAvailability = 'https://comtradeapi.un.org/bulk/v1/get/' + typeCode + '/' + freqCode + '/' + clCode
+        baseURLDataAvailability = 'https://comtradeapi.un.org/bulk/v1/get/' + \
+            typeCode + '/' + freqCode + '/' + clCode
         prefixFile = 'FINAL'
 
-    PARAMS = dict(reportercode=reporterCode, period=period, publishedDateFrom=publishedDateFrom, publishedDateTo=publishedDateTo)
+    PARAMS = dict(reportercode=reporterCode, period=period,
+                  publishedDateFrom=publishedDateFrom, publishedDateTo=publishedDateTo)
     # add key
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET",baseURLDataAvailability, fields = fields, timeout=120)
+        resp = http.request("GET", baseURLDataAvailability,
+                            fields=fields, timeout=120)
         if resp.status != 200:
             print(resp.data.decode('utf-8'))
         else:
             jsonResult = json.loads(resp.data)
             if jsonResult['count'] == 0:
                 print('No data available based on the selection criteria')
             else:
-                df = json_normalize(jsonResult['data'])  # Results contain the required data
+                # Results contain the required data
+                df = json_normalize(jsonResult['data'])
                 totalFiles = df[df.columns[0]].count()
                 i = 0
                 while i < totalFiles:
                     # prepare file name
                     if tradeDataType == 'TARIFFLINE':
                         if (df.timestamp[i] is None):
                             timestamp = '1900-01-01'
                         else:
-                            timestamp = df.timestamp[i][:10]  
+                            timestamp = df.timestamp[i][:10]
                         fileName = "COMTRADE-" + prefixFile + "-" + df.typeCode[i] + df.freqCode[i] + str(df.reporterCode[i]).zfill(
                             3) + str(df.period[i]) + df.classificationCode[i] + "[" + timestamp + "].gz"
                     else:
                         if (df.publicationDate[i] is None):
                             publicationDate = '1900-01-01'
                         else:
-                            publicationDate = df.publicationDate[i][:10]                          
+                            publicationDate = df.publicationDate[i][:10]
                         fileName = "COMTRADE-" + prefixFile + "-" + df.typeCode[i] + df.freqCode[i] + str(
                             df.reporterCode[i]).zfill(
                             3) + str(df.period[i]) + df.classificationCode[i] + "[" + publicationDate + "].gz"
                     download_path = os.path.join(directory, fileName)
-                    #download file
+                    # download file
                     file_url = df.fileUrl[i]
                     PARAMS = dict()
                     PARAMS["subscription-key"] = subscription_key
-                    fieldsFILE = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-                    httpFILE = urllib3.PoolManager()
+                    fieldsFILE = dict(
+                        filter(lambda item: item[1] is not None, PARAMS.items()))
+                    if proxy_url:
+                        httpFILE = urllib3.ProxyManager(proxy_url=proxy_url)
+                    else:
+                        httpFILE = urllib3.PoolManager()
                     with open(download_path, 'wb') as out:
-                        r = httpFILE.request('GET', file_url, fields=fieldsFILE, preload_content=False)
+                        r = httpFILE.request(
+                            'GET', file_url, fields=fieldsFILE, preload_content=False)
                         shutil.copyfileobj(r, out)
                     r.release_conn()
                     print(fileName.replace(".gz", "") + ' downloaded')
                     download_path_gunzip = download_path.replace(".gz", ".txt")
                     if decompress is True:
-                        with gzip.open(download_path, "rb")  as f_in:
+                        with gzip.open(download_path, "rb") as f_in:
                             with open(download_path_gunzip, 'wb') as f_out:
                                 shutil.copyfileobj(f_in, f_out)
                         os.remove(download_path)
                     i = i + 1
                 print('Total of ' + str(i) + ' file(s) downloaded')
     except urllib3.exceptions.RequestError as err:
         print(f'Request error: {err}')
 
+
 def bulkDownloadFinalFile(subscription_key, directory, typeCode, freqCode, clCode, period=None, reporterCode=None, decompress=False, publishedDateFrom=None, publishedDateTo=None):
     bulkDownloadFile(subscription_key, directory, 'FINAL', typeCode, freqCode, clCode, period,
-                             reporterCode, decompress, publishedDateFrom, publishedDateTo)
-    
+                     reporterCode, decompress, publishedDateFrom, publishedDateTo)
+
+
 def bulkDownloadFinalClassicFile(subscription_key, directory, typeCode, freqCode, clCode, period=None, reporterCode=None, decompress=False, publishedDateFrom=None, publishedDateTo=None):
     bulkDownloadFile(subscription_key, directory, 'FINALCLASSIC', typeCode, freqCode, clCode, period,
-                             reporterCode, decompress, publishedDateFrom, publishedDateTo)
+                     reporterCode, decompress, publishedDateFrom, publishedDateTo)
+
 
 def bulkDownloadTarifflineFile(subscription_key, directory, typeCode, freqCode, clCode, period=None, reporterCode=None, decompress=False, publishedDateFrom=None, publishedDateTo=None):
     bulkDownloadFile(subscription_key, directory, 'TARIFFLINE', typeCode, freqCode, clCode, period,
-                             reporterCode, decompress, publishedDateFrom, publishedDateTo)
+                     reporterCode, decompress, publishedDateFrom, publishedDateTo)
+
 
 def bulkDownloadFinalFileDateRange(subscription_key, directory, typeCode, freqCode, clCode, period=None, reporterCode=None, decompress=False, publishedDateFrom=None, publishedDateTo=None):
     bulkDownloadFile(subscription_key, directory, 'FINAL', typeCode, freqCode, clCode, period,
-                             reporterCode, decompress, publishedDateFrom, publishedDateTo)
+                     reporterCode, decompress, publishedDateFrom, publishedDateTo)
+
 
 def bulkDownloadFinalClassicFileDateRange(subscription_key, directory, typeCode, freqCode, clCode, period=None, reporterCode=None, decompress=False, publishedDateFrom=None, publishedDateTo=None):
     bulkDownloadFile(subscription_key, directory, 'FINALCLASSIC', typeCode, freqCode, clCode, period,
-                             reporterCode, decompress, publishedDateFrom, publishedDateTo)    
+                     reporterCode, decompress, publishedDateFrom, publishedDateTo)
+
 
 def bulkDownloadTarifflineFileDateRange(subscription_key, directory, typeCode, freqCode, clCode, period=None, reporterCode=None, decompress=False, publishedDateFrom=None, publishedDateTo=None):
     bulkDownloadFile(subscription_key, directory, 'TARIFFLINE', typeCode, freqCode, clCode, period,
-                             reporterCode, decompress, publishedDateFrom, publishedDateTo)
+                     reporterCode, decompress, publishedDateFrom, publishedDateTo)
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/DataAvailability.py` & `comtradeapicall-1.2.1/src/comtradeapicall/DataAvailability.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,97 @@
 import json
 from pandas import json_normalize
 import urllib3
 
-def getLiveUpdate(subscription_key):
+
+def getLiveUpdate(subscription_key, proxy_url=None):
     baseURL = 'https://comtradeapi.un.org/data/v1/getLiveUpdate'
     PARAMS = dict()
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET",baseURL, fields = fields, timeout=120)
+        resp = http.request("GET", baseURL, fields=fields, timeout=120)
         if resp.status != 200:
             print(resp.data.decode('utf-8'))
         else:
             jsonResult = json.loads(resp.data)
             df = json_normalize(jsonResult['data'])
             return df
     except urllib3.exceptions.RequestError as err:
         print(f'Request error: {err}')
 
-def getDataAvailability(subscription_key, tradeDataType, dataAvailabilityType, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo):
-    
-    if(subscription_key is None):
+
+def getDataAvailability(subscription_key, tradeDataType, dataAvailabilityType, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo, proxy_url=None):
+
+    if (subscription_key is None):
         endpoint = "public"
-    else:  
+    else:
         endpoint = "data"
 
-    
-    if dataAvailabilityType=='BULK':
+    if dataAvailabilityType == 'BULK':
         if tradeDataType == 'TARIFFLINE':
-            baseURL = 'https://comtradeapi.un.org/bulk/v1/getTariffline/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/bulk/v1/getTariffline/' + \
+                typeCode + '/' + freqCode + '/' + clCode
         elif tradeDataType == 'FINALCLASSIC':
-            baseURL = 'https://comtradeapi.un.org/bulk/v1/getClassic/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/bulk/v1/getClassic/' + \
+                typeCode + '/' + freqCode + '/' + clCode
         else:
-            baseURL = 'https://comtradeapi.un.org/bulk/v1/get/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/bulk/v1/get/' + \
+                typeCode + '/' + freqCode + '/' + clCode
     else:
         if tradeDataType == 'TARIFFLINE':
-            baseURL = 'https://comtradeapi.un.org/' + endpoint + '/v1/getDaTariffline/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/' + endpoint + \
+                '/v1/getDaTariffline/' + typeCode + '/' + freqCode + '/' + clCode
         else:
-            baseURL = 'https://comtradeapi.un.org/' + endpoint + '/v1/getDa/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/' + endpoint + \
+                '/v1/getDa/' + typeCode + '/' + freqCode + '/' + clCode
 
-    PARAMS = dict(reportercode=reporterCode, period=period, publishedDateFrom=publishedDateFrom, publishedDateTo=publishedDateTo)
+    PARAMS = dict(reportercode=reporterCode, period=period,
+                  publishedDateFrom=publishedDateFrom, publishedDateTo=publishedDateTo)
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET", baseURL, fields = fields, timeout=120)
+        resp = http.request("GET", baseURL, fields=fields, timeout=120)
         if resp.status != 200:
             print(resp.data.decode('utf-8'))
         else:
             jsonResult = json.loads(resp.data)
             df = json_normalize(jsonResult['data'])
             return df
     except urllib3.exceptions.RequestError as err:
         print(f'Request error: {err}')
 
+
 def _getFinalDataAvailability(typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom=None, publishedDateTo=None):
     return getDataAvailability(None, 'FINAL', None, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo)
 
+
 def getFinalDataAvailability(subscription_key, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom=None, publishedDateTo=None):
     return getDataAvailability(subscription_key, 'FINAL', None, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo)
 
 
 def _getTarifflineDataAvailability(typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom=None, publishedDateTo=None):
     return getDataAvailability(None, 'TARIFFLINE', None, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo)
 
+
 def getTarifflineDataAvailability(subscription_key, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom=None, publishedDateTo=None):
     return getDataAvailability(subscription_key, 'TARIFFLINE', None, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo)
 
+
 def getFinalDataBulkAvailability(subscription_key, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom=None, publishedDateTo=None):
     return getDataAvailability(subscription_key, 'FINAL', 'BULK', typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo)
 
+
 def getFinalClassicDataBulkAvailability(subscription_key, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom=None, publishedDateTo=None):
     return getDataAvailability(subscription_key, 'FINALCLASSIC', 'BULK', typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo)
 
+
 def getTarifflineDataBulkAvailability(subscription_key, typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom=None, publishedDateTo=None):
     return getDataAvailability(subscription_key, 'TARIFFLINE', 'BULK', typeCode, freqCode, clCode, period, reporterCode, publishedDateFrom, publishedDateTo)
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/Metadata.py` & `comtradeapicall-1.2.1/src/comtradeapicall/Metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,113 @@
 import pandas as pd
 import json
 from pandas import json_normalize
 import urllib3
 
 
-
-def getMetadata(subscription_key, typeCode, freqCode, clCode, period, reporterCode, showHistory):
-    if(subscription_key is None):
+def getMetadata(subscription_key, typeCode, freqCode, clCode, period, reporterCode, showHistory, proxy_url=None):
+    if (subscription_key is None):
         endpoint = "public"
-    else:  
+    else:
         endpoint = "data"
-    
-    baseURL = 'https://comtradeapi.un.org/' + endpoint + '/v1/getMetadata/' + typeCode + '/' + freqCode + '/' + clCode
+
+    baseURL = 'https://comtradeapi.un.org/' + endpoint + \
+        '/v1/getMetadata/' + typeCode + '/' + freqCode + '/' + clCode
     PARAMS = dict(reporterCode=reporterCode, period=period)
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET",baseURL, fields = fields, timeout=120)
+        resp = http.request("GET", baseURL, fields=fields, timeout=120)
         if resp.status != 200:
             print(resp.data.decode('utf-8'))
         else:
             jsonResult = json.loads(resp.data)
             df = json_normalize(jsonResult['data'])
             FIELDS = ['notes']
             dt = df[FIELDS]
             dt = dt.explode('notes')
             df_final = (
                 pd.DataFrame(dt["notes"]
                              .apply(pd.Series))
             )
-            dt_final_latest = df_final[['datasetCode', 'publicationDate']].groupby("datasetCode").max()
+            dt_final_latest = df_final[['datasetCode', 'publicationDate']].groupby(
+                "datasetCode").max()
             dt_final_latest.loc[:, 'isLatestPublication'] = True
-            df_final_merge = df_final.merge(dt_final_latest, on='publicationDate', how='left')
-            if (showHistory == True):
+            df_final_merge = df_final.merge(
+                dt_final_latest, on='publicationDate', how='left')
+            if (showHistory):
                 return df_final_merge
             else:
                 return df_final_merge[df_final_merge.notnull()].query('isLatestPublication==True')
     except urllib3.exceptions.RequestError as err:
         print(f'Request error: {err}')
 
+
 def _getMetadata(typeCode, freqCode, clCode, period, reporterCode, showHistory):
     return getMetadata(None, typeCode, freqCode, clCode, period, reporterCode, showHistory)
 
-def listReference(category=None):
+
+def listReference(category=None, proxy_url=None):
     baseURL = 'https://comtradeapi.un.org/files/v1/app/reference/ListofReferences.json'
     try:
-        http = urllib3.PoolManager()
-        resp = http.request("GET",baseURL, timeout=120)
+        if proxy_url:
+            http = urllib3.ProxyManager(proxy_url=proxy_url)
+        else:
+            http = urllib3.PoolManager()
+        resp = http.request("GET", baseURL, timeout=120)
         if resp.status != 200:
             print(resp.data.decode('utf-8'))
         else:
             resp.encoding = 'utf-8-sig'
             jsonResult = json.loads(resp.data)
             df = json_normalize(jsonResult['results'])
             if category is not None:
                 return df.query("category=='" + category + "'")
             else:
                 return df
     except urllib3.exceptions.RequestError as err:
         print(f'Request error: {err}')
 
-def getReference(category):
+
+def getReference(category, proxy_url=None):
     try:
         baseURL = listReference(category).iloc[0]['fileuri']
-    except:
+    except:  # noqa: E722
         baseURL = ''
         print('Error in looking up the file URI for', category)
     if baseURL != '':
         try:
-            http = urllib3.PoolManager()
-            resp = http.request("GET",baseURL, timeout=120)
+            if proxy_url:
+                http = urllib3.ProxyManager(proxy_url=proxy_url)
+            else:
+                http = urllib3.PoolManager()
+            resp = http.request("GET", baseURL, timeout=120)
             if resp.status != 200:
                 print(resp.data.decode('utf-8'))
             else:
                 resp.encoding = 'utf-8-sig'
                 jsonResult = json.loads(resp.data)
-                df = json_normalize(jsonResult['results'])  # Results contain the required data
+                # Results contain the required data
+                df = json_normalize(jsonResult['results'])
                 return df
         except urllib3.exceptions.RequestError as err:
             print(f'Request error: {err}')
 
-def convertCountryIso3ToCode(countryIsoCode):
+
+def convertCountryIso3ToCode(countryIsoCode, proxy_url=None):
     baseURL = 'https://comtradeapi.un.org/files/v1/app/reference/country_area_code_iso.json'
-    http = urllib3.PoolManager()
-    resp = http.request("GET",baseURL, timeout=120)
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
+    resp = http.request("GET", baseURL, timeout=120)
     df = json_normalize(json.loads(resp.data)['results'])
     df['country_area_code'] = df['country_area_code'].astype(str)
     delim = ','
     iso_string = countryIsoCode
     iso_list = iso_string.split(delim)
     code_list = df[df['iso3'].isin(iso_list)]['country_area_code'].tolist()
     code_string = delim.join(code_list)
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/PreviewGet.py` & `comtradeapicall-1.2.1/src/comtradeapicall/PreviewGet.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,185 +3,199 @@
 import json
 from pandas import json_normalize
 import urllib3
 
 
 def getPreviewData(subscription_key, tradeDataType, typeCode, freqCode, clCode, period, reporterCode, cmdCode,
                    flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
-                              breakdownMode,
-                              countOnly, includeDesc):
+                   partnerCode,
+                   partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
+                   breakdownMode,
+                   countOnly, includeDesc, proxy_url):
     if subscription_key is not None:
         if tradeDataType == 'TARIFFLINE':
-            baseURL = 'https://comtradeapi.un.org/data/v1/getTariffline/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/data/v1/getTariffline/' + \
+                typeCode + '/' + freqCode + '/' + clCode
         else:
-            baseURL = 'https://comtradeapi.un.org/data/v1/get/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/data/v1/get/' + \
+                typeCode + '/' + freqCode + '/' + clCode
     else:
         if tradeDataType == 'TARIFFLINE':
-            baseURL = 'https://comtradeapi.un.org/public/v1/previewTariffline/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/public/v1/previewTariffline/' + \
+                typeCode + '/' + freqCode + '/' + clCode
         else:
-            baseURL = 'https://comtradeapi.un.org/public/v1/preview/' + typeCode + '/' + freqCode + '/' + clCode
+            baseURL = 'https://comtradeapi.un.org/public/v1/preview/' + \
+                typeCode + '/' + freqCode + '/' + clCode
 
     PARAMS = dict(reportercode=reporterCode, flowCode=flowCode,
                   period=period, cmdCode=cmdCode, partnerCode=partnerCode, partner2Code=partner2Code,
                   motCode=motCode, customsCode=customsCode,
                   maxRecords=maxRecords, format=format_output, aggregateBy=aggregateBy, breakdownMode=breakdownMode,
                   countOnly=countOnly, includeDesc=includeDesc)
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     if format_output is None:
         format_output = 'JSON'
     if format_output != 'JSON':
         print("Only JSON output is supported with this function")
     else:
         try:
-            resp = http.request("GET",baseURL, fields = fields, timeout=120)
+            resp = http.request("GET", baseURL, fields=fields, timeout=120)
             if resp.status != 200:
                 print(resp.data.decode('utf-8'))
             else:
                 jsonResult = json.loads(resp.data)
                 if countOnly:
                     dictCount = dict(count=jsonResult['count'])
                     df = pandas.DataFrame([dictCount])
                 else:
-                    df = json_normalize(jsonResult['data'])  # Results contain the required data
+                    # Results contain the required data
+                    df = json_normalize(jsonResult['data'])
                 return df
         except urllib3.exceptions.RequestError as err:
             print(f'Request error: {err}')
 
+
 def previewFinalData(typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
-                            aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None):
+                     partnerCode,
+                     partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                     aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None, proxy_url=None):
     return getPreviewData(None, 'FINAL', typeCode, freqCode, clCode, period, reporterCode,
-                                  cmdCode, flowCode,
-                                  partnerCode,
-                                  partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
-                                  breakdownMode,
-                                  countOnly, includeDesc)
+                          cmdCode, flowCode,
+                          partnerCode,
+                          partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
+                          breakdownMode,
+                          countOnly, includeDesc, proxy_url)
+
 
 def _previewFinalData(typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
-                            aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None):
+                      partnerCode,
+                      partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                      aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None, proxy_url=None):
     main_df = pandas.DataFrame()
     for single_period in list(period.split(",")):
         try:
             staging_df = previewFinalData(typeCode, freqCode, clCode, single_period, reporterCode, cmdCode, flowCode,
                                           partnerCode,
                                           partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
                                           breakdownMode,
-                                          countOnly, includeDesc)
-        except: #retry once more after 10 secs
+                                          countOnly, includeDesc, proxy_url)
+        except:  # retry once more after 10 secs  # noqa: E722
             print('Repeating API call for period: ' + single_period)
             t.sleep(10)
             staging_df = previewFinalData(typeCode, freqCode, clCode, single_period, reporterCode, cmdCode, flowCode,
-                     partnerCode,
-                     partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
-                     breakdownMode,
-                     countOnly, includeDesc)
+                                          partnerCode,
+                                          partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
+                                          breakdownMode,
+                                          countOnly, includeDesc)
         main_df = pandas.concat([main_df, staging_df])
     return main_df
 
 
 def previewTarifflineData(typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords= None, format_output=None,
-                              countOnly=None, includeDesc=None):
+                          partnerCode,
+                          partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                          countOnly=None, includeDesc=None, proxy_url=None):
     return getPreviewData(None, 'TARIFFLINE', typeCode, freqCode, clCode, period, reporterCode,
-                                  cmdCode, flowCode,
-                                  partnerCode,
-                                  partner2Code, customsCode, motCode, maxRecords, format_output, None,
-                                  None,
-                                  countOnly, includeDesc)
+                          cmdCode, flowCode,
+                          partnerCode,
+                          partner2Code, customsCode, motCode, maxRecords, format_output, None,
+                          None,
+                          countOnly, includeDesc, proxy_url)
+
 
 def _previewTarifflineData(typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords= None, format_output=None,
-                              countOnly=None, includeDesc=None):
+                           partnerCode,
+                           partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                           countOnly=None, includeDesc=None, proxy_url=None):
     main_df = pandas.DataFrame()
     for single_period in list(period.split(",")):
         try:
             staging_df = previewTarifflineData(typeCode, freqCode, clCode, single_period, reporterCode, cmdCode,
                                                flowCode,
                                                partnerCode,
                                                partner2Code, customsCode, motCode, maxRecords, format_output,
-                                               countOnly, includeDesc)
-        except: #retry once more after 10 secs
+                                               countOnly, includeDesc, proxy_url)
+        except:  # retry once more after 10 secs  # noqa: E722
             print('Repeating API call for period: ' + single_period)
             t.sleep(10)
             staging_df = previewTarifflineData(typeCode, freqCode, clCode, single_period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords, format_output,
-                              countOnly, includeDesc)
+                                               partnerCode,
+                                               partner2Code, customsCode, motCode, maxRecords, format_output,
+                                               countOnly, includeDesc)
         main_df = pandas.concat([main_df, staging_df])
     return main_df
 
+
 def getFinalData(subscription_key, typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
-                            aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None):
+                 partnerCode,
+                 partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                 aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None, proxy_url=None):
     return getPreviewData(subscription_key, 'FINAL', typeCode, freqCode, clCode, period, reporterCode,
-                                  cmdCode, flowCode,
-                                  partnerCode,
-                                  partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
-                                  breakdownMode,
-                                  countOnly, includeDesc)
+                          cmdCode, flowCode,
+                          partnerCode,
+                          partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
+                          breakdownMode,
+                          countOnly, includeDesc, proxy_url)
+
 
 def _getFinalData(subscription_key, typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
-                            aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None):
+                  partnerCode,
+                  partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                  aggregateBy=None, breakdownMode=None, countOnly=None, includeDesc=None, proxy_url=None):
     main_df = pandas.DataFrame()
     for single_period in list(period.split(",")):
         try:
             staging_df = getFinalData(subscription_key, typeCode, freqCode, clCode, single_period, reporterCode,
                                       cmdCode,
                                       flowCode, partnerCode,
                                       partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
                                       breakdownMode,
-                                      countOnly, includeDesc)
-        except: #retry once more after 10 secs
+                                      countOnly, includeDesc, proxy_url)
+        except:  # retry once more after 10 secs  # noqa: E722
             print('Repeating API call for period: ' + single_period)
             t.sleep(10)
             staging_df = getFinalData(subscription_key, typeCode, freqCode, clCode, single_period, reporterCode, cmdCode,
-                                  flowCode, partnerCode,
-                                  partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
-                                  breakdownMode,
-                                  countOnly, includeDesc)
+                                      flowCode, partnerCode,
+                                      partner2Code, customsCode, motCode, maxRecords, format_output, aggregateBy,
+                                      breakdownMode,
+                                      countOnly, includeDesc, proxy_url)
         main_df = pandas.concat([main_df, staging_df])
     return main_df
 
+
 def getTarifflineData(subscription_key, typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords= None, format_output=None,
-                              countOnly=None, includeDesc=None):
+                      partnerCode,
+                      partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                      countOnly=None, includeDesc=None, proxy_url=None):
     return getPreviewData(subscription_key, 'TARIFFLINE', typeCode, freqCode, clCode, period, reporterCode,
-                                  cmdCode, flowCode,
-                                  partnerCode,
-                                  partner2Code, customsCode, motCode, maxRecords, format_output, None,
-                                  None,
-                                  countOnly, includeDesc)
+                          cmdCode, flowCode,
+                          partnerCode,
+                          partner2Code, customsCode, motCode, maxRecords, format_output, None,
+                          None,
+                          countOnly, includeDesc, proxy_url)
+
 
 def _getTarifflineData(subscription_key, typeCode, freqCode, clCode, period, reporterCode, cmdCode, flowCode,
-                              partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords= None, format_output=None,
-                              countOnly=None, includeDesc=None):
+                       partnerCode,
+                       partner2Code, customsCode, motCode, maxRecords=None, format_output=None,
+                       countOnly=None, includeDesc=None, proxy_url=None):
     main_df = pandas.DataFrame()
     for single_period in list(period.split(",")):
         try:
             staging_df = getTarifflineData(subscription_key, typeCode, freqCode, clCode, single_period, reporterCode,
-                              cmdCode, flowCode, partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords, format_output,
-                              countOnly, includeDesc)
-        except: #retry once more after 10 secs
+                                           cmdCode, flowCode, partnerCode,
+                                           partner2Code, customsCode, motCode, maxRecords, format_output,
+                                           countOnly, includeDesc, proxy_url)
+        except:  # retry once more after 10 secs  # noqa: E722
             print('Repeating API call for period: ' + single_period)
             t.sleep(10)
             staging_df = getTarifflineData(subscription_key, typeCode, freqCode, clCode, single_period, reporterCode,
-                              cmdCode, flowCode, partnerCode,
-                              partner2Code, customsCode, motCode, maxRecords, format_output,
-                              countOnly, includeDesc)
+                                           cmdCode, flowCode, partnerCode,
+                                           partner2Code, customsCode, motCode, maxRecords, format_output,
+                                           countOnly, includeDesc, proxy_url)
         main_df = pandas.concat([main_df, staging_df])
     return main_df
-
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/SUV.py` & `comtradeapicall-1.2.1/src/comtradeapicall/SUV.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import json
 from pandas import json_normalize
 import urllib3
 
+
 def getSUV(subscription_key, typeCode='C', freqCode='A', clCode='HS', period=None, cmdCode=None,
-                   flowCode=None, qtyUnitCode=None):
-    baseURL = 'https://comtradeapi.un.org/data/v1/getSUV/' + typeCode + '/' + freqCode + '/' + clCode
+           flowCode=None, qtyUnitCode=None, proxy_url=None):
+    baseURL = 'https://comtradeapi.un.org/data/v1/getSUV/' + \
+        typeCode + '/' + freqCode + '/' + clCode
 
-    PARAMS = dict(flowCode=flowCode, period=period, cmdCode=cmdCode, qtyUnitCode=qtyUnitCode)
+    PARAMS = dict(flowCode=flowCode, period=period,
+                  cmdCode=cmdCode, qtyUnitCode=qtyUnitCode)
     PARAMS["subscription-key"] = subscription_key
-    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))  
-    http = urllib3.PoolManager()
+    fields = dict(filter(lambda item: item[1] is not None, PARAMS.items()))
+    if proxy_url:
+        http = urllib3.ProxyManager(proxy_url=proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        resp = http.request("GET",baseURL, fields = fields, timeout=120)
+        resp = http.request("GET", baseURL, fields=fields, timeout=120)
         if resp.status != 200:
             print(resp.data)
         else:
             jsonResult = json.loads(resp.data)
             df = json_normalize(jsonResult['data'])
             return df
     except urllib3.exceptions.RequestError as err:
-        print(f'Request error: {err}')
+        print(f'Request error: {err}')
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall/__init__.py` & `comtradeapicall-1.2.1/src/comtradeapicall/__init__.py`

 * *Files identical despite different names*

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall.egg-info/PKG-INFO` & `comtradeapicall-1.2.1/src/comtradeapicall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comtradeapicall
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package to call UN Comtrade APIs
 Author-email: untradestats <untradestats@gmail.com>
 Project-URL: Homepage, https://github.com/uncomtrade/comtradeapicall
 Project-URL: Bug Tracker, https://github.com/uncomtrade/comtradeapicall/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 # UN Comtrade API Package
 This package simplifies calling [APIs of UN Comtrade](https://comtradedeveloper.un.org) to extract and download data
  (and much more). 
 
 ## Details
 [UN Comtrade](https://comtrade.un.org) provides free and premium APIs to extract and download data/metadata, however
  it is quite a learning curve to understand all of APIs end-points and parameters. This package simplifies it by
-  calling a single python function with the appropriate parameters. Learn more about UN Comtrade at the [UN Comtrade wiki](https://unstats.un.org/wiki/display/comtrade/UN+Comtrade).
+  calling a single python function with the appropriate parameters. Learn more about UN Comtrade at the [UN Comtrade Docs](https://uncomtrade.org/docs).
 
 This project is intended to be deployed at [The Python Package Index](https://pypi.org/project/comtradeapicall/), therefore the structure of
  folders follows the suggested layout from [Packaging Python Project](https://packaging.python.org/en/latest/tutorials/packaging-projects/). The main scripts are located at **/src/comtradeapicall/**. And the folder **tests** contains the example scripts how to install and use the package.
  
  ## Prerequisites
 This package assumes using Python 3.7 and the expected package dependencies are listed in the "requirements.txt" file
  for PIP, you need to run the following command to get dependencies:
@@ -94,15 +94,15 @@
 
 - **SUV:** Model class to extract data on Standard Unit Values (SUV) and their ranges
   - getSUV(**subscription_key**, **SelectionCriteria**, **[qtyUnitCode]**) : return data frame with SUV data
 
 - **AIS:** Model class to extract experimental trade data generated from AIS (ships tracking movement). See [Cerdeiro, Komaromi, Liu and Saeed (2020)](https://www.imf.org/en/Publications/WP/Issues/2020/05/14/World-Seaborne-Trade-in-Real-Time-A-Proof-of-Concept-for-Building-AIS-based-Nowcasts-from-49393). *When consuming the data, users should understand its limitation.*  
   - getAIS(**subscription_key**, **AISSelectionCriteria**, **[vesselTypeCode]**) : return data frame with AIS trade data
 
-See differences between final and tariff line data at the [Wiki](https://unstats.un.org/wiki/display/comtrade/New+Comtrade+FAQ+for+First+Time+Users#NewComtradeFAQforFirstTimeUsers-Whatisthetarifflinedata?)
+See differences between final and tariff line data at the [Docs](https://uncomtrade.org/docs/what-is-tariffline-data/)
  
 ## Selection Criteria
 - typeCode(str) : Product type. Goods (C) or Services (S)
 - freqCode(str) : The time interval at which observations occur. Annual (A) or Monthly (M)
 - clCode(str) : Indicates the product classification used and which version (HS, SITC)
 - period(str) :  Combination of year and month (for monthly), year for (annual)
 - reporterCode(str) : The country or geographic area to which the measured statistical phenomenon relates
@@ -124,14 +124,18 @@
 ## AIS Selection Criteria
 - typeCode(str) : Product type. Only Goods (C)
 - freqCode(str) : The time interval at which observations occur. Daily (D)
 - datefrom(str) and dateto(str) :  Date(s) of observation - ASCII format
 - countryareaCode(str) : The country or geographic area to which the measured statistical phenomenon relates. Use *getReference('ais:countriesareas')* for the complete list.
 - vesselTypeCode(str) : The high level categorization of vessels transporting the goods. Use *getReference('ais:vesseltypes')* for the complete list.
 - flowCode(str) : Trade flow (exports, imports)
+
+## Proxy Server
+- proxy_url(str) : All functions that call the API support the proxy server. Use the parameter proxy_url.
+
  
 ## Examples of python usage
 - Extract Australia imports of commodity code 91 in classic mode in May 2022
 ``` python
 mydf = comtradeapicall.previewFinalData(typeCode='C', freqCode='M', clCode='HS', period='202205',
                                         reporterCode='36', cmdCode='91', flowCode='M', partnerCode=None,
                                         partner2Code=None,
```

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall.egg-info/PKG-INFO-W10LT-PF2ZCSNL` & `comtradeapicall-1.2.1/src/comtradeapicall.egg-info/PKG-INFO-W10LT-PF2ZCSNL`

 * *Files identical despite different names*

### Comparing `comtradeapicall-1.2.0/src/comtradeapicall.egg-info/SOURCES.txt` & `comtradeapicall-1.2.1/src/comtradeapicall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

