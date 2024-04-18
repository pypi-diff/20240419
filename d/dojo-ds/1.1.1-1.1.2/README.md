# Comparing `tmp/dojo_ds-1.1.1.tar.gz` & `tmp/dojo_ds-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_ds-1.1.1.tar", last modified: Thu Apr 18 19:38:18 2024, max compression
+gzip compressed data, was "dojo_ds-1.1.2.tar", last modified: Thu Apr 18 20:48:00 2024, max compression
```

## Comparing `dojo_ds-1.1.1.tar` & `dojo_ds-1.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.141604 dojo_ds-1.1.1/
--rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.1/AUTHORS.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/CONTRIBUTING.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/HISTORY.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.1/LICENSE
--rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/MANIFEST.in
--rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:38:18.141423 dojo_ds-1.1.1/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.1/README.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.121416 dojo_ds-1.1.1/docs/
--rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.1/docs/Makefile
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/authors.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.099342 dojo_ds-1.1.1/docs/build/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.100000 dojo_ds-1.1.1/docs/build/html/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.123353 dojo_ds-1.1.1/docs/build/html/_static/
--rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.1/docs/build/html/_static/file.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.1/docs/build/html/_static/minus.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.1/docs/build/html/_static/plus.png
--rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.1/docs/conf.py
--rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/contributing.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.1/docs/dojo_ds.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/history.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.1/docs/index.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.1/docs/installation.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/make.bat
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.1/docs/modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.1/docs/old_modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/readme.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.1/docs/usage.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.134170 dojo_ds-1.1.1/dojo_ds/
--rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 19:38:08.000000 dojo_ds-1.1.1/dojo_ds/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.1/dojo_ds/_eda_functions_plotly.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.1/dojo_ds/cli.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.1/dojo_ds/data_enrichment.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.1/dojo_ds/deploy.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.1/dojo_ds/eda.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.1/dojo_ds/evaluate.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.1/dojo_ds/imports.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.1/dojo_ds/insights.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.1/dojo_ds/matplotlib_style.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.1/dojo_ds/nlp.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    10346 2024-04-18 19:37:49.000000 dojo_ds-1.1.1/dojo_ds/time_series.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.1/dojo_ds/utils.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.140929 dojo_ds-1.1.1/dojo_ds.egg-info/
--rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/SOURCES.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/dependency_links.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/entry_points.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.1/dojo_ds.egg-info/not-zip-safe
--rw-r--r--   0 codingdojo   (502) staff       (20)      104 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/requires.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/top_level.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 19:38:18.142695 dojo_ds-1.1.1/setup.cfg
--rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 19:38:08.000000 dojo_ds-1.1.1/setup.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.139759 dojo_ds-1.1.1/tests/
--rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/tests/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.1/tests/test_dojo_ds.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.567912 dojo_ds-1.1.2/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.2/AUTHORS.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/HISTORY.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.2/LICENSE
+-rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/MANIFEST.in
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 20:48:00.567743 dojo_ds-1.1.2/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.2/README.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.542040 dojo_ds-1.1.2/docs/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.2/docs/Makefile
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/authors.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.522532 dojo_ds-1.1.2/docs/build/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.522700 dojo_ds-1.1.2/docs/build/html/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.543938 dojo_ds-1.1.2/docs/build/html/_static/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.2/docs/build/html/_static/file.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.2/docs/build/html/_static/minus.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.2/docs/build/html/_static/plus.png
+-rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.2/docs/conf.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/contributing.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.2/docs/dojo_ds.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/history.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.2/docs/index.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.2/docs/installation.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/make.bat
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.2/docs/modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.2/docs/old_modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/docs/readme.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.2/docs/usage.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.556860 dojo_ds-1.1.2/dojo_ds/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 20:47:52.000000 dojo_ds-1.1.2/dojo_ds/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.2/dojo_ds/_eda_functions_plotly.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.2/dojo_ds/cli.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.2/dojo_ds/data_enrichment.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.2/dojo_ds/deploy.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.2/dojo_ds/eda.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.2/dojo_ds/evaluate.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.2/dojo_ds/imports.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.2/dojo_ds/insights.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.2/dojo_ds/matplotlib_style.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.2/dojo_ds/nlp.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    16600 2024-04-18 20:47:40.000000 dojo_ds-1.1.2/dojo_ds/time_series.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.2/dojo_ds/utils.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.567144 dojo_ds-1.1.2/dojo_ds.egg-info/
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/entry_points.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.2/dojo_ds.egg-info/not-zip-safe
+-rw-r--r--   0 codingdojo   (502) staff       (20)      121 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/requires.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 20:48:00.000000 dojo_ds-1.1.2/dojo_ds.egg-info/top_level.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 20:48:00.568320 dojo_ds-1.1.2/setup.cfg
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 20:47:52.000000 dojo_ds-1.1.2/setup.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 20:48:00.566560 dojo_ds-1.1.2/tests/
+-rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.2/tests/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.2/tests/test_dojo_ds.py
```

### Comparing `dojo_ds-1.1.1/CONTRIBUTING.rst` & `dojo_ds-1.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/LICENSE` & `dojo_ds-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/PKG-INFO` & `dojo_ds-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.1
+Version: 1.1.2
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,14 +20,15 @@
 License-File: AUTHORS.rst
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: statsmodels>=0.13.5
 Requires-Dist: pmdarima==2.0.4
