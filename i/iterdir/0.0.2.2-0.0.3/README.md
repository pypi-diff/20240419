# Comparing `tmp/iterdir-0.0.2.2.tar.gz` & `tmp/iterdir-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterdir-0.0.2.2.tar", max compression
+gzip compressed data, was "iterdir-0.0.3.tar", max compression
```

## Comparing `iterdir-0.0.2.2.tar` & `iterdir-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.2.2/LICENSE
--rw-r--r--   0        0        0     8056 2024-04-16 11:00:53.760552 iterdir-0.0.2.2/iterdir/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.2.2/iterdir/py.typed
--rw-r--r--   0        0        0     1070 2024-04-16 14:58:34.770212 iterdir-0.0.2.2/pyproject.toml
--rw-r--r--   0        0        0      152 2024-04-16 08:39:39.205664 iterdir-0.0.2.2/readme.md
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 iterdir-0.0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.3/LICENSE
+-rw-r--r--   0        0        0     8211 2024-04-19 04:16:32.475900 iterdir-0.0.3/iterdir/__init__.py
+-rw-r--r--   0        0        0     6552 2024-04-19 04:16:07.416183 iterdir-0.0.3/iterdir/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.3/iterdir/py.typed
+-rw-r--r--   0        0        0     1068 2024-04-19 04:16:21.564032 iterdir-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-16 08:39:39.205664 iterdir-0.0.3/readme.md
+-rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 iterdir-0.0.3/PKG-INFO
```

### Comparing `iterdir-0.0.2.2/LICENSE` & `iterdir-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.2.2/iterdir/__init__.py` & `iterdir-0.0.3/iterdir/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 2)
+__version__ = (0, 0, 3)
 __all__ = ["DirEntry", "iterdir"]
 
 from collections import deque
 from collections.abc import Callable, Iterable, Iterator
-from os import fspath, listdir, scandir, stat, DirEntry as _DirEntry, PathLike
+from os import (
+    fspath, listdir, lstat, scandir, stat, stat_result, 
+    DirEntry as _DirEntry, PathLike, 
+)
 from os.path import (
     abspath, commonpath, basename, isfile, isdir, islink, join as joinpath, realpath, 
 )
 from pathlib import Path
 from typing import overload, Generic, Never, Optional, TypeVar
 
 
@@ -29,54 +32,55 @@
     def __subclasscheck__(cls, sub, /):
         if issubclass(sub, _DirEntry):
             return True
         return super().__subclasscheck__(sub)
 
 
 class DirEntry(Generic[AnyStr], metaclass=DirEntryMeta):
-    __slots__ = "path",
+    __slots__ = ("name", "path")
 
+    name: AnyStr
     path: AnyStr
 
     def __init__(self, /, path: AnyStr | PathLike[AnyStr]):
-        path = fspath(path)
-        if not path:
-            path = abspath(path)
+        path = abspath(fspath(path))
+        super().__setattr__("name", basename(path))
         super().__setattr__("path", path)
 
     def __fspath__(self, /) -> AnyStr:
         return self.path
 
     def __repr__(self, /) -> str:
         return f"<{type(self).__qualname__} {self.path!r}>"
 
     def __setattr__(self, key, val, /) -> Never:
         raise AttributeError("can't set attributes")
 
-    @property
-    def name(self, /) -> AnyStr:
-        return basename(self.path)
-
     def inode(self, /) -> int:
-        return stat(self.path).st_ino
+        return lstat(self.path).st_ino
 
     def is_dir(self, /, *, follow_symlinks: bool = True) -> bool:
         if follow_symlinks:
             return isdir(self.path)
         else:
             return not islink(self.path) and isdir(self.path)
 
     def is_file(self, /, *, follow_symlinks: bool = True) -> bool:
         if follow_symlinks:
             return isfile(self.path)
         else:
             return islink(self.path) or isfile(self.path) 
 
     is_symlink = islink
-    stat = stat
+
+    def stat(self, /, *, follow_symlinks: bool = True) -> stat_result:
+        if follow_symlinks:
+            return stat(self.path)
+        else:
+            return lstat(self.path)
 
 
 def _iterdir_bfs(
     top: PathType, 
     /, 
     is_dir: Callable[[PathType], bool], 
     iter_dir: Callable[[PathType], Iterable[PathType]],
```

### Comparing `iterdir-0.0.2.2/pyproject.toml` & `iterdir-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterdir"
-version = "0.0.2.2"
+version = "0.0.3"
 description = "iterdir."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 keywords = ["iterdir", "traverse"]
```

### Comparing `iterdir-0.0.2.2/PKG-INFO` & `iterdir-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterdir
-Version: 0.0.2.2
+Version: 0.0.3
 Summary: iterdir.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 License: MIT
 Keywords: iterdir,traverse
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

