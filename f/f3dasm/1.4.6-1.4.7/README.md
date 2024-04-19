# Comparing `tmp/f3dasm-1.4.6.tar.gz` & `tmp/f3dasm-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm-1.4.6.tar", last modified: Thu Dec  7 15:25:52 2023, max compression
+gzip compressed data, was "f3dasm-1.4.7.tar", last modified: Fri Apr 19 15:22:03 2024, max compression
```

## Comparing `f3dasm-1.4.6.tar` & `f3dasm-1.4.7.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.017574 f3dasm-1.4.6/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.4.6/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-07-07 13:46:05.000000 f3dasm-1.4.6/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     4479 2023-12-07 15:25:52.017574 f3dasm-1.4.6/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2900 2023-11-14 18:17:25.000000 f3dasm-1.4.6/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-12-07 15:18:37.000000 f3dasm-1.4.6/VERSION
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.009574 f3dasm-1.4.6/docs/
--rw-rw-r--   0 martin    (1000) martin    (1000)       88 2023-12-07 15:18:37.000000 f3dasm-1.4.6/docs/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-07-15 20:12:10.000000 f3dasm-1.4.6/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       85 2023-09-06 16:39:06.000000 f3dasm-1.4.6/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1401 2023-12-07 15:25:52.017574 f3dasm-1.4.6/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.009574 f3dasm-1.4.6/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.009574 f3dasm-1.4.6/src/f3dasm/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1776 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       27 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/__version__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.009574 f3dasm-1.4.6/src/f3dasm/_src/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/_argparser.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.009574 f3dasm-1.4.6/src/f3dasm/_src/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1385 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.009574 f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5136 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5479 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1510 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5940 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/datagenerator.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.009574 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/
--rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)      125 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8107 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4180 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9143 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/function.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/function_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    80522 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/src/f3dasm/_src/design/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/design/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    27863 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/design/domain.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6457 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/design/parameter.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8788 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/design/samplers.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3300 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_columns.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    15807 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_data.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8852 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_io.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9627 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_jobqueue.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    22910 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_newdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    46828 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/experimentdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12114 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/experimentsample.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/experimentdata/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4025 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/logger.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/src/f3dasm/_src/machinelearning/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/machinelearning/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/src/f3dasm/_src/optimization/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/src/f3dasm/_src/optimization/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2342 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1123 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/cg.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1224 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/lbfgsb.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1289 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/neldermead.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7163 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2097 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/optimizer_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1735 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/_src/optimization/randomsearch.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8914 2023-11-14 18:17:25.000000 f3dasm-1.4.6/src/f3dasm/_src/run_optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/src/f3dasm/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)      755 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/datageneration/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      993 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/datageneration/abaqus.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      906 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/datageneration/functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1351 2023-12-07 15:18:37.000000 f3dasm-1.4.6/src/f3dasm/design.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1665 2023-10-03 19:08:27.000000 f3dasm-1.4.6/src/f3dasm/optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.017574 f3dasm-1.4.6/src/f3dasm.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     4479 2023-12-07 15:25:51.000000 f3dasm-1.4.6/src/f3dasm.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2385 2023-12-07 15:25:52.000000 f3dasm-1.4.6/src/f3dasm.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-12-07 15:25:51.000000 f3dasm-1.4.6/src/f3dasm.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       86 2023-12-07 15:25:51.000000 f3dasm-1.4.6/src/f3dasm.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        7 2023-12-07 15:25:51.000000 f3dasm-1.4.6/src/f3dasm.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-12-07 15:25:52.013574 f3dasm-1.4.6/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.4.6/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.4.6/tests/__init__.pyc
--rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-10-02 00:02:33.000000 f3dasm-1.4.6/tests/conftest.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.4.6/tests/requirements.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.4.7/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-07-07 13:46:05.000000 f3dasm-1.4.7/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     4479 2024-04-19 15:22:03.207407 f3dasm-1.4.7/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2900 2023-11-14 18:17:25.000000 f3dasm-1.4.7/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-04-19 15:20:52.000000 f3dasm-1.4.7/VERSION
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.199407 f3dasm-1.4.7/docs/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       88 2023-12-07 15:18:37.000000 f3dasm-1.4.7/docs/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-07-15 20:12:10.000000 f3dasm-1.4.7/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       85 2023-09-06 16:39:06.000000 f3dasm-1.4.7/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1401 2024-04-19 15:22:03.211407 f3dasm-1.4.7/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.199407 f3dasm-1.4.7/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.203407 f3dasm-1.4.7/src/f3dasm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1776 2024-03-29 12:35:56.000000 f3dasm-1.4.7/src/f3dasm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       27 2023-12-07 15:18:37.000000 f3dasm-1.4.7/src/f3dasm/__version__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.203407 f3dasm-1.4.7/src/f3dasm/_src/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/_src/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/_argparser.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.203407 f3dasm-1.4.7/src/f3dasm/_src/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1385 2023-12-07 15:18:37.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.203407 f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5136 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5479 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1510 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8268 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/datagenerator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.203407 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.203407 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      125 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8220 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4389 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9183 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/function.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/function_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    80508 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.203407 f3dasm-1.4.7/src/f3dasm/_src/design/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/_src/design/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    29701 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/design/domain.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9767 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/design/parameter.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10657 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/design/samplers.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3300 2023-12-07 15:18:37.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_columns.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17550 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_data.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10047 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_io.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10455 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_jobqueue.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    23185 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_newdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    66267 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/experimentdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12738 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/experimentsample.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2023-12-07 15:18:37.000000 f3dasm-1.4.7/src/f3dasm/_src/experimentdata/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2125 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/hydra_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4025 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/logger.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/src/f3dasm/_src/machinelearning/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/_src/machinelearning/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/src/f3dasm/_src/optimization/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2023-12-07 15:18:37.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/src/f3dasm/_src/optimization/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2407 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1157 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/cg.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1258 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/lbfgsb.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1324 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/neldermead.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5903 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2097 2023-12-07 15:18:37.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/optimizer_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1770 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/_src/optimization/randomsearch.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8914 2023-11-14 18:17:25.000000 f3dasm-1.4.7/src/f3dasm/_src/run_optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/src/f3dasm/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      773 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/datageneration/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      993 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/datageneration/abaqus.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      906 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/datageneration/functions.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1442 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/design.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      791 2024-04-19 15:20:52.000000 f3dasm-1.4.7/src/f3dasm/hydra.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1665 2023-10-03 19:08:27.000000 f3dasm-1.4.7/src/f3dasm/optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/src/f3dasm.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     4479 2024-04-19 15:22:03.000000 f3dasm-1.4.7/src/f3dasm.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2436 2024-04-19 15:22:03.000000 f3dasm-1.4.7/src/f3dasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-04-19 15:22:03.000000 f3dasm-1.4.7/src/f3dasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       86 2024-04-19 15:22:03.000000 f3dasm-1.4.7/src/f3dasm.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-04-19 15:22:03.000000 f3dasm-1.4.7/src/f3dasm.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-19 15:22:03.207407 f3dasm-1.4.7/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.4.7/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.4.7/tests/__init__.pyc
+-rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-10-02 00:02:33.000000 f3dasm-1.4.7/tests/conftest.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.4.7/tests/requirements.txt
```

### Comparing `f3dasm-1.4.6/LICENSE` & `f3dasm-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/PKG-INFO` & `f3dasm-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.4.6
+Version: 1.4.7
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://f3dasm.readthedocs.io/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
```

### Comparing `f3dasm-1.4.6/README.md` & `f3dasm-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/setup.cfg` & `f3dasm-1.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/__init__.py` & `f3dasm-1.4.7/src/f3dasm/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/_argparser.py` & `f3dasm-1.4.7/src/f3dasm/_src/_argparser.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/__init__.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/abaqus/utils.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/abaqus/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/datagenerator.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/datagenerator.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from __future__ import annotations
 
 # Standard
 import sys
 from abc import abstractmethod
 from functools import partial
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Dict, List, Optional
 
 if sys.version_info < (3, 8):  # NOQA
     from typing_extensions import Protocol  # NOQA
 else:
     from typing import Protocol
 
 # Third-party
