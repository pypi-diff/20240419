# Comparing `tmp/generic_exporters-0.0.6.tar.gz` & `tmp/generic_exporters-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic_exporters-0.0.6.tar", last modified: Thu Apr 18 01:39:15 2024, max compression
+gzip compressed data, was "generic_exporters-0.0.7.tar", last modified: Fri Apr 19 17:29:23 2024, max compression
```

## Comparing `generic_exporters-0.0.6.tar` & `generic_exporters-0.0.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.coverage
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:14.997583 generic_exporters-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.001582 generic_exporters-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/deploy-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.001582 generic_exporters-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:14.997583 generic_exporters-0.0.6/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:14.997583 generic_exporters-0.0.6/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.005582 generic_exporters-0.0.6/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.005582 generic_exporters-0.0.6/generic_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_awaitable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_mathable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/TODO.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/victoria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/exporters/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/framer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/processors/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/generic_exporters/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/generic_exporters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 01:39:14.000000 generic_exporters-0.0.6/generic_exporters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/processors/exporters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.009583 generic_exporters-0.0.6/tests/processors/exporters/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/test_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:15.013583 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_victoria.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/exporters/test_exporter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/processors/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_mathable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-18 01:39:03.000000 generic_exporters-0.0.6/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.646404 generic_exporters-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/.coverage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.630404 generic_exporters-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.634404 generic_exporters-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-19 17:29:23.646404 generic_exporters-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.634404 generic_exporters-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.630404 generic_exporters-0.0.7/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.630404 generic_exporters-0.0.7/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.638404 generic_exporters-0.0.7/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.638404 generic_exporters-0.0.7/generic_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/_awaitable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/_mathable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.642404 generic_exporters-0.0.7/generic_exporters/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.642404 generic_exporters-0.0.7/generic_exporters/processors/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.642404 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.642404 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/victoria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/exporters/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/framer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/processors/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/generic_exporters/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.646404 generic_exporters-0.0.7/generic_exporters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-19 17:29:23.000000 generic_exporters-0.0.7/generic_exporters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-19 17:29:23.000000 generic_exporters-0.0.7/generic_exporters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:29:23.000000 generic_exporters-0.0.7/generic_exporters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 17:29:23.000000 generic_exporters-0.0.7/generic_exporters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 17:29:23.000000 generic_exporters-0.0.7/generic_exporters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:29:23.646404 generic_exporters-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.642404 generic_exporters-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.642404 generic_exporters-0.0.7/tests/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.646404 generic_exporters-0.0.7/tests/processors/exporters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.646404 generic_exporters-0.0.7/tests/processors/exporters/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/processors/exporters/datastores/test_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:23.646404 generic_exporters-0.0.7/tests/processors/exporters/datastores/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/processors/exporters/datastores/timeseries/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/processors/exporters/datastores/timeseries/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/processors/exporters/datastores/timeseries/test_victoria.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/processors/exporters/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/processors/exporters/test_exporter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/processors/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/test_mathable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 17:29:08.000000 generic_exporters-0.0.7/tests/test_timeseries.py
```

### Comparing `generic_exporters-0.0.6/.coverage` & `generic_exporters-0.0.7/.coverage`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/.github/workflows/deploy-docs.yaml` & `generic_exporters-0.0.7/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/.github/workflows/pages.yml` & `generic_exporters-0.0.7/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/.github/workflows/pytest.yaml` & `generic_exporters-0.0.7/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/.github/workflows/release.yaml` & `generic_exporters-0.0.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/Makefile` & `generic_exporters-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/_build/html/_static/alabaster.css` & `generic_exporters-0.0.7/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/_build/html/_static/basic.css` & `generic_exporters-0.0.7/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/_build/html/_static/doctools.js` & `generic_exporters-0.0.7/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/_build/html/_static/language_data.js` & `generic_exporters-0.0.7/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/_build/html/_static/pygments.css` & `generic_exporters-0.0.7/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/_build/html/_static/searchtools.js` & `generic_exporters-0.0.7/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/_build/html/_static/sphinx_highlight.js` & `generic_exporters-0.0.7/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/conf.py` & `generic_exporters-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/docs/make.bat` & `generic_exporters-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/_awaitable.py` & `generic_exporters-0.0.7/generic_exporters/_awaitable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/_constant.py` & `generic_exporters-0.0.7/generic_exporters/_constant.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/_mathable.py` & `generic_exporters-0.0.7/generic_exporters/_mathable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/_time.py` & `generic_exporters-0.0.7/generic_exporters/_time.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/dataset.py` & `generic_exporters-0.0.7/generic_exporters/dataset.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/metric.py` & `generic_exporters-0.0.7/generic_exporters/metric.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/plan.py` & `generic_exporters-0.0.7/generic_exporters/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from decimal import Decimal
 from functools import cached_property
 from inspect import isawaitable
 from typing import (TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Coroutine, Dict, 
                     Iterable, Iterator, Mapping, Optional, Tuple, TypeVar, Union, final)
 
 import a_sync
+from a_sync.property import HiddenMethodDescriptor
 from bqplot import Figure
 from pandas import DataFrame
+from typing_extensions import Self
 
 from generic_exporters import _types
 from generic_exporters._awaitable import _AwaitableMixin
 from generic_exporters._time import _TimeDataBase
 from generic_exporters.dataset import Dataset
 from generic_exporters.timeseries import _TimeSeriesBase, TimeSeries, WideTimeSeries
 
@@ -25,14 +27,15 @@
     _M = TypeVar('_M')
 
 _T = TypeVar('_T', TimeSeries, WideTimeSeries)
 
 LooseDatetime = Union[datetime, Awaitable[datetime]]
 ReturnValue = Union[Decimal, Exception]
 
+
 logger = logging.getLogger(__name__)
 
 
 class _QueryPlan(_TimeDataBase, a_sync.ASyncIterable["TimeDataRow[_M]"], _AwaitableMixin[Dict[_M, _T]]):
     def __init__(
         self, 
         dataset: "Union[TimeSeries, WideTimeSeries]", 
@@ -86,36 +89,47 @@
         """
         from generic_exporters.processors import DataFramer
         return await DataFramer(self, interval=self.interval)
     
     async def _materialize(self) -> Dataset:
         """Materializes the query plan, executing the necessary asynchronous operations and returning the results."""
         return Dataset(await a_sync.map(self.__getitem__, self._aiter_timestamps()))
-
+    
+    @a_sync.cached_property
     async def start_timestamp(self) -> datetime:
         """Computes the start timestamp for the query, handling asynchronous resolution if necessary."""
-        return await self._start_timestamp if isawaitable(self._start_timestamp) else self._start_timestamp
+        timestamp = await self._start_timestamp if isawaitable(self._start_timestamp) else self._start_timestamp
+        return timestamp.astimezone(tz=timezone.utc)
+    __start_timestamp__: HiddenMethodDescriptor[Self, datetime]
 
     async def _aiter_timestamps(self, run_forever: bool = False) -> AsyncGenerator[datetime, None]:
         """Generates the timestamps to be queried based on the specified range and interval."""
-        timestamp: datetime = await self.start_timestamp(sync=False)
-        timestamp = timestamp.astimezone(tz=timezone.utc)
-        if run_forever is True:
-            while True:
-                while not _ts_is_ready(timestamp, self.interval):
-                    await asyncio.sleep((datetime.now(tz=timezone.utc) - self.interval - timestamp).total_seconds())
-                yield timestamp
-                timestamp += self.interval
-        elif run_forever is False:
-            while _ts_is_ready(timestamp, self.interval):
-                yield timestamp
-                timestamp += self.interval
-        else:
+        if not isinstance(run_forever, bool):
             raise TypeError(f'`run_forever` must be boolean. You passed {run_forever}')
 
+        timestamp: datetime = await self.__start_timestamp__
+
+        # gather historical timestamps
+        timestamps = []
+        while _ts_is_ready(timestamp, self.interval):
+            timestamps.append(timestamp)
+            timestamp = timestamp + self.interval
+
+        # yield historical timestamps hi-to-low
+        timestamps.reverse()
+        for timestamp in timestamps:
+            yield timestamp
+        del timestamps
+
+        while run_forever:
+            while not _ts_is_ready(timestamp, self.interval):
+                await _get_waiter(timestamp - self.interval)
+            yield timestamp
+            timestamp += self.interval
+
 
 @final
 class QueryPlan(_QueryPlan["Metric", Decimal]):
     """Represents a plan for querying time series data within a specified range.
 
     This class encapsulates the logic for generating and executing a plan to query
     time series data. It supports asynchronous iteration over the generated data points
@@ -182,7 +196,26 @@
         return a_sync.map(lambda metric: metric.produce(self.timestamp, sync=False), self.metrics)
     async def _materialize(self) -> Dict[_M, ReturnValue]:
         return await self.tasks
 
 @final
 class TimeDataRow(_TimeDataRow["Metric"]):
     """A future-like class that can be awaited to materialize results"""
+
+
+_waiters = {}
+
+async def _wait(wait_until: datetime) -> None:
+    await asyncio.sleep((wait_until - datetime.now(tz=timezone.utc)).total_seconds())
+
+def _wait_callback(t: asyncio.Task) -> None:
+    low_to_hi = sorted(_waiters)
+    for k in low_to_hi:
+        if _waiters[k] is t:
+            _waiters.pop(k)
+
+def _get_waiter(timestamp: datetime) -> "asyncio.Task[None]":
+    if timestamp not in _waiters:
+        waiter = asyncio.create_task(_wait(timestamp))
+        waiter.add_done_callback(_wait_callback)
+        _waiters[timestamp] = waiter
+    return _waiters[timestamp]
```

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/_base.py` & `generic_exporters-0.0.7/generic_exporters/processors/_base.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/exporters/_base.py` & `generic_exporters-0.0.7/generic_exporters/processors/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/default.py` & `generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/default.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/multi.py` & `generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/multi.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/sql.py` & `generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # TODO
 import asyncio
 from datetime import datetime
 from typing import Any, Dict, Optional
 
