# Comparing `tmp/synthx-0.3.0.tar.gz` & `tmp/synthx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-0.3.0.tar", max compression
+gzip compressed data, was "synthx-0.3.1.tar", max compression
```

## Comparing `synthx-0.3.0.tar` & `synthx-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7163 2024-03-25 15:42:05.698171 synthx-0.3.0/README.md
--rw-r--r--   0        0        0     1193 2024-04-18 01:36:31.290268 synthx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      371 2024-03-25 05:20:00.886950 synthx-0.3.0/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.3.0/synthx/core/__init__.py
--rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.3.0/synthx/core/dataset.py
--rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.3.0/synthx/core/result.py
--rw-r--r--   0        0        0     7004 2024-04-18 01:31:14.755420 synthx-0.3.0/synthx/core/sample.py
--rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.3.0/synthx/errors/__init__.py
--rw-r--r--   0        0        0     5975 2024-03-25 05:20:00.887250 synthx-0.3.0/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.3.0/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.3.0/synthx/stats/norm.py
--rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.3.0/synthx/stats/p.py
--rw-r--r--   0        0        0     7870 1970-01-01 00:00:00.000000 synthx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7163 2024-03-25 15:42:05.698171 synthx-0.3.1/README.md
+-rw-r--r--   0        0        0     1242 2024-04-19 06:33:17.570540 synthx-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-03-25 05:20:00.886950 synthx-0.3.1/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.3.1/synthx/core/__init__.py
+-rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.3.1/synthx/core/dataset.py
+-rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.3.1/synthx/core/result.py
+-rw-r--r--   0        0        0     7004 2024-04-18 01:31:14.755420 synthx-0.3.1/synthx/core/sample.py
+-rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.3.1/synthx/errors/__init__.py
+-rw-r--r--   0        0        0     6003 2024-04-19 06:33:17.570783 synthx-0.3.1/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.3.1/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.3.1/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.3.1/synthx/stats/p.py
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 synthx-0.3.1/PKG-INFO
```

### Comparing `synthx-0.3.0/README.md` & `synthx-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `synthx-0.3.0/pyproject.toml` & `synthx-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [tool.poetry]
 name = "synthx"
-version = "0.3.0"
+version = "0.3.1"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.26.4"
 pandas = "^2.2.1"
 polars = "^0.20.16"
 scipy = "^1.12.0"
 matplotlib = "^3.8.3"
+tqdm = "^4.66.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = {extras = ["pyproject"], version = "^5.13.2"}
 black = "^24.3.0"
 pylint = "^3.1.0"
 mypy = "^1.9.0"
 bandit = "^1.7.8"
 pytest = "^8.1.1"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.14.0"
 notebook = "^7.1.2"
+types-tqdm = "^4.66.0.20240417"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.isort]
```

### Comparing `synthx-0.3.0/synthx/core/dataset.py` & `synthx-0.3.1/synthx/core/dataset.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.0/synthx/core/result.py` & `synthx-0.3.1/synthx/core/result.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.0/synthx/core/sample.py` & `synthx-0.3.1/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.0/synthx/errors/__init__.py` & `synthx-0.3.1/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.0/synthx/method.py` & `synthx-0.3.1/synthx/method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Synthetic Control Method."""
 
 import numpy as np
 import scipy.optimize
+from tqdm import tqdm
 
 import synthx as sx
 from synthx.errors import NoFeasibleModelError
 
 
 def synthetic_control(dataset: sx.Dataset) -> sx.SyntheticControlResult:
     """Perform synthetic control analysis on the given dataset.
@@ -120,15 +121,15 @@
         dataset.data.filter(~dataset.data[dataset.unit_column].is_in(dataset.intervention_units))[
             dataset.unit_column
         ]
         .unique()
         .to_list()
     )
     df_placebo = dataset.data.filter(dataset.data[dataset.unit_column].is_in(control_units))
-    for test_unit_placebo in control_units:
+    for test_unit_placebo in tqdm(control_units):
         dataset_placebo = sx.Dataset(
             df_placebo,
             unit_column=dataset.unit_column,
             time_column=dataset.time_column,
             y_column=dataset.y_column,
             covariate_columns=dataset.covariate_columns,
             intervention_units=test_unit_placebo,
```

### Comparing `synthx-0.3.0/synthx/stats/norm.py` & `synthx-0.3.1/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.0/synthx/stats/p.py` & `synthx-0.3.1/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.0/PKG-INFO` & `synthx-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: polars (>=0.20.16,<0.21.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # synthx
 SynthX: A Python Library for Advanced Synthetic Control Analysis
 
 [![python code sanity check - lint](https://github.com/kenki931128/synthx/actions/workflows/python-code-lint.yaml/badge.svg)](https://github.com/kenki931128/synthx/actions/workflows/python-code-lint.yaml) [![python code sanity check - test](https://github.com/kenki931128/synthx/actions/workflows/python-code-test.yaml/badge.svg)](https://github.com/kenki931128/synthx/actions/workflows/python-code-test.yaml) [![PyPI Latest Release](https://img.shields.io/pypi/v/synthx.svg)](https://pypi.org/project/synthx/)
```

