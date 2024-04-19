# Comparing `tmp/iterative_ensemble_smoother-0.2.5.tar.gz` & `tmp/iterative_ensemble_smoother-0.2.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterative_ensemble_smoother-0.2.5.tar", last modified: Fri Apr 19 06:53:14 2024, max compression
+gzip compressed data, was "iterative_ensemble_smoother-0.2.5b0.tar", last modified: Fri Apr 12 11:55:15 2024, max compression
```

## Comparing `iterative_ensemble_smoother-0.2.5.tar` & `iterative_ensemble_smoother-0.2.5b0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.521528 iterative_ensemble_smoother-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.509528 iterative_ensemble_smoother-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.513528 iterative_ensemble_smoother-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.github/workflows/precommit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.github/workflows/upload_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/LITERATURE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-19 06:53:14.521528 iterative_ensemble_smoother-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.509528 iterative_ensemble_smoother-0.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.513528 iterative_ensemble_smoother-0.2.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/Adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/LinearRegression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/Oscillator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/Polynomial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.509528 iterative_ensemble_smoother-0.2.5/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.517528 iterative_ensemble_smoother-0.2.5/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/docs/source/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 06:53:14.521528 iterative_ensemble_smoother-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.509528 iterative_ensemble_smoother-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.517528 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 06:53:14.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/esmda.py
--rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/esmda_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/sies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/sies_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.517528 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-19 06:53:14.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-19 06:53:14.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:53:14.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 06:53:14.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 06:53:14.000000 iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.517528 iterative_ensemble_smoother-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.509528 iterative_ensemble_smoother-0.2.5/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.509528 iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.517528 iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.517528 iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:53:14.517528 iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/test_esmda.py
--rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/test_esmda_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19917 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    35674 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tests/test_sies.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-19 06:53:11.000000 iterative_ensemble_smoother-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.114689 iterative_ensemble_smoother-0.2.5b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/precommit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/upload_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/LITERATURE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.114689 iterative_ensemble_smoother-0.2.5b0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/Adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/LinearRegression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/Oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/Polynomial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_esmda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_esmda_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19917 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35674 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_sies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tox.ini
```

### Comparing `iterative_ensemble_smoother-0.2.5/.github/workflows/testing.yml` & `iterative_ensemble_smoother-0.2.5b0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/.github/workflows/upload_to_pypi.yml` & `iterative_ensemble_smoother-0.2.5b0/.github/workflows/upload_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/.gitignore` & `iterative_ensemble_smoother-0.2.5b0/.gitignore`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/.pre-commit-config.yaml` & `iterative_ensemble_smoother-0.2.5b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/CODE_OF_CONDUCT.md` & `iterative_ensemble_smoother-0.2.5b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/COPYING` & `iterative_ensemble_smoother-0.2.5b0/COPYING`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/LITERATURE.md` & `iterative_ensemble_smoother-0.2.5b0/LITERATURE.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/PKG-INFO` & `iterative_ensemble_smoother-0.2.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterative_ensemble_smoother
-Version: 0.2.5
+Version: 0.2.5b0
 Summary: A library for the iterative ensemble smoother algorithm.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>, Feda Curic <fcur@equinor.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Repository, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Bug Tracker, https://github.com/equinor/iterative_ensemble_smoother/issues
```

### Comparing `iterative_ensemble_smoother-0.2.5/README.md` & `iterative_ensemble_smoother-0.2.5b0/README.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/SECURITY.md` & `iterative_ensemble_smoother-0.2.5b0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/Adaptive.py` & `iterative_ensemble_smoother-0.2.5b0/docs/source/Adaptive.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/LinearRegression.py` & `iterative_ensemble_smoother-0.2.5b0/docs/source/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/Oscillator.py` & `iterative_ensemble_smoother-0.2.5b0/docs/source/Oscillator.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/Polynomial.py` & `iterative_ensemble_smoother-0.2.5b0/docs/source/Polynomial.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/_templates/autosummary/module.rst` & `iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/conf.py` & `iterative_ensemble_smoother-0.2.5b0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/glossary.rst` & `iterative_ensemble_smoother-0.2.5b0/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/docs/source/refs.bib` & `iterative_ensemble_smoother-0.2.5b0/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/pyproject.toml` & `iterative_ensemble_smoother-0.2.5b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/__init__.py` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/__init__.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/esmda.py` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/esmda_inversion.py` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda_inversion.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/experimental.py` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/experimental.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/sies.py` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/sies_inversion.py` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies_inversion.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother/utils.py` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/utils.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/PKG-INFO` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterative_ensemble_smoother
-Version: 0.2.5
+Version: 0.2.5b0
 Summary: A library for the iterative ensemble smoother algorithm.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>, Feda Curic <fcur@equinor.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Repository, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Bug Tracker, https://github.com/equinor/iterative_ensemble_smoother/issues
```

### Comparing `iterative_ensemble_smoother-0.2.5/src/iterative_ensemble_smoother.egg-info/SOURCES.txt` & `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv` & `iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv` & `iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv` & `iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tests/test_esmda.py` & `iterative_ensemble_smoother-0.2.5b0/tests/test_esmda.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tests/test_esmda_inversion.py` & `iterative_ensemble_smoother-0.2.5b0/tests/test_esmda_inversion.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tests/test_experimental.py` & `iterative_ensemble_smoother-0.2.5b0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tests/test_sies.py` & `iterative_ensemble_smoother-0.2.5b0/tests/test_sies.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5/tox.ini` & `iterative_ensemble_smoother-0.2.5b0/tox.ini`

 * *Files identical despite different names*

