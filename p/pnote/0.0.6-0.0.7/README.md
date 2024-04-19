# Comparing `tmp/pnote-0.0.6.tar.gz` & `tmp/pnote-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnote-0.0.6.tar", last modified: Wed Feb 14 14:37:16 2024, max compression
+gzip compressed data, was "pnote-0.0.7.tar", last modified: Wed Feb 14 14:48:29 2024, max compression
```

## Comparing `pnote-0.0.6.tar` & `pnote-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:37:16.213627 pnote-0.0.6/
--rw-r--r--   0 loic      (1000) loic      (1000)      615 2024-02-14 14:37:16.213627 pnote-0.0.6/PKG-INFO
--rw-r--r--   0 loic      (1000) loic      (1000)      461 2024-02-11 09:06:20.000000 pnote-0.0.6/README.md
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:37:16.213627 pnote-0.0.6/pnote/
--rw-r--r--   0 loic      (1000) loic      (1000)       55 2024-02-14 14:37:01.000000 pnote-0.0.6/pnote/__init__.py
--rw-r--r--   0 loic      (1000) loic      (1000)     1045 2024-02-14 08:55:19.000000 pnote-0.0.6/pnote/__main__.py
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:37:16.213627 pnote-0.0.6/pnote/layouts/
--rw-r--r--   0 loic      (1000) loic      (1000)       68 2024-02-14 14:30:03.000000 pnote-0.0.6/pnote/layouts/__init__.py
--rw-r--r--   0 loic      (1000) loic      (1000)      219 2024-02-13 08:30:46.000000 pnote-0.0.6/pnote/layouts/flat.py
--rw-r--r--   0 loic      (1000) loic      (1000)     1219 2024-02-14 14:36:21.000000 pnote-0.0.6/pnote/layouts/layout.py
--rw-r--r--   0 loic      (1000) loic      (1000)      244 2024-02-14 14:28:30.000000 pnote-0.0.6/pnote/layouts/yearly.py
--rw-r--r--   0 loic      (1000) loic      (1000)     3809 2024-02-14 08:55:19.000000 pnote-0.0.6/pnote/metadata.py
--rw-r--r--   0 loic      (1000) loic      (1000)     6248 2024-02-14 14:33:39.000000 pnote-0.0.6/pnote/project.py
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:37:16.213627 pnote-0.0.6/pnote/tools/
--rw-r--r--   0 loic      (1000) loic      (1000)       95 2024-02-14 08:55:19.000000 pnote-0.0.6/pnote/tools/__init__.py
--rw-r--r--   0 loic      (1000) loic      (1000)      428 2024-02-14 09:02:23.000000 pnote-0.0.6/pnote/tools/admin.py
--rw-r--r--   0 loic      (1000) loic      (1000)     1684 2024-02-14 14:16:49.000000 pnote-0.0.6/pnote/tools/search.py
--rw-r--r--   0 loic      (1000) loic      (1000)      850 2024-02-14 08:55:19.000000 pnote-0.0.6/pnote/tools/tag.py
--rw-r--r--   0 loic      (1000) loic      (1000)      112 2024-02-11 06:02:38.000000 pnote-0.0.6/pnote/tools/tool.py
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:37:16.213627 pnote-0.0.6/pnote.egg-info/
--rw-r--r--   0 loic      (1000) loic      (1000)      615 2024-02-14 14:37:16.000000 pnote-0.0.6/pnote.egg-info/PKG-INFO
--rw-r--r--   0 loic      (1000) loic      (1000)      473 2024-02-14 14:37:16.000000 pnote-0.0.6/pnote.egg-info/SOURCES.txt
--rw-r--r--   0 loic      (1000) loic      (1000)        1 2024-02-14 14:37:16.000000 pnote-0.0.6/pnote.egg-info/dependency_links.txt
--rw-r--r--   0 loic      (1000) loic      (1000)       37 2024-02-14 14:37:16.000000 pnote-0.0.6/pnote.egg-info/entry_points.txt
--rw-r--r--   0 loic      (1000) loic      (1000)       11 2024-02-14 14:37:16.000000 pnote-0.0.6/pnote.egg-info/requires.txt
--rw-r--r--   0 loic      (1000) loic      (1000)       19 2024-02-14 14:37:16.000000 pnote-0.0.6/pnote.egg-info/top_level.txt
--rwxr-xr-x   0 loic      (1000) loic      (1000)      382 2024-02-10 11:51:32.000000 pnote-0.0.6/pyproject.toml
--rw-r--r--   0 loic      (1000) loic      (1000)       38 2024-02-14 14:37:16.213627 pnote-0.0.6/setup.cfg
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:48:29.091527 pnote-0.0.7/
+-rw-r--r--   0 loic      (1000) loic      (1000)      615 2024-02-14 14:48:29.091527 pnote-0.0.7/PKG-INFO
+-rw-r--r--   0 loic      (1000) loic      (1000)      461 2024-02-11 09:06:20.000000 pnote-0.0.7/README.md
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:48:29.088194 pnote-0.0.7/pnote/
+-rw-r--r--   0 loic      (1000) loic      (1000)       55 2024-02-14 14:48:09.000000 pnote-0.0.7/pnote/__init__.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     1045 2024-02-14 08:55:19.000000 pnote-0.0.7/pnote/__main__.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     1238 2024-02-14 14:45:20.000000 pnote-0.0.7/pnote/layout.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     3809 2024-02-14 08:55:19.000000 pnote-0.0.7/pnote/metadata.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     6117 2024-02-14 14:47:48.000000 pnote-0.0.7/pnote/project.py
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:48:29.091527 pnote-0.0.7/pnote/tools/
+-rw-r--r--   0 loic      (1000) loic      (1000)       95 2024-02-14 08:55:19.000000 pnote-0.0.7/pnote/tools/__init__.py
+-rw-r--r--   0 loic      (1000) loic      (1000)      428 2024-02-14 09:02:23.000000 pnote-0.0.7/pnote/tools/admin.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     1684 2024-02-14 14:16:49.000000 pnote-0.0.7/pnote/tools/search.py
+-rw-r--r--   0 loic      (1000) loic      (1000)      850 2024-02-14 08:55:19.000000 pnote-0.0.7/pnote/tools/tag.py
+-rw-r--r--   0 loic      (1000) loic      (1000)      112 2024-02-11 06:02:38.000000 pnote-0.0.7/pnote/tools/tool.py
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2024-02-14 14:48:29.091527 pnote-0.0.7/pnote.egg-info/
+-rw-r--r--   0 loic      (1000) loic      (1000)      615 2024-02-14 14:48:29.000000 pnote-0.0.7/pnote.egg-info/PKG-INFO
+-rw-r--r--   0 loic      (1000) loic      (1000)      393 2024-02-14 14:48:29.000000 pnote-0.0.7/pnote.egg-info/SOURCES.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)        1 2024-02-14 14:48:29.000000 pnote-0.0.7/pnote.egg-info/dependency_links.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)       37 2024-02-14 14:48:29.000000 pnote-0.0.7/pnote.egg-info/entry_points.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)       11 2024-02-14 14:48:29.000000 pnote-0.0.7/pnote.egg-info/requires.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)       19 2024-02-14 14:48:29.000000 pnote-0.0.7/pnote.egg-info/top_level.txt
+-rwxr-xr-x   0 loic      (1000) loic      (1000)      382 2024-02-10 11:51:32.000000 pnote-0.0.7/pyproject.toml
+-rw-r--r--   0 loic      (1000) loic      (1000)       38 2024-02-14 14:48:29.091527 pnote-0.0.7/setup.cfg
```

### Comparing `pnote-0.0.6/PKG-INFO` & `pnote-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnote
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple note management tool
 Description-Content-Type: text/markdown
 Requires-Dist: jsonschema
 
 # Manage your notes with pnote!
 
 ## About
