# Comparing `tmp/referrers-0.3.2.tar.gz` & `tmp/referrers-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.3.2.tar", max compression
+gzip compressed data, was "referrers-0.3.3.tar", max compression
```

## Comparing `referrers-0.3.2.tar` & `referrers-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-08 21:18:50.216968 referrers-0.3.2/LICENSE
--rw-r--r--   0        0        0     6887 2024-04-08 21:18:50.216968 referrers-0.3.2/README.md
--rw-r--r--   0        0        0      372 2024-04-08 21:18:50.216968 referrers-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-08 21:18:50.216968 referrers-0.3.2/src/referrers/__init__.py
--rw-r--r--   0        0        0    37144 2024-04-08 21:18:50.216968 referrers-0.3.2/src/referrers/impl.py
--rw-r--r--   0        0        0     7420 1970-01-01 00:00:00.000000 referrers-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 17:05:14.757568 referrers-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6887 2024-04-19 17:05:14.757568 referrers-0.3.3/README.md
+-rw-r--r--   0        0        0      372 2024-04-19 17:05:14.761568 referrers-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-19 17:05:14.761568 referrers-0.3.3/src/referrers/__init__.py
+-rw-r--r--   0        0        0    37144 2024-04-19 17:05:14.761568 referrers-0.3.3/src/referrers/impl.py
+-rw-r--r--   0        0        0     7420 1970-01-01 00:00:00.000000 referrers-0.3.3/PKG-INFO
```

### Comparing `referrers-0.3.2/LICENSE` & `referrers-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.3.2/README.md` & `referrers-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `referrers-0.3.2/src/referrers/impl.py` & `referrers-0.3.3/src/referrers/impl.py`

 * *Files identical despite different names*

### Comparing `referrers-0.3.2/PKG-INFO` & `referrers-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: referrers
-Version: 0.3.2
+Version: 0.3.3
 Summary: Finds the graph of referrers for a Python object
 Author: Neil Ferguson
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

