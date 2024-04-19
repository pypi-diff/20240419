# Comparing `tmp/dagster-duckdb-0.23.2rc2.tar.gz` & `tmp/dagster-duckdb-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.23.2rc2.tar", last modified: Tue Apr 16 20:39:28 2024, max compression
+gzip compressed data, was "dagster-duckdb-0.23.2rc3.tar", last modified: Thu Apr 18 21:18:27 2024, max compression
```

## Comparing `dagster-duckdb-0.23.2rc2.tar` & `dagster-duckdb-0.23.2rc3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:28.168458 dagster-duckdb-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      681 2024-04-16 20:39:28.168458 dagster-duckdb-0.23.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:28.164458 dagster-duckdb-0.23.2rc2/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12026 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1716 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:28.168458 dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      681 2024-04-16 20:39:27.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-04-16 20:39:27.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:39:27.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:39:27.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2024-04-16 20:39:27.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-16 20:39:27.000000 dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-16 20:39:28.172458 dagster-duckdb-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1548 2024-04-16 20:26:55.000000 dagster-duckdb-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:27.726440 dagster-duckdb-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      681 2024-04-18 21:18:27.726440 dagster-duckdb-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:27.726440 dagster-duckdb-0.23.2rc3/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12026 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:27.726440 dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      681 2024-04-18 21:18:27.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-18 21:18:27.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:18:27.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:18:27.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-18 21:18:27.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-18 21:18:27.000000 dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-18 21:18:27.730440 dagster-duckdb-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-04-18 21:10:09.000000 dagster-duckdb-0.23.2rc3/setup.py
```

### Comparing `dagster-duckdb-0.23.2rc2/LICENSE` & `dagster-duckdb-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.2rc2/PKG-INFO` & `dagster-duckdb-0.23.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.23.2rc2/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.23.2rc3/dagster_duckdb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.2rc2/dagster_duckdb/resource.py` & `dagster-duckdb-0.23.2rc3/dagster_duckdb/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.2rc2/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.23.2rc3/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.23.2rc2/setup.py` & `dagster-duckdb-0.23.2rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "duckdb",
-        "dagster==1.7.2rc2",
+        "dagster==1.7.2rc3",
     ],
     extras_require={
         "pandas": [
             # Pinned pending duckdb removal of broken pandas import. Pin can be
             # removed as soon as it produces a working build.
             "pandas<2.1",
         ],
```

