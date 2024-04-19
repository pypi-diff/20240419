# Comparing `tmp/asf_search-7.0.9.tar.gz` & `tmp/asf_search-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asf_search-7.0.9.tar", last modified: Thu Apr 11 17:08:06 2024, max compression
+gzip compressed data, was "asf_search-7.1.0.tar", last modified: Fri Apr 19 17:32:55 2024, max compression
```

## Comparing `asf_search-7.0.9.tar` & `asf_search-7.1.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.389361 asf_search-7.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 17:08:00.000000 asf_search-7.0.9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.357362 asf_search-7.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.361362 asf_search-7.0.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.361362 asf_search-7.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/workflows/prod-request-merged.yml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-11 17:08:00.000000 asf_search-7.0.9/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-11 17:08:00.000000 asf_search-7.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    28585 2024-04-11 17:08:00.000000 asf_search-7.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-11 17:08:00.000000 asf_search-7.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-11 17:08:06.389361 asf_search-7.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-11 17:08:00.000000 asf_search-7.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.361362 asf_search-7.0.9/asf_search/
--rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.365362 asf_search-7.0.9/asf_search/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFSearchOptions/ASFSearchOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFSearchOptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFSearchOptions/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFSearchOptions/validator_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFSearchOptions/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFSession.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/ASFStackableProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.365362 asf_search-7.0.9/asf_search/CMR/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/CMR/MissionList.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/CMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/CMR/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/CMR/field_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/CMR/subquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/CMR/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.369362 asf_search-7.0.9/asf_search/Products/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/AIRSARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/ALOSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/ARIAS1GUNWProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/ERSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/JERSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/NISARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/OPERAS1Product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/RADARSATProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/S1BurstProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/S1Product.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/SEASATProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/SIRCProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/SMAPProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/UAVSARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/Products/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.369362 asf_search-7.0.9/asf_search/WKT/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/WKT/RepairEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/WKT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/WKT/validate_wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.369362 asf_search-7.0.9/asf_search/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/baseline/calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/baseline/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.369362 asf_search-7.0.9/asf_search/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/BEAMMODE.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/DATASET.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/FLIGHT_DIRECTION.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/INSTRUMENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/INTERNAL.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/PLATFORM.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/POLARIZATION.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/PRODUCT_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.369362 asf_search-7.0.9/asf_search/download/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/download/file_download_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.373362 asf_search-7.0.9/asf_search/export/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/export_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/jsonlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/jsonlite2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/kml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/export/metalink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.373362 asf_search-7.0.9/asf_search/health/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/health/health.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.373362 asf_search-7.0.9/asf_search/search/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/baseline_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/geo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/granule_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/product_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/search_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-11 17:08:00.000000 asf_search-7.0.9/asf_search/search/search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.389361 asf_search-7.0.9/asf_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-11 17:08:06.000000 asf_search-7.0.9/asf_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-11 17:08:06.000000 asf_search-7.0.9/asf_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:08:06.000000 asf_search-7.0.9/asf_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-11 17:08:06.000000 asf_search-7.0.9/asf_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 17:08:06.000000 asf_search-7.0.9/asf_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.373362 asf_search-7.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/0-Intro.md
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/1-Basic_Overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/2-Geographic_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/3-Granule_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/4-Baseline_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/5-Download.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/6-Outro.md
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-11 17:08:00.000000 asf_search-7.0.9/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-11 17:08:00.000000 asf_search-7.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:08:06.389361 asf_search-7.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-11 17:08:00.000000 asf_search-7.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/ASFProduct/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/ASFProduct/test_ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/ASFSearchOptions/test_ASFSearchOptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/ASFSearchResults/
--rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/ASFSearchResults/test_ASFSearchResults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/ASFSession/
--rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/ASFSession/test_ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/BaselineSearch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/BaselineSearch/Stack/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/BaselineSearch/Stack/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/BaselineSearch/test_baseline_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/CMR/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/CMR/test_MissionList.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/Search/
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/Search/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/Search/test_search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/Serialization/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/Serialization/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/WKT/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/WKT/test_validate_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.377362 asf_search-7.0.9/tests/download/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/download/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/pytest-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/pytest-managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.381362 asf_search-7.0.9/tests/yml_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:08:06.389361 asf_search-7.0.9/tests/yml_tests/Resources/
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Alos_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Alos_response_maxResults3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_L1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (127)    48181 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46473 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.kml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.metalink
--rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
--rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
--rw-r--r--   0 runner    (1001) docker     (127)    52821 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (127)    53132 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/JERS.yml
--rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/JERS_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    63985 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/OPERA_Products.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/RADARSAT.yml
--rw-r--r--   0 runner    (1001) docker     (127)   308082 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/RADARSAT_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)   376802 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
--rw-r--r--   0 runner    (1001) docker     (127)    38828 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/S1_baseline_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/S1_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18407 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/SLC_BURST.yml
--rw-r--r--   0 runner    (1001) docker     (127)  1807159 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/SLC_BURST_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/SMAP_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)   600436 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/ShorelineMask26.shp
--rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_ASFProduct.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_ASFSearchOptions.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22399 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_ASFSearchResults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_ASFSession.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_baseline_search.yml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_campaigns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_download.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_known_bugs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_notebooks.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_search.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_search_generator.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_serialization.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    30725 2024-04-11 17:08:00.000000 asf_search-7.0.9/tests/yml_tests/test_validate_wkt.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.625616 asf_search-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 17:32:51.000000 asf_search-7.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.589616 asf_search-7.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.593616 asf_search-7.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.593616 asf_search-7.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/prod-request-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-19 17:32:51.000000 asf_search-7.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-19 17:32:51.000000 asf_search-7.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-19 17:32:51.000000 asf_search-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-19 17:32:55.625616 asf_search-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-19 17:32:51.000000 asf_search-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.597616 asf_search-7.1.0/asf_search/
+-rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.597616 asf_search-7.1.0/asf_search/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/ASFSearchOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/validator_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFStackableProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.597616 asf_search-7.1.0/asf_search/CMR/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/MissionList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/field_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.601616 asf_search-7.1.0/asf_search/Products/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/AIRSARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/ALOSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/ARIAS1GUNWProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/ERSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/JERSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/NISARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/OPERAS1Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/RADARSATProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/S1BurstProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/S1Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/SEASATProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/SIRCProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/SMAPProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/UAVSARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.601616 asf_search-7.1.0/asf_search/WKT/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/WKT/RepairEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/WKT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/WKT/validate_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.601616 asf_search-7.1.0/asf_search/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/baseline/calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/baseline/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/BEAMMODE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/DATASET.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/FLIGHT_DIRECTION.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/INSTRUMENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/INTERNAL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/PLATFORM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/POLARIZATION.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/PRODUCT_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/download/file_download_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/export_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/jsonlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/jsonlite2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/kml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/metalink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/health/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/health/health.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/baseline_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/geo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/granule_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/product_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/search_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.621616 asf_search-7.1.0/asf_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/0-Intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/1-Basic_Overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/2-Geographic_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/3-Granule_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/4-Baseline_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/5-Download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/6-Outro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 17:32:51.000000 asf_search-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:32:55.625616 asf_search-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-19 17:32:51.000000 asf_search-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFProduct/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFProduct/test_ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFSearchOptions/test_ASFSearchOptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFSearchResults/
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFSearchResults/test_ASFSearchResults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFSession/
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFSession/test_ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/BaselineSearch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/BaselineSearch/Stack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/BaselineSearch/Stack/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/BaselineSearch/test_baseline_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/CMR/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/CMR/test_MissionList.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/Search/
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/Search/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/Search/test_search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/Serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/WKT/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/WKT/test_validate_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/download/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/download/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/pytest-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/pytest-managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.613616 asf_search-7.1.0/tests/yml_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.621616 asf_search-7.1.0/tests/yml_tests/Resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Alos_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_L1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    48181 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46473 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.kml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    52821 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    53132 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/JERS.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/JERS_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    63985 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/OPERA_Products.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   308082 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   376802 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    38828 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/S1_baseline_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/S1_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18407 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST.yml
+-rw-r--r--   0 runner    (1001) docker     (127)  1807159 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/SMAP_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   600436 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/ShorelineMask26.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFProduct.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFSearchOptions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22399 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFSearchResults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFSession.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_baseline_search.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_campaigns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_download.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_known_bugs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_notebooks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_search.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_search_generator.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_serialization.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    30725 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_validate_wkt.yml
```

### Comparing `asf_search-7.0.9/.github/ISSUE_TEMPLATE/bug_report.md` & `asf_search-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/.github/ISSUE_TEMPLATE/feature_request.md` & `asf_search-7.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/.github/workflows/prod-request-merged.yml` & `asf_search-7.1.0/.github/workflows/prod-request-merged.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/.github/workflows/pypi-publish.yml` & `asf_search-7.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/.github/workflows/run-pytest.yml` & `asf_search-7.1.0/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/.gitignore` & `asf_search-7.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/CHANGELOG.md` & `asf_search-7.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,26 @@
 - 
 
 ### Removed:
 -
 
 -->
 ------