@@ -183,7 +183,73 @@
         ----------
         func : Callable
             The function to add to the post-processing
         kwargs : dict
             The keyword arguments to pass to the post-processing function
         """
         self.post_process = partial(func, **kwargs)
+
+
+def convert_function(f: Callable,
+                     input: List[str],
+                     output: Optional[List[str]] = None,
+                     kwargs: Optional[Dict[str, Any]] = None,
+                     to_disk: Optional[List[str]] = None) -> DataGenerator:
+    """
+    Converts a given function `f` into a `DataGenerator` object.
+
+    Parameters
+    ----------
+    f : Callable
+        The function to be converted.
+    input : List[str]
+        A list of argument names required by the function.
+    output : Optional[List[str]], optional
+        A list of names for the return values of the function.
+        Defaults to None.
+    kwargs : Optional[Dict[str, Any]], optional
+        Additional keyword arguments passed to the function. Defaults to None.
+    to_disk : Optional[List[str]], optional
+        The list of output names where the value needs to be stored on disk.
+        Defaults to None.
+
+    Returns
+    -------
+    DataGenerator
+        A converted `DataGenerator` object.
+
+    Notes
+    -----
+
+    The function `f` can have any number of arguments and any number of returns
+    as long as they are consistent with the `input` and `output` arguments that
+    are given to this function.
+    """
+
+    kwargs = kwargs if kwargs is not None else {}
+    to_disk = to_disk if to_disk is not None else []
+    output = output if output is not None else []
+
+    class TempDataGenerator(DataGenerator):
+        def execute(self, **_kwargs) -> None:
+            _input = {input_name: self.experiment_sample.get(input_name)
+                      for input_name in input}
+            _output = f(**_input, **kwargs)
+
+            # check if output is empty
+            if output is None:
+                return
+
+            if len(output) == 1:
+                _output = (_output,)
+
+            for name, value in zip(output, _output):
+                if name in to_disk:
+                    self.experiment_sample.store(name=name,
+                                                 object=value,
+                                                 to_disk=True)
+                else:
+                    self.experiment_sample.store(name=name,
+                                                 object=value,
+                                                 to_disk=False)
+
+    return TempDataGenerator()
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/__init__.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,18 @@
             if hasattr(yy, "_value"):
                 yy = copy(yy._value)
         else:
             yy = copy(input)
 
         scale = abs(self.noise * yy)
 
+        if isinstance(input, float):
+            # convert to numpy float
+            input = np.float64(input)
+
         noise: np.ndarray = np.random.normal(
             loc=0.0, scale=scale, size=input.shape)
         y_noise = input + float(noise)
         return y_noise
 
     def reverse_augment(self, output: np.ndarray) -> np.ndarray:
         return self.augment
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,17 +85,23 @@
         if not self.offset or self.scale_bounds is None:
             return
 
         g = self._get_global_minimum_for_offset_calculation()
 
         unscaled_offset = np.atleast_1d(
             [
+                # np.random.uniform(
+                #     low=-abs(g[d] - self.scale_bounds[d, 0]),
+                #     high=abs(g[d] - self.scale_bounds[d, 1]))
+
+                # This is added so we only create offsets in one quadrant
+
                 np.random.uniform(
                     low=-abs(g[d] - self.scale_bounds[d, 0]),
-                    high=abs(g[d] - self.scale_bounds[d, 1]))
+                    high=0.0)
                 for d in range(self.dimensionality)
             ]
         )
 
         self.o = Offset(offset=unscaled_offset)
         self.augmentor.insert_input_augmentor(position=0, augmentor=self.o)
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/function.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
     def execute(self, experiment_sample: ExperimentSample) -> ExperimentSample:
         x, _ = experiment_sample.to_numpy()
 
         if isinstance(x, ArrayBox):
             x = x._value
             if isinstance(x, ArrayBox):
                 x = x._value
-
-        experiment_sample["y"] = float(self(x).ravel().astype(np.float32))
+        y = np.nan_to_num(self(x), nan=np.nan)
+        experiment_sample["y"] = float(y.ravel().astype(np.float64))
         return experiment_sample
 
     def _run(
             self, experiment_sample: ExperimentSample | np.ndarray,
             domain: Optional[Domain] = None, **kwargs) -> ExperimentSample:
         _experiment_sample = _experimentsample_factory(
             experiment_sample=experiment_sample, domain=domain)
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/function_factory.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/function_factory.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/datageneration/functions/pybenchfunction.py` & `f3dasm-1.4.7/src/f3dasm/_src/datageneration/functions/pybenchfunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 class Bartels(PyBenchFunction):
     """.. image:: ../img/functions/Bartels.png"""
 
     name = "Bartels"
     continuous = True
     convex = False
     separable = False
-    differentiable = False
+    differentiable = True
     multimodal = True
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -656,15 +656,15 @@
 class BukinN6(PyBenchFunction):
     """.. image:: ../img/functions/BukinN6.png"""
 
     name = "Bukin N. 6"
     continuous = True
     convex = True
     separable = False
-    differentiable = False
+    differentiable = True
     multimodal = True
     randomized_term = False
     parametric = False
     error_autograd = True
 
     @classmethod
     def is_dim_compatible(cls, d):
@@ -733,15 +733,15 @@
 class CrossInTray(PyBenchFunction):
     """.. image:: ../img/functions/CrossInTray.png"""
 
     name = "Cross-in-Tray"
     continuous = True
     convex = False
     separable = False
-    differentiable = False
+    differentiable = True
     multimodal = True
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -1245,15 +1245,15 @@
 class HolderTable(PyBenchFunction):
     """.. image:: ../img/functions/HolderTable.png"""
 
     name = "Holder-Table"
     continuous = True
     convex = False
     separable = False
-    differentiable = False
+    differentiable = True
     multimodal = True
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -1646,15 +1646,15 @@
 class Powell(PyBenchFunction):
     """.. image:: ../img/functions/Powell.png"""
 
     name = "Powell"
     continuous = True
     convex = True
     separable = True
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -2112,15 +2112,15 @@
 class Schwefel(PyBenchFunction):
     """.. image:: ../img/functions/Schwefel.png"""
 
     name = "Schwefel"
     continuous = True
     convex = False
     separable = True
-    differentiable = False
+    differentiable = True
     multimodal = True
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -2151,15 +2151,15 @@
 class Schwefel2_20(PyBenchFunction):
     """.. image:: ../img/functions/Schwefel2_20.png"""
 
     name = "Schwefel 2.20"
     continuous = True
     convex = True
     separable = True
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -2189,15 +2189,15 @@
 class Schwefel2_21(PyBenchFunction):
     """.. image:: ../img/functions/Schwefel2_21.png"""
 
     name = "Schwefel 2.21"
     continuous = True
     convex = True
     separable = True
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -2227,15 +2227,15 @@
 class Schwefel2_22(PyBenchFunction):
     """.. image:: ../img/functions/Schwefel2_22.png"""
 
     name = "Schwefel 2.22"
     continuous = True
     convex = True
     separable = True
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
     error_autograd = True
 
     @classmethod
     def is_dim_compatible(cls, d):
@@ -2266,15 +2266,15 @@
 class Schwefel2_23(PyBenchFunction):
     """.. image:: ../img/functions/Schwefel2_23.png"""
 
     name = "Schwefel 2.23"
     continuous = True
     convex = True
     separable = True
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -2486,15 +2486,15 @@
 class Sphere(PyBenchFunction):
     """.. image:: ../img/functions/Sphere.png"""
 
     name = "Sphere"
     continuous = True
     convex = True
     separable = True
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
@@ -2746,15 +2746,15 @@
 class XinSheYangN2(PyBenchFunction):
     """.. image:: ../img/functions/XinSheYangN2.png"""
 
     name = "Xin She Yang N.2"
     continuous = False
     convex = False
     separable = False
-    differentiable = False
+    differentiable = True
     multimodal = True
     randomized_term = False
     parametric = False
     error_autograd = True
 
     @classmethod
     def is_dim_compatible(cls, d):
@@ -2824,15 +2824,15 @@
 class XinSheYangN4(PyBenchFunction):
     """.. image:: ../img/functions/XinSheYangN4.png"""
 
     name = "Xin-She Yang N.4"
     continuous = True
     convex = True
     separable = False
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
     error_autograd = True
 
     @classmethod
     def is_dim_compatible(cls, d):
@@ -2862,15 +2862,15 @@
 class Zakharov(PyBenchFunction):
     """.. image:: ../img/functions/Zakharov.png"""
 
     name = "Zakharov"
     continuous = True
     convex = False
     separable = False
-    differentiable = False
+    differentiable = True
     multimodal = False
     randomized_term = False
     parametric = False
 
     @classmethod
     def is_dim_compatible(cls, d):
         assert (d is None) or (
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/design/domain.py` & `f3dasm-1.4.7/src/f3dasm/_src/design/domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,22 +54,42 @@
     space: Dict[str, _Parameter] = field(default_factory=dict)
     output_space: Dict[str, _OutputParameter] = field(default_factory=dict)
 
     def __len__(self) -> int:
         """The len() method returns the number of parameters"""
         return len(self.space)
 
-    def __eq__(self, other: Domain) -> bool:
+    def __eq__(self, __o: Domain) -> bool:
         """Custom equality comparison for Domain objects."""
 
-        if not isinstance(other, Domain):
+        if not isinstance(__o, Domain):
             return TypeError(f"Cannot compare Domain with \
-                {type(other.__name__)}")
+                {type(__o.__name__)}")
         return (
-            self.space == other.space)
+            self.space == __o.space)
+
+    def __add__(self, __o: Domain) -> Domain:
+        if not isinstance(__o, Domain):
+            raise TypeError(f"Cannot add Domain with {type(__o.__name__)}")
+
+        combined_space = {}
+        # Merge values for keys that are present in both dictionaries
+        for key in self.space.keys():
+            if key in __o.space:
+                combined_space[key] = self.space[key] + __o.space[key]
+            else:
+                combined_space[key] = self.space[key]
+
+        # Add keys from dict2 that are not present in dict1
+        for key in __o.space.keys():
+            if key not in self.space:
+                combined_space[key] = __o.space[key]
+
+        return Domain(space=combined_space,
+                      output_space={**self.output_space, **__o.output_space})
 
     def items(self) -> Iterator[_Parameter]:
         """Return an iterator over the items of the parameters"""
         return self.space.items()
 
     def values(self) -> Iterator[_Parameter]:
         """Return an iterator over the values of the parameters"""
@@ -424,15 +444,15 @@
         elif type == 'constant':
             self.add_constant(name, **kwargs)
         else:
             raise ValueError(
                 f"Unknown type {type}!"
                 f"Possible types are: 'float', 'int', 'category', 'constant'.")
 
-    def add_output(self, name: str, to_disk: bool):
+    def add_output(self, name: str, to_disk: bool, exist_ok=False):
         """Add a new output parameter to the domain.
 
         Parameters
         ----------
         name : str
             Name of the output parameter.
         to_disk : bool
@@ -442,17 +462,19 @@
         -------
         >>> domain = Domain()
         >>> domain.add_output('param1', True)
         >>> domain.space
         {'param1': OutputParameter(to_disk=True)}
         """
         if name in self.output_space:
-            raise KeyError(
-                f"Parameter {name} already exists in the domain! \
-                     Choose a different name.")
+            if not exist_ok:
+                raise KeyError(
+                    f"Parameter {name} already exists in the domain! \
+                        Choose a different name.")
+            return
 
         self.output_space[name] = _OutputParameter(to_disk)
 #                                                                       Getters
 # =============================================================================
 
     def get_continuous_parameters(self) -> Dict[str, _ContinuousParameter]:
         """Get all continuous input parameters.
@@ -720,14 +742,49 @@
         """
 
         if isinstance(names, str):
             names = [names]
 
         return Domain(space={key: self.space[key] for key in names})
 
+    def drop_output(self, names: str | Iterable[str]) -> Domain:
+        """Drop a subset of output parameters from the domain.
+
+        Parameters
+        ----------
+
+        names : str or Iterable[str]
+            The names of the output parameters to drop.
+
+        Returns
+        -------
+        Domain
+            A new domain with the dropped output parameters.
+
+        Example
+        -------
+        >>> domain = Domain()
+        >>> domain.output_space = {
+        ...     'param1': _OutputParameter(to_disk=True),
+        ...     'param2': _OutputParameter(to_disk=True),
+        ...     'param3': _OutputParameter(to_disk=True)
+        ... }
+        >>> domain.drop_output(['param1', 'param3'])
+        Domain({'param2': _OutputParameter(to_disk=True)})
+        """
+
+        if isinstance(names, str):
+            names = [names]
+
+        return Domain(
+            space=self.space,
+            output_space={key: self.output_space[key]
+                          for key in self.output_space
+                          if key not in names})
+
 #                                                                 Miscellaneous
 # =============================================================================
 
     def _all_input_continuous(self) -> bool:
         """Check if all input parameters are continuous"""
         return len(self) == len(self._filter(_ContinuousParameter))
 
@@ -749,15 +806,14 @@
         >>> domain.output_space
         {'output1': _ContinuousParameter(lower_bound=-inf, upper_bound=inf),
          'output2': _ContinuousParameter(lower_bound=-inf, upper_bound=inf),
          'output3': _ContinuousParameter(lower_bound=-inf, upper_bound=inf)}
         """
         for output_name in names:
             if not self.is_in_output(output_name):
