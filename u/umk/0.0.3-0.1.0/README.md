# Comparing `tmp/umk-0.0.3.tar.gz` & `tmp/umk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umk-0.0.3.tar", max compression
+gzip compressed data, was "umk-0.1.0.tar", max compression
```

## Comparing `umk-0.0.3.tar` & `umk-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,72 @@
--rw-r--r--   0        0        0    35148 2023-11-15 14:17:46.665185 umk-0.0.3/LICENSE
--rw-r--r--   0        0        0     3157 2023-11-15 14:17:46.665185 umk-0.0.3/README.md
--rw-r--r--   0        0        0     1225 2023-11-15 14:18:06.429375 umk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1027 2023-11-15 14:17:46.665185 umk-0.0.3/umk/__init__.py
--rw-r--r--   0        0        0      183 2023-11-15 14:17:46.665185 umk-0.0.3/umk/cli/__init__.py
--rw-r--r--   0        0        0     3658 2023-11-15 14:17:46.665185 umk-0.0.3/umk/cli/main.py
--rw-r--r--   0        0        0      616 2023-11-15 14:17:46.665185 umk-0.0.3/umk/cli/sections.py
--rw-r--r--   0        0        0        0 2023-11-15 14:17:46.665185 umk-0.0.3/umk/delve/__init__.py
--rw-r--r--   0        0        0     2167 2023-11-15 14:17:46.665185 umk-0.0.3/umk/delve/binary.py
--rw-r--r--   0        0        0     5465 2023-11-15 14:17:46.665185 umk-0.0.3/umk/delve/flags.py
--rw-r--r--   0        0        0     7199 2023-11-15 14:17:46.665185 umk-0.0.3/umk/dotunimake.py
--rw-r--r--   0        0        0      953 2023-11-15 14:17:46.665185 umk-0.0.3/umk/entrypoint.py
--rw-r--r--   0        0        0      834 2023-11-15 14:17:46.665185 umk-0.0.3/umk/exceptions.py
--rw-r--r--   0        0        0      797 2023-11-15 14:17:46.665185 umk-0.0.3/umk/globals.py
--rw-r--r--   0        0        0        0 2023-11-15 14:17:46.665185 umk-0.0.3/umk/golang/__init__.py
--rw-r--r--   0        0        0     2533 2023-11-15 14:17:46.665185 umk-0.0.3/umk/golang/build.py
--rw-r--r--   0        0        0     1166 2023-11-15 14:17:46.665185 umk-0.0.3/umk/golang/go.py
--rw-r--r--   0        0        0      803 2023-11-15 14:17:46.665185 umk-0.0.3/umk/golang/mod.py
--rw-r--r--   0        0        0     1161 2023-11-15 14:17:46.665185 umk-0.0.3/umk/golang/project.py
--rw-r--r--   0        0        0     3080 2023-11-15 14:17:46.669185 umk-0.0.3/umk/project.py
--rw-r--r--   0        0        0      215 2023-11-15 14:17:46.669185 umk-0.0.3/umk/remote/__init__.py
--rw-r--r--   0        0        0     5486 2023-11-15 14:17:46.669185 umk-0.0.3/umk/remote/docker.py
--rw-r--r--   0        0        0     2358 2023-11-15 14:17:46.669185 umk-0.0.3/umk/remote/interface.py
--rw-r--r--   0        0        0      934 2023-11-15 14:17:46.669185 umk-0.0.3/umk/remote/register.py
--rw-r--r--   0        0        0        1 2023-11-15 14:17:46.669185 umk-0.0.3/umk/system/__init__.py
--rw-r--r--   0        0        0      159 2023-11-15 14:17:46.669185 umk-0.0.3/umk/system/code.py
--rw-r--r--   0        0        0     1157 2023-11-15 14:17:46.669185 umk-0.0.3/umk/system/environs.py
--rw-r--r--   0        0        0     9498 2023-11-15 14:17:46.669185 umk-0.0.3/umk/system/filesystem.py
--rw-r--r--   0        0        0     7068 2023-11-15 14:17:46.669185 umk-0.0.3/umk/system/shell.py
--rw-r--r--   0        0        0      748 2023-11-15 14:17:46.669185 umk-0.0.3/umk/system/user.py
--rw-r--r--   0        0        0      331 2023-11-15 14:17:46.669185 umk-0.0.3/umk/vcs.py
--rw-r--r--   0        0        0        0 2023-11-15 14:17:46.669185 umk-0.0.3/unimake/__init__.py
--rw-r--r--   0        0        0     5588 2023-11-15 14:17:46.669185 umk-0.0.3/unimake/cli.py
--rw-r--r--   0        0        0      221 2023-11-15 14:17:46.669185 umk-0.0.3/unimake/entrypoint.py
--rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 umk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-18 22:18:42.177750 umk-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5528 2024-04-18 22:18:42.177750 umk-0.1.0/README.md
+-rw-r--r--   0        0        0     1210 2024-04-18 22:18:59.965815 umk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-04-18 22:18:42.181750 umk-0.1.0/umk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/config.py
+-rw-r--r--   0        0        0     5005 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/remote.py
+-rw-r--r--   0        0        0     4061 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/root.py
+-rw-r--r--   0        0        0     1891 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/target.py
+-rw-r--r--   0        0        0     1469 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/printers.py
+-rw-r--r--   0        0        0     3592 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/utils.py
+-rw-r--r--   0        0        0      574 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/errors.py
+-rw-r--r--   0        0        0      860 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/globals.py
+-rw-r--r--   0        0        0     2176 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/properties.py
+-rw-r--r--   0        0        0     3543 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/serialization.py
+-rw-r--r--   0        0        0     1425 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/typings.py
+-rw-r--r--   0        0        0      271 2024-04-18 22:18:42.181750 umk-0.1.0/umk/entrypoint.py
+-rw-r--r--   0        0        0        1 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/__init__.py
+-rw-r--r--   0        0        0     4970 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/delve.py
+-rw-r--r--   0        0        0     4261 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/docker/__init__.py
+-rw-r--r--   0        0        0    37808 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/docker/compose.py
+-rw-r--r--   0        0        0    15930 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/docker/file.py
+-rw-r--r--   0        0        0      368 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/git.py
+-rw-r--r--   0        0        0       61 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/go/__init__.py
+-rw-r--r--   0        0        0    13890 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/go/base.py
+-rw-r--r--   0        0        0       74 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     3170 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/copy.py
+-rw-r--r--   0        0        0     1757 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/factories.py
+-rw-r--r--   0        0        0     2330 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/installer.py
+-rw-r--r--   0        0        0     2617 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/move.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/project/__init__.py
+-rw-r--r--   0        0        0     4506 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/project/base.py
+-rw-r--r--   0        0        0     1559 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/project/golang.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/__init__.py
+-rw-r--r--   0        0        0     7487 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/docker.py
+-rw-r--r--   0        0        0     3072 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/interface.py
+-rw-r--r--   0        0        0     3137 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/ssh.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/__init__.py
+-rw-r--r--   0        0        0     1442 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/environs.py
+-rw-r--r--   0        0        0      791 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/platform.py
+-rw-r--r--   0        0        0     6656 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/shell.py
+-rw-r--r--   0        0        0      763 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/user.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/golang.py
+-rw-r--r--   0        0        0     2149 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/interface.py
+-rw-r--r--   0        0        0     6486 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/packages.py
+-rw-r--r--   0        0        0       64 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/utils/__init__.py
+-rw-r--r--   0        0        0     8514 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/utils/cli.py
+-rw-r--r--   0        0        0      159 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/utils/code.py
+-rw-r--r--   0        0        0      159 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/adapter/__init__.py
+-rw-r--r--   0        0        0     4590 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/adapter/docker/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/adapter/go/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/config/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/filesystem/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/project/__init__.py
+-rw-r--r--   0        0        0     1274 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/remote/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/system/__init__.py
+-rw-r--r--   0        0        0     1394 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/target/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/__init__.py
+-rw-r--r--   0        0        0     7892 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/config.py
+-rw-r--r--   0        0        0     3138 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/container.py
+-rw-r--r--   0        0        0     2630 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/errors.py
+-rw-r--r--   0        0        0     4873 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/project.py
+-rw-r--r--   0        0        0     6631 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/remotes.py
+-rw-r--r--   0        0        0     8982 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/targets.py
+-rw-r--r--   0        0        0     8189 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/utils.py
+-rw-r--r--   0        0        0     1592 2024-04-18 22:18:42.185750 umk-0.1.0/umk/state.py
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 umk-0.1.0/PKG-INFO
```

### Comparing `umk-0.0.3/LICENSE` & `umk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `umk-0.0.3/pyproject.toml` & `umk-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "umk"
-version = "0.0.3"
+version = "0.1.0"
 description = "Unimake is a set of development tools and frameworks for project maintaining. This tools makes it easy to organize development routines (such as building, testing, linting, running, etc)"
 authors = ["Edward Sarkisyan <edw.sarkisyan@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -13,37 +13,37 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 packages = [
     { include = "umk" },
-    { include = "unimake" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 rich = "^13.6.0"
 gitpython = "^3.1.37"
 asyncclick = "^8.1"
 anyio = "^4.0.0"
-python-dotenv = "^1.0.0"
 beartype = "^0.16.3"
 fs = "^2.4.16"
 multimethod = "^1.10"
+paramiko = "^3.3.1"
+pydantic = "^2.5.3"
+python-on-whales = "^0.69.0"
+pyyaml = "^6.0.1"
+python-dotenv = "^1.0.1"
 
 [tool.black]
 line-length = 100
 
 
 [tool.poetry.scripts]
 umk = 'umk:entrypoint'
-unimake = 'unimake:entrypoint'
 
 [tool.poetry.group.dev.dependencies]
-pyinstaller = "^6.1.0"
-black = "^23.10.1"
 pytest = "^7.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `umk-0.0.3/umk/remote/interface.py` & `umk-0.1.0/umk/framework/remote/interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,115 @@
