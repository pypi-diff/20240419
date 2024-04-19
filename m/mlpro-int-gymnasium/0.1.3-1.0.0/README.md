# Comparing `tmp/mlpro-int-gymnasium-0.1.3.tar.gz` & `tmp/mlpro_int_gymnasium-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-int-gymnasium-0.1.3.tar", last modified: Mon Apr  1 20:09:41 2024, max compression
+gzip compressed data, was "mlpro_int_gymnasium-1.0.0.tar", last modified: Fri Apr 19 05:21:26 2024, max compression
```

## Comparing `mlpro-int-gymnasium-0.1.3.tar` & `mlpro_int_gymnasium-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.963914 mlpro-int-gymnasium-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-01 20:09:41.963914 mlpro-int-gymnasium-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 20:09:41.963914 mlpro-int-gymnasium-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.955914 mlpro-int-gymnasium-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/multicartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/multicartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.721201 mlpro_int_gymnasium-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/multicartpole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/multicartpole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22969 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/test/test_examples.py
```

### Comparing `mlpro-int-gymnasium-0.1.3/LICENSE` & `mlpro_int_gymnasium-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.3/PKG-INFO` & `mlpro_int_gymnasium-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-gymnasium
-Version: 0.1.3
+Version: 1.0.0
 Summary: MLPro: Integration Gymnasium
 Home-page: https://mlpro-int-gymnasium.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-gymnasium.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
 Requires-Dist: gymnasium[all]>=0.29; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-Gymnasium/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-Gymnasium/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-gymnasium/badge/?version=latest)](https://mlpro-int-gymnasium.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-gymnasium.svg)](https://badge.fury.io/py/mlpro-int-gymnasium)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-gymnasium/mlpro-int-gymnasium/badges/version.svg)](https://anaconda.org/mlpro-int-gymnasium/mlpro)
```

### Comparing `mlpro-int-gymnasium-0.1.3/README.md` & `mlpro_int_gymnasium-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.3/setup.cfg` & `mlpro_int_gymnasium-1.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-gymnasium
-version = 0.1.3
+version = 1.0.0
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration Gymnasium
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-gymnasium.readthedocs.io
 project_urls = 
@@ -22,14 +22,14 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
-	mlpro[full]>=1.3.1
+	mlpro[full]>=1.4.0
 	gymnasium[all]>=0.29
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/multicartpole.py` & `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/multicartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/multicartpole.py` & `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/multicartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/basics.py` & `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-04-09  0.0.0     MRD      Copied from openai_gym wrapper
 ## -- 2023-04-10  1.0.0     MRD      First Release 
 ## -- 2023-04-19  1.0.1     MRD      Refactor reset function
 ## -- 2023-08-21  1.0.2     MRD      Saving the seed in variable self._p_seed
 ## -- 2024-02-16  1.0.3     SY       Relocation from MLPro to MLPro-Int-Gymnasium
+## -- 2024-04-19  1.0.4     DA       Alignment with MLPro 1.4.0
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.3 (2024-02-16)
+Ver. 1.0.4 (2024-04-19)
 
 This module provides wrapper classes for Gym environments from Farama-Foundation Gymnasium.
 
 See also: https://github.com/Farama-Foundation/Gymnasium
 
 """
 
 import gymnasium as gym
-from mlpro.wrappers.models import Wrapper
+from mlpro.wrappers import Wrapper
 from mlpro.rl import *
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
```

### Comparing `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/PKG-INFO` & `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-gymnasium
-Version: 0.1.3
+Version: 1.0.0
 Summary: MLPro: Integration Gymnasium
 Home-page: https://mlpro-int-gymnasium.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-gymnasium.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
 Requires-Dist: gymnasium[all]>=0.29; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-Gymnasium/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-Gymnasium/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-gymnasium/badge/?version=latest)](https://mlpro-int-gymnasium.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-gymnasium.svg)](https://badge.fury.io/py/mlpro-int-gymnasium)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-gymnasium/mlpro-int-gymnasium/badges/version.svg)](https://anaconda.org/mlpro-int-gymnasium/mlpro)
```

### Comparing `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/SOURCES.txt` & `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.3/test/test_environment.py` & `mlpro_int_gymnasium-1.0.0/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.3/test/test_examples.py` & `mlpro_int_gymnasium-1.0.0/test/test_examples.py`

 * *Files identical despite different names*

