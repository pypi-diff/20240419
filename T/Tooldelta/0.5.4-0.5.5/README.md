# Comparing `tmp/tooldelta-0.5.4.tar.gz` & `tmp/tooldelta-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.4.tar", max compression
+gzip compressed data, was "tooldelta-0.5.5.tar", max compression
```

## Comparing `tooldelta-0.5.4.tar` & `tooldelta-0.5.5.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rwxr-xr-x   0        0        0     1497 2024-04-17 13:22:32.158901 tooldelta-0.5.4/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-17 13:22:32.158901 tooldelta-0.5.4/README.md
--rwxr-xr-x   0        0        0      973 2024-04-17 13:22:49.482918 tooldelta-0.5.4/pyproject.toml
--rwxr-xr-x   0        0        0      330 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/__init__.py
--rw-r--r--   0        0        0     4963 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/auths.py
--rwxr-xr-x   0        0        0      599 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/basic_mods.py
--rwxr-xr-x   0        0        0    16782 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    10594 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/cfg.py
--rwxr-xr-x   0        0        0     7848 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/color_print.py
--rw-r--r--   0        0        0     2045 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    29713 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/frame.py
--rwxr-xr-x   0        0        0     3772 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      338 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    31347 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1080 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2138 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/logger.py
--rwxr-xr-x   0        0        0    29561 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/neo_libs/neo_conn.py
--rwxr-xr-x   0        0        0     1143 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/packets.py
--rwxr-xr-x   0        0        0    11378 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     2318 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     6200 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      345 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     6780 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9235 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    13702 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    13481 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1758 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/starter.py
--rwxr-xr-x   0        0        0      638 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9071 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-19 00:30:34.663456 tooldelta-0.5.5/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-19 00:30:34.663456 tooldelta-0.5.5/README.md
+-rwxr-xr-x   0        0        0      973 2024-04-19 00:30:46.263467 tooldelta-0.5.5/pyproject.toml
+-rwxr-xr-x   0        0        0      360 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    19961 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    12365 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10889 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1884 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    30100 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     4644 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    20488 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1276 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/logger.py
+-rwxr-xr-x   0        0        0    29616 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/neo_libs/neo_conn.py
+-rwxr-xr-x   0        0        0     1292 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    15769 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     7341 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      450 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     9975 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9146 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    16934 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16769 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1774 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      808 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9071 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.5/PKG-INFO
```

### Comparing `tooldelta-0.5.4/LICENSE` & `tooldelta-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.4/README.md` & `tooldelta-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.4/pyproject.toml` & `tooldelta-0.5.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.4" # This field is automatically set to the value in the version file
+version = "0.5.5" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.5.4/tooldelta/auths.py` & `tooldelta-0.5.5/tooldelta/auths.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Any
-import requests
+"认证模块"
+
 import getpass
-import json
 import hashlib
+from typing import Any
+import requests
+import ujson as json
 from tooldelta import constants
-from tooldelta.color_print import Print
+from .color_print import Print
 
 
 def liliya_login() -> str:
     """登录咕咕账号
 
     Raises:
         requests.exceptions.RequestException: 登录失败
```

### Comparing `tooldelta-0.5.4/tooldelta/builtins.py` & `tooldelta-0.5.5/tooldelta/builtins.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,297 +1,358 @@
-from .color_print import Print
-import ujson
+"""
+提供了一些实用方法的类
+
+Classes:
+- Builtins: 一个提供了线程、JSON操作和文件操作的实用方法的类。
+
+Methods:
+- ThreadExit: 用于线程终止的SystemExit的子类。
+- ClassicThread: 简化ToolDelta子线程创建的threading.Thread的子类。
+- TMPJson: 提供了加载、卸载、读取和写入JSON文件到缓存区的方法的类。
+- SimpleJsonDataReader: 提供了安全的JSON文件操作方法的类。
+- get_threads_list: 返回使用createThread创建的所有线程的列表。
+- SimpleFmt: 使用字典中的值替换字符串中的占位符的静态方法。
+"""
+
+from io import TextIOWrapper
 import os
-import threading
-import traceback
+import time
 import copy
+from typing import Any, Callable, Dict, List, Tuple, Optional
 import ctypes
-import time
-from typing import Any, Dict, List, Tuple, Optional
+import threading
+import traceback
+import json as rjson
+import ujson as json
+from .color_print import Print
 
 event_pool = {"tmpjson_save": threading.Event()}
 event_flags_pool = {"tmpjson_save": True}
 threads_list: list["Builtins.createThread"] = []
 
+
 class Builtins:
+    """提供了一些实用方法的类"""
     class ThreadExit(SystemExit):
-        "线程退出."
+        """线程退出."""
 
     class ClassicThread(threading.Thread):
-        def __init__(self, func, args: tuple = (), usage="", **kwargs):
-            """
-            方便地新建一个ToolDelta子线程
+        """简化ToolDelta子线程创建的threading.Thread的子类."""
+
+        def __init__(self, func: Callable, args: tuple = (), usage="", **kwargs):
+            """新建一个ToolDelta子线程
 
-            参数:
-                func: 线程方法
-                args: 方法的参数项 tuple
-                usage: 线程的用途说明
-                ..kwargs: 方法的关键字参数项
+            Args:
+                func (Callable): 线程方法
+                args (tuple, optional):方法的参数项
+                usage (str, optional): 线程的用途说明
+                kwargs (dict, optional): 方法的关键词参数项
             """
             super().__init__(target=func)
             self.func = func
             self.daemon = True
             self.all_args = [args, kwargs]
             self.usage = usage
             self.start()
+            self.stopping = False
+            self._thread_id = None
 
-        def run(self):
+        def run(self) -> None:
+            """线程运行方法"""
             threads_list.append(self)
             try:
                 self.func(*self.all_args[0], **self.all_args[1])
             except (Builtins.ThreadExit, SystemExit):
                 pass
-            except:
-                Print.print_err(f"线程 {self.usage or self.func.__name__} 出错:\n" + traceback.format_exc())
+            except Exception:
+                Print.print_err(
+                    f"线程 {self.usage or self.func.__name__} 出错:\n" + traceback.format_exc())
             finally:
                 threads_list.remove(self)
 
-        def get_id(self):
-            if hasattr(self, '_thread_id'):
-                return self._thread_id
-            for id, thread in threading._active.items():
-                if thread is self:
-                    return id
+        def get_id(self) -> int:
+            """获取线程的ID
+
+            Raises:
+                RuntimeError: 线程ID未知
+
+            Returns:
+                int: 线程ID
+            """
+            if self._thread_id is None:
+                for thread in threading.enumerate():
+                    if thread is self:
+                        self._thread_id = thread.ident
+                        break
+            if self._thread_id is None:
+                raise RuntimeError("Could not determine the thread's ID")
+            return self._thread_id
 
-        def stop(self):
+        def stop(self) -> None:
+            """终止线程"""
             self.stopping = True
+            self._thread_id = self.ident
             thread_id = self.get_id()
-            res = ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, ctypes.py_object(SystemExit))
+            res = ctypes.pythonapi.PyThreadState_SetAsyncExc(
+                thread_id, ctypes.py_object(SystemExit))
             if res > 1:
                 ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, 0)
                 Print.print_err("§c终止线程失败")
 
     createThread = ClassicThread
 
     class TMPJson:
+        """提供了加载、卸载、读取和写入JSON文件到缓存区的方法的类."""
         @staticmethod
-        def loadPathJson(path: str, needFileExists: bool = True):
+        def loadPathJson(path: str, needFileExists: bool = True) -> None:
             """
             将json文件从磁盘加载到缓存区, 以便快速读写.
             在缓存文件已加载的情况下, 再使用一次该方法不会有任何作用.
 
-            参数:
-                path: 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
-                needFileExists: 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且默认值为null
+            Args:
+                path (str): 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
+                needFileExists (bool, optional): 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且默认值为null
+
+            Raises:
+                err: 文件不存在时
             """
             if path in jsonPathTmp:
                 return
             try:
-                js = Builtins.SimpleJsonDataReader.SafeJsonLoad(path)
+                with open(path, 'r', encoding='utf-8') as file:
+                    js = Builtins.SimpleJsonDataReader.SafeJsonLoad(file)
             except FileNotFoundError as err:
                 if not needFileExists:
                     js = None
                 else:
                     raise err from None
             jsonPathTmp[path] = [False, js]
 
         @staticmethod
-        def unloadPathJson(path: str):
+        def unloadPathJson(path: str) -> bool:
             """
             将json文件从缓存区卸载(保存内容到磁盘), 之后不能再在缓存区对这个文件进行读写.
             在缓存文件已卸载的情况下, 再使用一次该方法不会有任何作用, 但是可以通过其返回的值来知道存盘有没有成功.
 
-            参数:
-                path: 文件的虚拟路径
+            Args:
+                path (str): 文件的虚拟路径
+
+            Returns:
+                bool: 存盘是否成功
             """
             if jsonPathTmp.get(path) is not None:
                 isChanged, dat = jsonPathTmp[path]
                 if isChanged:
-                    Builtins.SimpleJsonDataReader.SafeJsonDump(dat, path)
+                    with open(path, 'w', encoding='utf-8') as file:
+                        Builtins.SimpleJsonDataReader.SafeJsonDump(dat, file)
                 del jsonPathTmp[path]
                 return True
             return False
 
         @staticmethod
-        def read(path: str):
-            """
-            对缓存区的该虚拟路径的文件进行读操作
+        def read(path: str) -> list[Any] | dict[Any, Any] | Any:
+            """对缓存区的该虚拟路径的文件进行读操作, 返回一个深拷贝的JSON对象
+
+            Args:
+                path (str): 文件的虚拟路径
 
-            参数:
-                path: 文件的虚拟路径
+            Raises:
+                Exception: json路径未初始化, 不能进行读取和写入操作
+
+            Returns:
+                list[Any] | dict[Any, Any] | Any: 该虚拟路径的JSON
             """
             if path in jsonPathTmp:
-                val = jsonPathTmp.get(path)[1]
-                if isinstance(val, (list, dict)):
-                    val = copy.deepcopy(val)
-                return val
-            raise Exception("json路径未初始化, 不能进行读取和写入操作: " + path)
+                val = jsonPathTmp.get(path)
+                if val is not None:
+                    val = val[1]
+                    if isinstance(val, (list, dict)):
+                        val = copy.deepcopy(val)
+                    return val
+            raise ValueError("json路径未初始化, 不能进行读取和写入操作: " + path)
 
         @staticmethod
-        def get(path: str):
+        def get(path: str) -> None:
             """
             直接获取缓存区的该虚拟路径的JSON, 不使用copy
             WARNING: 如果你不知道有什么后果, 请老老实实使用`read(...)`而不是`get(...)`!
 
-            参数:
-                path: 文件的虚拟路径
+            Args:
+                path (str): 文件的虚拟路径
             """
             if path in jsonPathTmp:
-                val = jsonPathTmp.get(path)[1]
-                return val
-            raise Exception("json路径未初始化, 不能进行读取和写入操作: " + path)
-
+                val = jsonPathTmp.get(path)
+                if val is not None:
+                    val = val[1]
+                    return val
+            raise ValueError("json路径未初始化, 不能进行读取和写入操作: " + path)
 
         @staticmethod
-        def write(path: str, obj: Any):
+        def write(path: str, obj: Any) -> None:
             """
             对缓存区的该虚拟路径的文件进行写操作, 这将会覆盖之前的内容
 
-            参数:
-                path: 文件的虚拟路径
-                obj: 任何合法的JSON类型 例如 dict/list/str/bool/int/float
+            Args:
+                path (str): 文件的虚拟路径
+                obj (Any): 任何合法的JSON类型 例如 dict/list/str/bool/int/float
             """
             if path in jsonPathTmp:
                 jsonPathTmp[path] = [True, obj]
             else:
-                raise Exception("json路径未初始化, 不能进行读取和写入操作: " + path)
+                raise ValueError("json路径未初始化, 不能进行读取和写入操作: " + path)
 
         @staticmethod
-        def read_as_tmp(path: str, needFileExists: bool = True, timeout: int = 60):
-            """
-            读取json文件并将其从磁盘加载到缓存区, 以便一段时间内能快速读写.
-            推荐使用.
+        def read_as_tmp(path: str, needFileExists: bool = True, timeout: int = 60) -> Any:
+            """读取json文件并将其从磁盘加载到缓存区, 以便一段时间内能快速读写.
 
-            参数:
-                path: 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
-                needFileExists: 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且写入默认值null
-                timeout: 多久没有再进行读取操作时卸载缓存
+            Args:
+                path (str): 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
+                needFileExists (bool, optional): 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且写入默认值null
+                timeout (int, optional): 多久没有再进行读取操作时卸载缓存
+
+            Returns:
+                Any: 该虚拟路径的JSON
             """
             if path not in jsonUnloadPathTmp and not path in jsonPathTmp:
                 jsonUnloadPathTmp[path] = timeout + int(time.time())
                 Builtins.TMPJson.loadPathJson(path, needFileExists)
             return Builtins.TMPJson.read(path)
 
         @staticmethod
-        def write_as_tmp(path: str, obj: Any, needFileExists: bool = True, timeout: int = 60):
-            """
-            写入json文件并将其从磁盘加载到缓存区, 以便一段时间内能快速读写.
-            推荐使用.
+        def write_as_tmp(path: str, obj: Any, needFileExists: bool = True, timeout: int = 60) -> None:
+            """写入json文件并将其从磁盘加载到缓存区, 以便一段时间内能快速读写.
 
-            参数:
-                path: 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
-                obj: 任何合法的JSON类型 例如 dict/list/str/bool/int/float
-                needFileExists: 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且写入默认值null
-                timeout: 多久没有再进行读取操作时卸载缓存
+            Args:
+                path (str): 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
+                obj (Any): 任何合法的JSON类型 例如 dict/list/str/bool/int/float
+                needFileExists (bool, optional): 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且写入默认值null
+                timeout (int, optional): 多久没有再进行读取操作时卸载缓存
             """
             if path not in jsonUnloadPathTmp and not path in jsonPathTmp:
                 jsonUnloadPathTmp[path] = timeout + int(time.time())
                 Builtins.TMPJson.loadPathJson(path, needFileExists)
-            Builtins.TMPJson.write(obj)
+            Builtins.TMPJson.write(path, obj)
 
         @staticmethod
-        def cancel_change(path):
-            "取消缓存json所做的更改, 非必要情况请勿调用, 你不知道什么时候会自动保存所做更改"
+        def cancel_change(path: str) -> None:
+            """取消缓存json所做的更改, 非必要情况请勿调用, 你不知道什么时候会自动保存所做更改"""
             jsonPathTmp[path][0] = False
 
         @staticmethod
-        def get_tmps():
-            "不要调用!"
+        def get_tmps() -> Dict:
+            """不要调用!"""
             return jsonPathTmp.copy()
 
     class SimpleJsonDataReader:
+        """提供了安全的JSON文件操作方法的类."""
         @staticmethod
-        def SafeJsonDump(obj: str | dict | list, fp):
-            """
-            导出一个json文件, 会自动关闭文件读写接口.
+        def SafeJsonDump(obj: str | dict | list, fp: TextIOWrapper) -> None:
+            """将一个json对象写入一个文件, 会自动关闭文件读写接口.
 
-            参数:
-                obj: json对象.
-                fp: 由 `open(...)` 打开的文件读写口 或 文件路径.
+            Args:
+                obj (str | dict | list): JSON对象
+                fp (_type_): open(...)打开的文件读写口 或 文件路径
             """
             if isinstance(fp, str):
                 with open(fp, "w", encoding="utf-8") as file:
-                    file.write(ujson.dumps(obj, indent=4, ensure_ascii=False))
+                    file.write(json.dumps(obj, indent=4, ensure_ascii=False))
             else:
                 with fp:
-                    fp.write(ujson.dumps(obj, indent=4, ensure_ascii=False))
+                    fp.write(json.dumps(obj, indent=4, ensure_ascii=False))
 
         @staticmethod
-        def SafeJsonLoad(fp):
-            """
-            读取一个json文件, 会自动关闭文件读写接口.
+        def SafeJsonLoad(fp: TextIOWrapper) -> dict | list:
+            """从一个文件读取json对象, 会自动关闭文件读写接口.
+
+            Args:
+                fp (TextIOWrapper): open(...)打开的文件读写口
 
-            参数:
-                fp: open(...)打开的文件读写口 或 文件路径.
+            Returns:
+                dict | list: JSON对象
             """
             if isinstance(fp, str):
                 with open(fp, "r", encoding="utf-8") as file:
-                    return ujson.loads(file.read())
+                    return json.loads(file.read())
             with fp as file:
-                return ujson.loads(file.read())
+                return json.loads(file.read())
 
-        class DataReadError(ujson.JSONDecodeError):
-            ...
+        class DataReadError(json.JSONDecodeError):
+            """读取数据时发生错误"""
 
         @staticmethod
-        def readFileFrom(plugin_name: str, file: str, default: dict = None):
-            """
-            使用插件便捷地读取一个json文件,
-            这个文件应在 插件数据文件/<plugin_name>/<file>文件夹内, 文件夹不存在时也会自动创建
+        def readFileFrom(plugin_name: str, file: str, default: dict | None = None) -> dict | list:
+            """从插件数据文件夹读取一个json文件, 会自动创建文件夹和文件.
 
-            参数:
-                plugin_name: 插件名
-                file: 文件名
-                default: 不为None时: 当文件不存在则创建一个空文件, 使用default给出的json字典写入文件.
+            Args:
+                plugin_name (str): 插件名
+                file (str): 文件名
+                default (dict, optional): 默认值, 若文件不存在则会写入这个默认值
+
+            Raises:
+                Builtins.SimpleJsonDataReader.DataReadError: 读取数据时发生错误
+                err: 读取文件路径时发生错误
+
+            Returns:
+                dict | list: JSON对象
             """
             if file.endswith(".json"):
                 file = file[:-5]
             filepath = os.path.join("插件数据文件", plugin_name, f"{file}.json")
             os.makedirs(os.path.join("插件数据文件", plugin_name), exist_ok=True)
             try:
                 if default is not None and not os.path.isfile(filepath):
                     with open(filepath, "w", encoding="utf-8") as f:
                         Builtins.SimpleJsonDataReader.SafeJsonDump(default, f)
                     return default
                 with open(filepath, "r", encoding="utf-8") as f:
                     res = Builtins.SimpleJsonDataReader.SafeJsonLoad(f)
                 return res
-            except ujson.JSONDecodeError as err:
+            except rjson.JSONDecodeError as err:
+                # 判断是否有msg.doc.pos属性
                 raise Builtins.SimpleJsonDataReader.DataReadError(
                     err.msg, err.doc, err.pos
                 )
             except Exception as err:
                 Print.print_err(f"读文件路径 {filepath} 发生错误")
                 raise err
 
         @staticmethod
-        def writeFileTo(plugin_name: str, file: str, obj):
-            """
-            使用插件简单地写入一个json文件, 会覆盖原有内容
-            这个文件应在data/<plugin_name>/<file>文件夹内
+        def writeFileTo(plugin_name: str, file: str, obj: str | dict[Any, Any] | list[Any]) -> None:
+            """将一个json对象写入插件数据文件夹, 会自动创建文件夹和文件.
 
-            参数:
-                plugin_name: 插件名
-                file: 文件名
-                obj: 任何合法的JSON类型 例如 dict/list/str/bool/int/float
+            Args:
+                plugin_name (str): 插件名
+                file (str): 文件名
+                obj (str | dict[Any, Any] | list[Any]): JSON对象
             """
             os.makedirs(f"插件数据文件/{plugin_name}", exist_ok=True)
             with open(f"插件数据文件/{plugin_name}/{file}.json", "w", encoding="utf-8") as f:
                 Builtins.SimpleJsonDataReader.SafeJsonDump(obj, f)
 
     @staticmethod
-    def get_threads_list():
+    def get_threads_list() -> list["Builtins.createThread"]:
         "返回使用 createThread 创建的全线程列表."
         return threads_list
 
     @staticmethod
-    def SimpleFmt(kw: Dict[str, Any], __sub: str) -> str:
+    def SimpleFmt(kw: Dict[str, Any], *args: str) -> str:
         """
         快速将字符串内按照给出的dict的键值对替换掉内容.
 
         参数:
             kw: Dict[str, Any], 键值对应替换的内容
-            __sub: str, 需要被替换的字符串
+            *args: str, 需要被替换的字符串
 
         示例:
             >>> my_color = "red"; my_item = "apple"
             >>> kw = {"[颜色]": my_color, "[物品]": my_item}
             >>> Builtins.SimpleFmt(kw, "I like [颜色] [物品].")
             I like red apple.
         """
+        __sub = args[0]
         for k, v in kw.items():
             if k in __sub:
                 __sub = __sub.replace(k, str(v))
         return __sub
 
     @staticmethod
     def simpleAssert(cond: Any, exc: Any) -> None:
@@ -308,41 +369,42 @@
 
         @Builtins.run_as_new_thread
         def on_inject(self):
             ...
         """
 
         def thread_fun(*args: Tuple, **kwargs: Any) -> None:
-            Builtins.createThread(func, usage="简易线程方法:"+func.__name__, args=args, **kwargs)
+            Builtins.createThread(func, usage="简易线程方法:" +
+                                  func.__name__, args=args, **kwargs)
 
         return thread_fun
 
     run_as_new_thread = thread_func
     new_thread = thread_func
 
     @staticmethod
     def try_int(arg: Any) -> Optional[int]:
         """尝试将提供的参数化为int类型并返回, 否则返回None"""
         try:
             return int(arg)
