# Comparing `tmp/edstem_assignment_tracker-1.0.0.tar.gz` & `tmp/edstem_assignment_tracker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edstem_assignment_tracker-1.0.0.tar", last modified: Fri Apr 19 03:40:13 2024, max compression
+gzip compressed data, was "edstem_assignment_tracker-1.0.1.tar", last modified: Fri Apr 19 03:50:24 2024, max compression
```

## Comparing `edstem_assignment_tracker-1.0.0.tar` & `edstem_assignment_tracker-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:40:13.829956 edstem_assignment_tracker-1.0.0/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 03:40:13.829721 edstem_assignment_tracker-1.0.0/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.0/README.md
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:40:13.826467 edstem_assignment_tracker-1.0.0/edstem/
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:40:13.828148 edstem_assignment_tracker-1.0.0/edstem/integration/
--rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.0/edstem/integration/__init__.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.0/edstem/integration/get_data.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.0/edstem/integration/run_eat.py
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:40:13.828419 edstem_assignment_tracker-1.0.0/edstem/integration/storage/
--rw-r--r--   0 trevormoy   (501) staff       (20)    12149 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.0/edstem/integration/storage/main.cpp
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:40:13.829492 edstem_assignment_tracker-1.0.0/edstem_assignment_tracker.egg-info/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 03:40:13.000000 edstem_assignment_tracker-1.0.0/edstem_assignment_tracker.egg-info/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      390 2024-04-19 03:40:13.000000 edstem_assignment_tracker-1.0.0/edstem_assignment_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 03:40:13.000000 edstem_assignment_tracker-1.0.0/edstem_assignment_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 03:40:13.000000 edstem_assignment_tracker-1.0.0/edstem_assignment_tracker.egg-info/requires.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 03:40:13.000000 edstem_assignment_tracker-1.0.0/edstem_assignment_tracker.egg-info/top_level.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 03:40:13.830002 edstem_assignment_tracker-1.0.0/setup.cfg
--rw-r--r--   0 trevormoy   (501) staff       (20)     1197 2024-04-19 03:39:27.000000 edstem_assignment_tracker-1.0.0/setup.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:50:24.710761 edstem_assignment_tracker-1.0.1/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 03:50:24.710535 edstem_assignment_tracker-1.0.1/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.1/README.md
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:50:24.707477 edstem_assignment_tracker-1.0.1/edstem/
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:50:24.709063 edstem_assignment_tracker-1.0.1/edstem/integration/
+-rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.1/edstem/integration/__init__.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.1/edstem/integration/get_data.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.1/edstem/integration/run_eat.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:50:24.709344 edstem_assignment_tracker-1.0.1/edstem/integration/storage/
+-rw-r--r--   0 trevormoy   (501) staff       (20)    12149 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.1/edstem/integration/storage/main.cpp
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 03:50:24.710316 edstem_assignment_tracker-1.0.1/edstem_assignment_tracker.egg-info/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 03:50:24.000000 edstem_assignment_tracker-1.0.1/edstem_assignment_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      390 2024-04-19 03:50:24.000000 edstem_assignment_tracker-1.0.1/edstem_assignment_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 03:50:24.000000 edstem_assignment_tracker-1.0.1/edstem_assignment_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 03:50:24.000000 edstem_assignment_tracker-1.0.1/edstem_assignment_tracker.egg-info/requires.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 03:50:24.000000 edstem_assignment_tracker-1.0.1/edstem_assignment_tracker.egg-info/top_level.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 03:50:24.710809 edstem_assignment_tracker-1.0.1/setup.cfg
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1201 2024-04-19 03:49:55.000000 edstem_assignment_tracker-1.0.1/setup.py
```

### Comparing `edstem_assignment_tracker-1.0.0/PKG-INFO` & `edstem_assignment_tracker-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.0/README.md` & `edstem_assignment_tracker-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.0/edstem/integration/get_data.py` & `edstem_assignment_tracker-1.0.1/edstem/integration/get_data.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.0/edstem/integration/run_eat.py` & `edstem_assignment_tracker-1.0.1/edstem/integration/run_eat.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.0/edstem/integration/storage/main.cpp` & `edstem_assignment_tracker-1.0.1/edstem/integration/storage/main.cpp`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.0/edstem_assignment_tracker.egg-info/PKG-INFO` & `edstem_assignment_tracker-1.0.1/edstem_assignment_tracker.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.0/setup.py` & `edstem_assignment_tracker-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, Extension
 
 # Define the extension module for the C++ code
 cpp_extension = Extension('edstem.integration.storage', 
                           sources=['edstem/integration/storage/main.cpp'],
-                          include_dirs=['edstem/integration/storage'],
+                          include_dirs=['edstem/integration/storage/*.h'],
                         #   libraries=['your_cpp_library'],
                         #   library_dirs=['/path/to/cpp/libraries']
                           )
 
 setup(
     name='edstem-assignment-tracker',
-    version='1.0.0',
+    version='1.0.1',
     description='Edstem Assignment Tracker.',
     long_description='Edstem Assignment Tracker is a python package that allows you to easily track your assignments for the Edstem platform.',
     author='Trevor Moy',
     author_email='trevormoy14@uri.edu',
     url='https://github.com/SP24-212/Edstem-Tracker',
     packages=['edstem.integration'],
     ext_modules=[cpp_extension],  # Include the C++ extension module
```

