# Comparing `tmp/pyramid_blacksmith-2.1.0.tar.gz` & `tmp/pyramid_blacksmith-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramid_blacksmith-2.1.0.tar", max compression
+gzip compressed data, was "pyramid_blacksmith-2.2.0.tar", max compression
```

## Comparing `pyramid_blacksmith-2.1.0.tar` & `pyramid_blacksmith-2.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1528 2023-11-29 16:13:04.337517 pyramid_blacksmith-2.1.0/LICENSE
--rw-r--r--   0        0        0     1651 2023-11-29 16:13:04.337517 pyramid_blacksmith-2.1.0/README.rst
--rw-r--r--   0        0        0     1636 2023-12-01 14:41:40.789429 pyramid_blacksmith-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      497 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/__init__.py
--rw-r--r--   0        0        0    11450 2023-12-01 14:41:33.042656 pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/binding.py
--rw-r--r--   0        0        0     2925 2023-12-01 14:41:33.042656 pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/middleware.py
--rw-r--r--   0        0        0      976 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/middleware_factory.py
--rw-r--r--   0        0        0        0 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/py.typed
--rw-r--r--   0        0        0       57 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/typing.py
--rw-r--r--   0        0        0     1278 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/utils.py
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 pyramid_blacksmith-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1528 2023-11-29 16:13:04.337517 pyramid_blacksmith-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1651 2023-11-29 16:13:04.337517 pyramid_blacksmith-2.2.0/README.rst
+-rw-r--r--   0        0        0     1706 2024-04-19 15:19:30.683164 pyramid_blacksmith-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      497 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:57:33.929741 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/adapters/__init__.py
+-rw-r--r--   0        0        0     2108 2024-04-19 14:57:33.929741 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/adapters/zipkin.py
+-rw-r--r--   0        0        0    11519 2024-04-19 14:57:33.929741 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/binding.py
+-rw-r--r--   0        0        0     3196 2024-04-19 14:57:33.929741 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/middleware.py
+-rw-r--r--   0        0        0      976 2024-04-12 15:22:30.522733 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/middleware_factory.py
+-rw-r--r--   0        0        0        0 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/py.typed
+-rw-r--r--   0        0        0       57 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/typing.py
+-rw-r--r--   0        0        0     1278 2023-11-29 16:13:04.344183 pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/utils.py
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 pyramid_blacksmith-2.2.0/PKG-INFO
```

### Comparing `pyramid_blacksmith-2.1.0/LICENSE` & `pyramid_blacksmith-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyramid_blacksmith-2.1.0/README.rst` & `pyramid_blacksmith-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyramid_blacksmith-2.1.0/pyproject.toml` & `pyramid_blacksmith-2.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -9,41 +9,44 @@
   "Topic :: Internet :: WWW/HTTP",
 ]
 description = "Pyramid Bindings for Blacksmith"
 homepage = "https://github.com/mardiros/pyramid-blacksmith"
 name = "pyramid-blacksmith"
 readme = "README.rst"
 repository = "https://github.com/mardiros/pyramid-blacksmith"
-version = "2.1.0"
+version = "2.2.0"
 
 [tool.poetry.dependencies]
-blacksmith = "^2.0.0"
+blacksmith = "^2.7.2"
 pyramid = ">1.10, <3"
 prometheus-client = ">0.14"
 python = "^3.7"
+zk = { version = "^0.8.5", extras = ["zipkin"] }
 
