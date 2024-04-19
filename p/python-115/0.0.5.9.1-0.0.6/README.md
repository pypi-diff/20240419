# Comparing `tmp/python_115-0.0.5.9.1.tar.gz` & `tmp/python_115-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.9.1.tar", max compression
+gzip compressed data, was "python_115-0.0.6.tar", max compression
```

## Comparing `python_115-0.0.5.9.1.tar` & `python_115-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,29 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.9.1/LICENSE
--rw-r--r--   0        0        0   263879 2024-04-06 11:52:54.748855 python_115-0.0.5.9.1/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.9.1/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.9.1/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.9.1/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.9.1/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.9.1/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.9.1/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.9.1/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.9.1/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.9.1/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.9.1/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.9.1/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.9.1/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.9.1/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.9.1/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.9.1/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.9.1/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.9.1/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.9.1/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.9.1/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.9.1/p115/util/urlopen.py
--rw-r--r--   0        0        0     1274 2024-04-06 11:53:11.617183 python_115-0.0.5.9.1/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.9.1/readme.md
--rw-r--r--   0        0        0    35898 1970-01-01 00:00:00.000000 python_115-0.0.5.9.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6/LICENSE
+-rwxr-xr-x   0        0        0   269608 2024-04-19 14:51:04.366035 python_115-0.0.6/p115/__init__.py
+-rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6742 2024-04-19 15:25:32.941526 python_115-0.0.6/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1405 2024-04-19 15:22:56.504224 python_115-0.0.6/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.6/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.6/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.6/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.6/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1270 2024-04-19 15:26:14.699487 python_115-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6/readme.md
+-rw-r--r--   0        0        0    35894 1970-01-01 00:00:00.000000 python_115-0.0.6/PKG-INFO
```

### Comparing `python_115-0.0.5.9.1/LICENSE` & `python_115-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/__init__.py` & `python_115-0.0.6/p115/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,41 +396,40 @@
         """帮助函数：执行异步的网络请求
         """
         request_kwargs.pop("stream", None)
         req = self.async_session.request(method, url, **request_kwargs)
         if parse is None:
             async def request():
                 async with req as resp:
-                    pass
-            return request()
+                    return resp
         elif callable(parse):
             ac = argcount(parse)
             async def request():
                 async with req as resp:
                     if ac == 1:
                         ret = parse(resp)
                     else:
                         ret = parse(resp, (await resp.read()))
                     if isawaitable(ret):
                         ret = await ret
                     return ret
-            return request()
         elif parse:
             async def request():
                 async with req as resp:
                     content_type = resp.headers.get("Content-Type", "")
                     if content_type == "application/json":
                         return await resp.json()
                     elif content_type.startswith("application/json;"):
                         return loads(await resp.text())
                     elif content_type.startswith("text/"):
                         return await resp.text()
                     return await resp.read()
