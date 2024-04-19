# Comparing `tmp/Flask-Restless-NG-3.2.1.tar.gz` & `tmp/Flask-Restless-NG-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Restless-NG-3.2.1.tar", last modified: Fri Jan 19 21:21:18 2024, max compression
+gzip compressed data, was "Flask-Restless-NG-3.2.3.tar", last modified: Fri Apr 19 15:27:41 2024, max compression
```

## Comparing `Flask-Restless-NG-3.2.1.tar` & `Flask-Restless-NG-3.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-01-19 21:21:18.560459 Flask-Restless-NG-3.2.1/
-drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-01-19 21:21:18.541970 Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/
--rw-r--r--   0 mrevutsk (20854) staff       (20)     2108 2024-01-19 21:21:18.000000 Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/PKG-INFO
--rw-r--r--   0 mrevutsk (20854) staff       (20)      991 2024-01-19 21:21:18.000000 Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/SOURCES.txt
--rw-r--r--   0 mrevutsk (20854) staff       (20)        1 2024-01-19 21:21:18.000000 Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/dependency_links.txt
--rw-r--r--   0 mrevutsk (20854) staff       (20)        1 2023-10-14 16:00:05.000000 Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/not-zip-safe
--rw-r--r--   0 mrevutsk (20854) staff       (20)       76 2024-01-19 21:21:18.000000 Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/requires.txt
--rw-r--r--   0 mrevutsk (20854) staff       (20)       15 2024-01-19 21:21:18.000000 Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/top_level.txt
--rw-r--r--   0 mrevutsk (20854) staff       (20)    34520 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/LICENSE.AGPL
--rw-r--r--   0 mrevutsk (20854) staff       (20)     1479 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/LICENSE.BSD
--rw-r--r--   0 mrevutsk (20854) staff       (20)     1164 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/LICENSE.md
--rw-r--r--   0 mrevutsk (20854) staff       (20)       41 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/MANIFEST.in
--rw-r--r--   0 mrevutsk (20854) staff       (20)     2108 2024-01-19 21:21:18.560229 Flask-Restless-NG-3.2.1/PKG-INFO
--rw-r--r--   0 mrevutsk (20854) staff       (20)     3773 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/README.md
-drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-01-19 21:21:18.546958 Flask-Restless-NG-3.2.1/flask_restless/
--rw-r--r--   0 mrevutsk (20854) staff       (20)     1282 2024-01-19 21:14:51.000000 Flask-Restless-NG-3.2.1/flask_restless/__init__.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)      331 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/flask_restless/exceptions.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    13564 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/flask_restless/helpers.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    34293 2024-01-19 19:01:20.000000 Flask-Restless-NG-3.2.1/flask_restless/manager.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)      822 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/flask_restless/registry.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    16630 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/flask_restless/search.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    26751 2024-01-19 21:14:03.000000 Flask-Restless-NG-3.2.1/flask_restless/serialization.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)      263 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/flask_restless/typehints.py
-drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-01-19 21:21:18.551360 Flask-Restless-NG-3.2.1/flask_restless/views/
--rw-r--r--   0 mrevutsk (20854) staff       (20)      953 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/flask_restless/views/__init__.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    70866 2024-01-19 18:36:41.000000 Flask-Restless-NG-3.2.1/flask_restless/views/base.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)     1869 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/flask_restless/views/helpers.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    17677 2023-10-14 16:24:58.000000 Flask-Restless-NG-3.2.1/flask_restless/views/relationships.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    24639 2023-10-14 16:26:04.000000 Flask-Restless-NG-3.2.1/flask_restless/views/resources.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)      338 2024-01-19 21:21:18.560879 Flask-Restless-NG-3.2.1/setup.cfg
--rw-r--r--   0 mrevutsk (20854) staff       (20)     3817 2023-10-14 17:02:08.000000 Flask-Restless-NG-3.2.1/setup.py
-drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-01-19 21:21:18.559438 Flask-Restless-NG-3.2.1/tests/
--rw-r--r--   0 mrevutsk (20854) staff       (20)    41799 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_fetching.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    44506 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_filtering.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)     2124 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_flask_sqlalchemy.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    14032 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_manager.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)     1695 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_metadata.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)     3104 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_performance.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    20799 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_serialization.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)     3417 2024-01-19 20:59:06.000000 Flask-Restless-NG-3.2.1/tests/test_serializer.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    34204 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_updating.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)    36962 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.1/tests/test_updatingrelationship.py
--rw-r--r--   0 mrevutsk (20854) staff       (20)     8786 2024-01-19 18:36:30.000000 Flask-Restless-NG-3.2.1/tests/test_validation.py
+drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-04-19 15:27:41.867528 Flask-Restless-NG-3.2.3/
+drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-04-19 15:27:41.849573 Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     2108 2024-04-19 15:27:41.000000 Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/PKG-INFO
+-rw-r--r--   0 mrevutsk (20854) staff       (20)      991 2024-04-19 15:27:41.000000 Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 mrevutsk (20854) staff       (20)        1 2024-04-19 15:27:41.000000 Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 mrevutsk (20854) staff       (20)        1 2023-10-14 16:00:05.000000 Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/not-zip-safe
+-rw-r--r--   0 mrevutsk (20854) staff       (20)       76 2024-04-19 15:27:41.000000 Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/requires.txt
+-rw-r--r--   0 mrevutsk (20854) staff       (20)       15 2024-04-19 15:27:41.000000 Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/top_level.txt
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    34520 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/LICENSE.AGPL
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     1479 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/LICENSE.BSD
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     1164 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/LICENSE.md
+-rw-r--r--   0 mrevutsk (20854) staff       (20)       41 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/MANIFEST.in
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     2108 2024-04-19 15:27:41.867348 Flask-Restless-NG-3.2.3/PKG-INFO
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     3773 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/README.md
+drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-04-19 15:27:41.855129 Flask-Restless-NG-3.2.3/flask_restless/
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     1282 2024-04-19 15:06:54.000000 Flask-Restless-NG-3.2.3/flask_restless/__init__.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)      331 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/flask_restless/exceptions.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    13564 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/flask_restless/helpers.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    34293 2024-01-19 19:01:20.000000 Flask-Restless-NG-3.2.3/flask_restless/manager.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)      822 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/flask_restless/registry.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    16714 2024-04-19 15:05:56.000000 Flask-Restless-NG-3.2.3/flask_restless/search.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    26751 2024-01-19 21:14:03.000000 Flask-Restless-NG-3.2.3/flask_restless/serialization.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)      263 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/flask_restless/typehints.py
+drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-04-19 15:27:41.858293 Flask-Restless-NG-3.2.3/flask_restless/views/
+-rw-r--r--   0 mrevutsk (20854) staff       (20)      953 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/flask_restless/views/__init__.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    70866 2024-01-19 18:36:41.000000 Flask-Restless-NG-3.2.3/flask_restless/views/base.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     1869 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/flask_restless/views/helpers.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    17677 2023-10-14 16:24:58.000000 Flask-Restless-NG-3.2.3/flask_restless/views/relationships.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    24639 2023-10-14 16:26:04.000000 Flask-Restless-NG-3.2.3/flask_restless/views/resources.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)      338 2024-04-19 15:27:41.870329 Flask-Restless-NG-3.2.3/setup.cfg
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     3817 2023-10-14 17:02:08.000000 Flask-Restless-NG-3.2.3/setup.py
+drwxr-xr-x   0 mrevutsk (20854) staff       (20)        0 2024-04-19 15:27:41.866519 Flask-Restless-NG-3.2.3/tests/
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    41799 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_fetching.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    47205 2024-04-19 15:12:18.000000 Flask-Restless-NG-3.2.3/tests/test_filtering.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     2124 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_flask_sqlalchemy.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    14032 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_manager.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     1695 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_metadata.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     3104 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_performance.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    20799 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_serialization.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     3417 2024-01-19 20:59:06.000000 Flask-Restless-NG-3.2.3/tests/test_serializer.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    34204 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_updating.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)    36962 2023-10-14 15:55:54.000000 Flask-Restless-NG-3.2.3/tests/test_updatingrelationship.py
+-rw-r--r--   0 mrevutsk (20854) staff       (20)     8786 2024-01-19 18:36:30.000000 Flask-Restless-NG-3.2.3/tests/test_validation.py
```

### Comparing `Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/PKG-INFO` & `Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Restless-NG
-Version: 3.2.1
+Version: 3.2.3
 Summary: A fork of Flask-Restless with updated dependencies and bug fixes
 Home-page: https://github.com/mrevutskyi/flask-restless-ng
 Download-URL: https://pypi.python.org/pypi/Flask-Restless-NG
 Author: Maksym Revutskyi
 Author-email: maksym.revutskyi@gmail.com
 License: GNU AGPLv3+ or BSD
 Keywords: ReST,API,Flask
