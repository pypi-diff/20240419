# Comparing `tmp/openbb_derivatives-1.1.4.tar.gz` & `tmp/openbb_derivatives-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_derivatives-1.1.4.tar", max compression
+gzip compressed data, was "openbb_derivatives-1.1.5.tar", max compression
```

## Comparing `openbb_derivatives-1.1.4.tar` & `openbb_derivatives-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      441 2024-02-29 11:03:36.731500 openbb_derivatives-1.1.4/README.md
--rw-r--r--   0        0        0       15 2024-02-29 11:03:36.731747 openbb_derivatives-1.1.4/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      332 2024-02-29 11:03:36.731808 openbb_derivatives-1.1.4/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-02-29 11:03:36.731881 openbb_derivatives-1.1.4/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-03-13 16:36:51.560749 openbb_derivatives-1.1.4/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-02-29 11:03:36.732008 openbb_derivatives-1.1.4/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-03-13 16:36:51.561090 openbb_derivatives-1.1.4/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0      482 2024-04-01 14:18:22.785148 openbb_derivatives-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 openbb_derivatives-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      441 2024-04-17 12:33:20.497645 openbb_derivatives-1.1.5/README.md
+-rw-r--r--   0        0        0       15 2024-04-17 12:33:20.497645 openbb_derivatives-1.1.5/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-17 12:33:20.497645 openbb_derivatives-1.1.5/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-04-17 12:33:20.497645 openbb_derivatives-1.1.5/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-17 12:33:20.497645 openbb_derivatives-1.1.5/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-04-17 12:33:20.497645 openbb_derivatives-1.1.5/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-04-17 12:33:20.497645 openbb_derivatives-1.1.5/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0      482 2024-04-19 16:40:45.967163 openbb_derivatives-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 openbb_derivatives-1.1.5/PKG-INFO
```

### Comparing `openbb_derivatives-1.1.4/openbb_derivatives/futures/futures_router.py` & `openbb_derivatives-1.1.5/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_derivatives-1.1.4/openbb_derivatives/options/options_router.py` & `openbb_derivatives-1.1.5/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_derivatives-1.1.4/PKG-INFO` & `openbb_derivatives-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-derivatives
-Version: 1.1.4
+Version: 1.1.5
 Summary: Derivatives extension for OpenBB
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
 
 # OpenBB Derivatives Extension
 
 This extension provides derivatives data for the OpenBB Platform.
 
 ## Installation
```