-        except:
+        except Exception:
             return None
 
     @staticmethod
     def add_in_dialogue_player(player: str) -> None:
         """
         使玩家进入聊天栏对话模式, 可防止其在对话时继续触发另一个会话线程
 
         参数:
             player: str, 玩家名
         """
         if player not in in_dialogue_list:
             in_dialogue_list.append(player)
         else:
-            raise Exception("Already in a dialogue!")
+            raise ValueError("Already in a dialogue!")
 
     @staticmethod
     def remove_in_dialogue_player(player: str) -> None:
         """
         使玩家离开聊天栏对话模式
 
         参数:
@@ -405,28 +467,40 @@
         res = []
         for i in lst:
             if sub in i:
                 res.append(i)
         return res
 
     class ArgsReplacement:
+        """用于替换字符串中的占位符的类"""
+
         def __init__(self, kw: Dict[str, Any]):
             self.kw = kw
 
-        def replaceTo(self, __sub: str):
+        def replaceTo(self, __sub: str) -> str:
+            """
+
+            Args:
+                __sub (str): 需要替换的字符串
+
+            Returns:
+                str: 替换后的字符串
+            """
             for k, v in self.kw.items():
                 if k in __sub:
                     __sub = __sub.replace(k, str(v))
             return __sub
 
 
-def safe_close():
+def safe_close() -> None:
+    """安全关闭"""
     event_pool["tmpjson_save"].set()
     event_flags_pool["tmpjson_save"] = False
 
+
 def _tmpjson_save_thread():
     evt = event_pool["tmpjson_save"]
     secs = 0
     while 1:
         evt.wait(2)
         secs += 2
         if secs >= 60:
@@ -439,27 +513,29 @@
             if time.time() - v > 0:
                 Builtins.TMPJson.unloadPathJson(k)
                 del jsonUnloadPathTmp[k]
         if not event_flags_pool["tmpjson_save"]:
             return
 
 
-def tmpjson_save_thread():
+def tmpjson_save_thread() -> None:
+    """JSON缓存文件定时保存"""
     Builtins.createThread(_tmpjson_save_thread, usage="JSON缓存文件定时保存")
 
+
 def _dialogue_thread_run(player, func, exc_cb, args, kwargs):
     if not Builtins.player_in_dialogue(player):
         Builtins.add_in_dialogue_player(player)
     else:
         if exc_cb is not None:
             exc_cb(player)
         return
     try:
         func(*args, **kwargs)
-    except:
+    except Exception:
         Print.print_err(f"玩家{player}的会话线程 出现问题:")
         Print.print_err(traceback.format_exc())
     Builtins.remove_in_dialogue_player(player)
 
 
 jsonPathTmp = {}
 in_dialogue_list = []
```

### Comparing `tooldelta-0.5.4/tooldelta/cfg.py` & `tooldelta-0.5.5/tooldelta/cfg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-import ujson
+"""配置文件模块"""
+
 import os
+from typing import Any
+import ujson
 
 NoneType = type(None)
 
 PLUGINCFG_DEFAULT = {"配置版本": "0.0.1", "配置项": None}
 
 PLUGINCFG_STANDARD_TYPE = {"配置版本": str, "配置项": [type(None), dict]}
 
@@ -30,21 +33,29 @@
                     and obj >= 0,
                     Cfg.PNumber: lambda: isinstance(obj, (int, float)) and obj > 0,
                     Cfg.NNNumber: lambda: isinstance(obj, (int, float)) and obj >= 0,
                 }.get(i, lambda: isinstance(obj, typ))()
                 if result:
                     return True
             return False
-        except TypeError:
-            raise ValueError(f"Can't be: {typ}")
+        except TypeError as e:
+            raise ValueError(f"Can't be: {typ}") from e
     raise ValueError(f"Can't be: {typ}")
 
 
-def _CfgShowType(typ):
-    if type(typ) != type:
+def _CfgShowType(typ: Any) -> str:
+    """转换类型为中文字符串
+
+    Args:
+        typ (Any): 类型
+
+    Returns:
+        str: 中文字符串
+    """
+    if isinstance(typ, type):
         typ = type(typ)
     return {
         Cfg.PInt: "正整数",
         Cfg.NNInt: "非负整数",
         Cfg.PFloat: "正浮点小数",
         Cfg.NNFloat: "非负浮点小数",
         str: "字符串",
@@ -56,29 +67,36 @@
     }.get(typ, typ.__name__)
 
 
 FIND_NONE = r"%FindNone"
 
 
 class Cfg:
+    """配置文件模块"""
     class Group:
+        """配置文件的键组合, 用于检测多个键中的一个是否存在"""
+
         def __init__(self, *keys):
             self.members = keys
 
         def __repr__(self) -> str:
             return 'Cfg.Group("' + '", "'.join(self.members) + '")'
 
     class ConfigError(Exception):
-        def __init__(self, errStr: str, errPos: list = None):
+        "配置文件错误"
+
+        def __init__(self, errStr: str, errPos: list | None = None):
             if errPos is None:
                 errPos = []
             self.errPos = errPos
             self.args = (errStr,)
 
     class UnneccessaryKey:
+        "配置文件的多余键"
+
         def __init__(self, key):
             self.key = key
 
         def __repr__(self):
             return f"Cfg.UnneccessaryKey({self.key})"
 
     class ConfigKeyError(ConfigError):
@@ -105,43 +123,69 @@
     class PNumber:
         "配置文件的值限制: 正数"
 
     class NNNumber:
         "配置文件的值限制: 大于0的数"
 
     def get_cfg(self, path: str, standard_type: dict):
-        # 从path路径获取json文件文本信息, 并按照standard_type给出的标准形式进行检测.
+        "从path路径获取json文件文本信息, 并按照standard_type给出的标准形式进行检测."
         path = path if path.endswith(".json") else path + ".json"
         with open(path, "r", encoding="utf-8") as f:
             try:
                 obj = ujson.load(f)
-            except ujson.JSONDecodeError:
-                raise self.ConfigValueError("JSON配置文件格式不正确, 请修正或直接删除", None)
+            except ujson.JSONDecodeError as exc:
+                raise self.ConfigValueError(
+                    "JSON配置文件格式不正确, 请修正或直接删除", None) from exc
         self.check_dict_2(standard_type, obj)
         return obj
 
     @staticmethod
-    def default_cfg(path: str, default: dict, force: bool = False):
-        # 向path路径写入json文本, 若文件不存在或参数force为True, 将写入提供的默认json文本
+    def default_cfg(path: str, default: dict, force: bool = False) -> None:
+        """生成默认配置文件
+
+        Args:
+            path (str): 路径
+            default (dict): 默认配置
+            force (bool, optional): 是否强制生成
+        """
         path = path if path.endswith(".json") else path + ".json"
         if force or not os.path.isfile(path):
             with open(path, "w", encoding="utf-8") as f:
                 ujson.dump(default, f, indent=4, ensure_ascii=False)
 
     @staticmethod
-    def exists(path: str):
+    def exists(path: str) -> bool:
+        """判断文件是否存在
+
+        Args:
+            path (str): 路径
+
+        Returns:
+            bool: 是否存在
+        """
         return os.path.isfile(path if path.endswith(".json") else path + ".json")
 
     def getPluginConfigAndVersion(
         self,
         pluginName: str,
         standardType: dict,
         default: dict,
         default_vers: tuple[int, int, int],
-    ):
+    ) -> tuple[dict[str, Any], tuple[int, ...]]:
+        """获取插件配置文件及版本
+
+        Args:
+            pluginName (str): 插件名
+            standardType (dict): 标准类型
+            default (dict): 默认配置
+            default_vers (tuple[int, int, int]): 默认版本
+
+        Returns:
+             tuple[dict[str, Any], tuple[int, ...]]: 配置文件及版本
+        """
         # 详情见 插件编写指南.md
         assert isinstance(standardType, dict)
         p = "插件配置文件/" + pluginName
         if not self.exists(p) and default:
             defaultCfg = PLUGINCFG_DEFAULT.copy()
             defaultCfg["配置项"] = default
             defaultCfg["配置版本"] = ".".join([str(n) for n in default_vers])
@@ -149,15 +193,28 @@
             self.default_cfg(p + ".json", defaultCfg, force=True)
         cfg_stdtyp = PLUGINCFG_STANDARD_TYPE.copy()
         cfg_stdtyp["配置项"] = standardType
         cfgGet = self.get_cfg(p, cfg_stdtyp)
         cfgVers = tuple(int(c) for c in cfgGet["配置版本"].split("."))
         return cfgGet["配置项"], cfgVers
 
-    def check_auto(self, standard, val, fromkey="?"):
+    def check_auto(self, standard: type | dict | list, val: Any, fromkey: Any = "?") -> None:
+        """检查配置文件
+
+        Args:
+            standard (type, dict, list): 标准
+            val (Any): 值
+            fromkey (Any, optional): 键
+
+        Raises:
+            ValueError: 未知类型
+            self.ConfigValueError: 值错误
+            ValueError: 未知类型
+        """
+
         if fromkey == FIND_NONE:
             raise ValueError("不允许传入FindNone")
         if isinstance(standard, type):
             if not _CfgIsinstance(val, standard):
                 raise self.ConfigValueError(
                     f'JSON键"{fromkey}" 对应值的类型不正确: 需要 {_CfgShowType(standard)}, 实际上为 {_CfgShowType(val)}'
                 )
@@ -197,15 +254,27 @@
                     self.check_auto(std_val, val_get, key.key)
             else:
                 val_get = jsondict.get(key, FIND_NONE)
                 if val_get == FIND_NONE:
                     raise self.ConfigKeyError(f"不存在的JSON键: {key}")
                 self.check_auto(std_val, val_get, key)
 
-    def check_list_2(self, pattern: list, value, fromkey="?"):
+    def check_list_2(self, pattern: list, value: Any, fromkey: Any = "?") -> None:
+        """检查列表
+
+        Args:
+            pattern (list): 标准
+            value (Any): 值
+            fromkey (Any, optional): 键
+
+        Raises:
+            ValueError: 不是合法的标准列表检测样式
+            ValueError: 标准检测列表的长度不能为0
+            self.ConfigValueError: json键值错误
+        """
         if not isinstance(pattern, list):
             raise ValueError("不是合法的标准列表检测样式")
         if len(pattern) == 0:
             raise ValueError("标准检测列表的长度不能为0")
         if isinstance(pattern[0], str) and pattern[0].startswith(r"%list"):
             if not isinstance(value, list):
                 raise self.ConfigValueError(
@@ -221,15 +290,15 @@
             for val in value:
                 self.check_auto(pattern[1], val, fromkey)
         else:
             for single_type in pattern:
                 try:
                     self.check_auto(single_type, value, fromkey)
                     return
-                except Exception as err:
+                except Exception:
                     pass
             raise self.ConfigValueError(
                 f"JSON列表的值 \"{fromkey}\" 类型不正确: 需要 {' 或 '.join(_CfgShowType(i) for i in pattern)}, 实际上为 {_CfgShowType(value)}"
             )
 
     def auto_to_std(self, cfg):
         """
```

### Comparing `tooldelta-0.5.4/tooldelta/constants.py` & `tooldelta-0.5.5/tooldelta/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,18 @@
+" ToolDelta 常量定义 "
 from typing import List
-from tooldelta.launch_cli import FrameFBConn, FrameNeOmg, FrameNeOmgRemote
-from tooldelta.cfg import Cfg
-
+from .cfg import Cfg
+from .launch_cli import FrameNeOmg, FrameNeOmgRemote
 PRG_NAME = "ToolDelta"
 
 PLUGIN_MARKET_SOURCE_OFFICIAL = "https://tdload.tblstudio.cn/https://raw.githubusercontent.com/ToolDelta/ToolDelta-PluginMarket/main"
 
 LAUNCHERS: List[
-    tuple[str, type[FrameFBConn | FrameNeOmg | FrameNeOmgRemote]]
+    tuple[str, type[FrameNeOmg | FrameNeOmgRemote]]
 ] = [
-    (
-        "FastBuilder External 模式 (经典模式) §c(已停止维护, 无法适应新版本租赁服!)",
-        FrameFBConn,
-    ),
     ("NeOmega 框架 (NeOmega模式, 租赁服适应性强, 推荐)", FrameNeOmg),
     (
         "NeOmega 框架 (NeOmega连接模式, 需要先启动对应的neOmega接入点)",
         FrameNeOmgRemote,
     ),
 ]
```

### Comparing `tooldelta-0.5.4/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.5/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.4/tooldelta/frame.py` & `tooldelta-0.5.5/tooldelta/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 """
 整个系统由三个部分组成
     Frame: 负责整个 ToolDelta 的基本框架运行
     GameCtrl: 负责对接游戏
         - Launchers: 负责将不同启动器的游戏接口统一成固定的接口, 供插件在多平台游戏接口运行(FastBuilder External, NeOmega, (TLSP, etc.))
 """
 
-
-from typing import TYPE_CHECKING
+import os
+import sys
+import time
+import getpass
+import traceback
+from typing import TYPE_CHECKING, Callable
+import asyncio
+import ujson as json
+import requests
 import tooldelta
 from tooldelta import (
     auths,
     constants,
     plugin_market,
 )
 from .constants import PRG_NAME
 from .builtins import Builtins, safe_close
 from .get_tool_delta_version import get_tool_delta_version
 from .color_print import Print
-from .basic_mods import (
-    Callable,
-    os,
-    sys,
-    time,
-    traceback,
-    requests,
-    getpass
-)
 from .cfg import Cfg
 from .logger import publicLogger
 from .game_texts import GameTextsLoader
 from .urlmethod import if_token, fbtokenFix
 from .sys_args import sys_args_to_dict
 from .launch_cli import (
-    FrameFBConn,
     FrameNeOmg,
     FrameNeOmgRemote,
     SysStatus,
 )
 
-from .basic_mods import asyncio, json
 from .packets import PacketIDS
 from .plugin_load.injected_plugin import (
     execute_death_message,
     execute_init,
     execute_player_join,
     execute_player_prejoin,
     execute_player_left,
@@ -79,15 +75,15 @@
         self.serverNumber: int = 0
         self.serverPasswd: str = ""
         self.launchMode: int = 0
         self.consoleMenu = []
         self.on_plugin_err = staticmethod(
             lambda name, _, err: Print.print_err(f"插件 <{name}> 出现问题: \n{err}")
         )
-        self.launcher: FrameFBConn | FrameNeOmg | FrameNeOmgRemote
+        self.launcher: FrameNeOmg | FrameNeOmgRemote
         self.is_mir: bool
         self.plugin_market_url: str
         self.link_game_ctrl: "GameCtrl"
         self.link_plugin_group: "PluginGroup"
 
     def loadConfiguration(self) -> None:
         """加载配置文件"""
@@ -407,15 +403,15 @@
                 rsp = ""
                 while True:
                     res = sys.stdin.read(1)
                     if res == "\n":  # 如果是换行符，则输出当前输入并清空输入
                         break
                     if res in ("", "^C", "^D"):
                         Print.print_inf("按退出键退出中...")
-                        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg, FrameFBConn)):
+                        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg)):
                             self.launcher.status = SysStatus.NORMAL_EXIT
                         self.system_exit()
                         return
                     rsp += res
                 for _, _, func, triggers in self.consoleMenu:
                     if not rsp:
                         continue
@@ -443,15 +439,15 @@
             try:
                 self.link_game_ctrl.sendwscmd(
                     f"/kick {self.link_game_ctrl.bot_name} ToolDelta 退出中(看到这条消息请重新加入游戏)\nSTATUS CODE: {exit_status_code}"
                 )
             except Exception:
                 pass
         time.sleep(0.5)
-        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg, FrameFBConn)):
+        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg)):
             self.launcher.exit_event.set()
 
     def get_console_menus(self) -> list:
         """获取控制台命令列表
 
         Returns:
             list: 命令列表
@@ -508,22 +504,21 @@
         self.bot_name = ""
         self.linked_frame: Frame
         self.pkt_unique_id: int = 0
         self.pkt_cache: list = []
         self.require_listen_packets = {9, 79, 63}
         self.store_uuid_pkt: dict[str, str] | None = None
         self.launcher = self.linked_frame.launcher
-        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg, FrameFBConn)):
+        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg)):
             self.launcher.packet_handler = lambda pckType, pck: Builtins.createThread(
                 self.packet_handler, (pckType, pck), usage="数据包处理")
         self.sendcmd = self.launcher.sendcmd
         self.sendwscmd = self.launcher.sendwscmd
         self.sendwocmd = self.launcher.sendwocmd
         self.sendPacket = self.launcher.sendPacket
-        self.sendfbcmd = self.launcher.sendfbcmd
         if isinstance(self.linked_frame.launcher, FrameNeOmg):
             self.requireUUIDPacket = False
         else:
             self.requireUUIDPacket = True
 
     def set_listen_packets(self) -> None:
         """
@@ -671,22 +666,30 @@
         if res:
             self.allplayers = list(res.keys())
             self.players_uuid.update(res)
         else:
             while 1:
                 try:
                     cmd_result = self.sendwscmd("/list", True)
