# Comparing `tmp/jaraco.crypto-4.0.0.tar.gz` & `tmp/jaraco_crypto-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.crypto-4.0.0.tar", last modified: Fri Aug 11 18:49:45 2023, max compression
+gzip compressed data, was "jaraco_crypto-4.0.1.tar", last modified: Fri Apr 19 16:18:43 2024, max compression
```

## Comparing `jaraco.crypto-4.0.0.tar` & `jaraco_crypto-4.0.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.524196 jaraco.crypto-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.520196 jaraco.crypto-4.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.520196 jaraco.crypto-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-11 18:49:45.524196 jaraco.crypto-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.524196 jaraco.crypto-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.520196 jaraco.crypto-4.0.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.524196 jaraco.crypto-4.0.0/jaraco/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/evp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.524196 jaraco.crypto-4.0.0/jaraco/crypto/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/tests/test_cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/tests/test_digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/tests/test_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/jaraco/crypto/tests/test_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 18:49:45.524196 jaraco.crypto-4.0.0/jaraco.crypto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-11 18:49:45.000000 jaraco.crypto-4.0.0/jaraco.crypto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-11 18:49:45.000000 jaraco.crypto-4.0.0/jaraco.crypto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-11 18:49:45.000000 jaraco.crypto-4.0.0/jaraco.crypto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-11 18:49:45.000000 jaraco.crypto-4.0.0/jaraco.crypto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-11 18:49:45.000000 jaraco.crypto-4.0.0/jaraco.crypto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-11 18:49:45.524196 jaraco.crypto-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-11 18:49:25.000000 jaraco.crypto-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.245946 jaraco_crypto-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.237945 jaraco_crypto-4.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.237945 jaraco_crypto-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-19 16:18:43.245946 jaraco_crypto-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.237945 jaraco_crypto-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.233945 jaraco_crypto-4.0.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.241945 jaraco_crypto-4.0.1/jaraco/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/evp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.241945 jaraco_crypto-4.0.1/jaraco/crypto/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/tests/test_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/tests/test_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/tests/test_rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/jaraco/crypto/tests/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:18:43.241945 jaraco_crypto-4.0.1/jaraco.crypto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-19 16:18:43.000000 jaraco_crypto-4.0.1/jaraco.crypto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-19 16:18:43.000000 jaraco_crypto-4.0.1/jaraco.crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:18:43.000000 jaraco_crypto-4.0.1/jaraco.crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 16:18:43.000000 jaraco_crypto-4.0.1/jaraco.crypto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 16:18:43.000000 jaraco_crypto-4.0.1/jaraco.crypto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:18:43.245946 jaraco_crypto-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-19 16:18:23.000000 jaraco_crypto-4.0.1/tox.ini
```

### Comparing `jaraco.crypto-4.0.0/.github/workflows/main.yml` & `jaraco_crypto-4.0.1/.github/workflows/main.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,99 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
-  # Environment variables to support color support (jaraco/skeleton#66):
-  # Request colored output from CLI tools supporting it. Different tools
-  # interpret the value differently. For some, just being set is sufficient.
-  # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient. For tox, it must be one of
-  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
-  # in common is "1".
+  # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
-  # MyPy's color enforcement (must be a non-zero number)
-  MYPY_FORCE_COLOR: -42
-  # Recognized by the `py` package, dependency of `pytest` (must be "1")
-  PY_COLORS: 1
-  # Make tox-wrapped tools see color requests
-  TOX_TESTENV_PASSENV: >-
-    FORCE_COLOR
-    MYPY_FORCE_COLOR
-    NO_COLOR
-    PY_COLORS
-    PYTEST_THEME
-    PYTEST_THEME_MODE
 
   # Suppress noisy pip warnings
   PIP_DISABLE_PIP_VERSION_CHECK: 'true'
   PIP_NO_PYTHON_VERSION_WARNING: 'true'
   PIP_NO_WARN_SCRIPT_LOCATION: 'true'
 
