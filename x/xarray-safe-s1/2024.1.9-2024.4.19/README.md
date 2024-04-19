# Comparing `tmp/xarray-safe-s1-2024.1.9.tar.gz` & `tmp/xarray_safe_s1-2024.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-safe-s1-2024.1.9.tar", last modified: Tue Jan  9 08:51:40 2024, max compression
+gzip compressed data, was "xarray_safe_s1-2024.4.19.tar", last modified: Fri Apr 19 08:32:16 2024, max compression
```

## Comparing `xarray-safe-s1-2024.1.9.tar` & `xarray_safe_s1-2024.4.19.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.519079 xarray-safe-s1-2024.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.511079 xarray-safe-s1-2024.1.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.511079 xarray-safe-s1-2024.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-01-09 08:51:40.515079 xarray-safe-s1-2024.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.511079 xarray-safe-s1-2024.1.9/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.511079 xarray-safe-s1-2024.1.9/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.515079 xarray-safe-s1-2024.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.511079 xarray-safe-s1-2024.1.9/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.515079 xarray-safe-s1-2024.1.9/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/_static/css/xsar.css
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.515079 xarray-safe-s1-2024.1.9/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/examples/simple_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.515079 xarray-safe-s1-2024.1.9/safe_s1/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/safe_s1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/safe_s1/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    28885 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/safe_s1/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    52504 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/safe_s1/sentinel1_xml_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/safe_s1/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 08:51:40.519079 xarray-safe-s1-2024.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.515079 xarray-safe-s1-2024.1.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-01-09 08:51:19.000000 xarray-safe-s1-2024.1.9/test/test_s1reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:51:40.515079 xarray-safe-s1-2024.1.9/xarray_safe_s1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-01-09 08:51:40.000000 xarray-safe-s1-2024.1.9/xarray_safe_s1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-01-09 08:51:40.000000 xarray-safe-s1-2024.1.9/xarray_safe_s1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 08:51:40.000000 xarray-safe-s1-2024.1.9/xarray_safe_s1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-09 08:51:40.000000 xarray-safe-s1-2024.1.9/xarray_safe_s1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 08:51:40.000000 xarray-safe-s1-2024.1.9/xarray_safe_s1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.091180 xarray_safe_s1-2024.4.19/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.091180 xarray_safe_s1-2024.4.19/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.091180 xarray_safe_s1-2024.4.19/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.091180 xarray_safe_s1-2024.4.19/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.091180 xarray_safe_s1-2024.4.19/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/_static/css/xsar.css
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/examples/simple_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/highleveltests/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/highleveltests/open_SLC_IW.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/highleveltests/open_SLC_IW_S3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/safe_s1/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/safe_s1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/safe_s1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/safe_s1/getconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28974 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/safe_s1/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52508 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/safe_s1/sentinel1_xml_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/safe_s1/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-19 08:32:04.000000 xarray_safe_s1-2024.4.19/test/test_s1reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:32:16.095180 xarray_safe_s1-2024.4.19/xarray_safe_s1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-19 08:32:16.000000 xarray_safe_s1-2024.4.19/xarray_safe_s1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-19 08:32:16.000000 xarray_safe_s1-2024.4.19/xarray_safe_s1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:32:16.000000 xarray_safe_s1-2024.4.19/xarray_safe_s1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 08:32:16.000000 xarray_safe_s1-2024.4.19/xarray_safe_s1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 08:32:16.000000 xarray_safe_s1-2024.4.19/xarray_safe_s1.egg-info/top_level.txt
```

### Comparing `xarray-safe-s1-2024.1.9/.github/workflows/publish.yml` & `xarray_safe_s1-2024.4.19/.github/workflows/publish.yml`

 * *Files 20% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         run: |
           python -m build --sdist --wheel .
       - name: Check the built archives
         run: |
           twine check dist/*
           pip install dist/*.whl
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@2f6f737ca5f74c637829c0f5c3acd0e29ea5e8bf
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
         with:
           password: ${{ secrets.pypi_token }}
           repository_url: https://upload.pypi.org/legacy/
           verify_metadata: true
```

