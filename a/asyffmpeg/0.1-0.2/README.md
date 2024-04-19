# Comparing `tmp/asyffmpeg-0.1.tar.gz` & `tmp/asyffmpeg-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyffmpeg-0.1.tar", last modified: Thu Apr 18 17:37:42 2024, max compression
+gzip compressed data, was "asyffmpeg-0.2.tar", last modified: Fri Apr 19 05:56:15 2024, max compression
```

## Comparing `asyffmpeg-0.1.tar` & `asyffmpeg-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 17:37:42.591281 asyffmpeg-0.1/
--rw-rw-rw-   0        0        0     1901 2024-04-18 17:37:42.588272 asyffmpeg-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1461 2024-04-18 17:34:33.000000 asyffmpeg-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 17:37:42.576303 asyffmpeg-0.1/asyffmpeg/
--rw-rw-rw-   0        0        0    10798 2024-04-18 17:09:16.000000 asyffmpeg-0.1/asyffmpeg/__init__.py
--rw-rw-rw-   0        0        0     1140 2024-04-18 17:06:39.000000 asyffmpeg-0.1/asyffmpeg/statistic.py
--rw-rw-rw-   0        0        0      997 2024-04-18 16:54:54.000000 asyffmpeg-0.1/asyffmpeg/tempf.py
--rw-rw-rw-   0        0        0     2169 2024-04-18 16:53:26.000000 asyffmpeg-0.1/asyffmpeg/util.py
-drwxrwxrwx   0        0        0        0 2024-04-18 17:37:42.587275 asyffmpeg-0.1/asyffmpeg.egg-info/
--rw-rw-rw-   0        0        0     1901 2024-04-18 17:37:42.000000 asyffmpeg-0.1/asyffmpeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-18 17:37:42.000000 asyffmpeg-0.1/asyffmpeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 17:37:42.000000 asyffmpeg-0.1/asyffmpeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 17:37:42.000000 asyffmpeg-0.1/asyffmpeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 17:37:42.000000 asyffmpeg-0.1/asyffmpeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 17:37:42.592261 asyffmpeg-0.1/setup.cfg
--rw-rw-rw-   0        0        0      761 2024-04-18 17:37:31.000000 asyffmpeg-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:15.520590 asyffmpeg-0.2/
+-rw-rw-rw-   0        0        0     1944 2024-04-19 05:56:15.518596 asyffmpeg-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1504 2024-04-19 05:54:37.000000 asyffmpeg-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:15.506846 asyffmpeg-0.2/asyffmpeg/
+-rw-rw-rw-   0        0        0    10790 2024-04-19 05:53:21.000000 asyffmpeg-0.2/asyffmpeg/__init__.py
+-rw-rw-rw-   0        0        0     1140 2024-04-18 17:06:39.000000 asyffmpeg-0.2/asyffmpeg/statistic.py
+-rw-rw-rw-   0        0        0      997 2024-04-18 16:54:54.000000 asyffmpeg-0.2/asyffmpeg/tempf.py
+-rw-rw-rw-   0        0        0     2169 2024-04-18 16:53:26.000000 asyffmpeg-0.2/asyffmpeg/util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:15.517610 asyffmpeg-0.2/asyffmpeg.egg-info/
+-rw-rw-rw-   0        0        0     1944 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 05:56:15.520590 asyffmpeg-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      761 2024-04-19 05:56:12.000000 asyffmpeg-0.2/setup.py
```

### Comparing `asyffmpeg-0.1/PKG-INFO` & `asyffmpeg-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyffmpeg
-Version: 0.1
+Version: 0.2
 Summary: A library for asynchronous operation with FFmpeg, providing the ability to track events such as start, end, and encoding progress.
 Home-page: https://github.com/drhspfn/asyffmpeg
 Author: drhspfn
 Author-email: jenya.gsta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles
@@ -16,14 +16,15 @@
 
 ## Installation
 
 To install AsyFFmpeg, run the following command:
 
 ```bash
 pip install asyffmpeg
+pip install -r requirements.txt --upgrade
 ```
 
 ## Usage
 An example of how to use the library:
 ```python
 import asyncio
 from asyffmpeg import AsyFFmpeg
```

### Comparing `asyffmpeg-0.1/README.md` & `asyffmpeg-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 ## Installation
 
 To install AsyFFmpeg, run the following command:
 
 ```bash
 pip install asyffmpeg
+pip install -r requirements.txt --upgrade
 ```
 
 ## Usage
 An example of how to use the library:
 ```python
 import asyncio
 from asyffmpeg import AsyFFmpeg
```

### Comparing `asyffmpeg-0.1/asyffmpeg/__init__.py` & `asyffmpeg-0.2/asyffmpeg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from datetime import timedelta, datetime
 import logging
 from .statistic import Statistics
 import aiofiles
 from typing import Awaitable, Callable, Dict, List, Literal, Union
 from .tempf import TempFile
-from ffprobe.ffprobe import FFProbe
+from ffprobe import FFProbe
 
 from .util import convert_to_seconds
 
 class AsyFFmpeg:
     """
     A class for asynchronous FFmpeg processing.
```

### Comparing `asyffmpeg-0.1/asyffmpeg/statistic.py` & `asyffmpeg-0.2/asyffmpeg/statistic.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.1/asyffmpeg/tempf.py` & `asyffmpeg-0.2/asyffmpeg/tempf.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.1/asyffmpeg/util.py` & `asyffmpeg-0.2/asyffmpeg/util.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.1/asyffmpeg.egg-info/PKG-INFO` & `asyffmpeg-0.2/asyffmpeg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyffmpeg
-Version: 0.1
+Version: 0.2
 Summary: A library for asynchronous operation with FFmpeg, providing the ability to track events such as start, end, and encoding progress.
 Home-page: https://github.com/drhspfn/asyffmpeg
 Author: drhspfn
 Author-email: jenya.gsta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles
@@ -16,14 +16,15 @@
 
 ## Installation
 
 To install AsyFFmpeg, run the following command:
 
 ```bash
 pip install asyffmpeg
+pip install -r requirements.txt --upgrade
 ```
 
 ## Usage
 An example of how to use the library:
 ```python
 import asyncio
 from asyffmpeg import AsyFFmpeg
```

### Comparing `asyffmpeg-0.1/setup.py` & `asyffmpeg-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='asyffmpeg',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'aiofiles',
         'ffprobe',
         # Додайте інші залежності, які необхідні для вашого пакету
     ],
     author='drhspfn',
```