```

### Comparing `pnote-0.0.6/pnote/__main__.py` & `pnote-0.0.7/pnote/__main__.py`

 * *Files identical despite different names*

### Comparing `pnote-0.0.6/pnote/layouts/layout.py` & `pnote-0.0.7/pnote/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,24 +20,24 @@
     def create(self):
         file=self.todaypath()
         if not os.path.exists(file):
             open(file, 'a').close()
         return self.todaysubpath()
         
     def todayname(self):
-        format=self.today.strftime('%Y-%m-%d')
-        return format+self.conf["extension"]
+        return self.today.strftime(self.conf["filename"])
 
     def todaysubdir(self):
         """
         Must be overriden by child classes
         """
-        pass
+        subdir=self.today.strftime(self.conf["layout"])
+        if not os.path.exists(subdir):
+            Path(os.path.join(self.paths["files"],subdir)).mkdir(parents=True, exist_ok=True)
+        return subdir
 
     def todaysubpath(self):
         subdir=self.todaysubdir()
-        if not os.path.exists(self.todaysubdir()):
-            Path(os.path.join(self.paths["files"],subdir)).mkdir(parents=True, exist_ok=True)
         return os.path.join(self.todaysubdir(), self.todayname())
     
     def todaypath(self):
         return os.path.join(self.paths["files"],self.todaysubpath())
