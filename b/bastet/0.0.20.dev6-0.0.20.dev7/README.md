# Comparing `tmp/bastet-0.0.20.dev6.tar.gz` & `tmp/bastet-0.0.20.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastet-0.0.20.dev6.tar", last modified: Fri Apr 19 21:10:05 2024, max compression
+gzip compressed data, was "bastet-0.0.20.dev7.tar", last modified: Fri Apr 19 21:37:59 2024, max compression
```

## Comparing `bastet-0.0.20.dev6.tar` & `bastet-0.0.20.dev7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:10:05.932583 bastet-0.0.20.dev6/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 21:10:05.932583 bastet-0.0.20.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:10:05.932583 bastet-0.0.20.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:10:05.928583 bastet-0.0.20.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:10:05.928583 bastet-0.0.20.dev6/src/bastet/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:10:05.928583 bastet-0.0.20.dev6/src/bastet/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/reporting/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/reporting/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/reporting/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:10:05.932583 bastet-0.0.20.dev6/src/bastet/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/tools/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/tools/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/tools/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/tools/reuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-19 21:09:59.000000 bastet-0.0.20.dev6/src/bastet/tools/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:10:05.932583 bastet-0.0.20.dev6/src/bastet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 21:10:05.000000 bastet-0.0.20.dev6/src/bastet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-19 21:10:05.000000 bastet-0.0.20.dev6/src/bastet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:10:05.000000 bastet-0.0.20.dev6/src/bastet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 21:10:05.000000 bastet-0.0.20.dev6/src/bastet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 21:10:05.000000 bastet-0.0.20.dev6/src/bastet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 21:10:05.000000 bastet-0.0.20.dev6/src/bastet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:10:01.000000 bastet-0.0.20.dev6/version
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:37:59.264308 bastet-0.0.20.dev7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 21:37:59.264308 bastet-0.0.20.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:37:59.264308 bastet-0.0.20.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:37:59.256308 bastet-0.0.20.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:37:59.260308 bastet-0.0.20.dev7/src/bastet/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:37:59.260308 bastet-0.0.20.dev7/src/bastet/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/reporting/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/reporting/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/reporting/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:37:59.264308 bastet-0.0.20.dev7/src/bastet/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/tools/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/tools/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/tools/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/tools/reuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-19 21:37:52.000000 bastet-0.0.20.dev7/src/bastet/tools/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:37:59.264308 bastet-0.0.20.dev7/src/bastet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 21:37:59.000000 bastet-0.0.20.dev7/src/bastet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-19 21:37:59.000000 bastet-0.0.20.dev7/src/bastet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:37:59.000000 bastet-0.0.20.dev7/src/bastet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 21:37:59.000000 bastet-0.0.20.dev7/src/bastet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 21:37:59.000000 bastet-0.0.20.dev7/src/bastet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 21:37:59.000000 bastet-0.0.20.dev7/src/bastet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:37:54.000000 bastet-0.0.20.dev7/version
```

### Comparing `bastet-0.0.20.dev6/PKG-INFO` & `bastet-0.0.20.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastet
-Version: 0.0.20.dev6
+Version: 0.0.20.dev7
 Summary: Bastet Python Developers Tools (https://github.com/mewbotorg/bastet)
 Author-email: MewBot Org <mewbot@quicksilver.london>
 Maintainer-email: MewBot Org <mewbot@quicksilver.london>
 Project-URL: Source, https://github.com/mewbotorg/bastet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bastet-0.0.20.dev6/README.md` & `bastet-0.0.20.dev7/README.md`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/pyproject.toml` & `bastet-0.0.20.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/__main__.py` & `bastet-0.0.20.dev7/src/bastet/__main__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/config.py` & `bastet-0.0.20.dev7/src/bastet/config.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/reporting/__init__.py` & `bastet-0.0.20.dev7/src/bastet/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/reporting/abc.py` & `bastet-0.0.20.dev7/src/bastet/reporting/abc.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/reporting/console.py` & `bastet-0.0.20.dev7/src/bastet/reporting/console.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/reporting/github.py` & `bastet-0.0.20.dev7/src/bastet/reporting/github.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/runner.py` & `bastet-0.0.20.dev7/src/bastet/runner.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/tools/__init__.py` & `bastet-0.0.20.dev7/src/bastet/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/tools/audit.py` & `bastet-0.0.20.dev7/src/bastet/tools/audit.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/tools/exceptions.py` & `bastet-0.0.20.dev7/src/bastet/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/tools/format.py` & `bastet-0.0.20.dev7/src/bastet/tools/format.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/tools/lint.py` & `bastet-0.0.20.dev7/src/bastet/tools/lint.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/tools/reuse.py` & `bastet-0.0.20.dev7/src/bastet/tools/reuse.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet/tools/tool.py` & `bastet-0.0.20.dev7/src/bastet/tools/tool.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev6/src/bastet.egg-info/PKG-INFO` & `bastet-0.0.20.dev7/src/bastet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastet
-Version: 0.0.20.dev6
+Version: 0.0.20.dev7
 Summary: Bastet Python Developers Tools (https://github.com/mewbotorg/bastet)
 Author-email: MewBot Org <mewbot@quicksilver.london>
 Maintainer-email: MewBot Org <mewbot@quicksilver.london>
 Project-URL: Source, https://github.com/mewbotorg/bastet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bastet-0.0.20.dev6/src/bastet.egg-info/SOURCES.txt` & `bastet-0.0.20.dev7/src/bastet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