```

### Comparing `Flask-Restless-NG-3.2.1/Flask_Restless_NG.egg-info/SOURCES.txt` & `Flask-Restless-NG-3.2.3/Flask_Restless_NG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/LICENSE.AGPL` & `Flask-Restless-NG-3.2.3/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/LICENSE.BSD` & `Flask-Restless-NG-3.2.3/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/LICENSE.md` & `Flask-Restless-NG-3.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/PKG-INFO` & `Flask-Restless-NG-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Restless-NG
-Version: 3.2.1
+Version: 3.2.3
 Summary: A fork of Flask-Restless with updated dependencies and bug fixes
 Home-page: https://github.com/mrevutskyi/flask-restless-ng
 Download-URL: https://pypi.python.org/pypi/Flask-Restless-NG
 Author: Maksym Revutskyi
 Author-email: maksym.revutskyi@gmail.com
 License: GNU AGPLv3+ or BSD
 Keywords: ReST,API,Flask
```

### Comparing `Flask-Restless-NG-3.2.1/README.md` & `Flask-Restless-NG-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/__init__.py` & `Flask-Restless-NG-3.2.3/flask_restless/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # License version 3 and under the 3-clause BSD license. For more
 # information, see LICENSE.AGPL and LICENSE.BSD.
 """Provides classes for creating endpoints for interacting with
 SQLAlchemy models via the JSON API protocol.
 
 """
 #: The current version of this extension.
