# Comparing `tmp/sumo-wrapper-python-1.0.8.tar.gz` & `tmp/sumo_wrapper_python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumo-wrapper-python-1.0.8.tar", last modified: Tue Jan 23 08:13:16 2024, max compression
+gzip compressed data, was "sumo_wrapper_python-1.0.9.tar", last modified: Fri Apr 19 08:58:24 2024, max compression
```

## Comparing `sumo-wrapper-python-1.0.8.tar` & `sumo_wrapper_python-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.379641 sumo-wrapper-python-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.367641 sumo-wrapper-python-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.371641 sumo-wrapper-python-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17430 2024-01-23 08:13:16.379641 sumo-wrapper-python-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.371641 sumo-wrapper-python-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 08:13:16.379641 sumo-wrapper-python-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.371641 sumo-wrapper-python-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.371641 sumo-wrapper-python-1.0.8/src/sumo/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.375641 sumo-wrapper-python-1.0.8/src/sumo/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/_auth_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/_blob_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-23 08:13:16.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    14741 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/src/sumo/wrapper/sumo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.375641 sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17430 2024-01-23 08:13:16.000000 sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-23 08:13:16.000000 sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 08:13:16.000000 sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-23 08:13:16.000000 sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-23 08:13:16.000000 sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-23 08:13:16.000000 sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.375641 sumo-wrapper-python-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/tests/test_sumo_thin_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:13:16.375641 sumo-wrapper-python-1.0.8/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/tests/testdata/case.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-23 08:13:08.000000 sumo-wrapper-python-1.0.8/tests/testdata/surface.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.963958 sumo_wrapper_python-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.951958 sumo_wrapper_python-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.955958 sumo_wrapper_python-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/.github/workflows/build_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-04-19 08:58:24.959957 sumo_wrapper_python-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.955958 sumo_wrapper_python-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.955958 sumo_wrapper_python-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/_static/equinor-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/_static/equinor-logo2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25380 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/_static/equinor_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/_static/equinor_logo_only.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.955958 sumo_wrapper_python-1.0.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/docs/sumo-wrapper-python.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:58:24.963958 sumo_wrapper_python-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.951958 sumo_wrapper_python-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.955958 sumo_wrapper_python-1.0.9/src/sumo/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.959957 sumo_wrapper_python-1.0.9/src/sumo/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/_auth_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/_blob_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 08:58:24.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/src/sumo/wrapper/sumo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.959957 sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-04-19 08:58:24.000000 sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-19 08:58:24.000000 sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:58:24.000000 sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 08:58:24.000000 sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-19 08:58:24.000000 sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 08:58:24.000000 sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.959957 sumo_wrapper_python-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/tests/test_sumo_thin_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:58:24.959957 sumo_wrapper_python-1.0.9/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/tests/testdata/case.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-19 08:58:18.000000 sumo_wrapper_python-1.0.9/tests/testdata/surface.yml
```

### Comparing `sumo-wrapper-python-1.0.8/.github/workflows/linting.yml` & `sumo_wrapper_python-1.0.9/.github/workflows/linting.yml`

 * *Files 15% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 jobs:
   black:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8"]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - uses: psf/black@stable
         with:
           options: "--check --verbose --line-length 79"
           src: "./src/sumo/wrapper"
   flake8:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8"]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flake8
       - name: Analysing the code with flake8
```

### Comparing `sumo-wrapper-python-1.0.8/.github/workflows/publish_release.yml` & `sumo_wrapper_python-1.0.9/.github/workflows/publish_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
   buildAndPublish:
     name: Publish to PyPi
     permissions:
       id-token: write
     environment: production
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.8"
 
       - name: build
         run: |
           python -m pip install --upgrade build
           python -m build
```

### Comparing `sumo-wrapper-python-1.0.8/.github/workflows/pytest.yml` & `sumo_wrapper_python-1.0.9/.github/workflows/pytest.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
         python-version: ["3.8", "3.9", "3.10", "3.11"]
         os: [ubuntu-latest, windows-latest, macos-latest]
     permissions:
       contents: read
       id-token: write
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Azure Login
-        uses: Azure/login@v1
+        uses: Azure/login@v2
         with:
           client-id: f96c150d-cacf-4257-9cc9-54b2c68ec4ce
           tenant-id: 3aa4a235-b6e2-48d5-9195-7fcf05b459b0
           subscription-id: 87897772-fb27-495f-ae40-486a2df57baa
 
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install sumo-wrapper-python
         run: |
           python -m pip install --upgrade pip &&
           python -m pip install .[test]
