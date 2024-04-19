# Comparing `tmp/ecosystem-notebooks-0.1.7.tar.gz` & `tmp/ecosystem-notebooks-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecosystem-notebooks-0.1.7.tar", last modified: Wed Apr 10 02:06:34 2024, max compression
+gzip compressed data, was "ecosystem-notebooks-0.1.8.tar", last modified: Fri Apr 19 09:48:58 2024, max compression
```

## Comparing `ecosystem-notebooks-0.1.7.tar` & `ecosystem-notebooks-0.1.8.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.813865 ecosystem-notebooks-0.1.7/
--rw-r--r--   0 ericnewby   (501) staff       (20)     1069 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/LICENSE
--rw-r--r--   0 ericnewby   (501) staff       (20)      400 2023-10-13 03:48:11.000000 ecosystem-notebooks-0.1.7/MANIFEST.in
--rw-r--r--   0 ericnewby   (501) staff       (20)     3693 2024-04-10 02:06:34.813467 ecosystem-notebooks-0.1.7/PKG-INFO
--rw-r--r--   0 ericnewby   (501) staff       (20)     2966 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.7/README.rst
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.709787 ecosystem-notebooks-0.1.7/docs/
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.712684 ecosystem-notebooks-0.1.7/docs/images/
--rw-r--r--   0 ericnewby   (501) staff       (20)    62723 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/docs/images/jupyter_landing_page.png
--rw-r--r--   0 ericnewby   (501) staff       (20)    25467 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/docs/images/login.png
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.713818 ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/
--rw-r--r--   0 ericnewby   (501) staff       (20)     3693 2024-04-10 02:06:34.000000 ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/PKG-INFO
--rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2024-04-10 02:06:34.000000 ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/SOURCES.txt
--rw-r--r--   0 ericnewby   (501) staff       (20)        1 2024-04-10 02:06:34.000000 ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/dependency_links.txt
--rw-r--r--   0 ericnewby   (501) staff       (20)       17 2024-04-10 02:06:34.000000 ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/requires.txt
--rw-r--r--   0 ericnewby   (501) staff       (20)       19 2024-04-10 02:06:34.000000 ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/top_level.txt
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.716147 ecosystem-notebooks-0.1.7/prediction/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/__init__.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.740200 ecosystem-notebooks-0.1.7/prediction/apis/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     6645 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/apis/algorithm_client_pulse.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/auth_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2852 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/apis/data_ingestion_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    11002 2024-04-09 16:51:31.000000 ecosystem-notebooks-0.1.7/prediction/apis/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    13059 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/data_munging_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    97109 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.7/prediction/apis/deployment_management.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1069 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/apis/ecosystem_generation_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      889 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/ecosystem_home.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      408 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/ecosystem_main.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1146 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/ecosystem_user_profiles.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2085 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.7/prediction/apis/functions.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      263 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/apis/interactions.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    15423 2024-04-09 12:25:57.000000 ecosystem-notebooks-0.1.7/prediction/apis/online_learning_management.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     7959 2024-04-07 09:49:09.000000 ecosystem-notebooks-0.1.7/prediction/apis/prediction_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2067 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.7/prediction/apis/quickflat.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      246 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/settings_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      811 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/transaction_categorization.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1145 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/user_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2601 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/apis/utilities.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2439 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/apis/worker_aws.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     4005 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.7/prediction/apis/worker_file_service.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      520 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/worker_google.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     4954 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/worker_h2o.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      311 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/worker_microsoft.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      291 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/apis/worker_open_ai.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2860 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/apis/worker_uber.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.789770 ecosystem-notebooks-0.1.7/prediction/endpoints/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/algorithm_client_pulse.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1159 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/auth_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1765 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/data_ingestion_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     6042 2024-04-09 16:47:01.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     5350 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/data_munging_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      840 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/ecosystem_generation_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      598 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/ecosystem_home.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      335 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/ecosystem_main.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      754 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/ecosystem_user_profiles.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      155 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/interaction.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     5299 2024-04-07 09:47:48.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/prediction_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      178 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/settings_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      540 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/transaction_categorization.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      471 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/user_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1806 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/utilities.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1766 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/worker_aws.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2238 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/worker_file_service.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      331 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/worker_google.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3591 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/worker_h2o.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      173 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/worker_microsoft.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      167 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/worker_open_ai.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      831 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/endpoints/worker_uber.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/prediction/export_to_notebook.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2955 2023-06-02 11:33:45.000000 ecosystem-notebooks-0.1.7/prediction/jwt_access.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1952 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/nlp_utils.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     4412 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/notebook_functions.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1689 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/prediction_utils.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3815 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.7/prediction/request_utils.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.793996 ecosystem-notebooks-0.1.7/prediction/utils/
--rw-r--r--   0 ericnewby   (501) staff       (20)     5888 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/prediction/utils/endpoint_diff.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.799663 ecosystem-notebooks-0.1.7/runtime/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      517 2024-04-08 10:10:12.000000 ecosystem-notebooks-0.1.7/runtime/access.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.807103 ecosystem-notebooks-0.1.7/runtime/apis/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/apis/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     4488 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/runtime/apis/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     8791 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.7/runtime/apis/predictor_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      452 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/apis/restart_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      840 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/apis/runtime_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    14076 2023-04-24 06:53:33.000000 ecosystem-notebooks-0.1.7/runtime/apis/worker_utilities.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.812656 ecosystem-notebooks-0.1.7/runtime/endpoints/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/endpoints/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2431 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/runtime/endpoints/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2538 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/runtime/endpoints/predictor_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      302 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/endpoints/restart_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      283 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/endpoints/runtime_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     6123 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/runtime/endpoints/worker_utilities.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.7/runtime/export_to_notebook.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3632 2024-04-08 10:10:58.000000 ecosystem-notebooks-0.1.7/runtime/request_utils.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-10 02:06:34.812993 ecosystem-notebooks-0.1.7/runtime/utils/
--rw-r--r--   0 ericnewby   (501) staff       (20)     5079 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.7/runtime/utils/endpoint_diff.py
--rw-r--r--   0 ericnewby   (501) staff       (20)       38 2024-04-10 02:06:34.813929 ecosystem-notebooks-0.1.7/setup.cfg
--rw-r--r--   0 ericnewby   (501) staff       (20)     2151 2024-04-10 02:06:17.000000 ecosystem-notebooks-0.1.7/setup.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.799048 ecosystem-notebooks-0.1.8/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1069 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/LICENSE
+-rw-r--r--   0 ericnewby   (501) staff       (20)      400 2023-10-13 03:48:11.000000 ecosystem-notebooks-0.1.8/MANIFEST.in
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3646 2024-04-19 09:48:58.798906 ecosystem-notebooks-0.1.8/PKG-INFO
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2966 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.8/README.rst
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.777580 ecosystem-notebooks-0.1.8/docs/
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.779780 ecosystem-notebooks-0.1.8/docs/images/
+-rw-r--r--   0 ericnewby   (501) staff       (20)    62723 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/docs/images/jupyter_landing_page.png
+-rw-r--r--   0 ericnewby   (501) staff       (20)    25467 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/docs/images/login.png
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.780472 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3646 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/PKG-INFO
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/SOURCES.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)        1 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/dependency_links.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)       17 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/requires.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)       19 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/top_level.txt
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.782269 ecosystem-notebooks-0.1.8/prediction/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/__init__.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.790820 ecosystem-notebooks-0.1.8/prediction/apis/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     6645 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/algorithm_client_pulse.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/auth_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2852 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/data_ingestion_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    11030 2024-04-17 14:45:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    13059 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/data_munging_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)   132245 2024-04-19 08:38:39.000000 ecosystem-notebooks-0.1.8/prediction/apis/deployment_management.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2024-04-10 18:52:10.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_generation_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      889 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_home.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      408 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_main.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1146 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_user_profiles.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2085 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.8/prediction/apis/functions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      263 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/interactions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    21095 2024-04-10 03:03:23.000000 ecosystem-notebooks-0.1.8/prediction/apis/online_learning_management.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     9428 2024-04-10 18:23:18.000000 ecosystem-notebooks-0.1.8/prediction/apis/prediction_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2067 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.8/prediction/apis/quickflat.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      246 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/settings_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      811 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/transaction_categorization.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1145 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/user_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2601 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2439 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_aws.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4520 2024-04-10 18:26:15.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_file_service.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      520 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_google.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5168 2024-04-10 18:29:50.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_h2o.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      311 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_microsoft.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      291 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_open_ai.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2860 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_uber.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.794825 ecosystem-notebooks-0.1.8/prediction/endpoints/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/algorithm_client_pulse.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1159 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/auth_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1765 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/data_ingestion_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     6030 2024-04-17 14:50:54.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5350 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/data_munging_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      840 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_generation_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      598 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_home.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      335 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_main.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      754 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_user_profiles.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      155 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/interaction.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5299 2024-04-07 09:47:48.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/prediction_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      178 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/settings_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      540 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/transaction_categorization.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      471 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/user_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1806 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1766 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_aws.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2238 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_file_service.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      331 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_google.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3591 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_h2o.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      173 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_microsoft.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      167 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_open_ai.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      831 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_uber.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/export_to_notebook.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3190 2024-04-10 02:58:53.000000 ecosystem-notebooks-0.1.8/prediction/jwt_access.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1952 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/nlp_utils.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4412 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/notebook_functions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1689 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/prediction_utils.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3815 2024-04-18 19:20:21.000000 ecosystem-notebooks-0.1.8/prediction/request_utils.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.794973 ecosystem-notebooks-0.1.8/prediction/utils/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5888 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/utils/endpoint_diff.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.795919 ecosystem-notebooks-0.1.8/runtime/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      666 2024-04-10 03:03:23.000000 ecosystem-notebooks-0.1.8/runtime/access.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.797448 ecosystem-notebooks-0.1.8/runtime/apis/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/apis/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5011 2024-04-15 14:37:55.000000 ecosystem-notebooks-0.1.8/runtime/apis/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     9917 2024-04-16 16:08:31.000000 ecosystem-notebooks-0.1.8/runtime/apis/predictor_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      452 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/apis/restart_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      840 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/apis/runtime_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    14076 2023-04-24 06:53:33.000000 ecosystem-notebooks-0.1.8/runtime/apis/worker_utilities.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.798457 ecosystem-notebooks-0.1.8/runtime/endpoints/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2431 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2538 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/predictor_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      302 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/restart_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      283 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/runtime_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     6123 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/worker_utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/export_to_notebook.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3632 2024-04-08 10:10:58.000000 ecosystem-notebooks-0.1.8/runtime/request_utils.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.798631 ecosystem-notebooks-0.1.8/runtime/utils/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5079 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/utils/endpoint_diff.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)       38 2024-04-19 09:48:58.799102 ecosystem-notebooks-0.1.8/setup.cfg
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2151 2024-04-19 09:48:53.000000 ecosystem-notebooks-0.1.8/setup.py
```

### Comparing `ecosystem-notebooks-0.1.7/LICENSE` & `ecosystem-notebooks-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/PKG-INFO` & `ecosystem-notebooks-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: ecosystem-notebooks
-Version: 0.1.7
+Version: 0.1.8
 Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
 Home-page: https://github.com/ecosystemai/ecosystem-notebooks
 Author: EcosystemAi
 Author-email: jay@ecosystem.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Jupyter :: JupyterLab
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: pymongo
 
 Ecosystem Notebooks
 ===================
 
 What is Ecosystem Notebooks?
 ----------------------------
```

### Comparing `ecosystem-notebooks-0.1.7/README.rst` & `ecosystem-notebooks-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/docs/images/jupyter_landing_page.png` & `ecosystem-notebooks-0.1.8/docs/images/jupyter_landing_page.png`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/docs/images/login.png` & `ecosystem-notebooks-0.1.8/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/PKG-INFO` & `ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: ecosystem-notebooks
-Version: 0.1.7
+Version: 0.1.8
 Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
 Home-page: https://github.com/ecosystemai/ecosystem-notebooks
 Author: EcosystemAi
 Author-email: jay@ecosystem.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Jupyter :: JupyterLab
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: pymongo
 
 Ecosystem Notebooks
 ===================
 
 What is Ecosystem Notebooks?
 ----------------------------
```

