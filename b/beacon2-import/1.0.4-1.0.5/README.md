# Comparing `tmp/beacon2_import-1.0.4.tar.gz` & `tmp/beacon2-import-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beacon2_import-1.0.4.tar", last modified: Wed Apr 17 10:31:08 2024, max compression
+gzip compressed data, was "beacon2-import-1.0.5.tar", last modified: Fri Apr 19 11:34:09 2024, max compression
```

## Comparing `beacon2_import-1.0.4.tar` & `beacon2-import-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-17 10:31:08.126745 beacon2_import-1.0.4/
--rw-r--r--   0 khaled    (1000) khaled    (1000)      379 2024-04-17 10:31:08.126745 beacon2_import-1.0.4/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2_import-1.0.4/README.md
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-17 10:31:08.122745 beacon2_import-1.0.4/beacon2_import/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2_import-1.0.4/beacon2_import/__init__.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    16575 2024-04-08 11:19:40.000000 beacon2_import-1.0.4/beacon2_import/beacon2_import.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2_import-1.0.4/beacon2_import/utils.py
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-17 10:31:08.126745 beacon2_import-1.0.4/beacon2_import.egg-info/
--rw-r--r--   0 khaled    (1000) khaled    (1000)      379 2024-04-17 10:31:08.000000 beacon2_import-1.0.4/beacon2_import.egg-info/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      425 2024-04-17 10:31:08.000000 beacon2_import-1.0.4/beacon2_import.egg-info/SOURCES.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-04-17 10:31:08.000000 beacon2_import-1.0.4/beacon2_import.egg-info/dependency_links.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      140 2024-04-17 10:31:08.000000 beacon2_import-1.0.4/beacon2_import.egg-info/entry_points.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       63 2024-04-17 10:31:08.000000 beacon2_import-1.0.4/beacon2_import.egg-info/requires.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       36 2024-04-17 10:31:08.000000 beacon2_import-1.0.4/beacon2_import.egg-info/top_level.txt
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-17 10:31:08.126745 beacon2_import-1.0.4/beacon2_search/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2_import-1.0.4/beacon2_search/__init__.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    13150 2024-04-08 11:19:47.000000 beacon2_import-1.0.4/beacon2_search/beacon2_search.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2_import-1.0.4/beacon2_search/utils.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-04-17 10:31:08.126745 beacon2_import-1.0.4/setup.cfg
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      843 2024-04-17 10:30:40.000000 beacon2_import-1.0.4/setup.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 12:17:34.000000 beacon2_import-1.0.4/utils.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 11:34:09.197252 beacon2-import-1.0.5/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      211 2024-04-19 11:34:09.197252 beacon2-import-1.0.5/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2-import-1.0.5/README.md
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 11:34:09.197252 beacon2-import-1.0.5/beacon2_import/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2-import-1.0.5/beacon2_import/__init__.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    16575 2024-04-08 11:19:40.000000 beacon2-import-1.0.5/beacon2_import/beacon2_import.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2-import-1.0.5/beacon2_import/utils.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 11:34:09.197252 beacon2-import-1.0.5/beacon2_import.egg-info/
+-rw-r--r--   0 khaled    (1000) khaled    (1000)      211 2024-04-19 11:34:09.000000 beacon2-import-1.0.5/beacon2_import.egg-info/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      425 2024-04-19 11:34:09.000000 beacon2-import-1.0.5/beacon2_import.egg-info/SOURCES.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-04-19 11:34:09.000000 beacon2-import-1.0.5/beacon2_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      140 2024-04-19 11:34:09.000000 beacon2-import-1.0.5/beacon2_import.egg-info/entry_points.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       54 2024-04-19 11:34:09.000000 beacon2-import-1.0.5/beacon2_import.egg-info/requires.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       36 2024-04-19 11:34:09.000000 beacon2-import-1.0.5/beacon2_import.egg-info/top_level.txt
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 11:34:09.197252 beacon2-import-1.0.5/beacon2_search/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2-import-1.0.5/beacon2_search/__init__.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    13150 2024-04-08 11:19:47.000000 beacon2-import-1.0.5/beacon2_search/beacon2_search.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2-import-1.0.5/beacon2_search/utils.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-04-19 11:34:09.197252 beacon2-import-1.0.5/setup.cfg
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      824 2024-04-19 11:33:50.000000 beacon2-import-1.0.5/setup.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 12:17:34.000000 beacon2-import-1.0.5/utils.py
```

### Comparing `beacon2_import-1.0.4/beacon2_import/beacon2_import.py` & `beacon2-import-1.0.5/beacon2_import/beacon2_import.py`

 * *Files identical despite different names*

### Comparing `beacon2_import-1.0.4/beacon2_import/utils.py` & `beacon2-import-1.0.5/beacon2_import/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2_import-1.0.4/beacon2_search/beacon2_search.py` & `beacon2-import-1.0.5/beacon2_search/beacon2_search.py`

 * *Files identical despite different names*

### Comparing `beacon2_import-1.0.4/beacon2_search/utils.py` & `beacon2-import-1.0.5/beacon2_search/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2_import-1.0.4/setup.py` & `beacon2-import-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beacon2-import',
-    version='1.0.4',
+    version='1.0.5',
     author='Khaled Jumah',
     author_email='khalled.jooma@yahoo.com',
     description='Seamlessly import and query genomic variant data from a beacon',
     license = 'CC-BY-NC-4.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'beacon2-import = beacon2_import.beacon2_import:beacon2_import',
             'beacon2-search = beacon2_search.beacon2_search:beacon_query'
         ]
     },
     install_requires=[
        'jsonschema',
-       'argparse',
        'dataclasses',
        'typing',
        'bioblend',
        'cyvcf2',
        'pymongo',
     ],
     dependency_links=[
```

### Comparing `beacon2_import-1.0.4/utils.py` & `beacon2-import-1.0.5/utils.py`

 * *Files identical despite different names*

