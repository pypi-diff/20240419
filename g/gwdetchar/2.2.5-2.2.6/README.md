# Comparing `tmp/gwdetchar-2.2.5.tar.gz` & `tmp/gwdetchar-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.2.5.tar", last modified: Wed Apr 17 22:08:31 2024, max compression
+gzip compressed data, was "gwdetchar-2.2.6.tar", last modified: Fri Apr 19 00:15:42 2024, max compression
```

## Comparing `gwdetchar-2.2.5.tar` & `gwdetchar-2.2.6.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.646236 gwdetchar-2.2.5/
--rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/.codecov.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)       35 2023-09-20 21:04:35.000000 gwdetchar-2.2.5/.gitattributes
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.562078 gwdetchar-2.2.5/.github/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.576488 gwdetchar-2.2.5/.github/workflows/
--rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/.github/workflows/build.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/.github/workflows/docs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1377 2023-06-28 17:53:22.000000 gwdetchar-2.2.5/.github/workflows/lint.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/.gitignore
--rw-r--r--   0 egoetz     (501) staff       (20)      528 2023-11-17 16:53:31.000000 gwdetchar-2.2.5/.readthedocs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-09-20 20:17:46.000000 gwdetchar-2.2.5/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     4572 2024-04-17 22:08:31.645474 gwdetchar-2.2.5/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.577252 gwdetchar-2.2.5/ci/
--rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/ci/test-cli.sh
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.579687 gwdetchar-2.2.5/docs/
--rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/Makefile
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.562671 gwdetchar-2.2.5/docs/_static/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.580510 gwdetchar-2.2.5/docs/_static/css/
--rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/_static/css/custom.css
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.581092 gwdetchar-2.2.5/docs/api/
--rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/api/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/docs/conf.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.581705 gwdetchar-2.2.5/docs/conlog/
--rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/conlog/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.582565 gwdetchar-2.2.5/docs/daq/
--rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/docs/daq/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.583198 gwdetchar-2.2.5/docs/data/
--rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/data/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.583762 gwdetchar-2.2.5/docs/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/html/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.584201 gwdetchar-2.2.5/docs/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/lasso/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.584784 gwdetchar-2.2.5/docs/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/docs/nagios/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.585234 gwdetchar-2.2.5/docs/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/docs/omega/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.585753 gwdetchar-2.2.5/docs/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/docs/saturation/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.586271 gwdetchar-2.2.5/docs/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/docs/scattering/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.595656 gwdetchar-2.2.5/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.2.5/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-17 22:08:31.000000 gwdetchar-2.2.5/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.2.5/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.2.5/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.2.5/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.601381 gwdetchar-2.2.5/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.2.5/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    42120 2024-04-17 22:04:34.000000 gwdetchar-2.2.5/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.2.5/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.604631 gwdetchar-2.2.5/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    24217 2024-04-17 22:04:34.000000 gwdetchar-2.2.5/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.2.5/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.609609 gwdetchar-2.2.5/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    51942 2024-03-22 19:53:47.000000 gwdetchar-2.2.5/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.2.5/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.612781 gwdetchar-2.2.5/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.2.5/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.614656 gwdetchar-2.2.5/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.615965 gwdetchar-2.2.5/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.621404 gwdetchar-2.2.5/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14012 2023-08-04 18:20:44.000000 gwdetchar-2.2.5/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14414 2023-12-22 23:45:48.000000 gwdetchar-2.2.5/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20702 2024-03-22 19:53:47.000000 gwdetchar-2.2.5/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.625851 gwdetchar-2.2.5/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13519 2024-04-17 22:04:34.000000 gwdetchar-2.2.5/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.628203 gwdetchar-2.2.5/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.629402 gwdetchar-2.2.5/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.633014 gwdetchar-2.2.5/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32280 2024-03-22 19:53:47.000000 gwdetchar-2.2.5/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.636100 gwdetchar-2.2.5/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.642346 gwdetchar-2.2.5/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.2.5/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.2.5/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-17 22:08:31.643020 gwdetchar-2.2.5/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     4572 2024-04-17 22:08:31.000000 gwdetchar-2.2.5/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2832 2024-04-17 22:08:31.000000 gwdetchar-2.2.5/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-17 22:08:31.000000 gwdetchar-2.2.5/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2024-04-17 22:08:31.000000 gwdetchar-2.2.5/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      356 2024-04-17 22:08:31.000000 gwdetchar-2.2.5/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2024-04-17 22:08:31.000000 gwdetchar-2.2.5/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3465 2023-09-20 20:17:46.000000 gwdetchar-2.2.5/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-17 22:08:31.646379 gwdetchar-2.2.5/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.298390 gwdetchar-2.2.6/
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       35 2023-09-20 21:04:35.000000 gwdetchar-2.2.6/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.203400 gwdetchar-2.2.6/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.216274 gwdetchar-2.2.6/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/.github/workflows/docs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1377 2023-06-28 17:53:22.000000 gwdetchar-2.2.6/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      528 2023-11-17 16:53:31.000000 gwdetchar-2.2.6/.readthedocs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-09-20 20:17:46.000000 gwdetchar-2.2.6/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     4572 2024-04-19 00:15:42.297594 gwdetchar-2.2.6/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.216845 gwdetchar-2.2.6/ci/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/ci/test-cli.sh
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.218769 gwdetchar-2.2.6/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.204504 gwdetchar-2.2.6/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.219506 gwdetchar-2.2.6/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.220131 gwdetchar-2.2.6/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.220749 gwdetchar-2.2.6/docs/conlog/
+-rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/conlog/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.221421 gwdetchar-2.2.6/docs/daq/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/docs/daq/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.222095 gwdetchar-2.2.6/docs/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/data/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.222769 gwdetchar-2.2.6/docs/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/html/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.223474 gwdetchar-2.2.6/docs/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/lasso/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.224203 gwdetchar-2.2.6/docs/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/docs/nagios/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.224900 gwdetchar-2.2.6/docs/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/docs/omega/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.225869 gwdetchar-2.2.6/docs/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/docs/saturation/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.226637 gwdetchar-2.2.6/docs/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/docs/scattering/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.238312 gwdetchar-2.2.6/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.2.6/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-19 00:15:42.000000 gwdetchar-2.2.6/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.2.6/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.2.6/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.2.6/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.245729 gwdetchar-2.2.6/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.2.6/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    42120 2024-04-19 00:13:16.000000 gwdetchar-2.2.6/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.2.6/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.250044 gwdetchar-2.2.6/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24217 2024-04-17 22:04:34.000000 gwdetchar-2.2.6/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.2.6/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.255131 gwdetchar-2.2.6/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    51942 2024-03-22 19:53:47.000000 gwdetchar-2.2.6/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.2.6/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.258134 gwdetchar-2.2.6/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.2.6/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.260038 gwdetchar-2.2.6/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.260945 gwdetchar-2.2.6/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.265843 gwdetchar-2.2.6/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14012 2023-08-04 18:20:44.000000 gwdetchar-2.2.6/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14414 2023-12-22 23:45:48.000000 gwdetchar-2.2.6/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20702 2024-03-22 19:53:47.000000 gwdetchar-2.2.6/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.270165 gwdetchar-2.2.6/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13519 2024-04-17 22:04:34.000000 gwdetchar-2.2.6/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.273413 gwdetchar-2.2.6/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.275138 gwdetchar-2.2.6/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.280020 gwdetchar-2.2.6/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32280 2024-03-22 19:53:47.000000 gwdetchar-2.2.6/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.287480 gwdetchar-2.2.6/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.294557 gwdetchar-2.2.6/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.2.6/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.2.6/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 00:15:42.295322 gwdetchar-2.2.6/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4572 2024-04-19 00:15:42.000000 gwdetchar-2.2.6/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2832 2024-04-19 00:15:42.000000 gwdetchar-2.2.6/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-19 00:15:42.000000 gwdetchar-2.2.6/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2024-04-19 00:15:42.000000 gwdetchar-2.2.6/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      356 2024-04-19 00:15:42.000000 gwdetchar-2.2.6/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2024-04-19 00:15:42.000000 gwdetchar-2.2.6/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3465 2023-09-20 20:17:46.000000 gwdetchar-2.2.6/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-19 00:15:42.298535 gwdetchar-2.2.6/setup.cfg
```

### Comparing `gwdetchar-2.2.5/.github/workflows/build.yml` & `gwdetchar-2.2.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/.github/workflows/docs.yml` & `gwdetchar-2.2.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/.github/workflows/lint.yml` & `gwdetchar-2.2.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/.gitignore` & `gwdetchar-2.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/.readthedocs.yml` & `gwdetchar-2.2.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/CONTRIBUTING.md` & `gwdetchar-2.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/LICENSE` & `gwdetchar-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/PKG-INFO` & `gwdetchar-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.2.5
+Version: 2.2.6
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.2.5/README.rst` & `gwdetchar-2.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/ci/test-cli.sh` & `gwdetchar-2.2.6/ci/test-cli.sh`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/Makefile` & `gwdetchar-2.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/_static/css/custom.css` & `gwdetchar-2.2.6/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/conf.py` & `gwdetchar-2.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/conlog/index.rst` & `gwdetchar-2.2.6/docs/conlog/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/daq/index.rst` & `gwdetchar-2.2.6/docs/daq/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/data/index.rst` & `gwdetchar-2.2.6/docs/data/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/html/index.rst` & `gwdetchar-2.2.6/docs/html/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/index.rst` & `gwdetchar-2.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/lasso/index.rst` & `gwdetchar-2.2.6/docs/lasso/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/nagios/index.rst` & `gwdetchar-2.2.6/docs/nagios/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/omega/index.rst` & `gwdetchar-2.2.6/docs/omega/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/saturation/index.rst` & `gwdetchar-2.2.6/docs/saturation/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/docs/scattering/index.rst` & `gwdetchar-2.2.6/docs/scattering/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/__init__.py` & `gwdetchar-2.2.6/gwdetchar/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/cds.py` & `gwdetchar-2.2.6/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/cli.py` & `gwdetchar-2.2.6/gwdetchar/cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/condor.py` & `gwdetchar-2.2.6/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/conftest.py` & `gwdetchar-2.2.6/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/conlog.py` & `gwdetchar-2.2.6/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/const.py` & `gwdetchar-2.2.6/gwdetchar/const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/daq.py` & `gwdetchar-2.2.6/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/io/__init__.py` & `gwdetchar-2.2.6/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/io/datafind.py` & `gwdetchar-2.2.6/gwdetchar/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/io/html.py` & `gwdetchar-2.2.6/gwdetchar/io/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,17 +116,17 @@
 JQUERY_LAZY_JS = ('https://cdnjs.cloudflare.com/ajax/libs/jquery.lazy/'
                   '1.7.11/jquery.lazy.min.js')
 BOOTSTRAP_JS = ('https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/'
                 'dist/js/bootstrap.bundle.min.js')
 FANCYBOX_JS = ('https://cdn.jsdelivr.net/npm/@fancyapps/ui@5.0/'
                'dist/fancybox/fancybox.umd.js')
 
-GWBOOTSTRAP_CSS = ('https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.5/'
+GWBOOTSTRAP_CSS = ('https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.6/'
                    'lib/gwbootstrap.min.css')
-GWBOOTSTRAP_JS = ('https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.5/'
+GWBOOTSTRAP_JS = ('https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.6/'
                   'lib/gwbootstrap.min.js')
 
 CSS_FILES = [
     FONT_AWESOME_CSS,
     FONT_AWESOME_SOLID_CSS,
     GWBOOTSTRAP_CSS,
 ]
```

