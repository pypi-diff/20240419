# Comparing `tmp/npnn-0.0.1.tar.gz` & `tmp/npnn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npnn-0.0.1.tar", last modified: Wed Apr 17 15:19:45 2024, max compression
+gzip compressed data, was "npnn-0.0.2.tar", last modified: Fri Apr 19 10:21:39 2024, max compression
```

## Comparing `npnn-0.0.1.tar` & `npnn-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:19:45.299518 npnn-0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-04-17 13:52:58.000000 npnn-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2941 2024-04-17 15:19:45.299518 npnn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      782 2024-04-17 15:16:30.000000 npnn-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1012 2024-04-17 15:13:22.000000 npnn-0.0.1/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-17 15:19:45.299518 npnn-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 15:19:45.252642 npnn-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 15:19:45.268267 npnn-0.0.1/src/npnn/
--rw-rw-rw-   0        0        0      128 2024-04-17 15:10:44.000000 npnn-0.0.1/src/npnn/__init__.py
--rw-rw-rw-   0        0        0     4546 2024-04-17 14:53:17.000000 npnn-0.0.1/src/npnn/autograd.py
--rw-rw-rw-   0        0        0     1361 2024-04-17 11:15:59.000000 npnn-0.0.1/src/npnn/base.py
--rw-rw-rw-   0        0        0     7789 2024-04-17 06:42:46.000000 npnn-0.0.1/src/npnn/functional.py
--rw-rw-rw-   0        0        0     1232 2024-04-17 06:43:02.000000 npnn-0.0.1/src/npnn/nn.py
--rw-rw-rw-   0        0        0     4409 2024-04-17 10:55:12.000000 npnn-0.0.1/src/npnn/optim.py
--rw-rw-rw-   0        0        0     8580 2024-04-17 15:13:03.000000 npnn-0.0.1/src/npnn/test_autograd.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:19:45.283892 npnn-0.0.1/src/npnn.egg-info/
--rw-rw-rw-   0        0        0     2941 2024-04-17 15:19:45.000000 npnn-0.0.1/src/npnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-17 15:19:45.000000 npnn-0.0.1/src/npnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:19:45.000000 npnn-0.0.1/src/npnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-17 15:19:45.000000 npnn-0.0.1/src/npnn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 15:19:45.000000 npnn-0.0.1/src/npnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.187020 npnn-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-04-17 13:52:58.000000 npnn-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4055 2024-04-19 10:21:39.187020 npnn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2024-04-19 10:17:57.000000 npnn-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     2038 2024-04-19 10:21:15.000000 npnn-0.0.2/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:21:39.187020 npnn-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.155770 npnn-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.171396 npnn-0.0.2/src/npnn/
+-rw-rw-rw-   0        0        0      128 2024-04-17 15:10:44.000000 npnn-0.0.2/src/npnn/__init__.py
+-rw-rw-rw-   0        0        0     4546 2024-04-17 14:53:17.000000 npnn-0.0.2/src/npnn/autograd.py
+-rw-rw-rw-   0        0        0     1361 2024-04-17 11:15:59.000000 npnn-0.0.2/src/npnn/base.py
+-rw-rw-rw-   0        0        0     7789 2024-04-17 06:42:46.000000 npnn-0.0.2/src/npnn/functional.py
+-rw-rw-rw-   0        0        0     1232 2024-04-17 06:43:02.000000 npnn-0.0.2/src/npnn/nn.py
+-rw-rw-rw-   0        0        0     6111 2024-04-19 10:17:48.000000 npnn-0.0.2/src/npnn/optim.py
+-rw-rw-rw-   0        0        0     8580 2024-04-17 15:13:03.000000 npnn-0.0.2/src/npnn/test_autograd.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.187020 npnn-0.0.2/src/npnn.egg-info/
+-rw-rw-rw-   0        0        0     4055 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/top_level.txt
```

### Comparing `npnn-0.0.1/LICENSE` & `npnn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `npnn-0.0.1/PKG-INFO` & `npnn-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npnn
-Version: 0.0.1
+Version: 0.0.2
 Summary: NumPy Neural Network
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,26 +32,54 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Provides-Extra: cuda
-Requires-Dist: cupy; extra == "cuda"
+Provides-Extra: cuda11x
+Requires-Dist: cupy-cuda11x; extra == "cuda11x"
+Provides-Extra: cuda12x
+Requires-Dist: cupy-cuda12x; extra == "cuda12x"
 
-# NPNN
+# [npnn](https://pypi.org/project/npnn/0.0.1/)
 > NumPy Neural Network
 
-## What's `npnn`?
-> `npnn` is a a torch-like Python module for **gradient descent based machine learning** implemented with NumPy. 
+[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/0.0.1/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
 
 
-## Work with `npnn`!
-> construct a image classification neural network with npnn
+## What's npnn?
+> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
+
+### Dependency
+Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
+
+If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
+
+For example, my PC have CUDA v12.x (x86_64), so I use command:
+```bash
+pip install cupy-cuda12x
+pip install npnn
+```
+or in short:
+```bash
+pip install npnn[cuda12x]
+```
+check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
+
+
+### API references
+
+See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
+
+## Work with npnn!
+> Here we will construct a image classification neural network with npnn.
 
 BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
 
 ### Task
 Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
 
 - Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
```