-                print(f"Output {output_name} not in domain. Adding it.")
                 self.add_output(output_name, to_disk=False)
 
     def is_in_output(self, output_name: str) -> bool:
         """Check if output is in the domain
 
         Parameters
         ----------
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/design/parameter.py` & `f3dasm-1.4.7/src/f3dasm/_src/design/parameter.py`

 * *Files 26% similar despite different names*

```diff
@@ -62,14 +62,35 @@
 
     value: Any
     _type: ClassVar[str] = field(init=False, default="object")
 
     def __post_init__(self):
         self._check_hashable()
 
+    def __add__(self, __o: _Parameter
+                ) -> _ConstantParameter | _CategoricalParameter:
+        if isinstance(__o, _ConstantParameter):
+            if self.value == __o.value:
+                return self
+            else:
+                return _CategoricalParameter(
+                    categories=[self.value, __o.value])
+
+        if isinstance(__o, _CategoricalParameter):
+            return self.to_categorical() + __o
+
+        if isinstance(__o, _DiscreteParameter):
+            return self.to_categorical() + __o
+
+        if isinstance(__o, _ContinuousParameter):
+            raise ValueError("Cannot add continuous parameter to constant!")
+
+    def to_categorical(self) -> _CategoricalParameter:
+        return _CategoricalParameter(categories=[self.value])
+
     def _check_hashable(self):
         """Check if the value is hashable."""
         try:
             hash(self.value)
         except TypeError:
             raise TypeError("The value must be hashable.")
 
@@ -117,14 +138,39 @@
                      log distribution "
                 f"(low={self.lower_bound}, high={self.upper_bound})."
             )
 
         self._check_types()
         self._check_range()
 
+    def __add__(self, __o: _Parameter) -> _ContinuousParameter:
+        if not isinstance(__o, _ContinuousParameter):
+            raise ValueError(
+                "Cannot add non-continuous parameter to continuous!")
+
+        if self.log != __o.log:
+            raise ValueError(
+                "Cannot add continuous parameters with different log scales!")
+
+        if self.lower_bound == __o.lower_bound \
+                and self.upper_bound == __o.upper_bound:
+            # If both lower and upper bounds are the same,
+            # return the first object
+            return self
+
+        if self.lower_bound > __o.upper_bound \
+                or __o.lower_bound > self.upper_bound:
+            # If the ranges do not coincide, raise ValueError
+            raise ValueError("Ranges do not coincide, cannot add")
+
+        # For other scenarios, join the ranges
+        return _ContinuousParameter(
+            lower_bound=min(self.lower_bound, __o.lower_bound),
+            upper_bound=max(self.upper_bound, __o.upper_bound))
+
     def _check_types(self):
         """Check if the boundaries are actually floats"""
         if isinstance(self.lower_bound, int):
             self.lower_bound = float(self.lower_bound)
 
         if isinstance(self.upper_bound, int):
             self.upper_bound = float(self.upper_bound)
@@ -165,14 +211,30 @@
     _type: ClassVar[str] = field(init=False, default="int")
 
     def __post_init__(self):
 
         self._check_types()
         self._check_range()
 
+    def __add__(self, __o: _Parameter) -> _DiscreteParameter:
+        if isinstance(__o, _DiscreteParameter):
+            if self.lower_bound == __o.lower_bound and \
+                    self.upper_bound == __o.upper_bound and \
+                    self.step == __o.step:
+                return self
+
+        if isinstance(__o, _CategoricalParameter):
+            return __o + self
+
+        if isinstance(__o, _ConstantParameter):
+            return __o.to_categorical() + self
+
+        if isinstance(__o, _ContinuousParameter):
+            raise ValueError("Cannot add continuous parameter to discrete!")
+
     def _check_types(self):
         """Check if the boundaries are actually ints"""
         if not isinstance(self.lower_bound, int) or not isinstance(
                 self.upper_bound, int):
             raise TypeError(
                 f"Expect integer, got {type(self.lower_bound).__name__} and \
                      {type(self.upper_bound).__name__}")
@@ -201,14 +263,35 @@
 
     categories: Sequence[CategoricalType]
     _type: str = field(init=False, default="object")
 
     def __post_init__(self):
         self._check_duplicates()
 
+    def __add__(self, __o: _Parameter) -> _CategoricalParameter:
+        if isinstance(__o, _CategoricalParameter):
+            # join unique categories
+            joint_categories = list(set(self.categories + __o.categories))
+
+        if isinstance(__o, _ConstantParameter):
+            joint_categories = list(set(self.categories + [__o.value]))
+
+        if isinstance(__o, _DiscreteParameter):
+            roll_out_discrete = list(range(
+                __o.lower_bound, __o.upper_bound, __o.step))
+            joint_categories = list(set(self.categories + roll_out_discrete))
+
+        if isinstance(__o, _ContinuousParameter):
+            raise ValueError("Cannot add continuous parameter to categorical!")
+
+        return _CategoricalParameter(joint_categories)
+
+    def __eq__(self, __o: _CategoricalParameter) -> bool:
+        return set(self.categories) == set(__o.categories)
+
     def _check_duplicates(self):
         """Check if there are duplicates in the categories list"""
         if len(self.categories) != len(set(self.categories)):
             raise ValueError("Categories contain duplicates!")
 
 
 PARAMETERS = [_CategoricalParameter, _ConstantParameter,
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/design/samplers.py` & `f3dasm-1.4.7/src/f3dasm/_src/design/samplers.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 #                                                                       Modules
 # =============================================================================
 
 from __future__ import annotations
 
 # Standard
+import sys
+from itertools import product
+
+if sys.version_info < (3, 8):  # NOQA
+    from typing_extensions import Literal  # NOQA
+else:
+    from typing import Literal
+
 from typing import Optional
 
 # Third-party
 import numpy as np
 import pandas as pd
 from SALib.sample import latin, sobol_sequence
 
@@ -21,28 +29,33 @@
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
+SamplerNames = Literal['random', 'latin', 'sobol', 'grid']
 
 #                                                              Factory function
 # =============================================================================
 
+
 def _sampler_factory(sampler: str, domain: Domain) -> Sampler:
     if sampler.lower() == 'random':
         return RandomUniform(domain)
 
     elif sampler.lower() == 'latin':
         return LatinHypercube(domain)
 
     elif sampler.lower() == 'sobol':
         return SobolSequence(domain)
 
+    elif sampler.lower() == 'grid':
+        return GridSampler(domain)
+
     else:
         raise KeyError(f"Sampler {sampler} not found!"
                        f"Available built-in samplers are: 'random',"
                        f"'latin' and 'sobol'")
 
 
 #                                                                    Base Class
@@ -140,15 +153,16 @@
             ) + self.domain.get_constant_names()
         ]
 
         # First get an empty reference frame from the DoE
         empty_frame = self.domain._create_empty_dataframe()
 
         # Then, create a new frame from the samples and columnnames
-        samples_frame = pd.DataFrame(data=samples, columns=columnnames)
+        samples_frame = pd.DataFrame(
+            data=samples, columns=columnnames, dtype=object)
         df = pd.concat([empty_frame, samples_frame], sort=True)
 
         return df
 
     def __call__(self, domain: Domain, n_samples: int, seed: int):
         """Call the sampler"""
         self.domain = domain
@@ -279,7 +293,60 @@
         continuous = self.domain.continuous
 
         samples = sobol_sequence.sample(numsamples, len(continuous))
 
         # stretch samples
         samples = self._stretch_samples(samples)
         return samples
+
+
+class GridSampler(Sampler):
+    """Sampling via Grid Sampling
+
+    All the combination of the discrete and categorical parameters are
+    sampled. The argument number_of_samples is ignored.
+    Notes
+    -----
+    This sampler is at the moment only applicable for
+    discrete and categorical parameters.
+
+    """
+
+    def get_samples(self, numsamples: Optional[int] = None) -> pd.DataFrame:
+        """Receive samples of the search space
+
+        Parameters
+        ----------
+        numsamples
+            number of samples
+
+        Returns
+        -------
+            Data objects with the samples
+        """
+
+        self.set_seed(self.seed)
+
+        # If numsamples is None, take the object attribute number_of_samples
+        if numsamples is None:
+            numsamples = self.number_of_samples
+
+        continuous = self.domain.get_continuous_parameters()
+
+        if continuous:
+            raise ValueError("Grid sampling is only possible for domains \
+                             strictly with only discrete and \
+                            categorical parameters")
+
+        discrete = self.domain.get_discrete_parameters()
+        categorical = self.domain.get_categorical_parameters()
+
+        _iterdict = {}
+
+        for k, v in categorical.items():
+            _iterdict[k] = v.categories
+
+        for k, v, in discrete.items():
+            _iterdict[k] = range(v.lower_bound, v.upper_bound+1)
+
+        return pd.DataFrame(list(product(*_iterdict.values())),
+                            columns=_iterdict, dtype=object)
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_columns.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_columns.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_data.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         index : int, list
             The index of the data to get.
 
         Returns
         -------
             A subset of the data.
         """
+        # If the object is empty, return itself
+        if self.is_empty():
+            return self
+
         if isinstance(index, int):
             index = [index]
         return _Data(data=self.data.loc[index].copy(),
                      columns=self.columns)
 
     def __add__(self, other: _Data | Dict[str, Any]) -> _Data:
         """Add two Data objects together.
@@ -232,15 +236,15 @@
         """Export the _Data object to a numpy array.
 
         Returns
         -------
         np.ndarray
             numpy array with the data.
         """
-        return self.data.to_numpy()
+        return self.data.to_numpy(dtype=np.float32)
 
     def to_xarray(self, label: str) -> xr.DataArray:
         """Export the _Data object to a xarray DataArray.
 
         Parameters
         ----------
         label : str
@@ -260,15 +264,15 @@
         Returns
         -------
         pd.DataFrame
             pandas dataframe with the data.
         """
         df = deepcopy(self.data)
         df.columns = self.names
-        return df
+        return df.astype(object)
 
     def combine_data_to_multiindex(self, other: _Data,
                                    jobs_df: pd.DataFrame) -> pd.DataFrame:
         """Combine the data to a multiindex dataframe.
 
         Parameters
         ----------
@@ -343,14 +347,37 @@
         if isinstance(columns, str):
             columns = [columns]
         _selected_columns = _Columns(
             {column: self.columns.columns[column] for column in columns})
         return _Data(
             self.data[self.columns.iloc(columns)], columns=_selected_columns)
 
+    def drop(self, columns: Iterable[str] | str) -> _Data:
+        """Drop the selected columns from the data.
+
+        Parameters
+        ----------
+        columns : Iterable[str] | str
+            The columns to drop.
+
+        Returns
+        -------
+        _Data
+            The data without the selected columns
+        """
+        if isinstance(columns, str):
+            columns = [columns]
+        _selected_columns = _Columns(
+            {
+                name: None for name in self.columns.columns
+                if name not in columns})
+        return _Data(
+            data=self.data.drop(columns=self.columns.iloc(columns)),
+            columns=_selected_columns)
+
 #                                                        Append and remove data
 # =============================================================================
 
     def add(self, data: pd.DataFrame):
         try:
             last_index = self.data.index[-1]
         except IndexError:  # Empty dataframe
@@ -373,29 +400,46 @@
 
         new_indices = pd.RangeIndex(
             start=last_index + 1, stop=last_index + number_of_rows + 1, step=1)
         empty_data = pd.DataFrame(
             np.nan, index=new_indices, columns=self.data.columns)
         self.data = pd.concat([self.data, empty_data], ignore_index=False)
 
-    def add_column(self, name: str):
+    def add_column(self, name: str, exist_ok: bool = False):
+        if name in self.columns.names:
+            if not exist_ok:
+                raise ValueError(
+                    f"Column {name} already exists in the data. "
+                    "Set exist_ok to True to allow skipping existing columns.")
+            return
+
         if self.data.columns.empty:
             new_columns_index = 0
         else:
             new_columns_index = self.data.columns[-1] + 1
 
         self.columns.add(name)
         self.data[new_columns_index] = np.nan
 
     def remove(self, indices: List[int]):
         self.data = self.data.drop(indices)
 
     def round(self, decimals: int):
         self.data = self.data.round(decimals=decimals)
 
+    def overwrite(self, indices: Iterable[int], other: _Data | Dict[str, Any]):
+        if isinstance(other, Dict):
+            other = _convert_dict_to_data(other)
+
+        for other_column in other.columns.names:
+            if other_column not in self.columns.names:
+                self.add_column(other_column)
+
+        self.data.update(other.data.set_index(pd.Index(indices)))
+
 #                                                           Getters and setters
 # =============================================================================
 
     def get_data_dict(self, index: int) -> Dict[str, Any]:
         return self.to_dataframe().loc[index].to_dict()
 
     def set_data(self, index: int, value: Any, column: Optional[str] = None):
@@ -436,14 +480,24 @@
         else:
             self.data.index = indices
 
     def is_empty(self) -> bool:
         """Check if the data is empty."""
         return self.data.empty
 
+    def get_index_with_nan(self) -> pd.Index:
+        """Get the indices with NaN values.
+
+        Returns
+        -------
+        pd.Index
+            The indices with NaN values.
+        """
+        return self.indices[self.data.isna().any(axis=1)]
+
     def has_columnnames(self, names: Iterable[str]) -> bool:
         return set(names).issubset(self.names)
 
     def set_columnnames(self, names: Iterable[str]) -> None:
         for old_name, new_name in zip(self.names, names):
             self.columns.rename(old_name, new_name)
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_io.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # Standard
 import pickle
 from pathlib import Path
 from typing import Any, Mapping, Optional, Type
 
 # Third-party
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 # Local
 from ..logger import logger
 
