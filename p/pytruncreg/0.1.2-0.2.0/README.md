# Comparing `tmp/pytruncreg-0.1.2.tar.gz` & `tmp/pytruncreg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytruncreg-0.1.2.tar", last modified: Wed Apr 10 13:17:39 2024, max compression
+gzip compressed data, was "pytruncreg-0.2.0.tar", last modified: Fri Apr 19 13:25:12 2024, max compression
```

## Comparing `pytruncreg-0.1.2.tar` & `pytruncreg-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 13:17:39.151037 pytruncreg-0.1.2/
--rw-r--r--   0 ryo766     (503) staff       (20)     1065 2024-04-10 02:46:05.000000 pytruncreg-0.1.2/LICENSE
--rw-r--r--   0 ryo766     (503) staff       (20)     2934 2024-04-10 13:17:39.150765 pytruncreg-0.1.2/PKG-INFO
--rw-r--r--   0 ryo766     (503) staff       (20)     2592 2024-04-10 02:46:05.000000 pytruncreg-0.1.2/README.md
-drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 13:17:39.148909 pytruncreg-0.1.2/pytruncreg/
--rw-r--r--   0 ryo766     (503) staff       (20)       58 2024-04-10 13:16:18.000000 pytruncreg-0.1.2/pytruncreg/__init__.py
--rw-r--r--   0 ryo766     (503) staff       (20)     5709 2024-04-10 02:46:05.000000 pytruncreg-0.1.2/pytruncreg/truncreg.py
-drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 13:17:39.150434 pytruncreg-0.1.2/pytruncreg.egg-info/
--rw-r--r--   0 ryo766     (503) staff       (20)     2934 2024-04-10 13:17:39.000000 pytruncreg-0.1.2/pytruncreg.egg-info/PKG-INFO
--rw-r--r--   0 ryo766     (503) staff       (20)      241 2024-04-10 13:17:39.000000 pytruncreg-0.1.2/pytruncreg.egg-info/SOURCES.txt
--rw-r--r--   0 ryo766     (503) staff       (20)        1 2024-04-10 13:17:39.000000 pytruncreg-0.1.2/pytruncreg.egg-info/dependency_links.txt
--rw-r--r--   0 ryo766     (503) staff       (20)       19 2024-04-10 13:17:39.000000 pytruncreg-0.1.2/pytruncreg.egg-info/requires.txt
--rw-r--r--   0 ryo766     (503) staff       (20)       11 2024-04-10 13:17:39.000000 pytruncreg-0.1.2/pytruncreg.egg-info/top_level.txt
--rw-r--r--   0 ryo766     (503) staff       (20)       38 2024-04-10 13:17:39.151098 pytruncreg-0.1.2/setup.cfg
--rw-r--r--   0 ryo766     (503) staff       (20)      489 2024-04-10 13:17:07.000000 pytruncreg-0.1.2/setup.py
+drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-19 13:25:12.180367 pytruncreg-0.2.0/
+-rw-r--r--   0 ryo766     (503) staff       (20)     1101 2024-04-19 13:22:51.000000 pytruncreg-0.2.0/LICENSE
+-rw-r--r--   0 ryo766     (503) staff       (20)     3132 2024-04-19 13:25:12.180068 pytruncreg-0.2.0/PKG-INFO
+-rw-r--r--   0 ryo766     (503) staff       (20)     2790 2024-04-19 13:22:51.000000 pytruncreg-0.2.0/README.md
+drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-19 13:25:12.177296 pytruncreg-0.2.0/pytruncreg/
+-rw-r--r--   0 ryo766     (503) staff       (20)       58 2024-04-10 13:16:18.000000 pytruncreg-0.2.0/pytruncreg/__init__.py
+-rw-r--r--   0 ryo766     (503) staff       (20)     5709 2024-04-10 02:46:05.000000 pytruncreg-0.2.0/pytruncreg/truncreg.py
+drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-19 13:25:12.179615 pytruncreg-0.2.0/pytruncreg.egg-info/
+-rw-r--r--   0 ryo766     (503) staff       (20)     3132 2024-04-19 13:25:12.000000 pytruncreg-0.2.0/pytruncreg.egg-info/PKG-INFO
+-rw-r--r--   0 ryo766     (503) staff       (20)      241 2024-04-19 13:25:12.000000 pytruncreg-0.2.0/pytruncreg.egg-info/SOURCES.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)        1 2024-04-19 13:25:12.000000 pytruncreg-0.2.0/pytruncreg.egg-info/dependency_links.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)       19 2024-04-19 13:25:12.000000 pytruncreg-0.2.0/pytruncreg.egg-info/requires.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)       11 2024-04-19 13:25:12.000000 pytruncreg-0.2.0/pytruncreg.egg-info/top_level.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)       38 2024-04-19 13:25:12.180441 pytruncreg-0.2.0/setup.cfg
+-rw-r--r--   0 ryo766     (503) staff       (20)      489 2024-04-19 13:24:44.000000 pytruncreg-0.2.0/setup.py
```

### Comparing `pytruncreg-0.1.2/LICENSE` & `pytruncreg-0.2.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 CAUSALab
+Copyright (c) 2024 The President and Fellows of Harvard College
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytruncreg-0.1.2/PKG-INFO` & `pytruncreg-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pytruncreg
-Version: 0.1.2
+Version: 0.2.0
 Summary: Truncated Gaussian Regression Models
 Home-page: https://github.com/CausalInference/pytruncreg
 Author: Ryan ODea
 Author-email: ryanodea@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 
 # pytruncreg Overview