```

### Comparing `pnote-0.0.6/pnote/metadata.py` & `pnote-0.0.7/pnote/metadata.py`

 * *Files identical despite different names*

### Comparing `pnote-0.0.6/pnote/project.py` & `pnote-0.0.7/pnote/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os, json, socket, re, subprocess
 from datetime import datetime
 from jsonschema import validate
 from pathlib import Path
-from pnote.layouts import *
+from pnote.layout import *
 from pnote.metadata import *
 
 class ProjectConfig:
     FILE="config.json"
     DEFAULT_CONFIG = {
-        "layout": "flat",
-        "extension":".md",
+        "layout": "%Y/%m",
+        "filename": "%Y-%m-%d.md",
         "editor": "vim",
         "template": ""
     }
     SCHEMA_CONFIG = {
         "type": "object",
         "properties": {
             "layout": {"type": "string"},
-            "exension": {"type": "string"},
+            "filename": {"type": "string"},
             "editor": {"type": "string"},
             "template": {"type": "string"}
         },
         "required":[
             "layout",
-            "extension",
+            "filename",
             "editor",
             "template"
         ]
     }
     
     def __init__(self, root):
         self.pfile=os.path.join(root,self.FILE)
@@ -69,20 +69,16 @@
         }
 
         Path(self.paths["root"]).mkdir(parents=True, exist_ok=True)
         Path(self.paths["files"]).mkdir(parents=True, exist_ok=True)
 
         self.conf=ProjectConfig(self.paths["root"])
         self.metadata=Metadata(self.paths)
+        self.layout=Layout(self.conf,self.paths)
         
-        if self.conf["layout"]=="yearly":
-            self.layout=LayoutYearly(self.conf, self.paths)
-        else:
-            self.layout=LayoutFlat(self.conf, self.paths)
-            
         if os.path.exists(self.paths["lockfile"]):
             print("Your project contains a lock file! Your project might be corrupted :(")
             exit(1)
 
     def lock(self):
         open(self.paths["lockfile"], 'a').close()
```

### Comparing `pnote-0.0.6/pnote/tools/search.py` & `pnote-0.0.7/pnote/tools/search.py`

 * *Files identical despite different names*

### Comparing `pnote-0.0.6/pnote/tools/tag.py` & `pnote-0.0.7/pnote/tools/tag.py`

 * *Files identical despite different names*

### Comparing `pnote-0.0.6/pnote.egg-info/PKG-INFO` & `pnote-0.0.7/pnote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnote
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple note management tool
 Description-Content-Type: text/markdown
 Requires-Dist: jsonschema
 
 # Manage your notes with pnote!
 
 ## About
```

