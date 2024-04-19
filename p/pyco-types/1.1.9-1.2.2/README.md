# Comparing `tmp/pyco-types-1.1.9.tar.gz` & `tmp/pyco-types-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyco-types-1.1.9.tar", last modified: Fri Apr 19 02:50:49 2024, max compression
+gzip compressed data, was "dist/pyco-types-1.2.2.tar", last modified: Fri Apr 19 08:51:43 2024, max compression
```

## Comparing `pyco-types-1.1.9.tar` & `pyco-types-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 02:50:49.414783 pyco-types-1.1.9/
--rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.1.9/LICENSE.txt
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-19 02:50:49.413699 pyco-types-1.1.9/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)      226 2024-04-12 09:35:12.000000 pyco-types-1.1.9/README.md
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 02:50:49.406510 pyco-types-1.1.9/pyco_types/
--rw-r--r--   0 nico       (502) staff       (20)      341 2024-04-18 11:47:23.000000 pyco-types-1.1.9/pyco_types/__init__.py
--rw-r--r--   0 nico       (502) staff       (20)     1918 2024-04-18 14:06:09.000000 pyco-types-1.1.9/pyco_types/_cls_base.py
--rw-r--r--   0 nico       (502) staff       (20)     3567 2024-04-18 08:58:05.000000 pyco-types-1.1.9/pyco_types/_cls_meta.py
--rw-r--r--   0 nico       (502) staff       (20)     4314 2024-04-18 13:44:40.000000 pyco-types-1.1.9/pyco_types/_common.py
--rw-r--r--   0 nico       (502) staff       (20)     2109 2024-04-18 11:46:56.000000 pyco-types-1.1.9/pyco_types/_convert_meta.py
--rw-r--r--   0 nico       (502) staff       (20)     2314 2024-04-12 09:56:26.000000 pyco-types-1.1.9/pyco_types/_filter_funcs.py
--rw-r--r--   0 nico       (502) staff       (20)     6330 2024-04-18 08:50:19.000000 pyco-types-1.1.9/pyco_types/_int_exts.py
--rw-r--r--   0 nico       (502) staff       (20)      185 2024-04-19 02:50:27.000000 pyco-types-1.1.9/pyco_types/_version.py
--rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.1.9/pyco_types/co_datetime.py
--rw-r--r--   0 nico       (502) staff       (20)     2573 2024-04-18 11:47:23.000000 pyco-types-1.1.9/pyco_types/co_dict.py
--rw-r--r--   0 nico       (502) staff       (20)     4824 2024-04-18 14:28:01.000000 pyco-types-1.1.9/pyco_types/co_ext_base.py
--rw-r--r--   0 nico       (502) staff       (20)      722 2024-04-18 12:50:55.000000 pyco-types-1.1.9/pyco_types/co_func.py
--rw-r--r--   0 nico       (502) staff       (20)     2651 2024-04-11 04:25:38.000000 pyco-types-1.1.9/pyco_types/co_integer.py
--rw-r--r--   0 nico       (502) staff       (20)      662 2024-04-18 13:19:22.000000 pyco-types-1.1.9/pyco_types/co_interface.tmp.py
--rw-r--r--   0 nico       (502) staff       (20)     5034 2024-04-19 02:21:26.000000 pyco-types-1.1.9/pyco_types/co_json.py
--rw-r--r--   0 nico       (502) staff       (20)     5156 2024-04-18 11:46:59.000000 pyco-types-1.1.9/pyco_types/co_regex.py
--rw-r--r--   0 nico       (502) staff       (20)     6473 2024-04-18 11:46:56.000000 pyco-types-1.1.9/pyco_types/const.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 02:50:49.412304 pyco-types-1.1.9/pyco_types.egg-info/
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)      612 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/SOURCES.txt
--rw-r--r--   0 nico       (502) staff       (20)        1 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/dependency_links.txt
--rw-r--r--   0 nico       (502) staff       (20)       23 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/requires.txt
--rw-r--r--   0 nico       (502) staff       (20)       11 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/top_level.txt
--rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-19 02:50:49.415445 pyco-types-1.1.9/setup.cfg
--rw-r--r--   0 nico       (502) staff       (20)     1283 2024-01-01 11:35:19.000000 pyco-types-1.1.9/setup.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 08:51:43.358729 pyco-types-1.2.2/
+-rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.2.2/LICENSE.txt
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-19 08:51:43.358277 pyco-types-1.2.2/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)      226 2024-04-12 09:35:12.000000 pyco-types-1.2.2/README.md
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 08:51:43.353343 pyco-types-1.2.2/pyco_types/
+-rw-r--r--   0 nico       (502) staff       (20)      341 2024-04-18 11:47:23.000000 pyco-types-1.2.2/pyco_types/__init__.py
+-rw-r--r--   0 nico       (502) staff       (20)     1918 2024-04-18 14:06:09.000000 pyco-types-1.2.2/pyco_types/_cls_base.py
+-rw-r--r--   0 nico       (502) staff       (20)     3567 2024-04-18 08:58:05.000000 pyco-types-1.2.2/pyco_types/_cls_meta.py
+-rw-r--r--   0 nico       (502) staff       (20)     4314 2024-04-18 13:44:40.000000 pyco-types-1.2.2/pyco_types/_common.py
+-rw-r--r--   0 nico       (502) staff       (20)     2109 2024-04-18 11:46:56.000000 pyco-types-1.2.2/pyco_types/_convert_meta.py
+-rw-r--r--   0 nico       (502) staff       (20)     2314 2024-04-12 09:56:26.000000 pyco-types-1.2.2/pyco_types/_filter_funcs.py
+-rw-r--r--   0 nico       (502) staff       (20)     6330 2024-04-18 08:50:19.000000 pyco-types-1.2.2/pyco_types/_int_exts.py
+-rw-r--r--   0 nico       (502) staff       (20)      185 2024-04-19 08:49:26.000000 pyco-types-1.2.2/pyco_types/_version.py
+-rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.2.2/pyco_types/co_datetime.py
+-rw-r--r--   0 nico       (502) staff       (20)     2573 2024-04-18 11:47:23.000000 pyco-types-1.2.2/pyco_types/co_dict.py
+-rw-r--r--   0 nico       (502) staff       (20)     4824 2024-04-18 14:28:01.000000 pyco-types-1.2.2/pyco_types/co_ext_base.py
+-rw-r--r--   0 nico       (502) staff       (20)      722 2024-04-18 12:50:55.000000 pyco-types-1.2.2/pyco_types/co_func.py
+-rw-r--r--   0 nico       (502) staff       (20)     2651 2024-04-11 04:25:38.000000 pyco-types-1.2.2/pyco_types/co_integer.py
+-rw-r--r--   0 nico       (502) staff       (20)      662 2024-04-18 13:19:22.000000 pyco-types-1.2.2/pyco_types/co_interface.tmp.py
+-rw-r--r--   0 nico       (502) staff       (20)     5275 2024-04-19 08:46:57.000000 pyco-types-1.2.2/pyco_types/co_json.py
+-rw-r--r--   0 nico       (502) staff       (20)     5156 2024-04-18 11:46:59.000000 pyco-types-1.2.2/pyco_types/co_regex.py
+-rw-r--r--   0 nico       (502) staff       (20)     6473 2024-04-18 11:46:56.000000 pyco-types-1.2.2/pyco_types/const.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 08:51:43.357619 pyco-types-1.2.2/pyco_types.egg-info/
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-19 08:51:43.000000 pyco-types-1.2.2/pyco_types.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)      612 2024-04-19 08:51:43.000000 pyco-types-1.2.2/pyco_types.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (502) staff       (20)        1 2024-04-19 08:51:43.000000 pyco-types-1.2.2/pyco_types.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-19 08:51:43.000000 pyco-types-1.2.2/pyco_types.egg-info/requires.txt
+-rw-r--r--   0 nico       (502) staff       (20)       11 2024-04-19 08:51:43.000000 pyco-types-1.2.2/pyco_types.egg-info/top_level.txt
+-rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-19 08:51:43.358888 pyco-types-1.2.2/setup.cfg
+-rw-r--r--   0 nico       (502) staff       (20)     1310 2024-04-19 08:25:46.000000 pyco-types-1.2.2/setup.py
```

### Comparing `pyco-types-1.1.9/LICENSE.txt` & `pyco-types-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/PKG-INFO` & `pyco-types-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.9
+Version: 1.2.2
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.9/pyco_types/_cls_base.py` & `pyco-types-1.2.2/pyco_types/_cls_base.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/_cls_meta.py` & `pyco-types-1.2.2/pyco_types/_cls_meta.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/_common.py` & `pyco-types-1.2.2/pyco_types/_common.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/_convert_meta.py` & `pyco-types-1.2.2/pyco_types/_convert_meta.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/_filter_funcs.py` & `pyco-types-1.2.2/pyco_types/_filter_funcs.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/_int_exts.py` & `pyco-types-1.2.2/pyco_types/_int_exts.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/co_datetime.py` & `pyco-types-1.2.2/pyco_types/co_datetime.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/co_dict.py` & `pyco-types-1.2.2/pyco_types/co_dict.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/co_ext_base.py` & `pyco-types-1.2.2/pyco_types/co_ext_base.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/co_func.py` & `pyco-types-1.2.2/pyco_types/co_func.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/co_integer.py` & `pyco-types-1.2.2/pyco_types/co_integer.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/co_interface.tmp.py` & `pyco-types-1.2.2/pyco_types/co_interface.tmp.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/co_json.py` & `pyco-types-1.2.2/pyco_types/co_json.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json
 import uuid
 # import inspect
