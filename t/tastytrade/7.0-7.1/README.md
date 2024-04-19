# Comparing `tmp/tastytrade-7.0.tar.gz` & `tmp/tastytrade-7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-7.0.tar", last modified: Thu Feb 29 17:38:04 2024, max compression
+gzip compressed data, was "tastytrade-7.1.tar", last modified: Fri Apr 19 04:30:20 2024, max compression
```

## Comparing `tastytrade-7.0.tar` & `tastytrade-7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:38:04.755018 tastytrade-7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-29 17:38:01.000000 tastytrade-7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-02-29 17:38:04.755018 tastytrade-7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-02-29 17:38:01.000000 tastytrade-7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 17:38:04.755018 tastytrade-7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-29 17:38:01.000000 tastytrade-7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:38:04.751018 tastytrade-7.0/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38112 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:38:04.755018 tastytrade-7.0/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/dxfeed/underlying.py
--rw-r--r--   0 runner    (1001) docker     (127)    34948 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    33901 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-02-29 17:38:01.000000 tastytrade-7.0/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:38:04.755018 tastytrade-7.0/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-02-29 17:38:04.000000 tastytrade-7.0/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-29 17:38:04.000000 tastytrade-7.0/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 17:38:04.000000 tastytrade-7.0/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-29 17:38:04.000000 tastytrade-7.0/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-29 17:38:04.000000 tastytrade-7.0/tastytrade.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 17:38:04.755018 tastytrade-7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-02-29 17:38:01.000000 tastytrade-7.0/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-02-29 17:38:01.000000 tastytrade-7.0/tests/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-29 17:38:01.000000 tastytrade-7.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-29 17:38:01.000000 tastytrade-7.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-29 17:38:01.000000 tastytrade-7.0/tests/test_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-02-29 17:38:01.000000 tastytrade-7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-29 17:38:01.000000 tastytrade-7.0/tests/test_watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.329897 tastytrade-7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 04:30:15.000000 tastytrade-7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-19 04:30:20.329897 tastytrade-7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-19 04:30:15.000000 tastytrade-7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 04:30:20.329897 tastytrade-7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-19 04:30:15.000000 tastytrade-7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.325897 tastytrade-7.1/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38112 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.325897 tastytrade-7.1/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/underlying.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35007 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.329897 tastytrade-7.1/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.329897 tastytrade-7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_watchlists.py
```

### Comparing `tastytrade-7.0/LICENSE` & `tastytrade-7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/PKG-INFO` & `tastytrade-7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 7.0
+Version: 7.1
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3
 Requires-Dist: websockets>=11.0.3
 Requires-Dist: pydantic>=2.6.3
 Requires-Dist: pandas_market_calendars>=4.3.3
+Requires-Dist: fake_useragent>=1.5.1
 
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
    :alt: PyPI Package
 
 .. image:: https://static.pepy.tech/badge/tastytrade
    :target: https://pepy.tech/project/tastytrade
    :alt: PyPI Downloads
 
+
 Tastytrade Python SDK
 =====================
 
 A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
```

### Comparing `tastytrade-7.0/README.rst` & `tastytrade-7.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
    :target: https://pypi.org/project/tastytrade
    :alt: PyPI Package
 
 .. image:: https://static.pepy.tech/badge/tastytrade
    :target: https://pepy.tech/project/tastytrade
    :alt: PyPI Downloads
 
+
 Tastytrade Python SDK
 =====================
 
 A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
```

### Comparing `tastytrade-7.0/setup.py` & `tastytrade-7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 
 f = open('README.rst', 'r')
 LONG_DESCRIPTION = f.read()
 f.close()
 
 setup(
     name='tastytrade',
-    version='7.0',
+    version='7.1',
     description='An unofficial SDK for Tastytrade!',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
     license='MIT',
     install_requires=[
         'requests<3',
         'websockets>=11.0.3',
         'pydantic>=2.6.3',
-        'pandas_market_calendars>=4.3.3'
+        'pandas_market_calendars>=4.3.3',
+        'fake_useragent>=1.5.1',
     ],
     packages=find_packages(exclude=['ez_setup', 'tests*']),
     include_package_data=True
 )
```

### Comparing `tastytrade-7.0/tastytrade/__init__.py` & `tastytrade-7.1/tastytrade/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import logging
 
 API_URL = 'https://api.tastyworks.com'
 CERT_URL = 'https://api.cert.tastyworks.com'
