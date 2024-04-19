# Comparing `tmp/digitalhub_data-0.4.0b0.tar.gz` & `tmp/digitalhub_data-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_data-0.4.0b0.tar", last modified: Wed Apr 17 12:33:43 2024, max compression
+gzip compressed data, was "digitalhub_data-0.4.0b1.tar", last modified: Fri Apr 19 08:58:53 2024, max compression
```

## Comparing `digitalhub_data-0.4.0b0.tar` & `digitalhub_data-0.4.0b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      559 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       81 2023-11-20 10:01:24.000000 digitalhub_data-0.4.0b0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.270845 digitalhub_data-0.4.0b0/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-16 14:28:24.000000 digitalhub_data-0.4.0b0/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.270845 digitalhub_data-0.4.0b0/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.270845 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-16 14:28:25.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6512 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3134 2024-03-06 16:32:11.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-16 14:28:24.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5932 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b0/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b0/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b0/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      559 2024-04-17 12:33:43.000000 digitalhub_data-0.4.0b0/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-17 12:33:43.000000 digitalhub_data-0.4.0b0/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-17 12:33:43.000000 digitalhub_data-0.4.0b0/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-17 12:33:43.000000 digitalhub_data-0.4.0b0/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-17 12:33:43.000000 digitalhub_data-0.4.0b0/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-17 12:33:43.274845 digitalhub_data-0.4.0b0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-19 08:37:43.000000 digitalhub_data-0.4.0b1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.228596 digitalhub_data-0.4.0b1/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.228596 digitalhub_data-0.4.0b1/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.228596 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6489 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3134 2024-03-06 16:32:11.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5909 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b1/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b1/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-04-19 08:46:19.000000 digitalhub_data-0.4.0b1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/setup.cfg
```

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,18 +199,15 @@
         raise EntityError("Unknown file format. Only csv and parquet are supported.")
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         entity : str
             Entity type.
```

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,15 @@
         -------
         list[dict]
             List of objects related to project.
         """
         return list_dataitems(self.name, **kwargs)
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         entity : str
             Entity type.
```

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/entities/registries.py` & `digitalhub_data-0.4.0b1/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.4.0b1/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.4.0b1/digitalhub_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b0/pyproject.toml` & `digitalhub_data-0.4.0b1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.4.0b0"
+version = "0.4.0b1"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-core~=0.3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.4.0b0"
+current_version = "0.4.0b1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

