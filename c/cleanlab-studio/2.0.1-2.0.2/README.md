# Comparing `tmp/cleanlab-studio-2.0.1.tar.gz` & `tmp/cleanlab_studio-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-2.0.1.tar", last modified: Tue Apr  9 19:10:11 2024, max compression
+gzip compressed data, was "cleanlab_studio-2.0.2.tar", last modified: Fri Apr 19 18:53:16 2024, max compression
```

## Comparing `cleanlab-studio-2.0.1.tar` & `cleanlab_studio-2.0.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.040750 cleanlab-studio-2.0.1/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/clean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    24094 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    26845 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/trustworthy_language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/clean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30234 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/trustworthy_language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/setup.py
```

### Comparing `cleanlab-studio-2.0.1/LICENSE` & `cleanlab_studio-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/PKG-INFO` & `cleanlab_studio-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.1
+Version: 2.0.2
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-2.0.1/README.md` & `cleanlab_studio-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/api_service.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/dataset.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/click_helpers.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/upload.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/login/login.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/main.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/types.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/cli/util.py` & `cleanlab_studio-2.0.2/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/errors.py` & `cleanlab_studio-2.0.2/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/api/api.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/api/api.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/clean_helpers.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/constants.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/constants.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/__init__.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/settings.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/concurrency.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/concurrency.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/validation.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/validation.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/upload_helpers.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/internal/util.py` & `cleanlab_studio-2.0.2/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/studio/inference.py` & `cleanlab_studio-2.0.2/cleanlab_studio/studio/inference.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/studio/studio.py` & `cleanlab_studio-2.0.2/cleanlab_studio/studio/studio.py`

 * *Files 3% similar despite different names*

```diff
@@ -387,36 +387,47 @@
         self,
         quality_preset: TLMQualityPreset = "medium",
         *,
         options: Optional[trustworthy_language_model.TLMOptions] = None,
         timeout: Optional[float] = None,
         verbose: Optional[bool] = None,
     ) -> trustworthy_language_model.TLM:
-        """Gets a configured instance of Trustworthy Language Model (TLM).
+        """Instantiates a configured Trustworthy Language Model (TLM) instance.
 
