# Comparing `tmp/miniscons-0.6.0.tar.gz` & `tmp/miniscons-0.7.0.tar.gz`

## Comparing `miniscons-0.6.0.tar` & `miniscons-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,15 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/__init__.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/builds/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/builds/build.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/builds/target.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/__init__.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/flag.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/routine.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/services/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/services/compiler.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/services/environment.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.6.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.6.0/LICENSE.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.6.0/README.md
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 miniscons-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/__init__.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/build.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/compiler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/containers.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/environment.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/flag.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/routine.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/script.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/target.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.7.0/src/tasks.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.7.0/README.md
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 miniscons-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.7.0/PKG-INFO
```

### Comparing `miniscons-0.6.0/src/models/tasks.py` & `miniscons-0.7.0/src/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
-from .builds.build import Build
-from .scripts.flag import Flag
-from .scripts.routine import Routine
-from .scripts.script import Script
-from .builds.target import Target
+from .build import Build
+from .flag import Flag
+from .routine import Routine
+from .script import Script
+from .target import Target
 from dataclasses import dataclass, field
 from SCons.Environment import Environment
 
 
 @dataclass
 class Tasks:
-    builds: list[Build]
-
+    builds: list[Build] = field(default_factory=list)
     targets: list[Target] = field(default_factory=list)
     scripts: list[Script] = field(default_factory=list)
     routines: list[Routine] = field(default_factory=list)
     flags: list[Flag] = field(default_factory=list)
 
-    def __str__(self) -> str:
+    @property
+    def cli(self) -> str:
         fields = "\n\n".join(
             [
                 ":".join(
                     [k, "".join([f"\n  {i}" for i in v] if len(v) > 0 else "\n  -")]
                 )
                 for k, v in self.__dict__.items()
             ]
         )
 
         return f"\n{fields}\n"
 
     def dump(self) -> None:
-        sys.stdout.write(f"{self}\n")
+        sys.stdout.write(f"{self.cli}\n")
 
     def register(self, env: Environment) -> None:
         for group in self.__dict__.values():
             for task in group:
                 task.register(env)
```

### Comparing `miniscons-0.6.0/src/models/builds/target.py` & `miniscons-0.7.0/src/target.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.6.0/src/models/scripts/script.py` & `miniscons-0.7.0/src/build.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,23 @@
+import os
 from dataclasses import dataclass, field
 from SCons.Environment import Environment
-from typing import Optional
 
 
 @dataclass
-class Script:
+class Build:
     name: str
 
-    args: list[str] = field(default_factory=list)
-    prefix: Optional[str] = None
+    files: list[str] = field(default_factory=list)
+    flags: list[str] = field(default_factory=list)
+    output: str = "dist"
 
     def __repr__(self) -> str:
         return self.name
 
     @property
-    def action(self) -> str:
-        segments = [self.name, *self.args]
-
-        if self.prefix:
-            segments.insert(0, self.prefix)
-
-        return " ".join(segments)
+    def target(self) -> str:
+        return os.path.join(self.output, self.name)
 
     def register(self, env: Environment) -> None:
-        alias = env.Alias(self.name, [], self.action)
-        env.AlwaysBuild(alias)
+        env.Program(self.target, source=self.files, CXXFLAGS=self.flags)
+        env.Alias(self.name, self.target)
```

### Comparing `miniscons-0.6.0/LICENSE.md` & `miniscons-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniscons-0.6.0/pyproject.toml` & `miniscons-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "miniscons"
 description = "SCons builders."
-version = "0.6.0"
+version = "0.7.0"
 
 keywords = ["SCons", "SConstruct", "builders"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -65,15 +65,15 @@
 
 [tool.hatch.build.targets.wheel.sources]
 src = "miniscons"
 
 [tool.thx.jobs]
 lint = [
     "npx cspell . --dot",
-    "pylint src --disable=C0114,C0115,C0116,C0411",
+    "pylint src --disable=C0114,C0115,C0116,C0411,C3001",
     "mypy -m src --ignore-missing-import",
 ]
 
 format = [
     "black .",
     "isort . --no-sections --remove-redundant-aliases",
     "npx prettier . --write",
```

### Comparing `miniscons-0.6.0/PKG-INFO` & `miniscons-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: miniscons
-Version: 0.6.0
+Version: 0.7.0
 Summary: SCons builders.
 Project-URL: Homepage, https://github.com/JoelLefkowitz/miniscons
 Author-email: Joel Lefkowitz <joellefkowitz@hotmail.com>
 License: # MIT License
         
         Copyright (c) 2024 Joel Lefkowitz
```

