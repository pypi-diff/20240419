# Comparing `tmp/pyco-types-1.1.8.tar.gz` & `tmp/pyco-types-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyco-types-1.1.8.tar", last modified: Fri Apr 12 09:09:56 2024, max compression
+gzip compressed data, was "dist/pyco-types-1.1.9.tar", last modified: Fri Apr 19 02:50:49 2024, max compression
```

## Comparing `pyco-types-1.1.8.tar` & `pyco-types-1.1.9.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-12 09:09:56.878771 pyco-types-1.1.8/
--rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.1.8/LICENSE.txt
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-12 09:09:56.878407 pyco-types-1.1.8/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)       42 2023-09-11 08:05:54.000000 pyco-types-1.1.8/README.md
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-12 09:09:56.875002 pyco-types-1.1.8/pyco_types/
--rw-r--r--   0 nico       (502) staff       (20)      327 2023-09-13 03:32:10.000000 pyco-types-1.1.8/pyco_types/__init__.py
--rw-r--r--   0 nico       (502) staff       (20)     3709 2024-01-05 13:47:40.000000 pyco-types-1.1.8/pyco_types/_common.py
--rw-r--r--   0 nico       (502) staff       (20)     2109 2024-01-05 13:12:01.000000 pyco-types-1.1.8/pyco_types/_convert_meta.py
--rw-r--r--   0 nico       (502) staff       (20)     4111 2024-04-12 09:01:18.000000 pyco-types-1.1.8/pyco_types/_factory.py
--rw-r--r--   0 nico       (502) staff       (20)     6233 2024-04-11 04:36:21.000000 pyco-types-1.1.8/pyco_types/_int_exts.py
--rw-r--r--   0 nico       (502) staff       (20)      185 2024-04-12 09:05:39.000000 pyco-types-1.1.8/pyco_types/_version.py
--rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.1.8/pyco_types/co_datetime.py
--rw-r--r--   0 nico       (502) staff       (20)     2573 2024-04-11 02:14:39.000000 pyco-types-1.1.8/pyco_types/co_dict.py
--rw-r--r--   0 nico       (502) staff       (20)     3141 2024-04-12 09:07:04.000000 pyco-types-1.1.8/pyco_types/co_ext_base.py
--rw-r--r--   0 nico       (502) staff       (20)     2651 2024-04-11 04:25:38.000000 pyco-types-1.1.8/pyco_types/co_integer.py
--rw-r--r--   0 nico       (502) staff       (20)     3755 2024-01-05 13:43:50.000000 pyco-types-1.1.8/pyco_types/co_json.py
--rw-r--r--   0 nico       (502) staff       (20)     5156 2023-09-10 03:46:01.000000 pyco-types-1.1.8/pyco_types/co_regex.py
--rw-r--r--   0 nico       (502) staff       (20)     6473 2024-01-02 13:02:23.000000 pyco-types-1.1.8/pyco_types/const.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-12 09:09:56.877934 pyco-types-1.1.8/pyco_types.egg-info/
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)      506 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/SOURCES.txt
--rw-r--r--   0 nico       (502) staff       (20)        1 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/dependency_links.txt
--rw-r--r--   0 nico       (502) staff       (20)       23 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/requires.txt
--rw-r--r--   0 nico       (502) staff       (20)       11 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/top_level.txt
--rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-12 09:09:56.878937 pyco-types-1.1.8/setup.cfg
--rw-r--r--   0 nico       (502) staff       (20)     1283 2024-01-01 11:35:19.000000 pyco-types-1.1.8/setup.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 02:50:49.414783 pyco-types-1.1.9/
+-rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.1.9/LICENSE.txt
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-19 02:50:49.413699 pyco-types-1.1.9/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)      226 2024-04-12 09:35:12.000000 pyco-types-1.1.9/README.md
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 02:50:49.406510 pyco-types-1.1.9/pyco_types/
+-rw-r--r--   0 nico       (502) staff       (20)      341 2024-04-18 11:47:23.000000 pyco-types-1.1.9/pyco_types/__init__.py
+-rw-r--r--   0 nico       (502) staff       (20)     1918 2024-04-18 14:06:09.000000 pyco-types-1.1.9/pyco_types/_cls_base.py
+-rw-r--r--   0 nico       (502) staff       (20)     3567 2024-04-18 08:58:05.000000 pyco-types-1.1.9/pyco_types/_cls_meta.py
+-rw-r--r--   0 nico       (502) staff       (20)     4314 2024-04-18 13:44:40.000000 pyco-types-1.1.9/pyco_types/_common.py
+-rw-r--r--   0 nico       (502) staff       (20)     2109 2024-04-18 11:46:56.000000 pyco-types-1.1.9/pyco_types/_convert_meta.py
+-rw-r--r--   0 nico       (502) staff       (20)     2314 2024-04-12 09:56:26.000000 pyco-types-1.1.9/pyco_types/_filter_funcs.py
+-rw-r--r--   0 nico       (502) staff       (20)     6330 2024-04-18 08:50:19.000000 pyco-types-1.1.9/pyco_types/_int_exts.py
+-rw-r--r--   0 nico       (502) staff       (20)      185 2024-04-19 02:50:27.000000 pyco-types-1.1.9/pyco_types/_version.py
+-rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.1.9/pyco_types/co_datetime.py
+-rw-r--r--   0 nico       (502) staff       (20)     2573 2024-04-18 11:47:23.000000 pyco-types-1.1.9/pyco_types/co_dict.py
+-rw-r--r--   0 nico       (502) staff       (20)     4824 2024-04-18 14:28:01.000000 pyco-types-1.1.9/pyco_types/co_ext_base.py
+-rw-r--r--   0 nico       (502) staff       (20)      722 2024-04-18 12:50:55.000000 pyco-types-1.1.9/pyco_types/co_func.py
+-rw-r--r--   0 nico       (502) staff       (20)     2651 2024-04-11 04:25:38.000000 pyco-types-1.1.9/pyco_types/co_integer.py
+-rw-r--r--   0 nico       (502) staff       (20)      662 2024-04-18 13:19:22.000000 pyco-types-1.1.9/pyco_types/co_interface.tmp.py
+-rw-r--r--   0 nico       (502) staff       (20)     5034 2024-04-19 02:21:26.000000 pyco-types-1.1.9/pyco_types/co_json.py
+-rw-r--r--   0 nico       (502) staff       (20)     5156 2024-04-18 11:46:59.000000 pyco-types-1.1.9/pyco_types/co_regex.py
+-rw-r--r--   0 nico       (502) staff       (20)     6473 2024-04-18 11:46:56.000000 pyco-types-1.1.9/pyco_types/const.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-19 02:50:49.412304 pyco-types-1.1.9/pyco_types.egg-info/
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)      612 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (502) staff       (20)        1 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (502) staff       (20)       23 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/requires.txt
+-rw-r--r--   0 nico       (502) staff       (20)       11 2024-04-19 02:50:49.000000 pyco-types-1.1.9/pyco_types.egg-info/top_level.txt
+-rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-19 02:50:49.415445 pyco-types-1.1.9/setup.cfg
+-rw-r--r--   0 nico       (502) staff       (20)     1283 2024-01-01 11:35:19.000000 pyco-types-1.1.9/setup.py
```

### Comparing `pyco-types-1.1.8/LICENSE.txt` & `pyco-types-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.8/PKG-INFO` & `pyco-types-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.8
+Version: 1.1.9
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.8/pyco_types/_common.py` & `pyco-types-1.1.9/pyco_types/_common.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,25 +8,32 @@
 import builtins
 from pprint import pformat
 from collections import OrderedDict
 from types import FunctionType, ModuleType, MethodType
 
 
 class Symbol:
-    __slots__ = ["name", "kwargs"]
+    __slots__ = ["name", "bool_val", "kwargs"]
 
-    def __init__(self, name=".", **kwargs):
+    def __init__(self, name=".", bool_val=True, **kwargs):
         self.name = name
+        self.bool_val = bool_val
         self.kwargs = kwargs
 
     def __repr__(self):
         return f"<Symbol({self.name})>"
 
+    def __bool__(self):
+        return bool(self.bool_val)
 
-G_Symbol_UNSET = Symbol("UNSET")
+    def __eq__(self, other):
+        return id(self) == id(other)
+
+
+G_Symbol_UNSET = Symbol("UNSET", False)
 
 ##; @formatter:on
 ##; 不可变的简单类型（基本类型)
 ##; cannot import name 'NoneType' from 'types' !!!
 K_Python_Basic_Types = (
     type(None),
     str,
@@ -53,14 +60,28 @@
     bytearray,
     uuid.UUID,
     datetime.datetime,
     datetime.timedelta,
     datetime.date,
 )
 
+# K_Python_Object_Attrs = dir(object) 
+K_Python_Object_Attrs = [
+    '__class__', '__doc__',
+    '__hash__', '__init__', '__new__',
+    '__init_subclass__', '__subclasshook__',
+    '__dir__', '__setattr__', '__delattr__',
+    '__getattribute__', '__sizeof__',
+    '__reduce__', '__reduce_ex__',
+    '__str__', '__repr__', '__format__',
+    '__eq__', '__ne__',
+    '__ge__', '__gt__',
+    '__le__', '__lt__',
+]
+
 
 ##; @formatter:off
 
 def list_builin_type_names():
     attr_list = dir(builtins)
     basic_types = [name for name in attr_list if isinstance(getattr(builtins, name), type)]
     return basic_types
