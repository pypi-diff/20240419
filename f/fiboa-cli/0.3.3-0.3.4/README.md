# Comparing `tmp/fiboa-cli-0.3.3.tar.gz` & `tmp/fiboa_cli-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa-cli-0.3.3.tar", last modified: Fri Apr 12 14:10:20 2024, max compression
+gzip compressed data, was "fiboa_cli-0.3.4.tar", last modified: Fri Apr 19 11:49:53 2024, max compression
```

## Comparing `fiboa-cli-0.3.3.tar` & `fiboa_cli-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:10:20.877029 fiboa-cli-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-12 14:10:20.877029 fiboa-cli-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:10:20.877029 fiboa-cli-0.3.3/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/create_geoparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/rename_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:10:20.877029 fiboa-cli-0.3.3/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-12 14:10:20.000000 fiboa-cli-0.3.3/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-12 14:10:20.000000 fiboa-cli-0.3.3/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:10:20.000000 fiboa-cli-0.3.3/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 14:10:20.000000 fiboa-cli-0.3.3/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 14:10:20.000000 fiboa-cli-0.3.3/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 14:10:20.000000 fiboa-cli-0.3.3/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:10:20.877029 fiboa-cli-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:10:20.877029 fiboa-cli-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-12 14:10:16.000000 fiboa-cli-0.3.3/tests/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:49:53.961737 fiboa_cli-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-19 11:49:53.961737 fiboa_cli-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:49:53.961737 fiboa_cli-0.3.4/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/create_geoparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/rename_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:49:53.961737 fiboa_cli-0.3.4/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-19 11:49:53.000000 fiboa_cli-0.3.4/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-19 11:49:53.000000 fiboa_cli-0.3.4/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:49:53.000000 fiboa_cli-0.3.4/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 11:49:53.000000 fiboa_cli-0.3.4/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 11:49:53.000000 fiboa_cli-0.3.4/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 11:49:53.000000 fiboa_cli-0.3.4/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:49:53.961737 fiboa_cli-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:49:53.961737 fiboa_cli-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-19 11:49:50.000000 fiboa_cli-0.3.4/tests/test_jsonschema.py
```

### Comparing `fiboa-cli-0.3.3/LICENSE` & `fiboa_cli-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/PKG-INFO` & `fiboa_cli-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.3
+Version: 0.3.4
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa-cli-0.3.3/README.md` & `fiboa_cli-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/__init__.py` & `fiboa_cli-0.3.4/fiboa_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/convert.py` & `fiboa_cli-0.3.4/fiboa_cli/convert.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/convert_utils.py` & `fiboa_cli-0.3.4/fiboa_cli/convert_utils.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/create_geojson.py` & `fiboa_cli-0.3.4/fiboa_cli/create_geojson.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/create_geoparquet.py` & `fiboa_cli-0.3.4/fiboa_cli/create_geoparquet.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/geopandas.py` & `fiboa_cli-0.3.4/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/jsonschema.py` & `fiboa_cli-0.3.4/fiboa_cli/jsonschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from .util import load_datatypes, load_fiboa_schema
+from .util import log, load_datatypes, load_fiboa_schema
 from .jsonschema_template import jsonschema_template
 
 def jsonschema(config):
     core_schema = load_fiboa_schema(config)
     datatypes = load_datatypes(config['fiboa_version'])
     return create_jsonschema(core_schema, datatypes, config.get('id'))
 
@@ -89,15 +89,15 @@
         elif (isinstance(datatype_schema.get('type'), list)):
             datatype_schema.get('type', []).append("null")
         elif (isinstance(datatype_schema.get('oneOf'), list)):
             datatype_schema.get('oneOf', []).append({"type": "null"})
         elif (isinstance(datatype_schema.get('anyOf'), list)):
             datatype_schema.get('anyOf', []).append({"type": "null"})
         else:
-            print(f"Making schema {json.dumps(datatype_schema)} optional is not supported by this generator")
+            log(f"Making schema {json.dumps(datatype_schema)} optional is not supported by this generator")
 
     # Avoid conflicting statements
     if 'exclusiveMaximum' in prop_schema:
         datatype_schema.pop('maximum', None)
     if 'exclusiveMinimum' in prop_schema:
         datatype_schema.pop('minimum', None)
     if 'maximum' in prop_schema:
```

### Comparing `fiboa-cli-0.3.3/fiboa_cli/jsonschema_template.py` & `fiboa_cli-0.3.4/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/parquet.py` & `fiboa_cli-0.3.4/fiboa_cli/parquet.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/rename_extension.py` & `fiboa_cli-0.3.4/fiboa_cli/rename_extension.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/types.py` & `fiboa_cli-0.3.4/fiboa_cli/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,9 +185,7 @@
     "info": "white",
     "warning": "yellow",
     "error": "red",
     "success": "green"
 }
 
 SUPPORTED_PROTOCOLS = ["http", "https", "s3", "gs"]
-
-STAC_COLLECTION_SCHEMA = "http://schemas.stacspec.org/v1.0.0/collection-spec/json-schema/collection.json"
```

### Comparing `fiboa-cli-0.3.3/fiboa_cli/util.py` & `fiboa_cli-0.3.4/fiboa_cli/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from fsspec.implementations.http import HTTPFileSystem
 from fsspec.implementations.local import LocalFileSystem
 from pyarrow import NativeFile
 from pyarrow.fs import FSSpecHandler, PyFileSystem
 from tempfile import NamedTemporaryFile
 from typing import Union
 
-from .const import LOG_STATUS_COLOR, SUPPORTED_PROTOCOLS
+from .const import LOG_STATUS_COLOR, SUPPORTED_PROTOCOLS, STAC_COLLECTION_SCHEMA, GEOPARQUET_SCHEMA
 from .geopandas import decode_metadata, arrow_to_geopandas
 
 small_file_cache = {}
 big_file_cache = {}
 
 def log(text: str, status="info"):
     """Log a message with a severity level (which leads to different colors)"""
@@ -266,7 +266,30 @@
     iso = dt.isoformat()
     if iso.endswith("+00:00"):
         return iso[:-6] + "Z"
     elif re.search(r"[+-]\d{2}:\d{2}$", iso):
         raise ValueError("Timezone offset is not supported")
     else:
         return iso + "Z"
+
+
+def load_collection_schema(obj):
+    if "stac_version" in obj:
+        return load_file(STAC_COLLECTION_SCHEMA.format(version = obj["stac_version"]))
+    else:
+        return None
+
+
+def load_geoparquet_schema(obj):
+    if "version" in obj:
+        return load_file(GEOPARQUET_SCHEMA.format(version = obj["version"]))
+    else:
+        return None
+
+
+def log_extensions(collection, logger):
+    if len(collection["fiboa_extensions"]) == 0:
+        logger("fiboa extensions: none")
+    else:
+        logger("fiboa extensions:")
+        for ext in collection["fiboa_extensions"]:
+            logger(f"  - {ext}")
```

### Comparing `fiboa-cli-0.3.3/fiboa_cli/validate.py` & `fiboa_cli-0.3.4/fiboa_cli/validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import pyarrow.types as pat
 
 from jsonschema.validators import Draft7Validator
-from .const import STAC_COLLECTION_SCHEMA
 from .types import PA_TYPE_CHECK
 from .jsonschema import create_jsonschema
-from .util import get_collection, log as log_, load_datatypes, load_file, load_fiboa_schema, load_parquet_data, load_parquet_schema, merge_schemas
+from .util import get_collection, log as log_, log_extensions, load_datatypes, load_file, load_fiboa_schema, load_parquet_data, load_parquet_schema, merge_schemas, parse_metadata, load_collection_schema, load_geoparquet_schema
 from .validate_data import validate_column
 
-def log(text: str, status="info"):
+def log(text: str, status="info", bullet = True):
     # Indent logs
-    log_("  - " + str(text), status)
+    prefix = "  - " if bullet else "    "
+    log_(prefix + str(text), status)
 
 
 def validate(file, config):
     if file.endswith(".json") or file.endswith(".geojson"):
         return validate_geojson(file, config)
     else:
         return validate_parquet(file, config)
