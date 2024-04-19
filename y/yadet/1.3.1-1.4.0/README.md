# Comparing `tmp/yadet-1.3.1.tar.gz` & `tmp/yadet-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadet-1.3.1.tar", last modified: Thu Mar 14 21:39:08 2024, max compression
+gzip compressed data, was "yadet-1.4.0.tar", last modified: Fri Apr 19 13:30:54 2024, max compression
```

## Comparing `yadet-1.3.1.tar` & `yadet-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.560913 yadet-1.3.1/
--rw-rw-rw-   0        0        0     1091 2024-03-10 20:04:48.000000 yadet-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     1694 2024-03-14 21:39:08.558913 yadet-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2024-01-18 00:03:14.000000 yadet-1.3.1/README.md
--rw-rw-rw-   0        0        0      704 2024-03-14 21:38:41.000000 yadet-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 21:39:08.560913 yadet-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1038 2024-03-14 21:38:42.000000 yadet-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.473211 yadet-1.3.1/yadet/
--rw-rw-rw-   0        0        0       23 2024-03-14 21:38:20.000000 yadet-1.3.1/yadet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.506287 yadet-1.3.1/yadet/batch/
--rw-rw-rw-   0        0        0       38 2024-01-17 23:23:06.000000 yadet-1.3.1/yadet/batch/__init__.py
--rw-rw-rw-   0        0        0     4004 2024-03-10 20:07:20.000000 yadet-1.3.1/yadet/batch/batch_run.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.515814 yadet-1.3.1/yadet/config/
--rw-rw-rw-   0        0        0       34 2024-01-17 23:22:47.000000 yadet-1.3.1/yadet/config/__init__.py
--rw-rw-rw-   0        0        0     4537 2024-01-26 01:50:22.000000 yadet-1.3.1/yadet/config/project.py
--rw-rw-rw-   0        0        0     2453 2024-02-01 19:01:03.000000 yadet-1.3.1/yadet/config/table.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.517815 yadet-1.3.1/yadet/engine/
--rw-rw-rw-   0        0        0       45 2024-01-17 23:24:25.000000 yadet-1.3.1/yadet/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.525342 yadet-1.3.1/yadet/engine/source/
--rw-rw-rw-   0        0        0       73 2024-01-17 23:25:09.000000 yadet-1.3.1/yadet/engine/source/__init__.py
--rw-rw-rw-   0        0        0     1494 2024-01-17 23:26:32.000000 yadet-1.3.1/yadet/engine/source/base.py
--rw-rw-rw-   0        0        0     4129 2024-03-10 20:07:26.000000 yadet-1.3.1/yadet/engine/source/mssql.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.531340 yadet-1.3.1/yadet/engine/target/
--rw-rw-rw-   0        0        0       89 2024-01-17 23:25:18.000000 yadet-1.3.1/yadet/engine/target/__init__.py
--rw-rw-rw-   0        0        0      563 2024-01-27 02:52:35.000000 yadet-1.3.1/yadet/engine/target/base.py
--rw-rw-rw-   0        0        0     1695 2024-01-27 02:53:11.000000 yadet-1.3.1/yadet/engine/target/file_system.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.532848 yadet-1.3.1/yadet/errors/
--rw-rw-rw-   0        0        0       43 2024-01-17 21:45:06.000000 yadet-1.3.1/yadet/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.543388 yadet-1.3.1/yadet/helpers/
--rw-rw-rw-   0        0        0      117 2024-01-17 22:50:21.000000 yadet-1.3.1/yadet/helpers/__init__.py
--rw-rw-rw-   0        0        0      151 2024-01-17 22:50:11.000000 yadet-1.3.1/yadet/helpers/base.py
--rw-rw-rw-   0        0        0      442 2024-01-17 21:56:14.000000 yadet-1.3.1/yadet/helpers/json.py
--rw-rw-rw-   0        0        0      542 2024-01-20 19:08:09.000000 yadet-1.3.1/yadet/helpers/parser.py
--rw-rw-rw-   0        0        0       92 2024-01-17 21:49:23.000000 yadet-1.3.1/yadet/helpers/sql.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.550394 yadet-1.3.1/yadet/interface/
--rw-rw-rw-   0        0        0      128 2024-01-17 23:20:57.000000 yadet-1.3.1/yadet/interface/__init__.py
--rw-rw-rw-   0        0        0     1999 2024-03-14 21:37:46.000000 yadet-1.3.1/yadet/interface/extract_transfer.py
--rw-rw-rw-   0        0        0     2074 2024-02-01 18:55:18.000000 yadet-1.3.1/yadet/interface/source.py
--rw-rw-rw-   0        0        0      858 2024-02-01 18:59:48.000000 yadet-1.3.1/yadet/interface/target.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.554914 yadet-1.3.1/yadet/objects/
--rw-rw-rw-   0        0        0       28 2024-01-17 21:45:56.000000 yadet-1.3.1/yadet/objects/__init__.py
--rw-rw-rw-   0        0        0      118 2024-01-17 21:57:43.000000 yadet-1.3.1/yadet/objects/base.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:39:08.557914 yadet-1.3.1/yadet.egg-info/
--rw-rw-rw-   0        0        0     1694 2024-03-14 21:39:08.000000 yadet-1.3.1/yadet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2024-03-14 21:39:08.000000 yadet-1.3.1/yadet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 21:39:08.000000 yadet-1.3.1/yadet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-14 21:39:08.000000 yadet-1.3.1/yadet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-01-26 01:59:22.000000 yadet-1.3.1/yadet.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.393297 yadet-1.4.0/
+-rw-rw-rw-   0        0        0     1091 2024-03-10 20:04:48.000000 yadet-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1694 2024-04-19 13:30:54.391297 yadet-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2024-01-18 00:03:14.000000 yadet-1.4.0/README.md
+-rw-rw-rw-   0        0        0      704 2024-04-19 13:28:18.000000 yadet-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 13:30:54.393297 yadet-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2024-04-19 13:28:25.000000 yadet-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.185807 yadet-1.4.0/yadet/
+-rw-rw-rw-   0        0        0       23 2024-04-19 13:28:32.000000 yadet-1.4.0/yadet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.226377 yadet-1.4.0/yadet/batch/
+-rw-rw-rw-   0        0        0       38 2024-01-17 23:23:06.000000 yadet-1.4.0/yadet/batch/__init__.py
+-rw-rw-rw-   0        0        0     4004 2024-03-10 20:07:20.000000 yadet-1.4.0/yadet/batch/batch_run.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.250419 yadet-1.4.0/yadet/config/
+-rw-rw-rw-   0        0        0       34 2024-01-17 23:22:47.000000 yadet-1.4.0/yadet/config/__init__.py
+-rw-rw-rw-   0        0        0     4537 2024-01-26 01:50:22.000000 yadet-1.4.0/yadet/config/project.py
+-rw-rw-rw-   0        0        0     2453 2024-02-01 19:01:03.000000 yadet-1.4.0/yadet/config/table.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.253420 yadet-1.4.0/yadet/engine/
+-rw-rw-rw-   0        0        0       45 2024-01-17 23:24:25.000000 yadet-1.4.0/yadet/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.275961 yadet-1.4.0/yadet/engine/source/
+-rw-rw-rw-   0        0        0       73 2024-01-17 23:25:09.000000 yadet-1.4.0/yadet/engine/source/__init__.py
+-rw-rw-rw-   0        0        0     1494 2024-01-17 23:26:32.000000 yadet-1.4.0/yadet/engine/source/base.py
+-rw-rw-rw-   0        0        0     4129 2024-03-10 20:07:26.000000 yadet-1.4.0/yadet/engine/source/mssql.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.298997 yadet-1.4.0/yadet/engine/target/
+-rw-rw-rw-   0        0        0       89 2024-01-17 23:25:18.000000 yadet-1.4.0/yadet/engine/target/__init__.py
+-rw-rw-rw-   0        0        0      563 2024-01-27 02:52:35.000000 yadet-1.4.0/yadet/engine/target/base.py
+-rw-rw-rw-   0        0        0     1695 2024-01-27 02:53:11.000000 yadet-1.4.0/yadet/engine/target/file_system.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.305509 yadet-1.4.0/yadet/errors/
+-rw-rw-rw-   0        0        0       43 2024-01-17 21:45:06.000000 yadet-1.4.0/yadet/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.343153 yadet-1.4.0/yadet/helpers/
+-rw-rw-rw-   0        0        0      117 2024-01-17 22:50:21.000000 yadet-1.4.0/yadet/helpers/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-01-17 22:50:11.000000 yadet-1.4.0/yadet/helpers/base.py
+-rw-rw-rw-   0        0        0      442 2024-01-17 21:56:14.000000 yadet-1.4.0/yadet/helpers/json.py
+-rw-rw-rw-   0        0        0      542 2024-01-20 19:08:09.000000 yadet-1.4.0/yadet/helpers/parser.py
+-rw-rw-rw-   0        0        0       92 2024-01-17 21:49:23.000000 yadet-1.4.0/yadet/helpers/sql.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.373261 yadet-1.4.0/yadet/interface/
+-rw-rw-rw-   0        0        0      128 2024-01-17 23:20:57.000000 yadet-1.4.0/yadet/interface/__init__.py
+-rw-rw-rw-   0        0        0     1999 2024-03-14 21:37:46.000000 yadet-1.4.0/yadet/interface/extract_transfer.py
+-rw-rw-rw-   0        0        0     2074 2024-02-01 18:55:18.000000 yadet-1.4.0/yadet/interface/source.py
+-rw-rw-rw-   0        0        0      858 2024-02-01 18:59:48.000000 yadet-1.4.0/yadet/interface/target.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.386291 yadet-1.4.0/yadet/objects/
+-rw-rw-rw-   0        0        0       28 2024-01-17 21:45:56.000000 yadet-1.4.0/yadet/objects/__init__.py
+-rw-rw-rw-   0        0        0      118 2024-01-17 21:57:43.000000 yadet-1.4.0/yadet/objects/base.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:30:54.389297 yadet-1.4.0/yadet.egg-info/
+-rw-rw-rw-   0        0        0     1694 2024-04-19 13:30:54.000000 yadet-1.4.0/yadet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2024-04-19 13:30:54.000000 yadet-1.4.0/yadet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:30:54.000000 yadet-1.4.0/yadet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-19 13:30:54.000000 yadet-1.4.0/yadet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-01-26 01:59:22.000000 yadet-1.4.0/yadet.egg-info/zip-safe
```

### Comparing `yadet-1.3.1/LICENSE` & `yadet-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/PKG-INFO` & `yadet-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadet
-Version: 1.3.1
+Version: 1.4.0
 Summary: A simple and effective Python data extraction tool for getting batch data exports and store in a simple format.
 Home-page: https://github.com/robbitt07/yadet
 Author: Robert Goss
 Author-email: Robert Goss <robertgoss07@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/robbitt07/yadet
 Project-URL: Bug Tracker, https://github.com/robbitt07/yadet/issues
