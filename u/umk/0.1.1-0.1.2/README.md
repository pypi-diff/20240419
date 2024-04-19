# Comparing `tmp/umk-0.1.1.tar.gz` & `tmp/umk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umk-0.1.1.tar", max compression
+gzip compressed data, was "umk-0.1.2.tar", max compression
```

## Comparing `umk-0.1.1.tar` & `umk-0.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    35148 2024-04-18 23:11:54.315294 umk-0.1.1/LICENSE
--rw-r--r--   0        0        0     5528 2024-04-18 23:11:54.315294 umk-0.1.1/README.md
--rw-r--r--   0        0        0     1210 2024-04-18 23:12:14.007275 umk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       34 2024-04-18 23:11:54.319294 umk-0.1.1/umk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/__init__.py
--rw-r--r--   0        0        0       86 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/config.py
--rw-r--r--   0        0        0     5005 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/remote.py
--rw-r--r--   0        0        0     4061 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/root.py
--rw-r--r--   0        0        0     1891 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/cmd/target.py
--rw-r--r--   0        0        0     1469 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/printers.py
--rw-r--r--   0        0        0     3592 2024-04-18 23:11:54.319294 umk-0.1.1/umk/application/utils.py
--rw-r--r--   0        0        0      574 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/__init__.py
--rw-r--r--   0        0        0     2892 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/errors.py
--rw-r--r--   0        0        0      860 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/globals.py
--rw-r--r--   0        0        0     2176 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/properties.py
--rw-r--r--   0        0        0     3543 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/serialization.py
--rw-r--r--   0        0        0     1425 2024-04-18 23:11:54.319294 umk-0.1.1/umk/core/typings.py
--rw-r--r--   0        0        0      271 2024-04-18 23:11:54.319294 umk-0.1.1/umk/entrypoint.py
--rw-r--r--   0        0        0        1 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/__init__.py
--rw-r--r--   0        0        0     4970 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/delve.py
--rw-r--r--   0        0        0     4261 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/docker/__init__.py
--rw-r--r--   0        0        0    37808 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/docker/compose.py
--rw-r--r--   0        0        0    15930 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/docker/file.py
--rw-r--r--   0        0        0      368 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/git.py
--rw-r--r--   0        0        0       61 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/go/__init__.py
--rw-r--r--   0        0        0    13890 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/adapters/go/base.py
--rw-r--r--   0        0        0       74 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/__init__.py
--rw-r--r--   0        0        0     3170 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/copy.py
--rw-r--r--   0        0        0     1757 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/factories.py
--rw-r--r--   0        0        0     2330 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/installer.py
--rw-r--r--   0        0        0     2617 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/filesystem/move.py
--rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/project/__init__.py
--rw-r--r--   0        0        0     4506 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/project/base.py
--rw-r--r--   0        0        0     1559 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/project/golang.py
--rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/__init__.py
--rw-r--r--   0        0        0     7487 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/docker.py
--rw-r--r--   0        0        0     3072 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/interface.py
--rw-r--r--   0        0        0     3137 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/remote/ssh.py
--rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/__init__.py
--rw-r--r--   0        0        0     1442 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/environs.py
--rw-r--r--   0        0        0      791 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/platform.py
--rw-r--r--   0        0        0     6656 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/shell.py
--rw-r--r--   0        0        0      763 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/system/user.py
--rw-r--r--   0        0        0        0 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/__init__.py
--rw-r--r--   0        0        0     3439 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/golang.py
--rw-r--r--   0        0        0     2149 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/interface.py
--rw-r--r--   0        0        0     6486 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/target/packages.py
--rw-r--r--   0        0        0       64 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/utils/__init__.py
--rw-r--r--   0        0        0     8514 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/utils/cli.py
--rw-r--r--   0        0        0      159 2024-04-18 23:11:54.319294 umk-0.1.1/umk/framework/utils/code.py
--rw-r--r--   0        0        0      159 2024-04-18 23:11:54.319294 umk-0.1.1/umk/kit/__init__.py
--rw-r--r--   0        0        0      124 2024-04-18 23:11:54.319294 umk-0.1.1/umk/kit/adapter/__init__.py
--rw-r--r--   0        0        0     4590 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/adapter/docker/__init__.py
--rw-r--r--   0        0        0      111 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/adapter/go/__init__.py
--rw-r--r--   0        0        0      423 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/config/__init__.py
--rw-r--r--   0        0        0      272 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/filesystem/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/project/__init__.py
--rw-r--r--   0        0        0     1274 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/remote/__init__.py
--rw-r--r--   0        0        0      735 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/system/__init__.py
--rw-r--r--   0        0        0     1394 2024-04-18 23:11:54.323294 umk-0.1.1/umk/kit/target/__init__.py
--rw-r--r--   0        0        0      120 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/__init__.py
--rw-r--r--   0        0        0     7892 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/config.py
--rw-r--r--   0        0        0     3246 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/container.py
--rw-r--r--   0        0        0     2630 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/errors.py
--rw-r--r--   0        0        0     4873 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/project.py
--rw-r--r--   0        0        0     6631 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/remotes.py
--rw-r--r--   0        0        0     8982 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/targets.py
--rw-r--r--   0        0        0     8189 2024-04-18 23:11:54.323294 umk-0.1.1/umk/runtime/utils.py
--rw-r--r--   0        0        0     1592 2024-04-18 23:11:54.323294 umk-0.1.1/umk/state.py
--rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 umk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-19 11:59:39.783606 umk-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5528 2024-04-19 11:59:39.783606 umk-0.1.2/README.md
+-rw-r--r--   0        0        0     1210 2024-04-19 11:59:58.091637 umk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-04-19 11:59:39.787606 umk-0.1.2/umk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/cmd/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/cmd/config.py
+-rw-r--r--   0        0        0     5005 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/cmd/remote.py
+-rw-r--r--   0        0        0     4061 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/cmd/root.py
+-rw-r--r--   0        0        0     1891 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/cmd/target.py
+-rw-r--r--   0        0        0     1469 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/printers.py
+-rw-r--r--   0        0        0     3712 2024-04-19 11:59:39.787606 umk-0.1.2/umk/application/utils.py
+-rw-r--r--   0        0        0      574 2024-04-19 11:59:39.787606 umk-0.1.2/umk/core/__init__.py
+-rw-r--r--   0        0        0     2917 2024-04-19 11:59:39.787606 umk-0.1.2/umk/core/errors.py
+-rw-r--r--   0        0        0      860 2024-04-19 11:59:39.787606 umk-0.1.2/umk/core/globals.py
+-rw-r--r--   0        0        0     2234 2024-04-19 11:59:39.787606 umk-0.1.2/umk/core/properties.py
+-rw-r--r--   0        0        0     3543 2024-04-19 11:59:39.787606 umk-0.1.2/umk/core/serialization.py
+-rw-r--r--   0        0        0     1425 2024-04-19 11:59:39.787606 umk-0.1.2/umk/core/typings.py
+-rw-r--r--   0        0        0      271 2024-04-19 11:59:39.787606 umk-0.1.2/umk/entrypoint.py
+-rw-r--r--   0        0        0        1 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/__init__.py
+-rw-r--r--   0        0        0     4970 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/delve.py
+-rw-r--r--   0        0        0     4261 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/docker/__init__.py
+-rw-r--r--   0        0        0    37808 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/docker/compose.py
+-rw-r--r--   0        0        0    15930 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/docker/file.py
+-rw-r--r--   0        0        0      368 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/git.py
+-rw-r--r--   0        0        0       61 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/go/__init__.py
+-rw-r--r--   0        0        0    13890 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/adapters/go/base.py
+-rw-r--r--   0        0        0       74 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     3170 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/filesystem/copy.py
+-rw-r--r--   0        0        0     1757 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/filesystem/factories.py
+-rw-r--r--   0        0        0     2330 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/filesystem/installer.py
+-rw-r--r--   0        0        0     2617 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/filesystem/move.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/project/__init__.py
+-rw-r--r--   0        0        0     4506 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/project/base.py
+-rw-r--r--   0        0        0     1559 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/project/golang.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/remote/__init__.py
+-rw-r--r--   0        0        0     7487 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/remote/docker.py
+-rw-r--r--   0        0        0     3072 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/remote/interface.py
+-rw-r--r--   0        0        0     3137 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/remote/ssh.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/system/__init__.py
+-rw-r--r--   0        0        0     1442 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/system/environs.py
+-rw-r--r--   0        0        0      791 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/system/platform.py
+-rw-r--r--   0        0        0     6656 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/system/shell.py
+-rw-r--r--   0        0        0      763 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/system/user.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/target/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/target/golang.py
+-rw-r--r--   0        0        0     2149 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/target/interface.py
+-rw-r--r--   0        0        0     6486 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/target/packages.py
+-rw-r--r--   0        0        0       64 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/utils/__init__.py
+-rw-r--r--   0        0        0     8514 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/utils/cli.py
+-rw-r--r--   0        0        0      159 2024-04-19 11:59:39.787606 umk-0.1.2/umk/framework/utils/code.py
+-rw-r--r--   0        0        0      159 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/adapter/__init__.py
+-rw-r--r--   0        0        0     4590 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/adapter/docker/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/adapter/go/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/config/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/filesystem/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/project/__init__.py
+-rw-r--r--   0        0        0     1274 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/remote/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/system/__init__.py
+-rw-r--r--   0        0        0     1394 2024-04-19 11:59:39.787606 umk-0.1.2/umk/kit/target/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-19 11:59:39.787606 umk-0.1.2/umk/runtime/__init__.py
+-rw-r--r--   0        0        0     9126 2024-04-19 11:59:39.787606 umk-0.1.2/umk/runtime/config.py
+-rw-r--r--   0        0        0     3246 2024-04-19 11:59:39.787606 umk-0.1.2/umk/runtime/container.py
+-rw-r--r--   0        0        0     2630 2024-04-19 11:59:39.791606 umk-0.1.2/umk/runtime/errors.py
+-rw-r--r--   0        0        0     4873 2024-04-19 11:59:39.791606 umk-0.1.2/umk/runtime/project.py
+-rw-r--r--   0        0        0     6631 2024-04-19 11:59:39.791606 umk-0.1.2/umk/runtime/remotes.py
+-rw-r--r--   0        0        0     8982 2024-04-19 11:59:39.791606 umk-0.1.2/umk/runtime/targets.py
+-rw-r--r--   0        0        0     8189 2024-04-19 11:59:39.791606 umk-0.1.2/umk/runtime/utils.py
+-rw-r--r--   0        0        0     1592 2024-04-19 11:59:39.791606 umk-0.1.2/umk/state.py
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 umk-0.1.2/PKG-INFO
```

### Comparing `umk-0.1.1/LICENSE` & `umk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/README.md` & `umk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/pyproject.toml` & `umk-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "umk"
-version = "0.1.1"
+version = "0.1.2"
 description = "Unimake is a set of development tools and frameworks for project maintaining. This tools makes it easy to organize development routines (such as building, testing, linting, running, etc)"
 authors = ["Edward Sarkisyan <edw.sarkisyan@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `umk-0.1.1/umk/application/cmd/config.py` & `umk-0.1.2/umk/application/cmd/config.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/application/cmd/remote.py` & `umk-0.1.2/umk/application/cmd/remote.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/application/cmd/root.py` & `umk-0.1.2/umk/application/cmd/root.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/application/cmd/target.py` & `umk-0.1.2/umk/application/cmd/target.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/application/printers.py` & `umk-0.1.2/umk/application/printers.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/application/utils.py` & `umk-0.1.2/umk/application/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,29 +74,30 @@
             re = container.find_remote(False, state.remote.specific)
         else:
             return
         umk.core.globals.console.print(f"[bold]Forward execution to '{re.name}' remote environment: '{' '.join(state.remote.cmd)}'")
         re.execute(state.remote.cmd)
         sys.exit(0)
 
-    def config(file: bool, presets: tuple[str] | None, overrides: None | tuple[str] = None) -> runtime.Options.Config:
+    def config(file: bool, presets: tuple[str] | None = None, overrides: None | tuple[str] = None) -> runtime.Options.Config:
         result = runtime.Options.Config()
-        result.presets = list(presets)
+        result.presets = list(presets) if presets else []
         result.file = file
         if not overrides:
             return result
-        for entry in overrides:
-            name = ""
-            i = 0
-            for i, sym in enumerate(entry):
-                if sym != "=":
-                    name += sym
-                # TODO Validate entry symbols
-                else:
-                    break
-                if i > len(entry):
-                    # TODO Invalid syntax
-                    print(f"Invalid config entry: {entry}", file=sys.stderr)
-                    core.globals.close(-1)
-            value = entry[i+1:]
-            result.overrides[name] = value
+        if overrides is not None:
+            for entry in overrides:
+                name = ""
+                i = 0
+                for i, sym in enumerate(entry):
+                    if sym != "=":
+                        name += sym
+                    # TODO Validate entry symbols
+                    else:
+                        break
+                    if i > len(entry):
+                        # TODO Invalid syntax
+                        print(f"Invalid config entry: {entry}", file=sys.stderr)
+                        core.globals.close(-1)
+                value = entry[i+1:]
+                result.overrides[name] = value
         return result
```

### Comparing `umk-0.1.1/umk/core/__init__.py` & `umk-0.1.2/umk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/core/errors.py` & `umk-0.1.2/umk/core/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,27 @@
 
     def __str__(self):
         return " ".join(self.messages)
 
     @typeguard
     def print(self, printer: Callable[[...], Any]):
         self.print_messages(printer)
-        self.print_details(printer)
+        if self.details:
+            self.print_details(printer)
 
     @typeguard
     def print_messages(self, printer: Callable[[...], Any]):
         for message in self.messages:
             if message:
                 printer(f"[red bold]{message}")
 
     @typeguard
     def print_details(self, printer: Callable[[...], Any]):
-        cs = "[bold red]"
-        rs = "[bold red]"
+        cs = "bold red"
+        rs = "bold red"
         table = Table(show_header=True, show_edge=True, show_lines=False)
         table.add_column("Name", justify="left", style=cs, no_wrap=True)
         table.add_column("Default", justify="center", style=cs, no_wrap=True)
         table.add_column("Description", justify="left", style=cs, no_wrap=True)
         for detail in self.details:
             table.add_row(detail.name, detail.value, detail.description, style=rs)
         printer(table)
```

### Comparing `umk-0.1.1/umk/core/globals.py` & `umk-0.1.2/umk/core/globals.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/core/properties.py` & `umk-0.1.2/umk/core/properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     def __getitem__(self, name: str) -> Property:
         return self._items[name]
 
     @typeguard
     def __setitem__(self, name: str, value: Property):
         self._items[name] = value
 
+    def __bool__(self):
+        return bool(self._items)
+
     @typeguard
     def get(self, name: str, value: Any = None) -> Property:
         return self._items.get(name, value)
 
     @typeguard
     def add(self, prop: Property):
         self._items[prop.name] = prop
```

### Comparing `umk-0.1.1/umk/core/serialization.py` & `umk-0.1.2/umk/core/serialization.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/core/typings.py` & `umk-0.1.2/umk/core/typings.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/adapters/delve.py` & `umk-0.1.2/umk/framework/adapters/delve.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/adapters/docker/__init__.py` & `umk-0.1.2/umk/framework/adapters/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/adapters/docker/compose.py` & `umk-0.1.2/umk/framework/adapters/docker/compose.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/adapters/docker/file.py` & `umk-0.1.2/umk/framework/adapters/docker/file.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/adapters/go/base.py` & `umk-0.1.2/umk/framework/adapters/go/base.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/filesystem/copy.py` & `umk-0.1.2/umk/framework/filesystem/copy.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/filesystem/factories.py` & `umk-0.1.2/umk/framework/filesystem/factories.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/filesystem/installer.py` & `umk-0.1.2/umk/framework/filesystem/installer.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/filesystem/move.py` & `umk-0.1.2/umk/framework/filesystem/move.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/project/base.py` & `umk-0.1.2/umk/framework/project/base.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/project/golang.py` & `umk-0.1.2/umk/framework/project/golang.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/remote/docker.py` & `umk-0.1.2/umk/framework/remote/docker.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/remote/interface.py` & `umk-0.1.2/umk/framework/remote/interface.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/remote/ssh.py` & `umk-0.1.2/umk/framework/remote/ssh.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/system/environs.py` & `umk-0.1.2/umk/framework/system/environs.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/system/platform.py` & `umk-0.1.2/umk/framework/system/platform.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/system/shell.py` & `umk-0.1.2/umk/framework/system/shell.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/system/user.py` & `umk-0.1.2/umk/framework/system/user.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/target/golang.py` & `umk-0.1.2/umk/framework/target/golang.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/target/interface.py` & `umk-0.1.2/umk/framework/target/interface.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/target/packages.py` & `umk-0.1.2/umk/framework/target/packages.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/framework/utils/cli.py` & `umk-0.1.2/umk/framework/utils/cli.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/kit/adapter/docker/__init__.py` & `umk-0.1.2/umk/kit/adapter/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/kit/project/__init__.py` & `umk-0.1.2/umk/kit/project/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/kit/remote/__init__.py` & `umk-0.1.2/umk/kit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/kit/system/__init__.py` & `umk-0.1.2/umk/kit/system/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/kit/target/__init__.py` & `umk-0.1.2/umk/kit/target/__init__.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/runtime/config.py` & `umk-0.1.2/umk/runtime/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
+import sys
 
 from pydantic import ValidationError
 
 from umk import core
 from umk.kit import config
-from umk.core.typings import Callable, Any
+from umk.core.typings import Callable, Any, Type
 from umk.framework.filesystem import Path
 from umk.runtime import utils
 
 
 class Config(core.Model):
     class Update(core.Model):
         overrides: dict[str, config.Value] = core.Field(
@@ -70,27 +71,49 @@
         description="Config presets"
     )
     entries: dict[str, str] = core.Field(
         default_factory=dict,
         description="Config entries"
     )
 
-    def set(self, entry: str, value: config.Value):
+    def set(self, entry: str, value: str):
         if entry not in self.entries:
             core.globals.console.print(f"[yellow bold]Config: '{entry}' entry not found")
             return
-        tokens = entry.replace("-", "_").split(".")
-        if len(tokens) == 1:
-            setattr(self.instance, tokens[0], value)
-        else:
+
+        def find() -> tuple[Any, str, Type]:
+            tokens = entry.replace("-", "_").split(".")
             attr = tokens[-1]
             curr = self.instance
             for token in tokens[:-1]:
                 curr = getattr(curr, token)
-            setattr(curr, attr, value)
+            return curr, attr, type(getattr(curr, attr))
+
+        def assign(to: Any, which: str, what: str, t: Type):
+            if t == str:
+                setattr(to, which, what)
+            elif t == int:
+                setattr(to, which, int(what))
+            elif t == bool:
+                if what == "yes":
+                    setattr(to, which, True)
+                elif what == "no":
+                    setattr(to, which, False)
+                else:
+                    raise core.Error(
+                        "BadBool",
+                        f"Failed to set config entry '{entry}' value",
+                        "Valid boolean: 'yes', 'no'",
+                        f"Given: {value}"
+                    )
+            elif t == float:
+                setattr(to, which, float(what))
+
+        obj, name, typ = find()
+        assign(obj, name, value, typ)
 
     def get(self, entry: str, on_err: Any = None) -> config.Value | None:
         if entry not in self.entries:
             return on_err
         result = self.instance
         tokens = entry.replace("-", "_").split(".")
         for token in tokens:
@@ -171,14 +194,24 @@
                 v = getattr(root, n)
                 t = type(v)
                 if t in (str, int, bool, float):
                     token = f"{parent}.{n}".lstrip(".").replace("_", "-")
                     tokens[token] = f.description or ""
                 elif issubclass(t, core.Model):
                     recursive(v, f"{parent}.{n}", tokens)
+                else:
+                    e = n
+                    if parent:
+                        e = parent + "." + n
+                    raise core.Error(
+                        "UnsupportedConfigType",
+                        f"Failed to register config !",
+                        f"The entry '{e}' is an unsupported type: {t}",
+                        f"Only 'str | bool | int | float' are allowed."
+                    )
 
         if self.decorator.instance.registered:
             self.instance = self.decorator.instance.defers[0].func()
             self.entries = {}
             recursive(self.instance, "", self.entries)
 
         if self.decorator.preset.registered:
```

### Comparing `umk-0.1.1/umk/runtime/container.py` & `umk-0.1.2/umk/runtime/container.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/runtime/errors.py` & `umk-0.1.2/umk/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/runtime/project.py` & `umk-0.1.2/umk/runtime/project.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/runtime/remotes.py` & `umk-0.1.2/umk/runtime/remotes.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/runtime/targets.py` & `umk-0.1.2/umk/runtime/targets.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/runtime/utils.py` & `umk-0.1.2/umk/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/umk/state.py` & `umk-0.1.2/umk/state.py`

 * *Files identical despite different names*

### Comparing `umk-0.1.1/PKG-INFO` & `umk-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unimake is a set of development tools and frameworks for project maintaining. This tools makes it easy to organize development routines (such as building, testing, linting, running, etc)
 License: GPL-3.0-only
 Author: Edward Sarkisyan
 Author-email: edw.sarkisyan@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```