-## [v7.0.9](https://github.com/asfadmin/Discovery-asf_search/compare/v7.0.8...v7.0.9)
+## [v7.1.0](https://github.com/asfadmin/Discovery-asf_search/compare/v7.0.9...v7.1.0)
 ### Added
+- Improved logging in `ASFSession` authentication methods
+
+### Changed
+- Uses `ciso8601` module for parsing dates from CMR response, significant performance improvement post-query
+- `ASFSession` now allows for authorized user access to hidden/restricted CMR datasets via `auth_with_creds()` or `auth_with_cookiejar()` authentication methods (previously only supported via `auth_with_token()` method)
+- `ASFSession.auth_with_token()` now authenticates directly against EDL endpoint
+
+------
+## [v7.0.9](https://github.com/asfadmin/Discovery-asf_search/compare/v7.0.8...v7.0.9)
+### Changed
 - collection "ARIA_S1_GUNW" added to `ARIA_S1_GUNW` dataset, V3 products now loaded as `ARIAS1GUNWProduct` subclass
 - `ARIAS1GUNWProduct` now exposes `ariaVersion` and (for V3 products) `inputGranules` in `ARIAS1GUNWProduct.properties`
 
 ------
 ## [v7.0.8](https://github.com/asfadmin/Discovery-asf_search/compare/v7.0.7...v7.0.8)
 ### Added
 - `s3Urls` property added to `S1Product`, `OPERAS1Product`, and `NISARProduct` types, exposing direct access S3 links
