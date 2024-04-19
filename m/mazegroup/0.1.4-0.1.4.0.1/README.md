# Comparing `tmp/mazegroup-0.1.4.tar.gz` & `tmp/mazegroup-0.1.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazegroup-0.1.4.tar", last modified: Thu Apr 11 15:49:47 2024, max compression
+gzip compressed data, was "mazegroup-0.1.4.0.1.tar", last modified: Fri Apr 19 14:27:11 2024, max compression
```

## Comparing `mazegroup-0.1.4.tar` & `mazegroup-0.1.4.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.977552 mazegroup-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-11 15:49:47.977552 mazegroup-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-11 15:49:43.000000 mazegroup-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/calc/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/calc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/cd/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/cd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/echo/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/echo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/help/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/ls/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/pyeval/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/pyeval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/pyexec/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/pyexec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/pypkg/
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/pypkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/quit/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/quit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/saves/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/saves/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/sc/
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/sc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup/sc/out/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/sc/out/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.977552 mazegroup-0.1.4/mazegroup/sc/temp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/sc/temp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.977552 mazegroup-0.1.4/mazegroup/shell/
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 15:49:43.000000 mazegroup-0.1.4/mazegroup/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:47.973552 mazegroup-0.1.4/mazegroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-11 15:49:47.000000 mazegroup-0.1.4/mazegroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-11 15:49:47.000000 mazegroup-0.1.4/mazegroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:49:47.000000 mazegroup-0.1.4/mazegroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 15:49:47.000000 mazegroup-0.1.4/mazegroup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 15:49:47.000000 mazegroup-0.1.4/mazegroup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 15:49:47.000000 mazegroup-0.1.4/mazegroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:49:47.977552 mazegroup-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-11 15:49:43.000000 mazegroup-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/calc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/cd/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/cd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/echo/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/echo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/ls/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/pyeval/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/pyeval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/pyexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/pyexec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/pypkg/
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/pypkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/quit/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/quit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/saves/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/saves/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/sc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/sc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/sc/out/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/sc/out/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/sc/temp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/sc/temp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/setup.py
```

### Comparing `mazegroup-0.1.4/PKG-INFO` & `mazegroup-0.1.4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.4
+Version: 0.1.4.0.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.4/README.md` & `mazegroup-0.1.4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/calc/__init__.py` & `mazegroup-0.1.4.0.1/mazegroup/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/commands.py` & `mazegroup-0.1.4.0.1/mazegroup/commands.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/help/__init__.py` & `mazegroup-0.1.4.0.1/mazegroup/help/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/pyeval/__init__.py` & `mazegroup-0.1.4.0.1/mazegroup/pyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/pyexec/__init__.py` & `mazegroup-0.1.4.0.1/mazegroup/pyexec/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/pypkg/__init__.py` & `mazegroup-0.1.4.0.1/mazegroup/pypkg/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/sc/__init__.py` & `mazegroup-0.1.4.0.1/mazegroup/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/shell/__init__.py` & `mazegroup-0.1.4.0.1/mazegroup/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup/utils.py` & `mazegroup-0.1.4.0.1/mazegroup/utils.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/mazegroup.egg-info/PKG-INFO` & `mazegroup-0.1.4.0.1/mazegroup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.4
+Version: 0.1.4.0.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.4/mazegroup.egg-info/SOURCES.txt` & `mazegroup-0.1.4.0.1/mazegroup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4/setup.py` & `mazegroup-0.1.4.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mazegroup",
-    version="0.1.4",
+    version="0.1.4.0.1",
     description="MazeGroup.py is an general prupose library for Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Genius_um",
     python_requires=">=3.9",
     url="https://github.com/Geniusum/mazegroup.py",
     packages=find_packages(),#["mazegroup", "mazegroup/cli", "mazegroup/echo", "mazegroup/saves"], # find_packages(),
@@ -19,10 +19,11 @@
         'console_scripts': [
             'mg = mazegroup.cli:main',
             'mazegroup = mazegroup.cli:main'
         ]
     },
     install_requires=[
         "cryptography",
-        "colorama"
+        "colorama",
+        "keyboard"
     ]
 )
```