-        The returned TLM object can then be used as a drop-in replacement for an LLM, for estimating trustworthiness scores for LLM prompt/response pairs, and more. See the documentation for the [TLM](../trustworthy_language_model#class-TLM) class for more on what you can do with TLM.
+        The TLM object can be used as a drop-in replacement for an LLM, or, for estimating trustworthiness scores for arbitrary text prompt/response pairs, and more (see the [TLM documentation](../trustworthy_language_model#class-tlm)).
 
-        For advanced use cases, TLM supports a number of configuration options. The documentation below summarizes the options, and the [TLM tutorial](/tutorials/tlm) explains the tradeoffs in more detail.
+        For advanced use, TLM offers configuration options. The documentation below summarizes these options, and more details are explained in the [TLM tutorial](/tutorials/tlm).
 
         Args:
-            quality_preset (TLMQualityPreset): quality preset to use for TLM queries, which will determine the quality of the output responses and trustworthiness scores.
-            Supported presets include "best", "high", "medium", "low", "base".
-            The "best" and "high" presets will improve the LLM responses themselves, with "best" also returning the most reliable trustworthiness scores.
-            The "medium" and "low" presets will return standard LLM responses along with associated confidence scores,
-            with "medium" producing more reliable trustworthiness scores than low.
-            The "base" preset will not return any confidence score, just a standard LLM output response, this option is similar to using your favorite LLM API.
-            Higher presets have increased runtime and cost.
+            quality_preset (TLMQualityPreset): An optional preset to control the quality of TLM responses and trustworthiness scores vs. runtimes/costs.
+                TLMQualityPreset is a string specifying one of the supported presets, including "best", "high", "medium", "low", "base".
+
+                The "best" and "high" presets return improved LLM responses,
+                with "best" also returning more reliable trustworthiness scores than "high".
+                The "medium" and "low" presets return standard LLM responses along with associated trustworthiness scores,
+                with "medium" producing more reliable trustworthiness scores than low.
+                The "base" preset will not return any trustworthiness score, just a standard LLM response, and is similar to directly using your favorite LLM API.
+
+                Higher presets have increased runtime and cost (and may internally consume more tokens).
+                Reduce your preset if you see token-limit errors.
+                Details about each present are in the documentation for [TLMOptions](../trustworthy_language_model#class-tlmoptions).
+                Avoid using "best" or "high" presets if you primarily want to get trustworthiness scores, and are less concerned with improving LLM responses.
+                These presets have higher runtime/cost and are optimized to return more accurate LLM outputs, but not necessarily more reliable trustworthiness scores.
 
             options (TLMOptions, optional): a typed dict of advanced configuration options.
-            Options that can be passed in include "model", "max_tokens", "num_candidate_responses", "num_consistency_samples", "use_self_reflection".
+            Avaialable options (keys in this dict) include "model", "max_tokens", "num_candidate_responses", "num_consistency_samples", "use_self_reflection".
             For more details about the options, see the documentation for [TLMOptions](../trustworthy_language_model#class-tlmoptions).
+            If specified, these override any settings from the choice of `quality_preset`.
 
-            timeout (float, optional): timeout (in seconds) to apply to each method call. If a result is not produced within the timeout, a TimeoutError will be raised. Defaults to None, which does not apply a timeout.
+            timeout (float, optional): timeout (in seconds) to apply to each TLM prompt.
+            If a batch of data is passed in, the timeout will be applied to each individual item in the batch.
+            If a result is not produced within the timeout, a TimeoutError will be raised. Defaults to None, which does not apply a timeout.
 
-            verbose (bool, optional): whether to run in verbose mode, i.e., whether to show a tqdm progress bar when TLM is prompted with batches of data. If None, this will be determined automatically based on whether the code is running in an interactive environment such as a notebook.
+            verbose (bool, optional): whether to print outputs during execution, i.e., whether to show a progress bar when TLM is prompted with batches of data.
+            If None, this will be determined automatically based on whether the code is running in an interactive environment such as a Jupyter notebook.
 
         Returns:
             TLM: the [Trustworthy Language Model](../trustworthy_language_model#class-tlm) object
         """
         return trustworthy_language_model.TLM(
             self._api_key, quality_preset, options=options, timeout=timeout, verbose=verbose
         )
```

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/studio/trustworthy_language_model.py` & `cleanlab_studio-2.0.2/cleanlab_studio/studio/trustworthy_language_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Cleanlab's Trustworthy Language Model (TLM) is a large language model that gives more reliable answers and quantifies its uncertainty in these answers.
 
-**This module is not meant to be imported and used directly.** Instead, use [`Studio.TLM()`](/reference/python/studio/#method-tlm) to instantiate a [TLM](#class-TLM) object, and then you can use the methods like [`prompt()`](#method-prompt) and [`get_trustworthiness_score()`](#method-get_trustworthiness_score) documented in this page.
+**This module is not meant to be imported and used directly.** Instead, use [`Studio.TLM()`](/reference/python/studio/#method-tlm) to instantiate a [TLM](#class-TLM) object, and then you can use the methods like [`prompt()`](#method-prompt) and [`get_trustworthiness_score()`](#method-get_trustworthiness_score) documented on this page.
 
 The [Trustworthy Language Model tutorial](/tutorials/tlm/) further explains TLM and its use cases.
 """
 
 from __future__ import annotations
 
 import asyncio
@@ -30,31 +30,34 @@
 from cleanlab_studio.internal.constants import (
     _VALID_TLM_QUALITY_PRESETS,
     _TLM_MAX_RETRIES,
 )
 
 
 class TLM:
-    """Represents a Trustworthy Language Model (TLM) instance, bound to a Cleanlab Studio account.
+    """Represents a Trustworthy Language Model (TLM) instance, which is bound to a Cleanlab Studio account.
 
-    TLM should be configured and instantiated using the [`Studio.TLM()`](../studio/#method-tlm) method. Then, using the TLM object, you can [`prompt()`](#method-prompt) the language model, etc.
+    ** The TLM object is not meant to be constructed directly.** Instead, use the [`Studio.TLM()`](../studio/#method-tlm)
+    method to configure and instantiate a TLM object.
+    After you've instantiated the TLM object using [`Studio.TLM()`](../studio/#method-tlm), you can use the instance methods documented on this page.
     """
 
     def __init__(
         self,
         api_key: str,
         quality_preset: TLMQualityPreset,
         *,
         options: Optional[TLMOptions] = None,
         timeout: Optional[float] = None,
         verbose: Optional[bool] = None,
     ) -> None:
-        """Initializes a Trustworthy Language Model.
+        """Use `Studio.TLM()` instead of this method to initialize a TLM.
 
-        **Objects of this class are not meant to be constructed directly.** Instead, use [`Studio.TLM()`](../studio/#method-tlm), whose documentation also explains the different configuration options."""
+        lazydocs: ignore
+        """
         self._api_key = api_key
 
         if quality_preset not in _VALID_TLM_QUALITY_PRESETS:
             raise ValidationError(
                 f"Invalid quality preset {quality_preset} -- must be one of {_VALID_TLM_QUALITY_PRESETS}"
             )
 
@@ -83,25 +86,23 @@
         self._rate_handler = TlmRateHandler()
 
     async def _batch_prompt(
         self,
         prompts: Sequence[str],
         capture_exceptions: bool = False,
     ) -> Union[List[TLMResponse], List[Optional[TLMResponse]]]:
-        """Run batch of TLM prompts. The list returned will have the same length as the input list.
-
-        If capture_exceptions is True, the list will contain None in place of the response for any errors or timeout processing some inputs.
-        Otherwise, the method will raise an exception for any errors or timeout processing some inputs.
+        """Run a batch of prompts through TLM and get responses/scores for each prompt in the batch. The list returned will have the same length as the input list.
 
         Args:
             prompts (List[str]): list of prompts to run
-            capture_exceptions (bool): if should return None in place of the response for any errors or timeout processing some inputs
+            capture_exceptions (bool): if ``True``, the returned list will contain ``None`` in place of the response for any errors or timeout when processing a particular prompt from the batch.
+                If ``False``, this entire method will raise an exception if TLM fails to produce a result for any prompt in the batch.
 
         Returns:
-            Union[List[TLMResponse], List[Optional[TLMResponse]]]: TLM responses for each prompt (in supplied order)
+            Union[List[TLMResponse], List[Optional[TLMResponse]]]: TLM responses/scores for each prompt (in supplied order)
         """
         if capture_exceptions:
             per_query_timeout, per_batch_timeout = self._timeout, None
         else:
             per_query_timeout, per_batch_timeout = None, self._timeout
 
         # run batch of TLM
@@ -125,38 +126,38 @@
 
     async def _batch_get_trustworthiness_score(
         self,
         prompts: Sequence[str],
         responses: Sequence[str],
         capture_exceptions: bool = False,
     ) -> Union[List[float], List[Optional[float]]]:
-        """Run batch of TLM get confidence score.
+        """Run batch of TLM get trustworthiness score.
 
         capture_exceptions behavior:
         - If true, the list will contain None in place of the response for any errors or timeout processing some inputs.
         - Otherwise, the method will raise an exception for any errors or timeout processing some inputs.
 
         capture_exceptions interaction with timeout:
         - If true, timeouts are applied on a per-query basis (i.e. some queries may succeed while others fail)
         - If false, a single timeout is applied to the entire batch (i.e. all queries will fail if the timeout is reached)
 
         Args:
-            prompts (Sequence[str]): list of prompts to run get confidence score for
-            responses (Sequence[str]): list of responses to run get confidence score for
+            prompts (Sequence[str]): list of prompts to run get trustworthiness score for
+            responses (Sequence[str]): list of responses to run get trustworthiness score for
             capture_exceptions (bool): if should return None in place of the response for any errors or timeout processing some inputs
 
         Returns:
-            Union[List[float], List[Optional[float]]]: TLM confidence score for each prompt (in supplied order)
+            Union[List[float], List[Optional[float]]]: TLM trustworthiness score for each prompt (in supplied order)
         """
         if capture_exceptions:
             per_query_timeout, per_batch_timeout = self._timeout, None
         else:
             per_query_timeout, per_batch_timeout = None, self._timeout
 
-        # run batch of TLM get confidence score
+        # run batch of TLM get trustworthiness score
         tlm_responses = await self._batch_async(
             [
                 self._get_trustworthiness_score_async(
                     prompt,
                     response,
                     timeout=per_query_timeout,
                     capture_exceptions=capture_exceptions,
@@ -176,15 +177,15 @@
         self,
         tlm_coroutines: Sequence[Coroutine[None, None, Union[TLMResponse, float, None]]],
         batch_timeout: Optional[float] = None,
     ) -> Sequence[Union[TLMResponse, float, None]]:
         """Runs batch of TLM queries.
 
         Args:
-            tlm_coroutines (List[Coroutine[None, None, Union[TLMResponse, float, None]]]): list of query coroutines to run, returning TLM responses or confidence scores (or None if capture_exceptions is True)
+            tlm_coroutines (List[Coroutine[None, None, Union[TLMResponse, float, None]]]): list of query coroutines to run, returning TLM responses or trustworthiness scores (or None if capture_exceptions is True)
             batch_timeout (Optional[float], optional): timeout (in seconds) to run all queries, defaults to None (no timeout)
 
         Returns:
             Sequence[Union[TLMResponse, float, None]]: list of coroutine results, with preserved order
         """
         tlm_query_tasks = [asyncio.create_task(tlm_coro) for tlm_coro in tlm_coroutines]
 
@@ -222,24 +223,26 @@
         """
         Gets response and trustworthiness score for any text input.
 
         This method prompts the TLM with the given prompt(s), producing completions (like a standard LLM)
         but also provides trustworthiness scores quantifying the quality of the output.
 
         Args:
-            prompt (str | Sequence[str]): prompt (or list of multiple prompts) for the language model
+            prompt (str | Sequence[str]): prompt (or list of multiple prompts) for the language model.
+                Providing a batch of many prompts here will be faster than calling this method on each prompt separately.
         Returns:
             TLMResponse | List[TLMResponse]: [TLMResponse](#class-tlmresponse) object containing the response and trustworthiness score.
                 If multiple prompts were provided in a list, then a list of such objects is returned, one for each prompt.
-                This method will raise an exception if any errors occur or if you hit a timeout (given a timeout is specified),
-                and is suitable if strict error handling and immediate notification of any exceptions/timeouts is preferred.
-                However, you could lose any partial results if an exception is raised.
-                If saving partial results is important to you, you can call this method on smaller chunks of data at a time
-                (and save intermediate results as desired); you can also consider using the more advanced
-                [`try_prompt()`](#method-try_prompt) method instead.
+                This method will raise an exception if any errors occur or if you hit a timeout (given a timeout is specified).
+                Use it if you want strict error handling and immediate notification of any exceptions/timeouts.
+
+                If running this method on a big batch of prompts: you might lose partially completed results if TLM fails on any one of them.
+                To avoid losing partial results for the prompts that TLM did not fail on,
+                you can either call this method on smaller batches of prompts at a time
+                (and save intermediate results between batches), or use the [`try_prompt()`](#method-try_prompt) method instead.
         """
         validate_tlm_prompt(prompt)
 
         if isinstance(prompt, str):
             return cast(
                 TLMResponse,
                 self._event_loop.run_until_complete(
@@ -256,34 +259,34 @@
 
     def try_prompt(
         self,
         prompt: Sequence[str],
         /,
     ) -> List[Optional[TLMResponse]]:
         """
-        Gets response and trustworthiness score for any text input,
+        Gets response and trustworthiness score for any batch of prompts,
         handling any failures (errors of timeouts) by returning None in place of the failures.
 
         The list returned will have the same length as the input list, if there are any
         failures (errors or timeout) processing some inputs, the list will contain None in place of the response.
 
-        If there are any failures (errors or timeouts) processing some inputs, the list returned will have
-        the same length as the input list. In case of failure, the list will contain None in place of the response.
+        This is the recommended way to get TLM responses and trustworthiness scores for big datasets of many prompts,
+        where some individual TLM responses within the dataset may fail. It ensures partial results are not lost.
 
         Args:
             prompt (Sequence[str]): list of multiple prompts for the TLM
         Returns:
             List[Optional[TLMResponse]]: list of [TLMResponse](#class-tlmresponse) objects containing the response and trustworthiness score.
                 The returned list will always have the same length as the input list.
-                In case of failure on any prompt (due to timeouts or other erros),
-                the return list will contain None in place of the TLM response.
-                This method is suitable if you prioritize obtaining results for as many inputs as possible,
-                however you might miss out on certain error messages.
-                If you would prefer to be notified immediately about any errors or timeouts that might occur,
-                consider using the [`prompt()`](#method-prompt) method instead.
+                In case of TLM failure on any prompt (due to timeouts or other errors),
+                the return list will contain None in place of the TLM response for that failed prompt.
+                Use this to obtain TLM results for as many prompts as possible,
+                but you might miss out on certain error messages.
+                If you prefer to be notified immediately about any errors or timeouts when running many prompts,
+                use the [`prompt()`](#method-prompt) method instead.
         """
         validate_tlm_try_prompt(prompt)
 
         return cast(
             List[Optional[TLMResponse]],
             self._event_loop.run_until_complete(
                 self._batch_prompt(prompt, capture_exceptions=True),
@@ -293,15 +296,20 @@
     async def prompt_async(
         self,
         prompt: Union[str, Sequence[str]],
         /,
     ) -> Union[TLMResponse, List[TLMResponse]]:
         """
         Asynchronously get response and trustworthiness score for any text input from TLM.
-        This method is similar to the [`prompt()`](#method-prompt) method but operates asynchronously.
+        This method is similar to the [`prompt()`](#method-prompt) method but operates asynchronously,
+        allowing for non-blocking concurrent operations.
+
+        Use this method if prompts are streaming in one at a time, and you want to return results
+        for each one as quickly as possible, without the TLM execution of any one prompt blocking the execution of the others.
+        Asynchronous methods do not block until completion, so you will need to fetch the results yourself.
 
         Args:
             prompt (str | Sequence[str]): prompt (or list of multiple prompts) for the TLM
         Returns:
             TLMResponse | List[TLMResponse]: [TLMResponse](#class-tlmresponse) object containing the response and trustworthiness score.
                 If multiple prompts were provided in a list, then a list of such objects is returned, one for each prompt.
                 This method will raise an exception if any errors occur or if you hit a timeout (given a timeout is specified).
@@ -366,29 +374,30 @@
         }
 
     def get_trustworthiness_score(
         self,
         prompt: Union[str, Sequence[str]],
         response: Union[str, Sequence[str]],
     ) -> Union[float, List[float]]:
-        """Gets trustworthiness score for prompt-response pairs.
+        """Computes trustworthiness score for arbitrary given prompt-response pairs.
 
         Args:
             prompt (str | Sequence[str]): prompt (or list of prompts) for the TLM to evaluate
-            response (str | Sequence[str]): response (or list of responses) corresponding to the input prompts
+            response (str | Sequence[str]): existing response (or list of responses) associated with the input prompts.
+                These can be from any LLM or human-written responses.
         Returns:
             float | List[float]: float or list of floats (if multiple prompt-responses were provided) corresponding
                 to the TLM's trustworthiness score.
                 The score quantifies how confident TLM is that the given response is good for the given prompt.
-                This method will raise an exception if any errors occur or if you hit a timeout (given a timeout is specified),
-                and is suitable if strict error handling and immediate notification of any exceptions/timeouts is preferred.
-                However, you could lose any partial results if an exception is raised.
-                If saving partial results is important to you, you can call this method on smaller chunks of data at a time
-                (and save intermediate results as desired); you can also consider using the more advanced
-                [`try_get_trustworthiness_score()`](#method-try_get_trustworthiness_score) method instead.
+                If running on many prompt-response pairs simultaneously:
+                this method will raise an exception if any TLM errors or timeouts occur.
+                Use it if strict error handling and immediate notification of any exceptions/timeouts is preferred.
+                You will lose any partial results if an exception is raised.
+                If saving partial results is important, you can call this method on smaller batches of prompt-response pairs at a time
+                (and save intermediate results) or use the [`try_get_trustworthiness_score()`](#method-try_get_trustworthiness_score) method instead.
         """
         validate_tlm_prompt_response(prompt, response)
 
         if isinstance(prompt, str) and isinstance(response, str):
             return cast(
                 float,
                 self._event_loop.run_until_complete(
@@ -406,32 +415,36 @@
         )
 
     def try_get_trustworthiness_score(
         self,
         prompt: Sequence[str],
         response: Sequence[str],
     ) -> List[Optional[float]]:
-        """Gets trustworthiness score for prompt-response pairs.
-        The list returned will have the same length as the input list, if there are any
-        failures (errors or timeout) processing some inputs, the list will contain None
-        in place of the response.
+        """Gets trustworthiness score for batches of many prompt-response pairs.
+
+        The list returned will have the same length as the input list, if TLM hits any
+        errors or timeout processing certain inputs, the list will contain None
+        in place of the TLM score for this failed input.
+
+        This is the recommended way to get TLM trustworthiness scores for big datasets,
+        where some individual TLM calls within the dataset may fail. It will ensure partial results are not lost.
 
         Args:
             prompt (Sequence[str]): list of prompts for the TLM to evaluate
-            response (Sequence[str]): list of responses corresponding to the input prompts
+            response (Sequence[str]): list of existing responses corresponding to the input prompts (from any LLM or human-written)
         Returns:
             List[float]: list of floats corresponding to the TLM's trustworthiness score.
                 The score quantifies how confident TLM is that the given response is good for the given prompt.
                 The returned list will always have the same length as the input list.
-                In case of failure on any prompt-response pair (due to timeouts or other erros),
-                the return list will contain None in place of the trustworthiness score.
-                This method is suitable if you prioritize obtaining results for as many inputs as possible,
+                In case of TLM error or timeout on any prompt-response pair,
+                the returned list will contain None in place of the trustworthiness score.
+                Use this method if you prioritize obtaining results for as many inputs as possible,
                 however you might miss out on certain error messages.
-                If you would prefer to be notified immediately about any errors or timeouts that might occur,
-                consider using the [`get_trustworthiness_score()`](#method-get_trustworthiness_score) method instead.
+                If you prefer to be notified immediately about any errors or timeouts,
+                use the [`get_trustworthiness_score()`](#method-get_trustworthiness_score) method instead.
         """
         validate_try_tlm_prompt_response(prompt, response)
 
         return cast(
             List[Optional[float]],
             self._event_loop.run_until_complete(
                 self._batch_get_trustworthiness_score(prompt, response, capture_exceptions=True)
@@ -440,15 +453,20 @@
 
     async def get_trustworthiness_score_async(
         self,
         prompt: Union[str, Sequence[str]],
         response: Union[str, Sequence[str]],
     ) -> Union[float, List[float]]:
         """Asynchronously gets trustworthiness score for prompt-response pairs.
-        This method is similar to the [`get_trustworthiness_score()`](#method-get_trustworthiness_score) method but operates asynchronously.
+        This method is similar to the [`get_trustworthiness_score()`](#method-get_trustworthiness_score) method but operates asynchronously,
+        allowing for non-blocking concurrent operations.
+
+        Use this method if prompt-response pairs are streaming in, and you want to return TLM scores
+        for each pair as quickly as possible, without the TLM scoring of any one pair blocking the scoring of the others.
+        Asynchronous methods do not block until completion, so you will need to fetch the results yourself.
 
         Args:
             prompt (str | Sequence[str]): prompt (or list of prompts) for the TLM to evaluate
             response (str | Sequence[str]): response (or list of responses) corresponding to the input prompts
         Returns:
             float | List[float]: float or list of floats (if multiple prompt-responses were provided) corresponding
                 to the TLM's trustworthiness score.
@@ -491,15 +509,15 @@
             batch_index: index of the prompt in the batch, used for error messages
         Returns:
             float corresponding to the TLM's trustworthiness score
 
         """
         if self._quality_preset == "base":
             raise ValidationError(
-                "Cannot get confidence score with `base` quality_preset -- choose a higher preset."
+                "Cannot get trustworthiness score with `base` quality_preset -- choose a higher preset."
             )
 
         try:
             tlm_response = await asyncio.wait_for(
                 api.tlm_get_confidence_score(
                     self._api_key,
                     prompt,
@@ -535,40 +553,60 @@
 
     response: str
     trustworthiness_score: Optional[float]
 
 
 class TLMOptions(TypedDict):
     """Typed dict containing advanced configuration options for the Trustworthy Language Model.
-    Many of these arguments are automatically determined by the quality preset selected
-    (see the arguments in the TLM [initialization method](../studio#method-tlm) to learn more about the various quality presets),
-    but specifying custom values here will override any default values from the quality preset.
+    Many of these configurations are automatically determined by the quality preset selected
+    (see the arguments in the TLM [initialization method](../studio#method-tlm) to learn more about quality presets).
+    Specifying custom values here will override any default values from the quality preset.
+
+    For all options described below, higher/more expensive settings will lead to longer runtimes and may consume more tokens internally.
+    The high token cost might make it such that you are not able to run long prompts (or prompts with long responses) in your account,
+    unless your token limits are increased. If you are hit token limit issues, try using lower/less expensive settings
+    to be able to run longer prompts/responses.
+
+    The default values corresponding to each quality preset (specified when instantiating [`Studio.TLM()`](../studio/#method-tlm)) are:
+    - **best:** `num_candidate_responses` = 6, `num_consistency_samples` = 8, `use_self_reflection` = True. This preset will improve LLM responses.
+    - **high:** `num_candidate_responses` = 4, `num_consistency_samples` = 8, `use_self_reflection` = True. This preset will improve LLM responses.
+    - **medium:** `num_candidate_responses` = 1, `num_consistency_samples` = 8, `use_self_reflection` = True.
+    - **low:** `num_candidate_responses` = 1, `num_consistency_samples` = 4, `use_self_reflection` = True.
+    - **base:** `num_candidate_responses` = 1, `num_consistency_samples` = 0, `use_self_reflection` = False. This preset is equivalent to a regular LLM call.
+
+    By default, the TLM is set to the "medium" quality preset. The default `model` used is "gpt-3.5-turbo-16k", and `max_tokens` is 512 for all quality presets.
+    You can set custom values for these arguments regardless of the quality preset specified.
 
     Args:
         model (str, default = "gpt-3.5-turbo-16k"): underlying LLM to use (better models will yield better results).
         Models currently supported include "gpt-3.5-turbo-16k", "gpt-4".
 
         max_tokens (int, default = 512): the maximum number of tokens to generate in the TLM response.
-        The minimum value for this parameter is 64, and the maximum is 512.
+        This number will impact the maximum number of tokens you will see in the output response, and also the number of tokens
+        that can be generated internally within the TLM (to estimate the trustworthiness score).
+        Higher values here can produce better (more reliable) TLM responses and trustworthiness scores, but at higher costs/runtimes.
+        If you are experiencing token limit errors while using the TLM (especially on higher quality presets), consider lowering this number.
+        This parameter must be between 64 and 512.
 
-        num_candidate_responses (int, default = 1): this controls how many candidate responses are internally generated.
+        num_candidate_responses (int, default = 1): how many alternative candidate responses are internally generated by TLM.
         TLM scores the trustworthiness of each candidate response, and then returns the most trustworthy one.
-        Higher values here can produce better (more accurate) responses from the TLM, but at higher costs/runtimes.
-        The minimum value for this parameter is 1, and the maximum is 20.
-
-        num_consistency_samples (int, default = 5): this controls how many samples are internally generated to evaluate the LLM-response-consistency.
-        This is a big part of the returned trustworthiness_score, in particular to evaluate strange input prompts or prompts that are too open-ended
-        to receive a clearly defined 'good' response.
-        Higher values here produce better (more reliable) TLM confidence scores, but at higher costs/runtimes.
-        The minimum value for this parameter is 0, and the maximum is 20.
-
-        use_self_reflection (bool, default = `True`): this controls whether self-reflection is used to have the LLM reflect upon the response it is
-        generating and explicitly self-evaluate the accuracy of that response.
-        This is a big part of the trustworthiness score, in particular for evaluating responses that are obviously incorrect/bad for a
-        standard prompt (with well-defined answers) that LLMs should be able to handle.
+        Higher values here can produce better (more accurate) responses from the TLM, but at higher costs/runtimes (and internally consumes more tokens).
+        This parameter must be between 1 and 20.
+        When it is 1, TLM simply returns a standard LLM response and does not attempt to improve it.
+
+        num_consistency_samples (int, default = 8): the amount of internal sampling to evaluate LLM-response-consistency.
+        This consistency forms a big part of the returned trustworthiness score, helping quantify the epistemic uncertainty associated with
+        strange prompts or prompts that are too vague/open-ended to receive a clearly defined 'good' response.
+        Higher values here produce better (more reliable) TLM trustworthiness scores, but at higher costs/runtimes.
+        This parameter must be between 0 and 20.
+
+        use_self_reflection (bool, default = `True`): whether the LLM is asked to self-reflect upon the response it
+        generated and self-evaluate this response.
+        This self-reflection forms a big part of the trustworthiness score, helping quantify aleatoric uncertainty associated with challenging prompts
+        and helping catch answers that are obviously incorrect/bad for a prompt asking for a well-defined answer that LLMs should be able to handle.
         Setting this to False disables the use of self-reflection and may produce worse TLM trustworthiness scores, but will reduce costs/runtimes.
     """
 
     model: NotRequired[str]
     max_tokens: NotRequired[int]
     num_candidate_responses: NotRequired[int]
     num_consistency_samples: NotRequired[int]
```

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio/utils/synthetic.py` & `cleanlab_studio-2.0.2/cleanlab_studio/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab_studio-2.0.2/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.1
+Version: 2.0.2
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-2.0.1/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab_studio-2.0.2/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.1/setup.py` & `cleanlab_studio-2.0.2/setup.py`

 * *Files identical despite different names*