-  # Disable the spinner, noise in GHA; TODO(webknjaz): Fix this upstream
-  # Must be "1".
-  TOX_PARALLEL_NO_SPINNER: 1
+  # Ensure tests can sense settings about the environment
+  TOX_OVERRIDE: >-
+    testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
-        - python: pypy3.9
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.12' }}
+    continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox
 
-  docs:
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
-    env:
-      TOXENV: docs
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run
-        run: tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    - docs
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
@@ -105,20 +104,19 @@
       contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.crypto-4.0.0/LICENSE` & `jaraco_crypto-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-4.0.0/NEWS.rst` & `jaraco_crypto-4.0.1/NEWS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v4.0.1
+======
+
+No significant changes.
+
+
 v4.0.0
 ======
 
 Deprecations and Removals
 -------------------------
 
 - Removed blowfish. Use pypi/blowfish instead.
```

### Comparing `jaraco.crypto-4.0.0/PKG-INFO` & `jaraco_crypto-4.0.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,24 @@
-Metadata-Version: 2.1
-Name: jaraco.crypto
-Version: 4.0.0
-Summary: Cryptography support by jaraco
-Home-page: https://github.com/jaraco/jaraco.crypto
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: LICENSE
-
 .. image:: https://img.shields.io/pypi/v/jaraco.crypto.svg
    :target: https://pypi.org/project/jaraco.crypto
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.crypto.svg
 
-.. image:: https://github.com/jaraco/jaraco.crypto/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.crypto/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.crypto/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/jaracocrypto/badge/?version=latest
    :target: https://jaracocrypto.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 A set of cryptographic routines and utilities
 implemented in pure Python.
 
 ================
 Acknowledgements
```

### Comparing `jaraco.crypto-4.0.0/docs/index.rst` & `jaraco_crypto-4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/cert.py` & `jaraco_crypto-4.0.1/jaraco/crypto/cert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import ctypes
 
 from .support import find_library
 
 
 class Stack(ctypes.Structure):
     _fields_ = [
-        ('num', ctypes.c_int),
-        ('data', ctypes.POINTER(ctypes.c_char_p)),
-        ('sorted', ctypes.c_int),
-        ('num_alloc', ctypes.c_int),
-        ('comp', ctypes.c_void_p),
+        ("num", ctypes.c_int),
+        ("data", ctypes.POINTER(ctypes.c_char_p)),
+        ("sorted", ctypes.c_int),
+        ("num_alloc", ctypes.c_int),
+        ("comp", ctypes.c_void_p),
     ]
 
 
 class CRYPTO_EX_DATA(ctypes.Structure):
     _fields_ = [
-        ('sk', ctypes.c_void_p),
-        ('dummy', ctypes.c_int),
+        ("sk", ctypes.c_void_p),
+        ("dummy", ctypes.c_int),
     ]
 
 
 class BIO(ctypes.Structure):
     _fields_ = [
-        ('method', ctypes.c_void_p),
-        ('callback', ctypes.c_void_p),
-        ('cb_arg', ctypes.c_char_p),
-        ('init', ctypes.c_int),
-        ('shutdown', ctypes.c_int),
-        ('flags', ctypes.c_int),
-        ('retry_reason', ctypes.c_int),
-        ('num', ctypes.c_int),
-        ('ptr', ctypes.c_void_p),
-        ('next_bio', ctypes.c_void_p),
-        ('prev_bio', ctypes.c_void_p),
-        ('references', ctypes.c_int),
-        ('num_read', ctypes.c_ulong),
-        ('num_write', ctypes.c_ulong),
-        ('ex_data', CRYPTO_EX_DATA),
+        ("method", ctypes.c_void_p),
+        ("callback", ctypes.c_void_p),
+        ("cb_arg", ctypes.c_char_p),
+        ("init", ctypes.c_int),
+        ("shutdown", ctypes.c_int),
+        ("flags", ctypes.c_int),
+        ("retry_reason", ctypes.c_int),
+        ("num", ctypes.c_int),
+        ("ptr", ctypes.c_void_p),
+        ("next_bio", ctypes.c_void_p),
+        ("prev_bio", ctypes.c_void_p),
+        ("references", ctypes.c_int),
+        ("num_read", ctypes.c_ulong),
+        ("num_write", ctypes.c_ulong),
+        ("ex_data", CRYPTO_EX_DATA),
     ]
 
 
 FILETYPE_PEM = 1
 FILETYPE_ASN1 = 2
 
