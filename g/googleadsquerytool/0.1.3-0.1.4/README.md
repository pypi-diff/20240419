# Comparing `tmp/googleadsquerytool-0.1.3.tar.gz` & `tmp/googleadsquerytool-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleadsquerytool-0.1.3.tar", max compression
+gzip compressed data, was "googleadsquerytool-0.1.4.tar", max compression
```

## Comparing `googleadsquerytool-0.1.3.tar` & `googleadsquerytool-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      157 2024-04-18 19:39:30.627572 googleadsquerytool-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-18 19:08:34.904765 googleadsquerytool-0.1.3/googleadsquerytool/googleadsquerytool/__init__.py
--rw-r--r--   0        0        0     3951 2024-04-18 12:38:43.656115 googleadsquerytool-0.1.3/googleadsquerytool/googleadsquerytool/googleadsquerytool.py
--rw-r--r--   0        0        0      394 2024-04-18 19:49:15.597768 googleadsquerytool-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 googleadsquerytool-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      157 2024-04-18 19:39:30.627572 googleadsquerytool-0.1.4/README.md
+-rw-r--r--   0        0        0     3951 2024-04-18 12:38:43.656115 googleadsquerytool-0.1.4/googleadsquerytool.py
+-rw-r--r--   0        0        0      394 2024-04-18 19:56:49.269210 googleadsquerytool-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 googleadsquerytool-0.1.4/PKG-INFO
```

### Comparing `googleadsquerytool-0.1.3/googleadsquerytool/googleadsquerytool/googleadsquerytool.py` & `googleadsquerytool-0.1.4/googleadsquerytool.py`

 * *Files identical despite different names*

### Comparing `googleadsquerytool-0.1.3/PKG-INFO` & `googleadsquerytool-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleadsquerytool
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a package you can use to query reporting data from the Google Ads API.
 Author: caspercrause
 Author-email: ccrause07@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