@@ -35,14 +36,17 @@
 
 LOCK_FILENAME = "lock"
 DOMAIN_FILENAME = "domain"
 INPUT_DATA_FILENAME = "input"
 OUTPUT_DATA_FILENAME = "output"
 JOBS_FILENAME = "jobs"
 
+RESOLUTION_MATPLOTLIB_FIGURE = 300
+MAX_TRIES = 10
+
 #                                                               Storing methods
 # =============================================================================
 
 
 class _Store:
     """Base class for storing and loading output data from disk"""
     suffix: int
@@ -112,15 +116,15 @@
         """
         with open(self.path.with_suffix(self.suffix), 'rb') as file:
             return pickle.load(file)
 
 
 class NumpyStore(_Store):
     """Class to store and load objects using the numpy protocol"""
-    suffix: int = '.npy'
+    suffix: str = '.npy'
 
     def store(self) -> None:
         """
         Store the object to disk using the numpy protocol
         """
         np.save(file=self.path.with_suffix(self.suffix), arr=self.object)
 
@@ -134,15 +138,15 @@
             The loaded object
         """
         return np.load(file=self.path.with_suffix(self.suffix))
 
 
 class PandasStore(_Store):
     """Class to store and load objects using the pandas protocol"""
-    suffix: int = '.csv'
+    suffix: str = '.csv'
 
     def store(self) -> None:
         """
         Store the object to disk using the pandas protocol
         """
         self.object.to_csv(self.path.with_suffix(self.suffix))
 
@@ -156,15 +160,15 @@
             The loaded object
         """
         return pd.read_csv(self.path.with_suffix(self.suffix))
 
 
 class XarrayStore(_Store):
     """Class to store and load objects using the xarray protocol"""
-    suffix: int = '.nc'
+    suffix: str = '.nc'
 
     def store(self) -> None:
         """
         Store the object to disk using the xarray protocol
         """
         self.object.to_netcdf(self.path.with_suffix(self.suffix))
 
@@ -176,20 +180,60 @@
         -------
         xr.DataArray | xr.Dataset
             The loaded object
         """
         return xr.open_dataset(self.path.with_suffix(self.suffix))
 
 
