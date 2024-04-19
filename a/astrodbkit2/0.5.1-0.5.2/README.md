# Comparing `tmp/astrodbkit2-0.5.1.tar.gz` & `tmp/astrodbkit2-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrodbkit2-0.5.1.tar", last modified: Fri Apr 21 18:10:55 2023, max compression
+gzip compressed data, was "astrodbkit2-0.5.2.tar", last modified: Fri Apr 19 19:12:14 2024, max compression
```

## Comparing `astrodbkit2-0.5.1.tar` & `astrodbkit2-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.840833 astrodbkit2-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/astrodbkit2/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/astrodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/schema_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/astrodbkit2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_astrodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/astrodbkit2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/astrodb.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/spectra.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/licenses/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-21 18:10:55.848833 astrodbkit2-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.587697 astrodbkit2-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.579697 astrodbkit2-0.5.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.575697 astrodbkit2-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.579697 astrodbkit2-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-19 19:12:14.583697 astrodbkit2-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.579697 astrodbkit2-0.5.2/astrodbkit2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34969 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/astrodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/schema_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.583697 astrodbkit2-0.5.2/astrodbkit2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/tests/test_astrodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/tests/test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/astrodbkit2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.583697 astrodbkit2-0.5.2/astrodbkit2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 19:12:14.000000 astrodbkit2-0.5.2/astrodbkit2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.583697 astrodbkit2-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/docs/astrodb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20574 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/docs/spectra.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/docs/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:14.583697 astrodbkit2-0.5.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/licenses/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-19 19:12:14.587697 astrodbkit2-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1960 2024-04-19 19:11:58.000000 astrodbkit2-0.5.2/setup.py
```

### Comparing `astrodbkit2-0.5.1/.devcontainer/devcontainer.json` & `astrodbkit2-0.5.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5.1/.github/workflows/python-publish.yml` & `astrodbkit2-0.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5.1/.github/workflows/test-package.yml` & `astrodbkit2-0.5.2/.github/workflows/test-package.yml`

 * *Files 20% similar despite different names*

```diff
@@ -11,37 +11,38 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.8, 3.9, '3.10', 3.11]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flake8 pytest pytest-astropy pytest-cov sphinx-astropy codecov
         # install package and requirements
-        pip install .
-    - name: Lint with flake8
+        pip install ".[all]"
+    - name: Lint with ruff
       run: |
         # stop the build if there are Python syntax errors or undefined names
-        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+        ruff check astrodbkit2 --select=E9,F63,F7,F82 --statistics
+        # exit-zero treats all errors as warnings.
+        ruff check astrodbkit2 --config=pyproject.toml --exit-zero
     - name: Test with pytest
       run: |
         pytest --cov --cov-config=setup.cfg --cov-report=term --cov-report=xml:coverage.xml
-    - name: Post coverage report
-      run: |
-        codecov
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v3
+      env:
+         CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
     - name: Build docs
       run: |
         cd docs
         sphinx-build -W -b html . _build/html
```

### Comparing `astrodbkit2-0.5.1/.gitignore` & `astrodbkit2-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5.1/PKG-INFO` & `astrodbkit2-0.5.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-Metadata-Version: 2.1
-Name: astrodbkit2
-Version: 0.5.1
-Summary: Astronomical database handler code
-Home-page: 
-Author: David Rodriguez
-Author-email: drodriguez@stsci.edu
-License: BSD 3-Clause
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: docs
-License-File: licenses/LICENSE.rst
-
 Astronomical database handler code
 ----------------------------------
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
-.. image:: https://github.com/dr-rodriguez/AstrodbKit2/workflows/Test%20Astrodbkit2/badge.svg?branch=main
-    :target: https://github.com/dr-rodriguez/AstrodbKit2/actions
+.. image:: https://github.com/astrodbtoolkit/AstrodbKit2/workflows/Test%20Astrodbkit2/badge.svg?branch=main
+    :target: https://github.com/astrodbtoolkit/AstrodbKit2/actions
 
-.. image:: https://codecov.io/gh/dr-rodriguez/AstrodbKit2/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/dr-rodriguez/AstrodbKit2
+.. image:: https://codecov.io/gh/astrodbtoolkit/AstrodbKit2/graph/badge.svg?token=LMKVN65D82 
+    :target: https://codecov.io/gh/astrodbtoolkit/AstrodbKit2
 
 AstrodbKit2 is an astronomical database handler code built on top of SQLAlchemy.
-This is built to work with the `SIMPLE database <https://github.com/kelle/SIMPLE>`_, though
+This is built to work with the `SIMPLE database <https://github.com/SIMPLE-AstroDB/SIMPLE-db>`_, though
 similarly constructed databases will work.
 
 Documentation is available at `https://astrodbkit2.readthedocs.io/en/latest/ <https://astrodbkit2.readthedocs.io/en/latest/>`_
 
 License
 -------
```

### Comparing `astrodbkit2-0.5.1/README.rst` & `astrodbkit2-0.5.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,53 @@
+Metadata-Version: 2.1
+Name: astrodbkit2
+Version: 0.5.2
+Summary: Astronomical database handler code
+Home-page: 
+Author: David Rodriguez
+Author-email: drodriguez@stsci.edu
+License: BSD 3-Clause
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: licenses/LICENSE.rst
+Requires-Dist: astropy
+Requires-Dist: astroquery
+Requires-Dist: sqlalchemy>=2.0
+Requires-Dist: pandas>=1.0.4
+Requires-Dist: packaging
+Requires-Dist: specutils>=1.0
+Requires-Dist: tqdm
+Provides-Extra: all
+Requires-Dist: astrodbkit2[docs,test]; extra == "all"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-astropy; extra == "test"
+Requires-Dist: darker==1.7.2; extra == "test"
+Requires-Dist: black==23.9.1; extra == "test"
+Requires-Dist: pre-commit==3.4.0; extra == "test"
+Requires-Dist: ruff==0.3.7; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx-astropy; extra == "docs"
+
 Astronomical database handler code
 ----------------------------------
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
-.. image:: https://github.com/dr-rodriguez/AstrodbKit2/workflows/Test%20Astrodbkit2/badge.svg?branch=main
-    :target: https://github.com/dr-rodriguez/AstrodbKit2/actions
+.. image:: https://github.com/astrodbtoolkit/AstrodbKit2/workflows/Test%20Astrodbkit2/badge.svg?branch=main
+    :target: https://github.com/astrodbtoolkit/AstrodbKit2/actions
 
-.. image:: https://codecov.io/gh/dr-rodriguez/AstrodbKit2/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/dr-rodriguez/AstrodbKit2
+.. image:: https://codecov.io/gh/astrodbtoolkit/AstrodbKit2/graph/badge.svg?token=LMKVN65D82 
+    :target: https://codecov.io/gh/astrodbtoolkit/AstrodbKit2
 
 AstrodbKit2 is an astronomical database handler code built on top of SQLAlchemy.
-This is built to work with the `SIMPLE database <https://github.com/kelle/SIMPLE>`_, though
+This is built to work with the `SIMPLE database <https://github.com/SIMPLE-AstroDB/SIMPLE-db>`_, though
 similarly constructed databases will work.
 
 Documentation is available at `https://astrodbkit2.readthedocs.io/en/latest/ <https://astrodbkit2.readthedocs.io/en/latest/>`_
 
 License
 -------
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/__init__.py` & `astrodbkit2-0.5.2/astrodbkit2/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,30 +2,41 @@
 
 # Packages may add whatever they like to this file, but
 # should keep this content at the top.
 # ----------------------------------------------------------------------------
 # from ._astropy_init import *   # noqa
 # ----------------------------------------------------------------------------
 
-__all__ = ['__version__']
+__all__ = ["__version__"]
 
 # from .example_mod import *   # noqa
 # Then you can be explicit to control what ends up in the namespace,
 # __all__ += ['do_primes']   # noqa
 # or you can keep everything from the subpackage with the following instead
 # __all__ += example_mod.__all__
 
 try:
     from .version import version as __version__
 except ImportError:
-    __version__ = ''
+    __version__ = ""
 
 # Global variables
 
 # These describe the various database tables and their links
-REFERENCE_TABLES = ['Publications', 'Telescopes', 'Instruments', 'Modes', 'Filters', 'PhotometryFilters',
-                    'Citations', 'References', 'Versions', 'Parameters']
+REFERENCE_TABLES = [
+    "Publications",
+    "Telescopes",
+    "Instruments",
+    "Modes",
+    "Filters",
+    "PhotometryFilters",
+    "Citations",
+    "References",
+    "Versions",
+    "Parameters",
+    "Regimes",
+]
 # REFERENCE_TABLES is a list of tables that do not link to the primary table.
 # These are treated separately from the other data tables that are all assumed to be linked to the primary table.
-PRIMARY_TABLE = 'Sources'  # the primary table used for storing objects
-PRIMARY_TABLE_KEY = 'source'  # the name of the primary key in the primary table; this is used for joining tables
-FOREIGN_KEY = 'source'  # the name of the foreign key in other tables that refer back to the primary
+PRIMARY_TABLE = "Sources"  # the primary table used for storing objects
+PRIMARY_TABLE_KEY = "source"  # the name of the primary key in the primary table; this is used for joining tables
+FOREIGN_KEY = "source"  # the name of the foreign key in other tables that refer back to the primary
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/astrodb.py` & `astrodbkit2-0.5.2/astrodbkit2/astrodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-# Main database handler code
+"""Main database handler code"""
 
