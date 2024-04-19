# Comparing `tmp/openbb_finviz-1.0.3.tar.gz` & `tmp/openbb_finviz-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_finviz-1.0.3.tar", max compression
+gzip compressed data, was "openbb_finviz-1.0.4.tar", max compression
```

## Comparing `openbb_finviz-1.0.3.tar` & `openbb_finviz-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      442 2024-03-13 16:36:51.709028 openbb_finviz-1.0.3/README.md
--rw-r--r--   0        0        0     1005 2024-03-21 17:38:35.639348 openbb_finviz-1.0.3/openbb_finviz/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709375 openbb_finviz-1.0.3/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9574 2024-03-21 17:38:35.639523 openbb_finviz-1.0.3/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-03-13 16:36:51.709567 openbb_finviz-1.0.3/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-03-13 16:36:51.709649 openbb_finviz-1.0.3/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-03-18 09:35:41.452443 openbb_finviz-1.0.3/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-03-13 16:36:51.709793 openbb_finviz-1.0.3/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709818 openbb_finviz-1.0.3/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709850 openbb_finviz-1.0.3/openbb_finviz/py.typed
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709895 openbb_finviz-1.0.3/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-03-13 16:36:51.709953 openbb_finviz-1.0.3/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709976 openbb_finviz-1.0.3/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0      477 2024-04-01 14:19:38.514072 openbb_finviz-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 openbb_finviz-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      442 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/README.md
+-rw-r--r--   0        0        0     1005 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9573 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0      477 2024-04-19 16:41:30.451265 openbb_finviz-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 openbb_finviz-1.0.4/PKG-INFO
```

### Comparing `openbb_finviz-1.0.3/openbb_finviz/__init__.py` & `openbb_finviz-1.0.4/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.3/openbb_finviz/models/compare_groups.py` & `openbb_finviz-1.0.4/openbb_finviz/models/compare_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         if v is not None and "%" in str(v):
             return float(v.replace("%", "")) / 100
         return v if v else None
 
     @field_validator("market_cap", "volume", mode="before", check_fields=False)
     @classmethod
     def validate_abbreviated_numbers(cls, v):
-        """Checks for abbreviated string values."""
+        """Check for abbreviated string values."""
         if v is not None and isinstance(v, str):
             v = (
                 v.replace("M", "e+6")
                 .replace("B", "e+9")
                 .replace("T", "e+12")
                 .replace("K", "e+3")
             )
```

### Comparing `openbb_finviz-1.0.3/openbb_finviz/models/equity_profile.py` & `openbb_finviz-1.0.4/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.3/openbb_finviz/models/key_metrics.py` & `openbb_finviz-1.0.4/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.3/openbb_finviz/models/price_performance.py` & `openbb_finviz-1.0.4/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.3/openbb_finviz/models/price_target.py` & `openbb_finviz-1.0.4/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.3/openbb_finviz/utils/definitions.py` & `openbb_finviz-1.0.4/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.3/PKG-INFO` & `openbb_finviz-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-finviz
-Version: 1.0.3
+Version: 1.0.4
 Summary: Finviz extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: finvizfinance (==0.14.7)
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Finviz Data Provider Extension
 
 This extension integrates the [Finviz](https://finviz.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

