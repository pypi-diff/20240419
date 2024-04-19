# Comparing `tmp/sedeuce-1.0.8.tar.gz` & `tmp/sedeuce-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedeuce-1.0.8.tar", last modified: Sat Oct  7 03:26:47 2023, max compression
+gzip compressed data, was "sedeuce-1.0.9.tar", last modified: Fri Apr 19 01:35:31 2024, max compression
```

## Comparing `sedeuce-1.0.8.tar` & `sedeuce-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:26:47.033006 sedeuce-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-07 03:26:36.000000 sedeuce-1.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-07 03:26:36.000000 sedeuce-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2023-10-07 03:26:47.033006 sedeuce-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2023-10-07 03:26:36.000000 sedeuce-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-10-07 03:26:36.000000 sedeuce-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-07 03:26:47.033006 sedeuce-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2023-10-07 03:26:36.000000 sedeuce-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:26:47.029006 sedeuce-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:26:47.029006 sedeuce-1.0.8/src/sedeuce/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-10-07 03:26:36.000000 sedeuce-1.0.8/src/sedeuce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-10-07 03:26:36.000000 sedeuce-1.0.8/src/sedeuce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48646 2023-10-07 03:26:36.000000 sedeuce-1.0.8/src/sedeuce/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-10-07 03:26:36.000000 sedeuce-1.0.8/src/sedeuce/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2023-10-07 03:26:36.000000 sedeuce-1.0.8/src/sedeuce/sed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17837 2023-10-07 03:26:36.000000 sedeuce-1.0.8/src/sedeuce/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:26:47.033006 sedeuce-1.0.8/src/sedeuce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2023-10-07 03:26:46.000000 sedeuce-1.0.8/src/sedeuce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-10-07 03:26:46.000000 sedeuce-1.0.8/src/sedeuce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 03:26:46.000000 sedeuce-1.0.8/src/sedeuce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-07 03:26:46.000000 sedeuce-1.0.8/src/sedeuce.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-07 03:26:46.000000 sedeuce-1.0.8/src/sedeuce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-07 03:26:46.000000 sedeuce-1.0.8/src/sedeuce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:35:31.680465 sedeuce-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 01:35:24.000000 sedeuce-1.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 01:35:24.000000 sedeuce-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-19 01:35:31.680465 sedeuce-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-19 01:35:24.000000 sedeuce-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 01:35:24.000000 sedeuce-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 01:35:31.680465 sedeuce-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-19 01:35:24.000000 sedeuce-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:35:31.680465 sedeuce-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:35:31.680465 sedeuce-1.0.9/src/sedeuce/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-19 01:35:24.000000 sedeuce-1.0.9/src/sedeuce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-19 01:35:24.000000 sedeuce-1.0.9/src/sedeuce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48646 2024-04-19 01:35:24.000000 sedeuce-1.0.9/src/sedeuce/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-19 01:35:24.000000 sedeuce-1.0.9/src/sedeuce/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-04-19 01:35:24.000000 sedeuce-1.0.9/src/sedeuce/sed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-04-19 01:35:24.000000 sedeuce-1.0.9/src/sedeuce/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:35:31.680465 sedeuce-1.0.9/src/sedeuce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-19 01:35:31.000000 sedeuce-1.0.9/src/sedeuce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 01:35:31.000000 sedeuce-1.0.9/src/sedeuce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:35:31.000000 sedeuce-1.0.9/src/sedeuce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 01:35:31.000000 sedeuce-1.0.9/src/sedeuce.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 01:35:31.000000 sedeuce-1.0.9/src/sedeuce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 01:35:31.000000 sedeuce-1.0.9/src/sedeuce.egg-info/top_level.txt
```

### Comparing `sedeuce-1.0.8/LICENSE.md` & `sedeuce-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/PKG-INFO` & `sedeuce-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sedeuce
-Version: 1.0.8
+Version: 1.0.9
 Summary: A seductive sed clone in Python with both CLI and library interfaces
 Home-page: https://github.com/Tails86/sedeuce
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/sedeuce
 Project-URL: Bug Reports, https://github.com/Tails86/sedeuce/issues
 Project-URL: Source Code, https://github.com/Tails86/sedeuce
```

### Comparing `sedeuce-1.0.8/README.md` & `sedeuce-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/setup.py` & `sedeuce-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/src/sedeuce/__init__.py` & `sedeuce-1.0.9/src/sedeuce/__init__.py`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/src/sedeuce/__main__.py` & `sedeuce-1.0.9/src/sedeuce/__main__.py`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/src/sedeuce/commands.py` & `sedeuce-1.0.9/src/sedeuce/commands.py`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/src/sedeuce/conditions.py` & `sedeuce-1.0.9/src/sedeuce/conditions.py`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/src/sedeuce/sed.py` & `sedeuce-1.0.9/src/sedeuce/sed.py`

 * *Files identical despite different names*

### Comparing `sedeuce-1.0.8/src/sedeuce/utils.py` & `sedeuce-1.0.9/src/sedeuce/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 import os
 import sys
 import threading
 from typing import Any, Union, List
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 PACKAGE_NAME = 'sedeuce'
 
 VERSION_PARTS = [int(i) for i in __version__.split('.')]
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 # sed syntax
```

### Comparing `sedeuce-1.0.8/src/sedeuce.egg-info/PKG-INFO` & `sedeuce-1.0.9/src/sedeuce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sedeuce
-Version: 1.0.8
+Version: 1.0.9
 Summary: A seductive sed clone in Python with both CLI and library interfaces
 Home-page: https://github.com/Tails86/sedeuce
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/sedeuce
 Project-URL: Bug Reports, https://github.com/Tails86/sedeuce/issues
 Project-URL: Source Code, https://github.com/Tails86/sedeuce
```