```

### Comparing `yadet-1.3.1/README.md` & `yadet-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/pyproject.toml` & `yadet-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yadet"
-version = "1.3.1"
+version = "1.4.0"
 authors = [
   { name="Robert Goss", email="robertgoss07@gmail.com" }
 ]
 description = "A simple and effective Python data extraction tool for getting batch data exports and store in a simple format."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yadet-1.3.1/setup.py` & `yadet-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 
 install_requires = ["pyodbc"]
 
 setup(
     name="yadet",
-    version="1.3.1",
+    version="1.4.0",
     author="Robert Goss",
     author_email="robertgoss07@gmail.com",
     packages=[
         "yadet", "yadet.batch", "yadet.config", "yadet.engine", "yadet.engine.source", 
         "yadet.engine.target", "yadet.errors", "yadet.helpers", "yadet.interface", 
         "yadet.objects"
     ],
```

### Comparing `yadet-1.3.1/yadet/batch/batch_run.py` & `yadet-1.4.0/yadet/batch/batch_run.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/config/project.py` & `yadet-1.4.0/yadet/config/project.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/config/table.py` & `yadet-1.4.0/yadet/config/table.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/engine/source/base.py` & `yadet-1.4.0/yadet/engine/source/base.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/engine/source/mssql.py` & `yadet-1.4.0/yadet/engine/source/mssql.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/engine/target/base.py` & `yadet-1.4.0/yadet/engine/target/base.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/engine/target/file_system.py` & `yadet-1.4.0/yadet/engine/target/file_system.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/helpers/parser.py` & `yadet-1.4.0/yadet/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/interface/extract_transfer.py` & `yadet-1.4.0/yadet/interface/extract_transfer.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/interface/source.py` & `yadet-1.4.0/yadet/interface/source.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet/interface/target.py` & `yadet-1.4.0/yadet/interface/target.py`

 * *Files identical despite different names*

### Comparing `yadet-1.3.1/yadet.egg-info/PKG-INFO` & `yadet-1.4.0/yadet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadet
-Version: 1.3.1
+Version: 1.4.0
 Summary: A simple and effective Python data extraction tool for getting batch data exports and store in a simple format.
 Home-page: https://github.com/robbitt07/yadet
 Author: Robert Goss
 Author-email: Robert Goss <robertgoss07@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/robbitt07/yadet
 Project-URL: Bug Tracker, https://github.com/robbitt07/yadet/issues
```

### Comparing `yadet-1.3.1/yadet.egg-info/SOURCES.txt` & `yadet-1.4.0/yadet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

