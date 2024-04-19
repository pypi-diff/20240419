# Comparing `tmp/xunter-0.1.3.tar.gz` & `tmp/xunter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xunter-0.1.3.tar", last modified: Fri Apr 19 10:29:51 2024, max compression
+gzip compressed data, was "xunter-0.1.4.tar", last modified: Fri Apr 19 11:32:27 2024, max compression
```

## Comparing `xunter-0.1.3.tar` & `xunter-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:51.128340 xunter-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 10:29:46.000000 xunter-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 10:29:46.000000 xunter-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-19 10:29:51.128340 xunter-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-19 10:29:46.000000 xunter-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:29:51.128340 xunter-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 10:29:46.000000 xunter-0.1.3/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2915 2024-04-19 10:29:46.000000 xunter-0.1.3/xunter
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:51.128340 xunter-0.1.3/xunter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-19 10:29:51.000000 xunter-0.1.3/xunter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 10:29:51.000000 xunter-0.1.3/xunter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:29:51.000000 xunter-0.1.3/xunter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 10:29:51.000000 xunter-0.1.3/xunter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 10:29:51.000000 xunter-0.1.3/xunter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-19 10:29:46.000000 xunter-0.1.3/xunter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-19 10:29:46.000000 xunter-0.1.3/xunter2excel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:32:27.591412 xunter-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 11:32:22.000000 xunter-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 11:32:22.000000 xunter-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-19 11:32:27.591412 xunter-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-19 11:32:22.000000 xunter-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:32:27.591412 xunter-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 11:32:22.000000 xunter-0.1.4/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2915 2024-04-19 11:32:22.000000 xunter-0.1.4/xunter
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:32:27.591412 xunter-0.1.4/xunter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-19 11:32:27.000000 xunter-0.1.4/xunter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 11:32:27.000000 xunter-0.1.4/xunter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:32:27.000000 xunter-0.1.4/xunter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 11:32:27.000000 xunter-0.1.4/xunter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 11:32:27.000000 xunter-0.1.4/xunter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-19 11:32:22.000000 xunter-0.1.4/xunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-19 11:32:22.000000 xunter-0.1.4/xunter2excel
```

### Comparing `xunter-0.1.3/LICENSE` & `xunter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xunter-0.1.3/PKG-INFO` & `xunter-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.1.3
+Version: 0.1.4
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
@@ -36,14 +36,15 @@
 
 ## Install
 
 Install xunter into the environment where xonsh you want to trace resides.
 
 ```xsh
 pip install xunter
+# or: pip install git+https://github.com/anki-code/xunter
 ```
 
 ## Usage
 
 Xunter is working as drop-in replacement of `xonsh` with additional arguments:
 ```xsh
 xonsh  --no-rc -c "2+2"
@@ -51,15 +52,15 @@
 #      ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^
 #            xonsh         xunter
 ```
 Examples:
 ```xsh
 xunter --no-rc -c "2+2" ++depth-lt 10
 xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
-xunter --no-rc -c '2+2' ++filter 'Q(filename_has="main.py")'
+xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 
 xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q(function="run_subproc")'
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
@@ -67,27 +68,25 @@
 #   <= xunter/xunter:91:<module>
 #   - time_sec=[0.1505]
 
 # Don't forget about xonsh`s awesome macro call:
 xunter --no-rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
-and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). 
+and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
+Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
 ## Convert log to table
 
 ```python
 xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter
 xunter2excel /tmp/22.xunter
 ```
 
