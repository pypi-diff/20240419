# Comparing `tmp/umk-0.1.0.tar.gz` & `tmp/umk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umk-0.1.0.tar", max compression
+gzip compressed data, was "umk-0.1.1.tar", max compression
```

## Comparing `umk-0.1.0.tar` & `umk-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    35148 2024-04-18 22:18:42.177750 umk-0.1.0/LICENSE
--rw-r--r--   0        0        0     5528 2024-04-18 22:18:42.177750 umk-0.1.0/README.md
--rw-r--r--   0        0        0     1210 2024-04-18 22:18:59.965815 umk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       34 2024-04-18 22:18:42.181750 umk-0.1.0/umk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/__init__.py
--rw-r--r--   0        0        0       86 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/config.py
--rw-r--r--   0        0        0     5005 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/remote.py
--rw-r--r--   0        0        0     4061 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/root.py
--rw-r--r--   0        0        0     1891 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/cmd/target.py
--rw-r--r--   0        0        0     1469 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/printers.py
--rw-r--r--   0        0        0     3592 2024-04-18 22:18:42.181750 umk-0.1.0/umk/application/utils.py
--rw-r--r--   0        0        0      574 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/__init__.py
--rw-r--r--   0        0        0     2892 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/errors.py
--rw-r--r--   0        0        0      860 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/globals.py
--rw-r--r--   0        0        0     2176 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/properties.py
--rw-r--r--   0        0        0     3543 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/serialization.py
--rw-r--r--   0        0        0     1425 2024-04-18 22:18:42.181750 umk-0.1.0/umk/core/typings.py
--rw-r--r--   0        0        0      271 2024-04-18 22:18:42.181750 umk-0.1.0/umk/entrypoint.py
--rw-r--r--   0        0        0        1 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/__init__.py
--rw-r--r--   0        0        0     4970 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/delve.py
--rw-r--r--   0        0        0     4261 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/docker/__init__.py
--rw-r--r--   0        0        0    37808 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/docker/compose.py
--rw-r--r--   0        0        0    15930 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/docker/file.py
--rw-r--r--   0        0        0      368 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/git.py
--rw-r--r--   0        0        0       61 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/go/__init__.py
--rw-r--r--   0        0        0    13890 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/adapters/go/base.py
--rw-r--r--   0        0        0       74 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/__init__.py
--rw-r--r--   0        0        0     3170 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/copy.py
--rw-r--r--   0        0        0     1757 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/factories.py
--rw-r--r--   0        0        0     2330 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/installer.py
--rw-r--r--   0        0        0     2617 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/filesystem/move.py
--rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/project/__init__.py
--rw-r--r--   0        0        0     4506 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/project/base.py
--rw-r--r--   0        0        0     1559 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/project/golang.py
--rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/__init__.py
--rw-r--r--   0        0        0     7487 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/docker.py
--rw-r--r--   0        0        0     3072 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/interface.py
--rw-r--r--   0        0        0     3137 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/remote/ssh.py
--rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/__init__.py
--rw-r--r--   0        0        0     1442 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/environs.py
--rw-r--r--   0        0        0      791 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/platform.py
--rw-r--r--   0        0        0     6656 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/shell.py
--rw-r--r--   0        0        0      763 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/system/user.py
--rw-r--r--   0        0        0        0 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/__init__.py
--rw-r--r--   0        0        0     3439 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/golang.py
--rw-r--r--   0        0        0     2149 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/interface.py
--rw-r--r--   0        0        0     6486 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/target/packages.py
--rw-r--r--   0        0        0       64 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/utils/__init__.py
--rw-r--r--   0        0        0     8514 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/utils/cli.py
--rw-r--r--   0        0        0      159 2024-04-18 22:18:42.181750 umk-0.1.0/umk/framework/utils/code.py
--rw-r--r--   0        0        0      159 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/__init__.py
--rw-r--r--   0        0        0      124 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/adapter/__init__.py
--rw-r--r--   0        0        0     4590 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/adapter/docker/__init__.py
--rw-r--r--   0        0        0      111 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/adapter/go/__init__.py
--rw-r--r--   0        0        0      423 2024-04-18 22:18:42.181750 umk-0.1.0/umk/kit/config/__init__.py
--rw-r--r--   0        0        0      272 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/filesystem/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/project/__init__.py
--rw-r--r--   0        0        0     1274 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/remote/__init__.py
--rw-r--r--   0        0        0      735 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/system/__init__.py
--rw-r--r--   0        0        0     1394 2024-04-18 22:18:42.185750 umk-0.1.0/umk/kit/target/__init__.py
--rw-r--r--   0        0        0      120 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/__init__.py
--rw-r--r--   0        0        0     7892 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/config.py
--rw-r--r--   0        0        0     3138 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/container.py
--rw-r--r--   0        0        0     2630 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/errors.py
--rw-r--r--   0        0        0     4873 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/project.py
--rw-r--r--   0        0        0     6631 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/remotes.py
--rw-r--r--   0        0        0     8982 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/targets.py
--rw-r--r--   0        0        0     8189 2024-04-18 22:18:42.185750 umk-0.1.0/umk/runtime/utils.py
--rw-r--r--   0        0        0     1592 2024-04-18 22:18:42.185750 umk-0.1.0/umk/state.py
--rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 umk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-18 23:11:54.315294 umk-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5528 2024-04-18 23:11:54.315294 umk-0.1.1/README.md
+-rw-r--r--   0        0        0     1210 2024-04-18 23:12:14.007275 umk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-04-18 23:11:54.319294 umk-0.1.1/umk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/config.py
+-rw-r--r--   0        0        0     5005 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/remote.py
+-rw-r--r--   0        0        0     4061 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/root.py
+-rw-r--r--   0        0        0     1891 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/target.py
+-rw-r--r--   0        0        0     1469 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/printers.py
+-rw-r--r--   0        0        0     3592 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/utils.py
+-rw-r--r--   0        0        0      574 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/errors.py
+-rw-r--r--   0        0        0      860 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/globals.py
+-rw-r--r--   0        0        0     2176 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/properties.py
+-rw-r--r--   0        0        0     3543 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/serialization.py
+-rw-r--r--   0        0        0     1425 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/typings.py
+-rw-r--r--   0        0        0      271 2024-04-18 23:11:54.319294 umk-0.1.1/umk/entrypoint.py
+-rw-r--r--   0        0        0        1 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/__init__.py
+-rw-r--r--   0        0        0     4970 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/delve.py
+-rw-r--r--   0        0        0     4261 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/docker/__init__.py
+-rw-r--r--   0        0        0    37808 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/docker/compose.py
+-rw-r--r--   0        0        0    15930 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/docker/file.py
+-rw-r--r--   0        0        0      368 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/git.py
+-rw-r--r--   0        0        0       61 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/go/__init__.py
+-rw-r--r--   0        0        0    13890 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/go/base.py
+-rw-r--r--   0        0        0       74 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     3170 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/copy.py
+-rw-r--r--   0        0        0     1757 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/factories.py
+-rw-r--r--   0        0        0     2330 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/installer.py
+-rw-r--r--   0        0        0     2617 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/move.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/project/__init__.py
+-rw-r--r--   0        0        0     4506 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/project/base.py
+-rw-r--r--   0        0        0     1559 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/project/golang.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/__init__.py
+-rw-r--r--   0        0        0     7487 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/docker.py
+-rw-r--r--   0        0        0     3072 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/interface.py
+-rw-r--r--   0        0        0     3137 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/ssh.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/__init__.py
+-rw-r--r--   0        0        0     1442 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/environs.py
+-rw-r--r--   0        0        0      791 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/platform.py
+-rw-r--r--   0        0        0     6656 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/shell.py
+-rw-r--r--   0        0        0      763 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/user.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/golang.py
+-rw-r--r--   0        0        0     2149 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/interface.py
+-rw-r--r--   0        0        0     6486 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/packages.py
+-rw-r--r--   0        0        0       64 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/utils/__init__.py
+-rw-r--r--   0        0        0     8514 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/utils/cli.py
+-rw-r--r--   0        0        0      159 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/utils/code.py
+-rw-r--r--   0        0        0      159 2024-04-18 23:11:54.319294 umk-0.1.1/umk/kit/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-18 23:11:54.319294 umk-0.1.1/umk/kit/adapter/__init__.py
+-rw-r--r--   0        0        0     4590 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/adapter/docker/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/adapter/go/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/config/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/filesystem/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/project/__init__.py
+-rw-r--r--   0        0        0     1274 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/remote/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/system/__init__.py
+-rw-r--r--   0        0        0     1394 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/target/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/__init__.py
+-rw-r--r--   0        0        0     7892 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/config.py
+-rw-r--r--   0        0        0     3246 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/container.py
+-rw-r--r--   0        0        0     2630 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/errors.py
+-rw-r--r--   0        0        0     4873 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/project.py
+-rw-r--r--   0        0        0     6631 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/remotes.py
+-rw-r--r--   0        0        0     8982 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/targets.py
+-rw-r--r--   0        0        0     8189 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/utils.py
+-rw-r--r--   0        0        0     1592 2024-04-18 23:11:54.323294 umk-0.1.1/umk/state.py
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 umk-0.1.1/PKG-INFO
```

### Comparing `umk-0.1.0/LICENSE` & `umk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/README.md` & `umk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/pyproject.toml` & `umk-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "umk"
-version = "0.1.0"
+version = "0.1.1"
 description = "Unimake is a set of development tools and frameworks for project maintaining. This tools makes it easy to organize development routines (such as building, testing, linting, running, etc)"
 authors = ["Edward Sarkisyan <edw.sarkisyan@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `umk-0.1.0/umk/application/cmd/config.py` & `umk-0.1.1/umk/application/cmd/config.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/application/cmd/remote.py` & `umk-0.1.1/umk/application/cmd/remote.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/application/cmd/root.py` & `umk-0.1.1/umk/application/cmd/root.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/application/cmd/target.py` & `umk-0.1.1/umk/application/cmd/target.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/application/printers.py` & `umk-0.1.1/umk/application/printers.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/application/utils.py` & `umk-0.1.1/umk/application/utils.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/core/__init__.py` & `umk-0.1.1/umk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/core/errors.py` & `umk-0.1.1/umk/core/errors.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/core/globals.py` & `umk-0.1.1/umk/core/globals.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/core/properties.py` & `umk-0.1.1/umk/core/properties.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/core/serialization.py` & `umk-0.1.1/umk/core/serialization.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/core/typings.py` & `umk-0.1.1/umk/core/typings.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/adapters/delve.py` & `umk-0.1.1/umk/framework/adapters/delve.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/adapters/docker/__init__.py` & `umk-0.1.1/umk/framework/adapters/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/adapters/docker/compose.py` & `umk-0.1.1/umk/framework/adapters/docker/compose.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/adapters/docker/file.py` & `umk-0.1.1/umk/framework/adapters/docker/file.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/adapters/go/base.py` & `umk-0.1.1/umk/framework/adapters/go/base.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/filesystem/copy.py` & `umk-0.1.1/umk/framework/filesystem/copy.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/filesystem/factories.py` & `umk-0.1.1/umk/framework/filesystem/factories.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/filesystem/installer.py` & `umk-0.1.1/umk/framework/filesystem/installer.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/filesystem/move.py` & `umk-0.1.1/umk/framework/filesystem/move.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/project/base.py` & `umk-0.1.1/umk/framework/project/base.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/project/golang.py` & `umk-0.1.1/umk/framework/project/golang.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/remote/docker.py` & `umk-0.1.1/umk/framework/remote/docker.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/remote/interface.py` & `umk-0.1.1/umk/framework/remote/interface.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/remote/ssh.py` & `umk-0.1.1/umk/framework/remote/ssh.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/system/environs.py` & `umk-0.1.1/umk/framework/system/environs.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/system/platform.py` & `umk-0.1.1/umk/framework/system/platform.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/system/shell.py` & `umk-0.1.1/umk/framework/system/shell.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/system/user.py` & `umk-0.1.1/umk/framework/system/user.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/target/golang.py` & `umk-0.1.1/umk/framework/target/golang.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/target/interface.py` & `umk-0.1.1/umk/framework/target/interface.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/target/packages.py` & `umk-0.1.1/umk/framework/target/packages.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/framework/utils/cli.py` & `umk-0.1.1/umk/framework/utils/cli.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/kit/adapter/docker/__init__.py` & `umk-0.1.1/umk/kit/adapter/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/kit/project/__init__.py` & `umk-0.1.1/umk/kit/project/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/kit/remote/__init__.py` & `umk-0.1.1/umk/kit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/kit/system/__init__.py` & `umk-0.1.1/umk/kit/system/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/kit/target/__init__.py` & `umk-0.1.1/umk/kit/target/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/runtime/config.py` & `umk-0.1.1/umk/runtime/config.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/runtime/container.py` & `umk-0.1.1/umk/runtime/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,30 +45,33 @@
         self.remotes = Remote()
 
     def load(self, options: Options):
         root = options.root.expanduser().resolve().absolute()
         sys.path.insert(0, root.as_posix())
 
         with_config = (root / "config.py").exists()
+        with_remote = (root / "remote.py").exists()
 
         self.config.init()
         self.project.init()
         self.targets.init()
         self.remotes.init()
 
         if with_config:
             self.script(root, "config")
         self.script(root, "project")
-        self.script(root, "remotes")
+        if with_remote:
+            self.script(root, "remotes")
 
         if with_config:
             self.config.setup(options.config)
         self.project.setup(self.config.instance)
         self.targets.setup(self.config.instance, self.project.instance)
-        self.remotes.setup(self.config.instance, self.project.instance)
+        if with_remote:
+            self.remotes.setup(self.config.instance, self.project.instance)
 
     def find_remote(self, default: bool, specific: str) -> remote.Interface:
         if default:
             result = self.remotes.get(self.remotes.default)
             if not result:
                 core.globals.error_console.print(
                     'Failed to find default remote environment! '
```

### Comparing `umk-0.1.0/umk/runtime/errors.py` & `umk-0.1.1/umk/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/runtime/project.py` & `umk-0.1.1/umk/runtime/project.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/runtime/remotes.py` & `umk-0.1.1/umk/runtime/remotes.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/runtime/targets.py` & `umk-0.1.1/umk/runtime/targets.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/runtime/utils.py` & `umk-0.1.1/umk/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/umk/state.py` & `umk-0.1.1/umk/state.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.0/PKG-INFO` & `umk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Unimake is a set of development tools and frameworks for project maintaining. This tools makes it easy to organize development routines (such as building, testing, linting, running, etc)
 License: GPL-3.0-only
 Author: Edward Sarkisyan
 Author-email: edw.sarkisyan@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