-__all__ = ['__version__', 'Database', 'or_', 'and_', 'create_database']
+__all__ = ["__version__", "Database", "or_", "and_", "create_database"]
 
-import os
 import json
+import os
 import sqlite3
+
 import numpy as np
 import pandas as pd
+import sqlalchemy.types as sqlalchemy_types
+from astropy.coordinates import SkyCoord
 from astropy.table import Table as AstropyTable
 from astropy.units.quantity import Quantity
-from astropy.coordinates import SkyCoord
-from sqlalchemy.orm import sessionmaker, declarative_base
-from sqlalchemy.orm.query import Query
+from sqlalchemy import Table, and_, create_engine, event, or_, text
 from sqlalchemy.engine import Engine
-import sqlalchemy.types as sqlalchemy_types
-from sqlalchemy import event, create_engine, Table
-from sqlalchemy import or_, and_, text
+from sqlalchemy.orm import declarative_base, sessionmaker
+from sqlalchemy.orm.query import Query
 from tqdm import tqdm
-from . import REFERENCE_TABLES, PRIMARY_TABLE, PRIMARY_TABLE_KEY, FOREIGN_KEY
-from .utils import json_serializer, get_simbad_names, deprecated_alias, datetime_json_parser
+
+from . import FOREIGN_KEY, PRIMARY_TABLE, PRIMARY_TABLE_KEY, REFERENCE_TABLES
 from .spectra import load_spectrum
+from .utils import datetime_json_parser, deprecated_alias, get_simbad_names, json_serializer
 
 try:
     from .version import version as __version__
 except ImportError:
-    __version__ = ''
+    __version__ = ""
 
-# pylint: disable=dangerous-default-value, too-many-arguments, trailing-whitespace
+# pylint: disable=dangerous-default-value, too-many-arguments, trailing-whitespace, abstract-method
 
 # For SQLAlchemy ORM Declarative mapping
-# User created schema should import and use astrodb.Base so that 
+# User created schema should import and use astrodb.Base so that
 # create_database can properly handle them
 Base = declarative_base()
 
 
 class AstrodbQuery(Query):
-    # Subclassing the Query class to add more functionality.
-    # See: https://stackoverflow.com/questions/15936111/sqlalchemy-can-you-add-custom-methods-to-the-query-object
-    def _make_astropy(self):
+    """Subclassing the Query class to add more functionality.
+    See: https://stackoverflow.com/questions/15936111/sqlalchemy-can-you-add-custom-methods-to-the-query-object
+    """
+
+    def _make_astropy(self, **kwargs):
+        """Helper method to convert query results to an Astropy Table"""
         temp = self.all()
         if len(temp) > 0:
-            t = AstropyTable(rows=temp, names=temp[0]._fields)
+            t = AstropyTable(rows=temp, names=temp[0]._fields, **kwargs)
         else:
-            t = AstropyTable(temp)
+            t = AstropyTable(temp, **kwargs)
         return t
 
     def astropy(self, spectra=None, spectra_format=None, **kwargs):
         """
         Allow SQLAlchemy query output to be formatted as an astropy Table
 
         Parameters
@@ -58,28 +62,28 @@
 
         Returns
         -------
         t : astropy.Table
             Table output of query
         """
 
-        t = self._make_astropy()
+        t = self._make_astropy(**kwargs)
 
         # Apply spectra conversion
         if spectra is not None:
             if not isinstance(spectra, (list, tuple)):
                 spectra = [spectra]
             for col in spectra:
                 if col in t.colnames:
                     t[col] = [load_spectrum(x, spectra_format=spectra_format) for x in t[col]]
 
         return t
 
     def table(self, *args, **kwargs):
-        # Alternative for getting astropy Table
+        """Alternative method for getting astropy Table"""
         return self.astropy(*args, **kwargs)
 
     def pandas(self, spectra=None, spectra_format=None, **kwargs):
         """
         Allow SQLAlchemy query output to be formatted as a pandas DataFrame
 
         Parameters
@@ -92,38 +96,38 @@
         Returns
         -------
         df : pandas.DataFrame
             DataFrame output of query
         """
 
         # Relying on astropy to convert to pandas for simplicity as that handles the column names
-        df = self._make_astropy().to_pandas()
+        df = self._make_astropy(**kwargs).to_pandas()
 
         # Apply spectra conversion
         if spectra is not None:
             if not isinstance(spectra, (list, tuple)):
                 spectra = [spectra]
             for col in spectra:
                 if col in df.columns.to_list():
                     df[col] = df[col].apply(lambda x: load_spectrum(x, spectra_format=spectra_format))
 
         return df
 
-    def spectra(self, spectra=['spectrum', 'access_url'], fmt='astropy', **kwargs):
+    def spectra(self, spectra=["spectrum", "access_url"], fmt="astropy", **kwargs):
         """
         Convenience method fo that uses default column name for spectra conversion
 
         Parameters
         ----------
         spectra : str or list
             List of columns to process as spectra
         fmt : str
             Output format (Default: astropy)
         """
-        if fmt == 'pandas':
+        if fmt == "pandas":
             return self.pandas(spectra=spectra, **kwargs)
         else:
             return self.astropy(spectra=spectra, **kwargs)
 
 
 def load_connection(connection_string, sqlite_foreign=True, base=None, connection_arguments={}):
     """Return session, base, and engine objects for connecting to the database.
@@ -150,33 +154,35 @@
         Provides a base class for declarative class definitions.
     engine : engine object
         Provides a source of database connectivity and behavior.
     """
 
     engine = create_engine(connection_string, connect_args=connection_arguments)
     if not base:
-       base = declarative_base()
+        base = declarative_base()
     base.metadata.bind = engine
-    Session = sessionmaker(bind=engine, query_cls=AstrodbQuery)
+    Session = sessionmaker(bind=engine, query_cls=AstrodbQuery)  # pylint: disable=invalid-name
     session = Session()
 
     # Enable foreign key checks in SQLite
-    if 'sqlite' in connection_string and sqlite_foreign:
+    if "sqlite" in connection_string and sqlite_foreign:
         set_sqlite()
     # elif 'postgresql' in connection_string:
     #     # Set up schema in postgres (must be lower case?)
     #     from sqlalchemy import DDL
     #     event.listen(Base.metadata, 'before_create', DDL("CREATE SCHEMA IF NOT EXISTS ivoa"))
     #     event.listen(Base.metadata, 'before_create', DDL("CREATE SCHEMA IF NOT EXISTS tap_schema"))
 
     return session, base, engine
 
 
 def set_sqlite():
-    # Special overrides when using SQLite
+    """Special overrides when using SQLite"""
+    # pylint: disable=unused-argument
+
     @event.listens_for(Engine, "connect")
     def set_sqlite_pragma(dbapi_connection, connection_record):
         # Enable foreign key checking in SQLite
         cursor = dbapi_connection.cursor()
         cursor.execute("PRAGMA foreign_keys=ON")
         cursor.close()
 
@@ -197,16 +203,17 @@
     session, base, engine = load_connection(connection_string, base=Base)
     if drop_tables:
         base.metadata.drop_all()
     base.metadata.create_all(engine)  # this explicitly creates the database
     return session, base, engine
 
 
-def copy_database_schema(source_connection_string, destination_connection_string, sqlite_foreign=False,
-                         ignore_tables=[], copy_data=False):
+def copy_database_schema(
+    source_connection_string, destination_connection_string, sqlite_foreign=False, ignore_tables=[], copy_data=False
+):
     """
     Copy a database schema (ie, all tables and columns) from one database to another
     Adapted from https://gist.github.com/pawl/9935333
 
     Parameters
     ----------
     source_connection_string : str
@@ -233,15 +240,15 @@
         if table.name in ignore_tables:
             continue
 
         dest_table = Table(table.name, dest_metadata)
 
         # Copy schema and create newTable from oldTable
         for column in src_metadata.tables[table.name].columns:
-            dest_table.append_column(column._copy())
+            dest_table.append_column(column._copy())  # pylint: disable=protected-access
         dest_table.create(bind=dest_engine)
 
         # Copy data, row by row
         if copy_data:
             table_data = src_session.query(src_metadata.tables[table.name]).all()
             for row in table_data:
                 dest_session.execute(dest_table.insert().values(row))
@@ -251,22 +258,27 @@
     src_session.close()
     dest_session.close()
     src_engine.dispose()
     dest_engine.dispose()
 
 
 class Database:
-    def __init__(self, connection_string,
-                 reference_tables=REFERENCE_TABLES,
-                 primary_table=PRIMARY_TABLE,
-                 primary_table_key=PRIMARY_TABLE_KEY,
-                 foreign_key=FOREIGN_KEY,
-                 column_type_overrides={},
-                 sqlite_foreign=True,
-                 connection_arguments={}):
+    """Database handler class"""
+
+    def __init__(
+        self,
+        connection_string,
+        reference_tables=REFERENCE_TABLES,
+        primary_table=PRIMARY_TABLE,
+        primary_table_key=PRIMARY_TABLE_KEY,
+        foreign_key=FOREIGN_KEY,
+        column_type_overrides={},
+        sqlite_foreign=True,
+        connection_arguments={},
+    ):
         """
         Wrapper for database calls and utility functions
 
         Parameters
         ----------
         connection_string : str
             Connection string to establish a database connection
