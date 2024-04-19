# Comparing `tmp/valor_client-0.21.2.tar.gz` & `tmp/valor_client-0.21.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.21.2.tar", last modified: Wed Apr 17 18:20:10 2024, max compression
+gzip compressed data, was "valor_client-0.21.3.tar", last modified: Fri Apr 19 17:21:04 2024, max compression
```

## Comparing `valor_client-0.21.2.tar` & `valor_client-0.21.3.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.536908 valor_client-0.21.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 18:20:03.000000 valor_client-0.21.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 18:20:10.536908 valor_client-0.21.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 18:20:03.000000 valor_client-0.21.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:20:10.540909 valor_client-0.21.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 18:20:03.000000 valor_client-0.21.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.532909 valor_client-0.21.2/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.532909 valor_client-0.21.2/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.532909 valor_client-0.21.2/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.532909 valor_client-0.21.2/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.532909 valor_client-0.21.2/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12523 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.532909 valor_client-0.21.2/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    34427 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-17 18:20:03.000000 valor_client-0.21.2/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.536908 valor_client-0.21.2/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53932 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.536908 valor_client-0.21.2/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.536908 valor_client-0.21.2/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58814 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-17 18:20:03.000000 valor_client-0.21.2/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:20:10.536908 valor_client-0.21.2/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 18:20:10.000000 valor_client-0.21.2/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-17 18:20:10.000000 valor_client-0.21.2/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:20:10.000000 valor_client-0.21.2/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 18:20:10.000000 valor_client-0.21.2/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 18:20:10.000000 valor_client-0.21.2/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.637343 valor_client-0.21.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 17:21:00.000000 valor_client-0.21.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-19 17:21:04.637343 valor_client-0.21.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 17:21:00.000000 valor_client-0.21.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:21:04.637343 valor_client-0.21.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 17:21:00.000000 valor_client-0.21.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53334 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.21.2/LICENSE` & `valor_client-0.21.3/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/PKG-INFO` & `valor_client-0.21.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.21.2
+Version: 0.21.3
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.21.2/pyproject.toml` & `valor_client-0.21.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/conftest.py` & `valor_client-0.21.3/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/coretypes/test_core.py` & `valor_client-0.21.3/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.21.3/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/coretypes/test_filtering.py` & `valor_client-0.21.3/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/schemas/test_filters.py` & `valor_client-0.21.3/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/schemas/test_geojson.py` & `valor_client-0.21.3/unit-tests/schemas/test_geojson.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     # test property 'ymin'
     assert poly.ymin == 0
 
     # test property 'ymax'
     assert poly.ymax == 5
 
 
-def test_boundingbox():
+def test_box():
     p1 = (-1, -2)
     p2 = (10, -2)
     p3 = (10, 11)
     p4 = (-1, 11)
     coords = [[p1, p2, p3, p4, p1]]
 
     # test validation
```

### Comparing `valor_client-0.21.2/unit-tests/schemas/test_label.py` & `valor_client-0.21.3/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.21.3/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     metadata["f"] = datetime.time.fromisoformat("12:12:12:100000")
     metadata["g"] = datetime.timedelta(days=1)
     assert Dictionary(metadata).get_value() == metadata
 
     assert Dictionary(metadata).to_dict() == {
         "type": "dictionary",
         "value": {
-            "a": {"type": "integer", "value": 123},
-            "b": {"type": "float", "value": 123.4},
-            "c": {"type": "string", "value": "123.4"},
+            "a": 123,
+            "b": 123.4,
+            "c": "123.4",
             "d": {"type": "datetime", "value": "2023-01-01T12:12:12"},
             "e": {"type": "date", "value": "2023-01-01"},
             "f": {"type": "time", "value": "12:12:12.100000"},
             "g": {"type": "duration", "value": 86400.0},
         },
     }
 
@@ -62,17 +62,17 @@
     metadata["c"] = str(123.4)
     metadata["d"] = datetime.datetime.fromisoformat("2023-01-01T12:12:12")
     metadata["e"] = datetime.date.fromisoformat("2023-01-01")
     metadata["f"] = datetime.time.fromisoformat("12:12:12:100000")
     metadata["g"] = datetime.timedelta(days=1)
 
     metadata_json = {
-        "a": {"type": "integer", "value": 123},
-        "b": {"type": "float", "value": 123.4},
-        "c": {"type": "string", "value": "123.4"},
+        "a": 123,
+        "b": 123.4,
+        "c": "123.4",
         "d": {"type": "datetime", "value": "2023-01-01T12:12:12"},
         "e": {"type": "date", "value": "2023-01-01"},
         "f": {"type": "time", "value": "12:12:12.100000"},
         "g": {"type": "duration", "value": 86400.0},
     }
 
     assert Dictionary(metadata).encode_value() == metadata_json
