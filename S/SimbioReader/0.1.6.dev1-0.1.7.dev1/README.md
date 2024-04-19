# Comparing `tmp/simbioreader-0.1.6.dev1.tar.gz` & `tmp/simbioreader-0.1.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simbioreader-0.1.6.dev1.tar", last modified: Fri Apr 19 16:45:23 2024, max compression
+gzip compressed data, was "simbioreader-0.1.7.dev1.tar", last modified: Fri Apr 19 17:08:44 2024, max compression
```

## Comparing `simbioreader-0.1.6.dev1.tar` & `simbioreader-0.1.7.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:45:23.415977 simbioreader-0.1.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-19 16:45:23.415977 simbioreader-0.1.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:45:23.415977 simbioreader-0.1.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:45:23.411977 simbioreader-0.1.6.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:45:23.411977 simbioreader-0.1.6.dev1/src/SimbioReader/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/externals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/SimbioReader/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:45:23.411977 simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-19 16:45:23.000000 simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 16:45:23.000000 simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:45:23.000000 simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 16:45:23.000000 simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 16:45:23.000000 simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 16:45:23.000000 simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-19 16:45:19.000000 simbioreader-0.1.6.dev1/src/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:08:44.166266 simbioreader-0.1.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-19 17:08:44.166266 simbioreader-0.1.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:08:44.166266 simbioreader-0.1.7.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:08:44.162266 simbioreader-0.1.7.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:08:44.166266 simbioreader-0.1.7.dev1/src/SimbioReader/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/externals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/SimbioReader/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:08:44.166266 simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-19 17:08:44.000000 simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 17:08:44.000000 simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:08:44.000000 simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 17:08:44.000000 simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 17:08:44.000000 simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 17:08:44.000000 simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-19 17:08:39.000000 simbioreader-0.1.7.dev1/src/test.py
```

### Comparing `simbioreader-0.1.6.dev1/LICENSE` & `simbioreader-0.1.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.6.dev1/PKG-INFO` & `simbioreader-0.1.7.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimbioReader
-Version: 0.1.6.dev1
+Version: 0.1.7.dev1
 Summary: Python Reader for the data from SIMBIO-SYS instrument suite on-board the ESA mission BepiColombo
 Author-email: Romolo Politi <Romolo.Politi@inaf.it>
 License: GNU GPL ver3
 Project-URL: Repository, https://github.com/SIMBIO-SYS/SimbioReader
 Keywords: data reader,Space Mission,BepiColombo,SIMBIO-SYS
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simbioreader-0.1.6.dev1/README.md` & `simbioreader-0.1.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.6.dev1/pyproject.toml` & `simbioreader-0.1.7.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SimbioReader"
-version = "0.1.6-dev1"
+version = "0.1.7-dev1"
 description="Python Reader for the data from SIMBIO-SYS instrument suite on-board the ESA mission BepiColombo"
 dependencies = [
     "numpy",
     "pandas",
     "rich",
     "update_checker",
     'importlib-metadata; python_version>"3.10"',
```

### Comparing `simbioreader-0.1.6.dev1/src/SimbioReader/externals.py` & `simbioreader-0.1.7.dev1/src/SimbioReader/externals.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.6.dev1/src/SimbioReader/filters.py` & `simbioreader-0.1.7.dev1/src/SimbioReader/filters.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.6.dev1/src/SimbioReader/phases.py` & `simbioreader-0.1.7.dev1/src/SimbioReader/phases.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,19 +98,26 @@
         "name": "ssmm_load",
         "phase": "cruise",
         "LPName": "Cruise"
     },
     "ico10": {
         "start": "2023-11-05 23:30:00",
         "stop": "2023-11-06 02:00:00",
-        "name": "ssmm_load",
+        "name": "ico10",
+        "phase": "cruise",
+        "LPName": "Cruise"
+    },
+    "ico11": {
+        "start": "2024-04-08 00:00:00",
+        "stop": "2024-04-08 04:00:00",
+        "name": "ico11",
         "phase": "cruise",
         "LPName": "Cruise"
     },
     "None":{
-        "start" : "2023-11-06 02:00:01",
+        "start" : "2024-04-08 04:00:01",
         "stop"  : "2028-12-31 23:59:59",
         "name"  : "None",
         "phase" : "None",
         "LPName": "None"
     }
 }
```

### Comparing `simbioreader-0.1.6.dev1/src/SimbioReader/tools.py` & `simbioreader-0.1.7.dev1/src/SimbioReader/tools.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.6.dev1/src/SimbioReader/version.py` & `simbioreader-0.1.7.dev1/src/SimbioReader/version.py`

 * *Files identical despite different names*

### Comparing `simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/PKG-INFO` & `simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimbioReader
-Version: 0.1.6.dev1
+Version: 0.1.7.dev1
 Summary: Python Reader for the data from SIMBIO-SYS instrument suite on-board the ESA mission BepiColombo
 Author-email: Romolo Politi <Romolo.Politi@inaf.it>
 License: GNU GPL ver3
 Project-URL: Repository, https://github.com/SIMBIO-SYS/SimbioReader
 Keywords: data reader,Space Mission,BepiColombo,SIMBIO-SYS
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simbioreader-0.1.6.dev1/src/SimbioReader.egg-info/SOURCES.txt` & `simbioreader-0.1.7.dev1/src/SimbioReader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

