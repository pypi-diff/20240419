# Comparing `tmp/pysolcast-2.0.1.tar.gz` & `tmp/pysolcast-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolcast-2.0.1.tar", max compression
+gzip compressed data, was "pysolcast-2.0.2.tar", max compression
```

## Comparing `pysolcast-2.0.1.tar` & `pysolcast-2.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      175 2024-02-16 01:20:53.091090 pysolcast-2.0.1/AUTHORS.rst
--rw-r--r--   0        0        0    11357 2024-02-16 01:20:53.091090 pysolcast-2.0.1/LICENSE
--rw-r--r--   0        0        0     1302 2024-02-16 01:20:53.091090 pysolcast-2.0.1/README.rst
--rw-r--r--   0        0        0      717 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      124 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pysolcast/__init__.py
--rw-r--r--   0        0        0     3239 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pysolcast/base.py
--rw-r--r--   0        0        0      391 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pysolcast/exceptions.py
--rw-r--r--   0        0        0     1730 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pysolcast/rooftop.py
--rw-r--r--   0        0        0     2998 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pysolcast/utility.py
--rw-r--r--   0        0        0      861 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pysolcast/weather.py
--rw-r--r--   0        0        0     2276 2024-02-16 01:20:53.091090 pysolcast-2.0.1/pysolcast/world.py
--rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 pysolcast-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      175 2024-04-19 13:12:25.766183 pysolcast-2.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0    11357 2024-04-19 13:12:25.766183 pysolcast-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1302 2024-04-19 13:12:25.766183 pysolcast-2.0.2/README.rst
+-rw-r--r--   0        0        0      717 2024-04-19 13:12:25.766183 pysolcast-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-04-19 13:12:25.766183 pysolcast-2.0.2/pysolcast/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-19 13:12:25.766183 pysolcast-2.0.2/pysolcast/base.py
+-rw-r--r--   0        0        0      391 2024-04-19 13:12:25.766183 pysolcast-2.0.2/pysolcast/exceptions.py
+-rw-r--r--   0        0        0     1730 2024-04-19 13:12:25.766183 pysolcast-2.0.2/pysolcast/rooftop.py
+-rw-r--r--   0        0        0     2998 2024-04-19 13:12:25.770183 pysolcast-2.0.2/pysolcast/utility.py
+-rw-r--r--   0        0        0      861 2024-04-19 13:12:25.770183 pysolcast-2.0.2/pysolcast/weather.py
+-rw-r--r--   0        0        0     2276 2024-04-19 13:12:25.770183 pysolcast-2.0.2/pysolcast/world.py
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 pysolcast-2.0.2/PKG-INFO
```

### Comparing `pysolcast-2.0.1/LICENSE` & `pysolcast-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolcast-2.0.1/README.rst` & `pysolcast-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pysolcast-2.0.1/pyproject.toml` & `pysolcast-2.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "pysolcast"
-version = "2.0.1"
+version = "2.0.2"
 description = ""
 authors = ["Nathaniel McAuliffe <nathanielmcauliffe@hotmail.com>"]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 anyconfig = "0.14.0"
 isodate = "0.6.1"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "1.0.1"
-tox = "4.12.1"
-pytest = "8.0.0"
-pytest-cov = "4.1.0"
-sphinx-autodoc-typehints = "2.0.0"
-autopep8 = "2.0.4"
-rope = "1.12.0"
+tox = "4.14.2"
+pytest = "8.1.1"
+pytest-cov = "5.0.0"
+sphinx-autodoc-typehints = "2.1.0"
+autopep8 = "2.1.0"
+rope = "1.13.0"
 pydocstyle = "6.3.0"
 pycodestyle = "2.11.1"
 mock = "5.1.0"
-pylint = "3.0.3"
+pylint = "3.1.0"
 setuptools-scm = "8.0.4"
-Sphinx = "7.2.6"
+Sphinx = "7.3.7"
 responses = "^0.25.0"
 
 
 [build-system]
 requires = ["poetry-core >= 1.9.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysolcast-2.0.1/pysolcast/base.py` & `pysolcast-2.0.2/pysolcast/base.py`

 * *Files identical despite different names*

### Comparing `pysolcast-2.0.1/pysolcast/rooftop.py` & `pysolcast-2.0.2/pysolcast/rooftop.py`

 * *Files identical despite different names*

### Comparing `pysolcast-2.0.1/pysolcast/utility.py` & `pysolcast-2.0.2/pysolcast/utility.py`

 * *Files identical despite different names*

### Comparing `pysolcast-2.0.1/pysolcast/weather.py` & `pysolcast-2.0.2/pysolcast/weather.py`

 * *Files identical despite different names*

### Comparing `pysolcast-2.0.1/pysolcast/world.py` & `pysolcast-2.0.2/pysolcast/world.py`

 * *Files identical despite different names*

### Comparing `pysolcast-2.0.1/PKG-INFO` & `pysolcast-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysolcast
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 Author: Nathaniel McAuliffe
 Author-email: nathanielmcauliffe@hotmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