```

### Comparing `valor_client-0.21.2/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.21.3/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.21.3/unit-tests/symbolic/collections/test_structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -393,28 +393,49 @@
     v2 = objcls.nullable(permutations[0][0])
     assert v2.get_value() is not None
     assert v2.is_none().get_value() is False  # type: ignore - always a bool
     assert v2.is_not_none().get_value() is True  # type: ignore - always a bool
 
     # test encoding
     assert {
-        "k0": {"type": "bool", "value": True},
-        "k1": {"type": "string", "value": "v1"},
-        "k2": {"type": "integer", "value": 123},
-        "k3": {"type": "float", "value": 1.24},
+        "k0": True,
+        "k1": "v1",
+        "k2": 123,
+        "k3": 1.24,
         "k4": {"type": "datetime", "value": "2024-01-01T00:00:00"},
         "k5": {"type": "date", "value": "2024-01-01"},
         "k6": {"type": "time", "value": "01:00:00"},
         "k7": {"type": "duration", "value": 100.0},
-        "k8": {"type": "point", "value": (1, -1)},
-        "k9": {"type": "multipoint", "value": [(0, 0), (1, 1)]},
-        "k10": {"type": "linestring", "value": [(0, 0), (1, 1)]},
-        "k11": {"type": "multilinestring", "value": [[(0, 0), (1, 1)]]},
+        "k8": {
+            "type": "geojson",
+            "value": {"type": "Point", "coordinates": (1, -1)},
+        },
+        "k9": {
+            "type": "geojson",
+            "value": {"type": "MultiPoint", "coordinates": [(0, 0), (1, 1)]},
+        },
+        "k10": {
+            "type": "geojson",
+            "value": {"type": "LineString", "coordinates": [(0, 0), (1, 1)]},
+        },
+        "k11": {
+            "type": "geojson",
+            "value": {
+                "type": "MultiLineString",
+                "coordinates": [[(0, 0), (1, 1)]],
+            },
+        },
         "k12": {
-            "type": "polygon",
-            "value": [[(0, 0), (1, 1), (0, 1), (0, 0)]],
+            "type": "geojson",
+            "value": {
+                "type": "Polygon",
+                "coordinates": [[(0, 0), (1, 1), (0, 1), (0, 0)]],
+            },
         },
         "k13": {
-            "type": "multipolygon",
-            "value": [[[(0, 0), (1, 1), (0, 1), (0, 0)]]],
+            "type": "geojson",
+            "value": {
+                "type": "MultiPolygon",
+                "coordinates": [[[(0, 0), (1, 1), (0, 1), (0, 0)]]],
+            },
         },
     } == Dictionary(x).encode_value()
```

### Comparing `valor_client-0.21.2/unit-tests/symbolic/test_operators.py` & `valor_client-0.21.3/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.21.3/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.21.3/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,35 @@
             "owner": "some_owner",
             "name": "some_name",
             "key": "some_key",
             "attribute": "some_attribute",
         },
     }
 
+    # test '__eq__'
+    assert s == Symbol(
+        owner="some_owner",
+        name="some_name",
+        attribute="some_attribute",
+        key="some_key",
+    )
+    assert not (s == "symbol")
+
+    # test '__ne__'
+    assert not (
+        s
+        != Symbol(
+            owner="some_owner",
+            name="some_name",
+            attribute="some_attribute",
+            key="some_key",
+        )
+    )
+    assert s != "symbol"
+
 
 def _test_symbolic_outputs(v, s=Symbol(name="test")):
     assert s.to_dict() == v.to_dict()
     assert s.to_dict() == v.get_symbol().to_dict()
     assert s.__repr__() == v.__repr__()
     assert s.__str__() == v.__str__()
     assert v.is_symbolic and not v.is_value
@@ -81,17 +102,48 @@
     # test symbolic variables
 
     var_method1 = Variable.symbolic(name="test")
     var_method2 = Variable.preprocess(value=Symbol(name="test"))
     _test_symbolic_outputs(var_method1)
     _test_symbolic_outputs(var_method2)
 
