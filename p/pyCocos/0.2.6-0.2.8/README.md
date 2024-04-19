# Comparing `tmp/pycocos-0.2.6.tar.gz` & `tmp/pycocos-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycocos-0.2.6.tar", last modified: Mon Apr 15 18:59:45 2024, max compression
+gzip compressed data, was "pycocos-0.2.8.tar", last modified: Fri Apr 19 05:57:54 2024, max compression
```

## Comparing `pycocos-0.2.6.tar` & `pycocos-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:59:45.304827 pycocos-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 18:59:41.000000 pycocos-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-15 18:59:45.300827 pycocos-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-15 18:59:41.000000 pycocos-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:59:45.304827 pycocos-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 18:59:41.000000 pycocos-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:59:45.300827 pycocos-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:59:45.300827 pycocos-0.2.6/src/pyCocos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-15 18:59:45.000000 pycocos-0.2.6/src/pyCocos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-15 18:59:45.000000 pycocos-0.2.6/src/pyCocos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:59:45.000000 pycocos-0.2.6/src/pyCocos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 18:59:45.000000 pycocos-0.2.6/src/pyCocos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 18:59:45.000000 pycocos-0.2.6/src/pyCocos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:59:45.300827 pycocos-0.2.6/src/pycocos/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 18:59:41.000000 pycocos-0.2.6/src/pycocos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:59:45.300827 pycocos-0.2.6/src/pycocos/components/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 18:59:41.000000 pycocos-0.2.6/src/pycocos/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15851 2024-04-15 18:59:41.000000 pycocos-0.2.6/src/pycocos/components/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-15 18:59:41.000000 pycocos-0.2.6/src/pycocos/components/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 18:59:41.000000 pycocos-0.2.6/src/pycocos/components/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-15 18:59:41.000000 pycocos-0.2.6/src/pycocos/components/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    53060 2024-04-15 18:59:41.000000 pycocos-0.2.6/src/pycocos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.963013 pycocos-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 05:57:51.000000 pycocos-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-19 05:57:54.963013 pycocos-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-19 05:57:51.000000 pycocos-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:57:54.963013 pycocos-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-19 05:57:51.000000 pycocos-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.959012 pycocos-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.963013 pycocos-0.2.8/src/pyCocos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.959012 pycocos-0.2.8/src/pycocos/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.963013 pycocos-0.2.8/src/pycocos/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15891 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53080 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/main.py
```

### Comparing `pycocos-0.2.6/LICENSE` & `pycocos-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.6/PKG-INFO` & `pycocos-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.6
+Version: 0.2.8
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycocos-0.2.6/README.md` & `pycocos-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.6/setup.py` & `pycocos-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyCocos",
-    version="0.2.6",
+    version="0.2.8",
     author="Nacho Herrera",
     author_email="github@nachoherrera.com.ar",
     description="Python connector for Cocos Capital's Rest APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nacho-herrera/pyCocos",
     packages=setuptools.find_packages(where='src'),
```

### Comparing `pycocos-0.2.6/src/pyCocos.egg-info/PKG-INFO` & `pycocos-0.2.8/src/pyCocos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.6
+Version: 0.2.8
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycocos-0.2.6/src/pycocos/components/client.py` & `pycocos-0.2.8/src/pycocos/components/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,19 +332,19 @@
             segment (str): Segment of instruments
 
         Returns:
             list: List of instruments quotes
         """
         return self.api_request(
             urls.endpoints["tickers_list"].format(
-                instrument_type.value,
-                instrumet_subtype.value,
-                settlement.value,
-                currency.value,
-                segment.value,
+                instrument_type,
+                instrumet_subtype,
+                settlement,
+                currency,
+                segment,
             )
         )
 
     def get_tickers_pagination(
         self,
         instrument_type: str,
         instrument_subtype: str,
@@ -461,15 +461,15 @@
                 json=json_data,
             )
 
         if method == "delete":
             response = self.session.delete(self._api_url(path), json=json_data)
 
         if not response:
-            raise ApiException("Bad HTTP API Response")
+            raise ApiException(f"Bad HTTP API Response. Error code: {response.status_code}. Server response {response.text}")
 
         json_response = simplejson.loads(response.text)
 
         if response.status_code == 401:
             if retry:
                 self.api_request(path, retry=False)
             else:
```

### Comparing `pycocos-0.2.6/src/pycocos/components/enums.py` & `pycocos-0.2.8/src/pycocos/components/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     OTROS = "OTROS"
     PF = "PF"
     PROV = "PROVINCIALES"
     TOP = "TOP"
     USD = "NACIONALES_USD"
     BONOS_CORP = "BONOSC"
 
-
 class Settlement(Enum):
     """Enumerates the settlement options for trades in the application."""
 
     T0 = "CI"
     T1 = "24hs"
     T2 = "48hs"
     NONE = ""
```

### Comparing `pycocos-0.2.6/src/pycocos/components/urls.py` & `pycocos-0.2.8/src/pycocos/components/urls.py`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.6/src/pycocos/main.py` & `pycocos-0.2.8/src/pycocos/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
 
         Returns:
             bool: True if there are sufficient funds, False otherwise.
         """
         long_ticker: str = payload['long_ticker']
         instrument_code, settlement, segment, _, currency = long_ticker.split("-")
         
-        #instrument_code = self._find_instrument_code(long_ticker)
+        global_instrument_code = self._find_instrument_code(long_ticker)
         settlement = self._get_cocos_settlement(settlement)
         segment = self._get_cocos_segment(segment)
         
         if not settlement or not segment:
             return False
 
         # validate the possible combinations of order parameters
@@ -1124,20 +1124,20 @@
             if "price" in payload:
                 raise ApiException("The paramenter 'price' can't be present in MARKET order")
             if "amount" in payload and "quantity" in payload:
                 raise ApiException("The parameters 'amount' and 'quantity' can't be present simultaneously in MARKET order")
         
         # check order total
         if "price" not in payload:
-            price = self._get_instrument_snapshot_value_by_key(instrument_code, long_ticker, segment, "ask")
+            price = self._get_instrument_snapshot_value_by_key(global_instrument_code, long_ticker, segment, "ask")
         else:
             price = payload["price"]
         
         if 'amount' not in payload.items():
-            price_factor = self._get_price_factor(instrument_code, long_ticker, segment)
+            price_factor = self._get_price_factor(global_instrument_code, long_ticker, segment)
             order_total = float(payload["quantity"]) * float(payload["price"]) / price_factor
         else:
             order_total = float(payload["amount"])
         
         available_funds = self.funds_available()
         available_at_settlement_currency: float = available_funds[settlement.value][
             currency.lower()
```