-                    if cmd_result:
-                        self.allplayers = (
-                            cmd_result
-                            .OutputMessages[1]
-                            .Parameters[0]
-                            .split(", ")
-                        )
-                        break
+                    if cmd_result is None:
+                        Print.print_err("获取全局玩家失败..重试")
+                        continue
+                    if cmd_result.OutputMessages is None or len(cmd_result.OutputMessages) < 2:
+                        Print.print_err("获取全局玩家失败..重试")
+                        continue
+                    if cmd_result.OutputMessages[1].Parameters is None or len(cmd_result.OutputMessages[1].Parameters) < 1:
+                        Print.print_err("获取全局玩家失败..重试")
+                        continue
+                    self.allplayers = (
+                        cmd_result
+                        .OutputMessages[1]
+                        .Parameters[0]
+                        .split(", ")
+                    )
+                    break
                 except TimeoutError:
                     Print.print_war("获取全局玩家失败..重试")
         self.bot_name = self.launcher.get_bot_name()
         if self.bot_name is None:
             self.bot_name = self.allplayers[0]
         self.linked_frame.comsole_cmd_start()
         self.linked_frame.link_plugin_group.execute_init(
@@ -737,15 +740,15 @@
 
         Args:
             target (str): 玩家名/目标选择器
             text (str): 文本
         """
         self.sendwocmd(f"title {target} subtitle {text}")
 
-    def player_actionbar(self, target: str, text: str) ->None:
+    def player_actionbar(self, target: str, text: str) -> None:
         """向玩家展示动作栏文本
 
         Args:
             target (str): 玩家名/目标选择器
             text (str): 文本
         """
         self.sendwocmd(f"title {target} actionbar {text}")
```

### Comparing `tooldelta-0.5.4/tooldelta/game_texts.py` & `tooldelta-0.5.5/tooldelta/game_texts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,128 @@
-from .basic_mods import (
-    os,
-    requests,
-    re,
-    tarfile,
-    gzip,
-    json,
-    importlib,
-    threading,
-    time,
-)
-from .urlmethod import download_file_singlethreaded
+"还原游戏常见字符串"
+import os
+import re
+import tarfile
+import gzip
+from importlib import util
+import threading
+from glob import glob
 from typing import Dict
+import requests
+import ujson as json
+from .urlmethod import download_file_singlethreaded
 from .color_print import Print
-from glob import glob
 
 
 class GameTextsLoader:
+    "还原游戏常见字符串"
+
     def __init__(self) -> None:
+        "初始化"
         self.base_path = os.path.join(os.getcwd(), "插件数据文件", "game_texts")
         self.check_initial_run()
         self.start_auto_update_thread()
         self.game_texts_data: Dict[str, str] = self.load_data()
 
     @staticmethod
     def get_latest_version() -> str:
-        return re.match(
+        """获取最新版本号
+
+        Returns:
+            str: 版本号
+        """
+        result = re.match(
             r"(\d+\.\d+\.\d+)",
             requests.get(
-                "https://api.github.com/repos/ToolDelta/GameText/releases/latest"
+                "https://api.github.com/repos/ToolDelta/GameText/releases/latest", timeout=5
             ).json()["tag_name"],
-        ).group()
+        )
+        if not isinstance(result, type(None)):
+            return result.group()
+        raise ValueError("无法获取最新版本号")
 
     def check_initial_run(self) -> None:
+        "检查初始运行"
         version_file_path: str = os.path.join(self.base_path, "version")
         if not os.path.exists(version_file_path):
             latest_version: str = self.get_latest_version()
             with open(version_file_path, "w", encoding="utf-8") as f:
                 f.write(latest_version)
             self.download_and_extract(latest_version)
 
     def start_auto_update_thread(self) -> None:
+        "启用自动更新线程"
         threading.Timer(24 * 60 * 60, self.auto_update).start()
 
     def auto_update(self) -> None:
+        "自动更新"
         version_file_path: str = os.path.join(self.base_path, "version")
         with open(version_file_path, "r", encoding="utf-8") as f:
             version: str = f.read()
         latest_version: str = self.get_latest_version()
         if version != latest_version:
             self.download_and_extract(latest_version)
         threading.Timer(24 * 60 * 60, self.auto_update).start()
 
-    def download_and_extract(self, version):
+    def download_and_extract(self, version) -> None:
+        "下载并解压"
         packets_url: str = (
             f"https://hub.gitmirror.com/?q=https://github.com/ToolDelta/GameText/releases/download/{version}/ToolDelta_Game_Texts.tar.gz"
         )
-        archive_path = os.path.join(self.base_path, "ToolDelta_Game_Texts.tar.gz")
+        archive_path = os.path.join(
+            self.base_path, "ToolDelta_Game_Texts.tar.gz")
         download_file_singlethreaded(packets_url, archive_path)
         self.extract_data_archive(archive_path)
 
     def load_data(self) -> Dict[str, str]:
+        """加载数据
+
+        Returns:
+            Dict[str, str]: 数据
+        """
         try:
             all_values: Dict[str, str] = {}
             for file_path in glob(
                 os.path.join(self.base_path, "src", "**", "*.py"), recursive=True
             ):
-                module_name: str = os.path.basename(file_path).replace(".py", "")
-                spec: importlib.util.spec_from_file_location = (
-                    importlib.util.spec_from_file_location(module_name, file_path)
+                module_name: str = os.path.basename(
+                    file_path).replace(".py", "")
+                spec = (
+                    util.spec_from_file_location(
+                        module_name, file_path)
                 )
-                module: importlib.util.module_from_spec = (
-                    importlib.util.module_from_spec(spec)
+                if isinstance(spec, type(None)) or isinstance(spec.loader, type(None)):
+                    Print.print_war(
+                        f"Failed to load module from {file_path}")
+                    continue
+                module = (
+                    util.module_from_spec(spec)
                 )
                 spec.loader.exec_module(module)
                 for var_name in dir(module):
                     if not var_name.startswith("__"):
                         var_value = getattr(module, var_name)
                         if isinstance(var_value, dict):
                             all_values.update(var_value)
             return all_values
-        except Exception as err:
+        except Exception:
             return {}
 
     def extract_data_archive(self, zip_path: str) -> bool:
+        """解压数据归档
+
+        Args:
+            zip_path (str): 压缩包路径
+
+        Returns:
+            bool: 是否成功
+        """
         try:
             with gzip.open(zip_path, "rb") as f_in, tarfile.open(
-                fileobj=f_in, mode="r"
+                fileobj=f_in, mode="r:gz" # type: ignore
             ) as tar:
                 tar.extractall(self.base_path)
                 with open(
                     os.path.join(self.base_path, "src_tree.json"), "w", encoding="utf-8"
                 ) as f:
                     json.dump(tar.getnames(), f)
                 return True
```

### Comparing `tooldelta-0.5.4/tooldelta/launch_cli.py` & `tooldelta-0.5.5/tooldelta/neo_libs/neo_conn.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,764 +1,928 @@
-"""客户端启动器框架"""
-
-import os
+import ctypes
+import ujson as json
+import os.path
+import traceback
 import threading
-import shlex
-import uuid
-import time
-import json
-import random
-import subprocess
+import enum
+from typing import Iterable, Tuple, Optional, Union, Any, Callable, List, Dict
+from threading import Thread
+from dataclasses import dataclass
+from tooldelta.color_print import Print
+from tooldelta.packets import Packet_CommandOutput
+
+CInt = ctypes.c_longlong
+CString = ctypes.c_char_p
+CBytes = ctypes.POINTER(ctypes.c_char)
+
+
+class byteCSlice(ctypes.Structure):
+    _fields_ = [
+        ("data", ctypes.POINTER(ctypes.c_char)),
+        ("len", ctypes.c_longlong),
+        ("cap", ctypes.c_longlong),
+    ]
+
+
+def toCString(string: str):
+    return ctypes.c_char_p(bytes(string, encoding="utf-8"))
+
+
+def to_GoInt(i: int):
+    return ctypes.c_longlong(i)
+
+
+def toPyString(cstring: bytes):
+    if cstring is None:
+        return ""
+    return cstring.decode(encoding="utf-8")
+
+
+def toByteCSlice(bs: bytes):
+    l = len(bs)
+    kwargs = {
+        "data": (ctypes.c_char * l)(*bs),
+        "len": l,
+        "cap": l,
+    }
+    return byteCSlice(**kwargs)
+
+
+# define lib path and how to load it
 import platform
-from typing import Callable, Optional
-import requests
-import ujson
-
-import tooldelta
-from tooldelta import constants
-from .cfg import Cfg
-from .fb_conn import fbconn
-from .builtins import Builtins
-from .color_print import Print
-from .basic_mods import socketio
-from .sys_args import sys_args_to_dict
-from .packets import Packet_CommandOutput, PacketIDS
-from .urlmethod import download_file_singlethreaded, get_free_port
-
-Config = Cfg()
-
-
-class SysStatus:
-    """系统状态码
-
-    LOADING: 启动器正在加载
-    LAUNCHING: 启动器正在启动
-    RUNNING: 启动器正在运行
-    NORMAL_EXIT: 正常退出
-    FB_LAUNCH_EXC: FastBuilder 启动异常
-    CRASHED_EXIT: 启动器崩溃退出
-    NEED_RESTART: 需要重启
-    """
-    LOADING = 100
-    LAUNCHING = 101
-    RUNNING = 102
-    NORMAL_EXIT = 103
-    FB_LAUNCH_EXC = 104
-    CRASHED_EXIT = 105
-    NEED_RESTART = 106
-    launch_type = "None"
-
-
-class StandardFrame:
-    """提供了标准的启动器框架, 作为 ToolDelta 和游戏交互的接口"""
-    launch_type = "Original"
-
-    def __init__(self, serverNumber, password, fbToken, auth_server_url):
-        self.serverNumber = serverNumber
-        self.serverPassword = password
-        self.fbToken = fbToken
-        self.auth_server = auth_server_url
-        self.system_type = platform.uname().system
-        self.inject_events = []
-        self.packet_handler: Callable | None = lambda pckType, pck: None
-        self.need_listen_packets = {9, 63, 79}
-        self._launcher_listener = None
-        self.exit_event = threading.Event()
-        self.status = SysStatus.LOADING
-
-    def add_listen_packets(self, *pcks: int):
-        for i in pcks:
-            self.need_listen_packets.add(i)
 
-    @staticmethod
-    def launch():
-        raise Exception("Cannot launch this launcher")
+sys_machine = platform.machine().lower()
+sys_type = platform.uname().system
+sys_fn = os.path.join(os.getcwd(), "tooldelta")
+if sys_machine == "x86_64":
+    sys_machine = "amd64"
+elif sys_machine == "aarch64":
+    sys_machine = "arm64"
+if sys_type == "Windows":
+    lib_path = f"neomega_windows_{sys_machine}.dll"
+    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+    LIB = ctypes.cdll.LoadLibrary(lib_path)
+elif "TERMUX_VERSION" in os.environ:
+    lib_path = "neomega_android_arm64.so"
+    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+    LIB = ctypes.CDLL(lib_path)
+elif sys_type == "Linux":
+    lib_path = f"neomega_linux_{sys_machine}.so"
+    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+    LIB = ctypes.CDLL(lib_path)
+else:
+    lib_path = f"neomega_macos_{sys_machine}.dylib"
+    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+    LIB = ctypes.CDLL(lib_path)
 
-    def listen_launched(self, cb):
-        self._launcher_listener = cb
+# define lib functions
 
-    @staticmethod
-    def get_players_and_uuids():
-        return None
+# lib core functions: connect
+LIB.ConnectOmega.argtypes = [CString]
+LIB.ConnectOmega.restype = CString
 
-    @staticmethod
-    def get_bot_name():
-        return None
 
-    def update_status(self, new_status):
-        self.status = new_status
-        if new_status == SysStatus.NORMAL_EXIT:
-            tooldelta.safe_jump(out_task=True)
-            self.exit_event.set()  # 设置事件，触发等待结束
-        if new_status == SysStatus.CRASHED_EXIT:
-            tooldelta.safe_jump(out_task=False)
-            self.exit_event.set()
+def ConnectOmega(address):
+    r = LIB.ConnectOmega(toCString(address))
+    if r is not None:
+        raise Exception(toPyString(r))
 
-    get_all_players = None
 
-    @staticmethod
-    def sendcmd(cmd: str, waitForResp: bool = False, timeout: int | float = 30) -> Optional[Packet_CommandOutput]:
-        ...
+@dataclass
+class AccountOptions:
+    AuthServer: str = "https://api.fastbuilder.pro"
+    UserToken: str = ""
+    UserName: str = ""
+    UserPassword: str = ""
+    ServerCode: str = ""
+    ServerPassword: str = ""
 
-    @staticmethod
-    def sendwscmd(cmd: str, waitForResp: bool = False, timeout: int | float = 30) -> Optional[Packet_CommandOutput]:
-        ...
 
-    @staticmethod
-    def sendwocmd(cmd: str) -> None:
-        ...
+LIB.StartOmega.argtypes = [CString, CString]
+LIB.StartOmega.restype = CString
 
-    @staticmethod
-    def sendfbcmd(cmd: str) -> None:
-        ...
 
-    @staticmethod
-    def sendPacket(pckID: int, pck: str) -> None:
-        ...
+def StartOmega(address, AccountOptions):
+    r = LIB.StartOmega(
+        toCString(address), toCString(json.dumps(AccountOptions.__dict__))
+    )
+    if r is not None:
+        raise Exception(toPyString(r))
 
-    @staticmethod
-    def sendPacketJson(pckID: int, pck: str) -> None:
-        ...
 
-    @staticmethod
-    def is_op(player: str) -> bool:
-        ...
+LIB.OmegaAvailable.restype = ctypes.c_uint8
 
 
-class FrameFBConn(StandardFrame):
-    # 使用原生 FastBuilder External 连接
-    cmds_reqs = []
-    cmds_resp = {}
-
-    def __init__(self, serverNumber, password, fbToken, auth_server):
-        super().__init__(serverNumber, password, fbToken, auth_server)
-        self.injected = False
-        self.downloadMissingFiles()
-        self.init_all_functions()
+def OmegaAvailable():
+    if LIB.OmegaAvailable() != 1:
+        raise Exception("omega Core disconnected")
 
-    def launch(self):
-        try:
-            free_port = get_free_port(10000)
-            self.runFB(port=free_port)
-            self.run_conn(port=free_port)
-            Builtins.createThread(self.output_fb_msgs_thread)
-            self.process_game_packets()
-        except Exception as err:
-            return err
-
-    def runFB(self, ip="127.0.0.1", port=8080):
-        if self.system_type == "Linux":
-            os.system("/usr/bin/chmod +x ./phoenixbuilder")
-            con_cmd = rf"./phoenixbuilder -A {self.auth_server} -t fbtoken --no-readline --no-update-check --listen-external {ip}:{port} -c {self.serverNumber} {f'-p {self.serverPassword}' if self.serverPassword else ''}"
-
-        # windows updated "./PRGM" command.
-        if self.system_type == "Windows":
-            con_cmd = rf".\phoenixbuilder.exe -A {self.auth_server} -t fbtoken --no-readline --no-update-check --listen-external {ip}:{port} -c {self.serverNumber} {f'-p {self.serverPassword}' if self.serverPassword else ''}"
-        self.fb_pipe = subprocess.Popen(
-            con_cmd,
-            stdin=subprocess.PIPE,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.STDOUT,
-        )
 
-    def run_conn(self, ip="127.0.0.1", port=8080, timeout=None):
-        connect_fb_start_time = time.time()
-        max_con_time = timeout or 10
-        while 1:
-            try:
-                self.con = fbconn.ConnectFB(f"{ip}:{port}")
-                Print.print_suc("§a成功连接上FastBuilder.")
-                return 1
-            except:
-                if time.time() - connect_fb_start_time > max_con_time:
-                    Print.print_err(f"§4{max_con_time}秒内未连接上FB，已退出")
-                    self.close_fb()
-                    raise SystemExit
-                if self.status == SysStatus.FB_LAUNCH_EXC:
-                    Print.print_err("§4连接FB时出现问题，已退出")
-                    self.close_fb()
-                    raise SystemExit
-
-    def output_fb_msgs_thread(self):
-        while 1:
-            tmp: str = self.fb_pipe.stdout.readline().decode("utf-8").strip("\n")
-            if not tmp:
-                continue
-            if " 简体中文" in tmp:
-                # seems will be unable forever because it's no longer supported.
-                try:
-                    self.fb_pipe.stdin.write(f"{tmp[1]}\n".encode("utf-8"))
-                    self.fb_pipe.stdin.flush()
-                    Print.print_inf(f"语言已自动选择为简体中文： [{tmp[1]}]")
-                except IndexError:
-                    Print.print_war("未能自动选择为简体中文")
-            elif "ERROR" in tmp:
-                if "Server not found" in tmp:
-                    Print.print_err(
-                        f"§c租赁服号: {self.serverNumber} 未找到, 有可能是租赁服关闭中, 或是设置了等级或密码"
-                    )
-                    self.update_status(SysStatus.CRASHED_EXIT)
-
-                elif "Unauthorized rental server number" in tmp:
-                    Print.print_err(
-                        f"§c租赁服号: {self.serverNumber} ，你还没有该服务器号的卡槽， 请前往用户中心购买"
-                    )
-                    self.update_status(SysStatus.CRASHED_EXIT)
-                elif "Failed to contact with API" in tmp:
-                    Print.print_err(
-                        "§c无法连接到验证服务器, 可能是FB服务器崩溃, 或者是你的IP处于黑名单中"
-                    )
-                    try:
-                        Print.print_war("尝试连接到 FastBuilder 验证服务器")
-                        requests.get("http://user.fastbuilder.pro", timeout=10)
-                        Print.print_err(
-                            "??? 未知情况， 有可能只是验证服务器崩溃， 用户中心并没有崩溃"
-                        )
-                    except:
-                        Print.print_err(
-                            "§cFastBuilder服务器无法访问， 请等待修复(加入FastBuilder频道查看详情)"
-                        )
-                    self.update_status(SysStatus.CRASHED_EXIT)
-                elif "Invalid token" in tmp:
-                    Print.print_err("§cFastBuilder Token 无法使用， 请重新下载")
-                    self.update_status(SysStatus.CRASHED_EXIT)
-                elif "netease.report.kick.hint" in tmp:
-                    Print.print_err(
-                        "§c无法连接到网易租赁服 -> 网易土豆的常见问题，检查你的租赁服状态（等级、是否开启、密码）并重试, 也可能是你的网络问题"
-                    )
-                    self.update_status(SysStatus.CRASHED_EXIT)
-                elif "Press ENTER to exit." in tmp:
-                    Print.print_err("§c程序退出")
-                    self.update_status(SysStatus.CRASHED_EXIT)
-                else:
-                    Print.print_with_info(tmp, "§b  FB  §r")
+# end lib core functions: connect
 
-            elif "Transfer: accept new connection @ " in tmp:
-                Print.print_with_info(
-                    "FastBuilder 监听端口已开放: " + tmp.split()[-1], "§b  FB  "
-                )
-            elif "Successfully created minecraft dialer." in tmp:
-                Print.print_with_info("§e成功创建于 Minecraft 的链接", "§b  FB  §r")
-            elif tmp.startswith("panic"):
-                Print.print_err(f"FastBuilder 出现问题: {tmp}")
-            else:
-                Print.print_with_info(tmp, "§b  FB  §r")
 
-    def close_fb(self):
-        try:
-            self.fb_pipe.stdin.write("exit\n".encode("utf-8"))
-            self.fb_pipe.stdin.flush()
-        except:
-            pass
-        try:
-            self.fb_pipe.kill()
-        except:
-            pass
-        Print.print_suc("成功关闭FB进程")
+# lib core: event basic
+class Event(ctypes.Structure):
+    _fields_ = [("type", CString), ("retriever", CString)]
 
-    def process_game_packets(self):
-        try:
-            for packet_bytes in fbconn.RecvGamePacket(self.con):
-                packet_type = packet_bytes[0]
-                if packet_type not in self.need_listen_packets:
-                    continue
-                packet_mapping = ujson.loads(
-                    fbconn.GamePacketBytesAsIsJsonStr(packet_bytes)
-                )
-                if packet_type == PacketIDS.CommandOutput:
-                    cmd_uuid = packet_mapping["CommandOrigin"]["UUID"].encode()
-                    if cmd_uuid in self.cmds_reqs:
-                        self.cmds_resp[cmd_uuid] = [
-                            time.time(), packet_mapping]
-                self.packet_handler(packet_type, packet_mapping)
-                if not self.injected and packet_type == PacketIDS.PlayerList:
-                    self.injected = True
-                    Builtins.createThread(self._launcher_listener)
-        except StopIteration:
-            pass
-        self.update_status(SysStatus.CRASHED_EXIT)
 
-    def downloadMissingFiles(self):
-        "获取缺失文件"
-        Print.print_with_info("§d将自动检测缺失文件并补全", "§d 加载 ")
-        mirror_src = "https://tdload.tblstudio.cn/"
-        file_get_src = (
-            mirror_src
-            + "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/require_files.json"
+LIB.EventPoll.restype = Event
+
+
+def EventPoll() -> tuple[str, str]:
+    event = LIB.EventPoll()
+    return toPyString(event.type), toPyString(event.retriever)
+
+
+def OmitEvent():
+    LIB.OmitEvent()
+
+
+# end lib core: event
+
+# event retrievers
+LIB.ConsumeOmegaConnError.restype = CString
+LIB.ConsumeCommandResponseCB.restype = CString
+
+
+class MCPacketEvent(ctypes.Structure):
+    _fields_ = [("packetDataAsJsonStr", CString), ("convertError", CString)]
+
+
+LIB.ConsumeMCPacket.restype = MCPacketEvent
+
+# Async Actions
+# cmds
+
+LIB.SendWebSocketCommandNeedResponse.argtypes = [CString, CString]
+
+
+def SendWebSocketCommandNeedResponse(cmd: str, retrieverID: str):
+    OmegaAvailable()
+    LIB.SendWebSocketCommandNeedResponse(toCString(cmd), toCString(retrieverID))
+
+
+LIB.SendPlayerCommandNeedResponse.argtypes = [CString, CString]
+
+
+def SendPlayerCommandNeedResponse(cmd: str, retrieverID: str):
+    OmegaAvailable()
+    LIB.SendPlayerCommandNeedResponse(toCString(cmd), toCString(retrieverID))
+
+
+# OneWay Actions
+LIB.SendWOCommand.argtypes = [CString]
+
+
+def SendSettingsCommand(cmd: str):
+    OmegaAvailable()
+    LIB.SendWOCommand(toCString(cmd))
+
+
+LIB.SendWebSocketCommandOmitResponse.argtypes = [CString]
+
+
+def SendWebSocketCommandOmitResponse(cmd: str):
+    OmegaAvailable()
+    LIB.SendWebSocketCommandOmitResponse(toCString(cmd))
+
+
+LIB.SendPlayerCommandOmitResponse.argtypes = [CString]
+
+
+def SendPlayerCommandOmitResponse(cmd: str):
+    OmegaAvailable()
+    LIB.SendPlayerCommandOmitResponse(toCString(cmd))
+
+
+# Instance Actions
+LIB.FreeMem.argtypes = [ctypes.c_void_p]
+LIB.ListenAllPackets.argtypes = None
+LIB.GetPacketNameIDMapping.restype = CString
+LIB.JsonStrAsIsGamePacketBytes.argtypes = [CInt, CString]
+
+
+class JsonStrAsIsGamePacketBytes_return(ctypes.Structure):
+    _fields_ = [("pktBytes", CBytes), ("l", CInt), ("err", CString)]
+
+
+LIB.JsonStrAsIsGamePacketBytes.restype = JsonStrAsIsGamePacketBytes_return
+
+
+def JsonStrAsIsGamePacketBytes(packetID: int, jsonStr: str) -> bytes:
+    r = LIB.JsonStrAsIsGamePacketBytes(to_GoInt(packetID), toCString(jsonStr))
+    if toPyString(r.err) != "":
+        raise ValueError(toPyString(r.err))
+    bs = r.pktBytes[: r.l]
+    LIB.FreeMem(r.pktBytes)
+    return bs
+
+
+LIB.SendGamePacket.argtypes = [CInt, CString]
+LIB.SendGamePacket.restype = CString
+
+
+def SendGamePacket(packetID: int, jsonStr: str) -> None:
+    r = LIB.SendGamePacket(to_GoInt(packetID), toCString(jsonStr))
+    if toPyString(r) != "":
+        raise ValueError(toPyString(r))
+
+
+LIB.GetClientMaintainedBotBasicInfo.restype = CString
+
+
+# ClientMaintainedBotBasicInfo will not change
+@dataclass
+class ClientMaintainedBotBasicInfo:
+    BotName: str = ""
+    BotRuntimeID: int = 0
+    BotUniqueID: int = 0
+    BotIdentity: str = ""
+    BotUUIDStr: str = ""
+
+
+LIB.GetClientMaintainedExtendInfo.restype = CString
+
+
+# any member of ClientMaintainedExtendInfo could be not found(which means related info not currently received from server)
+@dataclass
+class ClientMaintainedExtendInfo:
+    CompressThreshold: Optional[int] = None
+    WorldGameMode: Optional[int] = None
+    WorldDifficulty: Optional[int] = None
+    Time: Optional[int] = None
+    DayTime: Optional[int] = None
+    TimePercent: Optional[float] = None
+    GameRules: Optional[Dict[str, Any]] = None
+
+
+LIB.GetAllOnlinePlayers.restype = CString
+LIB.ReleaseBindPlayer.argtypes = [CString]
+LIB.PlayerName.argtypes = [CString]
+LIB.PlayerName.restype = CString
+LIB.PlayerEntityUniqueID.argtypes = [CString]
+LIB.PlayerEntityUniqueID.restype = ctypes.c_int64
+LIB.PlayerLoginTime.argtypes = [CString]
+LIB.PlayerLoginTime.restype = ctypes.c_int64
+LIB.PlayerPlatformChatID.argtypes = [CString]
+LIB.PlayerPlatformChatID.restype = CString
+LIB.PlayerBuildPlatform.argtypes = [CString]
+LIB.PlayerBuildPlatform.restype = ctypes.c_int32
+LIB.PlayerSkinID.argtypes = [CString]
+LIB.PlayerSkinID.restype = CString
+LIB.PlayerPropertiesFlag.argtypes = [CString]
+LIB.PlayerPropertiesFlag.restype = ctypes.c_uint32
+LIB.PlayerCommandPermissionLevel.argtypes = [CString]
+LIB.PlayerCommandPermissionLevel.restype = ctypes.c_uint32
+LIB.PlayerActionPermissions.argtypes = [CString]
+LIB.PlayerActionPermissions.restype = ctypes.c_uint32
+LIB.PlayerGetAbilityString.argtypes = [CString]
+LIB.PlayerGetAbilityString.restype = CString
+LIB.PlayerOPPermissionLevel.argtypes = [CString]
+LIB.PlayerOPPermissionLevel.restype = ctypes.c_uint32
+LIB.PlayerCustomStoredPermissions.argtypes = [CString]
+LIB.PlayerCustomStoredPermissions.restype = ctypes.c_uint32
+LIB.PlayerDeviceID.argtypes = [CString]
+LIB.PlayerDeviceID.restype = CString
+LIB.PlayerEntityRuntimeID.argtypes = [CString]
+LIB.PlayerEntityRuntimeID.restype = ctypes.c_uint64
+LIB.PlayerEntityMetadata.argtypes = [CString]
+LIB.PlayerEntityMetadata.restype = CString
+LIB.PlayerIsOP.argtypes = [CString]
+LIB.PlayerIsOP.restype = ctypes.c_uint8
+LIB.PlayerOnline.argtypes = [CString]
+LIB.PlayerOnline.restype = ctypes.c_uint8
+
+LIB.GetPlayerByUUID.argtypes = [CString]
+LIB.GetPlayerByUUID.restype = CString
+
+LIB.GetPlayerByName.argtypes = [CString]
+LIB.GetPlayerByName.restype = CString
+
+LIB.ConsumePlayerChange.restype = CString
+LIB.InterceptPlayerJustNextInput.argtypes = [CString, CString]
+LIB.ConsumeChat.restype = CString
+
+LIB.PlayerChat.argtypes = [CString, CString]
+LIB.PlayerTitle.argtypes = [CString, CString, CString]
+LIB.PlayerActionBar.argtypes = [CString, CString]
+LIB.SetPlayerAbility.argtypes = [CString, CString]
+
+LIB.ListenCommandBlock.argtypes = [CString]
+LIB.PlaceCommandBlock.argtypes = [CString]
+
+
+def ConsumeChat() -> "Chat":
+    chatData = json.loads(toPyString(LIB.ConsumeChat()))
+    return Chat(**chatData)
+
+
+class Counter:
+    def __init__(self, prefix: str) -> None:
+        self.current_i = 0
+        self.prefix = prefix
+
+    def __next__(self) -> int:
+        self.current_i += 1
+        return f"{self.prefix}_{self.current_i}"
+
+
+@dataclass
+class ActionPermissionMap:
+    ActionPermissionAttackMobs: bool = False
+    ActionPermissionAttackPlayers: bool = False
+    ActionPermissionBuild: bool = False
+    ActionPermissionDoorsAndSwitches: bool = False
+    ActionPermissionMine: bool = False
+    ActionPermissionOpenContainers: bool = False
+    ActionPermissionOperator: bool = False
+    ActionPermissionTeleport: bool = False
+    ActionPermissionUnknown: bool = False
+
+
+@dataclass
+class AdventureFlagsMap:
+    AdventureFlagAllowFlight: bool = False
+    AdventureFlagAutoJump: bool = False
+    AdventureFlagFlying: bool = False
+    AdventureFlagMuted: bool = False
+    AdventureFlagNoClip: bool = False
+    AdventureFlagWorldBuilder: bool = False
+    AdventureFlagWorldImmutable: bool = False
+    AdventureSettingsFlagsNoMvP: bool = False
+    AdventureSettingsFlagsNoPvM: bool = False
+    AdventureSettingsFlagsShowNameTags: bool = False
+
+
+@dataclass
+class Chat:
+    Name: str = ""
+    Msg: List[str] = ""
+    Type: int = 1
+    RawMsg: str = ""
+    RawName: str = ""
+    RawParameters: Optional[Any] = None
+    Aux: Optional[Any] = None
+
+
+@dataclass
+class CommandOrigin:
+    Origin: int = 0
+    UUID: str = ""
+    RequestID: str = ""
+    PlayerUniqueID: int = 0
+
+
+@dataclass
+class OutputMessage:
+    Success: bool = False
+    Message: str = ""
+    Parameters: Optional[List[Any]] = None
+
+
+@dataclass
+class CommandOutput:
+    CommandOrigin: Optional["CommandOrigin"] = None
+    OutputType: int = 0
+    SuccessCount: int = 0
+    OutputMessages: Optional[List[OutputMessage]] = None
+    DataSet: Optional[Any] = None
+
+    @property
+    def as_dict(self):
+        return _unpack_command_output(self)
+
+
+def unpackCommandOutput(jsonStr: Optional[str]) -> Optional[CommandOutput]:
+    if jsonStr is None:
+        return None
+    commandOutputData = json.loads(jsonStr)
+    commandOrigin = CommandOrigin(**commandOutputData["CommandOrigin"])
+    dataset = None
+    if (
+        "DataSet" in commandOutputData.keys()
+        and commandOutputData["DataSet"] is not None
+        and commandOutputData["DataSet"] != ""
+    ):
+        dataset = json.loads(commandOutputData["DataSet"])
+    outputMessages = []
+    if (
+        "OutputMessages" in commandOutputData.keys()
+        and commandOutputData["OutputMessages"] is not None
+        and commandOutputData["OutputMessages"] != ""
+    ):
+        outputMessagesData = commandOutputData["OutputMessages"]
+        for outputMessageData in outputMessagesData:
+            outputMessage = OutputMessage(
+                Success=outputMessageData["Success"],
+                Message=outputMessageData["Message"],
+            )
+            parameters = []
+            if "Parameters" in outputMessageData.keys():
+                parametersData = outputMessageData["Parameters"]
+                for parameterData in parametersData:
+                    try:
+                        parameters.append(json.loads(parameterData))
+                    except:
+                        parameters.append(parameterData)
+            outputMessage.Parameters = parameters
+            outputMessages.append(outputMessage)
+    return CommandOutput(
+        CommandOrigin=commandOrigin,
+        OutputType=commandOutputData["OutputType"],
+        SuccessCount=commandOutputData["SuccessCount"],
+        OutputMessages=outputMessages,
+        DataSet=dataset,
+    )
+
+
+@dataclass
+class CommandBlockPlaceOption:
+    X: int = 0
+    Y: int = 0
+    Z: int = 0
+    BlockName: str = ""
+    BockState: str = ""
+    NeedRedStone: bool = False
+    Conditional: bool = False
+    Command: str = ""
+    Name: str = ""
+    TickDelay: int = 0
+    ShouldTrackOutput: bool = False
+    ExecuteOnFirstTick: bool = False
+
+
+@dataclass
+class QueriedPlayerPos:
+    dimension: int = 0
+    x: float = 0
+    y: float = 0.0
+    z: float = 0.0
+    yRot: float = 0.0
+
+
+class PlayerKit:
+    def __init__(self, uuid: str, parent: "ThreadOmega") -> None:
+        self.parent = parent
+        self._uuid = uuid
+        self._c_uuid = toCString(self._uuid)
+
+    @property
+    def uuid(self) -> str:
+        return self._uuid
+
+    @property
+    def name(self) -> str:
+        OmegaAvailable()
+        return toPyString(LIB.PlayerName(self._c_uuid))
+
+    @property
+    def entity_unique_id(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerEntityUniqueID(self._c_uuid))
+
+    @property
+    def op(self) -> bool:
+        OmegaAvailable()
+        return LIB.PlayerIsOP(self._c_uuid) == 1
+
+    @property
+    def online(self) -> bool:
+        OmegaAvailable()
+        return LIB.PlayerOnline(self._c_uuid) == 1
+
+    @property
+    def login_time(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerLoginTime(self._c_uuid))
+
+    @property
+    def platform_chat_id(self) -> str:
+        OmegaAvailable()
+        return toPyString(LIB.PlayerPlatformChatID(self._c_uuid))
+
+    @property
+    def build_platform(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerBuildPlatform(self._c_uuid))
+
+    @property
+    def skin_id(self) -> str:
+        OmegaAvailable()
+        return toPyString(LIB.PlayerSkinID(self._c_uuid))
+
+    @property
+    def device_id(self) -> str:
+        OmegaAvailable()
+        return toPyString(LIB.PlayerDeviceID(self._c_uuid))
+
+    @property
+    def properties_flag(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerPropertiesFlag(self._c_uuid))
+
+    @property
+    def command_permission_level(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerCommandPermissionLevel(self._c_uuid))
+
+    @property
+    def action_permissions(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerActionPermissions(self._c_uuid))
+
+    @property
+    def op_permissions_level(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerOPPermissionLevel(self._c_uuid))
+
+    @property
+    def custom_permissions(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerCustomStoredPermissions(self._c_uuid))
+
+    @property
+    def ability_map(self) -> Tuple[ActionPermissionMap, AdventureFlagsMap]:
+        OmegaAvailable()
+        maps = json.loads(toPyString(LIB.PlayerGetAbilityString(self._c_uuid)))
+        ActionPermissionMapData = maps["ActionPermissionMap"]
+        AdventureFlagsMapData = maps["AdventureFlagsMap"]
+        return ActionPermissionMap(**ActionPermissionMapData), AdventureFlagsMap(
+            **AdventureFlagsMapData
         )
-        try:
-            files_to_get = json.loads(
-                requests.get(file_get_src, timeout=30).text)
-        except json.JSONDecodeError:
-            Print.print_err("自动下载缺失文件失败: 文件源 JSON 不合法")
-            return False
-        except requests.Timeout:
-            Print.print_err("自动下载缺失文件失败: URL 请求出现问题: 请求超时")
-            return False
-        except Exception as err:
-            Print.print_err(f"自动下载缺失文件失败: URL 请求出现问题: {err}")
-            return False
-        try:
-            Print.print_with_info("§d正在检测需要补全的文件", "§d 加载 ")
-            mirrs = files_to_get["Mirror"]
-            files = files_to_get[self.system_type]
-            for fdir, furl in files.items():
-                if not os.path.isfile(fdir):
-                    Print.print_inf(f"文件: <{fdir}> 缺失, 正在下载..")
-                    succ = False
-                    for mirr in mirrs:
-                        try:
-                            download_file_singlethreaded(
-                                mirr + "/https://github.com/" + furl, fdir
-                            )
-                            succ = True
-                            break
-                        except requests.exceptions.RequestException:
-                            Print.print_war("镜像源故障, 正在切换")
-                    if not succ:
-                        Print.print_err("镜像源全不可用..")
-                        return False
-                    Print.print_inf(f"文件: <{fdir}> 下载完成        ")
-        except requests.Timeout:
-            Print.print_err("自动检测文件并补全时出现错误: 超时, 自动跳过")
-        except Exception as err:
-            Print.print_err(f"自动检测文件并补全时出现错误: {err}")
-            return False
-        return True
-
-    def init_all_functions(self):
-        def sendcmd(cmd: str, waitForResp: bool = False, timeout: int | float = 30):
-            uuid = fbconn.SendMCCommand(self.con, cmd)
-            if waitForResp:
-                self.cmds_reqs.append(uuid)
-                waitStartTime = time.time()
-                while 1:
-                    res = self.cmds_resp.get(uuid)
-                    if res is not None:
-                        self.cmds_reqs.remove(uuid)
-                        del self.cmds_resp[uuid]
-                        return Packet_CommandOutput(res[1])
-                    if time.time() - waitStartTime > timeout:
-                        self.cmds_reqs.remove(uuid)
-                        Print.print_war(f'sendcmd "{cmd}" 超时, 尝试 sendwscmd')
-                        return self.sendwscmd(cmd, True, timeout)
-
-        def sendwscmd(cmd: str, waitForResp: bool = False, timeout: int = 30):
-            uuid = fbconn.SendWSCommand(self.con, cmd)
-            if waitForResp:
-                self.cmds_reqs.append(uuid)
-                waitStartTime = time.time()
-                while 1:
-                    res = self.cmds_resp.get(uuid)
-                    if res is not None:
-                        self.cmds_reqs.remove(uuid)
-                        del self.cmds_resp[uuid]
-                        return Packet_CommandOutput(res[1])
-                    if time.time() - waitStartTime > timeout:
-                        self.cmds_reqs.remove(uuid)
-                        raise TimeoutError("指令超时")
-            else:
-                return uuid
-
-        self.sendcmd = sendcmd
-        self.sendwscmd = sendwscmd
-        self.sendwocmd = staticmethod(
-            lambda cmd: fbconn.SendNoResponseCommand(self.con, cmd)
+
+    @property
+    def entity_runtime_id(self) -> int:
+        OmegaAvailable()
+        return int(LIB.PlayerEntityRuntimeID(self._c_uuid))
+
+    @property
+    def entity_metadata(self) -> any:
+        OmegaAvailable()
+        return json.loads(toPyString(LIB.PlayerEntityMetadata(self._c_uuid)))
+
+    def query(self, conditions: Union[None, str, List[str]] = None) -> CommandOutput:
+        query_str = f'querytarget @a[name="{self.name}"'
+        if conditions is None:
+            query_str += "]"
+        elif isinstance(conditions, str):
+            query_str += "," + conditions + "]"
+        else:
+            query_str += "," + ",".join(conditions) + "]"
+        ret = self.parent.send_websocket_command_need_response(query_str)
+        return ret
+
+    def check_conditions(self, conditions: Union[None, str, List[str]] = None) -> bool:
+        return self.query(conditions).SuccessCount > 0
+
+    def set_ability_map(
+        self, action_permission: ActionPermissionMap, adventure_flag: AdventureFlagsMap
+    ):
+        jsonFlags = json.dumps(
+            {
+                "AdventureFlagsMap": adventure_flag.__dict__,
+                "ActionPermissionMap": action_permission.__dict__,
+            }
         )
-        self.sendPacket = self.sendPacketJson = staticmethod(
-            lambda pckID, pck: fbconn.SendGamePacketBytes(
-                self.con,
-                fbconn.JsonStrAsIsGamePacketBytes(
-                    pckID, ujson.dumps(pck, ensure_ascii=False)
-                ),
-            )
+        LIB.SetPlayerAbility(self._c_uuid, toCString(jsonFlags))
+
+    def __repr__(self) -> str:
+        return f"uuid={self.uuid},name={self.name},entity_unique_id={self.entity_unique_id},op={self.op},online={self.online}"
+
+    def __del__(self):
+        LIB.ReleaseBindPlayer(toCString(self._uuid))
+
+
+class ConnectType(enum.Enum):
+    Remote = "Remote"  # 连接到一个 neOmega Access Point
+    Local = "Local"  # 在内部启动一个单独的 neOmega Core
+
+
+class ThreadOmega:
+    def __init__(
+        self,
+        connect_type: ConnectType,
+        address: str = "tcp://localhost:24016",
+        accountOption: AccountOptions = None,
+    ) -> None:
+        self._thread_counter = Counter("thread")
+        self._running_threads: Dict[str, Thread] = {}
+        if connect_type == ConnectType.Local:
+            StartOmega(address, accountOption)
+            Print.print_inf(f"Omega 接入点已启动, 在 {address} 开放接口")
+        elif connect_type == ConnectType.Remote:
+            ConnectOmega(address)
+
+        # disconnect event
+        self._omega_disconnected_lock = threading.Event()
+        self._omega_disconnected_lock.clear()  # lock
+        self._omega_disconnected_reason = ""
+
+        # cmd events
+        self._cmd_callback_retriever_counter = Counter("cmd_callback")
+        self._omega_cmd_callback_events: Dict[str, Callable] = {}
+
+        # packet listeners
+        self._packet_listeners: Dict[str, List[Callable[[str, any], None]]] = {}
+
+        # setup actions
+        LIB.ListenAllPackets()  # make LIB listen to all packets and new packets will have eventType="MCPacket"
+        mapping = json.loads(toPyString(LIB.GetPacketNameIDMapping()))
+        self._packet_name_to_id_mapping: dict[str, int] = mapping
+        self._packet_id_to_name_mapping = {}
+        for packet_name, packet_id in self._packet_name_to_id_mapping.items():
+            self._packet_id_to_name_mapping[packet_id] = packet_name
+            self._packet_listeners[packet_name] = []
+
+        LIB.ListenPlayerChange()
+        self._player_change_listeners: List[Callable[[PlayerKit, str], None]] = []
+
+        # get bot basic info (this info will not change so we need to get it only once)
+        self._bot_basic_info = ClientMaintainedBotBasicInfo(
+            **json.loads(toPyString(LIB.GetClientMaintainedBotBasicInfo()))
         )
-        self.sendfbcmd = staticmethod(
-            lambda cmd: fbconn.SendFBCommand(self.con, cmd))
-        self.is_op = None
-
-
-class FrameNeOmg(StandardFrame):
-    # 使用 NeOmega 框架连接到游戏
-    launch_type = "NeOmega"
-
-    def __init__(self, serverNumber, password, fbToken, auth_server):
-        super().__init__(serverNumber, password, fbToken, auth_server)
-        self.status = None
-        self.launch_event = threading.Event()
-        self.injected = False
-        self.omega = None
-        self.TDC = None
-        self.neomg_proc = None
-        self.set_tooldelta_cli()
-        self.download_libs()
-        self.init_all_functions()
-        self.status = SysStatus.LOADING
-        self.secret_exit_key = ""
 
-    def set_omega(self, openat_port):
-        from .neo_libs import neo_conn
+        # player hooks
+        self._bind_players: Dict[str, PlayerKit] = {}
+
+        # named command block msg
+        self._name_command_block_msg_listeners: Dict[
+            str, List[Callable[[Chat], None]]
+        ] = {}
 
-        retries = 0
-        while retries <= 10:
+        # start routine
+        self.start_new(self._react)
+
+    def start_new(self, func: Callable, args: Iterable[Any] = ()):
+        try:
+            thread_i = next(self._thread_counter)
+        except StopIteration:
+            raise ValueError("thread counter overflow")
+
+        def clean_up(*args):
             try:
-                self.omega = neo_conn.ThreadOmega(
-                    connect_type=neo_conn.ConnectType.Remote,
-                    address=f"tcp://localhost:{openat_port}",
-                    accountOption=neo_conn.AccountOptions(
-                        AuthServer=self.auth_server,
-                        UserToken=self.fbToken,
-                        ServerCode=self.serverNumber,
-                        ServerPassword=str(self.serverPassword),
-                    ),
+                func(*args)
+            except Exception:
+                print(traceback.print_exc(limit=None, file=None, chain=True))
+            finally:
+                del self._running_threads[thread_i]
+
+        t = Thread(target=clean_up, args=args)
+        self._running_threads[thread_i] = t
+        t.start()
+
+    def _react(self):
+        while True:
+            eventType, retriever = EventPoll()
+            if eventType == "OmegaConnErr":
+                self._omega_disconnected_reason = toPyString(
+                    LIB.ConsumeOmegaConnError()
                 )
-                retries = 0
-                break
-            except Exception as err:
-                time.sleep(5)
-                retries += 1
-                Print.print_war(f"OMEGA 连接失败, 重连: 第 {retries} 次: {err}")
-                if retries > 5:
-                    Print.print_err("最大重试次数已达到")
-                    raise SystemExit
-
-    def set_tooldelta_cli(self):
-        if type(self) == FrameNeOmg:
-            self.TDC = ToolDeltaCli()
-
-    def start_neomega_proc(self):
-        free_port = get_free_port(24016)
-        access_point_file = (
-            f"neomega_{platform.uname().system.lower()}_access_point_{self.sys_machine}"
-        )
-        if "TERMUX_VERSION" in os.environ:
-            access_point_file = f"neomega_android_access_point_{self.sys_machine}"
-        if platform.system() == "Windows":
-            access_point_file += ".exe"
-        py_file_path = os.path.join(
-            os.getcwd(), "tooldelta", "neo_libs", access_point_file
-        )
-        if platform.uname().system.lower() == "linux":
-            os.system("chmod +x " + shlex.quote(py_file_path))
-        # 只需要+x即可
-        Print.print_inf(f"DEBUG: 将使用端口 {free_port}")
-        self.neomg_proc = subprocess.Popen(
-            [
-                py_file_path,
-                "-server",
-                str(self.serverNumber),
-                "-T",
-                self.fbToken,
-                "-access-point-addr",
-                f"tcp://localhost:{free_port}",
-                "-server-password",
-                str(self.serverPassword),
-                "-auth-server",
-                self.auth_server,
-            ],
-            stdin=subprocess.PIPE,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.STDOUT,
-        )
-        return free_port
+                self._omega_disconnected_lock.set()
+            elif eventType == "CommandResponseCB":
+                cmdResp = unpackCommandOutput(
+                    toPyString(LIB.ConsumeCommandResponseCB())
+                )
+                self._omega_cmd_callback_events[retriever](cmdResp)
+            elif eventType == "MCPacket":
+                packetTypeName = retriever
+                if packetTypeName == "":
+                    print("'', ignored")
+                    # TODO: some bugs
+                listeners = self._packet_listeners.get(packetTypeName, [])
+                if len(listeners) == 0:
+                    LIB.OmitEvent()
+                else:
+                    ret = LIB.ConsumeMCPacket()
+                    if toPyString(ret.convertError) != "":
+                        raise ValueError(toPyString(ret.convertError))
+                    jsonPkt = json.loads(toPyString(ret.packetDataAsJsonStr))
+                    for listener in listeners:
+                        self.start_new(listener, (packetTypeName, jsonPkt))
+            elif eventType == "PlayerChange":
+                playerUUID = retriever
+                if len(self._player_change_listeners) == 0:
+                    LIB.OmitEvent()
+                else:
+                    action = toPyString(LIB.ConsumePlayerChange())
+                    for callback in self._player_change_listeners:
+                        self.start_new(
+                            callback, (self._get_bind_player(playerUUID), action)
+                        )
 
-    def msg_show(self):
-        def _msg_show_thread():
-            while True:
-                msg_orig = self.neomg_proc.stdout.readline().decode("utf-8").strip("\n")
-                if msg_orig in ("", "SIGNAL: exit"):
-                    with Print.lock:
-                        Print.print_with_info(
-                            "ToolDelta: NEOMG 进程已结束", "§b NOMG ")
-                    self.update_status(SysStatus.NORMAL_EXIT)
-                    return
-                if "[neOmega 接入点]: 就绪" in msg_orig:
-                    self.launch_event.set()
-                elif f"STATUS CODE: {self.secret_exit_key}" in msg_orig:
-                    with Print.lock:
-                        Print.print_with_info("§a机器人已退出", "§b NOMG ")
-                    continue
-                with Print.lock:
-                    Print.print_with_info(msg_orig, "§b NOMG ")
-
-        Builtins.createThread(_msg_show_thread, usage="显示来自NeOmega的信息")
-
-    def make_secret_key(self):
-        self.secret_exit_key = hex(random.randint(10000, 99999))
-
-    def launch(self):
-        self.status = SysStatus.LAUNCHING
-        openat_port = self.start_neomega_proc()
-        self.msg_show()
-        self.launch_event.wait()
-        self.make_secret_key()
-        self.set_omega(openat_port)
-        self.update_status(SysStatus.RUNNING)
-        Print.print_suc("已开启接入点进程")
-        pcks = [
-            self.omega.get_packet_id_to_name_mapping(i)
-            for i in self.need_listen_packets
-        ]
-        self.omega.listen_packets(pcks, self.packet_handler_parent)
-        self._launcher_listener()
-        Print.print_suc("接入点已就绪!")
-        self.exit_event.wait()  # 等待事件的触发
-        if self.status == SysStatus.NORMAL_EXIT:
-            return SystemExit("正常退出.")
-        if self.status == SysStatus.CRASHED_EXIT:
-            return Exception("NeOmega 已崩溃")
-        return SystemError("未知的退出状态")
-
-    def download_libs(self):
-        """根据系统架构和平台下载所需的库。"""
-        cfgs = Config.get_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG_STD)
-        is_mir: bool = cfgs["是否使用github镜像"]
-        if is_mir:
-            mirror_src = "https://tdload.tblstudio.cn/" + \
-                "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/"
-            depen_url = "https://tdload.tblstudio.cn/" + \
-                "https://raw.githubusercontent.com/ToolDelta/DependencyLibrary/main/"
-        else:
-            mirror_src = "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/"
-            depen_url = "https://raw.githubusercontent.com/ToolDelta/DependencyLibrary/main/"
-        try:
-            require_depen = json.loads(
-                requests.get(
-                    f"{mirror_src}require_files.json", timeout=5
-                ).text
-            )
-        except Exception as err:
-            Print.print_err(f"获取依赖库表出现问题: {err}")
-            self.update_status(SysStatus.CRASHED_EXIT)
-            return
-        self.sys_machine = platform.machine().lower()
-        if self.sys_machine == "x86_64":
-            self.sys_machine = "amd64"
-        elif self.sys_machine == "aarch64":
-            self.sys_machine = "arm64"
-        if "TERMUX_VERSION" in os.environ:
-            sys_info_fmt: str = f"Android:{self.sys_machine.lower()}"
-        else:
-            sys_info_fmt: str = f"{platform.uname().system}:{self.sys_machine.lower()}"
-        source_dict: list[str] = require_depen[sys_info_fmt]
-        commit_remote = requests.get(
-            f"{depen_url}commit", timeout=5
-        ).text
-        commit_file_path = os.path.join(
-            os.getcwd(), "tooldelta", "neo_libs", "commit")
-        replace_file = False
-        if os.path.isfile(commit_file_path):
-            with open(commit_file_path, "r", encoding="utf-8") as f:
-                commit_local = f.read()
-            if commit_local != commit_remote:
-                Print.print_war("依赖库版本过期, 将重新下载")
-                replace_file = True
-        else:
-            replace_file = True
-        for v in source_dict:
-            pathdir = os.path.join(os.getcwd(), "tooldelta", "neo_libs", v)
-            url = depen_url + v
-            if not os.path.isfile(pathdir) or replace_file:
-                Print.print_with_info(f"正在下载依赖库 {pathdir} ...", "§a 下载 §r")
-                try:
-                    download_file_singlethreaded(url, pathdir)
-                except Exception as err:
-                    Print.print_err(f"下载依赖库出现问题: {err}")
-                    self.update_status(SysStatus.CRASHED_EXIT)
-                    return
-        if replace_file:
-            # 写入commit_remote，文字写入
-            with open(commit_file_path, "w", encoding="utf-8") as f:
-                f.write(commit_remote)
-            Print.print_suc("已完成依赖更新！")
-
-    def get_players_and_uuids(self):
-        players_uuid = {}
-        for i in self.omega.get_all_online_players():
-            players_uuid[i.name] = i.uuid
-        return players_uuid
-
-    def get_bot_name(self):
-        return self.omega.get_bot_name()
-
-    def packet_handler_parent(self, pkt_type, pkt):
-        pkt_type = self.omega.get_packet_name_to_id_mapping(pkt_type)
-        self.packet_handler(pkt_type, pkt)
-
-    def init_all_functions(self):
-        def sendcmd(cmd: str, waitForResp: bool = False, timeout: int | float = 30):
-            if waitForResp:
-                res = self.omega.send_player_command_need_response(
-                    cmd, timeout)
-                if res is None:
-                    raise TimeoutError("指令超时")
-                return res
-            self.omega.send_player_command_omit_response(cmd)
-            return
-
-        def sendwscmd(cmd: str, waitForResp: bool = False, timeout: int = 30):
-            if waitForResp:
-                res = self.omega.send_websocket_command_need_response(
-                    cmd, timeout)
-                if res is None:
-                    raise TimeoutError("指令超时")
-                return res
-            self.omega.send_websocket_command_omit_response(cmd)
-            return
-
-        def sendwocmd(cmd: str):
-            self.omega.send_settings_command(cmd)
-
-        def sendPacket(pktID: int, pkt: str):
-            self.omega.send_game_packet_in_json_as_is(pktID, pkt)
-
-        def sendfbcmd(_):
-            raise AttributeError("NeOmg模式无法发送FBCommand")
-
-        def is_op(player: str):
-            return self.omega.get_player_by_name(player).command_permission_level > 2
-
-        self.sendcmd = sendcmd
-        self.sendwscmd = sendwscmd
-        self.sendwocmd = sendwocmd
-        self.sendPacket = self.sendPacketJson = sendPacket
-        self.sendfbcmd = sendfbcmd
-        self.is_op = is_op
-
-
-class FrameNeOmgRemote(FrameNeOmg):
-    def __init__(self, serverNumber, password, fbToken, auth_server):
-        super().__init__(serverNumber, password, fbToken, auth_server)
+            elif eventType == "PlayerInterceptInput":
+                OmitEvent()
 
-    def launch(self):
-        try:
-            openat_port = int(sys_args_to_dict().get(
-                "access-point-port", "24020"))
-            if openat_port not in range(65536):
-                raise AssertionError
-        except (ValueError, AssertionError):
-            Print.print_err("启动参数 -access-point-port 错误: 不是1~65535的整数")
-        if openat_port == 0:
-            Print.print_war(
-                "未用启动参数指定链接neOmega接入点开放端口, 尝试使用默认端口 24015"
-            )
-            Print.print_inf("可使用启动参数 -access-point-port 端口 以指定接入点端口.")
-            openat_port = 24015
-            return SystemExit
-        Print.print_inf(f"将从端口 {openat_port} 连接至接入点(等待接入中).")
-        self.set_omega(openat_port)
-        Print.print_suc("已连接上接入点进程.")
-        pcks = [
-            self.omega.get_packet_id_to_name_mapping(i)
-            for i in self.need_listen_packets
-        ]
-        self.omega.listen_packets(pcks, self.packet_handler_parent)
-        self._launcher_listener()
-        Print.print_suc("接入点已就绪")
-        self.exit_event.wait()
-        self.update_status(SysStatus.NORMAL_EXIT)
-        if self.status == SysStatus.NORMAL_EXIT:
-            return SystemExit("正常退出.")
-        if self.status == SysStatus.CRASHED_EXIT:
-            return Exception("接入点已崩溃")
-        return SystemError("未知的退出状态")
-
-    def download_libs(self):
-        Print.print_inf("以 Remote 启动, 将不会检查库完整性")
-
-
-class MCBEWebSocket(StandardFrame):
-    def __init__(self, serverNumber, password, fbToken, auth_server):
-        global fcwslib
-        import fcwslib
-        self.ws_lib = fcwslib.server.Server(serverNumber, password)
-        self.ws_lib
-        self.ws_lib.run_forever()
-
-
-class ToolDeltaCli(object):
-    def __init__(self, address: dict = {"host": "tdaus.tooldelta.fit", "port": 0}) -> None:
-        # def __init__(self, address: dict = {"host": "127.0.0.1", "port": 9002}) -> None:
-        self.NoPort: bool = address.get("port", 0) == 0
-        self.S_ADDRESSS: dict = address
-        self.protocol: str = "http"
-        self.url: str = f'{self.protocol}://{self.S_ADDRESSS["host"]}:{self.S_ADDRESSS["port"]}' if self.NoPort == False else f'{self.protocol}://{self.S_ADDRESSS["host"]}'
-        self.SocketIO: socketio.Client = socketio.Client()
-        self.data_received_event: threading.Event = threading.Event()
-        self.connected_to_server: bool = True
-        threading.Thread(target=self.conn_aus, name="SocketIO_Conn").start()
-        while not self.SocketIO.connected and self.connected_to_server:
-            time.sleep(0.1)
-
-    def init_auth_v(self) -> None:
-        self.feature_code: str = str(uuid.uuid5(
-            uuid.NAMESPACE_DNS, str(time.perf_counter())))
-        self.token_ec: tuple = (self.feature_code, self.get_new_token())
+            elif eventType == "Chat":
+                OmitEvent()
 
-    def get_new_token(self) -> None:
-        try:
-            response = requests.post(
-                url=f'{self.url}/api/signin', data=json.dumps({"feature_code": self.feature_code}), timeout=5)
-            if response.status_code == 200:
-                return response.text
-        except requests.exceptions.ConnectionError as err:
-            return "null"
+            elif eventType == "NamedCommandBlockMsg":
+                blockName = retriever
+                listeners = self._name_command_block_msg_listeners[blockName]
+                if len(listeners) == 0:
+                    LIB.OmitEvent()
+                else:
+                    chat = ConsumeChat()
+                    for l in listeners:
+                        self.start_new(l, (chat,))
+
+    def wait_disconnect(self) -> str:
+        """return: disconnect reason"""
+        self._omega_disconnected_lock.wait()
+        return self._omega_disconnected_reason
 
-    def conn_aus(self) -> None:
+    @staticmethod
+    def _create_lock_and_result_setter():
+        lock = threading.Lock()
+        lock.acquire()
+        ret = [None]
+
+        def result_setter(result):
+            ret[0] = result
+            lock.release()
+
+        def result_getter(timeout: float = -1) -> Any:
+            lock.acquire(timeout=timeout)
+            return ret[0]
+
+        return result_setter, result_getter
+
+    def send_websocket_command_need_response(
+        self, cmd: str, timeout: float = -1
+    ) -> Optional[Packet_CommandOutput]:
+        setter, getter = self._create_lock_and_result_setter()
         try:
-            self.init_auth_v()
-            self.SocketIO.connect(
-                self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
-            Print.print_suc("ToolDelta成功连接到至Api服务器[Socket-IO]!")
-            while True:
-                if not self.SocketIO.connected:
-                    try:
-                        self.init_auth_v()
-                        self.SocketIO.connect(
-                            self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
-                        Print.print_suc("ToolDelta与Api服务器断开连接,已重新连接成功!")
-                    except:
-                        Print.print_war(
-                            "ToolDeltaApi服务器可能存在故障或当前网络环境异常，将停止使用ToolDeltaApi服务器!")
-                        break
-                time.sleep(10)
-        except Exception as err:
-            Print.print_war("ToolDelta无法连接至Api服务器,将停止使用其提供的功能!")
-            self.connected_to_server = False
-            threading.Thread(target=self.reconnect_to_server).start()
+            retriever_id = next(self._cmd_callback_retriever_counter)
+        except StopIteration as err:
+            raise ValueError("retriever counter overflow") from err
+        self._omega_cmd_callback_events[retriever_id] = setter
+        SendWebSocketCommandNeedResponse(cmd, retriever_id)
+        res = getter(timeout=timeout)
+        del self._omega_cmd_callback_events[retriever_id]
+        return res
+
+    def send_player_command_need_response(
+        self, cmd: str, timeout: float = -1
+    ) -> Optional[Packet_CommandOutput]:
+        setter, getter = self._create_lock_and_result_setter()
+        try:
+            retriever_id = next(self._cmd_callback_retriever_counter)
+        except StopIteration:
+            raise ValueError("retriever counter overflow")
+        self._omega_cmd_callback_events[retriever_id] = setter
+        SendPlayerCommandNeedResponse(cmd, retriever_id)
+        res = getter(timeout=timeout)
+        del self._omega_cmd_callback_events[retriever_id]
+        return res
+
+    @staticmethod
+    def send_settings_command(cmd: str):
+        SendSettingsCommand(cmd)
+
+    @staticmethod
+    def send_websocket_command_omit_response(cmd: str):
+        SendWebSocketCommandOmitResponse(cmd)
+
+    @staticmethod
+    def send_player_command_omit_response(cmd: str):
+        SendPlayerCommandOmitResponse(cmd)
+
+    def get_packet_name_to_id_mapping(
+        self, requires: Optional[Union[List[str], str]] = None
+    ) -> Union[Dict[str, int], int]:
+        if requires is None:
+            return dict(self._packet_name_to_id_mapping.items())
+        if isinstance(requires, list):
+            return {k: self._packet_name_to_id_mapping[k] for k in requires}
+        return self._packet_name_to_id_mapping[requires]
+
+    def get_packet_id_to_name_mapping(
+        self, requires: Optional[Union[List[int], int]] = None
+    ) -> Union[Dict[int, str], str]:
+        if requires is None:
+            return dict(self._packet_id_to_name_mapping.items())
+        if isinstance(requires, list):
+            return {k: self._packet_id_to_name_mapping[k] for k in requires}
+        return self._packet_id_to_name_mapping[requires]
+
+    def listen_packets(
+        self,
+        targets: Union[str | int, list[Dict[int, str] | str]],
+        callback: Callable[[str, Any], None],
+    ):
+        for k in self._packet_listeners.copy():
+            self._packet_listeners[k].clear()
+        if isinstance(targets, str):
+            targets = [targets]
+        if isinstance(targets, int):
+            targets = [f"{targets}"]
+        res = []
+        for t in targets:
+            if isinstance(t, int):
+                t = self.get_packet_id_to_name_mapping(t)
+            res.append(t)
+        for t in res:
+            self._packet_listeners[t].append(callback)
+
+    def construct_game_packet_bytes_in_json_as_is(
+        self, packet_type: Union[int, str], content: Any
+    ) -> tuple[int, bytes]:
+        if isinstance(packet_type, str):
+            packet_type = self.get_packet_name_to_id_mapping(packet_type)
+        return packet_type, JsonStrAsIsGamePacketBytes(packet_type, json.dumps(content))
+
+    def send_game_packet_in_json_as_is(
+        self, packet_type: Union[int, str], content: Any
+    ):
+        if isinstance(packet_type, str):
+            packet_type = self.get_packet_name_to_id_mapping(packet_type)
+        OmegaAvailable()
+        SendGamePacket(packet_type, json.dumps(content))
+
+    def get_bot_basic_info(self) -> ClientMaintainedBotBasicInfo:
+        return self._bot_basic_info
+
+    def get_bot_name(self) -> str:
+        return self._bot_basic_info.BotName
+
+    def get_bot_runtime_id(self) -> int:
+        return self._bot_basic_info.BotRuntimeID
+
+    def get_bot_unique_id(self) -> int:
+        return self._bot_basic_info.BotUniqueID
+
+    def get_bot_identity(self) -> str:
+        return self._bot_basic_info.BotIdentity
+
+    def get_bot_uuid_str(self) -> str:
+        return self._bot_basic_info.BotUUIDStr
+
+    @staticmethod
+    def get_extend_info() -> ClientMaintainedExtendInfo:
+        OmegaAvailable()
+        return ClientMaintainedExtendInfo(
+            **json.loads(toPyString(LIB.GetClientMaintainedExtendInfo()))
+        )
+
+    def _get_bind_player(self, uuidStr: str) -> Optional[PlayerKit]:
+        if uuidStr is None or uuidStr == "":
+            return None
+        if uuidStr in self._bind_players:
+            return self._bind_players[uuidStr]
+        bind_player = PlayerKit(uuidStr, self)
+        self._bind_players[uuidStr] = bind_player
+        return bind_player
+
+    def get_all_online_players(self):
+        OmegaAvailable()
+        playerUUIDS = json.loads(toPyString(LIB.GetAllOnlinePlayers()))
+        return [self._get_bind_player(uuidStr) for uuidStr in playerUUIDS]
+
+    def get_player_by_name(self, name: str) -> Optional[PlayerKit]:
+        OmegaAvailable()
+        playerUUID = toPyString(LIB.GetPlayerByName(toCString(name)))
+        return self._get_bind_player(playerUUID)
+
+    def get_player_by_uuid(self, uuidStr: str) -> Optional[PlayerKit]:
+        OmegaAvailable()
+        playerUUID = toPyString(LIB.GetPlayerByUUID(toCString(uuidStr)))
+        return self._get_bind_player(playerUUID)
+
+    def listen_player_change(self, callback: Callable[[PlayerKit, str], None]):
+        for player in self.get_all_online_players():
+            callback(player, "exist")
+        self._player_change_listeners.append(callback)
+
+    def listen_named_command_block(
+        self, command_block_name: str, callback: Callable[[Chat], None]
+    ):
+        if command_block_name not in self._name_command_block_msg_listeners:
+            self._name_command_block_msg_listeners[command_block_name] = []
+        LIB.ListenCommandBlock(toCString(command_block_name))
+        self._name_command_block_msg_listeners[command_block_name].append(callback)
+
+    @staticmethod
+    def place_command_block(place_option: CommandBlockPlaceOption):
+        LIB.PlaceCommandBlock(toCString(json.dumps(place_option.__dict__)))
+
+    def __del__(self):
+        for t in self._running_threads.values():
+            t.join()
+
+
+def _unpack_command_output(c: CommandOutput):
+    return {
+        "CommandOrigin": {
+            "Orogin": c.CommandOrigin.Origin,
+            "UUID": c.CommandOrigin.UUID,
+            "RequestID": c.CommandOrigin.RequestID,
+            "PlayerUniqueID": c.CommandOrigin.PlayerUniqueID,
+        },
+        "OutputMessages": [_unpack_output_msgs(i) for i in c.OutputMessages],
+        "OutputType": c.OutputType,
+        "SuccessCOunt": c.SuccessCount,
+        "DataSet": c.DataSet,
+    }
 
-    def reconnect_to_server(self, interval=20):
-        while not self.connected_to_server:
-            try:
-                self.init_auth_v()
-                self.SocketIO.connect(
-                    self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
-                Print.print_suc("ToolDelta成功重新连接至Api服务器!")
-                self.connected_to_server = True
-            except Exception as err:
-                time.sleep(interval)
-
-    def get_depends_table_data(self) -> dict:
-        if self.SocketIO.connected:
-            @self.SocketIO.on('depends_table_data', namespace='/api')
-            def handle_depends_table_data(data):
-                self.data_received_event.set()
-                self.depend_table_data = data
-            self.SocketIO.emit('get_depends_table', namespace='/api')
-            self.data_received_event.wait()  # 等待数据返回
-            self.data_received_event.clear()
-            return self.depend_table_data
-        else:
-            Print.print_war(
-                "Namespace /api is not connected yet. Please wait for connection.")
 
-    def get_version_updates(self) -> any:
-        if self.SocketIO.connected:
-            @self.SocketIO.on('version_updates', namespace='/api')
-            def handle_version_updates_data(data):
-                self.data_received_event.set()
-                self.latest_version_data = data
-
-            self.SocketIO.emit('get_version_update', namespace='/api')
-            self.data_received_event.wait()
-            self.data_received_event.clear()
-            return self.latest_version_data["latest_version_str"]
+def _unpack_output_msgs(c: OutputMessage):
+    return {"Success": c.Success, "Message": c.Message, "Parameters": c.Parameters}
```

### Comparing `tooldelta-0.5.4/tooldelta/launch_options.py` & `tooldelta-0.5.5/tooldelta/launch_options.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,31 @@
+"启动选项"
 import os
-from tooldelta.color_print import Print
-from tooldelta.starter import start_tool_delta
-from tooldelta.plugin_manager import plugin_manager
-from tooldelta.plugin_market import market
-from tooldelta.sys_args import sys_args_to_dict
+import signal
+from .color_print import Print
+from .starter import start_tool_delta
+from .plugin_manager import plugin_manager
+from .plugin_market import market
+from .sys_args import sys_args_to_dict
 
-# TODO: 这是启动界面, 在此方法下写启动选项(启动ToolDelta, 插件管理, 插件市场)
-def client_title():
+
+def signal_handler(*_) -> None:
+    """排除信号中断"""
+    return Print.print_war("ToolDelta 已忽略信号中断")
+
+
+signal.signal(signal.SIGINT, signal_handler)
+
+
+def client_title() -> None:
+    "选择启动模式"
     launch_mode = sys_args_to_dict()
     if launch_mode.get("l"):
+        if not isinstance(launch_mode["l"], str):
+            raise ValueError("启动模式参数不合法")
         r = launch_mode["l"]
     else:
         Print.clean_print("§b请选择启动模式(使用启动参数 -l <启动模式> 可以跳过该页面):")
         Print.clean_print("1 - 启动 ToolDelta")
         Print.clean_print("2 - 打开 ToolDelta 插件管理器")
         Print.clean_print("3 - 打开 ToolDelta 插件市场")
         r = input("请选择:").strip()
```

### Comparing `tooldelta-0.5.4/tooldelta/logger.py` & `tooldelta-0.5.5/tooldelta/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,46 @@
+"日志记录器"
 import os
 import time
 
 
 class ToolDeltaLogger:
+    "ToolDelta的日志记录器"
     INFO = "INFO"
     WARNING = "WARNING"
     ERROR = "ERROR"
     FATAL = "FATAL"
     OTHER_TYPE = "???"
 
     def __init__(self, log_path, name_fmt="%Y-%m-%d"):
+        "初始化"
         self.path = log_path
         self.name_fmt = name_fmt
         self.now_day = time.strftime("%Y-%m-%d")
         self.logging_fmt = "[%H-%M-%S]"
         self.lastLogTime = time.time()
         self.open_wrapper_io(log_path)
         self.enable_logger = False
         self.writable = True
 
-    def switch_logger(self, isopen: bool):
+    def switch_logger(self, isopen: bool) -> None:
+        "切换日志记录器状态"
         self.enable_logger = isopen
 
-    def open_wrapper_io(self, log_path: str):
+    def open_wrapper_io(self, log_path: str) -> None:
+        "打开IO流"
         self._wrapper = open(
             log_path + os.sep + time.strftime(self.name_fmt) + ".log",
             "a",
             encoding="utf-8",
             buffering=4096,
         )
 
-    def log_in(self, msg, level=INFO):
-        # 写入日志信息. level给定了其等级.
+    def log_in(self, msg, level=INFO) -> None:
+        "写入日志信息. level给定了其等级."
         if not self.writable or not self.enable_logger:
             return
         if not isinstance(msg, str):
             raise TypeError("only allows string")
         if "\n" in msg:
             msg = msg.replace("\n", "\n    ")
         if len(msg) > 200:
@@ -46,29 +51,32 @@
             + f" [{level}] "
             + (msg if msg.endswith("\n") else msg + "\n")
         )
         if time.time() - self.lastLogTime > 15:
             self._save_log()
             self.lastLogTime = time.time()
 
-    def _save_log(self):
+    def _save_log(self) -> None:
+        "保存日志"
         self._wrapper.flush()
 
-    def _check_is_another_day(self):
-        # 判断记录日志的时候是否已经是第二天, 是的话就变更文件名.
+    def _check_is_another_day(self) -> None:
+        "判断记录日志的时候是否已经是第二天, 是的话就变更文件名"
         if time.strftime("%Y-%m-%d") != self.now_day:
             self.exit()
             self.open_wrapper_io(self.path)
 
-    def exit(self):
+    def exit(self) -> None:
+        "退出时调用"
         if self.writable:
             self.writable = False
             self._save_log()
             self._wrapper.close()
 
 
-def new_logger(log_path: str):
+def new_logger(log_path: str) -> ToolDeltaLogger:
+    "创建一个新的日志记录器"
     os.makedirs(log_path, exist_ok=True)
     return ToolDeltaLogger(log_path)
 
 
 publicLogger = new_logger("日志文件")
```

### Comparing `tooldelta-0.5.4/tooldelta/packets.py` & `tooldelta-0.5.5/tooldelta/packets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+"构建数据包方便获取"
+
 class PacketIDS:
+    "数据包id"
     Text = 9
     PlayerList = 63
     CommandOutput = 79
 
 
 class SubPacket_CmdOutputMsg:
+    """命令输出消息子包构建"""
     Success: bool
     Message: str
     Parameters: list[str]
 
     def __init__(self, pkt: dict):
         self.Success = pkt["Success"]
         self.Parameters = pkt["Parameters"]
         self.Message = pkt["Message"]
 
 
 class SubPacket_CmdOrigin:
+    "命令来源子包构建"
     Origin: int
     UUID: str
     RequestID: str
     PlayerUniqueID: int
 
     def __init__(self, pkt: dict):
         self.Origin = pkt["Origin"]
         self.UUID = pkt["UUID"]
         self.RequestID = pkt["RequestID"]
         self.PlayerUniqueID = pkt["PlayerUniqueID"]
 
 
 class Packet_CommandOutput:
+    "命令输出包构建"
     CommandOrigin: SubPacket_CmdOrigin
     OutputType: int
     SuccessCount: int
     OutputMessages: list[SubPacket_CmdOutputMsg]
     as_dict: dict
 
     def __init__(self, pkt: dict):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tooldelta-0.5.4/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.5/tooldelta/plugin_load/PluginGroup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,144 +1,178 @@
+"插件管理器"
 import asyncio
-import importlib
-import threading
-import time
 import traceback
-from typing import Any, Callable, Type
+from typing import TYPE_CHECKING, Any, Callable, Union
 
-from tooldelta.color_print import Print
-from tooldelta.plugin_load.classic_plugin import Plugin
-from tooldelta.plugin_load import (
+from ..color_print import Print
+from ..plugin_load.classic_plugin import Plugin
+from ..plugin_load import (
     classic_plugin,
     injected_plugin,
     NON_FUNC,
     NotValidPluginError,
     PluginAPINotFoundError,
     PluginAPIVersionError,
 )
+from ..constants import PRG_NAME
+if TYPE_CHECKING:
+    from ..frame import Frame
+
 
 class PluginGroup:
-    plugins: list[Plugin] = []
+    "插件组"
+    plugins: list[list[str | Plugin]] = []
     plugins_funcs: dict[str, list] = {
         "on_def": [],
         "on_inject": [],
         "on_player_prejoin": [],
         "on_player_join": [],
         "on_player_message": [],
         "on_player_death": [],
         "on_player_leave": [],
     }
     plugin_added_cache = {"plugin": None, "packets": []}
     pluginAPI_added_cache = []
-    _broadcast_evts_cache = {}
+    broadcast_evts_cache = {}
 
     def __init__(self):
+        "初始化"
         self._listen_packet_ids = set()
         self._packet_funcs: dict[str, list[Callable]] = {}
-        self._plugins_api: dict[str, Plugin] = {}
+        self.plugins_api: dict[str, Plugin] = {}
         self._broadcast_listeners: dict[str, list[Callable]] = {}
         self.excType = 0
         self.normal_plugin_loaded_num = 0
         self.injected_plugin_loaded_num = 0
         self.loaded_plugins_name = []
-        self.linked_frame = None
+        self.linked_frame: Union["Frame" , None] = None
+
+    def add_plugin(self, plugin: type[Plugin]) -> type[Plugin]:
+        """添加插件
+
+        Args:
+            plugin (type[Plugin]): 插件主类
+
+        Raises:
+            NotValidPluginError: 插件主类必须继承Plugin类
 
-    def add_plugin(self, plugin: Plugin):
+        Returns:
+            type[Plugin]: 插件主类
+        """
         try:
             if not Plugin.__subclasscheck__(plugin):
                 raise NotValidPluginError(f"插件主类必须继承Plugin类 而不是 {plugin}")
-        except TypeError:
-            if not Plugin.__subclasscheck__(type(plugin)):
-                raise NotValidPluginError(
-                    f"插件主类必须继承Plugin类 而不是 {plugin.__class__.__name__}"
-                )
+        except TypeError as exc:
+            raise NotValidPluginError(
+                f"插件主类必须继承Plugin类 而不是 {plugin.__class__}") from exc
         self.plugin_added_cache["plugin"] = plugin
         self.test_plugin(plugin)
         return plugin
 
-    def add_plugin_as_api(self, apiName: str):
-        def _add_plugin_2_api(api_plugin: Type[Plugin]):
+    def add_plugin_as_api(self, apiName: str) -> Callable[[type[Plugin]], type[Plugin]]:
+        """添加插件作为API
+
+        Args:
+            apiName (str): API名
+
+        Returns:
+            Callable[[type[Plugin]], type[Plugin]]: 添加插件作为API
+        """
+        def _add_plugin_2_api(api_plugin:  type[Plugin]) -> type[Plugin]:
             if not Plugin.__subclasscheck__(api_plugin):
                 raise NotValidPluginError("API插件主类必须继承Plugin类")
             self.plugin_added_cache["plugin"] = api_plugin
             self.pluginAPI_added_cache.append(apiName)
             self.test_plugin(api_plugin)
             return api_plugin
 
         return _add_plugin_2_api
 
-    def add_packet_listener(self, pktID: int | list[int]):
-        """
+    def add_packet_listener(self, pktID: int | list[int]) -> Callable[[Callable], Callable]:
+        """添加数据包监听器
+
         将下面的方法作为一个MC数据包接收器
-        装饰器参数:
-            pktID: int | list[int], 数据包ID或多个ID
-        接收器方法参数:
-            pkt: dict, 数据包包体
+
+        Args:
+            pktID (int | list[int]): 数据包ID或多个ID
+
+        Returns:
+            Callable[[Callable], Callable]: 添加数据包监听器
         """
         def deco(func):
             if isinstance(pktID, int):
                 self.plugin_added_cache["packets"].append((pktID, func))
             else:
                 for i in pktID:
                     self.plugin_added_cache["packets"].append((i, func))
             return func
 
         return deco
 
-    def add_broadcast_listener(self, evt_name: str):
-        """
+    def add_broadcast_listener(self, evt_name: str) -> Callable[[Callable], Callable[[Any], bool]]:
+        """添加广播事件监听器
         将下面的方法作为一个广播事件接收器
-        装饰器参数:
-            evt_name: str, 事件类型
-        传入方法接受参数:
-            data: Any, 若事件带有附加参数, 则会传入附加参数, 否则传入None
-        返回参数: Any(返回的数据, 会被广播事件源收集, 默认None)
+
+        Args:
+            evt_name (str): 事件名
+
+        Returns:
+            Callable[[Callable], Callable]: 添加广播事件监听器
+
         原理:
         方法1 广播: hi, what's ur name? 附加参数=english_only
-            方法2 接收到广播并被执行: 方法2(english_only) -> my name is Super. -> 收集表
+            - 方法2 接收到广播并被执行: 方法2(english_only) -> my name is Super. -> 收集表
+
         事件1 获取到 收集表 作为返回: ["my name is Super."]
         """
 
-        def deco(func: Callable[[Any], bool]):
-            if self._broadcast_evts_cache.get(evt_name):
-                self._broadcast_evts_cache[evt_name].append(func)
+        def deco(func: Callable[[Any], bool]) -> Callable[[Any], bool]:
+            if self.broadcast_evts_cache.get(evt_name):
+                self.broadcast_evts_cache[evt_name].append(func)
             else:
-                self._broadcast_evts_cache[evt_name] = [func]
+                self.broadcast_evts_cache[evt_name] = [func]
             return func
 
         return deco
 
     def broadcastEvt(self, evt_name: str, data: Any = None) -> list[Any] | None:
         """
         向全局广播一个特定事件, 可以传入附加信息参数
-        参数:
-            evt_name: str, 事件名
-            **kwargs: 附加信息参数
-        返回:
-            收集到的数据的列表(如果接收到广播的方法返回了数据的话)
+        Args:
+            evt_name (str): 事件名
+            data (Any, optional): 附加信息参数
+        Returns:
+             list[Any] | None: 收集到的数据的列表(如果接收到广播的方法返回了数据的话)
         """
         callback_list = []
         res = self._broadcast_listeners.get(evt_name)
         if res:
             for f in res:
                 res2 = f(data)
                 if res2:
                     callback_list.append(res2)
         return callback_list
 
-    def test_plugin(self, plugin: type[Plugin]):
+    def test_plugin(self, plugin: type[Plugin]) -> None:
+        """测试插件是否符合要求
+
+        Args:
+            plugin (Plugin): 插件主类
+        """
         if self.linked_frame is None:
             # 很可能是直接单独运行此插件的代码.
             Print.clean_print(f"插件主类信息({plugin.name}): ")
-            Print.clean_print(f" - 作者: {plugin.author}\n - 版本: {plugin.version}")
+            Print.clean_print(
+                f" - 作者: {plugin.author}\n - 版本: {plugin.version}")
             Print.clean_print(
                 f" - 数据包监听: {', '.join(str(i) for i in self._listen_packet_ids)}"
             )
+
     @staticmethod
-    def help(plugin: Plugin):
+    def help(plugin: Plugin) -> None:
         """
         查看插件帮助.
         常用于查看 get_plugin_api() 方法获取到的插件实例的帮助.
         """
         plugin_docs = "<plugins.help>: " + plugin.name + "开放的API接口说明:\n"
         for attr_name, attr in plugin.__dict__.items():
             if not attr_name.startswith("__") and attr.__doc__ is not None:
@@ -147,156 +181,266 @@
                     + attr_name
                     + ":§f\n    "
                     + attr.__doc__.replace("\n", "\n    ")
                 )
         Print.clean_print(plugin_docs)
 
     def checkSystemVersion(self, need_vers: tuple[int, int, int]):
-        """检查ToolDelta系统的最低版本"""
-        if need_vers > self.linked_frame.sys_data.system_version:
+        """检查ToolDelta系统的版本
+
+        Args:
+            need_vers (tuple[int, int, int]): 需要的版本
+
+        Raises:
+            self.linked_frame.SystemVersionException: 该组件需要的ToolDelta系统版本
+        """
+        if self.linked_frame is not None and need_vers > self.linked_frame.sys_data.system_version:
             raise self.linked_frame.SystemVersionException(
-                f"该组件需要{self.linked_frame.PRG_NAME}为{'.'.join([str(i) for i in self.linked_frame.sys_data.system_version])}版本"
+                f"该组件需要{PRG_NAME}为{'.'.join([str(i) for i in self.linked_frame.sys_data.system_version])}版本"
             )
+        elif self.linked_frame is None:
+
+            raise ValueError("无法检查ToolDelta系统版本，请确保已经加载了ToolDelta系统组件")
 
     def get_plugin_api(self, apiName: str, min_version: tuple | None = None) -> Plugin:
+        """获取插件API
+
+        Args:
+            apiName (str): 插件API名
+            min_version (tuple | None, optional): API最低版本(若不填则默认不检查最低版本)
+
+        Raises:
+            PluginAPIVersionError: 插件API版本错误
+            PluginAPINotFoundError: 无法找到API插件
+
+        Returns:
+            Plugin: 插件API
         """
-        通过插件API名获取插件实例
-        参数:
-            apiName: 插件API名
-            min_version: API最低版本(若不填则默认不检查最低版本)
-        """
-        api = self._plugins_api.get(apiName)
+        api = self.plugins_api.get(apiName)
         if api:
             if min_version and api.version < min_version:
                 raise PluginAPIVersionError(apiName, min_version, api.version)
             return api
         raise PluginAPINotFoundError(f"无法找到API插件：{apiName}")
 
-    def set_frame(self, frame):
+    def set_frame(self, frame: "Frame") -> None:
+        "设置关联的框架"
         self.linked_frame = frame
 
-    def read_all_plugins(self):
+    def read_all_plugins(self) -> None:
+        """读取所有插件
+
+        Raises:
+            SystemExit: 读取插件出现问题
+        """
+        if self.linked_frame is None or self.linked_frame.on_plugin_err is None:
+            raise ValueError("无法读取插件，请确保已经加载了ToolDelta系统组件")
         try:
             classic_plugin.read_plugins(self)
             self.execute_def(self.linked_frame.on_plugin_err)
             asyncio.run(injected_plugin.load_plugin(self))
-        except Exception:
+        except Exception as err:
             err_str = "\n".join(traceback.format_exc().split("\n")[1:])
             Print.print_err(f"加载插件出现问题: \n{err_str}")
-            raise SystemExit
+            raise SystemExit from err
 
     @staticmethod
-    def load_plugin_hot(plugin_name: str, plugin_type: str):
+    def load_plugin_hot(plugin_name: str, plugin_type: str) -> None:
+        """热加载插件
+
+        Args:
+            plugin_name (str): 插件名
+            plugin_type (str): 插件类型
+        """
         plugin = None
         if plugin_type == "classic":
-            plugin = classic_plugin.load_plugin(plugin_name, True)
+            plugin = classic_plugin.load_plugin(plugin_name)
         elif plugin_type == "injected":
             asyncio.run(injected_plugin.load_plugin_file(plugin_name))
-        if plugin is not None:
-            plugin.on_def()
+        # 检查是否有on_def成员再执行
+        if plugin and hasattr(plugin, "on_def"):
+            plugin.on_def() # type: ignore
         Print.print_suc(f"成功热加载插件: {plugin_name}")
 
-    def _add_listen_packet_id(self, packetType: int):
+    def add_listen_packet_id(self, packetType: int) -> None:
+        """添加数据包监听
+
+        Args:
+            packetType (int): 数据包ID
+
+        Raises:
+            ValueError: 无法添加数据包监听，请确保已经加载了系统组件
+        """
+        if self.linked_frame is None:
+            raise ValueError("无法添加数据包监听，请确保已经加载了系统组件")
         self._listen_packet_ids.add(packetType)
         self.linked_frame.link_game_ctrl.add_listen_pkt(packetType)
 
-    def _add_listen_packet_func(self, packetType, func: Callable):
+    def add_listen_packet_func(self, packetType: int, func: Callable) -> None:
+        """添加数据包监听器
+
+        Args:
+            packetType (int): 数据包ID
+            func (Callable): 数据包监听器
+        """
         if self._packet_funcs.get(str(packetType)):
             self._packet_funcs[str(packetType)].append(func)
         else:
             self._packet_funcs[str(packetType)] = [func]
 
-    def _add_broadcast_evt(self, evt, func):
+    def add_broadcast_evt(self, evt: str, func: Callable) -> None:
+        """添加广播事件监听器
+
+        Args:
+            evt (str): 事件名
+            func (Callable): 事件监听器
+        """
         if self._broadcast_listeners.get(evt):
             self._broadcast_listeners[evt].append(func)
         else:
             self._broadcast_listeners[evt] = [func]
 
-    def execute_def(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC):
+    def execute_def(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC) -> None:
+        """执行插件的初始化方法
+
+        Args:
+            onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法. Defaults to NON_FUNC.
+
+        Raises:
+            SystemExit: 缺少前置
+            SystemExit: 前置版本过低
+        """
         for name, func in self.plugins_funcs["on_def"]:
             try:
                 func()
             except PluginAPINotFoundError as err:
                 Print.print_err(f"插件 {name} 需要包含该种接口的前置组件: {err.name}")
-                raise SystemExit
+                raise SystemExit from err
             except PluginAPIVersionError as err:
                 Print.print_err(
                     f"插件 {name} 需要该前置组件 {err.name} 版本: {err.m_ver}, 但是现有版本过低: {err.n_ver}"
                 )
-                raise SystemExit
+                raise SystemExit from err
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
-    def execute_init(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC):
+    def execute_init(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC) -> None:
+        """执行插件的初始化方法
+
+        Args:
+            onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
+        """
         for name, func in self.plugins_funcs["on_inject"]:
             try:
                 func()
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
     def execute_player_prejoin(
         self, player, onerr: Callable[[str, Exception, str], None] = NON_FUNC
-    ):
+    ) -> None:
+        """执行玩家加入前的方法
+
+        Args:
+            player (_type_): 玩家
+            onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
+        """
         for name, func in self.plugins_funcs["on_player_prejoin"]:
             try:
                 func(player)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
     def execute_player_join(
-        self, player, onerr: Callable[[str, Exception, str], None] = NON_FUNC
-    ):
+        self, player: str, onerr: Callable[[str, Exception, str], None] = NON_FUNC
+    ) -> None:
+        """执行玩家加入的方法
+
+        Args:
+            player (str): 玩家
+            onerr (Callable[[str, Exception, str], None], optional): q 插件出错时的处理方法
+        """
         for name, func in self.plugins_funcs["on_player_join"]:
             try:
                 func(player)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
     def execute_player_message(
-        self, player, msg, onerr: Callable[[str, Exception, str], None] = NON_FUNC
-    ):
+        self, player: str, msg: str, onerr: Callable[[str, Exception, str], None] = NON_FUNC
+    ) -> None:
+        """执行玩家消息的方法
+
+        Args:
+            player (str): 玩家
+            msg (str): 消息
+            onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
+        """
         pat = f"[{player}] "
         if msg.startswith(pat):
             msg = msg.strip(pat)
         for name, func in self.plugins_funcs["on_player_message"]:
             try:
                 func(player, msg)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
     def execute_player_leave(
-        self, player, onerr: Callable[[str, Exception, str], None] = NON_FUNC
-    ):
+        self, player: str, onerr: Callable[[str, Exception, str], None] = NON_FUNC
+    ) -> None:
+        """执行玩家离开的方法
+
+        Args:
+            player (str): 玩家
+            onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
+        """
         for name, func in self.plugins_funcs["on_player_leave"]:
             try:
                 func(player)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
     def execute_player_death(
         self,
         player: str,
         killer: str | None,
         msg: str,
         onerr: Callable[[str, Exception, str], None] = NON_FUNC,
     ):
