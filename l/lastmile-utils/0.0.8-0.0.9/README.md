# Comparing `tmp/lastmile_utils-0.0.8.tar.gz` & `tmp/lastmile_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastmile_utils-0.0.8.tar", last modified: Thu Dec  7 21:24:21 2023, max compression
+gzip compressed data, was "lastmile_utils-0.0.9.tar", last modified: Fri Dec  8 16:17:50 2023, max compression
```

## Comparing `lastmile_utils-0.0.8.tar` & `lastmile_utils-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.572094 lastmile_utils-0.0.8/
--rw-r--r--   0 jonathan   (501) staff       (20)      887 2023-12-07 21:24:21.571921 lastmile_utils-0.0.8/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)       30 2023-11-21 20:22:42.000000 lastmile_utils-0.0.8/README.md
--rw-r--r--   0 jonathan   (501) staff       (20)      617 2023-12-07 21:23:52.000000 lastmile_utils-0.0.8/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)      204 2023-12-07 07:00:15.000000 lastmile_utils-0.0.8/requirements.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-12-07 21:24:21.572133 lastmile_utils-0.0.8/setup.cfg
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.569356 lastmile_utils-0.0.8/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.569132 lastmile_utils-0.0.8/src/lastmile_utils/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.569297 lastmile_utils-0.0.8/src/lastmile_utils/lib/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.570946 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.571080 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/api/
--rw-r--r--   0 jonathan   (501) staff       (20)      288 2023-11-30 17:18:46.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/api/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)      219 2023-11-29 21:04:10.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/api_file.py
--rw-r--r--   0 jonathan   (501) staff       (20)     3711 2023-11-21 23:06:43.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/configs.py
--rw-r--r--   0 jonathan   (501) staff       (20)     4027 2023-12-07 21:22:56.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/functional.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1036 2023-11-29 20:22:43.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/module_mocking.py
--rw-r--r--   0 jonathan   (501) staff       (20)    12450 2023-12-07 20:06:03.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/core/utils.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.571312 lastmile_utils-0.0.8/src/lastmile_utils/lib/jupyter/
--rw-r--r--   0 jonathan   (501) staff       (20)       21 2023-11-30 19:40:06.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/jupyter/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)      197 2023-12-01 00:06:47.000000 lastmile_utils-0.0.8/src/lastmile_utils/lib/jupyter/utils.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.571719 lastmile_utils-0.0.8/src/lastmile_utils.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)      887 2023-12-07 21:24:21.000000 lastmile_utils-0.0.8/src/lastmile_utils.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      621 2023-12-07 21:24:21.000000 lastmile_utils-0.0.8/src/lastmile_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-12-07 21:24:21.000000 lastmile_utils-0.0.8/src/lastmile_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)      205 2023-12-07 21:24:21.000000 lastmile_utils-0.0.8/src/lastmile_utils.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       23 2023-12-07 21:24:21.000000 lastmile_utils-0.0.8/src/lastmile_utils.egg-info/top_level.txt
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.571427 lastmile_utils-0.0.8/src/scripts/
--rw-r--r--   0 jonathan   (501) staff       (20)    10944 2023-11-28 20:02:21.000000 lastmile_utils-0.0.8/src/scripts/lint.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-07 21:24:21.571545 lastmile_utils-0.0.8/tests/
--rw-r--r--   0 jonathan   (501) staff       (20)      163 2023-11-29 21:00:48.000000 lastmile_utils-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.041239 lastmile_utils-0.0.9/
+-rw-r--r--   0 jonathan   (501) staff       (20)      887 2023-12-08 16:17:50.041054 lastmile_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)       30 2023-11-21 20:22:42.000000 lastmile_utils-0.0.9/README.md
+-rw-r--r--   0 jonathan   (501) staff       (20)      617 2023-12-08 16:17:27.000000 lastmile_utils-0.0.9/pyproject.toml
+-rw-r--r--   0 jonathan   (501) staff       (20)      204 2023-12-07 07:00:15.000000 lastmile_utils-0.0.9/requirements.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-12-08 16:17:50.041275 lastmile_utils-0.0.9/setup.cfg
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.038555 lastmile_utils-0.0.9/src/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.038339 lastmile_utils-0.0.9/src/lastmile_utils/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.038496 lastmile_utils-0.0.9/src/lastmile_utils/lib/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.040117 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.040231 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/api/
+-rw-r--r--   0 jonathan   (501) staff       (20)      288 2023-11-30 17:18:46.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/api/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      219 2023-11-29 21:04:10.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/api_file.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     3711 2023-11-21 23:06:43.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/configs.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     4027 2023-12-07 21:22:56.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/functional.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1036 2023-11-29 20:22:43.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/module_mocking.py
+-rw-r--r--   0 jonathan   (501) staff       (20)    12703 2023-12-08 15:24:37.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/core/utils.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.040457 lastmile_utils-0.0.9/src/lastmile_utils/lib/jupyter/
+-rw-r--r--   0 jonathan   (501) staff       (20)       21 2023-11-30 19:40:06.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/jupyter/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      197 2023-12-01 00:06:47.000000 lastmile_utils-0.0.9/src/lastmile_utils/lib/jupyter/utils.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.040865 lastmile_utils-0.0.9/src/lastmile_utils.egg-info/
+-rw-r--r--   0 jonathan   (501) staff       (20)      887 2023-12-08 16:17:50.000000 lastmile_utils-0.0.9/src/lastmile_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)      621 2023-12-08 16:17:50.000000 lastmile_utils-0.0.9/src/lastmile_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-12-08 16:17:50.000000 lastmile_utils-0.0.9/src/lastmile_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)      205 2023-12-08 16:17:50.000000 lastmile_utils-0.0.9/src/lastmile_utils.egg-info/requires.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)       23 2023-12-08 16:17:50.000000 lastmile_utils-0.0.9/src/lastmile_utils.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.040563 lastmile_utils-0.0.9/src/scripts/
+-rw-r--r--   0 jonathan   (501) staff       (20)    10944 2023-11-28 20:02:21.000000 lastmile_utils-0.0.9/src/scripts/lint.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-12-08 16:17:50.040687 lastmile_utils-0.0.9/tests/
+-rw-r--r--   0 jonathan   (501) staff       (20)      163 2023-11-29 21:00:48.000000 lastmile_utils-0.0.9/tests/test_utils.py
```

### Comparing `lastmile_utils-0.0.8/PKG-INFO` & `lastmile_utils-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shared LM Python Libraries
 Author-email: Jonathan Lessinger <jonathan@lastmileai.dev>
 Project-URL: Homepage, https://github.com/lastmile-ai/lastmile_utils
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/lastmile_utils/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `lastmile_utils-0.0.8/pyproject.toml` & `lastmile_utils-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lastmile_utils"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name="Jonathan Lessinger", email="jonathan@lastmileai.dev" },
 ]
 description = "Shared LM Python Libraries"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lastmile_utils-0.0.8/src/lastmile_utils/lib/core/configs.py` & `lastmile_utils-0.0.9/src/lastmile_utils/lib/core/configs.py`

 * *Files identical despite different names*

