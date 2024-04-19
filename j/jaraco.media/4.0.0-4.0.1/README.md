# Comparing `tmp/jaraco.media-4.0.0.tar.gz` & `tmp/jaraco_media-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.media-4.0.0.tar", last modified: Tue Oct 25 15:28:09 2022, max compression
+gzip compressed data, was "jaraco_media-4.0.1.tar", last modified: Fri Apr 19 20:06:37 2024, max compression
```

## Comparing `jaraco.media-4.0.0.tar` & `jaraco_media-4.0.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.508071 jaraco.media-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.500071 jaraco.media-4.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.500071 jaraco.media-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-10-25 15:28:09.508071 jaraco.media-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.504071 jaraco.media-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.496071 jaraco.media-4.0.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.508071 jaraco.media-4.0.0/jaraco/media/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/concat.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/cropdetect.py
--rw-r--r--   0 runner    (1001) docker     (121)    12180 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/dvd.py
--rw-r--r--   0 runner    (1001) docker     (121)     6744 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/dvd_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6720 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/handbrake.py
--rw-r--r--   0 runner    (1001) docker     (121)     6317 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/index.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/isapiapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/matroska.py
--rw-r--r--   0 runner    (1001) docker     (121)     6692 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/splice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/srt-concat.py
--rw-r--r--   0 runner    (1001) docker     (121)     5325 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/srt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.508071 jaraco.media-4.0.0/jaraco/media/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    77972 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/tests/multi title output.txt
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/jaraco/media/tests/test_handbrake.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:28:09.504071 jaraco.media-4.0.0/jaraco.media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-10-25 15:28:09.000000 jaraco.media-4.0.0/jaraco.media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-25 15:28:09.000000 jaraco.media-4.0.0/jaraco.media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 15:28:09.000000 jaraco.media-4.0.0/jaraco.media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-10-25 15:28:09.000000 jaraco.media-4.0.0/jaraco.media.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-10-25 15:28:09.000000 jaraco.media-4.0.0/jaraco.media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-25 15:28:09.000000 jaraco.media-4.0.0/jaraco.media.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-10-25 15:28:09.508071 jaraco.media-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-25 15:27:27.000000 jaraco.media-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.839570 jaraco_media-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.831570 jaraco_media-4.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.831570 jaraco_media-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-19 20:06:37.839570 jaraco_media-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.831570 jaraco_media-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.827570 jaraco_media-4.0.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.835570 jaraco_media-4.0.1/jaraco/media/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/cropdetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/dvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/dvd_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/handbrake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/isapiapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/matroska.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/splice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/srt-concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/srt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.835570 jaraco_media-4.0.1/jaraco/media/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77972 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/tests/multi title output.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/jaraco/media/tests/test_handbrake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:06:37.835570 jaraco_media-4.0.1/jaraco.media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-19 20:06:37.000000 jaraco_media-4.0.1/jaraco.media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 20:06:37.000000 jaraco_media-4.0.1/jaraco.media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:06:37.000000 jaraco_media-4.0.1/jaraco.media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-19 20:06:37.000000 jaraco_media-4.0.1/jaraco.media.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 20:06:37.000000 jaraco_media-4.0.1/jaraco.media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 20:06:37.000000 jaraco_media-4.0.1/jaraco.media.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:06:37.839570 jaraco_media-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-19 20:06:18.000000 jaraco_media-4.0.1/tox.ini
```

### Comparing `jaraco.media-4.0.0/.github/workflows/main.yml` & `jaraco_media-4.0.1/.github/workflows/main.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,122 @@
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
+
+permissions:
+  contents: read
 
 env:
-  # Environment variables to support color support (jaraco/skeleton#66):
-  # Request colored output from CLI tools supporting it. Different tools
-  # interpret the value differently. For some, just being set is sufficient.
-  # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient.
-  FORCE_COLOR: -106
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
+  # Environment variable to support color support (jaraco/skeleton#66)
+  FORCE_COLOR: 1
 
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
-        - "3.7"
-        - "3.10"
-        - "3.11"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
+        - "3.8"
+        - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: pypy3.9
+        - python: "3.9"
+          platform: ubuntu-latest
+        - python: "3.10"
+          platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
+    continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run tests
+        run: python -m pip install tox
+      - name: Run
         run: tox
 
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+      - name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
+      - name: Install tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
+
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
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
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Release
+        run: python -m pip install tox
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.media-4.0.0/CHANGES.rst` & `jaraco_media-4.0.1/NEWS.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v4.0.1
+======
+
+Bugfixes
+--------
+
+- Utilize helpers in jaraco.packaging.metadata to parse the project's metadata. (#2)
+
+
 v4.0.0
 ======
 
 ``splice.splice_video`` now expects ``timestamps_include`` to be
 a ``starargs`` parameter instead of an explicit tuple.
 
 v3.7.0
