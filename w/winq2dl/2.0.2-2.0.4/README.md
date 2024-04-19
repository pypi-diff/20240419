# Comparing `tmp/winq2dl-2.0.2.tar.gz` & `tmp/winq2dl-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winq2dl-2.0.2.tar", last modified: Mon Jul 17 07:15:38 2023, max compression
+gzip compressed data, was "winq2dl-2.0.4.tar", last modified: Fri Apr 19 08:52:24 2024, max compression
```

## Comparing `winq2dl-2.0.2.tar` & `winq2dl-2.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:15:38.790126 winq2dl-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 07:15:38.790126 winq2dl-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-17 07:15:28.000000 winq2dl-2.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 07:15:28.000000 winq2dl-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:15:38.790126 winq2dl-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 07:15:28.000000 winq2dl-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:15:38.790126 winq2dl-2.0.2/winq2dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 07:15:38.000000 winq2dl-2.0.2/winq2dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-17 07:15:28.000000 winq2dl-2.0.2/winq2dl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:24.420335 winq2dl-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-19 08:52:24.420335 winq2dl-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 08:52:16.000000 winq2dl-2.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 08:52:16.000000 winq2dl-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:52:24.420335 winq2dl-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 08:52:16.000000 winq2dl-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:24.420335 winq2dl-2.0.4/winq2dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-19 08:52:24.000000 winq2dl-2.0.4/winq2dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-19 08:52:24.000000 winq2dl-2.0.4/winq2dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:52:24.000000 winq2dl-2.0.4/winq2dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 08:52:24.000000 winq2dl-2.0.4/winq2dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 08:52:24.000000 winq2dl-2.0.4/winq2dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-19 08:52:16.000000 winq2dl-2.0.4/winq2dl.py
```

### Comparing `winq2dl-2.0.2/setup.py` & `winq2dl-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `winq2dl-2.0.2/winq2dl.py` & `winq2dl-2.0.4/winq2dl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import ctypes
 import win32gui
 from ctypes import wintypes
 
-__version__ = "2.0.2"
+__version__ = "2.0.4"
 
 # Windows API Types
 CS_HREDRAW = 0x0002
 CS_VREDRAW = 0x0001
 LRESULT = ctypes.c_long
 CW_USEDEFAULT = -2147483648
```

