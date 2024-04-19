# Comparing `tmp/mlpro-int-pettingzoo-0.1.0.tar.gz` & `tmp/mlpro_int_pettingzoo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-int-pettingzoo-0.1.0.tar", last modified: Sat Feb 24 21:39:28 2024, max compression
+gzip compressed data, was "mlpro_int_pettingzoo-1.0.0.tar", last modified: Fri Apr 19 08:01:27 2024, max compression
```

## Comparing `mlpro-int-pettingzoo-0.1.0.tar` & `mlpro_int_pettingzoo-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 21:39:28.976516 mlpro-int-pettingzoo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-02-24 21:39:22.000000 mlpro-int-pettingzoo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-02-24 21:39:28.976516 mlpro-int-pettingzoo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-24 21:39:22.000000 mlpro-int-pettingzoo-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-24 21:39:22.000000 mlpro-int-pettingzoo-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-24 21:39:28.976516 mlpro-int-pettingzoo-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 21:39:28.972516 mlpro-int-pettingzoo-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 21:39:28.972516 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 21:39:22.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 21:39:28.976516 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-24 21:39:22.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23043 2024-02-24 21:39:22.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo/wrappers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 21:39:28.976516 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-02-24 21:39:28.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-24 21:39:28.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 21:39:28.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-24 21:39:28.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-24 21:39:28.000000 mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 21:39:28.976516 mlpro-int-pettingzoo-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-02-24 21:39:22.000000 mlpro-int-pettingzoo-0.1.0/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:27.669988 mlpro_int_pettingzoo-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-19 08:01:22.000000 mlpro_int_pettingzoo-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-19 08:01:27.669988 mlpro_int_pettingzoo-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-19 08:01:22.000000 mlpro_int_pettingzoo-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 08:01:22.000000 mlpro_int_pettingzoo-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 08:01:27.669988 mlpro_int_pettingzoo-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:27.665988 mlpro_int_pettingzoo-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:27.669988 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 08:01:22.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:27.669988 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 08:01:22.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23100 2024-04-19 08:01:22.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:27.669988 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-19 08:01:27.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-19 08:01:27.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:01:27.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 08:01:27.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 08:01:27.000000 mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:01:27.669988 mlpro_int_pettingzoo-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-19 08:01:22.000000 mlpro_int_pettingzoo-1.0.0/test/test_examples.py
```

### Comparing `mlpro-int-pettingzoo-0.1.0/LICENSE` & `mlpro_int_pettingzoo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-int-pettingzoo-0.1.0/PKG-INFO` & `mlpro_int_pettingzoo-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mlpro-int-pettingzoo
-Version: 0.1.0
+Version: 1.0.0
 Summary: MLPro: Integration PettingZoo
 Home-page: https://mlpro-int-pettingzoo.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-pettingzoo.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
-Requires-Dist: pettingzoo>=1.22.3; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
 Requires-Dist: pygame>=2.1.3; extra == "full"
 Requires-Dist: pymunk>=6.4.0; extra == "full"
+Requires-Dist: pettingzoo>=1.22.3; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-PettingZoo/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-PettingZoo/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-pettingzoo/badge/?version=latest)](https://mlpro-int-pettingzoo.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-pettingzoo.svg)](https://badge.fury.io/py/mlpro-int-pettingzoo)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-pettingzoo/mlpro-int-pettingzoo/badges/version.svg)](https://anaconda.org/mlpro-int-pettingzoo/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro-int-pettingzoo/mlpro-int-pettingzoo?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro-int-pettingzoo/mlpro-int-pettingzoo)
```

### Comparing `mlpro-int-pettingzoo-0.1.0/README.md` & `mlpro_int_pettingzoo-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-int-pettingzoo-0.1.0/setup.cfg` & `mlpro_int_pettingzoo-1.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-pettingzoo
-version = 0.1.0
+version = 1.0.0
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration PettingZoo
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-pettingzoo.readthedocs.io
 project_urls = 
@@ -22,16 +22,16 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
-	mlpro[full]>=1.3.1
-	pettingzoo>=1.22.3
+	mlpro[full]>=1.4.0
 	pygame>=2.1.3
 	pymunk>=6.4.0
+	pettingzoo>=1.22.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo/wrappers/basics.py` & `mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo/wrappers/basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,30 +42,31 @@
 ## -- 2022-11-09  2.0.2     DA       Refactoring
 ## -- 2022-11-29  2.0.3     DA       Refactoring
 ## -- 2022-12-21  2.0.4     SY       Update _recognize_space due to howto_rl_wp_003
 ## -- 2023-02-21  2.1.0     DA       Class WrEnvPZOO2MLPro: specific implementations for load(), _save()
 ## -- 2023-03-26  2.2.0     DA       Class WrEnvPZOO2MLPro: refactoring of persistence
 ## -- 2024-01-23  2.3.0     SY       Debug due to introduction of PettingZoo version 1.24.3
 ## -- 2024-02-16  2.3.1     SY       Wrapper Relocation from MLPro to MLPro-Int-PettingZoo
+## -- 2024-04-19  2.4.0     DA       Alignment with MLPRO 1.4.0
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 2.3.1 (2024-02-16)
+Ver. 2.4.0 (2024-04-19)
 
 This module provides wrapper classes for PettingZoo multi-agent environments.
 
 See also: https://pypi.org/project/PettingZoo/
 
 """
 
 
 import gymnasium
 from pydoc import locate
 import numpy as np
-from mlpro.wrappers.models import Wrapper
+from mlpro.wrappers import Wrapper
 from mlpro.rl import *
 from pettingzoo import AECEnv
 from pettingzoo.utils import agent_selector
 from pettingzoo.utils import wrappers
```

### Comparing `mlpro-int-pettingzoo-0.1.0/src/mlpro_int_pettingzoo.egg-info/PKG-INFO` & `mlpro_int_pettingzoo-1.0.0/src/mlpro_int_pettingzoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mlpro-int-pettingzoo
-Version: 0.1.0
+Version: 1.0.0
 Summary: MLPro: Integration PettingZoo
 Home-page: https://mlpro-int-pettingzoo.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-pettingzoo.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
-Requires-Dist: pettingzoo>=1.22.3; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
 Requires-Dist: pygame>=2.1.3; extra == "full"
 Requires-Dist: pymunk>=6.4.0; extra == "full"
+Requires-Dist: pettingzoo>=1.22.3; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-PettingZoo/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-PettingZoo/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-pettingzoo/badge/?version=latest)](https://mlpro-int-pettingzoo.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-pettingzoo.svg)](https://badge.fury.io/py/mlpro-int-pettingzoo)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-pettingzoo/mlpro-int-pettingzoo/badges/version.svg)](https://anaconda.org/mlpro-int-pettingzoo/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro-int-pettingzoo/mlpro-int-pettingzoo?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro-int-pettingzoo/mlpro-int-pettingzoo)
```

### Comparing `mlpro-int-pettingzoo-0.1.0/test/test_examples.py` & `mlpro_int_pettingzoo-1.0.0/test/test_examples.py`

 * *Files identical despite different names*