```

### Comparing `asf_search-7.0.9/LICENSE` & `asf_search-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/PKG-INFO` & `asf_search-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 7.0.9
+Version: 7.1.0
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -28,14 +28,15 @@
 Requires-Dist: shapely
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: importlib_metadata
 Requires-Dist: numpy
 Requires-Dist: dateparser
 Requires-Dist: tenacity==8.2.2
+Requires-Dist: ciso8601
 Provides-Extra: test
 Requires-Dist: pytest<7.2.0; extra == "test"
 Requires-Dist: pytest-automation; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
```

### Comparing `asf_search-7.0.9/README.md` & `asf_search-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/ASFProduct.py` & `asf_search-7.1.0/asf_search/ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/ASFSearchOptions/ASFSearchOptions.py` & `asf_search-7.1.0/asf_search/ASFSearchOptions/ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/ASFSearchOptions/validator_map.py` & `asf_search-7.1.0/asf_search/ASFSearchOptions/validator_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/ASFSearchOptions/validators.py` & `asf_search-7.1.0/asf_search/ASFSearchOptions/validators.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/ASFSearchResults.py` & `asf_search-7.1.0/asf_search/ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/ASFStackableProduct.py` & `asf_search-7.1.0/asf_search/ASFStackableProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/CMR/MissionList.py` & `asf_search-7.1.0/asf_search/CMR/MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/CMR/datasets.py` & `asf_search-7.1.0/asf_search/CMR/datasets.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/CMR/field_map.py` & `asf_search-7.1.0/asf_search/CMR/field_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/CMR/subquery.py` & `asf_search-7.1.0/asf_search/CMR/subquery.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/CMR/translate.py` & `asf_search-7.1.0/asf_search/CMR/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from asf_search.constants import CMR_PAGE_SIZE
 import re
 from shapely import wkt
 from shapely.geometry import Polygon
 from shapely.geometry.base import BaseGeometry
 from .field_map import field_map
 from .datasets import collections_per_platform
