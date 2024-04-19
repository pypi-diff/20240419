# Comparing `tmp/jztools-0.1.1.tar.gz` & `tmp/jztools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jztools-0.1.1.tar", last modified: Thu Apr 18 18:29:31 2024, max compression
+gzip compressed data, was "jztools-0.1.2.tar", last modified: Thu Apr 18 19:18:59 2024, max compression
```

## Comparing `jztools-0.1.1.tar` & `jztools-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 18:29:31.531456 jztools-0.1.1/
--rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-18 02:46:37.000000 jztools-0.1.1/LICENSE
--rw-r--r--   0 jazs       (501) staff       (20)      481 2024-04-18 18:29:31.531273 jztools-0.1.1/PKG-INFO
--rw-r--r--   0 jazs       (501) staff       (20)      221 2024-04-18 18:21:34.000000 jztools-0.1.1/README.md
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 18:29:31.529276 jztools-0.1.1/jztools/
--rw-r--r--   0 jazs       (501) staff       (20)       39 2024-04-17 23:46:09.000000 jztools-0.1.1/jztools/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)    13704 2024-04-17 23:46:09.000000 jztools-0.1.1/jztools/py.py
--rw-r--r--   0 jazs       (501) staff       (20)     4452 2024-04-17 23:46:09.000000 jztools-0.1.1/jztools/reference_sequence.py
--rw-r--r--   0 jazs       (501) staff       (20)     3688 2024-04-17 23:46:09.000000 jztools-0.1.1/jztools/rentemp.py
--rw-r--r--   0 jazs       (501) staff       (20)     7078 2024-04-17 23:46:09.000000 jztools-0.1.1/jztools/validation.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 18:29:31.531091 jztools-0.1.1/jztools.egg-info/
--rw-r--r--   0 jazs       (501) staff       (20)      481 2024-04-18 18:29:31.000000 jztools-0.1.1/jztools.egg-info/PKG-INFO
--rw-r--r--   0 jazs       (501) staff       (20)      423 2024-04-18 18:29:31.000000 jztools-0.1.1/jztools.egg-info/SOURCES.txt
--rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-18 18:29:31.000000 jztools-0.1.1/jztools.egg-info/dependency_links.txt
--rw-r--r--   0 jazs       (501) staff       (20)       15 2024-04-18 18:29:31.000000 jztools-0.1.1/jztools.egg-info/requires.txt
--rw-r--r--   0 jazs       (501) staff       (20)       14 2024-04-18 18:29:31.000000 jztools-0.1.1/jztools.egg-info/top_level.txt
--rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-18 18:29:31.531498 jztools-0.1.1/setup.cfg
--rw-r--r--   0 jazs       (501) staff       (20)      484 2024-04-18 18:25:17.000000 jztools-0.1.1/setup.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 18:29:31.527583 jztools-0.1.1/tests/
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 18:29:31.530822 jztools-0.1.1/tests/jztools/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 23:46:09.000000 jztools-0.1.1/tests/jztools/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     5892 2024-04-17 23:46:09.000000 jztools-0.1.1/tests/jztools/py.py
--rw-r--r--   0 jazs       (501) staff       (20)      135 2024-04-18 05:42:40.000000 jztools-0.1.1/tests/jztools/py_support.py
--rw-r--r--   0 jazs       (501) staff       (20)     3433 2024-04-17 23:46:09.000000 jztools-0.1.1/tests/jztools/reference_sequence.py
--rw-r--r--   0 jazs       (501) staff       (20)     3051 2024-04-17 23:46:09.000000 jztools-0.1.1/tests/jztools/validation.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 19:18:59.698690 jztools-0.1.2/
+-rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-18 02:46:37.000000 jztools-0.1.2/LICENSE
+-rw-r--r--   0 jazs       (501) staff       (20)      503 2024-04-18 19:18:59.698491 jztools-0.1.2/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)      221 2024-04-18 18:21:34.000000 jztools-0.1.2/README.md
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 19:18:59.696262 jztools-0.1.2/jztools/
+-rw-r--r--   0 jazs       (501) staff       (20)       39 2024-04-17 23:46:09.000000 jztools-0.1.2/jztools/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)    13704 2024-04-17 23:46:09.000000 jztools-0.1.2/jztools/py.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4452 2024-04-17 23:46:09.000000 jztools-0.1.2/jztools/reference_sequence.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3688 2024-04-17 23:46:09.000000 jztools-0.1.2/jztools/rentemp.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7078 2024-04-17 23:46:09.000000 jztools-0.1.2/jztools/validation.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 19:18:59.698283 jztools-0.1.2/jztools.egg-info/
+-rw-r--r--   0 jazs       (501) staff       (20)      503 2024-04-18 19:18:59.000000 jztools-0.1.2/jztools.egg-info/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)      444 2024-04-18 19:18:59.000000 jztools-0.1.2/jztools.egg-info/SOURCES.txt
+-rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-18 19:18:59.000000 jztools-0.1.2/jztools.egg-info/dependency_links.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       22 2024-04-18 19:18:59.000000 jztools-0.1.2/jztools.egg-info/requires.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       14 2024-04-18 19:18:59.000000 jztools-0.1.2/jztools.egg-info/top_level.txt
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 19:18:59.697157 jztools-0.1.2/scripts/
+-rw-r--r--   0 jazs       (501) staff       (20)     1259 2024-04-18 19:16:42.000000 jztools-0.1.2/scripts/test_install
+-rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-18 19:18:59.698737 jztools-0.1.2/setup.cfg
+-rw-r--r--   0 jazs       (501) staff       (20)      532 2024-04-18 19:18:12.000000 jztools-0.1.2/setup.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 19:18:59.694573 jztools-0.1.2/tests/
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 19:18:59.697981 jztools-0.1.2/tests/jztools/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 23:46:09.000000 jztools-0.1.2/tests/jztools/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5892 2024-04-17 23:46:09.000000 jztools-0.1.2/tests/jztools/py.py
+-rw-r--r--   0 jazs       (501) staff       (20)      135 2024-04-18 05:42:40.000000 jztools-0.1.2/tests/jztools/py_support.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3433 2024-04-17 23:46:09.000000 jztools-0.1.2/tests/jztools/reference_sequence.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3051 2024-04-17 23:46:09.000000 jztools-0.1.2/tests/jztools/validation.py
```

### Comparing `jztools-0.1.1/LICENSE` & `jztools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jztools-0.1.1/jztools/py.py` & `jztools-0.1.2/jztools/py.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.1/jztools/reference_sequence.py` & `jztools-0.1.2/jztools/reference_sequence.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.1/jztools/rentemp.py` & `jztools-0.1.2/jztools/rentemp.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.1/jztools/validation.py` & `jztools-0.1.2/jztools/validation.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.1/tests/jztools/py.py` & `jztools-0.1.2/tests/jztools/py.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.1/tests/jztools/reference_sequence.py` & `jztools-0.1.2/tests/jztools/reference_sequence.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.1/tests/jztools/validation.py` & `jztools-0.1.2/tests/jztools/validation.py`

 * *Files identical despite different names*

