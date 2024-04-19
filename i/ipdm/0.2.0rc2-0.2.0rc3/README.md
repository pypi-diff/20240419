# Comparing `tmp/ipdm-0.2.0rc2.tar.gz` & `tmp/ipdm-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipdm-0.2.0rc2.tar", last modified: Tue Apr  2 12:17:25 2024, max compression
+gzip compressed data, was "ipdm-0.2.0rc3.tar", last modified: Fri Apr 19 08:15:22 2024, max compression
```

## Comparing `ipdm-0.2.0rc2.tar` & `ipdm-0.2.0rc3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       27 2024-04-02 12:17:07.841571 ipdm-0.2.0rc2/README.md
--rw-r--r--   0        0        0      689 2024-04-02 12:17:25.841590 ipdm-0.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0      246 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/__init__.py
--rw-r--r--   0        0        0     5958 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/__main__.py
--rw-r--r--   0        0        0    23305 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/api.py
--rw-r--r--   0        0        0    18438 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/const.py
--rw-r--r--   0        0        0     1214 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/exceptions.py
--rw-r--r--   0        0        0     1595 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/logging.py
--rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/__init__.py
--rw-r--r--   0        0        0     4753 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/index.py
--rw-r--r--   0        0        0     6688 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/ipk.py
--rw-r--r--   0        0        0     5591 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/lock.py
--rw-r--r--   0        0        0     3516 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/requirement.py
--rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/project/__init__.py
--rw-r--r--   0        0        0      473 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/project/env.py
--rw-r--r--   0        0        0     6509 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/project/toml_file.py
--rw-r--r--   0        0        0      404 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/typing.py
--rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/__init__.py
--rw-r--r--   0        0        0     1230 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/_freeze.py
--rw-r--r--   0        0        0     2495 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/freeze.py
--rw-r--r--   0        0        0      768 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/git.py
--rw-r--r--   0        0        0      486 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/hash.py
--rw-r--r--   0        0        0     1615 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/loader.py
--rw-r--r--   0        0        0      997 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/resolve.py
--rw-r--r--   0        0        0      160 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/urlparser.py
--rw-r--r--   0        0        0       70 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/uuid.py
--rw-r--r--   0        0        0     1648 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/version.py
--rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/tests/__init__.py
--rw-r--r--   0        0        0      491 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/tests/test_api.py
--rw-r--r--   0        0        0     2601 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/tests/test_cli.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 ipdm-0.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/README.md
+-rw-r--r--   0        0        0      689 2024-04-19 08:15:22.201526 ipdm-0.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      246 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/__init__.py
+-rw-r--r--   0        0        0     5943 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/__main__.py
+-rw-r--r--   0        0        0    23305 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/api.py
+-rw-r--r--   0        0        0    18438 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/const.py
+-rw-r--r--   0        0        0     1214 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/exceptions.py
+-rw-r--r--   0        0        0     1595 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/logging.py
+-rw-r--r--   0        0        0        0 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/models/__init__.py
+-rw-r--r--   0        0        0     4753 2024-04-19 08:15:05.445366 ipdm-0.2.0rc3/src/ipm/models/index.py
+-rw-r--r--   0        0        0     6688 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/models/ipk.py
+-rw-r--r--   0        0        0     5591 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/models/lock.py
+-rw-r--r--   0        0        0     3516 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/models/requirement.py
+-rw-r--r--   0        0        0        0 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/project/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/project/env.py
+-rw-r--r--   0        0        0     6509 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/project/toml_file.py
+-rw-r--r--   0        0        0      404 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/typing.py
+-rw-r--r--   0        0        0        0 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/__init__.py
+-rw-r--r--   0        0        0     1230 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/_freeze.py
+-rw-r--r--   0        0        0     2495 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/freeze.py
+-rw-r--r--   0        0        0      768 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/git.py
+-rw-r--r--   0        0        0      486 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/hash.py
+-rw-r--r--   0        0        0     1615 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/loader.py
+-rw-r--r--   0        0        0      997 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/resolve.py
+-rw-r--r--   0        0        0      160 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/urlparser.py
+-rw-r--r--   0        0        0       70 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/uuid.py
+-rw-r--r--   0        0        0     1648 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/src/ipm/utils/version.py
+-rw-r--r--   0        0        0        0 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/tests/test_api.py
+-rw-r--r--   0        0        0     2601 2024-04-19 08:15:05.449365 ipdm-0.2.0rc3/tests/test_cli.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 ipdm-0.2.0rc3/PKG-INFO
```

### Comparing `ipdm-0.2.0rc2/pyproject.toml` & `ipdm-0.2.0rc3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ipdm"
-version = "0.2.0-rc.2"
+version = "0.2.0-rc.3"
 description = "Infini 包管理器"
 authors = [
     { name = "苏向夜", email = "fu050409@163.com" },
     { name = "简律纯", email = "leader@hydroroll.team" },
 ]
 dependencies = [
     "typer>=0.9.0",
```

### Comparing `ipdm-0.2.0rc2/src/ipm/__main__.py` & `ipdm-0.2.0rc3/src/ipm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pathlib import Path
 from ipm import api
 from ipm.exceptions import IPMException
 from ipm.logging import status, error, tada
 
 import typer
 
-status.start()
 main = typer.Typer(
     name="ipm", help="Infini 包管理器", no_args_is_help=True, add_completion=False
 )
 
 
 @main.command()
 def lock():
```

### Comparing `ipdm-0.2.0rc2/src/ipm/api.py` & `ipdm-0.2.0rc3/src/ipm/api.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/const.py` & `ipdm-0.2.0rc3/src/ipm/const.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/exceptions.py` & `ipdm-0.2.0rc3/src/ipm/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/logging.py` & `ipdm-0.2.0rc3/src/ipm/logging.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/models/index.py` & `ipdm-0.2.0rc3/src/ipm/models/index.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/models/ipk.py` & `ipdm-0.2.0rc3/src/ipm/models/ipk.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/models/lock.py` & `ipdm-0.2.0rc3/src/ipm/models/lock.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/models/requirement.py` & `ipdm-0.2.0rc3/src/ipm/models/requirement.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/project/toml_file.py` & `ipdm-0.2.0rc3/src/ipm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/utils/_freeze.py` & `ipdm-0.2.0rc3/src/ipm/utils/_freeze.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/utils/freeze.py` & `ipdm-0.2.0rc3/src/ipm/utils/freeze.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/utils/git.py` & `ipdm-0.2.0rc3/src/ipm/utils/git.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/utils/loader.py` & `ipdm-0.2.0rc3/src/ipm/utils/loader.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/utils/resolve.py` & `ipdm-0.2.0rc3/src/ipm/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/src/ipm/utils/version.py` & `ipdm-0.2.0rc3/src/ipm/utils/version.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc2/tests/test_cli.py` & `ipdm-0.2.0rc3/tests/test_cli.py`

 * *Files identical despite different names*