-The `truncreg` function is designed to estimate gaussian truncated regression models. The function requires `formula`, `data`, a truncation `point` and `direction` of truncation. This python package is a translation of the original `truncreg` R package [CRAN](https://cran.r-project.org/web/packages/truncreg/index.html) by Yves Croissant and Achim Zeileis.
+[![PyPI version](https://badge.fury.io/py/pytruncreg.svg)](https://pypi.org/project/pytruncreg) \
+The `pytruncreg` package developed by [Harvard University's CausaLab](https://causalab.sph.harvard.edu/) is designed to estimate one-way truncated gaussian regression models. The `truncreg` function requires `formula`, `data`, a truncation `point` and `direction` of truncation. This python package is a translation of the original `truncreg` R package [CRAN](https://cran.r-project.org/web/packages/truncreg/index.html) by Yves Croissant and Achim Zeileis.
 
 ## Parameters
 - **formula** (str): String describing the model to be fitted in format `y ~ x_1 + x_2 + ... x_n`
 - **data** (DataFrame): The dataset containing the variables specified in the formula
 - **point** (float): The point of truncation in `y`
 - **direction** (str): Specifies the direction of truncation, taking values `"left"` or `"right"`
 - **scaled** (bool, optional): Default is `False`. When set to `True` the model will use a scaled version of the dependent variable
```

### Comparing `pytruncreg-0.1.2/README.md` & `pytruncreg-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # pytruncreg Overview
-The `truncreg` function is designed to estimate gaussian truncated regression models. The function requires `formula`, `data`, a truncation `point` and `direction` of truncation. This python package is a translation of the original `truncreg` R package [CRAN](https://cran.r-project.org/web/packages/truncreg/index.html) by Yves Croissant and Achim Zeileis.
+[![PyPI version](https://badge.fury.io/py/pytruncreg.svg)](https://pypi.org/project/pytruncreg) \
+The `pytruncreg` package developed by [Harvard University's CausaLab](https://causalab.sph.harvard.edu/) is designed to estimate one-way truncated gaussian regression models. The `truncreg` function requires `formula`, `data`, a truncation `point` and `direction` of truncation. This python package is a translation of the original `truncreg` R package [CRAN](https://cran.r-project.org/web/packages/truncreg/index.html) by Yves Croissant and Achim Zeileis.
 
 ## Parameters
 - **formula** (str): String describing the model to be fitted in format `y ~ x_1 + x_2 + ... x_n`
 - **data** (DataFrame): The dataset containing the variables specified in the formula
 - **point** (float): The point of truncation in `y`
 - **direction** (str): Specifies the direction of truncation, taking values `"left"` or `"right"`
 - **scaled** (bool, optional): Default is `False`. When set to `True` the model will use a scaled version of the dependent variable
```

### Comparing `pytruncreg-0.1.2/pytruncreg/truncreg.py` & `pytruncreg-0.2.0/pytruncreg/truncreg.py`

 * *Files identical despite different names*

### Comparing `pytruncreg-0.1.2/pytruncreg.egg-info/PKG-INFO` & `pytruncreg-0.2.0/pytruncreg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pytruncreg
-Version: 0.1.2
+Version: 0.2.0
 Summary: Truncated Gaussian Regression Models
 Home-page: https://github.com/CausalInference/pytruncreg
 Author: Ryan ODea
 Author-email: ryanodea@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 
 # pytruncreg Overview
-The `truncreg` function is designed to estimate gaussian truncated regression models. The function requires `formula`, `data`, a truncation `point` and `direction` of truncation. This python package is a translation of the original `truncreg` R package [CRAN](https://cran.r-project.org/web/packages/truncreg/index.html) by Yves Croissant and Achim Zeileis.
+[![PyPI version](https://badge.fury.io/py/pytruncreg.svg)](https://pypi.org/project/pytruncreg) \
+The `pytruncreg` package developed by [Harvard University's CausaLab](https://causalab.sph.harvard.edu/) is designed to estimate one-way truncated gaussian regression models. The `truncreg` function requires `formula`, `data`, a truncation `point` and `direction` of truncation. This python package is a translation of the original `truncreg` R package [CRAN](https://cran.r-project.org/web/packages/truncreg/index.html) by Yves Croissant and Achim Zeileis.
 
 ## Parameters
 - **formula** (str): String describing the model to be fitted in format `y ~ x_1 + x_2 + ... x_n`
 - **data** (DataFrame): The dataset containing the variables specified in the formula
 - **point** (float): The point of truncation in `y`
 - **direction** (str): Specifies the direction of truncation, taking values `"left"` or `"right"`
 - **scaled** (bool, optional): Default is `False`. When set to `True` the model will use a scaled version of the dependent variable
```

