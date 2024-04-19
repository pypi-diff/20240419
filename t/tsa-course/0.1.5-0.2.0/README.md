# Comparing `tmp/tsa_course-0.1.5.tar.gz` & `tmp/tsa_course-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsa_course-0.1.5.tar", last modified: Wed Apr 17 00:22:53 2024, max compression
+gzip compressed data, was "tsa_course-0.2.0.tar", last modified: Fri Apr 19 20:12:30 2024, max compression
```

## Comparing `tsa_course-0.1.5.tar` & `tsa_course-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-17 00:22:53.469711 tsa_course-0.1.5/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.1.5/LICENSE
--rw-r--r--   0 filippo   (1001) filippo   (1001)     8175 2024-04-17 00:22:53.469711 tsa_course-0.1.5/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     7455 2024-04-17 00:21:56.000000 tsa_course-0.1.5/README.md
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-17 00:22:53.469711 tsa_course-0.1.5/setup.cfg
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-17 00:22:10.000000 tsa_course-0.1.5/setup.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-17 00:22:53.469711 tsa_course-0.1.5/tsa_course/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.1.5/tsa_course/__init__.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)    13644 2024-04-17 00:13:18.000000 tsa_course-0.1.5/tsa_course/lecture11.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-17 00:22:53.469711 tsa_course-0.1.5/tsa_course.egg-info/
--rw-r--r--   0 filippo   (1001) filippo   (1001)     8175 2024-04-17 00:22:53.000000 tsa_course-0.1.5/tsa_course.egg-info/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      242 2024-04-17 00:22:53.000000 tsa_course-0.1.5/tsa_course.egg-info/SOURCES.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-17 00:22:53.000000 tsa_course-0.1.5/tsa_course.egg-info/dependency_links.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-17 00:22:53.000000 tsa_course-0.1.5/tsa_course.egg-info/requires.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-17 00:22:53.000000 tsa_course-0.1.5/tsa_course.egg-info/top_level.txt
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:12:30.065765 tsa_course-0.2.0/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.2.0/LICENSE
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8175 2024-04-19 20:12:30.065765 tsa_course-0.2.0/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     7455 2024-04-17 00:21:56.000000 tsa_course-0.2.0/README.md
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-19 20:12:30.065765 tsa_course-0.2.0/setup.cfg
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-19 20:11:36.000000 tsa_course-0.2.0/setup.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:12:30.065765 tsa_course-0.2.0/tsa_course/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.2.0/tsa_course/__init__.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1190 2024-04-18 13:30:31.000000 tsa_course-0.2.0/tsa_course/lecture1.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)    13644 2024-04-17 00:13:18.000000 tsa_course-0.2.0/tsa_course/lecture11.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     3309 2024-04-19 19:32:21.000000 tsa_course-0.2.0/tsa_course/lecture8.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:12:30.065765 tsa_course-0.2.0/tsa_course.egg-info/
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8175 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      288 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/SOURCES.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/dependency_links.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/requires.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/top_level.txt
```

### Comparing `tsa_course-0.1.5/LICENSE` & `tsa_course-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsa_course-0.1.5/PKG-INFO` & `tsa_course-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsa_course
-Version: 0.1.5
+Version: 0.2.0
 Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.1.5 Summary: A collection of
+Metadata-Version: 2.1 Name: tsa_course Version: 0.2.0 Summary: A collection of
 scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
 URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
 handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `tsa_course-0.1.5/README.md` & `tsa_course-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tsa_course-0.1.5/setup.py` & `tsa_course-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tsa_course",
-    version="0.1.5",
+    version="0.2.0",
     packages=find_packages(),
     python_requires='>=3.10',
     install_requires=[
         'numpy>1.19.5',
         'matplotlib',
         'scipy',
         'tqdm'
```

### Comparing `tsa_course-0.1.5/tsa_course/lecture11.py` & `tsa_course-0.2.0/tsa_course/lecture11.py`

 * *Files identical despite different names*

### Comparing `tsa_course-0.1.5/tsa_course.egg-info/PKG-INFO` & `tsa_course-0.2.0/tsa_course.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsa_course
-Version: 0.1.5
+Version: 0.2.0
 Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.1.5 Summary: A collection of
+Metadata-Version: 2.1 Name: tsa_course Version: 0.2.0 Summary: A collection of
 scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
 URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
 handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