+import a_sync
 from concurrent.futures import ThreadPoolExecutor
 from msgspec.json import encode
-from pony.orm import Database, Json, PrimaryKey, Required, db_session, select
+from pony.orm import Database, PrimaryKey, Required, db_session, select
 from pony.orm.core import Query
 
 from generic_exporters.processors.exporters.datastores.timeseries._base import TimeSeriesDataStoreBase
 
 
 Jsonable = Any
 
 db = Database()
 
 class SQLTimeSeriesKeyValueStore(TimeSeriesDataStoreBase):
+    push = None  # make abc work TODO refactor this out
     def __init__(self, **connection_params: Optional[Dict[str, Any]]) -> None:
         if not connection_params:
             from generic_exporters.processors.exporters.datastores.default import sqlite_settings as connection_params
         db.bind(**connection_params)
         db.generate_mapping(create_tables=True)
+        self.push = a_sync.ProcessingQueue(self._push, num_workers=10_000, return_data=False)
     async def data_exists(self, key: Jsonable, ts: datetime) -> bool:
         """Returns True if `key` returns results from your Postgres db at `ts`, False if not."""
         if (result_count := await TimeSeriesKV.count(key, ts)) == 0:
             return False
         elif result_count == 1:
             return True
         raise ValueError(f"`result_count` should not be > 1 but is {result_count}")
