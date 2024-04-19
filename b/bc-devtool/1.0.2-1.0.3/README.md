# Comparing `tmp/bc-devtool-1.0.2.tar.gz` & `tmp/bc-devtool-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/bc-devtool/bc-devtool/dist/.tmp-dceccnyq/bc-devtool-1.0.2.tar", last modified: Sun Dec 18 16:20:41 2022, max compression
+gzip compressed data, was "/home/runner/work/bc-devtool/bc-devtool/dist/.tmp-x9h9fxhp/bc-devtool-1.0.3.tar", last modified: Fri Apr 19 14:41:41 2024, max compression
```

## Comparing `bc-devtool-1.0.2.tar` & `bc-devtool-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      380 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10838 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/ali_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    44648 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/arg_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28296 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/dev_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/op_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/src/bc_devtool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/src/bc_devtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 16:20:41.000000 bc-devtool-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/test/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2022-12-18 16:20:17.000000 bc-devtool-1.0.2/test/test_configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/ali_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44648 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/arg_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/dev_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18397 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/op_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/src/bc_devtool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/src/bc_devtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:41:41.000000 bc-devtool-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/test/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-19 14:41:28.000000 bc-devtool-1.0.3/test/test_configurator.py
```

### Comparing `bc-devtool-1.0.2/LICENSE` & `bc-devtool-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/PKG-INFO` & `bc-devtool-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-devtool
-Version: 1.0.2
+Version: 1.0.3
 Summary: Gadgets to help with development
 Home-page: https://github.com/beichenzhizuoshi/bc-devtool
 Author: beichenzhizuoshi
 Author-email: beichenzhizuoshi@163.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `bc-devtool-1.0.2/README.md` & `bc-devtool-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/setup.cfg` & `bc-devtool-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bc-devtool
-version = 1.0.2
+version = 1.0.3
 description = Gadgets to help with development
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/beichenzhizuoshi/bc-devtool
 author = beichenzhizuoshi
 author_email = beichenzhizuoshi@163.com
 license = MIT
```

### Comparing `bc-devtool-1.0.2/src/bc_devtool/ali_script.py` & `bc-devtool-1.0.3/src/bc_devtool/ali_script.py`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/src/bc_devtool/arg_actions.py` & `bc-devtool-1.0.3/src/bc_devtool/arg_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
         enum_type = type(default_value[0])
       else:
         enum_type = type(default_value)
 
     chios = tuple(e.name.lower() for e in enum_type)
     self._enum = enum_type
     self._short = []