-lib = find_library('libcrypto') or find_library('libssl')
+lib = find_library("libcrypto") or find_library("libssl")
 assert lib, "Couldn't find OpenSSL"
 
 lib.BN_bn2hex.restype = ctypes.c_char_p
 
 
 class X509(ctypes.Structure):
     _fields_ = []  # type: ignore
@@ -74,12 +74,12 @@
     finally:
         lib.BIO_free(bio)
     if not cert:
         raise Exception("Exception loading cert")
     return ctypes.cast(cert, ctypes.POINTER(X509)).contents
 
 
-if __name__ == '__main__':
-    with open('server.pem', 'rb') as certfile:
+if __name__ == "__main__":
+    with open("server.pem", "rb") as certfile:
         cert_data = certfile.read()
     cert = load_certificate(FILETYPE_PEM, cert_data)
     print(cert.get_serial_number())
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/cipher.py` & `jaraco_crypto-4.0.1/jaraco/crypto/cipher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ctypes
 
-
 from . import evp
 
 CIPHER_ALGORITHMS = ("DES", "DES-EDE3", "BF", "AES-128", "AES-192", "AES-256")
 CIPHER_MODES = ("CBC", "CFB", "OFB", "ECB")
 
 
 class CipherError(Exception):
@@ -19,23 +18,21 @@
         """
         Create a CipherType from a cipher name.
 
         Takes one or two parameters. If one is supplied, it should be
         a dash-separated string of algorithm-mode.
         If two are supplied, they should be the algorithm and mode.
         """
-        cipher_name = '-'.join(cipher_name)
-        algorithm, mode = cipher_name.rsplit('-', 1)
-        assert algorithm in CIPHER_ALGORITHMS, (
-            "Unknown algorithm %(algorithm)s" % vars()
-        )
-        assert mode in CIPHER_MODES, "Unknown mode %(mode)s" % vars()
-        res = evp.get_cipherbyname(cipher_name.encode('ascii'))
+        cipher_name = "-".join(cipher_name)
+        algorithm, mode = cipher_name.rsplit("-", 1)
+        assert algorithm in CIPHER_ALGORITHMS, f"Unknown algorithm {algorithm}"
+        assert mode in CIPHER_MODES, f"Unknown mode {mode}"
+        res = evp.get_cipherbyname(cipher_name.encode("ascii"))
         if not res:
-            raise CipherError("Unknown cipher: %(cipher_name)s" % vars())
+            raise CipherError(f"Unknown cipher: {cipher_name}")
         res.contents.algorithm, res.contents.mode = algorithm, mode
         return res.contents
 
 
 class Cipher(ctypes.Structure):
     _fields_ = evp._cipher_context_fields
     finalized = False
@@ -43,27 +40,27 @@
     def __new__(cls, *a, **kw):
         return evp.lib.EVP_CIPHER_CTX_new().contents
 
     def __del__(self):
         evp.lib.EVP_CIPHER_CTX_free(self)
 
     def __init__(self, type, key, iv, encrypt=True):
-        key = key.encode('ascii')
-        iv = iv.encode('ascii')
+        key = key.encode("ascii")
+        iv = iv.encode("ascii")
         engine = None
         type = self.interpret_type(type)
         res = evp.CipherInit_ex(self, type, engine, key, iv, encrypt)
         if res == 0:
             raise CipherError(f"Unable to initialize cipher: {evp.get_error()}")
         self.out_data = []
 
     @staticmethod
     def interpret_type(type):
         if not isinstance(type, CipherType):
