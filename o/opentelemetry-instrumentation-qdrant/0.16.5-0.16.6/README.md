# Comparing `tmp/opentelemetry_instrumentation_qdrant-0.16.5.tar.gz` & `tmp/opentelemetry_instrumentation_qdrant-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.16.5.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.16.6.tar", max compression
```

## Comparing `opentelemetry_instrumentation_qdrant-0.16.5.tar` & `opentelemetry_instrumentation_qdrant-0.16.6.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      572 2024-04-17 04:27:26.213430 opentelemetry_instrumentation_qdrant-0.16.5/README.md
--rw-r--r--   0        0        0     1925 2024-04-17 04:27:26.213430 opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     2943 2024-04-17 04:27:26.213430 opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
--rw-r--r--   0        0        0     2828 2024-04-17 04:27:26.213430 opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
--rw-r--r--   0        0        0       23 2024-04-17 04:27:26.213430 opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/version.py
--rw-r--r--   0        0        0     3657 2024-04-17 04:27:26.213430 opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/wrapper.py
--rw-r--r--   0        0        0     1352 2024-04-17 04:27:55.961757 opentelemetry_instrumentation_qdrant-0.16.5/pyproject.toml
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.16.5/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/README.md
+-rw-r--r--   0        0        0     2114 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
+-rw-r--r--   0        0        0       42 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/config.py
+-rw-r--r--   0        0        0     2828 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
+-rw-r--r--   0        0        0      699 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/utils.py
+-rw-r--r--   0        0        0       23 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/version.py
+-rw-r--r--   0        0        0     3783 2024-04-19 09:17:49.328042 opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/wrapper.py
+-rw-r--r--   0        0        0     1352 2024-04-19 09:18:19.240252 opentelemetry_instrumentation_qdrant-0.16.6/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.16.6/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_qdrant-0.16.5/README.md` & `opentelemetry_instrumentation_qdrant-0.16.6/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/__init__.py` & `opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """OpenTelemetry Qdrant instrumentation"""
 
 import json
 import logging
 from pathlib import Path
+from opentelemetry.instrumentation.qdrant.config import Config
 from opentelemetry.instrumentation.qdrant.wrapper import _wrap
 import qdrant_client
 from typing import Collection
 from wrapt import wrap_function_wrapper
 
 
 from opentelemetry.trace import get_tracer
@@ -33,14 +34,18 @@
 
 MODULE = "qdrant_client"
 
 
 class QdrantInstrumentor(BaseInstrumentor):
     """An instrumentor for Qdrant's client library."""
 
+    def __init__(self, exception_logger=None):
+        super().__init__()
+        Config.exception_logger = exception_logger
+
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, __version__, tracer_provider)
         for wrapped_method in WRAPPED_METHODS:
```

### Comparing `opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.5/opentelemetry/instrumentation/qdrant/wrapper.py` & `opentelemetry_instrumentation_qdrant-0.16.6/opentelemetry/instrumentation/qdrant/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from opentelemetry import context as context_api
+from opentelemetry.instrumentation.qdrant.utils import dont_throw
 from opentelemetry.trace.status import Status, StatusCode
 from opentelemetry.instrumentation.utils import (
     _SUPPRESS_INSTRUMENTATION_KEY,
 )
 from opentelemetry.trace import SpanKind
 from opentelemetry.semconv.ai import SpanAttributes
 
@@ -70,39 +71,44 @@
 
         response = wrapped(*args, **kwargs)
         if response:
             span.set_status(Status(StatusCode.OK))
     return response
 
 
+@dont_throw
 def _set_collection_name_attribute(span, method, args, kwargs):
     _set_span_attribute(
         span,
         f"qdrant.{method}.collection_name",
         kwargs.get("collection_name") or args[0],
     )
 
 
+@dont_throw
 def _set_upsert_attributes(span, args, kwargs):
     points = kwargs.get("points") or args[1]
     if isinstance(points, list):
         length = len(points)
     else:
         length = len(
             points.ids
         )  # If using models.Batch instead of list[models.PointStruct]
     _set_span_attribute(span, "qdrant.upsert.points_count", length)
 
 
+@dont_throw
 def _set_upload_attributes(span, args, kwargs, method_name, param_name):
     points = list(kwargs.get(param_name) or args[1])
     _set_span_attribute(span, f"qdrant.{method_name}.points_count", len(points))
 
 
+@dont_throw
 def _set_search_attributes(span, args, kwargs):
     limit = kwargs.get("limit") or 10
     _set_span_attribute(span, SpanAttributes.VECTOR_DB_QUERY_TOP_K, limit)
 
 
+@dont_throw
 def _set_batch_search_attributes(span, args, kwargs, method):
     requests = kwargs.get("requests") or []
     _set_span_attribute(span, f"qdrant.{method}.requests_count", len(requests))
```

### Comparing `opentelemetry_instrumentation_qdrant-0.16.5/pyproject.toml` & `opentelemetry_instrumentation_qdrant-0.16.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-qdrant"
-version = "0.16.5"
+version = "0.16.6"
 description = "OpenTelemetry Qdrant instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant"
```

### Comparing `opentelemetry_instrumentation_qdrant-0.16.5/PKG-INFO` & `opentelemetry_instrumentation_qdrant-0.16.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-qdrant
-Version: 0.16.5
+Version: 0.16.6
 Summary: OpenTelemetry Qdrant instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-qdrant Version:
-0.16.5 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
+0.16.6 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-qdrant License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

