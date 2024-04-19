# Comparing `tmp/zodipy-0.9.0.tar.gz` & `tmp/zodipy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodipy-0.9.0.tar", max compression
+gzip compressed data, was "zodipy-0.9.1.tar", max compression
```

## Comparing `zodipy-0.9.0.tar` & `zodipy-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35148 2024-04-13 07:26:26.411863 zodipy-0.9.0/LICENSE
--rw-r--r--   0        0        0     5995 2024-04-13 09:11:02.454322 zodipy-0.9.0/README.md
--rw-r--r--   0        0        0     2244 2024-04-13 08:16:49.155424 zodipy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      276 2024-04-13 07:26:26.441718 zodipy-0.9.0/zodipy/__init__.py
--rw-r--r--   0        0        0     2826 2024-04-13 07:26:26.441950 zodipy-0.9.0/zodipy/_bandpass.py
--rw-r--r--   0        0        0      580 2024-04-13 07:26:26.442110 zodipy-0.9.0/zodipy/_constants.py
--rw-r--r--   0        0        0     1677 2024-04-13 07:26:26.442325 zodipy-0.9.0/zodipy/_contour.py
--rw-r--r--   0        0        0     2976 2024-04-13 07:26:26.442697 zodipy-0.9.0/zodipy/_emission.py
--rw-r--r--   0        0        0     4353 2024-04-13 07:26:26.442914 zodipy-0.9.0/zodipy/_interpolate_source.py
--rw-r--r--   0        0        0     4434 2024-04-13 07:26:26.443132 zodipy-0.9.0/zodipy/_ipd_comps.py
--rw-r--r--   0        0        0    15213 2024-04-13 08:34:40.194963 zodipy-0.9.0/zodipy/_ipd_dens_funcs.py
--rw-r--r--   0        0        0     2942 2024-04-13 07:26:26.443565 zodipy-0.9.0/zodipy/_ipd_model.py
--rw-r--r--   0        0        0     3248 2024-04-13 07:26:26.443729 zodipy-0.9.0/zodipy/_line_of_sight.py
--rw-r--r--   0        0        0     2297 2024-04-13 07:26:26.443909 zodipy-0.9.0/zodipy/_sky_coords.py
--rw-r--r--   0        0        0     2752 2024-04-13 07:26:26.444084 zodipy-0.9.0/zodipy/_source_funcs.py
--rw-r--r--   0        0        0      311 2024-04-13 07:26:26.444243 zodipy-0.9.0/zodipy/_types.py
--rw-r--r--   0        0        0      998 2024-04-13 07:26:26.444431 zodipy-0.9.0/zodipy/_unit_vectors.py
--rw-r--r--   0        0        0     3298 2024-04-13 07:26:26.444611 zodipy-0.9.0/zodipy/_validators.py
--rw-r--r--   0        0        0     4667 2024-04-13 07:26:26.444779 zodipy-0.9.0/zodipy/comps.py
--rw-r--r--   0        0        0     1997 2024-04-13 07:26:26.444939 zodipy-0.9.0/zodipy/model_registry.py
--rw-r--r--   0        0        0        0 2024-04-13 07:26:26.445008 zodipy-0.9.0/zodipy/py.typed
--rw-r--r--   0        0        0     6165 2024-04-13 07:26:26.445218 zodipy-0.9.0/zodipy/source_params.py
--rw-r--r--   0        0        0    24080 2024-04-13 07:26:26.445448 zodipy-0.9.0/zodipy/zodipy.py
--rw-r--r--   0        0        0     7061 1970-01-01 00:00:00.000000 zodipy-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-05-27 12:19:51.135025 zodipy-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5979 2024-04-19 07:14:30.048366 zodipy-0.9.1/README.md
+-rw-r--r--   0        0        0     2426 2024-04-19 07:43:16.564636 zodipy-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-03-21 02:36:07.680358 zodipy-0.9.1/zodipy/__init__.py
+-rw-r--r--   0        0        0     2826 2023-02-03 09:26:36.666633 zodipy-0.9.1/zodipy/_bandpass.py
+-rw-r--r--   0        0        0      580 2023-02-07 12:46:42.398482 zodipy-0.9.1/zodipy/_constants.py
+-rw-r--r--   0        0        0     1677 2023-02-03 09:26:36.669642 zodipy-0.9.1/zodipy/_contour.py
+-rw-r--r--   0        0        0     2976 2024-03-21 02:36:07.681352 zodipy-0.9.1/zodipy/_emission.py
+-rw-r--r--   0        0        0     4353 2024-03-21 02:36:07.682256 zodipy-0.9.1/zodipy/_interpolate_source.py
+-rw-r--r--   0        0        0     4434 2023-02-07 12:46:42.402979 zodipy-0.9.1/zodipy/_ipd_comps.py
+-rw-r--r--   0        0        0    15213 2024-04-16 10:58:46.677595 zodipy-0.9.1/zodipy/_ipd_dens_funcs.py
+-rw-r--r--   0        0        0     2942 2024-03-21 02:36:07.683943 zodipy-0.9.1/zodipy/_ipd_model.py
+-rw-r--r--   0        0        0     3248 2024-02-02 15:01:26.320632 zodipy-0.9.1/zodipy/_line_of_sight.py
+-rw-r--r--   0        0        0     2297 2024-03-21 02:36:07.685197 zodipy-0.9.1/zodipy/_sky_coords.py
+-rw-r--r--   0        0        0     2752 2024-04-19 07:06:17.490036 zodipy-0.9.1/zodipy/_source_funcs.py
+-rw-r--r--   0        0        0      311 2023-02-03 09:26:36.686612 zodipy-0.9.1/zodipy/_types.py
+-rw-r--r--   0        0        0      998 2023-02-03 09:26:36.688761 zodipy-0.9.1/zodipy/_unit_vectors.py
+-rw-r--r--   0        0        0     3298 2024-03-21 02:36:07.686171 zodipy-0.9.1/zodipy/_validators.py
+-rw-r--r--   0        0        0     4667 2023-09-15 08:50:24.694430 zodipy-0.9.1/zodipy/comps.py
+-rw-r--r--   0        0        0     1997 2023-09-15 08:50:24.696767 zodipy-0.9.1/zodipy/model_registry.py
+-rw-r--r--   0        0        0        0 2022-11-28 11:09:29.298004 zodipy-0.9.1/zodipy/py.typed
+-rw-r--r--   0        0        0     6165 2023-09-15 08:50:24.701308 zodipy-0.9.1/zodipy/source_params.py
+-rw-r--r--   0        0        0    24080 2024-03-22 13:59:45.674281 zodipy-0.9.1/zodipy/zodipy.py
+-rw-r--r--   0        0        0     7143 1970-01-01 00:00:00.000000 zodipy-0.9.1/PKG-INFO
```

### Comparing `zodipy-0.9.0/LICENSE` & `zodipy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/README.md` & `zodipy-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 Note that developers using Python 3.12 will need to upgrade their pip versions with `python3 -m pip install --upgrade pip` before being able to install ZodiPy. This is due to known incompatibilities between older pip versions and Python 3.12
 
 ## Tests, linting and formatting
 The following tools should be run from the root of the repository with no errors. (These are ran automatically as part of the CI workflows on GitHub, but should be tested locally first)
 
 - [pytest](https://docs.pytest.org/en/8.0.x/): Tests are run with pytest by simply running `pytest` in the command line in the root of the repository. 
-- [ruff](https://github.com/astral-sh/ruff): Formating and linting is done with `ruff` by simply running `ruff check zodipy/` and `ruff format zodipy/` in the command line in the root of the repository. 
+- [ruff](https://github.com/astral-sh/ruff): Formating and linting is done with `ruff` by simply running `ruff check` and `ruff format` in the command line in the root of the repository. 
 - [mypy](https://mypy-lang.org/): Type checking is done with `mypy` by simply running `mypy zodipy/` in the root of the repository.
 
 Remeber to add tests when implementing new features to maintain a high code coverage.
 
 ## Documentation
 We use [MkDocs](https://www.mkdocs.org/) to create our documentation. The documentation is built locally with `mkdocs build` from the repository root, and served with `mkdocs serve`.
```

### Comparing `zodipy-0.9.0/pyproject.toml` & `zodipy-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 [tool.poetry]
 name = "zodipy"
-homepage = "https://github.com/Cosmoglobe/zodipy"
-version = "0.9.0"
+version = "0.9.1"
 description = "Software for simulating zodiacal emission"
 authors = ["Metin San <metinisan@gmail.com>"]
 readme = "README.md"
-license = "GPL-3.0"
-exclude = ["test.py"]
+license = "GPL-3.0-or-later"
 classifiers = [
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Physics",
@@ -18,15 +16,19 @@
 keywords = [
     "astronomy",
     "astrophysics",
     "cosmology",
     "space",
     "science",
 ]
+exclude = ["test.py"]
 
+[tool.poetry.urls]
+documentation = "https://cosmoglobe.github.io/zodipy/"
+repository = "https://github.com/cosmoglobe/zodipy"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 numpy = "^1.26.4"
 healpy = "^1.16.6"
 astropy = ">=5.0.1"
 jplephem = "^2.17"
@@ -44,15 +46,14 @@
 mkdocs-material = "^9.0.1"
 mkdocstrings = "^0.23.0"
 mkdocstrings-python = "^1.7.3"
 ruff = "^0.3.7"
 markdown = "<3.4.0"
 hypothesis = "^6.99.11"
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 disable_error_code = ["misc"]
 plugins = "numpy.typing.mypy_plugin"
@@ -105,11 +106,16 @@
     "B905",
     "D100",
     "D104",
     "D105",
     "D107",
     "ANN101",
     "PLR0913",
-    "ISC001"
+    "ISC001",
+    "S311",
 ]
-exclude = ["tests/*", "docs/*"]
-lint.pydocstyle.convention = "google"
+# exclude = ["docs/*"]
+lint.pydocstyle.convention = "google"
+
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = ["S101"]
+"docs/*" = ["INP001", "T201", "S101"]
```

### Comparing `zodipy-0.9.0/zodipy/_bandpass.py` & `zodipy-0.9.1/zodipy/_bandpass.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_constants.py` & `zodipy-0.9.1/zodipy/_constants.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_contour.py` & `zodipy-0.9.1/zodipy/_contour.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_emission.py` & `zodipy-0.9.1/zodipy/_emission.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_interpolate_source.py` & `zodipy-0.9.1/zodipy/_interpolate_source.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_ipd_comps.py` & `zodipy-0.9.1/zodipy/_ipd_comps.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_ipd_dens_funcs.py` & `zodipy-0.9.1/zodipy/_ipd_dens_funcs.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_ipd_model.py` & `zodipy-0.9.1/zodipy/_ipd_model.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_line_of_sight.py` & `zodipy-0.9.1/zodipy/_line_of_sight.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_sky_coords.py` & `zodipy-0.9.1/zodipy/_sky_coords.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_source_funcs.py` & `zodipy-0.9.1/zodipy/_source_funcs.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_unit_vectors.py` & `zodipy-0.9.1/zodipy/_unit_vectors.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/_validators.py` & `zodipy-0.9.1/zodipy/_validators.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/comps.py` & `zodipy-0.9.1/zodipy/comps.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/model_registry.py` & `zodipy-0.9.1/zodipy/model_registry.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/source_params.py` & `zodipy-0.9.1/zodipy/source_params.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/zodipy/zodipy.py` & `zodipy-0.9.1/zodipy/zodipy.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.0/PKG-INFO` & `zodipy-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: zodipy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Software for simulating zodiacal emission
-Home-page: https://github.com/Cosmoglobe/zodipy
-License: GPL-3.0
+License: GPL-3.0-or-later
 Keywords: astronomy,astrophysics,cosmology,space,science
 Author: Metin San
 Author-email: metinisan@gmail.com
 Requires-Python: >=3.9
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: astropy (>=5.0.1)
 Requires-Dist: healpy (>=1.16.6,<2.0.0)
 Requires-Dist: jplephem (>=2.17,<3.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Project-URL: documentation, https://cosmoglobe.github.io/zodipy/
+Project-URL: repository, https://github.com/cosmoglobe/zodipy
 Description-Content-Type: text/markdown
 
 
 <img src="docs/img/zodipy_logo.png" width="350">
 
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat-square)](http://www.astropy.org/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zodipy?style=flat-square)
@@ -123,15 +124,15 @@
 
 Note that developers using Python 3.12 will need to upgrade their pip versions with `python3 -m pip install --upgrade pip` before being able to install ZodiPy. This is due to known incompatibilities between older pip versions and Python 3.12
 
 ## Tests, linting and formatting
 The following tools should be run from the root of the repository with no errors. (These are ran automatically as part of the CI workflows on GitHub, but should be tested locally first)
 
 - [pytest](https://docs.pytest.org/en/8.0.x/): Tests are run with pytest by simply running `pytest` in the command line in the root of the repository. 
-- [ruff](https://github.com/astral-sh/ruff): Formating and linting is done with `ruff` by simply running `ruff check zodipy/` and `ruff format zodipy/` in the command line in the root of the repository. 
+- [ruff](https://github.com/astral-sh/ruff): Formating and linting is done with `ruff` by simply running `ruff check` and `ruff format` in the command line in the root of the repository. 
 - [mypy](https://mypy-lang.org/): Type checking is done with `mypy` by simply running `mypy zodipy/` in the root of the repository.
 
 Remeber to add tests when implementing new features to maintain a high code coverage.
 
 ## Documentation
 We use [MkDocs](https://www.mkdocs.org/) to create our documentation. The documentation is built locally with `mkdocs build` from the repository root, and served with `mkdocs serve`.
```