+class FigureStore(_Store):
+    """Class to store and load objects using the matplotlib protocol"""
+    suffix: str = '.png'
+
+    def store(self) -> None:
+        """
+        Store the figure to disk as a png file
+
+        Notes
+        -----
+        - The figure is saved with a resolution of 300 dpi.
+        - The figure is saved with tight bounding boxes.
+        """
+        self.object.savefig(self.path.with_suffix(
+            self.suffix), dpi=RESOLUTION_MATPLOTLIB_FIGURE,
+            bbox_inches='tight')
+
+    def load(self) -> np.ndarray:
+        """
+        Load the image as an numpy array from disk
+        using the matplotlib `plt.imread` function.
+
+        Returns
+        -------
+        np.ndarray
+            The loaded image in the form of a numpy array
+
+        Notes
+        -----
+         The returned array has shape
+        - (M, N) for grayscale images.
+        - (M, N, 3) for RGB images.
+        - (M, N, 4) for RGBA images.
+
+        Images are returned as float arrays (0-1).
+        """
+        return plt.imread(self.path.with_suffix(self.suffix))
+
+
 STORE_TYPE_MAPPING: Mapping[Type, _Store] = {
     np.ndarray: NumpyStore,
     pd.DataFrame: PandasStore,
     pd.Series: PandasStore,
     xr.DataArray: XarrayStore,
-    xr.Dataset: XarrayStore
+    xr.Dataset: XarrayStore,
+    plt.Figure: FigureStore,
 }
 
 #                                                  Loading and saving functions
 # =============================================================================
 
 
 def load_object(path: Path, experimentdata_directory: Path,
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_jobqueue.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_jobqueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,31 +59,31 @@
             The name of the file that the jobs will be saved in.
         """
         if jobs is None:
             jobs = pd.Series(dtype='string')
 
         self.jobs: pd.Series = jobs
 
-    def __add__(self, other: _JobQueue | int) -> _JobQueue:
+    def __add__(self, other: _JobQueue | str) -> _JobQueue:
         """Add two JobQueue objects together.
 
         Parameters
         ----------
         other : JobQueue
             JobQueue object to add.
 
         Returns
         -------
         JobQueue
             JobQueue object containing the added jobs.
         """
-        if isinstance(other, int):
+        if isinstance(other, str):
             # make _JobQueue from the jobnumber
             other = _JobQueue(
-                pd.Series([Status.OPEN], index=[0], dtype='string'))
+                pd.Series(other, index=[0], dtype='string'))
 
         try:
             last_index = self.jobs.index[-1]
         except IndexError:  # Empty Series
             return _JobQueue(other.jobs)
 
         # Make a copy of other.jobs and modify its index
@@ -163,14 +163,32 @@
 
         return cls(pd.read_pickle(filename))
 
     def reset(self) -> None:
         """Resets the job queue."""
         self.jobs = pd.Series(dtype='string')
 
+    #                                                                    Select
+    # =========================================================================
+
+    def select_all(self, status: str) -> _JobQueue:
+        """Selects all jobs with a certain status.
+
+        Parameters
+        ----------
+        status : str
+            Status of the jobs to select
+
+        Returns
+        -------
+        JobQueue
+            JobQueue object containing the selected jobs.
+        """
+        return _JobQueue(self.jobs[self.jobs == status])
+
     #                                                                    Export
     # =========================================================================
 
     def store(self, filename: Path) -> None:
         """Stores the jobs in a pickle file.
 
         Parameters
@@ -229,14 +247,24 @@
             return
 
         new_indices = pd.RangeIndex(
             start=last_index + 1, stop=last_index + number_of_jobs + 1, step=1)
         jobs_to_add = pd.Series(status, index=new_indices, dtype='string')
         self.jobs = pd.concat([self.jobs, jobs_to_add], ignore_index=False)
 
+    def overwrite(
+            self, indices: Iterable[int],
+            other: _JobQueue | str) -> None:
+
+        if isinstance(other, str):
+            other = _JobQueue(
+                pd.Series([other], index=[0], dtype='string'))
+
+        self.jobs.update(other.jobs.set_axis(indices))
+
     #                                                                      Mark
     # =========================================================================
 
     def mark(self, index: int | slice | Iterable[int], status: Status) -> None:
         """Marks a job with a certain status.
 
         Parameters
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/_newdata.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/_newdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,14 +636,21 @@
         ----------
         decimals : int
             The number of decimals to round to.
         """
         self.data = [[round(value, decimals) for value in row]
                      for row in self.data]
 
+    def overwrite(self, data: _Data, indices: Iterable[int]):
+        # TODO: Implement this method!
+        ...
+
+#                                                           Getters and setters
+# =============================================================================
+
     def get_data_dict(self, index: int) -> Dict[str, Any]:
         """
         Get the data as a dictionary.
 
         Parameters
         ----------
         index : int
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/experimentdata.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/experimentdata.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from __future__ import annotations
 
 import sys
 # Standard
 import traceback
 from functools import wraps
 from pathlib import Path
+from time import sleep
 from typing import (Any, Callable, Dict, Iterable, Iterator, List, Optional,
                     Tuple, Type)
 
 if sys.version_info < (3, 8):  # NOQA
     from typing_extensions import Literal  # NOQA
 else:
     from typing import Literal
@@ -31,21 +32,21 @@
 from omegaconf import DictConfig
 from pathos.helpers import mp
 
 # Local
 from ..datageneration.datagenerator import DataGenerator
 from ..datageneration.functions.function_factory import _datagenerator_factory
 from ..design.domain import Domain, _domain_factory
-from ..design.samplers import Sampler, _sampler_factory
+from ..design.samplers import Sampler, SamplerNames, _sampler_factory
 from ..logger import logger
 from ..optimization import Optimizer
 from ..optimization.optimizer_factory import _optimizer_factory
 from ._data import DataTypes, _Data, _data_factory
 from ._io import (DOMAIN_FILENAME, EXPERIMENTDATA_SUBFOLDER,
-                  INPUT_DATA_FILENAME, JOBS_FILENAME, LOCK_FILENAME,
+                  INPUT_DATA_FILENAME, JOBS_FILENAME, LOCK_FILENAME, MAX_TRIES,
                   OUTPUT_DATA_FILENAME, _project_dir_factory)
 from ._jobqueue import NoOpenJobsError, Status, _jobs_factory
 from .experimentsample import ExperimentSample
 from .utils import number_of_overiterations, number_of_updates
 
 #                                                          Authorship & Credits
 # =============================================================================
@@ -145,14 +146,17 @@
         # For backwards compatibility; if the output_data has
         #  only one column, rename it to 'y'
         if self._output_data.names == [0]:
             self._output_data.set_columnnames(['y'])
 
     def __len__(self):
         """The len() method returns the number of datapoints"""
+        if self._input_data.is_empty():
+            return len(self._output_data)
+
         return len(self._input_data)
 
     def __iter__(self) -> Iterator[Tuple[Dict[str, Any]]]:
         self.current_index = 0
         return self
 
     def __next__(self) -> ExperimentSample:
@@ -160,31 +164,27 @@
             raise StopIteration
         else:
             index = self.index[self.current_index]
             self.current_index += 1
             return self.get_experiment_sample(index)
 
     def __add__(self,
-                other: ExperimentData | ExperimentSample) -> ExperimentData:
+                __o: ExperimentData | ExperimentSample) -> ExperimentData:
         """The + operator combines two ExperimentData objects"""
         # Check if the domains are the same
 
-        if not isinstance(other, (ExperimentData, ExperimentSample)):
+        if not isinstance(__o, (ExperimentData, ExperimentSample)):
             raise TypeError(
                 f"Can only add ExperimentData or "
-                f"ExperimentSample objects, not {type(other)}")
-
-        if isinstance(other, ExperimentData) and self.domain != other.domain:
-            raise ValueError(
-                "Cannot add ExperimentData objects with different domains")
+                f"ExperimentSample objects, not {type(__o)}")
 
         return ExperimentData(
-            input_data=self._input_data + other._input_data,
-            output_data=self._output_data + other._output_data,
-            jobs=self._jobs + other._jobs, domain=self.domain,
+            input_data=self._input_data + __o._input_data,
+            output_data=self._output_data + __o._output_data,
+            jobs=self._jobs + __o._jobs, domain=self.domain + __o.domain,
             project_dir=self.project_dir)
 
     def __eq__(self, __o: ExperimentData) -> bool:
         return all([self._input_data == __o._input_data,
                     self._output_data == __o._output_data,
                     self._jobs == __o._jobs,
                     self.domain == __o.domain])
@@ -212,39 +212,60 @@
         """
         @wraps(operation)
         def wrapper_func(self: ExperimentData, *args, **kwargs) -> None:
             lock = FileLock(
                 (self.
                  project_dir / EXPERIMENTDATA_SUBFOLDER / LOCK_FILENAME)
                 .with_suffix('.lock'))
+
+            # If the lock has been acquired:
             with lock:
-                self = ExperimentData.from_file(self.project_dir)
-                value = operation(self, *args, **kwargs)
-                self.store()
+                tries = 0
+                while tries < MAX_TRIES:
+                    try:
+                        self = ExperimentData.from_file(self.project_dir)
+                        value = operation(self, *args, **kwargs)
+                        self.store()
+                        break
+
+                    # Racing conditions can occur when the file is empty
+                    # and the file is being read at the same time
+                    except pd.errors.EmptyDataError:
+                        tries += 1
+                        logger.debug((
+                            f"EmptyDataError occurred, retrying"
+                            f" {tries+1}/{MAX_TRIES}"))
+                        sleep(1)
+
+                    raise pd.errors.EmptyDataError()
+
             return value
 
         return wrapper_func
     #                                                                Properties
     # =========================================================================
 
-    @property
+    @ property
     def index(self) -> pd.Index:
         """Returns an iterable of the job number of the experiments
 
         Returns
         -------
         pd.Index
             The job number of all the experiments in pandas Index format
         """
+        if self._input_data.is_empty():
+            return self._output_data.indices
+
         return self._input_data.indices
 
     #                                                  Alternative Constructors
     # =========================================================================
 
-    @classmethod
+    @ classmethod
     def from_file(cls: Type[ExperimentData],
                   project_dir: Path | str) -> ExperimentData:
         """Create an ExperimentData object from .csv and .json files.
 
         Parameters
         ----------
         project_dir : Path | str
@@ -273,28 +294,40 @@
     def from_sampling(cls, sampler: Sampler | str, domain: Domain | DictConfig,
                       n_samples: int = 1,
                       seed: Optional[int] = None) -> ExperimentData:
         """Create an ExperimentData object from a sampler.
 
         Parameters
         ----------
-        sampler : Sampler
-            Sampler object containing the sampling strategy.
+        sampler : Sampler | str
+            Sampler object containing the sampling strategy or one of the
+            built-in sampler names.
         domain : Domain | DictConfig
             Domain object containing the domain of the experiment or hydra
             DictConfig object containing the configuration.
         n_samples : int, optional
             Number of samples, by default 1.
         seed : int, optional
             Seed for the random number generator, by default None.
 
         Returns
         -------
         ExperimentData
             ExperimentData object containing the sampled data.
+
+        Note
+        ----
+
+        If a string is passed for the sampler argument, it should be one
+        of the built-in samplers:
+
+        * 'random' : Random sampling
+        * 'latin' : Latin Hypercube Sampling
+        * 'sobol' : Sobol Sequence Sampling
+        * 'grid' : Grid Search Sampling
         """
         experimentdata = cls(domain=domain)
         experimentdata.sample(sampler=sampler, n_samples=n_samples, seed=seed)
         return experimentdata
 
     @classmethod
     def from_yaml(cls, config: DictConfig) -> ExperimentData:
@@ -307,20 +340,25 @@
             experiment data.
 
         Returns
         -------
         ExperimentData
             ExperimentData object containing the loaded data.
         """
+        # Option 0: Both existing and sampling
+        if 'from_file' in config and 'from_sampling' in config:
+            return cls.from_file(config.from_file) + cls.from_sampling(
+                **config.from_sampling)
+
         # Option 1: From exisiting ExperimentData files
         if 'from_file' in config:
             return cls.from_file(config.from_file)
 
         # Option 2: Sample from the domain
-        elif 'from_sampling' in config:
+        if 'from_sampling' in config:
             return cls.from_sampling(**config.from_sampling)
 
         else:
             return cls(**config)
 
     @classmethod
     def _from_file_attempt(cls: Type[ExperimentData],
@@ -373,14 +411,61 @@
         """
 
         return ExperimentData(input_data=self._input_data[indices],
                               output_data=self._output_data[indices],
                               jobs=self._jobs[indices],
                               domain=self.domain, project_dir=self.project_dir)
 
+    def drop_output(self, names: Iterable[str] | str) -> ExperimentData:
+        """Drop a column from the output data
+
+        Parameters
+        ----------
+        names : Iteraeble | str
+            The names of the columns to drop.
+
+        Returns
+        -------
+        ExperimentData
+            The ExperimentData object with the column dropped.
+        """
+        return ExperimentData(input_data=self._input_data,
+                              output_data=self._output_data.drop(names),
+                              jobs=self._jobs, domain=self.domain.drop_output(
+                                  names),
+                              project_dir=self.project_dir)
+
+    def select_with_status(self, status: Literal['open', 'in progress',
+                                                 'finished', 'error']
+                           ) -> ExperimentData:
+        """Select a subset of the ExperimentData object with a given status
+
+        Parameters
+        ----------
+        status : Literal['open', 'in progress', 'finished', 'error']
+            The status to select.
+
+        Returns
+        -------
+        ExperimentData
+            The selected ExperimentData object with only the selected status.
+
+        Raises
+        ------
+        ValueError
+            Raised when invalid status is specified
+        """
+        if status not in [s.value for s in Status]:
+            raise ValueError(f"Invalid status {status} given. "
+                             f"\nChoose from values: "
+                             f"{', '.join([s.value for s in Status])}")
+
+        _indices = self._jobs.select_all(status).indices
+        return self.select(_indices)
+
     def get_input_data(self,
                        parameter_names: Optional[str | Iterable[str]] = None
                        ) -> ExperimentData:
         """Retrieve a subset of the input data from the ExperimentData object
 
         Parameters
         ----------
@@ -574,34 +659,41 @@
         input_data : Optional[DataTypes], optional
             input parameters of the added object, by default None
         output_data : Optional[DataTypes], optional
             output parameters of the added object, by default None
         jobs : Optional[Path  |  str], optional
             jobs off the added object, by default None
         """
-        self._add_experiments(ExperimentData(
+        self.add_experiments(ExperimentData(
             domain=domain, input_data=input_data,
             output_data=output_data,
             jobs=jobs))
 
-    def _add_experiments(self,
-                         experiment_sample: ExperimentSample | ExperimentData
-                         ) -> None:
+    def add_experiments(self,
+                        experiment_sample: ExperimentSample | ExperimentData
+                        ) -> None:
         """
         Add an ExperimentSample or ExperimentData to the ExperimentData
-         attribute.
+        attribute.
 
         Parameters
         ----------
         experiment_sample : ExperimentSample or ExperimentData
             Experiment(s) to add.
+
+        Raises
+        ------
+        ValueError
+            If -after checked- the indices of the input and output data
+            objects are not equal.
         """
 
         if isinstance(experiment_sample, ExperimentData):
             experiment_sample._reset_index()
+            self.domain += experiment_sample.domain
 
         self._input_data += experiment_sample._input_data
         self._output_data += experiment_sample._output_data
         self._jobs += experiment_sample._jobs
 
         # Check if indices of the internal objects are equal
         if not (self._input_data.indices.equals(self._output_data.indices)
@@ -609,15 +701,109 @@
             raise ValueError(f"Indices of the internal objects are not equal."
                              f"input_data {self._input_data.indices}, "
                              f"output_data {self._output_data.indices},"
                              f"jobs: {self._jobs.indices}")
 
         # Apparently you need to cast the types again
         # TODO: Breaks if values are NaN or infinite
-        self._input_data.cast_types(self.domain)
+        # self._input_data.cast_types(self.domain)
+
+    def overwrite(
+        self, indices: Iterable[int],
+            domain: Optional[Domain] = None,
+            input_data: Optional[DataTypes] = None,
+            output_data: Optional[DataTypes] = None,
+            jobs: Optional[Path | str] = None,
+            add_if_not_exist: bool = False
+    ) -> None:
+        """Overwrite the ExperimentData object.
+
+        Parameters
+        ----------
+        indices : Iterable[int]
+            The indices to overwrite.
+        domain : Optional[Domain], optional
+            Domain of the new object, by default None
+        input_data : Optional[DataTypes], optional
+            input parameters of the new object, by default None
+        output_data : Optional[DataTypes], optional
+            output parameters of the new object, by default None
+        jobs : Optional[Path  |  str], optional
+            jobs off the new object, by default None
+        add_if_not_exist : bool, optional
+            If True, the new objects are added if the requested indices
+            do not exist in the current ExperimentData object, by default False
+        """
+
+        # Be careful, if a job has output data and gets overwritten with a
+        # job that has no output data, the status is set to open. But the job
+        # will still have the output data!
+
+        # This is usually not a problem, because the output data will be
+        # immediately overwritten in optimization.
+
+        self._overwrite_experiments(
+            indices=indices,
+            experiment_sample=ExperimentData(
+                domain=domain, input_data=input_data,
+                output_data=output_data,
+                jobs=jobs),
+            add_if_not_exist=add_if_not_exist)
+
+    def _overwrite_experiments(
+        self, indices: Iterable[int],
+            experiment_sample: ExperimentSample | ExperimentData,
+            add_if_not_exist: bool) -> None:
+        """
+        Overwrite the ExperimentData object at the given indices.
+
+        Parameters
+        ----------
+        indices : Iterable[int]
+            The indices to overwrite.
+        experimentdata : ExperimentData | ExperimentSample
+            The new ExperimentData object to overwrite with.
+        add_if_not_exist : bool
+            If True, the new objects are added if the requested indices
+            do not exist in the current ExperimentData object.
+        """
+        if not all(pd.Index(indices).isin(self.index)):
+            if add_if_not_exist:
+                self.add_experiments(experiment_sample)
+                return
+            else:
+                raise ValueError(
+                    f"The given indices {indices} do not exist in the current "
+                    f"ExperimentData object. "
+                    f"If you want to add the new experiments, "
+                    f"set add_if_not_exist to True.")
+
+        self._input_data.overwrite(
+            indices=indices, other=experiment_sample._input_data)
+        self._output_data.overwrite(
+            indices=indices, other=experiment_sample._output_data)
+
+        self._jobs.overwrite(
+            indices=indices, other=experiment_sample._jobs)
+
+        if isinstance(experiment_sample, ExperimentData):
+            self.domain += experiment_sample.domain
+
+    @_access_file
+    def overwrite_disk(
+        self, indices: Iterable[int],
+            domain: Optional[Domain] = None,
+            input_data: Optional[DataTypes] = None,
+            output_data: Optional[DataTypes] = None,
+            jobs: Optional[Path | str] = None,
+            add_if_not_exist: bool = False
+    ) -> None:
+        self.overwrite(indices=indices, domain=domain, input_data=input_data,
+                       output_data=output_data, jobs=jobs,
+                       add_if_not_exist=add_if_not_exist)
 
     def add_input_parameter(
         self, name: str,
         type: Literal['float', 'int', 'category', 'constant'],
             **kwargs):
         """Add a new input column to the ExperimentData object.
 
@@ -629,26 +815,30 @@
             type of the new input column: float, int, category or constant
         kwargs
             additional arguments for the new parameter
         """
         self._input_data.add_column(name)
         self.domain.add(name=name, type=type, **kwargs)
 
-    def add_output_parameter(self, name: str, is_disk: bool) -> None:
+    def add_output_parameter(
+            self, name: str, is_disk: bool, exist_ok: bool = False) -> None:
         """Add a new output column to the ExperimentData object.
 
         Parameters
         ----------
         name
             name of the new output column
         is_disk
             Whether the output column will be stored on disk or not
+        exist_ok
+            If True, it will not raise an error if the output column already
+            exists, by default False
         """
-        self._output_data.add_column(name)
-        self.domain.add_output(name, is_disk)
+        self._output_data.add_column(name, exist_ok=exist_ok)
+        self.domain.add_output(name=name, to_disk=is_disk, exist_ok=exist_ok)
 
     def remove_rows_bottom(self, number_of_rows: int):
         """
         Remove a number of rows from the end of the ExperimentData object.
 
         Parameters
         ----------
@@ -667,15 +857,19 @@
         self._jobs.remove(indices)
 
     def _reset_index(self) -> None:
         """
         Reset the index of the ExperimentData object.
         """
         self._input_data.reset_index()
-        self._output_data.reset_index(self._input_data.indices)
+
+        if self._input_data.is_empty():
+            self._output_data.reset_index()
+        else:
+            self._output_data.reset_index(self._input_data.indices)
         self._jobs.reset_index()
 
 #                                                                  ExperimentSample
     # =============================================================================
 
     def get_experiment_sample(self, index: int) -> ExperimentSample:
         """
@@ -874,27 +1068,48 @@
         self.mark(self._jobs.indices, status)
 
     def mark_all_error_open(self) -> None:
         """
         Mark all the experiments that have the status 'error' open
         """
         self._jobs.mark_all_error_open()
+
+    def mark_all_in_progress_open(self) -> None:
+        """
+        Mark all the experiments that have the status 'in progress' open
+        """
+        self._jobs.mark_all_in_progress_open()
+
+    def mark_all_nan_open(self) -> None:
+        """
+        Mark all the experiments that have 'nan' in output open
+        """
+        indices = self._output_data.get_index_with_nan()
+        self.mark(indices=indices, status='open')
     #                                                            Datageneration
     # =========================================================================
 
-    def evaluate(self, data_generator: DataGenerator, mode: str = 'sequential',
+    def evaluate(self, data_generator: DataGenerator,
+                 mode: Literal['sequential', 'parallel',
+                               'cluster', 'cluster_parallel'] = 'sequential',
                  kwargs: Optional[dict] = None) -> None:
         """Run any function over the entirety of the experiments
 
         Parameters
         ----------
         data_generator : DataGenerator
             data grenerator to use
-        mode, optional
-            operational mode, by default 'sequential'
+        mode : str, optional
+            operational mode, by default 'sequential'. Choose between:
+
+            * 'sequential' : Run the operation sequentially
+            * 'parallel' : Run the operation on multiple cores
+            * 'cluster' : Run the operation on the cluster
+            * 'cluster_parallel' : Run the operation on the cluster in parallel
+
         kwargs, optional
             Any keyword arguments that need to
             be supplied to the function, by default None
 
         Raises
         ------
         ValueError
@@ -909,14 +1124,16 @@
 
         if mode.lower() == "sequential":
             return self._run_sequential(data_generator, kwargs)
         elif mode.lower() == "parallel":
             return self._run_multiprocessing(data_generator, kwargs)
         elif mode.lower() == "cluster":
             return self._run_cluster(data_generator, kwargs)
+        elif mode.lower() == "cluster_parallel":
+            return self._run_cluster_parallel(data_generator, kwargs)
         else:
             raise ValueError("Invalid parallelization mode specified.")
 
     def _run_sequential(self, data_generator: DataGenerator, kwargs: dict):
         """Run the operation sequentially
 
         Parameters
@@ -985,27 +1202,40 @@
             try:
                 experiment_sample = self._access_open_job_data()
                 options.append(
                     ({'experiment_sample': experiment_sample, **kwargs},))
             except NoOpenJobsError:
                 break
 
-        def f(options: Dict[str, Any]) -> Any:
-            logger.debug(
-                "Running experiment_sample"
-                f"{options['experiment_sample'].job_number}")
-            return data_generator._run(**options)
+        def f(options: Dict[str, Any]) -> Tuple[ExperimentSample, int]:
+            try:
+
+                logger.debug(
+                    f"Running experiment_sample "
+                    f"{options['experiment_sample'].job_number}")
+
+                return (data_generator._run(**options), 0)  # no *args!
+
+            except Exception as e:
+                error_msg = f"Error in experiment_sample \
+                     {options['experiment_sample'].job_number}: {e}"
+                error_traceback = traceback.format_exc()
+                logger.error(f"{error_msg}\n{error_traceback}")
+                return (options['experiment_sample'], 1)
 
         with mp.Pool() as pool:
             # maybe implement pool.starmap_async ?
-            _experiment_samples: List[ExperimentSample] = pool.starmap(
-                f, options)
+            _experiment_samples: List[
+                Tuple[ExperimentSample, int]] = pool.starmap(f, options)
 
-        for _experiment_sample in _experiment_samples:
-            self._set_experiment_sample(_experiment_sample)
+        for _experiment_sample, exit_code in _experiment_samples:
+            if exit_code == 0:
+                self._set_experiment_sample(_experiment_sample)
+            else:
+                self._set_error(_experiment_sample.job_number)
 
     def _run_cluster(self, data_generator: DataGenerator, kwargs: dict):
         """Run the operation on the cluster
 
         Parameters
         ----------
         operation : ExperimentSampleCallable
@@ -1031,253 +1261,475 @@
                 logger.debug("No Open jobs left!")
                 break
 
             try:
                 _experiment_sample = data_generator._run(
                     experiment_sample, **kwargs)
                 self._write_experiment_sample(_experiment_sample)
-            except Exception as e:
-                error_msg = "Error in experiment_sample "
-                f"{experiment_sample._jobnumber}: {e}"
+            except Exception:
+                n = experiment_sample.job_number
+                error_msg = f"Error in experiment_sample {n}: "
                 error_traceback = traceback.format_exc()
                 logger.error(f"{error_msg}\n{error_traceback}")
                 self._write_error(experiment_sample._jobnumber)
                 continue
 
         self = self.from_file(self.project_dir)
         # Remove the lockfile from disk
         (self.project_dir / EXPERIMENTDATA_SUBFOLDER / LOCK_FILENAME
          ).with_suffix('.lock').unlink(missing_ok=True)
 
+    def _run_cluster_parallel(
+            self, data_generator: DataGenerator, kwargs: dict):
+        """Run the operation on the cluster and parallelize it over cores
+
+        Parameters
+        ----------
+        operation : ExperimentSampleCallable
+            function execution for every entry in the ExperimentData object
+        kwargs : dict
+            Any keyword arguments that need to be supplied to the function
+
+        Raises
+        ------
+        NoOpenJobsError
+            Raised when there are no open jobs left
+        """
+        # Retrieve the updated experimentdata object from disc
+        try:
+            self = self.from_file(self.project_dir)
+        except FileNotFoundError:  # If not found, store current
+            self.store()
+
+        no_jobs = False
+
+        while True:
+            es_list = []
+            for core in range(mp.cpu_count()):
+                try:
+                    es_list.append(self._get_open_job_data())
+                except NoOpenJobsError:
+                    logger.debug("No Open jobs left!")
+                    no_jobs = True
+                    break
+
+            d = self.select([e.job_number for e in es_list])
+
+            d._run_multiprocessing(
+                data_generator=data_generator, kwargs=kwargs)
+
+            # TODO access resource first!
+            self.overwrite_disk(
+                indices=d.index, input_data=d._input_data,
+                output_data=d._output_data, jobs=d._jobs,
+                domain=d.domain, add_if_not_exist=False)
+
+            if no_jobs:
+                break
+
+        self = self.from_file(self.project_dir)
+        # Remove the lockfile from disk
+        (self.project_dir / EXPERIMENTDATA_SUBFOLDER / LOCK_FILENAME
+         ).with_suffix('.lock').unlink(missing_ok=True)
+
     #                                                              Optimization
     # =========================================================================
 
     def optimize(self, optimizer: Optimizer | str,
                  data_generator: DataGenerator | str,
-                 iterations: int, kwargs: Optional[Dict[str, Any]] = None,
+                 iterations: int,
+                 kwargs: Optional[Dict[str, Any]] = None,
                  hyperparameters: Optional[Dict[str, Any]] = None,
-                 x0_selection: str = 'best') -> None:
+                 x0_selection: Literal['best', 'random',
+                                       'last',
+                                       'new'] | ExperimentData = 'best',
+                 sampler: Optional[Sampler | str] = 'random',
+                 overwrite: bool = False,
+                 callback: Optional[Callable] = None) -> None:
         """Optimize the experimentdata object
 
         Parameters
         ----------
-        optimizer : Optimizer
-            Optimizer object to use
+        optimizer : Optimizer | str
+            Optimizer object
         data_generator : DataGenerator | str
-            Data generator object to use
+            DataGenerator object
         iterations : int
-            Number of iterations to run
+            number of iterations
         kwargs : Dict[str, Any], optional
-            Any additional keyword arguments that need to be supplied to \
-            the data generator, by default None
+            any additional keyword arguments that will be passed to
+            the DataGenerator
         hyperparameters : Dict[str, Any], optional
-            Any additional hyperparameters that need to be supplied to the \
-            optimizer, by default None
-        x0_selection : str, optional
-            How to select the initial design, by default 'best'
+            any additional keyword arguments that will be passed to
+            the optimizer
+        x0_selection : str | ExperimentData
+            How to select the initial design. By default 'best'
+            The following x0_selections are available:
+
+            * 'best': Select the best designs from the current experimentdata
+            * 'random': Select random designs from the current experimentdata
+            * 'last': Select the last designs from the current experimentdata
+            * 'new': Create new random designs from the current experimentdata
+
+            If the x0_selection is 'new', new designs are sampled with the
+            sampler provided. The number of designs selected is equal to the
+            population size of the optimizer.
+
+            If an ExperimentData object is passed as x0_selection,
+            the optimizer will use the input_data and output_data from this
+            object as initial samples.
+        sampler: Sampler, optional
+            If x0_selection = 'new', the sampler to use. By default 'random'
+        overwrite: bool, optional
+            If True, the optimizer will overwrite the current data. By default
+            False
+        callback : Callable, optional
+            A callback function that is called after every iteration. It has
+            the following signature:
+
+                    ``callback(intermediate_result: ExperimentData)``
+
+            where the first argument is a parameter containing an
+            `ExperimentData` object with the current iterate(s).
 
         Raises
         ------
         ValueError
             Raised when invalid x0_selection is specified
-        ValueError
-            Raised when invalid optimizer type is specified
-
-        Note
-        ----
-        The following x0_selections are available:
-
-        * 'best': Select the best designs from the current experimentdata
-        * 'random': Select random designs from the current experimentdata
-        * 'last': Select the last designs from the current experimentdata
-
-        The number of designs selected is equal to the \
-        population size of the optimizer
         """
+        # Create the data generator object if a string reference is passed
         if isinstance(data_generator, str):
             data_generator: DataGenerator = _datagenerator_factory(
-                data_generator, self.domain, kwargs)
+                data_generator=data_generator,
+                domain=self.domain, kwargs=kwargs)
 