```

### Comparing `jaraco.media-4.0.0/LICENSE` & `jaraco_media-4.0.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.media-4.0.0/PKG-INFO` & `jaraco_media-4.0.1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,24 @@
-Metadata-Version: 2.1
-Name: jaraco.media
-Version: 4.0.0
-Summary: DVD and other multimedia tools
-Home-page: https://github.com/jaraco/jaraco.media
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: LICENSE
-
 .. image:: https://img.shields.io/pypi/v/jaraco.media.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.media
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.media.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.media
 
-.. image:: https://github.com/jaraco/jaraco.media/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.media/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.media/actions?query=workflow%3A%22tests%22
    :alt: tests
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 
 concat
 ------
 
 FFmpeg provides a routine to
```

### Comparing `jaraco.media-4.0.0/docs/conf.py` & `jaraco_media-4.0.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
 extensions = [
     'sphinx.ext.autodoc',
     'jaraco.packaging.sphinx',
 ]
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `jaraco.media-4.0.0/jaraco/media/arguments.py` & `jaraco_media-4.0.1/jaraco/media/arguments.py`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco/media/concat.py` & `jaraco_media-4.0.1/jaraco/media/concat.py`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco/media/config.py` & `jaraco_media-4.0.1/jaraco/media/config.py`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco/media/cropdetect.py` & `jaraco_media-4.0.1/jaraco/media/cropdetect.py`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco/media/dvd.py` & `jaraco_media-4.0.1/jaraco/media/dvd.py`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco/media/dvd_info.py` & `jaraco_media-4.0.1/jaraco/media/dvd_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import sys
 import datetime
 import argparse
 from itertools import count
 from subprocess import Popen, PIPE, STDOUT
 from typing import Set
 
+from jaraco.packaging.metadata import extract_author, extract_email, hunt_down_url
+
 try:
     from importlib import metadata  # type: ignore
 except ImportError:
     import importlib_metadata as metadata  # type: ignore
 
 
 def banner():
@@ -30,16 +32,16 @@
     ==================================================
     <BLANKLINE>
     """
     md = metadata.metadata('jaraco.media')
 
     print(50 * '=')
     print(f'{md["Name"]} version {md["Version"]}')
-    print(f'{md["Author"]} <{md["Author-Email"]}>')
-    print(f'{md["Home-page"]}')
+    print(f'{extract_author(md)} <{extract_email(md)}>')
+    print(f'{hunt_down_url(md)}')
     print(50 * '=')
     print()
 
 
 class MetaTitleParser(type):
     """
     A metaclass for title parsers that keeps track of all of them.
```

### Comparing `jaraco.media-4.0.0/jaraco/media/handbrake.py` & `jaraco_media-4.0.1/jaraco/media/handbrake.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 import platform
 import sys
 import ctypes
 
 import path
 import jaraco.path
 from jaraco.ui import menu
-from jaraco.functools import call_aside
+from jaraco.functools import invoke
 
 try:
     from jaraco.windows.power import no_sleep
 except ImportError:
     from jaraco.context import null as no_sleep
 from more_itertools.recipes import consume
 
 from . import dvd
 from . import config
 
 
-@call_aside
+@invoke
 def add_hidden_method():
     """
     >>> path.Path('.').is_hidden()
     False
     """
     path.Path.is_hidden = jaraco.path.is_hidden
```

### Comparing `jaraco.media-4.0.0/jaraco/media/index.py` & `jaraco_media-4.0.1/jaraco/media/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,19 +133,17 @@
     )
     params.VirtualDirs = [vd]
     isapi.install.HandleCommandLine(params)
 
 
 def serve():
     Site.setup_application('/')
