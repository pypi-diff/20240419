# Comparing `tmp/Xodia24-0.0.5.tar.gz` & `tmp/Xodia24-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xodia24-0.0.5.tar", last modified: Mon Apr  1 15:09:11 2024, max compression
+gzip compressed data, was "Xodia24-0.0.6.tar", last modified: Fri Apr 19 05:37:56 2024, max compression
```

## Comparing `Xodia24-0.0.5.tar` & `Xodia24-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 15:09:11.489318 Xodia24-0.0.5/
--rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5809 2024-04-01 15:09:11.486949 Xodia24-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5075 2024-04-01 15:09:02.000000 Xodia24-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 15:09:11.478932 Xodia24-0.0.5/Xodia24.egg-info/
--rw-rw-rw-   0        0        0     5809 2024-04-01 15:09:10.000000 Xodia24-0.0.5/Xodia24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-01 15:09:11.000000 Xodia24-0.0.5/Xodia24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 15:09:10.000000 Xodia24-0.0.5/Xodia24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-01 15:09:10.000000 Xodia24-0.0.5/Xodia24.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 15:09:10.000000 Xodia24-0.0.5/Xodia24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 15:09:11.492148 Xodia24-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1200 2024-04-01 15:08:03.000000 Xodia24-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:37:56.023146 Xodia24-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5809 2024-04-19 05:37:56.019893 Xodia24-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5075 2024-04-01 15:09:02.000000 Xodia24-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 05:37:56.011221 Xodia24-0.0.6/Xodia24.egg-info/
+-rw-rw-rw-   0        0        0     5809 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 05:37:56.023146 Xodia24-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2024-04-19 05:37:50.000000 Xodia24-0.0.6/setup.py
```

### Comparing `Xodia24-0.0.5/LICENSE` & `Xodia24-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.5/PKG-INFO` & `Xodia24-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Xodia24-0.0.5/README.md` & `Xodia24-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.5/Xodia24.egg-info/PKG-INFO` & `Xodia24-0.0.6/Xodia24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Xodia24-0.0.5/setup.py` & `Xodia24-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Python package providing a custom environment for simulating tank battles'
 LONG_DESCRIPTION = 'Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid.'
 
 # Setting up
 setup(
     name="Xodia24",
     version=VERSION,
```

