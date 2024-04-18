# Comparing `tmp/ziptimezone-0.1.6.tar.gz` & `tmp/ziptimezone-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.1.6.tar", max compression
+gzip compressed data, was "ziptimezone-0.1.7.tar", max compression
```

## Comparing `ziptimezone-0.1.6.tar` & `ziptimezone-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.1.6/LICENSE
--rw-r--r--   0        0        0      298 2024-04-18 20:05:12.524095 ziptimezone-0.1.6/README.md
--rw-r--r--   0        0        0      488 2024-04-18 21:42:14.955130 ziptimezone-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.1.6/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-18 17:39:45.000000 ziptimezone-0.1.6/ziptimezone/core.py
--rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.1.6/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.1.6/ziptimezone/mappings.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 ziptimezone-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.1.7/LICENSE
+-rw-r--r--   0        0        0      298 2024-04-18 20:05:12.524095 ziptimezone-0.1.7/README.md
+-rw-r--r--   0        0        0      487 2024-04-18 21:44:17.870357 ziptimezone-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.1.7/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-18 17:39:45.000000 ziptimezone-0.1.7/ziptimezone/core.py
+-rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.1.7/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.1.7/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 ziptimezone-0.1.7/PKG-INFO
```

### Comparing `ziptimezone-0.1.6/ziptimezone/__init__.py` & `ziptimezone-0.1.7/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.6/ziptimezone/core.py` & `ziptimezone-0.1.7/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.6/ziptimezone/geocode.py` & `ziptimezone-0.1.7/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.6/ziptimezone/mappings.py` & `ziptimezone-0.1.7/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.6/PKG-INFO` & `ziptimezone-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pgeocode (>=0.4.0,<0.5.0)
-Requires-Dist: timezonefinder (>=6.1.0,<7.0.0)
+Requires-Dist: timezonefinder (==5.2.0)
 Description-Content-Type: text/markdown
 
 ### This is basically a simple wrapper around pgeocode and timezonefinder packages.
 ### Convenience functions to get:
 ### 1. The latitude and longitude for a given US or Puerto Rico Zip Code
 ### 2. The more commonly identifiable timezone for a given zipcode(ex: Eastern, Central, Mountain, et al)
```