-VERSION = '7.0'
+VERSION = '7.1'
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 from .account import Account  # noqa: E402
 from .search import symbol_search  # noqa: E402
 from .session import CertificationSession, ProductionSession  # noqa: E402
-from .streamer import (AccountStreamer, DXFeedStreamer,  # noqa: E402
-                       DXLinkStreamer)
+from .streamer import AccountStreamer, DXLinkStreamer  # noqa: E402
 from .watchlists import PairsWatchlist, Watchlist  # noqa: E402
 
 __all__ = [
     'Account',
     'AccountStreamer',
     'CertificationSession',
-    'DXFeedStreamer',
     'DXLinkStreamer',
     'PairsWatchlist',
     'ProductionSession',
     'Watchlist',
     'symbol_search'
 ]
```

### Comparing `tastytrade-7.0/tastytrade/account.py` & `tastytrade-7.1/tastytrade/account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/candle.py` & `tastytrade-7.1/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/event.py` & `tastytrade-7.1/tastytrade/dxfeed/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,12 +46,14 @@
         """
         objs = []
         size = len(cls.model_fields)
         multiples = len(data) / size
         if not multiples.is_integer():
             msg = 'Mapper data input values are not a multiple of the key size'
             raise TastytradeError(msg)
+        keys = cls.model_fields.keys()
         for i in range(int(multiples)):
             offset = i * size
             local_values = data[offset:(i + 1) * size]
-            objs.append(cls(*local_values))
+            event_dict = dict(zip(keys, local_values))
+            objs.append(cls(**event_dict))
         return objs
```

### Comparing `tastytrade-7.0/tastytrade/dxfeed/greeks.py` & `tastytrade-7.1/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/profile.py` & `tastytrade-7.1/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/quote.py` & `tastytrade-7.1/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/summary.py` & `tastytrade-7.1/tastytrade/dxfeed/summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 from .event import Event
 
 
 class Summary(Event):
     """
     Summary is an information snapshot about the trading session including
-    session highs, lows, etc. This record has two goals:
-
-    1. Transmit OHLC values.
-    2. Provide data for charting. OHLC is required for a daily chart, and
-    if an exchange does not provide it, the charting services refer to the
+    session highs, lows, etc. This record has two goals: Transmit OHLC
+    values, and provide data for charting. OHLC is required for a daily chart,
+    and if an exchange does not provide it, the charting services refer to the
     Summary event.
 
     Before opening the bidding, the values are reset to N/A or NaN.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
```

### Comparing `tastytrade-7.0/tastytrade/dxfeed/theoprice.py` & `tastytrade-7.1/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/timeandsale.py` & `tastytrade-7.1/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/trade.py` & `tastytrade-7.1/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/dxfeed/underlying.py` & `tastytrade-7.1/tastytrade/dxfeed/underlying.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/instruments.py` & `tastytrade-7.1/tastytrade/instruments.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
     """
     Dataclass representing a specific strike in an options chain, containing
     the symbols for the call and put options.
     """
     strike_price: Decimal
     call: str
     put: str
+    call_streamer_symbol: str
+    put_streamer_symbol: str
 
 
 class TickSize(TastytradeJsonDataclass):
     """
     Dataclass representing the tick size for an instrument.
     """
     value: Decimal