@@ -285,19 +297,20 @@
             will set the table spectra, column spectrum to be of type TEXT()
         sqlite_foreign : bool
             Flag to enable/disable use of foreign keys with SQLite. Default: True
         connection_arguments : dict
             Additional connection arguments, like {'check_same_thread': False}. Default: {}
         """
 
-        if connection_string == 'sqlite://':
+        if connection_string == "sqlite://":
             self.session, self.base, self.engine = create_database(connection_string)
         else:
-            self.session, self.base, self.engine = load_connection(connection_string, sqlite_foreign=sqlite_foreign,
-                                                                   connection_arguments=connection_arguments)
+            self.session, self.base, self.engine = load_connection(
+                connection_string, sqlite_foreign=sqlite_foreign, connection_arguments=connection_arguments
+            )
 
         # Convenience methods
         self.query = self.session.query
         self.save_db = self.save_database
         self.load_db = self.load_database
 
         # Prep the tables
@@ -307,38 +320,40 @@
 
         self._reference_tables = reference_tables
         self._primary_table = primary_table
         self._primary_table_key = primary_table_key
         self._foreign_key = foreign_key
 
         if len(self.metadata.tables) == 0:
-            print('Database empty. Import schema (eg, from astrodbkit.schema_example import *) '
-                  'and then run create_database()')
-            raise RuntimeError('Create database first.')
+            print(
+                "Database empty. Import schema (eg, from astrodbkit.schema_example import *) "
+                "and then run create_database()"
+            )
+            raise RuntimeError("Create database first.")
 
         # Set tables as explicit attributes of this class
         for table in self.metadata.tables:
             self.__setattr__(table, self.metadata.tables[table])
 
         # If column overrides are provided, this will set the types to whatever the user provided
         if len(column_type_overrides) > 0:
             for k, v in column_type_overrides.items():
-                tab, col = k.split('.')
+                tab, col = k.split(".")
                 self.metadata.tables[tab].columns[col].type = v
 
     # Generic methods
     @staticmethod
     def _handle_format(temp, fmt):
         # Internal method to handle SQLAlchemy output and format it
-        if fmt.lower() in ('astropy', 'table'):
+        if fmt.lower() in ("astropy", "table"):
             if len(temp) > 0:
                 results = AstropyTable(rows=temp, names=temp[0]._fields)
             else:
                 results = AstropyTable(temp)
-        elif fmt.lower() == 'pandas':
+        elif fmt.lower() == "pandas":
             if len(temp) > 0:
                 results = pd.DataFrame(temp, columns=temp[0]._fields)
             else:
                 results = pd.DataFrame(temp)
         else:
             results = temp
 
@@ -422,18 +437,25 @@
 
         if pretty_print:
             print(json.dumps(data_dict, indent=4, default=json_serializer))
 
         return data_dict
 
     # Text query methods
-    @deprecated_alias(format='fmt')
-    def search_object(self, name, output_table=None, resolve_simbad=False,
-                      table_names={'Sources': ['source', 'shortname'], 'Names': ['other_name']},
-                      fmt='table', fuzzy_search=True, verbose=True):
+    @deprecated_alias(format="fmt")
+    def search_object(
+        self,
+        name,
+        output_table=None,
+        resolve_simbad=False,
+        table_names={"Sources": ["source", "shortname"], "Names": ["other_name"]},
+        fmt="table",
+        fuzzy_search=True,
+        verbose=True,
+    ):
         """
         Query the database for the object specified. By default will return the primary table,
         but this can be specified. Users can also request to resolve the object name via Simbad and query against
         all Simbad names.
 
         Parameters
         ----------
@@ -458,73 +480,70 @@
         List of SQLAlchemy results
         """
 
         # Set table to output and verify it exists
         if output_table is None:
             output_table = self._primary_table
         if output_table not in self.metadata.tables:
-            raise RuntimeError(f'Table {output_table} is not in the database')
+            raise RuntimeError(f"Table {output_table} is not in the database")
 
         match_column = self._foreign_key
         if output_table == self._primary_table:
             match_column = self._primary_table_key
 
         # Query Simbad to get additional names and join them to list to search
         if resolve_simbad:
             simbad_names = get_simbad_names(name, verbose=verbose)
             name = list(set(simbad_names + [name]))
             if verbose:
-                print(f'Including Simbad names, searching for: {name}')
+                print(f"Including Simbad names, searching for: {name}")
 
         # Turn name into a list
         if not isinstance(name, list):
             name = [name]
 
         # Verify provided tables exist in database
         for k in table_names.keys():
             if k not in self.metadata.tables:
-                raise RuntimeError(f'Table {k} is not in the database')
+                raise RuntimeError(f"Table {k} is not in the database")
 
         # Get source for objects that match the provided names
         # The following will build the filters required to query all specified tables
         # approximately by case-insensitive names.
         # This is not really optimized as it does separate DB calls,
         # but is the simpler setup and at our scale is sufficient
         matched_names = []
         for k, col_list in table_names.items():
             for v in col_list:
                 if fuzzy_search:
-                    filters = [self.metadata.tables[k].columns[v].ilike(f'%{n}%')
-                               for n in name]
+                    filters = [self.metadata.tables[k].columns[v].ilike(f"%{n}%") for n in name]
                 else:
-                    filters = [self.metadata.tables[k].columns[v].ilike(f'{n}')
-                               for n in name]
+                    filters = [self.metadata.tables[k].columns[v].ilike(f"{n}") for n in name]
 
                 # Column to be returned
                 if k == self._primary_table:
                     output_to_match = self.metadata.tables[k].columns[self._primary_table_key]
                 else:
                     output_to_match = self.metadata.tables[k].columns[self._foreign_key]
 
-                temp = self.query(output_to_match).\
-                    filter(or_(*filters)).\
-                    distinct().\
-                    all()
+                temp = self.query(output_to_match).filter(or_(*filters)).distinct().all()
                 matched_names += [s[0] for s in temp]
 
         # Join the matched sources with the desired table
-        temp = self.query(self.metadata.tables[output_table]).\
-            filter(self.metadata.tables[output_table].columns[match_column].in_(matched_names)).\
-            all()
+        temp = (
+            self.query(self.metadata.tables[output_table])
+            .filter(self.metadata.tables[output_table].columns[match_column].in_(matched_names))
+            .all()
+        )
 
         results = self._handle_format(temp, fmt)
 
         return results
 
-    def search_string(self, value, fmt='table', fuzzy_search=True, verbose=True):
+    def search_string(self, value, fmt="table", fuzzy_search=True, verbose=True):
         """
         Search an abitrary string across all string columns in the full database
 
         Parameters
         ----------
         value : str
             String to search for
@@ -541,46 +560,46 @@
         """
 
         # Loop over all tables to build the results
         output_dict = {}
         for table in self.metadata.tables:
             # Gather only string-type columns
             columns = self.metadata.tables[table].columns
-            col_list = [c for c in columns
-                        if isinstance(c.type, sqlalchemy_types.String)
-                        or isinstance(c.type, sqlalchemy_types.Text)
-                        or isinstance(c.type, sqlalchemy_types.Unicode)]
+            col_list = [
+                c
+                for c in columns
+                if isinstance(c.type, sqlalchemy_types.String)
+                or isinstance(c.type, sqlalchemy_types.Text)
+                or isinstance(c.type, sqlalchemy_types.Unicode)
+            ]
 
             # Construct filters to query for each string column
             filters = []
             for c in col_list:
                 if fuzzy_search:
-                    filters += [c.ilike(f'%{value}%')]
+                    filters += [c.ilike(f"%{value}%")]
                 else:
-                    filters += [c.ilike(f'{value}')]
+                    filters += [c.ilike(f"{value}")]
 
             # Perform the actual query
-            temp = self.query(self.metadata.tables[table]). \
-                filter(or_(*filters)). \
-                distinct(). \
-                all()
+            temp = self.query(self.metadata.tables[table]).filter(or_(*filters)).distinct().all()
 
             # Append results to dictionary output in specified format
             if len(temp) > 0:
                 results = self._handle_format(temp, fmt)
                 if verbose:
                     print(table)
                     print(results)
                 output_dict[table] = results
 
         return output_dict
 
     # General query methods
-    @deprecated_alias(format='fmt')
-    def sql_query(self, query, fmt='default'):
+    @deprecated_alias(format="fmt")
+    def sql_query(self, query, fmt="default"):
         """
         Wrapper for a direct SQL query.
 
         Parameters
         ----------
         query : str
             Query to be performed
@@ -593,16 +612,26 @@
         """
 
         with self.engine.connect() as conn:
             temp = conn.execute(text(query)).fetchall()
 
         return self._handle_format(temp, fmt)
 
-    def query_region(self, target_coords, radius=Quantity(10, unit='arcsec'), output_table=None, fmt='table',
-                    coordinate_table=None, ra_col='ra', dec_col='dec', frame='icrs', unit='deg'):
+    def query_region(
+        self,
+        target_coords,
+        radius=Quantity(10, unit="arcsec"),
+        output_table=None,
+        fmt="table",
+        coordinate_table=None,
+        ra_col="ra",
+        dec_col="dec",
+        frame="icrs",
+        unit="deg",
+    ):
         """
         Perform a cone search of the given coordinates and return the specified output table.
 
         Parameters
         ----------
         target_coords : SkyCoord
             Astropy SkyCoord object of coordinates to search around