-    cherrypy.config.update(
-        {
-            'server.socket_host': '::0',
-        }
-    )
+    cherrypy.config.update({
+        'server.socket_host': '::0',
+    })
     if hasattr(cherrypy.engine, "signal_handler"):
         cherrypy.engine.signal_handler.subscribe()
     if hasattr(cherrypy.engine, "console_control_handler"):
         cherrypy.engine.console_control_handler.subscribe()
     cherrypy.engine.start()
     cherrypy.engine.block()
```

### Comparing `jaraco.media-4.0.0/jaraco/media/matroska.py` & `jaraco_media-4.0.1/jaraco/media/matroska.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,42 +21,38 @@
 
 def handle_command_line():
     args = get_args()
     filename = args.filename
     basename = os.path.basename(filename)
     name, ext = os.path.splitext(basename)
     message("Unpacking file: %s" % filename)
-    subprocess.Popen(
-        [
-            r'C:\Program Files (x86)\mkvtoolnix\mkvextract',  # 'mkvextract',
-            'tracks',
-            filename,
-            '2:temp_video.mp4',
-            '1:temp_audio.ogg',
-            # f'3:{name}.srt',
-        ]
-    ).wait()
+    subprocess.Popen([
+        r'C:\Program Files (x86)\mkvtoolnix\mkvextract',  # 'mkvextract',
+        'tracks',
+        filename,
+        '2:temp_video.mp4',
+        '1:temp_audio.ogg',
+        # f'3:{name}.srt',
+    ]).wait()
 
     message(f"Repacking file: {name}.mp4")
-    subprocess.Popen(
-        [
-            r'C:\Program Files\ffmpeg-git-9251942-win64-shared\bin\ffmpeg.exe',
-            # 'ffmpeg',
-            '-i',
-            'temp_audio.ogg',
-            '-i',
-            'temp_video.mp4',
-            '-vcodec',
-            'copy',
-            # 'libx264',
-            '-r',
-            '47.95',
-            name + '.mp4',
-        ]
-    ).wait()
+    subprocess.Popen([
+        r'C:\Program Files\ffmpeg-git-9251942-win64-shared\bin\ffmpeg.exe',
+        # 'ffmpeg',
+        '-i',
+        'temp_audio.ogg',
+        '-i',
+        'temp_video.mp4',
+        '-vcodec',
+        'copy',
+        # 'libx264',
+        '-r',
+        '47.95',
+        name + '.mp4',
+    ]).wait()
 
     message("Cleaning files")
     map(os.remove, ['temp_video.mp4', 'temp_audio.ogg'])
 
 
 if __name__ == "__main__":
     handle_command_line()
```

### Comparing `jaraco.media-4.0.0/jaraco/media/splice.py` & `jaraco_media-4.0.1/jaraco/media/splice.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         "error",
         "-select_streams",
         "v:0",
         "-show_entries",
         *options,
         "-of",
         "csv=print_section=0",
-        input_file.as_posix(),
+        input_file,
     )
     keyframe_output = subprocess.run(
         ffprobe_command, capture_output=True, check=True, encoding="UTF-8"
     )
     return keyframe_output.stdout
 
 
