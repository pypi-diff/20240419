# Comparing `tmp/pyarmor.cli.core-6.5.0.zip` & `tmp/pyarmor.cli.core-6.5.1.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 9001 bytes, number of entries: 16
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/
--rw-r--r--  2.0 unx     2647 b- defN 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/PKG-INFO
--rw-r--r--  2.0 unx     2033 b- defN 24-Feb-02 10:34 pyarmor.cli.core-6.5.0/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/setup.cfg
--rw-r--r--  2.0 unx     1548 b- defN 23-Jul-02 16:45 pyarmor.cli.core-6.5.0/README.rst
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor/cli/core/
--rw-r--r--  2.0 unx     4647 b- defN 24-Feb-02 09:50 pyarmor.cli.core-6.5.0/pyarmor/cli/core/__init__.py
--rw-r--r--  2.0 unx     1513 b- defN 23-Jun-06 07:58 pyarmor.cli.core-6.5.0/pyarmor/cli/core/features.py
--rw-r--r--  2.0 unx     2798 b- defN 23-Jun-08 15:05 pyarmor.cli.core-6.5.0/pyarmor/cli/core/runtime.py
--rw-r--r--  2.0 unx     2647 b- defN 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      265 b- defN 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-29 10:11 pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/dependency_links.txt
-16 files, 18145 bytes uncompressed, 6353 bytes compressed:  65.0%
+Zip file size: 8999 bytes, number of entries: 16
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/
+-rw-r--r--  2.0 unx     2647 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/PKG-INFO
+-rw-r--r--  2.0 unx     2033 b- defN 24-Apr-13 10:14 pyarmor.cli.core-6.5.1/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/setup.cfg
+-rw-r--r--  2.0 unx     1548 b- defN 23-Jul-02 16:45 pyarmor.cli.core-6.5.1/README.rst
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor/cli/core/
+-rw-r--r--  2.0 unx     4647 b- defN 24-Apr-13 10:14 pyarmor.cli.core-6.5.1/pyarmor/cli/core/__init__.py
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jun-06 07:58 pyarmor.cli.core-6.5.1/pyarmor/cli/core/features.py
+-rw-r--r--  2.0 unx     2798 b- defN 23-Jun-08 15:05 pyarmor.cli.core-6.5.1/pyarmor/cli/core/runtime.py
+-rw-r--r--  2.0 unx     2647 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      265 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/dependency_links.txt
+16 files, 18145 bytes uncompressed, 6351 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,49 +1,49 @@
-Filename: pyarmor.cli.core-6.5.0/
+Filename: pyarmor.cli.core-6.5.1/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor/
+Filename: pyarmor.cli.core-6.5.1/pyarmor/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/
+Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/PKG-INFO
+Filename: pyarmor.cli.core-6.5.1/PKG-INFO
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/setup.py
+Filename: pyarmor.cli.core-6.5.1/setup.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/setup.cfg
+Filename: pyarmor.cli.core-6.5.1/setup.cfg
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/README.rst
+Filename: pyarmor.cli.core-6.5.1/README.rst
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor/cli/
+Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor/cli/core/
+Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor/cli/core/__init__.py
+Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/__init__.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor/cli/core/features.py
+Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/features.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor/cli/core/runtime.py
+Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/runtime.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/PKG-INFO
+Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/SOURCES.txt
+Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/top_level.txt
+Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/dependency_links.txt
+Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor.cli.core-6.5.0/PKG-INFO` & `pyarmor.cli.core-6.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor.cli.core
-Version: 6.5.0
+Version: 6.5.1
 Summary: Provide extension module pytransform3 for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: pyarmo.cli.core
         ===============
```

## Comparing `pyarmor.cli.core-6.5.0/setup.py` & `pyarmor.cli.core-6.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from setuptools import setup
 
-__VERSION__ = '6.5.0'
+__VERSION__ = '6.5.1'
 
 with open('README.rst') as f:
     long_description = f.read()
 
 is_android = hasattr(sys, 'getandroidapilevel')
 is_freebsd = sys.platform.startswith(('freebsd', 'openbsd', 'isilon onefs'))
```

## Comparing `pyarmor.cli.core-6.5.0/README.rst` & `pyarmor.cli.core-6.5.1/README.rst`

 * *Files identical despite different names*

## Comparing `pyarmor.cli.core-6.5.0/pyarmor/cli/core/__init__.py` & `pyarmor.cli.core-6.5.1/pyarmor/cli/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  @File: pyarmor/core/__init__.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: Thu Jan 12 17:29:25 CST 2023
 #
 
-__VERSION__ = '6.5.0'
+__VERSION__ = '6.5.1'
 
 
 def format_platform():
     import platform
     import sys
     from struct import calcsize
```

## Comparing `pyarmor.cli.core-6.5.0/pyarmor/cli/core/features.py` & `pyarmor.cli.core-6.5.1/pyarmor/cli/core/features.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli.core-6.5.0/pyarmor/cli/core/runtime.py` & `pyarmor.cli.core-6.5.1/pyarmor/cli/core/runtime.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli.core-6.5.0/pyarmor.cli.core.egg-info/PKG-INFO` & `pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor.cli.core
-Version: 6.5.0
+Version: 6.5.1
 Summary: Provide extension module pytransform3 for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: pyarmo.cli.core
         ===============
```

