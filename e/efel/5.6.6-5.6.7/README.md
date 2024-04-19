# Comparing `tmp/efel-5.6.6.tar.gz` & `tmp/efel-5.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-5.6.6.tar", last modified: Tue Apr  9 12:32:59 2024, max compression
+gzip compressed data, was "efel-5.6.7.tar", last modified: Fri Apr 19 14:30:25 2024, max compression
```

## Comparing `efel-5.6.6.tar` & `efel-5.6.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:32:59.246397 efel-5.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 12:32:57.000000 efel-5.6.6/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-09 12:32:57.000000 efel-5.6.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-09 12:32:57.000000 efel-5.6.6/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-09 12:32:57.000000 efel-5.6.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-09 12:32:57.000000 efel-5.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-09 12:32:59.246397 efel-5.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-09 12:32:57.000000 efel-5.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:32:59.242397 efel-5.6.6/efel/
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-09 12:32:57.000000 efel-5.6.6/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-09 12:32:57.000000 efel-5.6.6/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 12:32:59.246397 efel-5.6.6/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-04-09 12:32:57.000000 efel-5.6.6/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:32:59.246397 efel-5.6.6/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/EfelExceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (127)    92113 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 12:32:57.000000 efel-5.6.6/efel/cppcore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-09 12:32:57.000000 efel-5.6.6/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:32:59.246397 efel-5.6.6/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-09 12:32:57.000000 efel-5.6.6/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-09 12:32:57.000000 efel-5.6.6/efel/pyfeatures/cppfeature_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-09 12:32:57.000000 efel-5.6.6/efel/pyfeatures/isi.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-09 12:32:57.000000 efel-5.6.6/efel/pyfeatures/multitrace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-09 12:32:57.000000 efel-5.6.6/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 12:32:57.000000 efel-5.6.6/efel/pyfeatures/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 12:32:57.000000 efel-5.6.6/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:32:59.246397 efel-5.6.6/efel/units/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 12:32:57.000000 efel-5.6.6/efel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-09 12:32:57.000000 efel-5.6.6/efel/units/units.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:32:59.242397 efel-5.6.6/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-09 12:32:59.000000 efel-5.6.6/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-09 12:32:59.000000 efel-5.6.6/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:32:59.000000 efel-5.6.6/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 12:32:59.000000 efel-5.6.6/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 12:32:59.000000 efel-5.6.6/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 12:32:57.000000 efel-5.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-09 12:32:59.246397 efel-5.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-09 12:32:57.000000 efel-5.6.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-09 12:32:57.000000 efel-5.6.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:30:25.639157 efel-5.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 14:30:23.000000 efel-5.6.7/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-19 14:30:23.000000 efel-5.6.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-19 14:30:23.000000 efel-5.6.7/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-19 14:30:23.000000 efel-5.6.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-19 14:30:23.000000 efel-5.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-19 14:30:25.639157 efel-5.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-19 14:30:23.000000 efel-5.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:30:25.631157 efel-5.6.7/efel/
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-19 14:30:23.000000 efel-5.6.7/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-19 14:30:23.000000 efel-5.6.7/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 14:30:25.639157 efel-5.6.7/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-19 14:30:23.000000 efel-5.6.7/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:30:25.635157 efel-5.6.7/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/EfelExceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92113 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 14:30:23.000000 efel-5.6.7/efel/cppcore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-19 14:30:23.000000 efel-5.6.7/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:30:25.635157 efel-5.6.7/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-19 14:30:23.000000 efel-5.6.7/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 14:30:23.000000 efel-5.6.7/efel/pyfeatures/cppfeature_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-19 14:30:23.000000 efel-5.6.7/efel/pyfeatures/isi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-19 14:30:23.000000 efel-5.6.7/efel/pyfeatures/multitrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-19 14:30:23.000000 efel-5.6.7/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-19 14:30:23.000000 efel-5.6.7/efel/pyfeatures/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 14:30:23.000000 efel-5.6.7/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:30:25.639157 efel-5.6.7/efel/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 14:30:23.000000 efel-5.6.7/efel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-19 14:30:23.000000 efel-5.6.7/efel/units/units.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:30:25.631157 efel-5.6.7/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-19 14:30:25.000000 efel-5.6.7/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 14:30:25.000000 efel-5.6.7/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:30:25.000000 efel-5.6.7/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 14:30:25.000000 efel-5.6.7/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 14:30:25.000000 efel-5.6.7/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 14:30:24.000000 efel-5.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 14:30:25.639157 efel-5.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-19 14:30:24.000000 efel-5.6.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-19 14:30:24.000000 efel-5.6.7/versioneer.py
```

### Comparing `efel-5.6.6/COPYING` & `efel-5.6.7/COPYING`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/COPYING.less` & `efel-5.6.7/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/LICENSE.txt` & `efel-5.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/PKG-INFO` & `efel-5.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 5.6.6
+Version: 5.6.7
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
@@ -177,18 +177,18 @@
 ```python
 import efel
 ```
 
 To get a list with all the available feature names
 
 ```python