-            if not hasattr(type, '__iter__'):
+            if not hasattr(type, "__iter__"):
                 type = [type]
             type = CipherType.from_name(*type)
         return type
 
     def set_padding(self, padding=True):
         evp.CIPHER_CTX_set_padding(self, padding)
 
@@ -99,16 +96,16 @@
         self.finalized = True
         out = ctypes.create_string_buffer(evp.MAX_BLOCK_LENGTH)
         out_len = ctypes.c_int()
         res = evp.CipherFinal_ex(self, out, out_len)
         if res != 1:
             raise CipherError(f"Error finalizing cipher: {evp.get_error()}")
         self.out_data.append(out.raw[: out_len.value])
-        self.finalize = lambda: ''.join(self.out_data)
-        return b''.join(self.out_data)
+        self.finalize = lambda: "".join(self.out_data)
+        return b"".join(self.out_data)
 
 
 evp.get_cipherbyname.argtypes = (ctypes.c_char_p,)  # type: ignore
 evp.get_cipherbyname.restype = ctypes.POINTER(CipherType)  # type: ignore
 
 
 # https://www.openssl.org/docs/man3.1/man3/EVP_CipherInit_ex.html
@@ -131,15 +128,15 @@
 _final_args = (
     ctypes.POINTER(Cipher),  # ctx
     ctypes.c_char_p,  # out[m]
     ctypes.POINTER(ctypes.c_int),  # outl
 )
 evp.EncryptInit_ex.argtypes = (  # type: ignore
     evp.DecryptInit_ex.argtypes  # type: ignore
-) = (_init_args[:2] + _init_args[3:5])
+) = _init_args[:2] + _init_args[3:5]
 evp.CipherInit_ex.argtypes = _init_args  # type: ignore
 evp.EncryptUpdate.argtypes = (  # type: ignore
     evp.DecryptUpdate.argtypes  # type: ignore
 ) = evp.CipherUpdate.argtypes = _update_args  # type: ignore
 evp.EncryptFinal_ex.argtypes = (  # type: ignore
     evp.DecryptFinal_ex.argtypes  # type: ignore
 ) = evp.CipherFinal_ex.argtypes = _final_args  # type: ignore
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/digest.py` & `jaraco_crypto-4.0.1/jaraco/crypto/digest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import ctypes
 
-
 from . import evp
 
 
 class DigestError(Exception):
     pass
 
 
 class DigestType(ctypes.Structure):
     _fields_ = evp._digest_type_fields
 
     @classmethod
     def from_name(cls, digest_name):
-        res = evp.get_digestbyname(digest_name.encode('ascii'))
+        res = evp.get_digestbyname(digest_name.encode("ascii"))
         if not res:
-            raise DigestError("Unknown Digest: %(digest_name)s" % vars())
+            raise DigestError(f"Unknown Digest: {digest_name}")
         return res.contents
 
 
 class Digest(ctypes.Structure):
     _fields_ = evp._digest_context_fields
     finalized = False
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/evp.py` & `jaraco_crypto-4.0.1/jaraco/crypto/evp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,76 @@
-import itertools
 import ctypes
+import itertools
 from ctypes import (
+    POINTER,
+    c_char,
+    c_char_p,
     c_int,
+    c_uint,
     c_ulong,
     c_void_p,
-    c_char_p,
-    POINTER,
-    c_uint,
-    c_char,
 )
 
 from .support import find_library
 