@@ -99,20 +99,20 @@
     post_duration = round(end - next_keyframe, TIME_PRECISION + 1)
     copy_command = (
         "ffmpeg",
         "-y",
         "-ss",
         str(next_keyframe),
         "-i",
-        input_file.as_posix(),
+        input_file,
         "-t",
         str(post_duration),
         "-c",
         "copy",
-        post_output_path.as_posix(),
+        post_output_path,
     )
     subprocess.run(copy_command, check=True)
     return post_output_path, post_duration
 
 
 def file_block_adjusted(
     idx, input_file, keyframe_times, keyframe_times_rounded, start, temp_path
@@ -127,24 +127,24 @@
     pre_duration = round(next_keyframe - start, TIME_PRECISION + 1)
     encode_command = (
         "ffmpeg",
         "-y",
         "-ss",
         str(start),
         "-i",
-        input_file.as_posix(),
+        input_file,
         "-t",
         str(pre_duration),
         "-video_track_timescale",
         time_base,
         "-c:v",
         "libx264",
         "-preset",
         "veryfast",
-        pre_output_path.as_posix(),
+        pre_output_path,
     )
     subprocess.run(encode_command, check=True)
     return pre_output_path, pre_duration
 
 
 def gen_file_block(
     end, idx, input_file, keyframe_times, keyframe_times_rounded, start, temp_path
@@ -154,36 +154,40 @@
     end = convert_timestamp_to_s(end)
 
     output_path, duration = file_block_adjusted(
         idx, input_file, keyframe_times, keyframe_times_rounded, start, temp_path
     ) or file_block_natural(
         end, idx, input_file, keyframe_times, keyframe_times_rounded, start, temp_path
     )
-    return f"file '{output_path.as_posix()}'\nduration {duration}\n"
+    return f"file '{output_path}'\nduration {duration}\n"
 
 
 @contextlib.contextmanager
 def TemporaryPath():
     with tempfile.TemporaryDirectory() as temp_dir:
         yield pathlib.Path(temp_dir)
 
 
-@autocommand.autocommand(__name__)  # noqa: F722
-def splice_video(  # noqa: F722
-    input_file: "The media file to read in",  # type: ignore
-    output_file: "The file to output the edited result to",  # type: ignore
+@autocommand.autocommand(__name__)
+def splice_video(
+    input_file: (  # type: ignore
+        convert_path,
+        "The media file to read in",  # noqa: F722
+    ),
+    output_file: (  # type: ignore
+        convert_path,
+        "The file to output the edited result to",  # noqa: F722
+    ),
     *timestamps_include: (  # type: ignore
         split_range,
-        "Start and end timestamps to to include in the final video, "  # noqa: F722
+        "Start and end timestamps to include in the final video, "  # noqa: F722
         "in the form HH:MM:SS.ffffff-HH:MM:SS.ffffff or SS.fff-SS.fff",
     ),
 ):
     "Split and combine specific chunks from a media w/ffmpeg."
-    input_file = convert_path(input_file)
-    output_file = convert_path(output_file)
 
     print("Retrieving keyframes")
     keyframe_times = get_keyframe_times(input_file)
     keyframe_times_rounded = [
         round(frame_time, TIME_PRECISION) for frame_time in keyframe_times
     ]
     with TemporaryPath() as temp_path:
@@ -210,13 +214,13 @@
             "ffmpeg",
             "-y",
             "-f",
             "concat",
             "-safe",
             "0",
             "-i",
-            concat_file_path.as_posix(),
+            concat_file_path,
             "-c",
             "copy",
-            output_file.as_posix(),
+            output_file,
         )
         subprocess.run(concat_command, check=True)
```

### Comparing `jaraco.media-4.0.0/jaraco/media/srt-concat.py` & `jaraco_media-4.0.1/jaraco/media/srt-concat.py`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco/media/srt.py` & `jaraco_media-4.0.1/jaraco/media/srt.py`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco/media/tests/multi title output.txt` & `jaraco_media-4.0.1/jaraco/media/tests/multi title output.txt`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/jaraco.media.egg-info/SOURCES.txt` & `jaraco_media-4.0.1/jaraco.media.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
-setup.cfg
+ruff.toml
+towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 jaraco.media.egg-info/PKG-INFO
```

### Comparing `jaraco.media-4.0.0/jaraco.media.egg-info/entry_points.txt` & `jaraco_media-4.0.1/jaraco.media.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `jaraco.media-4.0.0/setup.cfg` & `jaraco_media-4.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-[metadata]
-name = jaraco.media
-author = Jason R. Coombs
-author_email = jaraco@jaraco.com
-description = DVD and other multimedia tools
-long_description = file:README.rst
-url = https://github.com/jaraco/jaraco.media
-classifiers = 
-	Development Status :: 5 - Production/Stable
-	Intended Audience :: Developers
-	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-
-[options]
-packages = find_namespace:
-include_package_data = true
-python_requires = >=3.7
-install_requires = 
-	jaraco.text >= 3.4
-	jaraco.ui
-	jaraco.context
-	jaraco.path >= 3.1
-	jaraco.functools
-	jaraco.itertools >= 6.2
-	httpagentparser
-	more_itertools
-	path
-	inflect
-	importlib_metadata; python_version < "3.8"
-	autocommand
-	tempora
-
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
-
-[options.extras_require]
-testing = 
-	pytest >= 6
-	pytest-checkdocs >= 2.4
-	pytest-flake8
-	flake8 < 5
-	pytest-black >= 0.3.7; \
-	python_implementation != "PyPy"
-	pytest-cov
-	pytest-mypy >= 0.9.1; \
-	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
-	
-	cherrypy
-	genshi
-	importlib_resources
-docs = 
-	sphinx >= 3.5
-	jaraco.packaging >= 9
-	rst.linker >= 1.9
-	furo
-
-[options.entry_points]
-console_scripts = 
-	encode-dvd = jaraco.media.dvd:encode_dvd
-	rip-subtitles = jaraco.media.dvd:rip_subtitles
-	crop-detect = jaraco.media.cropdetect:execute
-	dvd-info = jaraco.media.dvd_info:main
-	transcode = jaraco.media.dvd:transcode
-	fix-fourcc = jaraco.media.dvd:fix_fourcc
-	serve-index = jaraco.media.index:serve
-	multibrake = jaraco.media.handbrake:multibrake
-	quick-brake = jaraco.media.handbrake:quick_brake
-	mkv-to-mp4 = jaraco.media.matroska:handle_command_line
-	adjust-sub = jaraco.media.srt:AdjustCommand.run
-	update-anydvd = jaraco.media.dvd:update_anydvd
-
-[egg_info]
-tag_build = 
-tag_date = 0
+[build-system]
+requires = ["setuptools>=61.2", "setuptools_scm[toml]>=3.4.1"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "jaraco.media"
+authors = [
+	{ name = "Jason R. Coombs", email = "jaraco@jaraco.com" },
+]
+description = "DVD and other multimedia tools"
+readme = "README.rst"
+classifiers = [
+	"Development Status :: 5 - Production/Stable",
+	"Intended Audience :: Developers",
+	"License :: OSI Approved :: MIT License",
+	"Programming Language :: Python :: 3",
+	"Programming Language :: Python :: 3 :: Only",
+]
+requires-python = ">=3.8"
+dependencies = [
+	"jaraco.text >= 3.4",
+	"jaraco.ui",
+	"jaraco.context",
+	"jaraco.path >= 3.1",
+	"jaraco.functools",
+	"jaraco.itertools >= 6.2",
+	"httpagentparser",
+	"more_itertools",
+	"path",
+	"inflect",
+	'importlib_metadata; python_version < "3.8"',
+	"autocommand",
+	"tempora",
+	"jaraco.packaging >= 10.1",
+]
+dynamic = ["version"]
+
+[project.urls]
+Homepage = "https://github.com/jaraco/jaraco.media"
+
+[project.optional-dependencies]
+testing = [
+	# upstream
+	"pytest >= 6, != 8.1.*",
+	"pytest-checkdocs >= 2.4",
+	"pytest-cov",
+	"pytest-mypy",
+	"pytest-enabler >= 2.2",
+	"pytest-ruff >= 0.2.1",
+
+	# local
+	"cherrypy",
+	"genshi",
+	"importlib_resources",
+]
+docs = [
+	# upstream
+	"sphinx >= 3.5",
+	"jaraco.packaging >= 9.3",
+	"rst.linker >= 1.9",
+	"furo",
+	"sphinx-lint",
+
+	# local
+]
+
+[project.scripts]
+encode-dvd = "jaraco.media.dvd:encode_dvd"
+rip-subtitles = "jaraco.media.dvd:rip_subtitles"
+crop-detect = "jaraco.media.cropdetect:execute"
+dvd-info = "jaraco.media.dvd_info:main"
+transcode = "jaraco.media.dvd:transcode"
+fix-fourcc = "jaraco.media.dvd:fix_fourcc"
+serve-index = "jaraco.media.index:serve"
+multibrake = "jaraco.media.handbrake:multibrake"
+quick-brake = "jaraco.media.handbrake:quick_brake"
+mkv-to-mp4 = "jaraco.media.matroska:handle_command_line"
+adjust-sub = "jaraco.media.srt:AdjustCommand.run"
+update-anydvd = "jaraco.media.dvd:update_anydvd"
 
+[tool.setuptools_scm]
```

