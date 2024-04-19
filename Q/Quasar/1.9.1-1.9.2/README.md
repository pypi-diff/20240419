# Comparing `tmp/Quasar-1.9.1.tar.gz` & `tmp/Quasar-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quasar-1.9.1.tar", last modified: Wed Feb  7 10:59:05 2024, max compression
+gzip compressed data, was "Quasar-1.9.2.tar", last modified: Fri Apr 19 08:09:20 2024, max compression
```

## Comparing `Quasar-1.9.1.tar` & `Quasar-1.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-02-07 10:59:05.209702 Quasar-1.9.1/
--rw-rw-r--   0 marko     (1000) marko     (1000)      633 2019-07-01 09:06:00.000000 Quasar-1.9.1/LICENSE
--rw-rw-r--   0 marko     (1000) marko     (1000)      208 2022-04-28 11:04:25.000000 Quasar-1.9.1/MANIFEST.in
--rw-rw-r--   0 marko     (1000) marko     (1000)      730 2024-02-07 10:59:05.209702 Quasar-1.9.1/PKG-INFO
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-02-07 10:59:05.205702 Quasar-1.9.1/Quasar.egg-info/
--rw-rw-r--   0 marko     (1000) marko     (1000)      730 2024-02-07 10:59:05.000000 Quasar-1.9.1/Quasar.egg-info/PKG-INFO
--rw-rw-r--   0 marko     (1000) marko     (1000)      517 2024-02-07 10:59:05.000000 Quasar-1.9.1/Quasar.egg-info/SOURCES.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)        1 2024-02-07 10:59:05.000000 Quasar-1.9.1/Quasar.egg-info/dependency_links.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)      107 2024-02-07 10:59:05.000000 Quasar-1.9.1/Quasar.egg-info/entry_points.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)        1 2022-04-28 13:46:58.000000 Quasar-1.9.1/Quasar.egg-info/not-zip-safe
--rw-rw-r--   0 marko     (1000) marko     (1000)       44 2024-02-07 10:59:05.000000 Quasar-1.9.1/Quasar.egg-info/requires.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)        7 2024-02-07 10:59:05.000000 Quasar-1.9.1/Quasar.egg-info/top_level.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)      393 2019-07-01 09:06:00.000000 Quasar-1.9.1/README.pypi
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-02-07 10:59:05.205702 Quasar-1.9.1/quasar/
--rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-07-01 09:06:00.000000 Quasar-1.9.1/quasar/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)      137 2019-07-01 09:06:00.000000 Quasar-1.9.1/quasar/__main__.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-02-07 10:59:05.205702 Quasar-1.9.1/quasar/launcher/
--rw-rw-r--   0 marko     (1000) marko     (1000)     3171 2019-09-09 11:35:44.000000 Quasar-1.9.1/quasar/launcher/__init__.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-02-07 10:59:05.205702 Quasar-1.9.1/quasar/launcher/icons/
--rw-rw-r--   0 marko     (1000) marko     (1000)    73483 2019-07-01 09:06:00.000000 Quasar-1.9.1/quasar/launcher/icons/quasar.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)    50694 2019-07-01 09:06:00.000000 Quasar-1.9.1/quasar/launcher/icons/splash.png
--rw-rw-r--   0 marko     (1000) marko     (1000)      841 2019-07-01 09:06:00.000000 Quasar-1.9.1/quasar/launcher/splash.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     4932 2019-09-09 11:35:44.000000 Quasar-1.9.1/quasar/launcher/update_check.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-02-07 10:59:05.209702 Quasar-1.9.1/quasar/tests/
--rw-rw-r--   0 marko     (1000) marko     (1000)      481 2019-07-01 09:34:14.000000 Quasar-1.9.1/quasar/tests/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1676 2019-09-09 11:35:44.000000 Quasar-1.9.1/quasar/tests/test_update_check.py
--rw-rw-r--   0 marko     (1000) marko     (1000)       44 2024-02-07 09:37:45.000000 Quasar-1.9.1/requirements.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)       38 2024-02-07 10:59:05.209702 Quasar-1.9.1/setup.cfg
--rw-rw-r--   0 marko     (1000) marko     (1000)     1870 2024-02-07 10:22:43.000000 Quasar-1.9.1/setup.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-04-19 08:09:20.266767 Quasar-1.9.2/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      633 2019-07-01 09:06:00.000000 Quasar-1.9.2/LICENSE
+-rw-rw-r--   0 marko     (1000) marko     (1000)      208 2022-04-28 11:04:25.000000 Quasar-1.9.2/MANIFEST.in
+-rw-rw-r--   0 marko     (1000) marko     (1000)      730 2024-04-19 08:09:20.266767 Quasar-1.9.2/PKG-INFO
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-04-19 08:09:20.262767 Quasar-1.9.2/Quasar.egg-info/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      730 2024-04-19 08:09:20.000000 Quasar-1.9.2/Quasar.egg-info/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)      517 2024-04-19 08:09:20.000000 Quasar-1.9.2/Quasar.egg-info/SOURCES.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2024-04-19 08:09:20.000000 Quasar-1.9.2/Quasar.egg-info/dependency_links.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)      107 2024-04-19 08:09:20.000000 Quasar-1.9.2/Quasar.egg-info/entry_points.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2022-04-28 13:46:58.000000 Quasar-1.9.2/Quasar.egg-info/not-zip-safe
+-rw-rw-r--   0 marko     (1000) marko     (1000)       44 2024-04-19 08:09:20.000000 Quasar-1.9.2/Quasar.egg-info/requires.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        7 2024-04-19 08:09:20.000000 Quasar-1.9.2/Quasar.egg-info/top_level.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)      393 2019-07-01 09:06:00.000000 Quasar-1.9.2/README.pypi
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-04-19 08:09:20.262767 Quasar-1.9.2/quasar/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-07-01 09:06:00.000000 Quasar-1.9.2/quasar/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      137 2019-07-01 09:06:00.000000 Quasar-1.9.2/quasar/__main__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-04-19 08:09:20.262767 Quasar-1.9.2/quasar/launcher/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3171 2019-09-09 11:35:44.000000 Quasar-1.9.2/quasar/launcher/__init__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-04-19 08:09:20.262767 Quasar-1.9.2/quasar/launcher/icons/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    73483 2019-07-01 09:06:00.000000 Quasar-1.9.2/quasar/launcher/icons/quasar.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)    50694 2019-07-01 09:06:00.000000 Quasar-1.9.2/quasar/launcher/icons/splash.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)      841 2019-07-01 09:06:00.000000 Quasar-1.9.2/quasar/launcher/splash.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4932 2019-09-09 11:35:44.000000 Quasar-1.9.2/quasar/launcher/update_check.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-04-19 08:09:20.262767 Quasar-1.9.2/quasar/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      481 2019-07-01 09:34:14.000000 Quasar-1.9.2/quasar/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1676 2019-09-09 11:35:44.000000 Quasar-1.9.2/quasar/tests/test_update_check.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)       44 2024-04-18 13:28:52.000000 Quasar-1.9.2/requirements.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       38 2024-04-19 08:09:20.266767 Quasar-1.9.2/setup.cfg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1870 2024-04-18 13:28:52.000000 Quasar-1.9.2/setup.py
```

### Comparing `Quasar-1.9.1/LICENSE` & `Quasar-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/PKG-INFO` & `Quasar-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quasar
-Version: 1.9.1
+Version: 1.9.2
 Summary: Quasar is a collection of data analysis toolboxes extending the Orange suite.
 Home-page: https://quasar.codes
 Author: Canadian Light Source, Biolab UL, Soleil, Elettra
 Author-email: marko@toplak.io
 License: GPLv3+
 Keywords: orange3,spectroscopy,infrared
 License-File: LICENSE