+        """
+
+        Args:
+            player (str): 玩家
+            killer (str | None): 击杀者
+            msg (str): 消息
+            onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
+        """
         for name, func in self.plugins_funcs["on_player_death"]:
             try:
                 func(player, killer, msg)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
-    def processPacketFunc(self, pktID: int, pkt: dict):
+    def processPacketFunc(self, pktID: int, pkt: dict) -> bool:
+        """处理数据包监听器
+
+        Args:
+            pktID (int): 数据包ID
+            pkt (dict): 数据包
+
+        Returns:
+            bool: 是否处理成功
+        """
         d = self._packet_funcs.get(str(pktID))
         if d:
             for func in d:
                 try:
                     res = func(pkt)
                     if res:
                         return True
-                except:
+                except Exception:
                     Print.print_err(f"插件方法 {func.__name__} 出错：")
                     Print.print_err(traceback.format_exc())
         return False
 
 
 plugin_group = PluginGroup()
```

### Comparing `tooldelta-0.5.4/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.5/tooldelta/plugin_load/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,53 @@
-NON_FUNC = lambda *_: None
+"插件加载主模块"
+
+from typing import Any
+
+
+def NON_FUNC(*_) -> None:
+    "空函数"
+    return None
 
 
 class PluginSkip(EOFError):
