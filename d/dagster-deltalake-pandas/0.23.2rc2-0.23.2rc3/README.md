# Comparing `tmp/dagster-deltalake-pandas-0.23.2rc2.tar.gz` & `tmp/dagster-deltalake-pandas-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-deltalake-pandas-0.23.2rc2.tar", last modified: Tue Apr 16 20:36:27 2024, max compression
+gzip compressed data, was "dagster-deltalake-pandas-0.23.2rc3.tar", last modified: Thu Apr 18 21:16:16 2024, max compression
```

## Comparing `dagster-deltalake-pandas-0.23.2rc2.tar` & `dagster-deltalake-pandas-0.23.2rc3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:36:27.896080 dagster-deltalake-pandas-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11344 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      781 2024-04-16 20:36:27.896080 dagster-deltalake-pandas-0.23.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      151 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:36:27.896080 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas/
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas/deltalake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:36:27.896080 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      781 2024-04-16 20:36:27.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-16 20:36:27.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:36:27.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:36:27.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-16 20:36:27.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:36:27.000000 dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      135 2024-04-16 20:36:27.896080 dagster-deltalake-pandas-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1490 2024-04-16 20:26:55.000000 dagster-deltalake-pandas-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:16.029520 dagster-deltalake-pandas-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      781 2024-04-18 21:16:16.029520 dagster-deltalake-pandas-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:16.025520 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas/deltalake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:16.025520 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      781 2024-04-18 21:16:15.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-18 21:16:15.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:16:15.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:16:15.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-18 21:16:15.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 21:16:15.000000 dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2024-04-18 21:16:16.029520 dagster-deltalake-pandas-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-04-18 21:10:09.000000 dagster-deltalake-pandas-0.23.2rc3/setup.py
```

### Comparing `dagster-deltalake-pandas-0.23.2rc2/LICENSE` & `dagster-deltalake-pandas-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-pandas-0.23.2rc2/PKG-INFO` & `dagster-deltalake-pandas-0.23.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-pandas
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for storing Pandas DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas/deltalake_pandas_type_handler.py` & `dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas/deltalake_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-pandas-0.23.2rc2/dagster_deltalake_pandas.egg-info/PKG-INFO` & `dagster-deltalake-pandas-0.23.2rc3/dagster_deltalake_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-pandas
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for storing Pandas DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-pandas-0.23.2rc2/setup.py` & `dagster-deltalake-pandas-0.23.2rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_deltalake_pandas_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc2",
-        "dagster-deltalake==0.23.2rc2",
+        "dagster==1.7.2rc3",
+        "dagster-deltalake==0.23.2rc3",
         "pandas",
     ],
     zip_safe=False,
 )
```