```

### Comparing `tastytrade-7.0/tastytrade/metrics.py` & `tastytrade-7.1/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/order.py` & `tastytrade-7.1/tastytrade/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date, datetime
 from decimal import Decimal
 from enum import Enum
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from tastytrade import VERSION
 from tastytrade.utils import TastytradeJsonDataclass
 
 
 class InstrumentType(str, Enum):
     """
@@ -279,28 +279,28 @@
     in_flight_at: Optional[datetime] = None
     live_at: Optional[datetime] = None
     received_at: Optional[datetime] = None
     reject_reason: Optional[str] = None
     user_id: Optional[str] = None
     username: Optional[str] = None
     terminal_at: Optional[datetime] = None
-    complex_order_id: Optional[str] = None
+    complex_order_id: Optional[Union[str, int]] = None
     complex_order_tag: Optional[str] = None
-    preflight_id: Optional[str] = None
+    preflight_id: Optional[Union[str, int]] = None
     order_rule: Optional[OrderRule] = None
 
 
 class PlacedComplexOrder(TastytradeJsonDataclass):
     """
     Dataclass containing information about an already placed complex order.
     """
     account_number: str
     type: str
     orders: List[PlacedOrder]
-    id: Optional[str] = None
+    id: Optional[Union[str, int]] = None
     trigger_order: Optional[PlacedOrder] = None
     terminal_at: Optional[str] = None
     ratio_price_threshold: Optional[Decimal] = None
     ratio_price_comparator: Optional[str] = None
     ratio_price_is_threshold_based_on_notional: Optional[bool] = None
     related_orders: Optional[List[Dict[str, str]]] = None
```

### Comparing `tastytrade-7.0/tastytrade/search.py` & `tastytrade-7.1/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade/session.py` & `tastytrade-7.1/tastytrade/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from abc import ABC
 from typing import Any, Dict, Optional
 
 import requests
+from fake_useragent import UserAgent  # type: ignore
 
 from tastytrade import API_URL, CERT_URL
-from tastytrade.utils import TastytradeError, validate_response
+from tastytrade.utils import (TastytradeError, TastytradeJsonDataclass,
+                              validate_response)
+
+
+class TwoFactorInfo(TastytradeJsonDataclass):
+    is_active: bool
+    type: Optional[str] = None
 
 
 class Session(ABC):
     """
     An abstract class which contains the basic functionality of a session.
     """
     base_url: str
@@ -104,14 +111,27 @@
         #: A single-use token which can be used to login without a password
         self.remember_token: Optional[str] = \
             json['data']['remember-token'] if remember_me else None
         #: The headers to use for API requests
         self.headers: Dict[str, str] = {'Authorization': self.session_token}
         self.validate()
 
+        # Pull streamer tokens and urls
+        response = requests.get(
+            f'{self.base_url}/api-quote-tokens',
+            headers=self.headers
+        )
+        validate_response(response)
+        data = response.json()['data']
+        self.streamer_token = data['token']
+        self.dxlink_url = data['dxlink-url']
+        self.streamer_headers = {
+            'Authorization': f'Bearer {self.streamer_token}'
+        }
+
 
 class ProductionSession(Session):
     """
     Contains a local user login which can then be used to interact with the
     remote API.
 
     :param login: tastytrade username or email
@@ -163,25 +183,41 @@
         self.user: Dict[str, str] = json['data']['user']
         #: The session token used to authenticate requests
         self.session_token: str = json['data']['session-token']
         #: A single-use token which can be used to login without a password
         self.remember_token: Optional[str] = \
             json['data']['remember-token'] if remember_me else None
         #: The headers to use for API requests
-        self.headers: Dict[str, str] = {'Authorization': self.session_token}
+        self.headers: Dict[str, str] = {
+            'Authorization': self.session_token,
+            'User-Agent': UserAgent().random
+        }
         self.validate()
 
-        #: Pull streamer tokens and urls
+        # Pull streamer tokens and urls
         response = requests.get(
             f'{self.base_url}/quote-streamer-tokens',
             headers=self.headers
         )
         validate_response(response)
         data = response.json()['data']
         self.streamer_token = data['token']
-        url = data['websocket-url'] + '/cometd'
-        self.dxfeed_url = url.replace('https', 'wss')
         self.dxlink_url = data['dxlink-url']
-        self.rest_url = data['websocket-url'] + '/rest/events.json'
         self.streamer_headers = {
             'Authorization': f'Bearer {self.streamer_token}'
         }
+
+    def get_2fa_info(self) -> TwoFactorInfo:
+        """
+        Gets the 2FA info for the current user.
+
+        :return: a dictionary containing the 2FA info.
+        """
+        response = requests.get(
+            f'{self.base_url}/users/me/two-factor-method',
+            headers=self.headers
+        )
+        validate_response(response)
+
+        data = response.json()['data']
+
+        return TwoFactorInfo(**data)
```

### Comparing `tastytrade-7.0/tastytrade/streamer.py` & `tastytrade-7.1/tastytrade/streamer.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 from typing import Any, AsyncIterator, Dict, List, Optional, Union
 
 import websockets
 
 from tastytrade import logger
 from tastytrade.account import (Account, AccountBalance, CurrentPosition,
                                 TradingStatus)
