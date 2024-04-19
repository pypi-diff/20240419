# Comparing `tmp/openbb_commodity-1.0.3.tar.gz` & `tmp/openbb_commodity-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_commodity-1.0.3.tar", max compression
+gzip compressed data, was "openbb_commodity-1.0.4.tar", max compression
```

## Comparing `openbb_commodity-1.0.3.tar` & `openbb_commodity-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      459 2024-04-17 12:33:20.497645 openbb_commodity-1.0.3/README.md
--rw-r--r--   0        0        0       34 2024-04-17 12:33:20.497645 openbb_commodity-1.0.3/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-17 12:33:20.497645 openbb_commodity-1.0.3/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0      470 2024-04-19 16:40:00.579066 openbb_commodity-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_commodity-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      459 2024-04-17 12:33:20.497645 openbb_commodity-1.0.4/README.md
+-rw-r--r--   0        0        0       34 2024-04-17 12:33:20.497645 openbb_commodity-1.0.4/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-17 12:33:20.497645 openbb_commodity-1.0.4/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0      470 2024-04-19 17:04:46.316050 openbb_commodity-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_commodity-1.0.4/PKG-INFO
```

### Comparing `openbb_commodity-1.0.3/openbb_commodity/commodity_router.py` & `openbb_commodity-1.0.4/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_commodity-1.0.3/PKG-INFO` & `openbb_commodity-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-commodity
-Version: 1.0.3
+Version: 1.0.4
 Summary: Commodity extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

