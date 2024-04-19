# Comparing `tmp/edstem_assignment_tracker-1.0.6.tar.gz` & `tmp/edstem_assignment_tracker-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edstem_assignment_tracker-1.0.6.tar", last modified: Fri Apr 19 05:10:53 2024, max compression
+gzip compressed data, was "edstem_assignment_tracker-1.0.7.tar", last modified: Fri Apr 19 15:21:02 2024, max compression
```

## Comparing `edstem_assignment_tracker-1.0.6.tar` & `edstem_assignment_tracker-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 05:10:53.346053 edstem_assignment_tracker-1.0.6/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 05:10:53.345836 edstem_assignment_tracker-1.0.6/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.6/README.md
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 05:10:53.342253 edstem_assignment_tracker-1.0.6/edstem/
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 05:10:53.343421 edstem_assignment_tracker-1.0.6/edstem/integration/
--rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.6/edstem/integration/__init__.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.6/edstem/integration/get_data.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.6/edstem/integration/run_eat.py
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 05:10:53.344715 edstem_assignment_tracker-1.0.6/edstem/integration/storage/
--rw-r--r--   0 trevormoy   (501) staff       (20)    16744 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.6/edstem/integration/storage/avl.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)    11872 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.6/edstem/integration/storage/bh.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)    12090 2024-04-19 04:10:46.000000 edstem_assignment_tracker-1.0.6/edstem/integration/storage/main.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)      309 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.6/edstem/integration/storage/node.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)     5586 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.6/edstem/integration/storage/st.cpp
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 05:10:53.345641 edstem_assignment_tracker-1.0.6/edstem_assignment_tracker.egg-info/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 05:10:53.000000 edstem_assignment_tracker-1.0.6/edstem_assignment_tracker.egg-info/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      529 2024-04-19 05:10:53.000000 edstem_assignment_tracker-1.0.6/edstem_assignment_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 05:10:53.000000 edstem_assignment_tracker-1.0.6/edstem_assignment_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 05:10:53.000000 edstem_assignment_tracker-1.0.6/edstem_assignment_tracker.egg-info/requires.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 05:10:53.000000 edstem_assignment_tracker-1.0.6/edstem_assignment_tracker.egg-info/top_level.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 05:10:53.346102 edstem_assignment_tracker-1.0.6/setup.cfg
--rw-r--r--   0 trevormoy   (501) staff       (20)     1428 2024-04-19 05:10:31.000000 edstem_assignment_tracker-1.0.6/setup.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:21:02.302950 edstem_assignment_tracker-1.0.7/
+-rw-r--r--   0 trevormoy   (501) staff       (20)       48 2024-04-19 04:25:47.000000 edstem_assignment_tracker-1.0.7/MANIFEST.in
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 15:21:02.302708 edstem_assignment_tracker-1.0.7/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.7/README.md
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:21:02.297017 edstem_assignment_tracker-1.0.7/edstem/
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:21:02.298494 edstem_assignment_tracker-1.0.7/edstem/integration/
+-rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.7/edstem/integration/__init__.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.7/edstem/integration/get_data.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1205 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.7/edstem/integration/run_eat.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:21:02.301463 edstem_assignment_tracker-1.0.7/edstem/integration/storage/
+-rw-r--r--   0 trevormoy   (501) staff       (20)    16961 2024-04-19 14:58:57.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/avl.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     2982 2024-04-19 12:28:10.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/avl.h
+-rw-r--r--   0 trevormoy   (501) staff       (20)    12157 2024-04-19 14:56:45.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/bh.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1738 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/bh.h
+-rw-r--r--   0 trevormoy   (501) staff       (20)    12183 2024-04-19 13:48:06.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/main.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)      309 2024-04-19 12:27:38.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/node.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1286 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/node.h
+-rw-r--r--   0 trevormoy   (501) staff       (20)     5586 2024-04-19 12:27:37.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/st.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1549 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.7/edstem/integration/storage/st.h
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:21:02.302476 edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 15:21:02.000000 edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      724 2024-04-19 15:21:02.000000 edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 15:21:02.000000 edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       58 2024-04-19 15:21:02.000000 edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 15:21:02.000000 edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/requires.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 15:21:02.000000 edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/top_level.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 15:21:02.303001 edstem_assignment_tracker-1.0.7/setup.cfg
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1371 2024-04-19 15:20:27.000000 edstem_assignment_tracker-1.0.7/setup.py
```

### Comparing `edstem_assignment_tracker-1.0.6/PKG-INFO` & `edstem_assignment_tracker-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.6
+Version: 1.0.7
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.6/README.md` & `edstem_assignment_tracker-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.6/edstem/integration/get_data.py` & `edstem_assignment_tracker-1.0.7/edstem/integration/get_data.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.6/edstem/integration/run_eat.py` & `edstem_assignment_tracker-1.0.7/edstem/integration/run_eat.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.6/edstem/integration/storage/avl.cpp` & `edstem_assignment_tracker-1.0.7/edstem/integration/storage/avl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -364,16 +364,21 @@
 }
 
 void AVLTree::printTitle(EATNode* node, int i){
     std::cout << RED << "Title: " << RESET << node->data.second.first[i] << " ";
     return;
 }
 
