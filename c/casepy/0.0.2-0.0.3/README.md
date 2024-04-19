# Comparing `tmp/casepy-0.0.2.tar.gz` & `tmp/casepy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casepy-0.0.2.tar", last modified: Fri Apr 19 06:27:44 2024, max compression
+gzip compressed data, was "casepy-0.0.3.tar", last modified: Fri Apr 19 06:39:34 2024, max compression
```

## Comparing `casepy-0.0.2.tar` & `casepy-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:27:44.248728 casepy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 06:27:34.000000 casepy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-19 06:27:44.248728 casepy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 06:27:34.000000 casepy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:27:44.248728 casepy-0.0.2/casepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-19 06:27:44.000000 casepy-0.0.2/casepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-19 06:27:44.000000 casepy-0.0.2/casepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:27:44.000000 casepy-0.0.2/casepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:27:44.000000 casepy-0.0.2/casepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:27:44.248728 casepy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-19 06:27:34.000000 casepy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:39:34.243067 casepy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 06:39:27.000000 casepy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-19 06:39:34.243067 casepy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 06:39:27.000000 casepy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:39:34.243067 casepy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 06:39:27.000000 casepy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:39:34.243067 casepy-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:39:34.243067 casepy-0.0.3/src/casepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/top_level.txt
```

### Comparing `casepy-0.0.2/LICENSE` & `casepy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `casepy-0.0.2/PKG-INFO` & `casepy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >2.7.0
```

### Comparing `casepy-0.0.2/README.md` & `casepy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `casepy-0.0.2/casepy.egg-info/PKG-INFO` & `casepy-0.0.3/src/casepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >2.7.0
```