@@ -629,54 +658,56 @@
         List of SQLAlchemy results
         """
 
         # Set table to output and verify it exists
         if output_table is None:
             output_table = self._primary_table
         if output_table not in self.metadata.tables:
-            raise RuntimeError(f'Table {output_table} is not in the database')
+            raise RuntimeError(f"Table {output_table} is not in the database")
 
         # Radius conversion
         if not isinstance(radius, Quantity):
-            radius = Quantity(radius, unit='arcsec')
+            radius = Quantity(radius, unit="arcsec")
 
         # Get the column name to use for matching
         match_column = self._foreign_key
         if output_table == self._primary_table:
             match_column = self._primary_table_key
 
         # Grab the specified coordinate table (Sources by default) to construct SkyCoord objects
         if coordinate_table is None:
             coordinate_table = self._primary_table
         if coordinate_table not in self.metadata.tables:
-            raise RuntimeError(f'Table {coordinate_table} is not in the database')
+            raise RuntimeError(f"Table {coordinate_table} is not in the database")
         coordinate_match_column = self._foreign_key
         if coordinate_table == self._primary_table:
             coordinate_match_column = self._primary_table_key
 
         # This is adapted from the original astrodbkit code
         df = self.query(self.metadata.tables[coordinate_table]).pandas()
-        df[['ra', 'dec']] = df[[ra_col, dec_col]].apply(pd.to_numeric)  # convert everything to floats
-        mask = df['ra'].isnull()
+        df[["ra", "dec"]] = df[[ra_col, dec_col]].apply(pd.to_numeric)  # convert everything to floats
+        mask = df["ra"].isnull()
         df = df[~mask]
 
         # Native use of astropy SkyCoord objects here
-        coord_list = SkyCoord(df['ra'].tolist(), df['dec'].tolist(), frame=frame, unit=unit)
+        coord_list = SkyCoord(df["ra"].tolist(), df["dec"].tolist(), frame=frame, unit=unit)
         sep_list = coord_list.separation(target_coords)  # sky separations for each db object against target position
         good = sep_list <= radius
 
         if sum(good) > 0:
             matched_list = df[coordinate_match_column][good]
         else:
             matched_list = []
 
         # Join the matched sources with the desired table
-        temp = self.query(self.metadata.tables[output_table]). \
-            filter(self.metadata.tables[output_table].columns[match_column].in_(matched_list)). \
-            all()
+        temp = (
+            self.query(self.metadata.tables[output_table])
+            .filter(self.metadata.tables[output_table].columns[match_column].in_(matched_list))
+            .all()
+        )
         results = self._handle_format(temp, fmt)
 
         return results
 
     # Object output methods
     def save_json(self, name, directory):
         """
@@ -687,24 +718,26 @@
         name : str
             Name of source to match by primary key.
             Alternatively can also be a row from a query against the source table.
         directory : str
             Name of directory in which to save the output JSON
         """
 
+        # pylint: disable=unnecessary-dunder-call
+
         if isinstance(name, str):
             source_name = str(name)
             data = self.inventory(name)
         else:
             source_name = str(name.__getattribute__(self._primary_table_key))
             data = self.inventory(name.__getattribute__(self._primary_table_key))
 
         # Clean up spaces and other special characters
-        filename = source_name.lower().replace(' ', '_').replace('*', '').strip() + '.json'
-        with open(os.path.join(directory, filename), 'w') as f:
+        filename = source_name.lower().replace(" ", "_").replace("*", "").strip() + ".json"
+        with open(os.path.join(directory, filename), "w", encoding="utf-8") as f:
             f.write(json.dumps(data, indent=4, default=json_serializer))
 
     def save_reference_table(self, table, directory):
         """
 
         Parameters
         ----------
@@ -712,17 +745,17 @@
             Name of reference table to output
         directory : str
             Name of directory in which to save the output JSON
         """
 
         results = self.session.query(self.metadata.tables[table]).all()
         data = [row._asdict() for row in results]
-        filename = table + '.json'
+        filename = table + ".json"
         if len(data) > 0:
-            with open(os.path.join(directory, filename), 'w') as f:
+            with open(os.path.join(directory, filename), "w", encoding="utf-8") as f:
                 f.write(json.dumps(data, indent=4, default=json_serializer))
 
     def save_database(self, directory, clear_first=True):
         """
         Output contents of the database into the specified directory as JSON files.
         Source objects have individual JSON files with all data for that object.
         Reference tables have a single JSON for all contents in the table.
@@ -733,15 +766,15 @@
             Name of directory in which to save the output JSON
         clear_first : bool
             First clear the directory of all existing JSON (useful to capture DB deletions). Default: True
         """
 
         # Clear existing files first from that directory
         if clear_first:
-            print('Clearing existing JSON files...')
+            print("Clearing existing JSON files...")
             for filename in os.listdir(directory):
                 os.remove(os.path.join(directory, filename))
 
         # Output reference tables
         for table in self._reference_tables:
             # Skip reference tables that are not actually in the database
             if table not in self.metadata.tables.keys():
@@ -750,15 +783,15 @@
             self.save_reference_table(table, directory)
 
         # Output primary objects
         for row in tqdm(self.query(self.metadata.tables[self._primary_table])):
             self.save_json(row, directory)
 
     # Object input methods
-    def add_table_data(self, data, table, fmt='csv'):
+    def add_table_data(self, data, table, fmt="csv"):
         """
         Method to insert data into the database. Column names in the file must match those of the database table.
         Additional columns in the supplied table are ignored.
         Format options include:
 
          - csv
          - astropy
@@ -771,34 +804,34 @@
             Name of file or Table or DataFrame to load
         table : str
             Name of table to insert records into
         fmt : str
             Data format. Default: csv
         """
 
-        if fmt.lower() == 'csv':
+        if fmt.lower() == "csv":
             df = pd.read_csv(data)
-        elif fmt.lower() == 'astropy':
+        elif fmt.lower() == "astropy":
             df = data.to_pandas()
-        elif fmt.lower() == 'pandas':
+        elif fmt.lower() == "pandas":
             df = data.copy()
         else:
-            raise RuntimeError(f'Unrecognized format {fmt}')
+            raise RuntimeError(f"Unrecognized format {fmt}")
 
         # Foreign key constraints will prevent inserts of missing sources,
         # but for clarity we'll check first and exit if there are missing sources
         if table != self._primary_table:
             source_list = df[self._foreign_key].to_list()
             primary_column = self.metadata.tables[self._primary_table].columns[self._primary_table_key]
             matched_sources = self.query(primary_column).filter(primary_column.in_(source_list)).all()
             missing_sources = np.setdiff1d(source_list, matched_sources)
             if len(missing_sources) > 0:
-                print(f'{len(missing_sources)} missing source(s):')
+                print(f"{len(missing_sources)} missing source(s):")
                 print(missing_sources)
-                raise RuntimeError(f'There are missing entries in {self._primary_table} table. These must exist first.')
+                raise RuntimeError(f"There are missing entries in {self._primary_table} table. These must exist first.")
 
         # Convert format for SQLAlchemy
         data = [row.to_dict() for _, row in df.iterrows()]
 
         # Remove unused columns
         column_names = self.metadata.tables[table].columns.keys()
         fixed_data = [{k: v for k, v in d.items() if k in (d.keys() & column_names)} for d in data]
@@ -817,34 +850,35 @@
             Name of table to load. Table must already exist in the schema.
         directory : str
             Name of directory containing the JSON file
         verbose : bool
             Flag to enable diagnostic messages
         """
 
-        filename = os.path.join(directory, table+'.json')
+        filename = os.path.join(directory, table + ".json")
         if os.path.exists(filename):
-            with open(filename, 'r') as f:
+            with open(filename, "r", encoding="utf-8") as f:
                 data = json.load(f)
                 with self.engine.begin() as conn:
                     conn.execute(self.metadata.tables[table].insert().values(data))
         else:
-            if verbose: print(f'{table}.json not found.')
+            if verbose:
+                print(f"{table}.json not found.")
 
     def load_json(self, filename):
         """
         Load single source JSON into the database
 
         Parameters
         ----------
         filename : str
             Name of directory containing the JSON file
         """
 
-        with open(filename, 'r') as f:
+        with open(filename, "r", encoding="utf-8") as f:
             data = json.load(f, object_hook=datetime_json_parser)
 
         # Loop through the dictionary, adding data to the database.
         # Ensure that Sources is added first
         source = data[self._primary_table][0][self._primary_table_key]
         with self.engine.begin() as conn:
             conn.execute(self.metadata.tables[self._primary_table].insert().values(data[self._primary_table]))
