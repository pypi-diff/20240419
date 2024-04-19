# Comparing `tmp/openbb_crypto-1.1.4.tar.gz` & `tmp/openbb_crypto-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_crypto-1.1.4.tar", max compression
+gzip compressed data, was "openbb_crypto-1.1.5.tar", max compression
```

## Comparing `openbb_crypto-1.1.4.tar` & `openbb_crypto-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      457 2024-02-29 11:03:36.729571 openbb_crypto-1.1.4/README.md
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.729885 openbb_crypto-1.1.4/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1010 2024-03-13 16:36:51.556530 openbb_crypto-1.1.4/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.730010 openbb_crypto-1.1.4/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-03-13 16:36:51.557010 openbb_crypto-1.1.4/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.730131 openbb_crypto-1.1.4/openbb_crypto/py.typed
--rw-r--r--   0        0        0      452 2024-04-01 14:17:17.986638 openbb_crypto-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 openbb_crypto-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      457 2024-04-17 12:33:20.497645 openbb_crypto-1.1.5/README.md
+-rw-r--r--   0        0        0       31 2024-04-17 12:33:20.497645 openbb_crypto-1.1.5/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-17 12:33:20.497645 openbb_crypto-1.1.5/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-04-17 12:33:20.497645 openbb_crypto-1.1.5/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-17 12:33:20.497645 openbb_crypto-1.1.5/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.497645 openbb_crypto-1.1.5/openbb_crypto/py.typed
+-rw-r--r--   0        0        0      452 2024-04-19 16:40:20.391107 openbb_crypto-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 openbb_crypto-1.1.5/PKG-INFO
```

### Comparing `openbb_crypto-1.1.4/openbb_crypto/crypto_router.py` & `openbb_crypto-1.1.5/openbb_crypto/crypto_router.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     StandardParams,
 )
 from openbb_core.app.query import Query
 from openbb_core.app.router import Router
 
 from openbb_crypto.price.price_router import router as price_router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Cryptocurrency market data.")
 router.include_router(price_router)
 
 
 # pylint: disable=unused-argument
 @router.command(
     model="CryptoSearch",
     examples=[
```

### Comparing `openbb_crypto-1.1.4/openbb_crypto/price/price_router.py` & `openbb_crypto-1.1.5/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_crypto-1.1.4/PKG-INFO` & `openbb_crypto-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-crypto
-Version: 1.1.4
+Version: 1.1.5
 Summary: Crypto extension for OpenBB
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
 
 # Crypto data extension for OpenBB Platform
 
 This extension provides a set of commands for crypto data retrieval.
 
 ## Installation
```

