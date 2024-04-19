# Comparing `tmp/resample-1.8.1.tar.gz` & `tmp/resample-1.8.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resample-1.8.1.tar", last modified: Fri Apr 19 09:23:58 2024, max compression
+gzip compressed data, was "resample-1.8.1rc1.tar", last modified: Fri Apr 19 09:21:37 2024, max compression
```

## Comparing `resample-1.8.1.tar` & `resample-1.8.1rc1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.161780 resample-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 09:23:51.000000 resample-1.8.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.149780 resample-1.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.153780 resample-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-19 09:23:51.000000 resample-1.8.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-19 09:23:51.000000 resample-1.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 09:23:51.000000 resample-1.8.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 09:23:51.000000 resample-1.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 09:23:51.000000 resample-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 09:23:51.000000 resample-1.8.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-19 09:23:51.000000 resample-1.8.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 09:23:51.000000 resample-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 09:23:51.000000 resample-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-19 09:23:58.161780 resample-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-19 09:23:51.000000 resample-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.153780 resample-1.8.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 09:23:51.000000 resample-1.8.1/benchmarks/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-19 09:23:51.000000 resample-1.8.1/benchmarks/test_jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 09:23:51.000000 resample-1.8.1/benchmarks/test_rcont.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-19 09:23:51.000000 resample-1.8.1/benchmarks/test_usp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.153780 resample-1.8.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 09:23:51.000000 resample-1.8.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.157780 resample-1.8.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    46843 2024-04-19 09:23:51.000000 resample-1.8.1/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86616 2024-04-19 09:23:51.000000 resample-1.8.1/doc/bench_rcont.json
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-19 09:23:51.000000 resample-1.8.1/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-19 09:23:51.000000 resample-1.8.1/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.157780 resample-1.8.1/doc/example/
--rw-r--r--   0 runner    (1001) docker     (127)   181138 2024-04-19 09:23:51.000000 resample-1.8.1/doc/example/tag_and_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 09:23:51.000000 resample-1.8.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-19 09:23:51.000000 resample-1.8.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 09:23:51.000000 resample-1.8.1/doc/make_raw_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 09:23:51.000000 resample-1.8.1/doc/plot_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-19 09:23:51.000000 resample-1.8.1/doc/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.157780 resample-1.8.1/doc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-19 09:23:51.000000 resample-1.8.1/doc/tutorial/confidence_intervals.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-19 09:23:51.000000 resample-1.8.1/doc/tutorial/jackknife_vs_bootstrap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    73522 2024-04-19 09:23:51.000000 resample-1.8.1/doc/tutorial/permutation_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   141793 2024-04-19 09:23:51.000000 resample-1.8.1/doc/tutorial/sklearn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42094 2024-04-19 09:23:51.000000 resample-1.8.1/doc/tutorial/usp_continuous_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-04-19 09:23:51.000000 resample-1.8.1/doc/tutorial/variance_fit_parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 09:23:51.000000 resample-1.8.1/doc/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-19 09:23:51.000000 resample-1.8.1/doc/update_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-19 09:23:51.000000 resample-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:23:58.161780 resample-1.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.149780 resample-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.157780 resample-1.8.1/src/resample/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 09:23:51.000000 resample-1.8.1/src/resample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 09:23:51.000000 resample-1.8.1/src/resample/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-19 09:23:51.000000 resample-1.8.1/src/resample/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 09:23:51.000000 resample-1.8.1/src/resample/empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-19 09:23:51.000000 resample-1.8.1/src/resample/jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-19 09:23:51.000000 resample-1.8.1/src/resample/permutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.161780 resample-1.8.1/src/resample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-19 09:23:58.000000 resample-1.8.1/src/resample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-19 09:23:58.000000 resample-1.8.1/src/resample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:23:58.000000 resample-1.8.1/src/resample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 09:23:58.000000 resample-1.8.1/src/resample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 09:23:58.000000 resample-1.8.1/src/resample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:23:58.161780 resample-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-19 09:23:51.000000 resample-1.8.1/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-19 09:23:51.000000 resample-1.8.1/tests/test_empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-19 09:23:51.000000 resample-1.8.1/tests/test_jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-19 09:23:51.000000 resample-1.8.1/tests/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 09:23:51.000000 resample-1.8.1/tests/test_util.py
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

