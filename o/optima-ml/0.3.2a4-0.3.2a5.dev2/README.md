# Comparing `tmp/optima-ml-0.3.2a4.tar.gz` & `tmp/optima_ml-0.3.2a5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optima-ml-0.3.2a4.tar", last modified: Fri Apr  5 11:57:50 2024, max compression
+gzip compressed data, was "optima_ml-0.3.2a5.dev2.tar", last modified: Fri Apr 19 01:05:05 2024, max compression
```

## Comparing `optima-ml-0.3.2a4.tar` & `optima_ml-0.3.2a5.dev2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/
--rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima-ml-0.3.2a4/LICENSE
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.736590 optima-ml-0.3.2a4/OPTIMA/
--rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima-ml-0.3.2a4/OPTIMA/__main__.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/builtin/
--rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/OPTIMA/builtin/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    35186 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/OPTIMA/builtin/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/OPTIMA/builtin/figures_of_merit.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    66743 2024-03-23 18:21:18.000000 optima-ml-0.3.2a4/OPTIMA/builtin/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/builtin/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    15439 2024-02-15 12:31:11.000000 optima-ml-0.3.2a4/OPTIMA/builtin/search_space.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/core/
--rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/core/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    91727 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-03-23 18:05:57.000000 optima-ml-0.3.2a4/OPTIMA/core/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8297 2024-03-23 18:21:18.000000 optima-ml-0.3.2a4/OPTIMA/core/search_space.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-03-23 18:53:01.000000 optima-ml-0.3.2a4/OPTIMA/core/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    79736 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/training.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    80215 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/variable_optimization.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16272 2024-04-05 11:41:05.000000 optima-ml-0.3.2a4/OPTIMA/defaults.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/hardware_configs/
--rw-rw-r--   0 erik     (30000) erik     (30003)     2823 2024-02-19 17:16:10.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/Dresden_Taurus.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16772 2024-03-30 12:31:40.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/common.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-02-19 18:33:13.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/helpers.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/helpers/
--rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/helpers/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/helpers/extract_data_from_NTuples.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/helpers/manage_ray_nodes.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/keras/
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/keras/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    28626 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/keras/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/keras/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/keras/training.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/OPTIMA/lightning/
--rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima-ml-0.3.2a4/OPTIMA/lightning/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-03-24 16:56:32.000000 optima-ml-0.3.2a4/OPTIMA/lightning/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/lightning/training.py
--rwxrwxr-x   0 erik     (30000) erik     (30003)    98442 2024-04-05 11:55:00.000000 optima-ml-0.3.2a4/OPTIMA/optima.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/OPTIMA/resources/
--rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima-ml-0.3.2a4/OPTIMA/resources/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima-ml-0.3.2a4/OPTIMA/resources/config_verification.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-03-23 18:53:01.000000 optima-ml-0.3.2a4/OPTIMA/resources/pbt_with_seed.py
--rw-r--r--   0 erik     (30000) erik     (30003)    88892 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)    87511 2024-04-05 11:54:01.000000 optima-ml-0.3.2a4/README.md
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/optima_ml.egg-info/
--rw-r--r--   0 erik     (30000) erik     (30003)    88892 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/entry_points.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      173 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/requires.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/top_level.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/setup.cfg
--rw-rw-r--   0 erik     (30000) erik     (30003)     4223 2024-03-23 18:53:01.000000 optima-ml-0.3.2a4/setup.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/tests/
--rw-rw-r--   0 erik     (30000) erik     (30003)    37821 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/tests/test_builtin.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8594 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/tests/test_core.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6398 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/tests/test_integration.py
--rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima-ml-0.3.2a4/tests/test_integration_sameMachine.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-03-24 16:53:28.000000 optima-ml-0.3.2a4/tests/test_preprocessing.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.2a5.dev2/LICENSE
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.2a5.dev2/OPTIMA/__main__.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35402 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/figures_of_merit.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    66743 2024-03-23 18:21:18.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/search_space.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/core/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    85793 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-03-23 18:05:57.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    25159 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/search_space.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-03-23 18:53:01.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    79735 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/training.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    80215 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/variable_optimization.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16272 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/defaults.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2827 2024-04-17 12:02:38.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/Dresden_Taurus.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16772 2024-03-30 12:31:40.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/common.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-02-19 18:33:13.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/helpers.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/
+-rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/extract_data_from_NTuples.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/manage_ray_nodes.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/keras/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    28643 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/training.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-03-24 16:56:32.000000 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/training.py
+-rwxrwxr-x   0 erik     (30000) erik     (30003)    99180 2024-04-19 01:04:38.000000 optima_ml-0.3.2a5.dev2/OPTIMA/optima.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/resources/
+-rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.2a5.dev2/OPTIMA/resources/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.2a5.dev2/OPTIMA/resources/config_verification.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-03-23 18:53:01.000000 optima_ml-0.3.2a5.dev2/OPTIMA/resources/pbt_with_seed.py
+-rw-r--r--   0 erik     (30000) erik     (30003)    88934 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)    87528 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/README.md
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/
+-rw-r--r--   0 erik     (30000) erik     (30003)    88934 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      178 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/requires.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/top_level.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/setup.cfg
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4234 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/setup.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/tests/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    37821 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/tests/test_builtin.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8594 2024-02-07 21:12:40.000000 optima_ml-0.3.2a5.dev2/tests/test_core.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6398 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/tests/test_integration.py
+-rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima_ml-0.3.2a5.dev2/tests/test_integration_sameMachine.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-03-24 16:53:28.000000 optima_ml-0.3.2a5.dev2/tests/test_preprocessing.py
```

### Comparing `optima-ml-0.3.2a4/LICENSE` & `optima_ml-0.3.2a5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/builtin/evaluation.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/builtin/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,15 +574,18 @@
             stacked=True,
         )
 
         # draw the histogram
         # for each contribution to the histogram, we need to provide the type of contribution (step or scatter), the
         # index of the reference to use for the ratio subplot, and bin content itself..
         bin_contents_with_type = zip(["step"] * num_classes, [None] * num_classes, bin_contents)
