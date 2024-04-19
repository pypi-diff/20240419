# Comparing `tmp/owmpy-1.0.4.tar.gz` & `tmp/owmpy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owmpy-1.0.4.tar", last modified: Sun Apr  7 19:39:41 2024, max compression
+gzip compressed data, was "owmpy-1.0.5.tar", last modified: Fri Apr 19 10:49:41 2024, max compression
```

## Comparing `owmpy-1.0.4.tar` & `owmpy-1.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 19:39:41.393553 owmpy-1.0.4/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)     1081 2024-04-07 10:00:37.000000 owmpy-1.0.4/LICENSE
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       25 2024-04-07 13:21:34.000000 owmpy-1.0.4/MANIFEST.in
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 19:39:41.393553 owmpy-1.0.4/PKG-INFO
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      778 2024-04-07 12:42:49.000000 owmpy-1.0.4/README.md
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 19:39:41.387553 owmpy-1.0.4/owmpy/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      261 2024-04-07 19:39:36.000000 owmpy-1.0.4/owmpy/__init__.py
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 19:39:41.389553 owmpy-1.0.4/owmpy/core/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       76 2024-04-07 12:13:57.000000 owmpy-1.0.4/owmpy/core/__init__.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       40 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/core/api_exception.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      795 2024-04-07 12:48:31.000000 owmpy-1.0.4/owmpy/core/base_client.py
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 19:39:41.389553 owmpy-1.0.4/owmpy/current/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       58 2024-04-07 12:34:14.000000 owmpy-1.0.4/owmpy/current/__init__.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      962 2024-04-07 12:34:08.000000 owmpy-1.0.4/owmpy/current/client.py
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 19:39:41.391553 owmpy-1.0.4/owmpy/current/response/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      202 2024-04-07 12:13:57.000000 owmpy-1.0.4/owmpy/current/response/__init__.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      108 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/current/response/clouds.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      176 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/current/response/coord.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      903 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/current/response/main.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       98 2024-04-07 12:13:57.000000 owmpy-1.0.4/owmpy/current/response/rain.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      947 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/current/response/response.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      328 2024-04-07 19:34:21.000000 owmpy-1.0.4/owmpy/current/response/sys.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      481 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/current/response/weather.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      317 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/current/response/wind.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:15:49.000000 owmpy-1.0.4/owmpy/py.typed
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 19:39:41.392553 owmpy-1.0.4/owmpy/utils/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      130 2024-04-07 12:13:57.000000 owmpy-1.0.4/owmpy/utils/__init__.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      218 2024-04-07 12:13:57.000000 owmpy-1.0.4/owmpy/utils/short_long.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)     2187 2024-04-07 12:13:58.000000 owmpy-1.0.4/owmpy/utils/standard_units.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      451 2024-04-07 12:13:57.000000 owmpy-1.0.4/owmpy/utils/units.py
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 19:39:41.392553 owmpy-1.0.4/owmpy.egg-info/
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 19:39:41.000000 owmpy-1.0.4/owmpy.egg-info/PKG-INFO
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      767 2024-04-07 19:39:41.000000 owmpy-1.0.4/owmpy.egg-info/SOURCES.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)        1 2024-04-07 19:39:41.000000 owmpy-1.0.4/owmpy.egg-info/dependency_links.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       31 2024-04-07 19:39:41.000000 owmpy-1.0.4/owmpy.egg-info/requires.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)        6 2024-04-07 19:39:41.000000 owmpy-1.0.4/owmpy.egg-info/top_level.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      231 2024-04-07 10:21:28.000000 owmpy-1.0.4/pyproject.toml
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       36 2024-04-07 10:39:25.000000 owmpy-1.0.4/requirements.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       38 2024-04-07 19:39:41.393553 owmpy-1.0.4/setup.cfg
--rw-rw-r--   0 ernie     (1000) ernie     (1000)     1156 2024-04-07 14:22:34.000000 owmpy-1.0.4/setup.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-19 10:49:41.368012 owmpy-1.0.5/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     1081 2024-04-07 10:00:37.000000 owmpy-1.0.5/LICENSE
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       25 2024-04-07 13:21:34.000000 owmpy-1.0.5/MANIFEST.in
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-19 10:49:41.368012 owmpy-1.0.5/PKG-INFO
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      778 2024-04-07 12:42:49.000000 owmpy-1.0.5/README.md
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-19 10:49:41.364012 owmpy-1.0.5/owmpy/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      261 2024-04-19 10:47:49.000000 owmpy-1.0.5/owmpy/__init__.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-19 10:49:41.365012 owmpy-1.0.5/owmpy/core/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       76 2024-04-07 12:13:57.000000 owmpy-1.0.5/owmpy/core/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       40 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/core/api_exception.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      795 2024-04-07 12:48:31.000000 owmpy-1.0.5/owmpy/core/base_client.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-19 10:49:41.366012 owmpy-1.0.5/owmpy/current/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       92 2024-04-19 10:39:23.000000 owmpy-1.0.5/owmpy/current/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      962 2024-04-07 12:34:08.000000 owmpy-1.0.5/owmpy/current/client.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-19 10:49:41.367012 owmpy-1.0.5/owmpy/current/response/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      287 2024-04-19 10:41:03.000000 owmpy-1.0.5/owmpy/current/response/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      108 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/current/response/clouds.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      176 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/current/response/coord.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      903 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/current/response/main.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       98 2024-04-07 12:13:57.000000 owmpy-1.0.5/owmpy/current/response/rain.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      947 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/current/response/response.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      328 2024-04-07 19:34:21.000000 owmpy-1.0.5/owmpy/current/response/sys.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      481 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/current/response/weather.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      317 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/current/response/wind.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:15:49.000000 owmpy-1.0.5/owmpy/py.typed
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-19 10:49:41.368012 owmpy-1.0.5/owmpy/utils/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      214 2024-04-19 10:39:58.000000 owmpy-1.0.5/owmpy/utils/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      218 2024-04-07 12:13:57.000000 owmpy-1.0.5/owmpy/utils/short_long.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     2187 2024-04-07 12:13:58.000000 owmpy-1.0.5/owmpy/utils/standard_units.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      451 2024-04-07 12:13:57.000000 owmpy-1.0.5/owmpy/utils/units.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-19 10:49:41.368012 owmpy-1.0.5/owmpy.egg-info/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-19 10:49:41.000000 owmpy-1.0.5/owmpy.egg-info/PKG-INFO
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      767 2024-04-19 10:49:41.000000 owmpy-1.0.5/owmpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        1 2024-04-19 10:49:41.000000 owmpy-1.0.5/owmpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       31 2024-04-19 10:49:41.000000 owmpy-1.0.5/owmpy.egg-info/requires.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        6 2024-04-19 10:49:41.000000 owmpy-1.0.5/owmpy.egg-info/top_level.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      280 2024-04-19 10:42:11.000000 owmpy-1.0.5/pyproject.toml
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       36 2024-04-07 10:39:25.000000 owmpy-1.0.5/requirements.txt
+-rw-r--r--   0 ernie     (1000) ernie     (1000)       38 2024-04-19 10:49:41.368012 owmpy-1.0.5/setup.cfg
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     1156 2024-04-19 10:42:20.000000 owmpy-1.0.5/setup.py
```

### Comparing `owmpy-1.0.4/LICENSE` & `owmpy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/PKG-INFO` & `owmpy-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owmpy
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wrapper for the OpenWeatherMap API
 Home-page: https://github.com/ernieIzde8ski/open_weather_mappy
 Author: Ernest Izdebski
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owmpy-1.0.4/README.md` & `owmpy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/owmpy/core/base_client.py` & `owmpy-1.0.5/owmpy/core/base_client.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/owmpy/current/client.py` & `owmpy-1.0.5/owmpy/current/client.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/owmpy/current/response/main.py` & `owmpy-1.0.5/owmpy/current/response/main.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/owmpy/current/response/response.py` & `owmpy-1.0.5/owmpy/current/response/response.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/owmpy/utils/standard_units.py` & `owmpy-1.0.5/owmpy/utils/standard_units.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/owmpy.egg-info/PKG-INFO` & `owmpy-1.0.5/owmpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owmpy
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wrapper for the OpenWeatherMap API
 Home-page: https://github.com/ernieIzde8ski/open_weather_mappy
 Author: Ernest Izdebski
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owmpy-1.0.4/owmpy.egg-info/SOURCES.txt` & `owmpy-1.0.5/owmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.4/setup.py` & `owmpy-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import re
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 string_equality = re.compile(r"""__([\w_]+)__\s*=\s*"(.+)"$""")
 
 data = {}
 
 with open("owmpy/__init__.py", "r") as file:
     for line in file.readlines():
```

