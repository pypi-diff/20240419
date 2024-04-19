# Comparing `tmp/dagster-pandera-0.23.2rc2.tar.gz` & `tmp/dagster-pandera-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pandera-0.23.2rc2.tar", last modified: Tue Apr 16 20:35:14 2024, max compression
+gzip compressed data, was "dagster-pandera-0.23.2rc3.tar", last modified: Thu Apr 18 21:18:22 2024, max compression
```

## Comparing `dagster-pandera-0.23.2rc2.tar` & `dagster-pandera-0.23.2rc3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:14.611936 dagster-pandera-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-pandera-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-16 20:26:55.000000 dagster-pandera-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      676 2024-04-16 20:35:14.611936 dagster-pandera-0.23.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-04-16 20:26:55.000000 dagster-pandera-0.23.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:14.611936 dagster-pandera-0.23.2rc2/dagster_pandera/
--rw-r--r--   0 root         (0) root         (0)     9259 2024-04-16 20:26:55.000000 dagster-pandera-0.23.2rc2/dagster_pandera/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:26:55.000000 dagster-pandera-0.23.2rc2/dagster_pandera/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-pandera-0.23.2rc2/dagster_pandera/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:14.611936 dagster-pandera-0.23.2rc2/dagster_pandera.egg-info/
--rw-r--r--   0 root         (0) root         (0)      676 2024-04-16 20:35:14.000000 dagster-pandera-0.23.2rc2/dagster_pandera.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2024-04-16 20:35:14.000000 dagster-pandera-0.23.2rc2/dagster_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:35:14.000000 dagster-pandera-0.23.2rc2/dagster_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-16 20:35:14.000000 dagster-pandera-0.23.2rc2/dagster_pandera.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 20:35:14.000000 dagster-pandera-0.23.2rc2/dagster_pandera.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      150 2024-04-16 20:35:14.615936 dagster-pandera-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1362 2024-04-16 20:26:55.000000 dagster-pandera-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:22.350402 dagster-pandera-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-pandera-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-18 21:10:09.000000 dagster-pandera-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-18 21:18:22.350402 dagster-pandera-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-18 21:10:09.000000 dagster-pandera-0.23.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:22.346402 dagster-pandera-0.23.2rc3/dagster_pandera/
+-rw-r--r--   0 root         (0) root         (0)     9259 2024-04-18 21:10:09.000000 dagster-pandera-0.23.2rc3/dagster_pandera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 21:10:09.000000 dagster-pandera-0.23.2rc3/dagster_pandera/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-pandera-0.23.2rc3/dagster_pandera/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:18:22.350402 dagster-pandera-0.23.2rc3/dagster_pandera.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-18 21:18:22.000000 dagster-pandera-0.23.2rc3/dagster_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      322 2024-04-18 21:18:22.000000 dagster-pandera-0.23.2rc3/dagster_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:18:22.000000 dagster-pandera-0.23.2rc3/dagster_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-18 21:18:22.000000 dagster-pandera-0.23.2rc3/dagster_pandera.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-18 21:18:22.000000 dagster-pandera-0.23.2rc3/dagster_pandera.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-18 21:18:22.350402 dagster-pandera-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-18 21:10:09.000000 dagster-pandera-0.23.2rc3/setup.py
```

### Comparing `dagster-pandera-0.23.2rc2/LICENSE` & `dagster-pandera-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.23.2rc2/PKG-INFO` & `dagster-pandera-0.23.2rc3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pandera-0.23.2rc2/dagster_pandera/__init__.py` & `dagster-pandera-0.23.2rc3/dagster_pandera/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.23.2rc2/dagster_pandera.egg-info/PKG-INFO` & `dagster-pandera-0.23.2rc3/dagster_pandera.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pandera-0.23.2rc2/setup.py` & `dagster-pandera-0.23.2rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_pandera_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.2rc2", "pandas", "pandera>=0.14.2"],
+    install_requires=["dagster==1.7.2rc3", "pandas", "pandera>=0.14.2"],
     extras_require={
         "test": [
             "pytest",
         ],
     },
 )
```