-    ...
+    "跳过插件加载"
+
 
 class NotValidPluginError(AssertionError):
-    # 仅加载插件时引发, 不是合法插件的报错
-    ...
+    "仅加载插件时引发, 不是合法插件的报错"
+
 
 class PluginAPINotFoundError(ModuleNotFoundError):
+    "插件API未找到错误"
+
     def __init__(self, name):
         self.name = name
 
+
 class PluginAPIVersionError(ModuleNotFoundError):
+    "插件API版本错误"
+
     def __init__(self, name, m_ver, n_ver):
         self.name = name
         self.m_ver = m_ver
         self.n_ver = n_ver
 
+
 class PluginRegData:
-    # 插件注册信息类
-    def __init__(self, name: str, plugin_data: dict = None, is_registered=True, is_enabled=True):
+    "插件注册数据"
+
+    def __init__(self, name: str, plugin_data: dict | None = None, is_registered=True, is_enabled=True):
+        """插件注册数据
+
+        Args:
+            name (str): 插件名
+            plugin_data (dict | None, optional): 插件数据
+            is_registered (bool, optional): 是否已注册
+            is_enabled (bool, optional): 是否启用
+        """
         if plugin_data is None:
             plugin_data = {}
         self.name: str = name
         if isinstance(plugin_data.get("version"), str):
             self.version: tuple = tuple(
                 int(i) for i in plugin_data.get("version", "0.0.0").split(".")
             )