-
 get_digestbyname = None
 DigestInit = None
 DigestInit_ex = None
 DigestUpdate = None
 DigestFinal_ex = None
 get_cipherbyname = None
 
 MAX_MD_SIZE = 64
 
 _digest_type_fields = [
-    ('type', c_int),
-    ('pkey_type', c_int),
-    ('md_size', c_int),
-    ('flags', c_ulong),
-    ('init', c_void_p),
-    ('update', c_void_p),
-    ('final', c_void_p),
-    ('copy', c_void_p),
-    ('cleanup', c_void_p),
-    ('sign', c_void_p),
-    ('verify', c_void_p),
-    ('required_pkey_type', c_int * 5),
-    ('block_size', c_int),
-    ('ctx_size', c_int),
-    ('md_ctrl', c_void_p),
+    ("type", c_int),
+    ("pkey_type", c_int),
+    ("md_size", c_int),
+    ("flags", c_ulong),
+    ("init", c_void_p),
+    ("update", c_void_p),
+    ("final", c_void_p),
+    ("copy", c_void_p),
+    ("cleanup", c_void_p),
+    ("sign", c_void_p),
+    ("verify", c_void_p),
+    ("required_pkey_type", c_int * 5),
+    ("block_size", c_int),
+    ("ctx_size", c_int),
+    ("md_ctrl", c_void_p),
 ]
 
 _digest_context_fields = [
-    ('p_type', c_void_p),  # POINTER(DigestType)
-    ('engine', c_void_p),  # todo, POINTER(ENGINE)
-    ('flags', c_ulong),
-    ('md_data', c_void_p),
-    ('pctx', c_void_p),  # todo, POINTER(EVP_PKEY_CTX)
-    ('update_func', c_void_p),
+    ("p_type", c_void_p),  # POINTER(DigestType)
+    ("engine", c_void_p),  # todo, POINTER(ENGINE)
+    ("flags", c_ulong),
+    ("md_data", c_void_p),
+    ("pctx", c_void_p),  # todo, POINTER(EVP_PKEY_CTX)
+    ("update_func", c_void_p),
 ]
 
 
 def _reg(name):
     """
     Copy the function by the given name from the EVP library into this
     namespace.
     """
-    libname = 'EVP_' + name
+    libname = "EVP_" + name
     globals()[name] = getattr(lib, libname)
 
 
-lib = find_library('libcrypto') or find_library('libssl')
+lib = find_library("libcrypto") or find_library("libssl")
 assert lib, "Couldn't find OpenSSL"
 
 # Define the argtypes and result types for the EVP functions
 list(
     map(
         _reg,
-        'get_digestbyname DigestInit DigestInit_ex '
-        'DigestUpdate DigestFinal_ex CIPHER_CTX_set_padding'.split(),
+        "get_digestbyname DigestInit DigestInit_ex "
+        "DigestUpdate DigestFinal_ex CIPHER_CTX_set_padding".split(),
     )
 )
 
 
 def _set_digest_arg_types(DigestType, Digest):
     get_digestbyname.argtypes = (c_char_p,)
     get_digestbyname.restype = POINTER(DigestType)
@@ -96,64 +95,64 @@
     DigestFinal_ex.restype = c_int
     lib.EVP_MD_CTX_new.restype = POINTER(Digest)
     lib.EVP_MD_CTX_new.argtypes = None
     lib.EVP_MD_CTX_free.restype = None
     lib.EVP_MD_CTX_free.argtypes = (POINTER(Digest),)
 
 
