# Comparing `tmp/edstem_assignment_tracker-1.0.2.tar.gz` & `tmp/edstem_assignment_tracker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edstem_assignment_tracker-1.0.2.tar", last modified: Fri Apr 19 04:00:30 2024, max compression
+gzip compressed data, was "edstem_assignment_tracker-1.0.3.tar", last modified: Fri Apr 19 04:12:18 2024, max compression
```

## Comparing `edstem_assignment_tracker-1.0.2.tar` & `edstem_assignment_tracker-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:00:30.387684 edstem_assignment_tracker-1.0.2/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:00:30.387473 edstem_assignment_tracker-1.0.2/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.2/README.md
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:00:30.384290 edstem_assignment_tracker-1.0.2/edstem/
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:00:30.385876 edstem_assignment_tracker-1.0.2/edstem/integration/
--rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.2/edstem/integration/__init__.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.2/edstem/integration/get_data.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.2/edstem/integration/run_eat.py
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:00:30.386162 edstem_assignment_tracker-1.0.2/edstem/integration/storage/
--rw-r--r--   0 trevormoy   (501) staff       (20)    12149 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.2/edstem/integration/storage/main.cpp
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:00:30.387219 edstem_assignment_tracker-1.0.2/edstem_assignment_tracker.egg-info/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:00:30.000000 edstem_assignment_tracker-1.0.2/edstem_assignment_tracker.egg-info/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      390 2024-04-19 04:00:30.000000 edstem_assignment_tracker-1.0.2/edstem_assignment_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 04:00:30.000000 edstem_assignment_tracker-1.0.2/edstem_assignment_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 04:00:30.000000 edstem_assignment_tracker-1.0.2/edstem_assignment_tracker.egg-info/requires.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 04:00:30.000000 edstem_assignment_tracker-1.0.2/edstem_assignment_tracker.egg-info/top_level.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 04:00:30.387730 edstem_assignment_tracker-1.0.2/setup.cfg
--rw-r--r--   0 trevormoy   (501) staff       (20)     1197 2024-04-19 04:00:23.000000 edstem_assignment_tracker-1.0.2/setup.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:12:18.164141 edstem_assignment_tracker-1.0.3/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:12:18.163908 edstem_assignment_tracker-1.0.3/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.3/README.md
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:12:18.161236 edstem_assignment_tracker-1.0.3/edstem/
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:12:18.162585 edstem_assignment_tracker-1.0.3/edstem/integration/
+-rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.3/edstem/integration/__init__.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.3/edstem/integration/get_data.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.3/edstem/integration/run_eat.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:12:18.162719 edstem_assignment_tracker-1.0.3/edstem/integration/storage/
+-rw-r--r--   0 trevormoy   (501) staff       (20)    12090 2024-04-19 04:10:46.000000 edstem_assignment_tracker-1.0.3/edstem/integration/storage/main.cpp
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 04:12:18.163673 edstem_assignment_tracker-1.0.3/edstem_assignment_tracker.egg-info/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 04:12:18.000000 edstem_assignment_tracker-1.0.3/edstem_assignment_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      390 2024-04-19 04:12:18.000000 edstem_assignment_tracker-1.0.3/edstem_assignment_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 04:12:18.000000 edstem_assignment_tracker-1.0.3/edstem_assignment_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 04:12:18.000000 edstem_assignment_tracker-1.0.3/edstem_assignment_tracker.egg-info/requires.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 04:12:18.000000 edstem_assignment_tracker-1.0.3/edstem_assignment_tracker.egg-info/top_level.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 04:12:18.164194 edstem_assignment_tracker-1.0.3/setup.cfg
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1198 2024-04-19 04:11:54.000000 edstem_assignment_tracker-1.0.3/setup.py
```

### Comparing `edstem_assignment_tracker-1.0.2/PKG-INFO` & `edstem_assignment_tracker-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.2
+Version: 1.0.3
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.2/README.md` & `edstem_assignment_tracker-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.2/edstem/integration/get_data.py` & `edstem_assignment_tracker-1.0.3/edstem/integration/get_data.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.2/edstem/integration/run_eat.py` & `edstem_assignment_tracker-1.0.3/edstem/integration/run_eat.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.2/edstem/integration/storage/main.cpp` & `edstem_assignment_tracker-1.0.3/edstem/integration/storage/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #include <iostream>
 #include <fstream>
 #include <sstream>
 #include <string>
 #include <cstdlib>
-#include "bh.h"
-#include "bh.cpp"
 #include "avl.h"
-#include "node.cpp"
-#include "st.cpp"
-#include "avl.cpp"
+#include "st.h"
+#include "bh.h"
 
 void clearTerminal();
 
 int main(int argc, char* argv[]) {
 
     std::ifstream file("edstem/integration/edstem-data/data.txt");
```

### Comparing `edstem_assignment_tracker-1.0.2/edstem_assignment_tracker.egg-info/PKG-INFO` & `edstem_assignment_tracker-1.0.3/edstem_assignment_tracker.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.2
+Version: 1.0.3
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.2/setup.py` & `edstem_assignment_tracker-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, Extension
 
 # Define the extension module for the C++ code
 cpp_extension = Extension('edstem.integration.storage', 
-                          sources=['edstem/integration/storage/main.cpp'],
-                          include_dirs=['edstem/integration/storage'],
+                          sources=['edstem/integration/storage/main.cpp']
+                        #   include_dirs=['edstem/integration/storage'],
                         #   libraries=['your_cpp_library'],
                         #   library_dirs=['/path/to/cpp/libraries']
                           )
 
 setup(
     name='edstem-assignment-tracker',
-    version='1.0.2',
+    version='1.0.3',
     description='Edstem Assignment Tracker.',
     long_description='Edstem Assignment Tracker is a python package that allows you to easily track your assignments for the Edstem platform.',
     author='Trevor Moy',
     author_email='trevormoy14@uri.edu',
     url='https://github.com/SP24-212/Edstem-Tracker',
     packages=['edstem.integration'],
     ext_modules=[cpp_extension],  # Include the C++ extension module
```