-from beartype import beartype
-from umk.globals import Global
-from umk.system.environs import OptEnv
-from umk.system import code
+from umk import core
+from umk.framework import utils
+from umk.framework.filesystem import AnyPath, OptPath
+from umk.framework.system.environs import OptEnv
+
+
+class Interface(core.Model):
+    name: str = core.Field(
+        default="",
+        description="Remote environment name",
+    )
+    description: str = core.Field(
+        default="",
+        description="Remote environment description",
+    )
+    default: bool = core.Field(
+        default=False,
+        description="Whether this remote environment are default or not",
+    )
+
+    def object(self) -> core.Object:
+        result = core.Object()
+        result.type = "Remote." + type(self).__name__.split(".")[-1]
+        for name in self.model_fields:
+            props = self.property(name)
+            for prop in props:
+                result.properties.add(prop)
+        return result
+
+    def property(self, name: str) -> list[core.Property]:
+        field = self.model_fields[name]
+        if not field.repr:
+            return []
+        return [
+            core.Property(
+                name=name,
+                description=field.description,
+                value=getattr(self, name)
+            )
+        ]
 
-
-class Interface:
-    forbidden_names = ("build", "destroy", "up", "down", "shell", "exec")
-    @property
-    def name(self) -> str:
+    def build(self, **kwargs):
         """
-        Remote environment name.
+        Build remote environment.
         """