```

### Comparing `pyco-types-1.1.8/pyco_types/_convert_meta.py` & `pyco-types-1.1.9/pyco_types/_convert_meta.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.8/pyco_types/_factory.py` & `pyco-types-1.1.9/pyco_types/_cls_meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,46 +15,43 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 ##; Utilities: python3.8/site-packages/six
 """
- 
+
 __author__ = "Benjamin Peterson <benjamin@python.org>"
 __version__ = "1.16.0"
 
 ##: Usage: 以下三者写法是等价的
 ### 1:
 class A(metaclass=SingletonMeta):
     pass
 
 ### 2:
 class A(with_metaclass(SingletonMeta)):
     pass
-    
+
 ### 3:
 @add_metaclass(SingletonMeta)
 class A():
     pass
-        
+
 """
 
 from __future__ import absolute_import
 
-import functools
-import itertools
-import operator
 import sys
 import types
 
 
 class SingletonMeta(type):
     def __init__(cls, *args, **kwargs):
-        cls.__instance = None
+        cls.__instance = None                                                     
         super(SingletonMeta, cls).__init__(*args, **kwargs)
 
     def __call__(cls, *args, **kwargs):
         if cls.__instance is None:
             cls.__instance = super(SingletonMeta, cls).__call__(*args, **kwargs)
         return cls.__instance
 
@@ -99,27 +96,7 @@
         orig_vars.pop('__dict__', None)
         orig_vars.pop('__weakref__', None)
         if hasattr(cls, '__qualname__'):
             orig_vars['__qualname__'] = cls.__qualname__
         return metaclass(cls.__name__, cls.__bases__, orig_vars)
 
     return wrapper
-
-
-def wrap_base_class(*base_class):
-    """
-    @wrap_base_class(BaseClass)
-    class ParentClass():
-        def __init__(self, *args, **kwargs):
-            print("ParentClass __init__ called")
-    """
-
-    def decorator(cls):
-        class WrappedClass(cls, *base_class):
-            def __init__(self, *args, **kwargs):
-                base_class.__init__(self, *args, **kwargs)
-                if hasattr(cls, '__init__'):
-                    cls.__init__(self, *args, **kwargs)
-
-        return WrappedClass
-
-    return decorator
```

### Comparing `pyco-types-1.1.8/pyco_types/_int_exts.py` & `pyco-types-1.1.9/pyco_types/_int_exts.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,25 @@
     ("=", "查询字符串中的键值对分隔符"),
     ("+", "空格的编码（在查询字符串中）"),
     ("$", "在某些上下文中用作分隔符"),
     (",", "在某些上下文中用作分隔符"),
 ]
 
 
-def str2int(vstr: str, base: int, **kwargs):
+def str2int(vstr: str, base: int, charsets=None, **kwargs):
     # charsets = kwargs.get("charsets", EXT_INTSTR_CHARSETS)
-    char_map = kwargs.get("char_map", DEF_INTSTR_CHAR_MAP)
+    if isinstance(charsets, str):
+        char_map = dict((c, v) for v, c in enumerate(charsets))
+    else:
+        char_map = kwargs.get("char_map", DEF_INTSTR_CHAR_MAP)
     num = 0
     for i, char in enumerate(vstr):