-from tastytrade.dxfeed import (Candle, Channel, Event, EventType, Greeks,
-                               Profile, Quote, Summary, TheoPrice, TimeAndSale,
-                               Trade, Underlying)
+from tastytrade.dxfeed import (Candle, Event, EventType, Greeks, Profile,
+                               Quote, Summary, TheoPrice, TimeAndSale, Trade,
+                               Underlying)
 from tastytrade.order import (InstrumentType, OrderChain, PlacedOrder,
                               PriceEffect)
 from tastytrade.session import CertificationSession, ProductionSession, Session
 from tastytrade.utils import TastytradeError, TastytradeJsonDataclass
 from tastytrade.watchlists import Watchlist
 
 CERT_STREAMER_URL = 'wss://streamer.cert.tastyworks.com'
 STREAMER_URL = 'wss://streamer.tastyworks.com'
 
+DXLINK_VERSION = '0.1-js/0.40.4-WB2'
+
 
 class QuoteAlert(TastytradeJsonDataclass):
     """
     Dataclass that contains information about a quote alert
     """
     user_external_id: str
     symbol: str
@@ -248,364 +250,14 @@
         }
         if value:
             message['value'] = value
         logger.debug('sending alert subscription: %s', message)
         await self._websocket.send(json.dumps(message))  # type: ignore
 
 