### Comparing `gwdetchar-2.2.5/gwdetchar/io/ligolw.py` & `gwdetchar-2.2.6/gwdetchar/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.2.6/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.2.6/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.2.6/gwdetchar/io/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.2.6/gwdetchar/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/__init__.py` & `gwdetchar-2.2.6/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/__main__.py` & `gwdetchar-2.2.6/gwdetchar/lasso/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/core.py` & `gwdetchar-2.2.6/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/old.py` & `gwdetchar-2.2.6/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/plot.py` & `gwdetchar-2.2.6/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.2.6/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.2.6/gwdetchar/lasso/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.2.6/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.2.6/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/mct.py` & `gwdetchar-2.2.6/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/nagios/__init__.py` & `gwdetchar-2.2.6/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/nagios/__main__.py` & `gwdetchar-2.2.6/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/nagios/core.py` & `gwdetchar-2.2.6/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.2.6/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.2.6/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/__init__.py` & `gwdetchar-2.2.6/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/__main__.py` & `gwdetchar-2.2.6/gwdetchar/omega/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/batch.py` & `gwdetchar-2.2.6/gwdetchar/omega/batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/config.py` & `gwdetchar-2.2.6/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/core.py` & `gwdetchar-2.2.6/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/html.py` & `gwdetchar-2.2.6/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/plot.py` & `gwdetchar-2.2.6/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.2.6/gwdetchar/omega/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.2.6/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.2.6/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.2.6/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.2.6/gwdetchar/omega/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.2.6/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.2.6/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/overflow.py` & `gwdetchar-2.2.6/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/plot.py` & `gwdetchar-2.2.6/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/saturation/__init__.py` & `gwdetchar-2.2.6/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/saturation/__main__.py` & `gwdetchar-2.2.6/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/saturation/core.py` & `gwdetchar-2.2.6/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.2.6/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.2.6/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/__init__.py` & `gwdetchar-2.2.6/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/__main__.py` & `gwdetchar-2.2.6/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/core.py` & `gwdetchar-2.2.6/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/plot.py` & `gwdetchar-2.2.6/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/simple.py` & `gwdetchar-2.2.6/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.2.6/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.2.6/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.2.6/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.2.6/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.2.6/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/__init__.py` & `gwdetchar-2.2.6/gwdetchar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_cds.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_cli.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_condor.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_const.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_daq.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_plot.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/tests/test_utils.py` & `gwdetchar-2.2.6/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar/utils.py` & `gwdetchar-2.2.6/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.2.6/gwdetchar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.2.5
+Version: 2.2.6
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.2.5/gwdetchar.egg-info/SOURCES.txt` & `gwdetchar-2.2.6/gwdetchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.2.6/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.2.5/pyproject.toml` & `gwdetchar-2.2.6/pyproject.toml`

 * *Files identical despite different names*