-        v = char_map[char]
-        if v >= base:
-            raise Exception(f"invalid $base({base})<=$char({char}:{v}), $vstr={vstr}[{i}]")
+        v = char_map.get(char, None)
+        if v is None or v >= base:
+            raise Exception(f"invalid $base({base}), with $vstr[{i}]={char}({v})")
         else:
             num = num * base + v
     return num
 
 
 def int2str(vnum: int, base: int, charsets=DEF_INTSTR_CHARSETS):
     """
@@ -143,36 +146,36 @@
 
 
 def uint_from_str(
     vstr: str, default_base: int = 10,
     default_value=0, charsets=DEF_INTSTR_CHARSETS, **kwargs
 ):
     ##; NOTE: 只支持无符号的整形数值，不支持浮点数
+    if not vstr:
+        return default_value
+
     max_b = len(charsets)
-    prefix_map = kwargs.get("prefix_map", DEF_PREFIX_BASE_MAP)  # type: dict
     if default_base > max_b:
         raise ValueError(
             f"Invalid $default_base=({default_base}), it must be ranged in [2, {max_b}]"
             f", or <= 0(default=10, -1 is depends on $vstr.prefix), $charsets={charsets}"
         )
-    if not vstr:
-        return default_value
 
+    prefix_map = kwargs.get("prefix_map", DEF_PREFIX_BASE_MAP)  # type: dict
     p = vstr[:2]
     base = prefix_map.get(p, None)
+    char_map = dict((c, v) for v, c in enumerate(charsets))
     if base is None:
-        if p.isdigit():
+        if p.isdigit() and default_base <= 36:
             return int(vstr, default_base)
         elif default_base > 2:
-            char_map = dict((c, v) for v, c in enumerate(charsets))
             return str2int(vstr, default_base, char_map=char_map)
         else:
             raise ValueError(
                 f"Invalid $default_base={default_base}, $vstr.prefix={p},\n"
                 f"Expected $prefix_map=({pformat(prefix_map)})"
                 f",$vstr.size=len({vstr}({vstr[:20]})"
             )
     else:
         if default_base > 2 and default_base != base:
             warnings.warn(f"check $base={base}({p}), but$default_base={default_base}")
-        char_map = dict((c, v) for v, c in enumerate(charsets))
-        return str2int(vstr, base, char_map=char_map)
+        return str2int(vstr[2:], base, char_map=char_map)
```

### Comparing `pyco-types-1.1.8/pyco_types/co_datetime.py` & `pyco-types-1.1.9/pyco_types/co_datetime.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.8/pyco_types/co_dict.py` & `pyco-types-1.1.9/pyco_types/co_dict.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.8/pyco_types/co_integer.py` & `pyco-types-1.1.9/pyco_types/co_integer.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.8/pyco_types/co_json.py` & `pyco-types-1.1.9/pyco_types/co_json.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import uuid
 # import inspect
 from pprint import pformat
-from datetime import datetime
+from datetime import datetime, date
 from logging import root as logger
 from pyco_types._convert_meta import find_converter, Converter
-from pyco_types._common import K_Python_Common_Types, CommonException
+from pyco_types._common import K_Python_Common_Types, CommonException, G_Symbol_UNSET
 
 
 def pformat_any(data, depth=2, width=80, indent=2, **kwargs):
     return " :: ".join([str(type(data)), pformat(data, indent=indent, width=width, depth=depth)])
 
 
 def parse_json(data, **kwargs):
@@ -48,65 +48,92 @@
         "getJson",  # json response
         "toDict",
         "asDict",  # SQLAlchemy Rows
     ]
 
     ##； @_jsonify_strict: 如果设置为 True, 则尝试使用原生 JSON, 可能会异常
     ##； @_jsonify_strict: 如果设置为 False, 则不管怎样都能返回 序列化的结果（不一定符合预期）
-    _custom_kwargs = dict(
-        datetime_fmt='%Y-%m-%d %H:%M:%S',
-        jsonify_methods=_jsonify_methods,
-    )
     _jsonify_strict = False
-    _pformat_depth = 2
-    _datetime_fmt = '%Y-%m-%d %H:%M:%S'
+    _jsonify_logger = logger
+    __stringify_map = dict()  # (k:Type, v:Tuple(func, msg))
 
     @classmethod
-    def stringify_with_converter(cls, obj):
-        cvt = find_converter(obj)
-        if cvt is None:
-            return False, pformat_any(obj, depth=cls._pformat_depth)
-        else:
-            return True, cvt.stringify(obj)
+    def _get_stringify(cls, obj,
+                       with_converter=True,
+                       with_methods=True,
+                       flag_property=True,
+                       **kwargs,
+                       ):
+        cvt, _ = cls.__stringify_map.get(type(obj), (G_Symbol_UNSET, "_"))
+        if cvt is G_Symbol_UNSET:
+            if with_converter:
+                cvter = find_converter(obj)
+                if isinstance(cvter, Converter):
+                    ##; stringify with Converter class_method
+                    cvt = cvter.stringify
+                    cls.register_stringify(type(obj), cvt, f"converter={cvter}")
+                    return cvt
+            if with_methods:
+                for k in cls._jsonify_methods:
+                    fn = getattr(obj, k, G_Symbol_UNSET)  ## instance_method
+                    if fn is G_Symbol_UNSET:
+                        continue
+                    elif callable(fn):
+                        ##; stringify with instance_method
+                        cvt = lambda x, method=k: getattr(x, method)()
+                        cls.register_stringify(type(obj), cvt, f"method={k}")
+                        break
+                    elif isinstance(fn, K_Python_Common_Types) and flag_property:
+                        ##; stringify with instance_property
+                        cvt = lambda x, property=k: getattr(x, property, G_Symbol_UNSET)
+                        cls.register_stringify(type(obj), cvt, f"property={k}")
+                        break
+        return cvt
+
+    @classmethod
+    def register_stringify(cls, otype, str_func, msg="-"):
+        cls.__stringify_map[otype] = (str_func, msg)
+        cls._jsonify_logger.info(f"[CustomJSONEncoder] register_stringify: ({otype}:{str_func}),{msg}")
+
+
+    register_stringify(
+        type(date),
+        lambda x: x.strftime('%Y-%m-%d'),
+        msg="fmt:'%Y-%m-%d'"
+    )
+    register_stringify(
+        type(datetime),
+        lambda x: x.strftime('%Y-%m-%d %H:%M:%S'),
+        msg="fmt:'%Y-%m-%d' %Y-%m-%d %H:%M:%S"
+    )
+    register_stringify(
+        type(uuid.UUID),
+        str,
+    )
 
     @classmethod
-    def serialize(cls, obj, strict=False, with_converter=True, **kwargs):
+    def serialize(cls, obj, strict=False, **kwargs):
         ##; common types
-        datetime_fmt = kwargs.pop("datetime_fmt", cls._datetime_fmt)
-        if isinstance(obj, datetime):
-            # default use TZ-LOCAL, eg: "2021-03-22 20:32:02.271068+08:00"
-            return obj.strftime(datetime_fmt)
-        elif isinstance(obj, uuid.UUID):
-            return str(obj)
-
-        ##; stringify with instance
-        for k in cls._jsonify_methods:
-            fn = getattr(obj, k, None)  ## instance_method
-            if callable(fn):
-                return fn()
-            elif isinstance(fn, K_Python_Common_Types):
-                return fn
-
-        ##; stringify_with_converter
-        if with_converter:
-            flag, txt = cls.stringify_with_converter(obj)
-            if flag:
-                return txt
-            elif not strict:
-                return txt
-
-        raise CommonException(
-            f"Object({type(obj)}) is not serializable. \nobj:{obj}",
-            errno=50020,
-            origin=obj,
-            with_converter=with_converter,
-        )
+        cvt = cls._get_stringify(obj, **kwargs)
+        if callable(cvt):
+            return cvt(obj)
+        elif not strict:
+            func = kwargs.get("default", pformat_any)
+            return func(obj)
+        else:
+            raise CommonException(
+                f"Object({type(obj)}) is not registered with stringify"
+                f"\nobj:{obj}",
+                errno=50020,
+                origin=obj,
+                _kwargs=kwargs,
+            )
 
     def default(self, obj):
-        return self.serialize(obj, strict=True)
+        return self.serialize(obj, strict=self._jsonify_strict)
 
 
 def json_format(data, indent=2, autoflat=True, cls=CustomJSONEncoder, ensure_ascii=False, **kwargs):
     if isinstance(data, str) and autoflat:
         data = parse_json(data)
     return json.dumps(
         data, indent=indent,
```

### Comparing `pyco-types-1.1.8/pyco_types/co_regex.py` & `pyco-types-1.1.9/pyco_types/co_regex.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.8/pyco_types/const.py` & `pyco-types-1.1.9/pyco_types/const.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.8/pyco_types.egg-info/PKG-INFO` & `pyco-types-1.1.9/pyco_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.8
+Version: 1.1.9
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.8/setup.py` & `pyco-types-1.1.9/setup.py`

 * *Files identical despite different names*

