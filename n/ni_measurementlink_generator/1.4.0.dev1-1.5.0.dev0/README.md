# Comparing `tmp/ni_measurementlink_generator-1.4.0.dev1.tar.gz` & `tmp/ni_measurementlink_generator-1.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_generator-1.4.0.dev1.tar", max compression
+gzip compressed data, was "ni_measurementlink_generator-1.5.0.dev0.tar", max compression
```

## Comparing `ni_measurementlink_generator-1.4.0.dev1.tar` & `ni_measurementlink_generator-1.5.0.dev0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      616 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/README.md
--rw-r--r--   0        0        0      149 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/__main__.py
--rw-r--r--   0        0        0        0 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/py.typed
--rw-r--r--   0        0        0     6500 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/template.py
--rw-r--r--   0        0        0     2593 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/_helpers.py.mako
--rw-r--r--   0        0        0     1690 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.measproj.mako
--rw-r--r--   0        0        0     5143 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.measui.mako
--rw-r--r--   0        0        0     1567 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.py.mako
--rw-r--r--   0        0        0      815 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
--rw-r--r--   0        0        0      247 2024-03-08 14:27:02.765118 ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/start.bat.mako
--rw-r--r--   0        0        0     1606 2024-03-08 14:27:20.913210 ni_measurementlink_generator-1.4.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.4.0.dev1/setup.py
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.4.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      616 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/README.md
+-rw-r--r--   0        0        0      149 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/py.typed
+-rw-r--r--   0        0        0     6500 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/template.py
+-rw-r--r--   0        0        0     2593 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/_helpers.py.mako
+-rw-r--r--   0        0        0     1690 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako
+-rw-r--r--   0        0        0     5143 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako
+-rw-r--r--   0        0        0     1567 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako
+-rw-r--r--   0        0        0      815 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
+-rw-r--r--   0        0        0      247 2024-04-19 19:40:07.048515 ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/start.bat.mako
+-rw-r--r--   0        0        0     1606 2024-04-19 19:40:21.588612 ni_measurementlink_generator-1.5.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.5.0.dev0/PKG-INFO
```

### Comparing `ni_measurementlink_generator-1.4.0.dev1/README.md` & `ni_measurementlink_generator-1.5.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/template.py` & `ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/template.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/_helpers.py.mako` & `ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/_helpers.py.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.measproj.mako` & `ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.measui.mako` & `ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.py.mako` & `ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.4.0.dev1/ni_measurementlink_generator/templates/measurement.serviceconfig.mako` & `ni_measurementlink_generator-1.5.0.dev0/ni_measurementlink_generator/templates/measurement.serviceconfig.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.4.0.dev1/pyproject.toml` & `ni_measurementlink_generator-1.5.0.dev0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ni_measurementlink_generator"
-version = "1.4.0-dev1"
+version = "1.5.0-dev0"
 description = "MeasurementLink Code Generator for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md"
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `ni_measurementlink_generator-1.4.0.dev1/PKG-INFO` & `ni_measurementlink_generator-1.5.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ni-measurementlink-generator
-Version: 1.4.0.dev1
+Name: ni_measurementlink_generator
+Version: 1.5.0.dev0
 Summary: MeasurementLink Code Generator for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Hardware
 Requires-Dist: Mako (>=1.2.1,<2.0.0)
 Requires-Dist: click (>=8.1.3)
 Project-URL: Repository, https://github.com/ni/measurementlink-python/
 Description-Content-Type: text/markdown
```