@@ -870,36 +904,40 @@
         verbose : bool
             Flag to enable diagnostic messages
         """
 
         # Clear existing database contents
         # reversed(sorted_tables) can help ensure that foreign key dependencies are taken care of first
         for table in reversed(self.metadata.sorted_tables):
-            if verbose: print(f'Deleting {table.name} table')
+            if verbose:
+                print(f"Deleting {table.name} table")
             with self.engine.begin() as conn:
                 conn.execute(self.metadata.tables[table.name].delete())
 
         # Load reference tables first
         for table in self._reference_tables:
-            if verbose: print(f'Loading {table} table')
+            if verbose:
+                print(f"Loading {table} table")
             self.load_table(table, directory, verbose=verbose)
 
         # Load object data
-        if verbose: print('Loading object tables')
+        if verbose:
+            print("Loading object tables")
         for file in tqdm(os.listdir(directory)):
             # Skip reference tables
-            core_name = file.replace('.json', '')
+            core_name = file.replace(".json", "")
             if core_name in self._reference_tables:
                 continue
 
             # Skip non-JSON files or hidden files
-            if not file.endswith('.json') or file.startswith('.'):
+            if not file.endswith(".json") or file.startswith("."):
                 continue
 
             self.load_json(os.path.join(directory, file))
 
     def dump_sqlite(self, database_name):
-        if self.engine.url.drivername == 'sqlite':
+        """Output database as a sqlite file"""
+        if self.engine.url.drivername == "sqlite":
             destconn = sqlite3.connect(database_name)
             self.engine.raw_connection().backup(destconn)
         else:
-            print('AstrodbKit2: dump_sqlite not available for non-sqlite databases')
+            print("AstrodbKit2: dump_sqlite not available for non-sqlite databases")
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/schema_example.py` & `astrodbkit2-0.5.2/astrodbkit2/schema_example.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,142 @@
-# Example schema for part of the SIMPLE database
+"""Example schema for part of the SIMPLE database"""
+
+# pylint: disable=unused-argument, unused-import
 
-import sqlalchemy as sa
-from sqlalchemy import Boolean, Column, Float, ForeignKey, Integer, String, BigInteger, Enum, Date, DateTime
 import enum
+
+import sqlalchemy as sa
+from sqlalchemy import Boolean, Column, Enum, Float, ForeignKey, String
+from sqlalchemy.orm import validates
+
 from astrodbkit2.astrodb import Base
 from astrodbkit2.views import view
 
 
 # -------------------------------------------------------------------------------------------------------------------
 # Reference tables
 class Publications(Base):
     """ORM for publications table.
     This stores reference information (DOI, bibcodes, etc) and has shortname as the primary key
     """
-    __tablename__ = 'Publications'
+
+    __tablename__ = "Publications"
     name = Column(String(30), primary_key=True, nullable=False)
     bibcode = Column(String(100))
     doi = Column(String(100))
     description = Column(String(1000))
 
 
 class Telescopes(Base):
-    __tablename__ = 'Telescopes'
+    """Telescopes table"""
+    __tablename__ = "Telescopes"
     name = Column(String(30), primary_key=True, nullable=False)
-    reference = Column(String(30), ForeignKey('Publications.name', ondelete='cascade'))
+    reference = Column(String(30), ForeignKey("Publications.name", ondelete="cascade"))
 
 
 class Instruments(Base):
-    __tablename__ = 'Instruments'
+    """Instruments table"""
+    __tablename__ = "Instruments"
     name = Column(String(30), primary_key=True, nullable=False)
-    reference = Column(String(30), ForeignKey('Publications.name', ondelete='cascade'))
+    reference = Column(String(30), ForeignKey("Publications.name", ondelete="cascade"))
 
 
 # -------------------------------------------------------------------------------------------------------------------
 # Enumerations tables
 class Regime(enum.Enum):
     """Enumeration for spectral type regime"""
-    optical = 'optical'
-    infrared = 'infrared'
-    ultraviolet = 'ultraviolet'
-    radio = 'radio'
+
+    # pylint: disable=invalid-name
+    optical = "optical"
+    infrared = "infrared"
+    ultraviolet = "ultraviolet"
+    radio = "radio"
 
 
 # -------------------------------------------------------------------------------------------------------------------
 # Main tables
 class Sources(Base):
     """ORM for the sources table. This stores the main identifiers for our objects along with ra and dec"""
-    __tablename__ = 'Sources'
+
+    __tablename__ = "Sources"
     source = Column(String(100), primary_key=True, nullable=False)
     ra = Column(Float)
     dec = Column(Float)
     shortname = Column(String(30))  # not needed?
-    reference = Column(String(30), ForeignKey('Publications.name', ondelete='cascade'), nullable=False)
+    reference = Column(String(30), ForeignKey("Publications.name", ondelete="cascade"), nullable=False)
     comments = Column(String(1000))
 
+    @validates("ra")
+    def validate_ra(self, key, value):
+        """Ensure RA is within bounds"""
+        if value > 360 or value < 0:
+            raise ValueError("RA not in allowed range (0..360)")
+        return value
+
+    @validates("dec")
+    def validate_dec(self, key, value):
+        """Ensure Dec is within bounds"""
+        if value > 90 or value < -90:
+            raise ValueError("Dec not in allowed range (-90..90)")
+        return value
+
 
 class Names(Base):
-    __tablename__ = 'Names'
-    source = Column(String(100), ForeignKey('Sources.source', ondelete='cascade'), nullable=False, primary_key=True)
+    """Names table"""
+    __tablename__ = "Names"
+    source = Column(String(100), ForeignKey("Sources.source", ondelete="cascade"), nullable=False, primary_key=True)
     other_name = Column(String(100), primary_key=True, nullable=False)
 
 
 class Photometry(Base):
-    __tablename__ = 'Photometry'
-    source = Column(String(100), ForeignKey('Sources.source', ondelete='cascade', onupdate='cascade'), nullable=False, primary_key=True)
+    """Photometry table"""
+    __tablename__ = "Photometry"
+    source = Column(
+        String(100),
+        ForeignKey("Sources.source", ondelete="cascade", onupdate="cascade"),
+        nullable=False,
+        primary_key=True,
+    )
     band = Column(String(30), primary_key=True)
     ucd = Column(String(100))
     magnitude = Column(Float)
     magnitude_error = Column(Float)
-    telescope = Column(String(30), ForeignKey('Telescopes.name', ondelete='cascade'))
-    instrument = Column(String(30), ForeignKey('Instruments.name', ondelete='cascade'))
+    telescope = Column(String(30), ForeignKey("Telescopes.name", ondelete="cascade"))
+    instrument = Column(String(30), ForeignKey("Instruments.name", ondelete="cascade"))
     epoch = Column(String(30))
     comments = Column(String(1000))
-    reference = Column(String(30), ForeignKey('Publications.name', ondelete='cascade'), primary_key=True)
+    reference = Column(String(30), ForeignKey("Publications.name", ondelete="cascade"), primary_key=True)
 
 
 class SpectralTypes(Base):
-    __tablename__ = 'SpectralTypes'
-    source = Column(String(100), ForeignKey('Sources.source', ondelete='cascade', onupdate='cascade'), nullable=False, primary_key=True)
+    """SpectralTypes table"""
+    __tablename__ = "SpectralTypes"
+    source = Column(
+        String(100),
+        ForeignKey("Sources.source", ondelete="cascade", onupdate="cascade"),
+        nullable=False,
+        primary_key=True,
+    )
     spectral_type = Column(Float)
     spectral_type_error = Column(Float)
-    regime = Column(Enum(Regime, create_constraint=True), primary_key=True)  # restricts to a few values: Optical, Infrared
+    regime = Column(
+        Enum(Regime, create_constraint=True), primary_key=True
+    )  # restricts to a few values: Optical, Infrared
     best = Column(Boolean)  # flag for indicating if this is the best measurement or not
     comments = Column(String(1000))
-    reference = Column(String(30), ForeignKey('Publications.name', ondelete='cascade'), primary_key=True)
+    reference = Column(String(30), ForeignKey("Publications.name", ondelete="cascade"), primary_key=True)
 
 
 # -------------------------------------------------------------------------------------------------------------------
 # Views
 SampleView = view(
-        "SampleView",
-        Base.metadata,
-        sa.select(
-            Sources.source.label("source"),
-            Sources.ra.label("s_ra"),
-            Sources.dec.label("s_dec"),
-            SpectralTypes.spectral_type.label("spectral_type"),
-        ).select_from(Sources).join(SpectralTypes, Sources.source == SpectralTypes.source)
-        )
+    "SampleView",
+    Base.metadata,
+    sa.select(
+        Sources.source.label("source"),
+        Sources.ra.label("s_ra"),
+        Sources.dec.label("s_dec"),
+        SpectralTypes.spectral_type.label("spectral_type"),
+    )
+    .select_from(Sources)
+    .join(SpectralTypes, Sources.source == SpectralTypes.source),
+)
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/spectra.py` & `astrodbkit2-0.5.2/astrodbkit2/spectra.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,102 +1,103 @@
 """Functions to handle loading of spectrum objects"""
 
 import os
-import numpy as np
+
 import astropy.units as u
-from astropy.wcs import WCS
+import numpy as np
 from astropy.io import fits
 from astropy.nddata import StdDevUncertainty
 from astropy.units import Unit
+from astropy.wcs import WCS
 from specutils import Spectrum1D
-from specutils.io.registers import data_loader
 from specutils.io.parsing_utils import read_fileobj_or_hdulist
+from specutils.io.registers import data_loader
 
 # pylint: disable=no-member, unused-argument
 
+
 def _identify_spex(filename):
     """
     Check whether the given file is a SpeX data product.
     """
     try:
         with fits.open(filename, memmap=False) as hdulist:
-            return 'spex' in hdulist[0].header['INSTRUME'].lower() and \
-                   'irtf' in hdulist[0].header['TELESCOP'].lower()
+            return "spex" in hdulist[0].header["INSTRUME"].lower() and "irtf" in hdulist[0].header["TELESCOP"].lower()
     except Exception:  # pylint: disable=broad-except,
         return False
 
 
 def identify_spex_prism(origin, *args, **kwargs):
     """
     Confirm this is a SpeX Prism FITS file.
     See FITS keyword reference at http://irtfweb.ifa.hawaii.edu/~spex/observer/
     Notes: GRAT has values of: ShortXD, Prism, LXD_long, LXD_short, SO_long, SO_short
     """
     is_spex = _identify_spex(args[0])
     if is_spex:
         with fits.open(args[0], memmap=False) as hdulist:
-            return (isinstance(args[0], str) and
-                    os.path.splitext(args[0].lower())[1] == '.fits' and
-                    is_spex
-                    and ('lowres' in hdulist[0].header['GRAT'].lower() or
-                         'prism' in hdulist[0].header['GRAT'].lower())
-                    )
+            return (
+                isinstance(args[0], str)
+                and os.path.splitext(args[0].lower())[1] == ".fits"
+                and is_spex
+                and ("lowres" in hdulist[0].header["GRAT"].lower() or "prism" in hdulist[0].header["GRAT"].lower())
+            )
     else:
         return is_spex
 
 
-@data_loader("Spex Prism", identifier=identify_spex_prism, extensions=['fits'], dtype=Spectrum1D)
+@data_loader("Spex Prism", identifier=identify_spex_prism, extensions=["fits"], dtype=Spectrum1D)
 def spex_prism_loader(filename, **kwargs):
     """Open a SpeX Prism file and convert it to a Spectrum1D object"""
 
     with fits.open(filename, **kwargs) as hdulist:
         header = hdulist[0].header
 
         tab = hdulist[0].data
 
         # Handle missing/incorrect units
         try:
-            flux_unit = header['YUNITS'].replace('ergs', 'erg ').strip()
-            wave_unit = header['XUNITS'].replace('Microns', 'um')
+            flux_unit = header["YUNITS"].replace("ergs", "erg ").strip()
+            wave_unit = header["XUNITS"].replace("Microns", "um")
         except (KeyError, ValueError):
             # For now, assume some default units
-            flux_unit = 'erg'
-            wave_unit = 'um'
+            flux_unit = "erg"
+            wave_unit = "um"
 
         wave, data = tab[0] * Unit(wave_unit), tab[1] * Unit(flux_unit)
 
         if tab.shape[0] == 3:
             uncertainty = StdDevUncertainty(tab[2])
         else:
             uncertainty = None
 
-        meta = {'header': header}
+        meta = {"header": header}
 
     return Spectrum1D(flux=data, spectral_axis=wave, uncertainty=uncertainty, meta=meta)
 
 
 def identify_wcs1d_multispec(origin, *args, **kwargs):
     """
     Identifier for WCS1D multispec
     """
-    hdu = kwargs.get('hdu', 0)
+    hdu = kwargs.get("hdu", 0)
 
     # Check if number of axes is one and dimension of WCS is greater than one
     with read_fileobj_or_hdulist(*args, **kwargs) as hdulist:
-        return (hdulist[hdu].header.get('WCSDIM', 1) > 1 and
-                hdulist[hdu].header['NAXIS'] > 1  and
-                'WAT0_001' in hdulist[hdu].header and
-                hdulist[hdu].header.get('WCSDIM', 1) == hdulist[hdu].header['NAXIS'] and
-                'LINEAR' in hdulist[hdu].header.get('CTYPE1', ''))
+        return (
+            hdulist[hdu].header.get("WCSDIM", 1) > 1
+            and hdulist[hdu].header["NAXIS"] > 1
+            and "WAT0_001" in hdulist[hdu].header
+            and hdulist[hdu].header.get("WCSDIM", 1) == hdulist[hdu].header["NAXIS"]
+            and "LINEAR" in hdulist[hdu].header.get("CTYPE1", "")
+        )
 
 
-@data_loader("wcs1d-multispec", identifier=identify_wcs1d_multispec, extensions=['fits'],
-             dtype=Spectrum1D, priority=10)
-def wcs1d_multispec_loader(file_obj, flux_unit=None,
-                      hdu=0, verbose=False, **kwargs):
+@data_loader("wcs1d-multispec", identifier=identify_wcs1d_multispec, extensions=["fits"], dtype=Spectrum1D, priority=10)
+def wcs1d_multispec_loader(file_obj, flux_unit=None, hdu=0, verbose=False, **kwargs):
     """
     Loader for multiextension spectra as wcs1d. Adapted from wcs1d_fits_loader
 
     Parameters
     ----------
     file_obj : str, file-like or HDUList
         FITS file name, object (provided from name by Astropy I/O Registry),