-_reg('get_cipherbyname')
+_reg("get_cipherbyname")
 
 
 _cipher_fields = [
-    ('nid', c_int),
-    ('block_size', c_int),
-    ('key_len', c_int),
-    ('iv_len', c_int),
-    ('flags', c_ulong),
-    ('init', c_void_p),
-    ('do_cipher', c_void_p),
-    ('cleanup', c_void_p),
-    ('ctx_size', c_int),
-    ('set_asn1_parameters', c_void_p),
-    ('get_asn1_parameters', c_void_p),
-    ('ctrl', c_void_p),
-    ('app_data', c_void_p),
+    ("nid", c_int),
+    ("block_size", c_int),
+    ("key_len", c_int),
+    ("iv_len", c_int),
+    ("flags", c_ulong),
+    ("init", c_void_p),
+    ("do_cipher", c_void_p),
+    ("cleanup", c_void_p),
+    ("ctx_size", c_int),
+    ("set_asn1_parameters", c_void_p),
+    ("get_asn1_parameters", c_void_p),
+    ("ctrl", c_void_p),
+    ("app_data", c_void_p),
 ]
 
 MAX_IV_LENGTH = 16
 MAX_BLOCK_LENGTH = 32
 MAX_KEY_LENGTH = 32
 
 _cipher_context_fields = [
-    ('cipher', c_void_p),  # POINTER(CipherType)
-    ('engine', c_void_p),  # POINTER(ENGINE)
-    ('encrypt', c_int),
-    ('buf_len', c_int),
-    ('oiv', c_char * MAX_IV_LENGTH),
-    ('iv', c_char * MAX_IV_LENGTH),
-    ('buf', c_char * MAX_BLOCK_LENGTH),
-    ('num', c_int),
-    ('app_data', c_void_p),
-    ('key_len', c_int),
-    ('flags', c_ulong),
-    ('cipher_data', c_void_p),
-    ('final_used', c_int),
-    ('block_mask', c_int),
-    ('final', c_char * MAX_BLOCK_LENGTH),
+    ("cipher", c_void_p),  # POINTER(CipherType)
+    ("engine", c_void_p),  # POINTER(ENGINE)
+    ("encrypt", c_int),
+    ("buf_len", c_int),
+    ("oiv", c_char * MAX_IV_LENGTH),
+    ("iv", c_char * MAX_IV_LENGTH),
+    ("buf", c_char * MAX_BLOCK_LENGTH),
+    ("num", c_int),
+    ("app_data", c_void_p),
+    ("key_len", c_int),
+    ("flags", c_ulong),
+    ("cipher_data", c_void_p),
+    ("final_used", c_int),
+    ("block_mask", c_int),
+    ("final", c_char * MAX_BLOCK_LENGTH),
 ]
 
 # EncryptInit_ex = lib.EVP_EncryptInit_ex
 # DecryptInit_ex = lib.EVP_DecryptInit_ex
 # ...
 for ed, method in itertools.product(
-    ['Encrypt', 'Decrypt', 'Cipher'],
-    ['Init_ex', 'Update', 'Final_ex'],
+    ["Encrypt", "Decrypt", "Cipher"],
+    ["Init_ex", "Update", "Final_ex"],
 ):
-    local_name = ''.join([ed, method])
-    lib_name = ''.join(['EVP_', ed, method])
+    local_name = "".join([ed, method])
+    lib_name = "".join(["EVP_", ed, method])
     func = getattr(lib, lib_name)
     func.restype = c_int
     globals()[local_name] = func
 
 
 def get_error():
     err = lib.ERR_get_error()
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/rand.py` & `jaraco_crypto-4.0.1/jaraco/crypto/rand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ctypes
 
-
 from .evp import lib
 
 
 class RandError(Exception):
     pass
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/support.py` & `jaraco_crypto-4.0.1/jaraco/crypto/support.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
+import contextlib
 import ctypes
+import glob
+import itertools
 import os
 import platform
 import subprocess
-import glob
-import contextlib
-import itertools
 
 
 def _run_cmd(cmd):
-    return subprocess.check_output(cmd.split(' '), text=True, encoding='utf-8')
+    return subprocess.check_output(cmd.split(" "), text=True, encoding="utf-8")
 
 
 def find_lib_Linux(lib_name):
-    for line in _run_cmd('ldconfig -p').splitlines():
-        lib, _, rest = line.strip().partition(' ')
-        _, _, path = rest.rpartition(' ')
-        found_name, _, _ = lib.partition('.')
+    for line in _run_cmd("ldconfig -p").splitlines():
+        lib, _, rest = line.strip().partition(" ")
+        _, _, path = rest.rpartition(" ")
+        found_name, _, _ = lib.partition(".")
         if lib_name == found_name:
             return path
 
 
 def find_library(lib_name):
     """
     Given a name like libcrypto, find the best match and load it.
     """
-    func = globals()[f'find_lib_{platform.system()}']
+    func = globals()[f"find_lib_{platform.system()}"]
     found = func(lib_name)
     return found and ctypes.cdll.LoadLibrary(found)
 
 
 def _brew_paths():
     with contextlib.suppress(subprocess.CalledProcessError):
