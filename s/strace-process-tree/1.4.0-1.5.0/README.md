# Comparing `tmp/strace-process-tree-1.4.0.tar.gz` & `tmp/strace-process-tree-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strace-process-tree-1.4.0.tar", last modified: Tue Jun 27 06:44:35 2023, max compression
+gzip compressed data, was "strace-process-tree-1.5.0.tar", last modified: Fri Apr 19 10:43:40 2024, max compression
```

## Comparing `strace-process-tree-1.4.0.tar` & `strace-process-tree-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/
--rw-r--r--   0 mg        (1000) mg        (1000)      126 2019-08-22 13:46:49.000000 strace-process-tree-1.4.0/.coveragerc
--rw-r--r--   0 mg        (1000) mg        (1000)       71 2019-08-21 13:01:00.000000 strace-process-tree-1.4.0/.gitignore
--rw-rw-r--   0 mg        (1000) mg        (1000)     3527 2023-06-27 06:43:42.000000 strace-process-tree-1.4.0/CHANGES.rst
--rw-r--r--   0 mg        (1000) mg        (1000)    18092 2019-08-21 13:59:11.000000 strace-process-tree-1.4.0/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      175 2019-08-21 14:00:54.000000 strace-process-tree-1.4.0/MANIFEST.in
--rw-rw-r--   0 mg        (1000) mg        (1000)      366 2020-10-24 10:07:13.000000 strace-process-tree-1.4.0/Makefile
--rw-rw-r--   0 mg        (1000) mg        (1000)     3498 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/PKG-INFO
--rw-rw-r--   0 mg        (1000) mg        (1000)     2404 2020-11-30 19:57:48.000000 strace-process-tree-1.4.0/README.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      841 2023-05-29 09:02:57.000000 strace-process-tree-1.4.0/appveyor.yml
--rw-r--r--   0 mg        (1000) mg        (1000)       44 2019-08-21 13:47:16.000000 strace-process-tree-1.4.0/pytest.ini
--rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 strace-process-tree-1.4.0/release.mk
--rw-rw-r--   0 mg        (1000) mg        (1000)      398 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/setup.cfg
--rwxrwxr-x   0 mg        (1000) mg        (1000)     1872 2023-05-30 10:47:10.000000 strace-process-tree-1.4.0/setup.py
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-27 06:44:35.899506 strace-process-tree-1.4.0/strace_process_tree.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     3498 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      514 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       65 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/entry_points.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-08-21 12:43:27.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/not-zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)       20 2023-06-27 06:44:35.000000 strace-process-tree-1.4.0/strace_process_tree.egg-info/top_level.txt
--rwxrwxr-x   0 mg        (1000) mg        (1000)    15372 2023-06-27 06:43:51.000000 strace-process-tree-1.4.0/strace_process_tree.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1126 2019-08-21 11:55:33.000000 strace-process-tree-1.4.0/strace_process_tree_example_output.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     7072 2019-08-21 11:55:33.000000 strace-process-tree-1.4.0/strace_process_tree_example_verbose_output.txt
--rw-r--r--   0 mg        (1000) mg        (1000)    19942 2023-06-27 06:40:05.000000 strace-process-tree-1.4.0/tests.py
--rw-rw-r--   0 mg        (1000) mg        (1000)      700 2023-05-29 09:02:57.000000 strace-process-tree-1.4.0/tox.ini
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-04-19 10:43:40.760088 strace-process-tree-1.5.0/
+-rw-r--r--   0 mg        (1000) mg        (1000)      126 2019-08-22 13:46:49.000000 strace-process-tree-1.5.0/.coveragerc
+-rw-r--r--   0 mg        (1000) mg        (1000)       71 2019-08-21 13:01:00.000000 strace-process-tree-1.5.0/.gitignore
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3710 2024-04-19 10:43:16.000000 strace-process-tree-1.5.0/CHANGES.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)    18092 2019-08-21 13:59:11.000000 strace-process-tree-1.5.0/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      175 2019-08-21 14:00:54.000000 strace-process-tree-1.5.0/MANIFEST.in
+-rw-rw-r--   0 mg        (1000) mg        (1000)      366 2020-10-24 10:07:13.000000 strace-process-tree-1.5.0/Makefile
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3549 2024-04-19 10:43:40.760088 strace-process-tree-1.5.0/PKG-INFO
+-rw-rw-r--   0 mg        (1000) mg        (1000)     2404 2020-11-30 19:57:48.000000 strace-process-tree-1.5.0/README.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      871 2023-10-05 13:32:26.000000 strace-process-tree-1.5.0/appveyor.yml
+-rw-r--r--   0 mg        (1000) mg        (1000)       44 2019-08-21 13:47:16.000000 strace-process-tree-1.5.0/pytest.ini
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 strace-process-tree-1.5.0/release.mk
+-rw-rw-r--   0 mg        (1000) mg        (1000)      398 2024-04-19 10:43:40.764088 strace-process-tree-1.5.0/setup.cfg
+-rwxrwxr-x   0 mg        (1000) mg        (1000)     1922 2023-10-05 13:32:26.000000 strace-process-tree-1.5.0/setup.py
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-04-19 10:43:40.760088 strace-process-tree-1.5.0/strace_process_tree.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     3549 2024-04-19 10:43:40.000000 strace-process-tree-1.5.0/strace_process_tree.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      514 2024-04-19 10:43:40.000000 strace-process-tree-1.5.0/strace_process_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2024-04-19 10:43:40.000000 strace-process-tree-1.5.0/strace_process_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       65 2024-04-19 10:43:40.000000 strace-process-tree-1.5.0/strace_process_tree.egg-info/entry_points.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-08-21 12:43:27.000000 strace-process-tree-1.5.0/strace_process_tree.egg-info/not-zip-safe
+-rw-r--r--   0 mg        (1000) mg        (1000)       20 2024-04-19 10:43:40.000000 strace-process-tree-1.5.0/strace_process_tree.egg-info/top_level.txt
+-rwxrwxr-x   0 mg        (1000) mg        (1000)    15415 2024-04-19 10:43:16.000000 strace-process-tree-1.5.0/strace_process_tree.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1126 2019-08-21 11:55:33.000000 strace-process-tree-1.5.0/strace_process_tree_example_output.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     7072 2019-08-21 11:55:33.000000 strace-process-tree-1.5.0/strace_process_tree_example_verbose_output.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)    20444 2024-04-19 10:36:48.000000 strace-process-tree-1.5.0/tests.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)      706 2023-10-05 13:32:26.000000 strace-process-tree-1.5.0/tox.ini
```

### Comparing `strace-process-tree-1.4.0/CHANGES.rst` & `strace-process-tree-1.5.0/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Changes
 =======
 
 