@@ -38,32 +61,52 @@
         self.plugin_id = plugin_data.get("plugin-id", "???")
         self.is_registered = is_registered
         if plugin_data.get("enabled") is not None:
             self.is_enabled = plugin_data["enabled"]
         else:
             self.is_enabled = is_enabled
 
-    def dump(self):
+    def dump(self) -> dict[str, Any]:
+        "转储数据"
         return {
             "author": self.author,
             "version": ".".join([str(i) for i in self.version]),
             "plugin-type": self.plugin_type,
             "description": self.description,
             "pre-plugins": self.pre_plugins,
             "plugin-id": self.plugin_id,
             "enabled": self.is_enabled
         }
 
     @property
-    def version_str(self):
+    def version_str(self) -> str:
+        """版本字符串
+
+        Returns:
+            str: 版本字符串
+        """
         return ".".join(str(i) for i in self.version)
 
     @property
-    def plugin_type_str(self):
+    def plugin_type_str(self) -> str:
+        """插件类型字符串
+
+        Returns:
+            str: 插件类型字符串
+        """
         return {
             "classic": "主类式",
             "injected": "注入式",
             "unknown": "未知类型",
         }.get(self.plugin_type, "未知类型")
 
-def plugin_is_enabled(pname: str):
+
+def plugin_is_enabled(pname: str) -> bool:
+    """插件是否启用
+
+    Args:
+        pname (str): 插件名
+
+    Returns:
+        bool: 是否启用
+    """
     return not pname.endswith("+disabled")