-[tool.poetry.dev-dependencies]
+
+[tool.poetry.extras]
+prometheus = ["prometheus-client"]
+
+[tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
-coverage = {version = "^6.2", extras = ["toml"]}
+coverage = { version = "^6.2", extras = ["toml"] }
 esbonio = "^0.14.1"
 flake8 = "^4.0.1"
 furo = "^2022"
 isort = "^5.10.1"
-mypy = "^0.982"
+mypy = "^1.4"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 redis = "^4.1.0"
 sphinx = "^4.2.0"
 sphinx-autodoc-typehints = "^1.12.0"
 tomlkit = "^0.11.5"
 types-redis = "^4.1.8"
 types-setuptools = "^57.4.7"
-
-[tool.poetry.extras]
-prometheus = ["prometheus-client"]
+zk = "^0.8.5"
 
 [tool.pytest.ini_options]
 norecursedirs = "docs"
 
 [tool.pyright]
 ignore = ["examples"]
 include = ["src"]
```

### Comparing `pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/binding.py` & `pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
             self.settings.get(f"{self.prefix}.middlewares", []), flatten=False
         )
         classes = {
             "prometheus": "pyramid_blacksmith.middleware:PrometheusMetricsBuilder",
             "circuitbreaker": "pyramid_blacksmith.middleware:CircuitBreakerBuilder",
             "http_cache": "pyramid_blacksmith.middleware:HTTPCacheBuilder",
             "static_headers": "pyramid_blacksmith.middleware:HTTPStaticHeadersBuilder",
+            "zipkin": "pyramid_blacksmith.middleware:ZipkinBuilder",
         }
         for middleware in value:
             try:
                 middleware, cls = middleware.split(maxsplit=1)
             except ValueError:
                 cls = classes.get(middleware, middleware)
             cls = resolve_entrypoint(cls)
```

### Comparing `pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/middleware.py` & `pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,20 @@
     PrometheusMetrics,
     SyncCircuitBreakerMiddleware,
     SyncHTTPAddHeadersMiddleware,
     SyncHTTPCacheMiddleware,
     SyncHTTPMiddleware,
     SyncPrometheusMiddleware,
 )
+from blacksmith.middleware._sync.zipkin import SyncZipkinMiddleware
 from pyramid.exceptions import ConfigurationError  # type: ignore
 
 from pyramid_blacksmith.typing import Settings
 
+from .adapters.zipkin import TraceContext
 from .utils import list_to_dict, resolve_entrypoint
 
 
 class AbstractMiddlewareBuilder(abc.ABC):
     def __init__(
         self,
         settings: Settings,
@@ -78,7 +80,12 @@
 
 
 class HTTPStaticHeadersBuilder(AbstractMiddlewareBuilder):
     def build(self) -> SyncHTTPAddHeadersMiddleware:
         settings = list_to_dict(self.settings, self.prefix)
         headers = {key.rstrip(":"): val for key, val in settings.items()}
         return SyncHTTPAddHeadersMiddleware(headers)
+
+
+class ZipkinBuilder(AbstractMiddlewareBuilder):
+    def build(self) -> SyncZipkinMiddleware:
+        return SyncZipkinMiddleware(TraceContext)  # type: ignore
```

### Comparing `pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/middleware_factory.py` & `pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/middleware_factory.py`

 * *Files identical despite different names*

### Comparing `pyramid_blacksmith-2.1.0/src/pyramid_blacksmith/utils.py` & `pyramid_blacksmith-2.2.0/src/pyramid_blacksmith/utils.py`

 * *Files identical despite different names*

### Comparing `pyramid_blacksmith-2.1.0/PKG-INFO` & `pyramid_blacksmith-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid-blacksmith
-Version: 2.1.0
+Version: 2.2.0
 Summary: Pyramid Bindings for Blacksmith
 Home-page: https://github.com/mardiros/pyramid-blacksmith
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pyramid
@@ -16,17 +16,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: prometheus
-Requires-Dist: blacksmith (>=2.0.0,<3.0.0)
+Requires-Dist: blacksmith (>=2.7.2,<3.0.0)
 Requires-Dist: prometheus-client (>0.14) ; extra == "prometheus"
 Requires-Dist: pyramid (>1.10,<3)
+Requires-Dist: zk[zipkin] (>=0.8.5,<0.9.0)
 Project-URL: Repository, https://github.com/mardiros/pyramid-blacksmith
 Description-Content-Type: text/x-rst
 
 pyramid-blacksmith
 ==================
 
 .. image:: https://github.com/mardiros/pyramid-blacksmith/actions/workflows/gh-pages.yml/badge.svg
```