-        colors = sns.color_palette()
+        if (num_classes <= 10 and not explicit_testing_dataset) or num_classes <= 5:
+            colors = sns.color_palette()
+        else:
+            colors = sns.color_palette("husl", num_classes if not explicit_testing_dataset else 2 * num_classes)
         colors_errors = [None] * (num_classes - 1) + ["0.4"]  # only the uppermost contribution should have error bars
         if class_labels is not None:
             legend_labels = class_labels if not binary_classification else class_labels[::-1]
         else:
             legend_labels = (
                 [f"Class {k}" for k in range(num_classes)] if not binary_classification else ["Background", "Signal"]
             )
```

### Comparing `optima-ml-0.3.2a4/OPTIMA/builtin/figures_of_merit.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/builtin/figures_of_merit.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/builtin/inputs.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/builtin/inputs.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/core/evaluation.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/core/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,24 @@
 from ray import tune
 
 import OPTIMA.core.training
 import OPTIMA.core.model
 import OPTIMA.builtin.evaluation
 import OPTIMA.builtin.inputs
 import OPTIMA.builtin.search_space
-from OPTIMA.core.search_space import tune_search_space_type, run_config_search_space_entry_type
+from OPTIMA.core.search_space import run_config_search_space_entry_type
 
 
 def evaluate_experiment(
     analysis: tune.ExperimentAnalysis,
     training_func: Callable,
     run_config: ModuleType,
     optimize_name: str,
     optimize_op: Union[Literal["max"], Literal["min"]],
-    search_space: tune_search_space_type,
-    run_config_search_space: dict[str, run_config_search_space_entry_type],
+    search_space: dict[str, run_config_search_space_entry_type],
     results_dir: str,
     inputs_split: list[ray.ObjectRef],
     targets_split: list[ray.ObjectRef],
     weights_split: list[ray.ObjectRef],
     normalized_weights_split: list[ray.ObjectRef],
     input_handler: OPTIMA.builtin.inputs.InputHandler,
     custom_metrics: Optional[list[tuple[str, Callable]]] = None,
@@ -123,17 +122,15 @@
         Reference to the function performing the training. This is given to ``perform_crossvalidation``.
     run_config : ModuleType
         Reference to the imported run-config file.
     optimize_name : str
         Name of the target metric.
     optimize_op : Union[Literal["max"], Literal["min"]]
         Specifies if the target metric is to be maximized or minimized. Can be either ``'max'`` or ``'min'``.
-    search_space : tune_search_space_type
-        The tune search space provided to the Tuner.
-    run_config_search_space : dict[str, run_config_search_space_entry_type]
+    search_space : dict[str, run_config_search_space_entry_type]
         The search space as defined in the run-config.
     results_dir : str
         Path to the directory where the results are to be saved.
     inputs_split : list[ray.ObjectRef]
         List containing the object reference to the numpy array of input features for the training, validation and (if
         used) testing sets.
     targets_split : list[ray.ObjectRef]
@@ -346,20 +343,14 @@
                 pickle.dump((all_model_configs, trial_ids), file)
         else:
             print(f"{os.path.join(results_dir, 'configs.pickle')} already exists, reloading...")
             with open(os.path.join(results_dir, "configs.pickle"), "rb") as file:
                 all_model_configs, trial_ids = pickle.load(file)
 
         # start with results from the best metric values
-        # get the hp limit and rounding function
-        if hasattr(run_config, "limit_and_round_hyperparameters"):
-            limit_and_round_hps = run_config.limit_and_round_hyperparameters
-        else:
-            limit_and_round_hps = OPTIMA.builtin.search_space.limit_and_round_hyperparameters
-
         dirs_to_evaluate = (
             []
         )  # will contain the paths to the directories containing the models to evaluate (best model from optimization + crossvalidation models)
         model_configs_to_evaluate = []  # will contain the configs of the best models
         for metric, best_trial, best_epoch in zip(best_trials.index, best_trials["trial"], best_trials["best epoch"]):
             # get the config of this trial, add the best epoch and save it to the model_configs_to_evaluate list; this is
             # later given to the crossvalidation function to train multiple models for each config
@@ -371,15 +362,15 @@
                         "trial_id"
                     ] = trial_id  # best_trail is full path to the optimization folder while trails in trial_list as only the names
                     break
             model_configs_to_evaluate.append(model_config_to_evaluate)
 
             # round the config where necessary (in the same way as during the optimization), and add the hyperparameters to
             # the dataframe containing the configs of the best trials
-            model_config = limit_and_round_hps(model_configs_to_evaluate[-1])
+            model_config = model_configs_to_evaluate[-1]
             for hp in model_configs_df.index:
                 model_configs_df.loc[hp, metric] = model_config[hp]
 
             # create the target folder for the following crossvalidation
             target_folder = os.path.join(results_dir, metric if len(best_trials.index) > 1 else "", "best_value")
             dirs_to_evaluate.append(target_folder)  # mark target_folder to be evaluated later
             if not os.path.exists(target_folder):
@@ -397,15 +388,15 @@
                 for trial_id in trial_ids:
                     if trial_id in best_trial:
                         model_config_to_evaluate[
                             "trial_id"
                         ] = trial_id  # best_trail is full path to the optimization folder while trails in trial_list as only the names
                         break
                 model_configs_to_evaluate.append(model_config_to_evaluate)
-                model_config = limit_and_round_hps(model_configs_to_evaluate[-1])
+                model_config = model_configs_to_evaluate[-1]
                 for hp in model_configs_df.index:
                     model_configs_df.loc[hp, f"{metric} fit"] = model_config[hp]
                 target_folder = os.path.join(results_dir, metric if len(best_trials_fit.index) > 1 else "", "best_fit")
                 dirs_to_evaluate.append(target_folder)  # mark target_folder to be evaluated later
                 if not os.path.exists(target_folder):
                     os.makedirs(target_folder)
 