+import orjson
 from pprint import pformat
 from datetime import datetime, date
 from logging import root as logger
-from pyco_types._convert_meta import find_converter, Converter
-from pyco_types._common import K_Python_Common_Types, CommonException, G_Symbol_UNSET
+from ._convert_meta import find_converter, Converter
+from ._common import K_Python_Common_Types, CommonException, G_Symbol_UNSET
 
 
 def pformat_any(data, depth=2, width=80, indent=2, **kwargs):
     return " :: ".join([str(type(data)), pformat(data, indent=indent, width=width, depth=depth)])
 
 
 def parse_json(data, **kwargs):
     if isinstance(data, str) and data.startswith('"') and data.endswith('"'):
         try:
-            obj = json.loads(data, **kwargs)
+            # obj = json.loads(data, **kwargs)
+            obj = orjson.loads(data)
             return obj
         except:
             ## import json5
             return data
     else:
         return data
 
@@ -90,30 +92,14 @@
         return cvt
 
     @classmethod
     def register_stringify(cls, otype, str_func, msg="-"):
         cls.__stringify_map[otype] = (str_func, msg)
         cls._jsonify_logger.info(f"[CustomJSONEncoder] register_stringify: ({otype}:{str_func}),{msg}")
 
-
-    register_stringify(
-        type(date),
-        lambda x: x.strftime('%Y-%m-%d'),
-        msg="fmt:'%Y-%m-%d'"
-    )
-    register_stringify(
-        type(datetime),
-        lambda x: x.strftime('%Y-%m-%d %H:%M:%S'),
-        msg="fmt:'%Y-%m-%d' %Y-%m-%d %H:%M:%S"
-    )
-    register_stringify(
-        type(uuid.UUID),
-        str,
-    )
-
     @classmethod
     def serialize(cls, obj, strict=False, **kwargs):
         ##; common types
         cvt = cls._get_stringify(obj, **kwargs)
         if callable(cvt):
             return cvt(obj)
         elif not strict:
