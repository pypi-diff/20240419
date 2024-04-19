# Comparing `tmp/numpy_neuron-0.1.tar.gz` & `tmp/numpy_neuron-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy_neuron-0.1.tar", last modified: Fri Apr 19 20:23:16 2024, max compression
+gzip compressed data, was "numpy_neuron-0.2.tar", last modified: Fri Apr 19 20:34:45 2024, max compression
```

## Comparing `numpy_neuron-0.1.tar` & `numpy_neuron-0.2.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:23:16.186176 numpy_neuron-0.1/
--rw-r--r--   0 jensen     (501) staff       (20)     1771 2024-04-19 20:23:16.185999 numpy_neuron-0.1/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      368 2024-04-19 17:22:41.000000 numpy_neuron-0.1/README.md
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:23:16.183806 numpy_neuron-0.1/nn/
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:23:16.185829 numpy_neuron-0.1/nn/numpy_neuron.egg-info/
--rw-r--r--   0 jensen     (501) staff       (20)     1771 2024-04-19 20:23:16.000000 numpy_neuron-0.1/nn/numpy_neuron.egg-info/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      242 2024-04-19 20:23:16.000000 numpy_neuron-0.1/nn/numpy_neuron.egg-info/SOURCES.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 20:23:16.000000 numpy_neuron-0.1/nn/numpy_neuron.egg-info/dependency_links.txt
--rw-r--r--   0 jensen     (501) staff       (20)        4 2024-04-19 20:23:16.000000 numpy_neuron-0.1/nn/numpy_neuron.egg-info/top_level.txt
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:23:16.185528 numpy_neuron-0.1/nn/src/
--rw-r--r--   0 jensen     (501) staff       (20)       70 2024-04-18 15:06:29.000000 numpy_neuron-0.1/nn/src/__init__.py
--rw-r--r--   0 jensen     (501) staff       (20)     1339 2024-04-18 15:06:29.000000 numpy_neuron-0.1/nn/src/activation.py
--rw-r--r--   0 jensen     (501) staff       (20)     2485 2024-04-18 15:06:29.000000 numpy_neuron-0.1/nn/src/loss.py
--rw-r--r--   0 jensen     (501) staff       (20)     6455 2024-04-19 17:16:49.000000 numpy_neuron-0.1/nn/src/nn.py
--rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 20:23:16.186217 numpy_neuron-0.1/setup.cfg
--rw-r--r--   0 jensen     (501) staff       (20)      769 2024-04-19 20:12:12.000000 numpy_neuron-0.1/setup.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:34:45.921082 numpy_neuron-0.2/
+-rw-r--r--   0 jensen     (501) staff       (20)     1098 2024-04-19 20:34:45.920895 numpy_neuron-0.2/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)      575 2024-04-19 20:29:13.000000 numpy_neuron-0.2/README.md
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:34:45.919935 numpy_neuron-0.2/nn/
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:34:45.920727 numpy_neuron-0.2/nn/numpy_neuron.egg-info/
+-rw-r--r--   0 jensen     (501) staff       (20)     1098 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)      174 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/SOURCES.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/dependency_links.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/top_level.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 20:34:45.921122 numpy_neuron-0.2/setup.cfg
+-rw-r--r--   0 jensen     (501) staff       (20)      768 2024-04-19 20:33:39.000000 numpy_neuron-0.2/setup.py
```

### Comparing `numpy_neuron-0.1/setup.py` & `numpy_neuron-0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="numpy_neuron",
-    version="0.1",
+    version="0.2",
     author="Jensen Holm",
     author_email="jensen.dev.01@gmail.com",
     description="Simple, lightweight neural network framework built in numpy",
-    long_description=open('warning.md').read(),
+    long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Jensen-holm/Numpy-Neuron",
     project_urls={
         "Bug Tracker": "https://github.com/Jensen-holm/Numpy-Neuron/issues"
     },
     package_dir={"": "nn"},
     packages=find_packages(where="nn"),
```