+        # Create the optimizer object if a string reference is passed
         if isinstance(optimizer, str):
             optimizer: Optimizer = _optimizer_factory(
                 optimizer, self.domain, hyperparameters)
 
+        # Create the sampler object if a string reference is passed
+        if isinstance(sampler, str):
+            sampler: Sampler = _sampler_factory(sampler, self.domain)
+
         if optimizer.type == 'scipy':
             self._iterate_scipy(
-                optimizer, data_generator, iterations, kwargs, x0_selection)
+                optimizer=optimizer, data_generator=data_generator,
+                iterations=iterations, kwargs=kwargs,
+                x0_selection=x0_selection,
+                sampler=sampler,
+                overwrite=overwrite,
+                callback=callback)
         else:
             self._iterate(
-                optimizer, data_generator, iterations, kwargs, x0_selection)
+                optimizer=optimizer, data_generator=data_generator,
+                iterations=iterations, kwargs=kwargs,
+                x0_selection=x0_selection,
+                sampler=sampler,
+                overwrite=overwrite,
+                callback=callback)
 
     def _iterate(self, optimizer: Optimizer, data_generator: DataGenerator,
-                 iterations: int, kwargs: dict, x0_selection: str):
+                 iterations: int, kwargs: Dict[str, Any], x0_selection: str,
+                 sampler: Sampler, overwrite: bool,
+                 callback: Callable):
         """Internal represenation of the iteration process
 
         Parameters
         ----------
         optimizer : Optimizer
             Optimizer object
         data_generator : DataGenerator
             DataGenerator object
         iterations : int
             number of iterations
-        kwargs : dict, optional
-            any additional keyword arguments that will be passed to \
-            the DataGenerator, by default None
-        x0_selection : str
-            How to select the initial design
+        kwargs : Dict[str, Any]
+            any additional keyword arguments that will be passed to
+            the DataGenerator
+        x0_selection : str | ExperimentData
+            How to select the initial design.
+            The following x0_selections are available:
+
+            * 'best': Select the best designs from the current experimentdata
+            * 'random': Select random designs from the current experimentdata
+            * 'last': Select the last designs from the current experimentdata
+            * 'new': Create new random designs from the current experimentdata
+
+            If the x0_selection is 'new', new designs are sampled with the
+            sampler provided. The number of designs selected is equal to the
+            population size of the optimizer.
+
+            If an ExperimentData object is passed as x0_selection,
+            the optimizer will use the input_data and output_data from this
+            object as initial samples.
+
+        sampler: Sampler
+            If x0_selection = 'new', the sampler to use
+        overwrite: bool
+            If True, the optimizer will overwrite the current data.
+        callback : Callable
+            A callback function that is called after every iteration. It has
+            the following signature:
+
+                    ``callback(intermediate_result: ExperimentData)``
+
+            where the first argument is a parameter containing an
+            `ExperimentData` object with the current iterate(s).
 
         Raises
         ------
         ValueError
             Raised when invalid x0_selection is specified
+        """
+        last_index = self.index[-1] if not self.index.empty else -1
 
