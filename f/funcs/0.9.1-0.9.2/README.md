# Comparing `tmp/funcs-0.9.1.tar.gz` & `tmp/funcs-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.9.1.tar", max compression
+gzip compressed data, was "funcs-0.9.2.tar", max compression
```

## Comparing `funcs-0.9.1.tar` & `funcs-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1092 2024-02-26 12:14:42.684979 funcs-0.9.1/LICENSE
--rw-r--r--   0        0        0     2870 2024-02-26 12:14:42.684979 funcs-0.9.1/README.md
--rw-r--r--   0        0        0     1740 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/__init__.py
--rw-r--r--   0        0        0      883 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/application.py
--rw-r--r--   0        0        0     1079 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/callers.py
--rw-r--r--   0        0        0     5470 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/composition.py
--rw-r--r--   0        0        0      832 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/debug.py
--rw-r--r--   0        0        0      436 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/decorators.py
--rw-r--r--   0        0        0     6369 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/flow.py
--rw-r--r--   0        0        0     2644 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/functions.py
--rw-r--r--   0        0        0      418 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/getters.py
--rw-r--r--   0        0        0      782 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/primitives.py
--rw-r--r--   0        0        0        0 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/py.typed
--rw-r--r--   0        0        0     1113 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/reduction.py
--rw-r--r--   0        0        0     1031 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/types.py
--rw-r--r--   0        0        0     2346 2024-02-26 12:14:42.684979 funcs-0.9.1/funcs/unpacking.py
--rw-r--r--   0        0        0     2491 2024-02-26 12:14:42.684979 funcs-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 funcs-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-15 10:34:26.228075 funcs-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2870 2024-03-15 10:34:26.228075 funcs-0.9.2/README.md
+-rw-r--r--   0        0        0     1740 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/application.py
+-rw-r--r--   0        0        0     1079 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/callers.py
+-rw-r--r--   0        0        0     5470 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/composition.py
+-rw-r--r--   0        0        0      832 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/debug.py
+-rw-r--r--   0        0        0      436 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/decorators.py
+-rw-r--r--   0        0        0     6365 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/flow.py
+-rw-r--r--   0        0        0     2644 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/functions.py
+-rw-r--r--   0        0        0      418 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/getters.py
+-rw-r--r--   0        0        0      782 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/py.typed
+-rw-r--r--   0        0        0     1113 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/reduction.py
+-rw-r--r--   0        0        0      705 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/types.py
+-rw-r--r--   0        0        0     2346 2024-03-15 10:34:26.228075 funcs-0.9.2/funcs/unpacking.py
+-rw-r--r--   0        0        0     2490 2024-03-15 10:34:26.228075 funcs-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 funcs-0.9.2/PKG-INFO
```

### Comparing `funcs-0.9.1/LICENSE` & `funcs-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/README.md` & `funcs-0.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.9.1"
+funcs = "^0.9.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.9.1/funcs/__init__.py` & `funcs-0.9.2/funcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import inspect, tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
```

### Comparing `funcs-0.9.1/funcs/application.py` & `funcs-0.9.2/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/funcs/callers.py` & `funcs-0.9.2/funcs/callers.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/funcs/composition.py` & `funcs-0.9.2/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/funcs/debug.py` & `funcs-0.9.2/funcs/debug.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/funcs/flow.py` & `funcs-0.9.2/funcs/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     SimpleContextManager,
     Unary,
     is_subclass,
 )
 from typing_extensions import ParamSpec
 
 from funcs.decorators import wraps
-from funcs.types import MarkerOr, is_not_marker, marker
+from funcs.types import MarkerOr, is_marker, marker
 
 __all__ = ("once", "reraise", "reraise_with", "suppress", "post_processing", "wrap_with")
 
 P = ParamSpec("P")
 
 R = TypeVar("R")
 S = TypeVar("S")
@@ -36,15 +36,15 @@
     """
     result: MarkerOr[R] = marker
 
     @wraps(function)
     def wrap(*args: P.args, **kwargs: P.kwargs) -> R:
         nonlocal result
 
-        if is_not_marker(result):
+        if not is_marker(result):
             return result
 
         result = function(*args, **kwargs)
 
         return result
 
     return wrap
```

### Comparing `funcs-0.9.1/funcs/functions.py` & `funcs-0.9.2/funcs/functions.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/funcs/primitives.py` & `funcs-0.9.2/funcs/primitives.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/funcs/reduction.py` & `funcs-0.9.2/funcs/reduction.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/funcs/types.py` & `funcs-0.9.2/funcs/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Any, TypeVar, Union
+from typing import TypeVar, Union
 
 from solus import Singleton
-from typing_extensions import TypeGuard
+from typing_extensions import TypeIs
 
-__all__ = ("Marker", "MarkerOr", "marker", "is_marker", "is_not_marker")
+__all__ = ("Marker", "MarkerOr", "marker", "is_marker")
 
 T = TypeVar("T")
 
 
 class Marker(Singleton):
     """Represents markers used in various checks."""
 
@@ -15,29 +15,17 @@
 marker = Marker()
 """The instance of [`Marker`][funcs.types.Marker]."""
 
 MarkerOr = Union[Marker, T]
 """The union of [`Marker`][funcs.types.Marker] and `T`."""
 
 
-def is_marker(item: Any) -> TypeGuard[Marker]:
+def is_marker(item: MarkerOr[T]) -> TypeIs[Marker]:
     """Checks if the given `item` is [`marker`][funcs.types.marker].
 
     Arguments:
         item: The item to check.
 
     Returns:
         Whether the given `item` is [`marker`][funcs.types.marker].
     """
     return item is marker
-
-
-def is_not_marker(item: MarkerOr[T]) -> TypeGuard[T]:
-    """Checks if the given `item` is *not* [`marker`][funcs.types.marker].
-
-    Arguments:
-        item: The item to check.
-
-    Returns:
-        Whether the given `item` is *not* [`marker`][funcs.types.marker].
-    """
-    return item is not marker
```

### Comparing `funcs-0.9.1/funcs/unpacking.py` & `funcs-0.9.2/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.9.1/pyproject.toml` & `funcs-0.9.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.9.1"
+version = "0.9.2"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -34,35 +34,35 @@
 
 typing-aliases = ">= 1.7.1"
 typing-extensions = ">= 4.10.0"
 
 solus = ">= 1.2.2"
 
 [tool.poetry.group.format.dependencies]
-ruff = "0.2.2"
+ruff = "0.3.2"
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.8.0"
+mypy = "1.9.0"
 
 [tool.poetry.group.check.dependencies.pre-commit]
 version = "3.6.2"
 python = ">= 3.9"
 
 [tool.poetry.group.test.dependencies]
-coverage = "7.4.3"
-pytest = "8.0.2"
+coverage = "7.4.4"
+pytest = "8.1.1"
 pytest-cov = "4.1.0"
-hypothesis = "6.98.12"
+hypothesis = "6.99.6"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
-mkdocs-material = "9.5.11"
+mkdocs-material = "9.5.13"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.24.0"
 extras = ["python"]
 
 [tool.poetry.group.release]
 optional = true
@@ -97,15 +97,15 @@
 directory = "coverage"
 
 [tool.mypy]
 strict = true
 
 [tool.changelogging]
 name = "funcs"
-version = "0.9.1"
+version = "0.9.2"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.9.1/PKG-INFO` & `funcs-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.9.1
+Version: 0.9.2
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,15 +71,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.9.1"
+funcs = "^0.9.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

