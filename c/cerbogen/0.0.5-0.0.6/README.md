# Comparing `tmp/cerbogen-0.0.5.tar.gz` & `tmp/cerbogen-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.5.tar", last modified: Fri Apr 19 07:06:01 2024, max compression
+gzip compressed data, was "cerbogen-0.0.6.tar", last modified: Fri Apr 19 07:12:22 2024, max compression
```

## Comparing `cerbogen-0.0.5.tar` & `cerbogen-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:06:01.126746 cerbogen-0.0.5/
--rw-rw-rw-   0        0        0      700 2024-04-19 07:06:01.125745 cerbogen-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 07:06:01.112748 cerbogen-0.0.5/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.5/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8856 2024-04-19 07:05:53.000000 cerbogen-0.0.5/cerbogen/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.5/cerbogen/check.py
--rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.5/cerbogen/plot.py
--rw-rw-rw-   0        0        0     8982 2024-04-19 06:02:06.000000 cerbogen-0.0.5/cerbogen/ui.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:06:01.124747 cerbogen-0.0.5/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      700 2024-04-19 07:06:00.000000 cerbogen-0.0.5/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-04-19 07:06:01.000000 cerbogen-0.0.5/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:06:00.000000 cerbogen-0.0.5/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-19 07:06:00.000000 cerbogen-0.0.5/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-19 07:06:00.000000 cerbogen-0.0.5/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 07:06:01.126746 cerbogen-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      866 2024-04-19 07:06:00.000000 cerbogen-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:12:22.224123 cerbogen-0.0.6/
+-rw-rw-rw-   0        0        0      700 2024-04-19 07:12:22.222119 cerbogen-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 07:12:22.187119 cerbogen-0.0.6/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.6/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     8856 2024-04-19 07:05:53.000000 cerbogen-0.0.6/cerbogen/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.6/cerbogen/check.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:12:22.220117 cerbogen-0.0.6/cerbogen/ffmpeg/
+-rw-rw-rw-   0        0        0    35147 2023-12-31 08:04:26.000000 cerbogen-0.0.6/cerbogen/ffmpeg/LICENSE
+-rw-rw-rw-   0        0        0    42234 2023-12-31 08:04:27.000000 cerbogen-0.0.6/cerbogen/ffmpeg/README.txt
+-rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.6/cerbogen/plot.py
+-rw-rw-rw-   0        0        0     8982 2024-04-19 06:02:06.000000 cerbogen-0.0.6/cerbogen/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:12:22.221118 cerbogen-0.0.6/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      700 2024-04-19 07:12:22.000000 cerbogen-0.0.6/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-19 07:12:22.000000 cerbogen-0.0.6/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:12:22.000000 cerbogen-0.0.6/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-19 07:12:22.000000 cerbogen-0.0.6/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 07:12:22.000000 cerbogen-0.0.6/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:12:22.224123 cerbogen-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      909 2024-04-19 07:12:21.000000 cerbogen-0.0.6/setup.py
```

### Comparing `cerbogen-0.0.5/PKG-INFO` & `cerbogen-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.5/cerbogen/cerbogen.py` & `cerbogen-0.0.6/cerbogen/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.5/cerbogen/check.py` & `cerbogen-0.0.6/cerbogen/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.5/cerbogen/plot.py` & `cerbogen-0.0.6/cerbogen/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.5/cerbogen/ui.py` & `cerbogen-0.0.6/cerbogen/ui.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.5/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.6/cerbogen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.5/setup.py` & `cerbogen-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cerbogen',
-    version = '0.0.5',
+    version = '0.0.6',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
+
+     package_data={'': ['ffmpeg/*']},
+
     install_requires=[
          "matplotlib", "pydub", "numpy", "wave", "librosa"
     ],
 
     python_requires='>=3.6',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

