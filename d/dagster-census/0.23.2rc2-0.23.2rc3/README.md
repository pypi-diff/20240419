# Comparing `tmp/dagster-census-0.23.2rc2.tar.gz` & `tmp/dagster-census-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-census-0.23.2rc2.tar", last modified: Tue Apr 16 20:36:47 2024, max compression
+gzip compressed data, was "dagster-census-0.23.2rc3.tar", last modified: Thu Apr 18 21:17:11 2024, max compression
```

## Comparing `dagster-census-0.23.2rc2.tar` & `dagster-census-0.23.2rc3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:36:47.872122 dagster-census-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      708 2024-04-16 20:36:47.872122 dagster-census-0.23.2rc2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:36:47.872122 dagster-census-0.23.2rc2/dagster_census/
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/dagster_census/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3551 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/dagster_census/ops.py
--rw-r--r--   0 root         (0) root         (0)    10798 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/dagster_census/resources.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/dagster_census/types.py
--rw-r--r--   0 root         (0) root         (0)     1325 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/dagster_census/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/dagster_census/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:36:47.872122 dagster-census-0.23.2rc2/dagster_census.egg-info/
--rw-r--r--   0 root         (0) root         (0)      708 2024-04-16 20:36:47.000000 dagster-census-0.23.2rc2/dagster_census.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2024-04-16 20:36:47.000000 dagster-census-0.23.2rc2/dagster_census.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:36:47.000000 dagster-census-0.23.2rc2/dagster_census.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:36:47.000000 dagster-census-0.23.2rc2/dagster_census.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-16 20:36:47.000000 dagster-census-0.23.2rc2/dagster_census.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-16 20:36:47.000000 dagster-census-0.23.2rc2/dagster_census.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-16 20:36:47.876122 dagster-census-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1294 2024-04-16 20:26:55.000000 dagster-census-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:17:11.777908 dagster-census-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      708 2024-04-18 21:17:11.777908 dagster-census-0.23.2rc3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:17:11.773908 dagster-census-0.23.2rc3/dagster_census/
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/dagster_census/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/dagster_census/ops.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/dagster_census/resources.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/dagster_census/types.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/dagster_census/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/dagster_census/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:17:11.777908 dagster-census-0.23.2rc3/dagster_census.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      708 2024-04-18 21:17:11.000000 dagster-census-0.23.2rc3/dagster_census.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2024-04-18 21:17:11.000000 dagster-census-0.23.2rc3/dagster_census.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:17:11.000000 dagster-census-0.23.2rc3/dagster_census.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:17:11.000000 dagster-census-0.23.2rc3/dagster_census.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-18 21:17:11.000000 dagster-census-0.23.2rc3/dagster_census.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-18 21:17:11.000000 dagster-census-0.23.2rc3/dagster_census.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-18 21:17:11.777908 dagster-census-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-04-18 21:10:09.000000 dagster-census-0.23.2rc3/setup.py
```

### Comparing `dagster-census-0.23.2rc2/LICENSE` & `dagster-census-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.2rc2/PKG-INFO` & `dagster-census-0.23.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.23.2rc2/dagster_census/ops.py` & `dagster-census-0.23.2rc3/dagster_census/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.2rc2/dagster_census/resources.py` & `dagster-census-0.23.2rc3/dagster_census/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.2rc2/dagster_census/types.py` & `dagster-census-0.23.2rc3/dagster_census/types.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.2rc2/dagster_census/utils.py` & `dagster-census-0.23.2rc3/dagster_census/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.2rc2/dagster_census.egg-info/PKG-INFO` & `dagster-census-0.23.2rc3/dagster_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.23.2rc2/setup.py` & `dagster-census-0.23.2rc3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_census_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.2rc2"],
+    install_requires=["dagster==1.7.2rc3"],
     zip_safe=False,
 )
```