+1.5.0 (2024-04-19)
+------------------
+
+- Add support for Python 3.12.
+- Recognize the clone3 system call (`issue 11
+  <https://github.com/mgedmin/strace-process-tree/pull/11>`_).
+
+
 1.4.0 (2023-06-27)
 ------------------
 
-* Fix parsing `/* 1 var */` (`issue 9
+* Fix parsing ``/* 1 var */`` (`issue 9
   <https://github.com/mgedmin/strace-process-tree/pull/9>`_).
 * Removed support for Python 2.
 
 
 1.3.0 (2023-05-24)
 ------------------
```

### Comparing `strace-process-tree-1.4.0/LICENSE` & `strace-process-tree-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.4.0/PKG-INFO` & `strace-process-tree-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strace-process-tree
-Version: 1.4.0
+Version: 1.5.0
 Summary: Produce a process tree from an strace log
 Home-page: https://github.com/mgedmin/strace-process-tree
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL v2 or v3
 Keywords: strace log process tree
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 strace-process-tree
```

### Comparing `strace-process-tree-1.4.0/README.rst` & `strace-process-tree-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.4.0/appveyor.yml` & `strace-process-tree-1.5.0/appveyor.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     # https://www.appveyor.com/docs/installed-software#python lists available
     # versions
     - PYTHON: "C:\\Python37"
     - PYTHON: "C:\\Python38"
     - PYTHON: "C:\\Python39"
     - PYTHON: "C:\\Python310"
     - PYTHON: "C:\\Python311"
+    - PYTHON: "C:\\Python312"
 
 init:
   - "echo %PYTHON%"
 
 install:
   - ps: |
       if (-not (Test-Path $env:PYTHON)) {
```

### Comparing `strace-process-tree-1.4.0/release.mk` & `strace-process-tree-1.5.0/release.mk`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.4.0/setup.py` & `strace-process-tree-1.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     license="GPL v2 or v3",
     python_requires=">=3.7",
 
     py_modules=["strace_process_tree"],
```

### Comparing `strace-process-tree-1.4.0/strace_process_tree.egg-info/PKG-INFO` & `strace-process-tree-1.5.0/strace_process_tree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strace-process-tree
-Version: 1.4.0
+Version: 1.5.0
 Summary: Produce a process tree from an strace log
 Home-page: https://github.com/mgedmin/strace-process-tree
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL v2 or v3
 Keywords: strace log process tree
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 strace-process-tree
```

### Comparing `strace-process-tree-1.4.0/strace_process_tree.egg-info/SOURCES.txt` & `strace-process-tree-1.5.0/strace_process_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.4.0/strace_process_tree.py` & `strace-process-tree-1.5.0/strace_process_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re
 import string
 import sys
 from collections import defaultdict, namedtuple
 from functools import partial
 
 
-__version__ = '1.4.0'
+__version__ = '1.5.0'
 __author__ = 'Marius Gedminas <marius@gedmin.as>'
 __url__ = "https://github.com/mgedmin/strace-process-tree"
 __licence__ = 'GPL v2 or v3'  # or ask me for MIT
 
 
 Tree = namedtuple('Tree', 'trunk, fork, end, space')
 
@@ -313,23 +313,23 @@
     def __str__(self):
         return self.format(PlainTheme(unicode=True))
 
 
 def simplify_syscall(event):
     # clone(child_stack=0x..., flags=FLAGS, parent_tidptr=..., tls=...,
     #       child_tidptr=...) => clone(FLAGS)
-    if event.startswith('clone('):
-        event = re.sub('[(].*, flags=([^,]*), .*[)]', r'(\1)', event)
+    if event.startswith(('clone(', 'clone3(')):
+        event = re.sub('[(].*(?:, |{)flags=([^,]*), .*[)]', r'(\1)', event)
     return event.rstrip()
 
 
 def extract_command_line(event):
     # execve("/usr/bin/foo", ["foo", "bar"], [/* 45 vars */]) => foo bar
     # execve("/usr/bin/foo", ["foo", "bar"], [/* 1 var */]) => foo bar
-    if event.startswith('clone('):
+    if event.startswith(('clone(', 'clone3(')):
         if 'CLONE_THREAD' in event:
             return '(thread)'
         elif 'flags=CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD' in event:
             return '(fork)'
         else:
             return '...'
     elif event.startswith('execve('):
@@ -411,15 +411,15 @@
                 first_timestamp = e.timestamp
             timestamp -= first_timestamp
         if e.event.startswith('execve('):
             args, equal, result = e.event.rpartition(' = ')
             if result == '0':
                 name = mogrifier(args)
                 tree.handle_exec(e.pid, name, timestamp)
-        if e.event.startswith(('clone(', 'fork(', 'vfork(')):
+        if e.event.startswith(('clone(', 'clone3(', 'fork(', 'vfork(')):
             args, equal, result = e.event.rpartition(' = ')
             # if clone() fails, the event will look like this:
             #   clone(...) = -1 EPERM (Operation not permitted)
             # and it will fail the result.isdigit() check
             if result.isdigit():
                 child_pid = int(result)
                 name = mogrifier(args)
```

### Comparing `strace-process-tree-1.4.0/strace_process_tree_example_output.txt` & `strace-process-tree-1.5.0/strace_process_tree_example_output.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.4.0/strace_process_tree_example_verbose_output.txt` & `strace-process-tree-1.5.0/strace_process_tree_example_verbose_output.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.4.0/tests.py` & `strace-process-tree-1.5.0/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -291,14 +291,19 @@
         'clone(CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD)'
     )
     assert stp.simplify_syscall(
         'clone(child_stack=0x7fbb3690dfb0, flags=CLONE_VM|CLONE_FS|CLONE_FILES|CLONE_SIGHAND|CLONE_THREAD|CLONE_SYSVSEM|CLONE_SETTLS|CLONE_PARENT_SETTID|CLONE_CHILD_CLEARTID, parent_tidptr=0x7fbb3690e9d0, tls=0x7fbb3690e700, child_tidptr=0x7fbb3690e9d0)'
     ) == (
         'clone(CLONE_VM|CLONE_FS|CLONE_FILES|CLONE_SIGHAND|CLONE_THREAD|CLONE_SYSVSEM|CLONE_SETTLS|CLONE_PARENT_SETTID|CLONE_CHILD_CLEARTID)'
     )
+    assert stp.simplify_syscall(
+        'clone3({flags=CLONE_VM|CLONE_FS|CLONE_FILES|CLONE_SIGHAND|CLONE_THREAD|CLONE_SYSVSEM|CLONE_SETTLS|CLONE_PARENT_SETTID|CLONE_CHILD_CLEARTID, child_tid=0x7f1e00bff910, parent_tid=0x7f1e00bff910, exit_signal=0, stack=0x7f1e003ff000, stack_size=0x7feb40, tls=0x7f1e00bff640} => {parent_tid=[1942]}, 88)'
+    ) == (
+        'clone3(CLONE_VM|CLONE_FS|CLONE_FILES|CLONE_SIGHAND|CLONE_THREAD|CLONE_SYSVSEM|CLONE_SETTLS|CLONE_PARENT_SETTID|CLONE_CHILD_CLEARTID)'
+    )
 
 
 def test_extract_command_line():
     assert stp.extract_command_line(
         'exit_group(0)    '
     ) == (
         'exit_group(0)'
```

### Comparing `strace-process-tree-1.4.0/tox.ini` & `strace-process-tree-1.5.0/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py37,py38,py39,py310,py311,pypy3
+envlist = py37,py38,py39,py310,py311,py312,pypy3
 
 [testenv]
 deps =
     pytest
 commands =
     pytest {posargs}
```

