# Comparing `tmp/bastet-0.0.20.dev4.tar.gz` & `tmp/bastet-0.0.20.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastet-0.0.20.dev4.tar", last modified: Fri Apr 19 20:53:34 2024, max compression
+gzip compressed data, was "bastet-0.0.20.dev5.tar", last modified: Fri Apr 19 21:02:15 2024, max compression
```

## Comparing `bastet-0.0.20.dev4.tar` & `bastet-0.0.20.dev5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:34.043272 bastet-0.0.20.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 20:53:34.043272 bastet-0.0.20.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:53:34.047272 bastet-0.0.20.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:34.039272 bastet-0.0.20.dev4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:34.039272 bastet-0.0.20.dev4/src/bastet/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:34.043272 bastet-0.0.20.dev4/src/bastet/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/reporting/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/reporting/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/reporting/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:34.043272 bastet-0.0.20.dev4/src/bastet/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/tools/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/tools/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/tools/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/tools/reuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-04-19 20:53:27.000000 bastet-0.0.20.dev4/src/bastet/tools/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:34.043272 bastet-0.0.20.dev4/src/bastet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 20:53:34.000000 bastet-0.0.20.dev4/src/bastet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-19 20:53:34.000000 bastet-0.0.20.dev4/src/bastet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:53:34.000000 bastet-0.0.20.dev4/src/bastet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 20:53:34.000000 bastet-0.0.20.dev4/src/bastet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 20:53:34.000000 bastet-0.0.20.dev4/src/bastet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 20:53:34.000000 bastet-0.0.20.dev4/src/bastet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 20:53:29.000000 bastet-0.0.20.dev4/version
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:02:15.709315 bastet-0.0.20.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 21:02:15.709315 bastet-0.0.20.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:02:15.709315 bastet-0.0.20.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:02:15.705315 bastet-0.0.20.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:02:15.709315 bastet-0.0.20.dev5/src/bastet/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:02:15.709315 bastet-0.0.20.dev5/src/bastet/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/reporting/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/reporting/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/reporting/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:02:15.709315 bastet-0.0.20.dev5/src/bastet/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/tools/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/tools/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/tools/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/tools/reuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16596 2024-04-19 21:02:09.000000 bastet-0.0.20.dev5/src/bastet/tools/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:02:15.709315 bastet-0.0.20.dev5/src/bastet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 21:02:15.000000 bastet-0.0.20.dev5/src/bastet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-19 21:02:15.000000 bastet-0.0.20.dev5/src/bastet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:02:15.000000 bastet-0.0.20.dev5/src/bastet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 21:02:15.000000 bastet-0.0.20.dev5/src/bastet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 21:02:15.000000 bastet-0.0.20.dev5/src/bastet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 21:02:15.000000 bastet-0.0.20.dev5/src/bastet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:02:11.000000 bastet-0.0.20.dev5/version
```

### Comparing `bastet-0.0.20.dev4/PKG-INFO` & `bastet-0.0.20.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastet
-Version: 0.0.20.dev4
+Version: 0.0.20.dev5
 Summary: Bastet Python Developers Tools (https://github.com/mewbotorg/bastet)
 Author-email: MewBot Org <mewbot@quicksilver.london>
 Maintainer-email: MewBot Org <mewbot@quicksilver.london>
 Project-URL: Source, https://github.com/mewbotorg/bastet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bastet-0.0.20.dev4/README.md` & `bastet-0.0.20.dev5/README.md`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/pyproject.toml` & `bastet-0.0.20.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/__main__.py` & `bastet-0.0.20.dev5/src/bastet/__main__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/config.py` & `bastet-0.0.20.dev5/src/bastet/config.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/reporting/__init__.py` & `bastet-0.0.20.dev5/src/bastet/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/reporting/abc.py` & `bastet-0.0.20.dev5/src/bastet/reporting/abc.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/reporting/console.py` & `bastet-0.0.20.dev5/src/bastet/reporting/console.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/reporting/github.py` & `bastet-0.0.20.dev5/src/bastet/reporting/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,18 @@
     def format_sub_issue(issue: Annotation) -> str:
         """
         Converts an existing annotation into a line of text.
 
         This line can then be placed into an aggregate annotation.
         """
 
-        header = f"- {issue.tool.name} [{issue.code}] {issue.message}"
+        if issue.tool:
+            header = f"- {issue.tool.name} [{issue.code}] {issue.message}"
+        else:
+            header = f"- {issue.message}"
 
         if not issue.description:
             return header
 
         return f"{header}\n{textwrap.indent(issue.message.strip(), '  ')}"
 
     async def close(self) -> None:
```

### Comparing `bastet-0.0.20.dev4/src/bastet/runner.py` & `bastet-0.0.20.dev5/src/bastet/runner.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/tools/__init__.py` & `bastet-0.0.20.dev5/src/bastet/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/tools/audit.py` & `bastet-0.0.20.dev5/src/bastet/tools/audit.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/tools/exceptions.py` & `bastet-0.0.20.dev5/src/bastet/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/tools/format.py` & `bastet-0.0.20.dev5/src/bastet/tools/format.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/tools/lint.py` & `bastet-0.0.20.dev5/src/bastet/tools/lint.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/tools/reuse.py` & `bastet-0.0.20.dev5/src/bastet/tools/reuse.py`

 * *Files identical despite different names*

### Comparing `bastet-0.0.20.dev4/src/bastet/tools/tool.py` & `bastet-0.0.20.dev5/src/bastet/tools/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
         if isinstance(source, pathlib.Path):
             return source.absolute(), 0, 0
 
         return source[0].absolute(), source[1] or 0, source[2] or 0
 
     status: Status
     source: tuple[pathlib.Path, int, int]
-    tool: Tool
+    tool: Tool | None
     code: str
 
     message: str
     description: str | None
     diff: list[str] | None
 
     def __init__(  # noqa: PLR0913 - 6 args is "ok" here.
```

### Comparing `bastet-0.0.20.dev4/src/bastet.egg-info/PKG-INFO` & `bastet-0.0.20.dev5/src/bastet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastet
-Version: 0.0.20.dev4
+Version: 0.0.20.dev5
 Summary: Bastet Python Developers Tools (https://github.com/mewbotorg/bastet)
 Author-email: MewBot Org <mewbot@quicksilver.london>
 Maintainer-email: MewBot Org <mewbot@quicksilver.london>
 Project-URL: Source, https://github.com/mewbotorg/bastet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bastet-0.0.20.dev4/src/bastet.egg-info/SOURCES.txt` & `bastet-0.0.20.dev5/src/bastet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