-        return self._name
-
-    @name.setter
-    @beartype
-    def name(self, value: str):
-        if value in Interface.forbidden_names:
-            raise ValueError(f"Given remote environment name is forbidden: '{value}'")
-        self._name = value
+        self.__not_implemented()
 
-    @property
-    def description(self) -> str:
+    def destroy(self, **kwargs):
         """
-        Remote environment description.
+        Destroy remote environment.
         """
-        return self._description
-
-    @description.setter
-    @beartype
-    def description(self, value: str):
-        self._description = value
+        self.__not_implemented()
 
-    @property
-    def default(self) -> bool:
+    def up(self, **kwargs):
         """
-        Whether this remote environment are default or not.
+        Start remote environment.
         """
-        return self._default
+        self.__not_implemented()
 
-    @default.setter
-    @beartype
-    def default(self, value: bool):
-        self._default = value
+    def down(self, **kwargs):
+        """
+        Stop remote environment.
+        """
+        self.__not_implemented()
 
-    def build(self, *args, **kwargs):
+    def shell(self, **kwargs):
         """
-        Build remote environment.
+        Open remote environment shell.
         """
         self.__not_implemented()
 
-    def destroy(self, *args, **kwargs):
+    def login(self, **kwargs):
         """
-        Destroy remote environment.
+        Login remote environment.
         """
         self.__not_implemented()
 
-    def up(self, *args, **kwargs):
+    def logout(self, **kwargs):
         """
-        Start remote environment.
+        Logout remote environment.
         """
         self.__not_implemented()
 
-    def down(self, *args, **kwargs):
+    @core.typeguard
+    def execute(self, cmd: list[AnyPath], cwd: OptPath = None, env: OptEnv = None, **kwargs):
         """
-        Stop remote environment.
+        Execute command in remote environment.
         """
         self.__not_implemented()
 
-    def shell(self, *args, **kwargs):
+    @core.typeguard
+    def upload(self, items: dict[AnyPath, AnyPath], **kwargs):
         """
-        Open remote environment shell.
+        Upload given paths to remote environment.
         """
         self.__not_implemented()
 
-    def execute(self, cmd: list[str], cwd: str = '', env: OptEnv = None):
+    @core.typeguard
+    def download(self, items: dict[AnyPath, AnyPath], **kwargs):
         """
-        Execute command in remote environment.
+        Download given paths from remote environment.
         """
         self.__not_implemented()
 
     def __not_implemented(self):
-        Global.console.print(
-            f"[bold]The '{self.name}' remote environment has no '{code.caller(2)}' function. "
+        core.globals.console.print(
+            f"[bold]The '{self.name}' remote environment has no '{utils.caller(2)}' function. "
             f"It`s must be managed outside of this tool."
         )
 
-    @beartype
-    def __init__(self, name: str = "", description: str = "", default: bool = False):
-        self._name: str = name
-        self._default: bool = default
-        self._description = description
+    def __hash__(self) -> int:
+        return hash(self.name)
+
+    def __str__(self):
+        return f"umk.remote.Interface(name='{self.name}', description='{self.description}')"
```