-__version__ = '3.2.1'
+__version__ = '3.2.3'
 
 
 # The following names are available as part of the public API for Flask-Restless-NG.
 # End users of this package can import these names by doing
 # ``from flask_restless import APIManager``, for example.
 from .manager import APIManager  # noqa
 from .manager import IllegalArgumentError  # noqa
```

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/helpers.py` & `Flask-Restless-NG-3.2.3/flask_restless/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/manager.py` & `Flask-Restless-NG-3.2.3/flask_restless/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/registry.py` & `Flask-Restless-NG-3.2.3/flask_restless/registry.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/search.py` & `Flask-Restless-NG-3.2.3/flask_restless/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,16 @@
     'ilike': lambda f, a: f.ilike(a),
     'like': lambda f, a: f.like(a),
     'not_like': lambda f, a: ~f.like(a),
     'in': lambda f, a: f.in_(a),
     'not_in': lambda f, a: ~f.in_(a),
     'to_tsquery': lambda f, a: f.match(a),
     'plainto_tsquery': lambda f, a: f.op('@@')(func.plainto_tsquery(a)),
+    '@>': lambda f, a, fn: f.op('@>')(a),
+    '<@': lambda f, a, fn: f.op('<@')(a),
     # Operators which accept three arguments.
     'has': lambda f, a, fn: f.has(_sub_operator(f, a, fn)),
     'any': lambda f, a, fn: f.any(_sub_operator(f, a, fn)),
 }
 
 
 class Filter(object):
```

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/serialization.py` & `Flask-Restless-NG-3.2.3/flask_restless/serialization.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/views/__init__.py` & `Flask-Restless-NG-3.2.3/flask_restless/views/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/views/base.py` & `Flask-Restless-NG-3.2.3/flask_restless/views/base.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/views/helpers.py` & `Flask-Restless-NG-3.2.3/flask_restless/views/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/views/relationships.py` & `Flask-Restless-NG-3.2.3/flask_restless/views/relationships.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/flask_restless/views/resources.py` & `Flask-Restless-NG-3.2.3/flask_restless/views/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/setup.py` & `Flask-Restless-NG-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_fetching.py` & `Flask-Restless-NG-3.2.3/tests/test_fetching.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_filtering.py` & `Flask-Restless-NG-3.2.3/tests/test_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from sqlalchemy import DateTime
 from sqlalchemy import ForeignKey
 from sqlalchemy import Integer
 from sqlalchemy import String
 from sqlalchemy import Time
 from sqlalchemy import Unicode
 from sqlalchemy import func
+from sqlalchemy.dialects.postgresql import ARRAY
 from sqlalchemy.dialects.postgresql import INET
 from sqlalchemy.dialects.postgresql import TSVECTOR
 from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy.orm import backref
 from sqlalchemy.orm import relationship
 from testing.postgresql import PostgresqlFactory as PGFactory
 
