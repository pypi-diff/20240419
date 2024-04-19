# Comparing `tmp/luxos-0.0.2b7.tar.gz` & `tmp/luxos-0.0.2b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.2b7.tar", last modified: Thu Apr 18 13:06:01 2024, max compression
+gzip compressed data, was "luxos-0.0.2b8.tar", last modified: Thu Apr 18 15:03:27 2024, max compression
```

## Comparing `luxos-0.0.2b7.tar` & `luxos-0.0.2b8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 13:06:01.162823 luxos-0.0.2b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-18 13:05:28.000000 luxos-0.0.2b7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-18 13:05:59.000000 luxos-0.0.2b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:06:01.162823 luxos-0.0.2b7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.158823 luxos-0.0.2b7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 13:05:59.000000 luxos-0.0.2b7/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/luxos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_luxos_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.204679 luxos-0.0.2b8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 15:03:27.204679 luxos-0.0.2b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-18 15:02:56.000000 luxos-0.0.2b8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-18 15:03:25.000000 luxos-0.0.2b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:03:27.204679 luxos-0.0.2b8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.196678 luxos-0.0.2b8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.200679 luxos-0.0.2b8/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 15:03:25.000000 luxos-0.0.2b8/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.200679 luxos-0.0.2b8/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.200679 luxos-0.0.2b8/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/luxos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.204679 luxos-0.0.2b8/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.204679 luxos-0.0.2b8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_luxos_misc.py
```

### Comparing `luxos-0.0.2b7/PKG-INFO` & `luxos-0.0.2b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.2b7
+Version: 0.0.2b8
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.2b7/README.md` & `luxos-0.0.2b8/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/pyproject.toml` & `luxos-0.0.2b8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.2b7"
+version = "0.0.2b8"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.2b7/src/luxos/api.json` & `luxos-0.0.2b8/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/api.py` & `luxos-0.0.2b8/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/asyncops.py` & `luxos-0.0.2b8/src/luxos/asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/cli/v1.py` & `luxos-0.0.2b8/src/luxos/cli/v1.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/exceptions.py` & `luxos-0.0.2b8/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/misc.py` & `luxos-0.0.2b8/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/scripts/async_luxos.py` & `luxos-0.0.2b8/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/scripts/health_checker.py` & `luxos-0.0.2b8/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos/scripts/luxos.py` & `luxos-0.0.2b8/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.2b8/src/luxos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.2b7
+Version: 0.0.2b8
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.2b7/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.2b8/src/luxos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/tests/test_cli.py` & `luxos-0.0.2b8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/tests/test_luxos_asyncops.py` & `luxos-0.0.2b8/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b7/tests/test_luxos_misc.py` & `luxos-0.0.2b8/tests/test_luxos_misc.py`

 * *Files identical despite different names*

