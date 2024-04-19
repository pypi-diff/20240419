# Comparing `tmp/pymusicbox-0.0.2.tar.gz` & `tmp/pymusicbox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymusicbox-0.0.2.tar", last modified: Sun Apr  3 20:59:18 2022, max compression
+gzip compressed data, was "pymusicbox-0.0.3.tar", last modified: Fri Apr 19 04:39:59 2024, max compression
```

## Comparing `pymusicbox-0.0.2.tar` & `pymusicbox-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-04-03 20:59:18.170709 pymusicbox-0.0.2/
--rw-rw-rw-   0        0        0     1088 2022-04-03 18:58:17.000000 pymusicbox-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      436 2022-04-03 20:59:18.171706 pymusicbox-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       79 2022-04-03 18:58:17.000000 pymusicbox-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2022-04-03 18:58:17.000000 pymusicbox-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      491 2022-04-03 20:59:18.174703 pymusicbox-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-04-03 20:59:18.094703 pymusicbox-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-04-03 20:59:18.124704 pymusicbox-0.0.2/src/pymusicbox/
--rw-rw-rw-   0        0        0        0 2022-04-03 18:58:17.000000 pymusicbox-0.0.2/src/pymusicbox/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-03 20:59:18.147708 pymusicbox-0.0.2/src/pymusicbox/audio/
--rw-rw-rw-   0        0        0        0 2022-04-03 19:08:02.000000 pymusicbox-0.0.2/src/pymusicbox/audio/__init__.py
--rw-rw-rw-   0        0        0      169 2022-04-03 18:58:17.000000 pymusicbox-0.0.2/src/pymusicbox/audio/audio_utils.py
-drwxrwxrwx   0        0        0        0 2022-04-03 20:59:18.154703 pymusicbox-0.0.2/src/pymusicbox/symbolic/
--rw-rw-rw-   0        0        0        0 2022-04-03 19:08:02.000000 pymusicbox-0.0.2/src/pymusicbox/symbolic/__init__.py
--rw-rw-rw-   0        0        0     1097 2022-04-03 20:52:13.000000 pymusicbox-0.0.2/src/pymusicbox/symbolic/symbols.py
-drwxrwxrwx   0        0        0        0 2022-04-03 20:59:18.167701 pymusicbox-0.0.2/src/pymusicbox/synth/
--rw-rw-rw-   0        0        0        0 2022-04-03 19:08:02.000000 pymusicbox-0.0.2/src/pymusicbox/synth/__init__.py
--rw-rw-rw-   0        0        0     1860 2022-04-03 20:52:31.000000 pymusicbox-0.0.2/src/pymusicbox/synth/instrument.py
--rw-rw-rw-   0        0        0      136 2022-04-03 19:56:45.000000 pymusicbox-0.0.2/src/pymusicbox/synth/synthesizer.py
-drwxrwxrwx   0        0        0        0 2022-04-03 20:59:18.140705 pymusicbox-0.0.2/src/pymusicbox.egg-info/
--rw-rw-rw-   0        0        0      436 2022-04-03 20:59:17.000000 pymusicbox-0.0.2/src/pymusicbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2022-04-03 20:59:18.000000 pymusicbox-0.0.2/src/pymusicbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-03 20:59:17.000000 pymusicbox-0.0.2/src/pymusicbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-04-03 20:59:17.000000 pymusicbox-0.0.2/src/pymusicbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.498327 pymusicbox-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 04:39:59.498327 pymusicbox-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/src/pymusicbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/src/pymusicbox/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/audio/audio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/src/pymusicbox/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/symbolic/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/src/pymusicbox/synth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/synth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/src/pymusicbox/synth/instrument/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/synth/instrument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/synth/instrument/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-19 04:39:52.000000 pymusicbox-0.0.3/src/pymusicbox/synth/instrument/oscillator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:39:59.494327 pymusicbox-0.0.3/src/pymusicbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-19 04:39:59.000000 pymusicbox-0.0.3/src/pymusicbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 04:39:59.000000 pymusicbox-0.0.3/src/pymusicbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 04:39:59.000000 pymusicbox-0.0.3/src/pymusicbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 04:39:59.000000 pymusicbox-0.0.3/src/pymusicbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 04:39:59.000000 pymusicbox-0.0.3/src/pymusicbox.egg-info/top_level.txt
```

### Comparing `pymusicbox-0.0.2/LICENSE` & `pymusicbox-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

