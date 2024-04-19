# Comparing `tmp/declare-1.0.0.tar.gz` & `tmp/declare-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declare-1.0.0.tar", max compression
+gzip compressed data, was "declare-1.0.1.tar", max compression
```

## Comparing `declare-1.0.0.tar` & `declare-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-04-12 11:18:31.938782 declare-1.0.0/LICENSE
--rw-r--r--   0        0        0     6045 2024-04-12 11:20:03.194526 declare-1.0.0/README.md
--rw-r--r--   0        0        0      332 2024-04-12 11:20:23.375409 declare-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      371 2024-04-12 11:18:31.948419 declare-1.0.0/src/declare/__init__.py
--rw-r--r--   0        0        0     6013 2024-04-12 11:18:31.949028 declare-1.0.0/src/declare/_declare.py
--rw-r--r--   0        0        0        0 2024-04-12 11:18:31.949073 declare-1.0.0/src/declare/py.typed
--rw-r--r--   0        0        0     6667 1970-01-01 00:00:00.000000 declare-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-12 11:18:31.938782 declare-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6263 2024-04-19 10:43:57.334602 declare-1.0.1/README.md
+-rw-r--r--   0        0        0      375 2024-04-19 10:47:05.309173 declare-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      348 2024-04-19 10:39:10.398990 declare-1.0.1/src/declare/__init__.py
+-rw-r--r--   0        0        0     6082 2024-04-19 10:39:10.399607 declare-1.0.1/src/declare/_declare.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:18:31.949073 declare-1.0.1/src/declare/py.typed
+-rw-r--r--   0        0        0     6834 1970-01-01 00:00:00.000000 declare-1.0.1/PKG-INFO
```

### Comparing `declare-1.0.0/LICENSE` & `declare-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `declare-1.0.0/README.md` & `declare-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -162,20 +162,25 @@
 
 # Why?
 
 Textual uses a similar approach to declare [reactive attributes](https://textual.textualize.io/guide/reactivity/), which are a useful general programming concept. Alas, without Textual as a runtime, it wouldn't be possible to use Textual's reactive attributes in another project. 
 
 This library extracts some of the core features and makes them work without any other dependencies.
 
-There is some overlap with dataclasses, [Pydantic](https://docs.pydantic.dev/latest/), [attrs](https://www.attrs.org/en/stable/), and other similar projects.
+There is some overlap with dataclasses, [traitlets](https://traitlets.readthedocs.io/en/stable/using_traitlets.html), [Pydantic](https://docs.pydantic.dev/latest/), [attrs](https://www.attrs.org/en/stable/), and other similar projects.
 But Declare isn't intended to replace any of these projects, which offer way more features.
 In fact, you can add Declared attributes to the class objects created by these other libraries.
 
 # How?
 
 In a word: ["descriptors"](https://mathspp.com/blog/pydonts/describing-descriptors).
 Python's descriptor protocol has been around forever, but remains a under used feature, IMHO.
 
 # Who?
 
 - [@willmcgugan](https://twitter.com/willmcgugan)
 - [mastodon.social/@willmcgugan](https://mastodon.social/@willmcgugan)
+
+
+# Thanks!
+
+A huge thank you to [Chris Cardillo](https://github.com/chriscardillo) who very kindly let me have the `declare` name on Pypi.
```

### Comparing `declare-1.0.0/src/declare/_declare.py` & `declare-1.0.1/src/declare/_declare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from __future__ import annotations
 
 from copy import copy
-from typing import Callable, cast, Generic, overload, Type, TypeVar
+from typing import TYPE_CHECKING, Generic, TypeVar, cast, overload
 
-from typing_extensions import TypeAlias
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from typing_extensions import TypeAlias
 
 
 ObjectType = TypeVar("ObjectType")
 ValueType = TypeVar("ValueType")
-Validator: TypeAlias = Callable[[ObjectType, ValueType], ValueType]
-Watcher: TypeAlias = Callable[[ObjectType, ValueType | None, ValueType], None]
+
+Validator: TypeAlias = "Callable[[ObjectType, ValueType], ValueType]"
+Watcher: TypeAlias = "Callable[[ObjectType, ValueType | None, ValueType], None]"
+
 ValidateMethodType = TypeVar("ValidateMethodType", bound=Validator)
 WatchMethodType = TypeVar("WatchMethodType", bound=Watcher)
 
 
 class NoValue:
     """Sentinel type."""
 
@@ -141,24 +146,24 @@
     def __set_name__(self, owner: Type, name: str) -> None:
         self._owner = owner
         self._name = name
         self._private_name = f"__declare_private_{name}"
 
     @overload
     def __get__(
-        self: Declare[ValueType], obj: None, obj_type: Type[ObjectType]
+        self: Declare[ValueType], obj: None, obj_type: type[ObjectType]
     ) -> Declare[ValueType]: ...
 
     @overload
     def __get__(
-        self: Declare[ValueType], obj: ObjectType, obj_type: Type[ObjectType]
+        self: Declare[ValueType], obj: ObjectType, obj_type: type[ObjectType]
     ) -> ValueType: ...
 
     def __get__(
-        self: Declare[ValueType], obj: ObjectType | None, obj_type: Type[ObjectType]
+        self: Declare[ValueType], obj: ObjectType | None, obj_type: type[ObjectType]
     ) -> Declare[ValueType] | ValueType:
         if obj is None:
             return self
         if isinstance((value := getattr(obj, self._private_name, _NO_VALUE)), NoValue):
             value = copy(self._default) if self._copy_default else self._default
             setattr(obj, self._private_name, value)
             return value
```

### Comparing `declare-1.0.0/PKG-INFO` & `declare-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: declare
-Version: 1.0.0
+Version: 1.0.1
 Summary: Declare attributes
 License: MIT
 Author: Will McGugan
 Author-email: willmcgugan@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # What?
 
 Declare is a syntactical sugar for adding attributes to Python classes, with support for validation and *watching* attributes for changes.
 
 Declare works well with type-checkers such as MyPy, even though in many cases you don't need to write type annotations.
@@ -180,21 +179,26 @@
 
 # Why?
 
 Textual uses a similar approach to declare [reactive attributes](https://textual.textualize.io/guide/reactivity/), which are a useful general programming concept. Alas, without Textual as a runtime, it wouldn't be possible to use Textual's reactive attributes in another project. 
 
 This library extracts some of the core features and makes them work without any other dependencies.
 
-There is some overlap with dataclasses, [Pydantic](https://docs.pydantic.dev/latest/), [attrs](https://www.attrs.org/en/stable/), and other similar projects.
+There is some overlap with dataclasses, [traitlets](https://traitlets.readthedocs.io/en/stable/using_traitlets.html), [Pydantic](https://docs.pydantic.dev/latest/), [attrs](https://www.attrs.org/en/stable/), and other similar projects.
 But Declare isn't intended to replace any of these projects, which offer way more features.
 In fact, you can add Declared attributes to the class objects created by these other libraries.
 
 # How?
 
 In a word: ["descriptors"](https://mathspp.com/blog/pydonts/describing-descriptors).
 Python's descriptor protocol has been around forever, but remains a under used feature, IMHO.
 
 # Who?
 
 - [@willmcgugan](https://twitter.com/willmcgugan)
 - [mastodon.social/@willmcgugan](https://mastodon.social/@willmcgugan)
 
+
+# Thanks!
+
+A huge thank you to [Chris Cardillo](https://github.com/chriscardillo) who very kindly let me have the `declare` name on Pypi.
+
```

