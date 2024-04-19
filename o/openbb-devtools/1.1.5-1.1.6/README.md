# Comparing `tmp/openbb_devtools-1.1.5.tar.gz` & `tmp/openbb_devtools-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_devtools-1.1.5.tar", max compression
+gzip compressed data, was "openbb_devtools-1.1.6.tar", max compression
```

## Comparing `openbb_devtools-1.1.5.tar` & `openbb_devtools-1.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      604 2024-02-29 11:03:36.732430 openbb_devtools-1.1.5/README.md
--rw-r--r--   0        0        0       39 2024-02-29 11:03:36.732586 openbb_devtools-1.1.5/openbb_devtools/__init__.py
--rw-r--r--   0        0        0      711 2024-04-01 14:18:45.492574 openbb_devtools-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 openbb_devtools-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-04-17 12:33:20.497645 openbb_devtools-1.1.6/README.md
+-rw-r--r--   0        0        0       39 2024-04-17 12:33:20.497645 openbb_devtools-1.1.6/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0      711 2024-04-19 16:40:31.031130 openbb_devtools-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 openbb_devtools-1.1.6/PKG-INFO
```

### Comparing `openbb_devtools-1.1.5/README.md` & `openbb_devtools-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openbb_devtools-1.1.5/pyproject.toml` & `openbb_devtools-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-devtools"
-version = "1.1.5"
+version = "1.1.6"
 description = "Tools for OpenBB Platform Developers"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_devtools" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"               # scipy forces <4.0 explicitly
```

### Comparing `openbb_devtools-1.1.5/PKG-INFO` & `openbb_devtools-1.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-devtools
-Version: 1.1.5
+Version: 1.1.6
 Summary: Tools for OpenBB Platform Developers
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