@@ -128,18 +114,44 @@
                 _kwargs=kwargs,
             )
 
     def default(self, obj):
         return self.serialize(obj, strict=self._jsonify_strict)
 
 
-def json_format(data, indent=2, autoflat=True, cls=CustomJSONEncoder, ensure_ascii=False, **kwargs):
+CustomJSONEncoder.register_stringify(
+    date,
+    lambda x: x.strftime('%Y-%m-%d'),
+    msg="fmt:'%Y-%m-%d'"
+)
+CustomJSONEncoder.register_stringify(
+    datetime,
+    lambda x: x.strftime('%Y-%m-%d %H:%M:%S'),
+    msg="fmt:'%Y-%m-%d' %Y-%m-%d %H:%M:%S"
+)
+CustomJSONEncoder.register_stringify(
+    uuid.UUID,
+    str,
+)
+
+
+def json_format(data, indent=2, autoflat=True, cls=CustomJSONEncoder, ensure_ascii=False, default=None, **kwargs):
     if isinstance(data, str) and autoflat:
         data = parse_json(data)
+    if cls is None:
+        return json.dumps(data, indent=indent, default=default)
     return json.dumps(
         data, indent=indent,
         cls=cls, ensure_ascii=ensure_ascii, **kwargs
     )
 
 
-##; json_stringify 总能返回字符串结果, 不会抛出 TypeError
-json_stringify = lambda obj: json.dumps(obj, indent=2, default=CustomJSONEncoder.serialize)
+def json_dumps(data, default=CustomJSONEncoder.serialize):
+    return orjson.dumps(
+        data,
+        default=default,
+        option=(
+            orjson.OPT_NON_STR_KEYS
+            | orjson.OPT_APPEND_NEWLINE
+            | orjson.OPT_PASSTHROUGH_DATETIME
+        )
+    )  # type: bytes
```

### Comparing `pyco-types-1.1.9/pyco_types/co_regex.py` & `pyco-types-1.2.2/pyco_types/co_regex.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types/const.py` & `pyco-types-1.2.2/pyco_types/const.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/pyco_types.egg-info/PKG-INFO` & `pyco-types-1.2.2/pyco_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.9
+Version: 1.2.2
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.9/pyco_types.egg-info/SOURCES.txt` & `pyco-types-1.2.2/pyco_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.9/setup.py` & `pyco-types-1.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,10 +32,11 @@
     url="https://github.com/vmicode/pyco-types",
     author="dodoru",
     author_email="dodoru@foxmail.com",
     packages=find_packages(exclude=('tests', 'tests.*', 'docs', 'examples', '*.tests')),
     include_package_data=True,
     platforms="any",
     install_requires=[
-        "python-dateutil>=2.4.0"
+        "python-dateutil>=2.4.0",
+        "orjson>=3.10.0",
     ]
 )
```

