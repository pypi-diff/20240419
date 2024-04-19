# Comparing `tmp/rizaio-0.1.0a3.tar.gz` & `tmp/rizaio-0.1.0a4.tar.gz`

## Comparing `rizaio-0.1.0a3.tar` & `rizaio-0.1.0a4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/__init__.py
--rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_base_client.py
--rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_files.py
--rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_typing.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/lib/.keep
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/resources/__init__.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/resources/v1.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/types/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/types/v1_execute_params.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/types/v1_execute_response.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/__init__.py
--rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_base_client.py
--rw-r--r--   0        0        0    14784 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_resource.py
--rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/__init__.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/lib/.keep
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/resources/__init__.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/resources/code.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/types/__init__.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/types/code_execute_params.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/types/code_execute_response.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0    11680 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/__init__.py
+-rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_base_client.py
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_files.py
+-rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/_typing.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/lib/.keep
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/resources/__init__.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/resources/v1.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/types/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/types/v1_execute_params.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/riza/types/v1_execute_response.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/__init__.py
+-rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_base_client.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_resource.py
+-rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/__init__.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/lib/.keep
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/resources/__init__.py
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/resources/sandbox.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/types/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/types/sandbox_execute_params.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/src/rizaio/types/sandbox_execute_response.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 rizaio-0.1.0a4/PKG-INFO
```

### Comparing `rizaio-0.1.0a3/src/riza/__init__.py` & `rizaio-0.1.0a4/src/riza/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_base_client.py` & `rizaio-0.1.0a4/src/riza/_base_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_client.py` & `rizaio-0.1.0a4/src/riza/_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_compat.py` & `rizaio-0.1.0a4/src/riza/_compat.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_exceptions.py` & `rizaio-0.1.0a4/src/riza/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_files.py` & `rizaio-0.1.0a4/src/riza/_files.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_models.py` & `rizaio-0.1.0a4/src/riza/_models.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_qs.py` & `rizaio-0.1.0a4/src/riza/_qs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_resource.py` & `rizaio-0.1.0a4/src/riza/_resource.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_response.py` & `rizaio-0.1.0a4/src/riza/_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_streaming.py` & `rizaio-0.1.0a4/src/riza/_streaming.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_types.py` & `rizaio-0.1.0a4/src/riza/_types.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_utils/__init__.py` & `rizaio-0.1.0a4/src/riza/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_utils/_logs.py` & `rizaio-0.1.0a4/src/riza/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_utils/_proxy.py` & `rizaio-0.1.0a4/src/riza/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_utils/_sync.py` & `rizaio-0.1.0a4/src/riza/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_utils/_transform.py` & `rizaio-0.1.0a4/src/riza/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_utils/_typing.py` & `rizaio-0.1.0a4/src/riza/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/_utils/_utils.py` & `rizaio-0.1.0a4/src/riza/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/riza/resources/v1.py` & `rizaio-0.1.0a4/src/riza/resources/v1.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/__init__.py` & `rizaio-0.1.0a4/src/rizaio/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_base_client.py` & `rizaio-0.1.0a4/src/rizaio/_base_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_client.py` & `rizaio-0.1.0a4/src/rizaio/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "AsyncRiza",
     "Client",
     "AsyncClient",
 ]
 
 
 class Riza(SyncAPIClient):
-    code: resources.Code
+    sandbox: resources.Sandbox
     with_raw_response: RizaWithRawResponse
     with_streaming_response: RizaWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -100,15 +100,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.code = resources.Code(self)
+        self.sandbox = resources.Sandbox(self)
         self.with_raw_response = RizaWithRawResponse(self)
         self.with_streaming_response = RizaWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -210,15 +210,15 @@
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class AsyncRiza(AsyncAPIClient):
-    code: resources.AsyncCode
+    sandbox: resources.AsyncSandbox
     with_raw_response: AsyncRizaWithRawResponse
     with_streaming_response: AsyncRizaWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -268,15 +268,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.code = resources.AsyncCode(self)
+        self.sandbox = resources.AsyncSandbox(self)
         self.with_raw_response = AsyncRizaWithRawResponse(self)
         self.with_streaming_response = AsyncRizaWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -379,28 +379,28 @@
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class RizaWithRawResponse:
     def __init__(self, client: Riza) -> None:
-        self.code = resources.CodeWithRawResponse(client.code)
+        self.sandbox = resources.SandboxWithRawResponse(client.sandbox)
 
 
 class AsyncRizaWithRawResponse:
     def __init__(self, client: AsyncRiza) -> None:
-        self.code = resources.AsyncCodeWithRawResponse(client.code)
+        self.sandbox = resources.AsyncSandboxWithRawResponse(client.sandbox)
 
 
 class RizaWithStreamedResponse:
     def __init__(self, client: Riza) -> None:
-        self.code = resources.CodeWithStreamingResponse(client.code)
+        self.sandbox = resources.SandboxWithStreamingResponse(client.sandbox)
 
 
 class AsyncRizaWithStreamedResponse:
     def __init__(self, client: AsyncRiza) -> None:
-        self.code = resources.AsyncCodeWithStreamingResponse(client.code)
+        self.sandbox = resources.AsyncSandboxWithStreamingResponse(client.sandbox)
 
 
 Client = Riza
 
 AsyncClient = AsyncRiza
```

### Comparing `rizaio-0.1.0a3/src/rizaio/_compat.py` & `rizaio-0.1.0a4/src/rizaio/_compat.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_exceptions.py` & `rizaio-0.1.0a4/src/rizaio/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_files.py` & `rizaio-0.1.0a4/src/rizaio/_files.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_models.py` & `rizaio-0.1.0a4/src/rizaio/_models.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_qs.py` & `rizaio-0.1.0a4/src/rizaio/_qs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_resource.py` & `rizaio-0.1.0a4/src/rizaio/_resource.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_response.py` & `rizaio-0.1.0a4/src/rizaio/_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_streaming.py` & `rizaio-0.1.0a4/src/rizaio/_streaming.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_types.py` & `rizaio-0.1.0a4/src/rizaio/_types.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_utils/__init__.py` & `rizaio-0.1.0a4/src/rizaio/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_utils/_logs.py` & `rizaio-0.1.0a4/src/rizaio/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_utils/_proxy.py` & `rizaio-0.1.0a4/src/rizaio/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_utils/_sync.py` & `rizaio-0.1.0a4/src/rizaio/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_utils/_transform.py` & `rizaio-0.1.0a4/src/rizaio/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_utils/_typing.py` & `rizaio-0.1.0a4/src/rizaio/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/_utils/_utils.py` & `rizaio-0.1.0a4/src/rizaio/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/src/rizaio/resources/code.py` & `rizaio-0.1.0a4/src/rizaio/resources/sandbox.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import Dict, List
 from typing_extensions import Literal
 
 import httpx
 
-from ..types import CodeExecuteResponse, code_execute_params
+from ..types import SandboxExecuteResponse, sandbox_execute_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -21,25 +21,25 @@
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
 
-__all__ = ["Code", "AsyncCode"]
+__all__ = ["Sandbox", "AsyncSandbox"]
 
 
-class Code(SyncAPIResource):
+class Sandbox(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> CodeWithRawResponse:
-        return CodeWithRawResponse(self)
+    def with_raw_response(self) -> SandboxWithRawResponse:
+        return SandboxWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> CodeWithStreamingResponse:
-        return CodeWithStreamingResponse(self)
+    def with_streaming_response(self) -> SandboxWithStreamingResponse:
+        return SandboxWithStreamingResponse(self)
 
     def execute(
         self,
         *,
         args: List[str] | NotGiven = NOT_GIVEN,
         code: str | NotGiven = NOT_GIVEN,
         env: Dict[str, str] | NotGiven = NOT_GIVEN,
@@ -47,15 +47,15 @@
         stdin: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> CodeExecuteResponse:
+    ) -> SandboxExecuteResponse:
         """
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -68,31 +68,31 @@
                 {
                     "args": args,
                     "code": code,
                     "env": env,
                     "language": language,
                     "stdin": stdin,
                 },
-                code_execute_params.CodeExecuteParams,
+                sandbox_execute_params.SandboxExecuteParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=CodeExecuteResponse,
+            cast_to=SandboxExecuteResponse,
         )
 
 
-class AsyncCode(AsyncAPIResource):
+class AsyncSandbox(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncCodeWithRawResponse:
-        return AsyncCodeWithRawResponse(self)
+    def with_raw_response(self) -> AsyncSandboxWithRawResponse:
+        return AsyncSandboxWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncCodeWithStreamingResponse:
-        return AsyncCodeWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncSandboxWithStreamingResponse:
+        return AsyncSandboxWithStreamingResponse(self)
 
     async def execute(
         self,
         *,
         args: List[str] | NotGiven = NOT_GIVEN,
         code: str | NotGiven = NOT_GIVEN,
         env: Dict[str, str] | NotGiven = NOT_GIVEN,
@@ -100,15 +100,15 @@
         stdin: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> CodeExecuteResponse:
+    ) -> SandboxExecuteResponse:
         """
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -121,50 +121,50 @@
                 {
                     "args": args,
                     "code": code,
                     "env": env,
                     "language": language,
                     "stdin": stdin,
                 },
-                code_execute_params.CodeExecuteParams,
+                sandbox_execute_params.SandboxExecuteParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=CodeExecuteResponse,
+            cast_to=SandboxExecuteResponse,
         )
 
 