-## Investigations
-
-By putting `import ipdb; ipdb.set_trace()` in the any place of code you can investigate the environment interactively.
-
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
-
+* [xonsh-cheatsheet](https://github.com/anki-code/xonsh-cheatsheet)
 * [xonsh-install](https://github.com/anki-code/xonsh-install)
+* By putting `import ipdb; ipdb.set_trace()` into any place of code you can investigate the environment interactively.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.1.3 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.1.4 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -11,29 +11,32 @@
 Operating System :: OS Independent Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells Classifier: Topic :: Terminals
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: xonsh Requires-Dist: hunter
   xxuunntteerr is to profiling _x_o_n_s_h_ _s_h_e_l_l using _h_u_n_t_e_r. Time tracking is on board.
              If you like the idea click â­ on the repo and _t_w_e_e_t.
 ## Install Install xunter into the environment where xonsh you want to trace
-resides. ```xsh pip install xunter ``` ## Usage Xunter is working as drop-in
-replacement of `xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2"
-xunter --no-rc -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh
-xunter ``` Examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-
-rc ++depth-lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
-(filename_has="main.py")' xunter --no-rc -c 'echo 1' ++filter 'Q
+resides. ```xsh pip install xunter # or: pip install git+https://github.com/
+anki-code/xunter ``` ## Usage Xunter is working as drop-in replacement of
+`xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2" xunter --no-rc
+-c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ```
+Examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
+lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
+(filename_endswith="main.py")' xunter --no-rc -c 'echo 1' ++filter 'Q
 (filename_has="specs.py"),Q(function="run_subproc")' # [...]/site-packages/
 xonsh/procs/specs.py:910:run_subproc # <= xonsh/built_ins.py:206:
 subproc_captured_hiddenobject # <= :1: <= xonsh/codecache.py:64:
 run_compiled_code # <= xonsh/codecache.py:218:run_code_with_cache # <= xonsh/
 main.py:519:main_xonsh # <= xonsh/main.py:470:main # <= xunter/xunter:91: # -
 time_sec=[0.1505] # Don't forget about xonsh`s awesome macro call: xunter --no-
 rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ``` To set `++filter` read about [filters](https://python-
 hunter.readthedocs.io/en/latest/filtering.html) and take a look into the
-[cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). ##
-Convert log to table ```python xunter --no-rc -c "2+2" ++depth-lt 10 ++printer
-stack ++output /tmp/22.xunter xunter2excel /tmp/22.xunter ``` ## Investigations
-By putting `import ipdb; ipdb.set_trace()` in the any place of code you can
-investigate the environment interactively. ## Known issues If you see the
-unexpected exceptions try to install xonsh from the main branch first. ## See
-also * [xonsh-install](https://github.com/anki-code/xonsh-install)
+[cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). Use
+`./playground/trace.py` to experiment with the tracing filters and understand
+how it works. ## Convert log to table ```python xunter --no-rc -c "2+2"
+++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /tmp/
+22.xunter ``` ## Known issues If you see the unexpected exceptions try to
+install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
+(https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
+github.com/anki-code/xonsh-install) * By putting `import ipdb; ipdb.set_trace
+()` into any place of code you can investigate the environment interactively.
```

### Comparing `xunter-0.1.3/README.md` & `xunter-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ## Install
 
 Install xunter into the environment where xonsh you want to trace resides.
 
 ```xsh
 pip install xunter
+# or: pip install git+https://github.com/anki-code/xunter
 ```
 
 ## Usage
 
 Xunter is working as drop-in replacement of `xonsh` with additional arguments:
 ```xsh
 xonsh  --no-rc -c "2+2"
@@ -23,15 +24,15 @@
 #      ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^
 #            xonsh         xunter
 ```
 Examples:
 ```xsh
 xunter --no-rc -c "2+2" ++depth-lt 10
 xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
-xunter --no-rc -c '2+2' ++filter 'Q(filename_has="main.py")'
+xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 
 xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q(function="run_subproc")'
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
@@ -39,27 +40,25 @@
 #   <= xunter/xunter:91:<module>
 #   - time_sec=[0.1505]
 
 # Don't forget about xonsh`s awesome macro call:
 xunter --no-rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
-and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). 
+and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
+Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
 ## Convert log to table
 
 ```python
 xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter
 xunter2excel /tmp/22.xunter
 ```
 
-## Investigations
-
-By putting `import ipdb; ipdb.set_trace()` in the any place of code you can investigate the environment interactively.
-
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
-
+* [xonsh-cheatsheet](https://github.com/anki-code/xonsh-cheatsheet)
 * [xonsh-install](https://github.com/anki-code/xonsh-install)
+* By putting `import ipdb; ipdb.set_trace()` into any place of code you can investigate the environment interactively.
```

#### html2text {}

```diff
@@ -1,25 +1,28 @@
   xxuunntteerr is to profiling _x_o_n_s_h_ _s_h_e_l_l using _h_u_n_t_e_r. Time tracking is on board.
              If you like the idea click â­ on the repo and _t_w_e_e_t.
 ## Install Install xunter into the environment where xonsh you want to trace
-resides. ```xsh pip install xunter ``` ## Usage Xunter is working as drop-in
-replacement of `xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2"
-xunter --no-rc -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh
-xunter ``` Examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-
-rc ++depth-lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
-(filename_has="main.py")' xunter --no-rc -c 'echo 1' ++filter 'Q
+resides. ```xsh pip install xunter # or: pip install git+https://github.com/
+anki-code/xunter ``` ## Usage Xunter is working as drop-in replacement of
+`xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2" xunter --no-rc
+-c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ```
+Examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
+lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
+(filename_endswith="main.py")' xunter --no-rc -c 'echo 1' ++filter 'Q
 (filename_has="specs.py"),Q(function="run_subproc")' # [...]/site-packages/
 xonsh/procs/specs.py:910:run_subproc # <= xonsh/built_ins.py:206:
 subproc_captured_hiddenobject # <= :1: <= xonsh/codecache.py:64:
 run_compiled_code # <= xonsh/codecache.py:218:run_code_with_cache # <= xonsh/
 main.py:519:main_xonsh # <= xonsh/main.py:470:main # <= xunter/xunter:91: # -
 time_sec=[0.1505] # Don't forget about xonsh`s awesome macro call: xunter --no-
 rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ``` To set `++filter` read about [filters](https://python-
 hunter.readthedocs.io/en/latest/filtering.html) and take a look into the
-[cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). ##
-Convert log to table ```python xunter --no-rc -c "2+2" ++depth-lt 10 ++printer
-stack ++output /tmp/22.xunter xunter2excel /tmp/22.xunter ``` ## Investigations
-By putting `import ipdb; ipdb.set_trace()` in the any place of code you can
-investigate the environment interactively. ## Known issues If you see the
-unexpected exceptions try to install xonsh from the main branch first. ## See
-also * [xonsh-install](https://github.com/anki-code/xonsh-install)
+[cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). Use
+`./playground/trace.py` to experiment with the tracing filters and understand
+how it works. ## Convert log to table ```python xunter --no-rc -c "2+2"
+++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /tmp/
+22.xunter ``` ## Known issues If you see the unexpected exceptions try to
+install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
+(https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
+github.com/anki-code/xonsh-install) * By putting `import ipdb; ipdb.set_trace
+()` into any place of code you can investigate the environment interactively.
```

### Comparing `xunter-0.1.3/setup.py` & `xunter-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setuptools.setup(
     name='xunter',
-    version='0.1.3',
+    version='0.1.4',
     license='MIT',
     author='anki-code',
     author_email='no@no.no',
     description="Profiling for the xonsh shell based on hunter.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xunter-0.1.3/xunter` & `xunter-0.1.4/xunter`

 * *Files identical despite different names*

### Comparing `xunter-0.1.3/xunter.egg-info/PKG-INFO` & `xunter-0.1.4/xunter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.1.3
+Version: 0.1.4
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
@@ -36,14 +36,15 @@
 
 ## Install
 
 Install xunter into the environment where xonsh you want to trace resides.
 
 ```xsh
 pip install xunter
+# or: pip install git+https://github.com/anki-code/xunter
 ```
 
 ## Usage
 
 Xunter is working as drop-in replacement of `xonsh` with additional arguments:
 ```xsh
 xonsh  --no-rc -c "2+2"
@@ -51,15 +52,15 @@
 #      ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^
 #            xonsh         xunter
 ```
 Examples:
 ```xsh
 xunter --no-rc -c "2+2" ++depth-lt 10
 xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
-xunter --no-rc -c '2+2' ++filter 'Q(filename_has="main.py")'
+xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 
 xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q(function="run_subproc")'
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
@@ -67,27 +68,25 @@
 #   <= xunter/xunter:91:<module>
 #   - time_sec=[0.1505]
 
 # Don't forget about xonsh`s awesome macro call:
 xunter --no-rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
-and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). 
+and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
+Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
 ## Convert log to table
 
 ```python
 xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter
 xunter2excel /tmp/22.xunter
 ```
 
-## Investigations
-
-By putting `import ipdb; ipdb.set_trace()` in the any place of code you can investigate the environment interactively.
-
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
-
+* [xonsh-cheatsheet](https://github.com/anki-code/xonsh-cheatsheet)
 * [xonsh-install](https://github.com/anki-code/xonsh-install)
+* By putting `import ipdb; ipdb.set_trace()` into any place of code you can investigate the environment interactively.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.1.3 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.1.4 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -11,29 +11,32 @@
 Operating System :: OS Independent Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells Classifier: Topic :: Terminals
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: xonsh Requires-Dist: hunter
   xxuunntteerr is to profiling _x_o_n_s_h_ _s_h_e_l_l using _h_u_n_t_e_r. Time tracking is on board.
              If you like the idea click â­ on the repo and _t_w_e_e_t.
 ## Install Install xunter into the environment where xonsh you want to trace
-resides. ```xsh pip install xunter ``` ## Usage Xunter is working as drop-in
-replacement of `xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2"
-xunter --no-rc -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh
-xunter ``` Examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-
-rc ++depth-lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
-(filename_has="main.py")' xunter --no-rc -c 'echo 1' ++filter 'Q
+resides. ```xsh pip install xunter # or: pip install git+https://github.com/
+anki-code/xunter ``` ## Usage Xunter is working as drop-in replacement of
+`xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2" xunter --no-rc
+-c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ```
+Examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
+lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
+(filename_endswith="main.py")' xunter --no-rc -c 'echo 1' ++filter 'Q
 (filename_has="specs.py"),Q(function="run_subproc")' # [...]/site-packages/
 xonsh/procs/specs.py:910:run_subproc # <= xonsh/built_ins.py:206:
 subproc_captured_hiddenobject # <= :1: <= xonsh/codecache.py:64:
 run_compiled_code # <= xonsh/codecache.py:218:run_code_with_cache # <= xonsh/
 main.py:519:main_xonsh # <= xonsh/main.py:470:main # <= xunter/xunter:91: # -
 time_sec=[0.1505] # Don't forget about xonsh`s awesome macro call: xunter --no-
 rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ``` To set `++filter` read about [filters](https://python-
 hunter.readthedocs.io/en/latest/filtering.html) and take a look into the
-[cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). ##
-Convert log to table ```python xunter --no-rc -c "2+2" ++depth-lt 10 ++printer
-stack ++output /tmp/22.xunter xunter2excel /tmp/22.xunter ``` ## Investigations
-By putting `import ipdb; ipdb.set_trace()` in the any place of code you can
-investigate the environment interactively. ## Known issues If you see the
-unexpected exceptions try to install xonsh from the main branch first. ## See
-also * [xonsh-install](https://github.com/anki-code/xonsh-install)
+[cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html). Use
+`./playground/trace.py` to experiment with the tracing filters and understand
+how it works. ## Convert log to table ```python xunter --no-rc -c "2+2"
+++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /tmp/
+22.xunter ``` ## Known issues If you see the unexpected exceptions try to
+install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
+(https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
+github.com/anki-code/xonsh-install) * By putting `import ipdb; ipdb.set_trace
+()` into any place of code you can investigate the environment interactively.
```

### Comparing `xunter-0.1.3/xunter.py` & `xunter-0.1.4/xunter.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,27 @@
             If string must be one of 'repr' or 'safe_repr'. Default: ``'safe_repr'``.
 
     .. versionadded:: 1.2.0
     """
     EVENT_COLORS = CALL_COLORS
 
     locals = defaultdict(list)
-    output_filepath = None
+    overwrite_stream = None
 
     @classmethod
     def cleanup(cls):
         cls.locals = defaultdict(list)
 
     def __init__(self, *args, **kwargs):
         # <profile>
         self.timings = {}
         # </profile>
 
-        if self.output_filepath:
-            args['stream'] = open(self.output_filepath, 'w')
+        if self.overwrite_stream:
+            args['stream'] = self.overwrite_stream
 
         super(CallPrinterProfile, self).__init__(*args, **kwargs)
 
     def __call__(self, event):
         """
         Handle event and print filename, line number and source code. If event.kind is a `return` or `exception` also
         prints values.
@@ -189,15 +189,15 @@
         filename_alignment (int): Default size for the filename column (files are right-aligned). Default: ``40``.
         force_colors (bool): Force coloring. Default: ``False``.
         repr_limit (bool): Limit length of ``repr()`` output. Default: ``512``.
         repr_func (string or callable): Function to use instead of ``repr``.
             If string must be one of 'repr' or 'safe_repr'. Default: ``'safe_repr'``.
     """
 
-    output_filepath = None
+    overwrite_stream = None
 
     def __init__(self, depth=15, limit=2, **options):
         self.limit = limit
         self.depth = depth
         # <profile>
         self.timings = {}
         # </profile>
```

### Comparing `xunter-0.1.3/xunter2excel` & `xunter-0.1.4/xunter2excel`

 * *Files identical despite different names*

