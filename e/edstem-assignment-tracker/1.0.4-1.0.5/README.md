# Comparing `tmp/edstem_assignment_tracker-1.0.4.tar.gz` & `tmp/edstem_assignment_tracker-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edstem_assignment_tracker-1.0.4.tar", last modified: Fri Apr 19 04:29:34 2024, max compression
+gzip compressed data, was "edstem_assignment_tracker-1.0.5.tar", last modified: Fri Apr 19 04:52:56 2024, max compression
```

## Comparing `edstem_assignment_tracker-1.0.4.tar` & `edstem_assignment_tracker-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:29:34.213740 edstem_assignment_tracker-1.0.4/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:29:34.213529 edstem_assignment_tracker-1.0.4/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.4/README.md
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:29:34.211167 edstem_assignment_tracker-1.0.4/edstem/
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:29:34.212197 edstem_assignment_tracker-1.0.4/edstem/integration/
--rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.4/edstem/integration/__init__.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.4/edstem/integration/get_data.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.4/edstem/integration/run_eat.py
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:29:34.212321 edstem_assignment_tracker-1.0.4/edstem/integration/storage/
--rw-r--r--   0 trevormoy   (501) staff       (20)    12090 2024-04-19 04:10:46.000000 edstem_assignment_tracker-1.0.4/edstem/integration/storage/main.cpp
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:29:34.213321 edstem_assignment_tracker-1.0.4/edstem_assignment_tracker.egg-info/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:29:34.000000 edstem_assignment_tracker-1.0.4/edstem_assignment_tracker.egg-info/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      390 2024-04-19 04:29:34.000000 edstem_assignment_tracker-1.0.4/edstem_assignment_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 04:29:34.000000 edstem_assignment_tracker-1.0.4/edstem_assignment_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 04:29:34.000000 edstem_assignment_tracker-1.0.4/edstem_assignment_tracker.egg-info/requires.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 04:29:34.000000 edstem_assignment_tracker-1.0.4/edstem_assignment_tracker.egg-info/top_level.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 04:29:34.213791 edstem_assignment_tracker-1.0.4/setup.cfg
--rw-r--r--   0 trevormoy   (501) staff       (20)     1099 2024-04-19 04:29:27.000000 edstem_assignment_tracker-1.0.4/setup.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:52:56.690184 edstem_assignment_tracker-1.0.5/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:52:56.689984 edstem_assignment_tracker-1.0.5/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.5/README.md
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:52:56.687289 edstem_assignment_tracker-1.0.5/edstem/
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:52:56.688583 edstem_assignment_tracker-1.0.5/edstem/integration/
+-rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.5/edstem/integration/__init__.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.5/edstem/integration/get_data.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.5/edstem/integration/run_eat.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:52:56.688846 edstem_assignment_tracker-1.0.5/edstem/integration/storage/
+-rw-r--r--   0 trevormoy   (501) staff       (20)    12090 2024-04-19 04:10:46.000000 edstem_assignment_tracker-1.0.5/edstem/integration/storage/main.cpp
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:52:56.689731 edstem_assignment_tracker-1.0.5/edstem_assignment_tracker.egg-info/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:52:56.000000 edstem_assignment_tracker-1.0.5/edstem_assignment_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      390 2024-04-19 04:52:56.000000 edstem_assignment_tracker-1.0.5/edstem_assignment_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 04:52:56.000000 edstem_assignment_tracker-1.0.5/edstem_assignment_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 04:52:56.000000 edstem_assignment_tracker-1.0.5/edstem_assignment_tracker.egg-info/requires.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 04:52:56.000000 edstem_assignment_tracker-1.0.5/edstem_assignment_tracker.egg-info/top_level.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 04:52:56.690225 edstem_assignment_tracker-1.0.5/setup.cfg
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1074 2024-04-19 04:52:36.000000 edstem_assignment_tracker-1.0.5/setup.py
```

### Comparing `edstem_assignment_tracker-1.0.4/PKG-INFO` & `edstem_assignment_tracker-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.4
+Version: 1.0.5
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.4/README.md` & `edstem_assignment_tracker-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.4/edstem/integration/get_data.py` & `edstem_assignment_tracker-1.0.5/edstem/integration/get_data.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.4/edstem/integration/run_eat.py` & `edstem_assignment_tracker-1.0.5/edstem/integration/run_eat.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.4/edstem/integration/storage/main.cpp` & `edstem_assignment_tracker-1.0.5/edstem/integration/storage/main.cpp`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.4/edstem_assignment_tracker.egg-info/PKG-INFO` & `edstem_assignment_tracker-1.0.5/edstem_assignment_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.4
+Version: 1.0.5
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.4/setup.py` & `edstem_assignment_tracker-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, Extension
 
 # Define the extension module for the C++ code
 cpp_extension = Extension('edstem.integration.storage', 
                           sources=['edstem/integration/storage/main.cpp'],
-                          include_dirs=['edstem/integration/storage']
+                          include_dirs=['.']
                           )
 
 setup(
     name='edstem-assignment-tracker',
-    version='1.0.4',
+    version='1.0.5',
     description='Edstem Assignment Tracker.',
     long_description='Edstem Assignment Tracker is a python package that allows you to easily track your assignments for the Edstem platform.',
     author='Trevor Moy',
     author_email='trevormoy14@uri.edu',
     url='https://github.com/SP24-212/Edstem-Tracker',
     packages=['edstem.integration'],
     include_package_data=True,
```
