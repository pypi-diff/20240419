# Comparing `tmp/pip_blame-0.2.2.tar.gz` & `tmp/pip_blame-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_blame-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pip_blame-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_blame-0.2.2.tar` & `pip_blame-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-12 22:44:10.475997 pip_blame-0.2.2/.gitignore
--rw-r--r--   0        0        0     2964 2024-04-19 10:03:08.886163 pip_blame-0.2.2/pip_blame.py
--rw-r--r--   0        0        0      516 2024-04-19 10:02:57.337185 pip_blame-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1617 2024-04-19 09:54:07.022889 pip_blame-0.2.2/readme.md
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pip_blame-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-12 22:44:10.475997 pip_blame-0.2.3/.gitignore
+-rw-r--r--   0        0        0     3000 2024-04-19 13:42:18.952844 pip_blame-0.2.3/pip_blame.py
+-rw-r--r--   0        0        0      516 2024-04-19 13:45:17.274577 pip_blame-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1617 2024-04-19 09:54:07.022889 pip_blame-0.2.3/readme.md
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pip_blame-0.2.3/PKG-INFO
```

### Comparing `pip_blame-0.2.2/pip_blame.py` & `pip_blame-0.2.3/pip_blame.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     requires: list[Requirement]
 
     @classmethod
     def from_pypi(cls, name: str):
         metadata = requests.get(f"https://pypi.org/pypi/{name}/json").json()
         return cls(
             version=metadata["info"]["version"],
-            requires=[Requirement(req) for req in metadata["info"]["requires_dist"]],
+            requires=[
+                Requirement(req) for req in metadata["info"]["requires_dist"] or []
+            ],
         )
 
     @classmethod
     def from_dist(cls, dist: Distribution):
         return cls(
             version=dist.version,
             requires=[Requirement(req) for req in dist.requires or []],
```

### Comparing `pip_blame-0.2.2/pyproject.toml` & `pip_blame-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "requests >=2.31",
   "rich >=13.7.1",
 ]
 description = "finds packages that prevent upgrading a transitive dependency"
 name = "pip-blame"
 readme = 'readme.md'
 requires-python = ">=3.8"
-version = "0.2.2"
+version = "0.2.3"
 
 [tool.flit.module]
 name = "pip_blame"
 
 [project.urls]
 Home = "https://github.com/banteg/pip-blame"
```

### Comparing `pip_blame-0.2.2/readme.md` & `pip_blame-0.2.3/readme.md`

 * *Files identical despite different names*

### Comparing `pip_blame-0.2.2/PKG-INFO` & `pip_blame-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-blame
-Version: 0.2.2
+Version: 0.2.3
 Summary: finds packages that prevent upgrading a transitive dependency
 Author: banteg
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging >=24
 Requires-Dist: requests >=2.31
 Requires-Dist: rich >=13.7.1
```