-        Note
-        ----
-        The following x0_selections are available:
+        if isinstance(x0_selection, str):
+            if x0_selection == 'new':
 
-        * 'best': Select the best designs from the current experimentdata
-        * 'random': Select random designs from the current experimentdata
-        * 'last': Select the last designs from the current experimentdata
+                if iterations < optimizer.hyperparameters.population:
+                    raise ValueError(
+                        f'For creating new samples, the total number of '
+                        f'requested iterations ({iterations}) cannot be '
+                        f'smaller than the population size '
+                        f'({optimizer.hyperparameters.population})')
+
+                init_samples = ExperimentData.from_sampling(
+                    domain=self.domain,
+                    sampler=sampler,
+                    n_samples=optimizer.hyperparameters.population,
+                    seed=optimizer.seed)
+
+                init_samples.evaluate(
+                    data_generator=data_generator, kwargs=kwargs,
+                    mode='sequential')
+
+                if callback is not None:
+                    callback(init_samples)
+
+                if overwrite:
+                    _indices = init_samples.index + last_index + 1
+                    self._overwrite_experiments(
+                        experiment_sample=init_samples,
+                        indices=_indices,
+                        add_if_not_exist=True)
+
+                else:
+                    self.add_experiments(init_samples)
+
+                x0_selection = 'last'
+                iterations -= optimizer.hyperparameters.population
+
+        x0 = x0_factory(experiment_data=self, mode=x0_selection,
+                        n_samples=optimizer.hyperparameters.population)
+        optimizer.set_data(x0)
 
-        The number of designs selected is equal to the \
-        population size of the optimizer
-        """
-        optimizer.set_x0(self, mode=x0_selection)
         optimizer._check_number_of_datapoints()
 
         optimizer._construct_model(data_generator)
 
         for _ in range(number_of_updates(
                 iterations,
                 population=optimizer.hyperparameters.population)):
             new_samples = optimizer.update_step(data_generator)
 
             # If new_samples is a tuple of input_data and output_data
             if isinstance(new_samples, tuple):
-                self.add(domain=self.domain,
-                         input_data=new_samples[0], output_data=new_samples[1])
+                new_samples = ExperimentData(
+                    domain=self.domain,
+                    input_data=new_samples[0],
+                    output_data=new_samples[1],
+                )
+            # If applicable, evaluate the new designs:
+            new_samples.evaluate(
+                data_generator, mode='sequential', kwargs=kwargs)
 
-            else:
-                self._add_experiments(new_samples)
+            if callback is not None:
+                callback(new_samples)
 
-            # If applicable, evaluate the new designs:
-            self.evaluate(data_generator, mode='sequential', kwargs=kwargs)
+            if overwrite:
+                _indices = new_samples.index + last_index + 1
+                self._overwrite_experiments(experiment_sample=new_samples,
+                                            indices=_indices,
+                                            add_if_not_exist=True)
+
+            else:
+                self.add_experiments(new_samples)
 
             optimizer.set_data(self)
 
-        # Remove overiterations
-        self.remove_rows_bottom(number_of_overiterations(
-            iterations, population=optimizer.hyperparameters.population))
+        if not overwrite:
+            # Remove overiterations
+            self.remove_rows_bottom(number_of_overiterations(
+                iterations, population=optimizer.hyperparameters.population))
 
         # Reset the optimizer
         optimizer.reset(ExperimentData(domain=self.domain))
 
     def _iterate_scipy(self, optimizer: Optimizer,
                        data_generator: DataGenerator,
                        iterations: int, kwargs: dict,
-                       x0_selection: str):
-        """Internal represenation of the iteration process for s
-        cipy-optimize algorithms
+                       x0_selection: str | ExperimentData,
+                       sampler: Sampler, overwrite: bool,
+                       callback: Callable):
+        """Internal represenation of the iteration process for scipy-minimize
+        optimizers.
 
         Parameters
         ----------
-        optimizer : _Optimizer
+        optimizer : Optimizer
             Optimizer object
         data_generator : DataGenerator
             DataGenerator object
         iterations : int
             number of iterations
-        kwargs : dict, optional
-            any additional keyword arguments that will be passed \
-            to the DataGenerator, by default None
-        x0_selection : str
-            How to select the initial design
+        kwargs : Dict[str, Any]
+            any additional keyword arguments that will be passed to
+            the DataGenerator
+        x0_selection : str | ExperimentData
+            How to select the initial design.
+            The following x0_selections are available:
+
+            * 'best': Select the best designs from the current experimentdata
+            * 'random': Select random designs from the current experimentdata
+            * 'last': Select the last designs from the current experimentdata
+            * 'new': Create new random designs from the current experimentdata
+
+            If the x0_selection is 'new', new designs are sampled with the
+            sampler provided. The number of designs selected is equal to the
+            population size of the optimizer.
+
+            If an ExperimentData object is passed as x0_selection,
+            the optimizer will use the input_data and output_data from this
+            object as initial samples.
+
+        sampler: Sampler
+            If x0_selection = 'new', the sampler to use
+        overwrite: bool
+            If True, the optimizer will overwrite the current data.
+        callback : Callable
+            A callback function that is called after every iteration. It has
+            the following signature:
+
+                    ``callback(intermediate_result: ExperimentData)``
+
+            where the first argument is a parameter containing an
+            `ExperimentData` object with the current iterate(s).
 
         Raises
         ------
         ValueError
             Raised when invalid x0_selection is specified
+        """
+        last_index = self.index[-1] if not self.index.empty else -1
+        n_data_before_iterate = len(self)
 
-        Note
-        ----
-        The following x0_selections are available:
+        if isinstance(x0_selection, str):
+            if x0_selection == 'new':
 
-        * 'best': Select the best designs from the current experimentdata
-        * 'random': Select random designs from the current experimentdata
-        * 'last': Select the last designs from the current experimentdata
+                if iterations < optimizer.hyperparameters.population:
+                    raise ValueError(
+                        f'For creating new samples, the total number of '
+                        f'requested iterations ({iterations}) cannot be '
+                        f'smaller than the population size '
+                        f'({optimizer.hyperparameters.population})')
+
+                init_samples = ExperimentData.from_sampling(
+                    domain=self.domain,
+                    sampler=sampler,
+                    n_samples=optimizer.hyperparameters.population,
+                    seed=optimizer.seed)
+
+                init_samples.evaluate(
+                    data_generator=data_generator, kwargs=kwargs,
+                    mode='sequential')
+
+                if callback is not None:
+                    callback(init_samples)
+
+                if overwrite:
+                    _indices = init_samples.index + last_index + 1
+                    self._overwrite_experiments(
+                        experiment_sample=init_samples,
+                        indices=_indices,
+                        add_if_not_exist=True)
 
-        The number of designs selected is equal to the \
-        population size of the optimizer
-        """
+                else:
+                    self.add_experiments(init_samples)
+
+                x0_selection = 'last'
+
+        x0 = x0_factory(experiment_data=self, mode=x0_selection,
+                        n_samples=optimizer.hyperparameters.population)
+        optimizer.set_data(x0)
 
-        optimizer.set_x0(self, mode=x0_selection)
-        n_data_before_iterate = len(self)
         optimizer._check_number_of_datapoints()
 
         optimizer.run_algorithm(iterations, data_generator)
 
-        # Do not add the first element, as this is already in the sampled data
-        self._add_experiments(optimizer.data.select(optimizer.data.index[1:]))
-
-        # TODO: At the end, the data should have
-        # n_data_before_iterate + iterations amount of elements!
-        # If x_new is empty, repeat best x0 to fill up total iteration
-        if len(self) == n_data_before_iterate:
-            repeated_x, repeated_y = self.get_n_best_output(
-                n_samples=1).to_numpy()
-            # repeated_last_element = self.get_n_best_output(
-            #     n_samples=1).to_numpy()[0].ravel()
-
-            for repetition in range(iterations):
-                # self._add_experiments(
-                #     ExperimentSample.from_numpy(repeated_last_element,
-                #                                 domain=self.domain))
-
-                self.add(
-                    domain=self.domain, input_data=repeated_x,
-                    output_data=repeated_y)
-
-        # Repeat last iteration to fill up total iteration
-        if len(self) < n_data_before_iterate + iterations:
-            last_design = self.get_experiment_sample(len(self)-1)
+        new_samples: ExperimentData = optimizer.data.select(
+            optimizer.data.index[1:])
+        new_samples.evaluate(data_generator, mode='sequential', kwargs=kwargs)
+
+        if callback is not None:
+            callback(new_samples)
+
+        if overwrite:
+            self.add_experiments(
+                optimizer.data.select([optimizer.data.index[-1]]))
+
+        elif not overwrite:
+            # Do not add the first element, as this is already
+            # in the sampled data
+            self.add_experiments(new_samples)
+
+            # TODO: At the end, the data should have
+            # n_data_before_iterate + iterations amount of elements!
+            # If x_new is empty, repeat best x0 to fill up total iteration
+            if len(self) == n_data_before_iterate:
+                repeated_sample = self.get_n_best_output(
+                    n_samples=1)
+
+                for repetition in range(iterations):
+                    self.add_experiments(repeated_sample)
+
+            # Repeat last iteration to fill up total iteration
+            if len(self) < n_data_before_iterate + iterations:
+                last_design = self.get_experiment_sample(len(self)-1)
 
-            while len(self) < n_data_before_iterate + iterations:
-                self._add_experiments(last_design)
+                while len(self) < n_data_before_iterate + iterations:
+                    self.add_experiments(last_design)
 
         # Evaluate the function on the extra iterations
-        self.evaluate(data_generator, mode='sequential')
+        self.evaluate(data_generator, mode='sequential', kwargs=kwargs)
 
         # Reset the optimizer
         optimizer.reset(ExperimentData(domain=self.domain))
 
     #                                                                  Sampling
     # =========================================================================
 
-    def sample(self, sampler: Sampler | str, n_samples: int = 1,
+    def sample(self, sampler: Sampler | SamplerNames, n_samples: int = 1,
                seed: Optional[int] = None) -> None:
         """Sample data from the domain providing the sampler strategy
 
         Parameters
         ----------
-        sampler : Sampler or str
+        sampler: Sampler | str
             Sampler callable or string of built-in sampler
+            If a string is passed, it should be one of the built-in samplers:
+
+            * 'random' : Random sampling
+            * 'latin' : Latin Hypercube Sampling
+            * 'sobol' : Sobol Sequence Sampling
+            * 'grid' : Grid Search Sampling
         n_samples : int, optional
             Number of samples to generate, by default 1
         seed : Optional[int], optional
             Seed to use for the sampler, by default None
 
-        Note
-        ----
-        If a string is passed, it should be one of the built-in samplers:
-
-        * 'random' : Random sampling
-        * 'latin' : Latin Hypercube Sampling
-        * 'sobol' : Sobol Sequence Sampling
-
         Raises
         ------
         ValueError
             Raised when invalid sampler type is specified
         """
 
         if isinstance(sampler, str):
@@ -1295,7 +1747,54 @@
 
         Parameters
         ----------
         project_dir : Path or str
             Path to the project directory
         """
         self.project_dir = _project_dir_factory(project_dir)