@@ -118,90 +119,106 @@
     """
 
     with read_fileobj_or_hdulist(file_obj, **kwargs) as hdulist:
         header = hdulist[hdu].header
         wcs = WCS(header)
 
         # Load data, convert units if BUNIT and flux_unit is provided and not the same
-        if 'BUNIT' in header:
-            data = u.Quantity(hdulist[hdu].data, unit=header['BUNIT'])
+        if "BUNIT" in header:
+            data = u.Quantity(hdulist[hdu].data, unit=header["BUNIT"])
             if u.A in data.unit.bases:
-                data = data * u.A/u.AA # convert ampere to Angroms
+                data = data * u.A / u.AA  # convert ampere to Angroms
             if flux_unit is not None:
                 data = data.to(flux_unit)
         else:
             data = u.Quantity(hdulist[hdu].data, unit=flux_unit)
 
-    if wcs.wcs.cunit[0] == '' and 'WAT1_001' in header:
+    if wcs.wcs.cunit[0] == "" and "WAT1_001" in header:
         # Try to extract from IRAF-style card or use Angstrom as default.
-        wat_dict = dict((rec.split('=') for rec in header['WAT1_001'].split()))
-        unit = wat_dict.get('units', 'Angstrom')
+        wat_dict = dict((rec.split("=") for rec in header["WAT1_001"].split()))
+        unit = wat_dict.get("units", "Angstrom")
         if hasattr(u, unit):
             wcs.wcs.cunit[0] = unit
         else:  # try with unit name stripped of excess plural 's'...
-            wcs.wcs.cunit[0] = unit.rstrip('s')
+            wcs.wcs.cunit[0] = unit.rstrip("s")
         if verbose:
             print(f"Extracted spectral axis unit '{unit}' from 'WAT1_001'")
-    elif wcs.wcs.cunit[0] == '':
-        wcs.wcs.cunit[0] = 'Angstrom'
+    elif wcs.wcs.cunit[0] == "":
+        wcs.wcs.cunit[0] = "Angstrom"
 
     # Compatibility attribute for lookup_table (gwcs) WCS
     wcs.unit = tuple(wcs.wcs.cunit)
 
     # Identify the correct parts of the data to store
     if len(data.shape) > 1:
         flux_data = data[0]
     else:
         flux_data = data
     uncertainty = None
-    if 'NAXIS3' in header:
-        for i in range(header['NAXIS3']):
-            if 'spectrum' in header.get(f'BANDID{i+1}', ''):
+    if "NAXIS3" in header:
+        for i in range(header["NAXIS3"]):
+            if "spectrum" in header.get(f"BANDID{i+1}", ""):
                 flux_data = data[i]
-            if 'sigma' in header.get(f'BANDID{i+1}', ''):
+            if "sigma" in header.get(f"BANDID{i+1}", ""):
                 uncertainty = data[i]
 
     # Reshape arrays if needed
     if len(flux_data) == 1 and len(flux_data.shape) > 1:
         flux_data = np.reshape(flux_data, -1)
         if uncertainty is not None:
             uncertainty = np.reshape(uncertainty, -1)
 
     # Convert uncertainty to StdDevUncertainty array
     if uncertainty is not None:
         uncertainty = StdDevUncertainty(uncertainty)
 
     # Manually generate spectral axis
-    pixels = [[i] + [0]*(wcs.naxis-1) for i in range(wcs.pixel_shape[0])]
+    pixels = [[i] + [0] * (wcs.naxis - 1) for i in range(wcs.pixel_shape[0])]
     spectral_axis = [i[0] for i in wcs.all_pix2world(pixels, 0)] * wcs.wcs.cunit[0]
 
     # Store header as metadata information
-    meta = {'header': header}
+    meta = {"header": header}
 
-    return Spectrum1D(flux=flux_data, spectral_axis=spectral_axis, uncertainty=uncertainty,
-                      meta=meta)
+    return Spectrum1D(flux=flux_data, spectral_axis=spectral_axis, uncertainty=uncertainty, meta=meta)
 
 
-def load_spectrum(filename, spectra_format=None):
-    """Attempt to load the filename as a spectrum object"""
+def load_spectrum(filename: str, spectra_format: str = None, raise_error: bool = False):
+    """Attempt to load the filename as a spectrum object
+
+    Parameters
+    ----------
+    filename
+        Name of the file to read
+    spectra_format
+        Optional file format, passed to Spectrum1D.read.
+        In its absense Spectrum1D.read will attempt to determine the format.
+    raise_error
+        Boolean to control if a failure to read the spectrum should raise an error.
+    """
 
     # Convert filename if using environment variables
-    if filename.startswith('$'):
+    if filename.startswith("$"):
         partial_path, _ = os.path.split(filename)
-        while partial_path != '':
+        while partial_path != "":
             partial_path, envvar_name = os.path.split(partial_path)
         abs_path = os.getenv(envvar_name[1:])
         if abs_path is not None:
             filename = filename.replace(envvar_name, abs_path)
         else:
-            print(f'Could not find environment variable {envvar_name}')
+            print(f"Could not find environment variable {envvar_name}")
 
     try:
         if spectra_format is not None:
             spec1d = Spectrum1D.read(filename, format=spectra_format)
         else:
             spec1d = Spectrum1D.read(filename)
     except Exception as e:  # pylint: disable=broad-except, invalid-name
-        print(f'Error loading {filename}: {e}')
-        spec1d = filename
+        msg = f"Error loading {filename}: {e}"
+
+        # Control whether an error should be explicitly raised if failing to read
+        if raise_error:
+            raise TypeError(msg) from e
+        else:
+            print(msg)
+            spec1d = filename
 
     return spec1d
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/tests/test_astrodb.py` & `astrodbkit2-0.5.2/astrodbkit2/tests/test_astrodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # Testing for astrodb
 
-import os
-import json
-import pytest
 import io
+import json
+import os
+
 import pandas as pd
+import pytest
 import sqlalchemy as sa
-from sqlalchemy.exc import IntegrityError
-from astropy.table import Table
 from astropy.coordinates import SkyCoord
-from astropy.units.quantity import Quantity
 from astropy.io import ascii
-from astrodbkit2.astrodb import Database, create_database, Base, copy_database_schema
-from astrodbkit2.views import view
+from astropy.table import Table
+from astropy.units.quantity import Quantity
+from sqlalchemy.exc import IntegrityError
+
+from astrodbkit2.astrodb import Database, copy_database_schema, create_database
 from astrodbkit2.schema_example import *
+from astrodbkit2.views import view
+
 try:
     import mock
 except ImportError:
     from unittest import mock
 
 
 DB_PATH = 'temp.db'
 
 
 def test_nodatabase():
     connection_string = 'sqlite:///:memory:'
     with pytest.raises(RuntimeError, match='Create database'):
-        db = Database(connection_string)
+        _ = Database(connection_string)
 
 
 @pytest.fixture(scope="module")
 def db_dir(tmpdir_factory):
     return tmpdir_factory.mktemp("data")
 
 
@@ -119,14 +122,39 @@
     sources_data = [{'source': 'Third star',
                      'reference': 'Schm10'}]
     with db.engine.connect() as conn:
         conn.execute(db.Sources.insert().values(sources_data))
         conn.commit()
 
 
+def test_orm_use(db):
+    # Tests using the SQLAlchemy ORM
+
+    # Adding and removing a basic source
+    s = Sources(source="V4046 Sgr", ra=273.54, dec=-32.79, reference="Schm10")
+    with db.session as session:
+        session.add(s)
+        # session.add_all([s])  # if adding a list of entries
+        session.commit()
+
+    assert db.query(db.Sources).filter(db.Sources.c.source == "V4046 Sgr").count() == 1
+
+    # Remove added source so other tests don't include it
+    with db.session as session:
+        session.delete(s)
+        session.commit()
+
+    assert db.query(db.Sources).filter(db.Sources.c.source == "V4046 Sgr").count() == 0
+
+    # Adding a source with problematic ra/dec to test validation
+    with pytest.raises(ValueError):
+        _ = Sources(source="V4046 Sgr", ra=9999, dec=-32.79, reference="Schm10")
+    with pytest.raises(ValueError):
+        _ = Sources(source="V4046 Sgr", ra=273.54, dec=-9999, reference="Schm10")
+    
 
 def test_add_table_data(db):
     # Test the add_table_data method
     file = io.StringIO("""source,band,magnitude,telescope,reference
 2MASS J13571237+1428398,WISE_W3,12.48,WISE,Cutr12
 2MASS J13571237+1428398,WISE_W4,9.56,WISE,Cutr12
 Not in DB,WISE_W4,0,WISE,Cutr12
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/tests/test_utils.py` & `astrodbkit2-0.5.2/astrodbkit2/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Testing for utils
 