-            return request()
-        return req
+        else:
+            return req
+        return request()
 
     def request(
         self, 
         /, 
         url: str, 
         method: str = "GET", 
         parse: None | bool | Callable = lambda resp, content: loads(content), 
@@ -816,15 +815,16 @@
                 # - 图片: 2
                 # - 音频: 3
                 # - 视频: 4
                 # - 压缩包: 5
                 # - 应用: 6
         """
         api = "https://webapi.115.com/files"
-        payload = {"aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", "offset": 0, "record_open_time": 1, "show_dir": 1, **payload}
+        payload = {"aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", 
+                   "offset": 0, "record_open_time": 1, "show_dir": 1, **payload}
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def fs_files2(
         self, 
         payload: dict = {}, 
         /, 
         async_: bool = False, 
@@ -869,15 +869,16 @@
                 # - 图片: 2
                 # - 音频: 3
                 # - 视频: 4
                 # - 压缩包: 5
                 # - 应用: 6
         """
         api = "https://aps.115.com/natsort/files.php"
-        payload = {"aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", "offset": 0, "record_open_time": 1, "show_dir": 1, **payload}
+        payload = {"aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", 
+                   "offset": 0, "record_open_time": 1, "show_dir": 1, **payload}
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def fs_files_edit(
         self, 
         payload: list | dict, 
         /, 
         async_: bool = False, 
@@ -4166,16 +4167,16 @@
 
     def inode(self, /) -> int:
         return self.id
 
     def iter(
         self, 
         /, 
-        topdown: bool = True, 
-        min_depth: int = 0, 
+        topdown: Optional[bool] = True, 
+        min_depth: int = 1, 
         max_depth: int = 1, 
         predicate: Optional[Callable[[Self], Optional[bool]]] = None, 
         onerror: Optional[bool] = None, 
         **kwargs, 
     ) -> Iterator[Self]:
         return self.fs.iter(
             self, 
@@ -4200,15 +4201,15 @@
         if path == path_new:
             return self
         return type(self)({"fs": self.fs, "path": path_new})
 
     def listdir(self, /, **kwargs) -> list[str]:
         return self.fs.listdir(self, **kwargs)
 
-    def listdir_attr(self, /, **kwargs) -> list[dict]:
+    def listdir_attr(self, /, **kwargs) -> list[AttrDict]:
         return self.fs.listdir_attr(self, **kwargs)
 
     def listdir_path(self, /, **kwargs) -> list[Self]:
         return self.fs.listdir_path(self, **kwargs)
 
     def match(
         self, 
@@ -4396,43 +4397,63 @@
         url = ns["url"] = self.fs.get_url(self)
         ns["url_expire_time"] = int(parse_qsl(urlparse(url).query)[0][1])
         return url
 
     def walk(
         self, 
         /, 
-        topdown: bool = True, 
+        topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable = None, 
+        **kwargs, 
     ) -> Iterator[tuple[str, list[str], list[str]]]:
         return self.fs.walk(
             self, 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             onerror=onerror, 
-            _top=self.path, 
+            **kwargs, 
+        )
+
+    def walk_attr(
+        self, 
+        /, 
+        topdown: Optional[bool] = True, 
+        min_depth: int = 0, 
+        max_depth: int = -1, 
+        onerror: None | bool | Callable = None, 
+        **kwargs, 
+    ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
+        return self.fs.walk_attr(
+            self, 
+            topdown=topdown, 
+            min_depth=min_depth, 
+            max_depth=max_depth, 
+            onerror=onerror, 
+            **kwargs, 
         )
 
     def walk_path(
         self, 
         /, 
-        topdown: bool = True, 
+        topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable = None, 
+        **kwargs, 
     ) -> Iterator[tuple[str, list[Self], list[Self]]]:
         return self.fs.walk_path(
             self, 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             onerror=onerror, 
-            _top=self.path, 
+            **kwargs, 
         )
 
     def with_name(self, name: str, /) -> Self:
         return self.parent.joinpath(name)
 
     def with_stem(self, stem: str, /) -> Self:
         return self.parent.joinpath(stem + self.suffix)
@@ -4922,47 +4943,107 @@
         if isinstance(id_or_path, path_class):
             return not id_or_path["is_directory"]
         try:
             return not self.attr(id_or_path, pid)["is_directory"]
         except FileNotFoundError:
             return False
 
-    # TODO: 支持宽度优先遍历
-    def iter(
+    def _iter_bfs(
+        self, 
+        top: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        min_depth: int = 1, 
+        max_depth: int = 1, 
+        predicate: Optional[Callable[[P115PathType], Optional[bool]]] = None, 
+        onerror: Optional[bool] = None, 
+        **kwargs, 
+    ) -> Iterator[P115PathType]:
+        dq: deque[tuple[int, P115PathType]] = deque()
+        push, pop = dq.append, dq.popleft
+        path_class = type(self).path_class
+        path = self.as_path(top, pid)
+        if not path.is_attr_loaded:
+            path()
+        push((0, path))
+        while dq:
+            depth, path = pop()
+            if min_depth <= 0:
+                pred = predicate(path) if predicate else True
+                if pred is None:
+                    return
+                elif pred:
+                    yield path
+                min_depth = 1
+            if depth == 0 and (not path.is_dir() or 0 <= max_depth <= depth):
+                return
+            depth += 1
+            try:
+                for attr in self.iterdir(path, **kwargs):
+                    path = path_class(attr)
+                    pred = predicate(path) if predicate else True
+                    if pred is None:
+                        continue
+                    elif pred and depth >= min_depth:
+                        yield path
+                    if path.is_dir() and (max_depth < 0 or depth < max_depth):
+                        push((depth, path))
+            except OSError as e:
+                if callable(onerror):
+                    onerror(e)
+                elif onerror:
+                    raise
+
+    def _iter_dfs(
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         topdown: bool = True, 
-        min_depth: int = 0, 
+        min_depth: int = 1, 
         max_depth: int = 1, 
         predicate: Optional[Callable[[P115PathType], Optional[bool]]] = None, 
         onerror: Optional[bool] = None, 
         **kwargs, 
     ) -> Iterator[P115PathType]:
         if not max_depth:
             return
-        if min_depth > 0:
+        global_yield_me = True
+        if min_depth > 1:
+            global_yield_me = False
             min_depth -= 1
+        elif min_depth <= 0:
+            path = self.as_path(top, pid)
+            if not path.is_attr_loaded:
+                path()
+            pred = predicate(path) if predicate else True
+            if pred is None:
+                return
+            elif pred:
+                yield path
+            if path.is_file():
+                return
+            min_depth = 1
+            top = path.id
         if max_depth > 0:
             max_depth -= 1
         path_class = type(self).path_class
         try:
             for attr in self.iterdir(top, pid, **kwargs):
                 path = path_class(attr)
-                yield_me = min_depth <= 0
+                yield_me = global_yield_me
                 if yield_me and predicate:
                     pred = predicate(path)
                     if pred is None:
                         continue
                     yield_me = pred 
                 if yield_me and topdown:
                     yield path
-                if path["is_directory"]:
-                    yield from self.iter(
+                if path.is_dir():
+                    yield from self._iter_dfs(
                         path, 
                         topdown=topdown, 
                         min_depth=min_depth, 
                         max_depth=max_depth, 
                         predicate=predicate, 
                         onerror=onerror, 
                     )
@@ -4970,14 +5051,48 @@
                     yield path
         except OSError as e:
             if callable(onerror):
                 onerror(e)
             elif onerror:
                 raise
 
+    def iter(
+        self, 
+        top: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        topdown: Optional[bool] = True, 
+        min_depth: int = 1, 
+        max_depth: int = 1, 
+        predicate: Optional[Callable[[P115PathType], Optional[bool]]] = None, 
+        onerror: Optional[bool] = None, 
+        **kwargs, 
+    ) -> Iterator[P115PathType]:
+        if topdown is None:
+            return self._iter_bfs(
+                top, 
+                pid, 
+                min_depth=min_depth, 
+                max_depth=max_depth, 
+                predicate=predicate, 
+                onerror=onerror, 
+                **kwargs, 
+            )
+        else:
+            return self._iter_dfs(
+                top, 
+                pid, 
+                topdown=topdown, 
+                min_depth=min_depth, 
+                max_depth=max_depth, 
+                predicate=predicate, 
+                onerror=onerror, 
+                **kwargs, 
+            )
+
     def listdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         full_path: bool = False, 
         **kwargs, 
@@ -5150,109 +5265,172 @@
         /, 
         pid: Optional[int] = None, 
     ) -> stat_result:
         raise UnsupportedOperation(errno.ENOSYS, 
             "`stat()` is currently not supported, use `attr()` instead."
         )
 
-    def walk(
+    def _walk_bfs(
+        self, 
+        top: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        min_depth: int = 0, 
+        max_depth: int = -1, 
+        onerror: None | bool | Callable = None, 
+        **kwargs, 
+    ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
+        dq: deque[tuple[int, AttrDict]] = deque()
+        push, pop = dq.append, dq.popleft
+        push((0, self.attr(top, pid)))
+        while dq:
+            depth, parent = pop()
+            depth += 1
+            try:
+                push_me = max_depth < 0 or depth < max_depth
+                if min_depth <= 0 or depth >= min_depth:
+                    dirs: list[AttrDict] = []
+                    files: list[AttrDict] = []
+                    for attr in self.iterdir(parent, **kwargs):
+                        if attr["is_directory"]:
+                            dirs.append(attr)
+                            if push_me:
+                                push((depth, attr))
+                        else:
+                            files.append(attr)
+                    yield parent["path"], dirs, files
+                elif push_me:
+                    for attr in self.iterdir(parent, **kwargs):
+                        if attr["is_directory"]:
+                            push((depth, attr))
+            except OSError as e:
+                if callable(onerror):
+                    onerror(e)
+                elif onerror:
+                    raise
+
+    def _walk_dfs(
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         topdown: bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable = None, 
-        _top: str = "", 
         **kwargs, 
-    ) -> Iterator[tuple[str, list[str], list[str]]]:
+    ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         if not max_depth:
             return
         if min_depth > 0:
             min_depth -= 1
         if max_depth > 0:
             max_depth -= 1
         yield_me = min_depth <= 0
         try:
-            if not _top:
-                _top = self.get_path(top, pid)
-            dirs: list[str] = []
-            files: list[str] = []
-            attrs: list[AttrDict] = []
+            dirs: list[AttrDict] = []
+            files: list[AttrDict] = []
             for attr in self.iterdir(top, pid, **kwargs):
                 if attr["is_directory"]:
-                    attrs.append(attr)
-                    dirs.append(attr["name"])
+                    dirs.append(attr)
                 else:
-                    files.append(attr["name"])
+                    files.append(attr)
             if yield_me and topdown:
-                yield _top, dirs, files
-            for attr in attrs:
-                yield from self.walk(
-                    attr["id"], 
+                yield self.get_path(top, pid), dirs, files
+            for attr in dirs:
+                yield from self._walk_dfs(
+                    attr, 
                     topdown=topdown, 
                     min_depth=min_depth, 
                     max_depth=max_depth, 
                     onerror=onerror, 
-                    _top=joinpath(_top, escape(attr["name"])), 
                 )
             if yield_me and not topdown:
-                yield _top, dirs, files
+                yield self.get_path(top, pid), dirs, files
         except OSError as e:
             if callable(onerror):
                 onerror(e)
             elif onerror:
                 raise
 
+    def walk(
+        self, 
+        top: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        topdown: Optional[bool] = True, 
+        min_depth: int = 0, 
+        max_depth: int = -1, 
+        onerror: None | bool | Callable = None, 
+        **kwargs, 
+    ) -> Iterator[tuple[str, list[str], list[str]]]:
+        for path, dirs, files in self.walk_attr(
+            top, 
+            pid, 
+            topdown=topdown, 
+            min_depth=min_depth, 
+            max_depth=max_depth, 
+            onerror=onerror, 
+            **kwargs, 
+        ):
+            yield path, [a["name"] for a in dirs], [a["name"] for a in files]
+
+    def walk_attr(
+        self, 
+        top: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        topdown: Optional[bool] = True, 
+        min_depth: int = 0, 
+        max_depth: int = -1, 
+        onerror: None | bool | Callable = None, 
+        **kwargs, 
+    ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
+        if topdown is None:
+            return self._walk_bfs(
+                top, 
+                pid, 
+                min_depth=min_depth, 
+                max_depth=max_depth, 
+                onerror=onerror, 
+                **kwargs, 
+            )
+        else:
+            return self._walk_dfs(
+                top, 
+                pid, 
+                topdown=topdown, 
+                min_depth=min_depth, 
+                max_depth=max_depth, 
+                onerror=onerror, 
+                **kwargs, 
+            )
+
     def walk_path(
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-        topdown: bool = True, 
+        topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable = None, 
-        _top: str = "", 
         **kwargs, 
     ) -> Iterator[tuple[str, list[P115PathType], list[P115PathType]]]:
-        if not max_depth:
-            return
-        if min_depth > 0:
-            min_depth -= 1
-        if max_depth > 0:
-            max_depth -= 1
-        yield_me = min_depth <= 0
         path_class = type(self).path_class
-        try:
-            if not _top:
-                _top = self.get_path(top, pid)
-            dirs: list[P115PathType] = []
-            files: list[P115PathType] = []
-            for attr in self.iterdir(top, pid, **kwargs):
-                (dirs if attr["is_directory"] else files).append(path_class(attr))
-            if yield_me and topdown:
-                yield _top, dirs, files
-            for path in dirs:
-                yield from self.walk_path(
-                    path["id"], 
-                    topdown=topdown, 
-                    min_depth=min_depth, 
-                    max_depth=max_depth, 
-                    onerror=onerror, 
-                    _top=joinpath(_top, escape(path["name"])), 
-                )
-            if yield_me and not topdown:
-                yield _top, dirs, files
-        except OSError as e:
-            if callable(onerror):
-                onerror(e)
-            elif onerror:
-                raise
+        for path, dirs, files in self.walk_attr(
+            top, 
+            pid, 
+            topdown=topdown, 
+            min_depth=min_depth, 
+            max_depth=max_depth, 
+            onerror=onerror, 
+            **kwargs, 
+        ):
+            yield path, [path_class(a) for a in dirs], [path_class(a) for a in files]
 
     cd  = chdir
     pwd = getcwd
     ls  = listdir
     la  = listdir_attr
     ll  = listdir_path
 
@@ -5622,15 +5800,15 @@
         else:
             attr = None
             if not refresh:
                 path_class = type(self).path_class
                 if isinstance(id_or_path, dict):
                     attr = id_or_path
                 elif isinstance(id_or_path, path_class):
-                    if id_or_path.is_attr_loaded:
+                    if not id_or_path.is_attr_loaded:
                         id_or_path()
                     attr = id_or_path.__dict__
             if attr is None:
                 attr = self.attr(id_or_path, pid)
             if not attr["is_directory"]:
                 raise NotADirectoryError(
                     errno.ENOTDIR, 
@@ -6472,14 +6650,15 @@
             return self.attr(id_or_path, pid)
         except FileNotFoundError:
             if isinstance(id_or_path, int):
                 raise ValueError(f"no such id: {id_or_path!r}")
             return self.upload(BytesIO(), id_or_path, pid=pid)
 
     # TODO: 增加功能，返回一个 Task 对象，可以获取上传进度，可随时取消
+    # TODO: 支持一个参数，不计算 sha1 等信息，直接就进行上传（就像网页版那样）
     def upload(
         self, 
         /, 
         file: bytes | str | PathLike | SupportsRead[bytes], 
         path: IDOrPathType = "", 
         pid: Optional[int] = None, 
         overwrite_or_ignore: Optional[bool] = None, 
@@ -7521,24 +7700,24 @@
             offset = 0
         if page_size <= 0:
             page_size = 1 << 10
         payload = {"offset": offset, "limit": page_size}
         count = 0
         while True:
             resp = check_response(self.client.recyclebin_list(payload))
-            if resp["offset"] != offset:
+            if resp["offset"] != payload["offset"]:
                 return
             if count == 0:
                 count = int(resp["count"])
             elif count != int(resp["count"]):
                 raise RuntimeError("detected count changes during iteration")
             yield from resp["data"]
             if len(resp["data"]) < resp["page_size"]:
                 return
-            payload["offset"] = offset + resp["page_size"]
+            payload["offset"] += resp["page_size"]
 
     def list(self, /, offset: int = 0, limit: int = 0) -> list[dict]:
         if limit <= 0:
             return list(self.iter(offset))
         resp = check_response(self.client.recyclebin_list({"offset": offset, "limit": limit}))
         if resp["offset"] != offset:
             return []
@@ -7656,15 +7835,15 @@
             if count == 0:
                 count = resp["count"]
             elif count != resp["count"]:
                 raise RuntimeError("detected count changes during iteration")
             yield from resp["list"]
             if len(resp["list"]) < page_size:
                 break
-            payload["offset"] = offset + page_size
+            payload["offset"] += page_size
 
     def list(self, /, offset: int = 0, limit: int = 0) -> list[dict]:
         if limit <= 0:
             return list(self.iter(offset))
         return check_response(self.client.share_list({"offset": offset, "limit": limit}))["list"]
 
     @check_response
@@ -7691,7 +7870,8 @@
 
 # TODO upload_tree 多线程和进度条，并且为每一个上传返回一个 task，可重试
 # TODO 能及时处理文件已不存在
 # TODO 为各个fs接口添加额外的请求参数
 # TODO 115中多个文件可以在同一目录下同名，如何处理
 # TODO 提供一个新的上传函数，上传如果失败，因为名字问题，则尝试用uuid名字，上传成功后，再进行改名，如果成功，删除原来的文件，不成功，则删掉上传的文件（如果上传成功了的话）
 # TODO 如果压缩包尚未解压，则使用 zipfile 之类的模块，去模拟文件系统
+
```

### Comparing `python_115-0.0.5.9.1/p115/util/_init_mimetypes.py` & `python_115-0.0.6/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/cipher.py` & `python_115-0.0.6/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/concurrent.py` & `python_115-0.0.6/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/download.py` & `python_115-0.0.6/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/file.py` & `python_115-0.0.6/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/hash.py` & `python_115-0.0.6/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/ignore.py` & `python_115-0.0.6/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/iter.py` & `python_115-0.0.6/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/path.py` & `python_115-0.0.6/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/property.py` & `python_115-0.0.6/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/response.py` & `python_115-0.0.6/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/retry.py` & `python_115-0.0.6/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/text.py` & `python_115-0.0.6/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/p115/util/urlopen.py` & `python_115-0.0.6/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/pyproject.toml` & `python_115-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.9.1"
+version = "0.0.6"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.5.9.1/readme.md` & `python_115-0.0.6/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9.1/PKG-INFO` & `python_115-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.9.1
+Version: 0.0.6
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

