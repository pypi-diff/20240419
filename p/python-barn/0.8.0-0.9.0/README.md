# Comparing `tmp/python-barn-0.8.0.tar.gz` & `tmp/python-barn-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-barn-0.8.0.tar", last modified: Tue May 16 21:52:14 2023, max compression
+gzip compressed data, was "python-barn-0.9.0.tar", last modified: Wed Nov  8 11:41:14 2023, max compression
```

## Comparing `python-barn-0.8.0.tar` & `python-barn-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.452464 python-barn-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 21:52:14.452464 python-barn-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 21:52:00.000000 python-barn-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.448463 python-barn-0.8.0/python_barn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:52:14.452464 python-barn-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 21:52:00.000000 python-barn-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.448463 python-barn-0.8.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.452464 python-barn-0.8.0/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/execute_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:41:14.809711 python-barn-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-11-08 11:41:14.805711 python-barn-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-11-08 11:41:04.000000 python-barn-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:41:14.805711 python-barn-0.9.0/python_barn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-11-08 11:41:14.000000 python-barn-0.9.0/python_barn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2023-11-08 11:41:14.000000 python-barn-0.9.0/python_barn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 11:41:14.000000 python-barn-0.9.0/python_barn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 11:41:14.000000 python-barn-0.9.0/python_barn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-08 11:41:14.000000 python-barn-0.9.0/python_barn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-08 11:41:14.000000 python-barn-0.9.0/python_barn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 11:41:14.809711 python-barn-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2023-11-08 11:41:04.000000 python-barn-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:41:14.805711 python-barn-0.9.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:41:14.805711 python-barn-0.9.0/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/actions/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/actions/execute_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/actions/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/actions/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/actions/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/actions/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2023-11-08 11:41:04.000000 python-barn-0.9.0/src/logging_utils.py
```

### Comparing `python-barn-0.8.0/PKG-INFO` & `python-barn-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.8.0
+Version: 0.9.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: PyYAML==6.0
 
 # barn
 
 barn is a Python-based command-line interface (CLI) tool that simplifies package management by providing an intuitive set of commands.
 It was inspired by the **yarn** counterpart from Javascript.
 Hence the interface was kept as similar as possible, so that if you are familiar with yarn you should pickup barn relatively fast.
```

### Comparing `python-barn-0.8.0/README.md` & `python-barn-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `python-barn-0.8.0/python_barn.egg-info/PKG-INFO` & `python-barn-0.9.0/python_barn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.8.0
+Version: 0.9.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: PyYAML==6.0
 
 # barn
 
 barn is a Python-based command-line interface (CLI) tool that simplifies package management by providing an intuitive set of commands.
 It was inspired by the **yarn** counterpart from Javascript.
 Hence the interface was kept as similar as possible, so that if you are familiar with yarn you should pickup barn relatively fast.
```

### Comparing `python-barn-0.8.0/setup.py` & `python-barn-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-barn",
-    version="0.8.0",
+    version="0.9.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "barn=src.cli:main",
         ],
     },
     package_data={
```

### Comparing `python-barn-0.8.0/src/actions/add.py` & `python-barn-0.9.0/src/actions/add.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.8.0/src/actions/execute_script.py` & `python-barn-0.9.0/src/actions/execute_script.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.8.0/src/actions/install.py` & `python-barn-0.9.0/src/actions/install.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.8.0/src/cli.py` & `python-barn-0.9.0/src/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
-from src.actions import install, add, init, execute_script, remove, show
-from src.core import barn_action, Context
 
 def main():
 
     title = r"""
 _________                   
 ______/ /_  ____ __________ 
 _____/ __ \/ __ `/ ___/ __ \
@@ -23,14 +21,16 @@
     class IgnoreUnknownArgParser(argparse.ArgumentParser):
         def error(self, message):
             pass
 
     parser = IgnoreUnknownArgParser(description='Barn CLI tool', add_help=False)
     subparsers = parser.add_subparsers(dest='command')
 
+    add_parser = subparsers.add_parser('init')
+
     # Add 'install' command
     subparsers.add_parser('install')
 
     # Add 'add' command
     add_parser = subparsers.add_parser('add')
     add_parser.add_argument(
         "requirement",
@@ -48,30 +48,36 @@
     # subparsers.add_parser('test')
 
     # Parse the arguments
  
     args, unknown_args = parser.parse_known_args()
 
     exit_code = 0
+
+    if args.command == 'init':
+        from src.actions import init
+        return init()
+
+    from src.actions import install, add, execute_script, remove, show
     if len(unknown_args) > 0 and args.command is None:
         _, exit_code = execute_script(unknown_args[0], unknown_args[1:])
     # If no command is given, print help and exit
     elif args.command is None:
+        print(install)
         _, exit_code = install()
     elif args.command == 'show':
         _, exit_code = show(args.package_name, verbose=args.verbose, files=args.files)
     elif args.command == 'install':
         _, exit_code = install()
     elif args.command == 'remove':
         _, exit_code = remove(args.package_name)
     elif args.command == 'add':
         _, exit_code = add(args.requirement)
-    elif args.command == 'init':
-        init()
     elif args.command == 'test':
+        from src.core import barn_action, Context
         @barn_action
         def test_action(context: Context=None):
             # Do whatever here
             context.add_dependency_to_project_yaml("test", "1.0.0")
         test_action()
     else:
         print("Unknown command: " + args.command)
```

### Comparing `python-barn-0.8.0/src/core.py` & `python-barn-0.9.0/src/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,23 +230,23 @@
 def is_env_initialized(base_dir: Path):
     return (
         (base_dir / "python_modules").is_dir() and
         (base_dir / "python_modules" / "bin" / "activate").is_file()
     )
 
 
-def find_project_yaml():
+def find_project_yaml(init=False):
     current_dir = Path.cwd()
     while current_dir != Path(current_dir.root):
         if is_barn_project(current_dir):
             return current_dir / "project.yaml"
         current_dir = current_dir.parent
-    
-    raise Exception("Barn could not find a project context to use. Are you in a project directory?")
-
+    if not init:
+        raise Exception("Barn could not find a project context to use. Are you in a project directory?")
+    return None
 
 
 
 def barn_action(action):
     project_yaml = find_project_yaml()
     root_dir = project_yaml.parent
     is_initialized = is_env_initialized(root_dir)
```

### Comparing `python-barn-0.8.0/src/logging_utils.py` & `python-barn-0.9.0/src/logging_utils.py`

 * *Files identical despite different names*

