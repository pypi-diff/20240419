# Comparing `tmp/HyperCoast-0.0.1.tar.gz` & `tmp/hypercoast-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyperCoast-0.0.1.tar", last modified: Mon Apr  8 16:21:26 2024, max compression
+gzip compressed data, was "hypercoast-0.0.2.tar", last modified: Fri Apr 19 02:49:14 2024, max compression
```

## Comparing `HyperCoast-0.0.1.tar` & `hypercoast-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.694833 HyperCoast-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.698833 HyperCoast-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.698833 HyperCoast-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 16:21:26.000000 HyperCoast-0.0.1/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-08 16:21:26.000000 HyperCoast-0.0.1/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:21:26.000000 HyperCoast-0.0.1/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 16:21:26.000000 HyperCoast-0.0.1/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 16:21:26.000000 HyperCoast-0.0.1/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 16:21:26.000000 HyperCoast-0.0.1/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:21:26.702833 HyperCoast-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 16:21:15.000000 HyperCoast-0.0.1/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.853634 hypercoast-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.857634 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.857634 hypercoast-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 02:49:01.000000 hypercoast-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 02:49:01.000000 hypercoast-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 02:49:14.861634 hypercoast-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 02:49:01.000000 hypercoast-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 02:49:01.000000 hypercoast-0.0.2/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 02:49:01.000000 hypercoast-0.0.2/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 02:49:01.000000 hypercoast-0.0.2/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-19 02:49:01.000000 hypercoast-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 02:49:01.000000 hypercoast-0.0.2/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-19 02:49:01.000000 hypercoast-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 02:49:01.000000 hypercoast-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 02:49:01.000000 hypercoast-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:49:14.861634 hypercoast-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 02:49:01.000000 hypercoast-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 02:49:01.000000 hypercoast-0.0.2/tests/test_hypercoast.py
```

### Comparing `HyperCoast-0.0.1/.github/workflows/docs-build.yml` & `hypercoast-0.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.github/workflows/docs.yml` & `hypercoast-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.github/workflows/installation.yml` & `hypercoast-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.github/workflows/macos.yml` & `hypercoast-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.github/workflows/pypi.yml` & `hypercoast-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.github/workflows/ubuntu.yml` & `hypercoast-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.github/workflows/windows.yml` & `hypercoast-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.gitignore` & `hypercoast-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/.pre-commit-config.yaml` & `hypercoast-0.0.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.5.0
+      rev: v4.6.0
       hooks:
           - id: check-toml
           - id: check-yaml
           - id: end-of-file-fixer
             types: [python]
           - id: trailing-whitespace
           - id: requirements-txt-fixer
           - id: check-added-large-files
             args: ["--maxkb=500"]
 
     - repo: https://github.com/psf/black
-      rev: 24.3.0
+      rev: 24.4.0
       hooks:
           - id: black-jupyter
             language_version: python3.11
 
     - repo: https://github.com/codespell-project/codespell
       rev: v2.2.6
       hooks:
```

### Comparing `HyperCoast-0.0.1/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.0.2/HyperCoast.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for processing hyperspetral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/giswqs/HyperCoast
+Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: leafmap
 Requires-Dist: numpy
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # HyperCoast
 
