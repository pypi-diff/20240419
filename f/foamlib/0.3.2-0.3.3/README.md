# Comparing `tmp/foamlib-0.3.2.tar.gz` & `tmp/foamlib-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.3.2.tar", last modified: Thu Apr 18 01:55:17 2024, max compression
+gzip compressed data, was "foamlib-0.3.3.tar", last modified: Fri Apr 19 14:34:29 2024, max compression
```

## Comparing `foamlib-0.3.2.tar` & `foamlib-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:55:17.307670 foamlib-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-18 01:55:08.000000 foamlib-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-18 01:55:17.307670 foamlib-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-18 01:55:08.000000 foamlib-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:55:17.303670 foamlib-0.3.2/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:55:17.303670 foamlib-0.3.2/foamlib/_files/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_files/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_files/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_files/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_files/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_files/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_files/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:55:08.000000 foamlib-0.3.2/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:55:17.303670 foamlib-0.3.2/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-18 01:55:17.000000 foamlib-0.3.2/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-18 01:55:17.000000 foamlib-0.3.2/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:55:17.000000 foamlib-0.3.2/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 01:55:17.000000 foamlib-0.3.2/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 01:55:17.000000 foamlib-0.3.2/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 01:55:08.000000 foamlib-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:55:17.307670 foamlib-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.014319 foamlib-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-19 14:34:24.000000 foamlib-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-19 14:34:29.014319 foamlib-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-19 14:34:24.000000 foamlib-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.010319 foamlib-0.3.3/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.014319 foamlib-0.3.3/foamlib/_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.014319 foamlib-0.3.3/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 14:34:24.000000 foamlib-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:34:29.014319 foamlib-0.3.3/setup.cfg
```

### Comparing `foamlib-0.3.2/LICENSE.txt` & `foamlib-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/PKG-INFO` & `foamlib-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.2/README.md` & `foamlib-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/foamlib/_cases.py` & `foamlib-0.3.3/foamlib/_cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import aioshutil
 
 from ._files import FoamFieldFile, FoamFile
 from ._util import is_sequence, run_process, run_process_async
 
 
 class FoamCaseBase(Sequence["FoamCaseBase.TimeDirectory"]):
-    def __init__(self, path: Union[Path, str]):
+    def __init__(self, path: Union[Path, str] = Path()):
         self.path = Path(path).absolute()
         if not self.path.is_dir():
             raise NotADirectoryError(f"{self.path} is not a directory")
 
     class TimeDirectory(Set[FoamFieldFile]):
         """
         An OpenFOAM time directory in a case.
```

### Comparing `foamlib-0.3.2/foamlib/_files/_base.py` & `foamlib-0.3.3/foamlib/_files/_base.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/foamlib/_files/_fields.py` & `foamlib-0.3.3/foamlib/_files/_fields.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/foamlib/_files/_files.py` & `foamlib-0.3.3/foamlib/_files/_files.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/foamlib/_files/_io.py` & `foamlib-0.3.3/foamlib/_files/_io.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/foamlib/_files/_parsing.py` & `foamlib-0.3.3/foamlib/_files/_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ParserElement,
     ParseResults,
     QuotedString,
     Word,
     c_style_comment,
     common,
     cpp_style_comment,
-    identbodychars,
+    identchars,
     printables,
 )
 
 from ._base import FoamDict
 
 
 def _list_of(entry: ParserElement) -> ParserElement:
@@ -79,15 +79,15 @@
 ).set_parse_action(lambda: True) | (
     Keyword("no") | Keyword("false") | Keyword("off") | Keyword("n") | Keyword("f")
 ).set_parse_action(lambda: False)
 _DIMENSIONS = (
     Literal("[").suppress() + common.number * 7 + Literal("]").suppress()
 ).set_parse_action(lambda tks: FoamDict.DimensionSet(*tks))
 _TENSOR = _list_of(common.number) | common.number
-_IDENTIFIER = Word(identbodychars + "$", printables.replace(";", ""))
+_IDENTIFIER = Word(identchars + "$", printables, exclude_chars=";")
 _DIMENSIONED = (Opt(_IDENTIFIER) + _DIMENSIONS + _TENSOR).set_parse_action(
     lambda tks: FoamDict.Dimensioned(*reversed(tks.as_list()))
 )
 _FIELD = (Keyword("uniform").suppress() + _TENSOR) | (
     Keyword("nonuniform").suppress() + _list_of(_TENSOR)
 )
 _TOKEN = QuotedString('"', unquote_results=False) | _IDENTIFIER
```

### Comparing `foamlib-0.3.2/foamlib/_files/_serialization.py` & `foamlib-0.3.3/foamlib/_files/_serialization.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/foamlib/_util.py` & `foamlib-0.3.3/foamlib/_util.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.2/foamlib.egg-info/PKG-INFO` & `foamlib-0.3.3/foamlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.2/pyproject.toml` & `foamlib-0.3.3/pyproject.toml`

 * *Files identical despite different names*