-        yield _run_cmd('brew --prefix openssl').strip() + '/lib'
+        yield _run_cmd("brew --prefix openssl").strip() + "/lib"
 
 
 def find_lib_Darwin(lib_name):
     heuristic_paths = [
-        '/usr/local/opt/openssl/lib/',
+        "/usr/local/opt/openssl/lib/",
     ]
     search_paths = itertools.chain(_brew_paths(), heuristic_paths)
-    return _search(lib_name, search_paths, '.dylib')
+    return _search(lib_name, search_paths, ".dylib")
 
 
 def find_lib_Windows(lib_name):
     """
     Default OpenSSL installs to the Windows system folder and are
     reachable without a path or extension, but must have the right
     name.
     """
     heuristic_paths = [
-        'C:\\Program Files\\OpenSSL',
-        '\\OpenSSL-Win64',
-        'C:\\Program Files\\OpenSSL-Win64-ARM',
+        "C:\\Program Files\\OpenSSL",
+        "\\OpenSSL-Win64",
+        "C:\\Program Files\\OpenSSL-Win64-ARM",
     ]
-    search_paths = os.environ['PATH'].split(os.pathsep) + heuristic_paths
-    return _search(lib_name, search_paths, '.dll')
+    search_paths = os.environ["PATH"].split(os.pathsep) + heuristic_paths
+    return _search(lib_name, search_paths, ".dll")
 
 
 def _search(lib_name, paths, ext):
     names = (
         name
         for path in paths
-        for name in glob.glob(path + os.sep + f'{lib_name}*{ext}')
+        for name in glob.glob(path + os.sep + f"{lib_name}*{ext}")
     )
 
     return next(names, None)
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/tests/test_cipher.py` & `jaraco_crypto-4.0.1/jaraco/crypto/tests/test_cipher.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 from jaraco.crypto import cipher
 
 
 def algorithm_modes():
     pairs = itertools.product(cipher.CIPHER_ALGORITHMS, cipher.CIPHER_MODES)
     for algorithm, mode in pairs:
         # apparently DES-EDE3-ECB is not a valid mode
-        if (algorithm, mode) == ('DES-EDE3', 'ECB'):
+        if (algorithm, mode) == ("DES-EDE3", "ECB"):
             continue
         yield algorithm, mode
 
 
-@pytest.mark.parametrize(['algorithm', 'mode'], algorithm_modes())
+@pytest.mark.parametrize(["algorithm", "mode"], algorithm_modes())
 def test_cipher_type(algorithm, mode):
     # One can pass the algorithm and mode separately or together
     cipher.CipherType.from_name(algorithm, mode)
-    cipher.CipherType.from_name(algorithm + '-' + mode)
+    cipher.CipherType.from_name(algorithm + "-" + mode)
 
 
 @pytest.mark.parametrize(
-    'data_parts', [('a' * i, 'b' * i, 'c' * i) for i in range(0, 1000, 50)]
+    "data_parts", [("a" * i, "b" * i, "c" * i) for i in range(0, 1000, 50)]
 )
 def test_cipher(data_parts):
     """
     Encrypt and decrypt the data_parts supplied and ensure the source
     matches the result.
     """
-    key = '11111111111111111111111111111111'
-    iv = '1111111111111111'
-    params = ('AES-256', 'CBC'), key, iv
+    key = "11111111111111111111111111111111"
+    iv = "1111111111111111"
+    params = ("AES-256", "CBC"), key, iv
     ce = cipher.Cipher(*params)
     list(map(ce.update, data_parts))
     data_enc = ce.finalize()
     cd = cipher.Cipher(*params, encrypt=False)
-    assert cd.finalize(data_enc) == ''.join(data_parts).encode()
+    assert cd.finalize(data_enc) == "".join(data_parts).encode()
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/tests/test_digest.py` & `jaraco_crypto-4.0.1/jaraco/crypto/tests/test_digest.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import pytest
 
 from jaraco.crypto import digest
 
 
 def test_load_valid_digest_type_by_name():
