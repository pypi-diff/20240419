# Comparing `tmp/Xodia24-0.0.6.tar.gz` & `tmp/Xodia24-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xodia24-0.0.6.tar", last modified: Fri Apr 19 05:37:56 2024, max compression
+gzip compressed data, was "Xodia24-0.0.7.tar", last modified: Fri Apr 19 05:54:21 2024, max compression
```

## Comparing `Xodia24-0.0.6.tar` & `Xodia24-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 05:37:56.023146 Xodia24-0.0.6/
--rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5809 2024-04-19 05:37:56.019893 Xodia24-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5075 2024-04-01 15:09:02.000000 Xodia24-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 05:37:56.011221 Xodia24-0.0.6/Xodia24.egg-info/
--rw-rw-rw-   0        0        0     5809 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 05:37:55.000000 Xodia24-0.0.6/Xodia24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 05:37:56.023146 Xodia24-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1200 2024-04-19 05:37:50.000000 Xodia24-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:54:21.529616 Xodia24-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5854 2024-04-19 05:54:21.521612 Xodia24-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5075 2024-04-01 15:09:02.000000 Xodia24-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 05:54:21.521612 Xodia24-0.0.7/Xodia24.egg-info/
+-rw-rw-rw-   0        0        0     5854 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-19 05:54:21.000000 Xodia24-0.0.7/Xodia24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 05:54:21.529616 Xodia24-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-04-19 05:50:18.000000 Xodia24-0.0.7/setup.py
```

### Comparing `Xodia24-0.0.6/LICENSE` & `Xodia24-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.6/PKG-INFO` & `Xodia24-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # Xodia24: PocketTank Environment
```

### Comparing `Xodia24-0.0.6/README.md` & `Xodia24-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.6/Xodia24.egg-info/PKG-INFO` & `Xodia24-0.0.7/Xodia24.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # Xodia24: PocketTank Environment
```

### Comparing `Xodia24-0.0.6/setup.py` & `Xodia24-0.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'Python package providing a custom environment for simulating tank battles'
 LONG_DESCRIPTION = 'Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid.'
 
 # Setting up
 setup(
     name="Xodia24",
     version=VERSION,
@@ -22,14 +22,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['gymnasium', 'numpy', 'matplotlib'],
     keywords=['python', 'reinforcement-learning', 'tank-battle'],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-        "License :: OSI Approved :: MIT License",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
     ]
 )
```