+
+
+def x0_factory(experiment_data: ExperimentData,
+               mode: str | ExperimentData, n_samples: int):
+    """Set the initial population to the best n samples of the given data
+
+    Parameters
+    ----------
+    experiment_data : ExperimentData
+        Data to be used for the initial population
+    mode : str
+        Mode of selecting the initial population, by default 'best'
+        The following modes are available:
+
+            - best: select the best n samples
+            - random: select n random samples
+            - last: select the last n samples
+    n_samples : int
+        Number of samples to select
+
+    Raises
+    ------
+    ValueError
+        Raises when the mode is not recognized
+    """
+    if isinstance(mode, ExperimentData):
+        x0 = mode
+
+    elif mode == 'best':
+        x0 = experiment_data.get_n_best_output(n_samples)
+
+    elif mode == 'random':
+        x0 = experiment_data.select(
+            np.random.choice(
+                experiment_data.index,
+                size=n_samples, replace=False))
+
+    elif mode == 'last':
+        x0 = experiment_data.select(
+            experiment_data.index[-n_samples:])
+
+    else:
+        raise ValueError(
+            f'Unknown selection mode {mode}, use best, random or last')
+
+    x0._reset_index()
+    return x0
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/experimentsample.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/experimentsample.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 
 #                                                                       Modules
 # =============================================================================
 
 from __future__ import annotations
 
 # Standard
+import sys
 from pathlib import Path
+
+if sys.version_info < (3, 8):  # NOQA
+    from typing_extensions import Literal  # NOQA
+else:
+    from typing import Literal
+
 from typing import Any, Dict, Optional, Tuple, Type
 
 # Third-party
 import autograd.numpy as np
 
 # Local
 from ..design.domain import Domain
@@ -191,15 +198,15 @@
         else:
             return value, False
 
     def __setitem__(self, key: str, value: Any):
         self._dict_output[key] = (value, False)
 
     def __repr__(self) -> str:
-        return (f"ExperimentSample({self.job_number} :"
+        return (f"ExperimentSample({self.job_number} ({self.jobs}) :"
                 f"{self.input_data} - {self.output_data})")
 
     @property
     def input_data(self) -> Dict[str, Any]:
         """Retrieve the input data of the design as a dictionary.
 
         Returns
@@ -253,16 +260,34 @@
         Returns
         -------
         int
             The job number of the design.
         """
         return self._jobnumber
 
+    @property
+    def jobs(self) -> Literal['finished', 'open']:
+        """Retrieve the job status.
+
+        Returns
+        -------
+        str
+            The job number of the design as a tuple.
+        """
+        # Check if the output contains values or not all nan
+        has_all_nan = np.all(np.isnan(list(self._output_data.values())))
+
+        if self._output_data and not has_all_nan:
+            status = 'finished'
+        else:
+            status = 'open'
+
+        return status
+
     # Alias
-    jobs = job_number
     _jobs = jobs
 
 #                                                                        Export
 # =============================================================================
 
     def to_numpy(self) -> Tuple[np.ndarray, np.ndarray]:
         """Converts the design to a tuple of numpy arrays.
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/experimentdata/utils.py` & `f3dasm-1.4.7/src/f3dasm/_src/experimentdata/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/logger.py` & `f3dasm-1.4.7/src/f3dasm/_src/logger.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/__init__.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/adapters/scipy_implementations.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/adapters/scipy_implementations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #                                                                       Modules
 # =============================================================================
 
+# Standard
+import warnings
+
 # Third-party core
 import autograd.numpy as np
 from scipy.optimize import minimize
 
 # Locals
 from ...datageneration.datagenerator import DataGenerator
 from ...experimentdata.experimentsample import ExperimentSample
@@ -15,20 +18,23 @@
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
+warnings.filterwarnings(
+    "ignore", message="^OptimizeWarning: Unknown solver options.*")
+
 
 class _SciPyOptimizer(Optimizer):
     type: str = 'scipy'
 
     def _callback(self, xk: np.ndarray, *args, **kwargs) -> None:
-        self.data._add_experiments(
+        self.data.add_experiments(
             ExperimentSample.from_numpy(xk, domain=self.domain))
 
     def update_step(self):
         """Update step function"""
         raise ValueError(
             'Scipy optimizers don\'t have an update steps. \
                  Multiple iterations are directly called \
@@ -52,16 +58,15 @@
             return float(y)
 
         self.hyperparameters.maxiter = iterations
 
         minimize(
             fun=fun,
             method=self.method,
-            # TODO: #89 Fix this with the newest gradient method!
-            jac='3-point',
+            jac=data_generator.dfdx,
             x0=self.data.get_n_best_output(1).to_numpy()[0].ravel(),
             callback=self._callback,
             options=self.hyperparameters.__dict__,
             bounds=self.domain.get_bounds(),
             tol=0.0,
         )
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/cg.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/cg.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,13 +24,13 @@
     """CG Parameters"""
 
     gtol: float = 0.0
 
 
 class CG(_SciPyOptimizer):
     """CG"""
-
+    require_gradients: bool = True
     method: str = "CG"
     hyperparameters: CG_Parameters = CG_Parameters()
 
     def get_info(self) -> List[str]:
         return ['Stable', 'First-Order', 'Single-Solution']
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/lbfgsb.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/lbfgsb.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,13 +29,13 @@
 
     ftol: float = 0.0
     gtol: float = 0.0
 
 
 class LBFGSB(_SciPyOptimizer):
     """L-BFGS-B"""
-
+    require_gradients: bool = True
     method: str = "L-BFGS-B"
     hyperparameters: LBFGSB_Parameters = LBFGSB_Parameters()
 
     def get_info(self) -> List[str]:
         return ['Stable', 'First-Order', 'Single-Solution']
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/neldermead.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/neldermead.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,13 +29,13 @@
     xatol: float = 0.0
     fatol: float = 0.0
     adaptive: bool = False
 
 
 class NelderMead(_SciPyOptimizer):
     """Nelder-Mead"""
-
+    require_gradients: bool = False
     method: str = "Nelder-Mead"
     hyperparameters: NelderMead_Parameters = NelderMead_Parameters()
 
     def get_info(self) -> List[str]:
         return ['Fast', 'Global', 'First-Order', 'Single-Solution']
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/optimizer.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/optimizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -69,38 +69,39 @@
 
     population: int = 1
     force_bounds: bool = True
 
 
 class Optimizer:
     type: ClassVar[str] = 'any'
+    require_gradients: ClassVar[bool] = False
     hyperparameters: OptimizerParameters = OptimizerParameters()
 
     def __init__(
             self, domain: Domain, seed: Optional[int] = None,
             name: Optional[str] = None, **hyperparameters):
         """Optimizer class for the optimization of a data-driven process
 
         Parameters
         ----------
         domain : Domain
             Domain indicating the search-space of the optimization parameters
         seed : Optional[int], optional
             Seed of the random number generator for stochastic optimization
-             processes, by default None, set to random
+            processes, by default None, set to random
         name : Optional[str], optional
             Name of the optimization object, by default None,
-             it will use the name of the class
+            it will use the name of the class
 
 
         Note
         ----
 
         Any additional keyword arguments will be used to overwrite
-         the default hyperparameters of the optimizer.
+        the default hyperparameters of the optimizer.
         """
 
         # Check if **hyperparameters is empty
         if not hyperparameters:
             hyperparameters = {}
 
         # Overwrite the default hyperparameters with the given hyperparameters
@@ -148,63 +149,23 @@
 
     def set_seed(self):
         """Set the seed of the random number generator"""
         ...
 
     def reset(self, data: ExperimentData):
         """Reset the optimizer to its initial state"""
-        self.data = data
+        self.set_data(data)
         self.__post_init__()
 
     def set_data(self, data: ExperimentData):
         """Set the data attribute to the given data"""
         self.data = data
 
-    def set_x0(self, experiment_data: ExperimentData, mode: str):
-        """Set the initial population to the best n samples of the given data
-
-        Parameters
-        ----------
-        experiment_data : ExperimentData
-            Data to be used for the initial population
-        mode : str
-            Mode of selecting the initial population, by default 'best'
-
-        Raises
-        ------
-        ValueError
-            Raises when the mode is not recognized
-
-        Note
-        ----
-        The following modes are available:
-            - best: select the best n samples
-            - random: select n random samples
-            - last: select the last n samples
-        """
-        if mode.lower() == 'best':
-            x0 = experiment_data.get_n_best_output(
-                self.hyperparameters.population)
-
-        elif mode.lower() == 'random':
-            x0 = experiment_data.select(
-                np.random.choice(
-                    experiment_data.index,
-                    self.hyperparameters.population, replace=False))
-
-        elif mode.lower() == 'last':
-            x0 = experiment_data.select(
-                experiment_data.index[-self.hyperparameters.population:])
-
-        else:
-            raise ValueError(
-                f'Unknown selection mode {mode}, use best, random or last')
-
-        x0._reset_index()
-        self.data = x0
+    def add_experiments(self, experiments: ExperimentData):
+        ...
 
     def get_name(self) -> str:
         """Get the name of the optimizer
 
         Returns
         -------
         str
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/optimizer_factory.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/optimization/randomsearch.py` & `f3dasm-1.4.7/src/f3dasm/_src/optimization/randomsearch.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """Hyperparameters for RandomSearch optimizer"""
 
     pass
 
 
 class RandomSearch(Optimizer):
     """Naive random search"""
-
+    require_gradients: bool = False
     hyperparameters: RandomSearch_Parameters = RandomSearch_Parameters()
 
     def set_seed(self):
         np.random.seed(self.seed)
 
     def update_step(
             self, data_generator: DataGenerator
```

### Comparing `f3dasm-1.4.6/src/f3dasm/_src/run_optimization.py` & `f3dasm-1.4.7/src/f3dasm/_src/run_optimization.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/datageneration/abaqus.py` & `f3dasm-1.4.7/src/f3dasm/datageneration/abaqus.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/datageneration/functions.py` & `f3dasm-1.4.7/src/f3dasm/datageneration/functions.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm/optimization.py` & `f3dasm-1.4.7/src/f3dasm/optimization.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.6/src/f3dasm.egg-info/PKG-INFO` & `f3dasm-1.4.7/src/f3dasm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.4.6
+Version: 1.4.7
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://f3dasm.readthedocs.io/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
```

### Comparing `f3dasm-1.4.6/src/f3dasm.egg-info/SOURCES.txt` & `f3dasm-1.4.7/src/f3dasm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 docs/requirements.txt
 src/f3dasm/__init__.py
 src/f3dasm/__version__.py
 src/f3dasm/design.py
+src/f3dasm/hydra.py
 src/f3dasm/optimization.py
 src/f3dasm.egg-info/PKG-INFO
 src/f3dasm.egg-info/SOURCES.txt
 src/f3dasm.egg-info/dependency_links.txt
 src/f3dasm.egg-info/requires.txt
 src/f3dasm.egg-info/top_level.txt
 src/f3dasm/_src/__init__.py
 src/f3dasm/_src/_argparser.py
+src/f3dasm/_src/hydra_utils.py
 src/f3dasm/_src/logger.py
 src/f3dasm/_src/run_optimization.py
 src/f3dasm/_src/datageneration/__init__.py
 src/f3dasm/_src/datageneration/datagenerator.py
 src/f3dasm/_src/datageneration/abaqus/__init__.py
 src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py
 src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py
```

### Comparing `f3dasm-1.4.6/tests/conftest.py` & `f3dasm-1.4.7/tests/conftest.py`

 * *Files identical despite different names*

