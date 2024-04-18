# Comparing `tmp/dojo_ds-1.1.2.tar.gz` & `tmp/dojo_ds-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_ds-1.1.2.tar", last modified: Thu Apr 18 20:48:00 2024, max compression
+gzip compressed data, was "dojo_ds-1.1.3.tar", last modified: Thu Apr 18 22:58:27 2024, max compression
```

## Comparing `dojo_ds-1.1.2.tar` & `dojo_ds-1.1.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.567912 dojo_ds-1.1.2/
--rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.2/AUTHORS.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/CONTRIBUTING.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/HISTORY.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.2/LICENSE
--rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/MANIFEST.in
--rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 20:48:00.567743 dojo_ds-1.1.2/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.2/README.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.542040 dojo_ds-1.1.2/docs/
--rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.2/docs/Makefile
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/authors.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.522532 dojo_ds-1.1.2/docs/build/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.522700 dojo_ds-1.1.2/docs/build/html/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.543938 dojo_ds-1.1.2/docs/build/html/_static/
--rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.2/docs/build/html/_static/file.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.2/docs/build/html/_static/minus.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.2/docs/build/html/_static/plus.png
--rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.2/docs/conf.py
--rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/contributing.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.2/docs/dojo_ds.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/history.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.2/docs/index.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.2/docs/installation.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/make.bat
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.2/docs/modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.2/docs/old_modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/readme.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.2/docs/usage.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.556860 dojo_ds-1.1.2/dojo_ds/
--rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 20:47:52.000000 dojo_ds-1.1.2/dojo_ds/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.2/dojo_ds/_eda_functions_plotly.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.2/dojo_ds/cli.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.2/dojo_ds/data_enrichment.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.2/dojo_ds/deploy.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.2/dojo_ds/eda.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.2/dojo_ds/evaluate.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.2/dojo_ds/imports.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.2/dojo_ds/insights.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.2/dojo_ds/matplotlib_style.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.2/dojo_ds/nlp.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    16600 2024-04-18 20:47:40.000000 dojo_ds-1.1.2/dojo_ds/time_series.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.2/dojo_ds/utils.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.567144 dojo_ds-1.1.2/dojo_ds.egg-info/
--rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/SOURCES.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/dependency_links.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/entry_points.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.2/dojo_ds.egg-info/not-zip-safe
--rw-r--r--   0 codingdojo   (502) staff       (20)      121 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/requires.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/top_level.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 20:48:00.568320 dojo_ds-1.1.2/setup.cfg
--rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 20:47:52.000000 dojo_ds-1.1.2/setup.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.566560 dojo_ds-1.1.2/tests/
--rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/tests/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.2/tests/test_dojo_ds.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.948877 dojo_ds-1.1.3/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.3/AUTHORS.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/HISTORY.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.3/LICENSE
+-rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/MANIFEST.in
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 22:58:27.948682 dojo_ds-1.1.3/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.3/README.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.930246 dojo_ds-1.1.3/docs/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.3/docs/Makefile
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/docs/authors.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.905431 dojo_ds-1.1.3/docs/build/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.905568 dojo_ds-1.1.3/docs/build/html/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.932678 dojo_ds-1.1.3/docs/build/html/_static/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.3/docs/build/html/_static/file.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.3/docs/build/html/_static/minus.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.3/docs/build/html/_static/plus.png
+-rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.3/docs/conf.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/docs/contributing.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.3/docs/dojo_ds.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/docs/history.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.3/docs/index.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.3/docs/installation.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/docs/make.bat
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.3/docs/modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.3/docs/old_modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/docs/readme.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.3/docs/usage.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.942535 dojo_ds-1.1.3/dojo_ds/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 22:58:21.000000 dojo_ds-1.1.3/dojo_ds/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.3/dojo_ds/_eda_functions_plotly.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.3/dojo_ds/cli.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.3/dojo_ds/data_enrichment.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.3/dojo_ds/deploy.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.3/dojo_ds/eda.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.3/dojo_ds/evaluate.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.3/dojo_ds/imports.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.3/dojo_ds/insights.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.3/dojo_ds/matplotlib_style.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.3/dojo_ds/nlp.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    20009 2024-04-18 22:57:07.000000 dojo_ds-1.1.3/dojo_ds/time_series.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.3/dojo_ds/utils.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.948021 dojo_ds-1.1.3/dojo_ds.egg-info/
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 22:58:27.000000 dojo_ds-1.1.3/dojo_ds.egg-info/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 22:58:27.000000 dojo_ds-1.1.3/dojo_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 22:58:27.000000 dojo_ds-1.1.3/dojo_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 22:58:27.000000 dojo_ds-1.1.3/dojo_ds.egg-info/entry_points.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.3/dojo_ds.egg-info/not-zip-safe
+-rw-r--r--   0 codingdojo   (502) staff       (20)      121 2024-04-18 22:58:27.000000 dojo_ds-1.1.3/dojo_ds.egg-info/requires.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 22:58:27.000000 dojo_ds-1.1.3/dojo_ds.egg-info/top_level.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 22:58:27.949388 dojo_ds-1.1.3/setup.cfg
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 22:58:21.000000 dojo_ds-1.1.3/setup.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 22:58:27.947198 dojo_ds-1.1.3/tests/
+-rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.3/tests/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.3/tests/test_dojo_ds.py
```

### Comparing `dojo_ds-1.1.2/CONTRIBUTING.rst` & `dojo_ds-1.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/LICENSE` & `dojo_ds-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/PKG-INFO` & `dojo_ds-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.2
+Version: 1.1.3
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-1.1.2/README.rst` & `dojo_ds-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/docs/Makefile` & `dojo_ds-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/docs/conf.py` & `dojo_ds-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/docs/dojo_ds.rst` & `dojo_ds-1.1.3/docs/dojo_ds.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/docs/installation.rst` & `dojo_ds-1.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/docs/make.bat` & `dojo_ds-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/__init__.py` & `dojo_ds-1.1.3/dojo_ds/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Custom Functions the Data Science Program
 __author__ = James Irving, Brenda Hungerford
 """
 __author__ = """James Irving"""
 __email__ = 'james.irving.phd@gmail.com'
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 from . import data_enrichment as data
 from . import eda 
 from . import evaluate
 from . import insights 
 from . import nlp
 from . import time_series
```

### Comparing `dojo_ds-1.1.2/dojo_ds/_eda_functions_plotly.py` & `dojo_ds-1.1.3/dojo_ds/_eda_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/data_enrichment.py` & `dojo_ds-1.1.3/dojo_ds/data_enrichment.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/deploy.py` & `dojo_ds-1.1.3/dojo_ds/deploy.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/eda.py` & `dojo_ds-1.1.3/dojo_ds/eda.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/evaluate.py` & `dojo_ds-1.1.3/dojo_ds/evaluate.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/insights.py` & `dojo_ds-1.1.3/dojo_ds/insights.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/nlp.py` & `dojo_ds-1.1.3/dojo_ds/nlp.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds/time_series.py` & `dojo_ds-1.1.3/dojo_ds/time_series.py`

 * *Files 13% similar despite different names*

```diff
@@ -414,8 +414,94 @@
     else: 
         try:
             from IPython.display import Markdown, display
             display_func = lambda x: display(Markdown(x))
         except:
             display_func = print
             
-        display_func(table)
+        display_func(table)
+        
+
+
+
+def make_best_arima(auto_model, ts_train, exog=None, fit_kws={}):
+    """
+    Fits a final ARIMA model using the best parameters obtained from an auto_model and evaluates its performance.
+
+    Parameters:
+    auto_model (AutoARIMA): The AutoARIMA model object that contains the best parameters.
+    ts_train (array-like): The time series data used for training the ARIMA model.
+    exog (array-like, optional): Exogenous variables to be included in the model. Default is None.
+    fit_kws (dict, optional): Additional keyword arguments to be passed to the `fit` method of the SARIMAX model. Default is an empty dictionary.
+
+    Returns:
+    SARIMAX: The fitted SARIMAX model with the best parameters.
+
+    """
+    best_model = tsa.SARIMAX(
+        ts_train,
+        exog=exog,
+        order=auto_model.order,
+        seasonal_order=auto_model.seasonal_order,
+        sarimax_kwargs=auto_model.sarimax_kwargs,
+    ).fit(disp=False, **fit_kws)
+    return best_model
+
+    
+            
+        
+def evaluate_ts_model(model, ts_train, ts_test, exog_train=None, exog_test=None,
+                      return_scores=False, show_summary=True,
+                      n_train_lags=None, figsize=(9,3),
+                      title='Comparing Forecast vs. True Data'):
+    """
+    Evaluates a time series model by generating forecasts and comparing them to the true data.
+
+    Parameters:
+    - model: The time series model to be evaluated (Either SARIMAX or AutoARIMA object)
+    - ts_train: The training time series data.
+    - ts_test: The testing time series data.
+    - exog_train: The exogenous variables for the training data (optional).
+    - exog_test: The exogenous variables for the testing data (optional).
+    - return_scores: Whether to return the model and regression metrics (optional, default=False).
+    - show_summary: Whether to display the model summary and diagnostics plots (optional, default=True).
+    - n_train_lags: The number of lagged values to include in the training data visualization (optional).
+    - figsize: The size of the forecast plot (optional, default=(9,3)).
+    - title: The title of the forecast plot (optional, default='Comparing Forecast vs. True Data').
+
+    Returns:
+    - If return_scores=True, returns the model and regression metrics.
+    - If return_scores=False, returns the model.
+
+    """
+    ## GET FORECAST             
+    # Check if auto-arima, if so, extract sarima model
+    if hasattr(model, "arima_res_"):
+        print(f"- Fitting a new ARIMA using the params from the auto_arima...")
+        model = make_best_arima(model, ts_train, exog=exog_train)
+        
+
+    # Get forecast         
+    forecast = model.get_forecast(exog=exog_test, steps=len(ts_test))
+    forecast_df = forecast.summary_frame()
+
+    # Visualize forecast
+    plot_forecast(ts_train, ts_test, forecast_df, 
+                  n_train_lags=n_train_lags, figsize=figsize,
+                 title=title)
+
+    plt.show()
+                    
+    # Get and display the regression metrics BEFORE showing plot
+    reg_res = regression_metrics_ts(ts_test, forecast_df['mean'], 
+                                        output_dict=True)
+    
+    if show_summary==True:
+        display(model.summary())
+        model.plot_diagnostics(figsize=(8,4))
+        plt.tight_layout()
+        plt.show()
+      
+    if return_scores:
+        return model, reg_res
+    else:
+        return model
```

### Comparing `dojo_ds-1.1.2/dojo_ds/utils.py` & `dojo_ds-1.1.3/dojo_ds/utils.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/dojo_ds.egg-info/PKG-INFO` & `dojo_ds-1.1.3/dojo_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.2
+Version: 1.1.3
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-1.1.2/dojo_ds.egg-info/SOURCES.txt` & `dojo_ds-1.1.3/dojo_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.2/setup.py` & `dojo_ds-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,10 +69,10 @@
     include_package_data=True,
     keywords='dojo_ds',
     name='dojo_ds',
     packages=find_packages(include=['dojo_ds', 'dojo_ds.*']),
     test_suite='tests',
     tests_require=load_requirements("./requirements.txt") + test_requirements,
     url='https://github.com/coding-dojo-data-science/dojo_ds',
-    version='1.1.2',
+    version='1.1.3',
     zip_safe=False,
 )
```

### Comparing `dojo_ds-1.1.2/tests/test_dojo_ds.py` & `dojo_ds-1.1.3/tests/test_dojo_ds.py`

 * *Files identical despite different names*