-import dateparser
+import ciso8601
 import logging
 
 
 def translate_opts(opts: ASFSearchOptions) -> List:
     # Need to add params which ASFSearchOptions cant support (like temporal),
     # so use a dict to avoid the validate_params logic:
     dict_opts = dict(opts)
@@ -153,16 +153,19 @@
     
     return float(value)
 
 def try_parse_date(value: str) -> Optional[str]:
     if value is None:
         return None
 
-    date = dateparser.parse(value)
-
+    try:
+        date = ciso8601.parse_datetime(value)
+    except ValueError:
+        return None
+    
     if date is None:
         return value
 
     if date.tzinfo is None:
         date = date.replace(tzinfo=timezone.utc)
         # Turn all inputs into a consistant format:
```

### Comparing `asf_search-7.0.9/asf_search/Products/AIRSARProduct.py` & `asf_search-7.1.0/asf_search/Products/AIRSARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/ALOSProduct.py` & `asf_search-7.1.0/asf_search/Products/ALOSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/ARIAS1GUNWProduct.py` & `asf_search-7.1.0/asf_search/Products/ARIAS1GUNWProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/ERSProduct.py` & `asf_search-7.1.0/asf_search/Products/ERSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/JERSProduct.py` & `asf_search-7.1.0/asf_search/Products/JERSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/NISARProduct.py` & `asf_search-7.1.0/asf_search/Products/NISARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/OPERAS1Product.py` & `asf_search-7.1.0/asf_search/Products/OPERAS1Product.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/RADARSATProduct.py` & `asf_search-7.1.0/asf_search/Products/RADARSATProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/S1BurstProduct.py` & `asf_search-7.1.0/asf_search/Products/S1BurstProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/S1Product.py` & `asf_search-7.1.0/asf_search/Products/S1Product.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/SEASATProduct.py` & `asf_search-7.1.0/asf_search/Products/SEASATProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/SIRCProduct.py` & `asf_search-7.1.0/asf_search/Products/SIRCProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/SMAPProduct.py` & `asf_search-7.1.0/asf_search/Products/SMAPProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/UAVSARProduct.py` & `asf_search-7.1.0/asf_search/Products/UAVSARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/Products/__init__.py` & `asf_search-7.1.0/asf_search/Products/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/WKT/validate_wkt.py` & `asf_search-7.1.0/asf_search/WKT/validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/__init__.py` & `asf_search-7.1.0/asf_search/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/baseline/calc.py` & `asf_search-7.1.0/asf_search/baseline/calc.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/baseline/stack.py` & `asf_search-7.1.0/asf_search/baseline/stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/constants/BEAMMODE.py` & `asf_search-7.1.0/asf_search/constants/BEAMMODE.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/constants/INTERNAL.py` & `asf_search-7.1.0/asf_search/constants/INTERNAL.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/constants/PRODUCT_TYPE.py` & `asf_search-7.1.0/asf_search/constants/PRODUCT_TYPE.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/download/download.py` & `asf_search-7.1.0/asf_search/download/download.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/exceptions.py` & `asf_search-7.1.0/asf_search/exceptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/export/csv.py` & `asf_search-7.1.0/asf_search/export/csv.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/export/export_translators.py` & `asf_search-7.1.0/asf_search/export/export_translators.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/export/geojson.py` & `asf_search-7.1.0/asf_search/export/geojson.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/export/jsonlite.py` & `asf_search-7.1.0/asf_search/export/jsonlite.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/export/jsonlite2.py` & `asf_search-7.1.0/asf_search/export/jsonlite2.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/export/kml.py` & `asf_search-7.1.0/asf_search/export/kml.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/export/metalink.py` & `asf_search-7.1.0/asf_search/export/metalink.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/health/health.py` & `asf_search-7.1.0/asf_search/health/health.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/baseline_search.py` & `asf_search-7.1.0/asf_search/search/baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/campaigns.py` & `asf_search-7.1.0/asf_search/search/campaigns.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/error_reporting.py` & `asf_search-7.1.0/asf_search/search/error_reporting.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/geo_search.py` & `asf_search-7.1.0/asf_search/search/geo_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/granule_search.py` & `asf_search-7.1.0/asf_search/search/granule_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/product_search.py` & `asf_search-7.1.0/asf_search/search/product_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/search.py` & `asf_search-7.1.0/asf_search/search/search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/search_count.py` & `asf_search-7.1.0/asf_search/search/search_count.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search/search/search_generator.py` & `asf_search-7.1.0/asf_search/search/search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/asf_search.egg-info/PKG-INFO` & `asf_search-7.1.0/asf_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 7.0.9
+Version: 7.1.0
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -28,14 +28,15 @@
 Requires-Dist: shapely
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: importlib_metadata
 Requires-Dist: numpy
 Requires-Dist: dateparser
 Requires-Dist: tenacity==8.2.2