```

### Comparing `tooldelta-0.5.4/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.5.5/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,61 @@
+"ToolDelta类式插件"
 import importlib
 import os
 import sys
 import traceback
-import typing
-from tooldelta.color_print import Print
-from tooldelta.builtins import Builtins
-from tooldelta.cfg import Cfg
-from tooldelta.plugin_load.funcs import unzip_plugin
-from tooldelta.plugin_load import plugin_is_enabled, NotValidPluginError
-from tooldelta.constants import TOOLDELTA_CLASSIC_PLUGIN
-
-if typing.TYPE_CHECKING:
-    # define Frame
-    from tooldelta.frame import Frame
-    from tooldelta.plugin_load.PluginGroup import PluginGroup
+from typing import TYPE_CHECKING, Callable, Union
+from ...color_print import Print
+from ...builtins import Builtins
+from ...cfg import Cfg
+from ...plugin_load.funcs import unzip_plugin
+from ...plugin_load import plugin_is_enabled, NotValidPluginError
+from ...constants import TOOLDELTA_CLASSIC_PLUGIN
+
+if TYPE_CHECKING:
+    # 类型注释
+    from ...frame import Frame
+    from ...plugin_load.PluginGroup import PluginGroup
 
 
 class Plugin:
+    "插件信息主类"
     name: str = ""
     version = (0, 0, 1)
     author = "?"
     description = "..."
 
     def __init__(self, frame: "Frame"):
         self.frame = frame
         self.game_ctrl = frame.get_game_control()
 
     @property
     def data_path(self) -> str:
+        "数据路径"
         return os.path.join("插件数据文件", self.name)
 
 
-plugin_group_cache:list["PluginGroup"] = [None]
+plugin_group_cache: list[Union["PluginGroup", None]] = [None]
 
 
-def read_plugins(plugin_grp: "PluginGroup"):
+def read_plugins(plugin_grp: "PluginGroup") -> None:
+    """读取插件
+
+    Args:
+        plugin_grp (PluginGroup): 插件组
+    """
     plugin_group_cache[0] = plugin_grp
     PLUGIN_PATH = os.path.join("插件文件", TOOLDELTA_CLASSIC_PLUGIN)
     sys.path.append(os.path.join("插件文件", TOOLDELTA_CLASSIC_PLUGIN))
     for plugin_dir in os.listdir(PLUGIN_PATH):
         if not plugin_is_enabled(plugin_dir):
             continue
         if (
-            not os.path.isdir(os.path.join(PLUGIN_PATH, plugin_dir.strip(".zip")))
+            not os.path.isdir(os.path.join(
+                PLUGIN_PATH, plugin_dir.strip(".zip")))
             and os.path.isfile(os.path.join(PLUGIN_PATH, plugin_dir))
             and plugin_dir.endswith(".zip")
         ):
             Print.print_with_info(f"§6正在解压插件{plugin_dir}, 请稍后", "§6 解压 ")
             unzip_plugin(
                 os.path.join(PLUGIN_PATH, plugin_dir),
                 os.path.join(PLUGIN_PATH, plugin_dir.strip(".zip")),
@@ -55,16 +64,39 @@
             plugin_dir = plugin_dir.strip(".zip")
         if os.path.isdir(os.path.join(PLUGIN_PATH, plugin_dir)):
             sys.path.append(os.path.join(PLUGIN_PATH, plugin_dir))
             load_plugin(plugin_dir)
             plugin_grp.loaded_plugins_name.append(plugin_dir)
 
 
-def load_plugin(plugin_dirname: str, hot_load=False):
+def load_plugin(plugin_dirname: str) -> Union[None, Plugin]:
+    """加载插件
+
+    Args:
+        plugin_dirname (str): 插件目录名
+        hot_load (bool, optional): 是否热加载
+
+    Raises:
+        ValueError: 插件组未初始化读取
+        ValueError: 插件组未绑定框架
+        ValueError: 插件主类需要作者名
+        ValueError: 插件主类需要作者名
+        NotValidPluginError: 插件 不合法
+        SystemExit: 插件名字不合法
+        SystemExit: 插件配置文件报错
+        SystemExit: 插件读取数据失败
+
+    Returns:
+        Union[None, Plugin]: 插件实例
+    """
     plugin_grp = plugin_group_cache[0]
+    if isinstance(plugin_grp, type(None)):
+        raise ValueError("插件组未初始化读取")
+    if isinstance(plugin_grp.linked_frame, type(None)):
+        raise ValueError("插件组未绑定框架")
     try:
         if os.path.isfile(
             os.path.join(
                 "插件文件", TOOLDELTA_CLASSIC_PLUGIN, plugin_dirname, "__init__.py"
             )
         ):
             importlib.__import__(plugin_dirname)
@@ -77,14 +109,16 @@
                 "需要调用1次 @plugins.add_plugin 以注册插件主类, 然而没有调用"
             ),
         )
         plugin: type[Plugin] = plugin_grp.plugin_added_cache["plugin"]
         if plugin.name is None:
             raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
         plugin_ins = plugin(plugin_grp.linked_frame)
+        if isinstance(plugin_ins, type(None)) or plugin_ins.name is "":
+            raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
         plugin_grp.plugins.append([plugin_ins.name, plugin_ins])
         _v0, _v1, _v2 = plugin_ins.version
         for evt_name in (
             "on_def",
             "on_inject",
             "on_player_prejoin",
             "on_player_join",
@@ -97,52 +131,53 @@
                     [plugin_ins.name, getattr(plugin_ins, evt_name)]
                 )
         Print.print_suc(
             f"成功载入插件 {plugin_ins.name} 版本: {_v0}.{_v1}.{_v2} 作者：{plugin_ins.author}"
         )
         plugin_grp.normal_plugin_loaded_num += 1
         if plugin_grp.plugin_added_cache["packets"] != []:
-            for pktType, func in plugin_grp.plugin_added_cache["packets"]:  # type: ignore
+            for pktType, func in plugin_grp.plugin_added_cache["packets"]:
                 pfunc = getattr(plugin_ins, func.__name__)
                 if pfunc is None:
                     raise NotValidPluginError("数据包监听不能在主插件类以外定义")