```

### Comparing `Quasar-1.9.1/Quasar.egg-info/PKG-INFO` & `Quasar-1.9.2/Quasar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quasar
-Version: 1.9.1
+Version: 1.9.2
 Summary: Quasar is a collection of data analysis toolboxes extending the Orange suite.
 Home-page: https://quasar.codes
 Author: Canadian Light Source, Biolab UL, Soleil, Elettra
 Author-email: marko@toplak.io
 License: GPLv3+
 Keywords: orange3,spectroscopy,infrared
 License-File: LICENSE
```

### Comparing `Quasar-1.9.1/Quasar.egg-info/SOURCES.txt` & `Quasar-1.9.2/Quasar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/quasar/launcher/__init__.py` & `Quasar-1.9.2/quasar/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/quasar/launcher/icons/quasar.svg` & `Quasar-1.9.2/quasar/launcher/icons/quasar.svg`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/quasar/launcher/icons/splash.png` & `Quasar-1.9.2/quasar/launcher/icons/splash.png`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/quasar/launcher/splash.py` & `Quasar-1.9.2/quasar/launcher/splash.py`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/quasar/launcher/update_check.py` & `Quasar-1.9.2/quasar/launcher/update_check.py`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/quasar/tests/test_update_check.py` & `Quasar-1.9.2/quasar/tests/test_update_check.py`

 * *Files identical despite different names*

### Comparing `Quasar-1.9.1/setup.py` & `Quasar-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from os import path
 
 from setuptools import setup, find_packages, Command
 
 NAME = "Quasar"
 
-VERSION = "1.9.1"
+VERSION = "1.9.2"
 
 DESCRIPTION = "Quasar is a collection of data analysis toolboxes extending the Orange suite."
 LONG_DESCRIPTION = open(path.join(path.dirname(__file__), 'README.pypi')).read()
 AUTHOR = 'Canadian Light Source, Biolab UL, Soleil, Elettra'
 AUTHOR_EMAIL = 'marko@toplak.io'
 URL = "https://quasar.codes"
```