-import pytest
 import json
 from datetime import datetime
 from decimal import Decimal
 from io import StringIO
+
+import pytest
 from astropy.table import Table
-from astrodbkit2.utils import json_serializer, get_simbad_names, _name_formatter, datetime_json_parser
+
+from astrodbkit2.utils import _name_formatter, datetime_json_parser, get_simbad_names, json_serializer
+
 try:
     import mock
 except ImportError:
     from unittest import mock
 
 
 @pytest.mark.parametrize('test_input, expected', [
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/tests/test_views.py` & `astrodbkit2-0.5.2/astrodbkit2/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tests for views
 # Adapted from https://github.com/sqlalchemy/sqlalchemy/wiki/Views
 
 import sqlalchemy as sa
-from sqlalchemy.orm import declarative_base
-from sqlalchemy.orm import Session
+from sqlalchemy.orm import Session, declarative_base
+
 from astrodbkit2.views import *
 
 
 def test_views():
     engine = sa.create_engine("sqlite://", echo=True)
     metadata = sa.MetaData()
     stuff = sa.Table(
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/utils.py` & `astrodbkit2-0.5.2/astrodbkit2/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,72 @@
-# Utility functions for Astrodbkit2
+"""Utility functions for Astrodbkit2"""
 
-import re
-import numpy as np
 import functools
+import re
 import warnings
 from datetime import datetime
 from decimal import Decimal
+
 from astroquery.simbad import Simbad
 
-__all__ = ['json_serializer', 'get_simbad_names']
+__all__ = ["json_serializer", "get_simbad_names"]
 
 
 def deprecated_alias(**aliases):
     """
     Decorator from StackOverflow
     https://stackoverflow.com/questions/49802412/how-to-implement-deprecation-in-python-with-argument-alias
     in order to handle deprecation of renamed columns
     To use: add @deprecated_alias(old_name='new_name')
     """
+
     def deco(f):
         @functools.wraps(f)
         def wrapper(*args, **kwargs):
             rename_kwargs(f.__name__, kwargs, aliases)
             return f(*args, **kwargs)
+
         return wrapper
+
     return deco
 
 
 def rename_kwargs(func_name, kwargs, aliases):
     """Helper function used be deprecated_alias"""
     for alias, new in aliases.items():
         if alias in kwargs:
             if new in kwargs:
-                raise TypeError('{} received both {} and {}'.format(
-                    func_name, alias, new))
-            warnings.warn('{} is deprecated; use {}'.format(alias, new),
-                          DeprecationWarning)
+                raise TypeError(f"{func_name} received both {alias} and {new}")
+            warnings.warn(f"{alias} is deprecated; use {new}", DeprecationWarning)
             kwargs[new] = kwargs.pop(alias)
 
 
 def json_serializer(obj):
     """Function describing how things should be serialized in JSON.
     Datetime objects are saved with datetime.isoformat(), Parameter class objects use clean_dict()
-    while all others use __dict__ """
+    while all others use __dict__"""
 
     if isinstance(obj, datetime):
         return obj.isoformat()
 
     if isinstance(obj, Decimal):
         return float(obj)
 
     if isinstance(obj, bytes):
-        return obj.decode('utf-8')
+        return obj.decode("utf-8")
 
     return obj.__dict__
 
 
 def datetime_json_parser(json_dict):
     """Function to convert JSON dictionary objects to datetime when possible.
     This is required to get datetime objects into the database.
     Adapted from: https://stackoverflow.com/questions/8793448/how-to-convert-to-a-python-datetime-object-with-json-loads
     """
-    for (key, value) in json_dict.items():
+    for key, value in json_dict.items():
         if isinstance(value, str):
             try:
                 json_dict[key] = datetime.fromisoformat(value)
             except (ValueError, AttributeError):
                 pass
         else:
             pass
@@ -86,22 +87,22 @@
     Cleaned up name
     """
 
     # Clean up multiple spaces
     name = re.sub(r"\s\s+", " ", name)
 
     # Clean up Simbad types
-    strings_to_delete = ['V* ', 'EM* ', 'NAME ', '** ', 'Cl* ', '* ']
+    strings_to_delete = ["V* ", "EM* ", "NAME ", "** ", "Cl* ", "* "]
     for pattern in strings_to_delete:
-        name = name.replace(pattern, '')
+        name = name.replace(pattern, "")
 
     name = name.strip()
 
     # Clean up 'hidden' names from Simbad
-    if 'HIDDEN' in name.upper():
+    if "HIDDEN" in name.upper():
         name = None
 
     return name
 
 
 def get_simbad_names(name, verbose=False):
     """
@@ -117,13 +118,13 @@
     Returns
     -------
     List of names
     """
 
     t = Simbad.query_objectids(name)
     if t is not None and len(t) > 0:
-        temp = [_name_formatter(s) for s in t['ID'].tolist()]
-        return [s for s in temp if s is not None and s != '']
+        temp = [_name_formatter(s) for s in t["ID"].tolist()]
+        return [s for s in temp if s is not None and s != ""]
     else:
         if verbose:
-            print(f'No Simbad match for {name}')
+            print(f"No Simbad match for {name}")
         return [name]
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2/views.py` & `astrodbkit2-0.5.2/astrodbkit2/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,58 @@
-# Logic to implement and set up views in SQLAlchemy
-# Adapted from https://github.com/sqlalchemy/sqlalchemy/wiki/Views
+"""Logic to implement and set up views in SQLAlchemy
+Adapted from https://github.com/sqlalchemy/sqlalchemy/wiki/Views
+"""
 
 import sqlalchemy as sa
 from sqlalchemy.ext import compiler
 from sqlalchemy.schema import DDLElement
 from sqlalchemy.sql import table
 
+# pylint: disable=abstract-method, missing-function-docstring, unused-argument, redefined-outer-name, protected-access, missing-class-docstring
+
 
 class CreateView(DDLElement):
     def __init__(self, name, selectable):
         self.name = name
         self.selectable = selectable
 
 
 class DropView(DDLElement):
     def __init__(self, name):
         self.name = name
 
 
 @compiler.compiles(CreateView)
 def _create_view(element, compiler, **kw):
+    # pylint: disable=consider-using-f-string
     return "CREATE VIEW %s AS %s" % (
         element.name,
         compiler.sql_compiler.process(element.selectable, literal_binds=True),
     )
 
 
 @compiler.compiles(DropView)
 def _drop_view(element, compiler, **kw):
+    # pylint: disable=consider-using-f-string
     return "DROP VIEW %s" % (element.name)
 
 
 def view_exists(ddl, target, connection, **kw):
     return ddl.name in sa.inspect(connection).get_view_names()
 
 
 def view_doesnt_exist(ddl, target, connection, **kw):
     return not view_exists(ddl, target, connection, **kw)
 
 
 def view(name, metadata, selectable):
     t = table(name)
 
-    t._columns._populate_separate_keys(
-        col._make_proxy(t) for col in selectable.selected_columns
-    )
+    t._columns._populate_separate_keys(col._make_proxy(t) for col in selectable.selected_columns)
 
     sa.event.listen(
         metadata,
         "after_create",
         CreateView(name, selectable).execute_if(callable_=view_doesnt_exist),
     )
-    sa.event.listen(
-        metadata, "before_drop", DropView(name).execute_if(callable_=view_exists)
-    )
+    sa.event.listen(metadata, "before_drop", DropView(name).execute_if(callable_=view_exists))
     return t
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2.egg-info/PKG-INFO` & `astrodbkit2-0.5.2/astrodbkit2.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 Metadata-Version: 2.1
 Name: astrodbkit2
-Version: 0.5.1
+Version: 0.5.2
 Summary: Astronomical database handler code
 Home-page: 
 Author: David Rodriguez
 Author-email: drodriguez@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: licenses/LICENSE.rst
+Requires-Dist: astropy
+Requires-Dist: astroquery
+Requires-Dist: sqlalchemy>=2.0
+Requires-Dist: pandas>=1.0.4
+Requires-Dist: packaging
+Requires-Dist: specutils>=1.0
+Requires-Dist: tqdm
+Provides-Extra: all
+Requires-Dist: astrodbkit2[docs,test]; extra == "all"
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-astropy; extra == "test"
+Requires-Dist: darker==1.7.2; extra == "test"
+Requires-Dist: black==23.9.1; extra == "test"
+Requires-Dist: pre-commit==3.4.0; extra == "test"
+Requires-Dist: ruff==0.3.7; extra == "test"
 Provides-Extra: docs
-License-File: licenses/LICENSE.rst
+Requires-Dist: sphinx-astropy; extra == "docs"
 
 Astronomical database handler code
 ----------------------------------
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
-.. image:: https://github.com/dr-rodriguez/AstrodbKit2/workflows/Test%20Astrodbkit2/badge.svg?branch=main
-    :target: https://github.com/dr-rodriguez/AstrodbKit2/actions
+.. image:: https://github.com/astrodbtoolkit/AstrodbKit2/workflows/Test%20Astrodbkit2/badge.svg?branch=main
+    :target: https://github.com/astrodbtoolkit/AstrodbKit2/actions
 
-.. image:: https://codecov.io/gh/dr-rodriguez/AstrodbKit2/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/dr-rodriguez/AstrodbKit2
+.. image:: https://codecov.io/gh/astrodbtoolkit/AstrodbKit2/graph/badge.svg?token=LMKVN65D82 
+    :target: https://codecov.io/gh/astrodbtoolkit/AstrodbKit2
 
 AstrodbKit2 is an astronomical database handler code built on top of SQLAlchemy.
-This is built to work with the `SIMPLE database <https://github.com/kelle/SIMPLE>`_, though
+This is built to work with the `SIMPLE database <https://github.com/SIMPLE-AstroDB/SIMPLE-db>`_, though
 similarly constructed databases will work.
 
 Documentation is available at `https://astrodbkit2.readthedocs.io/en/latest/ <https://astrodbkit2.readthedocs.io/en/latest/>`_
 
 License
 -------
```

### Comparing `astrodbkit2-0.5.1/astrodbkit2.egg-info/SOURCES.txt` & `astrodbkit2-0.5.2/astrodbkit2.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .codecov.yml
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yml
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 .devcontainer/devcontainer.json
```

### Comparing `astrodbkit2-0.5.1/docs/Makefile` & `astrodbkit2-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5.1/docs/conf.py` & `astrodbkit2-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5.1/docs/index.rst` & `astrodbkit2-0.5.2/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,18 @@
     db.query(db.Sources).table()    # equivalent to astropy
     db.query(db.Sources).pandas()   # Pandas DataFrame
 
 Example query for sources with declinations larger than 0::
 
     db.query(db.Sources).filter(db.Sources.c.dec > 0).table()
 
+Example query for rows with missing data::
+
+    db.query(db.Publications).filter(db.Publications.c.doi.is_(None)).table()
+
 Example query returning just a single column (source) and sorting sources by declination::
 
     db.query(db.Sources.c.source).order_by(db.Sources.c.dec).table()
 
 Example query joining Sources and Publications tables and return just several of the columns::
 
     db.query(db.Sources.c.source, db.Sources.c.reference, db.Publications.c.name)\
@@ -413,14 +417,66 @@
 
     # Save entire database to directory 'data'
     db.save_database('data')
 
 .. note:: To properly capture database deletes, the contents of the specified directory is first cleared before
           creating JSON files representing the current state of the database.
 
+Using the SQLAlchemy ORM
+========================
+
+The SQLAlchemy ORM (Object Relational Mapping) can be used for many of the examples provided above. 
+This also allows for adding extra functionality to your schema, such as validation.
+
+For example, the schema of your sources table could be written to validate RA/Dec as follows::
+
+    from sqlalchemy import Column, Float, String
+    from sqlalchemy.orm import validates
+
+    class Sources(Base):
+        """ORM for the sources table. This stores the main identifiers for our objects along with ra and dec"""
+
+        __tablename__ = "Sources"
+        source = Column(String(100), primary_key=True, nullable=False)
+        ra = Column(Float)
+        dec = Column(Float)
+
+        @validates("ra")
+        def validate_ra(self, key, value):
+            if value > 360 or value < 0:
+                raise ValueError("RA not in allowed range (0..360)")
+            return value
+        
+        @validates("dec")
+        def validate_dec(self, key, value):
+            if value > 90 or value < -90:
+                raise ValueError("Dec not in allowed range (-90..90)")
+            return value
+
+In your scripts, you can then create objects and populate them accordingly.
+For example::
+
+    from astrodbkit2.astrodb import Database
+    from schema import Sources
+
+    db = Database(connection_string)
+
+    # Create a new object and insert to database
+    s = Sources(source="V4046 Sgr", ra=273.54, dec=-32.79)
+    with db.session as session:
+        session.add(s)
+        session.commit()
+
+If the RA or Dec fail the validation checks, the creation of the object will raise a ValueError exception. 
+
+One can also use `session.add_all()` to insert a list of table entries and `session.delete()` to delete a single one. 
+These options can facilitate the creation of robust ingest scripts that are both intuitive (ie, instantiating objects in a pythonic way) 
+and that can take care of validating input values before they get to the database.
+
+
 Reference/API
 =============
 
 .. toctree::
    :maxdepth: 2
 
    astrodb.rst
```

### Comparing `astrodbkit2-0.5.1/docs/make.bat` & `astrodbkit2-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5.1/licenses/LICENSE.rst` & `astrodbkit2-0.5.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5.1/setup.cfg` & `astrodbkit2-0.5.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -26,27 +26,32 @@
 	tqdm
 
 [options.entry_points]
 console_scripts = 
 	astropy-package-template-example = packagename.example_mod:main
 
 [options.extras_require]
+all = 
+	astrodbkit2[test, docs]
 test = 
+	pytest
+	pytest-cov
 	pytest-astropy
+	darker==1.7.2
+	black==23.9.1
+	pre-commit==3.4.0
+	ruff==0.3.7
 docs = 
 	sphinx-astropy
 
 [options.package_data]
 astrodbkit2 = data/*
 
 [tool:pytest]
 testpaths = "astrodbkit2"
-astropy_header = true
-doctest_plus = enabled
-text_file_format = rst
 
 [coverage:run]
 omit = 
 	astrodbkit2/_astropy_init*
 	astrodbkit2/conftest.py
 	astrodbkit2/*setup_package*
 	astrodbkit2/tests/*
```

### Comparing `astrodbkit2-0.5.1/setup.py` & `astrodbkit2-0.5.2/setup.py`

 * *Files identical despite different names*

