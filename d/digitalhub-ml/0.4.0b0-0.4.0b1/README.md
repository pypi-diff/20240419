# Comparing `tmp/digitalhub_ml-0.4.0b0.tar.gz` & `tmp/digitalhub_ml-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_ml-0.4.0b0.tar", last modified: Wed Apr 17 12:34:18 2024, max compression
+gzip compressed data, was "digitalhub_ml-0.4.0b1.tar", last modified: Fri Apr 19 08:59:16 2024, max compression
```

## Comparing `digitalhub_ml-0.4.0b0.tar` & `digitalhub_ml-0.4.0b1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:34:18.631265 digitalhub_ml-0.4.0b0/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      550 2024-04-17 12:34:18.631265 digitalhub_ml-0.4.0b0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       74 2023-11-20 10:00:49.000000 digitalhub_ml-0.4.0b0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:34:18.623265 digitalhub_ml-0.4.0b0/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-04-16 14:28:24.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:34:18.627265 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:34:18.627265 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6252 2024-04-16 14:28:25.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6809 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:34:18.627265 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-04-16 14:28:25.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5811 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      991 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:34:18.627265 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-04-16 14:28:25.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.4.0b0/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:34:18.627265 digitalhub_ml-0.4.0b0/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      550 2024-04-17 12:34:18.000000 digitalhub_ml-0.4.0b0/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      864 2024-04-17 12:34:18.000000 digitalhub_ml-0.4.0b0/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-17 12:34:18.000000 digitalhub_ml-0.4.0b0/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-17 12:34:18.000000 digitalhub_ml-0.4.0b0/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-04-17 12:34:18.000000 digitalhub_ml-0.4.0b0/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-17 12:34:18.631265 digitalhub_ml-0.4.0b0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-19 08:38:22.000000 digitalhub_ml-0.4.0b1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6252 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6786 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5788 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      991 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      864 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-04-19 08:46:19.000000 digitalhub_ml-0.4.0b1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/setup.cfg
```

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/crud.py` & `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/entity.py` & `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,18 +142,15 @@
         return get_context(self.project)
 
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
         obj : dict
             Dictionary to parse.
```

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml/entities/models/spec.py` & `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/crud.py` & `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/entity.py` & `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,18 +116,15 @@
         -------
         list[dict]
             List of objects related to project.
         """
         return list_models(self.name, **kwargs)
 
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

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml/entities/projects/spec.py` & `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml/entities/registries.py` & `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b0/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b0/pyproject.toml` & `digitalhub_ml-0.4.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
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
     "digitalhub-data~=0.3",
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

