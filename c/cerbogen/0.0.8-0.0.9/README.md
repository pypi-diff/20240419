# Comparing `tmp/cerbogen-0.0.8.tar.gz` & `tmp/cerbogen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.8.tar", last modified: Fri Apr 19 08:03:58 2024, max compression
+gzip compressed data, was "cerbogen-0.0.9.tar", last modified: Fri Apr 19 08:07:30 2024, max compression
```

## Comparing `cerbogen-0.0.8.tar` & `cerbogen-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:03:58.195418 cerbogen-0.0.8/
--rw-rw-rw-   0        0        0      700 2024-04-19 08:03:58.195418 cerbogen-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:03:58.181417 cerbogen-0.0.8/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.8/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8856 2024-04-19 07:05:53.000000 cerbogen-0.0.8/cerbogen/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.8/cerbogen/check.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:03:58.193416 cerbogen-0.0.8/cerbogen/ffmpeg/
--rw-rw-rw-   0        0        0    35147 2023-12-31 08:04:26.000000 cerbogen-0.0.8/cerbogen/ffmpeg/LICENSE
--rw-rw-rw-   0        0        0    42234 2023-12-31 08:04:27.000000 cerbogen-0.0.8/cerbogen/ffmpeg/README.txt
--rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.8/cerbogen/plot.py
--rw-rw-rw-   0        0        0     8982 2024-04-19 06:02:06.000000 cerbogen-0.0.8/cerbogen/ui.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:03:58.194416 cerbogen-0.0.8/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      700 2024-04-19 08:03:58.000000 cerbogen-0.0.8/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-19 08:03:58.000000 cerbogen-0.0.8/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:03:58.000000 cerbogen-0.0.8/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-19 08:03:58.000000 cerbogen-0.0.8/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-19 08:03:58.000000 cerbogen-0.0.8/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 08:03:58.195418 cerbogen-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      909 2024-04-19 08:03:57.000000 cerbogen-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.389639 cerbogen-0.0.9/
+-rw-rw-rw-   0        0        0      700 2024-04-19 08:07:30.388636 cerbogen-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.367637 cerbogen-0.0.9/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.9/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     8856 2024-04-19 07:05:53.000000 cerbogen-0.0.9/cerbogen/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.9/cerbogen/check.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.387652 cerbogen-0.0.9/cerbogen/ffmpeg/
+-rw-rw-rw-   0        0        0    35147 2023-12-31 08:04:26.000000 cerbogen-0.0.9/cerbogen/ffmpeg/LICENSE
+-rw-rw-rw-   0        0        0    42234 2023-12-31 08:04:27.000000 cerbogen-0.0.9/cerbogen/ffmpeg/README.txt
+-rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.9/cerbogen/plot.py
+-rw-rw-rw-   0        0        0     8965 2024-04-19 08:05:35.000000 cerbogen-0.0.9/cerbogen/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.388636 cerbogen-0.0.9/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      700 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:07:30.389639 cerbogen-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      909 2024-04-19 08:07:29.000000 cerbogen-0.0.9/setup.py
```

### Comparing `cerbogen-0.0.8/PKG-INFO` & `cerbogen-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.8/cerbogen/cerbogen.py` & `cerbogen-0.0.9/cerbogen/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.8/cerbogen/check.py` & `cerbogen-0.0.9/cerbogen/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.8/cerbogen/ffmpeg/LICENSE` & `cerbogen-0.0.9/cerbogen/ffmpeg/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.8/cerbogen/ffmpeg/README.txt` & `cerbogen-0.0.9/cerbogen/ffmpeg/README.txt`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.8/cerbogen/plot.py` & `cerbogen-0.0.9/cerbogen/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.8/cerbogen/ui.py` & `cerbogen-0.0.9/cerbogen/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tkinter as tk
 from tkinter import ttk
 from tkinter import messagebox
-from CerboGen.modules.cerbogen import binbeats
+from cerbogen import binbeats
 
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from plot import Plot
 
 def generate_binaural_beats():
     base_f = float(base_entry.get())
```

### Comparing `cerbogen-0.0.8/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.9/cerbogen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.8/setup.py` & `cerbogen-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cerbogen',
-    version = '0.0.8',
+    version = '0.0.9',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```