@@ -1064,16 +1065,14 @@
         class Product(self.Base):
             __tablename__ = 'product'
             id = Column(Integer, primary_key=True)
             name = Column(String)
             document = Column(TSVECTOR)
 
         self.Product = Product
-        # This try/except skips the tests if we are unable to create the
-        # tables in the PostgreSQL database.
         self.Base.metadata.create_all(bind=self.engine)
         self.manager.create_api(Product)
 
         # Create common records
         self.product1 = self.Product(
             id=1, name='Porsche 911', document=func.to_tsvector('Porsche 911'))
         self.product2 = self.Product(
@@ -1122,7 +1121,86 @@
         # Search without the &.
         filters = [
             dict(name='document', op='plainto_tsquery', val='911 Porsche')]
         response = self.search('/api/product', filters)
         document = response.json
         products = document['data']
         assert [self.product1.id] == [int(product['id']) for product in products]
+
+
+class TestArrayOperators(SearchTestBase):
+    """Unit tests for the array operators in PostgreSQL.
+
+    For more information, see `Array Functions and Operators`_
+    in the PostgreSQL documentation.
+
+    .. _Array Functions and Operators:
+       https://www.postgresql.org/docs/current/functions-array.html
+
+    """
+
+    def setUp(self):
+        super(TestArrayOperators, self).setUp()
+
+        class Product(self.Base):
+            __tablename__ = 'product'
+            id = Column(Integer, primary_key=True)
+            name = Column(String)
+            tags = Column(ARRAY(String))
+
+        self.Product = Product
+        self.Base.metadata.create_all(bind=self.engine)
+        self.manager.create_api(Product)
+
+        # Create common records
+        self.product1 = self.Product(
+            id=1, name='Porsche 911', tags=['car', 'sport'])
+        self.product2 = self.Product(
+            id=2, name='Porsche 918', tags=['car', 'hybrid'])
+        self.session.add_all([self.product1, self.product2])
+        self.session.commit()
+
+    def tearDown(self):
+        """Closes the database and removes the temporary directory in
+        which it lives.
+
+        """
+        super(TestArrayOperators, self).tearDown()
+        self.database.stop()
+
+    # We know this method will be called by `setUp()` in the superclass,
+    # so we can set up the temporary database here.
+    def database_uri(self):
+        """Creates a PostgreSQL database and returns its connection URI."""
+        #: The PostgreSQL database used by the test methods in this class.
+        #:
+        #: This attribute stores a
+        #: :class:`~testing.postgresql.Postgresql` object, which must be
+        #: stopped in the :meth:`.tearDown` method.
+        self.database = PostgreSQL()
+
+        return self.database.url()
+
+    def test_contains(self):
+        """Test for the ``@>`` ("contains") operator.
+        For example:
+        .. sourcecode:: postgresql
+            tags @> ARRAY['car']
+        """
+        filters = [dict(name='tags', op='@>', val=['car'])]
+        response = self.search('/api/product', filters)
+        document = response.json
+        products = document['data']
+        assert [self.product1.id, self.product2.id] == sorted(
+            int(product['id']) for product in products)
+
+    def test_contained_by(self):
+        """Test for the ``<@`` ("contained by") operator.
+        For example:
+        .. sourcecode:: postgresql
+            tags <@ ARRAY['car', 'sport']
+        """
+        filters = [dict(name='tags', op='<@', val=['car', 'sport'])]
+        response = self.search('/api/product', filters)
+        document = response.json
+        products = document['data']
+        assert [self.product1.id] == [int(product['id']) for product in products]
```

### Comparing `Flask-Restless-NG-3.2.1/tests/test_flask_sqlalchemy.py` & `Flask-Restless-NG-3.2.3/tests/test_flask_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_manager.py` & `Flask-Restless-NG-3.2.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_metadata.py` & `Flask-Restless-NG-3.2.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_performance.py` & `Flask-Restless-NG-3.2.3/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_serialization.py` & `Flask-Restless-NG-3.2.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_serializer.py` & `Flask-Restless-NG-3.2.3/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_updating.py` & `Flask-Restless-NG-3.2.3/tests/test_updating.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_updatingrelationship.py` & `Flask-Restless-NG-3.2.3/tests/test_updatingrelationship.py`

 * *Files identical despite different names*

### Comparing `Flask-Restless-NG-3.2.1/tests/test_validation.py` & `Flask-Restless-NG-3.2.3/tests/test_validation.py`

 * *Files identical despite different names*