@@ -55,16 +55,15 @@
                     else:
                         path = ext
                     extensions[ext] = load_file(path)
                 except Exception as e:
                     log(f"Extension {ext} can't be loaded: {e}", "error")
                     valid = False
 
-    extension_info = ", ".join(collection["fiboa_extensions"]) or "none"
-    log("fiboa extensions: " + extension_info)
+    log_extensions(collection, lambda x: log(x, "info", False))
 
     return valid, extensions
 
 
 def validate_geojson(file, config):
     try:
         data = load_file(file)
@@ -143,37 +142,41 @@
                 log(f"{label}: VALID", "success")
 
     return valid
 
 
 def validate_parquet(file, config):
     parquet_schema = load_parquet_schema(file)
+    valid = True
 
     # Validate geo metadata in Parquet header
     if b"geo" not in parquet_schema.metadata:
         log("Parquet file schema does not have 'geo' key", "error")
         return False
     else:
-        # ToDo: We are not checking whether this is a valid GeoParquet file
-        log("The validator doesn't check whether this file contains valid GeoParquet metadata.", "info")
+        geo = parse_metadata(parquet_schema, b"geo")
+        if not validate_geoparquet_schema(geo):
+            valid = False
 
     # Validate fiboa metadata in Parquet header
     collection = {}
     if b"fiboa" not in parquet_schema.metadata:
         log("Parquet file schema does not have a 'fiboa' key", "warning")
         if not config.get("collection"):
             log("No collection specified", "error")
             return False
         else:
             collection = load_file(config.get("collection"))
     else:
-        collection = json.loads(parquet_schema.metadata[b"fiboa"])
+        collection = parse_metadata(parquet_schema, b"fiboa")
 
     # Validate Collection
-    valid, extensions = validate_collection(collection, config)
+    valid_collection, extensions = validate_collection(collection, config)
+    if not valid_collection:
+        valid = False
 
     # load the actual fiboa schema
     fiboa_schema = load_fiboa_schema(config)
 
     # Load data if needed
     gdf = None
     if config.get("data"):
@@ -255,26 +258,41 @@
     return valid
 
 
 # todo: use stac_validator instead of our own validation routine
 def validate_colletion_schema(obj):
     if "stac_version" in obj:
         try:
-            schema = load_file(STAC_COLLECTION_SCHEMA)
+            schema = load_collection_schema(obj)
             errors = validate_json_schema(obj, schema)
             for error in errors:
                 log(f"Collection: {error.path}: {error.message}", "error")
 
             return len(errors) == 0
         except Exception as e:
             log(f"Failed to validate STAC Collection due to an internal error: {e}", "warning")
 
     return True
 
 
+# todo: use a geoparquet validator instead of our own validation routine
+def validate_geoparquet_schema(obj):
+    if "version" in obj:
+        try:
+            schema = load_geoparquet_schema(obj)
+            errors = validate_json_schema(obj, schema)
+            for error in errors:
+                log(f"GeoParquet metadata: {error.path}: {error.message}", "error")
+
+            return len(errors) == 0
+        except Exception as e:
+            log(f"Failed to validate GeoParquet metadata due to an internal error: {e}", "error")
+
+    return False
+
 def validate_json_schema(obj, schema):
     if isinstance(obj, (bytearray, bytes, str)):
         obj = json.loads(obj)
 
     validator = Draft7Validator(schema)
     errors = sorted(validator.iter_errors(obj), key=lambda e: e.path)
     return errors
```

### Comparing `fiboa-cli-0.3.3/fiboa_cli/validate_data.py` & `fiboa_cli-0.3.4/fiboa_cli/validate_data.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli/validate_schema.py` & `fiboa_cli-0.3.4/fiboa_cli/validate_schema.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/fiboa_cli.egg-info/PKG-INFO` & `fiboa_cli-0.3.4/fiboa_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.3
+Version: 0.3.4
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa-cli-0.3.3/fiboa_cli.egg-info/SOURCES.txt` & `fiboa_cli-0.3.4/fiboa_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.3/setup.py` & `fiboa_cli-0.3.4/setup.py`

 * *Files identical despite different names*

