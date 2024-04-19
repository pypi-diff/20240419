# Comparing `tmp/openbb_wsj-1.1.4.tar.gz` & `tmp/openbb_wsj-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_wsj-1.1.4.tar", max compression
+gzip compressed data, was "openbb_wsj-1.1.5.tar", max compression
```

## Comparing `openbb_wsj-1.1.4.tar` & `openbb_wsj-1.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      427 2024-02-29 11:03:36.977654 openbb_wsj-1.1.4/README.md
--rw-r--r--   0        0        0     1044 2024-03-21 17:38:35.661411 openbb_wsj-1.1.4/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-02-29 11:03:36.977934 openbb_wsj-1.1.4/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-03-13 16:36:51.899375 openbb_wsj-1.1.4/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-03-13 16:36:51.899461 openbb_wsj-1.1.4/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0      433 2024-04-01 14:19:50.212823 openbb_wsj-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 openbb_wsj-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      427 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/README.md
+-rw-r--r--   0        0        0     1044 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0      433 2024-04-19 16:42:48.787460 openbb_wsj-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 openbb_wsj-1.1.5/PKG-INFO
```

### Comparing `openbb_wsj-1.1.4/openbb_wsj/__init__.py` & `openbb_wsj-1.1.5/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.1.4/openbb_wsj/models/active.py` & `openbb_wsj-1.1.5/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.1.4/openbb_wsj/models/gainers.py` & `openbb_wsj-1.1.5/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.1.4/openbb_wsj/models/losers.py` & `openbb_wsj-1.1.5/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.1.4/PKG-INFO` & `openbb_wsj-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-wsj
-Version: 1.1.4
+Version: 1.1.5
 Summary: wsj extension for OpenBB
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
 
 # OpenBB Wall St Journal Provider
 
 This extension integrates the [WSJ](https://wsj.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