-                plugin_grp._add_listen_packet_id(pktType)
-                plugin_grp._add_listen_packet_func(
+                plugin_grp.add_listen_packet_id(pktType)
+                plugin_grp.add_listen_packet_func(
                     pktType, pfunc
                 )
         if plugin_grp.pluginAPI_added_cache is not None:
             for _api in plugin_grp.pluginAPI_added_cache:
                 if isinstance(_api, str):
-                    plugin_grp._plugins_api[_api] = plugin_ins
+                    plugin_grp.plugins_api[_api] = plugin_ins
                 else:
                     (apiName, api) = _api
-                    plugin_grp._plugins_api[apiName] = api(plugin_grp.linked_frame)
-        if plugin_grp._broadcast_evts_cache != {}:
-            for evt, funcs in plugin_grp._broadcast_evts_cache.items():
+                    plugin_grp.plugins_api[apiName] = api(
+                        plugin_grp.linked_frame)
+        if plugin_grp.broadcast_evts_cache != {}:
+            for evt, funcs in plugin_grp.broadcast_evts_cache.items():
                 for func in funcs:
                     bfunc = getattr(plugin_ins, func.__name__)
                     if bfunc is not None:
                         # 在插件主类以内定义了广播接收器
                         func = bfunc
-                    plugin_grp._add_broadcast_evt(evt, func)
+                    plugin_grp.add_broadcast_evt(evt, func)
         return plugin_ins
     except NotValidPluginError as err:
         Print.print_err(f"插件 {plugin_dirname} 不合法: {err.args[0]}")
-        raise SystemExit
+        raise SystemExit from err
     except Cfg.ConfigError as err:
         Print.print_err(f"插件 {plugin_dirname} 配置文件报错：{err}")
         Print.print_err("你也可以直接删除配置文件, 重新启动ToolDelta以自动生成配置文件")
-        raise SystemExit
+        raise SystemExit from err
     except Builtins.SimpleJsonDataReader.DataReadError as err:
         Print.print_err(f"插件 {plugin_dirname} 读取数据失败: {err}")
-    except plugin_grp.linked_frame.SystemVersionException:
+    except plugin_grp.linked_frame.SystemVersionException as err:
         Print.print_err(f"插件 {plugin_dirname} 需要更高版本的ToolDelta加载: {err}")
     except Exception as err:
         Print.print_err(f"加载插件 {plugin_dirname} 出现问题, 报错如下: ")
         Print.print_err("§c" + traceback.format_exc())
-        raise SystemExit
+        raise SystemExit from err
     finally:
         plugin_grp.plugin_added_cache["plugin"] = None
         plugin_grp.plugin_added_cache["packets"].clear()
         plugin_grp.pluginAPI_added_cache.clear()
-        plugin_grp._broadcast_evts_cache.clear()
+        plugin_grp.broadcast_evts_cache.clear()
     return None
```

### Comparing `tooldelta-0.5.4/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.5/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+"注入式执行函数"
 import time
-import ujson as json
-from typing import TYPE_CHECKING, Any
-from typing import Optional
+from typing import TYPE_CHECKING, Any, Optional
 from tooldelta.color_print import Print
 from tooldelta.packets import Packet_CommandOutput
 if TYPE_CHECKING:
     from tooldelta.frame import Frame, GameCtrl
 
 
 def check_avaliable(sth: "GameCtrl") -> Optional[AttributeError]:
@@ -24,15 +23,15 @@
 
 
 def set_frame(my_Frame: "Frame") -> None:
     """
     全局初始化框架
 
     参数:
-        my_"Frame": 要设置的框架对象
+        my_Frame: 要设置的框架对象
     """
     global movent_frame, game_control  # pylint: disable=global-statement
     movent_frame = my_Frame
     game_control = my_Frame.get_game_control()
 
 
 def sendcmd(
@@ -43,22 +42,20 @@
 
     参数:
         cmd: 要发送的命令
         waitForResp: 是否等待响应,默认为 False
         timeout: 等待响应的超时时间（秒）,默认为 30
     """
     check_avaliable(game_control)
-    if game_control.sendcmd is None:
-        raise AttributeError(f"无法使用 {game_control.__class__.__name__}, 因为其还未被初始化")
     return game_control.sendcmd(cmd, waitForResp, timeout)
 
 
 def sendwscmd(
-    cmd: str, waitForResp: bool = False, timeout: int | float = 30
-) -> Packet_CommandOutput:
+    cmd: str, waitForResp: bool = False, timeout: float = 30
+) -> Packet_CommandOutput | None:
     """
     发送WSCMD命令到游戏控制器
 
     参数:
         cmd: 要发送的WSCMD命令
         waitForResp: 是否等待响应 默认为False
         timeout: 超时时间（秒） 默认为30
@@ -86,47 +83,38 @@
         pktID: 数据包ID
         pkt: 数据包内容
     """
     check_avaliable(game_control)
     game_control.sendPacket(pktID, pkt)
 
 
-def sendfbcmd(cmd: str) -> None:
-    """向FastBuilder发送命令\n
-    在除FastBuilder外的其他启动器上不可用
-
-    参数:
-        cmd: 要发送的命令。
-    """
-    check_avaliable(game_control)
-    game_control.sendfbcmd(cmd)
-
-
 def rawText(playername: str, text: str) -> None:
     """
     向指定玩家发送原始文本消息
 
     参数:
         playername: 玩家名称
         text: 要发送的文本
     """
-    sendcmd(r"""/tellraw %s {"rawtext":[{"text":"%s"}]}""" % (playername, text))
+    sendcmd(
+        r"""/tellraw %s {"rawtext":[{"text":"%s"}]}""" % (playername, text))
 
 
 def tellrawText(playername: str, title: str | None = None, text: str = "") -> None:
     """
     向指定玩家发送tellraw消息
 
     参数:
         playername: 玩家名称
         title: 标题文本（可选）
         text: 消息文本
     """
     if title is None:
-        sendcmd(r"""/tellraw %s {"rawtext":[{"text":"§r%s"}]}""" % (playername, text))
+        sendcmd(
+            r"""/tellraw %s {"rawtext":[{"text":"§r%s"}]}""" % (playername, text))
     else:
         sendcmd(
             r"""/tellraw %s {"rawtext":[{"text":"<%s> §r%s"}]}"""
             % (
                 playername,
                 title,
                 text,
@@ -161,24 +149,27 @@
 
     参数:
         sth: 目标选择器
         timeout: 超时时间，默认为5秒
     """
     check_avaliable(game_control)
     if not sth.startswith("@"):
-        raise Exception("Minecraft Target Selector is not correct.")
+        raise ValueError("Minecraft Target Selector is not correct.")
+    result = sendwscmd(f"/testfor {sth}", True, timeout)
+    if result is None:
+        raise ValueError("Failed to get the target.")
     result = (
-        game_control.sendwscmd(f"/testfor {sth}", True, timeout)
+        result
         .OutputMessages[0]
         .Parameters
     )
     if result:
         result = result[0]
         return result.split(", ")
-    return []
+    raise ValueError("Failed to get the target.")
 
 
 def find_key_from_value(dic: dict, val: Any) -> Optional[Any]:
     """
     从字典中根据值查找对应的键
 
     参数:
@@ -207,22 +198,24 @@
         ValueError: 当目标玩家不存在时抛出该异常
         ValueError: 当获取位置信息失败时抛出该异常
         AttributeError: 当获取玩家UUID失败时抛出该异常
     """
     check_avaliable(game_control)
     if targetNameToGet not in get_all_player() or targetNameToGet.startswith("@"):
         raise ValueError(f"Player {targetNameToGet} does not exist.")
-    result = sendwscmd(f'/querytarget @a[name="{targetNameToGet}"]', True, timeout)
+    result = sendwscmd(
+        f'/querytarget @a[name="{targetNameToGet}"]', True, timeout)
+    if isinstance(result, type(None)):
+        raise ValueError("Failed to get the position.")
     if not result.OutputMessages[0].Success:
-        raise ValueError(f"Failed to get the position: {result.OutputMessages[0]}")
+        raise ValueError(
+            f"Failed to get the position: {result.OutputMessages[0]}")
     parameter = result.OutputMessages[0].Parameters[0]
     if isinstance(parameter, str):
-        resultList = json.loads(parameter)
-    else:
-        resultList = parameter
+        raise ValueError("Failed to get the position.")
     result = {}
 
     if game_control.players_uuid is None:
         raise AttributeError("Failed to get the players_uuid.")
     targetName = targetNameToGet
     x = (
         parameter[0]["position"]["x"]
@@ -284,14 +277,16 @@
 
     参数:
         x: X坐标
         y: Y坐标
         z: Z坐标
     """
     res = sendwscmd(f"/testforblock {x} {y} {z} air", True)
+    if isinstance(res, type(None)):
+        raise ValueError("Failed to get the block.")
     if res.SuccessCount:
         return "air"
     return res.OutputMessages[0].Parameters[4].strip("%tile.").strip(".name")
 
 
 def getTickingAreaList() -> dict | AttributeError:
     """
```

### Comparing `tooldelta-0.5.4/tooldelta/plugin_market.py` & `tooldelta-0.5.5/tooldelta/plugin_market.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,124 @@
-import requests
-import json
+"插件商店生成与操作"
 import os
 import platform
 import shutil
 import tempfile
 import traceback
 import time
 import shlex
+import requests
+import ujson as json
 from tooldelta import urlmethod
-from tooldelta.builtins import Builtins
-from tooldelta.color_print import Print
-from tooldelta.plugin_load import PluginRegData
-from tooldelta.cfg import Cfg
-from tooldelta.constants import (
+from .builtins import Builtins
+from .color_print import Print
+from .plugin_load import PluginRegData
+from .cfg import Cfg
+from .constants import (
     PLUGIN_MARKET_SOURCE_OFFICIAL,
     TOOLDELTA_CLASSIC_PLUGIN,
     TOOLDELTA_INJECTED_PLUGIN
 )
+from .plugin_load.PluginGroup import plugin_group
 
 if platform.system().lower() == "windows":
     CLS_CMD = "cls"
 else:
     CLS_CMD = "clear"
 
-clear_screen = lambda: os.system(shlex.quote(CLS_CMD))
 
+def clear_screen() -> None:
+    "清屏"
+    os.system(shlex.quote(CLS_CMD))
+
+
+def path_dir(path: str) -> str | None:
+    """获取路径的上一级目录
 
-def _path_dir(path: str):
+    Args:
+        path (str): 路径
+
+    Returns:
+        str|None: 上一级目录
+    """
     if "/" not in path:
         return None
     return "/".join(path.split("/")[:-1])
 
 
-def _url_join(*urls):
+def url_join(*urls) -> str:
+    """连接URL
+
+    Returns:
+        str: 连接后的URL
+    """
     return "/".join(urls)
 
 
-def _get_json_from_url(url: str):
+def get_json_from_url(url: str) -> dict:
+    """从URL获取JSON数据
+
+    Args:
+        url (str): URL
+
+    Raises:
+        requests.RequestException: Url请求失败
+        requests.RequestException: 服务器返回了不正确的答复
+
+    Returns:
+        dict: JSON数据
+    """
     try:
-        resp = requests.get(url)
+        resp = requests.get(url, timeout=5)
         resp.raise_for_status()
         resptext = resp.text
-    except requests.RequestException:
-        raise Exception("URL请求失败")
+    except requests.RequestException as exc:
+        raise requests.RequestException("URL请求失败") from exc
     try:
         return json.loads(resptext)
-    except json.JSONDecodeError:
-        raise Exception(f"服务器返回了不正确的答复: {resptext}")
+    except json.JSONDecodeError as exc:
+        raise requests.RequestException(f"服务器返回了不正确的答复: {resptext}") from exc
 
 
 class PluginMarket:
-    plugin_id_name_map = None
-    def enter_plugin_market(self, source_url: str = None, in_game = False):
+    "插件市场类"
+
+    def __init__(self):
+        try:
+            self.plugins_download_url = Cfg().get_cfg(
+                "ToolDelta基本配置.json", {"插件市场源": str})["插件市场源"]
+        except Exception:
+            self.plugins_download_url = PLUGIN_MARKET_SOURCE_OFFICIAL
+        self.plugin_id_name_map: dict = self.get_plugin_id_name_map()
+
+    def enter_plugin_market(self, source_url: str | None = None, in_game=False) -> None:
+        """进入插件市场
+
+        Args:
+            source_url (str | None, optional): 插件市场源
+            in_game (bool, optional): 是否在游戏内
+        """
         Print.clean_print("§6正在连接到插件市场..")
         CTXS = 12
         try:
-            market_datas = self.get_datas_from_market(source_url)
-            plugin_ids_map = self.get_plugin_id_name_map()
+            if isinstance(source_url, str):
+                market_datas = self.get_datas_from_market(source_url)
+            market_datas = self.get_datas_from_market()
+            plugin_ids_map = self.plugin_id_name_map
             plugins_list = list(market_datas["MarketPlugins"].items())
             all_indexes = len(plugins_list)
             now_index = 0
             sum_pages = int((all_indexes - 1) / CTXS) + 1
             now_page = 0
             last_operation = ""
             while True:
                 clear_screen()
                 Print.print_inf(
-                    market_datas["SourceName"] + ": " + market_datas["Greetings"],
+                    market_datas["SourceName"] + ": " +
+                    market_datas["Greetings"],
                     need_log=False
                 )
                 now_page = int(now_index / CTXS) + 1
                 for i in range(now_index, now_index + CTXS):
                     if i in range(all_indexes):
                         plugin_id = plugins_list[i][0]
                         plugin_name = plugin_ids_map[plugin_id]
@@ -83,19 +131,21 @@
                             plugin_type = plugin_basic_datas['plugin-type']
                         Print.print_inf(
                             f" {i + 1}. §e{plugin_name} §av{plugin_basic_datas['version']} §b@{plugin_basic_datas['author']} §d{plugin_type}插件",
                             need_log=False
                         )
                     else:
                         Print.print_inf("")
-                Print.print_inf(f"§f第 {now_page} / {sum_pages} 页, 输入 §b+§f/§b- §f翻页", need_log=False)
+                Print.print_inf(
+                    f"§f第 {now_page} / {sum_pages} 页, 输入 §b+§f/§b- §f翻页", need_log=False)
                 Print.print_inf("§f输入插件序号选中插件并查看其下载页", need_log=False)
                 last_operation = (
                     (
-                        input(Print.fmt_info("§f回车键继续上次操作, §bq§f退出, 请输入:", "§f 输入 "))
+                        input(Print.fmt_info(
+                            "§f回车键继续上次操作, §bq§f退出, 请输入:", "§f 输入 "))
                         or last_operation
                     )
                     .lower()
                     .strip()
                 )
                 if last_operation == "+":
                     now_index += CTXS
@@ -103,36 +153,43 @@
                     now_index -= CTXS
                 elif last_operation == "q":
                     break
                 else:
                     res = Builtins.try_int(last_operation)
                     if res:
                         if res in range(1, all_indexes + 1):
-                            plugin_data = self.get_plugin_data_from_market(plugins_list[res - 1][0])
+                            plugin_data = self.get_plugin_data_from_market(
+                                plugins_list[res - 1][0])
                             ok, pres = self.choice_plugin(plugin_data)
                             if ok:
                                 if in_game:
-                                    from tooldelta.plugin_load.PluginGroup import plugin_group
                                     if plugin_data.name not in plugin_group.loaded_plugins_name:
                                         resp = input(
-                                            Print.fmt_info(f"§f可以直接热加载该插件: {plugin_data.name}, 是否加载(§aY§f/§cN§f): ")
+                                            Print.fmt_info(
+                                                f"§f可以直接热加载该插件: {plugin_data.name}, 是否加载(§aY§f/§cN§f): ")
                                         ).strip().lower()
                                         if resp == "y":
                                             for i in pres:
                                                 if i not in plugin_group.loaded_plugins_name:
                                                     try:
-                                                        plugin_group.load_plugin_hot(i.name, i.plugin_type)
+                                                        plugin_group.load_plugin_hot(
+                                                            i.name, i.plugin_type)
                                                     except BaseException as err:
-                                                        Print.print_err(f"插件热加载出现问题: {err}")
+                                                        Print.print_err(
+                                                            f"插件热加载出现问题: {err}")
                                     else:
-                                        Print.print_inf("插件已存在, 若要更新版本, 请重启 ToolDelta", need_log=False)
-                                        r = input(Print.fmt_info("§f输入 §cq §f退出, 其他则返回插件市场"))
+                                        Print.print_inf(
+                                            "插件已存在, 若要更新版本, 请重启 ToolDelta", need_log=False)
+                                        r = input(Print.fmt_info(
+                                            "§f输入 §cq §f退出, 其他则返回插件市场"))
                                 else:
-                                    Print.print_inf("下载插件后重启ToolDelta才能生效", need_log=False)
-                                r = input(Print.fmt_info("§f输入 §cq §f退出, 其他则返回插件市场"))
+                                    Print.print_inf(
+                                        "下载插件后重启ToolDelta才能生效", need_log=False)
+                                r = input(Print.fmt_info(
+                                    "§f输入 §cq §f退出, 其他则返回插件市场"))
                                 if r.lower() == "q":
                                     break
                             else:
                                 Print.print_inf("已取消.", need_log=False)
                                 time.sleep(1)
                         else:
                             Print.print_err("超出序号范围")
@@ -149,71 +206,112 @@
         except Exception as err:
             Print.print_err("获取插件市场插件出现问题, 报错如下:")
             Print.print_err(traceback.format_exc())
             return
         clear_screen()
         Print.clean_print("§a已从插件市场返回 ToolDelta 控制台.")
 
-    def get_datas_from_market(self, source_url: str = None):
-        if source_url is None:
-            source_url = Cfg().get_cfg("ToolDelta基本配置.json", {"插件市场源": str})["插件市场源"]
-        market_datas = _get_json_from_url(
-            _url_join(source_url, "market_tree.json")
+    def get_datas_from_market(self, source_url: str | None = None) -> dict:
+        """从插件市场获取数据
+
+        Args:
+            source_url (str | None, optional): 插件市场源, 默认为None,有则替换整体插件市场源
+
+        Returns:
+            dict: 插件市场数据
+        """
+        if isinstance(source_url, str):
+            self.plugins_download_url = self.plugins_download_url
+        market_datas = get_json_from_url(
+            url_join(self.plugins_download_url, "market_tree.json")
         )
-        self.plugins_download_url = source_url
         return market_datas
 
-    def get_plugin_data_from_market(self, plugin_id: str):
+    def get_plugin_data_from_market(self, plugin_id: str) -> PluginRegData:
+        """从插件市场获取插件数据
+
+        Args:
+            plugin_id (str): 插件ID
+
+        Raises:
+            KeyError: 无法通过ID查找插件
+
+        Returns:
+            PluginRegData: 插件注册数据
+        """
         plugin_name = self.plugin_id_name_map.get(plugin_id)
         if plugin_name is None:
             raise KeyError(f"无法通过ID: {plugin_id} 查找插件")
         data_url = self.plugins_download_url + "/" + plugin_name + "/datas.json"
-        res = requests.get(data_url)
+        res = requests.get(data_url, timeout=10)
         res.raise_for_status()
         datas = json.loads(res.text)
         return PluginRegData(plugin_name, datas)
 
-    def choice_plugin(self, plugin_data: PluginRegData):
+    def choice_plugin(self, plugin_data: PluginRegData) -> tuple[bool, list[PluginRegData]]:
+        """选中插件进行介绍与操作
+
+        Args:
+            plugin_data (PluginRegData): 插件注册数据
+
+        Returns:
+            tuple[bool, list[PluginRegData]]: 是否下载, 下载的插件列表
+        """
         pre_plugins_str = (
-            ", ".join([f"{k}§7v{v}" for k, v in plugin_data.pre_plugins.items()]) or "无"
+            ", ".join(
+                [f"{k}§7v{v}" for k, v in plugin_data.pre_plugins.items()]) or "无"
         )
         clear_screen()
         Print.print_inf(
             f"{plugin_data.name} v{plugin_data.version_str}", need_log=False
         )
         Print.print_inf(
             f"作者: §f{plugin_data.author}§7, 版本: §f{plugin_data.version_str} §b{plugin_data.plugin_type_str}",
             need_log=False,
         )
         Print.print_inf(f"前置插件: §f{pre_plugins_str}", need_log=False)
         Print.print_inf(f"介绍: {plugin_data.description}", need_log=False)
         Print.print_inf("", need_log=False)
-        res = input(Print.fmt_info("§f下载 = §aY§f, 取消 = §cN§f, 请输入:")).lower().strip()
+        res = input(Print.fmt_info(
+            "§f下载 = §aY§f, 取消 = §cN§f, 请输入:")).lower().strip()
         if res == "y":
             Print.clean_print(f"§6正在下载插件: §f{plugin_data.name}", end="\r")
             pres = self.download_plugin(plugin_data)
             pres.reverse()
             return True, pres
-        return False, None
+        return False, []
 
-    def get_plugin_id_name_map(self):
-        try:
-            src_url = Cfg().get_cfg("ToolDelta基本配置.json", {"插件市场源": str})["插件市场源"]
-        except:
-            src_url = PLUGIN_MARKET_SOURCE_OFFICIAL
-        res = requests.get(src_url + "/plugin_ids_map.json", timeout=10)
+    def get_plugin_id_name_map(self) -> dict:
+        """获取插件ID与插件名的映射
+
+        Returns:
+            dict: 插件ID与插件名的映射
+        """
+        res = requests.get(self.plugins_download_url +
+                           "/plugin_ids_map.json", timeout=5)
         res.raise_for_status()
-        res1 = json.loads(res.text)
+        res1: dict = json.loads(res.text)
         self.plugin_id_name_map = res1
         return res1
 
     def download_plugin(
         self,
         plugin_data: PluginRegData
-    ):
+    ) -> list[PluginRegData]:
+        """下载插件
+
+        Args:
+            plugin_data (PluginRegData): 插件注册数据
+
+        Raises:
+            ValueError: 未知插件类型
+
+        Returns:
+            list[PluginRegData]: 插件注册数据列表
+        """
         if self.plugin_id_name_map is None:
             self.plugin_id_name_map = self.get_plugin_id_name_map()
         pres = [plugin_data]
         download_paths = self.find_dirs(plugin_data)
         for plugin_id in plugin_data.pre_plugins:
             plugin_name = self.plugin_id_name_map[plugin_id]
             Print.clean_print(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
@@ -221,79 +319,103 @@
             pres += self.download_plugin(plugin_datas)
         cache_dir = tempfile.mkdtemp()
         try:
             for paths in download_paths:
                 if not paths.strip():
                     Print.print_war("下载路径为空, 跳过")
                     continue
-                url = _url_join(self.plugins_download_url, paths)
+                url = url_join(self.plugins_download_url, paths)
                 # Determine download path based on plugin type
                 match plugin_data.plugin_type:
                     case "classic":
                         download_path = os.path.join(
                             "插件文件", TOOLDELTA_CLASSIC_PLUGIN
                         )
                     case "injected":
                         download_path = os.path.join(
                             "插件文件", TOOLDELTA_INJECTED_PLUGIN
                         )
                     case _:
-                        raise Exception(
+                        raise ValueError(
                             f"未知插件类型: {plugin_data.plugin_type}, 你可能需要通知ToolDelta项目开发组解决"
                         )
-                os.makedirs(os.path.join(cache_dir, plugin_data.name), exist_ok=True)
-                path_last = _path_dir(paths)
+                os.makedirs(os.path.join(
+                    cache_dir, plugin_data.name), exist_ok=True)
+                path_last = path_dir(paths)
                 if path_last is not None:
                     # 自动创建文件夹
                     folder_path = os.path.join(cache_dir, path_last)
                     os.makedirs(folder_path, exist_ok=True)
-                urlmethod.download_unknown_file(url, os.path.join(cache_dir, paths))
+                urlmethod.download_unknown_file(
+                    url, os.path.join(cache_dir, paths))
             # Move downloaded files to target download path
             target_path = download_path
             os.makedirs(target_path, exist_ok=True)
             # 制作所需的目录结构
             for root, _, files in os.walk(cache_dir):
                 for filename in files:
                     source_file = os.path.join(root, filename)
                     target_file = os.path.join(
                         target_path, os.path.relpath(source_file, cache_dir)
                     )
                     os.makedirs(os.path.dirname(target_file), exist_ok=True)
                     shutil.move(source_file, target_file)
-            from tooldelta.plugin_manager import plugin_manager
-            # 注册插件
-            plugin_manager.push_plugin_reg_data(self.get_plugin_data_from_market(plugin_data.plugin_id))
+            from .plugin_manager import plugin_manager
+            plugin_manager.push_plugin_reg_data(
+                self.get_plugin_data_from_market(plugin_data.plugin_id))
             Print.clean_print(f"§a成功下载插件 §f{plugin_data.name}§a 至插件文件夹")
         finally:
             shutil.rmtree(cache_dir)
         return pres
 
-    def find_dirs(self, plugin_data: PluginRegData):
+    def find_dirs(self, plugin_data: PluginRegData) -> list[str]:
+        """查找插件目录
+
+        Args:
+            plugin_data (PluginRegData): 插件注册数据
+
+        Raises:
+            KeyError: 目录结构错误
+            eExceptionrr: 获取插件市场插件目录结构出现问题
+
+        Returns:
+            list[str]: 插件目录列表
+        """
         try:
-            data = _get_json_from_url(
-                _url_join(self.plugins_download_url, "directory.json")
+            data = get_json_from_url(
+                url_join(self.plugins_download_url, "directory.json")
             )
             data_list = []
             for folder, files in data.items():
                 if plugin_data.name == folder.split("/")[0]:
                     # 展开
                     for file in files:
                         data_list.append(folder + r"/" + file)
             return data_list
         except KeyError as err:
             Print.print_err(f"获取插件市场插件目录结构出现问题: 无法找到 {err}, 有可能是未来得及更新目录")
-            return
+            raise KeyError(f"无法找到 {err}, 有可能是未来得及更新目录") from err
         except Exception as err:
             Print.print_err(f"获取插件市场插件目录结构出现问题: {err}")
-            return
+            raise KeyError(f"获取插件市场插件目录结构出现问题: {err}")from err
 
-    @staticmethod
-    def get_latest_plugin_version(plugin_id: str):
-        try:
-            src_url = Cfg().get_cfg("ToolDelta基本配置.json", {"插件市场源": str})["插件市场源"]
-        except:
-            src_url = PLUGIN_MARKET_SOURCE_OFFICIAL
-        return _get_json_from_url(
-            _url_join(src_url, "latest_versions.json")
+    def get_latest_plugin_version(self, plugin_id: str) -> str:
+        """获取最新插件版本
+
+        Args:
+            plugin_id (str): 插件ID
+
+        Raises:
+            KeyError: 无法通过ID获取最新插件版本
+
+        Returns:
+            str: 最新插件版本
+        """
+        result = get_json_from_url(
+            url_join(self.plugins_download_url, "latest_versions.json")
         ).get(plugin_id)
+        if isinstance(result, str):
+            return result
+        raise KeyError(f"无法通过ID: {plugin_id} 获取最新插件版本")
+
 
 market = PluginMarket()
```

### Comparing `tooldelta-0.5.4/tooldelta/starter.py` & `tooldelta-0.5.5/tooldelta/starter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-import signal
+"""ToolDelta 启动器"""
+import os
 import time
-from tooldelta import builtins, urlmethod
-from tooldelta.frame import Frame
-from tooldelta.frame import GameCtrl
-from tooldelta.basic_mods import os, traceback
-from tooldelta.color_print import Print
-from tooldelta.plugin_load.PluginGroup import plugin_group
-from tooldelta.plugin_load.injected_plugin import movent
+import traceback
+from .builtins import tmpjson_save_thread
+from .urlmethod import check_update
+from .frame import Frame, GameCtrl
+from .color_print import Print
+from .plugin_load.PluginGroup import plugin_group
+from .plugin_load.injected_plugin import movent
 
 frame = Frame()
-def signal_handler(*arg):
-    # 排除信号中断
-    pass
-signal.signal(signal.SIGINT, signal_handler)
 
-def start_tool_delta():
-    # 初始化系统
+
+def start_tool_delta() -> None:
+    """启动ToolDelta"""
     plugin_group.set_frame(frame)
     try:
         frame.welcome()
-        urlmethod.check_update()
+        check_update()
         frame.basic_operation()
         frame.loadConfiguration()
         game_control = GameCtrl(frame)
         frame.set_game_control(game_control)
         frame.set_plugin_group(plugin_group)
         movent.set_frame(frame)
         plugin_group.read_all_plugins()
         frame.plugin_load_finished(plugin_group)
-        builtins.tmpjson_save_thread()
+        tmpjson_save_thread()
         frame.launcher.listen_launched(game_control.Inject)
         game_control.set_listen_packets()
-        # TODO: 自动更新需要时间间隔
         raise frame.launcher.launch()
     except (KeyboardInterrupt, SystemExit):
         pass
-    except:
+    except Exception:
         Print.print_err("ToolDelta 运行过程中出现问题: " + traceback.format_exc())
 
 
-def safe_jump(*, out_task=True, exit_directly=True):
+def safe_jump(*, out_task: bool = True, exit_directly: bool = True) -> None:
+    """安全退出
+
+    Args:
+        out_task (bool, optional): frame框架系统是否退出
+        exit_directly (bool, optional): 是否三秒强制直接退出
+    """
     if out_task:
         frame.system_exit()
     frame.safelyExit()
     if exit_directly:
         for _ in range(2, 0, -1):
             Print.print_war(f"{_}秒后强制退出...", end="\r")
             time.sleep(1)
```

### Comparing `tooldelta-0.5.4/tooldelta/sys_args.py` & `tooldelta-0.5.5/tooldelta/sys_args.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+"解析启动参数"
 import sys
 
-def sys_args_to_dict(argv: list[str] = sys.argv):
-    # 将启动参数分割为 -键=值 或 -键=None
+
+def sys_args_to_dict(argv: list[str] = sys.argv)-> dict[str, str | None]:
+    """将启动参数转换为字典
+
+    Args:
+        argv (list[str], optional): 启动参数
+
+    Returns:
+        dict[str, str | None]: 启动参数字典
+    """
     # 为什么不用 argsparser? 因为这样可以支持混合型启动参数
-    d: dict[str, str] = {}
+    d: dict[str, str | None] = {}
     i = 0
     while i < len(argv):
         arg = argv[i]
         if arg.startswith("-"):
             arg = arg.strip("--").strip("-")
             try:
                 val = argv[i + 1]
@@ -15,8 +24,8 @@
                     val = None
                 else:
                     i += 1
             except IndexError:
                 val = None
             d[arg] = val
         i += 1
-    return d
+    return d
```

### Comparing `tooldelta-0.5.4/tooldelta/urlmethod.py` & `tooldelta-0.5.5/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.4/PKG-INFO` & `tooldelta-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.4
+Version: 0.5.5
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.4 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.5 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: mido
```