+Requires-Dist: requests>=2.26.0
 
 =======
 dojo-ds
 =======
 
 
 .. image:: https://img.shields.io/pypi/v/dojo_ds.svg
```

### Comparing `dojo_ds-1.1.1/README.rst` & `dojo_ds-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/docs/Makefile` & `dojo_ds-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/docs/conf.py` & `dojo_ds-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/docs/dojo_ds.rst` & `dojo_ds-1.1.2/docs/dojo_ds.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/docs/installation.rst` & `dojo_ds-1.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/docs/make.bat` & `dojo_ds-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/__init__.py` & `dojo_ds-1.1.2/dojo_ds/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Custom Functions the Data Science Program
 __author__ = James Irving, Brenda Hungerford
 """
 __author__ = """James Irving"""
 __email__ = 'james.irving.phd@gmail.com'
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 from . import data_enrichment as data
 from . import eda 
 from . import evaluate
 from . import insights 
 from . import nlp
 from . import time_series
```

### Comparing `dojo_ds-1.1.1/dojo_ds/_eda_functions_plotly.py` & `dojo_ds-1.1.2/dojo_ds/_eda_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/data_enrichment.py` & `dojo_ds-1.1.2/dojo_ds/data_enrichment.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/deploy.py` & `dojo_ds-1.1.2/dojo_ds/deploy.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/eda.py` & `dojo_ds-1.1.2/dojo_ds/eda.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/evaluate.py` & `dojo_ds-1.1.2/dojo_ds/evaluate.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/insights.py` & `dojo_ds-1.1.2/dojo_ds/insights.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/nlp.py` & `dojo_ds-1.1.2/dojo_ds/nlp.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds/utils.py` & `dojo_ds-1.1.2/dojo_ds/utils.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/dojo_ds.egg-info/PKG-INFO` & `dojo_ds-1.1.2/dojo_ds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.1
+Version: 1.1.2
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,14 +20,15 @@
 License-File: AUTHORS.rst
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: statsmodels>=0.13.5
 Requires-Dist: pmdarima==2.0.4
+Requires-Dist: requests>=2.26.0
 
 =======
 dojo-ds
 =======
 
 
 .. image:: https://img.shields.io/pypi/v/dojo_ds.svg
```

### Comparing `dojo_ds-1.1.1/dojo_ds.egg-info/SOURCES.txt` & `dojo_ds-1.1.2/dojo_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.1/setup.py` & `dojo_ds-1.1.2/setup.py`

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
-    version='1.1.1',
+    version='1.1.2',
     zip_safe=False,
 )
```

### Comparing `dojo_ds-1.1.1/tests/test_dojo_ds.py` & `dojo_ds-1.1.2/tests/test_dojo_ds.py`

 * *Files identical despite different names*

