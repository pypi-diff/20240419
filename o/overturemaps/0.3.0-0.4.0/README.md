# Comparing `tmp/overturemaps-0.3.0.tar.gz` & `tmp/overturemaps-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overturemaps-0.3.0.tar", max compression
+gzip compressed data, was "overturemaps-0.4.0.tar", max compression
```

## Comparing `overturemaps-0.3.0.tar` & `overturemaps-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-04-06 10:31:26.935857 overturemaps-0.3.0/LICENSE
--rw-r--r--   0        0        0     2507 2024-04-11 15:34:22.013871 overturemaps-0.3.0/README.md
--rw-r--r--   0        0        0       75 2024-04-11 16:40:32.681725 overturemaps-0.3.0/overturemaps/__init__.py
--rw-r--r--   0        0        0     5086 2024-04-16 03:33:02.187599 overturemaps-0.3.0/overturemaps/cli.py
--rw-r--r--   0        0        0     3246 2024-04-16 03:37:08.217413 overturemaps-0.3.0/overturemaps/core.py
--rw-r--r--   0        0        0      480 2024-04-16 12:46:02.130484 overturemaps-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 overturemaps-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-06 10:31:26.935857 overturemaps-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2507 2024-04-11 15:34:22.013871 overturemaps-0.4.0/README.md
+-rw-r--r--   0        0        0       75 2024-04-11 16:40:32.681725 overturemaps-0.4.0/overturemaps/__init__.py
+-rw-r--r--   0        0        0     5086 2024-04-16 03:33:02.187599 overturemaps-0.4.0/overturemaps/cli.py
+-rw-r--r--   0        0        0     3246 2024-04-16 03:37:08.217413 overturemaps-0.4.0/overturemaps/core.py
+-rw-r--r--   0        0        0      479 2024-04-19 20:54:04.960647 overturemaps-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 overturemaps-0.4.0/PKG-INFO
```

### Comparing `overturemaps-0.3.0/LICENSE` & `overturemaps-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `overturemaps-0.3.0/README.md` & `overturemaps-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `overturemaps-0.3.0/overturemaps/cli.py` & `overturemaps-0.4.0/overturemaps/cli.py`

 * *Files identical despite different names*

### Comparing `overturemaps-0.3.0/overturemaps/core.py` & `overturemaps-0.4.0/overturemaps/core.py`

 * *Files identical despite different names*

### Comparing `overturemaps-0.3.0/PKG-INFO` & `overturemaps-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: overturemaps
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python tools for interacting with Overture Maps (overturemaps.org) data.
 License: MIT
 Author: Jacob Wasserman
 Author-email: jwasserman@meta.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: shapely (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
```