@@ -567,18 +558,15 @@
             optimization_str = f"training events: {[targets_train[targets_train[:, j] == 1].shape[0] for j in range(targets_train.shape[1])]}\n"
             optimization_str += f"validation events: {[targets_val[targets_val[:, j] == 1].shape[0] for j in range(targets_val.shape[1])]}\n"
             if run_config.use_testing_dataset:
                 optimization_str += f"test events: {[targets_test[targets_test[:, j] == 1].shape[0] for j in range(targets_test.shape[1])]}\n"
         optimization_str += "input variables: {}\n\n".format(", ".join(input_handler.get_vars()))
         optimization_str += "search space:\n"
         for hp in search_space.keys():
-            if hp in run_config_search_space.keys():
-                optimization_str += f"\t{hp}: {run_config_search_space[hp]}\n"
-            else:
-                optimization_str += f"\t{hp}: {search_space[hp]}\n"
+            optimization_str += f"\t{hp}: {search_space[hp]}\n"
 
         # write results to file
         if write_results:
             with open(os.path.join(results_dir, "results.txt"), "w") as results_file:
                 results_file.write(
                     optimization_str
                     + "\n"
@@ -734,122 +722,14 @@
                     best_trials_fit if not skip_fit_evaluation else None,
                     model_configs_df,
                     optimization_str + "\n" + optimization_results_string + "\n\n" + evaluation_string,
                     raw_values_list,
                 )
 
 
-def evaluate_search_algorithm_test_step(
-    analysis: tune.ExperimentAnalysis,
-    optimize_name: str,
-    optimize_op: Union[Literal["max"], Literal["min"]],
-    search_space: tune_search_space_type,
-    run_config_search_space: dict[str, run_config_search_space_entry_type],
-    results_dir: str,
-    inputs_split: list[np.ndarray],
-    targets_split: list[np.ndarray],
-    weights_split: list[np.ndarray],
-    input_handler: OPTIMA.builtin.inputs.InputHandler,
-    preprocessor: Any,
-    custom_metrics: Optional[list[tuple[str, Callable]]] = None,
-    composite_metrics: Optional[list[tuple[str, tuple[str, str], Callable]]] = None,
-    overtraining_conditions: Optional[list] = None,
-    write_results: bool = True,
-    return_results_str: bool = False,
-) -> None:
-    """(unmaintained!) Performs the evaluation of one of an optimization step when running with option ``--test_search_algorithm``.
-
-    This function performs the same evaluations done in ``evaluate_experiment`` to determine the best trial with the
-    two evaluation methods but skips the crossvalidation and evaluation of the individual models.
-
-    Parameters
-    ----------
-    analysis : tune.ExperimentAnalysis
-        The ``tune.ExperimentAnalysis``-object extracted from the ``tune.ResultsGrid`` returned by the ``Tuner``.
-    optimize_name : str
-        Name of the target metric.
-    optimize_op : Union[Literal["max"], Literal["min"]]
-        Specifies if the target metric is to be maximized or minimized. Can be either ``'max'`` or ``'min'``.
-    search_space : tune_search_space_type
-        The tune search space provided to the Tuner.
-    run_config_search_space : dict[str, run_config_search_space_entry_type]
-        The search space as defined in the run-config.
-    results_dir : str
-        Path to the directory where the results are to be saved.
-    inputs_split : list[np.ndarray]
-        List containing the numpy array of input features for the training, validation and (if used) testing sets.
-    targets_split : list[np.ndarray]
-        List containing the numpy array of target labels for the training, validation and (if used) testing sets.
-    weights_split : list[np.ndarray]
-        List containing the numpy array of event weights for the training, validation and (if used) testing sets.
-    input_handler : OPTIMA.builtin.inputs.InputHandler
-        Instance of the ``preprocessing.InputHandler``-class
-    preprocessor : Any
-        The fitted scaler used to preprocess the input features that were used for training during the optimization.
-    custom_metrics : Optional[list[tuple[str, Callable]]]
-        A list of `custom metrics` as defined in the run-config. (Default value = None)
-    composite_metrics : Optional[list[tuple[str, tuple[str, str], Callable]]]
-        A list of `composite metrics` as defined in the run-config. (Default value = None)
-    overtraining_conditions : Optional[list]
-        A list of `overtraining conditions` as defined in the run-config. (Default value = None)
-    write_results : bool
-        If ``True``, the results are written to `results.txt` in ``results_dir``. (Default value = True)
-    return_results_str : bool
-        If ``True``, the results string that is printed to console is also returned. (Default value = False)
-    """
-    if overtraining_conditions is None:
-        overtraining_conditions = []
-    if composite_metrics is None:
-        composite_metrics = []
-    if custom_metrics is None:
-        custom_metrics = []
-
-    # save analysis to disk for later manual evaluation
-    with open(os.path.join(results_dir, "analysis.pickle"), "wb") as file:
-        pickle.dump(analysis, file)
-
-    # build a list containing the names of all metrics, grouped together like [[train_loss, val_loss], [train_accuracy, val_accuracy], ...]
-    metric_names = []
-    optimize_name_included = False
-    for metric, _ in custom_metrics:
-        group = ("train_" + metric, "val_" + metric)
-        metric_names.append(group)
-        if optimize_name in group:
-            optimize_name_included = True
-    for metric, _, _ in composite_metrics:
-        metric_names.append(metric)
-        if metric == optimize_name:
-            optimize_name_included = True
-    if not optimize_name_included:
-        metric_names = [optimize_name] + metric_names
-
-    # get the results dataframes and remove all NaN and inf values
-    dfs_dirty = analysis.fetch_trial_dataframes()
-    dfs = clean_analysis_results(dfs_dirty, metric_names)
-
-    # now also save the dataframes
-    with open(os.path.join(results_dir, "dfs.pickle"), "wb") as file:
-        pickle.dump(dfs, file)
-
-    # go through dataframes and explicitly check if overtraining conditions are fulfilled, and add results (True/False)
-    # as new column "overtrained"
-    dfs_overtraining_checked = check_overtraining(dfs, overtraining_conditions)
-
-    # produce two sets of plots showing the overall progress of the experiment, one set containing all trials as datapoints,
-    # and one showing the evolution of the "best" trial; both as a function of time
-    draw_total_progress(
-        dfs_overtraining_checked,
-        optimize_name,
-        optimize_op,
-        metric_names,
-        figs_dir=results_dir,
-        reject_overtrained=True,
-    )
-
-
 def scientific_rounding(value, err, notation="separate"):
     """Helper function to perform scientific rounding based on the provided uncertainty.
 
     Notation can be 'bracket', meaning 0.0123 +- 0.0234 will become 0.012(23), or 'separate' where the rounded value and
     error will be returned separately
 
     Parameters
```

### Comparing `optima-ml-0.3.2a4/OPTIMA/core/inputs.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/core/inputs.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/core/model.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/core/model.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/core/tools.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/core/tools.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/core/training.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/core/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,14 @@
                     if self.parent_process is not None:
                         if not self.parent_process.is_alive():
                             sys.exit(0)
                     if time.time() - wait_start_time > 600:
                         self.termination_event.set()
                         sys.exit(0)
                     time.sleep(1)
-
                 self.report_queue_read_event.clear()
 
     def _do_early_stopping(self, epoch, logs=None, **kwargs: dict) -> bool:
         """Internal method that actually does the early stopping and updating of the state variables.
 
         Parameters
         ----------