### Comparing `npnn-0.0.1/pyproject.toml` & `npnn-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "npnn"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
   "numpy"
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Yang Zhang", email="mail@yangzhang.site" },
 ]
@@ -21,11 +21,12 @@
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
-cuda = ["cupy"]
+cuda11x = ["cupy-cuda11x"]
+cuda12x = ["cupy-cuda12x"]
 
 [project.urls]
 Homepage = "https://github.com/AIboy996/npnn"
```

### Comparing `npnn-0.0.1/src/npnn/autograd.py` & `npnn-0.0.2/src/npnn/autograd.py`

 * *Files identical despite different names*

### Comparing `npnn-0.0.1/src/npnn/base.py` & `npnn-0.0.2/src/npnn/base.py`

 * *Files identical despite different names*

### Comparing `npnn-0.0.1/src/npnn/functional.py` & `npnn-0.0.2/src/npnn/functional.py`

 * *Files identical despite different names*

### Comparing `npnn-0.0.1/src/npnn/nn.py` & `npnn-0.0.2/src/npnn/nn.py`

 * *Files identical despite different names*

### Comparing `npnn-0.0.1/src/npnn/optim.py` & `npnn-0.0.2/src/npnn/optim.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Provide gradietn descent optimizer"""
 
+from typing import Literal
+
 from .base import Optimizer, np
 from .autograd import Tensor
 
 
 class SGD(Optimizer):
     """
     Stochastic Gradient Descent optimizer.
@@ -14,28 +16,43 @@
         self,
         params: list[Tensor],
         lr: float = 0.001,
         momentum: float = 0,
         dampening: float = 0,
         weight_decay: float = 0,
         nesterov: bool = False,
+        regularization: Literal[None, "l1", "l2"] = None,
+        regular_strength: float = 1,
     ) -> None:
         super().__init__()
         self.params = params
         self.lr = lr
         self.momentum = momentum
         self.dampening = dampening
         self.weight_decay = weight_decay
         self.nesterov = nesterov
+        self.regularization = regularization
+        self.regular_strength = regular_strength
         self.step_now = 0
 
     def step(self):
         for param in self.params:
             x = param.data
-            g = param.grad / param.back_counter
+            if self.regularization is None:
+                g = param.grad / param.back_counter
+            elif self.regularization == "l2":
+                g = (
+                    param.grad + self.regular_strength * 2 * param.data
+                ) / param.back_counter
+            elif self.regularization == "l1":
+                g = (
+                    param.grad + self.regular_strength * np.sign(param.data)
+                ) / param.back_counter
+            else:
+                raise ValueError("Invalid regularization method.")
             if self.weight_decay != 0:
                 g = g + self.weight_decay * x
             if self.momentum != 0:
                 # param.b is the momentum cache
                 if self.step_now > 0:
                     param.b = self.momentum * param.b + (1 - self.dampening) * g
                 else:
@@ -61,28 +78,43 @@
     def __init__(
         self,
         params: list[Tensor],
         lr: float = 0.001,
         betas: list[float] = [0.9, 0.999],
         eps: float = 1e-8,
         weight_decay: float = 0,
+        regularization: Literal[None, "l1", "l2"] = None,
+        regular_strength: float = 0,
     ) -> None:
         super().__init__()
         self.params = params
         self.lr = lr
         self.betas = betas
         self.eps = eps
         self.weight_decay = weight_decay