-class DXFeedStreamer:  # pragma: no cover
-    """
-    A :class:`DXFeedStreamer` object is used to fetch quotes or greeks for a
-    given symbol or list of symbols. It should always be initialized as an
-    async context manager, or with the `create` function, since the object
-    cannot be fully instantiated without async.
-
-    Example usage::
-
-        from tastytrade import DXFeedStreamer
-        from tastytrade.dxfeed import EventType
-
-        # must be a production session
-        async with DXFeedStreamer(session) as streamer:
-            subs = ['SPY', 'GLD']  # list of quotes to fetch
-            await streamer.subscribe(EventType.QUOTE, subs)
-            quote = await streamer.get_event(EventType.QUOTE)
-            print(quote)
-
-    """
-    def __init__(self, session: ProductionSession):
-        self._counter = 0
-        self._lock: Lock = Lock()
-        self._queues: Dict[EventType, Queue] = defaultdict(Queue)
-        #: The unique client identifier received from the server
-        self.client_id: Optional[str] = None
-
-        self._auth_token = session.streamer_token
-        self._wss_url = session.dxfeed_url
-
-        self._connect_task = asyncio.create_task(self._connect())
-
-    async def __aenter__(self):
-        time_out = 100
-        while not self.client_id:
-            await asyncio.sleep(0.1)
-            time_out -= 1
-            if time_out < 0:
-                raise TastytradeError('Connection timed out')
-
-        return self
-
-    @classmethod
-    async def create(cls, session: ProductionSession) -> 'DXFeedStreamer':
-        self = cls(session)
-        return await self.__aenter__()
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self.close()
-
-    async def close(self):
-        """
-        Closes the websocket connection and cancels the heartbeat task.
-        """
-        self._connect_task.cancel()
-        self._heartbeat_task.cancel()
-
-    async def _next_id(self):
-        async with self._lock:
-            self._counter += 1
-        return self._counter
-
-    async def _connect(self) -> None:
-        """
-        Connect to the websocket server using the URL and
-        authorization token provided during initialization.
-        """
-        headers = {'Authorization': f'Bearer {self._auth_token}'}
-
-        async with websockets.connect(  # type: ignore
-            self._wss_url,
-            extra_headers=headers
-        ) as websocket:
-            self._websocket = websocket
-            await self._handshake()
-
-            while not self.client_id:
-                raw_message = await self._websocket.recv()
-                message = json.loads(raw_message)[0]
-
-                logger.debug('received: %s', message)
-                if message['channel'] == Channel.HANDSHAKE:
-                    if message['successful']:
-                        self.client_id = message['clientId']
-                        self._heartbeat_task = \
-                            asyncio.create_task(self._heartbeat())
-                    else:
-                        raise TastytradeError('Handshake failed')
-
-            # main loop
-            while True:
-                raw_message = await self._websocket.recv()
-                message = json.loads(raw_message)[0]
-
-                if (message['channel'] == Channel.DATA or
-                        message['channel'] == Channel.TIME_SERIES):
-                    logger.debug('data received: %s', message)
-                    await self._map_message(message['data'])
-                elif message['channel'] == Channel.SUBSCRIPTION:
-                    logger.debug('sub received: %s', message)
-
-    async def _handshake(self) -> None:
-        """
-        Sends a handshake message to the specified WebSocket
-        connection. The handshake message is sent as a JSON
-        encoded array with a single element, containing the
-        handshake message as its only element.
-        """
-        id = await self._next_id()
-        message = {
-            'id': id,
-            'version': '1.0',
-            'minimumVersion': '1.0',
-            'channel': Channel.HANDSHAKE,
-            'supportedConnectionTypes': [
-                'websocket',
-                'long-polling',
-                'callback-polling'
-            ],
-            'ext': {'com.devexperts.auth.AuthToken': self._auth_token},
-            'advice': {
-                'timeout': 60000,
-                'interval': 0
-            }
-        }
-        await self._websocket.send(json.dumps([message]))
-
-    async def listen(self, event_type: EventType) -> AsyncIterator[Event]:
-        """
-        Using the existing subscriptions, pulls events of the given type and
-        yield returns them. Never exits unless there's an error or the channel
-        is closed.
-
-        :param event_type: the type of event to listen for
-        """
-        while True:
-            yield await self._queues[event_type].get()
-
-    async def get_event(self, event_type: EventType) -> Event:
-        """
-        Using the existing subscription , pulls an event of the given type and
-        returns it.
-
-        :param event_type: the type of event to get
-        """
-        while True:
-            return await self._queues[event_type].get()
-
-    async def _heartbeat(self) -> None:
-        """
-        Sends a heartbeat message every 10 seconds to keep the connection
-        alive.
-        """
-        while True:
-            id = await self._next_id()
-            message = {
-                'id': id,
-                'channel': Channel.HEARTBEAT,
-                'clientId': self.client_id,
-                'connectionType': 'websocket'
-            }
-            logger.debug('sending heartbeat: %s', message)
-            await self._websocket.send(json.dumps([message]))
-            # send the heartbeat every 10 seconds
-            await asyncio.sleep(10)
-
-    async def subscribe(
-        self,
-        event_type: EventType,
-        symbols: List[str],
-        reset: bool = False
-    ) -> None:
-        """
-        Subscribes to quotes for given list of symbols. Used for recurring data
-        feeds.
-        For candles, use :meth:`subscribe_candle` instead.
-
-        :param event_type: type of subscription to add
-        :param symbols: list of symbols to subscribe for
-        :param reset:
-            whether to reset the subscription list (remove all other
-            subscriptions of all types)
-        """
-        id = await self._next_id()
-        message = {
-            'id': id,
-            'channel': Channel.SUBSCRIPTION,
-            'data': {
-                'reset': reset,
-                'add': {event_type: symbols}
-            },
-            'clientId': self.client_id
-        }
-        logger.debug('sending subscription: %s', message)
-        await self._websocket.send(json.dumps([message]))
-
-    async def unsubscribe(
-        self,
-        event_type: EventType,
-        symbols: List[str]
-    ) -> None:
-        """
-        Removes existing subscription for given list of symbols.
-        For candles, use :meth:`unsubscribe_candle` instead.
-
-        :param event_type: type of subscription to remove
-        :param symbols: list of symbols to unsubscribe from
-        """
-        id = await self._next_id()
-        message = {
-            'id': id,
-            'channel': Channel.SUBSCRIPTION,
-            'data': {'remove': {event_type: symbols}},
-            'clientId': self.client_id
-        }
-        logger.debug('sending unsubscription: %s', message)
-        await self._websocket.send(json.dumps([message]))
-
-    async def subscribe_candle(
-        self,
-        symbols: List[str],
-        interval: str,
-        start_time: datetime,
-        end_time: Optional[datetime] = None,
-        extended_trading_hours: bool = False,
-        reset: bool = False
-    ) -> None:
-        """
-        Subscribes to time series data for the given symbol.
-
-        :param symbols: list of symbols to get data for
-        :param interval:
-            the width of each candle in time, e.g. '15s', '5m', '1h', '3d',
-            '1w', '1mo'
-        :param start_time: starting time for the data range
-        :param end_time: ending time for the data range
-        :param extended_trading_hours: whether to include extended trading
-        :param reset: whether to reset the subscription list
-        """
-        id = await self._next_id()
-        key = EventType.CANDLE
-        message = {
-            'id': id,
-            'channel': Channel.SUBSCRIPTION,
-            'data': {
-                'reset': reset,
-                'addTimeSeries': {
-                    key: [{
-                        'eventSymbol': f'{ticker}{{={interval},tho=true}}'
-                        if extended_trading_hours
-                        else f'{ticker}{{={interval}}}',
-                        'fromTime': int(start_time.timestamp() * 1000)
-                    } for ticker in symbols]
-                }
-            },
-            'clientId': self.client_id
-        }
-        if end_time is not None:
-            message['data']['addTimeSeries'][key][0]['toTime'] = \
-                int(end_time.timestamp() * 1000)
-        await self._websocket.send(json.dumps([message]))
-
-    async def unsubscribe_candle(
-        self,
-        ticker: str,
-        interval: Optional[str] = None,
-        extended_trading_hours: bool = False
-    ) -> None:
-        """
-        Removes existing subscription for a candle.
-
-        :param ticker: symbol to unsubscribe from
-        :param interval: candle width to unsubscribe from
-        :param extended_trading_hours:
-            whether candle to unsubscribe from contains extended trading hours
-        """
-        id = await self._next_id()
-        message = {
-            'id': id,
-            'channel': Channel.SUBSCRIPTION,
-            'data': {
-                'removeTimeSeries': {
-                    EventType.CANDLE: [
-                        f'{ticker}{{={interval},tho=true}}'
-                        if extended_trading_hours
-                        else f'{ticker}{{={interval}}}'
-                    ]
-                }
-            },
-            'clientId': self.client_id
-        }
-        logger.debug('sending unsubscription: %s', message)
-        await self._websocket.send(json.dumps([message]))
-
-    async def _map_message(self, message) -> None:
-        """
-        Takes the raw JSON data, parses the events and places them into their
-        respective queues.
-
-        :param message: raw JSON data from the websocket
-        """
-        # the first time around, types are shown
-        if isinstance(message[0], str):
-            msg_type = message[0]
-        else:
-            msg_type = message[0][0]
-        # regardless, the second element will be the raw data
-        data = message[1]
-
-        # parse type or warn for unknown type
-        if msg_type == EventType.CANDLE:
-            candles = Candle.from_stream(data)
-            for candle in candles:
-                await self._queues[EventType.CANDLE].put(candle)
-        elif msg_type == EventType.GREEKS:
-            greeks = Greeks.from_stream(data)
-            for greek in greeks:
-                await self._queues[EventType.GREEKS].put(greek)
-        elif msg_type == EventType.PROFILE:
-            profiles = Profile.from_stream(data)
-            for profile in profiles:
-                await self._queues[EventType.PROFILE].put(profile)
-        elif msg_type == EventType.QUOTE:
-            quotes = Quote.from_stream(data)
-            for quote in quotes:
-                await self._queues[EventType.QUOTE].put(quote)
-        elif msg_type == EventType.SUMMARY:
-            summaries = Summary.from_stream(data)
-            for summary in summaries:
-                await self._queues[EventType.SUMMARY].put(summary)
-        elif msg_type == EventType.THEO_PRICE:
-            theo_prices = TheoPrice.from_stream(data)
-            for theo_price in theo_prices:
-                await self._queues[EventType.THEO_PRICE].put(theo_price)
-        elif msg_type == EventType.TIME_AND_SALE:
-            time_and_sales = TimeAndSale.from_stream(data)
-            for tas in time_and_sales:
-                await self._queues[EventType.TIME_AND_SALE].put(tas)
-        elif msg_type == EventType.TRADE:
-            trades = Trade.from_stream(data)
-            for trade in trades:
-                await self._queues[EventType.TRADE].put(trade)
-        elif msg_type == EventType.UNDERLYING:
-            underlyings = Underlying.from_stream(data)
-            for underlying in underlyings:
-                await self._queues[EventType.UNDERLYING].put(underlying)
-        else:
-            raise TastytradeError(f'Unknown message type received: {message}')
-
-
 class DXLinkStreamer:
     """
     A :class:`DXLinkStreamer` object is used to fetch quotes or greeks for a
     given symbol or list of symbols. It should always be initialized as an
     async context manager, or with the `create` function, since the object
     cannot be fully instantiated without async.
 
@@ -698,31 +350,31 @@
                         self._heartbeat_task = \
                             asyncio.create_task(self._heartbeat())
                 elif message['type'] == 'CHANNEL_OPENED':
                     channel = next(k for k, v in self._channels.items()
                                    if v == message['channel'])
                     self._subscription_state[channel] = message['type']
                 elif message['type'] == 'CHANNEL_CLOSED':
-                    pass
+                    logger.debug('Channel closed: %s', message)
                 elif message['type'] == 'FEED_CONFIG':
-                    pass
+                    logger.debug('Feed configured: %s', message)
                 elif message['type'] == 'FEED_DATA':
                     await self._map_message(message['data'])
                 elif message['type'] == 'KEEPALIVE':
                     pass
                 else:
                     raise TastytradeError('Unknown message type:', message)
 
     async def _setup_connection(self):
         message = {
             'type': 'SETUP',
             'channel': 0,
             'keepaliveTimeout': 60,
             'acceptKeepaliveTimeout': 60,
-            'version': '0.1-js/1.0.0'
+            'version': DXLINK_VERSION
         }
         await self._websocket.send(json.dumps(message))
 
     async def _authenticate_connection(self):
         message = {
             'type': 'AUTH',
             'channel': 0,
@@ -816,14 +468,51 @@
         await self._websocket.send(json.dumps(message))
         time_out = 100
         while not self._subscription_state[event_type] == 'CHANNEL_OPENED':
             await asyncio.sleep(0.1)
             time_out -= 1
             if time_out <= 0:
                 raise TastytradeError('Subscription channel not opened')
+        # setup the feed
+        await self._channel_setup(event_type)
+
+    async def _channel_setup(self, event_type: EventType) -> None:
+        message = {
+            'type': 'FEED_SETUP',
+            'channel': self._channels[event_type],
+            'acceptAggregationPeriod': 10,
+            'acceptDataFormat': 'COMPACT'
+        }
+
+        def dict_from_schema(event_class: Any):
+            schema = event_class.schema()
+            return {schema['title']: list(schema['properties'].keys())}
+
+        if event_type == EventType.CANDLE:
+            accept = dict_from_schema(Candle)
+        elif event_type == EventType.GREEKS:
+            accept = dict_from_schema(Greeks)
+        elif event_type == EventType.PROFILE:
+            accept = dict_from_schema(Profile)
+        elif event_type == EventType.QUOTE:
+            accept = dict_from_schema(Quote)
+        elif event_type == EventType.SUMMARY:
+            accept = dict_from_schema(Summary)
+        elif event_type == EventType.THEO_PRICE:
+            accept = dict_from_schema(TheoPrice)
+        elif event_type == EventType.TIME_AND_SALE:
+            accept = dict_from_schema(TimeAndSale)
+        elif event_type == EventType.TRADE:
+            accept = dict_from_schema(Trade)
+        elif event_type == EventType.UNDERLYING:
+            accept = dict_from_schema(Underlying)
+        message['acceptEventFields'] = accept
+        # send message
+        logger.debug('setting up feed: %s', message)
+        await self._websocket.send(json.dumps(message))
 
     async def unsubscribe(
         self,
         event_type: EventType,
         symbols: List[str]
     ) -> None:
         """
