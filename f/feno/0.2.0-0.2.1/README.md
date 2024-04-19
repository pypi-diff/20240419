# Comparing `tmp/feno-0.2.0.tar.gz` & `tmp/feno-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.2.0.tar", last modified: Mon Apr  8 17:34:43 2024, max compression
+gzip compressed data, was "feno-0.2.1.tar", last modified: Fri Apr 19 14:05:38 2024, max compression
```

## Comparing `feno-0.2.0.tar` & `feno-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 17:34:43.040024 feno-0.2.0/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.2.0/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.2.0/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 17:34:43.040024 feno-0.2.0/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.2.0/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)     1233 2024-04-08 17:25:27.000000 feno-0.2.0/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.2.0/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-08 17:34:43.043357 feno-0.2.0/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.2.0/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 17:34:43.026691 feno-0.2.0/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 17:34:43.036691 feno-0.2.0/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-08 17:34:31.000000 feno-0.2.0/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2273 2024-04-08 17:24:02.000000 feno-0.2.0/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5271 2024-04-08 17:22:14.000000 feno-0.2.0/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.2.0/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.2.0/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.2.0/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8886 2024-04-08 14:12:05.000000 feno-0.2.0/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.2.0/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4378 2024-04-08 17:28:46.000000 feno-0.2.0/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.2.0/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.2.0/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11894 2024-04-08 15:58:02.000000 feno-0.2.0/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.2.0/src/feno/remote_md.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 17:34:43.040024 feno-0.2.0/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 17:34:43.000000 feno-0.2.0/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-08 17:34:43.000000 feno-0.2.0/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-08 17:34:43.000000 feno-0.2.0/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-08 17:34:43.000000 feno-0.2.0/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-08 17:34:43.000000 feno-0.2.0/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-08 17:34:43.000000 feno-0.2.0/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.800307 feno-0.2.1/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.2.1/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.2.1/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-19 14:05:38.800307 feno-0.2.1/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.2.1/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     1300 2024-04-19 14:05:20.000000 feno-0.2.1/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.2.1/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-19 14:05:38.800307 feno-0.2.1/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3157 2024-04-08 22:42:29.000000 feno-0.2.1/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.780307 feno-0.2.1/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.793640 feno-0.2.1/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-19 14:04:46.000000 feno-0.2.1/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2273 2024-04-08 17:24:02.000000 feno-0.2.1/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5271 2024-04-08 17:22:14.000000 feno-0.2.1/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.2.1/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.2.1/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.2.1/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9189 2024-04-19 14:04:18.000000 feno-0.2.1/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.2.1/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4378 2024-04-08 17:28:46.000000 feno-0.2.1/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.2.1/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4907 2024-04-08 23:40:15.000000 feno-0.2.1/src/feno/lock.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.2.1/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11894 2024-04-08 15:58:02.000000 feno-0.2.1/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.2.1/src/feno/remote_md.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.796974 feno-0.2.1/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      192 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.2.0/LICENSE` & `feno-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/PKG-INFO` & `feno-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.2.0
+Version: 0.2.1
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.2.0/README.md` & `feno-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/changelog.md` & `feno-0.2.1/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+- 0.2.1
+  - add: clear folder without removing it, changing inodes
 - 0.2.0
   - add: improved indexed checking for unused hooks
   - fix: remove extra newline in feno
   - add: ignore node_modules and .json files as feno targets
   - add: indexed needs now base folder as parameter
 - 0.1.9
   - add: mddp filter links procuram em modo recursivo
```

### Comparing `feno-0.2.0/setup.py` & `feno-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example: $ pip install sampleproject[dev]
     # Similar to `install_requires` above, these must be valid existing projects
     extras_require={'dev': ['check-manifest'],
                     'test': ['coverage'],
                     },  # Optional
 
-    entry_points={'console_scripts': ['feno=feno.__main__:main', 'mdpp=feno.mdpp:main', 'filter=feno.filter:main', 'indexer=feno.indexer:main', 'check=feno.check:main'], },
+    entry_points={'console_scripts': ['feno=feno.__main__:main', 'lock=feno.lock:lock', 'unlock=feno.lock:unlock', 'mdpp=feno.mdpp:main', 'filter=feno.filter:main', 'indexer=feno.indexer:main', 'check=feno.check:main'], },
 
     project_urls={'Bug Reports': 'https://github.com/senapk/feno/issues',
                   'Source': 'https://github.com/senapk/feno/',
                   },  # Optional https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
 )
```

### Comparing `feno-0.2.0/src/feno/__main__.py` & `feno-0.2.1/src/feno/__main__.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/actions.py` & `feno-0.2.1/src/feno/actions.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/cases.py` & `feno-0.2.1/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/check.py` & `feno-0.2.1/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/css_style.py` & `feno-0.2.1/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/filter.py` & `feno-0.2.1/src/feno/filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 class Mode(enum.Enum):
     ADD = 1 # inserir cortando por degrau
     RAW = 2 # inserir tudo
     DEL = 3 # apagar tudo
 
 class LegacyFilter:
-    def __init__(self, filename):
+    def __init__(self, filename: str):
+        super().__init__()
         self.mode = Mode.RAW
         self.level = 1
         self.com = "//"
         if filename.endswith(".py"):
             self.com = "#"
         elif filename.endswith(".puml"):
             self.com = "'"
@@ -238,16 +239,21 @@
             print("Error: target must be a folder in recursive mode")
             exit()
         if os.path.exists(args.output):
             if not args.force:
                 print("Error: output folder already exists")
                 exit()
             else:
-                shutil.rmtree(args.output)
-                os.makedirs(args.output)
+                # recursive delete all folder content without deleting the folder itself
+                for file in os.listdir(args.output):
+                    path = os.path.join(args.output, file)
+                    if os.path.isdir(path):
+                        shutil.rmtree(path)
+                    else:
+                        os.remove(path)
 
         deep_filter = DeepFilter().set_cheat(args.cheat).set_quiet(args.quiet).set_indent(args.indent)
         deep_filter.copy(args.target, args.output, 10)
         exit()
 
     file = args.target
     success, content = open_file(file)
```

### Comparing `feno-0.2.0/src/feno/html.py` & `feno-0.2.1/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/indexer.py` & `feno-0.2.1/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/jsontools.py` & `feno-0.2.1/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/mdpp.py` & `feno-0.2.1/src/feno/mdpp.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno/remote_md.py` & `feno-0.2.1/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.0/src/feno.egg-info/PKG-INFO` & `feno-0.2.1/src/feno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.2.0
+Version: 0.2.1
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.2.0/src/feno.egg-info/SOURCES.txt` & `feno-0.2.1/src/feno.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/feno/cases.py
 src/feno/check.py
 src/feno/css_style.py
 src/feno/filter.py
 src/feno/html.py
 src/feno/indexer.py
 src/feno/jsontools.py
+src/feno/lock.py
 src/feno/log.py
 src/feno/mdpp.py
 src/feno/remote_md.py
 src/feno.egg-info/PKG-INFO
 src/feno.egg-info/SOURCES.txt
 src/feno.egg-info/dependency_links.txt
 src/feno.egg-info/entry_points.txt
```

