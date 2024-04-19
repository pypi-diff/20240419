# Comparing `tmp/dagster-duckdb-polars-0.23.2rc2.tar.gz` & `tmp/dagster-duckdb-polars-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-polars-0.23.2rc2.tar", last modified: Tue Apr 16 20:35:43 2024, max compression
+gzip compressed data, was "dagster-duckdb-polars-0.23.2rc3.tar", last modified: Thu Apr 18 21:19:22 2024, max compression
```

## Comparing `dagster-duckdb-polars-0.23.2rc2.tar` & `dagster-duckdb-polars-0.23.2rc3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:43.459998 dagster-duckdb-polars-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      675 2024-04-16 20:35:43.459998 dagster-duckdb-polars-0.23.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      149 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:43.459998 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars/
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8910 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars/duckdb_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:43.459998 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      675 2024-04-16 20:35:43.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-04-16 20:35:43.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:35:43.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:35:43.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-16 20:35:43.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-16 20:35:43.000000 dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-16 20:35:43.459998 dagster-duckdb-polars-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1386 2024-04-16 20:26:55.000000 dagster-duckdb-polars-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:19:22.990827 dagster-duckdb-polars-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      675 2024-04-18 21:19:22.990827 dagster-duckdb-polars-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:19:22.986827 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8910 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars/duckdb_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:19:22.990827 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      675 2024-04-18 21:19:22.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-04-18 21:19:22.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:19:22.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:19:22.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-18 21:19:22.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 21:19:22.000000 dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-18 21:19:22.990827 dagster-duckdb-polars-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-04-18 21:10:09.000000 dagster-duckdb-polars-0.23.2rc3/setup.py
```

### Comparing `dagster-duckdb-polars-0.23.2rc2/LICENSE` & `dagster-duckdb-polars-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.23.2rc2/PKG-INFO` & `dagster-duckdb-polars-0.23.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckdb-polars
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars/duckdb_polars_type_handler.py` & `dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars/duckdb_polars_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.23.2rc2/dagster_duckdb_polars.egg-info/PKG-INFO` & `dagster-duckdb-polars-0.23.2rc3/dagster_duckdb_polars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckdb-polars
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-polars-0.23.2rc2/setup.py` & `dagster-duckdb-polars-0.23.2rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_polars_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc2",
-        "dagster-duckdb==0.23.2rc2",
+        "dagster==1.7.2rc3",
+        "dagster-duckdb==0.23.2rc3",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

