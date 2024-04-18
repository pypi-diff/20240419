# Comparing `tmp/ute_wrapper-2.4.1.tar.gz` & `tmp/ute_wrapper-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ute_wrapper-2.4.1.tar", max compression
+gzip compressed data, was "ute_wrapper-2.5.0.tar", max compression
```

## Comparing `ute_wrapper-2.4.1.tar` & `ute_wrapper-2.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    32473 2024-03-09 22:46:26.096733 ute_wrapper-2.4.1/LICENSE
--rw-r--r--   0        0        0     2926 2024-03-09 22:46:26.096733 ute_wrapper-2.4.1/README.md
--rw-r--r--   0        0        0     1719 2024-03-09 22:46:26.097733 ute_wrapper-2.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-09 22:46:26.122732 ute_wrapper-2.4.1/src/ute_wrapper/__init__.py
--rw-r--r--   0        0        0      170 2024-03-09 22:46:26.097733 ute_wrapper-2.4.1/src/ute_wrapper/constants.py
--rw-r--r--   0        0        0      829 2024-03-09 22:46:26.097733 ute_wrapper-2.4.1/src/ute_wrapper/exceptions.py
--rw-r--r--   0        0        0      490 2024-03-09 22:46:26.097733 ute_wrapper-2.4.1/src/ute_wrapper/models.py
--rwxr-xr-x   0        0        0    14570 2024-03-09 22:46:26.097733 ute_wrapper-2.4.1/src/ute_wrapper/ute.py
--rw-r--r--   0        0        0     3803 1970-01-01 00:00:00.000000 ute_wrapper-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-04-18 22:16:07.950269 ute_wrapper-2.5.0/LICENSE
+-rw-r--r--   0        0        0     3181 2024-04-18 22:16:07.951269 ute_wrapper-2.5.0/README.md
+-rw-r--r--   0        0        0     1719 2024-04-18 22:16:07.951269 ute_wrapper-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 22:16:07.976269 ute_wrapper-2.5.0/src/ute_wrapper/__init__.py
+-rw-r--r--   0        0        0      170 2024-04-18 22:16:07.951269 ute_wrapper-2.5.0/src/ute_wrapper/constants.py
+-rw-r--r--   0        0        0      829 2024-04-18 22:16:07.951269 ute_wrapper-2.5.0/src/ute_wrapper/exceptions.py
+-rw-r--r--   0        0        0      490 2024-04-18 22:16:07.951269 ute_wrapper-2.5.0/src/ute_wrapper/models.py
+-rwxr-xr-x   0        0        0    14570 2024-04-18 22:16:07.951269 ute_wrapper-2.5.0/src/ute_wrapper/ute.py
+-rw-r--r--   0        0        0     4058 1970-01-01 00:00:00.000000 ute_wrapper-2.5.0/PKG-INFO
```

### Comparing `ute_wrapper-2.4.1/LICENSE` & `ute_wrapper-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ute_wrapper-2.4.1/README.md` & `ute_wrapper-2.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # UTE API Wrapper 🇺🇾
 
+# THIS API NO LONGER WORKS
+
+UTE deprecated the API that this wrapper uses on April 15th 2024. More information [here](https://github.com/rogsme/ute_homeassistant_integration/issues/3#issuecomment-2054332575).
+
+I'll archive this repository in a few days.
+
 <p align="center">
     <img src="https://gitlab.com/uploads/-/system/project/avatar/48558040/icon.png" alt="ute-wrapper"/>
 </p>
 
 [![codecov](https://codecov.io/gl/rogs/ute/graph/badge.svg?token=D1B2J3EB6K)](https://codecov.io/gl/rogs/ute)
 [![PyPI version](https://badge.fury.io/py/ute-wrapper.svg)](https://badge.fury.io/py/ute-wrapper)
```

### Comparing `ute_wrapper-2.4.1/pyproject.toml` & `ute_wrapper-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ute-wrapper"
-version = "2.4.1"
+version = "2.5.0"
 description = "A wrapper to interact with UTE's API"
 authors = ["Roger Gonzalez <roger@rogs.me>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://gitlab.com/rogs/ute/"
 repository = "https://gitlab.com/rogs/ute/"
 documentation = "https://gitlab.com/rogs/ute/-/blob/master/README.md"
```

### Comparing `ute_wrapper-2.4.1/src/ute_wrapper/exceptions.py` & `ute_wrapper-2.5.0/src/ute_wrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `ute_wrapper-2.4.1/src/ute_wrapper/ute.py` & `ute_wrapper-2.5.0/src/ute_wrapper/ute.py`

 * *Files identical despite different names*

### Comparing `ute_wrapper-2.4.1/PKG-INFO` & `ute_wrapper-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ute-wrapper
-Version: 2.4.1
+Version: 2.5.0
 Summary: A wrapper to interact with UTE's API
 Home-page: https://gitlab.com/rogs/ute/
 License: GPL-3.0-or-later
 Keywords: API,wrapper,UTE,Uruguay
 Author: Roger Gonzalez
 Author-email: roger@rogs.me
 Requires-Python: >=3.9
@@ -18,14 +18,20 @@
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Project-URL: Documentation, https://gitlab.com/rogs/ute/-/blob/master/README.md
 Project-URL: Repository, https://gitlab.com/rogs/ute/
 Description-Content-Type: text/markdown
 
 # UTE API Wrapper 🇺🇾
 
+# THIS API NO LONGER WORKS
+
+UTE deprecated the API that this wrapper uses on April 15th 2024. More information [here](https://github.com/rogsme/ute_homeassistant_integration/issues/3#issuecomment-2054332575).
+
+I'll archive this repository in a few days.
+
 <p align="center">
     <img src="https://gitlab.com/uploads/-/system/project/avatar/48558040/icon.png" alt="ute-wrapper"/>
 </p>
 
 [![codecov](https://codecov.io/gl/rogs/ute/graph/badge.svg?token=D1B2J3EB6K)](https://codecov.io/gl/rogs/ute)
 [![PyPI version](https://badge.fury.io/py/ute-wrapper.svg)](https://badge.fury.io/py/ute-wrapper)
```

