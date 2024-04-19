# Comparing `tmp/fmu-sumo-1.2.1.tar.gz` & `tmp/fmu_sumo-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmu-sumo-1.2.1.tar", last modified: Wed Apr 10 09:04:44 2024, max compression
+gzip compressed data, was "fmu_sumo-1.2.2.tar", last modified: Fri Apr 19 10:06:13 2024, max compression
```

## Comparing `fmu-sumo-1.2.1.tar` & `fmu_sumo-1.2.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.244065 fmu-sumo-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.244065 fmu-sumo-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/build_docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_no_access_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.244065 fmu-sumo-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor-logo2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    25380 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor_logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor_logo_only.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_templates/layout.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2058 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/explorer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/examples/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/examples/tables.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.240065 fmu-sumo-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/sumo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/sumo/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/realization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.252065 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_aggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/timefilter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.252065 fmu-sumo-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.240065 fmu-sumo-1.2.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.252065 fmu-sumo-1.2.1/tests/data/test_case_080/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/data/test_case_080/case2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/tests/test_access/
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_manage_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_read_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_write_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_no_access_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_objects_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.864165 fmu_sumo-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.848165 fmu_sumo-1.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.852165 fmu_sumo-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/build_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_manage_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_read_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_write_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.github/workflows/run_tests_access_no_access_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-19 10:06:13.864165 fmu_sumo-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.852165 fmu_sumo-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.852165 fmu_sumo-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/_static/equinor-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/_static/equinor-logo2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25380 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/_static/equinor_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/_static/equinor_logo_only.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.852165 fmu_sumo-1.2.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/_templates/layout.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2058 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/explorer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.852165 fmu_sumo-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/examples/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/examples/tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:06:13.864165 fmu_sumo-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.848165 fmu_sumo-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.852165 fmu_sumo-1.2.2/src/fmu/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.852165 fmu_sumo-1.2.2/src/fmu/sumo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.856165 fmu_sumo-1.2.2/src/fmu/sumo/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 10:06:13.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.856165 fmu_sumo-1.2.2/src/fmu/sumo/explorer/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/contexts/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/contexts/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/contexts/realization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.860164 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_child_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_document_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/case_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/cube_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/dictionary_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/polygons_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/surface_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/table_aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/table_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/src/fmu/sumo/explorer/timefilter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.860164 fmu_sumo-1.2.2/src/fmu_sumo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-19 10:06:13.000000 fmu_sumo-1.2.2/src/fmu_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-19 10:06:13.000000 fmu_sumo-1.2.2/src/fmu_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:06:13.000000 fmu_sumo-1.2.2/src/fmu_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 10:06:13.000000 fmu_sumo-1.2.2/src/fmu_sumo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 10:06:13.000000 fmu_sumo-1.2.2/src/fmu_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.860164 fmu_sumo-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.848165 fmu_sumo-1.2.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.860164 fmu_sumo-1.2.2/tests/data/test_case_080/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/data/test_case_080/case2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:06:13.860164 fmu_sumo-1.2.2/tests/test_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/test_access/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/test_access/tst_access_drogon_manage_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/test_access/tst_access_drogon_read_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/test_access/tst_access_drogon_write_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/test_access/tst_access_no_access_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-19 10:06:09.000000 fmu_sumo-1.2.2/tests/test_objects_table.py
```

### Comparing `fmu-sumo-1.2.1/.github/pull_request_template.md` & `fmu_sumo-1.2.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/build_docs.yaml` & `fmu_sumo-1.2.2/.github/workflows/build_docs.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/publish_release.yaml` & `fmu_sumo-1.2.2/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_login.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_manage_login.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_login.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests_access_no_access_login.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-name: Test access DROGON-READ login
+name: Test access NO-ACCESS login
 
 on:
   pull_request:
     branches: [main]
   schedule:
-    - cron: "24 4 * * *"
+    - cron: "54 4 * * *"
   workflow_dispatch:
 
 jobs:
   build_pywheels:
     name: PY ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
@@ -21,15 +21,15 @@
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Azure Login
         uses: Azure/login@v2
         with:
-          client-id: 121279f7-331a-45fd-9a5f-62d9026694a7
+          client-id: fea86a50-0f48-4cef-ba4d-1d789a00b701
           tenant-id: 3aa4a235-b6e2-48d5-9195-7fcf05b459b0
           allow-no-subscriptions: true
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
@@ -43,9 +43,9 @@
         run: |
           az --version
           az account list
           pip list | grep -i sumo
           access_token=$(az account get-access-token --scope api://88d2b022-3539-4dda-9e66-853801334a86/.default --query accessToken --output tsv)
           export ACCESS_TOKEN=$access_token
 
-          pytest -s --timeout=300 tests/test_access/tst_access_drogon_read_login.py
+          pytest -s --timeout=300 tests/test_access/tst_access_no_access_login.py
```

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_login.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_read_login.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-name: Test access DROGON-WRITE login
+name: Test access DROGON-READ login
 
 on:
   pull_request:
     branches: [main]
   schedule:
-    - cron: "34 4 * * *"
+    - cron: "58 4 * * *"
   workflow_dispatch:
 
 jobs:
   build_pywheels:
     name: PY ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
@@ -21,15 +21,15 @@
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Azure Login
         uses: Azure/login@v2
         with:
-          client-id: 556cac03-e416-4ed6-86d7-d9d3f965d72e
+          client-id: 121279f7-331a-45fd-9a5f-62d9026694a7
           tenant-id: 3aa4a235-b6e2-48d5-9195-7fcf05b459b0
           allow-no-subscriptions: true
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
@@ -43,9 +43,9 @@
         run: |
           az --version
           az account list
           pip list | grep -i sumo
           access_token=$(az account get-access-token --scope api://88d2b022-3539-4dda-9e66-853801334a86/.default --query accessToken --output tsv)
           export ACCESS_TOKEN=$access_token
 
-          pytest -s --timeout=300 tests/test_access/tst_access_drogon_write_login.py
+          pytest -s --timeout=300 tests/test_access/tst_access_drogon_read_login.py
```

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/.github/workflows/run_tests_access_no_access_login.yaml` & `fmu_sumo-1.2.2/.github/workflows/run_tests_access_drogon_write_login.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-name: Test access NO-ACCESS login
+name: Test access DROGON-WRITE login
 
 on:
   pull_request:
     branches: [main]
   schedule:
-    - cron: "54 4 * * *"
+    - cron: "56 4 * * *"
   workflow_dispatch:
 
 jobs:
   build_pywheels:
     name: PY ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
@@ -21,15 +21,15 @@
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Azure Login
         uses: Azure/login@v2
         with:
-          client-id: fea86a50-0f48-4cef-ba4d-1d789a00b701
+          client-id: 556cac03-e416-4ed6-86d7-d9d3f965d72e
           tenant-id: 3aa4a235-b6e2-48d5-9195-7fcf05b459b0
           allow-no-subscriptions: true
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
@@ -43,9 +43,9 @@
         run: |
           az --version
           az account list
           pip list | grep -i sumo
           access_token=$(az account get-access-token --scope api://88d2b022-3539-4dda-9e66-853801334a86/.default --query accessToken --output tsv)
           export ACCESS_TOKEN=$access_token
 
-          pytest -s --timeout=300 tests/test_access/tst_access_no_access_login.py
+          pytest -s --timeout=300 tests/test_access/tst_access_drogon_write_login.py
```

### Comparing `fmu-sumo-1.2.1/.gitignore` & `fmu_sumo-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/CONTRIBUTING.md` & `fmu_sumo-1.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/LICENSE` & `fmu_sumo-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/PKG-INFO` & `fmu_sumo-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu-sumo
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python package for interacting with Sumo in an FMU setting
 Author: Equinor
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fmu-sumo-1.2.1/SECURITY.md` & `fmu_sumo-1.2.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/docs/_static/equinor-logo.png` & `fmu_sumo-1.2.2/docs/_static/equinor-logo.png`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/docs/_static/equinor-logo2.jpg` & `fmu_sumo-1.2.2/docs/_static/equinor-logo2.jpg`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/docs/_static/equinor_logo.jpg` & `fmu_sumo-1.2.2/docs/_static/equinor_logo.jpg`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/docs/_static/equinor_logo_only.jpg` & `fmu_sumo-1.2.2/docs/_static/equinor_logo_only.jpg`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/docs/conf.py` & `fmu_sumo-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/docs/explorer.rst` & `fmu_sumo-1.2.2/docs/explorer.rst`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/docs/index.rst` & `fmu_sumo-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/examples/explorer.ipynb` & `fmu_sumo-1.2.2/examples/explorer.ipynb`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/examples/tables.ipynb` & `fmu_sumo-1.2.2/examples/tables.ipynb`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/pyproject.toml` & `fmu_sumo-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/_utils.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/_utils.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/aggregation.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/contexts/aggregation.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/observation.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/contexts/observation.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/realization.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/contexts/realization.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/explorer.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/__init__.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_child.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_child_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_document.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/_document_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/case.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/case_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/cube.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/cube_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/dictionary.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/dictionary_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/polygons.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/polygons_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/surface.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/surface_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/table.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_aggregated.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/table_aggregated.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_collection.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/objects/table_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/pit.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/pit.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu/sumo/explorer/timefilter.py` & `fmu_sumo-1.2.2/src/fmu/sumo/explorer/timefilter.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/src/fmu_sumo.egg-info/PKG-INFO` & `fmu_sumo-1.2.2/src/fmu_sumo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu-sumo
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python package for interacting with Sumo in an FMU setting
 Author: Equinor
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fmu-sumo-1.2.1/src/fmu_sumo.egg-info/SOURCES.txt` & `fmu_sumo-1.2.2/src/fmu_sumo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/context.py` & `fmu_sumo-1.2.2/tests/context.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/data/test_case_080/case2.json` & `fmu_sumo-1.2.2/tests/data/test_case_080/case2.json`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/test_access/README.md` & `fmu_sumo-1.2.2/tests/test_access/README.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_manage_login.py` & `fmu_sumo-1.2.2/tests/test_access/tst_access_drogon_manage_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_read_login.py` & `fmu_sumo-1.2.2/tests/test_access/tst_access_drogon_read_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_write_login.py` & `fmu_sumo-1.2.2/tests/test_access/tst_access_drogon_write_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/test_access/tst_access_no_access_login.py` & `fmu_sumo-1.2.2/tests/test_access/tst_access_no_access_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/test_explorer.py` & `fmu_sumo-1.2.2/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.1/tests/test_objects_table.py` & `fmu_sumo-1.2.2/tests/test_objects_table.py`

 * *Files identical despite different names*