-    super().__init__(option_strings, dest, nargs, const, default_value, type, chios, required, help, metavar)
+    super().__init__(option_strings, dest, nargs, const, default_value, None, chios, required, help, metavar)
 
   def _find_enum_object(self, name: str) -> TypeVar('AE', bound=enum.Enum):
     """根据参数获取对应的枚举对象,优先查找别名参数,再查找枚举字符串参数
 
     Args:
         self (_type_):
         bound (enum.Enum, optional): Defaults to enum.Enum.
```

### Comparing `bc-devtool-1.0.2/src/bc_devtool/configurator.py` & `bc-devtool-1.0.3/src/bc_devtool/configurator.py`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/src/bc_devtool/dev_tools.py` & `bc-devtool-1.0.3/src/bc_devtool/dev_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # /usr/bin/python3
+# from __future__ import annotations
 from __future__ import annotations
 
 import argparse
 import enum
 import gettext
 import logging
 import os
 import re
 from enum import auto
 from enum import Enum
 from enum import unique
 from pathlib import Path
 from typing import List
 
-import bc_devtool
+from bc_devtool import __version__
 from bc_devtool import arg_actions as aa
 from bc_devtool import file_util
 from bc_devtool import utils
 from bc_devtool.utils import simple_log
 from git import Repo
 
 
-VERSION = bc_devtool.__version__
+VERSION = __version__
 _ = gettext.translation('dev_tools', Path.joinpath(Path(__file__).parent, 'locale'), fallback=True).gettext
 REPO_PATH = '.repo/manifests/default.xml'
 recore_error = None
 
 SOURCE_SUFFIXS = ['cpp', 'cc', 'c', 'h', 'hpp', 'txt', 'py', 'cmake', 'java']
 
 
@@ -339,19 +340,19 @@
       'transform_known': _('已知文件编码转换其它编码'),
       'transform_auto': _('自动检测文件编码转换'),
       'crlf_to_lf': _('CRLF 换行转 LF 换行'),
       'lf_to_crlf': _('LF 换行转 CRLF 换行'),
       'cn_transform': _('检测中文文件编码转换')
   }
 
-  command_action: aa.TrueRequiredAction = cmd_e.add_argument('--cmd', type=EncodingTransform, action=aa.TrueRequiredAction,
-                                                             action_type=aa.EnumAction,
-                                                             help='\n\n'.join('{}: {}'.format(key, value)
-                                                                              for key, value in encoding_choices_help.items()),
-                                                             default=[EncodingTransform.VIEW], nargs='*')
+  command_action: aa.TrueRequiredAction = cmd_e.add_argument(
+      '--cmd', type=EncodingTransform, action=aa.TrueRequiredAction, bind_value=True, action_type=aa.EnumAction,
+      help='\n\n'.join('{}: {}'.format(key, value) for key, value in encoding_choices_help.items()),
+      default=[EncodingTransform.VIEW],
+      nargs='*')
 
   cmd_e.add_argument('files', nargs='*', default=[os.getcwd()], help=_('处理的文件集合'), action=aa.PathAction)
   cmd_e.add_argument('--recursive', action=argparse.BooleanOptionalAction, default=True, help=_('递归处理目录'))
 
   from_action = cmd_e.add_argument('-f', '--from', action=aa.EnumAction, type=FileEncoding, help=_('转换前的编码'))
   to_action = cmd_e.add_argument('-t', '--to', action=aa.EnumAction, type=FileEncoding, help=_('转换后的编码'))
```

### Comparing `bc-devtool-1.0.2/src/bc_devtool/file_util.py` & `bc-devtool-1.0.3/src/bc_devtool/file_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,21 +345,25 @@
         f.write(self._content)
       return True
     return False
 
   def _guess_input_output_encoding(self, result: FileConverterResult) -> bool:
     if self._guessed:
       return True
-    if not self.from_encoding:
-      attrs = get_binary_encoding(self._content)
-      if attrs['confidence'] < self._confidence:
-        result.failed().failed_reson(_('检测文件 {} 编码 {} 精确度太低: {}, 最小处理精确度: {}').format(
-            self.input, attrs['encoding'], attrs['confidence'], self._confidence))
-        return False
-      self.from_encoding = attrs['encoding']
+
+    attrs = get_binary_encoding(self._content)
+    if attrs['confidence'] < self._confidence:
+      result.failed().failed_reson(_('检测文件 {} 编码 {} 精确度太低: {}, 最小处理精确度: {}').format(
+          self.input, attrs['encoding'], attrs['confidence'], self._confidence))
+      return False
+
+    if self.from_encoding and self.from_encoding != attrs['encoding']:
+      # 当猜测的编译与输入编码不符合时,避免错误应该跳过
+      return False
+    self.from_encoding = attrs['encoding']
 
     # 规范化编码字符串,后续可以直接字符串比较编码
     info = codecs.lookup(self.from_encoding)
     if info:
       self.from_encoding = info.name
     else:
       result.failed().failed_reson(_('输入文件 {} 编码不支持: {}').format(self.input, self.from_encoding))
```

### Comparing `bc-devtool-1.0.2/src/bc_devtool/op_menu.py` & `bc-devtool-1.0.3/src/bc_devtool/op_menu.py`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/src/bc_devtool/utils.py` & `bc-devtool-1.0.3/src/bc_devtool/utils.py`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/src/bc_devtool.egg-info/PKG-INFO` & `bc-devtool-1.0.3/src/bc_devtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-devtool
-Version: 1.0.2
+Version: 1.0.3
 Summary: Gadgets to help with development
 Home-page: https://github.com/beichenzhizuoshi/bc-devtool
 Author: beichenzhizuoshi
 Author-email: beichenzhizuoshi@163.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `bc-devtool-1.0.2/src/bc_devtool.egg-info/SOURCES.txt` & `bc-devtool-1.0.3/src/bc_devtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/test/test_actions.py` & `bc-devtool-1.0.3/test/test_actions.py`

 * *Files identical despite different names*

### Comparing `bc-devtool-1.0.2/test/test_configurator.py` & `bc-devtool-1.0.3/test/test_configurator.py`

 * *Files identical despite different names*

