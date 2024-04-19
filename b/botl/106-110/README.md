# Comparing `tmp/botl-106.tar.gz` & `tmp/botl-110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botl-106.tar", last modified: Thu Apr  4 12:25:42 2024, max compression
+gzip compressed data, was "botl-110.tar", last modified: Fri Apr 19 12:06:46 2024, max compression
```

## Comparing `botl-106.tar` & `botl-110.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.689670 botl-106/
--rw-r--r--   0 bart      (1000) bart      (1000)     3963 2024-04-04 12:25:42.689670 botl-106/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3440 2024-04-04 12:15:24.000000 botl-106/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.685670 botl-106/botl/
--rw-r--r--   0 bart      (1000) bart      (1000)       80 2024-04-04 11:34:13.000000 botl-106/botl/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4026 2024-04-04 12:07:39.000000 botl-106/botl/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      904 2024-04-04 11:48:34.000000 botl-106/botl/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1582 2024-04-04 12:05:43.000000 botl-106/botl/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)      321 2024-04-04 11:47:18.000000 botl-106/botl/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1733 2024-04-04 11:47:57.000000 botl-106/botl/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      865 2024-04-04 11:46:43.000000 botl-106/botl/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1608 2024-04-04 12:10:33.000000 botl-106/botl/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.689670 botl-106/botl/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      436 2024-04-04 11:31:06.000000 botl-106/botl/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      220 2024-04-04 11:38:19.000000 botl-106/botl/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      229 2024-04-04 12:11:53.000000 botl-106/botl/modules/dbg.py
--rw-r--r--   0 bart      (1000) bart      (1000)      534 2024-04-04 11:31:06.000000 botl-106/botl/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      405 2024-04-04 11:38:51.000000 botl-106/botl/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      800 2024-04-04 11:40:01.000000 botl-106/botl/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    18973 2024-04-04 11:40:19.000000 botl-106/botl/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      825 2024-04-04 11:40:51.000000 botl-106/botl/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2469 2024-04-04 11:41:08.000000 botl-106/botl/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    16437 2024-04-04 11:41:23.000000 botl-106/botl/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      245 2024-04-04 11:41:42.000000 botl-106/botl/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2409 2024-04-04 11:42:03.000000 botl-106/botl/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    10919 2024-04-04 11:42:15.000000 botl-106/botl/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3195 2024-04-04 11:42:35.000000 botl-106/botl/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1181 2024-04-04 11:42:49.000000 botl-106/botl/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1061 2024-04-04 11:43:07.000000 botl-106/botl/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5240 2024-04-04 11:43:22.000000 botl-106/botl/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3137 2024-04-04 11:43:38.000000 botl-106/botl/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6154 2024-04-04 11:48:18.000000 botl-106/botl/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-04 11:48:07.000000 botl-106/botl/parser.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3435 2024-04-04 11:46:19.000000 botl-106/botl/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      344 2024-04-04 11:47:29.000000 botl-106/botl/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2029 2024-04-04 12:10:16.000000 botl-106/botl/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1151 2024-04-04 11:46:52.000000 botl-106/botl/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-04 11:47:07.000000 botl-106/botl/utils.py
--rw-r--r--   0 bart      (1000) bart      (1000)      779 2024-04-04 12:09:42.000000 botl-106/botl/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.689670 botl-106/botl.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3963 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      812 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       47 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      840 2024-04-04 12:16:12.000000 botl-106/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-04 12:25:42.689670 botl-106/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-04 11:31:06.000000 botl-106/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.154775 botl-110/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-19 12:06:46.154775 botl-110/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3438 2024-04-19 11:31:35.000000 botl-110/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.150776 botl-110/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     2261 2024-04-19 12:00:28.000000 botl-110/bin/botl
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     4474 2024-04-19 11:54:20.000000 botl-110/bin/botlbot
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     2384 2024-04-19 11:31:26.000000 botl-110/bin/botld
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.150776 botl-110/botl/
+-rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-19 11:09:23.000000 botl-110/botl/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1364 2024-04-19 11:09:23.000000 botl-110/botl/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-19 11:09:23.000000 botl-110/botl/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1922 2024-04-19 11:09:23.000000 botl-110/botl/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-19 11:09:23.000000 botl-110/botl/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1089 2024-04-19 11:09:23.000000 botl-110/botl/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-19 11:09:23.000000 botl-110/botl/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1930 2024-04-19 11:09:23.000000 botl-110/botl/find.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1362 2024-04-19 11:09:23.000000 botl-110/botl/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.154775 botl-110/botl/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      500 2024-04-19 11:35:02.000000 botl-110/botl/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-04-19 11:11:55.000000 botl-110/botl/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      403 2024-04-19 11:13:15.000000 botl-110/botl/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-19 11:13:31.000000 botl-110/botl/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      834 2024-04-19 11:13:58.000000 botl-110/botl/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17621 2024-04-19 11:25:12.000000 botl-110/botl/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      776 2024-04-19 11:15:36.000000 botl-110/botl/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      371 2024-04-19 11:36:24.000000 botl-110/botl/modules/man.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3552 2024-04-19 11:16:02.000000 botl-110/botl/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17081 2024-04-19 11:16:31.000000 botl-110/botl/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      240 2024-04-19 11:16:41.000000 botl-110/botl/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2400 2024-04-19 11:16:52.000000 botl-110/botl/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    11001 2024-04-19 11:12:04.000000 botl-110/botl/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2761 2024-04-19 11:19:37.000000 botl-110/botl/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1184 2024-04-19 11:17:55.000000 botl-110/botl/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1038 2024-04-19 11:18:07.000000 botl-110/botl/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5130 2024-04-19 11:18:37.000000 botl-110/botl/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2933 2024-04-19 11:18:56.000000 botl-110/botl/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5799 2024-04-19 11:19:09.000000 botl-110/botl/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-19 11:09:23.000000 botl-110/botl/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-19 11:07:31.000000 botl-110/botl/parser.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      752 2024-04-19 11:09:23.000000 botl-110/botl/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-19 11:09:23.000000 botl-110/botl/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-19 11:09:23.000000 botl-110/botl/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-19 11:09:23.000000 botl-110/botl/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-19 11:09:23.000000 botl-110/botl/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-19 11:07:31.000000 botl-110/botl/utils.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1101 2024-04-19 11:09:23.000000 botl-110/botl/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.154775 botl-110/botl.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      860 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      857 2024-04-19 12:03:01.000000 botl-110/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-19 12:06:46.154775 botl-110/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      196 2024-04-19 12:01:22.000000 botl-110/setup.py
```

### Comparing `botl-106/PKG-INFO` & `botl-110/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 106
+Version: 110
 Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
@@ -142,28 +142,28 @@
     rss - add a feed
     thr - show the running threads
 
 SYSTEMD
 
 ::
 
