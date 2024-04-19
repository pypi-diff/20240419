# Comparing `tmp/torchsurv-0.1.1.tar.gz` & `tmp/torchsurv-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsurv-0.1.1.tar", last modified: Mon Apr 15 19:59:42 2024, max compression
+gzip compressed data, was "torchsurv-0.1.2.tar", last modified: Fri Apr 19 07:41:35 2024, max compression
```

## Comparing `torchsurv-0.1.1.tar` & `torchsurv-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.904712 torchsurv-0.1.1/
--rw-r--r--   0 kruscpe1   (501) staff       (20)     1103 2024-04-12 12:52:01.000000 torchsurv-0.1.1/LICENSE.txt
--rw-r--r--   0 kruscpe1   (501) staff       (20)    11631 2024-04-15 19:59:42.904180 torchsurv-0.1.1/PKG-INFO
--rw-r--r--   0 kruscpe1   (501) staff       (20)     9117 2024-04-15 15:50:10.000000 torchsurv-0.1.1/README.md
--rw-r--r--   0 kruscpe1   (501) staff       (20)     1577 2024-04-15 19:52:54.000000 torchsurv-0.1.1/pyproject.toml
--rw-r--r--   0 kruscpe1   (501) staff       (20)       38 2024-04-15 19:59:42.904770 torchsurv-0.1.1/setup.cfg
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.886891 torchsurv-0.1.1/src/
--rw-r--r--   0 kruscpe1   (501) staff       (20)        0 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/__init__.py
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.887608 torchsurv-0.1.1/src/torchsurv/
--rw-r--r--   0 kruscpe1   (501) staff       (20)      156 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/torchsurv/__init__.py
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.892809 torchsurv-0.1.1/src/torchsurv/loss/
--rw-r--r--   0 kruscpe1   (501) staff       (20)       74 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/torchsurv/loss/__init__.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)    10116 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/torchsurv/loss/cox.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     9292 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/torchsurv/loss/momentum.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)    15149 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/torchsurv/loss/weibull.py
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.895132 torchsurv-0.1.1/src/torchsurv/metrics/
--rw-r--r--   0 kruscpe1   (501) staff       (20)       50 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/torchsurv/metrics/__init__.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)    53258 2024-04-15 14:53:50.000000 torchsurv-0.1.1/src/torchsurv/metrics/auc.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)    38002 2024-04-15 14:53:50.000000 torchsurv-0.1.1/src/torchsurv/metrics/brier_score.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)    37223 2024-04-15 14:53:50.000000 torchsurv-0.1.1/src/torchsurv/metrics/cindex.py
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.896794 torchsurv-0.1.1/src/torchsurv/stats/
--rw-r--r--   0 kruscpe1   (501) staff       (20)        0 2024-04-15 14:53:50.000000 torchsurv-0.1.1/src/torchsurv/stats/__init__.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     3458 2024-04-15 14:53:50.000000 torchsurv-0.1.1/src/torchsurv/stats/ipcw.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     9715 2024-04-15 14:53:50.000000 torchsurv-0.1.1/src/torchsurv/stats/kaplan_meier.py
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.897498 torchsurv-0.1.1/src/torchsurv/tools/
--rw-r--r--   0 kruscpe1   (501) staff       (20)     4747 2024-04-12 12:52:01.000000 torchsurv-0.1.1/src/torchsurv/tools/validate_inputs.py
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.903613 torchsurv-0.1.1/src/torchsurv.egg-info/
--rw-r--r--   0 kruscpe1   (501) staff       (20)    11631 2024-04-15 19:59:42.000000 torchsurv-0.1.1/src/torchsurv.egg-info/PKG-INFO
--rw-r--r--   0 kruscpe1   (501) staff       (20)      861 2024-04-15 19:59:42.000000 torchsurv-0.1.1/src/torchsurv.egg-info/SOURCES.txt
--rw-r--r--   0 kruscpe1   (501) staff       (20)        1 2024-04-15 19:59:42.000000 torchsurv-0.1.1/src/torchsurv.egg-info/dependency_links.txt
--rw-r--r--   0 kruscpe1   (501) staff       (20)       41 2024-04-15 19:59:42.000000 torchsurv-0.1.1/src/torchsurv.egg-info/requires.txt
--rw-r--r--   0 kruscpe1   (501) staff       (20)       19 2024-04-15 19:59:42.000000 torchsurv-0.1.1/src/torchsurv.egg-info/top_level.txt
-drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-15 19:59:42.902776 torchsurv-0.1.1/tests/
--rw-r--r--   0 kruscpe1   (501) staff       (20)    12674 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_auc.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)    10876 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_brier_score.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)    10492 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_cindex.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     4941 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_cox.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     3526 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_ipcw.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     7884 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_kaplan_meier.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     4928 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_mnist.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     1452 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_momentum.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     2652 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_train.py
--rw-r--r--   0 kruscpe1   (501) staff       (20)     9462 2024-04-12 12:52:01.000000 torchsurv-0.1.1/tests/test_weibull.py
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.841036 torchsurv-0.1.2/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     1103 2024-04-12 12:52:01.000000 torchsurv-0.1.2/LICENSE.txt
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    13667 2024-04-19 07:41:35.840498 torchsurv-0.1.2/PKG-INFO
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    11178 2024-04-19 07:40:50.000000 torchsurv-0.1.2/README.md
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     1562 2024-04-19 07:40:50.000000 torchsurv-0.1.2/pyproject.toml
+-rw-r--r--   0 kruscpe1   (501) staff       (20)       38 2024-04-19 07:41:35.841091 torchsurv-0.1.2/setup.cfg
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.820265 torchsurv-0.1.2/src/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)        0 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/__init__.py
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.820708 torchsurv-0.1.2/src/torchsurv/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)      156 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/torchsurv/__init__.py
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.825448 torchsurv-0.1.2/src/torchsurv/loss/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)       74 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/torchsurv/loss/__init__.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    10116 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/torchsurv/loss/cox.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     9292 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/torchsurv/loss/momentum.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    15149 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/torchsurv/loss/weibull.py
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.828746 torchsurv-0.1.2/src/torchsurv/metrics/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)       50 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/torchsurv/metrics/__init__.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    53258 2024-04-15 14:53:50.000000 torchsurv-0.1.2/src/torchsurv/metrics/auc.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    38002 2024-04-15 14:53:50.000000 torchsurv-0.1.2/src/torchsurv/metrics/brier_score.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    37223 2024-04-15 14:53:50.000000 torchsurv-0.1.2/src/torchsurv/metrics/cindex.py
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.831132 torchsurv-0.1.2/src/torchsurv/stats/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)        0 2024-04-15 14:53:50.000000 torchsurv-0.1.2/src/torchsurv/stats/__init__.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     3458 2024-04-15 14:53:50.000000 torchsurv-0.1.2/src/torchsurv/stats/ipcw.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     9715 2024-04-15 14:53:50.000000 torchsurv-0.1.2/src/torchsurv/stats/kaplan_meier.py
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.832170 torchsurv-0.1.2/src/torchsurv/tools/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     4747 2024-04-12 12:52:01.000000 torchsurv-0.1.2/src/torchsurv/tools/validate_inputs.py
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.839799 torchsurv-0.1.2/src/torchsurv.egg-info/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    13667 2024-04-19 07:41:35.000000 torchsurv-0.1.2/src/torchsurv.egg-info/PKG-INFO
+-rw-r--r--   0 kruscpe1   (501) staff       (20)      861 2024-04-19 07:41:35.000000 torchsurv-0.1.2/src/torchsurv.egg-info/SOURCES.txt
+-rw-r--r--   0 kruscpe1   (501) staff       (20)        1 2024-04-19 07:41:35.000000 torchsurv-0.1.2/src/torchsurv.egg-info/dependency_links.txt
+-rw-r--r--   0 kruscpe1   (501) staff       (20)       31 2024-04-19 07:41:35.000000 torchsurv-0.1.2/src/torchsurv.egg-info/requires.txt
+-rw-r--r--   0 kruscpe1   (501) staff       (20)       19 2024-04-19 07:41:35.000000 torchsurv-0.1.2/src/torchsurv.egg-info/top_level.txt
+drwxr-xr-x   0 kruscpe1   (501) staff       (20)        0 2024-04-19 07:41:35.838158 torchsurv-0.1.2/tests/
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    12674 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_auc.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    10876 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_brier_score.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)    10492 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_cindex.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     4941 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_cox.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     3526 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_ipcw.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     7884 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_kaplan_meier.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     4928 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_mnist.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     1452 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_momentum.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     2652 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_train.py
+-rw-r--r--   0 kruscpe1   (501) staff       (20)     9462 2024-04-12 12:52:01.000000 torchsurv-0.1.2/tests/test_weibull.py
```

### Comparing `torchsurv-0.1.1/LICENSE.txt` & `torchsurv-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/PKG-INFO` & `torchsurv-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,15 @@
-Metadata-Version: 2.1
-Name: torchsurv
-Version: 0.1.1
-Summary: Survival analysis made easy with pytorch
-Author-email: Thibaud Coroller <thibaud.coroller@novartis.com>, Melodie Monod <melodie.monod@novartis.com>, Peter Krusche <peter.krusche@novartis.com>, Qian Cao <qian.cao@fda.hhs.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2023 Novartis Pharmaceuticals Corporation
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/Novartis/torchsurv
-Project-URL: Repository, https://github.com/Novartis/torchsurv
-Project-URL: Documentation, https://opensource.nibr.com/torchsurv/
-Project-URL: IssueTracker, https://github.com/Novartis/torchsurv/issues
-Project-URL: Changelog, https://opensource.nibr.com/torchsurv/CHANGELOG.html
-Keywords: example,project,tutorial
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: torch
-Requires-Dist: lightning
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: torchmetrics
-
-# Survival analysis made easy
-
-> :warning: :construction: **We are still working on the publication of this project and appreciate your patience until everything will be ready.** :construction: :warning:
+# Deep survival analysis made easy
 
 ![CodeQC](https://github.com/Novartis/torchsurv/actions/workflows/codeqc.yml/badge.svg?branch=main)
 ![Docs](https://github.com/Novartis/torchsurv/actions/workflows/docs.yml/badge.svg?branch=main)
+[![PyPI - Version](https://img.shields.io/pypi/v/torchsurv)](https://pypi.org/project/torchsurv/)
+[![arXiv](https://img.shields.io/badge/arXiv-2404.10761-f9f107.svg)](https://arxiv.org/abs/2404.10761)
+[![Documentation](https://img.shields.io/badge/GithubPage-Sphinx-blue)](https://opensource.nibr.com/torchsurv/)
+[![Downloads](https://static.pepy.tech/badge/torchsurv)](https://pepy.tech/project/torchsurv)
 
 `TorchSurv` is a Python package that serves as a companion tool to perform deep survival modeling within the `PyTorch` environment. Unlike existing libraries that impose specific parametric forms on users, `TorchSurv` enables the use of custom `PyTorch`-based deep survival models.  With its lightweight design, minimal input requirements, full `PyTorch` backend, and freedom from restrictive survival model parameterizations, `TorchSurv` facilitates efficient survival model implementation, particularly beneficial for high-dimensional input data scenarios.
 
 ## TL;DR
 
 Our idea is to **keep things simple**. You are free to use any model architecture you want! Our code has 100% PyTorch backend and behaves like any other functions (losses or metrics) you may be familiar with.
 
@@ -83,31 +36,46 @@
 # You can test whether the observed c-index is greater than 0.5 (random estimator)
 cindex.p_value(method="noether", alternative="two_sided")
 
 # You can even compare the metrics between two models (e.g., vs. model B)
 cindex.compare(cindexB)
 ```
 
-## Installation
+## Installation and dependencies
 
 First, install the package:
 
 ```bash
 pip install torchsurv
 ```
 
-or for local installation (from package root)
+or for local installation (from package root / clone of this git repository):
 
 ```bash
 pip install -e .
 ```
 
 If you use Conda, you can install requirements into a conda environment
 using the `environment.yml` file included in the `dev` subfolder of the source repository.
 
+Using the package has the following dependencies which will be installed automatically via pip:
+
+* [torch](https://pytorch.org/): Consider pre-installing if you have specific system requirements (CPU / GPU / CUDA version).
+* [scipy](https://scipy.org/): We use some statistical helper functions to calculate metrics.
+* [torchmetrics](https://lightning.ai/docs/torchmetrics/stable/): We use some statistical helper functions to calculate metrics.
+
+To run the tests and example notebooks, you need to install the following additional packages:
+
+* [lifelines](https://lifelines.readthedocs.io/en/latest/)
+* [scikit-survival](https://scikit-survival.readthedocs.io/en/stable/)
+* [pytorch_lightning](https://lightning.ai/docs/pytorch/stable/) (and [lightning](https://lightning.ai/))
+
+To build the documentation and for package development, please see [the development notes](https://opensource.nibr.com/torchsurv/devnotes.html) and
+[dev/environment.yml](dev/environment.yml).
+
 ## Getting started
 
 We recommend starting with the [introductory guide](https://opensource.nibr.com/torchsurv/notebooks/introduction.html), where you'll find an overview of the package's functionalities.
 
 ### Survival data
 
 We simulate a random batch of 64 subjects. Each subject is associated with a binary event status (= `True` if event occured), a time-to-event or censoring and 16 covariates.
@@ -251,16 +219,31 @@
 
 1. Create Issues: If you encounter bugs, have feature requests, or want to suggest improvements, please create an [issue](https://github.com/Novartis/torchsurv/issues) in the GitHub repository. Make sure to provide detailed information about the problem, including code for reproducibility, or enhancement you're proposing.
 
 2. Fork and Pull Requests: If you're willing to address an existing issue or contribute a new feature, fork the repository, create a new branch, make your changes, and then submit a pull request. Please ensure your code follows our coding conventions and include tests for any new functionality.
 
 By contributing to this project, you agree to license your contributions under the same license as this project.
 
-## Contact
+## Contacts
+
+* [Thibaud Coroller](mailto:thibaud.coroller@novartis.com?subject=TorchSurv) `(creator, maintainer)`
+* [Mélodie Monod](mailto:melodie.monod@novartis.com?subject=TorchSurv) `(creator, maintainer)`
+* [Peter Krusche](mailto:peter.krusche@novartis.com?subject=TorchSurv) `(author, maintainer)`
+* [Qian Cao](mailto:qian.cao@fda.hhs.gov@novartis.com?subject=TorchSurv) `(author, maintainer)`
 
-If you have any questions, suggestions, or feedback, feel free to reach out to [us](https://opensource.nibr.com/torchsurv/AUTHORS.html).
+If you have any questions, suggestions, or feedback, feel free to reach out the developement team [us](https://opensource.nibr.com/torchsurv/AUTHORS.html).
 
 ## Cite
 
 If you use this project in academic work or publications, we appreciate citing it using the following BibTeX entry:
 
-TEMPORARY PLACEHOLDER.
+```
+@misc{monod2024torchsurv,
+      title={TorchSurv: A Lightweight Package for Deep Survival Analysis}, 
+      author={M{\'{e}}lodie Monod and Peter Krusche and Qian Cao and Berkman Sahiner and Nicholas Petrick and David Ohlssen and Thibaud Coroller},
+      year={2024},
+      eprint={2404.10761},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG},
+      doi={https://doi.org/10.48550/arXiv.2404.10761}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchsurv-0.1.1/pyproject.toml` & `torchsurv-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchsurv"
-version = "0.1.1"
+version = "0.1.2"
 description = "Survival analysis made easy with pytorch"
 authors = [
     {name = "Thibaud Coroller", email = "thibaud.coroller@novartis.com"},
     {name = "Melodie Monod", email = "melodie.monod@novartis.com"},
     {name = "Peter Krusche", email = "peter.krusche@novartis.com"},
     {name = "Qian Cao", email = "qian.cao@fda.hhs.com"}
 ]
@@ -26,15 +26,14 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
   "torch",
-  "lightning",
   "scipy",
   "numpy",
   "torchmetrics",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Novartis/torchsurv"
```

### Comparing `torchsurv-0.1.1/src/torchsurv/loss/cox.py` & `torchsurv-0.1.2/src/torchsurv/loss/cox.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/loss/momentum.py` & `torchsurv-0.1.2/src/torchsurv/loss/momentum.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/loss/weibull.py` & `torchsurv-0.1.2/src/torchsurv/loss/weibull.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/metrics/auc.py` & `torchsurv-0.1.2/src/torchsurv/metrics/auc.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/metrics/brier_score.py` & `torchsurv-0.1.2/src/torchsurv/metrics/brier_score.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/metrics/cindex.py` & `torchsurv-0.1.2/src/torchsurv/metrics/cindex.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/stats/ipcw.py` & `torchsurv-0.1.2/src/torchsurv/stats/ipcw.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/stats/kaplan_meier.py` & `torchsurv-0.1.2/src/torchsurv/stats/kaplan_meier.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv/tools/validate_inputs.py` & `torchsurv-0.1.2/src/torchsurv/tools/validate_inputs.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/src/torchsurv.egg-info/PKG-INFO` & `torchsurv-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsurv
-Version: 0.1.1
+Version: 0.1.2
 Summary: Survival analysis made easy with pytorch
 Author-email: Thibaud Coroller <thibaud.coroller@novartis.com>, Melodie Monod <melodie.monod@novartis.com>, Peter Krusche <peter.krusche@novartis.com>, Qian Cao <qian.cao@fda.hhs.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Novartis Pharmaceuticals Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,25 +38,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: torch
-Requires-Dist: lightning
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: torchmetrics
 
-# Survival analysis made easy
-
-> :warning: :construction: **We are still working on the publication of this project and appreciate your patience until everything will be ready.** :construction: :warning:
+# Deep survival analysis made easy
 
 ![CodeQC](https://github.com/Novartis/torchsurv/actions/workflows/codeqc.yml/badge.svg?branch=main)
 ![Docs](https://github.com/Novartis/torchsurv/actions/workflows/docs.yml/badge.svg?branch=main)
+[![PyPI - Version](https://img.shields.io/pypi/v/torchsurv)](https://pypi.org/project/torchsurv/)
+[![arXiv](https://img.shields.io/badge/arXiv-2404.10761-f9f107.svg)](https://arxiv.org/abs/2404.10761)
+[![Documentation](https://img.shields.io/badge/GithubPage-Sphinx-blue)](https://opensource.nibr.com/torchsurv/)
+[![Downloads](https://static.pepy.tech/badge/torchsurv)](https://pepy.tech/project/torchsurv)
 
 `TorchSurv` is a Python package that serves as a companion tool to perform deep survival modeling within the `PyTorch` environment. Unlike existing libraries that impose specific parametric forms on users, `TorchSurv` enables the use of custom `PyTorch`-based deep survival models.  With its lightweight design, minimal input requirements, full `PyTorch` backend, and freedom from restrictive survival model parameterizations, `TorchSurv` facilitates efficient survival model implementation, particularly beneficial for high-dimensional input data scenarios.
 
 ## TL;DR
 
 Our idea is to **keep things simple**. You are free to use any model architecture you want! Our code has 100% PyTorch backend and behaves like any other functions (losses or metrics) you may be familiar with.
 
@@ -83,31 +84,46 @@
 # You can test whether the observed c-index is greater than 0.5 (random estimator)
 cindex.p_value(method="noether", alternative="two_sided")
 
 # You can even compare the metrics between two models (e.g., vs. model B)
 cindex.compare(cindexB)
 ```
 
-## Installation
+## Installation and dependencies
 
 First, install the package:
 
 ```bash
 pip install torchsurv
 ```
 
-or for local installation (from package root)
+or for local installation (from package root / clone of this git repository):
 
 ```bash
 pip install -e .
 ```
 
 If you use Conda, you can install requirements into a conda environment
 using the `environment.yml` file included in the `dev` subfolder of the source repository.
 
+Using the package has the following dependencies which will be installed automatically via pip:
+
+* [torch](https://pytorch.org/): Consider pre-installing if you have specific system requirements (CPU / GPU / CUDA version).
+* [scipy](https://scipy.org/): We use some statistical helper functions to calculate metrics.
+* [torchmetrics](https://lightning.ai/docs/torchmetrics/stable/): We use some statistical helper functions to calculate metrics.
+
+To run the tests and example notebooks, you need to install the following additional packages:
+
+* [lifelines](https://lifelines.readthedocs.io/en/latest/)
+* [scikit-survival](https://scikit-survival.readthedocs.io/en/stable/)
+* [pytorch_lightning](https://lightning.ai/docs/pytorch/stable/) (and [lightning](https://lightning.ai/))
+
+To build the documentation and for package development, please see [the development notes](https://opensource.nibr.com/torchsurv/devnotes.html) and
+[dev/environment.yml](dev/environment.yml).
+
 ## Getting started
 
 We recommend starting with the [introductory guide](https://opensource.nibr.com/torchsurv/notebooks/introduction.html), where you'll find an overview of the package's functionalities.
 
 ### Survival data
 
 We simulate a random batch of 64 subjects. Each subject is associated with a binary event status (= `True` if event occured), a time-to-event or censoring and 16 covariates.
@@ -251,16 +267,31 @@
 
 1. Create Issues: If you encounter bugs, have feature requests, or want to suggest improvements, please create an [issue](https://github.com/Novartis/torchsurv/issues) in the GitHub repository. Make sure to provide detailed information about the problem, including code for reproducibility, or enhancement you're proposing.
 
 2. Fork and Pull Requests: If you're willing to address an existing issue or contribute a new feature, fork the repository, create a new branch, make your changes, and then submit a pull request. Please ensure your code follows our coding conventions and include tests for any new functionality.
 
 By contributing to this project, you agree to license your contributions under the same license as this project.
 
-## Contact
+## Contacts
+
+* [Thibaud Coroller](mailto:thibaud.coroller@novartis.com?subject=TorchSurv) `(creator, maintainer)`
+* [Mélodie Monod](mailto:melodie.monod@novartis.com?subject=TorchSurv) `(creator, maintainer)`
+* [Peter Krusche](mailto:peter.krusche@novartis.com?subject=TorchSurv) `(author, maintainer)`
+* [Qian Cao](mailto:qian.cao@fda.hhs.gov@novartis.com?subject=TorchSurv) `(author, maintainer)`
 
-If you have any questions, suggestions, or feedback, feel free to reach out to [us](https://opensource.nibr.com/torchsurv/AUTHORS.html).
+If you have any questions, suggestions, or feedback, feel free to reach out the developement team [us](https://opensource.nibr.com/torchsurv/AUTHORS.html).
 
 ## Cite
 
 If you use this project in academic work or publications, we appreciate citing it using the following BibTeX entry:
 
-TEMPORARY PLACEHOLDER.
+```
+@misc{monod2024torchsurv,
+      title={TorchSurv: A Lightweight Package for Deep Survival Analysis}, 
+      author={M{\'{e}}lodie Monod and Peter Krusche and Qian Cao and Berkman Sahiner and Nicholas Petrick and David Ohlssen and Thibaud Coroller},
+      year={2024},
+      eprint={2404.10761},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG},
+      doi={https://doi.org/10.48550/arXiv.2404.10761}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchsurv-0.1.1/src/torchsurv.egg-info/SOURCES.txt` & `torchsurv-0.1.2/src/torchsurv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_auc.py` & `torchsurv-0.1.2/tests/test_auc.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_brier_score.py` & `torchsurv-0.1.2/tests/test_brier_score.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_cindex.py` & `torchsurv-0.1.2/tests/test_cindex.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_cox.py` & `torchsurv-0.1.2/tests/test_cox.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_ipcw.py` & `torchsurv-0.1.2/tests/test_ipcw.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_kaplan_meier.py` & `torchsurv-0.1.2/tests/test_kaplan_meier.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_mnist.py` & `torchsurv-0.1.2/tests/test_mnist.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_momentum.py` & `torchsurv-0.1.2/tests/test_momentum.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_train.py` & `torchsurv-0.1.2/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `torchsurv-0.1.1/tests/test_weibull.py` & `torchsurv-0.1.2/tests/test_weibull.py`

 * *Files identical despite different names*

