# Comparing `tmp/tooldelta-0.5.5.tar.gz` & `tmp/tooldelta-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.5.tar", max compression
+gzip compressed data, was "tooldelta-0.5.6.tar", max compression
```

## Comparing `tooldelta-0.5.5.tar` & `tooldelta-0.5.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1497 2024-04-19 00:30:34.663456 tooldelta-0.5.5/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-19 00:30:34.663456 tooldelta-0.5.5/README.md
--rwxr-xr-x   0        0        0      973 2024-04-19 00:30:46.263467 tooldelta-0.5.5/pyproject.toml
--rwxr-xr-x   0        0        0      360 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/auths.py
--rwxr-xr-x   0        0        0    19961 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    12365 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10889 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/color_print.py
--rw-r--r--   0        0        0     1884 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    30100 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/frame.py
--rwxr-xr-x   0        0        0     4644 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    20488 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1276 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/logger.py
--rwxr-xr-x   0        0        0    29616 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/neo_libs/neo_conn.py
--rwxr-xr-x   0        0        0     1292 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/packets.py
--rwxr-xr-x   0        0        0    15769 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     7341 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      450 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     9975 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9146 2024-04-19 00:30:34.667456 tooldelta-0.5.5/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    16934 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16769 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1774 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/starter.py
--rwxr-xr-x   0        0        0      808 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9071 2024-04-19 00:30:34.671456 tooldelta-0.5.5/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-19 13:43:42.401255 tooldelta-0.5.6/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-19 13:43:42.401255 tooldelta-0.5.6/README.md
+-rwxr-xr-x   0        0        0      973 2024-04-19 13:43:51.737315 tooldelta-0.5.6/pyproject.toml
+-rwxr-xr-x   0        0        0      360 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    19961 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    12365 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10889 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1884 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    30100 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     4644 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    20497 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1276 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/logger.py
+-rw-r--r--   0        0        0    29616 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1292 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    15769 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     7341 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      450 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     9975 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9146 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    16934 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16769 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1774 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      808 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9071 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.6/PKG-INFO
```

### Comparing `tooldelta-0.5.5/LICENSE` & `tooldelta-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/README.md` & `tooldelta-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/pyproject.toml` & `tooldelta-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.5" # This field is automatically set to the value in the version file
+version = "0.5.6" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.5.5/tooldelta/auths.py` & `tooldelta-0.5.6/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/builtins.py` & `tooldelta-0.5.6/tooldelta/builtins.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/cfg.py` & `tooldelta-0.5.6/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/color_print.py` & `tooldelta-0.5.6/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/constants.py` & `tooldelta-0.5.6/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.6/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/frame.py` & `tooldelta-0.5.6/tooldelta/frame.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/game_texts.py` & `tooldelta-0.5.6/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/launch_cli.py` & `tooldelta-0.5.6/tooldelta/launch_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import platform
 from typing import Callable, Optional
 import ujson as json
 import requests
 import tooldelta
 
 from tooldelta import constants
-from .neo_libs import neo_conn
+from . import neo_conn
 from .cfg import Cfg
 from .builtins import Builtins
 from .color_print import Print
 from .sys_args import sys_args_to_dict
 from .packets import Packet_CommandOutput
 from .urlmethod import download_file_singlethreaded, get_free_port
 
@@ -551,15 +551,16 @@
         Raises:
             AssertionError: 端口号错误
 
         Returns:
             SystemExit | Exception | SystemError: 退出状态
         """
         try:
-            openat_port = int(sys_args_to_dict().get("access-point-port") or "24020")
+            openat_port = int(sys_args_to_dict().get(
+                "access-point-port") or "24020")
             if openat_port not in range(65536):
                 raise AssertionError
         except (ValueError, AssertionError):
             Print.print_err("启动参数 -access-point-port 错误: 不是1~65535的整数")
         if openat_port == 0:
             Print.print_war(
                 "未用启动参数指定链接neOmega接入点开放端口, 尝试使用默认端口 24015"
```

### Comparing `tooldelta-0.5.5/tooldelta/launch_options.py` & `tooldelta-0.5.6/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/logger.py` & `tooldelta-0.5.6/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/neo_libs/neo_conn.py` & `tooldelta-0.5.6/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/packets.py` & `tooldelta-0.5.6/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.6/tooldelta/plugin_load/PluginGroup.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.6/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.5.6/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/plugin_manager.py` & `tooldelta-0.5.6/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/plugin_market.py` & `tooldelta-0.5.6/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/starter.py` & `tooldelta-0.5.6/tooldelta/starter.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/sys_args.py` & `tooldelta-0.5.6/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/tooldelta/urlmethod.py` & `tooldelta-0.5.6/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.5/PKG-INFO` & `tooldelta-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.5
+Version: 0.5.6
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
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.5 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.6 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: mido
```

