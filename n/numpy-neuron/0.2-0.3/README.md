# Comparing `tmp/numpy_neuron-0.2.tar.gz` & `tmp/numpy_neuron-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy_neuron-0.2.tar", last modified: Fri Apr 19 20:34:45 2024, max compression
+gzip compressed data, was "numpy_neuron-0.3.tar", last modified: Fri Apr 19 21:04:39 2024, max compression
```

## Comparing `numpy_neuron-0.2.tar` & `numpy_neuron-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:34:45.921082 numpy_neuron-0.2/
--rw-r--r--   0 jensen     (501) staff       (20)     1098 2024-04-19 20:34:45.920895 numpy_neuron-0.2/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      575 2024-04-19 20:29:13.000000 numpy_neuron-0.2/README.md
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:34:45.919935 numpy_neuron-0.2/nn/
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 20:34:45.920727 numpy_neuron-0.2/nn/numpy_neuron.egg-info/
--rw-r--r--   0 jensen     (501) staff       (20)     1098 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      174 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/SOURCES.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/dependency_links.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 20:34:45.000000 numpy_neuron-0.2/nn/numpy_neuron.egg-info/top_level.txt
--rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 20:34:45.921122 numpy_neuron-0.2/setup.cfg
--rw-r--r--   0 jensen     (501) staff       (20)      768 2024-04-19 20:33:39.000000 numpy_neuron-0.2/setup.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:04:39.612991 numpy_neuron-0.3/
+-rw-r--r--   0 jensen     (501) staff       (20)     2547 2024-04-19 21:04:39.612731 numpy_neuron-0.3/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)     2425 2024-04-19 21:03:47.000000 numpy_neuron-0.3/README.md
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:04:39.611747 numpy_neuron-0.3/nn/
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:04:39.612563 numpy_neuron-0.3/nn/numpy_neuron.egg-info/
+-rw-r--r--   0 jensen     (501) staff       (20)     2547 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)      174 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/SOURCES.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/dependency_links.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/top_level.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 21:04:39.613035 numpy_neuron-0.3/setup.cfg
+-rw-r--r--   0 jensen     (501) staff       (20)      760 2024-04-19 21:02:14.000000 numpy_neuron-0.3/setup.py
```

### Comparing `numpy_neuron-0.2/setup.py` & `numpy_neuron-0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="numpy_neuron",
-    version="0.2",
+    version="0.3",
     author="Jensen Holm",
     author_email="jensen.dev.01@gmail.com",
     description="Simple, lightweight neural network framework built in numpy",
-    long_description=open('README.md').read(),
+    long_description=open("about_package.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Jensen-holm/Numpy-Neuron",
-    project_urls={
-        "Bug Tracker": "https://github.com/Jensen-holm/Numpy-Neuron/issues"
-    },
+    project_urls={"Bug Tracker": "https://github.com/Jensen-holm/Numpy-Neuron/issues"},
     package_dir={"": "nn"},
     packages=find_packages(where="nn"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
-
```