-void AVLTree::printStatus(EATNode* node, int i){
-    std::cout << RED << "Status: " << RESET << node->data.second.first[i] << " ";
+void AVLTree::printStatus(EATNode* node, int i) {
+    if (node->data.second.first[i] == "attempted") {
+        std::cout << RED << "Status: " << RESET << node->data.second.first[i] << " ";
+    } 
+    else if (node->data.second.first[i] == "unattempted") {
+        std::cout << RED << "Status: " << RESET << node->data.second.first[i] << " ";
+    }
     return;
 }
 
 void AVLTree::printUserScore(EATNode* node, int i){
     std::cout << RED << "User Score: " << RESET << node->data.second.first[i] << " ";
     return;
 }
```

### Comparing `edstem_assignment_tracker-1.0.6/edstem/integration/storage/bh.cpp` & `edstem_assignment_tracker-1.0.7/edstem/integration/storage/bh.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -228,25 +228,28 @@
 
 void BinaryHeap::printTitle(int i, int j){
     std::cout << RED << "Title: " << RESET << heap[i]->data.second.first[j] << " ";
     return;
 }
 
 void BinaryHeap::printStatus(int i, int j){
-    std::cout << RED << "Status: " << RESET << heap[i]->data.second.first[j] << " ";
+    // just to avoid possibly printing the user's score  if the status is a stoi we need to skip
+    if (heap[i]->data.second.first[j] == "unattempted" || heap[i]->data.second.first[j] == "attempted") {
+        std::cout << RED << "Status: " << RESET << heap[i]->data.second.first[j] << " ";
+    }
     return;
 }
 
 void BinaryHeap::printUserScore(int i, int j){
-    std::cout << RED << "User Score: " << RESET << heap[i]->data.second.first[j] << " ";
+    std::cout << RED << "User Score: " << RESET << heap[i]->data.second.first[heap[i]->data.second.first.size() -3]  << " ";
     return;
 }
 
 void BinaryHeap::printPotentialScore(int i, int j){
-    std::cout << RED << "Potential Score: " << RESET << heap[i]->data.second.first[j] << " ";
+    std::cout << RED << "Potential Score: " << RESET << heap[i]->data.second.first[heap[i]->data.second.first.size() -2]  << " ";
     return;
 }
 
 // function to print 1 of every lesson type
 void BinaryHeap::printAllTypes() {
     // we are only going to print 1 of each lesson type (i.e. cpp, python, java, etc.)
```

### Comparing `edstem_assignment_tracker-1.0.6/edstem/integration/storage/main.cpp` & `edstem_assignment_tracker-1.0.7/edstem/integration/storage/main.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 #include <iostream>
 #include <fstream>
 #include <sstream>
 #include <string>
 #include <cstdlib>
+#include "avl.cpp"
+#include "bh.cpp"
+#include "st.cpp"
+#include "node.cpp"
+#include "node.h"
 #include "avl.h"
 #include "st.h"
 #include "bh.h"
 
 void clearTerminal();
 
 int main(int argc, char* argv[]) {
```

### Comparing `edstem_assignment_tracker-1.0.6/edstem/integration/storage/st.cpp` & `edstem_assignment_tracker-1.0.7/edstem/integration/storage/st.cpp`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.6/edstem_assignment_tracker.egg-info/PKG-INFO` & `edstem_assignment_tracker-1.0.7/edstem_assignment_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.6
+Version: 1.0.7
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.6/setup.py` & `edstem_assignment_tracker-1.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, Extension
 
 # Define the extension module for the C++ code
 cpp_extension = Extension('edstem.integration.storage', 
-                          sources=['edstem/integration/storage/main.cpp',
-                                   'edstem/integration/storage/st.cpp',
-                                   'edstem/integration/storage/bh.cpp',
-                                    'edstem/integration/storage/avl.cpp',
-                                    'edstem/integration/storage/node.cpp'
-                                   ],
-                          include_dirs=['edstem/integration/storage']
+                        sources=['edstem/integration/storage/main.cpp'],
+                        include_dirs=['edstem/integration/storage/'],
+                        language='c++',
+                        extra_compile_args=['-std=c++11']
                           )
 
 setup(
     name='edstem-assignment-tracker',
-    version='1.0.6',
+    version='1.0.7',
     description='Edstem Assignment Tracker.',
     long_description='Edstem Assignment Tracker is a python package that allows you to easily track your assignments for the Edstem platform.',
     author='Trevor Moy',
     author_email='trevormoy14@uri.edu',
     url='https://github.com/SP24-212/Edstem-Tracker',
     packages=['edstem.integration'],
+    package_data={'edstem.integration.storage': ['*.h']},
     include_package_data=True,
     ext_modules=[cpp_extension],  # Include the C++ extension module
     install_requires=['edapiwl==0.0.3',
                        'colorama'],  # Python dependencies
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+    entry_points={
+        'console_scripts': [
+            'ed-tracker = edstem.integration:run_eat'
+        ]
+    }
 )
```