-    save the following it in /etc/systems/system/botl.service and
+    save the following it in /etc/systemd/system/botl.service and
     replace "<user>" with the user running pipx
 
     [Unit]
     Description=bot library
     Requires=network-online.target
     After=network-online.target
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.botl
-    ExecStart=/home/<user>/.local/pipx/venvs/botl/bin/botl -d
+    ExecStart=/home/<user>/.local/pipx/venvs/botl/bin/botld
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
```

### Comparing `botl-106/README.rst` & `botl-110/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -126,28 +126,28 @@
     rss - add a feed
     thr - show the running threads
 
 SYSTEMD
 
 ::
 
-    save the following it in /etc/systems/system/botl.service and
+    save the following it in /etc/systemd/system/botl.service and
     replace "<user>" with the user running pipx
 
     [Unit]
     Description=bot library
     Requires=network-online.target
     After=network-online.target
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.botl
-    ExecStart=/home/<user>/.local/pipx/venvs/botl/bin/botl -d
+    ExecStart=/home/<user>/.local/pipx/venvs/botl/bin/botld
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
```

### Comparing `botl-106/botl/__main__.py` & `botl-110/bin/botlbot`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,119 @@
+#!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212
+# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,E0611
 # ruff: noqa: E402
 
 
+"""NAME
+
+    BOTL - bot library
+
+SYNOPSIS
+
+    botl <cmd> [key=val] [key==val]
+
+OPTIONS
+
+    -a     load all modules
+    -c     start console
+    -d     start daemon
+    -h     display help
+    -v     use verbose
+
+EXAMPLE
+
+    botl -cav
+
+COPYRIGHT
+
+    BOTL is Public Domain."""
+
+
 "main"
 
 
 import getpass
 import os
 import pwd
+import readline # pylint: disable=W0611
 import sys
 import termios
 import time
 
 
-from .client  import Client, cmnd
-from .default import Default
-from .errors  import Errors,debug
-from .event   import Event
-from .object  import cdir
-from .parser  import parse_cmd
-from .utils   import spl
-from .workdir import Workdir
-
-
-from . import modules
-
-
-Cfg          = Default()
-Cfg.mod      = "cmd,mod"
-Cfg.name     = "botl"
-Cfg.version  = "106"
-Cfg.dir      = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile  = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.workdir = Cfg.dir
+sys.path.insert(0, os.getcwd())
+
+
+from botl.client  import Client, cmnd, parse_cmd, spl
+from botl.command import Command
+from botl.default import Default
+from botl.errors  import debug, enable, errors
+from botl.event   import Event
+from botl.object  import cdir
+from botl.runtime  import broker
+from botl.workdir import Workdir, skel
+
+
+from botl import modules
+
+
+if os.path.exists("mods"):
+    import mods
+else:
+    mods = None
+
+
+Cfg             = Default()
+Cfg.mod         = "cmd,mod"
+Cfg.opts        = ""
+Cfg.name        = "botl"
+Cfg.version     = "552"
+Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
+Workdir.workdir = Cfg.wd
 
 
 dte = time.ctime(time.time()).replace("  ", " ")
-ext = os._exit 
 
 
 class Console(Client):
 
-    "Console"
+    def __init__(self):
+        Client.__init__(self)
+        broker.add(self)
 
     def announce(self, txt):
-        "blind announce"
+        pass
 
     def callback(self, evt):
-        "run and wait for callback to finish."
         Client.callback(self, evt)
-        evt.wait(5.0)
+        evt.wait()
 
     def poll(self):
-        "reconstruct event from input."
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
-    def say(self, _channel, txt):
-        "say text in channel."
+    def say(self, channel, txt):
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
 def daemon(pidfile, verbose=False):
-    "fork into the background."
     pid = os.fork()
     if pid != 0:
-        ext(0)
+        os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
-        ext(0)
+        os._exit(0)
     if not verbose:
         with open('/dev/null', 'r', encoding="utf-8") as sis:
             os.dup2(sis.fileno(), sys.stdin.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as sos:
             os.dup2(sos.fileno(), sys.stdout.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as ses:
             os.dup2(ses.fileno(), sys.stderr.fileno())
@@ -88,38 +122,33 @@
     if os.path.exists(pidfile):
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
-def init(pkg, modstr, disable=""):
-    "start inits in modules."
+def init(pkg, modstr):
     mds = []
     for modname in spl(modstr):
-        if modname in spl(disable):
-            continue
         module = getattr(pkg, modname, None)
         if not module:
             continue
         if "init" in dir(module):
             module.init()
             mds.append(module)
     return mds
 
 
 def privileges(username):
-    "lower privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
 def wrap(func):
-    "restore terminal"
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
@@ -127,55 +156,59 @@
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
 def ver(event):
-    "show version."
     event.reply(f"{Cfg.name.upper()} {Cfg.version}")
 
 
-"runtime"
-
-
 def main():
-    "main code"
-    Workdir.skel()
-    Errors.enable(print)
-    #Client.add(ver)
+    Command.add(ver)
+    enable(print)
+    skel()
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
-    result = None
     if 'a' in Cfg.opts:
-        Cfg.mod = "," + ",".join(modules.__dir__())
+        Cfg.mod = ",".join(modules.__dir__())
+        if mods:
+            Cfg.mod += "," + ",".join(mods.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
     if "h" in Cfg.opts:
         print(__doc__)
-        return result
+        return
     if "d" in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
         Cfg.user = getpass.getuser()
         daemon(Cfg.pidfile, "v" in Cfg.opts)
         privileges(Cfg.user)
         init(modules, Cfg.mod)
         while 1:
             time.sleep(1.0)
-    elif "c" in Cfg.opts:
+        return
+    if "c" in Cfg.opts:
         init(modules, Cfg.mod)
+        if mods:
+            Cfg.mod += "," + ",".join(mods.__dir__())
+            init(mods, Cfg.mod)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
-    elif Cfg.otxt:
-        cmnd(Cfg.otxt, print)
-    return result
+        return
+    if Cfg.otxt:
+        return cmnd(Cfg.otxt, print)
+
+
+def daemoned():
+    Cfg.opts += "d"
+    main()
 
 
 def wrapped():
-    "wrapped code"
     wrap(main)
-    Errors.show()
+    errors()
 
 
 if __name__ == "__main__":
     wrapped()
```

### Comparing `botl-106/botl/event.py` & `botl-110/botl/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,41 +14,29 @@
 
 class Event(Default):
 
     "Event"
 
     def __init__(self):
         Default.__init__(self)
+        self._thr    = None
         self._ready  = threading.Event()
         self.done    = False
         self.orig    = None
         self.result  = []
-        self.thr    = None
         self.txt     = ""
         self.type    = "event"
 
     def ready(self):
         "event is ready."
         self._ready.set()
 
     def reply(self, txt):
         "add text to the result"
         self.result.append(txt)
 
-    def wait(self, sec=None):
+    def wait(self):
         "wait for event to be ready."
-        if self.thr:
-            self.thr.join()
-        self._ready.wait(sec)
+        if self._thr:
+            self._thr.join()
+        self._ready.wait()
         return self.result
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Event',
-    )
-
-
-__all__ = __dir__()
```

### Comparing `botl-106/botl/handler.py` & `botl-110/botl/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212,W0718
+# pylint: disable=C,R,W0105,W0212
 
 
 "handler"
 
 
 import queue
 import threading
 import _thread
 
 
