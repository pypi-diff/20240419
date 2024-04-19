# Comparing `tmp/dagster-deltalake-0.23.2rc2.tar.gz` & `tmp/dagster-deltalake-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-deltalake-0.23.2rc2.tar", last modified: Tue Apr 16 20:37:15 2024, max compression
+gzip compressed data, was "dagster-deltalake-0.23.2rc3.tar", last modified: Thu Apr 18 21:18:32 2024, max compression
```

## Comparing `dagster-deltalake-0.23.2rc2.tar` & `dagster-deltalake-0.23.2rc3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:15.764179 dagster-deltalake-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11344 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      710 2024-04-16 20:37:15.764179 dagster-deltalake-0.23.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:15.764179 dagster-deltalake-0.23.2rc2/dagster_deltalake/
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6650 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake/config.py
--rw-r--r--   0 root         (0) root         (0)     9940 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake/handler.py
--rw-r--r--   0 root         (0) root         (0)     9439 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake/py.typed
--rw-r--r--   0 root         (0) root         (0)     1694 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake/resource.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:37:15.764179 dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/
--rw-r--r--   0 root         (0) root         (0)      710 2024-04-16 20:37:15.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-16 20:37:15.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:37:15.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:37:15.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-16 20:37:15.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-16 20:37:15.000000 dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      128 2024-04-16 20:37:15.768179 dagster-deltalake-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1411 2024-04-16 20:26:55.000000 dagster-deltalake-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:32.186471 dagster-deltalake-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      710 2024-04-18 21:18:32.186471 dagster-deltalake-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:32.186471 dagster-deltalake-0.23.2rc3/dagster_deltalake/
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6650 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake/config.py
+-rw-r--r--   0 root         (0) root         (0)     9940 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake/handler.py
+-rw-r--r--   0 root         (0) root         (0)     9435 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1694 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake/resource.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:32.186471 dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      710 2024-04-18 21:18:31.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-18 21:18:32.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:18:31.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:18:31.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-18 21:18:31.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-18 21:18:31.000000 dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-18 21:18:32.186471 dagster-deltalake-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-18 21:10:09.000000 dagster-deltalake-0.23.2rc3/setup.py
```

### Comparing `dagster-deltalake-0.23.2rc2/LICENSE` & `dagster-deltalake-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.2rc2/PKG-INFO` & `dagster-deltalake-0.23.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for Deltalake-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-0.23.2rc2/dagster_deltalake/__init__.py` & `dagster-deltalake-0.23.2rc3/dagster_deltalake/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.2rc2/dagster_deltalake/config.py` & `dagster-deltalake-0.23.2rc3/dagster_deltalake/config.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.2rc2/dagster_deltalake/handler.py` & `dagster-deltalake-0.23.2rc3/dagster_deltalake/handler.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.2rc2/dagster_deltalake/io_manager.py` & `dagster-deltalake-0.23.2rc3/dagster_deltalake/io_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         # schemas are just folders and automatically created on write.
         pass
 
     @staticmethod
     def get_select_statement(table_slice: TableSlice) -> str:
         # The select statement here is just for illustrative purposes,
         # and is never actually executed. It does however logically correspond
-        # the the operation being executed.
+        # the operation being executed.
         col_str = ", ".join(table_slice.columns) if table_slice.columns else "*"
 
         if table_slice.partition_dimensions and len(table_slice.partition_dimensions) > 0:
             query = f"SELECT {col_str} FROM {table_slice.schema}.{table_slice.table} WHERE\n"
             return query + _partition_where_clause(table_slice.partition_dimensions)
         else:
             return f"""SELECT {col_str} FROM {table_slice.schema}.{table_slice.table}"""
```

### Comparing `dagster-deltalake-0.23.2rc2/dagster_deltalake/resource.py` & `dagster-deltalake-0.23.2rc3/dagster_deltalake/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.2rc2/dagster_deltalake.egg-info/PKG-INFO` & `dagster-deltalake-0.23.2rc3/dagster_deltalake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for Deltalake-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-0.23.2rc2/setup.py` & `dagster-deltalake-0.23.2rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_deltalake_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "deltalake>=0.15",
-        "dagster==1.7.2rc2",
+        "dagster==1.7.2rc3",
     ],
     extras_require={
         "pandas": ["pandas"],
     },
     zip_safe=False,
 )
```