+        self.regularization = regularization
+        self.regular_strength = regular_strength
         self.step_now = 0
 
     def step(self):
         for param in self.params:
             beta1, beta2 = self.betas
             x = param.data
-            g = param.grad / param.back_counter
+            if self.regularization is None:
+                g = param.grad / param.back_counter
+            elif self.regularization == "l2":
+                g = (
+                    param.grad + self.regular_strength * 2 * param.data
+                ) / param.back_counter
+            elif self.regularization == "l1":
+                g = (
+                    param.grad + self.regular_strength * np.sign(param.data)
+                ) / param.back_counter
+            else:
+                raise ValueError("Invalid regularization method.")
             if self.weight_decay != 0:
                 g = g + self.weight_decay * x
             if self.step_now > 0:
                 # Update biased first moment estimate)
                 param.m = beta1 * param.m + (1 - beta1) * g
                 # Update biased second raw moment estimate
                 param.v = beta2 * param.v + (1 - beta2) * g**2
@@ -108,29 +140,42 @@
     from .functional import Inner, Norm, Add
 
     np.random.seed(0)
     inner = Inner()
     add = Add()
     norm = Norm()
     rand = np.random.random
-    SIZE = 10
+    SIZE = 3
     X = Tensor(rand((SIZE, SIZE)) * 2)
     beta = Tensor(rand(SIZE), requires_grad=True)
     y = Tensor(4 * (rand(SIZE) - 0.5))
     if sgd:
         optimizer = SGD(
-            params=[beta], momentum=0.1, dampening=0.5, lr=0.001, weight_decay=0.01
+            params=[beta],
+            momentum=0.1,
+            dampening=0.5,
+            lr=0.001,
+            weight_decay=0.01,
+            regularization="l2",
+            regular_strength=0.1,
         )
     else:
-        optimizer = Adam(params=[beta], lr=0.01, weight_decay=0.01)
+        optimizer = Adam(
+            params=[beta],
+            lr=0.01,
+            weight_decay=0.01,
+            regularization="l2",
+            regular_strength=0,
+        )
     for _ in range(iterations):
         loss = norm(add(inner(X, beta), -y))
         loss.backward()
         optimizer.step()
         optimizer.zero_grad()
+    print("using", np.__name__)
     if np.__name__ == "cupy":
         res = scipy.optimize.lsq_linear(X.data.get(), y.data.get())
     elif np.__name__ == "numpy":
         res = scipy.optimize.lsq_linear(X.data, y.data)
     print(res.x, res.cost, res.status)
     print(beta.data, loss.data[0])
```

### Comparing `npnn-0.0.1/src/npnn/test_autograd.py` & `npnn-0.0.2/src/npnn/test_autograd.py`

 * *Files identical despite different names*

### Comparing `npnn-0.0.1/src/npnn.egg-info/PKG-INFO` & `npnn-0.0.2/src/npnn.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npnn
-Version: 0.0.1
+Version: 0.0.2
 Summary: NumPy Neural Network
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,26 +32,54 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Provides-Extra: cuda
-Requires-Dist: cupy; extra == "cuda"
+Provides-Extra: cuda11x
+Requires-Dist: cupy-cuda11x; extra == "cuda11x"
+Provides-Extra: cuda12x
+Requires-Dist: cupy-cuda12x; extra == "cuda12x"
 
-# NPNN
+# [npnn](https://pypi.org/project/npnn/0.0.1/)
 > NumPy Neural Network
 
-## What's `npnn`?
-> `npnn` is a a torch-like Python module for **gradient descent based machine learning** implemented with NumPy. 
+[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/0.0.1/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
 
 
-## Work with `npnn`!
-> construct a image classification neural network with npnn
+## What's npnn?
+> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
+
+### Dependency
+Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
+
+If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
+
+For example, my PC have CUDA v12.x (x86_64), so I use command:
+```bash
+pip install cupy-cuda12x
+pip install npnn
+```
+or in short:
+```bash
+pip install npnn[cuda12x]
+```
+check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
+
+
+### API references
+
+See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
+
+## Work with npnn!
+> Here we will construct a image classification neural network with npnn.
 
 BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
 
 ### Task
 Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
 
 - Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
```

