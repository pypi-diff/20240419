# Comparing `tmp/langevin_sampling-1.1.tar.gz` & `tmp/langevin_sampling-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevin_sampling-1.1.tar", last modified: Fri Apr 19 21:15:16 2024, max compression
+gzip compressed data, was "langevin_sampling-1.2.tar", last modified: Fri Apr 19 21:24:42 2024, max compression
```

## Comparing `langevin_sampling-1.1.tar` & `langevin_sampling-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:15:16.333287 langevin_sampling-1.1/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1101 2024-04-19 02:21:02.000000 langevin_sampling-1.1/LICENSE
--rw-r--r--   0 ali       (1000) ali       (1000)     4084 2024-04-19 21:15:16.333287 langevin_sampling-1.1/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     3484 2024-04-19 21:14:54.000000 langevin_sampling-1.1/README.md
--rw-rw-r--   0 ali       (1000) ali       (1000)      104 2024-04-19 02:21:02.000000 langevin_sampling-1.1/pyproject.toml
--rw-rw-r--   0 ali       (1000) ali       (1000)      670 2024-04-19 21:15:16.333287 langevin_sampling-1.1/setup.cfg
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:15:16.329287 langevin_sampling-1.1/src/
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:15:16.333287 langevin_sampling-1.1/src/langevin_sampling/
--rw-rw-r--   0 ali       (1000) ali       (1000)     3178 2024-04-19 02:21:02.000000 langevin_sampling-1.1/src/langevin_sampling/SGLD.py
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 02:21:02.000000 langevin_sampling-1.1/src/langevin_sampling/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4037 2024-04-19 02:21:02.000000 langevin_sampling-1.1/src/langevin_sampling/precondSGLD.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     9605 2024-04-19 02:21:02.000000 langevin_sampling-1.1/src/langevin_sampling/samplers.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:15:16.333287 langevin_sampling-1.1/src/langevin_sampling.egg-info/
--rw-r--r--   0 ali       (1000) ali       (1000)     4084 2024-04-19 21:15:16.000000 langevin_sampling-1.1/src/langevin_sampling.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      401 2024-04-19 21:15:16.000000 langevin_sampling-1.1/src/langevin_sampling.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-04-19 21:15:16.000000 langevin_sampling-1.1/src/langevin_sampling.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       39 2024-04-19 21:15:16.000000 langevin_sampling-1.1/src/langevin_sampling.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-04-19 21:15:16.000000 langevin_sampling-1.1/src/langevin_sampling.egg-info/top_level.txt
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:24:42.971622 langevin_sampling-1.2/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1101 2024-04-19 02:21:02.000000 langevin_sampling-1.2/LICENSE
+-rw-r--r--   0 ali       (1000) ali       (1000)     4084 2024-04-19 21:24:42.971622 langevin_sampling-1.2/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3484 2024-04-19 21:14:54.000000 langevin_sampling-1.2/README.md
+-rw-rw-r--   0 ali       (1000) ali       (1000)      104 2024-04-19 02:21:02.000000 langevin_sampling-1.2/pyproject.toml
+-rw-rw-r--   0 ali       (1000) ali       (1000)      670 2024-04-19 21:24:42.971622 langevin_sampling-1.2/setup.cfg
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:24:42.967622 langevin_sampling-1.2/src/
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:24:42.971622 langevin_sampling-1.2/src/langevin_sampling/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3178 2024-04-19 02:21:02.000000 langevin_sampling-1.2/src/langevin_sampling/SGLD.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 02:21:02.000000 langevin_sampling-1.2/src/langevin_sampling/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4037 2024-04-19 02:21:02.000000 langevin_sampling-1.2/src/langevin_sampling/precondSGLD.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9605 2024-04-19 02:21:02.000000 langevin_sampling-1.2/src/langevin_sampling/samplers.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-19 21:24:42.971622 langevin_sampling-1.2/src/langevin_sampling.egg-info/
+-rw-r--r--   0 ali       (1000) ali       (1000)     4084 2024-04-19 21:24:42.000000 langevin_sampling-1.2/src/langevin_sampling.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      401 2024-04-19 21:24:42.000000 langevin_sampling-1.2/src/langevin_sampling.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-04-19 21:24:42.000000 langevin_sampling-1.2/src/langevin_sampling.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       39 2024-04-19 21:24:42.000000 langevin_sampling-1.2/src/langevin_sampling.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-04-19 21:24:42.000000 langevin_sampling-1.2/src/langevin_sampling.egg-info/top_level.txt
```

### Comparing `langevin_sampling-1.1/LICENSE` & `langevin_sampling-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langevin_sampling-1.1/PKG-INFO` & `langevin_sampling-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langevin_sampling
-Version: 1.1
+Version: 1.2
 Summary: Sampling with gradient-based Markov Chain Monte Carlo approaches
 Home-page: https://github.com/alisiahkoohi/Langevin-dynamics
 Author: Ali Siahkoohi
 Author-email: ali.siahkoohi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langevin_sampling-1.1/README.md` & `langevin_sampling-1.2/README.md`

 * *Files identical despite different names*

### Comparing `langevin_sampling-1.1/setup.cfg` & `langevin_sampling-1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = langevin_sampling
-version = 1.1
+version = 1.2
 author = Ali Siahkoohi
 author_email = ali.siahkoohi@gmail.com
 description = Sampling with gradient-based Markov Chain Monte Carlo approaches
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alisiahkoohi/Langevin-dynamics
 classifiers =
```

### Comparing `langevin_sampling-1.1/src/langevin_sampling/SGLD.py` & `langevin_sampling-1.2/src/langevin_sampling/SGLD.py`

 * *Files identical despite different names*

### Comparing `langevin_sampling-1.1/src/langevin_sampling/precondSGLD.py` & `langevin_sampling-1.2/src/langevin_sampling/precondSGLD.py`

 * *Files identical despite different names*

### Comparing `langevin_sampling-1.1/src/langevin_sampling/samplers.py` & `langevin_sampling-1.2/src/langevin_sampling/samplers.py`

 * *Files identical despite different names*

### Comparing `langevin_sampling-1.1/src/langevin_sampling.egg-info/PKG-INFO` & `langevin_sampling-1.2/src/langevin_sampling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langevin_sampling
-Version: 1.1
+Version: 1.2
 Summary: Sampling with gradient-based Markov Chain Monte Carlo approaches
 Home-page: https://github.com/alisiahkoohi/Langevin-dynamics
 Author: Ali Siahkoohi
 Author-email: ali.siahkoohi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