### Comparing `resample-1.8.1/.github/workflows/docs.yml` & `resample-1.8.1rc1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/.github/workflows/release.yml` & `resample-1.8.1rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/.github/workflows/test.yml` & `resample-1.8.1rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/.pre-commit-config.yaml` & `resample-1.8.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/CITATION.cff` & `resample-1.8.1rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/LICENSE` & `resample-1.8.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/PKG-INFO` & `resample-1.8.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resample
-Version: 1.8.1
+Version: 1.8.1rc1
 Summary: Resampling-based inference in Python
 Author-email: Daniel Saxton <dsaxton@pm.me>, Hans Dembinski <hans.dembinski@gmail.com>
 License: BSD-3-Clause
 Project-URL: repository, http://github.com/resample-project/resample
 Project-URL: documentation, https://resample.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `resample-1.8.1/README.rst` & `resample-1.8.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/benchmarks/test_bootstrap.py` & `resample-1.8.1rc1/benchmarks/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/benchmarks/test_jackknife.py` & `resample-1.8.1rc1/benchmarks/test_jackknife.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/benchmarks/test_rcont.py` & `resample-1.8.1rc1/benchmarks/test_rcont.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/benchmarks/test_usp.py` & `resample-1.8.1rc1/benchmarks/test_usp.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/Makefile` & `resample-1.8.1rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/_static/logo.svg` & `resample-1.8.1rc1/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/bench_rcont.json` & `resample-1.8.1rc1/doc/bench_rcont.json`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/changelog.rst` & `resample-1.8.1rc1/doc/changelog.rst`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/conf.py` & `resample-1.8.1rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/example/tag_and_probe.ipynb` & `resample-1.8.1rc1/doc/example/tag_and_probe.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/make.bat` & `resample-1.8.1rc1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/make_raw_logo.py` & `resample-1.8.1rc1/doc/make_raw_logo.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/plot_bench.py` & `resample-1.8.1rc1/doc/plot_bench.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/tutorial/confidence_intervals.ipynb` & `resample-1.8.1rc1/doc/tutorial/confidence_intervals.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/tutorial/jackknife_vs_bootstrap.ipynb` & `resample-1.8.1rc1/doc/tutorial/jackknife_vs_bootstrap.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/tutorial/permutation_tests.ipynb` & `resample-1.8.1rc1/doc/tutorial/permutation_tests.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/tutorial/sklearn.ipynb` & `resample-1.8.1rc1/doc/tutorial/sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/tutorial/usp_continuous_data.ipynb` & `resample-1.8.1rc1/doc/tutorial/usp_continuous_data.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/tutorial/variance_fit_parameters.ipynb` & `resample-1.8.1rc1/doc/tutorial/variance_fit_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/doc/update_changelog.py` & `resample-1.8.1rc1/doc/update_changelog.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/pyproject.toml` & `resample-1.8.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/src/resample/__init__.py` & `resample-1.8.1rc1/src/resample/__init__.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/src/resample/_util.py` & `resample-1.8.1rc1/src/resample/_util.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/src/resample/bootstrap.py` & `resample-1.8.1rc1/src/resample/bootstrap.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/src/resample/empirical.py` & `resample-1.8.1rc1/src/resample/empirical.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/src/resample/jackknife.py` & `resample-1.8.1rc1/src/resample/jackknife.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/src/resample/permutation.py` & `resample-1.8.1rc1/src/resample/permutation.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/src/resample.egg-info/PKG-INFO` & `resample-1.8.1rc1/src/resample.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resample
-Version: 1.8.1
+Version: 1.8.1rc1
 Summary: Resampling-based inference in Python
 Author-email: Daniel Saxton <dsaxton@pm.me>, Hans Dembinski <hans.dembinski@gmail.com>
 License: BSD-3-Clause
 Project-URL: repository, http://github.com/resample-project/resample
 Project-URL: documentation, https://resample.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `resample-1.8.1/src/resample.egg-info/SOURCES.txt` & `resample-1.8.1rc1/src/resample.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/tests/test_bootstrap.py` & `resample-1.8.1rc1/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/tests/test_empirical.py` & `resample-1.8.1rc1/tests/test_empirical.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/tests/test_jackknife.py` & `resample-1.8.1rc1/tests/test_jackknife.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/tests/test_permutation.py` & `resample-1.8.1rc1/tests/test_permutation.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.1/tests/test_util.py` & `resample-1.8.1rc1/tests/test_util.py`

 * *Files identical despite different names*