-    async def push(self, key: Jsonable, ts: datetime, value: Jsonable) -> None:
+    
+    async def _push(self, key: Jsonable, ts: datetime, value: Jsonable) -> None:
         """Exports `data` to Victoria Metrics using `key` somehow. lol"""
         await TimeSeriesKV.insert(key, ts, value)
 
 
 db_thread = ThreadPoolExecutor(1)
 
 class TimeSeriesKV(db.Entity):
```

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/exporters/datastores/timeseries/victoria.py` & `generic_exporters-0.0.7/generic_exporters/processors/exporters/datastores/timeseries/victoria.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/exporters/exporter.py` & `generic_exporters-0.0.7/generic_exporters/processors/exporters/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,31 +23,30 @@
         buffer: timedelta = timedelta(minutes=5), 
         concurrency: Optional[int] = None, 
         sync: bool = True,
     ) -> None:
         super().__init__(query, datastore, concurrency=concurrency, sync=sync)
         self.buffer = buffer
         self.ensure_data = a_sync.ProcessingQueue(self._ensure_data, concurrency, return_data=False)
-        self._push = a_sync.ProcessingQueue(self.datastore.push, concurrency*10, return_data=False)
 
     @overload
     async def run(self, run_forever: Literal[True]) -> NoReturn:...
     @overload
     async def run(self, run_forever: Literal[False]) -> None:...
     async def run(self, run_forever: bool = False) -> Union[None, NoReturn]:
         """Exports the full history for this exporter's `Metric` to the datastore"""
         async for ts in self.query._aiter_timestamps(run_forever):
             self.ensure_data(ts)
         # wait for all rpc activity to complete
         await self.ensure_data.join()
         # wait for all data to be pushed to datastore
-        await self._push.join()
+        await self.datastore.push.join()
     
     @abstractmethod
     async def data_exists(self, timestamp: datetime) -> bool:
         """Returns True if data exists at `timestamp`, False if it does not and must be exported."""
 
     async def _ensure_data(self, ts: datetime) -> None:
         if not await self.data_exists(ts, sync=False):
             data = await self.query[ts]
             for key, value in data.items():
-                self._push(key, ts, value)
+                self.datastore.push(key, ts, value)
```

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/framer.py` & `generic_exporters-0.0.7/generic_exporters/processors/framer.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/processors/plotter.py` & `generic_exporters-0.0.7/generic_exporters/processors/plotter.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters/timeseries.py` & `generic_exporters-0.0.7/generic_exporters/timeseries.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/generic_exporters.egg-info/SOURCES.txt` & `generic_exporters-0.0.7/generic_exporters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/setup.py` & `generic_exporters-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/fixtures.py` & `generic_exporters-0.0.7/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/processors/exporters/datastores/test_multi.py` & `generic_exporters-0.0.7/tests/processors/exporters/datastores/test_multi.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_sql.py` & `generic_exporters-0.0.7/tests/processors/exporters/datastores/timeseries/test_sql.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/processors/exporters/datastores/timeseries/test_victoria.py` & `generic_exporters-0.0.7/tests/processors/exporters/datastores/timeseries/test_victoria.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/processors/test_base.py` & `generic_exporters-0.0.7/tests/processors/test_base.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/test_constant.py` & `generic_exporters-0.0.7/tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/test_dataset.py` & `generic_exporters-0.0.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/test_mathable.py` & `generic_exporters-0.0.7/tests/test_mathable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/test_metric.py` & `generic_exporters-0.0.7/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/test_plan.py` & `generic_exporters-0.0.7/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.6/tests/test_timeseries.py` & `generic_exporters-0.0.7/tests/test_timeseries.py`

 * *Files identical despite different names*