@@ -910,32 +599,52 @@
     async def _map_message(self, message) -> None:
         """
         Takes the raw JSON data, parses the events and places them into their
         respective queues.
 
         :param message: raw JSON data from the websocket
         """
-        for item in message:
-            msg_type = item.pop('eventType')
-            # parse type or warn for unknown type
-            if msg_type == EventType.CANDLE:
-                await self._queues[EventType.CANDLE].put(Candle(**item))
-            elif msg_type == EventType.GREEKS:
-                await self._queues[EventType.GREEKS].put(Greeks(**item))
-            elif msg_type == EventType.PROFILE:
-                await self._queues[EventType.PROFILE].put(Profile(**item))
-            elif msg_type == EventType.QUOTE:
-                await self._queues[EventType.QUOTE].put(Quote(**item))
-            elif msg_type == EventType.SUMMARY:
-                await self._queues[EventType.SUMMARY].put(Summary(**item))
-            elif msg_type == EventType.THEO_PRICE:
-                await self._queues[EventType.THEO_PRICE].put(TheoPrice(**item))
-            elif msg_type == EventType.TIME_AND_SALE:
-                tas = TimeAndSale(**item)
+        logger.debug('received message: %s', message)
+        if isinstance(message[0], str):
+            msg_type = message[0]
+        else:
+            msg_type = message[0][0]
+        data = message[1]
+        # parse type or warn for unknown type
+        if msg_type == EventType.CANDLE:
+            candles = Candle.from_stream(data)
+            for candle in candles:
+                await self._queues[EventType.CANDLE].put(candle)
+        elif msg_type == EventType.GREEKS:
+            greeks = Greeks.from_stream(data)
+            for greek in greeks:
+                await self._queues[EventType.GREEKS].put(greek)
+        elif msg_type == EventType.PROFILE:
+            profiles = Profile.from_stream(data)
+            for profile in profiles:
+                await self._queues[EventType.PROFILE].put(profile)
+        elif msg_type == EventType.QUOTE:
+            quotes = Quote.from_stream(data)
+            for quote in quotes:
+                await self._queues[EventType.QUOTE].put(quote)
+        elif msg_type == EventType.SUMMARY:
+            summaries = Summary.from_stream(data)
+            for summary in summaries:
+                await self._queues[EventType.SUMMARY].put(summary)
+        elif msg_type == EventType.THEO_PRICE:
+            theo_prices = TheoPrice.from_stream(data)
+            for theo_price in theo_prices:
+                await self._queues[EventType.THEO_PRICE].put(theo_price)
+        elif msg_type == EventType.TIME_AND_SALE:
+            time_and_sales = TimeAndSale.from_stream(data)
+            for tas in time_and_sales:
                 await self._queues[EventType.TIME_AND_SALE].put(tas)