-from .errors  import Errors
-from .object  import Object
-from .thread  import launch
+from .object import Object
+from .thread import launch
 
 
 class Handler:
 
     "Handler"
 
     def __init__(self):
-        self.cbs = Object()
+        self.cbs      = Object()
         self.queue    = queue.Queue()
         self.stopped  = threading.Event()
         self.threaded = True
 
     def callback(self, evt):
         "call callback based on event type."
         func = getattr(self.cbs, evt.type, None)
-        if func:
-            if self.threaded:
-                evt._thr = launch(func, evt)
-            else:
-                func(evt)
+        if not func:
+            evt.ready()
+            return
+        evt._thr = launch(func, self, evt)
 
     def loop(self):
         "proces events until interrupted."
         while not self.stopped.is_set():
             try:
                 evt = self.poll()
                 self.callback(evt)
             except (KeyboardInterrupt, EOFError):
                 _thread.interrupt_main()
-            except Exception as ex:
-                Errors.add(ex)
-                evt.ready()
 
     def poll(self):
         "function to return event."
         return self.queue.get()
 
     def put(self, evt):
         "put event into the queue."
@@ -62,19 +57,7 @@
     def start(self):
         "start the event loop."
         launch(self.loop)
 
     def stop(self):
         "stop the event loop."
         self.stopped.set()
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Handler',
-    )
-
-
-__all__ = __dir__()
```

### Comparing `botl-106/botl/modules/fnd.py` & `botl-110/botl/modules/tdo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,70 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=C,R,E0402
 
 
-"find"
+"todo list"
 
 
-from ..client  import Client
-from ..object  import fmt
-from ..persist import Persist, Workdir, find
+import time
 
 
-def fnd(event):
-    "find objects."
-    Workdir.skel()
-    if not event.rest:
-        res = sorted([x.split('.')[-1].lower() for x in Workdir.types()])
-        if res:
-            event.reply(",".join(res))
+from ..client  import laps
+from ..object  import Object
+from ..command import Command
+from ..find    import fntime, find
+from ..persist import whitelist
+from ..workdir import sync
+
+
+class NoDate(Exception):
+
+    pass
+
+
+class Todo(Object):
+
+    def __init__(self):
+        Object.__init__(self)
+        self.txt = ''
+
+
+whitelist(Todo)
+
+
+def dne(event):
+    if not event.args:
+        event.reply("dne <txt>")
         return
-    otype = event.args[0]
-    clz = Persist.long(otype)
-    if "." not in clz:
-        for fnm in Workdir.types():
-            claz = fnm.split(".")[-1]
-            if otype == claz.lower():
-                clz = fnm
+    selector = {'txt': event.args[0]}
     nmr = 0
-    for fnm, obj in find(clz, event.gets):
-        event.reply(f"{nmr} {fmt(obj)}")
+    for fnm, obj in find('todo', selector):
         nmr += 1
+        obj.__deleted__ = True
+        sync(obj, fnm)
+        event.reply('ok')
+        break
     if not nmr:
-        event.reply("no result")
+        event.reply("nothing todo")
+
+
+Command.add(dne)
+
+
+def tdo(event):
+    if not event.rest:
+        nmr = 0
+        for fnm, obj in find('todo'):
+            lap = laps(time.time()-fntime(fnm))
+            event.reply(f'{nmr} {obj.txt} {lap}')
+            nmr += 1
+        if not nmr:
+            event.reply("no todo")
+        return
+    obj = Todo()
+    obj.txt = event.rest
+    sync(obj)
+    event.reply('ok')
 
 
-Client.add(fnd)
+Command.add(tdo)
```

### Comparing `botl-106/botl/modules/irc.py` & `botl-110/botl/modules/irc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0718
+# pylint: disable=C,R,W0105,W0612,W0718,E0402,W0201,W0603
 # ruff: noqa: F841
 
 
 "internet relay chat"
 
 
 import base64
@@ -14,56 +14,61 @@
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from ..broker  import Broker
-from ..client  import Client
+from ..client  import Client, command
+from ..command import Command
 from ..default import Default
+from ..errors  import debug, later
 from ..event   import Event
-from ..errors  import Errors, debug
+from ..find    import last
 from ..object  import Object, edit, fmt, keys
-from ..persist import Persist, last, sync
+from ..persist import whitelist
+from ..runtime import broker
 from ..thread  import launch
+from ..workdir import sync
 
 
-NAME    = __file__.split(os.sep)[-3]
-get     = Broker.get
-saylock = _thread.allocate_lock()
+NAME       = __file__.split(os.sep)[-3]
+filterlist = ["PING", "PONG", "PRIVMSG"]
+saylock    = _thread.allocate_lock()
 
 
-Errors.filter = ["PING", "PONG", "PRIVMSG"]
+myirc = None
 
 
+def dbg(txt):
+    for flt in filterlist:
+        if flt in txt:
+            return
+    debug(txt)
+
 def init():
-    "initialize a irc bot."
+    global myirc
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
+    myirc = irc
     return irc
 
 
 def shutdown():
-    "shutdown irc bot."
-    for bot in Broker.all():
-        if "irc" not in type(bot):
-            continue
-        debug(f"IRC stopping {repr(bot)}")
-        bot.state.pongcheck = True
-        bot.state.keeprunning = False
-        bot.events.connected.clear()
-        bot.stop()
+    dbg(f"IRC stopping {myirc}")
+    if myirc:
+        myirc.state.pongcheck = True
+        myirc.state.keeprunning = False
+        myirc.events.connected.clear()
+        myirc.stop()
 
 
 class Config(Default):
 
-    "Config"
-
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
     realname = NAME
@@ -82,21 +87,19 @@
         self.nick = self.nick or Config.nick
         self.port = self.port or Config.port
         self.realname = self.realname or Config.realname
         self.server = self.server or Config.server
         self.username = self.username or Config.username
 
 
