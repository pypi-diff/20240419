# Comparing `tmp/graforvfl-1.0.0.tar.gz` & `tmp/graforvfl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graforvfl-1.0.0.tar", last modified: Tue Dec  5 02:15:24 2023, max compression
+gzip compressed data, was "graforvfl-1.1.0.tar", last modified: Fri Apr 19 00:50:19 2024, max compression
```

## Comparing `graforvfl-1.0.0.tar` & `graforvfl-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:15:24.887176 graforvfl-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2023-12-05 02:14:44.000000 graforvfl-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-05 02:14:44.000000 graforvfl-1.0.0/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-05 02:14:44.000000 graforvfl-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-12-05 02:14:44.000000 graforvfl-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14221 2023-12-05 02:15:24.887176 graforvfl-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2023-12-05 02:14:44.000000 graforvfl-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:15:24.883176 graforvfl-1.0.0/graforvfl/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:15:24.883176 graforvfl-1.0.0/graforvfl/network/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/network/base_rvfl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/network/mha_tune_rvfl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/network/standard_rvfl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:15:24.887176 graforvfl-1.0.0/graforvfl/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/shared/activator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/shared/boundary_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/shared/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/shared/randomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/shared/scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-05 02:14:44.000000 graforvfl-1.0.0/graforvfl/shared/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:15:24.887176 graforvfl-1.0.0/graforvfl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14221 2023-12-05 02:15:24.000000 graforvfl-1.0.0/graforvfl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-05 02:15:24.000000 graforvfl-1.0.0/graforvfl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 02:15:24.000000 graforvfl-1.0.0/graforvfl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-05 02:15:24.000000 graforvfl-1.0.0/graforvfl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-05 02:15:24.000000 graforvfl-1.0.0/graforvfl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 02:15:24.887176 graforvfl-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2023-12-05 02:14:44.000000 graforvfl-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:15:24.887176 graforvfl-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-12-05 02:14:44.000000 graforvfl-1.0.0/tests/test_MhaTuneRvfl.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-05 02:14:44.000000 graforvfl-1.0.0/tests/test_RvflClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-05 02:14:44.000000 graforvfl-1.0.0/tests/test_RvflRegressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:50:19.214789 graforvfl-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-19 00:49:39.000000 graforvfl-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-19 00:49:39.000000 graforvfl-1.1.0/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 00:49:39.000000 graforvfl-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 00:49:39.000000 graforvfl-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-19 00:50:19.214789 graforvfl-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-19 00:49:39.000000 graforvfl-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:50:19.210789 graforvfl-1.1.0/graforvfl/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:50:19.214789 graforvfl-1.1.0/graforvfl/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/network/base_rvfl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12634 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/network/gfo_rvfl_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/network/standard_rvfl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:50:19.214789 graforvfl-1.1.0/graforvfl/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/shared/activator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/shared/boundary_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/shared/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/shared/randomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/shared/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-19 00:49:39.000000 graforvfl-1.1.0/graforvfl/shared/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:50:19.214789 graforvfl-1.1.0/graforvfl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-19 00:50:19.000000 graforvfl-1.1.0/graforvfl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-19 00:50:19.000000 graforvfl-1.1.0/graforvfl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:50:19.000000 graforvfl-1.1.0/graforvfl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 00:50:19.000000 graforvfl-1.1.0/graforvfl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 00:50:19.000000 graforvfl-1.1.0/graforvfl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:50:19.214789 graforvfl-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-19 00:49:39.000000 graforvfl-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:50:19.214789 graforvfl-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-19 00:49:39.000000 graforvfl-1.1.0/tests/test_GfoRvflTuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-19 00:49:39.000000 graforvfl-1.1.0/tests/test_RvflClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 00:49:39.000000 graforvfl-1.1.0/tests/test_RvflRegressor.py
```

### Comparing `graforvfl-1.0.0/CODE_OF_CONDUCT.md` & `graforvfl-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `graforvfl-1.0.0/LICENSE` & `graforvfl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graforvfl-1.0.0/PKG-INFO` & `graforvfl-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: graforvfl
-Version: 1.0.0
-Summary: GrafoRVFL: A Python Library for Maximizing Performance of Random Vector Functional Link Network with Gradient-Free Optimization
+Version: 1.1.0
+Summary: GrafoRVFL: A Gradient-Free Optimization Framework for Boosting Random Vector Functional Link Network
 Home-page: https://github.com/thieu1995/GrafoRVFL
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://graforvfl.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/GrafoRVFL
 Project-URL: Bug Tracker, https://github.com/thieu1995/GrafoRVFL/issues
@@ -38,26 +38,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.1
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: scikit-learn>=1.0.2
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: mealpy>=3.0.1
-Requires-Dist: permetrics>=1.5.0
+Requires-Dist: permetrics>=2.0.0
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: pytest-cov==4.0.0; extra == "dev"
 Requires-Dist: flake8>=4.0.1; extra == "dev"
 
 
 # GrafoRVFL (GRAdient Free Optimized Random Vector Functional Link)
 
 ---
 
-[![GitHub release](https://img.shields.io/badge/release-1.0.0-yellow.svg)](https://github.com/thieu1995/GrafoRVFL/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.1.0-yellow.svg)](https://github.com/thieu1995/GrafoRVFL/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/graforvfl) 
 [![PyPI version](https://badge.fury.io/py/graforvfl.svg)](https://badge.fury.io/py/graforvfl)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graforvfl.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/graforvfl.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/graforvfl.svg)
 [![Downloads](https://pepy.tech/badge/graforvfl)](https://pepy.tech/project/graforvfl)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/graforvfl/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/graforvfl/actions/workflows/publish-package.yaml)
@@ -66,49 +66,42 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/graforvfl.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10258280.svg)](https://doi.org/10.5281/zenodo.10258280)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-GrafoRVFL is an open-source library in Python that employs gradient-free optimization ((GA, PSO, WOA, TLO, DE, ...) to 
+GrafoRVFL is an open-source library in Python that employs gradient-free optimization (GA, PSO, WOA, TLO, DE, ...) to 
 optimize Random Vector Functional Link Networks. It is entirely implemented based on Numpy and fully compatible 
 with the interfaces of the Scikit-Learn library. With GrafoRVFL, you can fine-tune the hyper-parameters of network 
 or optimize weights in the network using gradient-free optimizers.
 
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Provided Estimator**: RvflRegressor, RvflClassifier, MhaTuneRvfl
-* **Total Gradient Free based RVFL Regressor**: > 200 Models 
-* **Total Gradient Free based RVFL Classifier**: > 200 Models
-* **Supported performance metrics**: >= 67 (47 regressions and 20 classifications)
-* **Supported objective functions (as fitness functions or loss functions)**: >= 67 (47 regressions and 20 classifications)
 * **Documentation:** https://graforvfl.readthedocs.io
+* **Provided Estimator**: `RvflRegressor`, `RvflClassifier`, `GfoRvflTuner`
 * **Python versions:** >= 3.8.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Citation Request 
 
 * Learn more about Random Vector Functional Link from [this paper](https://doi.org/10.1016/j.ins.2015.09.025)
 
 * Learn more about on how to use Gradient Free Optimization to fine-tune the hyper-parameter of RVFL networks from 
 [this paper](https://doi.org/10.1109/TCSS.2022.3146974)
 
-* Learn more about on how to use Gradient Free Optimization to optimize the weights of RVFL netweorks from [this paper](https://doi.org/10.1109/SOCA.2018.00014)
-
-
 
 Please include these citations if you plan to use this library:
 
-```code
+```bibtex
 
 @software{nguyen_van_thieu_2023_10258280,
   author       = {Nguyen Van Thieu},
-  title        = {GrafoRVFL: A Python Library for Maximizing Performance of Random Vector Functional Link Network with Gradient-Free Optimization},
+  title        = {GrafoRVFL: A Gradient-Free Optimization Framework for Boosting Random Vector Functional Link Network},
   month        = dec,
   year         = 2023,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.10258280},
   url          = {https://github.com/thieu1995/GrafoRVFL}
 }
 
@@ -136,184 +129,80 @@
   booktitle={2018 IEEE 11th conference on service-oriented computing and applications (SOCA)},
   pages={49--56},
   year={2018},
   organization={IEEE},
   doi={10.1109/SOCA.2018.00014}
 }
 
-
 ```
 
 # Installation
 
 * Install the [current PyPI release](https://pypi.python.org/pypi/graforvfl):
 ```sh 
-$ pip install graforvfl==1.0.0
-```
-
-* Install directly from source code
-```sh 
-$ git clone https://github.com/thieu1995/GrafoRVFL.git
-$ cd GrafoRVFL
-$ python setup.py install
+$ pip install graforvfl
 ```
 
-* In case, you want to install the development version from Github:
-```sh 
-$ pip install git+https://github.com/thieu1995/GrafoRVFL 
-```
-
-After installation, you can import GrafoRVFL as any other Python module:
+After installation, you can check the installed version by:
 
 ```sh
 $ python
 >>> import graforvfl
 >>> graforvfl.__version__
 ```
 
-### Examples
-
-Please check all use cases and examples in folder [examples](examples).
-
-Current provided classes:
-
-```python
-from graforvfl import DataTransformer, Data
-from graforvfl import RvflRegressor, RvflClassifier, MhaTuneRvfl
-```
-
-##### `DataTransformer` class
-
-We provide many scaler classes that you can select and make a combination of transforming your data via 
-DataTransformer class. For example: scale data by `Loge` and then `Sqrt` and then `MinMax`:
-
-```python
-from graforvfl import DataTransformer
-import pandas as pd
-from sklearn.model_selection import train_test_split
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-X_train, y_train, X_test, y_test = train_test_split(X, y, test_size=0.2)
-
-dt = DataTransformer(scaling_methods=("loge", "sqrt", "minmax"))
-X_train_scaled = dt.fit_transform(X_train)
-X_test_scaled = dt.transform(X_test)
-```
-
-##### `Data` class
+# Example
 
-+ You can load your dataset into Data class
-+ You can split dataset to train and test set
-+ You can scale dataset without using DataTransformer class
-+ You can scale labels using LabelEncoder
+Below is the example code of how to use Gradient Free Optimization to tune hyper-parameter of RVFL network.
+The more complicated cases in the folder: [examples](/examples). You can also read the [documentation](https://graforvfl.readthedocs.io/) 
+for more detailed installation instructions, explanations, and examples.
 
 ```python
-from graforvfl import Data
-import pandas as pd
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
+from sklearn.datasets import load_breast_cancer
+from mealpy import StringVar, IntegerVar
+from graforvfl import Data, GfoRvflTuner
+
+## Load data object
+X, y = load_breast_cancer(return_X_y=True)
+data = Data(X, y)
+
+## Split train and test
+data.split_train_test(test_size=0.2, random_state=2, inplace=True)
+print(data.X_train.shape, data.X_test.shape)
 
-data = Data(X, y, name="position_salaries")
-
-#### Split dataset into train and test set
-data.split_train_test(test_size=0.2, shuffle=True, random_state=100, inplace=True)
-
-#### Feature Scaling
-data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard", "sqrt", "minmax"))
+## Scaling dataset
+data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard", "minmax"))
 data.X_test = scaler_X.transform(data.X_test)
 
-data.y_train, scaler_y = data.encode_label(data.y_train)  # This is for classification problem only
+data.y_train, scaler_y = data.encode_label(data.y_train)
 data.y_test = scaler_y.transform(data.y_test)
-```
 
-##### `Neural Network` class
-
-```python
-from graforvfl import RvflRegressor, RvflClassifier, MhaTuneRvfl
-from mealpy import IntegerVar, StringVar
-
-## 1. Use standard RVFL model for regression problem
-model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_uniform", trainer="OLS", alpha=0.5)
-
-## 2. Use standard RVFL model for classification problem 
-model = RvflClassifier(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="OLS", alpha=0.5)
-
-
-## 3. Use Gradient Free Optimization to fine-tune the hyper-parameter of RVFL network for regression problem
 # Design the boundary (parameters)
 my_bounds = [
     IntegerVar(lb=2, ub=1000, name="size_hidden"),
     StringVar(valid_sets=("none", "relu", "leaky_relu", "celu", "prelu", "gelu",
                           "elu", "selu", "rrelu", "tanh", "sigmoid"), name="act_name"),
     StringVar(valid_sets=("orthogonal", "he_uniform", "he_normal", "glorot_uniform", "glorot_normal",
                           "lecun_uniform", "lecun_normal", "random_uniform", "random_normal"), name="weight_initializer")
 ]
-opt_paras = {"name": "WOA", "epoch": 10, "pop_size": 20}
-model = MhaTuneRvfl(problem_type="regression", bounds=my_bounds, cv=3, scoring="MSE",
-                      optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True)
-```
-
-##### Supported functions in `model` object
-
-```python
-from graforvfl import RvflRegressor, Data 
-
-data = Data()       # Assumption that you have provided this object like above
 
-model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_uniform", trainer="OLS", alpha=0.5)
-
-## Train the model
+opt_paras = {"name": "WOA", "epoch": 10, "pop_size": 20}
+model = GfoRvflTuner(problem_type="classification", bounds=my_bounds, cv=3, scoring="AS",
+                      optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True, seed=42)
 model.fit(data.X_train, data.y_train)
-
-## Predicting a new result
-y_pred = model.predict(data.X_test)
-
-## Calculate metrics using score or scores functions.
-print(model.score(data.X_test, data.y_test, method="MAE"))
-print(model.scores(data.X_test, data.y_test, list_methods=["MAPE", "NNSE", "KGE", "MASE", "R2", "R", "R2S"]))
-
-## Calculate metrics using evaluate function
-print(model.evaluate(data.y_test, y_pred, list_metrics=("MSE", "RMSE", "MAPE", "NSE")))
-
-## Save performance metrics to csv file
-model.save_metrics(data.y_test, y_pred, list_metrics=("RMSE", "MAE"), save_path="history", filename="metrics.csv")
-
-## Save training loss to csv file
-model.save_loss_train(save_path="history", filename="loss.csv")
-
-## Save predicted label
-model.save_y_predicted(X=data.X_test, y_true=data.y_test, save_path="history", filename="y_predicted.csv")
-
-## Save model
-model.save_model(save_path="history", filename="traditional_mlp.pkl")
-
-## Load model 
-trained_model = RvflRegressor.load_model(load_path="history", filename="traditional_mlp.pkl")
+print(model.best_params)
+print(model.best_estimator)
+print(model.best_estimator.scores(data.X_test, data.y_test, list_methods=("PS", "RS", "NPV", "F1S", "F2S")))
 ```
 
-# Support (questions, problems)
+# Official channels 
+
+* [Official source code repository](https://github.com/thieu1995/GrafoRVFL)
+* [Official document](https://graforvfl.readthedocs.io/)
+* [Download releases](https://pypi.org/project/graforvfl/) 
+* [Issue tracker](https://github.com/thieu1995/GrafoRVFL/issues) 
+* [Notable changes log](/ChangeLog.md)
+* [Official discussion group](https://t.me/+fRVCJGuGJg1mNDg1)
 
-### Official Links 
+---
 
-* Official source code repo: https://github.com/thieu1995/GrafoRVFL
-* Official document: https://graforvfl.readthedocs.io/
-* Download releases: https://pypi.org/project/graforvfl/
-* Issue tracker: https://github.com/thieu1995/GrafoRVFL/issues
-* Notable changes log: https://github.com/thieu1995/GrafoRVFL/blob/main/ChangeLog.md
-* Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
-
-* This project also related to our another projects which are "optimization" and "machine learning", check it here:
-    * https://github.com/thieu1995/mealpy
-    * https://github.com/thieu1995/metaheuristics
-    * https://github.com/thieu1995/opfunu
-    * https://github.com/thieu1995/enoppy
-    * https://github.com/thieu1995/permetrics
-    * https://github.com/thieu1995/MetaCluster
-    * https://github.com/thieu1995/pfevaluator
-    * https://github.com/thieu1995/IntelELM
-    * https://github.com/thieu1995/reflame
-    * https://github.com/thieu1995/MetaPerceptron
-    * https://github.com/aiir-team
+Developed by: [Thieu](mailto:nguyenthieu2102@gmail.com?Subject=GrafoRVFL_QUESTIONS) @ 2023
```

### Comparing `graforvfl-1.0.0/graforvfl/__init__.py` & `graforvfl-1.1.0/graforvfl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 10/08/2023 ----------%
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 from graforvfl.shared.data_processor import DataTransformer, Data, get_dataset
 from graforvfl.network.standard_rvfl import RvflRegressor, RvflClassifier
-from graforvfl.network.mha_tune_rvfl import MhaTuneRvfl
+from graforvfl.network.gfo_rvfl_tuner import GfoRvflTuner
```

### Comparing `graforvfl-1.0.0/graforvfl/network/base_rvfl.py` & `graforvfl-1.1.0/graforvfl/network/base_rvfl.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,28 +40,33 @@
         The utilized method for training weights of hidden-output layer and weights of input-output layer.
             + MPI: Moore-Penrose inversion
             + OLS: Ordinary Least Squares (OLS) without regularization
             + L2: OLS regression with regularization
 
     alpha : float (Optional), default=0.5
         The penalty value for L2 method. Only effect when `trainer`="L2".
+
+    seed: int, default=None
+        Determines random number generation for weights and bias initialization.
+        Pass an int for reproducible results across multiple function calls.
     """
 
     SUPPORTED_CLS_METRICS = get_all_classification_metrics()
     SUPPORTED_REG_METRICS = get_all_regression_metrics()
     CLS_OBJ_LOSSES = None
     SUPPORTED_WEIGHT_INITIALIZER = [
         "orthogonal", "he_uniform", "he_normal", "glorot_uniform", "glorot_normal",
         "lecun_uniform", "lecun_normal", "random_uniform", "random_normal"
     ]
 
-    def __init__(self, size_hidden=10, act_name='sigmoid', weight_initializer="random_uniform", trainer="MPI", alpha=0.5):
+    def __init__(self, size_hidden=10, act_name='sigmoid', weight_initializer="random_uniform", trainer="MPI", alpha=0.5, seed=None):
         self.size_hidden = size_hidden
         self.act_name = act_name
         self.act_func = getattr(activator, self.act_name)
+        self.seed = seed
         self.weight_initializer, self.weight_randomer = self._get_weight_initializer(weight_initializer)
         self.trainer = trainer
         self.alpha = alpha
         self.weights = {}
         self.obj_scaler, self.loss_train = None, None
         self.n_labels, self.obj_scaler = None, None
 
@@ -80,34 +85,34 @@
         else:
             raise ValueError(f"method should be a string and belongs to {list_supported_methods}")
 
     def _trained(self, trainer="OLS", D=None, y=None):
         if trainer == "MPI":
             return np.linalg.pinv(D) @ y
         elif trainer == "L2":
-            ridge_model = Ridge(alpha=self.alpha, fit_intercept=False)
+            ridge_model = Ridge(alpha=self.alpha, fit_intercept=False, random_state=self.seed)
             return ridge_model.fit(D, y).coef_.T
         else:
-            ridge_model = Ridge(alpha=0.0, fit_intercept=False)
+            ridge_model = Ridge(alpha=0.0, fit_intercept=False, random_state=self.seed)
             return ridge_model.fit(D, y).coef_.T
 
     def fit(self, X, y):
         self.size_input = X.shape[1]
         if type(y) in (list, tuple, np.ndarray):
             y = np.squeeze(np.asarray(y))
             if y.ndim == 1:
                 self.size_output = 1
             elif y.ndim == 2:
                 self.size_output = y.shape[1]
             else:
                 raise TypeError("Invalid y array shape, it should be 1D vector or 2D matrix.")
         else:
             raise TypeError("Invalid y array type, it should be list, tuple or np.ndarray")
-        self.weights["Wh"] = self.weight_randomer((self.size_hidden, self.size_input))
-        self.weights["bh"] = self.weight_randomer(self.size_hidden).flatten()
+        self.weights["Wh"] = self.weight_randomer((self.size_hidden, self.size_input), seed=self.seed)
+        self.weights["bh"] = self.weight_randomer(self.size_hidden, seed=self.seed).flatten()
         H = self.act_func(X @ self.weights["Wh"].T + self.weights["bh"])
         D = np.concatenate((X, H), axis=1)
         self.weights["Wioho"] = self._trained(self.trainer, D, y)
         return self
 
     def predict(self, X):
         H = self.act_func(X @ self.weights["Wh"].T + self.weights["bh"])
@@ -127,25 +132,25 @@
     def set_weights(self, weights):
         self.weights = weights
 
     def get_weights_size(self):
         return np.sum([item.size for item in self.weights.values()])
 
     def __evaluate_reg(self, y_true, y_pred, list_metrics=("MSE", "MAE")):
-        rm = RegressionMetric(y_true=y_true, y_pred=y_pred, decimal=8)
+        rm = RegressionMetric(y_true=y_true, y_pred=y_pred)
         return rm.get_metrics_by_list_names(list_metrics)
 
     def __evaluate_cls(self, y_true, y_pred, list_metrics=("AS", "RS")):
-        cm = ClassificationMetric(y_true, y_pred, decimal=8)
+        cm = ClassificationMetric(y_true, y_pred)
         return cm.get_metrics_by_list_names(list_metrics)
 
     def __score_reg(self, X, y, method="RMSE"):
         method = self._check_method(method, list(self.SUPPORTED_REG_METRICS.keys()))
         y_pred = self.predict(X)
-        return RegressionMetric(y, y_pred, decimal=8).get_metric_by_name(method)[method]
+        return RegressionMetric(y, y_pred).get_metric_by_name(method)[method]
 
     def __scores_reg(self, X, y, list_methods=("MSE", "MAE")):
         y_pred = self.predict(X)
         return self.__evaluate_reg(y_true=y, y_pred=y_pred, list_metrics=list_methods)
 
     def __score_cls(self, X, y, method="AS"):
         method = self._check_method(method, list(self.SUPPORTED_CLS_METRICS.keys()))
@@ -153,15 +158,15 @@
         if self.n_labels > 2:
             if method in self.CLS_OBJ_LOSSES:
                 return_prob = True
         if return_prob:
             y_pred = self.predict_proba(X)
         else:
             y_pred = self.predict(X)
-        cm = ClassificationMetric(y_true=y, y_pred=y_pred, decimal=8)
+        cm = ClassificationMetric(y_true=y, y_pred=y_pred)
         return cm.get_metric_by_name(method)[method]
 
     def __scores_cls(self, X, y, list_methods=("AS", "RS")):
         list_errors = list(set(list_methods) & set(self.CLS_OBJ_LOSSES))
         list_scores = list((set(self.SUPPORTED_CLS_METRICS.keys()) - set(self.CLS_OBJ_LOSSES)) & set(list_methods))
         t1 = {}
         if len(list_errors) > 0:
```

### Comparing `graforvfl-1.0.0/graforvfl/network/standard_rvfl.py` & `graforvfl-1.1.0/graforvfl/network/standard_rvfl.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,29 +36,33 @@
             + MPI: Moore-Penrose inversion
             + OLS: Ordinary Least Squares (OLS) without regularization
             + L2: OLS regression with regularization
 
     alpha : float (Optional), default=0.5
         The penalty value for L2 method. Only effect when `trainer`="L2".
 
+    seed: int, default=None
+        Determines random number generation for weights and bias initialization.
+        Pass an int for reproducible results across multiple function calls.
+
     Examples
     --------
     >>> from graforvfl import RvflRegressor, Data
     >>> from sklearn.datasets import make_regression
     >>> X, y = make_regression(n_samples=200, random_state=1)
     >>> data = Data(X, y)
     >>> data.split_train_test(test_size=0.2, random_state=1)
-    >>> model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="OLS", alpha=0.5)
+    >>> model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="OLS", alpha=0.5, seed=42)
     >>> model.fit(data.X_train, data.y_train)
     >>> pred = model.predict(data.X_test)
     >>> print(pred)
     """
 
-    def __init__(self, size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI", alpha=0.5):
-        super().__init__(size_hidden=size_hidden, act_name=act_name, weight_initializer=weight_initializer, trainer=trainer, alpha=alpha)
+    def __init__(self, size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI", alpha=0.5, seed=None):
+        super().__init__(size_hidden=size_hidden, act_name=act_name, weight_initializer=weight_initializer, trainer=trainer, alpha=alpha, seed=seed)
 
     def score(self, X, y, method="RMSE"):
         return self._BaseRVFL__score_reg(X, y, method)
 
     def scores(self, X, y, list_methods=("MSE", "MAE")):
         return self._BaseRVFL__scores_reg(X, y, list_methods)
 
@@ -92,47 +96,52 @@
             + MPI: Moore-Penrose inversion
             + OLS: Ordinary Least Squares (OLS) without regularization
             + L2: OLS regression with regularization
 
     alpha : float (Optional), default=0.5
         The penalty value for L2 method. Only effect when `trainer`="L2".
 
+    seed: int, default=None
+        Determines random number generation for weights and bias initialization.
+        Pass an int for reproducible results across multiple function calls.
+
     Examples
     --------
     >>> from graforvfl import Data, RvflClassifier
     >>> from sklearn.datasets import make_classification
     >>> X, y = make_classification(n_samples=100, random_state=1)
     >>> data = Data(X, y)
     >>> data.split_train_test(test_size=0.2, random_state=1)
-    >>> model = RvflClassifier(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="OLS", alpha=0.5)
+    >>> model = RvflClassifier(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="OLS", alpha=0.5, seed=42)
     >>> model.fit(data.X_train, data.y_train)
     >>> pred = model.predict(data.X_test)
     >>> print(pred)
     array([1, 0, 1, 0, 1])
     """
 
     CLS_OBJ_LOSSES = ["CEL", "HL", "KLDL", "BSL"]
 
-    def __init__(self, size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI", alpha=0.5):
-        super().__init__(size_hidden=size_hidden, act_name=act_name, weight_initializer=weight_initializer, trainer=trainer, alpha=alpha)
+    def __init__(self, size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI", alpha=0.5, seed=None):
+        super().__init__(size_hidden=size_hidden, act_name=act_name, weight_initializer=weight_initializer, trainer=trainer, alpha=alpha, seed=seed)
         self.n_labels = None
         self.obj_scaler = None
 
     def fit(self, X, y):
         self.size_input = X.shape[1]
         if type(y) in (list, tuple, np.ndarray):
             y = np.squeeze(np.asarray(y))
             if y.ndim == 1:
                 self.n_labels = len(np.unique(y))
                 self.size_output = self.n_labels
+                self.classes_ = np.unique(y)
             else:
                 raise TypeError("Invalid y array shape, it should be 1D vector containing labels 0, 1, 2,.. and so on.")
         else:
             raise TypeError("Invalid y array type, it should be list, tuple or np.ndarray")
-        ohe_scaler = OneHotEncoder(sparse=False)
+        ohe_scaler = OneHotEncoder(sparse_output=False)
         ohe_scaler.fit(np.reshape(y, (-1, 1)))
         self.obj_scaler = ObjectiveScaler(obj_name="softmax", ohe_scaler=ohe_scaler)
         y_scaled = self.obj_scaler.transform(y)
 
         self.weights["Wh"] = self.weight_randomer((self.size_hidden, self.size_input))
         self.weights["bh"] = self.weight_randomer(self.size_hidden).flatten()
         H = self.act_func(X @ self.weights["Wh"].T + self.weights["bh"])
```

### Comparing `graforvfl-1.0.0/graforvfl/shared/activator.py` & `graforvfl-1.1.0/graforvfl/shared/activator.py`

 * *Files identical despite different names*

### Comparing `graforvfl-1.0.0/graforvfl/shared/boundary_controller.py` & `graforvfl-1.1.0/graforvfl/shared/boundary_controller.py`

 * *Files identical despite different names*

### Comparing `graforvfl-1.0.0/graforvfl/shared/data_processor.py` & `graforvfl-1.1.0/graforvfl/shared/data_processor.py`

 * *Files identical despite different names*

### Comparing `graforvfl-1.0.0/graforvfl/shared/randomer.py` & `graforvfl-1.1.0/graforvfl/shared/randomer.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,65 +13,78 @@
         return (shape, 1)
     elif type(shape) in (list, tuple, np.ndarray) and len(shape) == 1:
         return (shape[0], 1)
     else:
         return shape
 
 
-def orthogonal_initializer(shape, gain=1.0):
+def get_generator(seed=None):
+    return np.random.default_rng(seed)
+
+
+def orthogonal_initializer(shape, gain=1.0, seed=None):
+    generator = get_generator(seed)
     shape = get_correct_shape(shape)
     flat_shape = (shape[0], np.prod(shape[1:]))
-    a = np.random.normal(0.0, 1.0, flat_shape)
+    a = generator.normal(0., 1., flat_shape)
     u, _, v = np.linalg.svd(a, full_matrices=False)
     q = u if u.shape == flat_shape else v
     q = q.reshape(shape)
     return gain * q[:shape[0], :shape[1]]
 
 
-def he_uniform_initializer(shape):
+def he_uniform_initializer(shape, seed=None):
+    generator = get_generator(seed)
     shape = get_correct_shape(shape)
     fan_in = shape[0] if len(shape) == 2 else np.prod(shape[1:])
     limit = np.sqrt(6 / fan_in)
-    return np.random.uniform(-limit, limit, shape)
+    return generator.uniform(-limit, limit, shape)
 
 
-def he_normal_initializer(shape):
+def he_normal_initializer(shape, seed=None):
+    generator = get_generator(seed)
     shape = get_correct_shape(shape)
     fan_in = shape[0] if len(shape) == 2 else np.prod(shape[1:])
     stddev = np.sqrt(2 / fan_in)
-    return np.random.normal(0.0, stddev, shape)
+    return generator.normal(0.0, stddev, shape)
 
 
-def glorot_uniform_initializer(shape):
+def glorot_uniform_initializer(shape, seed=None):
+    generator = get_generator(seed)
     shape = get_correct_shape(shape)
     fan_in, fan_out = shape
     limit = np.sqrt(6 / (fan_in + fan_out))
-    return np.random.uniform(-limit, limit, shape)
+    return generator.uniform(-limit, limit, shape)
 
 
-def glorot_normal_initializer(shape):
+def glorot_normal_initializer(shape, seed=None):
+    generator = get_generator(seed)
     shape = get_correct_shape(shape)
     fan_in, fan_out = shape
     stddev = np.sqrt(2 / (fan_in + fan_out))
-    return np.random.normal(0.0, stddev, shape)
+    return generator.normal(0.0, stddev, shape)
 
 
-def lecun_uniform_initializer(shape):
+def lecun_uniform_initializer(shape, seed=None):
+    generator = get_generator(seed)
     shape = get_correct_shape(shape)
     fan_in = shape[0] if len(shape) == 2 else np.prod(shape[1:])
     limit = np.sqrt(3 / fan_in)
-    return np.random.uniform(-limit, limit, shape)
+    return generator.uniform(-limit, limit, shape)
 
 
-def lecun_normal_initializer(shape):
+def lecun_normal_initializer(shape, seed=None):
+    generator = get_generator(seed)
     shape = get_correct_shape(shape)
     fan_in = shape[0] if len(shape) == 2 else np.prod(shape[1:])
     stddev = np.sqrt(1 / fan_in)
-    return np.random.normal(0.0, stddev, shape)
+    return generator.normal(0.0, stddev, shape)
 
 
-def random_uniform_initializer(shape, minval=0.0, maxval=1.0):
-    return np.random.uniform(minval, maxval, shape)
+def random_uniform_initializer(shape, minval=0.0, maxval=1.0, seed=None):
+    generator = get_generator(seed)
+    return generator.uniform(minval, maxval, shape)
 
 
-def random_normal_initializer(shape, mean=0.0, stddev=1.0):
-    return np.random.normal(mean, stddev, shape)
+def random_normal_initializer(shape, mean=0.0, stddev=1.0, seed=None):
+    generator = get_generator(seed)
+    return generator.normal(mean, stddev, shape)
```

### Comparing `graforvfl-1.0.0/graforvfl/shared/scaler.py` & `graforvfl-1.1.0/graforvfl/shared/scaler.py`

 * *Files identical despite different names*

### Comparing `graforvfl-1.0.0/graforvfl/shared/scorer.py` & `graforvfl-1.1.0/graforvfl/shared/scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from permetrics.regression import RegressionMetric
 from permetrics.classification import ClassificationMetric
 
 
 def get_metrics(problem, y_true, y_pred, metrics=None, testcase="test"):
     if problem == "regression":
         evaluator = RegressionMetric(y_true, y_pred)
-        paras = [{"decimal": 4}, ] * len(metrics)
+        paras = [{}, ] * len(metrics)
     else:
         evaluator = ClassificationMetric(y_true, y_pred)
         paras = [{"average": "weighted"}, ] * len(metrics)
     if type(metrics) is dict:
         result = evaluator.get_metrics_by_dict(metrics)
     elif type(metrics) in (tuple, list):
         result = evaluator.get_metrics_by_list_names(metrics, paras)
```

### Comparing `graforvfl-1.0.0/graforvfl.egg-info/PKG-INFO` & `graforvfl-1.1.0/graforvfl.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: graforvfl
-Version: 1.0.0
-Summary: GrafoRVFL: A Python Library for Maximizing Performance of Random Vector Functional Link Network with Gradient-Free Optimization
+Version: 1.1.0
+Summary: GrafoRVFL: A Gradient-Free Optimization Framework for Boosting Random Vector Functional Link Network
 Home-page: https://github.com/thieu1995/GrafoRVFL
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://graforvfl.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/GrafoRVFL
 Project-URL: Bug Tracker, https://github.com/thieu1995/GrafoRVFL/issues
@@ -38,26 +38,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.1
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: scikit-learn>=1.0.2
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: mealpy>=3.0.1
-Requires-Dist: permetrics>=1.5.0
+Requires-Dist: permetrics>=2.0.0
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: pytest-cov==4.0.0; extra == "dev"
 Requires-Dist: flake8>=4.0.1; extra == "dev"
 
 
 # GrafoRVFL (GRAdient Free Optimized Random Vector Functional Link)
 
 ---
 
-[![GitHub release](https://img.shields.io/badge/release-1.0.0-yellow.svg)](https://github.com/thieu1995/GrafoRVFL/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.1.0-yellow.svg)](https://github.com/thieu1995/GrafoRVFL/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/graforvfl) 
 [![PyPI version](https://badge.fury.io/py/graforvfl.svg)](https://badge.fury.io/py/graforvfl)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graforvfl.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/graforvfl.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/graforvfl.svg)
 [![Downloads](https://pepy.tech/badge/graforvfl)](https://pepy.tech/project/graforvfl)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/graforvfl/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/graforvfl/actions/workflows/publish-package.yaml)
@@ -66,49 +66,42 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/graforvfl.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10258280.svg)](https://doi.org/10.5281/zenodo.10258280)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-GrafoRVFL is an open-source library in Python that employs gradient-free optimization ((GA, PSO, WOA, TLO, DE, ...) to 
+GrafoRVFL is an open-source library in Python that employs gradient-free optimization (GA, PSO, WOA, TLO, DE, ...) to 
 optimize Random Vector Functional Link Networks. It is entirely implemented based on Numpy and fully compatible 
 with the interfaces of the Scikit-Learn library. With GrafoRVFL, you can fine-tune the hyper-parameters of network 
 or optimize weights in the network using gradient-free optimizers.
 
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Provided Estimator**: RvflRegressor, RvflClassifier, MhaTuneRvfl
-* **Total Gradient Free based RVFL Regressor**: > 200 Models 
-* **Total Gradient Free based RVFL Classifier**: > 200 Models
-* **Supported performance metrics**: >= 67 (47 regressions and 20 classifications)
-* **Supported objective functions (as fitness functions or loss functions)**: >= 67 (47 regressions and 20 classifications)
 * **Documentation:** https://graforvfl.readthedocs.io
+* **Provided Estimator**: `RvflRegressor`, `RvflClassifier`, `GfoRvflTuner`
 * **Python versions:** >= 3.8.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Citation Request 
 
 * Learn more about Random Vector Functional Link from [this paper](https://doi.org/10.1016/j.ins.2015.09.025)
 
 * Learn more about on how to use Gradient Free Optimization to fine-tune the hyper-parameter of RVFL networks from 
 [this paper](https://doi.org/10.1109/TCSS.2022.3146974)
 
-* Learn more about on how to use Gradient Free Optimization to optimize the weights of RVFL netweorks from [this paper](https://doi.org/10.1109/SOCA.2018.00014)
-
-
 
 Please include these citations if you plan to use this library:
 
-```code
+```bibtex
 
 @software{nguyen_van_thieu_2023_10258280,
   author       = {Nguyen Van Thieu},
-  title        = {GrafoRVFL: A Python Library for Maximizing Performance of Random Vector Functional Link Network with Gradient-Free Optimization},
+  title        = {GrafoRVFL: A Gradient-Free Optimization Framework for Boosting Random Vector Functional Link Network},
   month        = dec,
   year         = 2023,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.10258280},
   url          = {https://github.com/thieu1995/GrafoRVFL}
 }
 
@@ -136,184 +129,80 @@
   booktitle={2018 IEEE 11th conference on service-oriented computing and applications (SOCA)},
   pages={49--56},
   year={2018},
   organization={IEEE},
   doi={10.1109/SOCA.2018.00014}
 }
 
-
 ```
 
 # Installation
 
 * Install the [current PyPI release](https://pypi.python.org/pypi/graforvfl):
 ```sh 
-$ pip install graforvfl==1.0.0
-```
-
-* Install directly from source code
-```sh 
-$ git clone https://github.com/thieu1995/GrafoRVFL.git
-$ cd GrafoRVFL
-$ python setup.py install
+$ pip install graforvfl
 ```
 
-* In case, you want to install the development version from Github:
-```sh 
-$ pip install git+https://github.com/thieu1995/GrafoRVFL 
-```
-
-After installation, you can import GrafoRVFL as any other Python module:
+After installation, you can check the installed version by:
 
 ```sh
 $ python
 >>> import graforvfl
 >>> graforvfl.__version__
 ```
 
-### Examples
-
-Please check all use cases and examples in folder [examples](examples).
-
-Current provided classes:
-
-```python
-from graforvfl import DataTransformer, Data
-from graforvfl import RvflRegressor, RvflClassifier, MhaTuneRvfl
-```
-
-##### `DataTransformer` class
-
-We provide many scaler classes that you can select and make a combination of transforming your data via 
-DataTransformer class. For example: scale data by `Loge` and then `Sqrt` and then `MinMax`:
-
-```python
-from graforvfl import DataTransformer
-import pandas as pd
-from sklearn.model_selection import train_test_split
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-X_train, y_train, X_test, y_test = train_test_split(X, y, test_size=0.2)
-
-dt = DataTransformer(scaling_methods=("loge", "sqrt", "minmax"))
-X_train_scaled = dt.fit_transform(X_train)
-X_test_scaled = dt.transform(X_test)
-```
-
-##### `Data` class
+# Example
 
-+ You can load your dataset into Data class
-+ You can split dataset to train and test set
-+ You can scale dataset without using DataTransformer class
-+ You can scale labels using LabelEncoder
+Below is the example code of how to use Gradient Free Optimization to tune hyper-parameter of RVFL network.
+The more complicated cases in the folder: [examples](/examples). You can also read the [documentation](https://graforvfl.readthedocs.io/) 
+for more detailed installation instructions, explanations, and examples.
 
 ```python
-from graforvfl import Data
-import pandas as pd
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
+from sklearn.datasets import load_breast_cancer
+from mealpy import StringVar, IntegerVar
+from graforvfl import Data, GfoRvflTuner
+
+## Load data object
+X, y = load_breast_cancer(return_X_y=True)
+data = Data(X, y)
+
+## Split train and test
+data.split_train_test(test_size=0.2, random_state=2, inplace=True)
+print(data.X_train.shape, data.X_test.shape)
 
-data = Data(X, y, name="position_salaries")
-
-#### Split dataset into train and test set
-data.split_train_test(test_size=0.2, shuffle=True, random_state=100, inplace=True)
-
-#### Feature Scaling
-data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard", "sqrt", "minmax"))
+## Scaling dataset
+data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard", "minmax"))
 data.X_test = scaler_X.transform(data.X_test)
 
-data.y_train, scaler_y = data.encode_label(data.y_train)  # This is for classification problem only
+data.y_train, scaler_y = data.encode_label(data.y_train)
 data.y_test = scaler_y.transform(data.y_test)
-```
 
-##### `Neural Network` class
-
-```python
-from graforvfl import RvflRegressor, RvflClassifier, MhaTuneRvfl
-from mealpy import IntegerVar, StringVar
-
-## 1. Use standard RVFL model for regression problem
-model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_uniform", trainer="OLS", alpha=0.5)
-
-## 2. Use standard RVFL model for classification problem 
-model = RvflClassifier(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="OLS", alpha=0.5)
-
-
-## 3. Use Gradient Free Optimization to fine-tune the hyper-parameter of RVFL network for regression problem
 # Design the boundary (parameters)
 my_bounds = [
     IntegerVar(lb=2, ub=1000, name="size_hidden"),
     StringVar(valid_sets=("none", "relu", "leaky_relu", "celu", "prelu", "gelu",
                           "elu", "selu", "rrelu", "tanh", "sigmoid"), name="act_name"),
     StringVar(valid_sets=("orthogonal", "he_uniform", "he_normal", "glorot_uniform", "glorot_normal",
                           "lecun_uniform", "lecun_normal", "random_uniform", "random_normal"), name="weight_initializer")
 ]
-opt_paras = {"name": "WOA", "epoch": 10, "pop_size": 20}
-model = MhaTuneRvfl(problem_type="regression", bounds=my_bounds, cv=3, scoring="MSE",
-                      optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True)
-```
-
-##### Supported functions in `model` object
-
-```python
-from graforvfl import RvflRegressor, Data 
-
-data = Data()       # Assumption that you have provided this object like above
 
-model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_uniform", trainer="OLS", alpha=0.5)
-
-## Train the model
+opt_paras = {"name": "WOA", "epoch": 10, "pop_size": 20}
+model = GfoRvflTuner(problem_type="classification", bounds=my_bounds, cv=3, scoring="AS",
+                      optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True, seed=42)
 model.fit(data.X_train, data.y_train)
-
-## Predicting a new result
-y_pred = model.predict(data.X_test)
-
-## Calculate metrics using score or scores functions.
-print(model.score(data.X_test, data.y_test, method="MAE"))
-print(model.scores(data.X_test, data.y_test, list_methods=["MAPE", "NNSE", "KGE", "MASE", "R2", "R", "R2S"]))
-
-## Calculate metrics using evaluate function
-print(model.evaluate(data.y_test, y_pred, list_metrics=("MSE", "RMSE", "MAPE", "NSE")))
-
-## Save performance metrics to csv file
-model.save_metrics(data.y_test, y_pred, list_metrics=("RMSE", "MAE"), save_path="history", filename="metrics.csv")
-
-## Save training loss to csv file
-model.save_loss_train(save_path="history", filename="loss.csv")
-
-## Save predicted label
-model.save_y_predicted(X=data.X_test, y_true=data.y_test, save_path="history", filename="y_predicted.csv")
-
-## Save model
-model.save_model(save_path="history", filename="traditional_mlp.pkl")
-
-## Load model 
-trained_model = RvflRegressor.load_model(load_path="history", filename="traditional_mlp.pkl")
+print(model.best_params)
+print(model.best_estimator)
+print(model.best_estimator.scores(data.X_test, data.y_test, list_methods=("PS", "RS", "NPV", "F1S", "F2S")))
 ```
 
-# Support (questions, problems)
+# Official channels 
+
+* [Official source code repository](https://github.com/thieu1995/GrafoRVFL)
+* [Official document](https://graforvfl.readthedocs.io/)
+* [Download releases](https://pypi.org/project/graforvfl/) 
+* [Issue tracker](https://github.com/thieu1995/GrafoRVFL/issues) 
+* [Notable changes log](/ChangeLog.md)
+* [Official discussion group](https://t.me/+fRVCJGuGJg1mNDg1)
 
-### Official Links 
+---
 
-* Official source code repo: https://github.com/thieu1995/GrafoRVFL
-* Official document: https://graforvfl.readthedocs.io/
-* Download releases: https://pypi.org/project/graforvfl/
-* Issue tracker: https://github.com/thieu1995/GrafoRVFL/issues
-* Notable changes log: https://github.com/thieu1995/GrafoRVFL/blob/main/ChangeLog.md
-* Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
-
-* This project also related to our another projects which are "optimization" and "machine learning", check it here:
-    * https://github.com/thieu1995/mealpy
-    * https://github.com/thieu1995/metaheuristics
-    * https://github.com/thieu1995/opfunu
-    * https://github.com/thieu1995/enoppy
-    * https://github.com/thieu1995/permetrics
-    * https://github.com/thieu1995/MetaCluster
-    * https://github.com/thieu1995/pfevaluator
-    * https://github.com/thieu1995/IntelELM
-    * https://github.com/thieu1995/reflame
-    * https://github.com/thieu1995/MetaPerceptron
-    * https://github.com/aiir-team
+Developed by: [Thieu](mailto:nguyenthieu2102@gmail.com?Subject=GrafoRVFL_QUESTIONS) @ 2023
```

### Comparing `graforvfl-1.0.0/graforvfl.egg-info/SOURCES.txt` & `graforvfl-1.1.0/graforvfl.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 graforvfl.egg-info/PKG-INFO
 graforvfl.egg-info/SOURCES.txt
 graforvfl.egg-info/dependency_links.txt
 graforvfl.egg-info/requires.txt
 graforvfl.egg-info/top_level.txt
 graforvfl/network/__init__.py
 graforvfl/network/base_rvfl.py
-graforvfl/network/mha_tune_rvfl.py
+graforvfl/network/gfo_rvfl_tuner.py
 graforvfl/network/standard_rvfl.py
 graforvfl/shared/__init__.py
 graforvfl/shared/activator.py
 graforvfl/shared/boundary_controller.py
 graforvfl/shared/data_processor.py
 graforvfl/shared/randomer.py
 graforvfl/shared/scaler.py
 graforvfl/shared/scorer.py
-tests/test_MhaTuneRvfl.py
+tests/test_GfoRvflTuner.py
 tests/test_RvflClassifier.py
 tests/test_RvflRegressor.py
```

### Comparing `graforvfl-1.0.0/setup.py` & `graforvfl-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="graforvfl",
-    version="1.0.0",
+    version="1.1.0",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
-    description="GrafoRVFL: A Python Library for Maximizing Performance of Random Vector Functional Link Network with Gradient-Free Optimization",
+    description="GrafoRVFL: A Gradient-Free Optimization Framework for Boosting Random Vector Functional Link Network",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["random vector functional link", "machine learning", "artificial intelligence",
               "deep learning", "neural networks", "single hidden layer network",
               "random projection", "RVFL", "feed-forward neural network", "artificial neural network",
               "classification", "regression", "supervised learning", "online learning", "generalization",
               "optimization algorithms", "Kernel RVFL", "Cross-validation"
@@ -67,13 +67,13 @@
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
     install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2",
-                      "pandas>=1.3.5", "mealpy>=3.0.1", "permetrics>=1.5.0"],
+                      "pandas>=1.3.5", "mealpy>=3.0.1", "permetrics>=2.0.0"],
     extras_require={
         "dev": ["pytest>=7.0", "pytest-cov==4.0.0", "flake8>=4.0.1"],
     },
     python_requires='>=3.8',
 )
```

### Comparing `graforvfl-1.0.0/tests/test_MhaTuneRvfl.py` & `graforvfl-1.1.0/tests/test_GfoRvflTuner.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 # Created by "Thieu" at 15:45, 15/08/2023 ----------%
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy import IntegerVar, StringVar
-from graforvfl import MhaTuneRvfl
+from graforvfl import GfoRvflTuner
 
 np.random.seed(42)
 
 
-def test_MhaTuneRvfl_class():
+def test_GfoRvflTuner_class():
     X = np.random.uniform(low=0.0, high=1.0, size=(100, 5))
     noise = np.random.normal(loc=0.0, scale=0.1, size=(100, 5))
     y = 2 * X + 1 + noise
 
     # Design the boundary (parameters)
     my_bounds = [
         IntegerVar(lb=2, ub=1000, name="size_hidden"),
         StringVar(valid_sets=("none", "relu", "leaky_relu", "celu", "prelu", "gelu",
                               "elu", "selu", "rrelu", "tanh", "sigmoid"), name="act_name"),
         StringVar(valid_sets=("orthogonal", "he_uniform", "he_normal", "glorot_uniform", "glorot_normal",
                               "lecun_uniform", "lecun_normal", "random_uniform", "random_normal"), name="weight_initializer")
     ]
 
     opt_paras = {"name": "WOA", "epoch": 5, "pop_size": 10}
-    model = MhaTuneRvfl(problem_type="regression", bounds=my_bounds, cv=3, scoring="MSE",
-                        optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True)
+    model = GfoRvflTuner(problem_type="regression", bounds=my_bounds, cv=3, scoring="MSE",
+                         optimizer="OriginalWOA", optimizer_paras=opt_paras, seed=42, verbose=True)
     model.fit(X, y)
     print(model.best_params)
     print(model.best_estimator)
 
     pred = model.predict(X)
-    assert MhaTuneRvfl.SUPPORTED_CLS_METRICS == model.SUPPORTED_CLS_METRICS
+    assert GfoRvflTuner.SUPPORTED_CLS_METRICS == model.SUPPORTED_CLS_METRICS
     assert len(pred) == X.shape[0]
```

### Comparing `graforvfl-1.0.0/tests/test_RvflClassifier.py` & `graforvfl-1.1.0/tests/test_RvflClassifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from graforvfl import RvflClassifier
 
-np.random.seed(41)
+np.random.seed(42)
 
 
 def test_RvflClassifier_class():
     X = np.random.rand(100, 6)
     y = np.random.randint(0, 2, size=100)
 
-    model = RvflClassifier(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI")
+    model = RvflClassifier(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI", seed=42)
     model.fit(X, y)
     pred = model.predict(X)
     assert RvflClassifier.SUPPORTED_CLS_METRICS == model.SUPPORTED_CLS_METRICS
     assert pred[0] in (0, 1)
```

### Comparing `graforvfl-1.0.0/tests/test_RvflRegressor.py` & `graforvfl-1.1.0/tests/test_RvflRegressor.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from graforvfl import RvflRegressor
 
-np.random.seed(41)
+np.random.seed(42)
 
 
 def test_RvflRegressor_class():
     X = np.random.rand(100, 6)
     y = np.random.randint(0, 2, size=100)
 
-    model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI")
+    model = RvflRegressor(size_hidden=10, act_name='sigmoid', weight_initializer="random_normal", trainer="MPI", seed=42)
     model.fit(X, y)
     pred = model.predict(X)
     assert RvflRegressor.SUPPORTED_CLS_METRICS == model.SUPPORTED_CLS_METRICS
     assert len(pred) == X.shape[0]
```

