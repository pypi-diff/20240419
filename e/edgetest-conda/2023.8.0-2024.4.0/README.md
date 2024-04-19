# Comparing `tmp/edgetest-conda-2023.8.0.tar.gz` & `tmp/edgetest_conda-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-conda-2023.8.0.tar", last modified: Tue Aug 29 13:47:26 2023, max compression
+gzip compressed data, was "edgetest_conda-2024.4.0.tar", last modified: Fri Apr 19 17:27:27 2024, max compression
```

## Comparing `edgetest-conda-2023.8.0.tar` & `edgetest_conda-2024.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:47:26.038531 edgetest-conda-2023.8.0/
--rw-r--r--   0 runner    (1001) docker     (999)       59 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       56 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     3225 2023-08-29 13:47:26.038531 edgetest-conda-2023.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2048 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:47:26.038531 edgetest-conda-2023.8.0/edgetest_conda/
--rw-r--r--   0 runner    (1001) docker     (999)      324 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/edgetest_conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4440 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/edgetest_conda/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:47:26.038531 edgetest-conda-2023.8.0/edgetest_conda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3225 2023-08-29 13:47:26.000000 edgetest-conda-2023.8.0/edgetest_conda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      415 2023-08-29 13:47:26.000000 edgetest-conda-2023.8.0/edgetest_conda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 13:47:26.000000 edgetest-conda-2023.8.0/edgetest_conda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-29 13:47:26.000000 edgetest-conda-2023.8.0/edgetest_conda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 13:47:00.000000 edgetest-conda-2023.8.0/edgetest_conda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      374 2023-08-29 13:47:26.000000 edgetest-conda-2023.8.0/edgetest_conda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       21 2023-08-29 13:47:26.000000 edgetest-conda-2023.8.0/edgetest_conda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     2695 2023-08-29 13:47:26.038531 edgetest-conda-2023.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:47:26.038531 edgetest-conda-2023.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    11576 2023-08-29 13:46:57.000000 edgetest-conda-2023.8.0/tests/test_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:27:27.972528 edgetest_conda-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-19 17:27:27.972528 edgetest_conda-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:27:27.968528 edgetest_conda-2024.4.0/edgetest_conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/edgetest_conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/edgetest_conda/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:27:27.968528 edgetest_conda-2024.4.0/edgetest_conda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-19 17:27:27.000000 edgetest_conda-2024.4.0/edgetest_conda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 17:27:27.000000 edgetest_conda-2024.4.0/edgetest_conda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:27:27.000000 edgetest_conda-2024.4.0/edgetest_conda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 17:27:27.000000 edgetest_conda-2024.4.0/edgetest_conda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:27:07.000000 edgetest_conda-2024.4.0/edgetest_conda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-19 17:27:27.000000 edgetest_conda-2024.4.0/edgetest_conda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 17:27:27.000000 edgetest_conda-2024.4.0/edgetest_conda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-19 17:27:27.972528 edgetest_conda-2024.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:27:27.968528 edgetest_conda-2024.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-04-19 17:27:04.000000 edgetest_conda-2024.4.0/tests/test_hook.py
```

### Comparing `edgetest-conda-2023.8.0/LICENSE` & `edgetest_conda-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-conda-2023.8.0/PKG-INFO` & `edgetest_conda-2024.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: edgetest-conda
-Version: 2023.8.0
-Summary: Conda edgetest plugin
-Home-page: https://github.com/capitalone/edgetest-conda
-Author: Akshay Gupta
-Author-email: akshay.gupta2@capitalone.com
-Maintainer: Akshay Gupta
-Maintainer-email: akshay.gupta2@capitalone.com
-Project-URL: Documentation, https://capitalone.github.io/edgetest-conda
-Project-URL: Bug Tracker, https://github.com/capitalone/edgetest-conda/issues
-Project-URL: Source Code, https://github.com/capitalone/edgetest-conda
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: qa
-Provides-Extra: build
-Provides-Extra: dev
-License-File: LICENSE
-License-File: AUTHORS.md
-
 # Conda edgetest plugin
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edgetest-conda)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![PyPI version](https://badge.fury.io/py/edgetest-conda.svg)](https://badge.fury.io/py/edgetest-conda)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/edgetest-conda/badges/version.svg)](https://anaconda.org/conda-forge/edgetest-conda)
```

### Comparing `edgetest-conda-2023.8.0/edgetest_conda/plugin.py` & `edgetest_conda-2024.4.0/edgetest_conda/plugin.py`

 * *Files identical despite different names*

### Comparing `edgetest-conda-2023.8.0/setup.cfg` & `edgetest_conda-2024.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
-packages = find:
 install_requires = 
 	edgetest>=2022.3.0
 
 [options.extras_require]
 docs = 
 	furo
 	sphinx
```

### Comparing `edgetest-conda-2023.8.0/tests/test_hook.py` & `edgetest_conda-2024.4.0/tests/test_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 
 PIP_LIST_MAMBA = """
 [{"name": "myupgrade", "version": "0.2.0"}, {"name": "mamba", "version": "0.14.1"}]
 """
 
 TABLE_OUTPUT = """
 
-=============  ===============  ===================  =================
-Environment    Passing tests    Upgraded packages    Package version
-=============  ===============  ===================  =================
-myenv          True             myupgrade            0.2.0
-=============  ===============  ===================  =================
+=============  ==================  ===============  ===================  ==================  =================
+Environment    Setup successful    Passing tests    Upgraded packages    Lowered packages    Package version
+=============  ==================  ===============  ===================  ==================  =================
+myenv          True                True             myupgrade                                0.2.0
+=============  ==================  ===============  ===================  ==================  =================
 """
 
 
 @pytest.mark.parametrize("config", [CFG, CFG_NOCONDA])
 def test_addoption(config, tmpdir):
     """Test the addoption hook."""
     location = tmpdir.mkdir("mylocation")
```

