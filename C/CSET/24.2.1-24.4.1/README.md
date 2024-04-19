# Comparing `tmp/CSET-24.2.1.tar.gz` & `tmp/cset-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CSET-24.2.1.tar", last modified: Mon Mar  4 09:19:06 2024, max compression
+gzip compressed data, was "cset-24.4.1.tar", last modified: Fri Apr 19 08:36:34 2024, max compression
```

## Comparing `CSET-24.2.1.tar` & `cset-24.4.1.tar`

### file list

```diff
@@ -1,118 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.994437 CSET-24.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-03-04 09:18:38.000000 CSET-24.2.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-04 09:18:38.000000 CSET-24.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-04 09:19:06.994437 CSET-24.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-04 09:18:38.000000 CSET-24.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.966437 CSET-24.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.966437 CSET-24.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.966437 CSET-24.2.1/docs/source/background/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/background/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/background/why-cset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/background/why-workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.970437 CSET-24.2.1/docs/source/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/code-review.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/git.rst
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20084 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/release_page.png
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/releases.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/contributing/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.970437 CSET-24.2.1/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/getting-started/create-first-recipe.rst
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/getting-started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/getting-started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/getting-started/recipe-graph-details.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/getting-started/recipe-graph.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/getting-started/run-recipe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/getting-started/visualise-recipe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.970437 CSET-24.2.1/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/reference/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/reference/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/reference/internal.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/reference/operators.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/reference/recipe-format.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/reference/recipe-graph.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.970437 CSET-24.2.1/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/usage/add-diagnostic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/usage/operator-recipes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-04 09:18:38.000000 CSET-24.2.1/docs/source/usage/workflow-installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-04 09:18:38.000000 CSET-24.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.970437 CSET-24.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-04 09:18:38.000000 CSET-24.2.1/requirements/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.974437 CSET-24.2.1/requirements/locks/
--rw-r--r--   0 runner    (1001) docker     (127)    24543 2024-03-04 09:18:38.000000 CSET-24.2.1/requirements/locks/py310-lock-linux-64.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24419 2024-03-04 09:18:38.000000 CSET-24.2.1/requirements/locks/py311-lock-linux-64.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24419 2024-03-04 09:18:38.000000 CSET-24.2.1/requirements/locks/py312-lock-linux-64.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24761 2024-03-04 09:18:38.000000 CSET-24.2.1/requirements/locks/py39-lock-linux-64.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 09:19:06.994437 CSET-24.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.966437 CSET-24.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.974437 CSET-24.2.1/src/CSET/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.974437 CSET-24.2.1/src/CSET/operators/
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/convection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/operators/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.978437 CSET-24.2.1/src/CSET/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/recipes/CAPE_ratio_plot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/recipes/aggregate_precipitation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/recipes/extract_instant_air_temp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/recipes/initial_time-step_surface_air_temperature_ensemble_postage_stamp_plot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/recipes/mean_surface_air_temperature_spatial_plot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-04 09:18:38.000000 CSET-24.2.1/src/CSET/recipes/meaned_model_level_air_temperature_spatial_plot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.994437 CSET-24.2.1/src/CSET.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-04 09:19:06.000000 CSET-24.2.1/src/CSET.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-04 09:19:06.000000 CSET-24.2.1/src/CSET.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 09:19:06.000000 CSET-24.2.1/src/CSET.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-04 09:19:06.000000 CSET-24.2.1/src/CSET.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-04 09:19:06.000000 CSET-24.2.1/src/CSET.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-04 09:19:06.000000 CSET-24.2.1/src/CSET.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.978437 CSET-24.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.978437 CSET-24.2.1/tests/operators/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_convection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/operators/test_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.982437 CSET-24.2.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)    29314 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/air_temp.nc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:19:06.990437 CSET-24.2.1/tests/test_data/convection/
--rw-r--r--   0 runner    (1001) docker     (127)  2148486 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/convection/ECFlagB.nc
--rw-r--r--   0 runner    (1001) docker     (127)  2148486 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/convection/ECFlagB_2.nc
--rw-r--r--   0 runner    (1001) docker     (127)  1760308 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/convection/MUCAPE.nc
--rw-r--r--   0 runner    (1001) docker     (127)  1730888 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/convection/MUCIN.nc
--rw-r--r--   0 runner    (1001) docker     (127)  1071846 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/convection/SBCAPE.nc
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/ensemble_air_temp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/exeter_em01.nc
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/exeter_em02.nc
--rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/exeter_ensemble_single_file.nc
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/noop_recipe.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/plot_instant_air_temp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_data/plot_instant_air_temp_collapse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-04 09:18:38.000000 CSET-24.2.1/tests/test_run_recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.482542 cset-24.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-04-19 08:36:12.000000 cset-24.4.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 08:36:12.000000 cset-24.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-19 08:36:34.482542 cset-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-19 08:36:12.000000 cset-24.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.458542 cset-24.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 08:36:12.000000 cset-24.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.458542 cset-24.4.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.458542 cset-24.4.1/docs/source/background/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/background/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/background/why-cset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/background/why-workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.458542 cset-24.4.1/docs/source/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/code-review.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29985 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/failing_pr_check.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/git.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/open_pr_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20084 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/release_page.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/contributing/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.458542 cset-24.4.1/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/getting-started/create-first-recipe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/getting-started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/getting-started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/getting-started/recipe-graph-details.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/getting-started/recipe-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/getting-started/run-recipe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/getting-started/visualise-recipe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.462542 cset-24.4.1/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/reference/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/reference/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/reference/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/reference/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/reference/recipe-format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/reference/recipe-graph.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.462542 cset-24.4.1/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/usage/add-diagnostic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/usage/common-errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/usage/operator-recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   108375 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/usage/rose-edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-19 08:36:12.000000 cset-24.4.1/docs/source/usage/workflow-installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-19 08:36:12.000000 cset-24.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.462542 cset-24.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 08:36:12.000000 cset-24.4.1/requirements/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.462542 cset-24.4.1/requirements/locks/
+-rw-r--r--   0 runner    (1001) docker     (127)    25144 2024-04-19 08:36:12.000000 cset-24.4.1/requirements/locks/py310-lock-linux-64.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-04-19 08:36:12.000000 cset-24.4.1/requirements/locks/py311-lock-linux-64.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-04-19 08:36:12.000000 cset-24.4.1/requirements/locks/py312-lock-linux-64.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25362 2024-04-19 08:36:12.000000 cset-24.4.1/requirements/locks/py39-lock-linux-64.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:36:34.482542 cset-24.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.454542 cset-24.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.462542 cset-24.4.1/src/CSET/
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.466542 cset-24.4.1/src/CSET/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/_plot_page_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/convection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/operators/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.466542 cset-24.4.1/src/CSET/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/CAPE_ratio_plot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/aggregate_precipitation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/extract_instant_air_temp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/generic_plevel_spatial_plot_sequence.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/generic_surface_domain_mean_time_series.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/generic_surface_spatial_plot_sequence.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/initial_time-step_surface_air_temperature_ensemble_postage_stamp_plot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/lfric_generic_surface_domain_mean_time_series.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/lfric_generic_surface_spatial_plot_sequence.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/mean_surface_air_temperature_spatial_plot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/meaned_model_level_air_temperature_spatial_plot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/stash_surface_domain_mean_time_series.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/stash_surface_spatial_plot_sequence.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-19 08:36:12.000000 cset-24.4.1/src/CSET/recipes/surface_air_temperature_spatial_plot_time_sequence.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.482542 cset-24.4.1/src/CSET.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-19 08:36:34.000000 cset-24.4.1/src/CSET.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-19 08:36:34.000000 cset-24.4.1/src/CSET.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:36:34.000000 cset-24.4.1/src/CSET.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 08:36:34.000000 cset-24.4.1/src/CSET.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 08:36:34.000000 cset-24.4.1/src/CSET.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 08:36:34.000000 cset-24.4.1/src/CSET.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.470542 cset-24.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 08:36:12.000000 cset-24.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-19 08:36:12.000000 cset-24.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.470542 cset-24.4.1/tests/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_convection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-19 08:36:12.000000 cset-24.4.1/tests/operators/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.470542 cset-24.4.1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    29314 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/air_temp.nc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.482542 cset-24.4.1/tests/test_data/convection/
+-rw-r--r--   0 runner    (1001) docker     (127)  2148486 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/convection/ECFlagB.nc
+-rw-r--r--   0 runner    (1001) docker     (127)  2148486 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/convection/ECFlagB_2.nc
+-rw-r--r--   0 runner    (1001) docker     (127)  1760308 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/convection/MUCAPE.nc
+-rw-r--r--   0 runner    (1001) docker     (127)  1730888 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/convection/MUCIN.nc
+-rw-r--r--   0 runner    (1001) docker     (127)  1071846 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/convection/SBCAPE.nc
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/ensemble_air_temp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/exeter_em01.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/exeter_em02.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/exeter_ensemble_single_file.nc
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/noop_recipe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/plot_instant_air_temp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/plot_instant_air_temp_collapse.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:34.482542 cset-24.4.1/tests/test_data/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)    11525 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/regrid/out_rectilinearGeogCS_0p5deg.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   329473 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/regrid/regrid_rectilinearGeogCS.nc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_data/template_file.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-19 08:36:12.000000 cset-24.4.1/tests/test_run_recipes.py
```

### Comparing `CSET-24.2.1/LICENCE` & `cset-24.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/PKG-INFO` & `cset-24.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSET
-Version: 24.2.1
+Version: 24.4.1
 Summary: Toolkit for evaluation and investigation of numerical models for weather and climate applications.
 Author: Met Office, NIWA
 License: Apache-2.0
 Project-URL: Documentation, https://metoffice.github.io/CSET
 Project-URL: Source, https://github.com/MetOffice/CSET
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -53,15 +53,15 @@
 In addition to reading the working practices, the key
 recommendation is early communication. Open an [issue on
 Github](https://github.com/MetOffice/CSET/issues) with your proposed change or
 addition in the design phase, and then others can provide guidance early.
 
 ## Licence
 
-Copyright © 2022-2023 Met Office and contributors.
+Copyright © 2022-2024 Met Office and contributors.
 
 Licensed under the [Apache License, Version 2.0](LICENCE) (the "License"); You
 may obtain a copy of the License at
 
 <http://www.apache.org/licenses/LICENSE-2.0>
 
 Unless required by applicable law or agreed to in writing, software distributed
```

### Comparing `CSET-24.2.1/README.md` & `cset-24.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 In addition to reading the working practices, the key
 recommendation is early communication. Open an [issue on
 Github](https://github.com/MetOffice/CSET/issues) with your proposed change or
 addition in the design phase, and then others can provide guidance early.
 
 ## Licence
 
-Copyright © 2022-2023 Met Office and contributors.
+Copyright © 2022-2024 Met Office and contributors.
 
 Licensed under the [Apache License, Version 2.0](LICENCE) (the "License"); You
 may obtain a copy of the License at
 
 <http://www.apache.org/licenses/LICENSE-2.0>
 
 Unless required by applicable law or agreed to in writing, software distributed
```

### Comparing `CSET-24.2.1/docs/Makefile` & `cset-24.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/background/why-cset.rst` & `cset-24.4.1/docs/source/background/why-cset.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/background/why-workflow.rst` & `cset-24.4.1/docs/source/background/why-workflow.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/conf.py` & `cset-24.4.1/docs/source/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,29 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
     "sphinx.ext.doctest",
+    "sphinx.ext.extlinks",
 ]
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "furo"
 
 # -- LaTeX output configuration ----------------------------------------------
 # https://www.sphinx-doc.org/en/master/latex.html
 
 latex_engine = "xelatex"
 latex_elements = {"papersize": "a4paper"}
 latex_show_urls = "footnote"
+
+# -- Extlinks configuration --------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/extensions/extlinks.html
+
+extlinks = {
+    "issue": ("https://github.com/MetOffice/CSET/issues/%s", "Issue #%s"),
+    "pr": ("https://github.com/MetOffice/CSET/pull/%s", "PR #%s"),
+}
```

### Comparing `CSET-24.2.1/docs/source/contributing/code-review.rst` & `cset-24.4.1/docs/source/contributing/code-review.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/contributing/documentation.rst` & `cset-24.4.1/docs/source/contributing/documentation.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/contributing/getting-started.rst` & `cset-24.4.1/docs/source/contributing/getting-started.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Before you Contribute
-=====================
+Set-up code and tooling
+=======================
 
 Contributing
 ------------
 
 Contributions are readily welcome! In addition to reading the `working
 practices`_, the key recommendation is early communication. Open an issue on
 Github with your proposed change or addition in the design phase, and then
```

### Comparing `CSET-24.2.1/docs/source/contributing/git.rst` & `cset-24.4.1/docs/source/contributing/git.rst`

 * *Files 3% similar despite different names*

```diff
@@ -134,19 +134,33 @@
 ``git restore --staged <file>`` command. Having this index makes it easier
 to split a change into multiple commits if desired.
 
 **Commits**: The core unit of git. Each commit describes the state of the
 working tree at the point where it is committed. Contains information like a
 commit message, the date when the commit was made, and author information. It
 also contains a reference to any parent commits, which defines the repository
-history.
+history. Create a new commit with the ``git commit`` command. When fixing
+an issue include the issue number in the commit message body, e.g.:
+
+.. code-block:: text
+
+    Stop foo doing bar
+
+    Description of why this change was made.
+    Fixes #123
 
 **Branch**: A special reference to a particular commit. If a new child commit is
 created the reference moves to that new commit.
 
+* List your local branches with the command ``git branch``.
+* Create a new branch with ``git switch -c <branch-name>``.
+* Switch between local branches with the command ``git switch <branch-name>``. You
+  will need to commit your changes before switching.
+
+
 **Tag**: A special reference to a a particular commit. Unlike a branch it doesn't
 move.
 
 git rebase
 ~~~~~~~~~~
 
 A rebase changes the base commit from which your changes are made. The rebase
```

### Comparing `CSET-24.2.1/docs/source/contributing/release_page.png` & `cset-24.4.1/docs/source/contributing/release_page.png`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/contributing/releases.rst` & `cset-24.4.1/docs/source/contributing/releases.rst`

 * *Files 18% similar despite different names*

```diff
@@ -23,31 +23,48 @@
 follow the ``YY.MM.patch`` format, so the first release in February 2024 would
 be ``v24.2.0``. Patch releases should only contain bugfixes, and may be released
 for older versions, (e.g: ``v24.2.5`` could be released after February). We
 should target one feature release a month, so things are not stuck on the trunk
 for too long, though quiet periods (e.g: Summer, Christmas) may see a release
 missed.
 
-Backwards Compatibility Policy
-------------------------------
+Deprecation policy
+------------------
 
-As soon as we have users for CSET maintaining a certain level of backwards
-compatibility becomes important, as they will want their use of CSET to continue
-to work in future. As such it is useful to define a backwards compatibility
-policy that sets expectations about the way backwards incompatible (AKA
-"breaking") changes are made.
-
-Some things to consider:
-
-* How quickly backwards incompatible changes can be made.
-* How long deprecation periods should be for different sizes of change.
-* How the changes will be communicated with users.
-* Guidance on avoiding making backwards incompatible changes where possible.
+Any change to CSET that removes or significantly alters user-visible behavior
+that is described in the CSET documentation will be deprecated for a minimum of
+6 months before the change occurs.
+
+Certain changes may be fast tracked and have a deprecation period of 3 months.
+This requires at least two members of the CSET team to be in favor of doing so,
+and no maintainers opposing.
+
+Deprecation will take the form of a warning being issued by CSET when the
+feature is used. Longer deprecation periods, or deprecation warnings for
+behavior changes that would not normally be covered by this policy, are also
+possible depending on circumstances, but this is at the discretion of the
+maintainers.
+
+Note that the documentation is the sole reference for what counts as agreed
+behavior. If something isn’t explicitly mentioned in the documentation, it can
+be changed without warning, or any deprecation period, in a release. However, we
+are aware that the documentation isn’t always complete - PRs that document
+existing behavior with the intention of covering that behavior with the above
+deprecation process are always acceptable, and will be considered on their
+merits.
+
+Python Support Policy
+---------------------
 
-Making a Release
+CSET follows `NEP 29`_, supporting all python versions released in the prior 42
+months.
+
+.. _NEP 29: https://numpy.org/neps/nep-0029-deprecation_policy.html
+
+Making a release
 ----------------
 
 Making a release is mostly automated. With the use of `setuptools_scm`_ you
 don't even need to increment a version number. To create a release you should
 use the GitHub web UI. Go to the `Releases`_ page, and press `Draft a new
 release`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CSET-24.2.1/docs/source/contributing/testing.rst` & `cset-24.4.1/docs/source/contributing/testing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -92,17 +92,16 @@
 .. _This article: https://jml.io/pages/test-docstrings.html
 
 Pre-commit Checks
 -----------------
 
 Some very quick checks to catch any very obvious mistakes. They are usually
 setup to run automatically when you make a commit. The checks are installed from
-.pre-commit-config.yaml, and currently involve blacking python code, linting
-with flake8, and checking all files are well formed (no trailing whitespace,
-etc.).
+.pre-commit-config.yaml, and currently involve formatting python code, linting,
+and checking all files are well formed (no trailing whitespace, etc.).
 
 .. code-block:: bash
 
     # Install the pre-commit helper.
     pip install pre-commit
     # Install the checks into git
     pre-commit install
```

### Comparing `CSET-24.2.1/docs/source/getting-started/create-first-recipe.rst` & `cset-24.4.1/docs/source/getting-started/create-first-recipe.rst`

 * *Files 7% similar despite different names*

```diff
@@ -70,32 +70,34 @@
       Extracts and plots the 1.5m air temperature from a file. The temperature
       is averaged across the time coordinate.
 
 
 Recipe Steps
 ------------
 
-Just as in baking you would follow a recipe step-by-step, so does CSET. The
-steps of the recipe are all under the ``steps`` key. Each block prefixed with a
-``-`` (which makes a list in YAML) is a step, and they are run in order from top
-to bottom.
+When baking you follow a recipe step-by-step, CSET does the same with its
+recipes. The steps of the recipe are contained within one of two keys. The
+``parallel`` key for independent tasks that process the raw data, and the
+``collate`` key for sequential tasks that bring together the processed data into
+the final output. Each block prefixed with a ``-`` (which makes a list in YAML)
+is an individual step, and they are run in order from top to bottom.
 
 Each step has an ``operator`` key, which specifies which operator to use. A
 `complete list of operators is in the documentation`_, but for this tutorial we
 will describe them here.
 
 .. _complete list of operators is in the documentation: https://metoffice.github.io/CSET/reference/operators
 
 The first step reads in the model data. This is done with the
 ``read.read_cubes`` operator. The first step is special, and receives the path
 to the input data as its implicit input.
 
 .. code-block:: yaml
 
-    steps:
+    parallel:
       - operator: read.read_cubes
 
 Once we have read the data, we need to filter them down to the data we require
 for our computations. ``filter.filter_cubes`` is the operator for that. It also
 ensures that the CubeList returned by ``read.read_cubes`` is turned into a Cube.
 
 .. code-block:: yaml
@@ -151,15 +153,15 @@
 .. code-block:: yaml
 
     title: Mean Surface Air Temperature Spatial Plot
     description: |
       Extracts and plots the 1.5m air temperature from a file. The temperature
       is averaged across the time coordinate.
 
-    steps:
+    parallel:
       - operator: read.read_cubes
 
       - operator: filters.filter_cubes
         constraint:
           operator: constraints.combine_constraints
           stash_constraint:
             operator: constraints.generate_stash_constraint
```

### Comparing `CSET-24.2.1/docs/source/getting-started/installation.rst` & `cset-24.4.1/docs/source/getting-started/installation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 a simple command.
 
 .. code-block:: bash
 
     cset --version
 
 This command should output the installed version of CSET. This will look
-something like ``CSET v0.4.0``.
+something like ``CSET vX.Y.Z``.
 
 You now have CSET installed, so try another tutorial.
 
 .. note::
 
     This page details installing a released version of CSET. If you instead want
     to run a development version that has yet to be released, see
```

### Comparing `CSET-24.2.1/docs/source/getting-started/recipe-graph-details.svg` & `cset-24.4.1/docs/source/getting-started/recipe-graph-details.svg`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/getting-started/recipe-graph.svg` & `cset-24.4.1/docs/source/getting-started/recipe-graph.svg`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/getting-started/run-recipe.rst` & `cset-24.4.1/docs/source/getting-started/run-recipe.rst`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 temperature. There is a pre-existing recipe for this that can be retrieved with
 the CSET cookbook command.
 
 Try the following:
 
 .. code-block:: bash
 
-    cset cookbook -o recipes
+    cset cookbook -o recipes mean_surface_air_temperature_spatial_plot.yaml
 
-This will write out a recipes folder containing recipe ``.yaml`` files to your
+This will write out a recipes folder containing recipe ``.yaml`` file to your
 current directory. We will use the
 ``mean_surface_air_temperature_spatial_plot.yaml`` recipe.
 
 Now you need to find some data to process. You can `download an example file
 here`_, or with the following command.
 
 .. code-block:: bash
@@ -36,13 +36,13 @@
 .. code-block:: bash
 
     cset bake -i air_temp.nc -o output/ -r recipes/mean-air-temp-spacial-plot.yaml
 
 This will run the recipe and leave its output in the specified output directory.
 
 The most interesting output will be the plot, which you can look at with
-``xdg-open output/plot.svg``.
+``xdg-open output/plot.png``.
 
 You've now successfully run CSET with a pre-existing recipe. In the next
 tutorial we will see what is going on inside.
 
 .. _download an example file here: https://github.com/MetOffice/CSET/raw/main/tests/test_data/air_temp.nc
```

### Comparing `CSET-24.2.1/docs/source/getting-started/visualise-recipe.rst` & `cset-24.4.1/docs/source/getting-started/visualise-recipe.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/index.rst` & `cset-24.4.1/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
    self
    getting-started/index
    usage/index
    reference/index
    background/index
    contributing/index
+   changelog
    GitHub <https://github.com/MetOffice/CSET>
 
 :abbr:`CSET (Convective and turbulence scale Evaluation and verification Tool)`
 is a toolkit for evaluation, verification and investigation of convective- and
 turbulence-scale numerical models for weather and climate applications, cutting
 across time and space scales.
 
@@ -29,16 +30,18 @@
 tools and flexible evaluation code that can adapt to users needs.
 
 For diagnostic developers it provides a legacy for diagnostics and observations.
 It is build on a modern software stack using python 3 and METplus. Clear
 documentation, working practices, automatic testing, and open access promote
 contributions.
 
-For more information on how to use it and get involved as a developer, see
-:doc:`/background/why-cset`
+For information on how to use CSET, see :doc:`getting-started/index`.
+
+For information on getting involved as a developer, see
+:doc:`contributing/index`.
 
 Use the side bar to the left to access other pages of the documentation.
 
 Useful Links
 ------------
 
 `Source Code`_ | `Issue Tracker`_ | Releases_
@@ -46,11 +49,11 @@
 .. _Source Code: https://github.com/MetOffice/CSET
 .. _Issue Tracker: https://github.com/MetOffice/CSET/issues
 .. _Releases: https://github.com/MetOffice/CSET/releases
 
 Licence
 -------
 
-Copyright © 2022-2023 Met Office and contributors. CSET is distributed under the
+Copyright © 2022-2024 Met Office and contributors. CSET is distributed under the
 `Apache 2.0 License`_, in the hope that it will be useful.
 
 .. _Apache 2.0 License: https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `CSET-24.2.1/docs/source/reference/cli.rst` & `cset-24.4.1/docs/source/reference/cli.rst`

 * *Files 23% similar despite different names*

```diff
@@ -9,44 +9,46 @@
 Used to run a recipe on some data. The recipe, input directory, and output
 directory must be provided. Additional help is available with the ``--help``
 option. The recipe format is described on the :doc:`/usage/operator-recipes`
 page.
 
 .. code-block:: text
 
-    usage: cset bake [-h] -i INPUT_DIR -o OUTPUT_DIR -r RECIPE
+    usage: cset bake [-h] [-i INPUT_DIR] -o OUTPUT_DIR -r RECIPE [--pre-only | --post-only]
 
     options:
-    -h, --help            show this help message and exit
+    -h, --help              show this help message and exit
     -i INPUT_DIR, --input-dir INPUT_DIR
                             directory containing input data
     -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                             directory to write output into
     -r RECIPE, --recipe RECIPE
                             recipe file to read
+    --parallel-only         only run parallel steps
+    --collate-only          only run collation steps
 
 .. _cset-cookbook-command:
 
 cset cookbook
 ~~~~~~~~~~~~~
 
-Saves the included recipe files to a local directory. This allows access to
-pre-created recipes for many common tasks. See :doc:`/usage/operator-recipes`
-for descriptions of available recipes.
+Saves an included recipe file to a local directory. This allows access to
+pre-created recipes for many common tasks. See :doc:`/usage/operator-recipes`,
+or use ``--details`` for descriptions of available recipes.
 
 .. code-block:: text
 
-    usage: cset cookbook [-h] [-l] [-o OUTPUT_DIR] [recipe]
+    usage: cset cookbook [-h] [-d] [-o OUTPUT_DIR] [recipe]
 
     positional arguments:
-    recipe                recipe to output or detail. Omit for all.
+    recipe                recipe to output or detail
 
     options:
     -h, --help            show this help message and exit
-    -l, --list            list available recipes. Supplied recipes are detailed.
+    -d, --details         list available recipes. Supplied recipes are detailed.
     -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                             directory to save recipes. If omitted uses $PWD
 
 .. _cset-graph-command:
 
 cset graph
 ~~~~~~~~~~
```

### Comparing `CSET-24.2.1/docs/source/reference/glossary.rst` & `cset-24.4.1/docs/source/reference/glossary.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/reference/internal.rst` & `cset-24.4.1/docs/source/reference/internal.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/reference/operators.rst` & `cset-24.4.1/docs/source/reference/operators.rst`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 
 CSET.operators.read
 -------------------
 
 .. automodule:: CSET.operators.read
    :members:
 
+CSET.operators.regrid
+---------------------
+
+.. automodule:: CSET.operators.regrid
+   :members:
+
 CSET.operators.write
 --------------------
 
 .. automodule:: CSET.operators.write
    :members:
 
 Convection Operators
```

### Comparing `CSET-24.2.1/docs/source/reference/recipe-graph.svg` & `cset-24.4.1/docs/source/reference/recipe-graph.svg`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/usage/add-diagnostic.rst` & `cset-24.4.1/docs/source/usage/add-diagnostic.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/docs/source/usage/operator-recipes.rst` & `cset-24.4.1/docs/source/usage/operator-recipes.rst`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/pyproject.toml` & `cset-24.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
-filterwarnings = ['ignore::DeprecationWarning:pytest']
+filterwarnings = [
+    # https://github.com/dateutil/dateutil/issues/1314
+    "ignore::DeprecationWarning:dateutil",
+    "ignore:numpy.ndarray size changed:RuntimeWarning",
+]
 minversion = "7"
 pythonpath = ["src"]
 testpaths = ["tests"]
 
 [tool.coverage.run]
 branch = true
 relative_files = true
```

### Comparing `CSET-24.2.1/requirements/locks/py310-lock-linux-64.txt` & `cset-24.4.1/requirements/locks/py310-lock-linux-64.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,85 +14,90 @@
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.27.0-hd590300_0.conda#f6afff0e9ee08d2f1b897881a4f38cdb
+https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/geos-3.12.1-h59595ed_0.conda#8c0f4f71f5a59ceb0c6fa9f51501066d
-https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
-https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.1-h0b41bf4_3.conda#96f3b11872ef6fad973eac856cd2624f
-https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
+https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
+https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.2-hd590300_0.conda#3bf7b9fd5a7136126e0234db4b87c8b6
+https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
-https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.2-h59595ed_1.conda#127b0be54c1c90760d7fe02ea7a56426
+https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.3-h59595ed_0.conda#5e97e271911b8b2001a8b71860c32faa
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
-https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.19-hd590300_0.conda#1635570038840ee3f9c71d22aa5b8b6d
+https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
-https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libmo_unpack-3.1.2-hf484d3e_1001.tar.bz2#95f32a6a5a666d33886ca5627239f03d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_0.conda#30de3fd9b3b602f7473f30e684eeea8c
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-h59595ed_2.conda#7dbaa197d7ba6032caf7ae7f32c1efa0
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_0.conda#51a753e64a3027bd7e23a189b1f6e91e
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.43.2-h59595ed_0.conda#71004cbf7924e19c02746ccde9fd7123
 https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
-https://conda.anaconda.org/conda-forge/linux-64/snappy-1.1.10-h9fff704_0.conda#e6d228cd0bb74a51dd18f5bfce0b4115
+https://conda.anaconda.org/conda-forge/linux-64/snappy-1.2.0-hdb0a2a9_1.conda#843bbb8ace1d64ac50d64639ff38b014
 https://conda.anaconda.org/conda-forge/linux-64/xorg-kbproto-1.0.7-h7f98852_1002.tar.bz2#4b230e8381279d76131116660f5a241a
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.1.1-hd590300_0.conda#b462a33c0be1421532f28bfe8f4a7514
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda#2c80dc38fface310c9bd81b17037fee5
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
 https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2#06feff3d2634e3097ce2fe681474b534
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xxhash-0.8.2-hd590300_0.conda#f08fb5c89edfc4aadee1c81d4cfb1fa1
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.6.2-h59595ed_0.conda#53fb86322bdb89496d7579fe3f02fd61
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h2a13503_7.conda#bd77f8da987968ec3927990495dc22e4
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.1-h2797004_0.conda#fc4ccadfbf6d4784de88c41704792562
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libudunits2-2.2.28-h40f5838_3.conda#4bdace082e911a3e1f1f0b721bed5b56
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.5-h232c23b_0.conda#c442ebfda7a475f5e78f1c8e45f1e919
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
-https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.42-hcad00b1_0.conda#679c8961826aa4b50653bce17ee52abe
+https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
-https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-h0f2a231_0.conda#009521b7ed97cca25f8f997f9e745976
+https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
+https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.78.4-h783c2da_0.conda#d86baf8740d1a906b9716f2a0bac2f2d
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.26-pthreads_h413a1c8_0.conda#760ae35415f5ba8b15d09df5afe8b23a
-https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-ha9c0a0a_2.conda#55ed21669b2015f77c180feb1dd41930
-https://conda.anaconda.org/conda-forge/linux-64/python-3.10.13-hd12c33a_1_cpython.conda#ed38140af93f81319ebc472fbcf16cca
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.1-h2c6b66d_0.conda#93acf31b379acebada263b9bce3dc6ed
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
+https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
+https://conda.anaconda.org/conda-forge/linux-64/python-3.10.14-hd12c33a_0_cpython.conda#2b4ba962994e8bd4be9ff5b64b75aff2
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.2-h2c6b66d_0.conda#1423efca06ed343c1da0fc429bae0779
 https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-h40f5838_3.conda#6bb8deb138f87c9d48320ac21b87e7a1
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.7-h8ee46fc_0.conda#49e482d882669206653b095f5206c05b
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda#077b6e8ad6a3ddb741fce2496dd01bec
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/antlr-python-runtime-4.11.1-pyhd8ed1ab_0.tar.bz2#15109c4977d39ad7aa3423f57243e286
 https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.1.0-hd590300_1.conda#f27a24d46e3ea7b70a1f98e50c62508f
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py310hc6cd4ac_1.conda#1f95722c94f00b69af69a066c7433714
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
@@ -100,114 +105,114 @@
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-3.0.0-pyhd8ed1ab_0.conda#753d29fe41bb881e4b9c004f0abf973f
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py310hff52083_3.conda#c159dcd29bbd80b187b1c5d5f73cc971
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.1-pyhd8ed1ab_0.conda#0c1729b74a8152fde6a38ba0a2ab9f45
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.2.0-pyhca7485f_0.conda#fad86b90138cf5d82c6f5a2ed6e683d9
-https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_4.conda#252a696860674caf7a855e16f680d63a
+https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.3.1-pyhca7485f_0.conda#b7f0662ef2c9d4404f0af9eef5ed2fde
+https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_5.conda#8fdb82e5d9694dd8e9ed9ac8fdf48a26
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py310hd41b1e2_1.conda#b8d67603d43b23ce7e988a5d81a7ab79
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-21_linux64_openblas.conda#0ac9f44fc096772b0aa092119b00c3ca
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.5.0-hca28451_0.conda#7144d5a828e2cae218e0e3c98d8a0aeb
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.3.2-h658648e_1.conda#0ebb65e8d86843865796c7c95a941f34
 https://conda.anaconda.org/conda-forge/noarch/locket-1.0.0-pyhd8ed1ab_0.tar.bz2#91e27ef3d05cc772ce627e51cff111c4
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py310h2372a71_0.conda#f6703fa0214a00bf49d1bef6dc7672d0
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
-https://conda.anaconda.org/conda-forge/noarch/packaging-23.2-pyhd8ed1ab_0.conda#79002079284aa895f883c6b7f3f88fd6
+https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
 https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.1-pyhd8ed1ab_0.conda#176f7d56f0cfe9008bdf1bccd7de02fb
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pyshp-2.3.1-pyhd8ed1ab_0.tar.bz2#92a889dc236a5197612bc85bee6d7174
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/linux-64/python-xxhash-3.4.1-py310h2372a71_0.conda#b631b889b0b4bc2fca7b8b977ca484b2
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py310h2372a71_1.conda#bb010e368de4940771368bc3dc4c63e7
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py310h2372a71_0.conda#dcf6d2535586c77b31425ed835610c54
-https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.0-py310h3d77a66_0.conda#f573f0d35a662801b10911ffb12f6e49
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.1.1-pyhd8ed1ab_0.conda#576de899521b7d43674ba3ef6eae9142
+https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py310h3d77a66_0.conda#55b40e33fae0b983b48d2f7aff8a8978
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.10.0-pyha770c72_0.conda#16ae769069b380646c47142d719ef466
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py310h2372a71_0.conda#72637c58d36d9475fda24700c9796f19
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.42.0-pyhd8ed1ab_0.conda#1cdea58981c5cbc17b51973bcaddcea7
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py310h2fee648_0.conda#45846a970e71ac98fd327da5d40a0a2c
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.3-py310h2372a71_1.conda#d9c1e9a3a198a7d4454261fbc220b89b
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.49.0-py310h2372a71_0.conda#e61ae80fde506b70a88e5e06376d2068
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.4-py310h2372a71_0.conda#2d948842110ae68e4f2e7738f92bf7e1
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py310h2372a71_0.conda#1a4773624145c15b92820fe6c87c5fcd
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.0.1-pyha770c72_0.conda#746623a787e06191d80a2133e5daff17
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/isodate-0.6.1-pyhd8ed1ab_0.tar.bz2#4a62c93c1b5c0b920508ae3fd285eaf5
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-21_linux64_openblas.conda#4a3816d06451c4946e2db26b86472cb6
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h119a65a_9.conda#cfebc557e54905dadc355c0e9f003004
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-21_linux64_openblas.conda#1a42f305615c3867684e049e85927531
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda#2a75b296096adabbabadd5e9782e5fcc
 https://conda.anaconda.org/conda-forge/noarch/partd-1.4.1-pyhd8ed1ab_0.conda#acf4b7c0bcd5fa3b0e05801c4d2accd6
-https://conda.anaconda.org/conda-forge/linux-64/pillow-10.2.0-py310h01dd4db_0.conda#9ec32d0d90f7670eb29bbba18299cf29
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py310hf73ecf8_0.conda#1de56cf017dfd02aa84093206a0141a8
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/linux-64/proj-9.3.1-h1d62c97_0.conda#44ec51d0857d9be26158bb85caa74fdb
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.0.2-pyhd8ed1ab_0.conda#40bd3ef942b9642a3eb20b0bbf92469b
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py310h2372a71_0.conda#50b7d9b39099cdbabf65bf27df73a793
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.10.0-hd8ed1ab_0.conda#091683b9150d2ebaa62fd7e2c86433da
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.0.1-hd8ed1ab_0.conda#4a2f43a20fa404b998859c6a470ba316
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py310hb13e2d6_0.conda#6593de64c935768b6bad3e19b3e978be
 https://conda.anaconda.org/conda-forge/linux-64/pyproj-3.6.1-py310hd5c30f3_5.conda#dc2ee770a2299307f3c127af79160d25
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda#06eb685a3a0b146347a58dda979485da
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda#c54c0107057d67ddf077751339ec2c63
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_0.conda#3b8ef3a2d80f3d89d0ae7e3c975e6c57
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_1.conda#a1986ad21c766ff22f7bae93f0641020
 https://conda.anaconda.org/conda-forge/noarch/tox-3.27.1-pyhd8ed1ab_0.tar.bz2#62b743e1030b17163c70654601afb60d
 https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py310hd41b1e2_4.conda#35e87277fba9944b8a975113538bb5df
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py310h1f7b6fc_0.conda#31beda75384647959d5792a1a7dc571a
-https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.0-py310hd41b1e2_0.conda#85d2aaa7af046528d339da1e813c3a9f
-https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.2.1-pyhd8ed1ab_0.conda#72ac49d50b7af2159a8f4128bc1f856d
+https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py310hd41b1e2_0.conda#60ee50b1968f802f2a487ba36d4cce0d
+https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.1-pyhd8ed1ab_0.conda#52387f00fee8dcd5cf75f8886025293f
 https://conda.anaconda.org/conda-forge/noarch/identify-2.5.35-pyhd8ed1ab_0.conda#9472bfd206a2b7bb8143835e37667054
 https://conda.anaconda.org/conda-forge/linux-64/mo_pack-0.3.0-py310h2372a71_1.conda#dfcf64f67961eb9686676f96fdb4b4d1
-https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.0-ha41ecd1_0.conda#62f61784f6feddf19ffcba71d5f7dbbd
-https://conda.anaconda.org/conda-forge/linux-64/scipy-1.12.0-py310hb13e2d6_2.conda#cd3baec470071490bc5ab05da64c52b5
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_0.conda#2a6b1e6a1a0c301e4bfff82d7672437a
+https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.2-ha41ecd1_0.conda#a658eeabf188c3040da36b0763de2bfd
+https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py310hb13e2d6_0.conda#512cfc0369e247e3993a76030671cce0
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_1.conda#b065535ca8ca824703ae5537087e2206
 https://conda.anaconda.org/conda-forge/linux-64/shapely-2.0.3-py310hc3e127f_0.conda#fbc825d13cbcb2d5d3fbba22c83fd203
 https://conda.anaconda.org/conda-forge/noarch/tox-conda-0.9.2-pyhd8ed1ab_0.tar.bz2#8494c2ad4bef7bfe2e2d8603b4c2a185
 https://conda.anaconda.org/conda-forge/linux-64/cf-units-3.2.0-py310h1f7b6fc_4.conda#0ca55ca20891d393846695354b32ebc5
-https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h7f000aa_3.conda#0abfa7f9241a0f4fd732bc15773cfb0c
-https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.56.3-he3f83f7_1.conda#03bd1ddcc942867a19528877143b9852
-https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.3-py310h62c0568_0.conda#4a7296c0273eb01dfbed728dd6a6725a
+https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h280cfa0_4.conda#410f86e58e880dcc7b0e910a8e89c05c
+https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hce6bd6c_0.conda#0891de8980ee29828542dbf9578838b9
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py310h62c0568_0.conda#bdfa3aee52579c6b3dde12f52e266ef2
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py310hba70d50_100.conda#e19392760c7e4da3b9cb0ee5bf61bc4b
-https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.6.2-pyha770c72_0.conda#61534ee57ffdf26d7b1b514d33daccc4
-https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.22.0-py310hcc13569_1.conda#31ef447724fb19066a9d00a660dab1bd
+https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.0-pyha770c72_0.conda#846ba0877cda9c4f11e13720cacd1968
+https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.23.0-py310hcc13569_0.conda#89a13de526ea3008341e3a2aeab4da7e
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-9.0.0-h78e8752_1.conda#a3f4cd4a512ec5db35ffbf25ba11f537
-https://conda.anaconda.org/conda-forge/noarch/iris-3.8.0-pyha770c72_0.conda#6a92f316e0c5fc52c9d7cff5fa348bc3
+https://conda.anaconda.org/conda-forge/noarch/iris-3.8.1-pyha770c72_0.conda#b08a116ef1607e7e960a4caa902e3a90
 https://conda.anaconda.org/conda-forge/linux-64/pygraphviz-1.12-py310h31db22a_0.conda#4d4f24425228fd801f8d749580261d06
 https://conda.anaconda.org/conda-forge/noarch/sphinx-basic-ng-1.0.0b2-pyhd8ed1ab_1.conda#a631f5c7b7f5045448f966ad71aa2881
 https://conda.anaconda.org/conda-forge/noarch/furo-2024.1.29-pyhd8ed1ab_0.conda#f67437927d5ead424d7dcf1f4d9b7c66
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0.conda#26acae54b06f178681bfb551760f5dd1
```

### Comparing `CSET-24.2.1/requirements/locks/py311-lock-linux-64.txt` & `cset-24.4.1/requirements/locks/py311-lock-linux-64.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,85 +14,90 @@
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.27.0-hd590300_0.conda#f6afff0e9ee08d2f1b897881a4f38cdb
+https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/geos-3.12.1-h59595ed_0.conda#8c0f4f71f5a59ceb0c6fa9f51501066d
-https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
-https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.1-h0b41bf4_3.conda#96f3b11872ef6fad973eac856cd2624f
-https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
+https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
+https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.2-hd590300_0.conda#3bf7b9fd5a7136126e0234db4b87c8b6
+https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
-https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.2-h59595ed_1.conda#127b0be54c1c90760d7fe02ea7a56426
+https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.3-h59595ed_0.conda#5e97e271911b8b2001a8b71860c32faa
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
-https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.19-hd590300_0.conda#1635570038840ee3f9c71d22aa5b8b6d
+https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
-https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libmo_unpack-3.1.2-hf484d3e_1001.tar.bz2#95f32a6a5a666d33886ca5627239f03d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_0.conda#30de3fd9b3b602f7473f30e684eeea8c
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-h59595ed_2.conda#7dbaa197d7ba6032caf7ae7f32c1efa0
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_0.conda#51a753e64a3027bd7e23a189b1f6e91e
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.43.2-h59595ed_0.conda#71004cbf7924e19c02746ccde9fd7123
 https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
-https://conda.anaconda.org/conda-forge/linux-64/snappy-1.1.10-h9fff704_0.conda#e6d228cd0bb74a51dd18f5bfce0b4115
+https://conda.anaconda.org/conda-forge/linux-64/snappy-1.2.0-hdb0a2a9_1.conda#843bbb8ace1d64ac50d64639ff38b014
 https://conda.anaconda.org/conda-forge/linux-64/xorg-kbproto-1.0.7-h7f98852_1002.tar.bz2#4b230e8381279d76131116660f5a241a
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.1.1-hd590300_0.conda#b462a33c0be1421532f28bfe8f4a7514
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda#2c80dc38fface310c9bd81b17037fee5
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
 https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2#06feff3d2634e3097ce2fe681474b534
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xxhash-0.8.2-hd590300_0.conda#f08fb5c89edfc4aadee1c81d4cfb1fa1
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.6.2-h59595ed_0.conda#53fb86322bdb89496d7579fe3f02fd61
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h2a13503_7.conda#bd77f8da987968ec3927990495dc22e4
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.1-h2797004_0.conda#fc4ccadfbf6d4784de88c41704792562
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libudunits2-2.2.28-h40f5838_3.conda#4bdace082e911a3e1f1f0b721bed5b56
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.5-h232c23b_0.conda#c442ebfda7a475f5e78f1c8e45f1e919
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
-https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.42-hcad00b1_0.conda#679c8961826aa4b50653bce17ee52abe
+https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
-https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-h0f2a231_0.conda#009521b7ed97cca25f8f997f9e745976
+https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
+https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.78.4-h783c2da_0.conda#d86baf8740d1a906b9716f2a0bac2f2d
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.26-pthreads_h413a1c8_0.conda#760ae35415f5ba8b15d09df5afe8b23a
-https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-ha9c0a0a_2.conda#55ed21669b2015f77c180feb1dd41930
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
+https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/python-3.11.8-hab00c5b_0_cpython.conda#2fdc314ee058eda0114738a9309d3683
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.1-h2c6b66d_0.conda#93acf31b379acebada263b9bce3dc6ed
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.2-h2c6b66d_0.conda#1423efca06ed343c1da0fc429bae0779
 https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-h40f5838_3.conda#6bb8deb138f87c9d48320ac21b87e7a1
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.7-h8ee46fc_0.conda#49e482d882669206653b095f5206c05b
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda#077b6e8ad6a3ddb741fce2496dd01bec
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/antlr-python-runtime-4.11.1-pyhd8ed1ab_0.tar.bz2#15109c4977d39ad7aa3423f57243e286
 https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.1.0-hd590300_1.conda#f27a24d46e3ea7b70a1f98e50c62508f
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py311hb755f60_1.conda#cce9e7c3f1c307f2a5fb08a2922d6164
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
@@ -100,113 +105,113 @@
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-3.0.0-pyhd8ed1ab_0.conda#753d29fe41bb881e4b9c004f0abf973f
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_3.conda#1c33f55e5cdcc2a2b973c432b5225bfe
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.1-pyhd8ed1ab_0.conda#0c1729b74a8152fde6a38ba0a2ab9f45
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.2.0-pyhca7485f_0.conda#fad86b90138cf5d82c6f5a2ed6e683d9
-https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_4.conda#252a696860674caf7a855e16f680d63a
+https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.3.1-pyhca7485f_0.conda#b7f0662ef2c9d4404f0af9eef5ed2fde
+https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_5.conda#8fdb82e5d9694dd8e9ed9ac8fdf48a26
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py311h9547e67_1.conda#2c65bdf442b0d37aad080c8a4e0d452f
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-21_linux64_openblas.conda#0ac9f44fc096772b0aa092119b00c3ca
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.5.0-hca28451_0.conda#7144d5a828e2cae218e0e3c98d8a0aeb
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.3.2-h658648e_1.conda#0ebb65e8d86843865796c7c95a941f34
 https://conda.anaconda.org/conda-forge/noarch/locket-1.0.0-pyhd8ed1ab_0.tar.bz2#91e27ef3d05cc772ce627e51cff111c4
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py311h459d7ec_0.conda#a322b4185121935c871d201ae00ac143
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
-https://conda.anaconda.org/conda-forge/noarch/packaging-23.2-pyhd8ed1ab_0.conda#79002079284aa895f883c6b7f3f88fd6
+https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
 https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.1-pyhd8ed1ab_0.conda#176f7d56f0cfe9008bdf1bccd7de02fb
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pyshp-2.3.1-pyhd8ed1ab_0.tar.bz2#92a889dc236a5197612bc85bee6d7174
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/linux-64/python-xxhash-3.4.1-py311h459d7ec_0.conda#60b5332b3989fda37884b92c7afd6a91
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py311h459d7ec_1.conda#52719a74ad130de8fb5d047dc91f247a
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py311h459d7ec_0.conda#7865c897d89a39abc0056d89e37bd9e9
-https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.0-py311h7145743_0.conda#33a306351198ac8da1f0d1541d3569f5
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.1.1-pyhd8ed1ab_0.conda#576de899521b7d43674ba3ef6eae9142
+https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py311h7145743_0.conda#68d0518377e72b76d9cd2ec6ebdd4e16
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.10.0-pyha770c72_0.conda#16ae769069b380646c47142d719ef466
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.42.0-pyhd8ed1ab_0.conda#1cdea58981c5cbc17b51973bcaddcea7
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py311hb3a22ac_0.conda#b3469563ac5e808b0cd92810d0697043
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.3-py311h459d7ec_1.conda#4fb7f674bf6839da62317a7c6e725c55
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.49.0-py311h459d7ec_0.conda#d66c9e36ab104f94e35b015c86c2fcb4
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.4-py311h459d7ec_0.conda#1aa22cb84e68841ec206ee066457bdf0
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py311h459d7ec_0.conda#17e1997cc17c571d5ad27bd0159f616c
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.0.1-pyha770c72_0.conda#746623a787e06191d80a2133e5daff17
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/isodate-0.6.1-pyhd8ed1ab_0.tar.bz2#4a62c93c1b5c0b920508ae3fd285eaf5
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-21_linux64_openblas.conda#4a3816d06451c4946e2db26b86472cb6
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h119a65a_9.conda#cfebc557e54905dadc355c0e9f003004
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-21_linux64_openblas.conda#1a42f305615c3867684e049e85927531
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda#2a75b296096adabbabadd5e9782e5fcc
 https://conda.anaconda.org/conda-forge/noarch/partd-1.4.1-pyhd8ed1ab_0.conda#acf4b7c0bcd5fa3b0e05801c4d2accd6
-https://conda.anaconda.org/conda-forge/linux-64/pillow-10.2.0-py311ha6c5da5_0.conda#a5ccd7f2271f28b7d2de0b02b64e3796
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py311h18e6fac_0.conda#6c520a9d36c9d7270988c7a6c360d6d4
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/linux-64/proj-9.3.1-h1d62c97_0.conda#44ec51d0857d9be26158bb85caa74fdb
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.0.2-pyhd8ed1ab_0.conda#40bd3ef942b9642a3eb20b0bbf92469b
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py311h459d7ec_0.conda#4dccc0bc3bb4d6e5c30bccbd053c4f90
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.10.0-hd8ed1ab_0.conda#091683b9150d2ebaa62fd7e2c86433da
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.0.1-hd8ed1ab_0.conda#4a2f43a20fa404b998859c6a470ba316
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py311h64a7726_0.conda#a502d7aad449a1206efb366d6a12c52d
 https://conda.anaconda.org/conda-forge/linux-64/pyproj-3.6.1-py311hca0b8b9_5.conda#cac429fcb9126d5e6f02c8ba61c2a811
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda#06eb685a3a0b146347a58dda979485da
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda#c54c0107057d67ddf077751339ec2c63
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_0.conda#3b8ef3a2d80f3d89d0ae7e3c975e6c57
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_1.conda#a1986ad21c766ff22f7bae93f0641020
 https://conda.anaconda.org/conda-forge/noarch/tox-3.27.1-pyhd8ed1ab_0.tar.bz2#62b743e1030b17163c70654601afb60d
 https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py311h9547e67_4.conda#586da7df03b68640de14dc3e8bcbf76f
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py311h1f0f07a_0.conda#b7e6d52b39e199238c3400cafaabafb3
-https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.0-py311h9547e67_0.conda#40828c5b36ef52433e21f89943e09f33
-https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.2.1-pyhd8ed1ab_0.conda#72ac49d50b7af2159a8f4128bc1f856d
+https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py311h9547e67_0.conda#74ad0ae64f1ef565e27eda87fa749e84
+https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.1-pyhd8ed1ab_0.conda#52387f00fee8dcd5cf75f8886025293f
 https://conda.anaconda.org/conda-forge/noarch/identify-2.5.35-pyhd8ed1ab_0.conda#9472bfd206a2b7bb8143835e37667054
 https://conda.anaconda.org/conda-forge/linux-64/mo_pack-0.3.0-py311h459d7ec_1.conda#45b8d355bbcdd27588c2d266bcfdff84
-https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.0-ha41ecd1_0.conda#62f61784f6feddf19ffcba71d5f7dbbd
-https://conda.anaconda.org/conda-forge/linux-64/scipy-1.12.0-py311h64a7726_2.conda#24ca5107ab75c5521067b8ba505dfae5
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_0.conda#2a6b1e6a1a0c301e4bfff82d7672437a
+https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.2-ha41ecd1_0.conda#a658eeabf188c3040da36b0763de2bfd
+https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py311h64a7726_0.conda#d443c70b4a05f50236c70b9c79beff64
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_1.conda#b065535ca8ca824703ae5537087e2206
 https://conda.anaconda.org/conda-forge/linux-64/shapely-2.0.3-py311h2032efe_0.conda#e982956906078eeac9feb3b8db10d011
 https://conda.anaconda.org/conda-forge/noarch/tox-conda-0.9.2-pyhd8ed1ab_0.tar.bz2#8494c2ad4bef7bfe2e2d8603b4c2a185
 https://conda.anaconda.org/conda-forge/linux-64/cf-units-3.2.0-py311h1f0f07a_4.conda#1e105c1a8ea2163507726144b401eb1b
-https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h7f000aa_3.conda#0abfa7f9241a0f4fd732bc15773cfb0c
-https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.56.3-he3f83f7_1.conda#03bd1ddcc942867a19528877143b9852
-https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.3-py311h54ef318_0.conda#014c115be880802d2372ac6ed665f526
+https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h280cfa0_4.conda#410f86e58e880dcc7b0e910a8e89c05c
+https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hce6bd6c_0.conda#0891de8980ee29828542dbf9578838b9
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py311h54ef318_0.conda#150186110f111b458f86c04361351337
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py311he8ad708_100.conda#597b1ad6cb7011b7561c20ea30295cae
-https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.6.2-pyha770c72_0.conda#61534ee57ffdf26d7b1b514d33daccc4
-https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.22.0-py311h320fe9a_1.conda#10d1806e20da040c58c36deddf51c70c
+https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.0-pyha770c72_0.conda#846ba0877cda9c4f11e13720cacd1968
+https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.23.0-py311h320fe9a_0.conda#fcda2652548238199b7de71dbde4e7fe
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-9.0.0-h78e8752_1.conda#a3f4cd4a512ec5db35ffbf25ba11f537
-https://conda.anaconda.org/conda-forge/noarch/iris-3.8.0-pyha770c72_0.conda#6a92f316e0c5fc52c9d7cff5fa348bc3
+https://conda.anaconda.org/conda-forge/noarch/iris-3.8.1-pyha770c72_0.conda#b08a116ef1607e7e960a4caa902e3a90
 https://conda.anaconda.org/conda-forge/linux-64/pygraphviz-1.12-py311hbf5cbc9_0.conda#135bb7a5bc83c167ddbf1de01d8313f3
 https://conda.anaconda.org/conda-forge/noarch/sphinx-basic-ng-1.0.0b2-pyhd8ed1ab_1.conda#a631f5c7b7f5045448f966ad71aa2881
 https://conda.anaconda.org/conda-forge/noarch/furo-2024.1.29-pyhd8ed1ab_0.conda#f67437927d5ead424d7dcf1f4d9b7c66
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0.conda#26acae54b06f178681bfb551760f5dd1
```

### Comparing `CSET-24.2.1/requirements/locks/py312-lock-linux-64.txt` & `cset-24.4.1/requirements/locks/py312-lock-linux-64.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,85 +14,90 @@
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.27.0-hd590300_0.conda#f6afff0e9ee08d2f1b897881a4f38cdb
+https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/geos-3.12.1-h59595ed_0.conda#8c0f4f71f5a59ceb0c6fa9f51501066d
-https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
-https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.1-h0b41bf4_3.conda#96f3b11872ef6fad973eac856cd2624f
-https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
+https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
+https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.2-hd590300_0.conda#3bf7b9fd5a7136126e0234db4b87c8b6
+https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
-https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.2-h59595ed_1.conda#127b0be54c1c90760d7fe02ea7a56426
+https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.3-h59595ed_0.conda#5e97e271911b8b2001a8b71860c32faa
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
-https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.19-hd590300_0.conda#1635570038840ee3f9c71d22aa5b8b6d
+https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
-https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libmo_unpack-3.1.2-hf484d3e_1001.tar.bz2#95f32a6a5a666d33886ca5627239f03d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_0.conda#30de3fd9b3b602f7473f30e684eeea8c
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-h59595ed_2.conda#7dbaa197d7ba6032caf7ae7f32c1efa0
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_0.conda#51a753e64a3027bd7e23a189b1f6e91e
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.43.2-h59595ed_0.conda#71004cbf7924e19c02746ccde9fd7123
 https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
-https://conda.anaconda.org/conda-forge/linux-64/snappy-1.1.10-h9fff704_0.conda#e6d228cd0bb74a51dd18f5bfce0b4115
+https://conda.anaconda.org/conda-forge/linux-64/snappy-1.2.0-hdb0a2a9_1.conda#843bbb8ace1d64ac50d64639ff38b014
 https://conda.anaconda.org/conda-forge/linux-64/xorg-kbproto-1.0.7-h7f98852_1002.tar.bz2#4b230e8381279d76131116660f5a241a
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.1.1-hd590300_0.conda#b462a33c0be1421532f28bfe8f4a7514
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda#2c80dc38fface310c9bd81b17037fee5
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
 https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2#06feff3d2634e3097ce2fe681474b534
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xxhash-0.8.2-hd590300_0.conda#f08fb5c89edfc4aadee1c81d4cfb1fa1
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.6.2-h59595ed_0.conda#53fb86322bdb89496d7579fe3f02fd61
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h2a13503_7.conda#bd77f8da987968ec3927990495dc22e4
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.1-h2797004_0.conda#fc4ccadfbf6d4784de88c41704792562
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libudunits2-2.2.28-h40f5838_3.conda#4bdace082e911a3e1f1f0b721bed5b56
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.5-h232c23b_0.conda#c442ebfda7a475f5e78f1c8e45f1e919
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
-https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.42-hcad00b1_0.conda#679c8961826aa4b50653bce17ee52abe
+https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
-https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-h0f2a231_0.conda#009521b7ed97cca25f8f997f9e745976
+https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
+https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.78.4-h783c2da_0.conda#d86baf8740d1a906b9716f2a0bac2f2d
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.26-pthreads_h413a1c8_0.conda#760ae35415f5ba8b15d09df5afe8b23a
-https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-ha9c0a0a_2.conda#55ed21669b2015f77c180feb1dd41930
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
+https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda#ad7b68400f3a6ebe72b00be093c7f301
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.1-h2c6b66d_0.conda#93acf31b379acebada263b9bce3dc6ed
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.2-h2c6b66d_0.conda#1423efca06ed343c1da0fc429bae0779
 https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-h40f5838_3.conda#6bb8deb138f87c9d48320ac21b87e7a1
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.7-h8ee46fc_0.conda#49e482d882669206653b095f5206c05b
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda#077b6e8ad6a3ddb741fce2496dd01bec
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/antlr-python-runtime-4.11.1-pyhd8ed1ab_0.tar.bz2#15109c4977d39ad7aa3423f57243e286
 https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.1.0-hd590300_1.conda#f27a24d46e3ea7b70a1f98e50c62508f
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py312h30efb56_1.conda#45801a89533d3336a365284d93298e36
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
@@ -100,113 +105,113 @@
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-3.0.0-pyhd8ed1ab_0.conda#753d29fe41bb881e4b9c004f0abf973f
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py312h7900ff3_3.conda#1b90835ae26b9b8250b302649359a989
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.1-pyhd8ed1ab_0.conda#0c1729b74a8152fde6a38ba0a2ab9f45
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.2.0-pyhca7485f_0.conda#fad86b90138cf5d82c6f5a2ed6e683d9
-https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_4.conda#252a696860674caf7a855e16f680d63a
+https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.3.1-pyhca7485f_0.conda#b7f0662ef2c9d4404f0af9eef5ed2fde
+https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_5.conda#8fdb82e5d9694dd8e9ed9ac8fdf48a26
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py312h8572e83_1.conda#c1e71f2bc05d8e8e033aefac2c490d05
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-21_linux64_openblas.conda#0ac9f44fc096772b0aa092119b00c3ca
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.5.0-hca28451_0.conda#7144d5a828e2cae218e0e3c98d8a0aeb
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.3.2-h658648e_1.conda#0ebb65e8d86843865796c7c95a941f34
 https://conda.anaconda.org/conda-forge/noarch/locket-1.0.0-pyhd8ed1ab_0.tar.bz2#91e27ef3d05cc772ce627e51cff111c4
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py312h98912ed_0.conda#6ff0b9582da2d4a74a1f9ae1f9ce2af6
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
-https://conda.anaconda.org/conda-forge/noarch/packaging-23.2-pyhd8ed1ab_0.conda#79002079284aa895f883c6b7f3f88fd6
+https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
 https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.1-pyhd8ed1ab_0.conda#176f7d56f0cfe9008bdf1bccd7de02fb
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pyshp-2.3.1-pyhd8ed1ab_0.tar.bz2#92a889dc236a5197612bc85bee6d7174
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/linux-64/python-xxhash-3.4.1-py312h98912ed_0.conda#a8f9739e0ada2320148c92ddd608864f
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda#e3fd78d8d490af1d84763b9fe3f2e552
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py312h98912ed_0.conda#05f31c2a79ba61df8d6d903ce4a4ce7b
-https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.0-py312h9118e91_0.conda#e4610184b6aaee7c572cdd9a41c44913
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.1.1-pyhd8ed1ab_0.conda#576de899521b7d43674ba3ef6eae9142
+https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py312h9118e91_0.conda#76dc72c065cc15f69b96656b3431a5a4
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.10.0-pyha770c72_0.conda#16ae769069b380646c47142d719ef466
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.42.0-pyhd8ed1ab_0.conda#1cdea58981c5cbc17b51973bcaddcea7
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py312hf06ca03_0.conda#56b0ca764ce23cc54f3f7e2a7b970f6d
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.3-py312h98912ed_1.conda#f5522063e841b6277b92a8beb6a13905
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.49.0-py312h98912ed_0.conda#b0d9bd8d89f85d031783e497e6e3bbad
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.4-py312h98912ed_0.conda#7002151fcfe55ded0595fc7c3f5e1209
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py312h98912ed_0.conda#f0cd0e54adf65aaa976f5731b7a3f383
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.0.1-pyha770c72_0.conda#746623a787e06191d80a2133e5daff17
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/isodate-0.6.1-pyhd8ed1ab_0.tar.bz2#4a62c93c1b5c0b920508ae3fd285eaf5
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-21_linux64_openblas.conda#4a3816d06451c4946e2db26b86472cb6
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h119a65a_9.conda#cfebc557e54905dadc355c0e9f003004
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-21_linux64_openblas.conda#1a42f305615c3867684e049e85927531
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda#2a75b296096adabbabadd5e9782e5fcc
 https://conda.anaconda.org/conda-forge/noarch/partd-1.4.1-pyhd8ed1ab_0.conda#acf4b7c0bcd5fa3b0e05801c4d2accd6
-https://conda.anaconda.org/conda-forge/linux-64/pillow-10.2.0-py312hf3581a9_0.conda#f35cb852483290b40b5a47e117e80a1d
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py312hdcec9eb_0.conda#425bb325f970e57a047ac57c4586489d
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/linux-64/proj-9.3.1-h1d62c97_0.conda#44ec51d0857d9be26158bb85caa74fdb
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.0.2-pyhd8ed1ab_0.conda#40bd3ef942b9642a3eb20b0bbf92469b
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py312h98912ed_0.conda#a99a06a875138829ef65f44bbe2c30ca
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.10.0-hd8ed1ab_0.conda#091683b9150d2ebaa62fd7e2c86433da
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.0.1-hd8ed1ab_0.conda#4a2f43a20fa404b998859c6a470ba316
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py312heda63a1_0.conda#d8285bea2a350f63fab23bf460221f3f
 https://conda.anaconda.org/conda-forge/linux-64/pyproj-3.6.1-py312h38f1c37_5.conda#867baf2a7c5c6147e05ecc90f6c52a0c
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda#06eb685a3a0b146347a58dda979485da
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda#c54c0107057d67ddf077751339ec2c63
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_0.conda#3b8ef3a2d80f3d89d0ae7e3c975e6c57
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_1.conda#a1986ad21c766ff22f7bae93f0641020
 https://conda.anaconda.org/conda-forge/noarch/tox-3.27.1-pyhd8ed1ab_0.tar.bz2#62b743e1030b17163c70654601afb60d
 https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py312h8572e83_4.conda#52c9e25ee0a32485a102eeecdb7eef52
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py312hc7c0aa3_0.conda#bd11505f0fe9bd8bcec01ce1220f63c7
-https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.0-py312h8572e83_0.conda#b6249daaaf4577e6f72d95fc4ab767c6
-https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.2.1-pyhd8ed1ab_0.conda#72ac49d50b7af2159a8f4128bc1f856d
+https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py312h8572e83_0.conda#12c6a831ef734f0b2dd4caff514cbb7f
+https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.1-pyhd8ed1ab_0.conda#52387f00fee8dcd5cf75f8886025293f
 https://conda.anaconda.org/conda-forge/noarch/identify-2.5.35-pyhd8ed1ab_0.conda#9472bfd206a2b7bb8143835e37667054
 https://conda.anaconda.org/conda-forge/linux-64/mo_pack-0.3.0-py312h98912ed_1.conda#d5273d1e67b7b3a871a0a711c6532a2f
-https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.0-ha41ecd1_0.conda#62f61784f6feddf19ffcba71d5f7dbbd
-https://conda.anaconda.org/conda-forge/linux-64/scipy-1.12.0-py312heda63a1_2.conda#17729ab9bbb780e93458c7857afffcab
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_0.conda#2a6b1e6a1a0c301e4bfff82d7672437a
+https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.2-ha41ecd1_0.conda#a658eeabf188c3040da36b0763de2bfd
+https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py312heda63a1_0.conda#c53b9f319cafc679476f5613599857e8
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_1.conda#b065535ca8ca824703ae5537087e2206
 https://conda.anaconda.org/conda-forge/linux-64/shapely-2.0.3-py312h9e6bd2c_0.conda#5e0580a84d702cda52c8b0245e4c14d2
 https://conda.anaconda.org/conda-forge/noarch/tox-conda-0.9.2-pyhd8ed1ab_0.tar.bz2#8494c2ad4bef7bfe2e2d8603b4c2a185
 https://conda.anaconda.org/conda-forge/linux-64/cf-units-3.2.0-py312hc7c0aa3_4.conda#d9c9fa64fdf4e57d7f8957b957d784a0
-https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h7f000aa_3.conda#0abfa7f9241a0f4fd732bc15773cfb0c
-https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.56.3-he3f83f7_1.conda#03bd1ddcc942867a19528877143b9852
-https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.3-py312he5832f3_0.conda#3b0545901b09b1376b9c0e0ec72409de
+https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h280cfa0_4.conda#410f86e58e880dcc7b0e910a8e89c05c
+https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hce6bd6c_0.conda#0891de8980ee29828542dbf9578838b9
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py312he5832f3_0.conda#5377a9a29f607eebe4ad63eb82bcb575
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py312h26027e0_100.conda#2d7b4954dc5a090796e0ba89c325d09b
-https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.6.2-pyha770c72_0.conda#61534ee57ffdf26d7b1b514d33daccc4
-https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.22.0-py312hfb8ada1_1.conda#17e09fffccc807ef2d2644f21883d64f
+https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.0-pyha770c72_0.conda#846ba0877cda9c4f11e13720cacd1968
+https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.23.0-py312hfb8ada1_0.conda#73e223e294f96540f293bf977a37696c
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-9.0.0-h78e8752_1.conda#a3f4cd4a512ec5db35ffbf25ba11f537
-https://conda.anaconda.org/conda-forge/noarch/iris-3.8.0-pyha770c72_0.conda#6a92f316e0c5fc52c9d7cff5fa348bc3
+https://conda.anaconda.org/conda-forge/noarch/iris-3.8.1-pyha770c72_0.conda#b08a116ef1607e7e960a4caa902e3a90
 https://conda.anaconda.org/conda-forge/linux-64/pygraphviz-1.12-py312h7a1eb4d_0.conda#614fb9d778358220fed4f79e1a260922
 https://conda.anaconda.org/conda-forge/noarch/sphinx-basic-ng-1.0.0b2-pyhd8ed1ab_1.conda#a631f5c7b7f5045448f966ad71aa2881
 https://conda.anaconda.org/conda-forge/noarch/furo-2024.1.29-pyhd8ed1ab_0.conda#f67437927d5ead424d7dcf1f4d9b7c66
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0.conda#26acae54b06f178681bfb551760f5dd1
```

### Comparing `CSET-24.2.1/requirements/locks/py39-lock-linux-64.txt` & `cset-24.4.1/requirements/locks/py39-lock-linux-64.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,85 +14,90 @@
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.27.0-hd590300_0.conda#f6afff0e9ee08d2f1b897881a4f38cdb
+https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/geos-3.12.1-h59595ed_0.conda#8c0f4f71f5a59ceb0c6fa9f51501066d
-https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
-https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.1-h0b41bf4_3.conda#96f3b11872ef6fad973eac856cd2624f
-https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
+https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
+https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.2-hd590300_0.conda#3bf7b9fd5a7136126e0234db4b87c8b6
+https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
-https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.2-h59595ed_1.conda#127b0be54c1c90760d7fe02ea7a56426
+https://conda.anaconda.org/conda-forge/linux-64/libaec-1.1.3-h59595ed_0.conda#5e97e271911b8b2001a8b71860c32faa
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
-https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.19-hd590300_0.conda#1635570038840ee3f9c71d22aa5b8b6d
+https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
-https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libmo_unpack-3.1.2-hf484d3e_1001.tar.bz2#95f32a6a5a666d33886ca5627239f03d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_0.conda#30de3fd9b3b602f7473f30e684eeea8c
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-h59595ed_2.conda#7dbaa197d7ba6032caf7ae7f32c1efa0
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_0.conda#51a753e64a3027bd7e23a189b1f6e91e
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.43.2-h59595ed_0.conda#71004cbf7924e19c02746ccde9fd7123
 https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
-https://conda.anaconda.org/conda-forge/linux-64/snappy-1.1.10-h9fff704_0.conda#e6d228cd0bb74a51dd18f5bfce0b4115
+https://conda.anaconda.org/conda-forge/linux-64/snappy-1.2.0-hdb0a2a9_1.conda#843bbb8ace1d64ac50d64639ff38b014
 https://conda.anaconda.org/conda-forge/linux-64/xorg-kbproto-1.0.7-h7f98852_1002.tar.bz2#4b230e8381279d76131116660f5a241a
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.1.1-hd590300_0.conda#b462a33c0be1421532f28bfe8f4a7514
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda#2c80dc38fface310c9bd81b17037fee5
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
 https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2#06feff3d2634e3097ce2fe681474b534
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xxhash-0.8.2-hd590300_0.conda#f08fb5c89edfc4aadee1c81d4cfb1fa1
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.6.2-h59595ed_0.conda#53fb86322bdb89496d7579fe3f02fd61
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h2a13503_7.conda#bd77f8da987968ec3927990495dc22e4
+https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
+https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.1-h2797004_0.conda#fc4ccadfbf6d4784de88c41704792562
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libudunits2-2.2.28-h40f5838_3.conda#4bdace082e911a3e1f1f0b721bed5b56
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.5-h232c23b_0.conda#c442ebfda7a475f5e78f1c8e45f1e919
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
-https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.42-hcad00b1_0.conda#679c8961826aa4b50653bce17ee52abe
+https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
-https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-h0f2a231_0.conda#009521b7ed97cca25f8f997f9e745976
+https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
+https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.78.4-h783c2da_0.conda#d86baf8740d1a906b9716f2a0bac2f2d
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.26-pthreads_h413a1c8_0.conda#760ae35415f5ba8b15d09df5afe8b23a
-https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-ha9c0a0a_2.conda#55ed21669b2015f77c180feb1dd41930
-https://conda.anaconda.org/conda-forge/linux-64/python-3.9.18-h0755675_1_cpython.conda#255a7002aeec7a067ff19b545aca6328
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.1-h2c6b66d_0.conda#93acf31b379acebada263b9bce3dc6ed
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
+https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
+https://conda.anaconda.org/conda-forge/linux-64/python-3.9.19-h0755675_0_cpython.conda#d9ee3647fbd9e8595b8df759b2bbefb8
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.45.2-h2c6b66d_0.conda#1423efca06ed343c1da0fc429bae0779
 https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-h40f5838_3.conda#6bb8deb138f87c9d48320ac21b87e7a1
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.7-h8ee46fc_0.conda#49e482d882669206653b095f5206c05b
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda#077b6e8ad6a3ddb741fce2496dd01bec
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/antlr-python-runtime-4.11.1-pyhd8ed1ab_0.tar.bz2#15109c4977d39ad7aa3423f57243e286
 https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.1.0-hd590300_1.conda#f27a24d46e3ea7b70a1f98e50c62508f
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py39h3d6467e_1.conda#c48418c8b35f1d59ae9ae1174812b40a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
@@ -100,116 +105,116 @@
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-3.0.0-pyhd8ed1ab_0.conda#753d29fe41bb881e4b9c004f0abf973f
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py39hf3d152e_3.conda#09a48956e1c155907fd0d626f3e80f2e
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.1-pyhd8ed1ab_0.conda#0c1729b74a8152fde6a38ba0a2ab9f45
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.2.0-pyhca7485f_0.conda#fad86b90138cf5d82c6f5a2ed6e683d9
-https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_4.conda#252a696860674caf7a855e16f680d63a
+https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.3.1-pyhca7485f_0.conda#b7f0662ef2c9d4404f0af9eef5ed2fde
+https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_5.conda#8fdb82e5d9694dd8e9ed9ac8fdf48a26
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py39h7633fee_1.conda#c9f74d717e5a2847a9f8b779c54130f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-21_linux64_openblas.conda#0ac9f44fc096772b0aa092119b00c3ca
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.5.0-hca28451_0.conda#7144d5a828e2cae218e0e3c98d8a0aeb
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.3.2-h658648e_1.conda#0ebb65e8d86843865796c7c95a941f34
 https://conda.anaconda.org/conda-forge/noarch/locket-1.0.0-pyhd8ed1ab_0.tar.bz2#91e27ef3d05cc772ce627e51cff111c4
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py39hd1e30aa_0.conda#9a9a22eb1f83c44953319ee3b027769f
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
-https://conda.anaconda.org/conda-forge/noarch/packaging-23.2-pyhd8ed1ab_0.conda#79002079284aa895f883c6b7f3f88fd6
+https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
 https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.1-pyhd8ed1ab_0.conda#176f7d56f0cfe9008bdf1bccd7de02fb
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pyshp-2.3.1-pyhd8ed1ab_0.tar.bz2#92a889dc236a5197612bc85bee6d7174
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/linux-64/python-xxhash-3.4.1-py39hd1e30aa_0.conda#756cb152772a225587a05ca0ec68fc08
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py39hd1e30aa_1.conda#37218233bcdc310e4fde6453bc1b40d8
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py39hd1e30aa_0.conda#b1961e70cfe8e1eac243faf933d1813f
-https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.0-py39h7efa1f9_0.conda#cb3dfd14bb45827d3570c014d5d9f22b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.1.1-pyhd8ed1ab_0.conda#576de899521b7d43674ba3ef6eae9142
+https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py39h7efa1f9_0.conda#078b4b64a101cd6da6b588cd99bd6158
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.10.0-pyha770c72_0.conda#16ae769069b380646c47142d719ef466
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py39hd1e30aa_0.conda#1da984bbb6e765743e13388ba7b7b2c8
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.42.0-pyhd8ed1ab_0.conda#1cdea58981c5cbc17b51973bcaddcea7
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py39h7a31438_0.conda#ac992767d7f8ed2cb27e71e78f0fb2d7
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.3-py39hd1e30aa_1.conda#b7cb2f01e9d6d390bbc63c0012a32d41
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.49.0-py39hd1e30aa_0.conda#dd1b02484cc8c31d4093111a82b6efb2
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.4-py39hd1e30aa_0.conda#6f8b9c064e8393bc6b25ef1085192ba6
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py39hd1e30aa_0.conda#79f5dd8778873faa54e8f7b2729fe8a6
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.0.1-pyha770c72_0.conda#746623a787e06191d80a2133e5daff17
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.1.2-pyhd8ed1ab_0.conda#6f4399795892835bd192ea210ca69447
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/noarch/isodate-0.6.1-pyhd8ed1ab_0.tar.bz2#4a62c93c1b5c0b920508ae3fd285eaf5
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-21_linux64_openblas.conda#4a3816d06451c4946e2db26b86472cb6
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h119a65a_9.conda#cfebc557e54905dadc355c0e9f003004
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-21_linux64_openblas.conda#1a42f305615c3867684e049e85927531
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda#2a75b296096adabbabadd5e9782e5fcc
 https://conda.anaconda.org/conda-forge/noarch/partd-1.4.1-pyhd8ed1ab_0.conda#acf4b7c0bcd5fa3b0e05801c4d2accd6
-https://conda.anaconda.org/conda-forge/linux-64/pillow-10.2.0-py39had0adad_0.conda#2972754dc054bb079d1d121918b5126f
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py39h90c7501_0.conda#1e3b6af9592be71ce19f0a6aae05d97b
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/linux-64/proj-9.3.1-h1d62c97_0.conda#44ec51d0857d9be26158bb85caa74fdb
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.0.2-pyhd8ed1ab_0.conda#40bd3ef942b9642a3eb20b0bbf92469b
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py39hd1e30aa_0.conda#2289054e90cf07e35280bbe798811dc8
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.10.0-hd8ed1ab_0.conda#091683b9150d2ebaa62fd7e2c86433da
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
-https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.1.2-pyhd8ed1ab_0.conda#c69b222e1a89945b80feb249d57d8949
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.0.1-hd8ed1ab_0.conda#4a2f43a20fa404b998859c6a470ba316
+https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py39h474f0d3_0.conda#aa265f5697237aa13cc10f53fa8acc4f
 https://conda.anaconda.org/conda-forge/linux-64/pyproj-3.6.1-py39h15b0fa6_5.conda#85e186c7ff673b0d0026782ec353fb2a
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda#06eb685a3a0b146347a58dda979485da
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda#c54c0107057d67ddf077751339ec2c63
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_0.conda#3b8ef3a2d80f3d89d0ae7e3c975e6c57
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-8.0.4-pyhd8ed1ab_1.conda#a1986ad21c766ff22f7bae93f0641020
 https://conda.anaconda.org/conda-forge/noarch/tox-3.27.1-pyhd8ed1ab_0.tar.bz2#62b743e1030b17163c70654601afb60d
 https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py39h7633fee_4.conda#b66595fbda99771266f042f42c7457be
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py39h44dd56e_0.conda#baea2f5dfb3ab7b1c836385d2e1daca7
-https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.0-py39h7633fee_0.conda#ed71ad3e30eb03da363fb797419cce98
-https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.2.1-pyhd8ed1ab_0.conda#72ac49d50b7af2159a8f4128bc1f856d
+https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py39h7633fee_0.conda#bdc188e59857d6efab332714e0d01d93
+https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.1-pyhd8ed1ab_0.conda#52387f00fee8dcd5cf75f8886025293f
 https://conda.anaconda.org/conda-forge/noarch/identify-2.5.35-pyhd8ed1ab_0.conda#9472bfd206a2b7bb8143835e37667054
 https://conda.anaconda.org/conda-forge/linux-64/mo_pack-0.3.0-py39hd1e30aa_1.conda#ca63612907462c8e36edcc9bbacc253e
-https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.0-ha41ecd1_0.conda#62f61784f6feddf19ffcba71d5f7dbbd
-https://conda.anaconda.org/conda-forge/linux-64/scipy-1.12.0-py39h474f0d3_2.conda#6ab241b2023730f6b41712dc1b503afa
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_0.conda#2a6b1e6a1a0c301e4bfff82d7672437a
+https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.2-ha41ecd1_0.conda#a658eeabf188c3040da36b0763de2bfd
+https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py39h474f0d3_0.conda#46ae0ecba9726ab4fa44c78fefa522cf
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-8.0.4-hd8ed1ab_1.conda#b065535ca8ca824703ae5537087e2206
 https://conda.anaconda.org/conda-forge/linux-64/shapely-2.0.3-py39h6404dd3_0.conda#1520f039123452cd2de847068449a618
 https://conda.anaconda.org/conda-forge/noarch/tox-conda-0.9.2-pyhd8ed1ab_0.tar.bz2#8494c2ad4bef7bfe2e2d8603b4c2a185
 https://conda.anaconda.org/conda-forge/linux-64/cf-units-3.2.0-py39h44dd56e_4.conda#81310d21bf9d91754c1220c585bb72d6
-https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h7f000aa_3.conda#0abfa7f9241a0f4fd732bc15773cfb0c
-https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.56.3-he3f83f7_1.conda#03bd1ddcc942867a19528877143b9852
-https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.3-py39he9076e7_0.conda#5456bdfe5809ebf5689eda6c808b686e
+https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h280cfa0_4.conda#410f86e58e880dcc7b0e910a8e89c05c
+https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hce6bd6c_0.conda#0891de8980ee29828542dbf9578838b9
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py39he9076e7_0.conda#1919384a8420e7bb25f6c3a582e0857c
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py39h4282601_100.conda#d2809fbf0d8ae7b8ca92c456cb44a7d4
-https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.6.2-pyha770c72_0.conda#61534ee57ffdf26d7b1b514d33daccc4
-https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.22.0-py39hddac248_1.conda#8dd2eb1e7aa9a33a92a75bdcea3f0dd0
+https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.0-pyha770c72_0.conda#846ba0877cda9c4f11e13720cacd1968
+https://conda.anaconda.org/conda-forge/linux-64/cartopy-0.23.0-py39hddac248_0.conda#aa02350ccb542c83272f9cb7e4dfe15e
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-9.0.0-h78e8752_1.conda#a3f4cd4a512ec5db35ffbf25ba11f537
-https://conda.anaconda.org/conda-forge/noarch/iris-3.8.0-pyha770c72_0.conda#6a92f316e0c5fc52c9d7cff5fa348bc3
+https://conda.anaconda.org/conda-forge/noarch/iris-3.8.1-pyha770c72_0.conda#b08a116ef1607e7e960a4caa902e3a90
 https://conda.anaconda.org/conda-forge/linux-64/pygraphviz-1.11-py39h7ef11f9_2.conda#0eab4d12fd2bab26e0ca5aec2d822c0a
 https://conda.anaconda.org/conda-forge/noarch/sphinx-basic-ng-1.0.0b2-pyhd8ed1ab_1.conda#a631f5c7b7f5045448f966ad71aa2881
 https://conda.anaconda.org/conda-forge/noarch/furo-2024.1.29-pyhd8ed1ab_0.conda#f67437927d5ead424d7dcf1f4d9b7c66
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0.conda#26acae54b06f178681bfb551760f5dd1
```

### Comparing `CSET-24.2.1/src/CSET/__init__.py` & `cset-24.4.1/src/CSET/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import argparse
 import logging
 import os
 import sys
 from importlib.metadata import version
 from pathlib import Path
 
+from CSET._common import ArgumentError
+
 
 def main():
     """CLI entrypoint."""
     parser = argparse.ArgumentParser(
         prog="cset", description="Convective Scale Evaluation Tool"
     )
     parser.add_argument(
@@ -38,20 +40,19 @@
         "--version", action="version", version=f"CSET v{version('CSET')}"
     )
 
     # https://docs.python.org/3/library/argparse.html#sub-commands
     subparsers = parser.add_subparsers(title="subcommands", dest="subparser")
 
     # Run operator chain
-    parser_bake = subparsers.add_parser("bake", help="run a recipe file")
+    parser_bake = subparsers.add_parser("bake", help="run steps from a recipe file")
     parser_bake.add_argument(
         "-i",
         "--input-dir",
         type=Path,
-        required=True,
         help="directory containing input data",
     )
     parser_bake.add_argument(
         "-o",
         "--output-dir",
         type=Path,
         required=True,
@@ -60,14 +61,21 @@
     parser_bake.add_argument(
         "-r",
         "--recipe",
         type=Path,
         required=True,
         help="recipe file to read",
     )
+    bake_step_control = parser_bake.add_mutually_exclusive_group()
+    bake_step_control.add_argument(
+        "--parallel-only", action="store_true", help="only run parallel steps"
+    )
+    bake_step_control.add_argument(
+        "--collate-only", action="store_true", help="only run collation steps"
+    )
     parser_bake.set_defaults(func=_bake_command)
 
     parser_graph = subparsers.add_parser("graph", help="visualise a recipe file")
     parser_graph.add_argument(
         "-d",
         "--details",
         action="store_true",
@@ -90,88 +98,146 @@
     )
     parser_graph.set_defaults(func=_graph_command)
 
     parser_cookbook = subparsers.add_parser(
         "cookbook", help="unpack included recipes to a folder"
     )
     parser_cookbook.add_argument(
-        "-l",
-        "--list",
+        "-d",
+        "--details",
         action="store_true",
-        help="list available recipes. Supplied recipes are detailed.",
+        help="list available recipes. Supplied recipes are detailed",
     )
     parser_cookbook.add_argument(
         "-o",
         "--output-dir",
         type=Path,
         help="directory to save recipes. If omitted uses $PWD",
         default=Path.cwd(),
     )
     parser_cookbook.add_argument(
         "recipe",
         type=str,
         nargs="?",
-        help="recipe to output or detail. Omit for all.",
+        help="recipe to output or detail",
         default="",
     )
     parser_cookbook.set_defaults(func=_cookbook_command)
 
+    parser_recipe_id = subparsers.add_parser("recipe-id", help="get the ID of a recipe")
+    parser_recipe_id.add_argument(
+        "-r",
+        "--recipe",
+        type=Path,
+        required=True,
+        help="recipe file to read",
+    )
+    parser_recipe_id.set_defaults(func=_recipe_id_command)
+
     cli_args = sys.argv[1:] + os.getenv("CSET_ADDOPTS", "").split()
     args, unparsed_args = parser.parse_known_args(cli_args)
 
     # Setup logging.
     logging.captureWarnings(True)
-    if args.verbose >= 2:
-        loglevel = logging.DEBUG
-    elif args.verbose == 1:
-        loglevel = logging.INFO
-    else:
-        loglevel = logging.WARNING
+    loglevel = calculate_loglevel(args)
     logger = logging.getLogger()
     logger.setLevel(min(loglevel, logging.INFO))
     stderr_log = logging.StreamHandler()
     stderr_log.addFilter(lambda record: record.levelno >= loglevel)
     stderr_log.setFormatter(logging.Formatter("%(asctime)s %(levelname)s %(message)s"))
     logger.addHandler(stderr_log)
 
-    # Execute the specified subcommand.
-    if args.subparser:
-        try:
-            args.func(args, unparsed_args)
-        except ValueError:
-            parser.print_usage()
-            sys.exit(2)
-    else:
+    if args.subparser is None:
+        print("Please choose a command.", file=sys.stderr)
+        parser.print_usage()
+        sys.exit(127)
+
+    try:
+        # Execute the specified subcommand.
+        args.func(args, unparsed_args)
+    except ArgumentError as err:
+        logging.error(err)
         parser.print_usage()
-        sys.exit(2)
+        sys.exit(3)
+
+
+def calculate_loglevel(args) -> int:
+    """Calculate the logging level to apply.
+
+    Level is based on verbose argument and the LOGLEVEL environment variable.
+    """
+    try:
+        name_to_level = logging.getLevelNamesMapping()
+    except AttributeError:
+        # logging.getLevelNamesMapping() is python 3.11 or newer. Using
+        # implementation detail for older versions.
+        name_to_level = logging._nameToLevel
+    # Level from CLI flags.
+    if args.verbose >= 2:
+        loglevel = logging.DEBUG
+    elif args.verbose == 1:
+        loglevel = logging.INFO
+    else:
+        loglevel = logging.WARNING
+    return min(
+        loglevel,
+        # Level from environment variable.
+        name_to_level.get(os.getenv("LOGLEVEL"), logging.ERROR),
+    )
 
 
 def _bake_command(args, unparsed_args):
     from CSET._common import parse_variable_options
-    from CSET.operators import execute_recipe
+    from CSET.operators import execute_recipe_collate, execute_recipe_parallel
 
     recipe_variables = parse_variable_options(unparsed_args)
-
-    execute_recipe(args.recipe, args.input_dir, args.output_dir, recipe_variables)
+    if not args.collate_only:
+        # Input dir is needed for parallel steps, but not collate steps.
+        if not args.input_dir:
+            raise ArgumentError("the following arguments are required: -i/--input-dir")
+        execute_recipe_parallel(
+            args.recipe, args.input_dir, args.output_dir, recipe_variables
+        )
+    if not args.parallel_only:
+        execute_recipe_collate(args.recipe, args.output_dir, recipe_variables)
 
 
 def _graph_command(args, unparsed_args):
     from CSET.graph import save_graph
 
     save_graph(
         args.recipe,
         args.output_path,
         auto_open=not args.output_path,
         detailed=args.details,
     )
 
 
 def _cookbook_command(args, unparsed_args):
-    from CSET.recipes import detail_recipe, list_available_recipes, unpack_recipes
+    from CSET.recipes import detail_recipe, list_available_recipes, unpack_recipe
 
-    if args.list:
-        if args.recipe:
+    if args.recipe:
+        if args.details:
             detail_recipe(args.recipe)
         else:
-            list_available_recipes()
+            try:
+                unpack_recipe(args.output_dir, args.recipe)
+            except FileNotFoundError:
+                logging.error("Recipe %s does not exist.", args.recipe)
+                sys.exit(1)
     else:
-        unpack_recipes(args.output_dir, args.recipe)
+        list_available_recipes()
+
+
+def _recipe_id_command(args, unparsed_args):
+    from uuid import uuid4
+
+    from CSET._common import parse_recipe, parse_variable_options, slugify
+
+    recipe_variables = parse_variable_options(unparsed_args)
+    recipe = parse_recipe(args.recipe, recipe_variables)
+    try:
+        recipe_id = slugify(recipe["title"])
+    except KeyError:
+        logging.warning("Recipe has no title; Falling back to random recipe_id.")
+        recipe_id = str(uuid4())
+    print(recipe_id)
```

### Comparing `CSET-24.2.1/src/CSET/__main__.py` & `cset-24.4.1/src/CSET/__main__.py`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/src/CSET/graph.py` & `cset-24.4.1/src/CSET/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,21 +57,21 @@
     """
     recipe = parse_recipe(recipe_file)
     if save_path is None:
         save_path = Path(f"{tempfile.gettempdir()}/{uuid4()}.svg")
 
     def step_parser(step: dict, prev_node: str) -> str:
         """Parse recipe to add nodes to graph and link them with edges."""
-        logging.debug(f"Executing step: {step}")
+        logging.debug("Executing step: %s", step)
         node = str(uuid4())
         graph.add_node(node, label=step["operator"])
         kwargs = {}
         for key in step.keys():
             if isinstance(step[key], dict) and "operator" in step[key]:
-                logging.debug(f"Recursing into argument: {key}")
+                logging.debug("Recursing into argument: %s", key)
                 sub_node = step_parser(step[key], prev_node)
                 graph.add_edge(sub_node, node)
             elif key != "operator":
                 kwargs[key] = step[key]
         graph.add_edge(prev_node, node)
 
         if detailed:
@@ -81,15 +81,16 @@
         return node
 
     graph = pygraphviz.AGraph(directed=True)
 
     prev_node = "START"
     graph.add_node(prev_node)
     try:
-        for step in recipe["steps"]:
+        # TODO: Expand to cover collate too.
+        for step in recipe["parallel"]:
             prev_node = step_parser(step, prev_node)
     except KeyError as err:
         raise ValueError("Invalid recipe") from err
 
     graph.draw(save_path, format="svg", prog="dot")
     print(f"Graph rendered to {save_path}")
```

### Comparing `CSET-24.2.1/src/CSET/operators/aggregate.py` & `cset-24.4.1/src/CSET/operators/aggregate.py`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/src/CSET/operators/collapse.py` & `cset-24.4.1/src/CSET/operators/collapse.py`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/src/CSET/operators/constraints.py` & `cset-24.4.1/src/CSET/operators/constraints.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Operators to generate constraints to filter with."""
 
 from datetime import datetime
 from typing import Union
 
 import iris
 import iris.cube
+import iris.exceptions
 
 
 def generate_stash_constraint(stash: str, **kwargs) -> iris.AttributeConstraint:
     """Generate constraint from STASH code.
 
     Operator that takes a stash string, and uses iris to generate a constraint
     to be passed into the read operator to minimize the CubeList the read
@@ -85,14 +86,51 @@
     model_level_number = int(model_level_number)
     model_level_number_constraint = iris.Constraint(
         model_level_number=model_level_number
     )
     return model_level_number_constraint
 
 
+def generate_pressure_level_constraint(
+    pressure_levels: Union[int, list[int]], **kwargs
+) -> iris.Constraint:
+    """Generate constraint for the specified pressure_levels.
+
+    If no pressure levels are specified then any cube with a pressure coordinate
+    is rejected.
+
+    Arguments
+    ---------
+    pressure_levels: int|list
+        List of integer pressure levels in hPa either as single integer
+        for a single level or a list of multiple integers.
+
+    Returns
+    -------
+    pressure_constraint: iris.Constraint
+    """
+    # If pressure_level is an integer it is converted into a list.
+    if isinstance(pressure_levels, int):
+        pressure_levels = [pressure_levels]
+    if len(pressure_levels) == 0:
+        # If none specified reject cubes with pressure level coordinate.
+        def no_pressure_coordinate(cube):
+            try:
+                cube.coord("pressure")
+            except iris.exceptions.CoordinateNotFoundError:
+                return True
+            return False
+
+        pressure_constraint = iris.Constraint(cube_func=no_pressure_coordinate)
+    else:
+        pressure_constraint = iris.Constraint(pressure=pressure_levels)
+
+    return pressure_constraint
+
+
 def generate_cell_methods_constraint(cell_methods: list, **kwargs) -> iris.Constraint:
     """Generate constraint from cell methods.
 
     Operator that takes a list of cell methods and generates a constraint from
     that.
 
     Arguments
@@ -102,18 +140,15 @@
 
     Returns
     -------
     cell_method_constraint: iris.Constraint
     """
 
     def check_cell_methods(cube: iris.cube.Cube):
-        if cube.cell_methods == tuple(cell_methods):
-            return True
-        else:
-            return False
+        return cube.cell_methods == tuple(cell_methods)
 
     cell_methods_constraint = iris.Constraint(cube_func=check_cell_methods)
     return cell_methods_constraint
 
 
 def generate_time_constraint(
     time_start: str, time_end: str = None, **kwargs
```

### Comparing `CSET-24.2.1/src/CSET/operators/convection.py` & `cset-24.4.1/src/CSET/operators/convection.py`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/src/CSET/operators/filters.py` & `cset-24.4.1/src/CSET/operators/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,19 +45,20 @@
         If the constraint doesn't produce a single cube.
     """
     filtered_cubes = cube.extract(constraint)
     # Return directly if already a cube.
     if isinstance(filtered_cubes, iris.cube.Cube):
         return filtered_cubes
     # Check filtered cubes is a CubeList containing one cube.
-    if len(filtered_cubes) == 1:
+    if isinstance(filtered_cubes, iris.cube.CubeList) and len(filtered_cubes) == 1:
         return filtered_cubes[0]
     else:
         raise ValueError(
-            f"Constraint doesn't produce single cube. {constraint}\n{filtered_cubes}"
+            f"Constraint doesn't produce single cube. Constraint: {constraint}"
+            f"\nSource: {cube}\nResult: {filtered_cubes}"
         )
 
 
 def filter_multiple_cubes(
     cubes: Union[iris.cube.Cube, iris.cube.CubeList],
     **kwargs,
 ) -> iris.cube.CubeList:
@@ -84,9 +85,11 @@
     if isinstance(cubes, iris.cube.Cube):
         cubes = iris.cube.CubeList((cubes,))
     if len(kwargs) < 1:
         raise ValueError("Must have at least one constraint.")
     try:
         filtered_cubes = cubes.extract_cubes(kwargs.values())
     except iris.exceptions.ConstraintMismatchError as err:
-        raise ValueError() from err
+        raise ValueError(
+            "The constraints don't produce a single cube per constraint."
+        ) from err
     return filtered_cubes
```

### Comparing `CSET-24.2.1/src/CSET/operators/read.py` & `cset-24.4.1/src/CSET/operators/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from pathlib import Path
 
 import iris
 import iris.coords
 import iris.cube
 import numpy as np
 
+from CSET._common import iter_maybe
+
 
 def read_cube(
     loadpath: Path,
     constraint: iris.Constraint = None,
     filename_pattern: str = "*",
     **kwargs,
 ) -> iris.cube.Cube:
@@ -101,15 +103,15 @@
     Deterministic data will be loaded with a realization of 0, allowing it to be
     processed in the same way as ensemble data.
 
     Arguments
     ---------
     loadpath: pathlike
         Path to where .pp/.nc files are located
-    constraint: iris.Constraint or iris.ConstraintCombination, optional
+    constraint: iris.Constraint | iris.ConstraintCombination, optional
         Constraints to filter data by
     filename_pattern: str, optional
         Unix shell-style pattern to match filenames to. Defaults to "*"
 
     Returns
     -------
     cubes: iris.cube.CubeList
@@ -122,17 +124,20 @@
     """
     if isinstance(loadpath, str):
         loadpath = Path(loadpath)
 
     if loadpath.is_dir():
         loadpath = sorted(loadpath.glob(filename_pattern))
 
-    logging.info("Loading file(s): %s", loadpath)
+    logging.info(
+        "Loading files:\n%s", "\n".join(str(path) for path in iter_maybe(loadpath))
+    )
 
     if constraint is not None:
+        logging.debug("Constraint: %s", constraint)
         cubes = iris.load(loadpath, constraint)
     else:
         cubes = iris.load(loadpath)
     if _is_ensemble(cubes):
         logging.info("Ensemble data, reloading with correct handling.")
         if constraint:
             cubes = iris.load(loadpath, constraint, callback=_ensemble_callback)
@@ -144,14 +149,17 @@
         # same way as ensembles.
         for cube in cubes:
             cube.add_aux_coord(
                 iris.coords.AuxCoord(
                     np.int32(0), standard_name="realization", units="1"
                 )
             )
+    logging.debug("Loaded cubes: %s", cubes)
+    if len(cubes) == 0:
+        logging.warning("No cubes loaded, check your constraints!")
     return cubes
 
 
 def _is_ensemble(cubelist: iris.cube.CubeList) -> bool:
     """Test if a cubelist is likely to be ensemble data.
 
     If cubes either have a realization dimension, or there are multiple files
```

### Comparing `CSET-24.2.1/src/CSET/operators/write.py` & `cset-24.4.1/src/CSET/operators/write.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,43 +10,55 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Operators for writing various types of files to disk."""
 
+import secrets
 from pathlib import Path
 from typing import Union
 
 import iris
 import iris.cube
 
 from CSET._common import get_recipe_metadata, slugify
 
 
 def write_cube_to_nc(
-    cube: Union[iris.cube.Cube, iris.cube.CubeList], filename: Path = None, **kwargs
+    cube: Union[iris.cube.Cube, iris.cube.CubeList],
+    filename: str = None,
+    overwrite: bool = False,
+    **kwargs,
 ) -> str:
     """Write a cube to a NetCDF file.
 
-    This operator expects an iris cube object that will then be passed to MET
-    for further processing.
+    This operator expects an iris cube object that will then be saved to disk.
 
     Arguments
     ---------
     cube: iris.cube.Cube | iris.cube.CubeList
         Data to save.
-    filename: Path, optional
+    filename: str, optional
         Path to save the cubes too. Defaults to the recipe title + .nc
+    overwrite: bool, optional
+        Whether to overwrite an existing file. If False the filename will have a
+        unique suffix added. Defaults to False.
 
     Returns
     -------
     Cube | CubeList
         The inputted cube(list) (so further operations can be applied)
     """
     if filename is None:
         filename = slugify(get_recipe_metadata().get("title", "Untitled"))
+
+    # Append a unique suffix if not overwriting. We use randomness rather than a
+    # sequence number to avoid race conditions with multiple job runners.
+    if not overwrite:
+        filename = f"{filename}_{secrets.token_urlsafe(16)}.nc"
+
     # Ensure that output filename is a Path with a .nc suffix
     filename = Path(filename).with_suffix(".nc")
     # Save the file as nc compliant (iris should handle this)
     iris.save(cube, filename, zlib=True)
     return cube
```

### Comparing `CSET-24.2.1/src/CSET/recipes/CAPE_ratio_plot.yaml` & `cset-24.4.1/src/CSET/recipes/CAPE_ratio_plot.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 title: CAPE ratio plot
 description: |
   Extracts data required for, and calculates the CAPE ratio diagnostic, plotting on a map.
 
-steps:
+parallel:
   - operator: read.read_cubes
 
   - operator: convection.cape_ratio
     SBCAPE:
         operator: filters.filter_cubes
         constraint:
             operator: constraints.generate_stash_constraint
```

### Comparing `CSET-24.2.1/src/CSET/recipes/__init__.py` & `cset-24.4.1/src/CSET/recipes/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,78 +10,103 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Operations on recipes."""
 
+import importlib.resources
 import logging
+import sys
 import warnings
-from importlib.resources import files
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Iterable
 
 import ruamel.yaml
 
-import CSET.recipes as recipes
+
+def _version_agnostic_importlib_resources_file() -> Path:
+    """Transitional wrapper to importlib.resources.files().
+
+    Importlib behaviour changed in 3.12 to avoid circular dependencies.
+    """
+    if sys.version_info.minor >= 12:
+        input_dir = importlib.resources.files()
+    else:
+        import CSET.recipes
+
+        input_dir = importlib.resources.files(CSET.recipes)
+    return input_dir
 
 
 def _recipe_files_in_tree(
     recipe_name: str = None, input_dir: Path = None
 ) -> Iterable[Path]:
-    """Yield recipe file paths matching the recipe name."""
+    """Yield recipe file Paths matching the recipe name."""
     if recipe_name is None:
         recipe_name = ""
     if input_dir is None:
-        input_dir = files(recipes)
+        input_dir = _version_agnostic_importlib_resources_file()
     for file in input_dir.iterdir():
         logging.debug("Testing %s", file)
         if recipe_name in file.name and file.is_file() and file.suffix == ".yaml":
             yield file
         elif file.is_dir() and file.name[0] != "_":  # Excludes __pycache__
             yield from _recipe_files_in_tree(recipe_name, file)
 
 
-def unpack_recipes(recipe_dir: Path, recipe_name: str = None) -> None:
+def _get_recipe_file(recipe_name: str, input_dir: Path = None) -> Path:
+    """Return a Path to the recipe file."""
+    if input_dir is None:
+        input_dir = _version_agnostic_importlib_resources_file()
+    file = input_dir / recipe_name
+    logging.debug("Getting recipe: %s", file)
+    if not file.is_file():
+        raise FileNotFoundError("Recipe file does not exist.", recipe_name)
+    return file
+
+
+def unpack_recipe(recipe_dir: Path, recipe_name: str) -> None:
     """
     Unpacks recipes files into a directory, creating it if it doesn't exist.
 
     Parameters
     ----------
     recipe_dir: Path
         Path to a directory into which to unpack the recipe files.
+    recipe_name: str
+        Name of recipe to unpack.
 
     Raises
     ------
     FileExistsError
         If recipe_dir already exists, and is not a directory.
 
     OSError
         If recipe_dir cannot be created, such as insufficient permissions, or
         lack of space.
     """
-    logging.debug("Saving recipes to %s", recipe_dir)
+    file = _get_recipe_file(recipe_name)
     recipe_dir.mkdir(parents=True, exist_ok=True)
-    for file in _recipe_files_in_tree(recipe_name):
-        logging.debug("Saving %s", file.name)
-        if recipe_dir.joinpath(file.name).exists():
-            warnings.warn(
-                f"{file.name} already exists in target directory, skipping.",
-                stacklevel=2,
-            )
-        else:
-            logging.info("Unpacking %s to %s", file.name, recipe_dir / file.name)
-            (recipe_dir / file.name).write_bytes(file.read_bytes())
+    output_file = recipe_dir / file.name
+    logging.debug("Saving recipe to %s", output_file)
+    if output_file.exists():
+        warnings.warn(
+            f"{file.name} already exists in target directory, skipping.", stacklevel=2
+        )
+        return
+    logging.info("Unpacking %s to %s", file.name, output_file)
+    output_file.write_bytes(file.read_bytes())
 
 
 def list_available_recipes() -> None:
     """List available recipes to stdout."""
     print("Available recipes:")
     for file in _recipe_files_in_tree():
-        print(f"\t{file.stem}")
+        print(f"\t{file.name}")
 
 
 def detail_recipe(recipe_name: str) -> None:
     """Detail the recipe to stdout.
 
     If multiple recipes match the given name they will all be displayed.
 
@@ -89,9 +114,9 @@
     ----------
     recipe_name: str
         Partial match for the recipe name.
     """
     for file in _recipe_files_in_tree(recipe_name):
         with ruamel.yaml.YAML(typ="safe", pure=True) as yaml:
             recipe = yaml.load(file)
-        print(f"\n\t{file.stem}\n\t{''.join('─' * len(file.stem))}\n")
+        print(f"\n\t{file.name}\n\t{''.join('─' * len(file.name))}\n")
         print(recipe.get("description"))
```

### Comparing `CSET-24.2.1/src/CSET/recipes/aggregate_precipitation.yaml` & `cset-24.4.1/src/CSET/recipes/aggregate_precipitation.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 title: Extract sub-hourly or hourly ppn and aggregate to user defined intervals
 description: |
   Extracts out the sub-hourly or hourly
   LARGE SCALE RAINFALL RATE (KG/M2/S) (stash m01s04i203) from a file
   and aggregates it up to new intervals and writes it to a new time coordinate.
 
-steps:
+parallel:
   - operator: read.read_cubes
 
   - operator: filters.filter_cubes
     constraint:
       operator: constraints.combine_constraints
       stash_constraint:
         operator: constraints.generate_stash_constraint
```

### Comparing `CSET-24.2.1/src/CSET/recipes/extract_instant_air_temp.yaml` & `cset-24.4.1/src/CSET/recipes/extract_instant_air_temp.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 description: |
   Extracts out the instantaneous 1.5m air temperature from a file and writes it
   to a new one.
 section: Grid Stat
 major_cat: Major Category 1
 minor_cat: Minor Category 1
 
-steps:
+parallel:
   - operator: read.read_cubes
     constraint:
       operator: constraints.generate_stash_constraint
       stash: m01s03i236
 
   - operator: filters.filter_cubes
     constraint:
```

### Comparing `CSET-24.2.1/src/CSET/recipes/initial_time-step_surface_air_temperature_ensemble_postage_stamp_plot.yaml` & `cset-24.4.1/src/CSET/recipes/initial_time-step_surface_air_temperature_ensemble_postage_stamp_plot.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 title: Initial Time-step Surface Air Temperature Ensemble Postage Stamp Plot
 description: |
   Plots the first time-step from a set of ensemble air temperature files with a
   filename containing the ensemble member in the form `\*_em\*.nc`.
 
-steps:
+parallel:
   - operator: read.read_cubes
     filename_pattern: "*_em*.nc"
     constraint:
       operator: constraints.generate_stash_constraint
       stash: m01s03i236
 
   - operator: collapse.collapse
     coordinate: time
     method: MIN
 
   - operator: plot.postage_stamp_contour_plot
-    filename: plot.svg
+    filename: plot.png
 
   - operator: write.write_cube_to_nc
```

### Comparing `CSET-24.2.1/src/CSET/recipes/mean_surface_air_temperature_spatial_plot.yaml` & `cset-24.4.1/src/CSET/recipes/mean_surface_air_temperature_spatial_plot.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 title: Mean Surface Air Temperature Spatial Plot
 description: |
   Extracts and plots the 1.5m air temperature from a file. The temperature
   is averaged across the time coordinate.
 
-steps:
+parallel:
   - operator: read.read_cubes
     constraint:
       operator: constraints.generate_stash_constraint
       stash: m01s03i236
 
   - operator: filters.filter_cubes
     constraint:
```

### Comparing `CSET-24.2.1/src/CSET/recipes/meaned_model_level_air_temperature_spatial_plot.yaml` & `cset-24.4.1/src/CSET/recipes/meaned_model_level_air_temperature_spatial_plot.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 title: Meaned Model Level Air Temperature Spatial Plot
 description: |
   Extracts out the instantaneous model level air temperature from a file and writes it
   to a new one.
 
-steps:
+parallel:
   - operator: read.read_cubes
     constraint:
       operator: constraints.generate_var_constraint
       varname: air_temperature
 
   - operator: filters.filter_cubes
     constraint:
```

### Comparing `CSET-24.2.1/src/CSET.egg-info/PKG-INFO` & `cset-24.4.1/src/CSET.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSET
-Version: 24.2.1
+Version: 24.4.1
 Summary: Toolkit for evaluation and investigation of numerical models for weather and climate applications.
 Author: Met Office, NIWA
 License: Apache-2.0
 Project-URL: Documentation, https://metoffice.github.io/CSET
 Project-URL: Source, https://github.com/MetOffice/CSET
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -53,15 +53,15 @@
 In addition to reading the working practices, the key
 recommendation is early communication. Open an [issue on
 Github](https://github.com/MetOffice/CSET/issues) with your proposed change or
 addition in the design phase, and then others can provide guidance early.
 
 ## Licence
 
-Copyright © 2022-2023 Met Office and contributors.
+Copyright © 2022-2024 Met Office and contributors.
 
 Licensed under the [Apache License, Version 2.0](LICENCE) (the "License"); You
 may obtain a copy of the License at
 
 <http://www.apache.org/licenses/LICENSE-2.0>
 
 Unless required by applicable law or agreed to in writing, software distributed
```

### Comparing `CSET-24.2.1/src/CSET.egg-info/SOURCES.txt` & `cset-24.4.1/src/CSET.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 LICENCE
 MANIFEST.in
 README.md
 pyproject.toml
 docs/Makefile
+docs/source/changelog.rst
 docs/source/conf.py
 docs/source/index.rst
 docs/source/background/index.rst
 docs/source/background/why-cset.rst
 docs/source/background/why-workflow.rst
 docs/source/contributing/code-review.rst
 docs/source/contributing/documentation.rst
+docs/source/contributing/failing_pr_check.png
 docs/source/contributing/getting-started.rst
 docs/source/contributing/git.rst
 docs/source/contributing/index.rst
+docs/source/contributing/open_pr_symbol.png
 docs/source/contributing/release_page.png
 docs/source/contributing/releases.rst
 docs/source/contributing/testing.rst
 docs/source/getting-started/create-first-recipe.rst
 docs/source/getting-started/index.rst
 docs/source/getting-started/installation.rst
 docs/source/getting-started/recipe-graph-details.svg
@@ -27,16 +30,18 @@
 docs/source/reference/glossary.rst
 docs/source/reference/index.rst
 docs/source/reference/internal.rst
 docs/source/reference/operators.rst
 docs/source/reference/recipe-format.rst
 docs/source/reference/recipe-graph.svg
 docs/source/usage/add-diagnostic.rst
+docs/source/usage/common-errors.rst
 docs/source/usage/index.rst
 docs/source/usage/operator-recipes.rst
+docs/source/usage/rose-edit.png
 docs/source/usage/workflow-installation.rst
 requirements/environment.yml
 requirements/locks/py310-lock-linux-64.txt
 requirements/locks/py311-lock-linux-64.txt
 requirements/locks/py312-lock-linux-64.txt
 requirements/locks/py39-lock-linux-64.txt
 src/CSET/__init__.py
@@ -46,30 +51,40 @@
 src/CSET.egg-info/PKG-INFO
 src/CSET.egg-info/SOURCES.txt
 src/CSET.egg-info/dependency_links.txt
 src/CSET.egg-info/entry_points.txt
 src/CSET.egg-info/requires.txt
 src/CSET.egg-info/top_level.txt
 src/CSET/operators/__init__.py
+src/CSET/operators/_plot_page_template.html
 src/CSET/operators/aggregate.py
 src/CSET/operators/collapse.py
 src/CSET/operators/constraints.py
 src/CSET/operators/convection.py
 src/CSET/operators/filters.py
 src/CSET/operators/misc.py
 src/CSET/operators/plot.py
 src/CSET/operators/read.py
+src/CSET/operators/regrid.py
 src/CSET/operators/write.py
 src/CSET/recipes/CAPE_ratio_plot.yaml
 src/CSET/recipes/__init__.py
 src/CSET/recipes/aggregate_precipitation.yaml
 src/CSET/recipes/extract_instant_air_temp.yaml
+src/CSET/recipes/generic_plevel_spatial_plot_sequence.yaml
+src/CSET/recipes/generic_surface_domain_mean_time_series.yaml
+src/CSET/recipes/generic_surface_spatial_plot_sequence.yaml
 src/CSET/recipes/initial_time-step_surface_air_temperature_ensemble_postage_stamp_plot.yaml
+src/CSET/recipes/lfric_generic_surface_domain_mean_time_series.yaml
+src/CSET/recipes/lfric_generic_surface_spatial_plot_sequence.yaml
 src/CSET/recipes/mean_surface_air_temperature_spatial_plot.yaml
 src/CSET/recipes/meaned_model_level_air_temperature_spatial_plot.yaml
+src/CSET/recipes/stash_surface_domain_mean_time_series.yaml
+src/CSET/recipes/stash_surface_spatial_plot_sequence.yaml
+src/CSET/recipes/surface_air_temperature_spatial_plot_time_sequence.yaml
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_common.py
 tests/test_graph.py
 tests/test_recipes.py
 tests/test_run_recipes.py
@@ -77,21 +92,25 @@
 tests/operators/test_collapse.py
 tests/operators/test_constraints.py
 tests/operators/test_convection.py
 tests/operators/test_filters.py
 tests/operators/test_misc.py
 tests/operators/test_plots.py
 tests/operators/test_read.py
+tests/operators/test_regrid.py
 tests/operators/test_write.py
 tests/test_data/air_temp.nc
 tests/test_data/ensemble_air_temp.yaml
 tests/test_data/exeter_em01.nc
 tests/test_data/exeter_em02.nc
 tests/test_data/exeter_ensemble_single_file.nc
 tests/test_data/noop_recipe.yaml
 tests/test_data/plot_instant_air_temp.yaml
 tests/test_data/plot_instant_air_temp_collapse.yaml
+tests/test_data/template_file.html
 tests/test_data/convection/ECFlagB.nc
 tests/test_data/convection/ECFlagB_2.nc
 tests/test_data/convection/MUCAPE.nc
 tests/test_data/convection/MUCIN.nc
-tests/test_data/convection/SBCAPE.nc
+tests/test_data/convection/SBCAPE.nc
+tests/test_data/regrid/out_rectilinearGeogCS_0p5deg.nc
+tests/test_data/regrid/regrid_rectilinearGeogCS.nc
```

### Comparing `CSET-24.2.1/tests/conftest.py` & `cset-24.4.1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import pytest
 
 
 @pytest.fixture()
 def tmp_working_dir(tmp_path, monkeypatch):
     """Change the working directory for a test."""
     monkeypatch.chdir(tmp_path)
+    return tmp_path
 
 
 @pytest.fixture(scope="session")
 def cubes():
     """Get an iris CubeList."""
     import CSET.operators.read as read
```

### Comparing `CSET-24.2.1/tests/operators/test_aggregate.py` & `cset-24.4.1/tests/operators/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/operators/test_collapse.py` & `cset-24.4.1/tests/operators/test_collapse.py`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/operators/test_constraints.py` & `cset-24.4.1/tests/operators/test_constraints.py`

 * *Files 24% similar despite different names*

```diff
@@ -64,14 +64,41 @@
     )
     assert expected_time_constraint in repr(time_constraint)
     # Try with implicit end
     time_constraint = constraints.generate_time_constraint("2023-03-24T00:00:00+00:00")
     assert expected_time_constraint in repr(time_constraint)
 
 
+def test_generate_pressure_level_constraint_single_level():
+    """Generate constraint for a single pressure level."""
+    pressure_constraint = constraints.generate_pressure_level_constraint(
+        pressure_levels=1000
+    )
+    expected_pressure_constraint = "Constraint(coord_values={'pressure': [1000]})"
+    assert expected_pressure_constraint in repr(pressure_constraint)
+
+
+def test_generate_pressure_level_constraint_multi_level():
+    """Generate constraint for multiple pressure levels."""
+    pressure_constraint = constraints.generate_pressure_level_constraint(
+        pressure_levels=[200, 800]
+    )
+    expected_pressure_constraint = "Constraint(coord_values={'pressure': [200, 800]})"
+    assert expected_pressure_constraint in repr(pressure_constraint)
+
+
+def test_generate_pressure_level_constraint_no_pressure():
+    """Generate constraint for not having pressure levels."""
+    pressure_constraint = constraints.generate_pressure_level_constraint(
+        pressure_levels=[]
+    )
+    expected_pressure_constraint = "Constraint(cube_func=<function generate_pressure_level_constraint.<locals>.no_pressure_coordinate at"
+    assert expected_pressure_constraint in repr(pressure_constraint)
+
+
 def test_combine_constraints():
     """Combine constraint."""
     stash_constraint = constraints.generate_stash_constraint("m01s03i236")
     var_constraint = constraints.generate_var_constraint("test")
     combined_constraint = constraints.combine_constraints(
         stash_constraint,
         a=var_constraint,
```

### Comparing `CSET-24.2.1/tests/operators/test_filters.py` & `cset-24.4.1/tests/operators/test_filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,52 +15,79 @@
 """Test filter operators."""
 
 import iris.cube
 import pytest
 
 from CSET.operators import constraints, filters
 
+constraint_single = constraints.combine_constraints(
+    constraints.generate_stash_constraint("m01s03i236"),
+    a=constraints.generate_cell_methods_constraint([]),
+)
 
-def test_filter_cubes(cubes):
-    """Filter cube and verify."""
+
+def test_filter_cubes_cubelist(cubes):
+    """Test filtering a CubeList."""
     constraint = constraints.generate_cell_methods_constraint([])
-    # Test filtering a CubeList.
     cube = filters.filter_cubes(cubes, constraint)
     assert cube.cell_methods == ()
     expected_cube = "<iris 'Cube' of air_temperature / (K) (time: 3; grid_latitude: 17; grid_longitude: 13)>"
     assert repr(cube) == expected_cube
-    # Test for exception when multiple cubes returned.
+
+
+def test_filter_cubes_cube(cube):
+    """Test filtering a Cube."""
+    constraint = constraints.generate_cell_methods_constraint([])
+    single_cube = filters.filter_cubes(cube, constraint)
+    assert repr(cube) == repr(single_cube)
+
+
+def test_filter_cubes_multiple_returned_exception(cubes):
+    """Test for exception when multiple cubes returned."""
     constraint = constraints.generate_stash_constraint("m01s03i236")
     with pytest.raises(ValueError):
         filters.filter_cubes(cubes, constraint)
-    # Test filtering a Cube.
-    single_cube = filters.filter_cubes(cube, constraint)
-    assert repr(cube) == repr(single_cube)
 
 
-def test_filter_multiple_cubes(cubes):
-    """Filter multiple cubes and verify."""
-    # Test to a CubeList of a single Cube.
-    constraint_single = constraints.combine_constraints(
-        constraints.generate_stash_constraint("m01s03i236"),
-        a=constraints.generate_cell_methods_constraint([]),
+def test_filter_cubes_pressure_coord(cube):
+    """Test a cube without a pressure coordinate is passed through."""
+    pressure_constraint = constraints.generate_pressure_level_constraint(
+        pressure_levels=[]
     )
+    assert filters.filter_cubes(cube, pressure_constraint)
+
+
+def test_filter_cubes_pressure_coord_none_returned(cube):
+    """Test exception when pressure coordinate is excluded."""
+    pressure_constraint = constraints.generate_pressure_level_constraint(
+        pressure_levels=[]
+    )
+    cube = cube.copy()
+    cube.add_aux_coord(iris.coords.DimCoord(100, var_name="pressure"))
+    with pytest.raises(ValueError):
+        filters.filter_cubes(cube, pressure_constraint)
+
+
+def test_filter_multiple_cubes(cubes):
+    """Test to a CubeList of a single Cube."""
     filtered_cubes = filters.filter_multiple_cubes(cubes, c=constraint_single)
     assert isinstance(filtered_cubes, iris.cube.CubeList)
     assert len(filtered_cubes) == 1
     assert filtered_cubes[0].cell_methods == ()
 
-    # Test filtering a Cube.
-    filtered_cube = filters.filter_multiple_cubes(
-        filtered_cubes[0], c=constraint_single
-    )
+
+def test_filter_multiple_cubes_single_cube(cube):
+    """Test filtering a Cube."""
+    filtered_cube = filters.filter_multiple_cubes(cube, c=constraint_single)
     assert isinstance(filtered_cube, iris.cube.CubeList)
     assert len(filtered_cube) == 1
 
-    # Test filtering for multiple Cubes.
+
+def test_filter_multiple_cubes_multiple_out(cubes):
+    """Test filtering for multiple Cubes."""
     constraint_single_2 = constraints.combine_constraints(
         constraints.generate_stash_constraint("m01s03i236"),
         a=constraints.generate_cell_methods_constraint(
             [
                 iris.coords.CellMethod(
                     method="minimum", coords="time", intervals="1 hour"
                 )
@@ -68,20 +95,26 @@
         ),
     )
     filtered_multi_cubes = filters.filter_multiple_cubes(
         cubes, c1=constraint_single, c2=constraint_single_2
     )
     assert len(filtered_multi_cubes) == 2
 
-    # Test exception when no constraints given.
+
+def test_filter_multiple_cubes_no_constraint_exception(cubes):
+    """Test exception when no constraints given."""
     with pytest.raises(ValueError):
         filters.filter_multiple_cubes(cubes)
 
-    # Test exception when multiple cubes returned.
+
+def test_filter_multiple_cubes_returned(cubes):
+    """Test exception when multiple cubes returned."""
     constraint_multiple = constraints.generate_stash_constraint("m01s03i236")
     with pytest.raises(ValueError):
         filters.filter_multiple_cubes(cubes, c=constraint_multiple)
 
-    # Test exception when no Cubes returned.
+
+def test_filter_multiple_cubes_none_returned(cubes):
+    """Test exception when no Cubes returned."""
     constraint_none = constraints.generate_stash_constraint("m01s01i001")
     with pytest.raises(ValueError):
         filters.filter_multiple_cubes(cubes, c=constraint_none)
```

### Comparing `CSET-24.2.1/tests/operators/test_read.py` & `cset-24.4.1/tests/operators/test_read.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,22 @@
         "<iris 'Cube' of air_temperature / (K) (time: 2; grid_latitude: 17; grid_longitude: 13)>",
         "<iris 'Cube' of air_temperature / (K) (time: 3; grid_latitude: 17; grid_longitude: 13)>",
     ]
     for cube in cubes:
         assert repr(cube) in expected_cubes
 
 
+def test_read_cubes_no_cubes_warning():
+    """Warning emitted when constraint gives no cubes."""
+    # TODO: Warning doesn't reach pytest for some reason.
+    # with pytest.warns(Warning, match="No cubes loaded"):
+    cubes = read.read_cubes("tests/test_data/air_temp.nc", "non-existent")
+    assert len(cubes) == 0
+
+
 def test_read_cubes_ensemble_with_realization_coord():
     """Read ensemble data from a single file with a realization dimension."""
     cubes = read.read_cubes("tests/test_data/exeter_ensemble_single_file.nc")
     # Check ensemble members have been merged into a single cube.
     assert len(cubes) == 1
     cube = cubes[0]
     # Check realization is an integer.
```

### Comparing `CSET-24.2.1/tests/operators/test_write.py` & `cset-24.4.1/tests/operators/test_write.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 from CSET.operators import write
 
 
 def test_write_cube(tmp_path: Path, cube):
     """Write cube and verify it was written."""
     file_path = tmp_path / "cube.nc"
-    write.write_cube_to_nc(cube, file_path)
+    write.write_cube_to_nc(cube, file_path, overwrite=True)
     assert file_path.is_file()
 
 
-def test_write_cube_default_filename(tmp_working_dir, cube):
+def test_write_cube_default_filename(cube, tmp_working_dir):
     """Write cube without specifying a filename."""
     Path("meta.json").write_text("{}", encoding="UTF-8")
-    write.write_cube_to_nc(cube)
+    write.write_cube_to_nc(cube, overwrite=True)
     assert Path.cwd().joinpath("untitled.nc").is_file()
```

### Comparing `CSET-24.2.1/tests/test_data/air_temp.nc` & `cset-24.4.1/tests/test_data/air_temp.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/convection/ECFlagB.nc` & `cset-24.4.1/tests/test_data/convection/ECFlagB.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/convection/ECFlagB_2.nc` & `cset-24.4.1/tests/test_data/convection/ECFlagB_2.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/convection/MUCAPE.nc` & `cset-24.4.1/tests/test_data/convection/MUCAPE.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/convection/MUCIN.nc` & `cset-24.4.1/tests/test_data/convection/MUCIN.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/convection/SBCAPE.nc` & `cset-24.4.1/tests/test_data/convection/SBCAPE.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/exeter_em01.nc` & `cset-24.4.1/tests/test_data/exeter_em01.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/exeter_em02.nc` & `cset-24.4.1/tests/test_data/exeter_em02.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/exeter_ensemble_single_file.nc` & `cset-24.4.1/tests/test_data/exeter_ensemble_single_file.nc`

 * *Files identical despite different names*

### Comparing `CSET-24.2.1/tests/test_data/plot_instant_air_temp.yaml` & `cset-24.4.1/tests/test_data/plot_instant_air_temp_collapse.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-name: Extract Instant Air Temperature
+title: Plot average air temperature
 description: |
-  Extracts out the instantaneous 1.5m air temperature from a file and writes it
-  to a new one.
+  Plots the mean 1.5m air temperature over an area.
 
-steps:
+parallel:
   - operator: read.read_cubes
     constraint:
       operator: constraints.generate_stash_constraint
       stash: m01s03i236
 
   - operator: filters.filter_cubes
     constraint:
       operator: constraints.combine_constraints
       stash_constraint:
         operator: constraints.generate_stash_constraint
         stash: m01s03i236
       cell_methods_constraint:
         operator: constraints.generate_cell_methods_constraint
         cell_methods: []
-      time_constraint:
-        operator: constraints.generate_time_constraint
-        time_start: 2022-09-21T03:00:00
-        time_end: 2022-09-21T03:30:00
+
+  - operator: collapse.collapse
+    coordinate: 'time'
+    method: 'MEAN'
+    additional_percent: 90
 
   - operator: write.write_cube_to_nc
-    filename: processed_data.nc
 
   - operator: plot.spatial_contour_plot
-    filename: plot.svg
```

### Comparing `CSET-24.2.1/tests/test_data/plot_instant_air_temp_collapse.yaml` & `cset-24.4.1/tests/test_data/plot_instant_air_temp.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-name: Plot average air temperature
+title: Extract Instant Air Temperature
 description: |
-  Plots the mean 1.5m air temperature over an area.
+  Extracts out the instantaneous 1.5m air temperature from a file and writes it
+  to a new one.
 
-steps:
+parallel:
   - operator: read.read_cubes
     constraint:
       operator: constraints.generate_stash_constraint
       stash: m01s03i236
 
   - operator: filters.filter_cubes
     constraint:
       operator: constraints.combine_constraints
       stash_constraint:
         operator: constraints.generate_stash_constraint
         stash: m01s03i236
       cell_methods_constraint:
         operator: constraints.generate_cell_methods_constraint
         cell_methods: []
-
-  - operator: collapse.collapse
-    coordinate: 'time'
-    method: 'MEAN'
-    additional_percent: 90
+      time_constraint:
+        operator: constraints.generate_time_constraint
+        time_start: 2022-09-21T03:00:00Z
+        time_end: 2022-09-21T03:30:00Z
 
   - operator: write.write_cube_to_nc
+    filename: processed_data.nc
 
   - operator: plot.spatial_contour_plot
+    filename: plot.png
```

### Comparing `CSET-24.2.1/tests/test_graph.py` & `cset-24.4.1/tests/test_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     )
 
 
 def test_save_graph_no_operators_exception():
     """Exception raised from recipe with no operators."""
     with pytest.raises(ValueError):
         # Inline YAML form used.
-        graph.save_graph('{"steps": [{"argument": "no_operators"}]}')
+        graph.save_graph('{"parallel": [{"argument": "no_operators"}]}')
 
 
 def test_save_graph_auto_open_xdg_open(tmp_path: Path, monkeypatch):
     """Test the auto-opening of the graph with (a mocked) xdg-open."""
     xdg_open = tmp_path / "xdg-open"
     with open(xdg_open, "wt", encoding="UTF-8") as fp:
         fp.write("#!/bin/bash\ntrue")
```

### Comparing `CSET-24.2.1/tests/test_run_recipes.py` & `cset-24.4.1/tests/test_recipes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,73 @@
-# Copyright 2022 Met Office and contributors.
+# Copyright 2023 Met Office and contributors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for running CSET operator recipes."""
+"""Recipe tests."""
 
 from pathlib import Path
-from uuid import uuid4
 
 import pytest
 
-import CSET.operators
+import CSET.recipes
 
 
-def test_get_operator():
-    """Happy case."""
-    read_operator = CSET.operators.get_operator("read.read_cubes")
-    assert callable(read_operator)
+def test_recipe_files_in_tree():
+    """Get recipes in directory containing sub-directories."""
+    files = list(CSET.recipes._recipe_files_in_tree(input_dir=Path("tests")))
+    assert Path("tests/test_data/noop_recipe.yaml") in files
 
 
-def test_get_operator_exception_missing():
-    """Test exception for non-existent operators."""
-    with pytest.raises(ValueError):
-        CSET.operators.get_operator("non-existent.operator")
+def test_unpack(tmp_path: Path):
+    """Unpack recipes."""
+    CSET.recipes.unpack_recipe(tmp_path, "extract_instant_air_temp.yaml")
+    assert (tmp_path / "extract_instant_air_temp.yaml").is_file()
+    # Unpack everything and check a warning is produced when files collide.
+    with pytest.warns():
+        CSET.recipes.unpack_recipe(tmp_path, "extract_instant_air_temp.yaml")
 
 
-def test_get_operator_exception_type():
-    """Test exception if wrong type provided."""
-    with pytest.raises(ValueError):
-        CSET.operators.get_operator(["Not", b"a", "string", 1])
+def test_unpack_recipes_exception_collision(tmp_path: Path):
+    """Output path already exists and is not a directory."""
+    file_path = tmp_path / "regular_file"
+    file_path.touch()
+    with pytest.raises(FileExistsError):
+        CSET.recipes.unpack_recipe(file_path, "extract_instant_air_temp.yaml")
 
 
-def test_get_operator_exception_not_callable():
-    """Test exception if operator isn't a function."""
-    with pytest.raises(ValueError):
-        CSET.operators.get_operator("misc.__doc__")
+def test_unpack_recipes_exception_permission():
+    """Insufficient permission to create output directory.
 
+    Will fail if tests are run as root, but no one should do that, right?
+    """
+    with pytest.raises(OSError):
+        CSET.recipes.unpack_recipe(
+            Path("/usr/bin/cset"), "extract_instant_air_temp.yaml"
+        )
 
-def test_execute_recipe(tmp_path: Path):
-    """Execute recipe to test happy case (this is really an integration test)."""
-    input_file = Path("tests/test_data/air_temp.nc")
-    output_dir = tmp_path / f"{uuid4()}"
-    recipe_file = Path("tests/test_data/plot_instant_air_temp.yaml")
-    CSET.operators.execute_recipe(recipe_file, input_file, output_dir)
 
+def test_get_recipe_file():
+    """Get a recipe file from a specific location."""
+    file = CSET.recipes._get_recipe_file("noop_recipe.yaml", Path("tests/test_data"))
+    assert file.is_file()
 
-def test_execute_recipe_edge_cases(tmp_path: Path):
-    """Test weird edge cases. Also tests data paths not being pathlib Paths."""
-    input_file = "tests/test_data/air_temp.nc"
-    output_dir = tmp_path / f"{uuid4()}"
-    recipe = Path("tests/test_data/noop_recipe.yaml")
-    CSET.operators.execute_recipe(recipe, input_file, output_dir)
 
+def test_get_recipe_file_missing():
+    """Exception raised when recipe file not in location."""
+    with pytest.raises(FileNotFoundError):
+        CSET.recipes._get_recipe_file("non-existent", Path("tests/test_data"))
 
-def test_execute_recipe_invalid_output_dir(tmp_path: Path):
-    """Exception raised if output directory can't be created."""
-    recipe = '{"steps":[{"operator": misc.noop}]}'
-    input_file = Path("tests/test_data/air_temp.nc")
-    output_dir = tmp_path / "actually_a_file"
-    output_dir.touch()
-    with pytest.raises(FileExistsError):
-        CSET.operators.execute_recipe(recipe, input_file, output_dir)
+
+def test_get_recipe_file_in_package():
+    """Get a recipe file from a the default location inside the package."""
+    file = CSET.recipes._get_recipe_file("CAPE_ratio_plot.yaml")
+    assert file.is_file()
```

