# Comparing `tmp/simbioreader-0.1.4.dev1.tar.gz` & `tmp/simbioreader-0.1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simbioreader-0.1.4.dev1.tar", last modified: Tue Apr 16 21:17:44 2024, max compression
+gzip compressed data, was "simbioreader-0.1.5.dev1.tar", last modified: Fri Apr 19 16:27:59 2024, max compression
```

## Comparing `simbioreader-0.1.4.dev1.tar` & `simbioreader-0.1.5.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:44.959104 simbioreader-0.1.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-16 21:17:44.959104 simbioreader-0.1.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:17:44.959104 simbioreader-0.1.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:44.959104 simbioreader-0.1.4.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:44.959104 simbioreader-0.1.4.dev1/src/SimbioReader/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/externals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/SimbioReader/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:44.959104 simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-16 21:17:44.000000 simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-16 21:17:44.000000 simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:17:44.000000 simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 21:17:44.000000 simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-16 21:17:44.000000 simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 21:17:44.000000 simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-16 21:17:40.000000 simbioreader-0.1.4.dev1/src/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:27:59.946980 simbioreader-0.1.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-19 16:27:59.946980 simbioreader-0.1.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:27:59.946980 simbioreader-0.1.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:27:59.942980 simbioreader-0.1.5.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:27:59.946980 simbioreader-0.1.5.dev1/src/SimbioReader/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/externals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/SimbioReader/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:27:59.946980 simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-19 16:27:59.000000 simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 16:27:59.000000 simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:27:59.000000 simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 16:27:59.000000 simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 16:27:59.000000 simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 16:27:59.000000 simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-19 16:27:55.000000 simbioreader-0.1.5.dev1/src/test.py
```

### Comparing `simbioreader-0.1.4.dev1/LICENSE` & `simbioreader-0.1.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.4.dev1/PKG-INFO` & `simbioreader-0.1.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimbioReader
-Version: 0.1.4.dev1
+Version: 0.1.5.dev1
 Summary: Python Reader for the data from SIMBIO-SYS instrument suite on-board the ESA mission BepiColombo
 Author-email: Romolo Politi <Romolo.Politi@inaf.it>
 License: GNU GPL ver3
 Project-URL: Repository, https://github.com/SIMBIO-SYS/SimbioReader
 Keywords: data reader,Space Mission,BepiColombo,SIMBIO-SYS
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simbioreader-0.1.4.dev1/README.md` & `simbioreader-0.1.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.4.dev1/pyproject.toml` & `simbioreader-0.1.5.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SimbioReader"
-version = "0.1.4-dev1"
+version = "0.1.5-dev1"
 description="Python Reader for the data from SIMBIO-SYS instrument suite on-board the ESA mission BepiColombo"
 dependencies = [
     "numpy",
     "pandas",
     "rich",
     "update_checker",
     'importlib-metadata; python_version>"3.10"',
```

### Comparing `simbioreader-0.1.4.dev1/src/SimbioReader/externals.py` & `simbioreader-0.1.5.dev1/src/SimbioReader/externals.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.4.dev1/src/SimbioReader/filters.py` & `simbioreader-0.1.5.dev1/src/SimbioReader/filters.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.4.dev1/src/SimbioReader/phases.py` & `simbioreader-0.1.5.dev1/src/SimbioReader/phases.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,15 +95,22 @@
     "ssmm_load":{
         "start": "2023-05-30 11:00:00",
         "stop": "2023-06-01 18:00:00",
         "name": "ssmm_load",
         "phase": "cruise",
         "LPName": "Cruise"
     },
+    "ico10": {
+        "start": "2023-11-05 23:30:00",
+        "stop": "2023-11-06 02:00:00",
+        "name": "ssmm_load",
+        "phase": "cruise",
+        "LPName": "Cruise"
+    },
     "None":{
-        "start" : "2021-11-23 00:00:01",
+        "start" : "2023-11-06 02:00:01",
         "stop"  : "2028-12-31 23:59:59",
         "name"  : "None",
         "phase" : "None",
         "LPName": "None"
     }
 }
```

### Comparing `simbioreader-0.1.4.dev1/src/SimbioReader/tools.py` & `simbioreader-0.1.5.dev1/src/SimbioReader/tools.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.4.dev1/src/SimbioReader/version.py` & `simbioreader-0.1.5.dev1/src/SimbioReader/version.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/PKG-INFO` & `simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimbioReader
-Version: 0.1.4.dev1
+Version: 0.1.5.dev1
 Summary: Python Reader for the data from SIMBIO-SYS instrument suite on-board the ESA mission BepiColombo
 Author-email: Romolo Politi <Romolo.Politi@inaf.it>
 License: GNU GPL ver3
 Project-URL: Repository, https://github.com/SIMBIO-SYS/SimbioReader
 Keywords: data reader,Space Mission,BepiColombo,SIMBIO-SYS
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simbioreader-0.1.4.dev1/src/SimbioReader.egg-info/SOURCES.txt` & `simbioreader-0.1.5.dev1/src/SimbioReader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