### Comparing `lastmile_utils-0.0.8/src/lastmile_utils/lib/core/functional.py` & `lastmile_utils-0.0.9/src/lastmile_utils/lib/core/functional.py`

 * *Files identical despite different names*

### Comparing `lastmile_utils-0.0.8/src/lastmile_utils/lib/core/module_mocking.py` & `lastmile_utils-0.0.9/src/lastmile_utils/lib/core/module_mocking.py`

 * *Files identical despite different names*

### Comparing `lastmile_utils-0.0.8/src/lastmile_utils/lib/core/utils.py` & `lastmile_utils-0.0.9/src/lastmile_utils/lib/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import partial
+from hashlib import sha256
 import json
 import logging
 import os
 import sys
 import time
 from typing import (
     IO,
@@ -280,14 +281,18 @@
             return Err(f"distinct values: {value}, {x}")
     return Ok(value)
 
 
 only = enforce_unique
 
 
+def is_unique(iterable: Iterable[T]) -> bool:  # type: ignore[no-untyped-def]
+    return enforce_unique(iterable).is_ok()
+
+
 def dict_map(
     d: Mapping[T, U],
     key_fn: Optional[Callable[[T, U], T2]] = None,
     value_fn: Optional[Callable[[T, U], U2]] = None,
 ) -> dict[T2, U2]:
     """Like list map, but for dicts.
 
@@ -379,15 +384,15 @@
     try:
         return Ok(cls.model_validate_json(data))
     except ValidationError as e:
         return Err(str(e))
 
 
 def unzip(l: Sequence[tuple[T, U]]) -> tuple[list[T], list[U]]:
-    return tuple(zip(*l))  # type: ignore[fixme, return-value]
+    return tuple(map(list, zip(*l)))  # type: ignore[fixme, return-value]
 
 
 def print_result(
     r: Result[T, str], to: str | IO[str] | None = None
 ) -> Result[int, str]:
     data = fmt_result(r)
     match to:
@@ -437,8 +442,12 @@
         partial(
             pydantic_model_validate_from_json_file_handle,
             basemodel_type=basemodel_type,
         ),
         "r",
     )
 
-    return fn(path)
+    return fn(path)
+
+
+def hash_id(data: Any) -> str:
+    return sha256(str(data).encode("utf-8")).hexdigest()
```

### Comparing `lastmile_utils-0.0.8/src/lastmile_utils.egg-info/PKG-INFO` & `lastmile_utils-0.0.9/src/lastmile_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shared LM Python Libraries
 Author-email: Jonathan Lessinger <jonathan@lastmileai.dev>
 Project-URL: Homepage, https://github.com/lastmile-ai/lastmile_utils
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/lastmile_utils/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `lastmile_utils-0.0.8/src/lastmile_utils.egg-info/SOURCES.txt` & `lastmile_utils-0.0.9/src/lastmile_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lastmile_utils-0.0.8/src/scripts/lint.py` & `lastmile_utils-0.0.9/src/scripts/lint.py`

 * *Files identical despite different names*