### Comparing `xarray-safe-s1-2024.1.9/.pre-commit-config.yaml` & `xarray_safe_s1-2024.4.19/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/LICENSE` & `xarray_safe_s1-2024.4.19/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/PKG-INFO` & `xarray_safe_s1-2024.4.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2024.1.9
+Version: 2024.4.19
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `xarray-safe-s1-2024.1.9/README.md` & `xarray_safe_s1-2024.4.19/README.md`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/ci/requirements/environment.yaml` & `xarray_safe_s1-2024.4.19/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/docs/Makefile` & `xarray_safe_s1-2024.4.19/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/docs/conf.py` & `xarray_safe_s1-2024.4.19/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/docs/examples/simple_tutorial.ipynb` & `xarray_safe_s1-2024.4.19/docs/examples/simple_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/docs/index.rst` & `xarray_safe_s1-2024.4.19/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/docs/installing.rst` & `xarray_safe_s1-2024.4.19/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/docs/make.bat` & `xarray_safe_s1-2024.4.19/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/pyproject.toml` & `xarray_safe_s1-2024.4.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/safe_s1/metadata.py` & `xarray_safe_s1-2024.4.19/safe_s1/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-
+import pdb
 import dask
 import fsspec
 import numpy as np
 import rasterio
 import yaml
 from affine import Affine
 from rioxarray import rioxarray
@@ -17,15 +17,15 @@
 import warnings
 
 
 class Sentinel1Reader:
 
     def __init__(self, name, backend_kwargs=None):
         if not isinstance(name, (str, os.PathLike)):
-            raise ValueError(f"cannot deal with object of type {type(name)}: {name}")
+           raise ValueError(f"cannot deal with object of type {type(name)}: {name}")
         # gdal dataset name
         if not name.startswith('SENTINEL1_DS:'):
             name = 'SENTINEL1_DS:%s:' % name
         self.name = name
         """Gdal dataset name"""
         name_parts = self.name.split(':')
         if len(name_parts) > 3:
@@ -35,18 +35,21 @@
         name_parts[1] = os.path.basename(name_parts[1])
         self.short_name = ':'.join(name_parts)
         """Like name, but without path"""
         self.path = ':'.join(self.name.split(':')[1:-1])
         """Dataset path"""
         self.safe = os.path.basename(self.path)
 
+        self.path = os.fspath(self.path)
+
         if backend_kwargs is None:
             backend_kwargs = {}
-        self.path = os.fspath(self.path)
+
         storage_options = backend_kwargs.get("storage_options", {})
+
         mapper = fsspec.get_mapper(self.path, **storage_options)
         self.xml_parser = XmlParser(
             xpath_mappings=sentinel1_xml_mappings.xpath_mappings,
             compounds_vars=sentinel1_xml_mappings.compounds_vars,
             namespaces=sentinel1_xml_mappings.namespaces,
             mapper=mapper
         )
@@ -85,15 +88,14 @@
             self._multidataset = True
 
         self.dt = None
         self._dict = {
             'geolocationGrid': None,
         }
         if not self.multidataset:
-
             self._dict = {
                 'geolocationGrid': self.geoloc,
                 'orbit': self.orbit,
                 'image': self.image,
                 'azimuth_fmrate': self.azimuth_fmrate,
                 'doppler_estimate': self.doppler_estimate,
                 'bursts': self.bursts,
@@ -101,14 +103,17 @@
                 'noise_azimuth_raw': self.get_noise_azi_raw,
                 'noise_range_raw': self.get_noise_range_raw,
                 'antenna_pattern':self.antenna_pattern,
                 'swath_merging': self.swath_merging
             }
             self.dt = datatree.DataTree.from_dict(self._dict)
             assert self.dt==self.datatree
+        else:
+            print('multidataset')
+            raise Exception()
 
     def load_digital_number(self, resolution=None, chunks=None, resampling=rasterio.enums.Resampling.rms):
         """
         load digital_number from self.sar_meta.files['measurement'], as an `xarray.Dataset`.
 
         Parameters
         ----------
```

### Comparing `xarray-safe-s1-2024.1.9/safe_s1/sentinel1_xml_mappings.py` & `xarray_safe_s1-2024.4.19/safe_s1/sentinel1_xml_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
     )
     return df
 
 
 def xsd_files_func(xsd_product_file):
     """
     return a xarray Dataset with path of the different xsd files
-    :param xsd_product:
+    :param xsd_product: str
     :return:
     """
     ds = xr.Dataset()
 
     ds['xsd_product'] = xarray.DataArray(xsd_product_file)
     return ds
```

### Comparing `xarray-safe-s1-2024.1.9/safe_s1/xml_parser.py` & `xarray_safe_s1-2024.4.19/safe_s1/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2024.1.9/xarray_safe_s1.egg-info/PKG-INFO` & `xarray_safe_s1-2024.4.19/xarray_safe_s1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2024.1.9
+Version: 2024.4.19
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: numpy
 Requires-Dist: xarray
```

