# Comparing `tmp/asyffmpeg-0.2.tar.gz` & `tmp/asyffmpeg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyffmpeg-0.2.tar", last modified: Fri Apr 19 05:56:15 2024, max compression
+gzip compressed data, was "asyffmpeg-0.2.1.tar", last modified: Fri Apr 19 06:01:06 2024, max compression
```

## Comparing `asyffmpeg-0.2.tar` & `asyffmpeg-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:15.520590 asyffmpeg-0.2/
--rw-rw-rw-   0        0        0     1944 2024-04-19 05:56:15.518596 asyffmpeg-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1504 2024-04-19 05:54:37.000000 asyffmpeg-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:15.506846 asyffmpeg-0.2/asyffmpeg/
--rw-rw-rw-   0        0        0    10790 2024-04-19 05:53:21.000000 asyffmpeg-0.2/asyffmpeg/__init__.py
--rw-rw-rw-   0        0        0     1140 2024-04-18 17:06:39.000000 asyffmpeg-0.2/asyffmpeg/statistic.py
--rw-rw-rw-   0        0        0      997 2024-04-18 16:54:54.000000 asyffmpeg-0.2/asyffmpeg/tempf.py
--rw-rw-rw-   0        0        0     2169 2024-04-18 16:53:26.000000 asyffmpeg-0.2/asyffmpeg/util.py
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:15.517610 asyffmpeg-0.2/asyffmpeg.egg-info/
--rw-rw-rw-   0        0        0     1944 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 05:56:15.000000 asyffmpeg-0.2/asyffmpeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 05:56:15.520590 asyffmpeg-0.2/setup.cfg
--rw-rw-rw-   0        0        0      761 2024-04-19 05:56:12.000000 asyffmpeg-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:01:06.932465 asyffmpeg-0.2.1/
+-rw-rw-rw-   0        0        0     1953 2024-04-19 06:01:06.930451 asyffmpeg-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1504 2024-04-19 05:54:37.000000 asyffmpeg-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 06:01:06.916485 asyffmpeg-0.2.1/asyffmpeg/
+-rw-rw-rw-   0        0        0    10790 2024-04-19 05:53:21.000000 asyffmpeg-0.2.1/asyffmpeg/__init__.py
+-rw-rw-rw-   0        0        0     1140 2024-04-18 17:06:39.000000 asyffmpeg-0.2.1/asyffmpeg/statistic.py
+-rw-rw-rw-   0        0        0      997 2024-04-18 16:54:54.000000 asyffmpeg-0.2.1/asyffmpeg/tempf.py
+-rw-rw-rw-   0        0        0     2169 2024-04-18 16:53:26.000000 asyffmpeg-0.2.1/asyffmpeg/util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:01:06.928462 asyffmpeg-0.2.1/asyffmpeg.egg-info/
+-rw-rw-rw-   0        0        0     1953 2024-04-19 06:01:06.000000 asyffmpeg-0.2.1/asyffmpeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-19 06:01:06.000000 asyffmpeg-0.2.1/asyffmpeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 06:01:06.000000 asyffmpeg-0.2.1/asyffmpeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-19 06:01:06.000000 asyffmpeg-0.2.1/asyffmpeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 06:01:06.000000 asyffmpeg-0.2.1/asyffmpeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 06:01:06.932465 asyffmpeg-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      654 2024-04-19 06:01:02.000000 asyffmpeg-0.2.1/setup.py
```

### Comparing `asyffmpeg-0.2/PKG-INFO` & `asyffmpeg-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: asyffmpeg
-Version: 0.2
+Version: 0.2.1
 Summary: A library for asynchronous operation with FFmpeg, providing the ability to track events such as start, end, and encoding progress.
 Home-page: https://github.com/drhspfn/asyffmpeg
 Author: drhspfn
 Author-email: jenya.gsta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles
-Requires-Dist: ffprobe
+Requires-Dist: ffprobe-python
 
 # AsyFFmpeg
 
 AsyFFmpeg is a Python library for interacting asynchronously with FFmpeg to perform various operations on media files.
 
 ## Installation
```

### Comparing `asyffmpeg-0.2/README.md` & `asyffmpeg-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2/asyffmpeg/__init__.py` & `asyffmpeg-0.2.1/asyffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2/asyffmpeg/statistic.py` & `asyffmpeg-0.2.1/asyffmpeg/statistic.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2/asyffmpeg/tempf.py` & `asyffmpeg-0.2.1/asyffmpeg/tempf.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2/asyffmpeg/util.py` & `asyffmpeg-0.2.1/asyffmpeg/util.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2/asyffmpeg.egg-info/PKG-INFO` & `asyffmpeg-0.2.1/asyffmpeg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: asyffmpeg
-Version: 0.2
+Version: 0.2.1
 Summary: A library for asynchronous operation with FFmpeg, providing the ability to track events such as start, end, and encoding progress.
 Home-page: https://github.com/drhspfn/asyffmpeg
 Author: drhspfn
 Author-email: jenya.gsta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles
-Requires-Dist: ffprobe
+Requires-Dist: ffprobe-python
 
 # AsyFFmpeg
 
 AsyFFmpeg is a Python library for interacting asynchronously with FFmpeg to perform various operations on media files.
 
 ## Installation
```

### Comparing `asyffmpeg-0.2/setup.py` & `asyffmpeg-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='asyffmpeg',
-    version='0.2',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         'aiofiles',
-        'ffprobe',
-        # Додайте інші залежності, які необхідні для вашого пакету
+        'ffprobe-python',
     ],
     author='drhspfn',
     author_email='jenya.gsta@gmail.com',
     description='A library for asynchronous operation with FFmpeg, providing the ability to track events such as start, end, and encoding progress.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/drhspfn/asyffmpeg',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