```

### Comparing `sumo-wrapper-python-1.0.8/CONTRIBUTING.md` & `sumo_wrapper_python-1.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/LICENSE` & `sumo_wrapper_python-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/PKG-INFO` & `sumo_wrapper_python-1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo-wrapper-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python wrapper for the Sumo API
 Author: Equinor
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,166 +219,21 @@
 Requires-Dist: azure-identity>=1.13.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: PyYAML; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: autoapi; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
 
 # sumo-wrapper-python
 
-Python wrappers for Sumo APIs
+[![Documentation Status](https://readthedocs.org/projects/sumo-wrapper-python/badge/?version=latest)](https://sumo-wrapper-python.readthedocs.io/en/latest/?badge=latest)
 
-Want to contribute? Read our [contributing](./CONTRIBUTING.md) guidelines
+## Documentation and guidelines
+[sumo-wrapper-python documentation](https://sumo-wrapper-python.readthedocs.io/en/latest/)
 
-## Install:
+## Contribute
+[Contribution guidelines](./CONTRIBUTING.md)
 
-    pip install sumo-wrapper-python
-
-For internal Equinor users, this package is available through the Komodo
-distribution.
-
-# Table of contents
-
-- [sumo-wrapper-python](#sumo-wrapper-python)
-  - [Install:](#install)
-- [Table of contents](#table-of-contents)
-- [SumoClient](#sumoclient)
-    - [Initialization](#initialization)
-    - [Parameters](#parameters)
-          - [`token` logic](#token-logic)
-  - [Methods](#methods)
-    - [get(path, \*\*params)](#getpath-params)
-    - [post(path, json, blob, params)](#postpath-json-blob-params)
-    - [put(path, json, blob)](#putpath-json-blob)
-    - [delete(path)](#deletepath)
-  - [Async methods](#async-methods)
-
-# SumoClient
-
-A thin wrapper class for the Sumo API.
-
-### Initialization
-
-```python
-from sumo.wrapper import SumoClient
-
-sumo = SumoClient(env="dev")
-```
-
-### Parameters
-
-```python
-class SumoClient:
-    def __init__(
-        self,
-        env:str,
-        token:str=None,
-        interactive:bool=False,
-        verbosity:str="CRITICAL"
-    ):
-```
-
-- `env`: sumo environment
-- `token`: bearer token or refresh token
-- `interactive`: use interactive flow when authenticating
-- `verbosity`: "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
-
-###### `token` logic
-
-If an access token is provided in the `token` parameter, it will be used as long
-as it's valid. An error will be raised when it expires.
-
-If we are unable to decode the provided `token` as a JWT, we treat it as a
-refresh token and attempt to use it to retrieve an access token.
-
-If no `token` is provided, an authentication code flow/interactive flow is
-triggered to retrieve a token.
-
-## Methods
-
-`SumoClient` has one method for each HTTP-method that is used in the sumo-core
-API. See examples of how to use these methods below.
-
-All methods accepts a path argument. Path parameters can be interpolated into
-the path string. Example:
-
-```python
-object_id = "1234"
-
-# GET/objects('{obejctid}')
-sumo.get(f"/objects('{object_id}')")
-```
-
-### get(path, \*\*params)
-
-Performs a GET-request to sumo-core. Accepts query parameters as keyword
-arguments.
-
-```python
-# Retrieve userdata
-user_data = sumo.get("/userdata")
-
-# Search for objects
-results = sumo.get("/search",
-    query="class:surface",
-    size:3,
-    select=["_id"]
-)
-
-# Get object by id
-object_id = "159405ba-0046-b321-55ce-542f383ba5c7"
-
-obj = sumo.get(f"/objects('{object_id}')")
-```
-
-### post(path, json, blob, params)
-
-Performs a POST-request to sumo-core. Accepts json and blob, but not both at the
-same time.
-
-```python
-# Upload new parent object
-parent_object = sumo.post("/objects", json=parent_meta_data)
-
-# Upload child object
-parent_id = parent_object["_id"]
-
-child_object = sumo.post(f"/objects('{parent_id}')", json=child_meta_data)
-```
-
-### put(path, json, blob)
-
-Performs a PUT-request to sumo-core. Accepts json and blob, but not both at the
-same time.
-
-```python
-# Upload blob to child object
-child_id = child_object["_id"]
-
-sumo.put(f"/objects('{child_id}')/blob", blob=blob)
-```
-
-### delete(path)
-
-Performs a DELETE-request to sumo-core.
-
-```python
-# Delete blob
-sumo.delete(f"/objects('{child_id}')/blob")
-
-# Delete child object
-sumo.delete(f"/objects('{child_id}')")
-
-# Delete parent object
-sumo.delete(f"/objects('{parent_id}')")
-```
-
-## Async methods
-
-`SumoClient` also has *async* alternatives `get_async`, `post_async`, `put_async` and `delete_async`.
-These accept the same parameters as their synchronous counterparts, but have to be *awaited*.
-
-```python
-# Retrieve userdata
-user_data = await sumo.get_async("/userdata")
-```
```

### Comparing `sumo-wrapper-python-1.0.8/SECURITY.md` & `sumo_wrapper_python-1.0.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/docs/Makefile` & `sumo_wrapper_python-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/docs/conf.py` & `sumo_wrapper_python-1.0.9/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,48 +9,50 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-sys.path.insert(0, os.path.abspath('../src/'))
+sys.path.insert(0, os.path.abspath("../src/"))
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'sumo-wrapper-python'
-copyright = '2022, Sudo Team @ Equinor'
-author = 'Sudo Team @ Equinor'
+project = "sumo-wrapper-python"
+copyright = "2024, Sudo Team @ Equinor"
+author = "Sudo Team @ Equinor"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx.ext.napoleon', 'sphinx.ext.autodoc']
+extensions = [
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autodoc",
+]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
+html_logo = "_static/equinor-logo2.jpg"
 
-html_theme_options = {
-    "style_nav_header_background": "#C0C0C0",
-}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
+
```

### Comparing `sumo-wrapper-python-1.0.8/docs/make.bat` & `sumo_wrapper_python-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/pyproject.toml` & `sumo_wrapper_python-1.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -28,15 +28,21 @@
   "httpx>=0.24.1",
   "tenacity>=8.2.2",
   "azure-identity>=1.13.0",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "PyYAML"]
-docs = ["sphinx", "sphinx-rtd-theme"]
+docs = [
+  "sphinx",
+  "sphinx-rtd-theme",
+  "autoapi",
+  "sphinx-autodoc-typehints",
+  "sphinxcontrib-apidoc",
+]
 
 [project.urls]
 Repository = "https://github.com/equinor/sumo-wrapper-python"
 
 [project.scripts]
 sumo_login = "sumo.wrapper.login:main"
```

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/_auth_provider.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/_auth_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import platform
+from pathlib import Path
 import msal
 import os
 from datetime import datetime, timedelta
 import stat
 import sys
 import json
 import jwt
@@ -30,14 +32,17 @@
 
 
 class AuthProvider:
     def __init__(self, resource_id):
         self._resource_id = resource_id
         self._scope = scope_for_resource(resource_id)
         self._app = None
+        self._login_timeout_minutes = 5
+        os.system("")  # Ensure color init on all platforms (win10)
+
         return
 
     @tn.retry(
         retry=tn.retry_if_exception(_maybe_nfs_exception),
         stop=tn.stop_after_attempt(6),
         wait=(
             tn.wait_exponential(multiplier=0.5, exp_base=2)
@@ -53,15 +58,19 @@
         result = self._app.acquire_token_silent([self._scope], accounts[0])
         if result is None:
             return None
         # ELSE
         return result["access_token"]
 
     def get_authorization(self):
-        return {"Authorization": "Bearer " + self.get_token()}
+        token = self.get_token()
+        if token is None:
+            return ""
+
+        return {"Authorization": "Bearer " + token}
 
     pass
 
 
 class AuthProviderAccessToken(AuthProvider):
     def __init__(self, access_token):
         self._access_token = access_token
@@ -191,33 +200,32 @@
             + tn.wait_random_exponential(multiplier=0.5, exp_base=2)
         ),
         retry_error_callback=_return_last_value,
         before_sleep=_log_retry_info,
     )
     def login(self):
         scopes = [self._scope + " offline_access"]
-        login_timeout_minutes = 7
-        os.system("")  # Ensure color init on all platforms (win10)
         print(
             "\n\n \033[31m NOTE! \033[0m"
             + " Please login to Equinor Azure to enable Sumo access: "
-            + "we opened a login web-page for you in your browser."
+            + "we are opening a login web-page for you in your browser."
             + "\nYou should complete your login within "
-            + str(login_timeout_minutes)
+            + str(self._login_timeout_minutes)
             + " minutes, "
             + "that is before "
             + str(
                 (
-                    datetime.now() + timedelta(minutes=login_timeout_minutes)
+                    datetime.now()
+                    + timedelta(minutes=self._login_timeout_minutes)
                 ).strftime("%H:%M:%S")
             )
         )
         try:
             result = self._app.acquire_token_interactive(
-                scopes, timeout=(login_timeout_minutes * 60)
+                scopes, timeout=(self._login_timeout_minutes * 60)
             )
             if "error" in result:
                 print(
                     "\n\n \033[31m Error during Equinor Azure login "
                     "for Sumo access: \033[0m"
                 )
                 print("Err: ", json.dumps(result, indent=4))
@@ -226,15 +234,17 @@
             print(
                 "\n\n \033[31m Failed Equinor Azure login for Sumo access, "
                 "one possible reason is timeout \033[0m"
             )
             return
 
         protect_token_cache(self._resource_id, ".token")
-        print("Equinor Azure login for Sumo access was successful")
+        print(
+            "Equinor Azure login for Sumo access was successful (interactive)"
+        )
         return
 
     pass
 
 
 class AuthProviderDeviceCode(AuthProvider):
     def __init__(self, client_id, authority, resource_id):
@@ -257,32 +267,55 @@
             tn.wait_exponential(multiplier=0.5, exp_base=2)
             + tn.wait_random_exponential(multiplier=0.5, exp_base=2)
         ),
         retry_error_callback=_return_last_value,
         before_sleep=_log_retry_info,
     )
     def login(self):
-        flow = self._app.initiate_device_flow([self._scope])
-
-        if "error" in flow:
-            raise ValueError(
-                "Failed to create device flow. Err: %s"
-                % json.dumps(flow, indent=4)
+        try:
+            scopes = [self._scope + " offline_access"]
+            flow = self._app.initiate_device_flow(scopes)
+            if "error" in flow:
+                print(
+                    "\n\n \033[31m"
+                    + "Failed to initiate device-code login. Err: %s"
+                    + "\033[0m" % json.dumps(flow, indent=4)
+                )
+                return
+            flow["expires_at"] = (
+                int(time.time()) + self._login_timeout_minutes * 60
             )
 
-        print(flow["message"])
-        result = self._app.acquire_token_by_device_flow(flow)
+            print(
+                "\033[31m"
+                + " NOTE! Please login to Equinor Azure to enable Sumo access:"
+                + flow["message"]
+                + " \033[0m"
+                + "\nYou should complete your login within a few minutes"
+            )
+            result = self._app.acquire_token_by_device_flow(flow)
 
-        if "error" in result:
-            raise ValueError(
-                "Failed to acquire token by device flow. Err: %s"
-                % json.dumps(result, indent=4)
+            if "error" in result:
+                print(
+                    "\n\n \033[31m Error during Equinor Azure login "
+                    "for Sumo access: \033[0m"
+                )
+                print("Err: ", json.dumps(result, indent=4))
+                return
+        except Exception:
+            print(
+                "\n\n \033[31m Failed Equinor Azure login for Sumo access, "
+                "one possible reason is timeout \033[0m"
             )
+            return
 
         protect_token_cache(self._resource_id, ".token")
+        print(
+            "Equinor Azure login for Sumo access was successful (device-code)"
+        )
 
         return
 
     pass
 
 
 class AuthProviderManaged(AuthProvider):
@@ -380,8 +413,15 @@
                 "AZURE_CLIENT_ID",
                 "AZURE_AUTHORITY_HOST",
             ]
         ]
     ):
         return AuthProviderManaged(resource_id)
     # ELSE
+    lockfile_path = Path.home() / ".config/chromium/SingletonLock"
+    if Path(lockfile_path).is_symlink() and not str(
+        Path(lockfile_path).resolve()
+    ).__contains__(platform.node()):
+        # https://github.com/equinor/sumo-wrapper-python/issues/193
+        return AuthProviderDeviceCode(client_id, authority, resource_id)
+    # ELSE
     return AuthProviderInteractive(client_id, authority, resource_id)
```

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/_blob_client.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/_blob_client.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/_decorators.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/_decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+# For sphinx:
+from functools import wraps
+
+
 def raise_for_status(func):
+    @wraps(func)
     def wrapper(*args, **kwargs):
         # FIXME: in newer versions of httpx, raise_for_status() is chainable,
         # so we could simply write
         # return func(*args, **kwargs).raise_for_status()
         response = func(*args, **kwargs)
         response.raise_for_status()
         return response
 
     return wrapper
 
 
 def raise_for_status_async(func):
+    @wraps(func)
     async def wrapper(*args, **kwargs):
         # FIXME: in newer versions of httpx, raise_for_status() is chainable,
         # so we could simply write
         # return func(*args, **kwargs).raise_for_status()
         response = await func(*args, **kwargs)
         response.raise_for_status()
         return response
```

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/_logging.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/_logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,17 @@
                 "message": record.getMessage(),
                 "timestamp": dt,
                 "source": record.name,
                 "pathname": record.pathname,
                 "funcname": record.funcName,
                 "linenumber": record.lineno,
             }
+            if "objectUuid" in record.__dict__.keys():
+                json["objectUuid"] = record.__dict__.get("objectUuid")
+
             self._sumoClient.post("/message-log/new", json=json)
         except Exception:
             # Never fail on logging
             pass
 
         return
```

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/_retry_strategy.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/config.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/config.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/login.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -70,10 +70,15 @@
         args.env, interactive=args.interactive, devicecode=args.devicecode
     )
     token = sumo.authenticate()
 
     if args.print_token:
         print(f"TOKEN: {token}")
 
+    if token is not None:
+        print("Successfully logged in to Sumo environment: " + env)
+    else:
+        print("Failed login to Sumo environment: " + env)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `sumo-wrapper-python-1.0.8/src/sumo/wrapper/sumo_client.py` & `sumo_wrapper_python-1.0.9/src/sumo/wrapper/sumo_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,35 @@
             authority=f"{AUTHORITY_HOST_URI}/{TENANT_ID}",
             resource_id=APP_REGISTRATION[env]["RESOURCE_ID"],
             interactive=interactive,
             refresh_token=refresh_token,
             access_token=access_token,
             devicecode=devicecode,
         )
+        if (
+            self.auth.get_token() is None
+            and refresh_token is None
+            and access_token is None
+        ):
+            print("\n \033[31m !!! Falling back to device-code login:\033[0m")
+            self.auth = get_auth_provider(
+                client_id=APP_REGISTRATION[env]["CLIENT_ID"],
+                authority=f"{AUTHORITY_HOST_URI}/{TENANT_ID}",
+                resource_id=APP_REGISTRATION[env]["RESOURCE_ID"],
+                interactive=False,
+                refresh_token=None,
+                access_token=None,
+                devicecode=True,
+            )
+        if self.auth.get_token() is None:
+            print(
+                "\n\n \033[31m "
+                + "NOTE! Login failed/timed out. Giving up."
+                + "\033[0m"
+            )
 
         if env == "localhost":
             self.base_url = "http://localhost:8084/api/v1"
         else:
             self.base_url = f"https://main-sumo-{env}.radix.equinor.com/api/v1"
             pass
         return
```

### Comparing `sumo-wrapper-python-1.0.8/src/sumo_wrapper_python.egg-info/PKG-INFO` & `sumo_wrapper_python-1.0.9/src/sumo_wrapper_python.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo-wrapper-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python wrapper for the Sumo API
 Author: Equinor
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,166 +219,21 @@
 Requires-Dist: azure-identity>=1.13.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: PyYAML; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: autoapi; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
 
 # sumo-wrapper-python
 
-Python wrappers for Sumo APIs
+[![Documentation Status](https://readthedocs.org/projects/sumo-wrapper-python/badge/?version=latest)](https://sumo-wrapper-python.readthedocs.io/en/latest/?badge=latest)
 
-Want to contribute? Read our [contributing](./CONTRIBUTING.md) guidelines
+## Documentation and guidelines
+[sumo-wrapper-python documentation](https://sumo-wrapper-python.readthedocs.io/en/latest/)
 
-## Install:
+## Contribute
+[Contribution guidelines](./CONTRIBUTING.md)
 
-    pip install sumo-wrapper-python
-
-For internal Equinor users, this package is available through the Komodo
-distribution.
-
-# Table of contents
-
-- [sumo-wrapper-python](#sumo-wrapper-python)
-  - [Install:](#install)
-- [Table of contents](#table-of-contents)
-- [SumoClient](#sumoclient)
-    - [Initialization](#initialization)
-    - [Parameters](#parameters)
-          - [`token` logic](#token-logic)
-  - [Methods](#methods)
-    - [get(path, \*\*params)](#getpath-params)
-    - [post(path, json, blob, params)](#postpath-json-blob-params)
-    - [put(path, json, blob)](#putpath-json-blob)
-    - [delete(path)](#deletepath)
-  - [Async methods](#async-methods)
-
-# SumoClient
-
-A thin wrapper class for the Sumo API.
-
-### Initialization
-
-```python
-from sumo.wrapper import SumoClient
-
-sumo = SumoClient(env="dev")
-```
-
-### Parameters
-
-```python
-class SumoClient:
-    def __init__(
-        self,
-        env:str,
-        token:str=None,
-        interactive:bool=False,
-        verbosity:str="CRITICAL"
-    ):
-```
-
-- `env`: sumo environment
-- `token`: bearer token or refresh token
-- `interactive`: use interactive flow when authenticating
-- `verbosity`: "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
-
-###### `token` logic
-
-If an access token is provided in the `token` parameter, it will be used as long
-as it's valid. An error will be raised when it expires.
-
-If we are unable to decode the provided `token` as a JWT, we treat it as a
-refresh token and attempt to use it to retrieve an access token.
-
-If no `token` is provided, an authentication code flow/interactive flow is
-triggered to retrieve a token.
-
-## Methods
-
-`SumoClient` has one method for each HTTP-method that is used in the sumo-core
-API. See examples of how to use these methods below.
-
-All methods accepts a path argument. Path parameters can be interpolated into
-the path string. Example:
-
-```python
-object_id = "1234"
-
-# GET/objects('{obejctid}')
-sumo.get(f"/objects('{object_id}')")
-```
-
-### get(path, \*\*params)
-
-Performs a GET-request to sumo-core. Accepts query parameters as keyword
-arguments.
-
-```python
-# Retrieve userdata
-user_data = sumo.get("/userdata")
-
-# Search for objects
-results = sumo.get("/search",
-    query="class:surface",
-    size:3,
-    select=["_id"]
-)
-
-# Get object by id
-object_id = "159405ba-0046-b321-55ce-542f383ba5c7"
-
-obj = sumo.get(f"/objects('{object_id}')")
-```
-
-### post(path, json, blob, params)
-
-Performs a POST-request to sumo-core. Accepts json and blob, but not both at the
-same time.
-
-```python
-# Upload new parent object
-parent_object = sumo.post("/objects", json=parent_meta_data)
-
-# Upload child object
-parent_id = parent_object["_id"]
-
-child_object = sumo.post(f"/objects('{parent_id}')", json=child_meta_data)
-```
-
-### put(path, json, blob)
-
-Performs a PUT-request to sumo-core. Accepts json and blob, but not both at the
-same time.
-
-```python
-# Upload blob to child object
-child_id = child_object["_id"]
-
-sumo.put(f"/objects('{child_id}')/blob", blob=blob)
-```
-
-### delete(path)
-
-Performs a DELETE-request to sumo-core.
-
-```python
-# Delete blob
-sumo.delete(f"/objects('{child_id}')/blob")
-
-# Delete child object
-sumo.delete(f"/objects('{child_id}')")
-
-# Delete parent object
-sumo.delete(f"/objects('{parent_id}')")
-```
-
-## Async methods
-
-`SumoClient` also has *async* alternatives `get_async`, `post_async`, `put_async` and `delete_async`.
-These accept the same parameters as their synchronous counterparts, but have to be *awaited*.
-
-```python
-# Retrieve userdata
-user_data = await sumo.get_async("/userdata")
-```
```

### Comparing `sumo-wrapper-python-1.0.8/tests/test_sumo_thin_client.py` & `sumo_wrapper_python-1.0.9/tests/test_sumo_thin_client.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/tests/testdata/case.yml` & `sumo_wrapper_python-1.0.9/tests/testdata/case.yml`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-1.0.8/tests/testdata/surface.yml` & `sumo_wrapper_python-1.0.9/tests/testdata/surface.yml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 fmu:
   model:
     name: ff
     revision: 21.0.0.dev
     description:
       - detailed description
       - optional
-
+  
+  context:
+    stage: "realization"
+  
   workflow: # not sure, but a reference to the workflow / job that made this. Making it expandable.
     reference: rms/structural_model
 
   case:
     name: TestCase from fmu.sumo
     uuid: 8bb56d60-8758-481a-89a4-6bac8561d38e # (pseudo-)random valid uuid4
     user:
```

