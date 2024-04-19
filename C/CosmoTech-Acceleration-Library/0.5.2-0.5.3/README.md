# Comparing `tmp/CosmoTech_Acceleration_Library-0.5.2.tar.gz` & `tmp/cosmotech_acceleration_library-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech_Acceleration_Library-0.5.2.tar", last modified: Fri Mar 15 14:51:01 2024, max compression
+gzip compressed data, was "cosmotech_acceleration_library-0.5.3.tar", last modified: Fri Apr 19 13:59:40 2024, max compression
```

## Comparing `CosmoTech_Acceleration_Library-0.5.2.tar` & `cosmotech_acceleration_library-0.5.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.803227 CosmoTech_Acceleration_Library-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.795227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.795227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.795227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Core/DataInterface/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Core/DataInterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Core/DataStorage/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Core/DataStorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/writer/
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/tests/redis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.799227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:51:01.803227 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-15 14:51:01.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-15 14:51:01.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:51:01.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:51:01.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-15 14:51:01.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-15 14:51:01.000000 CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-15 14:51:01.803227 CosmoTech_Acceleration_Library-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/requirements.doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-15 14:50:57.000000 CosmoTech_Acceleration_Library-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:51:01.803227 CosmoTech_Acceleration_Library-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.686696 cosmotech_acceleration_library-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.678696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.678696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.678696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Core/DataInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Core/DataInterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Core/DataStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Core/DataStorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/tests/redis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:40.682696 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-19 13:59:40.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-19 13:59:40.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:59:40.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:59:40.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-19 13:59:40.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 13:59:40.000000 cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-19 13:59:40.686696 cosmotech_acceleration_library-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/requirements.doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-19 13:59:36.000000 cosmotech_acceleration_library-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:59:40.686696 cosmotech_acceleration_library-0.5.3/setup.cfg
```

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,26 +114,26 @@
             dataset = api_instance.find_dataset_by_id(
                 organization_id=self.organization_id,
                 dataset_id=dataset_id)
             parameters = dataset['connector']['parameters_values']
 
             is_adt = 'AZURE_DIGITAL_TWINS_URL' in parameters
             is_storage = 'AZURE_STORAGE_CONTAINER_BLOB_PREFIX' in parameters
-            is_legacy_twin_cache = 'TWIN_CACHE_NAME' in parameters  # Legacy twingraph dataset with specific connector
+            is_legacy_twin_cache = 'TWIN_CACHE_NAME' in parameters and dataset['twingraph_id'] is None  # Legacy twingraph dataset with specific connector
 
             if is_adt:
                 return {
                     "type": 'adt',
                     "content": self._download_adt_content(
                         adt_adress=parameters['AZURE_DIGITAL_TWINS_URL']),
                     "name": dataset['name']}
             elif is_legacy_twin_cache:
                 twin_cache_name = parameters['TWIN_CACHE_NAME']
                 return {
-                    "type": "adt",
+                    "type": "twincache",
                     "content": self._read_legacy_twingraph_content(twin_cache_name),
                     "name": dataset["name"]
                 }
             elif is_storage:
                 _file_name = parameters['AZURE_STORAGE_CONTAINER_BLOB_PREFIX'].replace(
                     '%WORKSPACE_FILE%/', '')
                 _content = self._download_file(_file_name)
@@ -141,15 +141,15 @@
                 return {
                     "type": _file_name.split('.')[-1],
                     "content": _content,
                     "name": dataset['name']
                 }
             else:
                 return {
-                    "type": "adt",
+                    "type": "twincache",
                     "content": self._read_twingraph_content(dataset_id),
                     "name": dataset["name"]
                 }
 
     def _read_twingraph_content(self, dataset_id: str) -> dict:
         with cosmotech_api.ApiClient(self.configuration) as api_client:
             dataset_api = DatasetApi(api_client)
```

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader_test.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader_test.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/tests/redis_test.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/tests/redis_test.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/PKG-INFO` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech_Acceleration_Library
-Version: 0.5.2
+Version: 0.5.3
 Summary: Acceleration libraries for CosmoTech cloud based solution development
 Author-email: Cosmo Tech <platform@cosmotech.com>
 Project-URL: Homepage, https://www.cosmotech.com
 Project-URL: Source, https://github.com/Cosmo-Tech/CosmoTech-Acceleration-Library
 Project-URL: Documentation, https://cosmo-tech.github.io/CosmoTech-Acceleration-Library
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,24 +15,29 @@
 Requires-Dist: azure-kusto-ingest==4.2.0
 Requires-Dist: redis==4.4.4
 Requires-Dist: redisgraph_bulk_loader==0.10.2
 Requires-Dist: cosmotech-api~=3.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.1.2
 Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: setuptools
 Provides-Extra: doc
 Requires-Dist: mkdocs==1.5.3; extra == "doc"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "doc"
 Requires-Dist: mkdocs-material==9.4.8; extra == "doc"
 Requires-Dist: mkdocstrings[python]==0.23.0; extra == "doc"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "doc"
 Requires-Dist: pymdown-extensions==10.3.1; extra == "doc"
 Requires-Dist: requirements-parser==0.5.0; extra == "doc"
 Requires-Dist: setuptools==69.1.0; extra == "doc"
 Requires-Dist: mike==2.0.0; extra == "doc"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-docker; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # CosmoTech-Acceleration-Library
 Acceleration library for CosmoTech cloud based solution development
 
 ## Code organisation
 
 In project root directory you'll find 4 main directories:
```

