# Comparing `tmp/numpy_neuron-0.3.tar.gz` & `tmp/numpy_neuron-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy_neuron-0.3.tar", last modified: Fri Apr 19 21:04:39 2024, max compression
+gzip compressed data, was "numpy_neuron-1.0.tar", last modified: Fri Apr 19 21:17:03 2024, max compression
```

## Comparing `numpy_neuron-0.3.tar` & `numpy_neuron-1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:04:39.612991 numpy_neuron-0.3/
--rw-r--r--   0 jensen     (501) staff       (20)     2547 2024-04-19 21:04:39.612731 numpy_neuron-0.3/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)     2425 2024-04-19 21:03:47.000000 numpy_neuron-0.3/README.md
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:04:39.611747 numpy_neuron-0.3/nn/
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:04:39.612563 numpy_neuron-0.3/nn/numpy_neuron.egg-info/
--rw-r--r--   0 jensen     (501) staff       (20)     2547 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      174 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/SOURCES.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/dependency_links.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:04:39.000000 numpy_neuron-0.3/nn/numpy_neuron.egg-info/top_level.txt
--rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 21:04:39.613035 numpy_neuron-0.3/setup.cfg
--rw-r--r--   0 jensen     (501) staff       (20)      760 2024-04-19 21:02:14.000000 numpy_neuron-0.3/setup.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:17:03.569781 numpy_neuron-1.0/
+-rw-r--r--   0 jensen     (501) staff       (20)     2606 2024-04-19 21:17:03.569591 numpy_neuron-1.0/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)     2469 2024-04-19 21:12:37.000000 numpy_neuron-1.0/README.md
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:17:03.568544 numpy_neuron-1.0/nn/
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:17:03.569439 numpy_neuron-1.0/nn/numpy_neuron.egg-info/
+-rw-r--r--   0 jensen     (501) staff       (20)     2606 2024-04-19 21:17:03.000000 numpy_neuron-1.0/nn/numpy_neuron.egg-info/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)      174 2024-04-19 21:17:03.000000 numpy_neuron-1.0/nn/numpy_neuron.egg-info/SOURCES.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:17:03.000000 numpy_neuron-1.0/nn/numpy_neuron.egg-info/dependency_links.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:17:03.000000 numpy_neuron-1.0/nn/numpy_neuron.egg-info/top_level.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 21:17:03.569815 numpy_neuron-1.0/setup.cfg
+-rw-r--r--   0 jensen     (501) staff       (20)      760 2024-04-19 21:16:40.000000 numpy_neuron-1.0/setup.py
```

### Comparing `numpy_neuron-0.3/PKG-INFO` & `numpy_neuron-1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: numpy_neuron
-Version: 0.3
+Version: 1.0
 Summary: Simple, lightweight neural network framework built in numpy
 Home-page: https://github.com/Jensen-holm/Numpy-Neuron
 Author: Jensen Holm
 Author-email: jensen.dev.01@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Numpy-Neuron
 
 A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh).
-Here is an example of how to use the package for training a classifier.
+
+## Install
+
+`pip install numpy_neuron`
+
+
+## Example
 
 ```py
 from sklearn import datasets
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import accuracy_score, precision_score, recall_score
 import numpy as np
@@ -81,15 +87,15 @@
     print(f"accuracy on validation set: {accuracy:.4f}")
 
 
 if __name__ == "__main__":
     train_nn_classifier()
 ```
 
-
 ## Roadmap
 
 **Optimizers**
-I would love to add the ability to modify the learning rate over each epoch to ensure
-that the gradient descent algorithm does not get stuck in local minima as easily.
 
+Currently the learning rate in a NN object is static during training. I would like 
+to work on developing at least the functionality for the Adam optimizer at some point.
+This would help prevent getting stuck in local minima of the loss function.
```

### Comparing `numpy_neuron-0.3/README.md` & `numpy_neuron-1.0/nn/numpy_neuron.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,31 @@
----
-title: Numpy-Neuron
-emoji: 🔙
-colorFrom: yellow
-colorTo: blue
-sdk: gradio
-sdk_version: 4.26.0
-app_file: gradio_app.py
-pinned: false
-license: mit
----
-
+Metadata-Version: 2.1
+Name: numpy_neuron
+Version: 1.0
+Summary: Simple, lightweight neural network framework built in numpy
+Home-page: https://github.com/Jensen-holm/Numpy-Neuron
+Author: Jensen Holm
+Author-email: jensen.dev.01@gmail.com
+Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 
 # Numpy-Neuron
 
 A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh).
-Here is an example of how to use the package for training a classifier.
+
+## Install
+
+`pip install numpy_neuron`
+
+
+## Example
 
 ```py
 from sklearn import datasets
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import accuracy_score, precision_score, recall_score
 import numpy as np
@@ -80,22 +87,15 @@
     print(f"accuracy on validation set: {accuracy:.4f}")
 
 
 if __name__ == "__main__":
     train_nn_classifier()
 ```
 
-
 ## Roadmap
 
 **Optimizers**
-I would love to add the ability to modify the learning rate over each epoch to ensure
-that the gradient descent algorithm does not get stuck in local minima as easily.
-
-
-## Gradio app demo development notes
 
-The remote added to this repo so that it runs on hugging face spaces
-`git remote add space git@hf.co:spaces/Jensen-holm/Numpy-Neuron` 
+Currently the learning rate in a NN object is static during training. I would like 
+to work on developing at least the functionality for the Adam optimizer at some point.
+This would help prevent getting stuck in local minima of the loss function.
 
-The command to force push to that space
-`git push --force space main`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `numpy_neuron-0.3/setup.py` & `numpy_neuron-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="numpy_neuron",
-    version="0.3",
+    version="1.0",
     author="Jensen Holm",
     author_email="jensen.dev.01@gmail.com",
     description="Simple, lightweight neural network framework built in numpy",
     long_description=open("about_package.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Jensen-holm/Numpy-Neuron",
     project_urls={"Bug Tracker": "https://github.com/Jensen-holm/Numpy-Neuron/issues"},
```