```

### Comparing `optima-ml-0.3.2a4/OPTIMA/core/variable_optimization.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/core/variable_optimization.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/defaults.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/defaults.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/hardware_configs/Dresden_Taurus.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/Dresden_Taurus.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class Romeo(SLURMCluster):
     cpus_per_node = 128
     gpus_per_node = 0
     mem_per_cpu = 1972
     threads_per_cpu_core = 2
     SMT_included_in_reservation = False
-    ray_headnodes_path = "/projects/materie-09/s7701085/running_ray_headnodes/running_ray_headnodes.pickle"
+    ray_headnodes_path = "/projects/materie-09/OPTIMA/running_ray_headnodes_romeo/running_ray_headnodes.pickle"
     ray_temp_path = "/tmp/ray"  # default
 
     def get_ports(self) -> dict[str, tuple[int, int]]:
         port_config = {
             "port": (6379, 1),
             "node_manager_port": (6700, 100),
             "object_manager_port": (6701, 100),
```

### Comparing `optima-ml-0.3.2a4/OPTIMA/hardware_configs/common.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/common.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/helpers/extract_data_from_NTuples.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/helpers/extract_data_from_NTuples.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/helpers/manage_ray_nodes.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/helpers/manage_ray_nodes.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/keras/model.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/keras/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     hyperparameters are supported. To use a different type of `Keras` model, a ``build_model``-function needs to be
     defined in the run-config.
 
     The following hyperparameters are supported:
 
     - ``'num_layers'``:    number of hidden layers
     - ``'units'``:         number of neurons per hidden layer
-    - ``'units_i'``:       number of neurons in hidden layer `i` (has higher priority than 'units')
+    - ``'units_i'``:       number of neurons in hidden layer `i`, counting from 1 (has higher priority than 'units')
     - ``'activation'``:    activation function; supported are:
         - ``'relu'``:      Rectified Linear Unit `A(x) = max(0, x)`
         - ``'tanh'``:      Hyperbolic Tangent `A(x) = tanh(x)`
         - ``'sigmoid'``:   Logistic Sigmoid `A(x) = 1 / (1 + e^(-x))`
         - ``'LeakyReLU'``: `A(x) = max(ax, x), 0 <= a <= 1`; here: ``a = 0.1``
         - ``'swish'``:     `A(x) = x / (1 + e^(-ax))`; here: ``a = 1``
         - ``'mish'``:      `A(x) = x * tanh(ln(1 + e^(x)))`
```

### Comparing `optima-ml-0.3.2a4/OPTIMA/keras/tools.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/keras/tools.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/keras/training.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/keras/training.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/lightning/inputs.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/lightning/inputs.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/lightning/training.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/lightning/training.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/optima.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/optima.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Main steering script of OPTIMA."""
 
 __author__ = "E. Bachmann"
 __licence__ = "GPL3"
-__version__ = "0.3.2alpha4"
+__version__ = "0.3.2alpha5_dev2"
 __maintainer__ = "E. Bachmann"
 
 import os
 import sys
 import shutil
 import logging
 import argparse
 import threading
+import functools
 
 if sys.platform == "darwin":
     import multiprocess as mp
 else:
     import multiprocessing as mp
 import pickle
+import dill
 import time
 import random as python_random
 
 import numpy as np
 import pyarrow
 import optuna
 
 os.environ["TUNE_RESULT_BUFFER_LENGTH"] = "1000"  # buffer Tune results; allows for speculative execution of trials to reduce overhead during peak reporting
 os.environ["RAY_DEDUP_LOGS"] = "0"  # disable log deduplication
+os.environ["TUNE_WARN_EXCESSIVE_EXPERIMENT_CHECKPOINT_SYNC_THRESHOLD_S"] = "0"  # temporary solution to disable annoying warnings until a better syncing is implemented
 import ray
 from ray import train, tune
 from ray.tune.schedulers import ASHAScheduler, PopulationBasedTrainingReplay
 # from ray.tune.search.hebo import HEBOSearch
 from ray.tune.search.optuna import OptunaSearch
 from ray.tune.logger import JsonLoggerCallback, CSVLoggerCallback
 from optuna.samplers import TPESampler
@@ -115,19 +118,23 @@
         # - checkpoint_event and checkpoint_queue are used when checking if the trainable should reload from a checkpoint
         # - report_event and report_queue are used to report back results
         # - report_queue_read_event signifies that the main process has finished the report and the subprocess can continue training
         # - termination_event is set when the training terminates internally via EarlyStopping to tell the main process to return
         checkpoint_event, checkpoint_queue = checkpoint_com
         report_event, report_queue, report_queue_read_event = report_com
 
-        # limit and quantize all hyperparameters properly
-        if hasattr(run_config, 'limit_and_round_hyperparameters'):
-            model_config = run_config.limit_and_round_hyperparameters(model_config)
-        else:
-            model_config = OPTIMA.builtin.search_space.limit_and_round_hyperparameters(model_config)
+        # limit all hyperparameters properly; since only non-conditional hyperparameters can go out of bounds (PBT does
+        # not support conditional hps), we don't need to do any deserialization
+        for hp, hp_search_space in run_config.search_space.items():
+            if isinstance(hp_search_space, dict) and "bounds" in hp_search_space.keys() and hp in model_config.keys():
+                bounds = hp_search_space["bounds"]
+                if (isinstance(bounds[0], int) or isinstance(bounds[0], float)) and model_config[hp] < bounds[0]:
+                    model_config[hp] = bounds[0]
+                elif (isinstance(bounds[1], int) or isinstance(bounds[1], float)) and model_config[hp] > bounds[1]:
+                    model_config[hp] = bounds[1]
 
         # convert the training, validation and testing data to tensorflow datasets or lighning dataloaders
         if run_config.model_type == "Keras":
             train_data = tf.data.Dataset.from_tensor_slices((inputs_train, targets_train, normalized_weights_train))
             val_data = tf.data.Dataset.from_tensor_slices((inputs_val, targets_val, normalized_weights_val))
 
             # batch the datasets for tensorflow
@@ -538,37 +545,53 @@
     object_store_memory = int(0.15 * max_ram)
     memory_per_trial = int(args.cpus_per_trial * args.mem_per_cpu * reservable_memory / max_ram * 1e6)
     print("Total available RAM in the cluster: " + str(max_ram / 1e9) + " GB")
     print("Reservable memory: " + str(reservable_memory / 1e9) + " GB")
     print("Object store memory: " + str(object_store_memory / 1e9) + " GB")
     print("Memory per trial: " + str(memory_per_trial / 1e9) + " GB")
 
-    # optionally define default values for every hyperparameter. The output of get_hp_defaults() is given to
-    # build_search_space (if defined in the run-config or when using the built-in build_model-function) to allow choosing
-    # default values for hyperparameters that are not specified in the search space. If a custom build_model()-function
-    # is defined in the run-config and no build_search_space() is given, the hyperparameter defaults will be ignored.
-    if hasattr(run_config, 'get_hp_defaults'):
-        hyperparameter_defaults = run_config.get_hp_defaults()
-    else:
-        hyperparameter_defaults = OPTIMA.builtin.search_space.get_hp_defaults()
-
-    # building the search space from the settings given in the config. First check, if a build_search_space-function is
-    # defined in the run-config. If not, check if a build_model-function is defined - if not, we can use the default
-    # build_search_space function. If a build_model-function is present, instead simply convert each entry in the
-    # run_config.search_space with the OptimizationTools.run_config_to_tune_converter-function.
-    if hasattr(run_config, 'build_search_space'):
-        search_space = run_config.build_search_space(hyperparameter_defaults, run_config)
-    elif not hasattr(run_config, 'build_model') and not run_config.model_type == "Lightning":
-        search_space = OPTIMA.builtin.search_space.build_search_space(hyperparameter_defaults, run_config)
-    else:
-        search_space = {hp: OPTIMA.builtin.search_space.run_config_to_tune_converter(run_config.search_space[hp]) for hp in run_config.search_space.keys()}
-
-    # add the maximum number of epochs and the seed to the search space; setting the seed this way allows for a different
-    # seed for each trial while keeping reproducibility
-    search_space["max_epochs"] = run_config.max_epochs
+    # when using the built-in build_model or compile_model-functions with Keras, get the corresponding hyperparameter
+    # default values and update missing search space entries with the corresponding fixed defaults
+    hyperparameter_defaults_build, hyperparameter_defaults_compile = OPTIMA.builtin.search_space.get_hp_defaults()
+    if run_config.model_type == 'Keras' and not hasattr(run_config, 'build_model'):
+        # check if 'units_i' hyperparameters are present in the search space. If yes, drop the 'units' default hyperparameter
+        if any(["units" in hp for hp in run_config.search_space.keys()]):
+            hyperparameter_defaults_build.pop("units")
+
+        # add missing default values
+        for hp_name, hp_value in hyperparameter_defaults_build.items():
+            if hp_name not in run_config.search_space.keys():
+                run_config.search_space[hp_name] = hp_value
+    if run_config.model_type == 'Keras' and not hasattr(run_config, 'compile_model'):
+        # add missing default values
+        for hp_name, hp_value in hyperparameter_defaults_compile.items():
+            if hp_name not in run_config.search_space.keys():
+                run_config.search_space[hp_name] = hp_value
+
+    # when using the built-in build_model or compile_model-functions with Keras, get the hyperparameters that allow
+    # mutation, and mark their search space entries as such unless they are explicitly marked as non-mutatable in the
+    # run-config
+    mutatable_hps_build, mutatable_hps_compile = OPTIMA.builtin.search_space.get_hps_to_mutate()
+    if run_config.model_type == 'Keras' and not hasattr(run_config, 'build_model'):
+        for hp in mutatable_hps_build:
+            if isinstance(run_config.search_space[hp], dict) and "supports_mutation" not in run_config.search_space[hp].keys():
+                run_config.search_space[hp]["supports_mutation"] = True
+    if run_config.model_type == 'Keras' and not hasattr(run_config, 'compile_model'):
+        for hp in mutatable_hps_compile:
+            if isinstance(run_config.search_space[hp], dict) and "supports_mutation" not in run_config.search_space[hp].keys():
+                run_config.search_space[hp]["supports_mutation"] = True
+
+    # add the maximum number of epochs to the search space
+    run_config.search_space["max_epochs"] = run_config.max_epochs
+
+    # build the search space for optuna
+    search_space_optuna = functools.partial(
+        OPTIMA.core.search_space.optuna_search_space,
+        OPTIMA.core.search_space.serialize_conditions(run_config.search_space)
+    )
 
     # clear the local Ray (temp) directory
     ray_local_dir = os.path.join(get_cluster(args.cluster).ray_temp_path, "ray_results") if args.cluster != 'local' else os.path.join("/tmp", "ray_results")
     if os.path.exists(ray_local_dir):
         shutil.rmtree(ray_local_dir)
 
     # setup ray
@@ -630,15 +653,15 @@
     # in case numpy is using int32 instead of int64, we can only have smaller values as seeds
     max_seeds = OPTIMA.core.tools.get_max_seeds()
 
     # initial optimization and input variable optimization
     if run_config.perform_variable_opt:
         print("Starting initial optimization phase using Optuna with ASHA scheduler...")
         print("Search space:")
-        print(search_space)
+        print(run_config.search_space)
 
         # to make Optimization reproducible (within the limits of high parallelization), set the random seeds
         if run_config.random_seed is not None:
             random_seed = run_config.random_seed
         else:
             random_seed = np.random.randint(*max_seeds)
         print(f"Using random seed: {random_seed}")
@@ -664,15 +687,16 @@
             OptunaWithSeed = OPTIMA.core.search_space.add_random_seed_suggestions(rng_varOpt.randint(*max_seeds))(OptunaSearch)
             search_algo = OptunaWithSeed(
                 metric=optimize_name,
                 mode=optimize_op,
                 sampler=TPESampler(multivariate=run_config.use_multivariate_TPE,
                                    warn_independent_sampling=True,
                                    n_startup_trials=max(args.max_pending_trials, 10),
-                                   seed=rng_varOpt.randint(*max_seeds))
+                                   seed=rng_varOpt.randint(*max_seeds)),
+                space=search_space_optuna,
             ) if run_config.use_TPESampler else None
 
             asha_scheduler = ASHAScheduler(
                 grace_period=run_config.ASHA_grace_period,
                 max_t=run_config.ASHA_max_t,
                 reduction_factor=run_config.ASHA_reduction_factor,
                 stop_last_trials=False
@@ -687,15 +711,15 @@
                 tuner = tune.Tuner.restore(os.path.abspath(optimization_dir_varOpt), trainable=trainable, resume_errored=True)
             else:
                 tuner = tune.Tuner(
                     tune.with_resources(
                         trainable,
                         resources=tune.PlacementGroupFactory([{"CPU": args.cpus_per_trial, "GPU": args.gpus_per_trial, "memory": memory_per_trial}]),
                     ),
-                    param_space=search_space,
+                    # param_space=search_space,
                     run_config=train.RunConfig(
                         name=os.path.basename(optimization_dir_varOpt),
                         storage_path=os.path.dirname(os.path.abspath(optimization_dir_varOpt)),  # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
                         local_dir=ray_local_dir,
                         storage_filesystem=pyarrow.fs.LocalFileSystem(),
                         stop=stopper,
                         checkpoint_config=train.CheckpointConfig(
@@ -752,15 +776,14 @@
         # evaluate optimization results
         best_trials, best_trials_fit, configs_df, results_str, crossval_model_info, crossval_input_data = \
             OPTIMA.core.evaluation.evaluate_experiment(analysis,
                                                        train_model,
                                                        run_config,
                                                        run_config.monitor_name,
                                                        run_config.monitor_op,
-                                                       search_space,
                                                        run_config.search_space,
                                                        results_dir_variableOpt,
                                                        inputs_split,
                                                        targets_split,
                                                        weights_split,
                                                        normalized_weights_split,
                                                        input_handler,
@@ -863,15 +886,15 @@
                                                          weighted_native_metrics=weighted_native_metrics
                                                          )
 
     # hyperparameter optimization with Optuna and ASHA
     if run_config.perform_main_hyperopt:
         print("Starting hyperparameter optimization using Optuna with ASHA scheduler...")
         print("Search space:")
-        print(search_space)
+        print(run_config.search_space)
 
         # to make Optimization reproducible (within the limits of high parallelization), set the random seeds
         if run_config.random_seed is not None:
             random_seed = run_config.random_seed
         else:
             random_seed = np.random.randint(*max_seeds)
         print(f"Using random seed: {random_seed}")
@@ -898,15 +921,16 @@
             OptunaWithSeed = OPTIMA.core.search_space.add_random_seed_suggestions(rng_optuna.randint(*max_seeds))(OptunaSearch)
             search_algo = OptunaWithSeed(
                 metric=optimize_name,
                 mode=optimize_op,
                 sampler=TPESampler(multivariate=run_config.use_multivariate_TPE,
                                    warn_independent_sampling=True,
                                    n_startup_trials=max(args.max_pending_trials, 10),
-                                   seed=rng_optuna.randint(*max_seeds))
+                                   seed=rng_optuna.randint(*max_seeds)),
+                space=search_space_optuna,
             ) if run_config.use_TPESampler else None
 
             asha_scheduler = ASHAScheduler(
                 grace_period=run_config.ASHA_grace_period,
                 max_t=run_config.ASHA_max_t,
                 reduction_factor=run_config.ASHA_reduction_factor,
                 stop_last_trials=False
@@ -921,15 +945,15 @@
             else:
                 tuner = tune.Tuner(
                     tune.with_resources(
                         trainable,
                         resources=tune.PlacementGroupFactory(
                             [{"CPU": args.cpus_per_trial, "GPU": args.gpus_per_trial, "memory": memory_per_trial}]),
                     ),
-                    param_space=search_space,
+                    # param_space=search_space,
                     run_config=train.RunConfig(
                         name=os.path.basename(optimization_dir_optuna),
                         storage_path=os.path.dirname(os.path.abspath(optimization_dir_optuna)),  # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
                         local_dir=ray_local_dir,
                         storage_filesystem=pyarrow.fs.LocalFileSystem(),  # all trials will be on the same filesystem, so we don't need syncing
                         stop=stopper,
                         checkpoint_config=train.CheckpointConfig(
@@ -987,15 +1011,14 @@
         # evaluate optimization results
         best_trials, best_trials_fit, configs_df = \
             OPTIMA.core.evaluation.evaluate_experiment(analysis,
                                                        train_model,
                                                        run_config,
                                                        run_config.monitor_name,
                                                        run_config.monitor_op,
-                                                       search_space,
                                                        run_config.search_space,
                                                        results_dir_optuna,
                                                        inputs_split,
                                                        targets_split,
                                                        weights_split,
                                                        normalized_weights_split,
                                                        input_handler,
@@ -1016,44 +1039,40 @@
             random_seed = run_config.random_seed
         else:
             random_seed = np.random.randint(*max_seeds)
         print(f"Using random seed: {random_seed}")
         random_seed = (random_seed * 3) % max_seeds[1]
         rng_PBT = np.random.RandomState(random_seed)
 
-        # updating search space to include best values from Optuna+ASHA run / set default values for parameters that
-        # cannot be optimized with PBT (e.g. number of layers)
-        if hasattr(run_config, "prepare_search_space_for_PBT"):
-            prepare_search_space_for_PBT = run_config.prepare_search_space_for_PBT
-        else:
-            prepare_search_space_for_PBT = OPTIMA.builtin.search_space.prepare_search_space_for_PBT
+        # for PBT, set all non-mutatable hyperparameters to the fixed best values found during the main hyperparameter
+        # optimization
         if run_config.perform_variable_opt or run_config.perform_main_hyperopt:
             print("Grabbing the best parameters from the Optuna+ASHA run to update the config...")
-            best_hp_values_optuna = {hp: values for hp, values in zip(configs_df.index,
-                                                                      configs_df[target_metric_for_PBT_init +
-                                                                                 (" fit" if run_config.use_fit_results_for_PBT else "")])}
-            search_space = prepare_search_space_for_PBT(search_space, best_hp_values_optuna)
+            best_hp_values_optuna = {
+                hp: values for hp, values in zip(
+                    configs_df.index,
+                    configs_df[target_metric_for_PBT_init + (" fit" if run_config.use_fit_results_for_PBT else "")]
+                )
+            }
         else:
-            print("Checking validity of search space...")
-            search_space = prepare_search_space_for_PBT(search_space, hyperparameter_defaults)
-        print("Updated search space:")
-        print(search_space)
+            best_hp_values_optuna = None
 
-        # for the population based training, we have to choose which hyperparameters should be mutated
-        if hasattr(run_config, 'get_PBT_hps_to_mutate'):
-            hyperparams_to_mutate = run_config.get_PBT_hps_to_mutate(search_space)
-        else:
-            hyperparams_to_mutate = OPTIMA.core.search_space.get_PBT_hps_to_mutate(search_space)
+        # prepare the search space for PBT and get the mutatable subset of the search space
+        search_space_PBT, hyperparams_to_mutate = OPTIMA.core.search_space.prepare_search_space_for_PBT(run_config.search_space, best_hp_values_optuna)
+
+        # print the updated search space
+        print("Updated search space:")
+        print(search_space_PBT)
 
         # since the search algorithm is completely ignored when using PBT, we cannot do the same trick to include the
         # random seed as for Optuna. Fortunately, PBT only optimizes hyperparameters provided in hyperparams_to_mutate,
         # so we can simply add a new search space entry for the seed. Unfortunately, the only way to make the sampling
-        # from the search space entries reproducible is to set the numpy global random state.
+        # from Tune search space entries reproducible is to set the numpy global random state.
         np.random.seed(rng_PBT.randint(*max_seeds))
-        search_space["seed"] = tune.randint(*max_seeds)
+        search_space_PBT["seed"] = tune.randint(*max_seeds)
 
         # if variable optimization or Optuna+ASHA run was performed before PBT, add subdirectory to optimization_dir
         if run_config.perform_variable_opt or run_config.perform_main_hyperopt:
             optimization_dir_PBT = os.path.join(optimization_dir, "PBT")
             results_dir_PBT = os.path.join(results_dir, "PBT")
         else:
             optimization_dir_PBT = optimization_dir
@@ -1070,15 +1089,15 @@
             tuner = tune.Tuner(
                 tune.with_resources(
                     trainable,
                     resources=tune.PlacementGroupFactory(
                         [{"CPU": args.cpus_per_trial, "GPU": args.gpus_per_trial, "memory": memory_per_trial}]),
                     # resources={"cpu": cpus_per_trial, "gpu": args.gpus_per_trial, "memory": memory_per_trial},
                 ),
-                param_space=search_space if not replay else None,
+                param_space=search_space_PBT if not replay else None,
                 run_config=train.RunConfig(
                     name=name,
                     storage_path=os.path.abspath(storage_path),  # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
                     local_dir=ray_local_dir,
                     storage_filesystem=pyarrow.fs.LocalFileSystem(),  # all trials will be on the same filesystem, so we don't need syncing
                     stop=stopper,
                     checkpoint_config=train.CheckpointConfig(
@@ -1157,16 +1176,15 @@
 
         best_trials, best_trials_fit, configs_df = \
             OPTIMA.core.evaluation.evaluate_experiment(analysis,
                                                        train_model,
                                                        run_config,
                                                        run_config.monitor_name,
                                                        run_config.monitor_op,
-                                                       search_space,
-                                                       run_config.search_space,
+                                                       search_space_PBT,
                                                        results_dir_PBT,
                                                        inputs_split,
                                                        targets_split,
                                                        weights_split,
                                                        normalized_weights_split,
                                                        input_handler,
                                                        custom_metrics=custom_metrics,
@@ -1218,17 +1236,17 @@
         exclude_node_list += args.exclude.split(",")
         job.excludes_list = exclude_node_list
     else:
         job.excludes_list = []
 
     def _optional_argument_formatter(key, value):
         if value is not None and value != "":
-            if value == True:
+            if isinstance(value, bool) and value:  # prevent integer 1 and 0 from being interpreted as bools
                 return f"--{key} "
-            if value == False:
+            if isinstance(value, bool) and not value:
                 return ""
             else:
                 return f"--{key} {value} "
         else:
             return ""
 
     # setup the environment
```

### Comparing `optima-ml-0.3.2a4/OPTIMA/resources/config_verification.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/resources/config_verification.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/OPTIMA/resources/pbt_with_seed.py` & `optima_ml-0.3.2a5.dev2/OPTIMA/resources/pbt_with_seed.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/PKG-INFO` & `optima_ml-0.3.2a5.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.2a4
+Version: 0.3.2a5.dev2
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -25,14 +25,15 @@
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: scikit-learn
+Requires-Dist: dill
 Provides-Extra: keras
 Requires-Dist: tensorflow==2.15.0; extra == "keras"
 Provides-Extra: lightning
 Requires-Dist: torch==2.1.2; extra == "lightning"
 Requires-Dist: lightning==2.1.2; extra == "lightning"
 
 
@@ -551,15 +552,15 @@
 ##### build_model
 
 A function that builds a Functional Keras multilayer perceptron for provided hyperparameter values. Supported
 hyperparameters are:
 
 - `'num_layers'`: the number of hidden layers
 - `'units'`: the number of neurons per hidden layer (constant for all layers)
-- `'units_i'`: the number of neurons in hidden layer `i` (has higher priority than `'units'`)
+- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`)
 - `'activation'`: the activation function
 - `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers
 - `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations
 - `'dropout'`: the dropout rate
 
 The input variables are normalized using a custom non-linear normalization layer, whose documentation can be found
 [here](https://optima-docs.docs.cern.ch/keras/tools.html#OPTIMA.keras.tools.NonLinearNormalization). This layer first
```

### Comparing `optima-ml-0.3.2a4/README.md` & `optima_ml-0.3.2a5.dev2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
 ##### build_model
 
 A function that builds a Functional Keras multilayer perceptron for provided hyperparameter values. Supported
 hyperparameters are:
 
 - `'num_layers'`: the number of hidden layers
 - `'units'`: the number of neurons per hidden layer (constant for all layers)
-- `'units_i'`: the number of neurons in hidden layer `i` (has higher priority than `'units'`)
+- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`)
 - `'activation'`: the activation function
 - `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers
 - `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations
 - `'dropout'`: the dropout rate
 
 The input variables are normalized using a custom non-linear normalization layer, whose documentation can be found
 [here](https://optima-docs.docs.cern.ch/keras/tools.html#OPTIMA.keras.tools.NonLinearNormalization). This layer first
```

### Comparing `optima-ml-0.3.2a4/optima_ml.egg-info/PKG-INFO` & `optima_ml-0.3.2a5.dev2/optima_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.2a4
+Version: 0.3.2a5.dev2
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -25,14 +25,15 @@
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: scikit-learn
+Requires-Dist: dill
 Provides-Extra: keras
 Requires-Dist: tensorflow==2.15.0; extra == "keras"
 Provides-Extra: lightning
 Requires-Dist: torch==2.1.2; extra == "lightning"
 Requires-Dist: lightning==2.1.2; extra == "lightning"
 
 
@@ -551,15 +552,15 @@
 ##### build_model
 
 A function that builds a Functional Keras multilayer perceptron for provided hyperparameter values. Supported
 hyperparameters are:
 
 - `'num_layers'`: the number of hidden layers
 - `'units'`: the number of neurons per hidden layer (constant for all layers)
-- `'units_i'`: the number of neurons in hidden layer `i` (has higher priority than `'units'`)
+- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`)
 - `'activation'`: the activation function
 - `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers
 - `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations
 - `'dropout'`: the dropout rate
 
 The input variables are normalized using a custom non-linear normalization layer, whose documentation can be found
 [here](https://optima-docs.docs.cern.ch/keras/tools.html#OPTIMA.keras.tools.NonLinearNormalization). This layer first
```

### Comparing `optima-ml-0.3.2a4/optima_ml.egg-info/SOURCES.txt` & `optima_ml-0.3.2a5.dev2/optima_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/setup.py` & `optima_ml-0.3.2a5.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     'numpy',
     'scipy',
     'pandas',
     'matplotlib',
     'seaborn',
     'tabulate',
     'scikit-learn',
+    'dill'
 ] + (['multiprocess'] if sys.platform == 'darwin' else [])
 
 
 EXTRAS = {
     'keras': ['tensorflow==2.15.0'] if sys.platform == 'linux' else ['tensorflow-macos==2.15.0'],
     'lightning': ['torch==2.1.2', 'lightning==2.1.2'],
 }
```

### Comparing `optima-ml-0.3.2a4/tests/test_builtin.py` & `optima_ml-0.3.2a5.dev2/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/tests/test_core.py` & `optima_ml-0.3.2a5.dev2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/tests/test_integration.py` & `optima_ml-0.3.2a5.dev2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/tests/test_integration_sameMachine.py` & `optima_ml-0.3.2a5.dev2/tests/test_integration_sameMachine.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a4/tests/test_preprocessing.py` & `optima_ml-0.3.2a5.dev2/tests/test_preprocessing.py`

 * *Files identical despite different names*

