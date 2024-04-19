# Comparing `tmp/sopel-ipython-0.0.2.tar.gz` & `tmp/sopel_ipython-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sopel-ipython-0.0.2.tar", last modified: Sun Dec 15 01:54:38 2019, max compression
+gzip compressed data, was "sopel_ipython-0.1.0.tar", last modified: Fri Apr 19 21:52:05 2024, max compression
```

## Comparing `sopel-ipython-0.0.2.tar` & `sopel_ipython-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0 dgw       (1000) dgw       (1000)        0 2019-12-15 01:54:38.000000 sopel-ipython-0.0.2/
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     1803 2019-12-15 01:54:38.000000 sopel-ipython-0.0.2/PKG-INFO
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      555 2019-08-24 03:24:54.000000 sopel-ipython-0.0.2/README.md
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     1157 2019-12-15 01:54:38.000000 sopel-ipython-0.0.2/setup.cfg
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      352 2019-12-15 01:47:32.000000 sopel-ipython-0.0.2/setup.py
-drwxrwxrwx   0 dgw       (1000) dgw       (1000)        0 2019-12-15 01:54:38.000000 sopel-ipython-0.0.2/sopel_ipython/
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     1775 2019-10-31 04:27:38.000000 sopel-ipython-0.0.2/sopel_ipython/__init__.py
-drwxrwxrwx   0 dgw       (1000) dgw       (1000)        0 2019-12-15 01:54:38.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)        1 2019-12-15 01:54:37.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/dependency_links.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)       41 2019-12-15 01:54:37.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/entry_points.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)        1 2019-12-15 01:54:37.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/not-zip-safe
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     1803 2019-12-15 01:54:37.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/PKG-INFO
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      169 2019-12-15 01:54:37.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/requires.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      314 2019-12-15 01:54:37.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/SOURCES.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)       14 2019-12-15 01:54:37.000000 sopel-ipython-0.0.2/sopel_ipython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:52:05.411145 sopel_ipython-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-19 21:51:59.000000 sopel_ipython-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 21:51:59.000000 sopel_ipython-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 21:51:59.000000 sopel_ipython-0.1.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-19 21:52:05.411145 sopel_ipython-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-19 21:51:59.000000 sopel_ipython-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-19 21:51:59.000000 sopel_ipython-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:52:05.411145 sopel_ipython-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:52:05.407145 sopel_ipython-0.1.0/sopel_ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 21:51:59.000000 sopel_ipython-0.1.0/sopel_ipython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:52:05.411145 sopel_ipython-0.1.0/sopel_ipython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-19 21:52:05.000000 sopel_ipython-0.1.0/sopel_ipython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 21:52:05.000000 sopel_ipython-0.1.0/sopel_ipython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:52:05.000000 sopel_ipython-0.1.0/sopel_ipython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 21:52:05.000000 sopel_ipython-0.1.0/sopel_ipython.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 21:52:05.000000 sopel_ipython-0.1.0/sopel_ipython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 21:52:05.000000 sopel_ipython-0.1.0/sopel_ipython.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sopel-ipython-0.0.2/README.md` & `sopel_ipython-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sopel-ipython-0.0.2/sopel_ipython/__init__.py` & `sopel_ipython-0.1.0/sopel_ipython/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,52 @@
-# coding=utf-8
 """
 ipython.py - Sopel IPython Console Module
 Copyright © 2014, Elad Alfassa <elad@fedoraproject.org>
+Copyright © 2022, dgw, technobabbl.es
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
 from __future__ import unicode_literals, absolute_import, print_function, division
 
 import sys
 
-import sopel
-import sopel.module
+from sopel import plugin
 
-import IPython
-if hasattr(IPython, 'terminal'):
-    from IPython.terminal.embed import InteractiveShellEmbed
-else:
-    from IPython.frontend.terminal.embed import InteractiveShellEmbed
+from IPython.terminal.embed import InteractiveShellEmbed
 
 
-console = None
-
-
-@sopel.module.commands('console')
-@sopel.module.require_admin('Only admins can start the interactive console')
+@plugin.commands('console')
+@plugin.require_admin('Only admins can start the interactive console')
 def interactive_shell(bot, trigger):
     """Starts an interactive IPython console"""
-    global console
-    if bot.memory.get('iconsole_running', False):
+    if bot.memory.get('ipython_console', None):
         bot.say('Console already running')
         return
     if not sys.__stdout__.isatty():
         bot.say('A tty is required to start the console')
         return
     if bot._daemon:
-        bot.say('Can\'t start console when running as a daemon')
+        bot.say("Can't start console when running as a daemon")
         return
 
     # Backup stderr/stdout wrappers
     old_stdout = sys.stdout
     old_stderr = sys.stderr
 
     # IPython wants actual stderr and stdout
     sys.stdout = sys.__stdout__
     sys.stderr = sys.__stderr__
 
-    banner1 = 'Sopel interactive shell (embedded IPython)'
-    banner2 = '`bot` and `trigger` are available. To exit, type exit'
-    exitmsg = 'Interactive shell closed'
-
-    console = InteractiveShellEmbed(banner1=banner1, banner2=banner2,
-                                    exit_msg=exitmsg)
-
-    bot.memory['iconsole_running'] = True
-    bot.say('console started')
-    console()
-    bot.memory['iconsole_running'] = False
+    bot.memory['ipython_console'] = InteractiveShellEmbed(
+        banner1='Sopel interactive shell (embedded IPython)',
+        banner2='`bot` and `trigger` are available; type `exit` to quit',
+        exit_msg='Interactive shell closed',
+    )
+
+    bot.say('Starting console')
+    bot.memory['ipython_console']()  # blocks until console is closed (Ctrl-D etc.)
+    del bot.memory['ipython_console']
 
     # Restore stderr/stdout wrappers
     sys.stdout = old_stdout
     sys.stderr = old_stderr
```

