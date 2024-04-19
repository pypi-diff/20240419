# Comparing `tmp/botocore-a-la-carte-cloudsearch-1.34.86.tar.gz` & `tmp/botocore-a-la-carte-cloudsearch-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-cloudsearch-1.34.86.tar", last modified: Thu Apr 18 01:00:11 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-cloudsearch-1.34.9.tar", last modified: Thu Dec 28 01:06:37 2023, max compression
```

## Comparing `botocore-a-la-carte-cloudsearch-1.34.86.tar` & `botocore-a-la-carte-cloudsearch-1.34.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:11.607215 botocore-a-la-carte-cloudsearch-1.34.86/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-18 01:00:11.000000 botocore-a-la-carte-cloudsearch-1.34.86/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-18 01:00:11.607215 botocore-a-la-carte-cloudsearch-1.34.86/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:11.603215 botocore-a-la-carte-cloudsearch-1.34.86/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:11.603215 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:11.603215 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:11.603215 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2011-02-01/
--rw-r--r--   0 runner    (1001) docker     (127)    13150 2024-04-18 01:00:01.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2011-02-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    84791 2024-04-18 01:00:01.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2011-02-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:11.603215 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2013-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-18 01:00:01.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2013-01-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 01:00:01.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2013-01-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 01:00:01.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2013-01-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    96766 2024-04-18 01:00:01.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2013-01-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:11.607215 botocore-a-la-carte-cloudsearch-1.34.86/botocore_a_la_carte_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-18 01:00:11.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore_a_la_carte_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 01:00:11.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore_a_la_carte_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:00:11.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore_a_la_carte_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 01:00:11.000000 botocore-a-la-carte-cloudsearch-1.34.86/botocore_a_la_carte_cloudsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:00:11.607215 botocore-a-la-carte-cloudsearch-1.34.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 01:00:11.000000 botocore-a-la-carte-cloudsearch-1.34.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.974250 botocore-a-la-carte-cloudsearch-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:37.000000 botocore-a-la-carte-cloudsearch-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:37.974250 botocore-a-la-carte-cloudsearch-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.970250 botocore-a-la-carte-cloudsearch-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.970250 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.970250 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.970250 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2011-02-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    13150 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2011-02-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84791 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2011-02-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.974250 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2013-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2013-01-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2013-01-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2013-01-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    96766 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2013-01-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.974250 botocore-a-la-carte-cloudsearch-1.34.9/botocore_a_la_carte_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:37.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore_a_la_carte_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-12-28 01:06:37.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore_a_la_carte_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:37.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore_a_la_carte_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:37.000000 botocore-a-la-carte-cloudsearch-1.34.9/botocore_a_la_carte_cloudsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:37.974250 botocore-a-la-carte-cloudsearch-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-28 01:06:37.000000 botocore-a-la-carte-cloudsearch-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/LICENSE.txt` & `botocore-a-la-carte-cloudsearch-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/PKG-INFO` & `botocore-a-la-carte-cloudsearch-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloudsearch
-Version: 1.34.86
+Version: 1.34.9
 Summary: cloudsearch data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2011-02-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2011-02-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2011-02-01/service-2.json` & `botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2011-02-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2013-01-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2013-01-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/botocore/data/cloudsearch/2013-01-01/service-2.json` & `botocore-a-la-carte-cloudsearch-1.34.9/botocore/data/cloudsearch/2013-01-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/botocore_a_la_carte_cloudsearch.egg-info/PKG-INFO` & `botocore-a-la-carte-cloudsearch-1.34.9/botocore_a_la_carte_cloudsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloudsearch
-Version: 1.34.86
+Version: 1.34.9
 Summary: cloudsearch data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/botocore_a_la_carte_cloudsearch.egg-info/SOURCES.txt` & `botocore-a-la-carte-cloudsearch-1.34.9/botocore_a_la_carte_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudsearch-1.34.86/setup.py` & `botocore-a-la-carte-cloudsearch-1.34.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-cloudsearch',
-    version="1.34.86",
+    version="1.34.9",
     description='cloudsearch data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/cloudsearch/*/*.json'],
```