+Requires-Dist: ciso8601
 Provides-Extra: test
 Requires-Dist: pytest<7.2.0; extra == "test"
 Requires-Dist: pytest-automation; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
```

### Comparing `asf_search-7.0.9/asf_search.egg-info/SOURCES.txt` & `asf_search-7.1.0/asf_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/0-Intro.md` & `asf_search-7.1.0/examples/0-Intro.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/1-Basic_Overview.ipynb` & `asf_search-7.1.0/examples/1-Basic_Overview.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/2-Geographic_Search.ipynb` & `asf_search-7.1.0/examples/2-Geographic_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/3-Granule_Search.ipynb` & `asf_search-7.1.0/examples/3-Granule_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/4-Baseline_Search.ipynb` & `asf_search-7.1.0/examples/4-Baseline_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/5-Download.ipynb` & `asf_search-7.1.0/examples/5-Download.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/6-Outro.md` & `asf_search-7.1.0/examples/6-Outro.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb` & `asf_search-7.1.0/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/examples/hello_world.py` & `asf_search-7.1.0/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/setup.py` & `asf_search-7.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     "requests",
     "shapely",
     "python-dateutil",
     "pytz",
     "importlib_metadata",
     "numpy",
     "dateparser",
-    "tenacity == 8.2.2"
+    "tenacity == 8.2.2",
+    "ciso8601"
 ]
 
 test_requirements = [
     "pytest < 7.2.0",
     "pytest-automation",
     "pytest-cov",
     "pytest-xdist",
```

### Comparing `asf_search-7.0.9/tests/ASFProduct/test_ASFProduct.py` & `asf_search-7.1.0/tests/ASFProduct/test_ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/ASFSearchOptions/test_ASFSearchOptions.py` & `asf_search-7.1.0/tests/ASFSearchOptions/test_ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/ASFSearchResults/test_ASFSearchResults.py` & `asf_search-7.1.0/tests/ASFSearchResults/test_ASFSearchResults.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Dict, List
 
-import dateparser
 import asf_search as asf
 from asf_search import ASFSearchResults
 import defusedxml.ElementTree as DefusedETree
 import xml.etree.ElementTree as ETree
 import json
 import shapely.wkt as WKT
 import requests
```

### Comparing `asf_search-7.0.9/tests/ASFSession/test_ASFSession.py` & `asf_search-7.1.0/tests/ASFSession/test_ASFSession.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,42 +12,47 @@
 def run_auth_with_creds(username: str, password: str):
     session = ASFSession()
     session.auth_with_creds(username=username, password=password)
 
 def run_auth_with_token(token: str):
     session = ASFSession()
 
-    with patch('asf_search.ASFSession.get') as mock_token_session:
+    with patch('asf_search.ASFSession.post') as mock_token_session:
         if not token.startswith('Bearer EDL'):
                 mock_token_session.return_value.status_code = 400
                 session.auth_with_token(token)
 
         mock_token_session.return_value.status_code = 200
         session.auth_with_token(token)
 
 def run_auth_with_cookiejar(cookies: List):
     cookiejar = http.cookiejar.CookieJar()
     for cookie in cookies:
         cookiejar.set_cookie(create_cookie(name=cookie.pop('name'), **cookie))
+
+    # requests.cookies.RequestsCookieJar, which has slightly different behaviour
     session = ASFSession()
-    session.auth_with_cookiejar(cookies)
+    session.auth_with_cookiejar(cookiejar)
+
+    request_cookiejar_session = ASFSession()
+    request_cookiejar_session.auth_with_cookiejar(session.cookies)
 
 def run_test_asf_session_rebuild_auth(
     original_domain: str, 
     response_domain: str, 
     response_code: numbers.Number, 
     final_token
     ):
 
     if final_token == 'None':
         final_token = None
 
     session = ASFSession()
 
-    with patch('asf_search.ASFSession.get') as mock_token_session:
+    with patch('asf_search.ASFSession.post') as mock_token_session:
         mock_token_session.return_value.status_code = 200
         session.auth_with_token("bad_token")
         
         req = requests.Request(original_domain)
         req.headers.update({'Authorization': 'Bearer fakeToken'})
 
         response = requests.Response()
```

### Comparing `asf_search-7.0.9/tests/BaselineSearch/Stack/test_stack.py` & `asf_search-7.1.0/tests/BaselineSearch/Stack/test_stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/BaselineSearch/test_baseline_search.py` & `asf_search-7.1.0/tests/BaselineSearch/test_baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/CMR/test_MissionList.py` & `asf_search-7.1.0/tests/CMR/test_MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/Search/test_search.py` & `asf_search-7.1.0/tests/Search/test_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/Search/test_search_generator.py` & `asf_search-7.1.0/tests/Search/test_search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/Serialization/test_serialization.py` & `asf_search-7.1.0/tests/Serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/WKT/test_validate_wkt.py` & `asf_search-7.1.0/tests/WKT/test_validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/download/test_download.py` & `asf_search-7.1.0/tests/download/test_download.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/pytest-config.yml` & `asf_search-7.1.0/tests/pytest-config.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/pytest-managers.py` & `asf_search-7.1.0/tests/pytest-managers.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Alos_response.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Alos_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Alos_response_maxResults3.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Alos_response_missing_baseline.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_L1.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_L1.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.csv` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.csv`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.kml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.kml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.metalink` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_ers_reference.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Fairbanks_ers_stack.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/JERS.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/JERS.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/JERS_stack.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/JERS_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/OPERA_Products.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/OPERA_Products.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/RADARSAT.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/RADARSAT_stack.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/S1_baseline_stack.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/S1_baseline_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/S1_response.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/S1_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/SLC_BURST.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/SLC_BURST_stack.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/SMAP_response.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/SMAP_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/ShorelineMask26.shp` & `asf_search-7.1.0/tests/yml_tests/Resources/ShorelineMask26.shp`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/Resources/Shovel_Creek_many_points.yml` & `asf_search-7.1.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_ASFProduct.yml` & `asf_search-7.1.0/tests/yml_tests/test_ASFProduct.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_ASFSearchOptions.yml` & `asf_search-7.1.0/tests/yml_tests/test_ASFSearchOptions.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_ASFSearchResults.yml` & `asf_search-7.1.0/tests/yml_tests/test_ASFSearchResults.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_ASFSession.yml` & `asf_search-7.1.0/tests/yml_tests/test_ASFSession.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_baseline_search.yml` & `asf_search-7.1.0/tests/yml_tests/test_baseline_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_download.yml` & `asf_search-7.1.0/tests/yml_tests/test_download.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_search.yml` & `asf_search-7.1.0/tests/yml_tests/test_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_serialization.yml` & `asf_search-7.1.0/tests/yml_tests/test_serialization.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_stack.yml` & `asf_search-7.1.0/tests/yml_tests/test_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.0.9/tests/yml_tests/test_validate_wkt.yml` & `asf_search-7.1.0/tests/yml_tests/test_validate_wkt.yml`

 * *Files identical despite different names*

