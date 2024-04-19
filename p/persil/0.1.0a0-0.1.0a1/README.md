# Comparing `tmp/persil-0.1.0a0.tar.gz` & `tmp/persil-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persil-0.1.0a0.tar", max compression
+gzip compressed data, was "persil-0.1.0a1.tar", max compression
```

## Comparing `persil-0.1.0a0.tar` & `persil-0.1.0a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2024-04-02 20:20:57.077884 persil-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     4328 2024-04-02 20:20:57.077884 persil-0.1.0a0/README.md
--rw-r--r--   0        0        0      462 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/__init__.py
--rw-r--r--   0        0        0    14293 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parser.py
--rw-r--r--   0        0        0      197 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parsers/__init__.py
--rw-r--r--   0        0        0      816 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parsers/from_enum.py
--rw-r--r--   0        0        0      413 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parsers/index.py
--rw-r--r--   0        0        0      362 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parsers/outcome.py
--rw-r--r--   0        0        0     1581 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parsers/regex.py
--rw-r--r--   0        0        0      869 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parsers/string.py
--rw-r--r--   0        0        0      827 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/parsers/tag.py
--rw-r--r--   0        0        0        0 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/py.typed
--rw-r--r--   0        0        0     1258 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/result.py
--rw-r--r--   0        0        0     1378 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/stream.py
--rw-r--r--   0        0        0      983 2024-04-02 20:20:57.077884 persil-0.1.0a0/persil/utils.py
--rw-r--r--   0        0        0      685 2024-04-02 20:20:57.077884 persil-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     4834 1970-01-01 00:00:00.000000 persil-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 20:34:50.010369 persil-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     4548 2024-04-02 20:34:50.010369 persil-0.1.0a1/README.md
+-rw-r--r--   0        0        0      462 2024-04-02 20:34:50.010369 persil-0.1.0a1/persil/__init__.py
+-rw-r--r--   0        0        0    14293 2024-04-02 20:34:50.010369 persil-0.1.0a1/persil/parser.py
+-rw-r--r--   0        0        0      197 2024-04-02 20:34:50.010369 persil-0.1.0a1/persil/parsers/__init__.py
+-rw-r--r--   0        0        0      816 2024-04-02 20:34:50.010369 persil-0.1.0a1/persil/parsers/from_enum.py
+-rw-r--r--   0        0        0      413 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/parsers/index.py
+-rw-r--r--   0        0        0      362 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/parsers/outcome.py
+-rw-r--r--   0        0        0     1581 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/parsers/regex.py
+-rw-r--r--   0        0        0      869 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/parsers/string.py
+-rw-r--r--   0        0        0      827 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/parsers/tag.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/py.typed
+-rw-r--r--   0        0        0     1258 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/result.py
+-rw-r--r--   0        0        0     1378 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/stream.py
+-rw-r--r--   0        0        0      983 2024-04-02 20:34:50.014369 persil-0.1.0a1/persil/utils.py
+-rw-r--r--   0        0        0      685 2024-04-02 20:34:50.014369 persil-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5054 1970-01-01 00:00:00.000000 persil-0.1.0a1/PKG-INFO
```

### Comparing `persil-0.1.0a0/LICENSE` & `persil-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/README.md` & `persil-0.1.0a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,28 +17,33 @@
 shortcuts had to be taken in many cases.
 
 ## Getting started
 
 Persil is a pure-Python library. You can install it with pip:
 
 ```shell
-pip install git+https://github.com/bdura/persil
+pip install persil
 ```
 
 Then, you can play with persil much the same way you would with Parsy,
 and enjoy the great developer experience that type-hinting brings to Persil.
 
 ### A basic example
 
 ```python
 from persil import regex
 
 year = regex(r"\d{4}").map(int)
 ```
 
+This example should drive home the point that Persil is heavily inspired by Parsy.
+The only difference in this particular case is type-safety:
+the persil version knows that `year` is a parser that expects
+a `str`, and outputs an `int`.
+
 ### More complex parsers
 
 Parsy uses generator functions as a most elegant solution to define complex parser.
 
 While you can still use this approach with Persil, you're encouraged to favour
 the `from_streamer` decorator:
 
@@ -134,8 +139,8 @@
     stream.apply(slash_parser)
     month = stream.apply(day_month_parser)
     stream.apply(slash_parser)
     day = stream.apply(day_month_parser)
     return datetime(year, month, day)
 ```
 
-That way, the parsers are only defined once.
+That way, the lower-level parsers are only defined once.
```

### Comparing `persil-0.1.0a0/persil/parser.py` & `persil-0.1.0a1/persil/parser.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/persil/parsers/from_enum.py` & `persil-0.1.0a1/persil/parsers/from_enum.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/persil/parsers/regex.py` & `persil-0.1.0a1/persil/parsers/regex.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/persil/parsers/string.py` & `persil-0.1.0a1/persil/parsers/string.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/persil/parsers/tag.py` & `persil-0.1.0a1/persil/parsers/tag.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/persil/result.py` & `persil-0.1.0a1/persil/result.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/persil/stream.py` & `persil-0.1.0a1/persil/stream.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/persil/utils.py` & `persil-0.1.0a1/persil/utils.py`

 * *Files identical despite different names*

### Comparing `persil-0.1.0a0/pyproject.toml` & `persil-0.1.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "persil"
-version = "0.1.0-alpha0"
+version = "0.1.0-alpha1"
 description = "Persil is a pure-python parsing library, inspired by Parsy"
 authors = ["Basile Dura <basile@bdura.me>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `persil-0.1.0a0/PKG-INFO` & `persil-0.1.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persil
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Persil is a pure-python parsing library, inspired by Parsy
 License: MIT
 Author: Basile Dura
 Author-email: basile@bdura.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,28 +32,33 @@
 shortcuts had to be taken in many cases.
 
 ## Getting started
 
 Persil is a pure-Python library. You can install it with pip:
 
 ```shell
-pip install git+https://github.com/bdura/persil
+pip install persil
 ```
 
 Then, you can play with persil much the same way you would with Parsy,
 and enjoy the great developer experience that type-hinting brings to Persil.
 
 ### A basic example
 
 ```python
 from persil import regex
 
 year = regex(r"\d{4}").map(int)
 ```
 
+This example should drive home the point that Persil is heavily inspired by Parsy.
+The only difference in this particular case is type-safety:
+the persil version knows that `year` is a parser that expects
+a `str`, and outputs an `int`.
+
 ### More complex parsers
 
 Parsy uses generator functions as a most elegant solution to define complex parser.
 
 While you can still use this approach with Persil, you're encouraged to favour
 the `from_streamer` decorator:
 
@@ -149,9 +154,9 @@
     stream.apply(slash_parser)
     month = stream.apply(day_month_parser)
     stream.apply(slash_parser)
     day = stream.apply(day_month_parser)
     return datetime(year, month, day)
 ```
 
-That way, the parsers are only defined once.
+That way, the lower-level parsers are only defined once.
```

