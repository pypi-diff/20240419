# Comparing `tmp/logiclayer-0.3.2.tar.gz` & `tmp/logiclayer-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logiclayer-0.3.2.tar", max compression
+gzip compressed data, was "logiclayer-0.3.3.tar", max compression
```

## Comparing `logiclayer-0.3.2.tar` & `logiclayer-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-16 17:44:47.451470 logiclayer-0.3.2/LICENSE
--rw-r--r--   0        0        0     3574 2024-04-16 17:44:47.451470 logiclayer-0.3.2/PACKAGE.md
--rw-r--r--   0        0        0      474 2024-04-16 17:44:47.451470 logiclayer-0.3.2/logiclayer/__init__.py
--rw-r--r--   0        0        0      894 2024-04-16 17:44:47.451470 logiclayer-0.3.2/logiclayer/auth.py
--rw-r--r--   0        0        0      623 2024-04-16 17:44:47.451470 logiclayer-0.3.2/logiclayer/common.py
--rw-r--r--   0        0        0     2689 2024-04-16 17:44:47.451470 logiclayer-0.3.2/logiclayer/decorators.py
--rw-r--r--   0        0        0     5201 2024-04-16 17:44:47.451470 logiclayer-0.3.2/logiclayer/logiclayer.py
--rw-r--r--   0        0        0     3878 2024-04-16 17:44:47.451470 logiclayer-0.3.2/logiclayer/module.py
--rw-r--r--   0        0        0      580 2024-04-16 17:44:47.455470 logiclayer-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 logiclayer-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-19 17:21:53.322917 logiclayer-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3574 2024-04-19 17:21:53.322917 logiclayer-0.3.3/PACKAGE.md
+-rw-r--r--   0        0        0      639 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/__init__.py
+-rw-r--r--   0        0        0      894 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/auth.py
+-rw-r--r--   0        0        0      623 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/common.py
+-rw-r--r--   0        0        0     2689 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/decorators.py
+-rw-r--r--   0        0        0     5201 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/logiclayer.py
+-rw-r--r--   0        0        0     4058 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/module.py
+-rw-r--r--   0        0        0      580 2024-04-19 17:21:53.326917 logiclayer-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 logiclayer-0.3.3/PKG-INFO
```

### Comparing `logiclayer-0.3.2/LICENSE` & `logiclayer-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.2/PACKAGE.md` & `logiclayer-0.3.3/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.2/logiclayer/auth.py` & `logiclayer-0.3.3/logiclayer/auth.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.2/logiclayer/common.py` & `logiclayer-0.3.3/logiclayer/common.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.2/logiclayer/decorators.py` & `logiclayer-0.3.3/logiclayer/decorators.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.2/logiclayer/logiclayer.py` & `logiclayer-0.3.3/logiclayer/logiclayer.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.2/logiclayer/module.py` & `logiclayer-0.3.3/logiclayer/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import dataclasses
+import dataclasses as dcls
 from collections import defaultdict
 from enum import Enum, auto
-from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type, Union
 
 from fastapi import APIRouter
 
 from .auth import AuthProvider, VoidAuthProvider
 from .common import LOGICLAYER_METHOD_ATTR, CallableMayReturnCoroutine
 
 if TYPE_CHECKING:
@@ -16,20 +16,20 @@
     EVENT_SHUTDOWN = auto()
     EVENT_STARTUP = auto()
     EXCEPTION_HANDLER = auto()
     HEALTHCHECK = auto()
     ROUTE = auto()
 
 
-@dataclasses.dataclass
+@dcls.dataclass
 class ModuleMethod:
     kind: MethodType
     func: CallableMayReturnCoroutine[Any]
     debug_only: bool = False
-    kwargs: Dict[str, Any] = dataclasses.field(default_factory=dict)
+    kwargs: Dict[str, Any] = dcls.field(default_factory=dict)
     path: str = ""
 
     def bound_to(self, instance: "LogicLayerModule") -> CallableMayReturnCoroutine[Any]:
         """Returns the bound function belonging to the instance of the
         LogicLayerModule subclass that matches the name of the original function.
 
         This bound function doesn't contain the 'self' parameter in its arguments.
@@ -80,16 +80,19 @@
     router: APIRouter
     _llexceptions: Dict[Type[Exception], ModuleMethod]
     _llhealthchecks: Tuple[ModuleMethod, ...]
     _llroutes: Tuple[ModuleMethod, ...]
     _llshutdown: Tuple[ModuleMethod, ...]
     _llstartup: Tuple[ModuleMethod, ...]
 
-    def __init__(self, *, auth: Optional[AuthProvider] = None, **kwargs):
+    def __init__(
+        self, *, auth: Optional[AuthProvider] = None, debug: bool = False, **kwargs
+    ):
         self.auth = auth or VoidAuthProvider()
+        self.debug = debug
         self.router = APIRouter(**kwargs)
 
     @property
     def name(self):
         return type(self).__name__
 
     @property
@@ -109,7 +112,15 @@
         router.on_startup.extend(item.bound_to(self) for item in self._llstartup)
         router.on_shutdown.extend(item.bound_to(self) for item in self._llshutdown)
 
         for item in self._llroutes:
             router.add_api_route(item.path, item.bound_to(self), **item.kwargs)
 
         app.include_router(router, **kwargs)
+
+
+@dcls.dataclass
+class ModuleStatus:
+    module: str
+    version: str
+    debug: Union[bool, dict]
+    extras: dict
```

### Comparing `logiclayer-0.3.2/PKG-INFO` & `logiclayer-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logiclayer
-Version: 0.3.2
+Version: 0.3.3
 Summary: A framework to quickly compose and use multiple functionalities as endpoints.
 Home-page: https://github.com/Datawheel/logiclayer
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

