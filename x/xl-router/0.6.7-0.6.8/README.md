# Comparing `tmp/xl_router-0.6.7.tar.gz` & `tmp/xl_router-0.6.8.tar.gz`

## Comparing `xl_router-0.6.7.tar` & `xl_router-0.6.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/restful.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/router.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/decorators/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/utils/log.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/utils/memory.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/utils/session.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/utils/base/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.7/src/xl_router/utils/database/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.6.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.6.7/LICENSE
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 xl_router-0.6.7/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 xl_router-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/__init__.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/restful.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/router.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/decorators/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/utils/log.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/utils/memory.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/utils/session.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/utils/base/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.8/src/xl_router/utils/database/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.6.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.6.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.8/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xl_router-0.6.8/PKG-INFO
```

### Comparing `xl_router-0.6.7/src/xl_router/__init__.py` & `xl_router-0.6.8/src/xl_router/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from zrouter.router import Router
+from xl_router.router import Router
 from flask import Flask, request 
 from flask.json import JSONEncoder
 from importlib import import_module
 import decimal
 
 
 class JsonEncoder(JSONEncoder):
```

### Comparing `xl_router-0.6.7/src/xl_router/restful.py` & `xl_router-0.6.8/src/xl_router/restful.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.7/src/xl_router/router.py` & `xl_router-0.6.8/src/xl_router/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from zrouter.exceptions import MessagePrompt
-from zrouter.utils.base.json import to_lowcase, iter_lowcase, iter_camel
+from xl_router.exceptions import MessagePrompt
+from xl_router.utils.base.json import to_lowcase, iter_lowcase, iter_camel
 from flask import Blueprint, request
 from jsonschema.exceptions import ValidationError
 import functools
 import random
 import os
 import importlib
 import inspect
```

### Comparing `xl_router-0.6.7/src/xl_router/utils/memory.py` & `xl_router-0.6.8/src/xl_router/utils/memory.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.7/src/xl_router/utils/session.py` & `xl_router-0.6.8/src/xl_router/utils/session.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.7/src/xl_router/utils/base/json.py` & `xl_router-0.6.8/src/xl_router/utils/base/json.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.7/LICENSE` & `xl_router-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.7/pyproject.toml` & `xl_router-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xl-router"
-version = "0.6.7"
+version = "0.6.8"
 authors = [
   { name="xilong", email="xilonglab@163.com" },
 ]
 description = "xilong router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