-
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
 [![image](https://img.shields.io/conda/vn/conda-forge/HyperCoast.svg)](https://anaconda.org/conda-forge/HyperCoast)
 
-
 **A Python package for processing hyperspetral data in coastal regions**
 
-
 -   Free software: MIT License
--   Documentation: https://giswqs.github.io/HyperCoast
-
+-   Documentation: https://hypercoast.org
 
 ## Features
 
--   TODO
+-  Visualize hyperspectral data
+-  Analyze hypersepctral data
+
```

### Comparing `HyperCoast-0.0.1/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.0.2/HyperCoast.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 .github/workflows/windows.yml
 HyperCoast.egg-info/PKG-INFO
 HyperCoast.egg-info/SOURCES.txt
 HyperCoast.egg-info/dependency_links.txt
 HyperCoast.egg-info/entry_points.txt
 HyperCoast.egg-info/requires.txt
 HyperCoast.egg-info/top_level.txt
+docs/CNAME
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/hypercoast.md
 docs/index.md
 docs/installation.md
```

### Comparing `HyperCoast-0.0.1/LICENSE` & `hypercoast-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HyperCoast-0.0.1/PKG-INFO` & `hypercoast-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for processing hyperspetral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/giswqs/HyperCoast
+Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: leafmap
 Requires-Dist: numpy
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # HyperCoast
 
-
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
 [![image](https://img.shields.io/conda/vn/conda-forge/HyperCoast.svg)](https://anaconda.org/conda-forge/HyperCoast)
 
-
 **A Python package for processing hyperspetral data in coastal regions**
 
-
 -   Free software: MIT License
--   Documentation: https://giswqs.github.io/HyperCoast
-
+-   Documentation: https://hypercoast.org
 
 ## Features
 
--   TODO
+-  Visualize hyperspectral data
+-  Analyze hypersepctral data
+
```

### Comparing `HyperCoast-0.0.1/docs/contributing.md` & `hypercoast-0.0.2/docs/contributing.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 You can contribute in many ways:
 
 ## Types of Contributions
 
 ### Report Bugs
 
-Report bugs at <https://github.com/giswqs/HyperCoast/issues>.
+Report bugs at <https://github.com/opengeos/HyperCoast/issues>.
 
 If you are reporting a bug, please include:
 
 -   Your operating system name and version.
 -   Any details about your local setup that might be helpful in troubleshooting.
 -   Detailed steps to reproduce the bug.
 
@@ -32,15 +32,15 @@
 HyperCoast could always use more documentation,
 whether as part of the official HyperCoast docs,
 in docstrings, or even on the web in blog posts, articles, and such.
 
 ### Submit Feedback
 
 The best way to send feedback is to file an issue at
-<https://github.com/giswqs/HyperCoast/issues>.
+<https://github.com/opengeos/HyperCoast/issues>.
 
 If you are proposing a feature:
 
 -   Explain in detail how it would work.
 -   Keep the scope as narrow as possible, to make it easier to implement.
 -   Remember that this is a volunteer-driven project, and that contributions are welcome :)
 
@@ -100,9 +100,9 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1.  The pull request should include tests.
 2.  If the pull request adds functionality, the docs should be updated.
     Put your new functionality into a function with a docstring, and add
     the feature to the list in README.rst.
 3.  The pull request should work for Python 3.8 and later, and
-    for PyPy. Check <https://github.com/giswqs/HyperCoast/pull_requests> and make sure that the tests pass for all
+    for PyPy. Check <https://github.com/opengeos/HyperCoast/pull_requests> and make sure that the tests pass for all
     supported Python versions.
```

### Comparing `HyperCoast-0.0.1/docs/installation.md` & `hypercoast-0.0.2/docs/installation.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 If you don't have [pip](https://pip.pypa.io) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process.
 
 ## From sources
 
 To install HyperCoast from sources, run this command in your terminal:
 
 ```
-pip install git+https://github.com/giswqs/HyperCoast
+pip install git+https://github.com/opengeos/HyperCoast
 ```
```

### Comparing `HyperCoast-0.0.1/mkdocs.yml` & `hypercoast-0.0.2/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 site_name: HyperCoast
 site_description: A Python package for processing hyperspetral data in coastal regions
 site_author: giswqs
-site_url: https://giswqs.github.io/HyperCoast
-repo_url: https://github.com/giswqs/HyperCoast
+site_url: https://hypercoast.org
+repo_url: https://github.com/opengeos/HyperCoast
 
 copyright: "Copyright &copy; 2024 - 2024 Qiusheng Wu"
 
 theme:
     palette:
         - scheme: default
           #   primary: blue
@@ -74,13 +74,13 @@
 nav:
     - Home: index.md
     - Installation: installation.md
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
-    - Report Issues: https://github.com/giswqs/HyperCoast/issues
+    - Report Issues: https://github.com/opengeos/HyperCoast/issues
     - Examples:
-        - examples/intro.ipynb
+          - examples/intro.ipynb
     - API Reference:
           - hypercoast module: hypercoast.md
           - common module: common.md
```

### Comparing `HyperCoast-0.0.1/pyproject.toml` & `hypercoast-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspetral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
@@ -71,12 +71,12 @@
 exclude = [
     "docs",
 ]
 max-line-length = 88
 
 
 [project.urls]
-Homepage = "https://github.com/giswqs/HyperCoast"
+Homepage = "https://github.com/opengeos/HyperCoast"
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
```

