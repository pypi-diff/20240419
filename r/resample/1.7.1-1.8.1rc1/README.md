# Comparing `tmp/resample-1.7.1.tar.gz` & `tmp/resample-1.8.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resample-1.7.1.tar", last modified: Mon Feb 12 17:01:06 2024, max compression
+gzip compressed data, was "resample-1.8.1rc1.tar", last modified: Fri Apr 19 09:21:37 2024, max compression
```

## Comparing `resample-1.7.1.tar` & `resample-1.8.1rc1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.715027 resample-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-12 17:00:53.000000 resample-1.7.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.699027 resample-1.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.703027 resample-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-12 17:00:53.000000 resample-1.7.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-12 17:00:53.000000 resample-1.7.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-12 17:00:53.000000 resample-1.7.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-12 17:00:53.000000 resample-1.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-12 17:00:53.000000 resample-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-12 17:00:53.000000 resample-1.7.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-12 17:00:53.000000 resample-1.7.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-12 17:00:53.000000 resample-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-12 17:00:53.000000 resample-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-02-12 17:01:06.711027 resample-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-12 17:00:53.000000 resample-1.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.703027 resample-1.7.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-12 17:00:53.000000 resample-1.7.1/benchmarks/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-12 17:00:53.000000 resample-1.7.1/benchmarks/test_jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-12 17:00:53.000000 resample-1.7.1/benchmarks/test_rcont.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-12 17:00:53.000000 resample-1.7.1/benchmarks/test_usp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.707027 resample-1.7.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-12 17:00:53.000000 resample-1.7.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.707027 resample-1.7.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    46843 2024-02-12 17:00:53.000000 resample-1.7.1/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86616 2024-02-12 17:00:53.000000 resample-1.7.1/doc/bench_rcont.json
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-02-12 17:00:53.000000 resample-1.7.1/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-02-12 17:00:53.000000 resample-1.7.1/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.707027 resample-1.7.1/doc/example/
--rw-r--r--   0 runner    (1001) docker     (127)   181138 2024-02-12 17:00:53.000000 resample-1.7.1/doc/example/tag_and_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-12 17:00:53.000000 resample-1.7.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-12 17:00:53.000000 resample-1.7.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-12 17:00:53.000000 resample-1.7.1/doc/make_raw_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-12 17:00:53.000000 resample-1.7.1/doc/plot_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-12 17:00:53.000000 resample-1.7.1/doc/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.707027 resample-1.7.1/doc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-02-12 17:00:53.000000 resample-1.7.1/doc/tutorial/confidence_intervals.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-02-12 17:00:53.000000 resample-1.7.1/doc/tutorial/jackknife_vs_bootstrap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    73522 2024-02-12 17:00:53.000000 resample-1.7.1/doc/tutorial/permutation_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   141793 2024-02-12 17:00:53.000000 resample-1.7.1/doc/tutorial/sklearn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42094 2024-02-12 17:00:53.000000 resample-1.7.1/doc/tutorial/usp_continuous_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-02-12 17:00:53.000000 resample-1.7.1/doc/tutorial/variance_fit_parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-12 17:00:53.000000 resample-1.7.1/doc/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-12 17:00:53.000000 resample-1.7.1/doc/update_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-12 17:00:53.000000 resample-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 17:01:06.715027 resample-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.703027 resample-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.711027 resample-1.7.1/src/resample/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-12 17:00:53.000000 resample-1.7.1/src/resample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-12 17:00:53.000000 resample-1.7.1/src/resample/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-02-12 17:00:53.000000 resample-1.7.1/src/resample/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-12 17:00:53.000000 resample-1.7.1/src/resample/empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-02-12 17:00:53.000000 resample-1.7.1/src/resample/jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-02-12 17:00:53.000000 resample-1.7.1/src/resample/permutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.711027 resample-1.7.1/src/resample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-02-12 17:01:06.000000 resample-1.7.1/src/resample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-12 17:01:06.000000 resample-1.7.1/src/resample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 17:01:06.000000 resample-1.7.1/src/resample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-12 17:01:06.000000 resample-1.7.1/src/resample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 17:01:06.000000 resample-1.7.1/src/resample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:01:06.711027 resample-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-02-12 17:00:53.000000 resample-1.7.1/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-02-12 17:00:53.000000 resample-1.7.1/tests/test_empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-02-12 17:00:53.000000 resample-1.7.1/tests/test_jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-02-12 17:00:53.000000 resample-1.7.1/tests/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-12 17:00:53.000000 resample-1.7.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.867431 resample-1.8.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 09:21:34.000000 resample-1.8.1rc1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.859431 resample-1.8.1rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.859431 resample-1.8.1rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-19 09:21:34.000000 resample-1.8.1rc1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-19 09:21:34.000000 resample-1.8.1rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 09:21:34.000000 resample-1.8.1rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 09:21:34.000000 resample-1.8.1rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 09:21:34.000000 resample-1.8.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 09:21:34.000000 resample-1.8.1rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-19 09:21:34.000000 resample-1.8.1rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 09:21:34.000000 resample-1.8.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 09:21:34.000000 resample-1.8.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-19 09:21:37.867431 resample-1.8.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-19 09:21:34.000000 resample-1.8.1rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.859431 resample-1.8.1rc1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 09:21:34.000000 resample-1.8.1rc1/benchmarks/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-19 09:21:34.000000 resample-1.8.1rc1/benchmarks/test_jackknife.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 09:21:34.000000 resample-1.8.1rc1/benchmarks/test_rcont.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-19 09:21:34.000000 resample-1.8.1rc1/benchmarks/test_usp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.863431 resample-1.8.1rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.863431 resample-1.8.1rc1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    46843 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86616 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/bench_rcont.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.863431 resample-1.8.1rc1/doc/example/
+-rw-r--r--   0 runner    (1001) docker     (127)   181138 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/example/tag_and_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/make_raw_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/plot_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.863431 resample-1.8.1rc1/doc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/tutorial/confidence_intervals.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/tutorial/jackknife_vs_bootstrap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    73522 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/tutorial/permutation_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   141793 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/tutorial/sklearn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42094 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/tutorial/usp_continuous_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/tutorial/variance_fit_parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-19 09:21:34.000000 resample-1.8.1rc1/doc/update_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-19 09:21:34.000000 resample-1.8.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:21:37.867431 resample-1.8.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.859431 resample-1.8.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.867431 resample-1.8.1rc1/src/resample/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 09:21:34.000000 resample-1.8.1rc1/src/resample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 09:21:34.000000 resample-1.8.1rc1/src/resample/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-19 09:21:34.000000 resample-1.8.1rc1/src/resample/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 09:21:34.000000 resample-1.8.1rc1/src/resample/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-19 09:21:34.000000 resample-1.8.1rc1/src/resample/jackknife.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-19 09:21:34.000000 resample-1.8.1rc1/src/resample/permutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.867431 resample-1.8.1rc1/src/resample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-19 09:21:37.000000 resample-1.8.1rc1/src/resample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-19 09:21:37.000000 resample-1.8.1rc1/src/resample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:21:37.000000 resample-1.8.1rc1/src/resample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 09:21:37.000000 resample-1.8.1rc1/src/resample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 09:21:37.000000 resample-1.8.1rc1/src/resample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:21:37.867431 resample-1.8.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-19 09:21:34.000000 resample-1.8.1rc1/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-19 09:21:34.000000 resample-1.8.1rc1/tests/test_empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-19 09:21:34.000000 resample-1.8.1rc1/tests/test_jackknife.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-19 09:21:34.000000 resample-1.8.1rc1/tests/test_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 09:21:34.000000 resample-1.8.1rc1/tests/test_util.py
```

### Comparing `resample-1.7.1/.github/workflows/docs.yml` & `resample-1.8.1rc1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/.github/workflows/release.yml` & `resample-1.8.1rc1/.github/workflows/release.yml`

 * *Files 17% similar despite different names*

```diff
@@ -10,28 +10,31 @@
   group: ${{ github.workflow }}-${{ github.head_ref }}
   cancel-in-progress: true
 
 env:
   PIP_ONLY_BINARY: ":all:"
 
 jobs:
-  build-and-publish:
+  release:
     runs-on: ubuntu-latest
 
+    environment:
+      name: pypi
+      url: https://pypi.org/p/resample
+    permissions:
+      id-token: write
+
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
           fetch-depth: 0  # needed by setuptools_scm
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
-        python-version: "3.10"
+        python-version: '3.11'
 
     - run: python -m pip install --upgrade pip build
     - run: python -m build
     - run: python -m pip install --prefer-binary $(echo dist/*.whl)'[test]'
     - run: python -m pytest
 
     - uses: pypa/gh-action-pypi-publish@release/v1
       if: github.event_name == 'push' && contains(github.event.ref, '/tags/')
-      with:
-        user: __token__
-        password: ${{ secrets.pypi_token }}
```

### Comparing `resample-1.7.1/.github/workflows/test.yml` & `resample-1.8.1rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/.pre-commit-config.yaml` & `resample-1.8.1rc1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 files: 'resample'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: check-case-conflict
   - id: check-docstring-first
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-yaml
   - id: debug-statements
@@ -14,24 +14,24 @@
   - id: mixed-line-ending
   - id: sort-simple-yaml
   - id: file-contents-sorter
   - id: trailing-whitespace
 
 # Ruff linter, replacement for flake8, isort, pydocstyle
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: 'v0.2.0'
+  rev: 'v0.3.7'
   hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
 
 # Python formatting
 - repo: https://github.com/psf/black-pre-commit-mirror
-  rev: 24.1.1
+  rev: 24.4.0
   hooks:
   - id: black
 
 # Python type checking
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: 'v1.8.0'
+  rev: 'v1.9.0'
   hooks:
   - id: mypy
     args: [--allow-redefinition, --ignore-missing-imports]
```

### Comparing `resample-1.7.1/CITATION.cff` & `resample-1.8.1rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/LICENSE` & `resample-1.8.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/PKG-INFO` & `resample-1.8.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resample
-Version: 1.7.1
+Version: 1.8.1rc1
 Summary: Resampling-based inference in Python
 Author-email: Daniel Saxton <dsaxton@pm.me>, Hans Dembinski <hans.dembinski@gmail.com>
 License: BSD-3-Clause
 Project-URL: repository, http://github.com/resample-project/resample
 Project-URL: documentation, https://resample.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `resample-1.7.1/README.rst` & `resample-1.8.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/benchmarks/test_bootstrap.py` & `resample-1.8.1rc1/benchmarks/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/benchmarks/test_jackknife.py` & `resample-1.8.1rc1/benchmarks/test_jackknife.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/benchmarks/test_rcont.py` & `resample-1.8.1rc1/benchmarks/test_rcont.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/benchmarks/test_usp.py` & `resample-1.8.1rc1/benchmarks/test_usp.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/Makefile` & `resample-1.8.1rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/_static/logo.svg` & `resample-1.8.1rc1/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/bench_rcont.json` & `resample-1.8.1rc1/doc/bench_rcont.json`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/changelog.rst` & `resample-1.8.1rc1/doc/changelog.rst`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/conf.py` & `resample-1.8.1rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/example/tag_and_probe.ipynb` & `resample-1.8.1rc1/doc/example/tag_and_probe.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/make.bat` & `resample-1.8.1rc1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/make_raw_logo.py` & `resample-1.8.1rc1/doc/make_raw_logo.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/plot_bench.py` & `resample-1.8.1rc1/doc/plot_bench.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/tutorial/confidence_intervals.ipynb` & `resample-1.8.1rc1/doc/tutorial/confidence_intervals.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/tutorial/jackknife_vs_bootstrap.ipynb` & `resample-1.8.1rc1/doc/tutorial/jackknife_vs_bootstrap.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/tutorial/permutation_tests.ipynb` & `resample-1.8.1rc1/doc/tutorial/permutation_tests.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/tutorial/sklearn.ipynb` & `resample-1.8.1rc1/doc/tutorial/sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/tutorial/usp_continuous_data.ipynb` & `resample-1.8.1rc1/doc/tutorial/usp_continuous_data.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/tutorial/variance_fit_parameters.ipynb` & `resample-1.8.1rc1/doc/tutorial/variance_fit_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/doc/update_changelog.py` & `resample-1.8.1rc1/doc/update_changelog.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/pyproject.toml` & `resample-1.8.1rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 [build-system]
-requires = [
-    "setuptools >= 61",
-    "setuptools_scm[toml] >= 6.2",
-]
+requires = ["setuptools >= 60", "setuptools_scm[toml] >= 8.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resample"
 requires-python = ">=3.8"
-dependencies = [
-    "numpy >= 1.21",
-    "scipy >= 1.10"
-]
+dependencies = ["numpy >= 1.21", "scipy >= 1.10"]
 authors = [
-    { name = "Daniel Saxton", email= "dsaxton@pm.me" },
-    { name = "Hans Dembinski", email = "hans.dembinski@gmail.com" }
+    { name = "Daniel Saxton", email = "dsaxton@pm.me" },
+    { name = "Hans Dembinski", email = "hans.dembinski@gmail.com" },
 ]
 readme = "README.rst"
 description = "Resampling-based inference in Python"
 license = { text = "BSD-3-Clause" }
 classifiers = [
     # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
     'Development Status :: 5 - Production/Stable',
@@ -38,23 +32,16 @@
 dynamic = ["version"]
 
 [project.urls]
 repository = "http://github.com/resample-project/resample"
 documentation = "https://resample.readthedocs.io/en/stable/"
 
 [project.optional-dependencies]
-test = [
-    "pytest",
-    "pytest-cov",
-    "coverage[toml]"
-]
-doc = [
-    "ipython",
-    "nbsphinx"
-]
+test = ["pytest", "pytest-cov", "coverage[toml]"]
+doc = ["ipython", "nbsphinx"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
 
 [tool.isort]
```

### Comparing `resample-1.7.1/src/resample/__init__.py` & `resample-1.8.1rc1/src/resample/__init__.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/src/resample/_util.py` & `resample-1.8.1rc1/src/resample/_util.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/src/resample/bootstrap.py` & `resample-1.8.1rc1/src/resample/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -291,14 +291,16 @@
     sample: "ArrayLike",
     *args: "ArrayLike",
     **kwargs: Any,
 ) -> np.ndarray:
     """
     Calculate bootstrap estimate of variance.
 
+    If the function returns a vector, the variance is computed elementwise.
+
     Parameters
     ----------
     fn : callable
         Estimator. Can be any mapping ℝⁿ → ℝᵏ, where n is the sample size
         and k is the length of the output array.
     sample : array-like
         Original sample.
@@ -323,14 +325,59 @@
     0.8
 
     """
     thetas = bootstrap(fn, sample, *args, **kwargs)
     return np.var(thetas, ddof=1, axis=0)
 
 
+def covariance(
+    fn: Callable[..., np.ndarray],
+    sample: "ArrayLike",
+    *args: "ArrayLike",
+    **kwargs: Any,
+) -> np.ndarray:
+    """
+    Calculate bootstrap estimate of covariance.
+
+    Parameters
+    ----------
+    fn : callable
+        Estimator. Can be any mapping ℝⁿ → ℝᵏ, where n is the sample size
+        and k is the length of the output array.
+    sample : array-like
+        Original sample.
+    *args : array-like
+        Optional additional arrays of the same length to resample.
+    **kwargs
+        Keyword arguments forwarded to :func:`resample`.
+
+    Returns
+    -------
+    ndarray
+        Bootstrap estimate of covariance. In general, this is a matrix, but if the
+        function maps to a scalar, it is scalar as well.
+
+    Examples
+    --------
+    Compute variance of arithmetic mean.
+
+    >>> from resample.bootstrap import variance
+    >>> import numpy as np
+    >>> x = np.arange(10)
+    >>> def fn(x):
+    ...     return np.mean(x), np.var(x)
+    >>> np.round(covariance(fn, x, size=10000, random_state=1), 1)
+    array([[0.8, 0. ],
+           [0. , 5.5]])
+
+    """
+    thetas = bootstrap(fn, sample, *args, **kwargs)
+    return np.cov(thetas, rowvar=False, ddof=1)
+
+
 def confidence_interval(
     fn: Callable[..., np.ndarray],
     sample: "ArrayLike",
     *args: "ArrayLike",
     cl: float = 0.95,
     ci_method: str = "bca",
     **kwargs: Any,
```

### Comparing `resample-1.7.1/src/resample/empirical.py` & `resample-1.8.1rc1/src/resample/empirical.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/src/resample/jackknife.py` & `resample-1.8.1rc1/src/resample/jackknife.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/src/resample/permutation.py` & `resample-1.8.1rc1/src/resample/permutation.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/src/resample.egg-info/PKG-INFO` & `resample-1.8.1rc1/src/resample.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resample
-Version: 1.7.1
+Version: 1.8.1rc1
 Summary: Resampling-based inference in Python
 Author-email: Daniel Saxton <dsaxton@pm.me>, Hans Dembinski <hans.dembinski@gmail.com>
 License: BSD-3-Clause
 Project-URL: repository, http://github.com/resample-project/resample
 Project-URL: documentation, https://resample.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `resample-1.7.1/src/resample.egg-info/SOURCES.txt` & `resample-1.8.1rc1/src/resample.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/tests/test_bootstrap.py` & `resample-1.8.1rc1/tests/test_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from resample.bootstrap import (
     _fit_parametric_family,
     bootstrap,
     confidence_interval,
     resample,
     variance,
+    covariance,
 )
 
 PARAMETRIC_CONTINUOUS = {
     # use scipy.stats names here
     "norm",
     "t",
     "laplace",
@@ -291,14 +292,25 @@
     data = np.arange(100)
     v = np.var(data) / len(data)
 
     r = variance(np.mean, data, size=1000, method=method, random_state=rng)
     assert r == pytest.approx(v, rel=0.05)
 
 
+@pytest.mark.parametrize("method", NON_PARAMETRIC)
+def test_covariance(method, rng):
+    cov = np.array([[1.0, 0.1], [0.1, 2.0]])
+    data = rng.multivariate_normal([0.1, 0.2], cov, size=1000)
+
+    r = covariance(
+        lambda x: np.mean(x, axis=0), data, size=1000, method=method, random_state=rng
+    )
+    assert_allclose(r, cov / len(data), atol=1e-3)
+
+
 def test_resample_deprecation(rng):
     data = [1, 2, 3]
     from numpy import VisibleDeprecationWarning
 
     with pytest.warns(VisibleDeprecationWarning):
         r = list(resample(data, 10))
         assert np.shape(r) == (10, 3)
```

### Comparing `resample-1.7.1/tests/test_empirical.py` & `resample-1.8.1rc1/tests/test_empirical.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/tests/test_jackknife.py` & `resample-1.8.1rc1/tests/test_jackknife.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/tests/test_permutation.py` & `resample-1.8.1rc1/tests/test_permutation.py`

 * *Files identical despite different names*

### Comparing `resample-1.7.1/tests/test_util.py` & `resample-1.8.1rc1/tests/test_util.py`

 * *Files identical despite different names*

