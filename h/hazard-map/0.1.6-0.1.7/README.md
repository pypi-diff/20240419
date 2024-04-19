# Comparing `tmp/hazard_map-0.1.6.tar.gz` & `tmp/hazard_map-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazard_map-0.1.6.tar", max compression
+gzip compressed data, was "hazard_map-0.1.7.tar", max compression
```

## Comparing `hazard_map-0.1.6.tar` & `hazard_map-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2278 2024-04-18 14:27:32.112775 hazard_map-0.1.6/hazard_map/__init__.py
--rw-r--r--   0        0        0    12733 2024-04-18 14:27:32.112775 hazard_map-0.1.6/hazard_map/hazard_map.py
--rw-r--r--   0        0        0      816 2024-04-18 14:27:32.113775 hazard_map-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2798 2024-04-18 14:27:32.113775 hazard_map-0.1.6/readme.md
--rw-r--r--   0        0        0     3526 1970-01-01 00:00:00.000000 hazard_map-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2523 2024-04-19 14:49:45.298214 hazard_map-0.1.7/hazard_map/__init__.py
+-rw-r--r--   0        0        0    16039 2024-04-19 15:48:48.146969 hazard_map-0.1.7/hazard_map/hazard_map.py
+-rw-r--r--   0        0        0      835 2024-04-19 15:50:51.142147 hazard_map-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2798 2024-04-18 11:25:24.658857 hazard_map-0.1.7/readme.md
+-rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 hazard_map-0.1.7/PKG-INFO
```

### Comparing `hazard_map-0.1.6/pyproject.toml` & `hazard_map-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "hazard-map"
-version = "0.1.6"
+version = "0.1.7"
 description = "Build and analyze a network model of hazards, causes, and controls"
 authors = ["Thom Cameron <thomcm@proton.me>"]
 readme = "readme.md"
 license = "license.txt"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 argparse = "^1.4"
+termcolor = "^2.4"
 numpy = "^1.26"
 pandas = "^2.2"
 openpyxl = "^3.1"
 networkx = "^3.3"
 scipy = "^1.13"
 matplotlib = "^3.8"
```

### Comparing `hazard_map-0.1.6/readme.md` & `hazard_map-0.1.7/readme.md`

 * *Files identical despite different names*

### Comparing `hazard_map-0.1.6/PKG-INFO` & `hazard_map-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazard-map
-Version: 0.1.6
+Version: 0.1.7
 Summary: Build and analyze a network model of hazards, causes, and controls
 License: license.txt
 Author: Thom Cameron
 Author-email: thomcm@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Requires-Dist: argparse (>=1.4,<2.0)
 Requires-Dist: matplotlib (>=3.8,<4.0)
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: openpyxl (>=3.1,<4.0)
 Requires-Dist: pandas (>=2.2,<3.0)
 Requires-Dist: scipy (>=1.13,<2.0)
+Requires-Dist: termcolor (>=2.4,<3.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
     <h1>
         hazard-map
     </h1>
 </div>
```

