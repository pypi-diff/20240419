# Comparing `tmp/pyracf-0.8.4.tar.gz` & `tmp/pyracf-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.8.4.tar", last modified: Tue Apr 16 21:33:11 2024, max compression
+gzip compressed data, was "pyracf-0.8.5.tar", last modified: Fri Apr 19 17:31:30 2024, max compression
```

## Comparing `pyracf-0.8.4.tar` & `pyracf-0.8.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.8.4/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.8.4/MANIFEST.in
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-16 21:33:11.184994 pyracf-0.8.4/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)    14510 2024-04-16 21:31:02.000000 pyracf-0.8.4/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-16 21:33:11.184994 pyracf-0.8.4/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-16 21:32:36.000000 pyracf-0.8.4/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    56953 2024-04-16 21:31:08.000000 pyracf-0.8.4/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-15 10:15:48.000000 pyracf-0.8.4/src/pyracf/getOffsets.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-15 10:15:48.000000 pyracf-0.8.4/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/pyracf.egg-info/
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      279 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/top_level.txt
+drwxr-xr-x   0 henri      (501) staff       (20)        0 2024-04-19 17:31:30.921931 pyracf-0.8.5/
+-rw-r--r--   0 henri      (501) staff       (20)    11357 2024-04-18 10:17:43.000000 pyracf-0.8.5/LICENSE
+-rw-r--r--   0 henri      (501) staff       (20)      172 2024-04-18 10:17:43.000000 pyracf-0.8.5/MANIFEST.in
+-rw-r--r--   0 henri      (501) staff       (20)    15118 2024-04-19 17:31:30.921702 pyracf-0.8.5/PKG-INFO
+-rw-r--r--   0 henri      (501) staff       (20)    14510 2024-04-19 17:29:55.000000 pyracf-0.8.5/README.md
+-rw-r--r--   0 henri      (501) staff       (20)       38 2024-04-19 17:31:30.921969 pyracf-0.8.5/setup.cfg
+-rw-r--r--   0 henri      (501) staff       (20)      956 2024-04-19 17:31:18.000000 pyracf-0.8.5/setup.py
+drwxr-xr-x   0 henri      (501) staff       (20)        0 2024-04-19 17:31:30.919204 pyracf-0.8.5/src/
+drwxr-xr-x   0 henri      (501) staff       (20)        0 2024-04-19 17:31:30.920406 pyracf-0.8.5/src/pyracf/
+-rw-r--r--   0 henri      (501) staff       (20)    56953 2024-04-19 17:29:55.000000 pyracf-0.8.5/src/pyracf/__init__.py
+-rw-r--r--   0 henri      (501) staff       (20)     1829 2024-04-18 10:17:43.000000 pyracf-0.8.5/src/pyracf/getOffsets.py
+-rw-r--r--   0 henri      (501) staff       (20)   253950 2024-04-18 10:17:43.000000 pyracf-0.8.5/src/pyracf/offsets.json
+drwxr-xr-x   0 henri      (501) staff       (20)        0 2024-04-19 17:31:30.921522 pyracf-0.8.5/src/pyracf.egg-info/
+-rw-r--r--   0 henri      (501) staff       (20)    15118 2024-04-19 17:31:30.000000 pyracf-0.8.5/src/pyracf.egg-info/PKG-INFO
+-rw-r--r--   0 henri      (501) staff       (20)      279 2024-04-19 17:31:30.000000 pyracf-0.8.5/src/pyracf.egg-info/SOURCES.txt
+-rw-r--r--   0 henri      (501) staff       (20)        1 2024-04-19 17:31:30.000000 pyracf-0.8.5/src/pyracf.egg-info/dependency_links.txt
+-rw-r--r--   0 henri      (501) staff       (20)       38 2024-04-19 17:31:30.000000 pyracf-0.8.5/src/pyracf.egg-info/requires.txt
+-rw-r--r--   0 henri      (501) staff       (20)        7 2024-04-19 17:31:30.000000 pyracf-0.8.5/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.8.4/LICENSE` & `pyracf-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/PKG-INFO` & `pyracf-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.4
+Version: 0.8.5
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyracf-0.8.4/README.md` & `pyracf-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/setup.py` & `pyracf-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.8.4",
+    version="0.8.5",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.8.4/src/pyracf/__init__.py` & `pyracf-0.8.5/src/pyracf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/src/pyracf/getOffsets.py` & `pyracf-0.8.5/src/pyracf/getOffsets.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/src/pyracf/offsets.json` & `pyracf-0.8.5/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.8.5/src/pyracf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.4
+Version: 0.8.5
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

