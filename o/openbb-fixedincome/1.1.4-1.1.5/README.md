# Comparing `tmp/openbb_fixedincome-1.1.4.tar.gz` & `tmp/openbb_fixedincome-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fixedincome-1.1.4.tar", max compression
+gzip compressed data, was "openbb_fixedincome-1.1.5.tar", max compression
```

## Comparing `openbb_fixedincome-1.1.4.tar` & `openbb_fixedincome-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      552 2024-02-29 11:03:36.738371 openbb_fixedincome-1.1.4/README.md
--rw-r--r--   0        0        0       32 2024-02-29 11:03:36.738645 openbb_fixedincome-1.1.4/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-02-29 11:03:36.738725 openbb_fixedincome-1.1.4/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-03-13 16:36:51.574325 openbb_fixedincome-1.1.4/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1541 2024-03-13 16:36:51.574749 openbb_fixedincome-1.1.4/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-02-29 11:03:36.738953 openbb_fixedincome-1.1.4/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-03-13 16:36:51.575058 openbb_fixedincome-1.1.4/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.739091 openbb_fixedincome-1.1.4/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-02-29 11:03:36.739181 openbb_fixedincome-1.1.4/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-03-13 16:36:51.575541 openbb_fixedincome-1.1.4/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-02-29 11:03:36.739375 openbb_fixedincome-1.1.4/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-03-13 16:36:51.575981 openbb_fixedincome-1.1.4/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0      483 2024-04-01 14:18:50.061603 openbb_fixedincome-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 openbb_fixedincome-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      552 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/README.md
+-rw-r--r--   0        0        0       32 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0      483 2024-04-19 16:39:15.718977 openbb_fixedincome-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 openbb_fixedincome-1.1.5/PKG-INFO
```

### Comparing `openbb_fixedincome-1.1.4/README.md` & `openbb_fixedincome-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.4/openbb_fixedincome/corporate/corporate_router.py` & `openbb_fixedincome-1.1.5/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.4/openbb_fixedincome/fixedincome_router.py` & `openbb_fixedincome-1.1.5/openbb_fixedincome/fixedincome_router.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_core.app.router import Router
 
 from openbb_fixedincome.corporate.corporate_router import router as corporate_router
 from openbb_fixedincome.government.government_router import router as government_router
 from openbb_fixedincome.rate.rate_router import router as rate_router
 from openbb_fixedincome.spreads.spreads_router import router as spreads_router
 
-router = Router(prefix="")
+router = Router(prefix="", description="Fixed Income market data.")
 router.include_router(rate_router)
 router.include_router(spreads_router)
 router.include_router(government_router)
 router.include_router(corporate_router)
 
 
 @router.command(
```

### Comparing `openbb_fixedincome-1.1.4/openbb_fixedincome/government/government_router.py` & `openbb_fixedincome-1.1.5/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.4/openbb_fixedincome/rate/rate_router.py` & `openbb_fixedincome-1.1.5/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.4/openbb_fixedincome/spreads/spreads_router.py` & `openbb_fixedincome-1.1.5/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.4/PKG-INFO` & `openbb_fixedincome-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-fixedincome
-Version: 1.1.4
+Version: 1.1.5
 Summary: Fixed income extension for OpenBB
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
 
 # OpenBB Fixed Income Extension
 
 This extension provides fixed income data for the OpenBB Platform.
 
 Features of the Fixed Income extension include information on government bonds and central bank rates.
```