-    digest.DigestType.from_name('SHA256')
+    digest.DigestType.from_name("SHA256")
 
 
 def test_load_invalid_digest_type_by_name():
     # dne is Does Not Exist
-    pytest.raises(digest.DigestError, digest.DigestType.from_name, 'sha-dne')
+    pytest.raises(digest.DigestError, digest.DigestType.from_name, "sha-dne")
 
 
 def test_digest():
-    digest_type = digest.DigestType.from_name('SHA512')
+    digest_type = digest.DigestType.from_name("SHA512")
     sha512 = digest.Digest(digest_type)
     sha512.update("test")
     assert not sha512.finalized
     digest_ = sha512.digest()
-    digest_str = binascii.hexlify(digest_).decode('ascii')
+    digest_str = binascii.hexlify(digest_).decode("ascii")
     assert len(digest_) == 64
     assert digest_str == (
         "ee26b0dd4af7e749aa1a8ee3c10ae992"
         "3f618980772e473f8819a5d4940e0db2"
         "7ac185f8a0e1d5f84f88bc887fd67b14"
         "3732c304cc5fa9ad8e6f57f50028a8ff"
     )
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/tests/test_rand.py` & `jaraco_crypto-4.0.1/jaraco/crypto/tests/test_rand.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     bytes = rand.pseudo_bytes(100)
     assert len(bytes) == 100
     assert bytes != rand.pseudo_bytes(100)
 
 
 def test_seed():
     pytest.skip("This fails, why?")
-    seed = 'bunch of bytes' * 1000
+    seed = "bunch of bytes" * 1000
     rand.cleanup()
     rand.seed(seed)
     bytes1 = rand.pseudo_bytes(100)
     rand.cleanup()
     rand.seed(seed)
     bytes2 = rand.pseudo_bytes(100)
     assert bytes1 == bytes2
```

### Comparing `jaraco.crypto-4.0.0/jaraco/crypto/tests/test_threads.py` & `jaraco_crypto-4.0.1/jaraco/crypto/tests/test_threads.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from threading import Thread
 
-from . import test_cipher
-from . import test_digest
+from . import test_cipher, test_digest
 
 
 class ThreadedTester(Thread):
     failed = False
 
     def run(self):
         try:
             test_digest.test_digest()
-            test_cipher.test_cipher(['a' * 1000, 'd' * 1000])
+            test_cipher.test_cipher(["a" * 1000, "d" * 1000])
             # test_evp.test_rand()
         except Exception as e:
             self.failed = True
             self.exception = e
 
 
 def test_threaded_crypto():
     threads = [ThreadedTester() for i in range(10)]
     map(lambda t: t.start(), threads)
     # wait for the threads to complete
     map(lambda t: t.join(), threads)
     assert all(not t.failed for t in threads), "Some threads failed"
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test_threaded_crypto()
```

### Comparing `jaraco.crypto-4.0.0/jaraco.crypto.egg-info/SOURCES.txt` & `jaraco_crypto-4.0.1/jaraco.crypto.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 LICENSE
 NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
-setup.cfg
+ruff.toml
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
```

### Comparing `jaraco.crypto-4.0.0/pytest.ini` & `jaraco_crypto-4.0.1/pytest.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [pytest]
 norecursedirs=dist build .tox .eggs
-addopts=--doctest-modules
+addopts=
+	--doctest-modules
+	--import-mode importlib
+consider_namespace_packages=true
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# shopkeep/pytest-black#55
-	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
-	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
-
-	# shopkeep/pytest-black#67
-	ignore:'encoding' argument not specified::pytest_black
-
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
 	# pypa/build#615
 	ignore:'encoding' argument not specified::build.env
 
+	# dateutil/dateutil#1284
+	ignore:datetime.datetime.utcfromtimestamp:DeprecationWarning:dateutil.tz.tz
+
 	## end upstream
 
 	# itsdangerous is pinned to old version
 	ignore:datetime.utcfromtimestamp\(\) is deprecated::itsdangerous
```

