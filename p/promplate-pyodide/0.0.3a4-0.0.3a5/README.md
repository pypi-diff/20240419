# Comparing `tmp/promplate_pyodide-0.0.3a4.tar.gz` & `tmp/promplate_pyodide-0.0.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate_pyodide-0.0.3a4.tar", last modified: Fri Mar  8 13:18:39 2024, max compression
+gzip compressed data, was "promplate_pyodide-0.0.3a5.tar", last modified: Fri Mar  8 13:43:18 2024, max compression
```

## Comparing `promplate_pyodide-0.0.3a4.tar` & `promplate_pyodide-0.0.3a5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      638 2024-03-03 12:43:31.933218 promplate_pyodide-0.0.3a4/README.md
--rw-r--r--   0        0        0      761 2024-03-08 13:18:39.617061 promplate_pyodide-0.0.3a4/pyproject.toml
--rw-r--r--   0        0        0     3761 2024-03-08 13:18:08.733301 promplate_pyodide-0.0.3a4/src/promplate_pyodide/__init__.py
--rw-r--r--   0        0        0     1503 2024-03-08 13:18:05.212931 promplate_pyodide-0.0.3a4/src/promplate_pyodide/utils/openai.py
--rw-r--r--   0        0        0      283 2024-03-08 08:23:05.264511 promplate_pyodide-0.0.3a4/src/promplate_pyodide/utils/proxy.py
--rw-r--r--   0        0        0      448 2024-03-08 13:18:08.733301 promplate_pyodide-0.0.3a4/src/promplate_pyodide/utils/warn.py
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 promplate_pyodide-0.0.3a4/PKG-INFO
+-rw-r--r--   0        0        0      638 2024-03-03 12:43:31.933218 promplate_pyodide-0.0.3a5/README.md
+-rw-r--r--   0        0        0      761 2024-03-08 13:43:18.937331 promplate_pyodide-0.0.3a5/pyproject.toml
+-rw-r--r--   0        0        0     3815 2024-03-08 13:43:00.603863 promplate_pyodide-0.0.3a5/src/promplate_pyodide/__init__.py
+-rw-r--r--   0        0        0     1503 2024-03-08 13:18:05.212931 promplate_pyodide-0.0.3a5/src/promplate_pyodide/utils/openai.py
+-rw-r--r--   0        0        0      283 2024-03-08 08:23:05.264511 promplate_pyodide-0.0.3a5/src/promplate_pyodide/utils/proxy.py
+-rw-r--r--   0        0        0      448 2024-03-08 13:18:08.733301 promplate_pyodide-0.0.3a5/src/promplate_pyodide/utils/warn.py
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 promplate_pyodide-0.0.3a5/PKG-INFO
```

### Comparing `promplate_pyodide-0.0.3a4/README.md` & `promplate_pyodide-0.0.3a5/README.md`

 * *Files identical despite different names*

### Comparing `promplate_pyodide-0.0.3a4/pyproject.toml` & `promplate_pyodide-0.0.3a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promplate-pyodide"
-version = "0.0.3a4"
+version = "0.0.3a5"
 description = "patches for promplate-core for running in pyodide runtime"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
     "promplate>=0.3.3.4,<0.3.4",
 ]
```

### Comparing `promplate_pyodide-0.0.3a4/src/promplate_pyodide/__init__.py` & `promplate_pyodide-0.0.3a5/src/promplate_pyodide/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,24 +30,26 @@
 
             res = open_url(cls._join_url(url))
             obj = cls(res.read())
             obj.name = Path(url).stem
 
             return obj
 
-    class Node(Loader, patch_class(promplate.Node)):
+    class Node(Loader, promplate.Node):
         """patched for making HTTP requests in pyodide runtime"""
 
-    class Template(Loader, patch_class(promplate.Template)):
+    class Template(Loader, promplate.Template):
         """patched for making HTTP requests in pyodide runtime"""
 
     promplate.template.Loader = Loader
     promplate.template.Template = promplate.Template = Template
     promplate.node.Node = promplate.Node = Node
 
+    promplate.node.Interruptable = patch_class(promplate.node.Interruptable)
+
     from .utils.proxy import to_js
 
     with suppress(ModuleNotFoundError):
         import promplate.llm.openai as o
 
         o.TextComplete = o.TextGenerate = o.ChatComplete = o.ChatGenerate = o.SyncTextOpenAI = o.SyncChatOpenAI = o.v1.TextComplete = o.v1.TextGenerate = o.v1.ChatComplete = o.v1.ChatGenerate = o.v1.SyncTextOpenAI = o.v1.SyncChatOpenAI = NotImplementedWarning  # fmt: off
```

### Comparing `promplate_pyodide-0.0.3a4/src/promplate_pyodide/utils/openai.py` & `promplate_pyodide-0.0.3a5/src/promplate_pyodide/utils/openai.py`

 * *Files identical despite different names*

### Comparing `promplate_pyodide-0.0.3a4/PKG-INFO` & `promplate_pyodide-0.0.3a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promplate-pyodide
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: patches for promplate-core for running in pyodide runtime
 Author-Email: Muspi Merol <me@promplate.dev>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: promplate<0.3.4,>=0.3.3.4
 Description-Content-Type: text/markdown
```

