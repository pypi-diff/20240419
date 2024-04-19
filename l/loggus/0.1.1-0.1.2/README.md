# Comparing `tmp/loggus-0.1.1.tar.gz` & `tmp/loggus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\loggus-0.1.1.tar", last modified: Wed Jun 29 05:41:30 2022, max compression
+gzip compressed data, was "dist\loggus-0.1.2.tar", last modified: Fri Apr 19 01:49:32 2024, max compression
```

## Comparing `loggus-0.1.1.tar` & `loggus-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-06-29 05:41:30.000000 loggus-0.1.1/
-drwxrwxrwx   0        0        0        0 2022-06-29 05:41:30.000000 loggus-0.1.1/loggus/
--rw-rw-rw-   0        0        0     3195 2022-06-29 01:23:58.000000 loggus-0.1.1/loggus/fields.py
--rw-rw-rw-   0        0        0     2345 2022-06-29 01:23:58.000000 loggus-0.1.1/loggus/formatter.py
--rw-rw-rw-   0        0        0     1315 2022-06-29 05:40:02.000000 loggus-0.1.1/loggus/frame.py
--rw-rw-rw-   0        0        0     6909 2022-06-29 01:23:58.000000 loggus-0.1.1/loggus/hooks.py
--rw-rw-rw-   0        0        0     1143 2022-06-29 03:47:15.000000 loggus-0.1.1/loggus/level.py
--rw-rw-rw-   0        0        0     6664 2022-06-29 05:20:28.000000 loggus-0.1.1/loggus/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-29 05:41:30.000000 loggus-0.1.1/loggus.egg-info/
--rw-rw-rw-   0        0        0        1 2022-06-29 05:41:29.000000 loggus-0.1.1/loggus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      450 2022-06-29 05:41:29.000000 loggus-0.1.1/loggus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2022-06-29 05:41:29.000000 loggus-0.1.1/loggus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      283 2022-06-29 05:41:29.000000 loggus-0.1.1/loggus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2022-06-29 05:41:29.000000 loggus-0.1.1/loggus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       69 2022-06-29 01:23:58.000000 loggus-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      450 2022-06-29 05:41:30.000000 loggus-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1455 2022-06-29 05:29:30.000000 loggus-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2022-06-29 05:41:30.000000 loggus-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1571 2022-06-29 05:40:37.000000 loggus-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 01:49:32.000000 loggus-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-19 01:49:32.000000 loggus-0.1.2/loggus/
+-rw-rw-rw-   0        0        0     3195 2022-06-29 01:23:58.000000 loggus-0.1.2/loggus/fields.py
+-rw-rw-rw-   0        0        0     2345 2022-06-29 01:23:58.000000 loggus-0.1.2/loggus/formatter.py
+-rw-rw-rw-   0        0        0     1362 2022-07-11 05:08:46.000000 loggus-0.1.2/loggus/frame.py
+-rw-rw-rw-   0        0        0     6909 2022-06-29 01:23:58.000000 loggus-0.1.2/loggus/hooks.py
+-rw-rw-rw-   0        0        0     1186 2022-07-11 05:08:46.000000 loggus-0.1.2/loggus/level.py
+-rw-rw-rw-   0        0        0      975 2024-04-19 01:48:33.000000 loggus-0.1.2/loggus/utils.py
+-rw-rw-rw-   0        0        0     6903 2024-04-19 01:44:50.000000 loggus-0.1.2/loggus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 01:49:32.000000 loggus-0.1.2/loggus.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-19 01:49:32.000000 loggus-0.1.2/loggus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      450 2024-04-19 01:49:32.000000 loggus-0.1.2/loggus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-04-19 01:49:32.000000 loggus-0.1.2/loggus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      299 2024-04-19 01:49:32.000000 loggus-0.1.2/loggus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 01:49:32.000000 loggus-0.1.2/loggus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2022-06-29 01:23:58.000000 loggus-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      450 2024-04-19 01:49:32.000000 loggus-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-12-22 09:35:49.000000 loggus-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 01:49:32.000000 loggus-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1625 2022-07-11 05:08:46.000000 loggus-0.1.2/setup.py
```

### Comparing `loggus-0.1.1/loggus/fields.py` & `loggus-0.1.2/loggus/fields.py`

 * *Files identical despite different names*

### Comparing `loggus-0.1.1/loggus/formatter.py` & `loggus-0.1.2/loggus/formatter.py`

 * *Files identical despite different names*

### Comparing `loggus-0.1.1/loggus/frame.py` & `loggus-0.1.2/loggus/frame.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# coding: utf-8
-import re, sys, inspect, colorama
-
-if sys.platform == "win32":
-    colorama.init(autoreset=True)
-
-if hasattr(sys, '_getframe'):
-    currentframe2 = lambda: sys._getframe(2)
-    currentframe3 = lambda: sys._getframe(3)
-else:
-    def currentframe2():
-        try:
-            raise
-        except Exception:
-            return sys.exc_info()[2].tb_frame.f_back.f_back
-    def currentframe3():
-        try:
-            raise
-        except Exception:
-            return sys.exc_info()[2].tb_frame.f_back.f_back.f_back
-
-varCallerName = "variables"
-varFieldRegex = re.compile(varCallerName + "\s*\((.*?)(?:$|\))", re.S).search
-
-
-def findCallerVariables(frame):
-    if inspect.istraceback(frame):
-        lineno = frame.tb_lineno
-        frame = frame.tb_frame
-    else:
-        lineno = frame.f_lineno
-    if not inspect.isframe(frame):
-        raise TypeError('{!r} is not a frame or traceback object'.format(frame))
-    start = lineno - 1
-    try:
-        lines, lnum = inspect.findsource(frame)
-    except OSError:
-        return ""
-    else:
-        start = max(0, min(start, len(lines) - 1))
-        codes = ""
-        for index in range(start, 0, -1):
-            line = lines[index]
-            codes = line + codes
-            if varCallerName in line:
-                break
-        return codes
+# coding: utf-8
+import re, sys, inspect, colorama
+
+if sys.platform == "win32":
+    colorama.init(autoreset=True)
+
+if hasattr(sys, '_getframe'):
+    currentframe2 = lambda: sys._getframe(2)
+    currentframe3 = lambda: sys._getframe(3)
+else:
+    def currentframe2():
+        try:
+            raise
+        except Exception:
+            return sys.exc_info()[2].tb_frame.f_back.f_back
+    def currentframe3():
+        try:
+            raise
+        except Exception:
+            return sys.exc_info()[2].tb_frame.f_back.f_back.f_back
+
+varCallerName = "variables"
+varFieldRegex = re.compile(varCallerName + "\s*\((.*?)(?:$|\))", re.S).search
+
+
+def findCallerVariables(frame):
+    if inspect.istraceback(frame):
+        lineno = frame.tb_lineno
+        frame = frame.tb_frame
+    else:
+        lineno = frame.f_lineno
+    if not inspect.isframe(frame):
+        raise TypeError('{!r} is not a frame or traceback object'.format(frame))
+    start = lineno - 1
+    try:
+        lines, lnum = inspect.findsource(frame)
+    except OSError:
+        return ""
+    else:
+        start = max(0, min(start, len(lines) - 1))
+        codes = ""
+        for index in range(start, 0, -1):
+            line = lines[index]
+            codes = line + codes
+            if varCallerName in line:
+                break
+        return codes
```

### Comparing `loggus-0.1.1/loggus/hooks.py` & `loggus-0.1.2/loggus/hooks.py`

 * *Files identical despite different names*

### Comparing `loggus-0.1.1/loggus/level.py` & `loggus-0.1.2/loggus/level.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# coding: utf-8
-class Level:
-
-    def __init__(self, string: str, integer: int, color: str):
-        self.describe = string
-        self.value = integer
-        self.color = color.format(string)
-        self.colorTmp = color
-
-    def toColor(self, msg: str):
-        return self.colorTmp.format(msg)
-
-    def __eq__(self, other):
-        return self.value == other.value
-
-    def __gt__(self, other):
-        return self.value > other.value
-
-    def __ge__(self, other):
-        return self.value >= other.value
-
-    def __lt__(self, other):
-        return self.value < other.value
-
-    def __le__(self, other):
-        return self.value <= other.value
-
-    def __hash__(self):
-        return self.value
-
-    def __str__(self):
-        return self.describe
-
-    __repr__ = __str__
-
-
-DEBUG = Level("debug", 10, "\033[1;37m{}\033[0m")
-INFO = Level("info", 20, "\033[1;32m{}\033[0m")
-WARNING = Level("warning", 30, "\033[1;33m{}\033[0m")
-ERROR = Level("error", 40, "\033[1;31m{}\033[0m")
-PANIC = Level("panic", 50, "\033[1;36m{}\033[0m")
-GetAllLevels = lambda: [DEBUG, INFO, WARNING, ERROR, PANIC]
-IsLevel = lambda level: level in GetAllLevels()
+# coding: utf-8
+class Level:
+
+    def __init__(self, string: str, integer: int, color: str):
+        self.describe = string
+        self.value = integer
+        self.color = color.format(string)
+        self.colorTmp = color
+
+    def toColor(self, msg: str):
+        return self.colorTmp.format(msg)
+
+    def __eq__(self, other):
+        return self.value == other.value
+
+    def __gt__(self, other):
+        return self.value > other.value
+
+    def __ge__(self, other):
+        return self.value >= other.value
+
+    def __lt__(self, other):
+        return self.value < other.value
+
+    def __le__(self, other):
+        return self.value <= other.value
+
+    def __hash__(self):
+        return self.value
+
+    def __str__(self):
+        return self.describe
+
+    __repr__ = __str__
+
+
+DEBUG = Level("debug", 10, "\033[1;37m{}\033[0m")
+INFO = Level("info", 20, "\033[1;32m{}\033[0m")
+WARNING = Level("warning", 30, "\033[1;33m{}\033[0m")
+ERROR = Level("error", 40, "\033[1;31m{}\033[0m")
+PANIC = Level("panic", 50, "\033[1;36m{}\033[0m")
+GetAllLevels = lambda: [DEBUG, INFO, WARNING, ERROR, PANIC]
+IsLevel = lambda level: level in GetAllLevels()
```

### Comparing `loggus-0.1.1/loggus/__init__.py` & `loggus-0.1.2/loggus/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,212 @@
-# coding: utf-8
-import threading, contextlib, traceback as _traceback
-from copy import deepcopy
-from typing import List, Dict
-from loggus.level import *
-from loggus.hooks import *
-from loggus.fields import *
-from loggus.formatter import *
-from loggus.frame import *
-
-__version__ = "0.1.1"
-__index_page__ = "https://github.com/czasg/loggus"
-__doc_page__ = "https://github.com/czasg/loggus/README.md"
-__author__ = "https://czasg.github.io/docusaurus/author/intro"
-
-
-class Logger:
-
-    def __init__(self):
-        self.stream = sys.stdout
-        self.formatter = TextFormatter
-        self.fieldKeys = [FieldKeyTime, FieldKeyLevel, FieldKeyMsg]
-        self.needFrame: bool = False
-        self.baseLevel: Level = INFO
-        self.colorSwitch: bool = True
-        self.hooks: Dict[Level, List[IHook]] = {
-            DEBUG: [],
-            INFO: [],
-            WARNING: [],
-            ERROR: [],
-            PANIC: [],
-        }
-
-    def AddHooks(self, *hooks: List[IHook]) -> None:
-        for hook in hooks:  # type: IHook
-            if not IsIHook(hook):
-                raise Exception(f"undefined Hook[{hook}]!")
-            for level in hook.GetLevels():
-                if not IsLevel(level):
-                    raise Exception(f"undefined Level[{level}]!")
-                self.hooks[level].append(hook)
-
-    def SetLevel(self, level: Level) -> None:
-        if not IsLevel(level):
-            raise Exception(f"undefined Level[{level}]!")
-        self.baseLevel = level
-
-    def SetFormatter(self, formatter: [IFormatter, TextFormatter, JsonFormatter]):
-        if not IsIFormatter(formatter):
-            raise Exception(f"undefined Formatter[{formatter}]")
-        if formatter is JsonFormatter:
-            self.colorSwitch = False
-        self.formatter = formatter
-
-    def CloseColor(self):
-        self.colorSwitch = False
-
-    def OpenColor(self):
-        self.colorSwitch = True
-
-    def FireHooks(self, entry, level, msg, output) -> None:
-        for hook in self.hooks[level]:  # type: IHook
-            hook.Fire(entry, level, msg, output)
-
-    def IsLevelEnabled(self, level: Level) -> bool:
-        return level >= self.baseLevel
-
-    def Write(self, output: str) -> None:
-        self.stream.write(output)
-        self.stream.flush()
-
-    def update(self, _: dict = None, **kwargs):
-        return NewEntry(self).update(_, **kwargs)
-
-    def variables(self, *args):
-        return NewEntry(self).variables(*args, currentframe=currentframe3)
-
-    def traceback(self):
-        NewEntry(self).traceback()
-
-    def trycache(self, callback=None, *args, **kwargs):
-        return NewEntry(self).trycache(callback, *args, **kwargs)
-
-    def debug(self, *args):
-        NewEntry(self).debug(*args)
-
-    def info(self, *args):
-        NewEntry(self).info(*args)
-
-    def warning(self, *args):
-        NewEntry(self).warning(*args)
-
-    def error(self, *args):
-        NewEntry(self).error(*args)
-
-    def panic(self, *args):
-        NewEntry(self).panic(*args)
-
-
-class Entry:
-
-    def __init__(self, logger: Logger):
-        self.logger = logger
-        self.fields = {}
-        self.frameFuncName = None
-        self.frameLineNo = None
-        self.frameFilePath = None
-
-    def update(self, _: dict = None, **kwargs):
-        fields = _ or {}
-        fields.update(kwargs)
-        entry = NewEntry(self.logger, self.fields)
-        entry.fields.update(fields)
-        return entry
-
-    def variables(self, *args, currentframe=currentframe2):
-        if not args:
-            return self
-        code = findCallerVariables(currentframe())
-        match = varFieldRegex(code)
-        if not match:
-            self.warning(f"variables regex not match")
-            return self
-        return self.update(dict(zip([field.strip() for field in match.group(1).split(",")], args)))
-
-    def traceback(self):
-        self.update(error=_traceback.format_exc().strip()).error("traceback")
-
-    @contextlib.contextmanager
-    def trycache(self, callback=None, *args, **kwargs):
-        try:
-            yield self
-        except Exception as e:
-            if callback:
-                try:
-                    callback(e, *args, **kwargs)
-                except:
-                    pass
-            self.traceback()
-
-    def _log(self, level: Level, msg: str):
-        entry = NewEntry(self.logger, self.fields)
-        output = entry.logger.formatter.Format(entry, level, msg)
-        entry.logger.FireHooks(entry, level, msg, output)
-        entry.logger.Write(output)
-
-    def log(self, level: Level, msg: str):
-        self._log(level, msg)
-        if level >= PANIC:
-            sys.exit(PANIC.value)
-
-    def debug(self, *args):
-        if self.logger.IsLevelEnabled(DEBUG):
-            self.log(DEBUG, " ".join([f"{arg}" for arg in args]))
-
-    def info(self, *args):
-        if self.logger.IsLevelEnabled(INFO):
-            self.log(INFO, " ".join([f"{arg}" for arg in args]))
-
-    def warning(self, *args):
-        if self.logger.IsLevelEnabled(WARNING):
-            self.log(WARNING, " ".join([f"{arg}" for arg in args]))
-
-    def error(self, *args):
-        if self.logger.IsLevelEnabled(ERROR):
-            self.log(ERROR, " ".join([f"{arg}" for arg in args]))
-
-    def panic(self, *args):
-        if self.logger.IsLevelEnabled(PANIC):
-            self.log(PANIC, " ".join([f"{arg}" for arg in args]))
-
-
-# func
-NewLogger = lambda: Logger()
-AddHooks = lambda *hooks: _logger.AddHooks(*hooks)
-SetLevel = lambda level: _logger.SetLevel(level)
-SetFormatter = lambda formatter: _logger.SetFormatter(formatter)
-CloseColor = lambda: _logger.CloseColor()
-OpenColor = lambda: _logger.OpenColor()
-# entry
-debug = lambda *args: NewEntry().debug(*args)
-info = lambda *args: NewEntry().info(*args)
-warning = lambda *args: NewEntry().warning(*args)
-error = lambda *args: NewEntry().error(*args)
-panic = lambda *args: NewEntry().panic(*args)
-update = lambda _=None, **kwargs: NewEntry().update(_, **kwargs)
-variables = lambda *args: NewEntry().variables(*args, currentframe=currentframe3)
-traceback = lambda: NewEntry().traceback()
-trycache = lambda callback=None, *args, **kwargs: NewEntry().trycache(callback, *args, **kwargs)
-# logger
-_logger = NewLogger()
-_loggerPool = {None: _logger}
-_lock = threading.Lock()
-
-
-def GetLogger(name: str = None):
-    with _lock:
-        if name not in _loggerPool:
-            _loggerPool[name] = NewLogger()
-        return _loggerPool[name]
-
-
-def NewEntry(logger=_logger, fields=None):
-    entry = Entry(logger)
-    if fields:
-        try:
-            fields = deepcopy(fields)
-        except:
-            fields = {f"{key}": f"{value}" for key, value in fields.items()}
-        entry.fields = fields
-    return entry
+# coding: utf-8
+import threading, contextlib, traceback as _traceback
+from copy import deepcopy
+from typing import List, Dict
+from loggus.level import *
+from loggus.hooks import *
+from loggus.fields import *
+from loggus.formatter import *
+from loggus.frame import *
+from loggus.utils import *
+
+__version__ = "0.1.2"
+__index_page__ = "https://github.com/czasg/loggus"
+__doc_page__ = "https://github.com/czasg/loggus/README.md"
+__author__ = "https://czasg.github.io/docusaurus/author/intro"
+
+
+class Logger:
+
+    def __init__(self):
+        self.stream = sys.stdout
+        self.formatter = TextFormatter
+        self.fieldKeys = [FieldKeyTime, FieldKeyLevel, FieldKeyMsg]
+        self.needFrame: bool = False
+        self.baseLevel: Level = INFO
+        self.colorSwitch: bool = True
+        self.hooks: Dict[Level, List[IHook]] = {
+            DEBUG: [],
+            INFO: [],
+            WARNING: [],
+            ERROR: [],
+            PANIC: [],
+        }
+
+    def AddHooks(self, *hooks: List[IHook]) -> None:
+        for hook in hooks:  # type: IHook
+            if not IsIHook(hook):
+                raise Exception(f"undefined Hook[{hook}]!")
+            for level in hook.GetLevels():
+                if not IsLevel(level):
+                    raise Exception(f"undefined Level[{level}]!")
+                self.hooks[level].append(hook)
+
+    def SetLevel(self, level: Level) -> None:
+        if not IsLevel(level):
+            raise Exception(f"undefined Level[{level}]!")
+        self.baseLevel = level
+
+    def SetFormatter(self, formatter: [IFormatter, TextFormatter, JsonFormatter]):
+        if not IsIFormatter(formatter):
+            raise Exception(f"undefined Formatter[{formatter}]")
+        if formatter is JsonFormatter:
+            self.colorSwitch = False
+        self.formatter = formatter
+
+    def CloseColor(self):
+        self.colorSwitch = False
+
+    def OpenColor(self):
+        self.colorSwitch = True
+
+    def FireHooks(self, entry, level, msg, output) -> None:
+        for hook in self.hooks[level]:  # type: IHook
+            hook.Fire(entry, level, msg, output)
+
+    def IsLevelEnabled(self, level: Level) -> bool:
+        return level >= self.baseLevel
+
+    def Write(self, output: str) -> None:
+        self.stream.write(output)
+        self.stream.flush()
+
+    def update(self, _: dict = None, **kwargs):
+        return NewEntry(self).update(_, **kwargs)
+
+    def variables(self, *args):
+        return NewEntry(self).variables(*args, currentframe=currentframe3)
+
+    def traceback(self):
+        NewEntry(self).traceback()
+
+    def trycache(self, callback=None, *args, **kwargs):
+        return NewEntry(self).trycache(callback, *args, **kwargs)
+
+    def debug(self, *args):
+        NewEntry(self).debug(*args)
+
+    def info(self, *args):
+        NewEntry(self).info(*args)
+
+    def warning(self, *args):
+        NewEntry(self).warning(*args)
+
+    def error(self, *args):
+        NewEntry(self).error(*args)
+
+    def panic(self, *args):
+        NewEntry(self).panic(*args)
+
+
+class Entry:
+
+    def __init__(self, logger: Logger):
+        self.logger = logger
+        self.fields = {}
+        self.frameFuncName = None
+        self.frameLineNo = None
+        self.frameFilePath = None
+
+    def update(self, _: dict = None, **kwargs):
+        fields = _ or {}
+        fields.update(kwargs)
+        entry = NewEntry(self.logger, self.fields)
+        entry.fields.update(fields)
+        return entry
+
+    def variables(self, *args, currentframe=currentframe2):
+        if not args:
+            return self
+        code = findCallerVariables(currentframe())
+        match = varFieldRegex(code)
+        if not match:
+            self.warning(f"variables regex not match")
+            return self
+        return self.update(dict(zip([field.strip() for field in match.group(1).split(",")], args)))
+
+    def traceback(self):
+        self.update(error=_traceback.format_exc().strip()).error("traceback")
+
+    @contextlib.contextmanager
+    def trycache(self, callback=None, *args, **kwargs):
+        try:
+            yield self
+        except Exception as e:
+            if callback:
+                try:
+                    callback(e, *args, **kwargs)
+                except:
+                    pass
+            self.traceback()
+
+    def _log(self, level: Level, msg: str):
+        entry = NewEntry(self.logger, self.fields)
+        output = entry.logger.formatter.Format(entry, level, msg)
+        entry.logger.FireHooks(entry, level, msg, output)
+        entry.logger.Write(output)
+
+    def log(self, level: Level, msg: str):
+        self._log(level, msg)
+        if level >= PANIC:
+            sys.exit(PANIC.value)
+
+    def debug(self, *args):
+        if self.logger.IsLevelEnabled(DEBUG):
+            self.log(DEBUG, " ".join([f"{arg}" for arg in args]))
+
+    def info(self, *args):
+        if self.logger.IsLevelEnabled(INFO):
+            self.log(INFO, " ".join([f"{arg}" for arg in args]))
+
+    def warning(self, *args):
+        if self.logger.IsLevelEnabled(WARNING):
+            self.log(WARNING, " ".join([f"{arg}" for arg in args]))
+
+    def error(self, *args):
+        if self.logger.IsLevelEnabled(ERROR):
+            self.log(ERROR, " ".join([f"{arg}" for arg in args]))
+
+    def panic(self, *args):
+        if self.logger.IsLevelEnabled(PANIC):
+            self.log(PANIC, " ".join([f"{arg}" for arg in args]))
+
+
+# func
+NewLogger = lambda: Logger()
+AddHooks = lambda *hooks: _logger.AddHooks(*hooks)
+SetLevel = lambda level: _logger.SetLevel(level)
+SetFormatter = lambda formatter: _logger.SetFormatter(formatter)
+CloseColor = lambda: _logger.CloseColor()
+OpenColor = lambda: _logger.OpenColor()
+# entry
+debug = lambda *args: NewEntry().debug(*args)
+info = lambda *args: NewEntry().info(*args)
+warning = lambda *args: NewEntry().warning(*args)
+error = lambda *args: NewEntry().error(*args)
+panic = lambda *args: NewEntry().panic(*args)
+update = lambda _=None, **kwargs: NewEntry().update(_, **kwargs)
+variables = lambda *args: NewEntry().variables(*args, currentframe=currentframe3)
+traceback = lambda: NewEntry().traceback()
+trycache = lambda callback=None, *args, **kwargs: NewEntry().trycache(callback, *args, **kwargs)
+# logger
+_logger = NewLogger()
+_loggerPool = {None: _logger}
+_lock = threading.Lock()
+
+
+def GetLogger(name: str = None):
+    with _lock:
+        if name not in _loggerPool:
+            _loggerPool[name] = NewLogger()
+        return _loggerPool[name]
+
+
+def NewEntry(logger=_logger, fields=None):
+    entry = Entry(logger)
+    if fields:
+        try:
+            fields = deepcopy(fields)
+        except:
+            fields = {f"{key}": f"{value}" for key, value in fields.items()}
+        entry.fields = fields
+    return entry
```

### Comparing `loggus-0.1.1/README.md` & `loggus-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-# loggus
-![Project status](https://img.shields.io/badge/version-0.1.1-green.svg)
-
-基于 python 的结构化日志库。利用 python 动态语言的特性，实现了一些独特功能。
-
-## 如何使用
-```python
-import loggus  # pip install loggus
-
-
-# 日志级别
-loggus.debug("debug")
-loggus.info("info")
-loggus.warning("warning")
-loggus.error("error")
-loggus.panic("panic")  # 程序退出 sys.exit(50)
-
-
-# 结构化日志
-loggus.update({"name":"log", "func": "test"}).info("info")
-loggus.update(name="log", func="test").info("info")
-
-
-# 变量解析
-name = "log"
-funcName = "test"
-loggus.variables(name, funcName).info("info")
-
-
-# 异常traceback
-try:
-    raise
-expect:
-    loggus.traceback()
-
-
-# 异常trycache
-with loggus.trycache():
-    raise 
-
-
-# 自定义Logger（注意：loggus初始化配置将不生效，配置内容见下）
-logger = loggus.GetLogger(__name__)
-```
-
-## 基础配置
-```python
-import loggus
-
-
-# 开启/关闭日志颜色
-loggus.OpenColor()  # 默认
-loggus.CloseColor()
-
-
-# 设置日志级别
-loggus.SetLevel(loggus.INFO)  # 默认
-loggus.SetLevel(loggus.ERROR)
-
-
-# 设置日志格式
-loggus.SetFormatter(loggus.TextFormatter)  # 默认
-loggus.SetFormatter(loggus.JsonFormatter)  # Json格式
-
-
-# 日志钩子
-class LogHook(loggus.IHook):
-    def GetLevels(self) -> list:
-        return [loggus.DEBUG]
-    def Fire(self, entry, level, msg, output) -> None:
-        print(entry, level, msg)
-loggus.AddHooks(LogHook())
-```
+# loggus
+[![PyPI version](https://badge.fury.io/py/loggus.svg)](https://badge.fury.io/py/loggus)
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+loggus 是一个基于 Python 的结构化日志库。与原生的 logging 相比，loggus 提炼了部分关键的结构化字段， 同时简化了结构化日志的使用方式，并改进了日志对象回收机制以确保更优的性能。 此外，loggus 还充分利用了 Python 动态语言的特性，实现了一系列独特的功能。
+
+## 快速开始
+```python
+import loggus  # pip install loggus
+
+
+# 日志级别
+loggus.debug("debug")
+loggus.info("info")
+loggus.warning("warning")
+loggus.error("error")
+loggus.panic("panic")  # 程序退出 sys.exit(50)
+
+
+# 结构化日志
+loggus.update({"name":"log", "func": "test"}).info("info")
+loggus.update(name="log", func="test").info("info")
+
+
+# 变量解析
+name = "log"
+funcName = "test"
+loggus.variables(name, funcName).info("info")
+
+
+# 异常traceback
+try:
+    raise
+expect:
+    loggus.traceback()
+
+
+# 异常trycache
+with loggus.trycache():
+    raise 
+
+
+# 自定义Logger（注意：loggus初始化配置将不生效，配置内容见下）
+logger = loggus.GetLogger(__name__)
+```
+
+## 基础配置
+```python
+import loggus
+
+
+# 开启/关闭日志颜色
+loggus.OpenColor()  # 默认
+loggus.CloseColor()
+
+
+# 设置日志级别
+loggus.SetLevel(loggus.INFO)  # 默认
+loggus.SetLevel(loggus.ERROR)
+
+
+# 设置日志格式
+loggus.SetFormatter(loggus.TextFormatter)  # 默认
+loggus.SetFormatter(loggus.JsonFormatter)  # Json格式
+
+
+# 日志钩子
+class LogHook(loggus.IHook):
+    def GetLevels(self) -> list:
+        return [loggus.DEBUG]
+    def Fire(self, entry, level, msg, output) -> None:
+        print(entry, level, msg)
+loggus.AddHooks(LogHook())
+```
```

### Comparing `loggus-0.1.1/setup.py` & `loggus-0.1.2/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import os
-import re
-import codecs
-
-from setuptools import setup, find_packages
-
-"""pip install twine
-1、python setup.py check
-2、python setup.py sdist
-3、twine upload dist/__packages__-__version__.tar.gz
-"""
-
-"""MANIFEST.in
-global-include pat1 pat2 ... > Include all files anywhere
-global-exclude pat1 pat2 ... > Exclude all files anywhere
-graft dir-pattern > Include all files under directories matching dir-pattern
-prune dir-pattern > Exclude all files under directories matching dir-pattern
-
-such as: global-exclude *.py[cod]
-"""
-
-
-def read(*parts):
-    here = os.path.abspath(os.path.dirname(__file__))
-    return codecs.open(os.path.join(here, *parts), 'r', encoding='utf-8').read()
-
-
-def find_version(*file_paths):
-    version_file = read(*file_paths)
-    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
-    if version_match:
-        return version_match.group(1)
-    else:
-        raise RuntimeError("Unable to find version string.")
-
-
-setup(
-    name='loggus',
-    version=find_version('loggus', '__init__.py'),
-    description="基于 python 的结构化日志库。利用 python 动态语言的特性，实现了一些独特功能。",
-    long_description="see https://github.com/czasg/loggus",
-    author='czasg',
-    author_email='972542644@qq.com',
-    url='https://github.com/czasg/loggus',
-    packages=find_packages(),
-    install_requires=[
-        "colorama",
-        "coverage",
-    ],
-    classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-    ],
-)
+import os
+import re
+import codecs
+
+from setuptools import setup, find_packages
+
+"""pip install twine
+1、python setup.py check
+2、python setup.py sdist
+3、twine upload dist/__packages__-__version__.tar.gz
+"""
+
+"""MANIFEST.in
+global-include pat1 pat2 ... > Include all files anywhere
+global-exclude pat1 pat2 ... > Exclude all files anywhere
+graft dir-pattern > Include all files under directories matching dir-pattern
+prune dir-pattern > Exclude all files under directories matching dir-pattern
+
+such as: global-exclude *.py[cod]
+"""
+
+
+def read(*parts):
+    here = os.path.abspath(os.path.dirname(__file__))
+    return codecs.open(os.path.join(here, *parts), 'r', encoding='utf-8').read()
+
+
+def find_version(*file_paths):
+    version_file = read(*file_paths)
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
+    if version_match:
+        return version_match.group(1)
+    else:
+        raise RuntimeError("Unable to find version string.")
+
+
+setup(
+    name='loggus',
+    version=find_version('loggus', '__init__.py'),
+    description="基于 python 的结构化日志库。利用 python 动态语言的特性，实现了一些独特功能。",
+    long_description="see https://github.com/czasg/loggus",
+    author='czasg',
+    author_email='972542644@qq.com',
+    url='https://github.com/czasg/loggus',
+    packages=find_packages(),
+    install_requires=[
+        "colorama",
+        "coverage",
+    ],
+    classifiers=[
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+    ],
+)
```

