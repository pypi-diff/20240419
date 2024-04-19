# Comparing `tmp/ziptimezone-0.1.8.tar.gz` & `tmp/ziptimezone-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.1.8.tar", max compression
+gzip compressed data, was "ziptimezone-0.1.9.tar", max compression
```

## Comparing `ziptimezone-0.1.8.tar` & `ziptimezone-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.1.8/LICENSE
--rw-r--r--   0        0        0      298 2024-04-18 20:05:12.524095 ziptimezone-0.1.8/README.md
--rw-r--r--   0        0        0      488 2024-04-18 22:04:28.546659 ziptimezone-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.1.8/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-18 17:39:45.000000 ziptimezone-0.1.8/ziptimezone/core.py
--rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.1.8/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.1.8/ziptimezone/mappings.py
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 ziptimezone-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.1.9/LICENSE
+-rw-r--r--   0        0        0      298 2024-04-18 20:05:12.524095 ziptimezone-0.1.9/README.md
+-rw-r--r--   0        0        0      487 2024-04-19 20:45:28.404390 ziptimezone-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.1.9/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-19 15:38:14.654911 ziptimezone-0.1.9/ziptimezone/core copy.py
+-rw-r--r--   0        0        0     3056 2024-04-19 20:45:15.084480 ziptimezone-0.1.9/ziptimezone/core.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:41:48.857464 ziptimezone-0.1.9/ziptimezone/data/.gitkeep
+-rw-r--r--   0        0        0     2697 2024-04-19 15:57:50.850984 ziptimezone-0.1.9/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.1.9/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.1.9/ziptimezone/mappings.py
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 ziptimezone-0.1.9/PKG-INFO
```

### Comparing `ziptimezone-0.1.8/ziptimezone/__init__.py` & `ziptimezone-0.1.9/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.8/ziptimezone/core.py` & `ziptimezone-0.1.9/ziptimezone/core copy.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.8/ziptimezone/geocode.py` & `ziptimezone-0.1.9/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.8/ziptimezone/mappings.py` & `ziptimezone-0.1.9/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.8/PKG-INFO` & `ziptimezone-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

