# Comparing `tmp/pip_blame-0.2.0.tar.gz` & `tmp/pip_blame-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_blame-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pip_blame-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_blame-0.2.0.tar` & `pip_blame-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-12 22:44:10.475997 pip_blame-0.2.0/.gitignore
--rw-r--r--   0        0        0     3007 2024-04-19 09:50:02.312330 pip_blame-0.2.0/pip_blame.py
--rw-r--r--   0        0        0      516 2024-04-19 09:49:04.445982 pip_blame-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1618 2024-04-19 08:48:02.594338 pip_blame-0.2.0/readme.md
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 pip_blame-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-12 22:44:10.475997 pip_blame-0.2.1/.gitignore
+-rw-r--r--   0        0        0     2962 2024-04-19 09:52:21.905018 pip_blame-0.2.1/pip_blame.py
+-rw-r--r--   0        0        0      516 2024-04-19 09:52:28.678081 pip_blame-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1617 2024-04-19 09:54:07.022889 pip_blame-0.2.1/readme.md
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pip_blame-0.2.1/PKG-INFO
```

### Comparing `pip_blame-0.2.0/pip_blame.py` & `pip_blame-0.2.1/pip_blame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from importlib.metadata import Distribution, distributions, distribution
 import sys
 
 import requests
 from packaging.requirements import Requirement
 from rich import print
-from rich.rule import Rule
 from dataclasses import dataclass
 
 
 @dataclass
 class Metadata:
     version: str
     requires: list[Requirement]
@@ -32,15 +31,14 @@
         return [req for req in self.requires if req.name == dependency]
 
     def contains(self, dependency, version) -> dict[Requirement, bool]:
         return {req: req.specifier.contains(version) for req in self.filter(dependency)}
 
 
 def main():
-    print(Rule())
     solution = []
     if len(sys.argv) < 2:
         print("usage: pip-blame NAME")
         return
     name = sys.argv[1]
     installed = distribution(name)
     latest = Metadata.from_pypi(name)
```

### Comparing `pip_blame-0.2.0/pyproject.toml` & `pip_blame-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "requests >=2.31",
   "rich >=13.7.1",
 ]
 description = "finds packages that prevent upgrading a transitive dependency"
 name = "pip-blame"
 readme = 'readme.md'
 requires-python = ">=3.8"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.flit.module]
 name = "pip_blame"
 
 [project.urls]
 Home = "https://github.com/banteg/pip-blame"
```

### Comparing `pip_blame-0.2.0/readme.md` & `pip_blame-0.2.1/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # pip-blame
 
 *finds packages that prevent upgrading a transitive dependency*
 
-<img width="500" alt="pip-blame" src="https://github.com/banteg/pip-blame/assets/4562643/e91ca9cf-3a10-42f9-aee7-cec78ff0da74">
-
+<img width="369" alt="pip-blame" src="https://github.com/banteg/pip-blame/assets/4562643/4981ca69-4952-4583-97c3-07dd7e93bed5">
 
 ## install
 
 ```
 pip install pip-blame
 ```
```

### Comparing `pip_blame-0.2.0/PKG-INFO` & `pip_blame-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pip-blame
-Version: 0.2.0
+Version: 0.2.1
 Summary: finds packages that prevent upgrading a transitive dependency
 Author: banteg
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging >=24
 Requires-Dist: requests >=2.31
 Requires-Dist: rich >=13.7.1
 Project-URL: Home, https://github.com/banteg/pip-blame
 
 # pip-blame
 
 *finds packages that prevent upgrading a transitive dependency*
 
-<img width="500" alt="pip-blame" src="https://github.com/banteg/pip-blame/assets/4562643/e91ca9cf-3a10-42f9-aee7-cec78ff0da74">
-
+<img width="369" alt="pip-blame" src="https://github.com/banteg/pip-blame/assets/4562643/4981ca69-4952-4583-97c3-07dd7e93bed5">
 
 ## install
 
 ```
 pip install pip-blame
 ```
```

