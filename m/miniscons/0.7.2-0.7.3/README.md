# Comparing `tmp/miniscons-0.7.2.tar.gz` & `tmp/miniscons-0.7.3.tar.gz`

## Comparing `miniscons-0.7.2.tar` & `miniscons-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/build.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/compiler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/containers.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/environment.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/flag.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/routine.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/script.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/target.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.7.2/src/tasks.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.7.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.7.2/LICENSE.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.7.2/README.md
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 miniscons-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/build.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/compiler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/containers.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/environment.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/flag.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/routine.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/script.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/target.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.7.3/src/tasks.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.7.3/LICENSE.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.7.3/README.md
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 miniscons-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.7.3/PKG-INFO
```

### Comparing `miniscons-0.7.2/src/build.py` & `miniscons-0.7.3/src/build.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 @dataclass
 class Build:
     name: str
 
     files: list[str] = field(default_factory=list)
     flags: list[str] = field(default_factory=list)
     output: str = "dist"
+    shared: bool = False
 
     def __repr__(self) -> str:
         return self.name
 
     @property
     def target(self) -> str:
         return os.path.join(self.output, self.name)
 
-    def node(self, file: str, env: Environment) -> str:
-        return env.Object(
-            f"{file.replace('.', '-')}-{self.name}", file, CXXFLAGS=self.flags
-        )
+    def nodes(self, env: Environment) -> list[str]:
+        return [
+            env.Object(
+                f"{file.replace('.', '-')}-{self.name}", file, CXXFLAGS=self.flags
+            )
+            for file in self.files
+        ]
 
     def register(self, env: Environment) -> None:
-        env.Program(self.target, [self.node(file, env) for file in self.files])
-        env.Alias(self.name, self.target)
+        if self.shared:
+            env.Library(self.target, self.nodes(env))
+        else:
+            env.Program(self.target, self.nodes(env))
+            env.Alias(self.name, self.target)
```

### Comparing `miniscons-0.7.2/src/script.py` & `miniscons-0.7.3/src/script.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.2/src/target.py` & `miniscons-0.7.3/src/target.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.2/src/tasks.py` & `miniscons-0.7.3/src/tasks.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.2/LICENSE.md` & `miniscons-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniscons-0.7.2/pyproject.toml` & `miniscons-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "miniscons"
 description = "SCons builders."
-version = "0.7.2"
+version = "0.7.3"
 
 keywords = ["SCons", "SConstruct", "builders"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `miniscons-0.7.2/PKG-INFO` & `miniscons-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: miniscons
-Version: 0.7.2
+Version: 0.7.3
 Summary: SCons builders.
 Project-URL: Homepage, https://github.com/JoelLefkowitz/miniscons
 Author-email: Joel Lefkowitz <joellefkowitz@hotmail.com>
 License: # MIT License
         
         Copyright (c) 2024 Joel Lefkowitz
```

