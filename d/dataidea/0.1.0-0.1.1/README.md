# Comparing `tmp/dataidea-0.1.0.tar.gz` & `tmp/dataidea-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.1.0.tar", max compression
+gzip compressed data, was "dataidea-0.1.1.tar", max compression
```

## Comparing `dataidea-0.1.0.tar` & `dataidea-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       41 2024-04-18 17:10:00.344848 dataidea-0.1.0/README.md
--rw-r--r--   0        0        0       71 2024-04-18 16:44:47.286351 dataidea-0.1.0/dataidea/tabular.py
--rw-r--r--   0        0        0      419 2024-04-18 17:53:11.548172 dataidea-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 dataidea-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-18 17:10:00.344848 dataidea-0.1.1/README.md
+-rw-r--r--   0        0        0      118 2024-04-18 19:52:54.371041 dataidea-0.1.1/dataidea/tabular.py
+-rw-r--r--   0        0        0      461 2024-04-18 19:53:07.190628 dataidea-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 dataidea-0.1.1/PKG-INFO
```

### Comparing `dataidea-0.1.0/PKG-INFO` & `dataidea-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: dataidea
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package to ease data analysis for DATAIDEA students
 License: MIT
 Author: jumashafara
 Author-email: jumashafara0@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
 Description-Content-Type: text/markdown
 
 This is a tool to simplify data analysis
```