-class CodeWithRawResponse:
-    def __init__(self, code: Code) -> None:
-        self._code = code
+class SandboxWithRawResponse:
+    def __init__(self, sandbox: Sandbox) -> None:
+        self._sandbox = sandbox
 
         self.execute = to_raw_response_wrapper(
-            code.execute,
+            sandbox.execute,
         )
 
 
-class AsyncCodeWithRawResponse:
-    def __init__(self, code: AsyncCode) -> None:
-        self._code = code
+class AsyncSandboxWithRawResponse:
+    def __init__(self, sandbox: AsyncSandbox) -> None:
+        self._sandbox = sandbox
 
         self.execute = async_to_raw_response_wrapper(
-            code.execute,
+            sandbox.execute,
         )
 
 
-class CodeWithStreamingResponse:
-    def __init__(self, code: Code) -> None:
-        self._code = code
+class SandboxWithStreamingResponse:
+    def __init__(self, sandbox: Sandbox) -> None:
+        self._sandbox = sandbox
 
         self.execute = to_streamed_response_wrapper(
-            code.execute,
+            sandbox.execute,
         )
 
 
-class AsyncCodeWithStreamingResponse:
-    def __init__(self, code: AsyncCode) -> None:
-        self._code = code
+class AsyncSandboxWithStreamingResponse:
+    def __init__(self, sandbox: AsyncSandbox) -> None:
+        self._sandbox = sandbox
 
         self.execute = async_to_streamed_response_wrapper(
-            code.execute,
+            sandbox.execute,
         )
```

### Comparing `rizaio-0.1.0a3/LICENSE` & `rizaio-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a3/pyproject.toml` & `rizaio-0.1.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rizaio"
-version = "0.1.0-alpha.3"
+version = "0.1.0-alpha.4"
 description = "The official Python library for the riza API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Riza", email = "hello@riza.io" },
 ]
 dependencies = [
```

### Comparing `rizaio-0.1.0a3/PKG-INFO` & `rizaio-0.1.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rizaio
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: The official Python library for the riza API
 Project-URL: Homepage, https://github.com/riza-io/riza-api-python
 Project-URL: Repository, https://github.com/riza-io/riza-api-python
 Author-email: Riza <hello@riza.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -62,16 +62,16 @@
 from rizaio import Riza
 
 client = Riza(
     # This is the default and can be omitted
     api_key=os.environ.get("RIZA_API_KEY"),
 )
 
-code_execute_response = client.code.execute()
-print(code_execute_response.exit_code)
+sandbox_execute_response = client.sandbox.execute()
+print(sandbox_execute_response.exit_code)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `RIZA_API_KEY="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
@@ -87,16 +87,16 @@
 client = AsyncRiza(
     # This is the default and can be omitted
     api_key=os.environ.get("RIZA_API_KEY"),
 )
 
 
 async def main() -> None:
-    code_execute_response = await client.code.execute()
-    print(code_execute_response.exit_code)
+    sandbox_execute_response = await client.sandbox.execute()
+    print(sandbox_execute_response.exit_code)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -121,15 +121,15 @@
 ```python
 import rizaio
 from rizaio import Riza
 
 client = Riza()
 
 try:
-    client.code.execute()
+    client.sandbox.execute()
 except rizaio.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except rizaio.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except rizaio.APIStatusError as e:
     print("Another non-200-range status code was received")
@@ -164,15 +164,15 @@
 # Configure the default for all requests:
 client = Riza(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
-client.with_options(max_retries=5).code.execute()
+client.with_options(max_retries=5).sandbox.execute()
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
@@ -187,15 +187,15 @@
 
 # More granular control:
 client = Riza(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5 * 1000).code.execute()
+client.with_options(timeout=5 * 1000).sandbox.execute()
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/riza-io/riza-api-python/tree/main/#retries).
 
 ## Advanced
@@ -226,33 +226,33 @@
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from rizaio import Riza
 
 client = Riza()
-response = client.code.with_raw_response.execute()
+response = client.sandbox.with_raw_response.execute()
 print(response.headers.get('X-My-Header'))
 
-code = response.parse()  # get the object that `code.execute()` would have returned
-print(code.exit_code)
+sandbox = response.parse()  # get the object that `sandbox.execute()` would have returned
+print(sandbox.exit_code)
 ```
 
 These methods return an [`APIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/rizaio/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/rizaio/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
-with client.code.with_streaming_response.execute() as response:
+with client.sandbox.with_streaming_response.execute() as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
```