-Persist.add(Config)
+whitelist(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
-    "TextWrap"
-
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -104,54 +107,47 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
-    "Output"
-
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
-        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
-        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
         chanlist = getattr(Output.cache, channel)
         chanlist.extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
-        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
-        "put text to output queue."
         if channel and channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
-        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -166,24 +162,21 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
-        "return size of channel cache."
         if chan in Output.cache:
             return len(getattr(Output.cache, chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
-    "IRC"
-
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
         self.channels = []
         self.events = Default()
@@ -206,23 +199,21 @@
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
-        Broker.add(self)
+        broker.add(self)
 
     def announce(self, txt):
-        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
     def docommand(self, cmd, *args):
-        "send command to server."
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -231,19 +222,18 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
-        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
-            debug("using SASL")
+            dbg("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.options |= ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1
             ctx.minimum_version = ssl.TLSVersion.TLSv1_2
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
@@ -258,51 +248,47 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
-        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
-        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as _ex:
+               ) as ex:
             pass
         except Exception as ex:
-            Errors.add(ex)
+            later(ex)
 
     def doconnect(self, server, nck, port=6667):
-        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
                 self.state.error = str(ex)
-                debug(str(ex))
-            debug(f"sleeping {self.cfg.sleep} seconds")
+                dbg(str(ex))
+            dbg(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
-        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.docommand('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
@@ -321,53 +307,49 @@
         elif cmd == '433':
             self.state.error = txt
             nck = self.cfg.nick + '_'
             self.docommand('NICK', nck)
         return evt
 
     def joinall(self):
-        "join all channels."
         for channel in self.channels:
             self.docommand('JOIN', channel)
 
     def keep(self):
-        "keep alive."
         while not self.stopped.is_set():
             if self.state.stopkeep:
                 self.state.stopkeep = False
                 break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.docommand('PING', self.cfg.server)
             if self.state.pongcheck:
-                debug("failed pongcheck, restarting")
+                dbg("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
-        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
-        "parse text into an event."
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
-        debug(txt)
+        dbg(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
@@ -417,15 +399,14 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
-        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -433,87 +414,81 @@
                     OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Errors.add(ex)
+                later(ex)
                 self.stop()
-                debug("handler stopped")
+                dbg("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
-        "send raw text."
         txt = txt.rstrip()
-        debug(txt)
+        dbg(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
                     OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Errors.add(ex)
+                later(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        "reconnect to server."
-        debug(f"reconnecting to {self.cfg.server}")
+        dbg(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
-        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.docommand('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
-        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
-        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
-        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
         launch(Client.start, self)
@@ -523,122 +498,101 @@
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        "stop bot."
         self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
-        "wait for ready."
         self.events.ready.wait()
 
 
-def cb_auth(evt):
-    "auth callback."
-    bot = get(evt.orig)
+def cb_auth(bot, evt):
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
-def cb_cap(evt):
-    "capabilities callback."
-    bot = get(evt.orig)
+def cb_cap(bot, evt):
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
-def cb_error(evt):
-    "error callback."
-    bot = get(evt.orig)
+def cb_error(bot, evt):
     if not bot.state.nrerror:
         bot.state.nrerror = 0
     bot.state.nrerror += 1
     bot.state.error = evt.txt
-    debug(evt.txt)
+    dbg(evt.txt)
 
 
-def cb_h903(evt):
-    "auth succeded callback."
-    bot = get(evt.orig)
+def cb_h903(bot, evt):
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_h904(evt):
-    "auth succeded callback."
-    bot = get(evt.orig)
+def cb_h904(bot, evt):
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_kill(evt):
-    "got killed callback."
+def cb_kill(bot, evt):
+    pass
 
 
-def cb_log(evt):
-    "log callback."
+def cb_log(bot, evt):
+    pass
 
 
-def cb_ready(evt):
-    "bot is ready callback."
-    bot = get(evt.orig)
-    if bot:
-        bot.events.ready.set()
+def cb_ready(bot, evt):
+    bot.events.ready.set()
 
 
-def cb_001(evt):
-    "first line received callback."
-    bot = get(evt.orig)
+def cb_001(bot, evt):
     bot.logon()
 
 
-def cb_notice(evt):
-    "notice callback."
-    bot = get(evt.orig)
+def cb_notice(bot, evt):
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
         bot.docommand('NOTICE', evt.channel, txt)
 
 
-def cb_privmsg(evt):
-    "privmsg callback."
-    bot = get(evt.orig)
+def cb_privmsg(bot, evt):
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
-        debug(f"command from {evt.origin}: {evt.txt}")
-        bot.command(evt)
+        dbg(f"command from {evt.origin}: {evt.txt}")
+        command(bot, evt)
 
 
-def cb_quit(evt):
-    "quit callback."
-    bot = get(evt.orig)
-    debug(f"quit from {bot.cfg.server}")
+def cb_quit(bot, evt):
+    dbg(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
+"commands"
+
+
 def cfg(event):
-    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
@@ -647,48 +601,46 @@
                    )
     else:
         edit(config, event.sets)
         sync(config, path)
         event.reply('ok')
 
 
-Client.add(cfg)
+Command.add(cfg)
 
 
 def mre(event):
-    "show from output cache."
     if not event.channel:
         event.reply('channel is not set.')
         return
-    bot = Broker.get(event.orig)
+    bot = broker.get(event.orig)
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
     if event.channel not in bot.cache:
         event.reply(f'no output in {event.channel} cache.')
         return
     for _x in range(3):
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
     event.reply(f'{size} more in cache')
 
 
-Client.add(mre)
+Command.add(mre)
 
 
 def pwd(event):
-    "create a base64 password."
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
 
 
-Client.add(pwd)
+Command.add(pwd)
```

### Comparing `botl-106/botl/modules/log.py` & `botl-110/botl/modules/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=R,C,E0402
 
 
 "log text"
 
 
 import time
 
 
-from ..client  import Client
+from ..client  import laps
+from ..command import Command
 from ..object  import Object
-from ..persist import Persist, find, fntime, sync
-from ..utils   import laps
+from ..find    import find, fntime
+from ..workdir import  sync
+from ..persist import whitelist
 
 
 class Log(Object):
 
-    "Log"
-
     def __init__(self):
-        Object.__init__()
+        super().__init__()
         self.txt = ''
 
-    def __yo__(self):
-        pass
-
-    def __yoyo__(self):
-        pass
-
 
-Persist.add(Log)
+whitelist(Log)
 
 
 def log(event):
-    "log text."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
@@ -46,8 +39,8 @@
         return
     obj = Log()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
 
 
-Client.add(log)
+Command.add(log)
```

### Comparing `botl-106/botl/modules/mdl.py` & `botl-110/botl/modules/mdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=C,R,W0613,E0402,W0105
 
 
 "genocide model of the netherlands"
 
 
 import datetime
 import time
 
 
-from ..broker   import Broker
-from ..client   import Client
+from ..client   import laps
+from ..command  import Command
 from ..event    import Event
-from ..object   import Object, construct, keys
+from ..object   import Object, construct, keys, values
 from ..repeater import Repeater
+from ..runtime  import broker
 from ..thread   import launch
-from ..utils    import laps
 
 
-def __dir__():
-    return (
-            'init',
-            'now'
-           )
+DAY = 24*60*60
+YEAR = 365*DAY
+SOURCE = "https://github.com/bthate/genocide"
+STARTDATE = "2020-01-01 00:00:00"
+STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
 
 def init():
-    "start genocide model."
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
             repeater = Repeater(sec, cbstats, evt, thrname=aliases.get(key))
             repeater.start()
     launch(daily, name="daily")
-
-
-DAY = 24*60*60
-YEAR = 365*DAY
-SOURCE = "https://github.com/bthate/genocide"
-STARTDATE = "2020-01-01 00:00:00"
-STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
+    
 
 
 oor = """"Totaal onderliggende doodsoorzaken (aantal)";
          "1 Infectieuze en parasitaire ziekten/Totaal infectieuze en parasitaire zktn (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.1 Tuberculose (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.2 Meningokokkeninfecties (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.3 Virale hepatitis (aantal)";
@@ -280,123 +273,134 @@
 
 oorzaak = Object()
 construct(oorzaak, zip(oor, aantal))
 oorzaken = Object()
 
 
 def getalias(txt):
-    "teturn matching alias."
-    result = None
     for key, value in aliases.items():
         if txt.lower() in key.lower():
-            result = value
-            break
-    return result
+            return value
 
 
 def getday():
-    "return timestamp of current day."
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
-    "return number of deaths by name."
     for k in keys(oorzaken):
         if name.lower() in k.lower():
             return int(getattr(oorzaken, k))
     return 0
 
 
 def seconds(nrs):
-    "calculate sedconds"
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
 
 def iswanted(k, line):
-    "see whether an item is wanted."
     for word in line:
         if word in k:
             return True
     return False
 
 
 def daily():
-    "run a callback daily."
     while 1:
         time.sleep(24*60*60)
-        cbnow(Event())
+        evt = Event()
+        cbnow(evt)
 
 
 def hourly():
-    "run a callback hourly."
     while 1:
         time.sleep(60*60)
-        cbnow(Event())
+        evt = Event()
+        cbnow(evt)
 
 
 def cbnow(evt):
-    "check status now callback."
-    if not evt:
-        evt = Event()
     delta = time.time() - STARTTIME
     txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
-        txt += f"{getalias(name)}: {nrtimes}"
+        txt += "%s: %s " % (getalias(name), nrtimes)
     txt += " http://genocide.rtfd.io"
-    for bot in Broker.all():
+    for bot in values(broker.objs):
         if "announce" in dir(bot):
             bot.announce(txt)
 
 
 def cbstats(evt):
-    "callback showing stats."
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
-        nrt = int(delta/needed)
-        nry = int(YEAR/needed)
-        nrd = int(DAY/needed)
+        nrtimes = int(delta/needed)
+        nryear = int(YEAR/needed)
+        nrday = int(DAY/needed)
         delta2 = time.time() - getday()
-        this = int(delta2/needed)
-        txt = f"#{nrt} died from {getalias(name)} ({this}/{nrd}) every {laps(needed)} ({nry}/year)"
-        for bot in Broker.all():
+        thisday = int(delta2/needed)
+        txt = "patient #%s died from %s (%s/%s) every %s (%s/year)" % (
+                                                               nrtimes,
+                                                               getalias(name),
+                                                               thisday,
+                                                               nrday,
+                                                               laps(needed),
+                                                               nryear,
+                                                              )
+        for bot in values(broker.objs):
             bot.announce(txt)
 
 
 def now(event):
-    "showing number of psychiatric patients victims."
     name = event.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         txt = laps(delta) + " "
-        nrt = int(delta/needed)
-        nrd = int(DAY/needed)
-        this = int(DAY % needed)
-        txt = f"#{nrt} died from {getalias(name)} ({this}/{nrd}) every {laps(needed)}"
+        nrtimes = int(delta/needed)
+        nryear = int(YEAR/needed)
+        nrday = int(DAY/needed)
+        thisday = int(DAY % needed)
+        txt += "patient #%s died from %s (%s/%s/%s) every %s" % (
+                                                                 nrtimes,
+                                                                 getalias(name),
+                                                                 thisday,
+                                                                 nrday,
+                                                                 nryear,
+                                                                 laps(needed)
+                                                                )
         event.reply(txt)
     else:
         event.reply("not needed")
 
 
-Client.add(now)
+Command.add(now)
+
+
+"interface"
+
+
+def __dir__():
+    return (
+            'init',
+            'now'
+           ) 
 
 
 def boot():
-    "format model data."
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
         if _nr == 0:
             continue
         if key.startswith('"'):
             key = key[1:]
```

### Comparing `botl-106/botl/modules/req.py` & `botl-110/botl/modules/req.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C.R
+# pylint: disable=C0115,C0116
 
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
@@ -75,16 +75,15 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
-from ..client import Client
+from ..command import Command
 
 
 def req(event):
-    "show request."
     event.reply(__doc__)
 
 
-Client.add(req)
+Command.add(req)
```

### Comparing `botl-106/botl/modules/rss.py` & `botl-110/botl/modules/rss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=C,R,W0105
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -14,22 +14,24 @@
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..broker   import Broker
-from ..client   import Client
+from ..client   import laps, spl
+from ..command  import Command
 from ..default  import Default
-from ..object   import Object, fmt, update
-from ..persist  import Persist, find, fntime, last, sync
+from ..find     import find, fntime, last
+from ..object   import Object, fmt, update, values
+from ..persist  import whitelist
 from ..repeater import Repeater
+from ..runtime  import broker
 from ..thread   import launch
-from ..utils    import laps, spl
+from ..workdir  import sync
 
 
 def init():
     "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
@@ -37,14 +39,22 @@
 
 DEBUG = False
 
 
 fetchlock = _thread.allocate_lock()
 
 
+TEMPLATE = """<opml version="1.0">
+    <head>
+        <title>rssbot opml</title>
+    </head>
+    <body>
+        <outline title="rssbot opml" text="24/7 feed fetcher">"""
+
+
 class Feed(Default):
 
     "Feed"
 
 
 class Rss(Default):
 
@@ -52,29 +62,23 @@
 
     def __init__(self):
         Default.__init__(self)
         self.display_list = 'title,link,author'
         self.rss          = ''
 
 
-Persist.add(Rss)
-
-
 class Seen(Default):
 
     "Seen"
 
     def __init__(self):
         Default.__init__(self)
         self.urls = []
 
 
-Persist.add(Seen)
-
-
 class Fetcher(Object):
 
     "Fetcher"
 
     def __init__(self):
         self.dosave = False
         self.seen = Seen()
@@ -127,15 +131,15 @@
             sync(self.seen, self.seenfn)
         txt = ''
         feedname = getattr(feed, 'name', None)
         if feedname:
             txt = f'[{feedname}] '
         for obj in result:
             txt2 = txt + self.display(obj)
-            for bot in Broker.all():
+            for bot in values(broker.objs):
                 if "announce" in dir(bot):
                     bot.announce(txt2.rstrip())
         return counter
 
     def run(self):
         "fetch all feeds."
         thrs = []
@@ -316,95 +320,83 @@
 
 
 def useragent(txt):
     "return useragent."
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
+"commands"
+
+
 def dpl(event):
     "set display items."
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
     for _fn, feed in find('rss', {'rss': event.args[0]}):
         if feed:
             update(feed, setter)
             sync(feed)
     event.reply('ok')
 
 
-Client.add(dpl)
-
-
 def exp(event):
     "export to opml."
     event.reply(TEMPLATE)
     nrs = 0
     for _fn, obj in find("rss"):
         nrs += 1
         name = obj.name or f"url{nrs}"
         txt = f'<outline name={name} display_list={obj.display_list} xmlUrl="{obj.rss}"/>'
         event.reply(" "*12 + txt)
     event.reply(" "*8 + "</outline>")
     event.reply("    <body>")
     event.reply("</opml>")
 
 
-Client.add(exp)
-
-
 def nme(event):
     "set name of feed."
     if len(event.args) != 2:
         event.reply('nme <stringinurl> <name>')
         return
     selector = {'rss': event.args[0]}
     for _fn, feed in find('rss', selector):
         if feed:
             feed.name = event.args[1]
             sync(feed)
     event.reply('ok')
 
 
-Client.add(nme)
-
-
 def rem(event):
     "remove a feed."
     if len(event.args) != 1:
         event.reply('rem <stringinurl>')
         return
     selector = {'rss': event.args[0]}
     for fnm, feed in find('rss', selector):
         if feed:
             feed.__deleted__ = True
             sync(feed, fnm)
     event.reply('ok')
 
 
-Client.add(rem)
-
-
 def res(event):
     "restore a feed."
     if len(event.args) != 1:
         event.reply('res <stringinurl>')
         return
     selector = {'rss': event.args[0]}
     for fnm, feed in find('rss', selector, deleted=True):
         if feed:
             feed.__deleted__ = False
             sync(feed, fnm)
     event.reply('ok')
 
 
-Client.add(res)
-
-
 def rss(event):
     "add a feed."
     if not event.rest:
         nrs = 0
         for fnm, feed in find('rss'):
             nrs += 1
             elp = laps(time.time()-fntime(fnm))
@@ -423,16 +415,18 @@
             return
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
 
 
-Client.add(rss)
+"register"
 
 
-TEMPLATE = """<opml version="1.0">
-    <head>
-        <title>rssbot opml</title>
-    </head>
-    <body>
-        <outline title="rssbot opml" text="24/7 feed fetcher">"""
+Command.add(dpl)
+Command.add(exp)
+Command.add(nme)
+Command.add(rem)
+Command.add(res)
+Command.add(rss)
+whitelist(Rss)
+whitelist(Seen)
```

### Comparing `botl-106/botl/modules/rst.py` & `botl-110/botl/modules/rst.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,138 +1,118 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=C,R,W0612,W0613
 
 
 "rest"
 
 
 import os
 import sys
 import time
 
 
 from http.server import HTTPServer, BaseHTTPRequestHandler
 
 
 from ..default import Default
-from ..errors  import Errors, debug
+from ..errors  import debug, later
+from ..find    import fns
 from ..object  import Object
-from ..persist import Persist, Workdir
 from ..thread  import launch
+from ..workdir import Workdir
 
 
 def init():
-    "start object server."
-    result = None
     try:
-        result = REST((Config.hostname, int(Config.port)), RESTHandler)
+        rest = REST((Config.hostname, int(Config.port)), RESTHandler)
     except OSError:
-        pass
-    if result:
-        launch(result.start)
-    return result
+        return
+    launch(rest.start)
+    return rest
 
 
 def html(txt):
-    "html template."
-    return f"<!doctype html><html>{txt}</html>"
+    return """<!doctype html>
+<html>
+   %s
+</html>
+""" % txt
 
 
 class Config(Default):
 
-    "Config"
-
     hostname = "localhost"
     port     = 10102
 
-    def __bla__(self):
-        pass
-
-    def __blabla__(self):
-        pass
-
 
 class REST(HTTPServer, Object):
 
-    "REST"
-
     allow_reuse_address = True
     daemon_thread = True
 
     def __init__(self, *args, **kwargs):
         HTTPServer.__init__(self, *args, **kwargs)
         Object.__init__(self)
         self.host = args[0]
         self._last = time.time()
         self._starttime = time.time()
         self._status = "start"
 
     def exit(self):
-        "shutdown server."
         self._status = ""
         time.sleep(0.2)
         self.shutdown()
 
-    def start(self):
-        "start server/"
+    def start(self): 
         self._status = "ok"
         self.serve_forever()
 
     def request(self):
-        "handler request."
         self._last = time.time()
 
     def error(self, request, addr):
-        "handle error."
-        exctype, excvalue, _tb = sys.exc_info()
+        exctype, excvalue, tb = sys.exc_info()
         exc = exctype(excvalue)
-        Errors.add(exc)
-        if request:
-            debug(f'{addr} {excvalue}')
+        later(exc)
+        debug('%s %s' % (addr, excvalue))
 
 
 class RESTHandler(BaseHTTPRequestHandler):
 
-    "RESTHandler"
-
     def setup(self):
-        "setup request."
         BaseHTTPRequestHandler.setup(self)
         self._ip = self.client_address[0]
         self._size = 0
 
     def send(self, txt):
-        "send text."
         self.wfile.write(bytes(txt, "utf-8"))
         self.wfile.flush()
 
     def write_header(self, htype='text/plain'):
-        "write a header."
         self.send_response(200)
-        self.send_header('Content-type', f'{htype}; charset="utf-8"')
+        self.send_header('Content-type', '%s; charset=%s ' % (htype, "utf-8"))
         self.send_header('Server', "1")
         self.end_headers()
 
-    def do_GET(self): # pylint: disable=C0103
-        "handle GET."
+    def do_GET(self):
         if self.path == "/":
             self.write_header("text/html")
             txt = ""
-            for fnm in Persist.fns():
+            for fnm in fns():
                 txt += f'<a href="http://{Config.hostname}:{Config.port}/{fnm}">{fnm}</a>\n'
             self.send(html(txt.strip()))
             return
         fnm = Workdir.workdir + os.sep + "store" + os.sep + self.path
         try:
-            with open(fnm, "r", encoding="utf-8") as file:
-                txt = file.read()
-                self.write_header("txt/plain")
-                self.send(html(txt))
+            f = open(fnm, "r", encoding="utf-8")
+            txt = f.read()
+            f.close()
+            self.write_header("txt/plain")
+            self.send(html(txt))
         except (TypeError, FileNotFoundError, IsADirectoryError) as ex:
             self.send_response(404)
-            Errors.add(ex)
+            later(ex)
             self.end_headers()
 
     def log(self, code):
-        "log access."
-        debug(f"{self.address_string()} code {code} path {self.path}")
+        debug('%s code %s path %s' % (self.address_string(), code, self.path))
```

### Comparing `botl-106/botl/modules/tmr.py` & `botl-110/botl/modules/tmr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=C,R,W0612,W0105,W0702,E0402
 
 
 "timer"
 
 
 import datetime
 import re
 import time as ttime
 
 
-from ..broker  import Broker
-from ..client  import Client
+from ..client  import laps
+from ..command import Command
 from ..event   import Event
-from ..object  import update
-from ..persist import Persist, find, sync
-from ..thread  import launch
+from ..find    import find
+from ..runtime import broker
 from ..timer   import Timer
-from ..utils   import laps
+from ..thread  import launch
+from ..persist import whitelist
+from ..object  import update
+from ..workdir import sync
 
 
 def init():
-    "start timers."
-    for _fn, obj in find("timer"):
+    for fnm, obj in find("timer"):
         if "time" not in obj:
             continue
         diff = float(obj.time) - ttime.time()
         if diff > 0:
-            bot = Broker.first()
+            bot = broker.first()
             evt = Event()
             update(evt, obj)
             evt.orig = object.__repr__(bot)
             timer = Timer(diff, evt.show)
             launch(timer.start)
 
 
@@ -59,34 +60,31 @@
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    "NoDate"
+    pass
 
 
-Persist.add(Timer)
+whitelist(Timer)
 
 
 def extract_date(daystr):
-    "extract date from string."
-    res = None
     for fmt in FORMATS:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
-            break
         except ValueError:
             res = None
-    return res
+        if res:
+            return res
 
 
 def get_day(daystr):
-    "return day from string."
     day = None
     month = None
     yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
         if ymdre:
             (day, month, yea) = ymdre.groups()
@@ -98,21 +96,20 @@
                 yea = ttime.strftime("%Y", ttime.localtime())
         except Exception as ex:
             raise NoDate(daystr) from ex
     if day:
         day = int(day)
         month = int(month)
         yea = int(yea)
-        date = f"{day} {MONTHS[month]} {yea}"
+        date = "%s %s %s" % (day, MONTHS[month], yea)
         return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
     raise NoDate(daystr)
 
 
 def get_hour(daystr):
-    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -126,27 +123,25 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
-    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
 def parse_time(txt):
-    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -161,77 +156,78 @@
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
 def to_day(daystr):
-    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
-    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
-            break
         except ValueError:
             res = None
+        if res:
+            return res
         line = ""
-    return res
 
 
 def today():
-    "return date."
     return str(datetime.datetime.today()).split()[0]
 
 
+"commands"
+
+
 def tmr(event):
-    "add a timer."
-    result = ""
     if not event.rest:
         nmr = 0
-        for _fn, obj in find('timer'):
+        for fnm, obj in find('timer'):
+            if "time" not in obj:
+                continue
             lap = float(obj.time) - ttime.time()
             if lap > 0:
                 event.reply(f'{nmr} {obj.txt} {laps(lap)}')
                 nmr += 1
-        return result
+        if not nmr:
+            event.reply("no timers")
+        return
     seconds = 0
     line = ""
     for word in event.args:
         if word.startswith("+"):
             try:
                 seconds = int(word[1:])
             except (ValueError, IndexError):
-                event.reply(f"{seconds} is not an integer")
-                return result
+                event.reply("%s is not an integer" % seconds)
+                return
         else:
             line += word + " "
     if seconds:
         target = ttime.time() + seconds
     else:
         try:
             target = get_day(event.rest)
         except NoDate:
             target = to_day(today())
         hour =  get_hour(event.rest)
         if hour:
             target += hour
     if not target or ttime.time() > target:
         event.reply("already passed given time.")
-        return result
+        return
     event.time = target
     diff = target - ttime.time()
     event.reply("ok " +  laps(diff))
     event.result = []
     event.result.append(event.rest)
     timer = Timer(diff, event.show, thrname=event.cmd)
     update(timer, event)
     sync(timer)
     launch(timer.start)
-    return result
 
 
-Client.add(tmr)
+Command.add(tmr)
```

### Comparing `botl-106/botl/modules/udp.py` & `botl-110/botl/modules/udp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,60 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=C0115,C0116,W0105,E0402,R0903
 
 
 "udp to irc relay"
 
 
 import select
 import socket
 import sys
 import threading
 import time
 
 
-from dataclasses import dataclass
-
-
-from ..broker import Broker
-from ..client import Client
-from ..object import Object
-from ..thread import launch
+from ..object  import Object, values
+from ..command import Command
+from ..runtime import broker
+from ..thread  import launch
 
 
 def init():
-    "start udp to irc relay."
     udpd = UDP()
     udpd.start()
     return udpd
 
 
-@dataclass
 class Cfg(Object):
 
-    "Cfg"
-
     addr = ""
     host = "localhost"
     port = 5500
 
 
 class UDP(Object):
 
-    "UDP"
-
     def __init__(self):
         Object.__init__(self)
         self.stopped = False
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         self._sock.setblocking(1)
         self._starttime = time.time()
         self.ready = threading.Event()
 
     def output(self, txt, addr=None):
-        "output to fleet."
         if addr:
             Cfg.addr = addr
-        for bot in Broker.all():
+        for bot in values(broker.objs):
             bot.announce(txt.replace("\00", ""))
 
     def loop(self):
-        "udp input loop."
         try:
             self._sock.bind((Cfg.host, Cfg.port))
         except socket.gaierror:
             return
         self.ready.set()
         while not self.stopped:
             (txt, addr) = self._sock.recvfrom(64000)
@@ -73,35 +62,31 @@
                 break
             data = str(txt.rstrip(), "utf-8")
             if not data:
                 break
             self.output(data, addr)
 
     def exit(self):
-        "stop relay."
         self.stopped = True
         self._sock.settimeout(0.01)
         self._sock.sendto(
                           bytes("exit", "utf-8"),
                           (Cfg.host, Cfg.port)
                          )
 
     def start(self):
-        "start relay."
         launch(self.loop)
 
 
 def toudp(host, port, txt):
-    "send udp packet to bot."
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.sendto(bytes(txt.strip(), "utf-8"), (host, port))
 
 
 def udp(event):
-    "send udp command."
     if event.rest:
         toudp(Cfg.host, Cfg.port, event.rest)
         event.reply(f"{len(event.rest)} characters sent")
         return
     if not select.select(
                          [sys.stdin, ],
                          [],
@@ -129,8 +114,8 @@
                 break
             size += len(txt)
             toudp(Cfg.host, Cfg.port, txt)
         if stop:
             break
 
 
-Client.add(udp)
+Command.add(udp)
```

### Comparing `botl-106/botl/object.py` & `botl-110/botl/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,R,W0105
 
 
-"object"
+"objects"
 
 
 import json
 import os
 import pathlib
 import _thread
```

### Comparing `botl-106/botl/parser.py` & `botl-110/botl/parser.py`

 * *Files identical despite different names*

### Comparing `botl-106/botl/persist.py` & `botl-110/botl/find.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,37 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,R,W0105
 
 
-"persist"
+"locate"
 
 
-import datetime
 import os
 import time
 
 
 from .default import Default
-from .object  import Object, fqn, read, search, update, write
-from .workdir import Workdir
-
-
-class Persist(Object):
-
-    "Persist"
-
-    classes = Object()
-
-    @staticmethod
-    def add(clz):
-        "add class to whitelist."
-        name = str(clz).split()[1][1:-2]
-        setattr(Persist.classes, name, clz)
-
-    @staticmethod
-    def fns(mtc=""):
-        "show list of files."
-        dname = ''
-        pth = Workdir.store(mtc)
-        for rootdir, dirs, _files in os.walk(pth, topdown=False):
-            if dirs:
-                for dname in sorted(dirs):
-                    if dname.count('-') == 2:
-                        ddd = os.path.join(rootdir, dname)
-                        fls = sorted(os.listdir(ddd))
-                        for fll in fls:
-                            yield Workdir.strip(os.path.join(ddd, fll))
-
-    @staticmethod
-    def long(name):
-        "match from single name to long name."
-        split = name.split(".")[-1].lower()
-        res = name
-        for named in Persist.classes:
-            if split in named.split(".")[-1].lower():
-                res = named
-                break
-        if "." not in res:
-            for fnm in Workdir.types():
-                claz = fnm.split(".")[-1]
-                if fnm == claz.lower():
-                    res = fnm
-        return res
+from .object  import fqn, search, update
+from .persist import long
+from .workdir import fetch, store, strip
+
+
+def fns(mtc=""):
+    "show list of files."
+    dname = ''
+    pth = store(mtc)
+    for rootdir, dirs, _files in os.walk(pth, topdown=False):
+        if dirs:
+            for dname in sorted(dirs):
+                if dname.count('-') == 2:
+                    ddd = os.path.join(rootdir, dname)
+                    fls = sorted(os.listdir(ddd))
+                    for fll in fls:
+                        yield strip(os.path.join(ddd, fll))
 
 
 def fntime(daystr):
     "convert file name to it's saved time."
     daystr = daystr.replace('_', ':')
     datestr = ' '.join(daystr.split(os.sep)[-2:])
     if '.' in datestr:
@@ -71,77 +42,36 @@
     if rest:
         timed += float('.' + rest)
     return timed
 
 
 def find(mtc, selector=None, index=None, deleted=False):
     "find object matching the selector dict."
-    clz = Persist.long(mtc)
+    clz = long(mtc)
     nrs = -1
-    for fnm in sorted(Persist.fns(clz), key=fntime):
+    for fnm in sorted(fns(clz), key=fntime):
         obj = Default()
         fetch(obj, fnm)
         if not deleted and '__deleted__' in obj:
             continue
         if selector and not search(obj, selector):
             continue
         nrs += 1
         if index is not None and nrs != int(index):
             continue
         yield (fnm, obj)
 
 
-def fetch(obj, pth):
-    "read object from disk."
-    pth2 = Workdir.store(pth)
-    read(obj, pth2)
-    return Workdir.strip(pth)
-
-
-def ident(obj):
-    "return an id for an object."
-    return os.path.join(
-                        fqn(obj),
-                        os.path.join(*str(datetime.datetime.now()).split())
-                       )
-
-
 def last(obj, selector=None):
     "return last object saved."
     if selector is None:
         selector = {}
     result = sorted(
                     find(fqn(obj), selector),
                     key=lambda x: fntime(x[0])
                    )
     res = None
     if result:
         inp = result[-1]
         update(obj, inp[-1])
         res = inp[0]
     return res
-
-def sync(obj, pth=None):
-    "sync object to disk."
-    if pth is None:
-        pth = ident(obj)
-    pth2 = Workdir.store(pth)
-    write(obj, pth2)
-    return pth
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Persist',
-        'fetch',
-        'fntime',
-        'find',
-        'last',
-        'ident',
-        'sync',
-    )
-
-
-__all__ = __dir__()
```

### Comparing `botl-106/botl/thread.py` & `botl-110/botl/thread.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import queue
 import threading
 import time
 import types
 
 
-from .errors import Errors
+from .errors import later
 
 
 class Thread(threading.Thread):
 
     "Thread"
 
     def __init__(self, func, thrname, *args, daemon=True, **kwargs):
@@ -42,15 +42,15 @@
 
     def run(self):
         "run this thread's payload."
         func, args = self.queue.get()
         try:
             self._result = func(*args)
         except Exception as ex:
-            Errors.add(ex)
+            later(ex)
             if args and "Event" in str(type(args[0])):
                 args[0].ready()
 
 
 def launch(func, *args, **kwargs):
     "launch a thread."
     nme = kwargs.get("name", name(func))
@@ -69,21 +69,7 @@
     if '__class__' in dir(obj) and '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     if '__class__' in dir(obj):
         return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
     if '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     return None
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Thread',
-        'launch',
-        'name'
-    )
-
-
-__all__ = __dir__()
```

### Comparing `botl-106/botl/timer.py` & `botl-110/botl/timer.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from .thread import launch
 
 
 class Timer:
 
-    "Timer"
+    "run a function at a specific time."
 
     def __init__(self, sleep, func, *args, thrname=None):
         self.args  = args
         self.func  = func
         self.sleep = sleep
         self.name  = thrname or str(self.func).split()[2]
         self.state = {}
@@ -43,19 +43,7 @@
         timer.start()
         self.timer   = timer
 
     def stop(self):
         "stop timer."
         if self.timer:
             self.timer.cancel()
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Timer',
-    )
-
-
-__all__ = __dir__()
```

### Comparing `botl-106/botl/utils.py` & `botl-110/botl/utils.py`

 * *Files identical despite different names*

### Comparing `botl-106/botl.egg-info/PKG-INFO` & `botl-110/botl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 106
+Version: 110
 Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
@@ -142,28 +142,28 @@
     rss - add a feed
     thr - show the running threads
 
 SYSTEMD
 
 ::
 
-    save the following it in /etc/systems/system/botl.service and
+    save the following it in /etc/systemd/system/botl.service and
     replace "<user>" with the user running pipx
 
     [Unit]
     Description=bot library
     Requires=network-online.target
     After=network-online.target
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.botl
-    ExecStart=/home/<user>/.local/pipx/venvs/botl/bin/botl -d
+    ExecStart=/home/<user>/.local/pipx/venvs/botl/bin/botld
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
```

### Comparing `botl-106/botl.egg-info/SOURCES.txt` & `botl-110/botl.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 README.rst
 pyproject.toml
 setup.py
+bin/botl
+bin/botlbot
+bin/botld
 botl/__init__.py
-botl/__main__.py
 botl/broker.py
 botl/client.py
+botl/command.py
 botl/default.py
 botl/errors.py
 botl/event.py
+botl/find.py
 botl/handler.py
 botl/object.py
 botl/parser.py
 botl/persist.py
 botl/repeater.py
+botl/runtime.py
 botl/thread.py
 botl/timer.py
 botl/utils.py
 botl/workdir.py
 botl.egg-info/PKG-INFO
 botl.egg-info/SOURCES.txt
 botl.egg-info/dependency_links.txt
-botl.egg-info/entry_points.txt
 botl.egg-info/top_level.txt
 botl.egg-info/zip-safe
 botl/modules/__init__.py
 botl/modules/cmd.py
-botl/modules/dbg.py
 botl/modules/err.py
 botl/modules/flt.py
 botl/modules/fnd.py
 botl/modules/irc.py
 botl/modules/log.py
+botl/modules/man.py
 botl/modules/mbx.py
 botl/modules/mdl.py
 botl/modules/mod.py
 botl/modules/req.py
 botl/modules/rss.py
 botl/modules/rst.py
 botl/modules/tdo.py
 botl/modules/thr.py
 botl/modules/tmr.py
-botl/modules/udp.py
+botl/modules/udp.py
+botl/modules/wsd.py
```

### Comparing `botl-106/pyproject.toml` & `botl-110/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,39 +4,40 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "botl"
 description = "bot library"
-version = "106"
+version = "110"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 
-[project.scripts]
-"botl" = "botl.__main__:wrapped"
-
-
 [project.urls]
 "home" = "https://pypi.org/project/botl"
 "bugs" = "https://github.com/xobjectz/botl/issues"
 "source" = "https://github.com/xobjectz/botl"
 
 
 [tool.setuptools]
+script-files = [
+    "bin/botl",
+    "bin/botld",
+    "bin/botlbot"
+]
 packages = [
     "botl",
     "botl.modules"
 ]
 zip-safe=true
```

