# Comparing `tmp/cerbogen-0.0.3.tar.gz` & `tmp/cerbogen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.3.tar", last modified: Fri Apr 19 06:37:40 2024, max compression
+gzip compressed data, was "cerbogen-0.0.4.tar", last modified: Fri Apr 19 07:03:56 2024, max compression
```

## Comparing `cerbogen-0.0.3.tar` & `cerbogen-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:37:40.402643 cerbogen-0.0.3/
--rw-rw-rw-   0        0        0      724 2024-04-19 06:37:40.394638 cerbogen-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 06:37:40.382636 cerbogen-0.0.3/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.3/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8857 2024-04-19 05:52:08.000000 cerbogen-0.0.3/cerbogen/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.3/cerbogen/check.py
--rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.3/cerbogen/plot.py
--rw-rw-rw-   0        0        0     8982 2024-04-19 06:02:06.000000 cerbogen-0.0.3/cerbogen/ui.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:37:40.393637 cerbogen-0.0.3/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      724 2024-04-19 06:37:40.000000 cerbogen-0.0.3/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-04-19 06:37:40.000000 cerbogen-0.0.3/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:37:40.000000 cerbogen-0.0.3/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-19 06:37:40.000000 cerbogen-0.0.3/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-19 06:37:40.000000 cerbogen-0.0.3/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 06:37:40.403641 cerbogen-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-04-19 06:37:39.000000 cerbogen-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:03:56.367076 cerbogen-0.0.4/
+-rw-rw-rw-   0        0        0      700 2024-04-19 07:03:56.366076 cerbogen-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 07:03:56.341076 cerbogen-0.0.4/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.4/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     8857 2024-04-19 05:52:08.000000 cerbogen-0.0.4/cerbogen/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.4/cerbogen/check.py
+-rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.4/cerbogen/plot.py
+-rw-rw-rw-   0        0        0     8982 2024-04-19 06:02:06.000000 cerbogen-0.0.4/cerbogen/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:03:56.366076 cerbogen-0.0.4/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      700 2024-04-19 07:03:56.000000 cerbogen-0.0.4/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-19 07:03:56.000000 cerbogen-0.0.4/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:03:56.000000 cerbogen-0.0.4/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-19 07:03:56.000000 cerbogen-0.0.4/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 07:03:56.000000 cerbogen-0.0.4/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:03:56.368076 cerbogen-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      866 2024-04-19 07:03:55.000000 cerbogen-0.0.4/setup.py
```

### Comparing `cerbogen-0.0.3/PKG-INFO` & `cerbogen-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: tkinter
 Requires-Dist: matplotlib
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: wave
 Requires-Dist: librosa
```

### Comparing `cerbogen-0.0.3/cerbogen/cerbogen.py` & `cerbogen-0.0.4/cerbogen/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.3/cerbogen/check.py` & `cerbogen-0.0.4/cerbogen/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.3/cerbogen/plot.py` & `cerbogen-0.0.4/cerbogen/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.3/cerbogen/ui.py` & `cerbogen-0.0.4/cerbogen/ui.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.3/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.4/cerbogen.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: tkinter
 Requires-Dist: matplotlib
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: wave
 Requires-Dist: librosa
```

### Comparing `cerbogen-0.0.3/setup.py` & `cerbogen-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cerbogen',
-    version = '0.0.3',
+    version = '0.0.4',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
     install_requires=[
-        "tkinter", "matplotlib", "pydub", "numpy", "wave", "librosa"
+         "matplotlib", "pydub", "numpy", "wave", "librosa"
     ],
 
     python_requires='>=3.6',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

