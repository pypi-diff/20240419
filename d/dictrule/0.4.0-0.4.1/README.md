# Comparing `tmp/dictrule-0.4.0.tar.gz` & `tmp/dictrule-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictrule-0.4.0.tar", last modified: Tue Apr 16 13:04:27 2024, max compression
+gzip compressed data, was "dictrule-0.4.1.tar", last modified: Fri Apr 19 19:27:28 2024, max compression
```

## Comparing `dictrule-0.4.0.tar` & `dictrule-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:04:27.579697 dictrule-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 13:04:21.000000 dictrule-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-04-16 13:04:27.575697 dictrule-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-16 13:04:21.000000 dictrule-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:04:27.579697 dictrule-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-16 13:04:21.000000 dictrule-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:04:27.571697 dictrule-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:04:27.575697 dictrule-0.4.0/src/dictrule/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:04:27.575697 dictrule-0.4.0/src/dictrule/built_in_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/comment_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/for_in_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/format_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/indent_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/inline_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/join_block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/join_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/built_in_rules/stringify_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/dr_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 13:04:21.000000 dictrule-0.4.0/src/dictrule/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:04:27.575697 dictrule-0.4.0/src/dictrule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-04-16 13:04:27.000000 dictrule-0.4.0/src/dictrule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-16 13:04:27.000000 dictrule-0.4.0/src/dictrule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:04:27.000000 dictrule-0.4.0/src/dictrule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:04:27.000000 dictrule-0.4.0/src/dictrule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 13:04:27.000000 dictrule-0.4.0/src/dictrule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.072445 dictrule-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 19:27:25.000000 dictrule-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-04-19 19:27:28.068445 dictrule-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-19 19:27:25.000000 dictrule-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:27:28.072445 dictrule-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-19 19:27:25.000000 dictrule-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.064445 dictrule-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.068445 dictrule-0.4.1/src/dictrule/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.068445 dictrule-0.4.1/src/dictrule/built_in_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/comment_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/for_in_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/format_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/indent_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/inline_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/join_block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/join_eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/stringify_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/dr_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/var_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.068445 dictrule-0.4.1/src/dictrule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/top_level.txt
```

### Comparing `dictrule-0.4.0/LICENSE` & `dictrule-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/PKG-INFO` & `dictrule-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
```

### Comparing `dictrule-0.4.0/README.md` & `dictrule-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/setup.py` & `dictrule-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/__init__.py` & `dictrule-0.4.1/src/dictrule/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 \__,_/_/\___/\__/_/   \__,_/_/\___/ 
 
 """
 
 from .generator import Generator
 from .rule import Rule
 from .context import Context
+from .var_property import var_property
+from .variable import Variable
 from .__version__ import (
     __title__,
     __description__,
     __url__,
     __version__,
     __author__,
     __author_email__,
@@ -51,14 +53,16 @@
     "EvalRule",
     "InlineRule",
     "IndentRule",
     "ForInRule",
     "JoinBlockRule",
     "JoinEvalRule",
     "FormatRule",
+    "var_property",
+    "Variable",
     "__title__",
     "__description__",
     "__url__",
     "__version__",
     "__author__",
     "__author_email__",
     "__license__",
```

### Comparing `dictrule-0.4.0/src/dictrule/__version__.py` & `dictrule-0.4.1/src/dictrule/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 \__,_/_/\___/\__/_/   \__,_/_/\___/    |___/\___/_/  /____/_/\____/_/ /_/ 
                                                                           
 """
 
 __title__ = "dictrule"
 __description__ = "Python rules defined by a dict and a text generator from the rules"
 __url__ = "https://github.com/elhoangvu/dictrule"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __author__ = "Zooxy Le"
 __author_email__ = "elhoangvu@gmail.com"
 __license__ = "MIT License"
 __copyright__ = "Copyright Zooxy Le"
```

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/__init__.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/block_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/block_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/comment_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/comment_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/eval_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/eval_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/for_in_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/for_in_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/format_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/format_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/indent_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/indent_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/inline_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/inline_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/join_block_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/join_block_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/join_eval_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/join_eval_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/built_in_rules/stringify_rule.py` & `dictrule-0.4.1/src/dictrule/built_in_rules/stringify_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/context.py` & `dictrule-0.4.1/src/dictrule/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 )
 
 from abc import (
     ABC,
 )
 
 from .exceptions import (
-    NoneValueException,
     InvalidValueException,
 )
 
 
 class Context:
     """Context class contains information for rule generation"""
 
@@ -46,18 +45,14 @@
         case_map: Dict[str, Context.Case] = {}
         for case in cases:
             if case.name in case_map:
                 raise InvalidValueException(
                     f"Found existed {Context.Case.__name__}: {case.name}"
                 )
 
-            name = case.name
-            if name is None:
-                raise NoneValueException(f"Invalid case name `{name}`")
-
             case_map[case.name] = case
 
         self._case_map = case_map
 
     @property
     def cases(self) -> List[Case]:
         """Getter for `cases` property
```

### Comparing `dictrule-0.4.0/src/dictrule/dr_property.py` & `dictrule-0.4.1/src/dictrule/dr_property.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,22 +16,27 @@
 
 class dr_property:
     """dictrule decorator that defines property for rules.
     Supports prefix matching and optional properties
 
     Properties decorated with `dr_property` must have the `dr_property._prefix` prefix.
 
-    Usage:
-        - Defines:
-            @dr_property(prefix_matching=True, optional=True)
-            def _eval(self, props: Dict[str, Any]) -> Any:
-                pass
-        - Parses:
-            key, value = self._eval(rule_dict)
-
+    Examples:
+    ---------
+    >>> rule_dict = {
+    ...     "eval": "prop.name"
+    ... }
+    >>> @dr_property(prefix_matching=True, optional=True)
+    ... def _eval(self, props: Dict[str, Any]) -> Any:
+    ...     pass
+    >>> key, value = self._eval(rule_dict)
+    >>> print(key)
+    eval
+    >>> print(value)
+    prop.name
     """
 
     _prefix = "_"
     _flag_key = "_is_dr_property"
     _name_key = "_dr_name"
     _optional_key = "_dr_optional"
```

### Comparing `dictrule-0.4.0/src/dictrule/generator.py` & `dictrule-0.4.1/src/dictrule/generator.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule/rule.py` & `dictrule-0.4.1/src/dictrule/rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.0/src/dictrule.egg-info/PKG-INFO` & `dictrule-0.4.1/src/dictrule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
```

### Comparing `dictrule-0.4.0/src/dictrule.egg-info/SOURCES.txt` & `dictrule-0.4.1/src/dictrule.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 src/dictrule/__init__.py
 src/dictrule/__version__.py
 src/dictrule/context.py
 src/dictrule/dr_property.py
 src/dictrule/exceptions.py
 src/dictrule/generator.py
 src/dictrule/rule.py
+src/dictrule/var_property.py
+src/dictrule/variable.py
 src/dictrule.egg-info/PKG-INFO
 src/dictrule.egg-info/SOURCES.txt
 src/dictrule.egg-info/dependency_links.txt
 src/dictrule.egg-info/not-zip-safe
 src/dictrule.egg-info/top_level.txt
 src/dictrule/built_in_rules/__init__.py
 src/dictrule/built_in_rules/block_rule.py
```