-    # nullable variables are not supported in the base class
-    with pytest.raises(NotImplementedError):
-        Variable.nullable("hello")
+    # test is_none
+    assert Variable.symbolic().is_none().to_dict() == {
+        "op": "isnull",
+        "arg": {
+            "type": "symbol",
+            "value": {
+                "name": "variable",
+                "owner": None,
+                "key": None,
+                "attribute": None,
+            },
+        },
+    }
+    assert Variable.symbolic().get_symbol() == Symbol(name="variable")
+    assert Variable(None).is_none().get_value() is True  # type: ignore - known output
+    assert Variable(1234).is_none().get_value() is False  # type: ignore - known output
+    with pytest.raises(TypeError):
+        Variable(1234).get_symbol()
+
+    # test is_not_none
+    assert Variable.symbolic().is_not_none().to_dict() == {
+        "op": "isnotnull",
+        "arg": {
+            "type": "symbol",
+            "value": {
+                "name": "variable",
+                "owner": None,
+                "key": None,
+                "attribute": None,
+            },
+        },
+    }
+    assert Variable(None).is_not_none().get_value() is False  # type: ignore - known output
+    assert Variable(1234).is_not_none().get_value() is True  # type: ignore - known output
 
 
 def _test_equatable(varA, varB, varC):
 
     # equal
     assert (varA == varB).to_dict() == {
         "op": "eq",
@@ -449,14 +501,16 @@
 
 
 def _test_encoding(objcls, value, encoded_value):
     assert (
         objcls(value).to_dict() == objcls.decode_value(encoded_value).to_dict()
     )
     assert encoded_value == objcls(value).encode_value()
+    assert objcls.decode_value(None) is None
+    assert objcls.nullable(None).encode_value() is None
 
 
 def _test_to_dict(objcls, value, type_name: typing.Optional[str] = None):
     type_name = type_name if type_name else objcls.__name__.lower()
     # test __init__
     assert objcls(value).to_dict() == {
         "type": type_name,
@@ -593,14 +647,48 @@
     assert v2.is_none().get_value() is False  # type: ignore - always a bool
     assert v2.is_not_none().get_value() is True  # type: ignore - always a bool
 
     # test encoding
     _test_encoding(objcls, True, True)
     _test_encoding(objcls, False, False)
 
+    # test and operation
+    assert (Bool(True) & Bool(True)).get_value() is True  # type: ignore - known output
+    assert (Bool(True) & Bool(False)).get_value() is False  # type: ignore - known output
+    assert (Bool(False) & Bool(True)).get_value() is False  # type: ignore - known output
+    assert (Bool(False) & Bool(False)).get_value() is False  # type: ignore - known output
+
+    # test or operation
+    assert (Bool(True) | Bool(True)).get_value() is True  # type: ignore - known output
+    assert (Bool(True) | Bool(False)).get_value() is True  # type: ignore - known output
+    assert (Bool(False) | Bool(True)).get_value() is True  # type: ignore - known output
+    assert (Bool(False) | Bool(False)).get_value() is False  # type: ignore - known output
+
+    # test xor operation
+    assert (Bool(True) ^ Bool(True)).get_value() is False  # type: ignore - known output
+    assert (Bool(True) ^ Bool(False)).get_value() is True  # type: ignore - known output
+    assert (Bool(False) ^ Bool(True)).get_value() is True  # type: ignore - known output
+    assert (Bool(False) ^ Bool(False)).get_value() is False  # type: ignore - known output
+
+    # test negation operation
+    assert (~Bool(True)).get_value() is False  # type: ignore - known output
+    assert (~Bool(False)).get_value() is True  # type: ignore - known output
+    assert (~Bool.symbolic()).to_dict() == {
+        "op": "negate",
+        "arg": {
+            "type": "symbol",
+            "value": {
+                "owner": None,
+                "name": "bool",
+                "key": None,
+                "attribute": None,
+            },
+        },
+    }
+
 
 def test_integer():
     # interoperable with builtin 'int'
     objcls = Integer
     permutations = [
         (100, 100),
         (100, -100),
@@ -619,14 +707,20 @@
         "__xor__",
         "intersects",
         "inside",
         "outside",
     ]:
         _test_unsupported(objcls, permutations, op)
 
+    # test equatable
+    assert (Integer.nullable(None) == Integer(1)).get_value() is False  # type: ignore - always a bool
+    assert (Integer(1) == Integer.nullable(None)).get_value() is False  # type: ignore - always a bool
+    assert (Integer.nullable(None) != Integer(1)).get_value() is True  # type: ignore - always a bool
+    assert (Integer(1) != Integer.nullable(None)).get_value() is True  # type: ignore - always a bool
+
     # test nullable
     v1 = objcls.nullable(None)
     assert v1.get_value() is None
     assert v1.is_none().get_value() is True  # type: ignore - always a bool
     assert v1.is_not_none().get_value() is False  # type: ignore - always a bool
     v2 = objcls.nullable(permutations[0][0])
     assert v2.get_value() is not None
```

### Comparing `valor_client-0.21.2/unit-tests/test_client.py` & `valor_client-0.21.3/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/unit-tests/test_viz.py` & `valor_client-0.21.3/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/__init__.py` & `valor_client-0.21.3/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/client.py` & `valor_client-0.21.3/valor/client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/coretypes.py` & `valor_client-0.21.3/valor/coretypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     EvaluationParameters,
     EvaluationRequest,
     Filter,
     Label,
 )
 from valor.schemas import List as SymbolicList
 from valor.schemas import StaticCollection, String
-from valor.schemas.compatibility import decode_api_format, encode_api_format
 
 FilterType = Union[list, dict, Filter]  # TODO - Remove this
 
 
 def _format_filter(filter_by: Optional[FilterType]) -> Filter:
     """
     Formats the various filter or constraint representations into a 'schemas.Filter' object.
@@ -693,16 +692,14 @@
         ----------
         name : String
             The name of the model.
         metadata : Dictionary
             A dictionary of metadata that describes the model.
         connection : ClientConnection, optional
             An initialized client connection.
-        symbol : Symbol, optional
-            Symbol to represent a model.
         """
         self.conn = connection
         super().__init__(name=name, metadata=metadata if metadata else dict())
 
     @classmethod
     def create(
         cls,
@@ -720,15 +717,14 @@
             The name of the model.
         metadata : dict, optional
             A dictionary of metadata that describes the model.
         connection : ClientConnection, optional
             An initialized client connection.
         """
         model = cls(name=name, metadata=metadata, connection=connection)
-        model.add_connection(connection)
         Client(connection).create_model(model)
         return model
 
     @classmethod
     def get(
         cls,
         name: str,
@@ -747,25 +743,14 @@
         Returns
         -------
         Union[valor.Model, None]
             The model or 'None' if it doesn't exist.
         """
         return Client(connection).get_model(name)
 
-    def add_connection(self, connection: Optional[ClientConnection]):
-        """
-        Stores a pre-existing connection.
-
-        Parameters
-        ----------
-        connection : ClientConnnetion, optional
-            An optional Valor client object for interacting with the API.
-        """
-        self.conn = connection
-
     def add_prediction(
         self,
         dataset: Dataset,
         prediction: Prediction,
     ) -> None:
         """
         Add a prediction to the model.
@@ -1213,15 +1198,15 @@
 
         Parameters
         ----------
         dataset : valor.Dataset
             The dataset to create.
         """
         if isinstance(dataset, Dataset):
-            dataset = encode_api_format(dataset)
+            dataset = dataset.encode_value()
         self.conn.create_dataset(dataset)
 
     def create_groundtruths(
         self,
         dataset: Dataset,
         groundtruths: List[GroundTruth],
     ):
@@ -1240,16 +1225,16 @@
         for groundtruth in groundtruths:
             if not isinstance(groundtruth, GroundTruth):
                 raise TypeError(
                     f"Expected ground truth to be of type 'valor.GroundTruth' not '{type(groundtruth)}'."
                 )
             if not isinstance(groundtruth.annotations._value, list):
                 raise TypeError
-            groundtruth_dict = encode_api_format(groundtruth)
-            groundtruth_dict["datum"]["dataset_name"] = dataset.get_name()
+            groundtruth_dict = groundtruth.encode_value()
+            groundtruth_dict["dataset_name"] = dataset.get_name()
             groundtruths_json.append(groundtruth_dict)
         self.conn.create_groundtruths(groundtruths_json)
 
     def get_groundtruth(
         self,
         dataset: Union[Dataset, str],
         datum: Union[Datum, str],
@@ -1273,16 +1258,16 @@
             dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
         datum_uid = datum.get_uid() if isinstance(datum, Datum) else datum
         try:
             resp = self.conn.get_groundtruth(
                 dataset_name=dataset_name, datum_uid=datum_uid
             )
-            resp = decode_api_format(resp)
-            return GroundTruth(**resp)
+            resp.pop("dataset_name")
+            return GroundTruth.decode_value(resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def finalize_dataset(self, dataset: Union[Dataset, str]) -> None:
         """
@@ -1312,18 +1297,19 @@
 
         Returns
         -------
         Union[Dataset, None]
             A Dataset with a matching name, or 'None' if one doesn't exist.
         """
         try:
-            resp = decode_api_format(self.conn.get_dataset(name))
-            dataset = Dataset(
-                **resp,
-                connection=self.conn,
+            dataset = Dataset.decode_value(
+                {
+                    **self.conn.get_dataset(name),
+                    "connection": self.conn,
+                }
             )
             return dataset
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
@@ -1345,16 +1331,15 @@
             A list of datasets.
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
         dataset_list = []
         for kwargs in self.conn.get_datasets(filter_):
-            kwargs = decode_api_format(kwargs)
-            dataset = Dataset(**kwargs, connection=self.conn)
+            dataset = Dataset.decode_value({**kwargs, "connection": self.conn})
             dataset_list.append(dataset)
         return dataset_list
 
     def get_datums(
         self,
         filter_by: Optional[FilterType] = None,
     ) -> List[Datum]:
@@ -1371,15 +1356,15 @@
         List[valor.Datum]
             A list datums.
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
         return [
-            Datum(**decode_api_format(datum))
+            Datum.decode_value(datum)
             for datum in self.conn.get_datums(filter_)
         ]
 
     def get_datum(
         self,
         dataset: Union[Dataset, str],
         uid: str,
@@ -1399,16 +1384,15 @@
             The requested datum or 'None' if it doesn't exist.
         """
         dataset_name = (
             dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
         try:
             resp = self.conn.get_datum(dataset_name=dataset_name, uid=uid)
-            resp = decode_api_format(resp)
-            return Datum(**resp)
+            return Datum.decode_value(resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def get_dataset_status(
         self,
@@ -1482,15 +1466,15 @@
 
         Parameters
         ----------
         model : valor.Model
             The model to create.
         """
         if isinstance(model, Model):
-            model = encode_api_format(model)
+            model = model.encode_value()
         self.conn.create_model(model)
 
     def create_predictions(
         self,
         dataset: Dataset,
         model: Model,
         predictions: List[Prediction],
@@ -1511,16 +1495,16 @@
         for prediction in predictions:
             if not isinstance(prediction, Prediction):
                 raise TypeError(
                     f"Expected prediction to be of type 'valor.Prediction' not '{type(prediction)}'."
                 )
             if not isinstance(prediction.annotations._value, list):
                 raise TypeError
-            prediction_dict = encode_api_format(prediction)
-            prediction_dict["datum"]["dataset_name"] = dataset.get_name()
+            prediction_dict = prediction.encode_value()
+            prediction_dict["dataset_name"] = dataset.get_name()
             prediction_dict["model_name"] = model.get_name()
             predictions_json.append(prediction_dict)
         self.conn.create_predictions(predictions_json)
 
     def get_prediction(
         self,
         dataset: Union[Dataset, str],
@@ -1551,16 +1535,17 @@
         datum_uid = datum.get_uid() if isinstance(datum, Datum) else datum
         try:
             resp = self.conn.get_prediction(
                 dataset_name=dataset_name,
                 model_name=model_name,
                 datum_uid=datum_uid,
             )
-            resp = decode_api_format(resp)
-            return Prediction(**resp)
+            resp.pop("dataset_name")
+            resp.pop("model_name")
+            return Prediction.decode_value(resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def finalize_inferences(
         self, dataset: Union[Dataset, str], model: Union[Model, str]
@@ -1591,18 +1576,20 @@
 
         Returns
         -------
         Union[valor.Model, None]
             A Model with matching name or 'None' if one doesn't exist.
         """
         try:
-            resp = decode_api_format(self.conn.get_model(name))
-            model = Model(**resp)
-            model.add_connection(self.conn)
-            return model
+            return Model.decode_value(
+                {
+                    **self.conn.get_model(name),
+                    "connection": self.conn,
+                }
+            )
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def get_models(
         self,
@@ -1622,17 +1609,15 @@
             A list of models.
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
         model_list = []
         for kwargs in self.conn.get_models(filter_):
-            kwargs = decode_api_format(kwargs)
-            model = Model(**kwargs)
-            model.add_connection(self.conn)
+            model = Model.decode_value({**kwargs, "connection": self.conn})
             model_list.append(model)
         return model_list
 
     def get_model_status(
         self,
         dataset_name: str,
         model_name: str,
```

### Comparing `valor_client-0.21.2/valor/enums.py` & `valor_client-0.21.3/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/exceptions.py` & `valor_client-0.21.3/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/metatypes.py` & `valor_client-0.21.3/valor/metatypes.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 from valor.schemas import Integer
 
 
 class ImageMetadata:
     """
     A class describing the metadata for a particular image.
 
-    Parameters
+    Attributes
     ----------
-    uid : str
-        The UID of the image.
-    height : int
-        The height of the image.
-    width : int
-        The width of the image.
-    metadata : dict
-        A dictionary of metadata that describes the image.
+    datum : valor.Datum
+        The underlying datum object.
+    height: int
+        The height of the image in pixels.
+    width: int
+        The width of the image in pixels.
     """
 
     def __init__(self, datum: Datum):
         """
-        Creates an `ImageMetadata` object from a `Datum`.
+        Creates an `ImageMetadata` object from a `valor.Datum`.
 
         Parameters
         ----------
         datum : Datum
             The `Datum` to extract metadata from.
         """
         if not isinstance(datum, Datum):
@@ -46,14 +44,28 @@
     def create(
         cls,
         uid: str,
         height: int,
         width: int,
         metadata: Optional[dict] = None,
     ):
+        """
+        Create an instance of ImageMetadata using components.
+
+        Parameters
+        ----------
+        uid: str
+            The uid of the image.
+        height: int
+            The height of the image in pixels.
+        width: int
+            The width of the image in pixels.
+        metadata: dict, optional
+            Any other associated metadata.
+        """
         if not isinstance(height, int) or not isinstance(width, int):
             raise TypeError("Height and width must be integers.")
         metadata = metadata if metadata else dict()
         metadata["height"] = height
         metadata["width"] = width
         return cls(
             datum=Datum(
@@ -75,35 +87,41 @@
             The UID of the image.
         """
         width, height = image.size
         return cls.create(uid=uid, height=height, width=width)
 
     @property
     def height(self) -> int:
+        """Returns image height in pixels."""
         value = self.datum.metadata["height"].get_value()
         if not isinstance(value, int):
             raise TypeError
         return int(value)
 
     @property
     def width(self) -> int:
+        """Returns image width in pixels."""
         value = self.datum.metadata["width"].get_value()
         if not isinstance(value, int):
             raise TypeError
         return int(value)
 
 
 class VideoFrameMetadata:
     """
     A class describing the metadata for the frame of a video.
 
-    Parameters
+    Attributes
     ----------
-    image : ImageMetadata
-        Metadata describing the frame of the video.
+    datum : valor.Datum
+        The underlying datum object.
+    height: int
+        The height of the image in pixels.
+    width: int
+        The width of the image in pixels.
     frame: int
         The number of seconds into the video that the frame was taken.
     """
 
     def __init__(self, datum: Datum):
         """
         Creates a `VideoFrameMetadata` object from a `Datum`.
@@ -131,14 +149,30 @@
         cls,
         uid: str,
         height: int,
         width: int,
         frame: int,
         metadata: Optional[dict] = None,
     ):
+        """
+        Create an instance of VideoFrameMetadata using components.
+
+        Parameters
+        ----------
+        uid: str
+            The uid of the image.
+        height: int
+            The height of the image in pixels.
+        width: int
+            The width of the image in pixels.
+        frame: int
+            The video frame index.
+        metadata: dict, optional
+            Any other associated metadata.
+        """
         if (
             not isinstance(height, int)
             or not isinstance(width, int)
             or not isinstance(frame, int)
         ):
             raise TypeError("Height, width and frame must be integers.")
         metadata = metadata if metadata else dict()
@@ -150,25 +184,28 @@
                 uid=uid,
                 metadata=metadata,
             )
         )
 
     @property
     def height(self) -> int:
+        """Returns image height in pixels."""
         value = self.datum.metadata["height"].get_value()
         if not isinstance(value, int):
             raise TypeError
         return int(value)
 
     @property
     def width(self) -> int:
+        """Returns image width in pixels."""
         value = self.datum.metadata["width"].get_value()
         if not isinstance(value, int):
             raise TypeError
         return int(value)
 
     @property
     def frame(self) -> int:
+        """Returns the video frame number."""
         value = self.datum.metadata["frame"].get_value()
         if not isinstance(value, int):
             raise TypeError
         return int(value)
```

### Comparing `valor_client-0.21.2/valor/schemas/__init__.py` & `valor_client-0.21.3/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/schemas/evaluation.py` & `valor_client-0.21.3/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/schemas/filters.py` & `valor_client-0.21.3/valor/schemas/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 LineString,
                 MultiLineString,
                 Polygon,
                 MultiPolygon,
             ),
         ):
             value = {
-                "type": type(variable).__name__.capitalize(),
+                "type": type(variable).__name__,
                 "coordinates": variable.get_value(),
             }
         elif isinstance(variable, (DateTime, Date, Time, Duration)):
             value = {type(variable).__name__.lower(): variable.encode_value()}
         else:
             value = variable.encode_value()
     else:
```

### Comparing `valor_client-0.21.2/valor/schemas/symbolic/collections.py` & `valor_client-0.21.3/valor/schemas/symbolic/collections.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,15 +119,23 @@
             raise TypeError(
                 "A StaticCollection does not store an internal value."
             )
 
     @classmethod
     def decode_value(cls, value: dict):
         """Decode object from JSON compatible dictionary."""
-        return cls(**value)
+        kwargs = dict()
+        types = cls._get_static_types()
+        for k, v in value.items():
+            type_ = types.get(k)
+            if type_ and issubclass(type_, Variable):
+                kwargs[k] = type_.decode_value(v)
+            else:
+                kwargs[k] = v
+        return cls(**kwargs)
 
     def encode_value(self):
         """Encode object to JSON compatible dictionary."""
         return {
             k: v.encode_value() for k, v in self._get_dynamic_values().items()
         }
 
@@ -160,18 +168,14 @@
         return self.encode_value().__repr__()
 
     def __str__(self):
         if self.is_symbolic:
             return super().__str__()
         return str(self.encode_value())
 
-    @property
-    def is_symbolic(self) -> bool:
-        return super().is_symbolic
-
 
 class Label(StaticCollection):
     """
     An object for labeling datasets, models, and annotations.
 
     Attributes
     ----------
```

### Comparing `valor_client-0.21.2/valor/schemas/symbolic/operators.py` & `valor_client-0.21.3/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/schemas/symbolic/types.py` & `valor_client-0.21.3/valor/schemas/symbolic/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         value: typing.Optional[typing.Any],
     ):
         """
         Initialize variable with an optional.
 
         Parameters
         ----------
-        value : Any
+        value : typing.Any
             The intended value of the variable.
         """
         if value is None:
             obj = cls.__new__(cls)
             obj._value = None
             return obj
         else:
@@ -219,27 +219,22 @@
         )
 
     @classmethod
     def __validate__(cls, value: typing.Any):
         """
         Validates typing.
 
+        Intended to be overridden in subclasses.
+
         Parameters
         ----------
         value : typing.Any
             The value to validate.
-
-        Raises
-        ------
-        NotImplementedError
-            This function is not implemented in the base class.
         """
-        raise NotImplementedError(
-            f"Variable of type `{cls.__name__}` cannot be assigned a value."
-        )
+        pass
 
     @classmethod
     def supports(cls, value: typing.Any) -> bool:
         """
         Checks if value is a supported type.
 
         Returns
@@ -260,23 +255,14 @@
             return None
         return cls(value=value)
 
     def encode_value(self) -> typing.Any:
         """Encode object to JSON compatible dictionary."""
         return self.get_value()
 
-    @classmethod
-    def from_dict(cls, value: dict):
-        """Decode a JSON-compatible dictionary into an instance of the variable."""
-        if set(value.keys()) != {"type", "value"}:
-            raise KeyError
-        elif value["type"] != cls.__name__.lower():
-            raise TypeError
-        return cls.decode_value(value["value"])
-
     def to_dict(self) -> dict:
         """Encode variable to a JSON-compatible dictionary."""
         if isinstance(self._value, Symbol):
             return self._value.to_dict()
         else:
             return {
                 "type": type(self).__name__.lower(),
@@ -372,16 +358,14 @@
     """
     Implementation of the built-in type 'bool' as a Variable.
 
     Parameters
     ----------
     value : bool, optional
         A boolean value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> Bool(True)
     """
 
     def __init__(self, value: bool):
@@ -536,16 +520,14 @@
     """
     Implementation of the built-in type 'int' as a Variable.
 
     Parameters
     ----------
     value : int, optional
         A integer value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> Integer(123)
     """
 
     def __init__(self, value: int):
@@ -563,16 +545,14 @@
     """
     Implementation of the built-in type 'float' as a Variable.
 
     Parameters
     ----------
     value : float, optional
         A float value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> Float(3.14)
     """
 
     def __init__(self, value: float):
@@ -590,16 +570,14 @@
     """
     Implementation of the built-in type 'str' as a Variable.
 
     Parameters
     ----------
     value : str, optional
         A string value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> String("hello world")
     """
 
     def __init__(self, value: str):
@@ -617,16 +595,14 @@
     """
     Implementation of the type 'datetime.datetime' as a Variable.
 
     Parameters
     ----------
     value : datetime.datetime, optional
         A datetime value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> import datetime
     >>> DateTime(datetime.datetime(year=2024, month=1, day=1))
     """
 
@@ -659,16 +635,14 @@
     """
     Implementation of the type 'datetime.date' as a Variable.
 
     Parameters
     ----------
     value : datetime.date, optional
         A date value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> import datetime
     >>> Date(datetime.date(year=2024, month=1, day=1))
     """
 
@@ -701,16 +675,14 @@
     """
     Implementation of the type 'datetime.time' as a Variable.
 
     Parameters
     ----------
     value : datetime.time, optional
         A time value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> import datetime
     >>> Time(datetime.time(hour=1, minute=1))
     """
 
@@ -743,16 +715,14 @@
     """
     Implementation of the type 'datetime.timedelta' as a Variable.
 
     Parameters
     ----------
     value : datetime.timedelta, optional
         A time duration.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> import datetime
     >>> Duration(datetime.timedelta(seconds=100))
     """
 
@@ -787,16 +757,14 @@
 
     Follows the GeoJSON specification (RFC 7946).
 
     Parameters
     ----------
     value : Tuple[float, float], optional
         A point.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> Point((1,2))
     """
 
     def __init__(
@@ -863,16 +831,14 @@
 
     Follows the GeoJSON specification (RFC 7946).
 
     Parameters
     ----------
     value : List[Tuple[float, float]], optional
         A multipoint.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> MultiPoint([(0,0), (0,1), (1,1)])
     """
 
     def __init__(
@@ -906,16 +872,14 @@
 
     Follows the GeoJSON specification (RFC 7946).
 
     Parameters
     ----------
     value : List[Tuple[float, float]], optional
         A linestring.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Methods
     -------
     colorspace(c='rgb')
         Represent the photo in the given colorspace.
     gamma(n=1.0)
         Change the photo's gamma exposure.
@@ -953,16 +917,14 @@
 
     Follows the GeoJSON specification (RFC 7946).
 
     Parameters
     ----------
     value : List[List[Tuple[float, float]]], optional
         A multilinestring.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     Create a single line.
     >>> MultiLineString([[(0,0), (0,1), (1,1), (0,0)]])
 
     Create 3 lines.
@@ -1009,16 +971,14 @@
 
     Follows the GeoJSON specification (RFC 7946).
 
     Parameters
     ----------
     value : List[List[Tuple[float, float]]], optional
         A polygon.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Attributes
     ----------
     area
     boundary
     holes
     xmin
@@ -1165,16 +1125,14 @@
 
     Note that this does not need to be axis-aligned.
 
     Parameters
     ----------
     value : List[List[Tuple[float, float]]], optional
         An polygon value representing a box.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Attributes
     ----------
     area
     polygon
     boundary
     holes
@@ -1286,16 +1244,14 @@
 
     Follows the GeoJSON specification (RFC 7946).
 
     Parameters
     ----------
     value : List[List[List[Tuple[float, float]]]], optional
         A list of polygons.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Attributes
     ----------
     area
     polygons
 
     Examples
@@ -1404,16 +1360,14 @@
             """
             Strongly-typed variable list.
 
             Parameters
             ----------
             value : typing.List[T], optional
                 A list of items with type T.
-            symbol : Symbol, optional
-                A symbolic representation.
             """
 
             def __init__(
                 self,
                 value: typing.List[typing.Any],
             ):
                 if value is not None:
@@ -1608,16 +1562,14 @@
     """
     Symbolic implementation of the built-in type 'dict'.
 
     Parameters
     ----------
     value : Dict[str, typing.Any], optional
         A dictionary of items.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> v = Dictionary({"k1": "v1", "k2": 3.14})
     >>> s = Dictionary.symbolic(name="some_var")
 
     # Create an equality expression.
@@ -1656,27 +1608,74 @@
         for k, v in value.items():
             if not isinstance(k, str):
                 raise TypeError("Dictionary keys must be of type 'str'")
 
     @classmethod
     def decode_value(cls, value: dict) -> typing.Any:
         """Decode object from JSON compatible dictionary."""
-        return cls(
-            {
-                k: get_type_by_name(v["type"]).decode_value(v["value"])
-                for k, v in value.items()
-            }
-        )
+        decoded_value = dict()
+        for k, v in value.items():
+            if isinstance(
+                v,
+                (
+                    bool,
+                    int,
+                    float,
+                    str,
+                ),
+            ):
+                decoded_value[k] = v
+            elif v["type"].lower() == "geojson":
+                decoded_value[k] = get_type_by_name(
+                    v["value"]["type"].lower()
+                ).decode_value(v["value"]["coordinates"])
+            else:
+                decoded_value[k] = get_type_by_name(
+                    v["type"].lower()
+                ).decode_value(v["value"])
+        return cls(decoded_value)
 
     def encode_value(self) -> dict:
         """Encode object to JSON compatible dictionary."""
+        encoding = dict()
         value = self.get_value()
         if value is None:
-            return dict()
-        return {k: v.to_dict() for k, v in self.items()}
+            return encoding
+        for k, v in self.items():
+            if isinstance(
+                v,
+                (
+                    Point,
+                    MultiPoint,
+                    LineString,
+                    MultiLineString,
+                    Polygon,
+                    MultiPolygon,
+                ),
+            ):
+                encoding[k] = {
+                    "type": "geojson",
+                    "value": {
+                        "type": type(v).__name__,
+                        "coordinates": v.encode_value(),
+                    },
+                }
+            elif isinstance(
+                v,
+                (
+                    Bool,
+                    Integer,
+                    Float,
+                    String,
+                ),
+            ):
+                encoding[k] = v.encode_value()
+            else:
+                encoding[k] = v.to_dict()
+        return encoding
 
     def __getitem__(self, __key: str):
         if self.is_symbolic:
             symbol = self.get_symbol()
             return DictionaryValue.symbolic(
                 owner=symbol._owner,
                 name=symbol._name,
@@ -1712,16 +1711,14 @@
     """
     Variable wrapper for 'valor.enums.TaskType'.
 
     Parameters
     ----------
     value : typing.Union[str, valor.enums.TaskType], optional
         A task type enum value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
     Examples
     --------
     >>> from valor.enums import TaskType
     >>> TaskTypeEnum(TaskType.CLASSIFICATION)
     >>> TaskTypeEnum("classification")
     """
@@ -1771,18 +1768,16 @@
     """
     Represents a binary mask.
 
     Parameters
     ----------
     value : Dict[str, typing.Union[np.ndarray, str, None]], optional
         An raster value.
-    symbol : Symbol, optional
-        A symbolic representation.
 
-    Parameters
+    Attributes
     ----------
     area
     array
     geometry
     height
     width
 
@@ -2006,16 +2001,14 @@
     """
     Represents a model embedding.
 
     Parameters
     ----------
     value : List[float], optional
         An embedding value.
-    symbol : Symbol, optional
-        A symbolic representation.
     """
 
     def __init__(
         self, value: typing.Union[typing.List[int], typing.List[float]]
     ):
         """
         Initializes an embedding.
```

### Comparing `valor_client-0.21.2/valor/type_checks.py` & `valor_client-0.21.3/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.2/valor/viz.py` & `valor_client-0.21.3/valor/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,22 +54,21 @@
     task_type: Union[enums.TaskType, None] = None,
 ) -> Tuple[Image.Image, Dict[str, Image.Image]]:
     """
     Creates a combined segmentation mask from a list of segmentations.
 
     Parameters
     -------
-    annotated_datums : List[Union[GroundTruth, Prediction]]
+    annotated_datum : Union[GroundTruth, Prediction]
         A list of segmentations. These all must have the same `image` attribute.
     label_key : str
         The label key to use.
     task_type : enums.TaskType
         The associated task type.
 
-
     Returns
     -------
     tuple
         The first element of the tuple is the combined mask, as an RGB PIL image. The second
         element is a color legend: it's a dict with the unique labels as keys and the
         PIL image swatches as values.
```

### Comparing `valor_client-0.21.2/valor_client.egg-info/PKG-INFO` & `valor_client-0.21.3/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.21.2
+Version: 0.21.3
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.21.2/valor_client.egg-info/SOURCES.txt` & `valor_client-0.21.3/valor_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 valor/coretypes.py
 valor/enums.py
 valor/exceptions.py
 valor/metatypes.py
 valor/type_checks.py
 valor/viz.py
 valor/schemas/__init__.py
-valor/schemas/compatibility.py
 valor/schemas/evaluation.py
 valor/schemas/filters.py
 valor/schemas/symbolic/__init__.py
 valor/schemas/symbolic/collections.py
 valor/schemas/symbolic/operators.py
 valor/schemas/symbolic/types.py
 valor_client.egg-info/PKG-INFO
```