### Comparing `CosmoTech_Acceleration_Library-0.5.2/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt` & `cosmotech_acceleration_library-0.5.3/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.doc.txt
+requirements.test.txt
 requirements.txt
 CosmoTech_Acceleration_Library/__init__.py
 CosmoTech_Acceleration_Library.egg-info/PKG-INFO
 CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
 CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
 CosmoTech_Acceleration_Library.egg-info/not-zip-safe
 CosmoTech_Acceleration_Library.egg-info/requires.txt
```

### Comparing `CosmoTech_Acceleration_Library-0.5.2/LICENSE` & `cosmotech_acceleration_library-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/PKG-INFO` & `cosmotech_acceleration_library-0.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech_Acceleration_Library
-Version: 0.5.2
+Version: 0.5.3
 Summary: Acceleration libraries for CosmoTech cloud based solution development
 Author-email: Cosmo Tech <platform@cosmotech.com>
 Project-URL: Homepage, https://www.cosmotech.com
 Project-URL: Source, https://github.com/Cosmo-Tech/CosmoTech-Acceleration-Library
 Project-URL: Documentation, https://cosmo-tech.github.io/CosmoTech-Acceleration-Library
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,24 +15,29 @@
 Requires-Dist: azure-kusto-ingest==4.2.0
 Requires-Dist: redis==4.4.4
 Requires-Dist: redisgraph_bulk_loader==0.10.2
 Requires-Dist: cosmotech-api~=3.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.1.2
 Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: setuptools
 Provides-Extra: doc
 Requires-Dist: mkdocs==1.5.3; extra == "doc"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "doc"
 Requires-Dist: mkdocs-material==9.4.8; extra == "doc"
 Requires-Dist: mkdocstrings[python]==0.23.0; extra == "doc"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "doc"
 Requires-Dist: pymdown-extensions==10.3.1; extra == "doc"
 Requires-Dist: requirements-parser==0.5.0; extra == "doc"
 Requires-Dist: setuptools==69.1.0; extra == "doc"
 Requires-Dist: mike==2.0.0; extra == "doc"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-docker; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # CosmoTech-Acceleration-Library
 Acceleration library for CosmoTech cloud based solution development
 
 ## Code organisation
 
 In project root directory you'll find 4 main directories:
```

### Comparing `CosmoTech_Acceleration_Library-0.5.2/README.md` & `cosmotech_acceleration_library-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.5.2/pyproject.toml` & `cosmotech_acceleration_library-0.5.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 dynamic = ["version", "dependencies", "optional-dependencies"]
 readme = {file = "README.md", content-type = "text/markdown"}
 
 
 [build-system]
 requires = ["setuptools", "wheel"]
 
+[tool.pytest.ini_options]
+pythonpath = ["."]
+addopts = "--cov-report term-missing:skip-covered --cov=CosmoTech_Acceleration_Library"
+
 [tool.setuptools]
 include-package-data = true
 package-data."*" = [
   "requirements.txt",
   "documentation.requirements.txt"
 ]
 zip-safe = false
@@ -26,8 +30,9 @@
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["CosmoTech_Acceleration_Library*"]
 
 [tool.setuptools.dynamic]
 version.attr = "CosmoTech_Acceleration_Library.__version__"
 dependencies.file = "requirements.txt"
-optional-dependencies.doc.file = "requirements.doc.txt"
+optional-dependencies.doc.file = "requirements.doc.txt"
+optional-dependencies.test.file = "requirements.test.txt"
```