-efel.getFeatureNames()
+efel.get_feature_names()
 ```
 
-The python function to extract features is getFeatureValues(...).
+The python function to extract features is get_feature_values(...).
 Below is a short example on how to use this function. The code and example
 trace are available
 [here](https://github.com/BlueBrain/eFEL/blob/master/examples/basic/basic_example1.py)
 
 ```python
 """Basic example 1 for eFEL"""
 
@@ -228,15 +228,15 @@
 
     # Multiple traces can be passed to the eFEL at the same time, so the
     # argument should be a list
     traces = [trace1]
 
     # Now we pass 'traces' to the efel and ask it to calculate the feature
     # values
-    traces_results = efel.getFeatureValues(traces,
+    traces_results = efel.get_feature_values(traces,
                                            ['AP_amplitude', 'voltage_base'])
 
     # The return value is a list of trace_results, every trace_results
     # corresponds to one trace in the 'traces' list above (in same order)
     for trace_results in traces_results:
         # trace_result is a dictionary, with as keys the requested features
         for feature_name, feature_values in trace_results.items():
```

### Comparing `efel-5.6.6/README.md` & `efel-5.6.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -152,18 +152,18 @@
 ```python
 import efel
 ```
 
 To get a list with all the available feature names
 
 ```python
-efel.getFeatureNames()
+efel.get_feature_names()
 ```
 
-The python function to extract features is getFeatureValues(...).
+The python function to extract features is get_feature_values(...).
 Below is a short example on how to use this function. The code and example
 trace are available
 [here](https://github.com/BlueBrain/eFEL/blob/master/examples/basic/basic_example1.py)
 
 ```python
 """Basic example 1 for eFEL"""
 
@@ -203,15 +203,15 @@
 
     # Multiple traces can be passed to the eFEL at the same time, so the
     # argument should be a list
     traces = [trace1]
 
     # Now we pass 'traces' to the efel and ask it to calculate the feature
     # values
-    traces_results = efel.getFeatureValues(traces,
+    traces_results = efel.get_feature_values(traces,
                                            ['AP_amplitude', 'voltage_base'])
 
     # The return value is a list of trace_results, every trace_results
     # corresponds to one trace in the 'traces' list above (in same order)
     for trace_results in traces_results:
         # trace_result is a dictionary, with as keys the requested features
         for feature_name, feature_values in trace_results.items():
```

### Comparing `efel-5.6.6/efel/DependencyV5.txt` & `efel-5.6.7/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/__init__.py` & `efel-5.6.7/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/api.py` & `efel-5.6.7/efel/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  along with this library; if not, write to the Free Software Foundation, Inc.,
  51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 # pylint: disable=W0602,W0603,W0702, F0401, W0612, R0912
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Callable
+from typing import Callable, Iterator, Literal, overload
 from typing_extensions import deprecated
 import numpy as np
 
 import efel
 import efel.cppcore as cppcore
 
 import efel.pyfeatures as pyfeatures
@@ -85,36 +85,35 @@
     set_double_setting("sahp_start", 5.0)
     set_int_setting("ignore_first_ISI", 1)
     set_double_setting("impedance_max_freq", 50.0)
 
     _initialise()
 
 
-@deprecated("Changing the dependency file will not be supported in the future.")
-def setDependencyFileLocation(location: str | Path) -> None:
+def set_dependency_file_location(location: str | Path) -> None:
     """Sets the location of the Dependency file.
 
     eFEL uses 'Dependency' files to let the user define versions of features to use.
     The installation directory of eFEL contains a default 'DependencyV5.txt' file.
     Unless users want to change this file, it is not necessary to call this function.
+    Modifying the Dependency file can be useful in debugging.
 
     Args:
         location: Path to the location of a Dependency file.
 
     Raises:
         FileNotFoundError: If the path to the dependency file doesn't exist.
     """
     location = Path(location)
     if not location.exists():
         raise FileNotFoundError(f"Path to dependency file {location} doesn't exist")
     _settings.dependencyfile_path = str(location)
 
 
-@deprecated("Changing the dependency file will not be supported in the future.")
-def getDependencyFileLocation() -> str:
+def get_dependency_file_location() -> str:
     """Gets the location of the Dependency file.
 
     Returns:
         Path to the location of a Dependency file.
     """
     return _settings.dependencyfile_path
 
@@ -126,38 +125,28 @@
         new_threshold: The new spike detection threshold value (in the same units
                        as the traces, e.g. mV).
     """
     _settings.threshold = new_threshold
     set_double_setting('Threshold', _settings.threshold)
 
 
-@deprecated("Use set_threshold instead")
-def setThreshold(newThreshold: float) -> None:
-    set_threshold(newThreshold)
-
-
 def set_derivative_threshold(new_derivative_threshold: float) -> None:
     """Set the threshold for the derivative for detecting the spike onset.
 
     Some features use a threshold on dV/dt to calculate the beginning of an
     action potential. This function allows you to set this threshold.
 
     Args:
         new_derivative_threshold: The new derivative threshold value (in the same units
                                   as the traces, e.g. mV/ms).
     """
     _settings.derivative_threshold = new_derivative_threshold
     set_double_setting('DerivativeThreshold', _settings.derivative_threshold)
 
 
-@deprecated("Use set_derivative_threshold instead")
-def setDerivativeThreshold(newDerivativeThreshold: float) -> None:
-    set_derivative_threshold(newDerivativeThreshold)
-
-
 def get_feature_names() -> list[str]:
     """Return a list with the name of all the available features
 
     Returns:
         A list that contains all the feature names available in
         the eFEL. These names can be used in the feature_names
         argument of e.g. get_feature_values()
@@ -167,29 +156,19 @@
     cppcore.getFeatureNames(feature_names)
 
     feature_names += pyfeatures.all_pyfeatures
 
     return feature_names
 
 
-@deprecated("Use get_feature_names instead")
-def getFeatureNames() -> list[str]:
-    return get_feature_names()
-
-
 def feature_name_exists(feature_name: str) -> bool:
     """Returns True if the feature name exists in eFEL, False otherwise."""
     return feature_name in get_feature_names()
 
 
-@deprecated("Use feature_name_exists instead")
-def FeatureNameExists(feature_name: str) -> bool:
-    return feature_name_exists(feature_name)
-
-
 def _get_feature(feature_name: str, raise_warnings=False) -> np.ndarray | None:
     """Get feature value, decide to use python or cpp"""
     if feature_name in pyfeatures.all_pyfeatures:
         return get_py_feature(feature_name)
     else:
         return get_cpp_feature(feature_name, raise_warnings=raise_warnings)
 
@@ -250,25 +229,14 @@
         # Check for NaN
         if distance != distance:
             return error_dist
 
         return distance
 
 
-@deprecated("Use get_distance instead")
-def getDistance(
-        trace,
-        featureName,
-        mean,
-        std,
-        trace_check=True,
-        error_dist=250) -> float:
-    return get_distance(trace, featureName, mean, std, trace_check, error_dist)
-
-
 def _initialise() -> None:
     """Set cppcore initial values."""
     cppcore.Initialize(_settings.dependencyfile_path, "log")
     # flush the GErrorString from previous runs by calling getgError()
     cppcore.getgError()
 
     # First set some settings that are used by the feature extraction
@@ -287,45 +255,53 @@
 
 
 def set_int_setting(setting_name: str, new_value: int) -> None:
     """Set a certain integer setting to a new value"""
     _int_settings[setting_name] = new_value
 
 
-@deprecated("Use set_int_setting instead")
-def setIntSetting(setting_name: str, new_value: int) -> None:
-    set_int_setting(setting_name, new_value)
-
-
 def set_double_setting(setting_name: str, new_value: float) -> None:
     """Set a certain double setting to a new value"""
     _double_settings[setting_name] = new_value
 
 
-@deprecated("Use set_double_setting instead")
-def setDoubleSetting(setting_name: str, new_value: float) -> None:
-    set_double_setting(setting_name, new_value)
-
-
 def set_str_setting(setting_name: str, new_value: str) -> None:
     """Set a certain string setting to a new value"""
     _string_settings[setting_name] = new_value
 
 
-@deprecated("Use set_str_setting instead")
-def setStrSetting(setting_name: str, new_value: str) -> None:
-    set_str_setting(setting_name, new_value)
+@overload
+def get_feature_values(
+    traces: list[dict],
+    feature_names: list[str],
+    parallel_map: Callable | None,
+    return_list: Literal[True],
+    raise_warnings: bool = True,
+) -> list:
+    ...
 
 
+@overload
 def get_feature_values(
-        traces: list[dict],
-        feature_names: list[str],
-        parallel_map: Callable | None = None,
-        return_list: bool = True,
-        raise_warnings: bool = True) -> list | map:
+    traces: list[dict],
+    feature_names: list[str],
+    parallel_map: Callable | None,
+    return_list: Literal[False],
+    raise_warnings: bool = True,
+) -> Iterator:
+    ...
+
+
+def get_feature_values(
+    traces: list[dict],
+    feature_names: list[str],
+    parallel_map: Callable | None = None,
+    return_list: bool = True,
+    raise_warnings: bool = True,
+) -> list | Iterator:
     """Calculate feature values for a list of traces.
 
     This function is the core of eFEL API. A list of traces (in the form
     of dictionaries) is passed as argument, together with a list of feature
     names.
 
     The return value consists of a list of dictionaries, one for each input
@@ -355,36 +331,23 @@
         The value is None if an error occured during the
         calculation of the feature.
     """
 
     if parallel_map is None:
         parallel_map = map
 
-    traces_featurenames = (
-        (trace, feature_names, raise_warnings)
-        for trace in traces)
+    traces_featurenames = ((trace, feature_names, raise_warnings) for trace in traces)
     map_result = parallel_map(_get_feature_values_serial, traces_featurenames)
 
     if return_list:
         return list(map_result)
     else:
         return map_result
 
 
-@deprecated("Use get_feature_values instead")
-def getFeatureValues(
-        traces,
-        featureNames,
-        parallel_map=None,
-        return_list=True,
-        raise_warnings=True):
-    return get_feature_values(
-        traces, featureNames, parallel_map, return_list, raise_warnings)
-
-
 def get_py_feature(feature_name: str) -> np.ndarray | None:
     """Return values of the given feature name."""
     return getattr(pyfeatures, feature_name)()
 
 
 def _get_feature_values_serial(
     trace_featurenames: tuple[dict, list[str], bool]
@@ -453,27 +416,97 @@
         The value is None if an error occured during the
         calculation of the feature, or if the feature value array
         was empty.
     """
     featureDicts = get_feature_values(
         traces,
         feature_names,
+        parallel_map=None,
+        return_list=True,
         raise_warnings=raise_warnings)
     for featureDict in featureDicts:  # type: ignore
         for (key, values) in list(featureDict.items()):
             if values is None or len(values) == 0:
                 featureDict[key] = None
             else:
                 featureDict[key] = np.mean(values)
 
     return featureDicts  # type: ignore
 
 
+reset()
+
+
+# Deprecated functions
+@deprecated("Use set_threshold instead")
+def setThreshold(newThreshold: float) -> None:
+    set_threshold(newThreshold)
+
+
+@deprecated("Use set_derivative_threshold instead")
+def setDerivativeThreshold(newDerivativeThreshold: float) -> None:
+    set_derivative_threshold(newDerivativeThreshold)
+
+
+@deprecated("Use get_feature_names instead")
+def getFeatureNames() -> list[str]:
+    return get_feature_names()
+
+
+@deprecated("Use feature_name_exists instead")
+def FeatureNameExists(feature_name: str) -> bool:
+    return feature_name_exists(feature_name)
+
+
+@deprecated("Use get_distance instead")
+def getDistance(
+        trace,
+        featureName,
+        mean,
+        std,
+        trace_check=True,
+        error_dist=250) -> float:
+    return get_distance(trace, featureName, mean, std, trace_check, error_dist)
+
+
+@deprecated("Use set_int_setting instead")
+def setIntSetting(setting_name: str, new_value: int) -> None:
+    set_int_setting(setting_name, new_value)
+
+
+@deprecated("Use set_double_setting instead")
+def setDoubleSetting(setting_name: str, new_value: float) -> None:
+    set_double_setting(setting_name, new_value)
+
+
+@deprecated("Use set_str_setting instead")
+def setStrSetting(setting_name: str, new_value: str) -> None:
+    set_str_setting(setting_name, new_value)
+
+
+@deprecated("Use get_feature_values instead")
+def getFeatureValues(
+        traces,
+        featureNames,
+        parallel_map=None,
+        return_list=True,
+        raise_warnings=True):
+    return get_feature_values(
+        traces, featureNames, parallel_map, return_list, raise_warnings)
+
+
 @deprecated("Use get_mean_feature_values instead")
 def getMeanFeatureValues(
         traces,
         featureNames,
         raise_warnings=True):
     return get_mean_feature_values(traces, featureNames, raise_warnings)
 
 
-reset()
+@deprecated("Use get_dependency_file_location instead")
+def getDependencyFileLocation() -> str:
+    return get_dependency_file_location()
+
+
+@deprecated("Use set_dependency_file_location instead")
+def setDependencyFileLocation(location: str | Path) -> None:
+    return set_dependency_file_location(location)
```

### Comparing `efel-5.6.6/efel/cppcore/DependencyTree.cpp` & `efel-5.6.7/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/DependencyTree.h` & `efel-5.6.7/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/EfelExceptions.h` & `efel-5.6.7/efel/cppcore/EfelExceptions.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/FillFptrTable.cpp` & `efel-5.6.7/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/FillFptrTable.h` & `efel-5.6.7/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/Global.h` & `efel-5.6.7/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV1.cpp` & `efel-5.6.7/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV1.h` & `efel-5.6.7/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV2.cpp` & `efel-5.6.7/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV2.h` & `efel-5.6.7/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV3.cpp` & `efel-5.6.7/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV3.h` & `efel-5.6.7/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV5.cpp` & `efel-5.6.7/efel/cppcore/LibV5.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/LibV5.h` & `efel-5.6.7/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/Utils.cpp` & `efel-5.6.7/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/Utils.h` & `efel-5.6.7/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/cfeature.cpp` & `efel-5.6.7/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/cfeature.h` & `efel-5.6.7/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/cppcore.cpp` & `efel-5.6.7/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/eFELLogger.h` & `efel-5.6.7/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/mapoperations.cpp` & `efel-5.6.7/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/mapoperations.h` & `efel-5.6.7/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore/types.h` & `efel-5.6.7/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/cppcore.pyi` & `efel-5.6.7/efel/cppcore.pyi`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/io.py` & `efel-5.6.7/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/pyfeatures/__init__.py` & `efel-5.6.7/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/pyfeatures/cppfeature_access.py` & `efel-5.6.7/efel/pyfeatures/cppfeature_access.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/pyfeatures/isi.py` & `efel-5.6.7/efel/pyfeatures/isi.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/pyfeatures/multitrace.py` & `efel-5.6.7/efel/pyfeatures/multitrace.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
     Backpropagating action potential is the action potential that is initiated
     in the soma and propagates to the dendrite. The attenuation is the ratio
     of the amplitude of the action potential in the soma and the dendrite.
     The attenuation is computed by first subtracting the resting potential
     from the voltage traces.
     """
-    f_values = efel.getFeatureValues([soma_trace, dendrite_trace], ["voltage_base"])
+    f_values = efel.get_feature_values(
+        [soma_trace, dendrite_trace], ["voltage_base"],
+        parallel_map=None, return_list=True, raise_warnings=True)
     vb_soma = f_values[0]["voltage_base"][0]
     vb_dend = f_values[1]["voltage_base"][0]
     v_soma = soma_trace["V"]
     v_dend = dendrite_trace["V"]
     res = (np.max(v_soma) - vb_soma) / (np.max(v_dend) - vb_dend)
     return res
```

### Comparing `efel-5.6.6/efel/pyfeatures/pyfeatures.py` & `efel-5.6.7/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel/pyfeatures/validation.py` & `efel-5.6.7/efel/pyfeatures/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Contains scientific validation methods on input signals."""
 import efel
 
 
 def check_ais_initiation(soma_trace: dict, ais_trace: dict) -> bool:
     """Checks the initiation of action potential in AIS with respect to soma."""
-    f_values = efel.getFeatureValues([soma_trace, ais_trace], ["AP_begin_time"])
+    f_values = efel.get_feature_values(
+        traces=[soma_trace, ais_trace], feature_names=["AP_begin_time"],
+        parallel_map=None, return_list=True, raise_warnings=True
+    )
     soma_ap_begin_time = f_values[0]["AP_begin_time"]
     ais_ap_begin_time = f_values[1]["AP_begin_time"]
 
     if soma_ap_begin_time is None or ais_ap_begin_time is None:
         raise ValueError("AP_begin_time feature is not computed")
 
     if len(soma_ap_begin_time) != len(ais_ap_begin_time):
```

### Comparing `efel-5.6.6/efel/units/units.json` & `efel-5.6.7/efel/units/units.json`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/efel.egg-info/PKG-INFO` & `efel-5.6.7/efel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 5.6.6
+Version: 5.6.7
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
@@ -177,18 +177,18 @@
 ```python
 import efel
 ```
 
 To get a list with all the available feature names
 
 ```python
-efel.getFeatureNames()
+efel.get_feature_names()
 ```
 
-The python function to extract features is getFeatureValues(...).
+The python function to extract features is get_feature_values(...).
 Below is a short example on how to use this function. The code and example
 trace are available
 [here](https://github.com/BlueBrain/eFEL/blob/master/examples/basic/basic_example1.py)
 
 ```python
 """Basic example 1 for eFEL"""
 
@@ -228,15 +228,15 @@
 
     # Multiple traces can be passed to the eFEL at the same time, so the
     # argument should be a list
     traces = [trace1]
 
     # Now we pass 'traces' to the efel and ask it to calculate the feature
     # values
-    traces_results = efel.getFeatureValues(traces,
+    traces_results = efel.get_feature_values(traces,
                                            ['AP_amplitude', 'voltage_base'])
 
     # The return value is a list of trace_results, every trace_results
     # corresponds to one trace in the 'traces' list above (in same order)
     for trace_results in traces_results:
         # trace_result is a dictionary, with as keys the requested features
         for feature_name, feature_values in trace_results.items():
```

### Comparing `efel-5.6.6/efel.egg-info/SOURCES.txt` & `efel-5.6.7/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/setup.py` & `efel-5.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.6/versioneer.py` & `efel-5.6.7/versioneer.py`

 * *Files identical despite different names*