-            elif msg_type == EventType.TRADE:
-                await self._queues[EventType.TRADE].put(Trade(**item))
-            elif msg_type == EventType.UNDERLYING:
-                undl = Underlying(**item)
-                await self._queues[EventType.UNDERLYING].put(undl)
-            else:
-                raise TastytradeError(f'Unknown message type: {message}')
+        elif msg_type == EventType.TRADE:
+            trades = Trade.from_stream(data)
+            for trade in trades:
+                await self._queues[EventType.TRADE].put(trade)
+        elif msg_type == EventType.UNDERLYING:
+            underlyings = Underlying.from_stream(data)
+            for underlying in underlyings:
+                await self._queues[EventType.UNDERLYING].put(underlying)
+        else:
+            raise TastytradeError(f'Unknown message type received: {message}')
```

### Comparing `tastytrade-7.0/tastytrade/utils.py` & `tastytrade-7.1/tastytrade/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,10 +214,13 @@
     """
     if response.status_code // 100 != 2:
         content = response.json()['error']
         error_message = f"{content['code']}: {content['message']}"
         errors = content.get('errors')
         if errors is not None:
             for error in errors:
-                error_message += f"\n{error['code']}: {error['message']}"
+                if "code" in error:
+                    error_message += f"\n{error['code']}: {error['message']}"
+                else:
+                    error_message += f"\n{error['domain']}: {error['reason']}"
 
         raise TastytradeError(error_message)
```

### Comparing `tastytrade-7.0/tastytrade/watchlists.py` & `tastytrade-7.1/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tastytrade.egg-info/PKG-INFO` & `tastytrade-7.1/tastytrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 7.0
+Version: 7.1
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3
 Requires-Dist: websockets>=11.0.3
 Requires-Dist: pydantic>=2.6.3
 Requires-Dist: pandas_market_calendars>=4.3.3
+Requires-Dist: fake_useragent>=1.5.1
 
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
    :alt: PyPI Package
 
 .. image:: https://static.pepy.tech/badge/tastytrade
    :target: https://pepy.tech/project/tastytrade
    :alt: PyPI Downloads
 
+
 Tastytrade Python SDK
 =====================
 
 A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
```

### Comparing `tastytrade-7.0/tastytrade.egg-info/SOURCES.txt` & `tastytrade-7.1/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tests/test_account.py` & `tastytrade-7.1/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tests/test_instruments.py` & `tastytrade-7.1/tests/test_instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tests/test_streamer.py` & `tastytrade-7.1/tests/test_streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tests/test_utils.py` & `tastytrade-7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.0/tests/test_watchlists.py` & `tastytrade-7.1/tests/test_watchlists.py`

 * *Files identical despite different names*

