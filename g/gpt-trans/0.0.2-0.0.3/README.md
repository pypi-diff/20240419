# Comparing `tmp/gpt_trans-0.0.2.tar.gz` & `tmp/gpt_trans-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_trans-0.0.2.tar", last modified: Fri Apr 19 09:56:55 2024, max compression
+gzip compressed data, was "gpt_trans-0.0.3.tar", last modified: Fri Apr 19 12:47:27 2024, max compression
```

## Comparing `gpt_trans-0.0.2.tar` & `gpt_trans-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-04-19 09:56:55.452617 gpt_trans-0.0.2/
--rw-r--r--   0 zilliz     (501) staff       (20)      331 2024-04-19 09:56:55.452388 gpt_trans-0.0.2/PKG-INFO
--rw-r--r--   0 zilliz     (501) staff       (20)     2507 2024-04-19 09:54:56.000000 gpt_trans-0.0.2/README.md
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-04-19 09:56:55.447454 gpt_trans-0.0.2/gpt_trans/
--rw-r--r--   0 zilliz     (501) staff       (20)        0 2024-04-19 04:53:22.000000 gpt_trans-0.0.2/gpt_trans/__init__.py
--rw-r--r--   0 zilliz     (501) staff       (20)     4623 2024-04-19 09:54:29.000000 gpt_trans-0.0.2/gpt_trans/main.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-04-19 09:56:55.452133 gpt_trans-0.0.2/gpt_trans.egg-info/
--rw-r--r--   0 zilliz     (501) staff       (20)      331 2024-04-19 09:56:55.000000 gpt_trans-0.0.2/gpt_trans.egg-info/PKG-INFO
--rw-r--r--   0 zilliz     (501) staff       (20)      258 2024-04-19 09:56:55.000000 gpt_trans-0.0.2/gpt_trans.egg-info/SOURCES.txt
--rw-r--r--   0 zilliz     (501) staff       (20)        1 2024-04-19 09:56:55.000000 gpt_trans-0.0.2/gpt_trans.egg-info/dependency_links.txt
--rw-r--r--   0 zilliz     (501) staff       (20)       50 2024-04-19 09:56:55.000000 gpt_trans-0.0.2/gpt_trans.egg-info/entry_points.txt
--rw-r--r--   0 zilliz     (501) staff       (20)       76 2024-04-19 09:56:55.000000 gpt_trans-0.0.2/gpt_trans.egg-info/requires.txt
--rw-r--r--   0 zilliz     (501) staff       (20)       10 2024-04-19 09:56:55.000000 gpt_trans-0.0.2/gpt_trans.egg-info/top_level.txt
--rw-r--r--   0 zilliz     (501) staff       (20)       38 2024-04-19 09:56:55.452655 gpt_trans-0.0.2/setup.cfg
--rw-r--r--   0 zilliz     (501) staff       (20)      535 2024-04-19 09:54:29.000000 gpt_trans-0.0.2/setup.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-04-19 12:47:27.293176 gpt_trans-0.0.3/
+-rw-r--r--   0 zilliz     (501) staff       (20)      165 2024-04-19 12:47:27.293045 gpt_trans-0.0.3/PKG-INFO
+-rw-r--r--   0 zilliz     (501) staff       (20)     2507 2024-04-19 09:54:56.000000 gpt_trans-0.0.3/README.md
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-04-19 12:47:27.291964 gpt_trans-0.0.3/gpt_trans/
+-rw-r--r--   0 zilliz     (501) staff       (20)        0 2024-04-19 04:53:22.000000 gpt_trans-0.0.3/gpt_trans/__init__.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     4623 2024-04-19 09:54:29.000000 gpt_trans-0.0.3/gpt_trans/main.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-04-19 12:47:27.292871 gpt_trans-0.0.3/gpt_trans.egg-info/
+-rw-r--r--   0 zilliz     (501) staff       (20)      165 2024-04-19 12:47:27.000000 gpt_trans-0.0.3/gpt_trans.egg-info/PKG-INFO
+-rw-r--r--   0 zilliz     (501) staff       (20)      258 2024-04-19 12:47:27.000000 gpt_trans-0.0.3/gpt_trans.egg-info/SOURCES.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)        1 2024-04-19 12:47:27.000000 gpt_trans-0.0.3/gpt_trans.egg-info/dependency_links.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)       50 2024-04-19 12:47:27.000000 gpt_trans-0.0.3/gpt_trans.egg-info/entry_points.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)       76 2024-04-19 12:47:27.000000 gpt_trans-0.0.3/gpt_trans.egg-info/requires.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)       10 2024-04-19 12:47:27.000000 gpt_trans-0.0.3/gpt_trans.egg-info/top_level.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)       38 2024-04-19 12:47:27.293220 gpt_trans-0.0.3/setup.cfg
+-rw-r--r--   0 zilliz     (501) staff       (20)      535 2024-04-19 12:18:17.000000 gpt_trans-0.0.3/setup.py
```

### Comparing `gpt_trans-0.0.2/README.md` & `gpt_trans-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt_trans-0.0.2/gpt_trans/main.py` & `gpt_trans-0.0.3/gpt_trans/main.py`

 * *Files identical despite different names*

### Comparing `gpt_trans-0.0.2/setup.py` & `gpt_trans-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gpt_trans',
-    version='0.0.2',
+    version='0.0.3',
     py_modules=['gpt_trans'],
     install_requires=[
         'langchain',
         'langchain_community',
         'langchain_core',
         'langchain_openai',
         'tqdm',
```

