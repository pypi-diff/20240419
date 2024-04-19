# Comparing `tmp/miniscons-0.7.6.tar.gz` & `tmp/miniscons-0.8.0.tar.gz`

## Comparing `miniscons-0.7.6.tar` & `miniscons-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/build.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/compiler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/containers.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/environment.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/flag.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/routine.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/script.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/target.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.7.6/src/tasks.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.7.6/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.7.6/LICENSE.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.7.6/README.md
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 miniscons-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/build.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/compiler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/containers.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/environment.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/flag.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/routine.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/script.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/target.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.8.0/src/tasks.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.8.0/README.md
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 miniscons-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.8.0/PKG-INFO
```

### Comparing `miniscons-0.7.6/src/build.py` & `miniscons-0.8.0/src/build.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.6/src/script.py` & `miniscons-0.8.0/src/script.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.6/src/target.py` & `miniscons-0.8.0/src/target.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.6/src/tasks.py` & `miniscons-0.8.0/src/tasks.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.6/LICENSE.md` & `miniscons-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.6/pyproject.toml` & `miniscons-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "miniscons"
 description = "SCons builders."
-version = "0.7.6"
+version = "0.8.0"
 
 keywords = ["SCons", "SConstruct", "builders"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `miniscons-0.7.6/PKG-INFO` & `miniscons-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: miniscons
-Version: 0.7.6
+Version: 0.8.0
 Summary: SCons builders.
 Project-URL: Homepage, https://github.com/JoelLefkowitz/miniscons
 Author-email: Joel Lefkowitz <joellefkowitz@hotmail.com>
 License: # MIT License
         
         Copyright (c) 2024 Joel Lefkowitz
```

