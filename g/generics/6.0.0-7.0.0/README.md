# Comparing `tmp/generics-6.0.0.tar.gz` & `tmp/generics-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generics-6.0.0.tar", max compression
+gzip compressed data, was "generics-7.0.0.tar", max compression
```

## Comparing `generics-6.0.0.tar` & `generics-7.0.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     1284 2022-10-18 19:29:25.976221 generics-6.0.0/LICENSE
--rw-r--r--   0        0        0     2341 2022-10-18 19:29:25.976221 generics-6.0.0/docs/index.md
--rw-r--r--   0        0        0      930 2022-10-18 19:33:56.735993 generics-6.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-18 19:29:25.980221 generics-6.0.0/src/_generics/__init__.py
--rw-r--r--   0        0        0      339 2022-10-18 19:33:15.411451 generics-6.0.0/src/_generics/delegate.py
--rw-r--r--   0        0        0      258 2022-10-18 19:29:25.980221 generics-6.0.0/src/_generics/exceptions.py
--rw-r--r--   0        0        0     6144 2022-10-18 19:33:43.591834 generics-6.0.0/src/_generics/private.py
--rw-r--r--   0        0        0      164 2022-10-18 19:29:25.980221 generics-6.0.0/src/generics/__init__.py
--rw-r--r--   0        0        0      262 2022-10-18 19:29:25.980221 generics-6.0.0/src/generics/exceptions.py
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 generics-6.0.0/setup.py
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 generics-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1284 2024-04-19 10:22:56.660787 generics-7.0.0/LICENSE
+-rw-r--r--   0        0        0     2368 2024-04-19 10:22:56.660787 generics-7.0.0/docs/index.md
+-rw-r--r--   0        0        0      916 2024-04-19 10:25:40.045302 generics-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 10:22:56.660787 generics-7.0.0/src/_generics/__init__.py
+-rw-r--r--   0        0        0      258 2024-04-19 10:22:56.660787 generics-7.0.0/src/_generics/exceptions.py
+-rw-r--r--   0        0        0     5762 2024-04-19 10:25:32.621279 generics-7.0.0/src/_generics/private.py
+-rw-r--r--   0        0        0       62 2024-04-19 10:22:56.660787 generics-7.0.0/src/generics/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-19 10:22:56.660787 generics-7.0.0/src/generics/exceptions.py
+-rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 generics-7.0.0/PKG-INFO
```

### Comparing `generics-6.0.0/LICENSE` & `generics-7.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020-2022 Josiah Kaviani
+Copyright 2020-2024 Josiah Kaviani
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
```

### Comparing `generics-6.0.0/docs/index.md` & `generics-7.0.0/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generics [![build](https://img.shields.io/github/workflow/status/proofit404/generics/release?style=flat-square)](https://github.com/proofit404/generics/actions/workflows/release.yml?query=branch%3Arelease) [![pypi](https://img.shields.io/pypi/v/generics?style=flat-square)](https://pypi.org/project/generics)
+# Generics [![build](https://img.shields.io/github/actions/workflow/status/proofit404/generics/release.yml?branch=release&style=flat-square)](https://github.com/proofit404/generics/actions/workflows/release.yml?query=branch%3Arelease) [![pypi](https://img.shields.io/pypi/v/generics?style=flat-square)](https://pypi.org/project/generics)
 
 A classy toolkit designed with OOP in mind.
 
 **[Documentation](https://proofit404.github.io/generics) |
 [Source Code](https://github.com/proofit404/generics) |
 [Task Tracker](https://github.com/proofit404/generics/issues)**
 
@@ -27,17 +27,17 @@
 
 >>> from generics import private
 
 >>> @private
 ... class User:
 ...     def __init__(self, name):
 ...         self.name = name
-...
 ...     def greet(self):
 ...         return f"Hello, {self.name}"
+...
 
 >>> user = User("Jeff")
 
 >>> user.greet()
 'Hello, Jeff'
 
 >>> hasattr(user, "name")
```

### Comparing `generics-6.0.0/pyproject.toml` & `generics-7.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 authors = ["Josiah Kaviani <proofit404@gmail.com>"]
 classifiers = [
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy"
 ]
 description = "A classy toolkit designed with OOP in mind."
 documentation = "https://proofit404.github.io/generics"
 homepage = "https://pypi.org/project/generics"
 license = "BSD-2-Clause"
 name = "generics"
 packages = [
-    { include = "_generics", from = "src" },
-    { include = "generics", from = "src" },
+  {from = "src", include = "_generics"},
+  {from = "src", include = "generics"}
 ]
 readme = "docs/index.md"
 repository = "https://github.com/proofit404/generics"
-version = "6.0.0"
+version = "7.0.0"
 
 [tool.poetry.dependencies]
 python = "*"
 
 [tool.poetry.urls]
 Changelog = "https://proofit404.github.io/generics/changelog"
 Issues = "https://github.com/proofit404/generics/issues"
```

### Comparing `generics-6.0.0/src/_generics/private.py` & `generics-7.0.0/src/_generics/private.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from inspect import signature
 from types import MemberDescriptorType
 
-from _generics.delegate import _dynamic
-from _generics.delegate import Delegate
 from _generics.exceptions import GenericClassError
 
 
 def private(cls):
     """Create class with private attributes."""
     methods = _get_methods(cls)
     init = _get_init(cls)
@@ -144,15 +142,14 @@
         return _get_method_1(cls, name, attribute)
 
 
 def _get_method_1(cls, name, attribute):
     return (
         _deny_static_method(attribute)
         or _deny_class_method(attribute)
-        or _get_delegate_method(cls, name, attribute)
         or _get_instance_method(cls, name, attribute)
         or _deny_class_attribute(attribute)
     )
 
 
 def _deny_static_method(attribute):
     if isinstance(attribute, staticmethod):
@@ -162,19 +159,14 @@
 
 def _deny_class_method(attribute):
     if isinstance(attribute, classmethod):
         message = "Do not use class methods (call constructor instead)"
         raise GenericClassError(message)
 
 
-def _get_delegate_method(cls, name, attribute):
-    if isinstance(attribute, Delegate):
-        return _DelegateMethod(cls, "__getattr__", _dynamic(attribute.f))
-
-
 def _get_instance_method(cls, name, attribute):
     if callable(attribute):
         return _Method(cls, name, attribute)
 
 
 def _deny_class_attribute(attribute):
     if not isinstance(attribute, MemberDescriptorType):
@@ -213,12 +205,7 @@
                     result = _wrap(result, methods)
                 return result
 
             def __repr__(_):
                 return f"Private::{instance!r}.{self.name}"
 
         return Method()
-
-
-class _DelegateMethod(_Method):
-    def is_underscore(self):
-        return False
```

### Comparing `generics-6.0.0/PKG-INFO` & `generics-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generics
-Version: 6.0.0
+Version: 7.0.0
 Summary: A classy toolkit designed with OOP in mind.
 Home-page: https://pypi.org/project/generics
 License: BSD-2-Clause
 Author: Josiah Kaviani
 Author-email: proofit404@gmail.com
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2
@@ -14,24 +14,25 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Project-URL: Changelog, https://proofit404.github.io/generics/changelog
 Project-URL: Documentation, https://proofit404.github.io/generics
 Project-URL: Issues, https://github.com/proofit404/generics/issues
 Project-URL: Repository, https://github.com/proofit404/generics
 Project-URL: Twitter, https://twitter.com/proofit404
 Description-Content-Type: text/markdown
 
-# Generics [![build](https://img.shields.io/github/workflow/status/proofit404/generics/release?style=flat-square)](https://github.com/proofit404/generics/actions/workflows/release.yml?query=branch%3Arelease) [![pypi](https://img.shields.io/pypi/v/generics?style=flat-square)](https://pypi.org/project/generics)
+# Generics [![build](https://img.shields.io/github/actions/workflow/status/proofit404/generics/release.yml?branch=release&style=flat-square)](https://github.com/proofit404/generics/actions/workflows/release.yml?query=branch%3Arelease) [![pypi](https://img.shields.io/pypi/v/generics?style=flat-square)](https://pypi.org/project/generics)
 
 A classy toolkit designed with OOP in mind.
 
 **[Documentation](https://proofit404.github.io/generics) |
 [Source Code](https://github.com/proofit404/generics) |
 [Task Tracker](https://github.com/proofit404/generics/issues)**
 
@@ -56,17 +57,17 @@
 
 >>> from generics import private
 
 >>> @private
 ... class User:
 ...     def __init__(self, name):
 ...         self.name = name
-...
 ...     def greet(self):
 ...         return f"Hello, {self.name}"
+...
 
 >>> user = User("Jeff")
 
 >>> user.greet()
 'Hello, Jeff'
 
 >>> hasattr(user, "name")
```