### Comparing `ecosystem-notebooks-0.1.7/ecosystem_notebooks.egg-info/SOURCES.txt` & `ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/algorithm_client_pulse.py` & `ecosystem-notebooks-0.1.8/prediction/apis/algorithm_client_pulse.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/auth_controller.py` & `ecosystem-notebooks-0.1.8/prediction/apis/auth_controller.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/data_ingestion_engine.py` & `ecosystem-notebooks-0.1.8/prediction/apis/data_ingestion_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/data_management_engine.py` & `ecosystem-notebooks-0.1.8/prediction/apis/data_management_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 	return meta
 
 def get_cassandra_to_mongo(auth, database, collection, sql, info=False):
 	"""
 	Execute a Cassandra SQL query and ingest the data to a MongoDB collection. The ecosystem server should be configured
 	to connect to the target Cassandra servers.
 
-	:param auth: Authentication object
+	:param auth: Token for accessing the ecosystem-server. Created using jwt_access.
 	:param database: Database to ingest the data to
 	:param collection: Collection to ingest the data to
 	:param sql: Cassandra SQL query to execute
 	"""
 	ep = endpoints.GET_CASSANDRA_TO_MONGODB
 	param_dict = {
 		"database": database,
@@ -348,23 +348,23 @@
 
 def execute_mongo_db_script(auth, json, info=False):
 	ep = endpoints.EXECUTE_MONGO_DB_SCRIPT
 	resp = request_utils.create(auth, ep, json=json, info=info)
 	result = resp.json()
 	return result
 
-# # Data Management Engine: Cassandra
-# def get_cassandra_sql(auth, sql, info=False):
-# 	ep = endpoints.GET_CASSANDRA_SQL
-# 	param_dict = {
-# 		"sql": sql
-# 	}
-# 	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-# 	result = resp.json()
-# 	return result
+# Data Management Engine: Cassandra
+def get_cassandra_sql(auth, sql, info=False):
+	ep = endpoints.GET_CASSANDRA_SQL
+	param_dict = {
+		"sql": sql
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
 
 # Data Management Engine: Presto
 def create_presto_sql(auth, connection, sql, info=False):
 	ep = endpoints.CREATE_PRESTO_SQL
 	param_dict = {
 		"connection": connection,
 		"sql": sql
```

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/data_munging_engine.py` & `ecosystem-notebooks-0.1.8/prediction/apis/data_munging_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/deployment_management.py` & `ecosystem-notebooks-0.1.8/prediction/apis/deployment_management.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Dict, Any
+# from typing import Dict, Any
 
 from prediction.apis import prediction_engine as pe
 from prediction.apis import algorithm_client_pulse as cp
-from prediction.apis import data_management_engine as d
+from prediction.apis import data_management_engine as dme
+from runtime.apis import predictor_engine as o
 
 from datetime import datetime
 from json import JSONDecodeError
 import json
 import pymongo
 
 
@@ -98,15 +99,16 @@
         max_version = max(version_list)
         pre_score_logic = [i["plugins"]["pre_score_class_code"] for i in project_details["deployment_step"] if
                             (i["plugins"]["pre_score_class_text"] == pre_score and i["version"] == max_version)][0]
     elif pre_score in pre_score_code_options:
         pre_score_logic = pre_score_code_options[pre_score]
     else:
         print(
-            "WARNING: pre_score_class not found in default options. Empty class saved to the deployment. To edit the class use the ecosystem.Ai plugin for IntelliJ or the ecosystem.Ai workbench")
+            "WARNING: pre_score_class not found in default options. Empty class saved to the deployment. To edit the "
+            "class use the ecosystem.Ai plugin for IntelliJ or the ecosystem.Ai workbench")
         pre_score_logic = ""
     return pre_score_logic
 
 def get_post_score_code(post_score, project_details):
     post_score_code_options = {
         "PlatformDynamicEngagement.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport com.ecosystem.utils.DataTypeConversions;\nimport com.ecosystem.utils.JSONArraySort;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\n/**\n * ECOSYSTEM.AI INTERNAL PLATFORM SCORING\n * Use this class to score with dynamic sampling configurations. This class is configured to work with no model.\n */\npublic class PlatformDynamicEngagement extends PostScoreSuper {\n\tprivate static final Logger LOGGER = LogManager.getLogger(PlatformDynamicEngagement.class.getName());\n\n\tpublic PlatformDynamicEngagement() {\n\t}\n\n\t/**\n\t * Pre-post predict logic\n\t */\n\tpublic void getPostPredict () {\n\t}\n\n\t/**\n\t * getPostPredict\n\t * Example params:\n\t *    {\"contextual_variable_one\":\"Easy Income Gold|Thin|Senior\", \"contextual_variable_two\":\"\", \"batch\": true}\n\t *\n\t * @param predictModelMojoResult Result from scoring\n\t * @param params                 Params carried from input\n\t * @param session                Session variable for Cassandra\n\t * @return JSONObject result to further post-scoring logic\n\t */\n\tpublic static JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n\t\tdouble startTimePost = System.nanoTime();\n\t\ttry {\n\t\t\t/** Setup JSON objects for specific prediction case */\n\t\t\tJSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n\t\t\t//JSONObject domainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n\n\t\t\tJSONObject offerMatrixWithKey = new JSONObject();\n\t\t\tboolean om = false;\n\t\t\tif (params.has(\"offerMatrixWithKey\")) {\n\t\t\t\tofferMatrixWithKey = params.getJSONObject(\"offerMatrixWithKey\");\n\t\t\t\tom = true;\n\t\t\t}\n\n\t\t\tJSONObject work = params.getJSONObject(\"in_params\");\n\n\t\t\t/***************************************************************************************************/\n\t\t\t/** Standardized approach to access dynamic datasets in plugin.\n\t\t\t * The options array is the data set/feature_store that's keeping track of the dynamic changes.\n\t\t\t * The optionParams is the parameter set that will influence the real-time behavior through param changes.\n\t\t\t */\n\t\t\t/***************************************************************************************************/\n\t\t\tJSONArray options = (JSONArray) ((\n\t\t\t\t\t(JSONObject) params.getJSONObject(\"dynamicCorpora\")\n\t\t\t\t\t\t\t.get(\"dynamic_engagement_options\")).get(\"data\"));\n\t\t\tJSONObject optionParams = (JSONObject) ((\n\t\t\t\t\t(JSONObject) params.getJSONObject(\"dynamicCorpora\")\n\t\t\t\t\t\t\t.get(\"dynamic_engagement\")).get(\"data\"));\n\n\t\t\tJSONObject contextual_variables = optionParams.getJSONObject(\"contextual_variables\");\n\t\t\tJSONObject randomisation = optionParams.getJSONObject(\"randomisation\");\n\n\t\t\t/***************************************************************************************************/\n\t\t\t/** Test if contextual variable is coming via api or feature store: API takes preference... */\n\t\t\tif (!work.has(\"contextual_variable_one\")) {\n\t\t\t\tif (featuresObj.has(contextual_variables.getString(\"contextual_variable_one_name\")))\n\t\t\t\t\twork.put(\"contextual_variable_one\", featuresObj.get(contextual_variables.getString(\"contextual_variable_one_name\")));\n\t\t\t\telse\n\t\t\t\t\twork.put(\"contextual_variable_one\", \"\");\n\t\t\t}\n\t\t\tif (!work.has(\"contextual_variable_two\")) {\n\t\t\t\tif (featuresObj.has(contextual_variables.getString(\"contextual_variable_two_name\")))\n\t\t\t\t\twork.put(\"contextual_variable_two\", featuresObj.get(contextual_variables.getString(\"contextual_variable_two_name\")));\n\t\t\t\telse\n\t\t\t\t\twork.put(\"contextual_variable_two\", \"\");\n\t\t\t}\n\t\t\t/***************************************************************************************************/\n\n\t\t\tJSONArray finalOffers = new JSONArray();\n\t\t\tint offerIndex = 0;\n\t\t\tint explore;\n\t\t\tString contextual_variable_one = String.valueOf(work.get(\"contextual_variable_one\"));\n\t\t\tString contextual_variable_two = String.valueOf(work.get(\"contextual_variable_two\"));\n\t\t\tfor (int j = 0; j < options.length(); j++) {\n\t\t\t\tJSONObject option = options.getJSONObject(j);\n\t\t\t\tString contextual_variable_one_Option = \"\";\n\t\t\t\tif (option.has(\"contextual_variable_one\") && !contextual_variable_one.equals(\"\"))\n\t\t\t\t\tcontextual_variable_one_Option = String.valueOf(option.get(\"contextual_variable_one\"));\n\t\t\t\tString contextual_variable_two_Option = \"\";\n\t\t\t\tif (option.has(\"contextual_variable_two\") && !contextual_variable_two.equals(\"\"))\n\t\t\t\t\tcontextual_variable_two_Option = String.valueOf(option.get(\"contextual_variable_two\"));\n\n\t\t\t\tif (contextual_variable_one_Option.equals(contextual_variable_one) && contextual_variable_two_Option.equals(contextual_variable_two)) {\n\n\t\t\t\t\tdouble alpha = (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"alpha\"));\n\t\t\t\t\tdouble beta = (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"beta\"));\n\t\t\t\t\tdouble accuracy = 0.001;\n\t\t\t\t\tif (option.has(\"accuracy\"))\n\t\t\t\t\t\taccuracy = (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"accuracy\"));\n\n\t\t\t\t\t/***************************************************************************************************/\n\t\t\t\t\t/* r IS THE RANDOMIZED SCORE VALUE */\n\t\t\t\t\tdouble p = 0.0;\n\t\t\t\t\tdouble arm_reward = 0.001;\n\t\t\t\t\tif (randomisation.getString(\"approach\").equals(\"epsilonGreedy\")) {\n\t\t\t\t\t\t// params.put(\"explore\", 0);\n\t\t\t\t\t\texplore = 0;\n\t\t\t\t\t\tp = DataTypeConversions.getDouble(option, \"arm_reward\");\n\t\t\t\t\t\tarm_reward = p;\n\t\t\t\t\t} else {\n\t\t\t\t\t\t/** REMEMBER THAT THIS IS HERE BECAUSE OF BATCH PROCESS, OTHERWISE IT REQUIRES THE TOTAL COUNTS */\n\t\t\t\t\t\t/* Phase 2: sampling - calculate the arms and rank them */\n\t\t\t\t\t\t// params.put(\"explore\", 0); // force explore to zero and use Thompson Sampling only!!\n\t\t\t\t\t\texplore = 0; // set as explore as the dynamic responder is exploration based...\n\t\t\t\t\t\tp = DataTypeConversions.getDouble(option, \"arm_reward\");\n\t\t\t\t\t\tarm_reward = p;\n\n\t\t\t\t\t}\n\t\t\t\t\t/** Check if values are correct */\n\t\t\t\t\tif (p != p) p = 0.0;\n\t\t\t\t\tif (alpha != alpha) alpha = 0.0;\n\t\t\t\t\tif (beta != beta) beta = 0.0;\n\t\t\t\t\tif (arm_reward != arm_reward) arm_reward = 0.0;\n\t\t\t\t\t/***************************************************************************************************/\n\n\t\t\t\t\tString offer = option.getString(\"optionKey\");\n\n\t\t\t\t\tJSONObject singleOffer = new JSONObject();\n\t\t\t\t\tdouble offer_value = 1.0;\n\t\t\t\t\tdouble offer_cost = 1.0;\n\t\t\t\t\tdouble modified_offer_score = p;\n\t\t\t\t\tif (om) {\n\t\t\t\t\t\tif (offerMatrixWithKey.has(offer)) {\n\n\t\t\t\t\t\t\tsingleOffer = offerMatrixWithKey.getJSONObject(offer);\n\n\t\t\t\t\t\t\tif (singleOffer.has(\"offer_price\"))\n\t\t\t\t\t\t\t\toffer_value = DataTypeConversions.getDouble(singleOffer, \"offer_price\");\n\t\t\t\t\t\t\tif (singleOffer.has(\"price\"))\n\t\t\t\t\t\t\t\toffer_value = DataTypeConversions.getDouble(singleOffer, \"price\");\n\n\t\t\t\t\t\t\tif (singleOffer.has(\"offer_cost\"))\n\t\t\t\t\t\t\t\toffer_cost = singleOffer.getDouble(\"offer_cost\");\n\t\t\t\t\t\t\tif (singleOffer.has(\"cost\"))\n\t\t\t\t\t\t\t\toffer_cost = singleOffer.getDouble(\"cost\");\n\n\t\t\t\t\t\t\tmodified_offer_score = p * ((double) offer_value - offer_cost);\n\t\t\t\t\t\t}\n\t\t\t\t\t}\n\n\t\t\t\t\tJSONObject finalOffersObject = new JSONObject();\n\n\t\t\t\t\tfinalOffersObject.put(\"offer\", offer);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", offer);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name_desc\", option.getString(\"option\"));\n\n\t\t\t\t\t/* process final */\n\t\t\t\t\tfinalOffersObject.put(\"score\", p);\n\t\t\t\t\tfinalOffersObject.put(\"final_score\", p);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", modified_offer_score);\n\t\t\t\t\tfinalOffersObject.put(\"offer_value\", offer_value);\n\t\t\t\t\tfinalOffersObject.put(\"price\", offer_value);\n\t\t\t\t\tfinalOffersObject.put(\"cost\", offer_cost);\n\n\t\t\t\t\tfinalOffersObject.put(\"p\", p);\n\t\t\t\t\tif (option.has(\"contextual_variable_one\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_one\", option.getString(\"contextual_variable_one\"));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_one\", \"\");\n\n\t\t\t\t\tif (option.has(\"contextual_variable_two\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_two\", option.getString(\"contextual_variable_two\"));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_two\", \"\");\n\n\t\t\t\t\tfinalOffersObject.put(\"alpha\", alpha);\n\t\t\t\t\tfinalOffersObject.put(\"beta\", beta);\n\t\t\t\t\tfinalOffersObject.put(\"weighting\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"weighting\")));\n\t\t\t\t\tfinalOffersObject.put(\"explore\", explore);\n\t\t\t\t\tfinalOffersObject.put(\"uuid\", params.get(\"uuid\"));\n\t\t\t\t\tfinalOffersObject.put(\"arm_reward\", arm_reward);\n\n\t\t\t\t\t/* Debugging variables */\n\t\t\t\t\tif (!option.has(\"expected_takeup\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"expected_takeup\", -1.0);\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"expected_takeup\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"expected_takeup\")));\n\n\t\t\t\t\tif (!option.has(\"propensity\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"propensity\", -1.0);\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"propensity\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"propensity\")));\n\n\t\t\t\t\tif (!option.has(\"epsilon_nominated\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"epsilon_nominated\", -1.0);\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"epsilon_nominated\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"epsilon_nominated\")));\n\n\t\t\t\t\tfinalOffers.put(offerIndex, finalOffersObject);\n\t\t\t\t\tofferIndex = offerIndex + 1;\n\t\t\t\t}\n\t\t\t}\n\n\t\t\tJSONArray sortJsonArray = JSONArraySort.sortArray(finalOffers, \"arm_reward\", \"double\", \"d\");\n\t\t\tpredictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n\t\t\tpredictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n\t\t\tdouble endTimePost = System.nanoTime();\n\t\t\tLOGGER.info(\"PlatformDynamicEngagement:I001: time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n\n\t\t} catch (Exception e) {\n\t\t\te.printStackTrace();\n\t\t\tLOGGER.error(e);\n\t\t}\n\n\t\treturn predictModelMojoResult;\n\n\t}\n\n}\n",
         "PostScoreBasic.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport com.ecosystem.utils.DataTypeConversions;\nimport com.ecosystem.utils.JSONArraySort;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\nimport java.util.ArrayList;\n\nimport static com.ecosystem.EcosystemResponse.obtainBudget;\n\n/**\n * This the ecosystem/Ai generic post-score template.\n * Customer plugin for specialized logic to be added to the runtime engine.\n * This class is loaded through the plugin loader system.\n */\npublic class PostScoreBasic extends PostScoreSuper {\n\tprivate static final Logger LOGGER = LogManager.getLogger(PostScoreBasic.class.getName());\n\n\tpublic PostScoreBasic() {\n\t}\n\n\t/**\n\t * Pre-post predict logic\n\t */\n\tpublic void getPostPredict () {\n\t}\n\n\t/**\n\t * getPostPredict\n\t *\n\t * @param predictModelMojoResult Result from scoring\n\t * @param params                 Params carried from input\n\t * @param session                Session variable for Cassandra\n\t * @param models \t\t\t\t Preloaded H2O Models\n\t * @return JSONObject result to further post-scoring logic\n\t */\n\tpublic static JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n\t\tdouble startTimePost = System.nanoTime();\n\t\ttry {\n\t\t\t/* Setup JSON objects for specific prediction case */\n\t\t\tJSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n\t\t\tJSONObject domainsProbabilityObj = new JSONObject();\n\t\t\tif (predictModelMojoResult.has(\"domainsProbabilityObj\"))\n\t\t\t\tdomainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n\n\t\t\t/* If whitelist settings then only allow offers on list */\n\t\t\tboolean whitelist = false;\n\t\t\tArrayList<String> offerWhiteList = new ArrayList<>();\n\t\t\tif (params.has(\"whitelist\")) {\n\t\t\t\tif (!params.getJSONObject(\"whitelist\").isEmpty()) {\n\t\t\t\t\tofferWhiteList = (ArrayList<String>) params.getJSONObject(\"whitelist\").get(\"whitelist\");\n\t\t\t\t\tparams.put(\"resultcount\", offerWhiteList.size());\n\t\t\t\t\twhitelist = DataTypeConversions.getBooleanFromString(params.getJSONObject(\"whitelist\").get(\"logicin\"));\n\t\t\t\t}\n\t\t\t}\n\n\t\t\tif (params.has(\"preloadCorpora\")) {\n\t\t\t\tif (params.getJSONObject(\"preloadCorpora\").has(\"network\")) {\n\t\t\t\t\tJSONObject a = params.getJSONObject(\"preloadCorpora\");\n\t\t\t\t\tJSONObject preloadCorpora = a.getJSONObject(\"network\");\n\t\t\t\t}\n\t\t\t}\n\n\t\t\tJSONArray finalOffers = new JSONArray();\n\t\t\tint resultcount = (int) params.get(\"resultcount\");\n\t\t\t/* For each offer in offer matrix determine eligibility */\n\t\t\t/* get selector field from properties: predictor.selector.setup */\n\t\t\t// String s = new JSONObject(settings.getSelectorSetup()).getJSONObject(\"lookup\").getString(\"fields\");\n\n\t\t\t/** This loop can be used to add number of offers/options to return result */\n\t\t\tJSONObject finalOffersObject = new JSONObject();\n\t\t\tint offerIndex = 0;\n\t\t\tfor (int i = 0; i < resultcount; i++) {\n\n\t\t\t\t/** Model type based approaches */\n\t\t\t\tString type = \"\";\n\t\t\t\tboolean explainability = false;\n\t\t\t\t// LOGGER.info(\"predictModelMojoResult: \" + predictModelMojoResult.toString());\n\t\t\t\tif (predictModelMojoResult.get(\"type\").getClass().getName().toLowerCase().contains(\"array\")) {\n\t\t\t\t\ttype = predictModelMojoResult\n\t\t\t\t\t\t\t.getJSONArray(\"type\")\n\t\t\t\t\t\t\t.get(0)\n\t\t\t\t\t\t\t.toString().toLowerCase().trim();\n\t\t\t\t\tif (predictModelMojoResult.has(\"shapley_contributions\"))\n\t\t\t\t\t\texplainability = true;\n\t\t\t\t} else {\n\t\t\t\t\ttype = ((String) predictModelMojoResult.get(\"type\")).toLowerCase().trim();\n\t\t\t\t}\n\n\t\t\t\t/** Offer name, defaults to type (replace with offer matrix etc) */\n\t\t\t\tif (featuresObj.has(\"offer_name_final\"))\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", featuresObj.get(\"offer_name_final\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", type);\n\n\t\t\t\tif (featuresObj.has(\"offer\"))\n\t\t\t\t\tfinalOffersObject.put(\"offer\", featuresObj.get(\"offer\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"offer\", type);\n\n\t\t\t\tif (featuresObj.has(\"offer_id\"))\n\t\t\t\t\tfinalOffersObject.put(\"offer\", featuresObj.get(\"offer_id\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"offer_id\", type);\n\n\t\t\t\tif (featuresObj.has(\"price\"))\n\t\t\t\t\tfinalOffersObject.put(\"price\", featuresObj.get(\"price\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"price\", 1.0);\n\n\t\t\t\tif (featuresObj.has(\"cost\"))\n\t\t\t\t\tfinalOffersObject.put(\"cost\", featuresObj.get(\"cost\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"cost\", 1.0);\n\n\t\t\t\t/** Score based on model type */\n\t\t\t\tif (type.contains(\"clustering\")) {\n\t\t\t\t\tfinalOffersObject.put(\"cluster\", predictModelMojoResult.getJSONArray(\"cluster\").get(0));\n\t\t\t\t\tfinalOffersObject.put(\"score\", DataTypeConversions.getDouble(domainsProbabilityObj, \"score\"));\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", DataTypeConversions.getDouble(domainsProbabilityObj, \"score\"));\n\t\t\t\t} else if (type.contains(\"anomalydetection\")) {\n\t\t\t\t\tdouble[] score = (double[]) domainsProbabilityObj.get(\"score\");\n\t\t\t\t\tfinalOffersObject.put(\"score\", score[0]);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score[0]);\n\t\t\t\t} else if (type.contains(\"regression\")) {\n\t\t\t\t\tObject score = predictModelMojoResult.getJSONArray(\"value\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score);\n\t\t\t\t} else if (type.contains(\"multinomial\")) {\n\t\t\t\t\tObject probability = predictModelMojoResult.getJSONArray(\"probability\").get(0);\n\t\t\t\t\tObject label = null;\n\t\t\t\t\ttry {\n\t\t\t\t\t\tlabel = predictModelMojoResult.getJSONArray(\"label\").get(0);\n\t\t\t\t\t} catch (Exception e) {\n\t\t\t\t\t\tLOGGER.error(\"PostScoreBasic:getPostPredict:E001: Error relates to scoring your model. The model wasn't loaded or is not accessible.\");\n\t\t\t\t\t\te.printStackTrace();\n\t\t\t\t\t}\n\t\t\t\t\tObject response = predictModelMojoResult.getJSONArray(\"response\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", probability);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", probability);\n\t\t\t\t\tfinalOffersObject.put(\"offer\", label);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", response);\n\t\t\t\t} else if (type.contains(\"coxph\")) {\n\t\t\t\t\tObject score = predictModelMojoResult.getJSONArray(\"value\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score);\n\t\t\t\t} else if (type.contains(\"wordembedding\")) {\n\t\t\t\t\tfloat[] score = (float[]) predictModelMojoResult.getJSONArray(\"_text_word2vec\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", Double.valueOf(String.valueOf(score[0])));\n\t\t\t\t\tfinalOffersObject.put(\"embedding\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", 0.0);\n\t\t\t\t} else if (type.contains(\"deeplearning\")) {\n\t\t\t\t\t/** From TensorFlow or PyTorch */\n\t\t\t\t\tObject score = domainsProbabilityObj.getDouble(\"1\");\n\t\t\t\t\tfinalOffersObject.put(\"score\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score);\n\t\t\t\t\tObject response = predictModelMojoResult.getJSONArray(\"response\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", response);\n\t\t\t\t} else if (type.contains(\"empty score\")) {\n\t\t\t\t\t/** This is typically used for data lookup only, obtain values from feature store! */\n\t\t\t\t\tif (featuresObj.has(\"offer_name\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"offer_name\", featuresObj.get(\"offer_name\"));\n\n\t\t\t\t\tif (featuresObj.has(\"offer\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"offer\", featuresObj.get(\"offer\"));\n\n\t\t\t\t\tif (featuresObj.has(\"score\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"score\", Double.valueOf(String.valueOf(featuresObj.get(\"score\"))));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"score\", 1.0);\n\n\t\t\t\t\tif (featuresObj.has(\"modified_offer_score\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", Double.valueOf(String.valueOf(featuresObj.get(\"modified_offer_score\"))));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", 1.0);\n\n\t\t\t\t\tif (featuresObj.has(\"cost\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"cost\", Double.valueOf(String.valueOf(featuresObj.get(\"cost\"))));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"cost\", 0.0);\n\n\t\t\t\t} else {\n\t\t\t\t\tfinalOffersObject.put(\"score\", 1.0);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", 1.0);\n\t\t\t\t}\n\n\t\t\t\tfinalOffersObject.put(\"offer_details\", domainsProbabilityObj);\n\t\t\t\tif (explainability) {\n\t\t\t\t\tfinalOffersObject.put(\"shapley_contributions\", predictModelMojoResult.get(\"shapley_contributions\"));\n\t\t\t\t\tfinalOffersObject.put(\"shapley_contributions_names\", predictModelMojoResult.get(\"shapley_contributions_names\"));\n\t\t\t\t}\n\n\t\t\t\t/** Default value, could be replaced by offer matrix or feature store */\n\t\t\t\tdouble offer_value = 1.0;\n\t\t\t\tfinalOffersObject.put(\"offer_value\", offer_value);\n\t\t\t\tfinalOffersObject.put(\"uuid\", params.get(\"uuid\"));\n\n\t\t\t\t/** Add other structures to the final result */\n\t\t\t\tfinalOffersObject.put(\"offer_matrix\", featuresObj);\n\n\t\t\t\t/** Budget processing option, if it's set in the properties */\n\t\t\t\tif (settings.getPredictorOfferBudget() != null) {\n\t\t\t\t\tJSONObject budgetItem = obtainBudget(featuresObj, params.getJSONObject(\"featuresObj\"), offer_value);\n\t\t\t\t\tdouble budgetSpendLimit = budgetItem.getDouble(\"spend_limit\");\n\t\t\t\t\tfinalOffersObject.put(\"spend_limit\", budgetSpendLimit);\n\t\t\t\t}\n\n\t\t\t\t/** Prepare offer array before final sorting */\n\t\t\t\tfinalOffers.put(offerIndex, finalOffersObject);\n\t\t\t\tofferIndex = offerIndex + 1;\n\t\t\t}\n\n\t\t\t/** Sort final offer list based on score */\n\t\t\tJSONArray sortJsonArray = JSONArraySort.sortArray(finalOffers, \"score\", \"double\", \"d\");\n\t\t\tpredictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n\t\t} catch (Exception e) {\n\t\t\tLOGGER.error(e);\n\t\t}\n\n\t\t/** Get top scores and test for explore/exploit randomization */\n\t\tpredictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n\t\tdouble endTimePost = System.nanoTime();\n\t\tLOGGER.info(\"getPostPredict:I001: execution time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n\t\treturn predictModelMojoResult;\n\t}\n\n}\n",
@@ -120,65 +122,174 @@
         max_version = max(version_list)
         post_score_logic = [i["plugins"]["post_score_class_code"] for i in project_details["deployment_step"] if
                         (i["plugins"]["post_score_class_text"] == post_score and i["version"] == max_version)][0]
     elif post_score in post_score_code_options:
         post_score_logic = post_score_code_options[post_score]
     else:
         print(
-            "WARNING: post_score_class not found in default options or existing deployments in project. Empty class saved to the deployment. To edit the class use the ecosystem.Ai plugin for IntelliJ or the ecosystem.Ai workbench")
+            "WARNING: post_score_class not found in default options or existing deployments in project. Empty class "
+            "saved to the deployment. To edit the class use the ecosystem.Ai plugin for IntelliJ or the ecosystem.Ai "
+            "workbench")
         post_score_logic = ""
     return post_score_logic
 
+
 def create_deployment(
         auth,
         project_id,
         deployment_id,
         description,
         plugin_pre_score_class,
         plugin_post_score_class,
         version,
         project_status,
+        mongo_connect,
+        mongo_server_port,
+        mongo_ecosystem_password,
+        mongo_ecosystem_user,
         budget_tracker="default",
         complexity="Low",
         performance_expectation="High",
         model_configuration="default",
         setup_offer_matrix="default",
         multi_armed_bandit="default",
         whitelist="default",
         model_selector="default",
         pattern_selector="default",
         logging_collection_response="ecosystemruntime_response",
         logging_collection="ecosystemruntime",
         logging_database="logging",
-        mongo_connect="mongodb://ecosystem_user:EcoEco321@ecosystem-server:54445/?authSource=admin",
-        mongo_server_port="ecosystem-server:54445",
-        mongo_ecosystem_password="EcoEco321",
-        mongo_ecosystem_user="ecosystem_user",
         scoring_engine_path_dev="http://ecosystem-runtime:8091",
         scoring_engine_path_test="http://ecosystem-runtime2:8091",
         scoring_engine_path_prod="http://ecosystem-runtime3:8091",
         models_path="/data/deployed/",
         data_path="/data/",
         build_server_path="",
         git_repo_path_branch="",
         download_path="",
         git_repo_path="",
         parameter_access="default",
         corpora="default",
         extensive_validation=False
 ):
-    #######################################################################################################################
+    """
+    Create or update a deployment linked to an existing project.
+
+   :param auth: Token for accessing the ecosystem-server. Created using the jwt_access package.
+   :param project_id: The name of the project to add the deployment step to.
+   :param deployment_id: The name of the deployment step that is to be created.
+   :param description: Description of the deployment step
+   :param version: The version of the deployment step being created. The combination of version and deployment_id cannot already exists within the deployment, i.e. you cannot overwrite an existing deployment
+   :param project_status: Specifies the environment to which the deployment should be sent when it is pushed. The allowed values are experiment, validate, production, disable.
+   :param plugin_pre_score_class: The name of the pre score logic class to be used in the runtime. Only default classes can be selected here. To create custom classes please use the ecosystem-runtime-locabuild repo or edit the classes in the workbench. The allowed values are PrePredictCustomer.java
+   :param plugin_post_score_class: The name of the post score logic class to be used in the runtime. Only default classes can be selected here. To create custom classes please use the ecosystem-runtime-locabuild repo or edit the classes in the workbench. The allowed values are PostScoreBasic.java, PostScoreRecommender.java, PlatformDynamicEngagement.java, PostScoreRecommenderOffers.java, PostScoreRecommenderMulti.java and PostScoreNetwork.java
+   :param budget_tracker: A dictionary of parameters required for managing the budget tracker functionality.
+   :param complexity: Indicate the expected complexity of the deployment, allowed values are Low, Medium and High
+   :param performance_expectation: Indicate the expected performance of the deployment, allowed values are Low, Medium and High
+   :param model_configuration: A dictionary of the parameters specifying the models used in the project. The key item in the dictionary is models_load - a comma separated string of the names of the models to be used in the deployment. model_note and model_outline fields can also be added for tracking purposes
+   :param setup_offer_matrix: A dictionary of parameters specifying the location of the offer matrix - a dataset containing information about the offers that could be recommended. The dictionary must contain a datasource, database, collection and offer_lookup_id. Datasource can be one of mongodb, cassandra or presto. Database and collection specify the location of the offer_matrix in the datasource. Offer_lookup_id is the name of the column which contains the unique identifier for the offers - allowed values are offer, offer_name and offer_id
+   :param multi_armed_bandit: A dictionary specifying the dynamic recommender behavior of the deployment. The dictionary must contain epsilon, duration and pulse_responder_id. epsilon is a portion of interactions that are presented with random results and should be a number between 0 and 1. duration is the period for which recommendations are cached in milliseconds TODO <Check this with Jay> . pulse_responder_id is the uuid of a Dynamic Interaction configuration, if not Dynamic Interaction configuration is being linked set this to ""
+   :param whitelist: A dictionary of parameters specifying the location of the whitelist - a dataset of customers and the list of offers for which they are eligible. The data set should contain two fields; customer_key and white_list. customer_key is the unique customer identifier and white_list is a list of offer_names for which the customer is eligible. The dictionary must contain a datasource, database and collection. Datasource can be one of mongodb, cassandra or presto. Database and collection specify the location of the whitelist in the datasource.
+   :param model_selector: A dictionary of parameters specifying the behavior of the model selector functionality. The model selector allows different models to be used based on the value of a field in the specified data set. The dictionary must contain datasource, database, table_collection, selector_column, selector and lookup.  Datasource can be one of mongodb, cassandra or presto. Database and collection specify the location of the model_selector dataset in the datasource. The selector_column is the name of the column in the dataset which is used to select between the different models. Lookup is a dictionary with the structure {"key":"customer","value":123 or '123',"fields'':"selector_column"}, where key is the field containing the unique customer identifier, value specified the type of the identifier as either a string ('123') or a number (123) and fields is the name of the selector column. Selector is the rule set used to choose models based on the values in the selector column. Selector is a dictionary with the format {"key_value_a":[0],"key_value_b":[1], ...} where the keys are the values of the fields in the selector column used to choose different models and the values are the indices of the model to be used, with the order as specified in the model_configuration argument
+   :param pattern_selector: A dictionary containing the parameters defining the behavior of the pattern selector. The dictionary contains two parameters; pattern and duration. pattern is a comma separated list of numbers which specifies the intervals at which customers are able to receive updated offers. duration defines the time intervals specified in the pattern parameter
+   :param parameter_access: A dictionary specifying the location from which customer data should be looked up. parameter_access should contain lookup, datasource, database, table_collection, lookup, lookup_defaults, fields, lookup_fields, create_virtual_variables and virtual_variables. lookup is a dictionary with the structure {"key":"customer","value":123 or '123'}, where key is the field containing the unique customer identifier, value specified the type of the identifier as either a string ('123') or a number (123). datasource can be one of mongodb, cassandra or presto. database and table_collection specify the location of the customer lookup in the datasource. fields is a comma separated list of the fields that should be read from the customer lookup. lookup_defaults are the default values to be used if the customer lookup fails, set to "" to not specify defaults. lookup_fields is the fields parameter in a list form ordered alphabetically create_virtual_variable is True if virtual variables are defined and False if not, virtual variables are defined by segmenting or combining fields from the customer lookup for us in the deployment. virtual_variables is a dictionary defining the virtual variables, which has the following form.
+   :param corpora: A list of additional datasets that are read by the deployment. corpora is a list of dictionaries where each dictionary gives the details of a data set. The dictionaries must have the following keys; database (mongodb or cassandra), db (the database containing the corpora), table (the collection containing the corpora), name (the name of the corpora used in the deployment) and type (static, dynamic or experiment). The dictionary can optionally contain a key field which, if present, is used as a lookup for each row or the corpora, where the default is to have the rows loaded as an array. The type field in the dictionary specifies how the corpora is loaded. A static type is loaded at deployment, a dynamic type is loaded at each prediction and experiment is a special type used for configuring network runtimes
+   :param logging_database: The mongo database where the deployment logs will be stored
+   :param logging_collection: The mongo collection where the predictions presented will be stored
+   :param logging_collection_response: The mongo collection where the customer responses to the predictions will be stored
+   :param mongo_connect: The connection string to the mongo database used by the deployment
+   :param mongo_server_port: The server and port in the mongo connection string
+   :param mongo_ecosystem_password: The password in the mongo connection string
+   :param mongo_ecosystem_user: The username in the mongo connection string
+   :param scoring_engine_path_dev: The url of the container to send the configuration to when the project status is experiment
+   :param scoring_engine_path_test: The url of the container to send the configuration to when the project status is validate
+   :param scoring_engine_path_prod: The url of the container to send the configuration to when the project status is production
+   :param models_path: The folder in the container where the models will be stored
+   :param data_path: The folder in the container where the generic data used by the container will be stored
+   :param build_server_path: The url of the build server to be used if customer logic is built into the container and a new container needs to be built containing said logic
+   :param git_repo_path: The git repo to store the customer logic
+   :param git_repo_path_branch: The branch to use for the repo specified in git_repo_path_branch
+   :param download_path: The url on Docker Hub where the built container will be pushed
+   :param extensive_validation: Indicator of whether potentially time consuming validation should be run before the deployment is created. This additional validation is checking whether the fields in the model_parameter are present in the linked collection and vice-versa
+
+   :return: The deployment configuration.
+
+   EXAMPLES:
+
+   Deployment creation example for an online learning configuration with an offer matrix, customer lookup, virtual variables
+   and a dynamic corpora specifying a default offer.
+
+   .. code-block:: python
+
+       deployment_step = dm.create_deployment(
+            auth_local,
+            project_id=project_id,
+            deployment_id="demo_online_learning",
+            description="Demonstration of online learning deployment",
+            plugin_pre_score_class="",
+            plugin_post_score_class="PostScoreDemoDynamic.java",
+            version="001",
+            project_status="experiment",
+            scoring_engine_path_dev="http://ecosystem-runtime:8091",
+            multi_armed_bandit={
+                        "epsilon": 0,
+                        "duration": 0,
+                        "pulse_responder_uuid": online_learning_uuid
+                        },
+            setup_offer_matrix={
+                        "offer_lookup_id": "offer_name",
+                        "database": "recommender",
+                        "table_collection": "online_offer_matrix",
+                        "datasource": "mongodb"
+                    },
+            corpora=[{ "name":"default_offer","database":"mongodb","db":"recommender","table":"online_default_offer","type":"static"}],
+            parameter_access={
+                        "lookup": {"value": 123,"key": "customer"},
+                        "create_virtual_variables":True,
+                        "lookup_defaults": "",
+                        "database": "recommender",
+                        "table_collection": "customer_feature_store",
+                        "lookup_fields": ["customer","revenue","activity","age",...],
+                        "datasource": "mongodb",
+                        "virtual_variables": [
+                            {
+                                "name": "revenue_category",
+                                "default": "gt-500",
+                                "type": "discretize",
+                                "original_variable": "revenue",
+                                "fields": [],
+                                "buckets": [
+                                    {"from": 0,"label": "lt-50","to": 50},
+                                    {"from": 50,"label": "50-250","to": 250},
+                                    {"from": 250,"label": "250-500","to": 500}
+                                ]
+                            },
+                            {
+                                "name": "activity_category",
+                                "default": "gt-15",
+                                "type": "discretize",
+                                "original_variable": "activity",
+                                "fields": [],
+                                "buckets": [
+                                    {"from": 0,"label": "lt-15","to": 15}
+                                ]
+                            }
+                        ]
+                    }
+       )
+
+    """
     # Check inputs have the required format and get default values where relevant
-    #######################################################################################################################
     # Get prediction project details and check that project exists
     try:
         project_details = pe.get_prediction_project(auth, project_id)
     except JSONDecodeError as error:
         raise ValueError(
-            "No project found with the given project ID. Please create your project before allocating deployments to it") from error
+            "No project found with the given project ID. Please create your project before allocating deployments to "
+            "it") from error
 
     # Get the dynamic confiugration details and check that the dynamic configuration exists
     if multi_armed_bandit == "default":
         multi_armed_bandit = get_multi_armed_bandit_default()
         is_multi_armed_bandit = False
     else:
         is_multi_armed_bandit = True
@@ -207,28 +318,30 @@
                 if dynamic_config_iter["uuid"] == multi_armed_bandit["pulse_responder_uuid"]:
                     found_pulse_responder = True
                     dynamic_config = dynamic_config_iter
             if not found_pulse_responder:
                 raise ValueError(
                     "pulse_responder_id in multi_armed_bandit not linked to a dynamic recommender configuration")
 
-    # Check that deployment_id is a string that doens't contain spaces and matches the dynamic configuration name if it exists
+    # Check that deployment_id is a string that doesn't contain spaces and matches the dynamic configuration name if it
+    # exists
     if not isinstance(deployment_id, str):
         raise TypeError("deployment_id should be a string")
     if multi_armed_bandit["pulse_responder_uuid"] != "":
         if deployment_id != dynamic_config["name"]:
             raise ValueError("deployment step and dynamic recommender should have the same name")
 
     # Check whether version already exists and that it is a string
     if not isinstance(version, str):
         raise TypeError("version should be a string")
     if "deployment_step" in project_details:
         for deployment_iter in project_details["deployment_step"]:
             if (version == deployment_iter["version"]) and (deployment_id == deployment_iter["deployment_id"]):
-                raise ValueError("The version specified for this deployment already exists, deployment not updated. Please update the version to update the deployment")
+                raise ValueError("The version specified for this deployment already exists, deployment not updated. "
+                                 "Please update the version to update the deployment")
 
     # Check that description is a string
     if not isinstance(description, str):
         raise TypeError("description should be a string")
 
     # Check that project status has an allowed value
     if project_status not in ["experiment", "validate", "production", "disable"]:
@@ -330,26 +443,29 @@
         if setup_offer_matrix["datasource"] not in ["mongodb", "cassandra", "presto"]:
             raise ValueError("datasource in setup_offer_matrix must be cassandra, mongodb or presto")
         if not isinstance(setup_offer_matrix["database"], str):
             raise TypeError("database in setup_offer_matrix should be a string")
         if not isinstance(setup_offer_matrix["table_collection"], str):
             raise TypeError("table_collection in setup_offer_matrix should be a string")
         if setup_offer_matrix["offer_lookup_id"] not in ["offer", "offer_id", "offer_name"]:
-            raise ValueError("offer_lookup_id in setup_offer_matrix must be offer, offer_name or presto")
+            raise ValueError("offer_lookup_id in setup_offer_matrix must be offer, offer_name or offer_id ")
         if setup_offer_matrix["datasource"] == "mongodb" and test_mongo_connection:
             db_offer_matrix = test_client[setup_offer_matrix["database"]]
-            if db_offer_matrix[setup_offer_matrix["collection"]].estimated_document_count() == 0:
+            if db_offer_matrix[setup_offer_matrix["table_collection"]].estimated_document_count() == 0:
                 print("WARNING: It looks like the offer matrix is empty")
             else:
-                test_offer_matrix_row = db_offer_matrix[setup_offer_matrix["collection"]].find_one().next()
+                test_offer_matrix_row = db_offer_matrix[setup_offer_matrix["table_collection"]].find().next()
                 if setup_offer_matrix["offer_lookup_id"] not in test_offer_matrix_row:
                     print("WARNING: It looks like the specified offer_lookup_id is not a field in the offer matrix")
         elif setup_offer_matrix["datasource"] == "cassandra" and test_cassandra_connection:
-            # TODO: Implement cassandra checks once Ramsay has added APIs
-            print("WARNING: cassandra connection could not be tested")
+            data_check = dme.get_cassandra_sql(auth, "SELECT * FROM {} LIMIT 1".format(setup_offer_matrix["table_collection"]))
+            if data_check["data"] == []:
+                print("WARNING: It looks like the offer matrix is empty or does not exist")
+            elif setup_offer_matrix["offer_lookup_id"] not in data_check["data"][0]:
+                print("WARNING: It looks like the specified offer_lookup_id is not a field in the offer matrix")
         elif setup_offer_matrix["datasource"] == "presto" and test_presto_connection:
             # TODO: Ask Jay how Presto connection works and figure our how to implement test on Presto Connection
             print("WARNING: presto connection could not be tested")
 
     # Check that the whitelist has the required format
     if whitelist == "default":
         whitelist = get_whitelist_default()
@@ -371,22 +487,27 @@
         if not isinstance(whitelist["collection"], str):
             raise TypeError("collection in whitelist should be a string")
         if whitelist["datasource"] == "mongodb" and test_mongo_connection:
             db_whitelist = test_client[whitelist["database"]]
             if db_whitelist[whitelist["collection"]].estimated_document_count() == 0:
                 print("WARNING: It looks like the whitelist is empty")
             else:
-                test_whitelist_row = db_whitelist[whitelist["collection"]].find_one().next()
+                test_whitelist_row = db_whitelist[whitelist["collection"]].find().next()
                 if "customer_key" not in test_whitelist_row:
                     print("WARNING: It looks like customer_key is not a field in the white list")
                 if "white_list" not in test_whitelist_row:
                     print("WARNING: It looks like white_list is not a field in the white list")
         elif whitelist["datasource"] == "cassandra" and test_cassandra_connection:
-            # TODO: Implement cassandra checks once Ramsay has added APIs
-            print("WARNING: cassandra connection could not be tested")
+            data_check = dme.get_cassandra_sql(auth, "SELECT * FROM {} LIMIT 1".format(whitelist["collection"]))
+            if data_check["data"] == []:
+                print("WARNING: It looks like the whitelist is empty or does not exist")
+            elif "customer_key" not in data_check["data"][0]:
+                print("WARNING: It looks like customer_key is not a field in the white list")
+            elif "white_list" not in data_check["data"][0]:
+                print("WARNING: It looks like white_list is not a field in the white list")
         elif whitelist["datasource"] == "presto" and test_presto_connection:
             # TODO: Ask Jay how Presto connection works and figure our how to implement test on Presto Connection
             print("WARNING: presto connection could not be tested")
 
     # Check that the model selector has the required format
     if model_selector == "default":
         model_selector = get_model_selector_default()
@@ -424,15 +545,15 @@
         if not isinstance(model_selector["table_collection"], str):
             raise TypeError("table_collection in model_selector should be a string")
         if model_selector["datasource"] == "mongodb" and test_mongo_connection:
             db_model_selector = test_client[model_selector["database"]]
             if db_model_selector[model_selector["table_collection"]].estimated_document_count() == 0:
                 print("WARNING: It looks like the model_selector is empty")
             else:
-                test_model_selector_row = db_model_selector[model_selector["table_collection"]].find_one().next()
+                test_model_selector_row = db_model_selector[model_selector["table_collection"]].find().next()
                 if model_selector["selector_column"] not in test_model_selector_row:
                     print("WARNING: It looks like selector_column is not a field in the model selector collection")
                 elif extensive_validation:
                     selector_values_cursor = db_model_selector[model_selector["table_collection"]].aggregate([{
                                                                                                                   "$group": {
                                                                                                                       "_id": "None",
                                                                                                                       "selector_values": {
@@ -447,18 +568,21 @@
                                 selector_value_in_dataset_iter) + " in the model selector database but not in the selector in the model_selector. If this row is looked up by the runtime a default value will be returned")
                     for selector_value_in_args_iter in model_selector["selector"]:
                         if selector_value_in_args_iter not in selector_values_in_dataset:
                             print("WARNING: " + str(
                                 selector_value_in_args_iter) + " in the selector in the model_selector is not present in the model selector dataset")
                 if model_selector["lookup"]["key"] not in test_model_selector_row:
                     print(
-                        "WARNING: It looks like key in the lookup in model_seelector is not a field in the model selector collection")
+                        "WARNING: It looks like key in the lookup in model_selector is not a field in the model selector collection")
         elif whitelist["datasource"] == "cassandra" and test_cassandra_connection:
-            # TODO: Implement cassandra checks once Ramsay has added APIs
-            print("WARNING: cassandra connection could not be tested")
+            data_check = dme.get_cassandra_sql(auth, "SELECT * FROM {} LIMIT 1".format(model_selector["table_collection"]))
+            if data_check["data"] == []:
+                print("WARNING: It looks like the model_selector is empty or does not exist")
+            elif model_selector["selector_column"] not in data_check["data"][0]:
+                print("WARNING: It looks like selector_column is not a field in the model selector collection")
         elif whitelist["datasource"] == "presto" and test_presto_connection:
             # TODO: Ask Jay how Presto connection works and figure our how to implement test on Presto Connection
             print("WARNING: presto connection could not be tested")
 
     # Check whether pattern selector contains the required parameters
     if pattern_selector == "default":
         pattern_selector = get_pattern_selector_default()
@@ -501,24 +625,28 @@
                 if corpora_key not in ["name", "database", "db", "table", "type", "key"]:
                     raise KeyError("corpora dictionaries can only contain name, database, db, table, type and key")
             if corpora_iter["database"] not in ["mongodb", "cassandra"]:
                 raise ValueError("database in corpora must be cassandra or mongodb")
             if corpora_iter["type"] not in ["static", "dynamic", "experiment"]:
                 raise ValueError("type in corpora must be static, dynamic or experiment")
             if corpora_iter["database"] == "mongodb" and test_mongo_connection:
-                db_corpora = test_client[corpora_iter["database"]]
+                db_corpora = test_client[corpora_iter["db"]]
                 if db_corpora[corpora_iter["table"]].estimated_document_count() == 0:
-                    print("WARNING: It looks like the corpora is empty")
+                    print("WARNING: It looks like the corpora {} is empty".format(corpora_iter["table"]))
                 elif "key" in corpora_iter:
-                    test_corpora_row = db_corpora[corpora_iter["table"]].find_one().next()
+                    test_corpora_row = db_corpora[corpora_iter["table"]].find().next()
                     if corpora_iter["key"] not in test_corpora_row:
                         print("WARNING: It looks like the specified key is missing from the corpora")
             elif corpora_iter["database"] == "cassandra" and test_cassandra_connection:
-                # TODO: Implement cassandra checks once Ramsay has added APIs
-                print("WARNING: cassandra connection could not be tested")
+                data_check = dme.get_cassandra_sql(auth, "SELECT * FROM {} LIMIT 1".format(corpora_iter["table"]))
+                if data_check["data"] == []:
+                    print("WARNING: It looks like the corpora {} is empty".format(corpora_iter["table"]))
+                elif "key" in corpora_iter:
+                    if corpora_iter["key"] not in data_check["data"][0]:
+                        print("WARNING: It looks like the specified key is missing from the corpora")
         corpora = {"corpora": json.dumps(corpora)}
 
     if parameter_access == "default":
         parameter_access = get_parameter_access_default()
         is_params_from_data_source = False
     else:
         is_params_from_data_source = True
@@ -561,31 +689,39 @@
         if not isinstance(parameter_access["virtual_variables"], list):
             raise TypeError("virtual_variables in parameter_access should be a list")
         if parameter_access["datasource"] == "mongodb" and test_mongo_connection:
             db_parameter_access = test_client[parameter_access["database"]]
             if db_parameter_access[parameter_access["table_collection"]].estimated_document_count() == 0:
                 print("WARNING: It looks like the parameter_access collection is empty")
             else:
-                test_parameter_access_row = db_parameter_access[parameter_access["collection"]].find_one().next()
+                test_parameter_access_row = db_parameter_access[parameter_access["table_collection"]].find().next()
                 if parameter_access["lookup"]["key"] not in test_parameter_access_row:
                     print("WARNING: It looks like the specified key is not a field in the parameter_access collection")
                 if type(test_parameter_access_row[parameter_access["lookup"]["key"]]) != type(
                         parameter_access["lookup"]["value"]):
-                    print(
-                        "WARNING: It looks like value specified in the lookup in parameter_access does not match the type found in the collection")
+                    print("WARNING: It looks like value specified in the lookup in parameter_access does not match the type found in the collection")
         elif parameter_access["datasource"] == "cassandra" and test_cassandra_connection:
-            # TODO: Implement cassandra checks once Ramsay has added APIs
-            print("WARNING: cassandra connection could not be tested")
+            data_check = dme.get_cassandra_sql(auth, "SELECT * FROM {} LIMIT 1".format(parameter_access["table_collection"]))
+            type_sql = "SELECT type FROM system_schema.columns WHERE keyspace_name = '{}' AND table_name = '{}' AND column_name = '{}'".format(parameter_access["table_collection"].split(".")[0],parameter_access["table_collection"].split(".")[1],parameter_access["lookup"]["key"])
+            if data_check["data"] == []:
+                print("WARNING: It looks like the parameter_access collection is empty")
+            elif parameter_access["lookup"]["key"] not in data_check["data"][0]:
+                print("WARNING: It looks like the specified key is not a field in the parameter_access collection")
+            else:
+                cassandra_type = dme.get_cassandra_sql(auth, type_sql)["data"][0]["type"]
+                if cassandra_type == "text" and not isinstance(parameter_access["lookup"]["value"], str):
+                    print("WARNING: It looks like value specified in the lookup in parameter_access does not match the type found in the collection")
+                elif cassandra_type != "text" and isinstance(parameter_access["lookup"]["value"], str):
+                    print("WARNING: It looks like value specified in the lookup in parameter_access does not match the type found in the collection")
         elif parameter_access["datasource"] == "presto" and test_presto_connection:
             # TODO: Ask Jay how Presto connection works and figure our how to implement test on Presto Connection
             print("WARNING: presto connection could not be tested")
 
-    #######################################################################################################################
     # Define constructs needed to create the deployment and add the deployment to the project
-    #######################################################################################################################
+
     multi_armed_bandit["epsilon"] = str(multi_armed_bandit["epsilon"])
 
     options = {
         "is_offer_matrix": is_offer_matrix,
         "is_multi_armed_bandit": is_multi_armed_bandit,
         "is_enable_plugins": True,
         "is_whitelist": is_whitelist,
@@ -675,15 +811,15 @@
             client_pulse_list = [d for d in existing_configurations["data"] if
                                  d["uuid"] == multi_armed_bandit["pulse_responder_uuid"]]
             client_pulse_doc = client_pulse_list[0]
             if "fields" in parameter_access:
                 client_pulse_doc["lookup_fields"] = parameter_access["fields"]
             if "virtual_variables" in parameter_access:
                 client_pulse_doc["virtual_variables"] = parameter_access["virtual_variables"]
-            d.add_documents(auth, {"database": "ecosystem_meta", "collection": "dynamic_engagement",
+            dme.add_documents(auth, {"database": "ecosystem_meta", "collection": "dynamic_engagement",
                                    "document": client_pulse_doc, "update": "uuid"})
 
     print("MESSAGE: Project deployment created")
     return deployment_step
 
 
 def create_project(
@@ -698,14 +834,33 @@
         data_lead,
         module_name="",
         module_module_owner="",
         module_description="",
         module_created_by="",
         module_version="",
 ):
+    """
+    Create a new project
+
+   :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+   :param project_id: The name of the project to be created.
+   :param project_description: Description of the project.
+   :param project_type: The type of the project.
+   :param purpose: The purpose of the project.
+   :param project_start_date: The start date of the project.
+   :param project_end_date: The end date of the project.
+   :param data_science_lead: The data science lead of the project.
+   :param data_lead: The data lead of the project.
+   :param module_name: The name of the module.
+   :param module_module_owner: The owner of the module.
+   :param module_description: The description of the module.
+   :param module_created_by: The creator of the module.
+   :param module_version: The version of the module.
+
+    """
     if not isinstance(project_id, str):
         raise TypeError("project_id should be a string")
     if not isinstance(project_description, str):
         raise TypeError("project_description should be a string")
     if not isinstance(project_type, str):
         raise TypeError("project_type should be a string")
     if not isinstance(purpose, str):
@@ -783,7 +938,387 @@
         , "updated_date": updated_date
         , "userid": "ecosystem"
     }
     pe.save_prediction_project(auth, project_doc)
 
     print("MESSAGE: Project created")
     return project_doc
+
+
+def link_collections_to_project(auth, project_id, collections):
+    """
+    Link collections to a project
+
+    :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+    :param project_id: The name of the project to link the collections to.
+    :param collections: The collections to link to the project in the format [{"database":"linked_database","collection":"linked_collection"}]
+    """
+    if not isinstance(project_id, str):
+        raise TypeError("project_id should be a string")
+    if not isinstance(collections, list):
+        raise TypeError("collections should be a list of dictionaries")
+    for collection_iter in collections:
+        if not isinstance(collection_iter, dict):
+            raise TypeError("collections should be a list of dictionaries")
+        if "database" not in collection_iter:
+            raise KeyError("collections dictionaries must contain database")
+        if "collection" not in collection_iter:
+            raise KeyError("collections dictionaries must contain collection")
+        for collection_key in collection_iter:
+            if collection_key not in ["database", "collection"]:
+                raise KeyError("collections dictionaries can only contain database and collection")
+            if not isinstance(collection_iter[collection_key], str):
+                raise TypeError("collection and database should contain strings")
+
+    project_details = pe.get_prediction_project(auth, project_id)
+    project_details["project_collections"] = collections
+    pe.save_prediction_project(auth, project_details)
+
+    return "MESSAGE: Collections linked to project"
+
+def link_dynamic_interactions_to_project(auth, project_id, interactions):
+    """
+    Link dynamic interactions to a project
+
+    :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+    :param project_id: The name of the project to link the interactions to.
+    :param interactions: The interactions to link to the project in the format [{"uuid":"f4990ecd-d438-4260-85ae-fc1fd915a266}]
+    """
+    if not isinstance(project_id, str):
+        raise TypeError("project_id should be a string")
+    if not isinstance(interactions, list):
+        raise TypeError("interactions should be a list of dictionaries")
+    for interaction_iter in interactions:
+        if not isinstance(interaction_iter, dict):
+            raise TypeError("interactions should be a list of dictionaries")
+        if "uuid" not in interaction_iter:
+            raise KeyError("interactions dictionaries must contain uuid")
+        for interaction_key in interaction_iter:
+            if interaction_key not in ["uuid"]:
+                raise KeyError("interactions dictionaries can only contain uuid")
+            if not isinstance(interaction_iter[interaction_key], str):
+                raise TypeError("uuid should be a string")
+
+    project_details = pe.get_prediction_project(auth, project_id)
+    dynamic_interactions = cp.list_pulse_responder_dynamic(auth)
+    uuid_list = [d["uuid"] for d in interactions]
+    linked_interactions = []
+    for dynamic_iter in dynamic_interactions["data"]:
+        if dynamic_iter["uuid"] in uuid_list:
+            linked_interactions.append({"uuid": dynamic_iter["uuid"], "name": dynamic_iter["name"], "date": dynamic_iter["date_updated"]})
+
+    project_details["project_dynamic_interactions"] = linked_interactions
+    pe.save_prediction_project(auth, project_details)
+
+    return "MESSAGE: Interactions linked to project"
+
+def single_test_calls(auth_runtime, testing_config, output_level):
+    """
+    Test the runtime by making individual calls and checking the response against user defined criteria
+
+    param: auth_runtime: The authentication object for the runtime
+    param: testing_config: The testing configuration
+    param: output_level: The level of output to print. Options are "quiet" and "verbose"
+
+    return: True if the tests pass, False otherwise
+    """
+    # Iterate through the testing config and call the runtime
+    # {
+    # "api_call":{
+    #             "campaign": deployment_id
+    #             , "subcampaign": "none"
+    #             , "channel": "notebooks"
+    #             , "customer": 27822914182
+    #             , "userid": "test"
+    #             , "numberoffers": 4
+    #             , "params": "{}"
+    #             }
+    # ,"check_offer_count":"Yes"
+    # ,"check_offer_response":"No"
+    # ,"expected_offer":""
+    # }
+    for test_iter in testing_config["individual_tests"]:
+        try:
+            offer_response = o.invocations(auth_runtime, test_iter["api_call"])
+            if output_level != "quiet":
+                print("Offer response:")
+                print(offer_response)
+        except Exception as e:
+            print("Error in runtime_test_individual_calls calling runtime: {0}".format(e))
+            return False
+
+        # Test the response
+        try:
+            # At a minimum, the response should contain a final_result key which is not an empty list
+            if "final_result" not in offer_response:
+                print("Error: final_result not in response")
+                return False
+            if offer_response["final_result"] == []:
+                print("Error: final_result is empty")
+                return False
+            if test_iter["check_offer_count"] == "Yes":
+                if len(offer_response["final_result"]) != test_iter["api_call"]["numberoffers"]:
+                    print("Error: number of offers is not {0}".format(test_iter["api_call"]["numberoffers"]))
+                    return False
+            if test_iter["check_offer_response"] == "Yes":
+                if offer_response["final_result"][0]["result"]["offer"] != test_iter["expected_offer"]:
+                    print("Error: {0} returned".format(offer_response["final_result"][0]["result"]["offer"]))
+                    return False
+        except Exception as e:
+            print("Error in runtime_test_individual_calls: {0}".format(e))
+            return False
+
+    return True
+
+
+def distribution_test(auth, auth_runtime, testing_config, output_level):
+    """
+    Test the runtime by making multiple calls and checking the distribution of the responses. Limited to calls for 10000 customers
+
+    :param auth: The authentication object for the ecosystem-server
+    :param auth_runtime: The authentication object for the runtime
+    :param testing_config: The testing configuration
+    :param output_level: The level of output to print. Options are "quiet" and "verbose"
+
+    :return: True if the tests pass, False otherwise
+    """
+    for test_iter in testing_config["distribution_tests"]:
+        # Specify a table containing a list of msisdns to call
+        customer_config = test_iter["customer_config"]
+        # Specify a table containing the expected offer distribution to run the comparison against
+        offer_distribution_config = test_iter["offer_distribution_config"]
+        # Error margin
+        error_margin = test_iter["error_margin"]
+        post_invocations_input = test_iter["api_call"]
+
+        customer_database = customer_config["database"]
+        offer_database = offer_distribution_config["database"]
+        # Load the tables
+        if customer_database == "mongodb":
+            customer_table = dme.get_data(auth_runtime, customer_config["db"], customer_config["table"], {}, 0,
+                                         customer_config["column"], 0)
+        elif customer_database == "cassandra":
+            customer_table = dme.get_cassandra_sql(auth, "SELECT {} FROM {}.{} LIMIT 10000".format(
+                customer_config["column"], customer_config["db"], customer_config["table"]))["data"]
+        else:
+            print("Error: customer_table database not supported, must be either mongodb or cassandra")
+            return False
+
+        if offer_database == "mongodb":
+            offer_list = dme.get_data(auth_runtime, offer_distribution_config["db"], offer_distribution_config["table"],
+                                     {}, 0, offer_distribution_config["offer_column"] + "," + offer_distribution_config[
+                                         "count_column"], 0)
+        elif offer_database == "cassandra":
+            offer_list = dme.get_cassandra_sql(auth, "SELECT {}, {} FROM {}.{} LIMIT 10000".format(
+                offer_distribution_config["offer_column"], offer_distribution_config["count_column"], offer_distribution_config["db"], offer_distribution_config["table"]))["data"]
+        else:
+            print("Error: offer_distribution_table database not supported, must be either mongodb or cassandra")
+            return False
+
+        # Get results
+        offer_results = {}
+        for msisdn_iter in customer_table:
+            try:
+                post_invocations_input["customer"] = msisdn_iter[customer_config["column"]]
+                offer_response = o.invocations(auth_runtime, post_invocations_input)
+                if output_level != "quiet":
+                    print(offer_response)
+                if "final_result" not in offer_response:
+                    print("Error: final_result not in response for msisdn {0}".format(
+                        msisdn_iter[customer_table["column"]]))
+                    return False
+                if offer_response["final_result"] == []:
+                    print("Error: final_result is empty for msisdn {0}".format(msisdn_iter[customer_table["column"]]))
+                    return False
+                offer_returned = offer_response["final_result"][0]["result"]["offer"]
+                if offer_returned not in offer_results:
+                    offer_results[offer_returned] = 1
+                else:
+                    offer_results[offer_returned] += 1
+            except Exception as e:
+                print("Error in runtime_test_distribution: {0}".format(e))
+                return False
+
+        # Check alignment with expected distribution
+        offer_column = offer_distribution_config["offer_column"]
+        count_column = offer_distribution_config["count_column"]
+        for offer_iter in offer_list:
+            if test_iter["check_missing_offers"] == "Yes":
+                if offer_iter[offer_column] not in offer_results:
+                    print("Error: offer {0} not returned".format(offer_iter[offer_distribution_config["offer_column"]]))
+                    return False
+            if offer_iter[offer_column] in offer_results:
+                if abs(offer_iter[count_column] - offer_results[offer_iter[offer_column]]) > error_margin:
+                    print("Error: offer {0} count {1} not within error margin of {2}".format(
+                        offer_iter[offer_distribution_config["offer_column"]],
+                        offer_results[offer_iter[offer_distribution_config["offer_column"]]], error_margin))
+                    return False
+
+    return True
+
+
+def test_deployment(auth, auth_runtime, project_id, deployment_id, version, output_level="quiet"):
+    """
+    Test a deployment using the testing configuration saved for the deployment
+
+    :param auth: The authentication object for the ecosystem-server
+    :param auth_runtime: The authentication object for the runtime
+    :param project_id: The project_id of the deployment
+    :param deployment_id: The deployment_id of the deployment
+    :param version: The version of the deployment
+    :param output_level: The level of output to print. Options are "quiet" and "verbose"
+    """
+    # Get testing config
+    try:
+        testing_config = dme.get_data(auth, "ecosystem_meta", "testing_configuration", {"project_id":project_id,"deployment_id": deployment_id,"version":version}, 0, {},0)[0]
+    except Exception as e:
+        print("Error retrieving testing config: {0}".format(e))
+        return "Testing Failed"
+
+    # Test your deployment
+    individual_tests = single_test_calls(auth_runtime, testing_config, output_level)
+    if not individual_tests:
+        print("Error in individual_tests")
+        return "Testing Failed"
+
+    distribution_tests = distribution_test(auth, auth_runtime, testing_config, output_level)
+    if not distribution_tests:
+        print("Error in distribution_tests")
+        return "Testing Failed"
+
+    return "Testing Passed"
+
+
+def create_network_configuration(auth, database, collection, name, type, switch_key="", selector_splits=[],selector_groups=[]):
+    """
+    Create a new network configuration and store it in mongo. Existing configurations stored in the same location will be overwritten.
+
+    :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+    :param database: The database to store the configuration in.
+    :param collection: The collection to store the configuration in.
+    :param name: The name of the network configuration.
+    :param type: The type of the network configuration. Allowed values are lookup, lookup_passthrough, experiment_selector and no logging router.
+    :param switch_key: The key to switch on for the lookup, lookup_passthrough and no_logging_router types.
+    :param selector_splits: The distribution splits for the experiment_selector type. Should be a list of numbers that define the allocation of customers to an experiment group. For example selector_splits=[0.2,0.8] would have a 20% probability of assigning customers to group 1 a 60% chance of assinging customers to group 2 and and 20% chance of assigning customers to group 3.
+    :param selector_groups: The groups to allocate customers to for the experiment_selector type. Should be a list of the runtime campaign names for the network nodes.
+    """
+
+    if not isinstance(database, str):
+        raise TypeError("database should be a string")
+    if not isinstance(collection, str):
+        raise TypeError("collection should be a string")
+    if not isinstance(name, str):
+        raise TypeError("name should be a string")
+    if not isinstance(type, str):
+        raise TypeError("type should be a string")
+    if not isinstance(switch_key, str):
+        raise TypeError("switch_key should be a string")
+    if not isinstance(selector_splits, list):
+        raise TypeError("selector_splits should be a list")
+    if not isinstance(selector_groups, list):
+        raise TypeError("selector_groups should be a list")
+    if type not in ["lookup", "lookup_passthrough", "experiment_selector", "no logging router"]:
+        raise ValueError("type should be lookup, lookup_passthrough, experiment_selector or no logging router")
+    if type in ["lookup", "lookup_passthrough", "no logging router"] and switch_key == "":
+        raise ValueError("switch_key should be specified for lookup, lookup_passthrough and no logging router types")
+    if type == "experiment_selector" and (selector_splits == [] or selector_groups == []):
+        raise ValueError("selector_splits and selector_groups should be specified for experiment_selector type")
+    if (type == "experiment_selector") and (len(selector_splits) != (len(selector_groups)-1)):
+        raise ValueError("selector_splits should have one less element than selector_groups")
+    if type == "experiment_selector":
+        for i in selector_groups:
+            if not isinstance(i, str):
+                raise TypeError("selector_groups should be a list of strings")
+        prev_split = 0
+        for i in selector_splits:
+            if not isinstance(i, (int, float)):
+                raise TypeError("selector_splits should be a list of numbers")
+            if i > 0 and i <= 1:
+                raise ValueError("selector_splits should be a list of numbers greater than 0 and less than 1")
+            if i <= prev_split:
+                raise ValueError("selector_splits be a strictly monotonically increasing list of numbers")
+
+    try:
+        network_configuration = {
+            "name": name
+            , "type": type
+        }
+        if type in ["lookup", "lookup_passthrough", "no logging router"]:
+            network_configuration["switch_key"] = switch_key
+        elif type == "experiment_selector":
+            selector = {}
+            selector["random_splits"] = selector_splits
+            selector["groups"] = selector_groups
+            network_configuration["selector"] = selector
+    except Exception as e:
+        print("Error creating network configuration: {0}".format(e))
+        return "Network configuration creation failed"
+
+    try:
+        dme.drop_document_collection(auth, database, collection)
+        dme.add_documents(auth, {"database": database, "collection": collection, "document": network_configuration, "update": "name"})
+    except Exception as e:
+        print("Error saving network configuration: {0}".format(e))
+        return "Network configuration save failed"
+
+    return "Network configuration created"
+
+def add_network_node(auth, database, collection, node_value, node_api_params):
+    """
+    Add a new network node to a network runtime configuration. Will replace existing network nodes with the same value.
+
+    :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+    :param database: The database to store the configuration in.
+    :param collection: The collection to store the configuration in.
+    :param node_value: The value of the node to add. The value is used by the network runtime to determine which node should be called.
+    :param node_api_params: The parameters to use when calling the node. Should be a dictionary of the parameters to pass to the node. These parameters will overridde the parameters of the same name passed through the api call.
+    """
+
+    if not isinstance(database, str):
+        raise TypeError("database should be a string")
+    if not isinstance(collection, str):
+        raise TypeError("collection should be a string")
+    if not isinstance(node_value, str):
+        raise TypeError("node_value should be a string")
+    if not isinstance(node_api_params, dict):
+        raise TypeError("node_api_params should be a dictionary")
+
+    try:
+        node_api_params["value"] = node_value
+        network_node = node_api_params
+    except Exception as e:
+        print("Error creating network node: {0}".format(e))
+        return "Network node creation failed"
+
+    try:
+        dme.add_documents(auth, {"database": database, "collection": collection, "document": network_node, "update": "value"})
+    except Exception as e:
+        print("Error saving network node: {0}".format(e))
+        return "Network node save failed"
+
+    return "Network node added"
+
+def remove_network_node(auth, database, collection, node_value):
+    """
+    Remove a network node from a network runtime configuration.
+
+    :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+    :param database: The database to store the configuration in.
+    :param collection: The collection to store the configuration in.
+    :param node_value: The value of the node to remove.
+    """
+
+    if not isinstance(database, str):
+        raise TypeError("database should be a string")
+    if not isinstance(collection, str):
+        raise TypeError("collection should be a string")
+    if not isinstance(node_value, str):
+        raise TypeError("node_value should be a string")
+
+    try:
+        {'database': 'mydb', 'collection': 'mycollection', 'key': 'KEY_NAME', 'value': 'KEY_VALUE_TO_DELETE'}
+        dme.delete_documents(auth, {"database": database, "collection": collection, "key":"value", "value": node_value})
+    except Exception as e:
+        print("Error removing network node: {0}".format(e))
+        return "Network node removal failed"
+
+    return "Network node removed"
```

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/ecosystem_generation_engine.py` & `ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_generation_engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,11 +27,17 @@
 def process_build(auth, json, info=False):
 	ep = endpoints.PROCESS_BUILD
 	resp = request_utils.create(auth, ep, json=json, info=False)
 	result = resp.json()
 	return result
 
 def process_push(auth, json, info=False):
+	"""
+	Push a deployment to the ecosystem-runtime
+
+	:param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+	:param json: The deployment config to be pushed to the ecosystem-runtime.
+	"""
 	ep = endpoints.PROCESS_PUSH
 	resp = request_utils.create(auth, ep, json=json, info=False)
 	result = resp.json()
 	return result
```

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/ecosystem_home.py` & `ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_home.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/ecosystem_user_profiles.py` & `ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_user_profiles.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/functions.py` & `ecosystem-notebooks-0.1.8/prediction/apis/functions.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/quickflat.py` & `ecosystem-notebooks-0.1.8/prediction/apis/quickflat.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/transaction_categorization.py` & `ecosystem-notebooks-0.1.8/prediction/apis/transaction_categorization.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/user_controller.py` & `ecosystem-notebooks-0.1.8/prediction/apis/user_controller.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/utilities.py` & `ecosystem-notebooks-0.1.8/prediction/apis/utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/worker_aws.py` & `ecosystem-notebooks-0.1.8/prediction/apis/worker_aws.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/worker_file_service.py` & `ecosystem-notebooks-0.1.8/prediction/apis/worker_file_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 from prediction.endpoints import worker_file_service as endpoints
 from prediction import request_utils
 
 def upload_file(auth, path, target_path, info=False):
+	"""
+	Upload a file to the ecosystem-server
+
+	:param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+	:param path: The path of the file to be uploaded.
+	:param target_path: The path where the file will be uploaded.
+	"""
 	ep = endpoints.UPLOAD_FILE
 	fileFp = open(path, "rb")
 	files = {"file": fileFp}
 	data = {"path": target_path}
 	resp = request_utils.create_only_auth_no_error(auth, ep, data=data, files=files)
 	return resp
 
@@ -76,14 +83,21 @@
 		"to": to_path,
 		"user": user
 	}
 	resp = request_utils.create(auth, ep, params=param_dict, info=info)
 	return resp
 
 def download(auth, target_path, download_path, info=False):
+	"""
+	Download a file from the ecosystem-server
+
+	:param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+	:param target_path: The path of the file to be downloaded.
+	:param download_path: The path where the downloaded file will be saved.
+	"""
 	ep = endpoints.DOWNLOAD
 	param_dict = {
 		"name": target_path,
 		"path": ""
 	}
 	resp = request_utils.create(auth, ep, params=param_dict, stream=True, info=info)
 	with open(download_path, "wb") as fd:
```

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/worker_google.py` & `ecosystem-notebooks-0.1.8/prediction/apis/worker_google.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/worker_h2o.py` & `ecosystem-notebooks-0.1.8/prediction/apis/worker_h2o.py`

 * *Files 17% similar despite different names*

```diff
@@ -111,14 +111,19 @@
 	ep = endpoints.SPLIT_FRAME
 	param_dict = {"frame": frame, "ratio": ratio}
 	resp = request_utils.create(auth, ep, params=param_dict, info=info)
 	result = resp.json()
 	return result
 
 def generate_model_detail(auth, info=False):
+	"""
+	Process the models saved to the ecosystem-server and generate the model details for display on the ecosystem-workbench.
+
+	:param auth: Token for accessing the ecosystem-server. Created using jwt_access.
+	"""
 	ep = endpoints.GENERATE_MODEL_DETAIL
 	resp = request_utils.create(auth, ep, info=info)
 	result = resp.json()
 	return result
 
 def download_model(auth, mojo_id, predict_id, info=False):
 	ep = endpoints.DOWNLOAD_MODEL
```

### Comparing `ecosystem-notebooks-0.1.7/prediction/apis/worker_uber.py` & `ecosystem-notebooks-0.1.8/prediction/apis/worker_uber.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/algorithm_client_pulse.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/algorithm_client_pulse.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/auth_controller.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/auth_controller.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/data_ingestion_engine.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/data_ingestion_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/data_management_engine.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/data_management_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,20 +178,21 @@
 	"endpoint": "/executeMongoDBscript",
 	"call_message": "{type} {endpoint}",
 	"error_message": "{type} {endpoint} {response_code}"
 }
 
 
 # # Data Management Engine: Cassandra
-# GET_CASSANDRA_SQL = {
-# 	"type": "get",
-# 	"endpoint": "/getCassandraSQL",
-# 	"call_message": "{type} {endpoint}",
-# 	"error_message": "{type} {endpoint} {response_code}"	
-# }
+GET_CASSANDRA_SQL = {
+	"type": "get",
+	"endpoint": "/getCassandraSql",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
 GET_CASSANDRA_TO_MONGODB = {
 	"type": "get",
 	"endpoint": "/getCassandraToMongoDB",
 	"call_message": "{type} {endpoint}",
 	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/data_munging_engine.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/data_munging_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/ecosystem_generation_engine.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_generation_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/ecosystem_home.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_home.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/ecosystem_user_profiles.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_user_profiles.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/prediction_engine.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/prediction_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/transaction_categorization.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/transaction_categorization.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/utilities.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/worker_aws.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_aws.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/worker_file_service.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_file_service.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/worker_h2o.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_h2o.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/endpoints/worker_uber.py` & `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_uber.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/jwt_access.py` & `ecosystem-notebooks-0.1.8/prediction/jwt_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 	"""Exception raised for expired authentication token."""
 	def __init__(self, expiry):
 		expiry_datetime = datetime.utcfromtimestamp(expiry).strftime("%Y-%m-%d %H:%M:%S")
 		message = "Authentication token expired on {}. Please login again.".format(expiry_datetime)
 		super().__init__(message)
 
 class Authenticate:
+	"""
+	Logs into the ecosystem server and retrieves an access token for authentication.
+
+	:param api_address: The url of the ecosystem server.
+	:param username: The username of the user.
+	:param password: The password of the user.
+	"""
 	def __init__(self, api_address, username, password):
 		self.api_address = api_address
 		self.username = username
 		self.password = password
 		token = self.__login(api_address, username, password)
 		self.access_token = token["access_token"]
 		self.refresh_token = token["refresh_token"]
```

### Comparing `ecosystem-notebooks-0.1.7/prediction/nlp_utils.py` & `ecosystem-notebooks-0.1.8/prediction/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/notebook_functions.py` & `ecosystem-notebooks-0.1.8/prediction/notebook_functions.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/prediction_utils.py` & `ecosystem-notebooks-0.1.8/prediction/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/request_utils.py` & `ecosystem-notebooks-0.1.8/prediction/request_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/prediction/utils/endpoint_diff.py` & `ecosystem-notebooks-0.1.8/prediction/utils/endpoint_diff.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/runtime/access.py` & `ecosystem-notebooks-0.1.8/runtime/access.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from runtime.apis import runtime_engine
 
 class Authenticate:
+	"""
+	Logs into the ecosystem runtime and retrieves an access token for authentication.
+
+	:param api_address: The url of the ecosystem runtime.
+	"""
 	def __init__(self, api_address):
 		self.api_address = api_address
 		self.auth_headers = {
 			"Accept": "*/*"
 		}
 		message = "Login Successful"
 		output = runtime_engine.no_auth_ping(api_address, "/ping", self.auth_headers, message)
```

### Comparing `ecosystem-notebooks-0.1.7/runtime/apis/data_management_engine.py` & `ecosystem-notebooks-0.1.8/runtime/apis/data_management_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,27 @@
 	resp = request_utils.create(auth, ep, params=param_dict, info=info)
 	meta = resp.json()
 	if "data" in meta:
 		meta = meta["data"]
 	return meta
 
 def get_data(auth, database, collection, field, limit, projections, skip, info=False):
+	"""
+	Get data from a MongoDB collection using the find syntax.
+
+	:param auth: Token for accessing the ecosystem-runtime. Created using access.
+	:param database: Name of the database.
+	:param collection: Name of the collection.
+	:param field: The mongodb find search query.
+	:param limit: The number of documents to return.
+	:param projections: The fields to include or exclude in mongodb find query format.
+	:param skip: The number of documents to skip.
+
+	:return: A list of all documents matching the find criteria.
+	"""
 	ep = endpoints.GET_MONGO_DB_FIND
 	param_dict = {
 		"database": database, 
 		"collection": collection,
 		"field": field,
 		"limit": limit,
 		"projections": projections,
```

### Comparing `ecosystem-notebooks-0.1.7/runtime/apis/predictor_engine.py` & `ecosystem-notebooks-0.1.8/runtime/apis/predictor_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -223,17 +223,42 @@
         "value": value
     }
     resp = request_utils.create(auth, ep, params=param_dict, info=info)
     meta = resp.json()
     return meta
 
 def invocations(auth, json, info=False):
+    """
+    Call the invocations endpoint of the ecosystem-runtime. This is the generic endpoint for making predictions using
+    the ecosystem-runtime.
+
+    :param auth: Token for accessing the ecosystem-runtime. Created using jwt_access.
+    :param json: The parameters to be passed to the invocations api.
+
+    EXAMPLES:
+
+    Call the invocations endpoint for a deployment with the deployment_id of "demo_deployment" and the customer lookup
+    of 1234567.
+    .. code-block:: python
+
+        offer_response = o.invocations(
+                                        auth,
+                                        {
+                                        "campaign": "demo_deployment",
+                                        "subcampaign": "none",
+                                        "channel": "notebooks",
+                                        "customer": 1234567,
+                                        "userid": "ecosystem",
+                                        "numberoffers": 4,
+                                        "params": "{}"
+                                        }
+                                      )
+    """
     ep = endpoints.INVOCATIONS
     resp = request_utils.create(auth, ep, json=json, info=info)
-    print(resp)
     meta = resp.json()
     return meta
 
 def response(auth, json, info=False):
     ep = endpoints.RESPONSE
     resp = request_utils.create(auth, ep, json=json, info=info)
     meta = resp.json()
```

### Comparing `ecosystem-notebooks-0.1.7/runtime/apis/runtime_engine.py` & `ecosystem-notebooks-0.1.8/runtime/apis/runtime_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/runtime/apis/worker_utilities.py` & `ecosystem-notebooks-0.1.8/runtime/apis/worker_utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/runtime/endpoints/data_management_engine.py` & `ecosystem-notebooks-0.1.8/runtime/endpoints/data_management_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/runtime/endpoints/predictor_engine.py` & `ecosystem-notebooks-0.1.8/runtime/endpoints/predictor_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/runtime/endpoints/worker_utilities.py` & `ecosystem-notebooks-0.1.8/runtime/endpoints/worker_utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/runtime/request_utils.py` & `ecosystem-notebooks-0.1.8/runtime/request_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/runtime/utils/endpoint_diff.py` & `ecosystem-notebooks-0.1.8/runtime/utils/endpoint_diff.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.7/setup.py` & `ecosystem-notebooks-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name='ecosystem-notebooks',
-    version='0.1.7',
+    version='0.1.8',
     description='Ecosystem Notebooks is a wrapper for the Ecosystem API servers.',
     long_description=Path("README.rst").read_text(encoding="utf-8"),
     url='https://github.com/ecosystemai/ecosystem-notebooks',
     author='EcosystemAi',
     author_email='jay@ecosystem.ai',
     license='MIT',
     packages=['runtime', 'runtime.apis', 'runtime.endpoints', 'runtime.utils', 'prediction', 'prediction.apis', 'prediction.endpoints', 'prediction.utils'],
```

