# Comparing `tmp/openbb_seeking_alpha-1.1.4.tar.gz` & `tmp/openbb_seeking_alpha-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_seeking_alpha-1.1.4.tar", max compression
+gzip compressed data, was "openbb_seeking_alpha-1.1.5.tar", max compression
```

## Comparing `openbb_seeking_alpha-1.1.4.tar` & `openbb_seeking_alpha-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      453 2024-02-29 11:03:36.969524 openbb_seeking_alpha-1.1.4/README.md
--rw-r--r--   0        0        0      512 2024-03-21 17:38:35.655868 openbb_seeking_alpha-1.1.4/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-02-29 11:03:36.969719 openbb_seeking_alpha-1.1.4/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-02-29 11:03:36.969804 openbb_seeking_alpha-1.1.4/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.969831 openbb_seeking_alpha-1.1.4/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-02-29 11:03:36.969907 openbb_seeking_alpha-1.1.4/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      493 2024-04-01 14:20:06.324578 openbb_seeking_alpha-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 openbb_seeking_alpha-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      453 2024-04-17 12:33:20.769645 openbb_seeking_alpha-1.1.5/README.md
+-rw-r--r--   0        0        0      512 2024-04-17 12:33:20.769645 openbb_seeking_alpha-1.1.5/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-17 12:33:20.769645 openbb_seeking_alpha-1.1.5/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-04-17 12:33:20.769645 openbb_seeking_alpha-1.1.5/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.769645 openbb_seeking_alpha-1.1.5/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-04-17 12:33:20.769645 openbb_seeking_alpha-1.1.5/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-19 16:42:43.075446 openbb_seeking_alpha-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 openbb_seeking_alpha-1.1.5/PKG-INFO
```

### Comparing `openbb_seeking_alpha-1.1.4/openbb_seeking_alpha/__init__.py` & `openbb_seeking_alpha-1.1.5/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_seeking_alpha-1.1.4/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_seeking_alpha-1.1.5/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_seeking_alpha-1.1.4/PKG-INFO` & `openbb_seeking_alpha-1.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-seeking-alpha
-Version: 1.1.4
+Version: 1.1.5
 Summary: Seeking Alpha extension for OpenBB
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
 
 # OpenBB Seeking Alpha Provider
 
 This extension integrates the [Seeking Alpha](https://seekingalpha.com) data provider into the OpenBB Platform.
 
 ## Installation
```

